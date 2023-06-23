# Comparing `tmp/opuscleaner-0.2.2.tar.gz` & `tmp/opuscleaner-0.3.0.tar.gz`

## Comparing `opuscleaner-0.2.2.tar` & `opuscleaner-0.3.0.tar`

### file list

```diff
@@ -1,100 +1,100 @@
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/__init__.py
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/_util.py
--rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/categories.py
--rwxr-xr-x   0        0        0    21105 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/clean.py
--rwxr-xr-x   0        0        0     2015 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/col.py
--rw-r--r--   0        0        0     1490 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/config.py
--rw-r--r--   0        0        0     1345 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/datasets.py
--rw-r--r--   0        0        0     9090 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/download.py
--rw-r--r--   0        0        0     7947 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/filters.py
--rw-r--r--   0        0        0     6452 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/opusfilter_compat.py
--rwxr-xr-x   0        0        0     4581 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/sample.py
--rw-r--r--   0        0        0    16891 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/server.py
--rwxr-xr-x   0        0        0     8153 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/threshold.py
--rw-r--r--   0        0        0     3391 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/filters/alpha_ratio.json
--rwxr-xr-x   0        0        0     3981 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/filters/alpha_ratio.py
--rw-r--r--   0        0        0     1261 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/filters/bicleaner_hardrules.json
--rw-r--r--   0        0        0     3714 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/filters/bifixer.json
--rwxr-xr-x   0        0        0      454 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/filters/bifixer_dedupe.py
--rwxr-xr-x   0        0        0     2440 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/filters/clean_common.py
--rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/filters/deescape-special-chars.json
--rwxr-xr-x   0        0        0      631 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/filters/deescape-special-chars.perl
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/filters/deescape_tsv.json
--rwxr-xr-x   0        0        0      343 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/filters/deescape_tsv.py
--rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/filters/detokenizer.json
--rwxr-xr-x   0        0        0    12473 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/filters/detokenizer.perl
--rw-r--r--   0        0        0     8692 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/filters/fasttext_filter.json
--rwxr-xr-x   0        0        0     3173 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/filters/fasttext_filter.py
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/filters/fix_elitr_eca.json
--rwxr-xr-x   0        0        0     1473 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/filters/fix_elitr_eca.py
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/filters/fix_quotes.json
--rwxr-xr-x   0        0        0      322 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/filters/fix_quotes.py
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/filters/fix_un_chinese.json
--rwxr-xr-x   0        0        0      354 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/filters/fix_un_chinese.py
--rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/filters/fix_wiki.json
--rwxr-xr-x   0        0        0     3569 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/filters/fix_wiki.py
--rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/filters/langid.json
--rwxr-xr-x   0        0        0     3019 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/filters/langid.py
--rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/filters/laser_similarity.json
--rwxr-xr-x   0        0        0     4525 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/filters/laser_similarity.py
--rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/filters/max_length.json
--rwxr-xr-x   0        0        0     1545 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/filters/max_length.py
--rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/filters/max_word_length.json
--rwxr-xr-x   0        0        0      869 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/filters/max_word_length.py
--rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/filters/num_mismatch.json
--rwxr-xr-x   0        0        0     1248 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/filters/num_mismatch.py
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/filters/regexp.json
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/filters/remove_empty_lines.json
--rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/filters/remove_frequent_patterns.json
--rwxr-xr-x   0        0        0     2700 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/filters/remove_frequent_patterns.py
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/filters/remove_frequent_patterns.txt
--rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/filters/sed.json
--rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/filters/segment_chinese.json
--rwxr-xr-x   0        0        0      200 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/filters/segment_chinese.py
--rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/filters/segment_japanese.json
--rwxr-xr-x   0        0        0      588 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/filters/segment_japanese.py
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/filters/simplify_chinese.json
--rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/filters/split_sentences.json
--rwxr-xr-x   0        0        0     1059 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/filters/split_sentences.py
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/filters/src_trg_ratio.json
--rwxr-xr-x   0        0        0     2298 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/filters/src_trg_ratio.py
--rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/filters/strip_suffix.json
--rwxr-xr-x   0        0        0     2271 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/filters/strip_suffix.py
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/filters/traditionalise_chinese.json
--rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/filters/opusfilter/AlphabetRatioFilter.json
--rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/filters/opusfilter/AverageWordLengthFilter.json
--rw-r--r--   0        0        0     4296 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/filters/opusfilter/CharacterScoreFilter.json
--rw-r--r--   0        0        0     1127 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/filters/opusfilter/Detokenizer.json
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/filters/opusfilter/HtmlTagFilter.json
--rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/filters/opusfilter/LengthFilter.json
--rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/filters/opusfilter/LengthRatioFilter.json
--rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/filters/opusfilter/LongWordFilter.json
--rw-r--r--   0        0        0     1049 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/filters/opusfilter/RegExpFilter.json
--rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/filters/opusfilter/RegExpSub.json
--rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/filters/opusfilter/Tokenizer.json
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/filters/opusfilter/WhitespaceNormalizer.json
--rwxr-xr-x   0        0        0     1808 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/filters/opusfilter/opusfilter-ersatz.py
--rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/frontend/index.html
--rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/frontend/assets/AddDatasetView.4182f0f7.css
--rw-r--r--   0        0        0     6379 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/frontend/assets/AddDatasetView.ff526466.js
--rw-r--r--   0        0        0     8179 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/frontend/assets/EditFiltersView.a7795492.css
--rw-r--r--   0        0        0   121398 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/frontend/assets/EditFiltersView.bc0dd7c3.js
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/frontend/assets/EditFiltersYamlView.28a1a7c9.js
--rw-r--r--   0        0        0     2328 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/frontend/assets/ListDatasetsView.0c61d7cc.js
--rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/frontend/assets/ListDatasetsView.79aac80d.css
--rw-r--r--   0        0        0     6270 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/frontend/assets/TagsEditor.23cf196f.js
--rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/frontend/assets/TagsEditor.ccc03a15.css
--rw-r--r--   0        0        0    38943 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/frontend/assets/data-cuate.84693c76.svg
--rw-r--r--   0        0        0     5490 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/frontend/assets/datailor-logo.fbfa6008.svg
--rw-r--r--   0        0        0    22166 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/frontend/assets/eu.24cff2c1.png
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/frontend/assets/hacks.1ae1ba64.js
--rw-r--r--   0        0        0   101750 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/frontend/assets/horizon-europe.80625b0c.png
--rw-r--r--   0        0        0     2120 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/frontend/assets/index.47848488.css
--rw-r--r--   0        0        0   124624 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/frontend/assets/index.6cc31f0d.js
--rw-r--r--   0        0        0    17440 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/frontend/assets/vue-select.9ddbca8a.js
--rw-r--r--   0        0        0     7480 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/opuscleaner/frontend/assets/vue-select.b0fac2a1.css
--rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/.gitignore
--rw-r--r--   0        0        0     3701 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/README.md
--rw-r--r--   0        0        0     2149 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     5288 2020-02-02 00:00:00.000000 opuscleaner-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 opuscleaner-0.3.0/opuscleaner/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opuscleaner-0.3.0/opuscleaner/__init__.py
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 opuscleaner-0.3.0/opuscleaner/_util.py
+-rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 opuscleaner-0.3.0/opuscleaner/categories.py
+-rwxr-xr-x   0        0        0    21105 2020-02-02 00:00:00.000000 opuscleaner-0.3.0/opuscleaner/clean.py
+-rwxr-xr-x   0        0        0     2015 2020-02-02 00:00:00.000000 opuscleaner-0.3.0/opuscleaner/col.py
+-rw-r--r--   0        0        0     1490 2020-02-02 00:00:00.000000 opuscleaner-0.3.0/opuscleaner/config.py
+-rw-r--r--   0        0        0     1341 2020-02-02 00:00:00.000000 opuscleaner-0.3.0/opuscleaner/datasets.py
+-rw-r--r--   0        0        0     9267 2020-02-02 00:00:00.000000 opuscleaner-0.3.0/opuscleaner/download.py
+-rw-r--r--   0        0        0     7947 2020-02-02 00:00:00.000000 opuscleaner-0.3.0/opuscleaner/filters.py
+-rw-r--r--   0        0        0     6452 2020-02-02 00:00:00.000000 opuscleaner-0.3.0/opuscleaner/opusfilter_compat.py
+-rwxr-xr-x   0        0        0     4581 2020-02-02 00:00:00.000000 opuscleaner-0.3.0/opuscleaner/sample.py
+-rw-r--r--   0        0        0    17103 2020-02-02 00:00:00.000000 opuscleaner-0.3.0/opuscleaner/server.py
+-rwxr-xr-x   0        0        0     8153 2020-02-02 00:00:00.000000 opuscleaner-0.3.0/opuscleaner/threshold.py
+-rw-r--r--   0        0        0     3391 2020-02-02 00:00:00.000000 opuscleaner-0.3.0/opuscleaner/filters/alpha_ratio.json
+-rwxr-xr-x   0        0        0     3981 2020-02-02 00:00:00.000000 opuscleaner-0.3.0/opuscleaner/filters/alpha_ratio.py
+-rw-r--r--   0        0        0     1261 2020-02-02 00:00:00.000000 opuscleaner-0.3.0/opuscleaner/filters/bicleaner_hardrules.json
+-rw-r--r--   0        0        0     3714 2020-02-02 00:00:00.000000 opuscleaner-0.3.0/opuscleaner/filters/bifixer.json
+-rwxr-xr-x   0        0        0      454 2020-02-02 00:00:00.000000 opuscleaner-0.3.0/opuscleaner/filters/bifixer_dedupe.py
+-rwxr-xr-x   0        0        0     2440 2020-02-02 00:00:00.000000 opuscleaner-0.3.0/opuscleaner/filters/clean_common.py
+-rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 opuscleaner-0.3.0/opuscleaner/filters/deescape-special-chars.json
+-rwxr-xr-x   0        0        0      631 2020-02-02 00:00:00.000000 opuscleaner-0.3.0/opuscleaner/filters/deescape-special-chars.perl
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 opuscleaner-0.3.0/opuscleaner/filters/deescape_tsv.json
+-rwxr-xr-x   0        0        0      343 2020-02-02 00:00:00.000000 opuscleaner-0.3.0/opuscleaner/filters/deescape_tsv.py
+-rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 opuscleaner-0.3.0/opuscleaner/filters/detokenizer.json
+-rwxr-xr-x   0        0        0    12473 2020-02-02 00:00:00.000000 opuscleaner-0.3.0/opuscleaner/filters/detokenizer.perl
+-rw-r--r--   0        0        0     8692 2020-02-02 00:00:00.000000 opuscleaner-0.3.0/opuscleaner/filters/fasttext_filter.json
+-rwxr-xr-x   0        0        0     3173 2020-02-02 00:00:00.000000 opuscleaner-0.3.0/opuscleaner/filters/fasttext_filter.py
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 opuscleaner-0.3.0/opuscleaner/filters/fix_elitr_eca.json
+-rwxr-xr-x   0        0        0     1473 2020-02-02 00:00:00.000000 opuscleaner-0.3.0/opuscleaner/filters/fix_elitr_eca.py
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 opuscleaner-0.3.0/opuscleaner/filters/fix_quotes.json
+-rwxr-xr-x   0        0        0      322 2020-02-02 00:00:00.000000 opuscleaner-0.3.0/opuscleaner/filters/fix_quotes.py
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 opuscleaner-0.3.0/opuscleaner/filters/fix_un_chinese.json
+-rwxr-xr-x   0        0        0      354 2020-02-02 00:00:00.000000 opuscleaner-0.3.0/opuscleaner/filters/fix_un_chinese.py
+-rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 opuscleaner-0.3.0/opuscleaner/filters/fix_wiki.json
+-rwxr-xr-x   0        0        0     3569 2020-02-02 00:00:00.000000 opuscleaner-0.3.0/opuscleaner/filters/fix_wiki.py
+-rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 opuscleaner-0.3.0/opuscleaner/filters/langid.json
+-rwxr-xr-x   0        0        0     3019 2020-02-02 00:00:00.000000 opuscleaner-0.3.0/opuscleaner/filters/langid.py
+-rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 opuscleaner-0.3.0/opuscleaner/filters/laser_similarity.json
+-rwxr-xr-x   0        0        0     4525 2020-02-02 00:00:00.000000 opuscleaner-0.3.0/opuscleaner/filters/laser_similarity.py
+-rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 opuscleaner-0.3.0/opuscleaner/filters/max_length.json
+-rwxr-xr-x   0        0        0     1545 2020-02-02 00:00:00.000000 opuscleaner-0.3.0/opuscleaner/filters/max_length.py
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 opuscleaner-0.3.0/opuscleaner/filters/max_word_length.json
+-rwxr-xr-x   0        0        0      869 2020-02-02 00:00:00.000000 opuscleaner-0.3.0/opuscleaner/filters/max_word_length.py
+-rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 opuscleaner-0.3.0/opuscleaner/filters/num_mismatch.json
+-rwxr-xr-x   0        0        0     1248 2020-02-02 00:00:00.000000 opuscleaner-0.3.0/opuscleaner/filters/num_mismatch.py
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 opuscleaner-0.3.0/opuscleaner/filters/regexp.json
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 opuscleaner-0.3.0/opuscleaner/filters/remove_empty_lines.json
+-rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 opuscleaner-0.3.0/opuscleaner/filters/remove_frequent_patterns.json
+-rwxr-xr-x   0        0        0     2700 2020-02-02 00:00:00.000000 opuscleaner-0.3.0/opuscleaner/filters/remove_frequent_patterns.py
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 opuscleaner-0.3.0/opuscleaner/filters/remove_frequent_patterns.txt
+-rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 opuscleaner-0.3.0/opuscleaner/filters/sed.json
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 opuscleaner-0.3.0/opuscleaner/filters/segment_chinese.json
+-rwxr-xr-x   0        0        0      200 2020-02-02 00:00:00.000000 opuscleaner-0.3.0/opuscleaner/filters/segment_chinese.py
+-rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 opuscleaner-0.3.0/opuscleaner/filters/segment_japanese.json
+-rwxr-xr-x   0        0        0      588 2020-02-02 00:00:00.000000 opuscleaner-0.3.0/opuscleaner/filters/segment_japanese.py
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 opuscleaner-0.3.0/opuscleaner/filters/simplify_chinese.json
+-rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 opuscleaner-0.3.0/opuscleaner/filters/split_sentences.json
+-rwxr-xr-x   0        0        0     1059 2020-02-02 00:00:00.000000 opuscleaner-0.3.0/opuscleaner/filters/split_sentences.py
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 opuscleaner-0.3.0/opuscleaner/filters/src_trg_ratio.json
+-rwxr-xr-x   0        0        0     2298 2020-02-02 00:00:00.000000 opuscleaner-0.3.0/opuscleaner/filters/src_trg_ratio.py
+-rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 opuscleaner-0.3.0/opuscleaner/filters/strip_suffix.json
+-rwxr-xr-x   0        0        0     2271 2020-02-02 00:00:00.000000 opuscleaner-0.3.0/opuscleaner/filters/strip_suffix.py
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 opuscleaner-0.3.0/opuscleaner/filters/traditionalise_chinese.json
+-rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 opuscleaner-0.3.0/opuscleaner/filters/opusfilter/AlphabetRatioFilter.json
+-rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 opuscleaner-0.3.0/opuscleaner/filters/opusfilter/AverageWordLengthFilter.json
+-rw-r--r--   0        0        0     4296 2020-02-02 00:00:00.000000 opuscleaner-0.3.0/opuscleaner/filters/opusfilter/CharacterScoreFilter.json
+-rw-r--r--   0        0        0     1127 2020-02-02 00:00:00.000000 opuscleaner-0.3.0/opuscleaner/filters/opusfilter/Detokenizer.json
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 opuscleaner-0.3.0/opuscleaner/filters/opusfilter/HtmlTagFilter.json
+-rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 opuscleaner-0.3.0/opuscleaner/filters/opusfilter/LengthFilter.json
+-rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 opuscleaner-0.3.0/opuscleaner/filters/opusfilter/LengthRatioFilter.json
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 opuscleaner-0.3.0/opuscleaner/filters/opusfilter/LongWordFilter.json
+-rw-r--r--   0        0        0     1049 2020-02-02 00:00:00.000000 opuscleaner-0.3.0/opuscleaner/filters/opusfilter/RegExpFilter.json
+-rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 opuscleaner-0.3.0/opuscleaner/filters/opusfilter/RegExpSub.json
+-rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 opuscleaner-0.3.0/opuscleaner/filters/opusfilter/Tokenizer.json
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 opuscleaner-0.3.0/opuscleaner/filters/opusfilter/WhitespaceNormalizer.json
+-rwxr-xr-x   0        0        0     1808 2020-02-02 00:00:00.000000 opuscleaner-0.3.0/opuscleaner/filters/opusfilter/opusfilter-ersatz.py
+-rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 opuscleaner-0.3.0/opuscleaner/frontend/index.html
+-rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 opuscleaner-0.3.0/opuscleaner/frontend/assets/AddDatasetView.1967bdb7.css
+-rw-r--r--   0        0        0     7006 2020-02-02 00:00:00.000000 opuscleaner-0.3.0/opuscleaner/frontend/assets/AddDatasetView.8b79ed74.js
+-rw-r--r--   0        0        0   121428 2020-02-02 00:00:00.000000 opuscleaner-0.3.0/opuscleaner/frontend/assets/EditFiltersView.877cfb0b.js
+-rw-r--r--   0        0        0     8179 2020-02-02 00:00:00.000000 opuscleaner-0.3.0/opuscleaner/frontend/assets/EditFiltersView.fa7331b7.css
+-rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 opuscleaner-0.3.0/opuscleaner/frontend/assets/EditFiltersYamlView.5763c641.js
+-rw-r--r--   0        0        0     2321 2020-02-02 00:00:00.000000 opuscleaner-0.3.0/opuscleaner/frontend/assets/ListDatasetsView.576d1862.js
+-rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 opuscleaner-0.3.0/opuscleaner/frontend/assets/ListDatasetsView.b8eb7e79.css
+-rw-r--r--   0        0        0     6270 2020-02-02 00:00:00.000000 opuscleaner-0.3.0/opuscleaner/frontend/assets/TagsEditor.3f956450.js
+-rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 opuscleaner-0.3.0/opuscleaner/frontend/assets/TagsEditor.ccc03a15.css
+-rw-r--r--   0        0        0    38943 2020-02-02 00:00:00.000000 opuscleaner-0.3.0/opuscleaner/frontend/assets/data-cuate.84693c76.svg
+-rw-r--r--   0        0        0     5490 2020-02-02 00:00:00.000000 opuscleaner-0.3.0/opuscleaner/frontend/assets/datailor-logo.fbfa6008.svg
+-rw-r--r--   0        0        0    22166 2020-02-02 00:00:00.000000 opuscleaner-0.3.0/opuscleaner/frontend/assets/eu.24cff2c1.png
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 opuscleaner-0.3.0/opuscleaner/frontend/assets/hacks.175c31f5.js
+-rw-r--r--   0        0        0   101750 2020-02-02 00:00:00.000000 opuscleaner-0.3.0/opuscleaner/frontend/assets/horizon-europe.80625b0c.png
+-rw-r--r--   0        0        0     2120 2020-02-02 00:00:00.000000 opuscleaner-0.3.0/opuscleaner/frontend/assets/index.47848488.css
+-rw-r--r--   0        0        0   124624 2020-02-02 00:00:00.000000 opuscleaner-0.3.0/opuscleaner/frontend/assets/index.aa84b8f1.js
+-rw-r--r--   0        0        0    17440 2020-02-02 00:00:00.000000 opuscleaner-0.3.0/opuscleaner/frontend/assets/vue-select.973ce47f.js
+-rw-r--r--   0        0        0     7480 2020-02-02 00:00:00.000000 opuscleaner-0.3.0/opuscleaner/frontend/assets/vue-select.b0fac2a1.css
+-rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 opuscleaner-0.3.0/.gitignore
+-rw-r--r--   0        0        0     4129 2020-02-02 00:00:00.000000 opuscleaner-0.3.0/README.md
+-rw-r--r--   0        0        0     2149 2020-02-02 00:00:00.000000 opuscleaner-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     5716 2020-02-02 00:00:00.000000 opuscleaner-0.3.0/PKG-INFO
```

### Comparing `opuscleaner-0.2.2/opuscleaner/categories.py` & `opuscleaner-0.3.0/opuscleaner/categories.py`

 * *Files identical despite different names*

### Comparing `opuscleaner-0.2.2/opuscleaner/clean.py` & `opuscleaner-0.3.0/opuscleaner/clean.py`

 * *Files identical despite different names*

### Comparing `opuscleaner-0.2.2/opuscleaner/col.py` & `opuscleaner-0.3.0/opuscleaner/col.py`

 * *Files identical despite different names*

### Comparing `opuscleaner-0.2.2/opuscleaner/config.py` & `opuscleaner-0.3.0/opuscleaner/config.py`

 * *Files identical despite different names*

### Comparing `opuscleaner-0.2.2/opuscleaner/datasets.py` & `opuscleaner-0.3.0/opuscleaner/datasets.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 #!/usr/bin/env python3
 """Lists datasets given a directory. It works by scanning the directory and looking for gz files."""
 import os
 from functools import wraps
 from glob import glob
 from itertools import groupby
 from pathlib import Path as Path
-from typing import Iterable, Dict
+from typing import Iterable, Dict, List, Tuple
 
 
-def list_datasets(path:str) -> Dict[str,Dict[str,Path]]:
+def list_datasets(path:str) -> Dict[str,List[Tuple[str,Path]]]:
     """Lists datasets given a directory. Scans the directories and returns a dictionary of the
     datasets encoutered. Dictionary looks like {dataset_name : { lang: path}}"""
     root = Path(path.split('*')[0])
 
     entries = (Path(entry) for entry in glob(path, recursive=True))
 
     files = [
@@ -27,20 +27,19 @@
         (name, list(files))
         for name, files in groupby(
             sorted(files, key=lambda entry: str(entry)),
             key=lambda entry: str(entry.relative_to(root)).rsplit('.', 2)[0])
     ]
 
     return {
-        name: {
-            entry.name.rsplit('.', 2)[1]: entry
+        name: [
+            (entry.name.rsplit('.', 2)[1], entry)
             for entry in files
-        }
+        ]
         for name, files in datasets
-        if len(files) > 1
     }
 
 
 def main() -> None:
     import sys
     import pprint
     pprint.pprint(list_datasets(sys.argv[1]))
```

### Comparing `opuscleaner-0.2.2/opuscleaner/download.py` & `opuscleaner-0.3.0/opuscleaner/download.py`

 * *Files 2% similar despite different names*

```diff
@@ -130,15 +130,15 @@
             return DownloadState.DOWNLOADED
         elif self._child.exitcode > 0:
             return DownloadState.FAILED
         else:
             return DownloadState.CANCELLED
 
 
-DownloadQueue = SimpleQueue[Optional[EntryDownload]]
+DownloadQueue = SimpleQueue#[Optional[EntryDownload]]
 
 
 class Downloader:
     def __init__(self, workers:int):
         self.queue: DownloadQueue = SimpleQueue()
         self.threads: List[Thread] = []
 
@@ -183,21 +183,27 @@
 
         with urlopen(f'{self.endpoint}?{urlencode(query)}') as fh:
             return [str(lang) for lang in json.load(fh).get('languages', [])]
 
     def get_dataset(self, id:int) -> Entry:
         return self._datasets[id]
 
-    def find_datasets(self, lang1:str, lang2:str) -> List[Entry]:
-        query = {
-            'source': lang1,
-            'target': lang2,
-            'preprocessing': 'moses'
-        }
-        
+    def find_datasets(self, lang1:str, lang2:Optional[str]=None) -> List[Entry]:
+        if lang2 is None:
+            query = {
+                'source': lang1,
+                'preprocessing': 'mono'
+            }
+        else:
+            query = {
+                'source': lang1,
+                'target': lang2,
+                'preprocessing': 'moses'
+            }
+
         with urlopen(f'{self.endpoint}?{urlencode(query)}') as fh:
             datasets = [cast_entry(entry) for entry in json.load(fh).get('corpora', [])]
 
         # FIXME dirty hack to keep a local copy to be able to do id based lookup
         # Related: https://github.com/Helsinki-NLP/OPUS-API/issues/3
         for dataset in datasets:
             self._datasets[dataset.id] = dataset
```

### Comparing `opuscleaner-0.2.2/opuscleaner/filters.py` & `opuscleaner-0.3.0/opuscleaner/filters.py`

 * *Files identical despite different names*

### Comparing `opuscleaner-0.2.2/opuscleaner/opusfilter_compat.py` & `opuscleaner-0.3.0/opuscleaner/opusfilter_compat.py`

 * *Files identical despite different names*

### Comparing `opuscleaner-0.2.2/opuscleaner/sample.py` & `opuscleaner-0.3.0/opuscleaner/sample.py`

 * *Files identical despite different names*

### Comparing `opuscleaner-0.2.2/opuscleaner/server.py` & `opuscleaner-0.3.0/opuscleaner/server.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,27 +4,28 @@
 import hashlib
 import json
 import os
 import re
 import subprocess
 import sys
 import traceback
-from contextlib import ExitStack
+from contextlib import ExitStack, asynccontextmanager
 from enum import Enum
 from glob import glob
 from itertools import chain, zip_longest
 from pprint import pprint
 from shutil import copyfileobj
 from tempfile import TemporaryFile
 from typing import NamedTuple, Optional, Iterable, TypeVar, Union, Literal, Any, AsyncIterator, Awaitable, cast, IO, List, Dict, Tuple, AsyncIterator
 from warnings import warn
 
 import yaml
 from fastapi import FastAPI, HTTPException
 from fastapi.encoders import jsonable_encoder
+from fastapi.middleware.gzip import GZipMiddleware
 from fastapi.responses import RedirectResponse, StreamingResponse
 from fastapi.staticfiles import StaticFiles
 from pydantic import BaseModel, parse_obj_as, validator, ValidationError
 from starlette.datastructures import URL
 from starlette.responses import FileResponse, RedirectResponse, Response
 from starlette.types import Scope
 
@@ -46,22 +47,23 @@
         os.path.join(os.path.dirname(__file__), 'frontend'),
         os.path.join(os.path.dirname(__file__), '../frontend/dist'),
     ]
     if os.path.exists(path)
 ))
 
 
-class File(BaseModel):
+class Column(BaseModel):
+    lang: str
     path: str
     size: int
 
 
 class Dataset(BaseModel):
     name: str
-    columns: Dict[str,File]
+    columns: List[Column]
 
 
 class FilterPipelinePatch(BaseModel):
     """A list of changes to a filter pipeline (used when updating filters)"""
     filters: List[FilterStep]
 
 
@@ -143,15 +145,15 @@
             returncode=output.returncode,
             stdout=lines,
             stderr=output.stderr.decode())
 
 
 class SampleCacheEntry(NamedTuple):
     checksum: bytes
-    future: asyncio.Task[FilterOutput]
+    future: asyncio.Task#[FilterOutput]
 
 
 sample_cache: Dict[str,List[SampleCacheEntry]] = {}
 
 
 def cache_hash(obj: Any, seed: bytes = bytes()) -> bytes:
     impl = hashlib.sha256(seed)
@@ -214,15 +216,15 @@
 def cancel_cached_tasks(name:str, offset:int) -> None:
     for entry in sample_cache[name][offset:]:
         entry.future.cancel()
     del sample_cache[name][offset:]
 
 
 async def get_sample(name:str, filters:List[FilterStep]) -> AsyncIterator[FilterOutput]:
-    columns: List[Tuple[str,Path]] = sorted(list_datasets(DATA_PATH)[name].items(), key=lambda pair: pair[0])
+    columns: List[Tuple[str,Path]] = list_datasets(DATA_PATH)[name]
     langs = [lang for lang, _ in columns]
 
     checksum = cache_hash([
         (name, str(path), path.stat().st_mtime)
         for name, path in columns
     ])
 
@@ -276,38 +278,51 @@
         (
             json.dumps(jsonable_encoder(line), separators=(',', ':')).encode() + b"\n"
             async for line in iterable
         ),
         media_type='application/json')
 
 
-app = FastAPI()
+@asynccontextmanager
+async def lifespan(app: FastAPI):
+    """
+    Place to do the start-up and shut-down operations of the web service.
+    See https://fastapi.tiangolo.com/advanced/events/#lifespan-events
+    """
+    set_global_filters(list_filters(FILTER_PATH))
+    yield
+    set_global_filters([])
+
+
+app = FastAPI(lifespan=lifespan)
+
+app.add_middleware(GZipMiddleware, minimum_size=512)
 
 @app.get('/api/datasets/')
 def api_list_datasets() -> List[Dataset]:
     return [
-        Dataset(name=name, columns={
-            lang: File(path=file.name, size=file.stat().st_size)
-            for lang, file in columns.items()
-        })
+        Dataset(name=name, columns=[
+            Column(lang=lang, path=file.name, size=file.stat().st_size)
+            for lang, file in columns
+        ])
         for name, columns in list_datasets(DATA_PATH).items()
     ]
 
 
 @app.get('/api/datasets/{name:path}/')
 def api_get_dataset(name:str) -> Dataset:
     columns = list_datasets(DATA_PATH).get(name)
 
     if not columns:
         raise HTTPException(status_code=404, detail='Dataset not found')
 
-    return Dataset(name=name, columns={
-        lang: File(path=file.name, size=file.stat().st_size)
-        for lang, file in columns.items()
-    })
+    return Dataset(name=name, columns=[
+        Column(lang=lang, path=file.name, size=file.stat().st_size)
+        for lang, file in columns
+    ])
 
 
 @app.get('/api/datasets/{name:path}/sample')
 async def api_get_sample(name:str) -> Response:
     return stream_jsonl(ParsedFilterOutput(output) async for output in get_sample(name, []))
 
 
@@ -316,18 +331,15 @@
     return stream_jsonl(ParsedFilterOutput(output) async for output in get_sample(name, filters))
 
 
 def make_pipeline(name:str, filters:List[FilterStep] = []) -> FilterPipeline:
     columns = list_datasets(DATA_PATH)[name]
     return FilterPipeline(
         version=1,
-        files=[file.name
-            for _, file in
-            sorted(columns.items(), key=lambda pair: pair[0])
-        ],
+        files=[file.name for _, file in columns],
         filters=filters
     )
 
 
 @app.get('/api/datasets/{name:path}/configuration.json')
 def api_get_dataset_filters(name:str) -> FilterPipeline:
 
@@ -462,19 +474,18 @@
     uvicorn.run(f'opuscleaner.server:app', port=args.port, reload=args.reload, log_level='info')
 
 
 async def sample_all_datasets(args):
     tasks = []
 
     for name, columns in list_datasets(DATA_PATH).items():
-        sorted_cols = sorted(columns.items(), key=lambda pair: pair[0])
-        langs = [lang for lang, _ in sorted_cols]
+        langs = [lang for lang, _ in columns]
         if not os.path.exists(sample_path(name, langs)):
             print(f"Sampling {name}...", file=sys.stderr)
-            tasks.append([name, sorted_cols])
+            tasks.append([name, columns])
 
     for task, result in zip(tasks, await asyncio.gather(*[compute_sample(*task) for task in tasks], return_exceptions=True)):
         if isinstance(result, Exception):
             print(f"Could not compute sample for {task[0]}: {result!s}", file=sys.stderr)
 
 
 def main_sample(args):
@@ -502,13 +513,11 @@
     parser_serve.add_argument('--reload', action='store_true', help='Enable auto-reload.')
     parser_serve.set_defaults(func=main_serve)
 
     parser_sample = subparsers.add_parser('sample')
     parser_sample.set_defaults(func=main_sample)
 
     args = parser.parse_args()
-
-    set_global_filters(list_filters(FILTER_PATH))
     args.func(args)
 
 if __name__ == '__main__':
     main()
```

### Comparing `opuscleaner-0.2.2/opuscleaner/threshold.py` & `opuscleaner-0.3.0/opuscleaner/threshold.py`

 * *Files identical despite different names*

### Comparing `opuscleaner-0.2.2/opuscleaner/filters/alpha_ratio.json` & `opuscleaner-0.3.0/opuscleaner/filters/alpha_ratio.json`

 * *Files identical despite different names*

### Comparing `opuscleaner-0.2.2/opuscleaner/filters/alpha_ratio.py` & `opuscleaner-0.3.0/opuscleaner/filters/alpha_ratio.py`

 * *Files identical despite different names*

### Comparing `opuscleaner-0.2.2/opuscleaner/filters/bicleaner_hardrules.json` & `opuscleaner-0.3.0/opuscleaner/filters/bicleaner_hardrules.json`

 * *Files identical despite different names*

### Comparing `opuscleaner-0.2.2/opuscleaner/filters/bifixer.json` & `opuscleaner-0.3.0/opuscleaner/filters/bifixer.json`

 * *Files identical despite different names*

### Comparing `opuscleaner-0.2.2/opuscleaner/filters/clean_common.py` & `opuscleaner-0.3.0/opuscleaner/filters/clean_common.py`

 * *Files identical despite different names*

### Comparing `opuscleaner-0.2.2/opuscleaner/filters/deescape-special-chars.perl` & `opuscleaner-0.3.0/opuscleaner/filters/deescape-special-chars.perl`

 * *Files identical despite different names*

### Comparing `opuscleaner-0.2.2/opuscleaner/filters/detokenizer.json` & `opuscleaner-0.3.0/opuscleaner/filters/detokenizer.json`

 * *Files identical despite different names*

### Comparing `opuscleaner-0.2.2/opuscleaner/filters/detokenizer.perl` & `opuscleaner-0.3.0/opuscleaner/filters/detokenizer.perl`

 * *Files identical despite different names*

### Comparing `opuscleaner-0.2.2/opuscleaner/filters/fasttext_filter.json` & `opuscleaner-0.3.0/opuscleaner/filters/fasttext_filter.json`

 * *Files identical despite different names*

### Comparing `opuscleaner-0.2.2/opuscleaner/filters/fasttext_filter.py` & `opuscleaner-0.3.0/opuscleaner/filters/fasttext_filter.py`

 * *Files identical despite different names*

### Comparing `opuscleaner-0.2.2/opuscleaner/filters/fix_elitr_eca.py` & `opuscleaner-0.3.0/opuscleaner/filters/fix_elitr_eca.py`

 * *Files identical despite different names*

### Comparing `opuscleaner-0.2.2/opuscleaner/filters/fix_wiki.json` & `opuscleaner-0.3.0/opuscleaner/filters/fix_wiki.json`

 * *Files identical despite different names*

### Comparing `opuscleaner-0.2.2/opuscleaner/filters/fix_wiki.py` & `opuscleaner-0.3.0/opuscleaner/filters/fix_wiki.py`

 * *Files identical despite different names*

### Comparing `opuscleaner-0.2.2/opuscleaner/filters/langid.json` & `opuscleaner-0.3.0/opuscleaner/filters/langid.json`

 * *Files identical despite different names*

### Comparing `opuscleaner-0.2.2/opuscleaner/filters/langid.py` & `opuscleaner-0.3.0/opuscleaner/filters/langid.py`

 * *Files identical despite different names*

### Comparing `opuscleaner-0.2.2/opuscleaner/filters/laser_similarity.json` & `opuscleaner-0.3.0/opuscleaner/filters/laser_similarity.json`

 * *Files identical despite different names*

### Comparing `opuscleaner-0.2.2/opuscleaner/filters/laser_similarity.py` & `opuscleaner-0.3.0/opuscleaner/filters/laser_similarity.py`

 * *Files identical despite different names*

### Comparing `opuscleaner-0.2.2/opuscleaner/filters/max_length.py` & `opuscleaner-0.3.0/opuscleaner/filters/max_length.py`

 * *Files identical despite different names*

### Comparing `opuscleaner-0.2.2/opuscleaner/filters/max_word_length.py` & `opuscleaner-0.3.0/opuscleaner/filters/max_word_length.py`

 * *Files identical despite different names*

### Comparing `opuscleaner-0.2.2/opuscleaner/filters/num_mismatch.py` & `opuscleaner-0.3.0/opuscleaner/filters/num_mismatch.py`

 * *Files identical despite different names*

### Comparing `opuscleaner-0.2.2/opuscleaner/filters/remove_frequent_patterns.py` & `opuscleaner-0.3.0/opuscleaner/filters/remove_frequent_patterns.py`

 * *Files identical despite different names*

### Comparing `opuscleaner-0.2.2/opuscleaner/filters/segment_japanese.py` & `opuscleaner-0.3.0/opuscleaner/filters/segment_japanese.py`

 * *Files identical despite different names*

### Comparing `opuscleaner-0.2.2/opuscleaner/filters/split_sentences.json` & `opuscleaner-0.3.0/opuscleaner/filters/split_sentences.json`

 * *Files identical despite different names*

### Comparing `opuscleaner-0.2.2/opuscleaner/filters/split_sentences.py` & `opuscleaner-0.3.0/opuscleaner/filters/split_sentences.py`

 * *Files identical despite different names*

### Comparing `opuscleaner-0.2.2/opuscleaner/filters/src_trg_ratio.py` & `opuscleaner-0.3.0/opuscleaner/filters/src_trg_ratio.py`

 * *Files identical despite different names*

### Comparing `opuscleaner-0.2.2/opuscleaner/filters/strip_suffix.json` & `opuscleaner-0.3.0/opuscleaner/filters/strip_suffix.json`

 * *Files identical despite different names*

### Comparing `opuscleaner-0.2.2/opuscleaner/filters/strip_suffix.py` & `opuscleaner-0.3.0/opuscleaner/filters/strip_suffix.py`

 * *Files identical despite different names*

### Comparing `opuscleaner-0.2.2/opuscleaner/filters/opusfilter/AverageWordLengthFilter.json` & `opuscleaner-0.3.0/opuscleaner/filters/opusfilter/AverageWordLengthFilter.json`

 * *Files identical despite different names*

### Comparing `opuscleaner-0.2.2/opuscleaner/filters/opusfilter/CharacterScoreFilter.json` & `opuscleaner-0.3.0/opuscleaner/filters/opusfilter/CharacterScoreFilter.json`

 * *Files identical despite different names*

### Comparing `opuscleaner-0.2.2/opuscleaner/filters/opusfilter/Detokenizer.json` & `opuscleaner-0.3.0/opuscleaner/filters/opusfilter/Detokenizer.json`

 * *Files identical despite different names*

### Comparing `opuscleaner-0.2.2/opuscleaner/filters/opusfilter/LengthFilter.json` & `opuscleaner-0.3.0/opuscleaner/filters/opusfilter/LengthFilter.json`

 * *Files identical despite different names*

### Comparing `opuscleaner-0.2.2/opuscleaner/filters/opusfilter/RegExpFilter.json` & `opuscleaner-0.3.0/opuscleaner/filters/opusfilter/RegExpFilter.json`

 * *Files identical despite different names*

### Comparing `opuscleaner-0.2.2/opuscleaner/filters/opusfilter/RegExpSub.json` & `opuscleaner-0.3.0/opuscleaner/filters/opusfilter/RegExpSub.json`

 * *Files identical despite different names*

### Comparing `opuscleaner-0.2.2/opuscleaner/filters/opusfilter/Tokenizer.json` & `opuscleaner-0.3.0/opuscleaner/filters/opusfilter/Tokenizer.json`

 * *Files identical despite different names*

### Comparing `opuscleaner-0.2.2/opuscleaner/filters/opusfilter/opusfilter-ersatz.py` & `opuscleaner-0.3.0/opuscleaner/filters/opusfilter/opusfilter-ersatz.py`

 * *Files identical despite different names*

### Comparing `opuscleaner-0.2.2/opuscleaner/frontend/assets/AddDatasetView.ff526466.js` & `opuscleaner-0.3.0/opuscleaner/frontend/assets/AddDatasetView.8b79ed74.js`

 * *Files 16% similar despite different names*

#### js-beautify {}

```diff
@@ -1,339 +1,387 @@
-var x = (n, o, l) => {
-    if (!o.has(n)) throw TypeError("Cannot " + l)
+var B = (t, n, o) => {
+    if (!n.has(t)) throw TypeError("Cannot " + o)
 };
-var b = (n, o, l) => (x(n, o, "read from private field"), l ? l.call(n) : o.get(n)),
-    B = (n, o, l) => {
-        if (o.has(n)) throw TypeError("Cannot add the same private member more than once");
-        o instanceof WeakSet ? o.add(n) : o.set(n, l)
+var w = (t, n, o) => (B(t, n, "read from private field"), o ? o.call(t) : n.get(t)),
+    A = (t, n, o) => {
+        if (n.has(t)) throw TypeError("Cannot add the same private member more than once");
+        n instanceof WeakSet ? n.add(t) : n.set(t, o)
     },
-    U = (n, o, l, _) => (x(n, o, "write to private field"), _ ? _.call(n, l) : o.set(n, l), l);
-var A = (n, o, l) => (x(n, o, "access private method"), l);
+    T = (t, n, o, c) => (B(t, n, "write to private field"), c ? c.call(t, o) : n.set(t, o), o);
+var j = (t, n, o) => (B(t, n, "access private method"), o);
 import {
-    _ as ae,
-    i as r,
-    m as S,
-    j as se,
-    aL as ne,
-    k as oe,
+    i as u,
+    j as Y,
+    k as Z,
     o as g,
-    c as y,
+    c as _,
     d as s,
-    n as L,
-    bw as le,
-    a4 as j,
-    v as N,
-    f as h,
-    b as T,
-    u as c,
-    F as P,
-    r as J,
-    a as re,
-    T as ie,
-    t as p,
-    bF as ue,
-    p as ce,
-    h as de
-} from "./index.6cc31f0d.js";
+    F,
+    r as P,
+    f as m,
+    t as v,
+    u as r,
+    _ as ee,
+    m as U,
+    aL as te,
+    n as b,
+    bw as ae,
+    a4 as $,
+    bu as R,
+    v as ne,
+    b as y,
+    bx as se,
+    a as oe,
+    T as le,
+    bF as re,
+    p as ie,
+    h as ue
+} from "./index.aa84b8f1.js";
 import {
-    C as z
-} from "./vue-select.9ddbca8a.js";
+    C
+} from "./vue-select.973ce47f.js";
 
-function pe(n) {
-    const o = n == 0 ? 0 : Math.floor(Math.log(n) / Math.log(1024));
-    return (n / Math.pow(1024, o)).toFixed(2) + " " + ["B", "kB", "MB", "GB", "TB"][o]
-}
-var d, C, q;
-class he {
-    constructor(o, l) {
-        B(this, C);
-        B(this, d, void 0);
-        this.interval = o, this.callback = l
+function ce(t) {
+    const n = t == 0 ? 0 : Math.floor(Math.log(t) / Math.log(1024));
+    return (t / Math.pow(1024, n)).toFixed(2) + " " + ["B", "kB", "MB", "GB", "TB"][n]
+}
+const z = u(0);
+async function L(t, n) {
+    try {
+        return z.value += 1, await (await fetch(t, n)).json()
+    } finally {
+        z.value -= 1
+    }
+}
+var h, k, J;
+class de {
+    constructor(n, o) {
+        A(this, k);
+        A(this, h, void 0);
+        this.interval = n, this.callback = o
     }
     start() {
-        b(this, d) && clearTimeout(b(this, d)), U(this, d, setTimeout(A(this, C, q).bind(this), this.interval))
+        w(this, h) && clearTimeout(w(this, h)), T(this, h, setTimeout(j(this, k, J).bind(this), this.interval))
     }
     stop() {
-        clearTimeout(b(this, d)), U(this, d, null)
+        clearTimeout(w(this, h)), T(this, h, null)
     }
     restart() {
         this.stop(), this.start()
     }
 }
-d = new WeakMap, C = new WeakSet, q = function() {
+h = new WeakMap, k = new WeakSet, J = function() {
     Promise.resolve(this.callback()).then(() => {
-        b(this, d) && this.start()
+        w(this, h) && this.start()
     })
 };
-const m = n => (ce("data-v-183e5481"), n = n(), de(), n),
-    ve = {
+const f = Y({});
+
+function pe() {
+    return f
+}
+async function he(t) {
+    return await L("/api/download/downloads/", {
+        method: "POST",
+        headers: {
+            "Content-Type": "application/json"
+        },
+        body: JSON.stringify(t.map(({
+            id: n
+        }) => ({
+            id: n
+        })))
+    })
+}
+async function q() {
+    return await L("/api/download/downloads/")
+}
+
+function ve(t) {
+    he([t]).then(n => {
+        Object.assign(f, G(n))
+    })
+}
+
+function ge(t) {
+    return t.id in f
+}
+async function me() {
+    return await L("/api/download/languages/")
+}
+async function _e(t) {
+    return await L(`/api/download/languages/${encodeURIComponent(t)}`)
+}
+async function fe(t) {
+    return await L(`/api/download/by-language/${encodeURIComponent(t)}`)
+}
+let E = new de(1e3, async () => {
+    const t = await q();
+    Object.assign(f, G(t))
+});
+Z(f, t => {
+    const n = new Set(["pending", "downloading"]);
+    Object.values(t).some(o => n.has(o.state)) ? E.restart() : E.stop()
+});
+
+function G(t) {
+    return Object.fromEntries(t.map(n => [n.entry.id, n]))
+}
+q().then(t => {
+    Object.assign(f, G(t))
+});
+const we = {
+        class: "downloads-popup"
+    },
+    be = s("summary", null, [s("h2", null, "Downloads")], -1),
+    ye = {
+        __name: "DownloadPopup",
+        setup(t) {
+            return (n, o) => (g(), _("details", we, [be, s("ul", null, [(g(!0), _(F, null, P(r(pe)(), c => (g(), _("li", {
+                key: c.entry.id
+            }, [m(v(c.entry.corpus) + " ", 1), s("em", null, v(c.state), 1)]))), 128))])]))
+        }
+    };
+const I = t => (ie("data-v-ec474531"), t = t(), ue(), t),
+    Le = {
         class: "downloader"
     },
-    ge = m(() => s("h1", {
+    Ie = I(() => s("h1", {
         class: "datasets-catalogue-title"
-    }, [h(" Datasets catalogue "), s("small", null, [s("em", null, "TODO"), h(" datasets")])], -1)),
-    me = {
+    }, [m(" Datasets catalogue "), s("small", null, [s("em", null, "TODO"), m(" datasets")])], -1)),
+    Oe = {
         class: "search-inputs"
     },
-    _e = {
+    Ne = ["value"],
+    De = ["value"],
+    Ue = {
         class: "dataset-list"
     },
-    fe = ["id"],
-    we = {
+    ke = ["id"],
+    Ve = {
         class: "dataset-name"
     },
-    be = {
+    Se = {
         class: "dataset-title"
     },
-    ye = ["href"],
-    ke = ["onClick", "disabled"],
-    De = {
+    Me = ["href"],
+    Be = ["onClick", "disabled"],
+    Ae = {
         class: "metadata-dataset"
     },
-    Ve = m(() => s("dt", null, "Version", -1)),
-    Oe = {
+    Te = I(() => s("dt", null, "Version", -1)),
+    $e = {
         title: "Version"
     },
-    Se = m(() => s("dt", null, "Languages", -1)),
-    Le = {
+    Ce = I(() => s("dt", null, "Languages", -1)),
+    Ge = {
         title: "Languages"
     },
-    Te = m(() => s("dt", null, "Pairs", -1)),
-    Ce = {
+    xe = I(() => s("dt", null, "Pairs", -1)),
+    je = {
         title: "Sentence pairs"
     },
-    Me = m(() => s("dt", null, "Size", -1)),
-    $e = {
+    Re = I(() => s("dt", null, "Size", -1)),
+    ze = {
         title: "Download size"
     },
-    Ie = {
-        class: "downloads-popup"
-    },
-    xe = m(() => s("summary", null, [s("h2", null, "Downloads")], -1)),
-    Be = {
+    Ee = {
         __name: "AddDatasetView",
-        setup(n) {
-            const o = [{
+        setup(t) {
+            function n(l) {
+                return l != ""
+            }
+            const o = {
+                    MONOLINGUAL: "monolingual",
+                    BILINGUAL: "bilingual"
+                },
+                c = [{
                     label: "Corpus name",
-                    compare: (a, e) => a.corpus.localeCompare(e.corpus)
+                    compare: (l, a) => l.corpus.localeCompare(a.corpus)
                 }, {
                     label: "Download size",
-                    compare: (a, e) => e.size - a.size
+                    compare: (l, a) => a.size - l.size
                 }, {
                     label: "Sentence pairs",
-                    compare: (a, e) => e.pairs - a.pairs
+                    compare: (l, a) => a.pairs - l.pairs
                 }],
-                l = r(o[0]),
-                _ = r(0),
+                V = u(c[0]),
+                S = new Map,
                 M = new Map,
-                $ = new Map,
-                k = r(""),
-                D = r(!0),
-                V = r(!0),
-                O = r(!0),
-                i = r(),
-                f = r(),
-                F = r(),
-                G = S(() => {
+                O = u(""),
+                N = u(!0),
+                d = u(o.BILINGUAL),
+                i = u(),
+                D = u(),
+                x = u(),
+                H = U(() => {
                     if (!i.value) return [];
-                    if (!M.has(i.value)) {
-                        const a = r([]);
-                        M.set(i.value, a), Y(i.value).then(e => {
-                            a.value = e
+                    if (!S.has(i.value)) {
+                        const l = u([]);
+                        S.set(i.value, l), _e(i.value).then(a => {
+                            l.value = a
                         })
                     }
-                    return M.get(i.value).value
+                    return S.get(i.value).value
                 }),
-                H = S(() => {
-                    const a = new Intl.DisplayNames([], {
+                K = U(() => {
+                    const l = new Intl.DisplayNames([], {
                         type: "language",
                         languageDisplay: "standard"
                     });
-                    return (F.value || []).map(e => {
+                    return (x.value || []).map(a => {
                         try {
                             return {
-                                lang: e,
-                                label: `${a.of(e)} (${e})`
+                                lang: a,
+                                label: `${l.of(a)} (${a})`
                             }
                         } catch {
                             return {
-                                lang: e,
-                                label: e
+                                lang: a,
+                                label: a
                             }
                         }
                     })
                 }),
-                K = S(() => {
-                    const a = new Intl.DisplayNames([], {
+                Q = U(() => {
+                    const l = new Intl.DisplayNames([], {
                         type: "language",
                         languageDisplay: "standard"
                     });
-                    return (G.value || []).map(e => {
+                    return (H.value || []).map(a => {
                         try {
                             return {
-                                lang: e,
-                                label: `${a.of(e)} (${e})`
+                                lang: a,
+                                label: `${l.of(a)} (${a})`
                             }
                         } catch {
                             return {
-                                lang: e,
-                                label: e
+                                lang: a,
+                                label: a
                             }
                         }
                     })
                 }),
-                Q = S(() => {
-                    if (!i.value || !f.value) return [];
-                    const a = `${i.value}-${f.value}`;
-                    if (!$.has(a)) {
-                        const t = r([]);
-                        $.set(a, t), Z(i.value, f.value).then(u => {
-                            t.value = u
-                        })
+                W = U(() => {
+                    let l;
+                    switch (d.value) {
+                        case o.BILINGUAL:
+                            if (!i.value || !D.value) return [];
+                            l = `${i.value}-${D.value}`;
+                            break;
+                        case o.MONOLINGUAL:
+                            if (!i.value) return [];
+                            l = `${i.value}`;
+                            break;
+                        default:
+                            throw new Error("Unknown preprocessing type")
                     }
-                    let e = $.get(a).value;
-                    return k.value.length > 0 && (e = e.filter(({
-                        corpus: t,
-                        group: u
-                    }) => t.toLowerCase().indexOf(k.value.toLowerCase()) !== -1)), e = e.filter(t => t.langs.length > 1 ? O.value : V.value), D.value && (e = Array.from(e.reduce((t, u) => ((!t.has(u.corpus) || t.get(u.corpus).version < u.version) && t.set(u.corpus, u), t), new Map).values())), e.sort(l.value.compare), e
-                }),
-                v = se({});
-            ne(async () => {
-                X().then(a => {
-                    F.value = a
-                }), E().then(a => {
-                    Object.assign(v, I(a))
+                    if (!M.has(l)) {
+                        const e = u([]);
+                        M.set(l, e), fe(l).then(p => e.value = p)
+                    }
+                    let a = M.get(l).value;
+                    return O.value.length > 0 && (a = a.filter(({
+                        corpus: e,
+                        group: p
+                    }) => e.toLowerCase().indexOf(O.value.toLowerCase()) !== -1)), a = a.filter(e => {
+                        switch (d.value) {
+                            case o.BILINGUAL:
+                                return e.langs.filter(n).length > 1;
+                            case o.MONOLINGUAL:
+                                return e.langs.filter(n).length == 1;
+                            default:
+                                return !1
+                        }
+                    }), N.value && (a = Array.from(a.reduce((e, p) => ((!e.has(p.corpus) || e.get(p.corpus).version < p.version) && e.set(p.corpus, p), e), new Map).values())), a.sort(V.value.compare), a
+                });
+            te(async () => {
+                me().then(l => {
+                    x.value = l
                 })
             });
-            let R = new he(1e3, async () => {
-                const a = await E();
-                Object.assign(v, I(a))
-            });
-            oe(v, a => {
-                const e = new Set(["pending", "downloading"]);
-                Object.values(a).some(t => e.has(t.state)) ? R.restart() : R.stop()
-            });
-
-            function I(a) {
-                return Object.fromEntries(a.map(e => [e.entry.id, e]))
-            }
-
-            function W(a) {
-                ee([a]).then(e => {
-                    Object.assign(v, I(e))
-                })
-            }
-            async function w(a, e) {
-                try {
-                    return _.value += 1, await (await fetch(a, e)).json()
-                } finally {
-                    _.value -= 1
-                }
-            }
-            async function X() {
-                return await w("/api/download/languages/")
-            }
-            async function Y(a) {
-                return await w(`/api/download/languages/${encodeURIComponent(a)}`)
-            }
-            async function Z(a, e) {
-                const t = `${a}-${e}`;
-                return await w(`/api/download/by-language/${encodeURIComponent(t)}`)
-            }
-            async function E() {
-                return await w("/api/download/downloads/")
-            }
-            async function ee(a) {
-                return await w("/api/download/downloads/", {
-                    method: "POST",
-                    headers: {
-                        "Content-Type": "application/json"
-                    },
-                    body: JSON.stringify(a.map(({
-                        id: e
-                    }) => ({
-                        id: e
-                    })))
-                })
-            }
-            const te = new Intl.NumberFormat;
-            return (a, e) => (g(), y("div", ve, [ge, s("div", me, [s("label", null, [L(s("input", {
+            const X = new Intl.NumberFormat;
+            return (l, a) => (g(), _("div", Le, [Ie, s("div", Oe, [s("label", null, [b(s("input", {
                 type: "search",
                 placeholder: "Search dataset\u2026",
-                "onUpdate:modelValue": e[0] || (e[0] = t => k.value = t)
+                "onUpdate:modelValue": a[0] || (a[0] = e => O.value = e)
             }, null, 512), [
-                [le, k.value]
+                [ae, O.value]
             ])]), s("label", {
-                class: j(["search-button", {
-                    checked: V.value
+                class: $(["search-button", {
+                    checked: d.value == o.MONOLINGUAL
                 }])
-            }, [L(s("input", {
-                type: "checkbox",
-                "onUpdate:modelValue": e[1] || (e[1] = t => V.value = t)
-            }, null, 512), [
-                [N, V.value]
-            ]), h(" Monolingual ")], 2), s("label", {
-                class: j(["search-button", {
-                    checked: O.value
+            }, [b(s("input", {
+                type: "radio",
+                name: "preprocessing",
+                "onUpdate:modelValue": a[1] || (a[1] = e => d.value = e),
+                value: o.MONOLINGUAL
+            }, null, 8, Ne), [
+                [R, d.value]
+            ]), m(" Monolingual ")], 2), s("label", {
+                class: $(["search-button", {
+                    checked: d.value == o.BILINGUAL
                 }])
-            }, [L(s("input", {
-                type: "checkbox",
-                "onUpdate:modelValue": e[2] || (e[2] = t => O.value = t)
-            }, null, 512), [
-                [N, O.value]
-            ]), h(" Bilingual ")], 2), s("label", {
-                class: j(["search-button", {
-                    checked: D.value
+            }, [b(s("input", {
+                type: "radio",
+                name: "preprocessing",
+                "onUpdate:modelValue": a[2] || (a[2] = e => d.value = e),
+                value: o.BILINGUAL
+            }, null, 8, De), [
+                [R, d.value]
+            ]), m(" Bilingual ")], 2), s("label", {
+                class: $(["search-button", {
+                    checked: N.value
                 }])
-            }, [L(s("input", {
+            }, [b(s("input", {
                 type: "checkbox",
-                "onUpdate:modelValue": e[3] || (e[3] = t => D.value = t)
+                "onUpdate:modelValue": a[3] || (a[3] = e => N.value = e)
             }, null, 512), [
-                [N, D.value]
-            ]), h(" Latest only ")], 2), s("label", null, [T(c(z), {
+                [ne, N.value]
+            ]), m(" Latest only ")], 2), s("label", null, [y(r(C), {
                 modelValue: i.value,
-                "onUpdate:modelValue": e[4] || (e[4] = t => i.value = t),
-                options: c(H),
+                "onUpdate:modelValue": a[4] || (a[4] = e => i.value = e),
+                options: r(K),
                 reduce: ({
-                    lang: t
-                }) => t,
+                    lang: e
+                }) => e,
                 placeholder: "Origin language"
-            }, null, 8, ["modelValue", "options", "reduce"])]), s("label", null, [T(c(z), {
-                modelValue: f.value,
-                "onUpdate:modelValue": e[5] || (e[5] = t => f.value = t),
-                options: c(K),
+            }, null, 8, ["modelValue", "options", "reduce"])]), b(s("label", null, [y(r(C), {
+                modelValue: D.value,
+                "onUpdate:modelValue": a[5] || (a[5] = e => D.value = e),
+                options: r(Q),
                 reduce: ({
-                    lang: t
-                }) => t,
+                    lang: e
+                }) => e,
                 placeholder: "Target language"
-            }, null, 8, ["modelValue", "options", "reduce"])]), s("label", null, [T(c(z), {
-                modelValue: l.value,
-                "onUpdate:modelValue": e[6] || (e[6] = t => l.value = t),
-                options: o,
+            }, null, 8, ["modelValue", "options", "reduce"])], 512), [
+                [se, d.value == o.BILINGUAL]
+            ]), s("label", null, [y(r(C), {
+                modelValue: V.value,
+                "onUpdate:modelValue": a[6] || (a[6] = e => V.value = e),
+                options: c,
                 placeholder: "Sort order"
-            }, null, 8, ["modelValue"])])]), s("div", _e, [(g(!0), y(P, null, J(c(Q), t => (g(), y("div", {
+            }, null, 8, ["modelValue"])])]), s("div", Ue, [(g(!0), _(F, null, P(r(W), e => (g(), _("div", {
                 class: "dataset",
-                key: t.id,
-                id: `did-${t.id}`
-            }, [s("div", we, [s("h3", be, [s("a", {
-                href: `https://opus.nlpl.eu/${t.corpus}-${t.version}.php`,
+                key: e.id,
+                id: `did-${e.id}`
+            }, [s("div", Ve, [s("h3", Se, [s("a", {
+                href: `https://opus.nlpl.eu/${e.corpus}-${e.version}.php`,
                 target: "_blank"
-            }, p(t.corpus), 9, ye)]), s("button", {
+            }, v(e.corpus), 9, Me)]), s("button", {
                 class: "download-dataset-button",
-                onClick: u => W(t),
-                disabled: t.id in v || "paths" in t
-            }, [h(" Download "), T(c(ue), {
+                onClick: p => r(ve)(e),
+                disabled: r(ge)(e) || "paths" in e
+            }, [m(" Download "), y(r(re), {
                 class: "download-icon"
-            })], 8, ke)]), s("dl", De, [Ve, s("dd", Oe, p(t.version), 1), Se, s("dd", Le, p(t.langs.join("\u2192")), 1), Te, s("dd", Ce, p(t.pairs ? c(te).format(t.pairs) : ""), 1), Me, s("dd", $e, p(t.size ? c(pe)(t.size) : ""), 1)])], 8, fe))), 128))]), (g(), re(ie, {
+            })], 8, Be)]), s("dl", Ae, [Te, s("dd", $e, v(e.version), 1), Ce, s("dd", Ge, v(e.langs.filter(n).join("\u2192")), 1), xe, s("dd", je, v(e.pairs ? r(X).format(e.pairs) : ""), 1), Re, s("dd", ze, v(e.size ? r(ce)(e.size) : ""), 1)])], 8, ke))), 128))]), (g(), oe(le, {
                 to: ".navbar"
-            }, [s("details", Ie, [xe, s("ul", null, [(g(!0), y(P, null, J(v, t => (g(), y("li", {
-                key: t.entry.id
-            }, [h(p(t.entry.corpus) + " ", 1), s("em", null, p(t.state), 1)]))), 128))])])]))]))
+            }, [y(ye)]))]))
         }
     },
-    ze = ae(Be, [
-        ["__scopeId", "data-v-183e5481"]
+    qe = ee(Ee, [
+        ["__scopeId", "data-v-ec474531"]
     ]);
 export {
-    ze as
+    qe as
     default
 };
```

### Comparing `opuscleaner-0.2.2/opuscleaner/frontend/assets/EditFiltersView.bc0dd7c3.js` & `opuscleaner-0.3.0/opuscleaner/frontend/assets/EditFiltersView.877cfb0b.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -40,15 +40,15 @@
     ab as co,
     T as sr,
     ac as vo,
     ad as po,
     ae as ho,
     af as mo,
     ag as go,
-    m as qt,
+    m as Qt,
     a as ce,
     y as _t,
     c as W,
     d as X,
     ah as yo,
     ai as bo,
     aj as So,
@@ -90,15 +90,15 @@
     o as U,
     h as Fn,
     aR as Qo,
     p as $n,
     aS as Zo,
     aT as ko,
     r as Gt,
-    aU as Qt,
+    aU as Zt,
     aV as dr,
     aW as qo,
     aX as Xe,
     aY as _o,
     aZ as ta,
     a_ as ea,
     a$ as na,
@@ -147,27 +147,27 @@
     bA as Ka,
     bB as pr,
     bC as Ha,
     bD as Wa,
     bE as Xa,
     B as Ya,
     U as za
-} from "./index.6cc31f0d.js";
+} from "./index.aa84b8f1.js";
 import {
     d as hr,
     a as Ja,
     T as Qa,
     b as Za
-} from "./TagsEditor.23cf196f.js";
+} from "./TagsEditor.3f956450.js";
 import {
     g as Ln
-} from "./hacks.1ae1ba64.js";
+} from "./hacks.175c31f5.js";
 import {
     C as ka
-} from "./vue-select.9ddbca8a.js";
+} from "./vue-select.973ce47f.js";
 const qa = () => {},
     _a = Object.freeze(Object.defineProperty({
         __proto__: null,
         compile: qa,
         EffectScope: jr,
         ReactiveEffect: Fr,
         customRef: $r,
@@ -209,15 +209,15 @@
         Suspense: co,
         Teleport: sr,
         Text: vo,
         callWithAsyncErrorHandling: po,
         callWithErrorHandling: ho,
         cloneVNode: mo,
         compatUtils: go,
-        computed: qt,
+        computed: Qt,
         createBlock: ce,
         createCommentVNode: _t,
         createElementBlock: W,
         createElementVNode: X,
         createHydrationRenderer: yo,
         createPropsRestProxy: bo,
         createRenderer: So,
@@ -261,15 +261,15 @@
         openBlock: U,
         popScopeId: Fn,
         provide: Qo,
         pushScopeId: $n,
         queuePostFlushCb: Zo,
         registerRuntimeCompiler: ko,
         renderList: Gt,
-        renderSlot: Qt,
+        renderSlot: Zt,
         resolveComponent: dr,
         resolveDirective: qo,
         resolveDynamicComponent: Xe,
         resolveFilter: _o,
         resolveTransitionHooks: ta,
         setBlockTracking: ea,
         setDevtoolsHook: na,
@@ -551,35 +551,35 @@
 function te() {
     var a = document.scrollingElement;
     return a || document.documentElement
 }
 
 function ft(a, e, n, i, r) {
     if (!(!a.getBoundingClientRect && a !== window)) {
-        var s, t, o, l, u, f, c;
-        if (a !== window && a.parentNode && a !== te() ? (s = a.getBoundingClientRect(), t = s.top, o = s.left, l = s.bottom, u = s.right, f = s.height, c = s.width) : (t = 0, o = 0, l = window.innerHeight, u = window.innerWidth, f = window.innerHeight, c = window.innerWidth), (e || n) && a !== window && (r = r || a.parentNode, !ae))
+        var s, t, o, l, u, c, f;
+        if (a !== window && a.parentNode && a !== te() ? (s = a.getBoundingClientRect(), t = s.top, o = s.left, l = s.bottom, u = s.right, c = s.height, f = s.width) : (t = 0, o = 0, l = window.innerHeight, u = window.innerWidth, c = window.innerHeight, f = window.innerWidth), (e || n) && a !== window && (r = r || a.parentNode, !ae))
             do
                 if (r && r.getBoundingClientRect && (G(r, "transform") !== "none" || n && G(r, "position") !== "static")) {
                     var d = r.getBoundingClientRect();
                     t -= d.top + parseInt(G(r, "border-top-width")), o -= d.left + parseInt(G(r, "border-left-width")), l = t + s.height, u = o + s.width;
                     break
                 } while (r = r.parentNode);
         if (i && a !== window) {
             var v = ge(r || a),
                 p = v && v.a,
                 h = v && v.d;
-            v && (t /= h, o /= p, c /= p, f /= h, l = t + f, u = o + c)
+            v && (t /= h, o /= p, f /= p, c /= h, l = t + c, u = o + f)
         }
         return {
             top: t,
             left: o,
             bottom: l,
             right: u,
-            width: c,
-            height: f
+            width: f,
+            height: c
         }
     }
 }
 
 function Qn(a, e, n) {
     for (var i = fe(a, !0), r = ft(a)[e]; i;) {
         var s = ft(i)[n],
@@ -736,36 +736,36 @@
                 return
             }
             var s = !1,
                 t = 0;
             a.forEach(function(o) {
                 var l = 0,
                     u = o.target,
-                    f = u.fromRect,
-                    c = ft(u),
+                    c = u.fromRect,
+                    f = ft(u),
                     d = u.prevFromRect,
                     v = u.prevToRect,
                     p = o.rect,
                     h = ge(u, !0);
-                h && (c.top -= h.f, c.left -= h.e), u.toRect = c, u.thisAnimationDuration && yn(d, c) && !yn(f, c) && (p.top - c.top) / (p.left - c.left) === (f.top - c.top) / (f.left - c.left) && (l = bi(p, d, v, r.options)), yn(c, f) || (u.prevFromRect = f, u.prevToRect = c, l || (l = r.options.animation), r.animate(u, p, c, l)), l && (s = !0, t = Math.max(t, l), clearTimeout(u.animationResetTimer), u.animationResetTimer = setTimeout(function() {
+                h && (f.top -= h.f, f.left -= h.e), u.toRect = f, u.thisAnimationDuration && yn(d, f) && !yn(c, f) && (p.top - f.top) / (p.left - f.left) === (c.top - f.top) / (c.left - f.left) && (l = bi(p, d, v, r.options)), yn(f, c) || (u.prevFromRect = c, u.prevToRect = f, l || (l = r.options.animation), r.animate(u, p, f, l)), l && (s = !0, t = Math.max(t, l), clearTimeout(u.animationResetTimer), u.animationResetTimer = setTimeout(function() {
                     u.animationTime = 0, u.prevFromRect = null, u.fromRect = null, u.prevToRect = null, u.thisAnimationDuration = null
                 }, l), u.thisAnimationDuration = l)
             }), clearTimeout(e), s ? e = setTimeout(function() {
                 typeof i == "function" && i()
             }, t) : typeof i == "function" && i(), a = []
         },
         animate: function(i, r, s, t) {
             if (t) {
                 G(i, "transition", ""), G(i, "transform", "");
                 var o = ge(this.el),
                     l = o && o.a,
                     u = o && o.d,
-                    f = (r.left - s.left) / (l || 1),
-                    c = (r.top - s.top) / (u || 1);
-                i.animatingX = !!f, i.animatingY = !!c, G(i, "transform", "translate3d(" + f + "px," + c + "px,0)"), this.forRepaintDummy = yi(i), G(i, "transition", "transform " + t + "ms" + (this.options.easing ? " " + this.options.easing : "")), G(i, "transform", "translate3d(0,0,0)"), typeof i.animated == "number" && clearTimeout(i.animated), i.animated = setTimeout(function() {
+                    c = (r.left - s.left) / (l || 1),
+                    f = (r.top - s.top) / (u || 1);
+                i.animatingX = !!c, i.animatingY = !!f, G(i, "transform", "translate3d(" + c + "px," + f + "px,0)"), this.forRepaintDummy = yi(i), G(i, "transition", "transform " + t + "ms" + (this.options.easing ? " " + this.options.easing : "")), G(i, "transform", "translate3d(0,0,0)"), typeof i.animated == "number" && clearTimeout(i.animated), i.animated = setTimeout(function() {
                     G(i, "transition", ""), G(i, "transform", ""), i.animated = !1, i.animatingX = !1, i.animatingY = !1
                 }, t)
             }
         }
     }
 }
 
@@ -835,38 +835,38 @@
         i = a.name,
         r = a.targetEl,
         s = a.cloneEl,
         t = a.toEl,
         o = a.fromEl,
         l = a.oldIndex,
         u = a.newIndex,
-        f = a.oldDraggableIndex,
-        c = a.newDraggableIndex,
+        c = a.oldDraggableIndex,
+        f = a.newDraggableIndex,
         d = a.originalEvent,
         v = a.putSortable,
         p = a.extraEventProperties;
     if (e = e || n && n[Rt], !!e) {
         var h, m = e.options,
             g = "on" + i.charAt(0).toUpperCase() + i.substr(1);
         window.CustomEvent && !ae && !Ye ? h = new CustomEvent(i, {
             bubbles: !0,
             cancelable: !0
-        }) : (h = document.createEvent("Event"), h.initEvent(i, !0, !0)), h.to = t || n, h.from = o || n, h.item = r || n, h.clone = s, h.oldIndex = l, h.newIndex = u, h.oldDraggableIndex = f, h.newDraggableIndex = c, h.originalEvent = d, h.pullMode = v ? v.lastPutMode : void 0;
+        }) : (h = document.createEvent("Event"), h.initEvent(i, !0, !0)), h.to = t || n, h.from = o || n, h.item = r || n, h.clone = s, h.oldIndex = l, h.newIndex = u, h.oldDraggableIndex = c, h.newDraggableIndex = f, h.originalEvent = d, h.pullMode = v ? v.lastPutMode : void 0;
         var y = ee(ee({}, p), ze.getEventProperties(i, e));
         for (var O in y) h[O] = y[O];
         n && n.dispatchEvent(h), m[g] && m[g].call(e, h)
     }
 }
 var Si = ["evt"],
     Ft = function(e, n) {
         var i = arguments.length > 2 && arguments[2] !== void 0 ? arguments[2] : {},
             r = i.evt,
             s = ai(i, Si);
         ze.pluginEvent.bind(z)(e, n, ee({
-            dragEl: w,
+            dragEl: M,
             parentEl: ht,
             ghostEl: q,
             rootEl: ut,
             nextEl: me,
             lastDownEl: rn,
             cloneEl: mt,
             cloneHidden: ue,
@@ -896,23 +896,23 @@
         }, s))
     };
 
 function Mt(a) {
     Fe(ee({
         putSortable: Dt,
         cloneEl: mt,
-        targetEl: w,
+        targetEl: M,
         rootEl: ut,
         oldIndex: Oe,
         oldDraggableIndex: Be,
         newIndex: Ut,
         newDraggableIndex: se
     }, a))
 }
-var w, ht, q, ut, me, rn, mt, ue, Oe, Ut, Be, se, Ze, Dt, xe = !1,
+var M, ht, q, ut, me, rn, mt, ue, Oe, Ut, Be, se, Ze, Dt, xe = !1,
     fn = !1,
     cn = [],
     pe, Xt, En, xn, qn, _n, $e, Se, Ke, He = !1,
     ke = !1,
     on, At, On = [],
     An = !1,
     dn = [],
@@ -931,22 +931,22 @@
         var i = G(e),
             r = parseInt(i.width) - parseInt(i.paddingLeft) - parseInt(i.paddingRight) - parseInt(i.borderLeftWidth) - parseInt(i.borderRightWidth),
             s = Ie(e, 0, n),
             t = Ie(e, 1, n),
             o = s && G(s),
             l = t && G(t),
             u = o && parseInt(o.marginLeft) + parseInt(o.marginRight) + ft(s).width,
-            f = l && parseInt(l.marginLeft) + parseInt(l.marginRight) + ft(t).width;
+            c = l && parseInt(l.marginLeft) + parseInt(l.marginRight) + ft(t).width;
         if (i.display === "flex") return i.flexDirection === "column" || i.flexDirection === "column-reverse" ? "vertical" : "horizontal";
         if (i.display === "grid") return i.gridTemplateColumns.split(" ").length <= 1 ? "vertical" : "horizontal";
         if (s && o.float && o.float !== "none") {
-            var c = o.float === "left" ? "left" : "right";
-            return t && (l.clear === "both" || l.clear === c) ? "vertical" : "horizontal"
+            var f = o.float === "left" ? "left" : "right";
+            return t && (l.clear === "both" || l.clear === f) ? "vertical" : "horizontal"
         }
-        return s && (o.display === "block" || o.display === "flex" || o.display === "table" || o.display === "grid" || u >= r && i[tr] === "none" || t && i[tr] === "none" && u + f > r) ? "vertical" : "horizontal"
+        return s && (o.display === "block" || o.display === "flex" || o.display === "table" || o.display === "grid" || u >= r && i[tr] === "none" || t && i[tr] === "none" && u + c > r) ? "vertical" : "horizontal"
     },
     xi = function(e, n, i) {
         var r = i ? e.left : e.top,
             s = i ? e.right : e.bottom,
             t = i ? e.width : e.height,
             o = i ? n.left : n.top,
             l = i ? n.right : n.bottom,
@@ -963,20 +963,20 @@
                     l = n >= t.top - s && n <= t.bottom + s;
                 if (o && l) return i = r
             }
         }), i
     },
     Ir = function(e) {
         function n(s, t) {
-            return function(o, l, u, f) {
-                var c = o.options.group.name && l.options.group.name && o.options.group.name === l.options.group.name;
-                if (s == null && (t || c)) return !0;
+            return function(o, l, u, c) {
+                var f = o.options.group.name && l.options.group.name && o.options.group.name === l.options.group.name;
+                if (s == null && (t || f)) return !0;
                 if (s == null || s === !1) return !1;
                 if (t && s === "clone") return s;
-                if (typeof s == "function") return n(s(o, l, u, f), t)(o, l, u, f);
+                if (typeof s == "function") return n(s(o, l, u, c), t)(o, l, u, c);
                 var d = (t ? o : l).options.group.name;
                 return s === !0 || typeof s == "string" && s === d || s.join && s.indexOf(d) > -1
             }
         }
         var i = {},
             r = e.group;
         (!r || nn(r) != "object") && (r = {
@@ -989,26 +989,26 @@
     Cr = function() {
         !Or && q && G(q, "display", "")
     };
 hn && document.addEventListener("click", function(a) {
     if (fn) return a.preventDefault(), a.stopPropagation && a.stopPropagation(), a.stopImmediatePropagation && a.stopImmediatePropagation(), fn = !1, !1
 }, !0);
 var he = function(e) {
-        if (w) {
+        if (M) {
             e = e.touches ? e.touches[0] : e;
             var n = Oi(e.clientX, e.clientY);
             if (n) {
                 var i = {};
                 for (var r in e) e.hasOwnProperty(r) && (i[r] = e[r]);
                 i.target = i.rootEl = n, i.preventDefault = void 0, i.stopPropagation = void 0, n[Rt]._onDragOver(i)
             }
         }
     },
     Ti = function(e) {
-        w && w.parentNode[Rt]._isOutsideThisEl(e.target)
+        M && M.parentNode[Rt]._isOutsideThisEl(e.target)
     };
 
 function z(a, e) {
     if (!(a && a.nodeType && a.nodeType === 1)) throw "Sortable: `el` must be an HTMLElement, not ".concat({}.toString.call(a));
     this.el = a, this.options = e = Ht({}, e), a[Rt] = this;
     var n = {
         group: null,
@@ -1060,88 +1060,88 @@
 }
 z.prototype = {
     constructor: z,
     _isOutsideThisEl: function(e) {
         !this.el.contains(e) && e !== this.el && (Se = null)
     },
     _getDirection: function(e, n) {
-        return typeof this.options.direction == "function" ? this.options.direction.call(this, e, n, w) : this.options.direction
+        return typeof this.options.direction == "function" ? this.options.direction.call(this, e, n, M) : this.options.direction
     },
     _onTapStart: function(e) {
         if (!!e.cancelable) {
             var n = this,
                 i = this.el,
                 r = this.options,
                 s = r.preventOnFilter,
                 t = e.type,
                 o = e.touches && e.touches[0] || e.pointerType && e.pointerType === "touch" && e,
                 l = (o || e).target,
                 u = e.target.shadowRoot && (e.path && e.path[0] || e.composedPath && e.composedPath()[0]) || l,
-                f = r.filter;
-            if (Mi(i), !w && !(/mousedown|pointerdown/.test(t) && e.button !== 0 || r.disabled) && !u.isContentEditable && !(!this.nativeDraggable && Ue && l && l.tagName.toUpperCase() === "SELECT") && (l = Jt(l, r.draggable, i, !1), !(l && l.animated) && rn !== l)) {
-                if (Oe = gt(l), Be = gt(l, r.draggable), typeof f == "function") {
-                    if (f.call(this, e, l, this)) {
+                c = r.filter;
+            if (Mi(i), !M && !(/mousedown|pointerdown/.test(t) && e.button !== 0 || r.disabled) && !u.isContentEditable && !(!this.nativeDraggable && Ue && l && l.tagName.toUpperCase() === "SELECT") && (l = Jt(l, r.draggable, i, !1), !(l && l.animated) && rn !== l)) {
+                if (Oe = gt(l), Be = gt(l, r.draggable), typeof c == "function") {
+                    if (c.call(this, e, l, this)) {
                         Mt({
                             sortable: n,
                             rootEl: u,
                             name: "filter",
                             targetEl: l,
                             toEl: i,
                             fromEl: i
                         }), Ft("filter", n, {
                             evt: e
                         }), s && e.cancelable && e.preventDefault();
                         return
                     }
-                } else if (f && (f = f.split(",").some(function(c) {
-                        if (c = Jt(u, c.trim(), i, !1), c) return Mt({
+                } else if (c && (c = c.split(",").some(function(f) {
+                        if (f = Jt(u, f.trim(), i, !1), f) return Mt({
                             sortable: n,
-                            rootEl: c,
+                            rootEl: f,
                             name: "filter",
                             targetEl: l,
                             fromEl: i,
                             toEl: i
                         }), Ft("filter", n, {
                             evt: e
                         }), !0
-                    }), f)) {
+                    }), c)) {
                     s && e.cancelable && e.preventDefault();
                     return
                 }
                 r.handle && !Jt(u, r.handle, i, !1) || this._prepareDragStart(e, o, l)
             }
         }
     },
     _prepareDragStart: function(e, n, i) {
         var r = this,
             s = r.el,
             t = r.options,
             o = s.ownerDocument,
             l;
-        if (i && !w && i.parentNode === s) {
+        if (i && !M && i.parentNode === s) {
             var u = ft(i);
-            if (ut = s, w = i, ht = w.parentNode, me = w.nextSibling, rn = i, Ze = t.group, z.dragged = w, pe = {
-                    target: w,
+            if (ut = s, M = i, ht = M.parentNode, me = M.nextSibling, rn = i, Ze = t.group, z.dragged = M, pe = {
+                    target: M,
                     clientX: (n || e).clientX,
                     clientY: (n || e).clientY
-                }, qn = pe.clientX - u.left, _n = pe.clientY - u.top, this._lastX = (n || e).clientX, this._lastY = (n || e).clientY, w.style["will-change"] = "all", l = function() {
+                }, qn = pe.clientX - u.left, _n = pe.clientY - u.top, this._lastX = (n || e).clientX, this._lastY = (n || e).clientY, M.style["will-change"] = "all", l = function() {
                     if (Ft("delayEnded", r, {
                             evt: e
                         }), z.eventCanceled) {
                         r._onDrop();
                         return
                     }
-                    r._disableDelayedDragEvents(), !zn && r.nativeDraggable && (w.draggable = !0), r._triggerDragStart(e, n), Mt({
+                    r._disableDelayedDragEvents(), !zn && r.nativeDraggable && (M.draggable = !0), r._triggerDragStart(e, n), Mt({
                         sortable: r,
                         name: "choose",
                         originalEvent: e
-                    }), vt(w, t.chosenClass, !0)
-                }, t.ignore.split(",").forEach(function(f) {
-                    Sr(w, f.trim(), Tn)
-                }), et(o, "dragover", he), et(o, "mousemove", he), et(o, "touchmove", he), et(o, "mouseup", r._onDrop), et(o, "touchend", r._onDrop), et(o, "touchcancel", r._onDrop), zn && this.nativeDraggable && (this.options.touchStartThreshold = 4, w.draggable = !0), Ft("delayStart", this, {
+                    }), vt(M, t.chosenClass, !0)
+                }, t.ignore.split(",").forEach(function(c) {
+                    Sr(M, c.trim(), Tn)
+                }), et(o, "dragover", he), et(o, "mousemove", he), et(o, "touchmove", he), et(o, "mouseup", r._onDrop), et(o, "touchend", r._onDrop), et(o, "touchcancel", r._onDrop), zn && this.nativeDraggable && (this.options.touchStartThreshold = 4, M.draggable = !0), Ft("delayStart", this, {
                     evt: e
                 }), t.delay && (!t.delayOnTouchOnly || n) && (!this.nativeDraggable || !(Ye || ae))) {
                 if (z.eventCanceled) {
                     this._onDrop();
                     return
                 }
                 et(o, "mouseup", r._disableDelayedDrag), et(o, "touchend", r._disableDelayedDrag), et(o, "touchcancel", r._disableDelayedDrag), et(o, "mousemove", r._delayedDragTouchMoveHandler), et(o, "touchmove", r._delayedDragTouchMoveHandler), t.supportPointer && et(o, "pointermove", r._delayedDragTouchMoveHandler), r._dragStartTimer = setTimeout(l, t.delay)
@@ -1149,46 +1149,46 @@
         }
     },
     _delayedDragTouchMoveHandler: function(e) {
         var n = e.touches ? e.touches[0] : e;
         Math.max(Math.abs(n.clientX - this._lastX), Math.abs(n.clientY - this._lastY)) >= Math.floor(this.options.touchStartThreshold / (this.nativeDraggable && window.devicePixelRatio || 1)) && this._disableDelayedDrag()
     },
     _disableDelayedDrag: function() {
-        w && Tn(w), clearTimeout(this._dragStartTimer), this._disableDelayedDragEvents()
+        M && Tn(M), clearTimeout(this._dragStartTimer), this._disableDelayedDragEvents()
     },
     _disableDelayedDragEvents: function() {
         var e = this.el.ownerDocument;
         tt(e, "mouseup", this._disableDelayedDrag), tt(e, "touchend", this._disableDelayedDrag), tt(e, "touchcancel", this._disableDelayedDrag), tt(e, "mousemove", this._delayedDragTouchMoveHandler), tt(e, "touchmove", this._delayedDragTouchMoveHandler), tt(e, "pointermove", this._delayedDragTouchMoveHandler)
     },
     _triggerDragStart: function(e, n) {
-        n = n || e.pointerType == "touch" && e, !this.nativeDraggable || n ? this.options.supportPointer ? et(document, "pointermove", this._onTouchMove) : n ? et(document, "touchmove", this._onTouchMove) : et(document, "mousemove", this._onTouchMove) : (et(w, "dragend", this), et(ut, "dragstart", this._onDragStart));
+        n = n || e.pointerType == "touch" && e, !this.nativeDraggable || n ? this.options.supportPointer ? et(document, "pointermove", this._onTouchMove) : n ? et(document, "touchmove", this._onTouchMove) : et(document, "mousemove", this._onTouchMove) : (et(M, "dragend", this), et(ut, "dragstart", this._onDragStart));
         try {
             document.selection ? an(function() {
                 document.selection.empty()
             }) : window.getSelection().removeAllRanges()
         } catch {}
     },
     _dragStarted: function(e, n) {
-        if (xe = !1, ut && w) {
+        if (xe = !1, ut && M) {
             Ft("dragStarted", this, {
                 evt: n
             }), this.nativeDraggable && et(document, "dragover", Ti);
             var i = this.options;
-            !e && vt(w, i.dragClass, !1), vt(w, i.ghostClass, !0), z.active = this, e && this._appendGhost(), Mt({
+            !e && vt(M, i.dragClass, !1), vt(M, i.ghostClass, !0), z.active = this, e && this._appendGhost(), Mt({
                 sortable: this,
                 name: "start",
                 originalEvent: n
             })
         } else this._nulling()
     },
     _emulateDragOver: function() {
         if (Xt) {
             this._lastX = Xt.clientX, this._lastY = Xt.clientY, Pr();
             for (var e = document.elementFromPoint(Xt.clientX, Xt.clientY), n = e; e && e.shadowRoot && (e = e.shadowRoot.elementFromPoint(Xt.clientX, Xt.clientY), e !== n);) n = e;
-            if (w.parentNode[Rt]._isOutsideThisEl(e), n)
+            if (M.parentNode[Rt]._isOutsideThisEl(e), n)
                 do {
                     if (n[Rt]) {
                         var i = void 0;
                         if (i = n[Rt]._onDragOver({
                                 clientX: Xt.clientX,
                                 clientY: Xt.clientY,
                                 target: e,
@@ -1206,175 +1206,175 @@
                 i = n.fallbackTolerance,
                 r = n.fallbackOffset,
                 s = e.touches ? e.touches[0] : e,
                 t = q && ge(q, !0),
                 o = q && t && t.a,
                 l = q && t && t.d,
                 u = qe && At && Zn(At),
-                f = (s.clientX - pe.clientX + r.x) / (o || 1) + (u ? u[0] - On[0] : 0) / (o || 1),
-                c = (s.clientY - pe.clientY + r.y) / (l || 1) + (u ? u[1] - On[1] : 0) / (l || 1);
+                c = (s.clientX - pe.clientX + r.x) / (o || 1) + (u ? u[0] - On[0] : 0) / (o || 1),
+                f = (s.clientY - pe.clientY + r.y) / (l || 1) + (u ? u[1] - On[1] : 0) / (l || 1);
             if (!z.active && !xe) {
                 if (i && Math.max(Math.abs(s.clientX - this._lastX), Math.abs(s.clientY - this._lastY)) < i) return;
                 this._onDragStart(e, !0)
             }
             if (q) {
-                t ? (t.e += f - (En || 0), t.f += c - (xn || 0)) : t = {
+                t ? (t.e += c - (En || 0), t.f += f - (xn || 0)) : t = {
                     a: 1,
                     b: 0,
                     c: 0,
                     d: 1,
-                    e: f,
-                    f: c
+                    e: c,
+                    f
                 };
                 var d = "matrix(".concat(t.a, ",").concat(t.b, ",").concat(t.c, ",").concat(t.d, ",").concat(t.e, ",").concat(t.f, ")");
-                G(q, "webkitTransform", d), G(q, "mozTransform", d), G(q, "msTransform", d), G(q, "transform", d), En = f, xn = c, Xt = s
+                G(q, "webkitTransform", d), G(q, "mozTransform", d), G(q, "msTransform", d), G(q, "transform", d), En = c, xn = f, Xt = s
             }
             e.cancelable && e.preventDefault()
         }
     },
     _appendGhost: function() {
         if (!q) {
             var e = this.options.fallbackOnBody ? document.body : ut,
-                n = ft(w, !0, qe, !0, e),
+                n = ft(M, !0, qe, !0, e),
                 i = this.options;
             if (qe) {
                 for (At = e; G(At, "position") === "static" && G(At, "transform") === "none" && At !== document;) At = At.parentNode;
                 At !== document.body && At !== document.documentElement ? (At === document && (At = te()), n.top += At.scrollTop, n.left += At.scrollLeft) : At = te(), On = Zn(At)
             }
-            q = w.cloneNode(!0), vt(q, i.ghostClass, !1), vt(q, i.fallbackClass, !0), vt(q, i.dragClass, !0), G(q, "transition", ""), G(q, "transform", ""), G(q, "box-sizing", "border-box"), G(q, "margin", 0), G(q, "top", n.top), G(q, "left", n.left), G(q, "width", n.width), G(q, "height", n.height), G(q, "opacity", "0.8"), G(q, "position", qe ? "absolute" : "fixed"), G(q, "zIndex", "100000"), G(q, "pointerEvents", "none"), z.ghost = q, e.appendChild(q), G(q, "transform-origin", qn / parseInt(q.style.width) * 100 + "% " + _n / parseInt(q.style.height) * 100 + "%")
+            q = M.cloneNode(!0), vt(q, i.ghostClass, !1), vt(q, i.fallbackClass, !0), vt(q, i.dragClass, !0), G(q, "transition", ""), G(q, "transform", ""), G(q, "box-sizing", "border-box"), G(q, "margin", 0), G(q, "top", n.top), G(q, "left", n.left), G(q, "width", n.width), G(q, "height", n.height), G(q, "opacity", "0.8"), G(q, "position", qe ? "absolute" : "fixed"), G(q, "zIndex", "100000"), G(q, "pointerEvents", "none"), z.ghost = q, e.appendChild(q), G(q, "transform-origin", qn / parseInt(q.style.width) * 100 + "% " + _n / parseInt(q.style.height) * 100 + "%")
         }
     },
     _onDragStart: function(e, n) {
         var i = this,
             r = e.dataTransfer,
             s = i.options;
         if (Ft("dragStart", this, {
                 evt: e
             }), z.eventCanceled) {
             this._onDrop();
             return
         }
-        Ft("setupClone", this), z.eventCanceled || (mt = Un(w), mt.draggable = !1, mt.style["will-change"] = "", this._hideClone(), vt(mt, this.options.chosenClass, !1), z.clone = mt), i.cloneId = an(function() {
-            Ft("clone", i), !z.eventCanceled && (i.options.removeCloneOnHide || ut.insertBefore(mt, w), i._hideClone(), Mt({
+        Ft("setupClone", this), z.eventCanceled || (mt = Un(M), mt.draggable = !1, mt.style["will-change"] = "", this._hideClone(), vt(mt, this.options.chosenClass, !1), z.clone = mt), i.cloneId = an(function() {
+            Ft("clone", i), !z.eventCanceled && (i.options.removeCloneOnHide || ut.insertBefore(mt, M), i._hideClone(), Mt({
                 sortable: i,
                 name: "clone"
             }))
-        }), !n && vt(w, s.dragClass, !0), n ? (fn = !0, i._loopId = setInterval(i._emulateDragOver, 50)) : (tt(document, "mouseup", i._onDrop), tt(document, "touchend", i._onDrop), tt(document, "touchcancel", i._onDrop), r && (r.effectAllowed = "move", s.setData && s.setData.call(i, r, w)), et(document, "drop", i), G(w, "transform", "translateZ(0)")), xe = !0, i._dragStartId = an(i._dragStarted.bind(i, n, e)), et(document, "selectstart", i), $e = !0, Ue && G(document.body, "user-select", "none")
+        }), !n && vt(M, s.dragClass, !0), n ? (fn = !0, i._loopId = setInterval(i._emulateDragOver, 50)) : (tt(document, "mouseup", i._onDrop), tt(document, "touchend", i._onDrop), tt(document, "touchcancel", i._onDrop), r && (r.effectAllowed = "move", s.setData && s.setData.call(i, r, M)), et(document, "drop", i), G(M, "transform", "translateZ(0)")), xe = !0, i._dragStartId = an(i._dragStarted.bind(i, n, e)), et(document, "selectstart", i), $e = !0, Ue && G(document.body, "user-select", "none")
     },
     _onDragOver: function(e) {
         var n = this.el,
             i = e.target,
             r, s, t, o = this.options,
             l = o.group,
             u = z.active,
-            f = Ze === l,
-            c = o.sort,
+            c = Ze === l,
+            f = o.sort,
             d = Dt || u,
             v, p = this,
             h = !1;
         if (An) return;
 
         function m(k, ot) {
             Ft(k, p, ee({
                 evt: e,
-                isOwner: f,
+                isOwner: c,
                 axis: v ? "vertical" : "horizontal",
                 revert: t,
                 dragRect: r,
                 targetRect: s,
-                canSort: c,
+                canSort: f,
                 fromSortable: d,
                 target: i,
                 completed: y,
                 onMove: function(ct, pt) {
-                    return _e(ut, n, w, r, ct, ft(ct), e, pt)
+                    return _e(ut, n, M, r, ct, ft(ct), e, pt)
                 },
                 changed: O
             }, ot))
         }
 
         function g() {
             m("dragOverAnimationCapture"), p.captureAnimationState(), p !== d && d.captureAnimationState()
         }
 
         function y(k) {
             return m("dragOverCompleted", {
                 insertion: k
-            }), k && (f ? u._hideClone() : u._showClone(p), p !== d && (vt(w, Dt ? Dt.options.ghostClass : u.options.ghostClass, !1), vt(w, o.ghostClass, !0)), Dt !== p && p !== z.active ? Dt = p : p === z.active && Dt && (Dt = null), d === p && (p._ignoreWhileAnimating = i), p.animateAll(function() {
+            }), k && (c ? u._hideClone() : u._showClone(p), p !== d && (vt(M, Dt ? Dt.options.ghostClass : u.options.ghostClass, !1), vt(M, o.ghostClass, !0)), Dt !== p && p !== z.active ? Dt = p : p === z.active && Dt && (Dt = null), d === p && (p._ignoreWhileAnimating = i), p.animateAll(function() {
                 m("dragOverAnimationComplete"), p._ignoreWhileAnimating = null
-            }), p !== d && (d.animateAll(), d._ignoreWhileAnimating = null)), (i === w && !w.animated || i === n && !i.animated) && (Se = null), !o.dragoverBubble && !e.rootEl && i !== document && (w.parentNode[Rt]._isOutsideThisEl(e.target), !k && he(e)), !o.dragoverBubble && e.stopPropagation && e.stopPropagation(), h = !0
+            }), p !== d && (d.animateAll(), d._ignoreWhileAnimating = null)), (i === M && !M.animated || i === n && !i.animated) && (Se = null), !o.dragoverBubble && !e.rootEl && i !== document && (M.parentNode[Rt]._isOutsideThisEl(e.target), !k && he(e)), !o.dragoverBubble && e.stopPropagation && e.stopPropagation(), h = !0
         }
 
         function O() {
-            Ut = gt(w), se = gt(w, o.draggable), Mt({
+            Ut = gt(M), se = gt(M, o.draggable), Mt({
                 sortable: p,
                 name: "change",
                 toEl: n,
                 newIndex: Ut,
                 newDraggableIndex: se,
                 originalEvent: e
             })
         }
         if (e.preventDefault !== void 0 && e.cancelable && e.preventDefault(), i = Jt(i, o.draggable, n, !0), m("dragOver"), z.eventCanceled) return h;
-        if (w.contains(e.target) || i.animated && i.animatingX && i.animatingY || p._ignoreWhileAnimating === i) return y(!1);
-        if (fn = !1, u && !o.disabled && (f ? c || (t = ht !== ut) : Dt === this || (this.lastPutMode = Ze.checkPull(this, u, w, e)) && l.checkPut(this, u, w, e))) {
-            if (v = this._getDirection(e, i) === "vertical", r = ft(w), m("dragOverValid"), z.eventCanceled) return h;
-            if (t) return ht = ut, g(), this._hideClone(), m("revert"), z.eventCanceled || (me ? ut.insertBefore(w, me) : ut.appendChild(w)), y(!0);
+        if (M.contains(e.target) || i.animated && i.animatingX && i.animatingY || p._ignoreWhileAnimating === i) return y(!1);
+        if (fn = !1, u && !o.disabled && (c ? f || (t = ht !== ut) : Dt === this || (this.lastPutMode = Ze.checkPull(this, u, M, e)) && l.checkPut(this, u, M, e))) {
+            if (v = this._getDirection(e, i) === "vertical", r = ft(M), m("dragOverValid"), z.eventCanceled) return h;
+            if (t) return ht = ut, g(), this._hideClone(), m("revert"), z.eventCanceled || (me ? ut.insertBefore(M, me) : ut.appendChild(M)), y(!0);
             var E = Vn(n, o.draggable);
             if (!E || Di(e, v, this) && !E.animated) {
-                if (E === w) return y(!1);
-                if (E && n === e.target && (i = E), i && (s = ft(i)), _e(ut, n, w, r, i, s, e, !!i) !== !1) return g(), n.appendChild(w), ht = n, O(), y(!0)
+                if (E === M) return y(!1);
+                if (E && n === e.target && (i = E), i && (s = ft(i)), _e(ut, n, M, r, i, s, e, !!i) !== !1) return g(), n.appendChild(M), ht = n, O(), y(!0)
             } else if (E && Ci(e, v, this)) {
                 var C = Ie(n, 0, o, !0);
-                if (C === w) return y(!1);
-                if (i = C, s = ft(i), _e(ut, n, w, r, i, s, e, !1) !== !1) return g(), n.insertBefore(w, C), ht = n, O(), y(!0)
+                if (C === M) return y(!1);
+                if (i = C, s = ft(i), _e(ut, n, M, r, i, s, e, !1) !== !1) return g(), n.insertBefore(M, C), ht = n, O(), y(!0)
             } else if (i.parentNode === n) {
                 s = ft(i);
                 var T = 0,
-                    $, L = w.parentNode !== n,
-                    I = !xi(w.animated && w.toRect || r, i.animated && i.toRect || s, v),
+                    $, L = M.parentNode !== n,
+                    I = !xi(M.animated && M.toRect || r, i.animated && i.toRect || s, v),
                     j = v ? "top" : "left",
-                    P = Qn(i, "top", "top") || Qn(w, "top", "top"),
-                    M = P ? P.scrollTop : void 0;
+                    P = Qn(i, "top", "top") || Qn(M, "top", "top"),
+                    w = P ? P.scrollTop : void 0;
                 Se !== i && ($ = s[j], He = !1, ke = !I && o.invertSwap || L), T = Ai(e, i, s, v, I ? 1 : o.swapThreshold, o.invertedSwapThreshold == null ? o.swapThreshold : o.invertedSwapThreshold, ke, Se === i);
                 var D;
                 if (T !== 0) {
-                    var R = gt(w);
+                    var R = gt(M);
                     do R -= T, D = ht.children[R]; while (D && (G(D, "display") === "none" || D === q))
                 }
                 if (T === 0 || D === i) return y(!1);
                 Se = i, Ke = T;
                 var H = i.nextElementSibling,
                     F = !1;
                 F = T === 1;
-                var N = _e(ut, n, w, r, i, s, e, F);
-                if (N !== !1) return (N === 1 || N === -1) && (F = N === 1), An = !0, setTimeout(Pi, 30), g(), F && !H ? n.appendChild(w) : i.parentNode.insertBefore(w, F ? H : i), P && xr(P, 0, M - P.scrollTop), ht = w.parentNode, $ !== void 0 && !ke && (on = Math.abs($ - ft(i)[j])), O(), y(!0)
+                var N = _e(ut, n, M, r, i, s, e, F);
+                if (N !== !1) return (N === 1 || N === -1) && (F = N === 1), An = !0, setTimeout(Pi, 30), g(), F && !H ? n.appendChild(M) : i.parentNode.insertBefore(M, F ? H : i), P && xr(P, 0, w - P.scrollTop), ht = M.parentNode, $ !== void 0 && !ke && (on = Math.abs($ - ft(i)[j])), O(), y(!0)
             }
-            if (n.contains(w)) return y(!1)
+            if (n.contains(M)) return y(!1)
         }
         return !1
     },
     _ignoreWhileAnimating: null,
     _offMoveEvents: function() {
         tt(document, "mousemove", this._onTouchMove), tt(document, "touchmove", this._onTouchMove), tt(document, "pointermove", this._onTouchMove), tt(document, "dragover", he), tt(document, "mousemove", he), tt(document, "touchmove", he)
     },
     _offUpEvents: function() {
         var e = this.el.ownerDocument;
         tt(e, "mouseup", this._onDrop), tt(e, "touchend", this._onDrop), tt(e, "pointerup", this._onDrop), tt(e, "touchcancel", this._onDrop), tt(document, "selectstart", this)
     },
     _onDrop: function(e) {
         var n = this.el,
             i = this.options;
-        if (Ut = gt(w), se = gt(w, i.draggable), Ft("drop", this, {
+        if (Ut = gt(M), se = gt(M, i.draggable), Ft("drop", this, {
                 evt: e
-            }), ht = w && w.parentNode, Ut = gt(w), se = gt(w, i.draggable), z.eventCanceled) {
+            }), ht = M && M.parentNode, Ut = gt(M), se = gt(M, i.draggable), z.eventCanceled) {
             this._nulling();
             return
         }
-        xe = !1, ke = !1, He = !1, clearInterval(this._loopId), clearTimeout(this._dragStartTimer), Rn(this.cloneId), Rn(this._dragStartId), this.nativeDraggable && (tt(document, "drop", this), tt(n, "dragstart", this._onDragStart)), this._offMoveEvents(), this._offUpEvents(), Ue && G(document.body, "user-select", ""), G(w, "transform", ""), e && ($e && (e.cancelable && e.preventDefault(), !i.dropBubble && e.stopPropagation()), q && q.parentNode && q.parentNode.removeChild(q), (ut === ht || Dt && Dt.lastPutMode !== "clone") && mt && mt.parentNode && mt.parentNode.removeChild(mt), w && (this.nativeDraggable && tt(w, "dragend", this), Tn(w), w.style["will-change"] = "", $e && !xe && vt(w, Dt ? Dt.options.ghostClass : this.options.ghostClass, !1), vt(w, this.options.chosenClass, !1), Mt({
+        xe = !1, ke = !1, He = !1, clearInterval(this._loopId), clearTimeout(this._dragStartTimer), Rn(this.cloneId), Rn(this._dragStartId), this.nativeDraggable && (tt(document, "drop", this), tt(n, "dragstart", this._onDragStart)), this._offMoveEvents(), this._offUpEvents(), Ue && G(document.body, "user-select", ""), G(M, "transform", ""), e && ($e && (e.cancelable && e.preventDefault(), !i.dropBubble && e.stopPropagation()), q && q.parentNode && q.parentNode.removeChild(q), (ut === ht || Dt && Dt.lastPutMode !== "clone") && mt && mt.parentNode && mt.parentNode.removeChild(mt), M && (this.nativeDraggable && tt(M, "dragend", this), Tn(M), M.style["will-change"] = "", $e && !xe && vt(M, Dt ? Dt.options.ghostClass : this.options.ghostClass, !1), vt(M, this.options.chosenClass, !1), Mt({
             sortable: this,
             name: "unchoose",
             toEl: ht,
             newIndex: null,
             newDraggableIndex: null,
             originalEvent: e
         }), ut !== ht ? (Ut >= 0 && (Mt({
@@ -1413,27 +1413,27 @@
             sortable: this,
             name: "end",
             toEl: ht,
             originalEvent: e
         }), this.save()))), this._nulling()
     },
     _nulling: function() {
-        Ft("nulling", this), ut = w = ht = q = me = mt = rn = ue = pe = Xt = $e = Ut = se = Oe = Be = Se = Ke = Dt = Ze = z.dragged = z.ghost = z.clone = z.active = null, dn.forEach(function(e) {
+        Ft("nulling", this), ut = M = ht = q = me = mt = rn = ue = pe = Xt = $e = Ut = se = Oe = Be = Se = Ke = Dt = Ze = z.dragged = z.ghost = z.clone = z.active = null, dn.forEach(function(e) {
             e.checked = !0
         }), dn.length = En = xn = 0
     },
     handleEvent: function(e) {
         switch (e.type) {
             case "drop":
             case "dragend":
                 this._onDrop(e);
                 break;
             case "dragenter":
             case "dragover":
-                w && (this._onDragOver(e), Ii(e));
+                M && (this._onDragOver(e), Ii(e));
                 break;
             case "selectstart":
                 e.preventDefault();
                 break
         }
     },
     toArray: function() {
@@ -1479,31 +1479,31 @@
     _showClone: function(e) {
         if (e.lastPutMode !== "clone") {
             this._hideClone();
             return
         }
         if (ue) {
             if (Ft("showClone", this), z.eventCanceled) return;
-            w.parentNode == ut && !this.options.group.revertClone ? ut.insertBefore(mt, w) : me ? ut.insertBefore(mt, me) : ut.appendChild(mt), this.options.group.revertClone && this.animate(w, mt), G(mt, "display", ""), ue = !1
+            M.parentNode == ut && !this.options.group.revertClone ? ut.insertBefore(mt, M) : me ? ut.insertBefore(mt, me) : ut.appendChild(mt), this.options.group.revertClone && this.animate(M, mt), G(mt, "display", ""), ue = !1
         }
     }
 };
 
 function Ii(a) {
     a.dataTransfer && (a.dataTransfer.dropEffect = "move"), a.cancelable && a.preventDefault()
 }
 
 function _e(a, e, n, i, r, s, t, o) {
     var l, u = a[Rt],
-        f = u.options.onMove,
-        c;
+        c = u.options.onMove,
+        f;
     return window.CustomEvent && !ae && !Ye ? l = new CustomEvent("move", {
         bubbles: !0,
         cancelable: !0
-    }) : (l = document.createEvent("Event"), l.initEvent("move", !0, !0)), l.to = e, l.from = a, l.dragged = n, l.draggedRect = i, l.related = r || e, l.relatedRect = s || ft(e), l.willInsertAfter = o, l.originalEvent = t, a.dispatchEvent(l), f && (c = f.call(u, l, t)), c
+    }) : (l = document.createEvent("Event"), l.initEvent("move", !0, !0)), l.to = e, l.from = a, l.dragged = n, l.draggedRect = i, l.related = r || e, l.relatedRect = s || ft(e), l.willInsertAfter = o, l.originalEvent = t, a.dispatchEvent(l), c && (f = c.call(u, l, t)), f
 }
 
 function Tn(a) {
     a.draggable = !1
 }
 
 function Pi() {
@@ -1521,28 +1521,28 @@
         r = 10;
     return e ? a.clientX > i.right + r || a.clientX <= i.right && a.clientY > i.bottom && a.clientX >= i.left : a.clientX > i.right && a.clientY > i.top || a.clientX <= i.right && a.clientY > i.bottom + r
 }
 
 function Ai(a, e, n, i, r, s, t, o) {
     var l = i ? a.clientY : a.clientX,
         u = i ? n.height : n.width,
-        f = i ? n.top : n.left,
-        c = i ? n.bottom : n.right,
+        c = i ? n.top : n.left,
+        f = i ? n.bottom : n.right,
         d = !1;
     if (!t) {
         if (o && on < u * r) {
-            if (!He && (Ke === 1 ? l > f + u * s / 2 : l < c - u * s / 2) && (He = !0), He) d = !0;
-            else if (Ke === 1 ? l < f + on : l > c - on) return -Ke
-        } else if (l > f + u * (1 - r) / 2 && l < c - u * (1 - r) / 2) return Ri(e)
+            if (!He && (Ke === 1 ? l > c + u * s / 2 : l < f - u * s / 2) && (He = !0), He) d = !0;
+            else if (Ke === 1 ? l < c + on : l > f - on) return -Ke
+        } else if (l > c + u * (1 - r) / 2 && l < f - u * (1 - r) / 2) return Ri(e)
     }
-    return d = d || t, d && (l < f + u * s / 2 || l > c - u * s / 2) ? l > f + u / 2 ? 1 : -1 : 0
+    return d = d || t, d && (l < c + u * s / 2 || l > f - u * s / 2) ? l > c + u / 2 ? 1 : -1 : 0
 }
 
 function Ri(a) {
-    return gt(w) < gt(a) ? 1 : -1
+    return gt(M) < gt(a) ? 1 : -1
 }
 
 function wi(a) {
     for (var e = a.tagName + a.className + a.src + a.href + a.textContent, n = e.length, i = 0; n--;) i += e.charCodeAt(n);
     return i.toString(36)
 }
 
@@ -1669,17 +1669,17 @@
         if (!!e.scroll) {
             var r = (a.touches ? a.touches[0] : a).clientX,
                 s = (a.touches ? a.touches[0] : a).clientY,
                 t = e.scrollSensitivity,
                 o = e.scrollSpeed,
                 l = te(),
                 u = !1,
-                f;
-            wn !== n && (wn = n, ln(), Le = e.scroll, f = e.scrollFn, Le === !0 && (Le = fe(n, !0)));
-            var c = 0,
+                c;
+            wn !== n && (wn = n, ln(), Le = e.scroll, c = e.scrollFn, Le === !0 && (Le = fe(n, !0)));
+            var f = 0,
                 d = Le;
             do {
                 var v = d,
                     p = ft(v),
                     h = p.top,
                     m = p.bottom,
                     g = p.left,
@@ -1690,26 +1690,26 @@
                     T = void 0,
                     $ = v.scrollWidth,
                     L = v.scrollHeight,
                     I = G(v),
                     j = v.scrollLeft,
                     P = v.scrollTop;
                 v === l ? (C = O < $ && (I.overflowX === "auto" || I.overflowX === "scroll" || I.overflowX === "visible"), T = E < L && (I.overflowY === "auto" || I.overflowY === "scroll" || I.overflowY === "visible")) : (C = O < $ && (I.overflowX === "auto" || I.overflowX === "scroll"), T = E < L && (I.overflowY === "auto" || I.overflowY === "scroll"));
-                var M = C && (Math.abs(y - r) <= t && j + O < $) - (Math.abs(g - r) <= t && !!j),
+                var w = C && (Math.abs(y - r) <= t && j + O < $) - (Math.abs(g - r) <= t && !!j),
                     D = T && (Math.abs(m - s) <= t && P + E < L) - (Math.abs(h - s) <= t && !!P);
-                if (!xt[c])
-                    for (var R = 0; R <= c; R++) xt[R] || (xt[R] = {});
-                (xt[c].vx != M || xt[c].vy != D || xt[c].el !== v) && (xt[c].el = v, xt[c].vx = M, xt[c].vy = D, clearInterval(xt[c].pid), (M != 0 || D != 0) && (u = !0, xt[c].pid = setInterval(function() {
+                if (!xt[f])
+                    for (var R = 0; R <= f; R++) xt[R] || (xt[R] = {});
+                (xt[f].vx != w || xt[f].vy != D || xt[f].el !== v) && (xt[f].el = v, xt[f].vx = w, xt[f].vy = D, clearInterval(xt[f].pid), (w != 0 || D != 0) && (u = !0, xt[f].pid = setInterval(function() {
                     i && this.layer === 0 && z.active._onTouchMove(vn);
                     var H = xt[this.layer].vy ? xt[this.layer].vy * o : 0,
                         F = xt[this.layer].vx ? xt[this.layer].vx * o : 0;
-                    typeof f == "function" && f.call(z.dragged.parentNode[Rt], F, H, a, vn, xt[this.layer].el) !== "continue" || xr(xt[this.layer].el, F, H)
+                    typeof c == "function" && c.call(z.dragged.parentNode[Rt], F, H, a, vn, xt[this.layer].el) !== "continue" || xr(xt[this.layer].el, F, H)
                 }.bind({
-                    layer: c
-                }), 24))), c++
+                    layer: f
+                }), 24))), f++
             } while (e.bubbleScroll && d !== l && (d = fe(d, !1)));
             Mn = u
         }
     }, 30),
     Dr = function(e) {
         var n = e.originalEvent,
             i = e.putSortable,
@@ -1717,17 +1717,17 @@
             s = e.activeSortable,
             t = e.dispatchSortableEvent,
             o = e.hideGhostForTarget,
             l = e.unhideGhostForTarget;
         if (!!n) {
             var u = i || s;
             o();
-            var f = n.changedTouches && n.changedTouches.length ? n.changedTouches[0] : n,
-                c = document.elementFromPoint(f.clientX, f.clientY);
-            l(), u && !u.el.contains(c) && (t("spill"), this.onSpill({
+            var c = n.changedTouches && n.changedTouches.length ? n.changedTouches[0] : n,
+                f = document.elementFromPoint(c.clientX, c.clientY);
+            l(), u && !u.el.contains(f) && (t("spill"), this.onSpill({
                 dragEl: r,
                 putSortable: i
             }))
         }
     };
 
 function Gn() {}
@@ -1781,18 +1781,18 @@
                 r = n.target,
                 s = n.onMove,
                 t = n.activeSortable,
                 o = n.changed,
                 l = n.cancel;
             if (!!t.options.swap) {
                 var u = this.sortable.el,
-                    f = this.options;
+                    c = this.options;
                 if (r && r !== u) {
-                    var c = Kt;
-                    s(r) !== !1 ? (vt(r, f.swapClass, !0), Kt = r) : Kt = null, c && c !== Kt && vt(c, f.swapClass, !1)
+                    var f = Kt;
+                    s(r) !== !1 ? (vt(r, c.swapClass, !0), Kt = r) : Kt = null, f && f !== Kt && vt(f, c.swapClass, !1)
                 }
                 o(), i(!0), l()
             }
         },
         drop: function(n) {
             var i = n.activeSortable,
                 r = n.putSortable,
@@ -1934,23 +1934,23 @@
                 s = n.insertion,
                 t = n.activeSortable,
                 o = n.parentEl,
                 l = n.putSortable,
                 u = this.options;
             if (s) {
                 if (r && t._hideClone(), Ne = !1, u.animation && Z.length > 1 && ($t || !r && !t.options.sort && !l)) {
-                    var f = ft(lt, !1, !0, !0);
+                    var c = ft(lt, !1, !0, !0);
                     Z.forEach(function(d) {
-                        d !== lt && (kn(d, f), o.appendChild(d))
+                        d !== lt && (kn(d, c), o.appendChild(d))
                     }), $t = !0
                 }
                 if (!r)
                     if ($t || en(), Z.length > 1) {
-                        var c = tn;
-                        t._showClone(i), t.options.animation && !tn && c && Vt.forEach(function(d) {
+                        var f = tn;
+                        t._showClone(i), t.options.animation && !tn && f && Vt.forEach(function(d) {
                             t.addAnimationState({
                                 target: d,
                                 rect: je
                             }), d.fromRect = je, d.thisAnimationDuration = null
                         })
                     } else t._showClone(i)
             }
@@ -1974,20 +1974,20 @@
             var i = n.originalEvent,
                 r = n.rootEl,
                 s = n.parentEl,
                 t = n.sortable,
                 o = n.dispatchSortableEvent,
                 l = n.oldIndex,
                 u = n.putSortable,
-                f = u || this.sortable;
+                c = u || this.sortable;
             if (!!i) {
-                var c = this.options,
+                var f = this.options,
                     d = s.children;
                 if (!Ee)
-                    if (c.multiDragKey && !this.multiDragKeyDown && this._deselectMultiDrag(), vt(lt, c.selectedClass, !~Z.indexOf(lt)), ~Z.indexOf(lt)) Z.splice(Z.indexOf(lt), 1), Me = null, Fe({
+                    if (f.multiDragKey && !this.multiDragKeyDown && this._deselectMultiDrag(), vt(lt, f.selectedClass, !~Z.indexOf(lt)), ~Z.indexOf(lt)) Z.splice(Z.indexOf(lt), 1), Me = null, Fe({
                         sortable: t,
                         rootEl: r,
                         name: "deselect",
                         targetEl: lt,
                         originalEvt: i
                     });
                     else {
@@ -1998,32 +1998,32 @@
                                 targetEl: lt,
                                 originalEvt: i
                             }), i.shiftKey && Me && t.el.contains(Me)) {
                             var v = gt(Me),
                                 p = gt(lt);
                             if (~v && ~p && v !== p) {
                                 var h, m;
-                                for (p > v ? (m = v, h = p) : (m = p, h = v + 1); m < h; m++) ~Z.indexOf(d[m]) || (vt(d[m], c.selectedClass, !0), Z.push(d[m]), Fe({
+                                for (p > v ? (m = v, h = p) : (m = p, h = v + 1); m < h; m++) ~Z.indexOf(d[m]) || (vt(d[m], f.selectedClass, !0), Z.push(d[m]), Fe({
                                     sortable: t,
                                     rootEl: r,
                                     name: "select",
                                     targetEl: d[m],
                                     originalEvt: i
                                 }))
                             }
                         } else Me = lt;
-                        Yt = f
+                        Yt = c
                     } if (Ee && this.isMultiDrag) {
                     if ($t = !1, (s[Rt].options.sort || s !== r) && Z.length > 1) {
                         var g = ft(lt),
                             y = gt(lt, ":not(." + this.options.selectedClass + ")");
-                        if (!Ne && c.animation && (lt.thisAnimationDuration = null), f.captureAnimationState(), !Ne && (c.animation && (lt.fromRect = g, Z.forEach(function(E) {
+                        if (!Ne && f.animation && (lt.thisAnimationDuration = null), c.captureAnimationState(), !Ne && (f.animation && (lt.fromRect = g, Z.forEach(function(E) {
                                 if (E.thisAnimationDuration = null, E !== lt) {
                                     var C = $t ? ft(E) : g;
-                                    E.fromRect = C, f.addAnimationState({
+                                    E.fromRect = C, c.addAnimationState({
                                         target: E,
                                         rect: C
                                     })
                                 }
                             })), en(), Z.forEach(function(E) {
                                 d[y] ? s.insertBefore(E, d[y]) : s.appendChild(E), y++
                             }), l === gt(lt))) {
@@ -2033,17 +2033,17 @@
                                     O = !0;
                                     return
                                 }
                             }), O && o("update")
                         }
                         Z.forEach(function(E) {
                             bn(E)
-                        }), f.animateAll()
+                        }), c.animateAll()
                     }
-                    Yt = f
+                    Yt = c
                 }(r === s || u && u.lastPutMode !== "clone") && Vt.forEach(function(E) {
                     E.parentNode && E.parentNode.removeChild(E)
                 })
             }
         },
         nullingGlobal: function() {
             this.isMultiDrag = Ee = !1, Vt.length = 0
@@ -2173,17 +2173,17 @@
             }, t.t = function(o, l) {
                 if (l & 1 && (o = t(o)), l & 8 || l & 4 && typeof o == "object" && o && o.__esModule) return o;
                 var u = Object.create(null);
                 if (t.r(u), Object.defineProperty(u, "default", {
                         enumerable: !0,
                         value: o
                     }), l & 2 && typeof o != "string")
-                    for (var f in o) t.d(u, f, function(c) {
-                        return o[c]
-                    }.bind(null, f));
+                    for (var c in o) t.d(u, c, function(f) {
+                        return o[f]
+                    }.bind(null, c));
                 return u
             }, t.n = function(o) {
                 var l = o && o.__esModule ? function() {
                     return o.default
                 } : function() {
                     return o
                 };
@@ -2196,66 +2196,66 @@
                 var o = t("b622"),
                     l = o("toStringTag"),
                     u = {};
                 u[l] = "z", r.exports = String(u) === "[object z]"
             },
             "0366": function(r, s, t) {
                 var o = t("1c0b");
-                r.exports = function(l, u, f) {
+                r.exports = function(l, u, c) {
                     if (o(l), u === void 0) return l;
-                    switch (f) {
+                    switch (c) {
                         case 0:
                             return function() {
                                 return l.call(u)
                             };
                         case 1:
-                            return function(c) {
-                                return l.call(u, c)
+                            return function(f) {
+                                return l.call(u, f)
                             };
                         case 2:
-                            return function(c, d) {
-                                return l.call(u, c, d)
+                            return function(f, d) {
+                                return l.call(u, f, d)
                             };
                         case 3:
-                            return function(c, d, v) {
-                                return l.call(u, c, d, v)
+                            return function(f, d, v) {
+                                return l.call(u, f, d, v)
                             }
                     }
                     return function() {
                         return l.apply(u, arguments)
                     }
                 }
             },
             "057f": function(r, s, t) {
                 var o = t("fc6a"),
                     l = t("241c").f,
                     u = {}.toString,
-                    f = typeof window == "object" && window && Object.getOwnPropertyNames ? Object.getOwnPropertyNames(window) : [],
-                    c = function(d) {
+                    c = typeof window == "object" && window && Object.getOwnPropertyNames ? Object.getOwnPropertyNames(window) : [],
+                    f = function(d) {
                         try {
                             return l(d)
                         } catch {
-                            return f.slice()
+                            return c.slice()
                         }
                     };
                 r.exports.f = function(v) {
-                    return f && u.call(v) == "[object Window]" ? c(v) : l(o(v))
+                    return c && u.call(v) == "[object Window]" ? f(v) : l(o(v))
                 }
             },
             "06cf": function(r, s, t) {
                 var o = t("83ab"),
                     l = t("d1e7"),
                     u = t("5c6c"),
-                    f = t("fc6a"),
-                    c = t("c04e"),
+                    c = t("fc6a"),
+                    f = t("c04e"),
                     d = t("5135"),
                     v = t("0cfb"),
                     p = Object.getOwnPropertyDescriptor;
                 s.f = o ? p : function(m, g) {
-                    if (m = f(m), g = c(g, !0), v) try {
+                    if (m = c(m), g = f(g, !0), v) try {
                         return p(m, g)
                     } catch {}
                     if (d(m, g)) return u(!l.f.call(m, g), m[g])
                 }
             },
             "0cfb": function(r, s, t) {
                 var o = t("83ab"),
@@ -2269,65 +2269,65 @@
                     }).a != 7
                 })
             },
             "13d5": function(r, s, t) {
                 var o = t("23e7"),
                     l = t("d58f").left,
                     u = t("a640"),
-                    f = t("ae40"),
-                    c = u("reduce"),
-                    d = f("reduce", {
+                    c = t("ae40"),
+                    f = u("reduce"),
+                    d = c("reduce", {
                         1: 0
                     });
                 o({
                     target: "Array",
                     proto: !0,
-                    forced: !c || !d
+                    forced: !f || !d
                 }, {
                     reduce: function(p) {
                         return l(this, p, arguments.length, arguments.length > 1 ? arguments[1] : void 0)
                     }
                 })
             },
             "14c3": function(r, s, t) {
                 var o = t("c6b6"),
                     l = t("9263");
-                r.exports = function(u, f) {
-                    var c = u.exec;
-                    if (typeof c == "function") {
-                        var d = c.call(u, f);
+                r.exports = function(u, c) {
+                    var f = u.exec;
+                    if (typeof f == "function") {
+                        var d = f.call(u, c);
                         if (typeof d != "object") throw TypeError("RegExp exec method returned something other than an Object or null");
                         return d
                     }
                     if (o(u) !== "RegExp") throw TypeError("RegExp#exec called on incompatible receiver");
-                    return l.call(u, f)
+                    return l.call(u, c)
                 }
             },
             "159b": function(r, s, t) {
                 var o = t("da84"),
                     l = t("fdbc"),
                     u = t("17c2"),
-                    f = t("9112");
-                for (var c in l) {
-                    var d = o[c],
+                    c = t("9112");
+                for (var f in l) {
+                    var d = o[f],
                         v = d && d.prototype;
                     if (v && v.forEach !== u) try {
-                        f(v, "forEach", u)
+                        c(v, "forEach", u)
                     } catch {
                         v.forEach = u
                     }
                 }
             },
             "17c2": function(r, s, t) {
                 var o = t("b727").forEach,
                     l = t("a640"),
                     u = t("ae40"),
-                    f = l("forEach"),
-                    c = u("forEach");
-                r.exports = !f || !c ? function(v) {
+                    c = l("forEach"),
+                    f = u("forEach");
+                r.exports = !c || !f ? function(v) {
                     return o(this, v, arguments.length > 1 ? arguments[1] : void 0)
                 } : [].forEach
             },
             "1be4": function(r, s, t) {
                 var o = t("d066");
                 r.exports = o("document", "documentElement")
             },
@@ -2338,28 +2338,28 @@
                 }
             },
             "1c7e": function(r, s, t) {
                 var o = t("b622"),
                     l = o("iterator"),
                     u = !1;
                 try {
-                    var f = 0,
-                        c = {
+                    var c = 0,
+                        f = {
                             next: function() {
                                 return {
-                                    done: !!f++
+                                    done: !!c++
                                 }
                             },
                             return: function() {
                                 u = !0
                             }
                         };
-                    c[l] = function() {
+                    f[l] = function() {
                         return this
-                    }, Array.from(c, function() {
+                    }, Array.from(f, function() {
                         throw 2
                     })
                 } catch {}
                 r.exports = function(d, v) {
                     if (!v && !u) return !1;
                     var p = !1;
                     try {
@@ -2383,97 +2383,97 @@
                     return t
                 }
             },
             "1dde": function(r, s, t) {
                 var o = t("d039"),
                     l = t("b622"),
                     u = t("2d00"),
-                    f = l("species");
-                r.exports = function(c) {
+                    c = l("species");
+                r.exports = function(f) {
                     return u >= 51 || !o(function() {
                         var d = [],
                             v = d.constructor = {};
-                        return v[f] = function() {
+                        return v[c] = function() {
                             return {
                                 foo: 1
                             }
-                        }, d[c](Boolean).foo !== 1
+                        }, d[f](Boolean).foo !== 1
                     })
                 }
             },
             "23cb": function(r, s, t) {
                 var o = t("a691"),
                     l = Math.max,
                     u = Math.min;
-                r.exports = function(f, c) {
-                    var d = o(f);
-                    return d < 0 ? l(d + c, 0) : u(d, c)
+                r.exports = function(c, f) {
+                    var d = o(c);
+                    return d < 0 ? l(d + f, 0) : u(d, f)
                 }
             },
             "23e7": function(r, s, t) {
                 var o = t("da84"),
                     l = t("06cf").f,
                     u = t("9112"),
-                    f = t("6eeb"),
-                    c = t("ce4e"),
+                    c = t("6eeb"),
+                    f = t("ce4e"),
                     d = t("e893"),
                     v = t("94ca");
                 r.exports = function(p, h) {
                     var m = p.target,
                         g = p.global,
                         y = p.stat,
                         O, E, C, T, $, L;
-                    if (g ? E = o : y ? E = o[m] || c(m, {}) : E = (o[m] || {}).prototype, E)
+                    if (g ? E = o : y ? E = o[m] || f(m, {}) : E = (o[m] || {}).prototype, E)
                         for (C in h) {
                             if ($ = h[C], p.noTargetGet ? (L = l(E, C), T = L && L.value) : T = E[C], O = v(g ? C : m + (y ? "." : "#") + C, p.forced), !O && T !== void 0) {
                                 if (typeof $ == typeof T) continue;
                                 d($, T)
-                            }(p.sham || T && T.sham) && u($, "sham", !0), f(E, C, $, p)
+                            }(p.sham || T && T.sham) && u($, "sham", !0), c(E, C, $, p)
                         }
                 }
             },
             "241c": function(r, s, t) {
                 var o = t("ca84"),
                     l = t("7839"),
                     u = l.concat("length", "prototype");
-                s.f = Object.getOwnPropertyNames || function(c) {
-                    return o(c, u)
+                s.f = Object.getOwnPropertyNames || function(f) {
+                    return o(f, u)
                 }
             },
             "25f0": function(r, s, t) {
                 var o = t("6eeb"),
                     l = t("825a"),
                     u = t("d039"),
-                    f = t("ad6d"),
-                    c = "toString",
+                    c = t("ad6d"),
+                    f = "toString",
                     d = RegExp.prototype,
-                    v = d[c],
+                    v = d[f],
                     p = u(function() {
                         return v.call({
                             source: "a",
                             flags: "b"
                         }) != "/a/b"
                     }),
-                    h = v.name != c;
-                (p || h) && o(RegExp.prototype, c, function() {
+                    h = v.name != f;
+                (p || h) && o(RegExp.prototype, f, function() {
                     var g = l(this),
                         y = String(g.source),
                         O = g.flags,
-                        E = String(O === void 0 && g instanceof RegExp && !("flags" in d) ? f.call(g) : O);
+                        E = String(O === void 0 && g instanceof RegExp && !("flags" in d) ? c.call(g) : O);
                     return "/" + y + "/" + E
                 }, {
                     unsafe: !0
                 })
             },
             "2ca0": function(r, s, t) {
                 var o = t("23e7"),
                     l = t("06cf").f,
                     u = t("50c4"),
-                    f = t("5a34"),
-                    c = t("1d80"),
+                    c = t("5a34"),
+                    f = t("1d80"),
                     d = t("ab13"),
                     v = t("c430"),
                     p = "".startsWith,
                     h = Math.min,
                     m = d("startsWith"),
                     g = !v && !m && !! function() {
                         var y = l(String.prototype, "startsWith");
@@ -2481,72 +2481,72 @@
                     }();
                 o({
                     target: "String",
                     proto: !0,
                     forced: !g && !m
                 }, {
                     startsWith: function(O) {
-                        var E = String(c(this));
-                        f(O);
+                        var E = String(f(this));
+                        c(O);
                         var C = u(h(arguments.length > 1 ? arguments[1] : void 0, E.length)),
                             T = String(O);
                         return p ? p.call(E, T, C) : E.slice(C, C + T.length) === T
                     }
                 })
             },
             "2d00": function(r, s, t) {
                 var o = t("da84"),
                     l = t("342f"),
                     u = o.process,
-                    f = u && u.versions,
-                    c = f && f.v8,
+                    c = u && u.versions,
+                    f = c && c.v8,
                     d, v;
-                c ? (d = c.split("."), v = d[0] + d[1]) : l && (d = l.match(/Edge\/(\d+)/), (!d || d[1] >= 74) && (d = l.match(/Chrome\/(\d+)/), d && (v = d[1]))), r.exports = v && +v
+                f ? (d = f.split("."), v = d[0] + d[1]) : l && (d = l.match(/Edge\/(\d+)/), (!d || d[1] >= 74) && (d = l.match(/Chrome\/(\d+)/), d && (v = d[1]))), r.exports = v && +v
             },
             "342f": function(r, s, t) {
                 var o = t("d066");
                 r.exports = o("navigator", "userAgent") || ""
             },
             "35a1": function(r, s, t) {
                 var o = t("f5df"),
                     l = t("3f8c"),
                     u = t("b622"),
-                    f = u("iterator");
-                r.exports = function(c) {
-                    if (c != null) return c[f] || c["@@iterator"] || l[o(c)]
+                    c = u("iterator");
+                r.exports = function(f) {
+                    if (f != null) return f[c] || f["@@iterator"] || l[o(f)]
                 }
             },
             "37e8": function(r, s, t) {
                 var o = t("83ab"),
                     l = t("9bf2"),
                     u = t("825a"),
-                    f = t("df75");
+                    c = t("df75");
                 r.exports = o ? Object.defineProperties : function(d, v) {
                     u(d);
-                    for (var p = f(v), h = p.length, m = 0, g; h > m;) l.f(d, g = p[m++], v[g]);
+                    for (var p = c(v), h = p.length, m = 0, g; h > m;) l.f(d, g = p[m++], v[g]);
                     return d
                 }
             },
             "3bbe": function(r, s, t) {
                 var o = t("861d");
                 r.exports = function(l) {
                     if (!o(l) && l !== null) throw TypeError("Can't set " + String(l) + " as a prototype");
                     return l
                 }
             },
             "3ca3": function(r, s, t) {
                 var o = t("6547").charAt,
                     l = t("69f3"),
                     u = t("7dd0"),
-                    f = "String Iterator",
-                    c = l.set,
-                    d = l.getterFor(f);
+                    c = "String Iterator",
+                    f = l.set,
+                    d = l.getterFor(c);
                 u(String, "String", function(v) {
-                    c(this, {
-                        type: f,
+                    f(this, {
+                        type: c,
                         string: String(v),
                         index: 0
                     })
                 }, function() {
                     var p = d(this),
                         h = p.string,
                         m = p.index,
@@ -2580,121 +2580,121 @@
             },
             "44ad": function(r, s, t) {
                 var o = t("d039"),
                     l = t("c6b6"),
                     u = "".split;
                 r.exports = o(function() {
                     return !Object("z").propertyIsEnumerable(0)
-                }) ? function(f) {
-                    return l(f) == "String" ? u.call(f, "") : Object(f)
+                }) ? function(c) {
+                    return l(c) == "String" ? u.call(c, "") : Object(c)
                 } : Object
             },
             "44d2": function(r, s, t) {
                 var o = t("b622"),
                     l = t("7c73"),
                     u = t("9bf2"),
-                    f = o("unscopables"),
-                    c = Array.prototype;
-                c[f] == null && u.f(c, f, {
+                    c = o("unscopables"),
+                    f = Array.prototype;
+                f[c] == null && u.f(f, c, {
                     configurable: !0,
                     value: l(null)
                 }), r.exports = function(d) {
-                    c[f][d] = !0
+                    f[c][d] = !0
                 }
             },
             "44e7": function(r, s, t) {
                 var o = t("861d"),
                     l = t("c6b6"),
                     u = t("b622"),
-                    f = u("match");
-                r.exports = function(c) {
+                    c = u("match");
+                r.exports = function(f) {
                     var d;
-                    return o(c) && ((d = c[f]) !== void 0 ? !!d : l(c) == "RegExp")
+                    return o(f) && ((d = f[c]) !== void 0 ? !!d : l(f) == "RegExp")
                 }
             },
             4930: function(r, s, t) {
                 var o = t("d039");
                 r.exports = !!Object.getOwnPropertySymbols && !o(function() {
                     return !String(Symbol())
                 })
             },
             "4d64": function(r, s, t) {
                 var o = t("fc6a"),
                     l = t("50c4"),
                     u = t("23cb"),
-                    f = function(c) {
+                    c = function(f) {
                         return function(d, v, p) {
                             var h = o(d),
                                 m = l(h.length),
                                 g = u(p, m),
                                 y;
-                            if (c && v != v) {
+                            if (f && v != v) {
                                 for (; m > g;)
                                     if (y = h[g++], y != y) return !0
                             } else
                                 for (; m > g; g++)
-                                    if ((c || g in h) && h[g] === v) return c || g || 0;
-                            return !c && -1
+                                    if ((f || g in h) && h[g] === v) return f || g || 0;
+                            return !f && -1
                         }
                     };
                 r.exports = {
-                    includes: f(!0),
-                    indexOf: f(!1)
+                    includes: c(!0),
+                    indexOf: c(!1)
                 }
             },
             "4de4": function(r, s, t) {
                 var o = t("23e7"),
                     l = t("b727").filter,
                     u = t("1dde"),
-                    f = t("ae40"),
-                    c = u("filter"),
-                    d = f("filter");
+                    c = t("ae40"),
+                    f = u("filter"),
+                    d = c("filter");
                 o({
                     target: "Array",
                     proto: !0,
-                    forced: !c || !d
+                    forced: !f || !d
                 }, {
                     filter: function(p) {
                         return l(this, p, arguments.length > 1 ? arguments[1] : void 0)
                     }
                 })
             },
             "4df4": function(r, s, t) {
                 var o = t("0366"),
                     l = t("7b0b"),
                     u = t("9bdd"),
-                    f = t("e95a"),
-                    c = t("50c4"),
+                    c = t("e95a"),
+                    f = t("50c4"),
                     d = t("8418"),
                     v = t("35a1");
                 r.exports = function(h) {
                     var m = l(h),
                         g = typeof this == "function" ? this : Array,
                         y = arguments.length,
                         O = y > 1 ? arguments[1] : void 0,
                         E = O !== void 0,
                         C = v(m),
                         T = 0,
-                        $, L, I, j, P, M;
-                    if (E && (O = o(O, y > 2 ? arguments[2] : void 0, 2)), C != null && !(g == Array && f(C)))
-                        for (j = C.call(m), P = j.next, L = new g; !(I = P.call(j)).done; T++) M = E ? u(j, O, [I.value, T], !0) : I.value, d(L, T, M);
+                        $, L, I, j, P, w;
+                    if (E && (O = o(O, y > 2 ? arguments[2] : void 0, 2)), C != null && !(g == Array && c(C)))
+                        for (j = C.call(m), P = j.next, L = new g; !(I = P.call(j)).done; T++) w = E ? u(j, O, [I.value, T], !0) : I.value, d(L, T, w);
                     else
-                        for ($ = c(m.length), L = new g($); $ > T; T++) M = E ? O(m[T], T) : m[T], d(L, T, M);
+                        for ($ = f(m.length), L = new g($); $ > T; T++) w = E ? O(m[T], T) : m[T], d(L, T, w);
                     return L.length = T, L
                 }
             },
             "4fad": function(r, s, t) {
                 var o = t("23e7"),
                     l = t("6f53").entries;
                 o({
                     target: "Object",
                     stat: !0
                 }, {
-                    entries: function(f) {
-                        return l(f)
+                    entries: function(c) {
+                        return l(c)
                     }
                 })
             },
             "50c4": function(r, s, t) {
                 var o = t("a691"),
                     l = Math.min;
                 r.exports = function(u) {
@@ -2707,16 +2707,16 @@
                     return t.call(o, l)
                 }
             },
             5319: function(r, s, t) {
                 var o = t("d784"),
                     l = t("825a"),
                     u = t("7b0b"),
-                    f = t("50c4"),
-                    c = t("a691"),
+                    c = t("50c4"),
+                    f = t("a691"),
                     d = t("1d80"),
                     v = t("8aa5"),
                     p = t("14c3"),
                     h = Math.max,
                     m = Math.min,
                     g = Math.floor,
                     y = /\$([$&'`]|\d\d?|<[^>]*>)/g,
@@ -2746,31 +2746,31 @@
                             var St = F.unicode;
                             F.lastIndex = 0
                         }
                         for (var ct = [];;) {
                             var pt = p(F, N);
                             if (pt === null || (ct.push(pt), !ot)) break;
                             var Ot = String(pt[0]);
-                            Ot === "" && (F.lastIndex = v(N, f(F.lastIndex), St))
+                            Ot === "" && (F.lastIndex = v(N, c(F.lastIndex), St))
                         }
                         for (var It = "", Et = 0, st = 0; st < ct.length; st++) {
                             pt = ct[st];
-                            for (var dt = String(pt[0]), Lt = h(m(c(pt.index), N.length), 0), wt = [], re = 1; re < pt.length; re++) wt.push(E(pt[re]));
+                            for (var dt = String(pt[0]), Lt = h(m(f(pt.index), N.length), 0), wt = [], re = 1; re < pt.length; re++) wt.push(E(pt[re]));
                             var de = pt.groups;
                             if (k) {
                                 var ie = [dt].concat(wt, Lt, N);
                                 de !== void 0 && ie.push(de);
                                 var Pt = String(R.apply(void 0, ie))
-                            } else Pt = M(dt, N, Lt, wt, de, R);
+                            } else Pt = w(dt, N, Lt, wt, de, R);
                             Lt >= Et && (It += N.slice(Et, Lt) + Pt, Et = Lt + dt.length)
                         }
                         return It + N.slice(Et)
                     }];
 
-                    function M(D, R, H, F, N, k) {
+                    function w(D, R, H, F, N, k) {
                         var ot = H + D.length,
                             St = F.length,
                             ct = O;
                         return N !== void 0 && (N = u(N), ct = y), T.call(k, ct, function(pt, Ot) {
                             var It;
                             switch (Ot.charAt(0)) {
                                 case "$":
@@ -2797,29 +2797,29 @@
                         })
                     }
                 })
             },
             5692: function(r, s, t) {
                 var o = t("c430"),
                     l = t("c6cd");
-                (r.exports = function(u, f) {
-                    return l[u] || (l[u] = f !== void 0 ? f : {})
+                (r.exports = function(u, c) {
+                    return l[u] || (l[u] = c !== void 0 ? c : {})
                 })("versions", []).push({
                     version: "3.6.5",
                     mode: o ? "pure" : "global",
                     copyright: "\xA9 2020 Denis Pushkarev (zloirock.ru)"
                 })
             },
             "56ef": function(r, s, t) {
                 var o = t("d066"),
                     l = t("241c"),
                     u = t("7418"),
-                    f = t("825a");
+                    c = t("825a");
                 r.exports = o("Reflect", "ownKeys") || function(d) {
-                    var v = l.f(f(d)),
+                    var v = l.f(c(d)),
                         p = u.f;
                     return p ? v.concat(p(d)) : v
                 }
             },
             "5a34": function(r, s, t) {
                 var o = t("44e7");
                 r.exports = function(l) {
@@ -2837,62 +2837,62 @@
                     }
                 }
             },
             "5db7": function(r, s, t) {
                 var o = t("23e7"),
                     l = t("a2bf"),
                     u = t("7b0b"),
-                    f = t("50c4"),
-                    c = t("1c0b"),
+                    c = t("50c4"),
+                    f = t("1c0b"),
                     d = t("65f0");
                 o({
                     target: "Array",
                     proto: !0
                 }, {
                     flatMap: function(p) {
                         var h = u(this),
-                            m = f(h.length),
+                            m = c(h.length),
                             g;
-                        return c(p), g = d(h, 0), g.length = l(g, h, h, m, 0, 1, p, arguments.length > 1 ? arguments[1] : void 0), g
+                        return f(p), g = d(h, 0), g.length = l(g, h, h, m, 0, 1, p, arguments.length > 1 ? arguments[1] : void 0), g
                     }
                 })
             },
             6547: function(r, s, t) {
                 var o = t("a691"),
                     l = t("1d80"),
-                    u = function(f) {
-                        return function(c, d) {
-                            var v = String(l(c)),
+                    u = function(c) {
+                        return function(f, d) {
+                            var v = String(l(f)),
                                 p = o(d),
                                 h = v.length,
                                 m, g;
-                            return p < 0 || p >= h ? f ? "" : void 0 : (m = v.charCodeAt(p), m < 55296 || m > 56319 || p + 1 === h || (g = v.charCodeAt(p + 1)) < 56320 || g > 57343 ? f ? v.charAt(p) : m : f ? v.slice(p, p + 2) : (m - 55296 << 10) + (g - 56320) + 65536)
+                            return p < 0 || p >= h ? c ? "" : void 0 : (m = v.charCodeAt(p), m < 55296 || m > 56319 || p + 1 === h || (g = v.charCodeAt(p + 1)) < 56320 || g > 57343 ? c ? v.charAt(p) : m : c ? v.slice(p, p + 2) : (m - 55296 << 10) + (g - 56320) + 65536)
                         }
                     };
                 r.exports = {
                     codeAt: u(!1),
                     charAt: u(!0)
                 }
             },
             "65f0": function(r, s, t) {
                 var o = t("861d"),
                     l = t("e8b5"),
                     u = t("b622"),
-                    f = u("species");
-                r.exports = function(c, d) {
+                    c = u("species");
+                r.exports = function(f, d) {
                     var v;
-                    return l(c) && (v = c.constructor, typeof v == "function" && (v === Array || l(v.prototype)) ? v = void 0 : o(v) && (v = v[f], v === null && (v = void 0))), new(v === void 0 ? Array : v)(d === 0 ? 0 : d)
+                    return l(f) && (v = f.constructor, typeof v == "function" && (v === Array || l(v.prototype)) ? v = void 0 : o(v) && (v = v[c], v === null && (v = void 0))), new(v === void 0 ? Array : v)(d === 0 ? 0 : d)
                 }
             },
             "69f3": function(r, s, t) {
                 var o = t("7f9a"),
                     l = t("da84"),
                     u = t("861d"),
-                    f = t("9112"),
-                    c = t("5135"),
+                    c = t("9112"),
+                    f = t("5135"),
                     d = t("f772"),
                     v = t("d012"),
                     p = l.WeakMap,
                     h, m, g, y = function(I) {
                         return g(I) ? m(I) : h(I, {})
                     },
                     O = function(I) {
@@ -2913,84 +2913,84 @@
                         return C.call(E, I) || {}
                     }, g = function(I) {
                         return T.call(E, I)
                     }
                 } else {
                     var L = d("state");
                     v[L] = !0, h = function(I, j) {
-                        return f(I, L, j), j
+                        return c(I, L, j), j
                     }, m = function(I) {
-                        return c(I, L) ? I[L] : {}
+                        return f(I, L) ? I[L] : {}
                     }, g = function(I) {
-                        return c(I, L)
+                        return f(I, L)
                     }
                 }
                 r.exports = {
                     set: h,
                     get: m,
                     has: g,
                     enforce: y,
                     getterFor: O
                 }
             },
             "6eeb": function(r, s, t) {
                 var o = t("da84"),
                     l = t("9112"),
                     u = t("5135"),
-                    f = t("ce4e"),
-                    c = t("8925"),
+                    c = t("ce4e"),
+                    f = t("8925"),
                     d = t("69f3"),
                     v = d.get,
                     p = d.enforce,
                     h = String(String).split("String");
                 (r.exports = function(m, g, y, O) {
                     var E = O ? !!O.unsafe : !1,
                         C = O ? !!O.enumerable : !1,
                         T = O ? !!O.noTargetGet : !1;
                     if (typeof y == "function" && (typeof g == "string" && !u(y, "name") && l(y, "name", g), p(y).source = h.join(typeof g == "string" ? g : "")), m === o) {
-                        C ? m[g] = y : f(g, y);
+                        C ? m[g] = y : c(g, y);
                         return
                     } else E ? !T && m[g] && (C = !0) : delete m[g];
                     C ? m[g] = y : l(m, g, y)
                 })(Function.prototype, "toString", function() {
-                    return typeof this == "function" && v(this).source || c(this)
+                    return typeof this == "function" && v(this).source || f(this)
                 })
             },
             "6f53": function(r, s, t) {
                 var o = t("83ab"),
                     l = t("df75"),
                     u = t("fc6a"),
-                    f = t("d1e7").f,
-                    c = function(d) {
+                    c = t("d1e7").f,
+                    f = function(d) {
                         return function(v) {
-                            for (var p = u(v), h = l(p), m = h.length, g = 0, y = [], O; m > g;) O = h[g++], (!o || f.call(p, O)) && y.push(d ? [O, p[O]] : p[O]);
+                            for (var p = u(v), h = l(p), m = h.length, g = 0, y = [], O; m > g;) O = h[g++], (!o || c.call(p, O)) && y.push(d ? [O, p[O]] : p[O]);
                             return y
                         }
                     };
                 r.exports = {
-                    entries: c(!0),
-                    values: c(!1)
+                    entries: f(!0),
+                    values: f(!1)
                 }
             },
             "73d9": function(r, s, t) {
                 var o = t("44d2");
                 o("flatMap")
             },
             7418: function(r, s) {
                 s.f = Object.getOwnPropertySymbols
             },
             "746f": function(r, s, t) {
                 var o = t("428f"),
                     l = t("5135"),
                     u = t("e538"),
-                    f = t("9bf2").f;
-                r.exports = function(c) {
+                    c = t("9bf2").f;
+                r.exports = function(f) {
                     var d = o.Symbol || (o.Symbol = {});
-                    l(d, c) || f(d, c, {
-                        value: u.f(c)
+                    l(d, f) || c(d, f, {
+                        value: u.f(f)
                     })
                 }
             },
             7839: function(r, s) {
                 r.exports = ["constructor", "hasOwnProperty", "isPrototypeOf", "propertyIsEnumerable", "toLocaleString", "toString", "valueOf"]
             },
             "7b0b": function(r, s, t) {
@@ -2999,16 +2999,16 @@
                     return Object(o(l))
                 }
             },
             "7c73": function(r, s, t) {
                 var o = t("825a"),
                     l = t("37e8"),
                     u = t("7839"),
-                    f = t("d012"),
-                    c = t("1be4"),
+                    c = t("d012"),
+                    f = t("1be4"),
                     d = t("cc12"),
                     v = t("f772"),
                     p = ">",
                     h = "<",
                     m = "prototype",
                     g = "script",
                     y = v("IE_PROTO"),
@@ -3021,35 +3021,35 @@
                         var j = I.parentWindow.Object;
                         return I = null, j
                     },
                     T = function() {
                         var I = d("iframe"),
                             j = "java" + g + ":",
                             P;
-                        return I.style.display = "none", c.appendChild(I), I.src = String(j), P = I.contentWindow.document, P.open(), P.write(E("document.F=Object")), P.close(), P.F
+                        return I.style.display = "none", f.appendChild(I), I.src = String(j), P = I.contentWindow.document, P.open(), P.write(E("document.F=Object")), P.close(), P.F
                     },
                     $, L = function() {
                         try {
                             $ = document.domain && new ActiveXObject("htmlfile")
                         } catch {}
                         L = $ ? C($) : T();
                         for (var I = u.length; I--;) delete L[m][u[I]];
                         return L()
                     };
-                f[y] = !0, r.exports = Object.create || function(j, P) {
-                    var M;
-                    return j !== null ? (O[m] = o(j), M = new O, O[m] = null, M[y] = j) : M = L(), P === void 0 ? M : l(M, P)
+                c[y] = !0, r.exports = Object.create || function(j, P) {
+                    var w;
+                    return j !== null ? (O[m] = o(j), w = new O, O[m] = null, w[y] = j) : w = L(), P === void 0 ? w : l(w, P)
                 }
             },
             "7dd0": function(r, s, t) {
                 var o = t("23e7"),
                     l = t("9ed3"),
                     u = t("e163"),
-                    f = t("d2bb"),
-                    c = t("d44e"),
+                    c = t("d2bb"),
+                    f = t("d44e"),
                     d = t("9112"),
                     v = t("6eeb"),
                     p = t("b622"),
                     h = t("c430"),
                     m = t("3f8c"),
                     g = t("ae93"),
                     y = g.IteratorPrototype,
@@ -3057,16 +3057,16 @@
                     E = p("iterator"),
                     C = "keys",
                     T = "values",
                     $ = "entries",
                     L = function() {
                         return this
                     };
-                r.exports = function(I, j, P, M, D, R, H) {
-                    l(P, j, M);
+                r.exports = function(I, j, P, w, D, R, H) {
+                    l(P, j, w);
                     var F = function(st) {
                             if (st === D && ct) return ct;
                             if (!O && st in ot) return ot[st];
                             switch (st) {
                                 case C:
                                     return function() {
                                         return new P(this, st)
@@ -3087,15 +3087,15 @@
                         N = j + " Iterator",
                         k = !1,
                         ot = I.prototype,
                         St = ot[E] || ot["@@iterator"] || D && ot[D],
                         ct = !O && St || F(D),
                         pt = j == "Array" && ot.entries || St,
                         Ot, It, Et;
-                    if (pt && (Ot = u(pt.call(new I)), y !== Object.prototype && Ot.next && (!h && u(Ot) !== y && (f ? f(Ot, y) : typeof Ot[E] != "function" && d(Ot, E, L)), c(Ot, N, !0, !0), h && (m[N] = L))), D == T && St && St.name !== T && (k = !0, ct = function() {
+                    if (pt && (Ot = u(pt.call(new I)), y !== Object.prototype && Ot.next && (!h && u(Ot) !== y && (c ? c(Ot, y) : typeof Ot[E] != "function" && d(Ot, E, L)), f(Ot, N, !0, !0), h && (m[N] = L))), D == T && St && St.name !== T && (k = !0, ct = function() {
                             return St.call(this)
                         }), (!h || H) && ot[E] !== ct && d(ot, E, ct), m[j] = ct, D)
                         if (It = {
                                 values: F(T),
                                 keys: R ? ct : F(C),
                                 entries: F($)
                             }, H)
@@ -3131,32 +3131,32 @@
                     })[1] != 7
                 })
             },
             8418: function(r, s, t) {
                 var o = t("c04e"),
                     l = t("9bf2"),
                     u = t("5c6c");
-                r.exports = function(f, c, d) {
-                    var v = o(c);
-                    v in f ? l.f(f, v, u(0, d)) : f[v] = d
+                r.exports = function(c, f, d) {
+                    var v = o(f);
+                    v in c ? l.f(c, v, u(0, d)) : c[v] = d
                 }
             },
             "861d": function(r, s) {
                 r.exports = function(t) {
                     return typeof t == "object" ? t !== null : typeof t == "function"
                 }
             },
             8875: function(r, s, t) {
                 var o, l, u;
-                (function(f, c) {
-                    l = [], o = c, u = typeof o == "function" ? o.apply(s, l) : o, u !== void 0 && (r.exports = u)
+                (function(c, f) {
+                    l = [], o = f, u = typeof o == "function" ? o.apply(s, l) : o, u !== void 0 && (r.exports = u)
                 })(typeof self < "u" ? self : this, function() {
-                    function f() {
-                        var c = Object.getOwnPropertyDescriptor(document, "currentScript");
-                        if (!c && "currentScript" in document && document.currentScript || c && c.get !== f && document.currentScript) return document.currentScript;
+                    function c() {
+                        var f = Object.getOwnPropertyDescriptor(document, "currentScript");
+                        if (!f && "currentScript" in document && document.currentScript || f && f.get !== c && document.currentScript) return document.currentScript;
                         try {
                             throw new Error
                         } catch ($) {
                             var d = /.*at [^(]*\((.*):(.+):(.+)\)$/ig,
                                 v = /@([^@]*):(\d+):(\d+)\s*$/ig,
                                 p = d.exec($.stack) || v.exec($.stack),
                                 h = p && p[1] || !1,
@@ -3165,28 +3165,28 @@
                                 y, O, E, C = document.getElementsByTagName("script");
                             h === g && (y = document.documentElement.outerHTML, O = new RegExp("(?:[^\\n]+?\\n){0," + (m - 2) + "}[^<]*<script>([\\d\\D]*?)<\\/script>[\\d\\D]*", "i"), E = y.replace(O, "$1").trim());
                             for (var T = 0; T < C.length; T++)
                                 if (C[T].readyState === "interactive" || C[T].src === h || h === g && C[T].innerHTML && C[T].innerHTML.trim() === E) return C[T];
                             return null
                         }
                     }
-                    return f
+                    return c
                 })
             },
             8925: function(r, s, t) {
                 var o = t("c6cd"),
                     l = Function.toString;
                 typeof o.inspectSource != "function" && (o.inspectSource = function(u) {
                     return l.call(u)
                 }), r.exports = o.inspectSource
             },
             "8aa5": function(r, s, t) {
                 var o = t("6547").charAt;
-                r.exports = function(l, u, f) {
-                    return u + (f ? o(l, u).length : 1)
+                r.exports = function(l, u, c) {
+                    return u + (c ? o(l, u).length : 1)
                 }
             },
             "8bbf": function(r, s) {
                 r.exports = n
             },
             "90e3": function(r, s) {
                 var t = 0,
@@ -3195,68 +3195,68 @@
                     return "Symbol(" + String(l === void 0 ? "" : l) + ")_" + (++t + o).toString(36)
                 }
             },
             9112: function(r, s, t) {
                 var o = t("83ab"),
                     l = t("9bf2"),
                     u = t("5c6c");
-                r.exports = o ? function(f, c, d) {
-                    return l.f(f, c, u(1, d))
-                } : function(f, c, d) {
-                    return f[c] = d, f
+                r.exports = o ? function(c, f, d) {
+                    return l.f(c, f, u(1, d))
+                } : function(c, f, d) {
+                    return c[f] = d, c
                 }
             },
             9263: function(r, s, t) {
                 var o = t("ad6d"),
                     l = t("9f7f"),
                     u = RegExp.prototype.exec,
-                    f = String.prototype.replace,
-                    c = u,
+                    c = String.prototype.replace,
+                    f = u,
                     d = function() {
                         var m = /a/,
                             g = /b*/g;
                         return u.call(m, "a"), u.call(g, "a"), m.lastIndex !== 0 || g.lastIndex !== 0
                     }(),
                     v = l.UNSUPPORTED_Y || l.BROKEN_CARET,
                     p = /()??/.exec("")[1] !== void 0,
                     h = d || p || v;
-                h && (c = function(g) {
+                h && (f = function(g) {
                     var y = this,
                         O, E, C, T, $ = v && y.sticky,
                         L = o.call(y),
                         I = y.source,
                         j = 0,
                         P = g;
                     return $ && (L = L.replace("y", ""), L.indexOf("g") === -1 && (L += "g"), P = String(g).slice(y.lastIndex), y.lastIndex > 0 && (!y.multiline || y.multiline && g[y.lastIndex - 1] !== `
-`) && (I = "(?: " + I + ")", P = " " + P, j++), E = new RegExp("^(?:" + I + ")", L)), p && (E = new RegExp("^" + I + "$(?!\\s)", L)), d && (O = y.lastIndex), C = u.call($ ? E : y, P), $ ? C ? (C.input = C.input.slice(j), C[0] = C[0].slice(j), C.index = y.lastIndex, y.lastIndex += C[0].length) : y.lastIndex = 0 : d && C && (y.lastIndex = y.global ? C.index + C[0].length : O), p && C && C.length > 1 && f.call(C[0], E, function() {
+`) && (I = "(?: " + I + ")", P = " " + P, j++), E = new RegExp("^(?:" + I + ")", L)), p && (E = new RegExp("^" + I + "$(?!\\s)", L)), d && (O = y.lastIndex), C = u.call($ ? E : y, P), $ ? C ? (C.input = C.input.slice(j), C[0] = C[0].slice(j), C.index = y.lastIndex, y.lastIndex += C[0].length) : y.lastIndex = 0 : d && C && (y.lastIndex = y.global ? C.index + C[0].length : O), p && C && C.length > 1 && c.call(C[0], E, function() {
                         for (T = 1; T < arguments.length - 2; T++) arguments[T] === void 0 && (C[T] = void 0)
                     }), C
-                }), r.exports = c
+                }), r.exports = f
             },
             "94ca": function(r, s, t) {
                 var o = t("d039"),
                     l = /#|\.prototype\./,
                     u = function(p, h) {
-                        var m = c[f(p)];
+                        var m = f[c(p)];
                         return m == v ? !0 : m == d ? !1 : typeof h == "function" ? o(h) : !!h
                     },
-                    f = u.normalize = function(p) {
+                    c = u.normalize = function(p) {
                         return String(p).replace(l, ".").toLowerCase()
                     },
-                    c = u.data = {},
+                    f = u.data = {},
                     d = u.NATIVE = "N",
                     v = u.POLYFILL = "P";
                 r.exports = u
             },
             "99af": function(r, s, t) {
                 var o = t("23e7"),
                     l = t("d039"),
                     u = t("e8b5"),
-                    f = t("861d"),
-                    c = t("7b0b"),
+                    c = t("861d"),
+                    f = t("7b0b"),
                     d = t("50c4"),
                     v = t("8418"),
                     p = t("65f0"),
                     h = t("1dde"),
                     m = t("b622"),
                     g = t("2d00"),
                     y = m("isConcatSpreadable"),
@@ -3264,124 +3264,124 @@
                     E = "Maximum allowed index exceeded",
                     C = g >= 51 || !l(function() {
                         var I = [];
                         return I[y] = !1, I.concat()[0] !== I
                     }),
                     T = h("concat"),
                     $ = function(I) {
-                        if (!f(I)) return !1;
+                        if (!c(I)) return !1;
                         var j = I[y];
                         return j !== void 0 ? !!j : u(I)
                     },
                     L = !C || !T;
                 o({
                     target: "Array",
                     proto: !0,
                     forced: L
                 }, {
                     concat: function(j) {
-                        var P = c(this),
-                            M = p(P, 0),
+                        var P = f(this),
+                            w = p(P, 0),
                             D = 0,
                             R, H, F, N, k;
                         for (R = -1, F = arguments.length; R < F; R++)
                             if (k = R === -1 ? P : arguments[R], $(k)) {
                                 if (N = d(k.length), D + N > O) throw TypeError(E);
-                                for (H = 0; H < N; H++, D++) H in k && v(M, D, k[H])
+                                for (H = 0; H < N; H++, D++) H in k && v(w, D, k[H])
                             } else {
                                 if (D >= O) throw TypeError(E);
-                                v(M, D++, k)
-                            } return M.length = D, M
+                                v(w, D++, k)
+                            } return w.length = D, w
                     }
                 })
             },
             "9bdd": function(r, s, t) {
                 var o = t("825a");
-                r.exports = function(l, u, f, c) {
+                r.exports = function(l, u, c, f) {
                     try {
-                        return c ? u(o(f)[0], f[1]) : u(f)
+                        return f ? u(o(c)[0], c[1]) : u(c)
                     } catch (v) {
                         var d = l.return;
                         throw d !== void 0 && o(d.call(l)), v
                     }
                 }
             },
             "9bf2": function(r, s, t) {
                 var o = t("83ab"),
                     l = t("0cfb"),
                     u = t("825a"),
-                    f = t("c04e"),
-                    c = Object.defineProperty;
-                s.f = o ? c : function(v, p, h) {
-                    if (u(v), p = f(p, !0), u(h), l) try {
-                        return c(v, p, h)
+                    c = t("c04e"),
+                    f = Object.defineProperty;
+                s.f = o ? f : function(v, p, h) {
+                    if (u(v), p = c(p, !0), u(h), l) try {
+                        return f(v, p, h)
                     } catch {}
                     if ("get" in h || "set" in h) throw TypeError("Accessors not supported");
                     return "value" in h && (v[p] = h.value), v
                 }
             },
             "9ed3": function(r, s, t) {
                 var o = t("ae93").IteratorPrototype,
                     l = t("7c73"),
                     u = t("5c6c"),
-                    f = t("d44e"),
-                    c = t("3f8c"),
+                    c = t("d44e"),
+                    f = t("3f8c"),
                     d = function() {
                         return this
                     };
                 r.exports = function(v, p, h) {
                     var m = p + " Iterator";
                     return v.prototype = l(o, {
                         next: u(1, h)
-                    }), f(v, m, !1, !0), c[m] = d, v
+                    }), c(v, m, !1, !0), f[m] = d, v
                 }
             },
             "9f7f": function(r, s, t) {
                 var o = t("d039");
 
-                function l(u, f) {
-                    return RegExp(u, f)
+                function l(u, c) {
+                    return RegExp(u, c)
                 }
                 s.UNSUPPORTED_Y = o(function() {
                     var u = l("a", "y");
                     return u.lastIndex = 2, u.exec("abcd") != null
                 }), s.BROKEN_CARET = o(function() {
                     var u = l("^r", "gy");
                     return u.lastIndex = 2, u.exec("str") != null
                 })
             },
             a2bf: function(r, s, t) {
                 var o = t("e8b5"),
                     l = t("50c4"),
                     u = t("0366"),
-                    f = function(c, d, v, p, h, m, g, y) {
+                    c = function(f, d, v, p, h, m, g, y) {
                         for (var O = h, E = 0, C = g ? u(g, y, 3) : !1, T; E < p;) {
                             if (E in v) {
-                                if (T = C ? C(v[E], E, d) : v[E], m > 0 && o(T)) O = f(c, d, T, l(T.length), O, m - 1) - 1;
+                                if (T = C ? C(v[E], E, d) : v[E], m > 0 && o(T)) O = c(f, d, T, l(T.length), O, m - 1) - 1;
                                 else {
                                     if (O >= 9007199254740991) throw TypeError("Exceed the acceptable array length");
-                                    c[O] = T
+                                    f[O] = T
                                 }
                                 O++
                             }
                             E++
                         }
                         return O
                     };
-                r.exports = f
+                r.exports = c
             },
             a352: function(r, s) {
                 r.exports = i
             },
             a434: function(r, s, t) {
                 var o = t("23e7"),
                     l = t("23cb"),
                     u = t("a691"),
-                    f = t("50c4"),
-                    c = t("7b0b"),
+                    c = t("50c4"),
+                    f = t("7b0b"),
                     d = t("65f0"),
                     v = t("8418"),
                     p = t("1dde"),
                     h = t("ae40"),
                     m = p("splice"),
                     g = h("splice", {
                         ACCESSORS: !0,
@@ -3394,20 +3394,20 @@
                     C = "Maximum allowed length exceeded";
                 o({
                     target: "Array",
                     proto: !0,
                     forced: !m || !g
                 }, {
                     splice: function($, L) {
-                        var I = c(this),
-                            j = f(I.length),
+                        var I = f(this),
+                            j = c(I.length),
                             P = l($, j),
-                            M = arguments.length,
+                            w = arguments.length,
                             D, R, H, F, N, k;
-                        if (M === 0 ? D = R = 0 : M === 1 ? (D = 0, R = j - P) : (D = M - 2, R = O(y(u(L), 0), j - P)), j + D - R > E) throw TypeError(C);
+                        if (w === 0 ? D = R = 0 : w === 1 ? (D = 0, R = j - P) : (D = w - 2, R = O(y(u(L), 0), j - P)), j + D - R > E) throw TypeError(C);
                         for (H = d(I, R), F = 0; F < R; F++) N = P + F, N in I && v(H, F, I[N]);
                         if (H.length = R, D < R) {
                             for (F = P; F < j - R; F++) N = F + R, k = F + D, N in I ? I[k] = I[N] : delete I[k];
                             for (F = j; F > j - R + D; F--) delete I[F - 1]
                         } else if (D > R)
                             for (F = j - R; F > P; F--) N = F + R - 1, k = F + D - 1, N in I ? I[k] = I[N] : delete I[k];
                         for (F = 0; F < D; F++) I[F + P] = arguments[F + 2];
@@ -3415,16 +3415,16 @@
                     }
                 })
             },
             a4d3: function(r, s, t) {
                 var o = t("23e7"),
                     l = t("da84"),
                     u = t("d066"),
-                    f = t("c430"),
-                    c = t("83ab"),
+                    c = t("c430"),
+                    f = t("83ab"),
                     d = t("4930"),
                     v = t("fdbf"),
                     p = t("d039"),
                     h = t("5135"),
                     m = t("e8b5"),
                     g = t("861d"),
                     y = t("825a"),
@@ -3433,15 +3433,15 @@
                     C = t("c04e"),
                     T = t("5c6c"),
                     $ = t("7c73"),
                     L = t("df75"),
                     I = t("241c"),
                     j = t("057f"),
                     P = t("7418"),
-                    M = t("06cf"),
+                    w = t("06cf"),
                     D = t("9bf2"),
                     R = t("d1e7"),
                     H = t("9112"),
                     F = t("6eeb"),
                     N = t("5692"),
                     k = t("f772"),
                     ot = t("d012"),
@@ -3457,78 +3457,78 @@
                     wt = "prototype",
                     re = ct("toPrimitive"),
                     de = Et.set,
                     ie = Et.getterFor(Lt),
                     Pt = Object[wt],
                     Ct = l.Symbol,
                     ve = u("JSON", "stringify"),
-                    Zt = M.f,
-                    kt = D.f,
+                    kt = w.f,
+                    qt = D.f,
                     Je = j.f,
                     mn = R.f,
                     Wt = N("symbols"),
                     le = N("op-symbols"),
                     ye = N("string-to-symbol-registry"),
                     Pe = N("symbol-to-string-registry"),
                     Ce = N("wks"),
                     De = l.QObject,
                     Ae = !De || !De[wt] || !De[wt].findChild,
-                    Re = c && p(function() {
-                        return $(kt({}, "a", {
+                    Re = f && p(function() {
+                        return $(qt({}, "a", {
                             get: function() {
-                                return kt(this, "a", {
+                                return qt(this, "a", {
                                     value: 7
                                 }).a
                             }
                         })).a != 7
                     }) ? function(Q, B, Y) {
-                        var nt = Zt(Pt, B);
-                        nt && delete Pt[B], kt(Q, B, Y), nt && Q !== Pt && kt(Pt, B, nt)
-                    } : kt,
+                        var nt = kt(Pt, B);
+                        nt && delete Pt[B], qt(Q, B, Y), nt && Q !== Pt && qt(Pt, B, nt)
+                    } : qt,
                     we = function(Q, B) {
                         var Y = Wt[Q] = $(Ct[wt]);
                         return de(Y, {
                             type: Lt,
                             tag: Q,
                             description: B
-                        }), c || (Y.description = B), Y
+                        }), f || (Y.description = B), Y
                     },
                     S = v ? function(Q) {
                         return typeof Q == "symbol"
                     } : function(Q) {
                         return Object(Q) instanceof Ct
                     },
                     b = function(B, Y, nt) {
                         B === Pt && b(le, Y, nt), y(B);
                         var rt = C(Y, !0);
                         return y(nt), h(Wt, rt) ? (nt.enumerable ? (h(B, dt) && B[dt][rt] && (B[dt][rt] = !1), nt = $(nt, {
                             enumerable: T(0, !1)
-                        })) : (h(B, dt) || kt(B, dt, T(1, {})), B[dt][rt] = !0), Re(B, rt, nt)) : kt(B, rt, nt)
+                        })) : (h(B, dt) || qt(B, dt, T(1, {})), B[dt][rt] = !0), Re(B, rt, nt)) : qt(B, rt, nt)
                     },
                     x = function(B, Y) {
                         y(B);
                         var nt = E(Y),
                             rt = L(nt).concat(at(nt));
                         return st(rt, function(jt) {
-                            (!c || V.call(nt, jt)) && b(B, jt, nt[jt])
+                            (!f || V.call(nt, jt)) && b(B, jt, nt[jt])
                         }), B
                     },
                     A = function(B, Y) {
                         return Y === void 0 ? $(B) : x($(B), Y)
                     },
                     V = function(B) {
                         var Y = C(B, !0),
                             nt = mn.call(this, Y);
                         return this === Pt && h(Wt, Y) && !h(le, Y) ? !1 : nt || !h(this, Y) || !h(Wt, Y) || h(this, dt) && this[dt][Y] ? nt : !0
                     },
                     J = function(B, Y) {
                         var nt = E(B),
                             rt = C(Y, !0);
                         if (!(nt === Pt && h(Wt, rt) && !h(le, rt))) {
-                            var jt = Zt(nt, rt);
+                            var jt = kt(nt, rt);
                             return jt && h(Wt, rt) && !(h(nt, dt) && nt[dt][rt]) && (jt.enumerable = !0), jt
                         }
                     },
                     _ = function(B) {
                         var Y = Je(E(B)),
                             nt = [];
                         return st(Y, function(rt) {
@@ -3546,30 +3546,30 @@
                 if (d || (Ct = function() {
                         if (this instanceof Ct) throw TypeError("Symbol is not a constructor");
                         var B = !arguments.length || arguments[0] === void 0 ? void 0 : String(arguments[0]),
                             Y = St(B),
                             nt = function(rt) {
                                 this === Pt && nt.call(le, rt), h(this, dt) && h(this[dt], Y) && (this[dt][Y] = !1), Re(this, Y, T(1, rt))
                             };
-                        return c && Ae && Re(Pt, Y, {
+                        return f && Ae && Re(Pt, Y, {
                             configurable: !0,
                             set: nt
                         }), we(Y, B)
                     }, F(Ct[wt], "toString", function() {
                         return ie(this).tag
                     }), F(Ct, "withoutSetter", function(Q) {
                         return we(St(Q), Q)
-                    }), R.f = V, D.f = b, M.f = J, I.f = j.f = _, P.f = at, pt.f = function(Q) {
+                    }), R.f = V, D.f = b, w.f = J, I.f = j.f = _, P.f = at, pt.f = function(Q) {
                         return we(ct(Q), Q)
-                    }, c && (kt(Ct[wt], "description", {
+                    }, f && (qt(Ct[wt], "description", {
                         configurable: !0,
                         get: function() {
                             return ie(this).description
                         }
-                    }), f || F(Pt, "propertyIsEnumerable", V, {
+                    }), c || F(Pt, "propertyIsEnumerable", V, {
                         unsafe: !0
                     }))), o({
                         global: !0,
                         wrap: !0,
                         forced: !d,
                         sham: !d
                     }, {
@@ -3597,15 +3597,15 @@
                         useSimple: function() {
                             Ae = !1
                         }
                     }), o({
                         target: "Object",
                         stat: !0,
                         forced: !d,
-                        sham: !c
+                        sham: !f
                     }, {
                         create: A,
                         defineProperty: b,
                         defineProperties: x,
                         getOwnPropertyDescriptor: J
                     }), o({
                         target: "Object",
@@ -3646,31 +3646,31 @@
                 }
                 Ct[wt][re] || H(Ct[wt], re, Ct[wt].valueOf), It(Ct, Lt), ot[dt] = !0
             },
             a630: function(r, s, t) {
                 var o = t("23e7"),
                     l = t("4df4"),
                     u = t("1c7e"),
-                    f = !u(function(c) {
-                        Array.from(c)
+                    c = !u(function(f) {
+                        Array.from(f)
                     });
                 o({
                     target: "Array",
                     stat: !0,
-                    forced: f
+                    forced: c
                 }, {
                     from: l
                 })
             },
             a640: function(r, s, t) {
                 var o = t("d039");
                 r.exports = function(l, u) {
-                    var f = [][l];
-                    return !!f && o(function() {
-                        f.call(null, u || function() {
+                    var c = [][l];
+                    return !!c && o(function() {
+                        c.call(null, u || function() {
                             throw 1
                         }, 1)
                     })
                 }
             },
             a691: function(r, s) {
                 var t = Math.ceil,
@@ -3679,20 +3679,20 @@
                     return isNaN(l = +l) ? 0 : (l > 0 ? o : t)(l)
                 }
             },
             ab13: function(r, s, t) {
                 var o = t("b622"),
                     l = o("match");
                 r.exports = function(u) {
-                    var f = /./;
+                    var c = /./;
                     try {
-                        "/./" [u](f)
+                        "/./" [u](c)
                     } catch {
                         try {
-                            return f[l] = !1, "/./" [u](f)
+                            return c[l] = !1, "/./" [u](c)
                         } catch {}
                     }
                     return !1
                 }
             },
             ac1f: function(r, s, t) {
                 var o = t("23e7"),
@@ -3713,51 +3713,51 @@
                     return l.global && (u += "g"), l.ignoreCase && (u += "i"), l.multiline && (u += "m"), l.dotAll && (u += "s"), l.unicode && (u += "u"), l.sticky && (u += "y"), u
                 }
             },
             ae40: function(r, s, t) {
                 var o = t("83ab"),
                     l = t("d039"),
                     u = t("5135"),
-                    f = Object.defineProperty,
-                    c = {},
+                    c = Object.defineProperty,
+                    f = {},
                     d = function(v) {
                         throw v
                     };
                 r.exports = function(v, p) {
-                    if (u(c, v)) return c[v];
+                    if (u(f, v)) return f[v];
                     p || (p = {});
                     var h = [][v],
                         m = u(p, "ACCESSORS") ? p.ACCESSORS : !1,
                         g = u(p, 0) ? p[0] : d,
                         y = u(p, 1) ? p[1] : void 0;
-                    return c[v] = !!h && !l(function() {
+                    return f[v] = !!h && !l(function() {
                         if (m && !o) return !0;
                         var O = {
                             length: -1
                         };
-                        m ? f(O, 1, {
+                        m ? c(O, 1, {
                             enumerable: !0,
                             get: d
                         }) : O[1] = 1, h.call(O, g, y)
                     })
                 }
             },
             ae93: function(r, s, t) {
                 var o = t("e163"),
                     l = t("9112"),
                     u = t("5135"),
-                    f = t("b622"),
-                    c = t("c430"),
-                    d = f("iterator"),
+                    c = t("b622"),
+                    f = t("c430"),
+                    d = c("iterator"),
                     v = !1,
                     p = function() {
                         return this
                     },
                     h, m, g;
-                [].keys && (g = [].keys(), "next" in g ? (m = o(o(g)), m !== Object.prototype && (h = m)) : v = !0), h == null && (h = {}), !c && !u(h, d) && l(h, d, p), r.exports = {
+                [].keys && (g = [].keys(), "next" in g ? (m = o(o(g)), m !== Object.prototype && (h = m)) : v = !0), h == null && (h = {}), !f && !u(h, d) && l(h, d, p), r.exports = {
                     IteratorPrototype: h,
                     BUGGY_SAFARI_ITERATORS: v
                 }
             },
             b041: function(r, s, t) {
                 var o = t("00ee"),
                     l = t("f5df");
@@ -3765,76 +3765,76 @@
                     return "[object " + l(this) + "]"
                 }
             },
             b0c0: function(r, s, t) {
                 var o = t("83ab"),
                     l = t("9bf2").f,
                     u = Function.prototype,
-                    f = u.toString,
-                    c = /^\s*function ([^ (]*)/,
+                    c = u.toString,
+                    f = /^\s*function ([^ (]*)/,
                     d = "name";
                 o && !(d in u) && l(u, d, {
                     configurable: !0,
                     get: function() {
                         try {
-                            return f.call(this).match(c)[1]
+                            return c.call(this).match(f)[1]
                         } catch {
                             return ""
                         }
                     }
                 })
             },
             b622: function(r, s, t) {
                 var o = t("da84"),
                     l = t("5692"),
                     u = t("5135"),
-                    f = t("90e3"),
-                    c = t("4930"),
+                    c = t("90e3"),
+                    f = t("4930"),
                     d = t("fdbf"),
                     v = l("wks"),
                     p = o.Symbol,
-                    h = d ? p : p && p.withoutSetter || f;
+                    h = d ? p : p && p.withoutSetter || c;
                 r.exports = function(m) {
-                    return u(v, m) || (c && u(p, m) ? v[m] = p[m] : v[m] = h("Symbol." + m)), v[m]
+                    return u(v, m) || (f && u(p, m) ? v[m] = p[m] : v[m] = h("Symbol." + m)), v[m]
                 }
             },
             b64b: function(r, s, t) {
                 var o = t("23e7"),
                     l = t("7b0b"),
                     u = t("df75"),
-                    f = t("d039"),
-                    c = f(function() {
+                    c = t("d039"),
+                    f = c(function() {
                         u(1)
                     });
                 o({
                     target: "Object",
                     stat: !0,
-                    forced: c
+                    forced: f
                 }, {
                     keys: function(v) {
                         return u(l(v))
                     }
                 })
             },
             b727: function(r, s, t) {
                 var o = t("0366"),
                     l = t("44ad"),
                     u = t("7b0b"),
-                    f = t("50c4"),
-                    c = t("65f0"),
+                    c = t("50c4"),
+                    f = t("65f0"),
                     d = [].push,
                     v = function(p) {
                         var h = p == 1,
                             m = p == 2,
                             g = p == 3,
                             y = p == 4,
                             O = p == 6,
                             E = p == 5 || O;
                         return function(C, T, $, L) {
-                            for (var I = u(C), j = l(I), P = o(T, $, 3), M = f(j.length), D = 0, R = L || c, H = h ? R(C, M) : m ? R(C, 0) : void 0, F, N; M > D; D++)
+                            for (var I = u(C), j = l(I), P = o(T, $, 3), w = c(j.length), D = 0, R = L || f, H = h ? R(C, w) : m ? R(C, 0) : void 0, F, N; w > D; D++)
                                 if ((E || D in j) && (F = j[D], N = P(F, D, I), p)) {
                                     if (h) H[D] = N;
                                     else if (N) switch (p) {
                                         case 3:
                                             return !0;
                                         case 5:
                                             return F;
@@ -3856,16 +3856,16 @@
                     findIndex: v(6)
                 }
             },
             c04e: function(r, s, t) {
                 var o = t("861d");
                 r.exports = function(l, u) {
                     if (!o(l)) return l;
-                    var f, c;
-                    if (u && typeof(f = l.toString) == "function" && !o(c = f.call(l)) || typeof(f = l.valueOf) == "function" && !o(c = f.call(l)) || !u && typeof(f = l.toString) == "function" && !o(c = f.call(l))) return c;
+                    var c, f;
+                    if (u && typeof(c = l.toString) == "function" && !o(f = c.call(l)) || typeof(c = l.valueOf) == "function" && !o(f = c.call(l)) || !u && typeof(c = l.toString) == "function" && !o(f = c.call(l))) return f;
                     throw TypeError("Can't convert object to primitive value")
                 }
             },
             c430: function(r, s) {
                 r.exports = !1
             },
             c6b6: function(r, s) {
@@ -3874,36 +3874,36 @@
                     return t.call(o).slice(8, -1)
                 }
             },
             c6cd: function(r, s, t) {
                 var o = t("da84"),
                     l = t("ce4e"),
                     u = "__core-js_shared__",
-                    f = o[u] || l(u, {});
-                r.exports = f
+                    c = o[u] || l(u, {});
+                r.exports = c
             },
             c740: function(r, s, t) {
                 var o = t("23e7"),
                     l = t("b727").findIndex,
                     u = t("44d2"),
-                    f = t("ae40"),
-                    c = "findIndex",
+                    c = t("ae40"),
+                    f = "findIndex",
                     d = !0,
-                    v = f(c);
-                c in [] && Array(1)[c](function() {
+                    v = c(f);
+                f in [] && Array(1)[f](function() {
                     d = !1
                 }), o({
                     target: "Array",
                     proto: !0,
                     forced: d || !v
                 }, {
                     findIndex: function(h) {
                         return l(this, h, arguments.length > 1 ? arguments[1] : void 0)
                     }
-                }), u(c)
+                }), u(f)
             },
             c8ba: function(r, s) {
                 var t;
                 t = function() {
                     return this
                 }();
                 try {
@@ -3913,85 +3913,85 @@
                 }
                 r.exports = t
             },
             c975: function(r, s, t) {
                 var o = t("23e7"),
                     l = t("4d64").indexOf,
                     u = t("a640"),
-                    f = t("ae40"),
-                    c = [].indexOf,
-                    d = !!c && 1 / [1].indexOf(1, -0) < 0,
+                    c = t("ae40"),
+                    f = [].indexOf,
+                    d = !!f && 1 / [1].indexOf(1, -0) < 0,
                     v = u("indexOf"),
-                    p = f("indexOf", {
+                    p = c("indexOf", {
                         ACCESSORS: !0,
                         1: 0
                     });
                 o({
                     target: "Array",
                     proto: !0,
                     forced: d || !v || !p
                 }, {
                     indexOf: function(m) {
-                        return d ? c.apply(this, arguments) || 0 : l(this, m, arguments.length > 1 ? arguments[1] : void 0)
+                        return d ? f.apply(this, arguments) || 0 : l(this, m, arguments.length > 1 ? arguments[1] : void 0)
                     }
                 })
             },
             ca84: function(r, s, t) {
                 var o = t("5135"),
                     l = t("fc6a"),
                     u = t("4d64").indexOf,
-                    f = t("d012");
-                r.exports = function(c, d) {
-                    var v = l(c),
+                    c = t("d012");
+                r.exports = function(f, d) {
+                    var v = l(f),
                         p = 0,
                         h = [],
                         m;
-                    for (m in v) !o(f, m) && o(v, m) && h.push(m);
+                    for (m in v) !o(c, m) && o(v, m) && h.push(m);
                     for (; d.length > p;) o(v, m = d[p++]) && (~u(h, m) || h.push(m));
                     return h
                 }
             },
             caad: function(r, s, t) {
                 var o = t("23e7"),
                     l = t("4d64").includes,
                     u = t("44d2"),
-                    f = t("ae40"),
-                    c = f("indexOf", {
+                    c = t("ae40"),
+                    f = c("indexOf", {
                         ACCESSORS: !0,
                         1: 0
                     });
                 o({
                     target: "Array",
                     proto: !0,
-                    forced: !c
+                    forced: !f
                 }, {
                     includes: function(v) {
                         return l(this, v, arguments.length > 1 ? arguments[1] : void 0)
                     }
                 }), u("includes")
             },
             cc12: function(r, s, t) {
                 var o = t("da84"),
                     l = t("861d"),
                     u = o.document,
-                    f = l(u) && l(u.createElement);
-                r.exports = function(c) {
-                    return f ? u.createElement(c) : {}
+                    c = l(u) && l(u.createElement);
+                r.exports = function(f) {
+                    return c ? u.createElement(f) : {}
                 }
             },
             ce4e: function(r, s, t) {
                 var o = t("da84"),
                     l = t("9112");
-                r.exports = function(u, f) {
+                r.exports = function(u, c) {
                     try {
-                        l(o, u, f)
+                        l(o, u, c)
                     } catch {
-                        o[u] = f
+                        o[u] = c
                     }
-                    return f
+                    return c
                 }
             },
             d012: function(r, s) {
                 r.exports = {}
             },
             d039: function(r, s) {
                 r.exports = function(t) {
@@ -4001,48 +4001,48 @@
                         return !0
                     }
                 }
             },
             d066: function(r, s, t) {
                 var o = t("428f"),
                     l = t("da84"),
-                    u = function(f) {
-                        return typeof f == "function" ? f : void 0
+                    u = function(c) {
+                        return typeof c == "function" ? c : void 0
                     };
-                r.exports = function(f, c) {
-                    return arguments.length < 2 ? u(o[f]) || u(l[f]) : o[f] && o[f][c] || l[f] && l[f][c]
+                r.exports = function(c, f) {
+                    return arguments.length < 2 ? u(o[c]) || u(l[c]) : o[c] && o[c][f] || l[c] && l[c][f]
                 }
             },
             d1e7: function(r, s, t) {
                 var o = {}.propertyIsEnumerable,
                     l = Object.getOwnPropertyDescriptor,
                     u = l && !o.call({
                         1: 2
                     }, 1);
-                s.f = u ? function(c) {
-                    var d = l(this, c);
+                s.f = u ? function(f) {
+                    var d = l(this, f);
                     return !!d && d.enumerable
                 } : o
             },
             d28b: function(r, s, t) {
                 var o = t("746f");
                 o("iterator")
             },
             d2bb: function(r, s, t) {
                 var o = t("825a"),
                     l = t("3bbe");
                 r.exports = Object.setPrototypeOf || ("__proto__" in {} ? function() {
                     var u = !1,
-                        f = {},
-                        c;
+                        c = {},
+                        f;
                     try {
-                        c = Object.getOwnPropertyDescriptor(Object.prototype, "__proto__").set, c.call(f, []), u = f instanceof Array
+                        f = Object.getOwnPropertyDescriptor(Object.prototype, "__proto__").set, f.call(c, []), u = c instanceof Array
                     } catch {}
                     return function(v, p) {
-                        return o(v), l(p), u ? c.call(v, p) : v.__proto__ = p, v
+                        return o(v), l(p), u ? f.call(v, p) : v.__proto__ = p, v
                     }
                 }() : void 0)
             },
             d3b7: function(r, s, t) {
                 var o = t("00ee"),
                     l = t("6eeb"),
                     u = t("b041");
@@ -4050,33 +4050,33 @@
                     unsafe: !0
                 })
             },
             d44e: function(r, s, t) {
                 var o = t("9bf2").f,
                     l = t("5135"),
                     u = t("b622"),
-                    f = u("toStringTag");
-                r.exports = function(c, d, v) {
-                    c && !l(c = v ? c : c.prototype, f) && o(c, f, {
+                    c = u("toStringTag");
+                r.exports = function(f, d, v) {
+                    f && !l(f = v ? f : f.prototype, c) && o(f, c, {
                         configurable: !0,
                         value: d
                     })
                 }
             },
             d58f: function(r, s, t) {
                 var o = t("1c0b"),
                     l = t("7b0b"),
                     u = t("44ad"),
-                    f = t("50c4"),
-                    c = function(d) {
+                    c = t("50c4"),
+                    f = function(d) {
                         return function(v, p, h, m) {
                             o(p);
                             var g = l(v),
                                 y = u(g),
-                                O = f(g.length),
+                                O = c(g.length),
                                 E = d ? O - 1 : 0,
                                 C = d ? -1 : 1;
                             if (h < 2)
                                 for (;;) {
                                     if (E in y) {
                                         m = y[E], E += C;
                                         break
@@ -4084,25 +4084,25 @@
                                     if (E += C, d ? E < 0 : O <= E) throw TypeError("Reduce of empty array with no initial value")
                                 }
                             for (; d ? E >= 0 : O > E; E += C) E in y && (m = p(m, y[E], E, g));
                             return m
                         }
                     };
                 r.exports = {
-                    left: c(!1),
-                    right: c(!0)
+                    left: f(!1),
+                    right: f(!0)
                 }
             },
             d784: function(r, s, t) {
                 t("ac1f");
                 var o = t("6eeb"),
                     l = t("d039"),
                     u = t("b622"),
-                    f = t("9263"),
-                    c = t("9112"),
+                    c = t("9263"),
+                    f = t("9112"),
                     d = u("species"),
                     v = !l(function() {
                         var y = /./;
                         return y.exec = function() {
                             var O = [];
                             return O.groups = {
                                 a: "7"
@@ -4141,49 +4141,49 @@
                             }, R.flags = "", R[T] = /./ [T]), R.exec = function() {
                                 return D = !0, null
                             }, R[T](""), !D
                         });
                     if (!$ || !L || y === "replace" && !(v && p && !m) || y === "split" && !g) {
                         var I = /./ [T],
                             j = E(T, "" [y], function(D, R, H, F, N) {
-                                return R.exec === f ? $ && !N ? {
+                                return R.exec === c ? $ && !N ? {
                                     done: !0,
                                     value: I.call(R, H, F)
                                 } : {
                                     done: !0,
                                     value: D.call(H, R, F)
                                 } : {
                                     done: !1
                                 }
                             }, {
                                 REPLACE_KEEPS_$0: p,
                                 REGEXP_REPLACE_SUBSTITUTES_UNDEFINED_CAPTURE: m
                             }),
                             P = j[0],
-                            M = j[1];
+                            w = j[1];
                         o(String.prototype, y, P), o(RegExp.prototype, T, O == 2 ? function(D, R) {
-                            return M.call(D, this, R)
+                            return w.call(D, this, R)
                         } : function(D) {
-                            return M.call(D, this)
+                            return w.call(D, this)
                         })
                     }
-                    C && c(RegExp.prototype[T], "sham", !0)
+                    C && f(RegExp.prototype[T], "sham", !0)
                 }
             },
             d81d: function(r, s, t) {
                 var o = t("23e7"),
                     l = t("b727").map,
                     u = t("1dde"),
-                    f = t("ae40"),
-                    c = u("map"),
-                    d = f("map");
+                    c = t("ae40"),
+                    f = u("map"),
+                    d = c("map");
                 o({
                     target: "Array",
                     proto: !0,
-                    forced: !c || !d
+                    forced: !f || !d
                 }, {
                     map: function(p) {
                         return l(this, p, arguments.length > 1 ? arguments[1] : void 0)
                     }
                 })
             },
             da84: function(r, s, t) {
@@ -4194,24 +4194,24 @@
                     r.exports = l(typeof globalThis == "object" && globalThis) || l(typeof window == "object" && window) || l(typeof self == "object" && self) || l(typeof o == "object" && o) || Function("return this")()
                 }).call(this, t("c8ba"))
             },
             dbb4: function(r, s, t) {
                 var o = t("23e7"),
                     l = t("83ab"),
                     u = t("56ef"),
-                    f = t("fc6a"),
-                    c = t("06cf"),
+                    c = t("fc6a"),
+                    f = t("06cf"),
                     d = t("8418");
                 o({
                     target: "Object",
                     stat: !0,
                     sham: !l
                 }, {
                     getOwnPropertyDescriptors: function(p) {
-                        for (var h = f(p), m = c.f, g = u(h), y = {}, O = 0, E, C; g.length > O;) C = m(h, E = g[O++]), C !== void 0 && d(y, E, C);
+                        for (var h = c(p), m = f.f, g = u(h), y = {}, O = 0, E, C; g.length > O;) C = m(h, E = g[O++]), C !== void 0 && d(y, E, C);
                         return y
                     }
                 })
             },
             dbf1: function(r, s, t) {
                 (function(o) {
                     t.d(s, "a", function() {
@@ -4224,52 +4224,52 @@
                     var u = l()
                 }).call(this, t("c8ba"))
             },
             ddb0: function(r, s, t) {
                 var o = t("da84"),
                     l = t("fdbc"),
                     u = t("e260"),
-                    f = t("9112"),
-                    c = t("b622"),
-                    d = c("iterator"),
-                    v = c("toStringTag"),
+                    c = t("9112"),
+                    f = t("b622"),
+                    d = f("iterator"),
+                    v = f("toStringTag"),
                     p = u.values;
                 for (var h in l) {
                     var m = o[h],
                         g = m && m.prototype;
                     if (g) {
                         if (g[d] !== p) try {
-                            f(g, d, p)
+                            c(g, d, p)
                         } catch {
                             g[d] = p
                         }
-                        if (g[v] || f(g, v, h), l[h]) {
+                        if (g[v] || c(g, v, h), l[h]) {
                             for (var y in u)
                                 if (g[y] !== u[y]) try {
-                                    f(g, y, u[y])
+                                    c(g, y, u[y])
                                 } catch {
                                     g[y] = u[y]
                                 }
                         }
                     }
                 }
             },
             df75: function(r, s, t) {
                 var o = t("ca84"),
                     l = t("7839");
-                r.exports = Object.keys || function(f) {
-                    return o(f, l)
+                r.exports = Object.keys || function(c) {
+                    return o(c, l)
                 }
             },
             e01a: function(r, s, t) {
                 var o = t("23e7"),
                     l = t("83ab"),
                     u = t("da84"),
-                    f = t("5135"),
-                    c = t("861d"),
+                    c = t("5135"),
+                    f = t("861d"),
                     d = t("9bf2").f,
                     v = t("e893"),
                     p = u.Symbol;
                 if (l && typeof p == "function" && (!("description" in p.prototype) || p().description !== void 0)) {
                     var h = {},
                         m = function() {
                             var T = arguments.length < 1 || arguments[0] === void 0 ? void 0 : String(arguments[0]),
@@ -4281,17 +4281,17 @@
                     g.constructor = m;
                     var y = g.toString,
                         O = String(p("test")) == "Symbol(test)",
                         E = /^Symbol\((.*)\)[^)]+$/;
                     d(g, "description", {
                         configurable: !0,
                         get: function() {
-                            var T = c(this) ? this.valueOf() : this,
+                            var T = f(this) ? this.valueOf() : this,
                                 $ = y.call(T);
-                            if (f(h, T)) return "";
+                            if (c(h, T)) return "";
                             var L = O ? $.slice(7, -1) : $.replace(E, "$1");
                             return L === "" ? void 0 : L
                         }
                     }), o({
                         global: !0,
                         forced: !0
                     }, {
@@ -4299,38 +4299,38 @@
                     })
                 }
             },
             e163: function(r, s, t) {
                 var o = t("5135"),
                     l = t("7b0b"),
                     u = t("f772"),
-                    f = t("e177"),
-                    c = u("IE_PROTO"),
+                    c = t("e177"),
+                    f = u("IE_PROTO"),
                     d = Object.prototype;
-                r.exports = f ? Object.getPrototypeOf : function(v) {
-                    return v = l(v), o(v, c) ? v[c] : typeof v.constructor == "function" && v instanceof v.constructor ? v.constructor.prototype : v instanceof Object ? d : null
+                r.exports = c ? Object.getPrototypeOf : function(v) {
+                    return v = l(v), o(v, f) ? v[f] : typeof v.constructor == "function" && v instanceof v.constructor ? v.constructor.prototype : v instanceof Object ? d : null
                 }
             },
             e177: function(r, s, t) {
                 var o = t("d039");
                 r.exports = !o(function() {
                     function l() {}
                     return l.prototype.constructor = null, Object.getPrototypeOf(new l) !== l.prototype
                 })
             },
             e260: function(r, s, t) {
                 var o = t("fc6a"),
                     l = t("44d2"),
                     u = t("3f8c"),
-                    f = t("69f3"),
-                    c = t("7dd0"),
+                    c = t("69f3"),
+                    f = t("7dd0"),
                     d = "Array Iterator",
-                    v = f.set,
-                    p = f.getterFor(d);
-                r.exports = c(Array, "Array", function(h, m) {
+                    v = c.set,
+                    p = c.getterFor(d);
+                r.exports = f(Array, "Array", function(h, m) {
                     v(this, {
                         type: d,
                         target: o(h),
                         index: 0,
                         kind: m
                     })
                 }, function() {
@@ -4353,86 +4353,86 @@
                     }
                 }, "values"), u.Arguments = u.Array, l("keys"), l("values"), l("entries")
             },
             e439: function(r, s, t) {
                 var o = t("23e7"),
                     l = t("d039"),
                     u = t("fc6a"),
-                    f = t("06cf").f,
-                    c = t("83ab"),
+                    c = t("06cf").f,
+                    f = t("83ab"),
                     d = l(function() {
-                        f(1)
+                        c(1)
                     }),
-                    v = !c || d;
+                    v = !f || d;
                 o({
                     target: "Object",
                     stat: !0,
                     forced: v,
-                    sham: !c
+                    sham: !f
                 }, {
                     getOwnPropertyDescriptor: function(h, m) {
-                        return f(u(h), m)
+                        return c(u(h), m)
                     }
                 })
             },
             e538: function(r, s, t) {
                 var o = t("b622");
                 s.f = o
             },
             e893: function(r, s, t) {
                 var o = t("5135"),
                     l = t("56ef"),
                     u = t("06cf"),
-                    f = t("9bf2");
-                r.exports = function(c, d) {
-                    for (var v = l(d), p = f.f, h = u.f, m = 0; m < v.length; m++) {
+                    c = t("9bf2");
+                r.exports = function(f, d) {
+                    for (var v = l(d), p = c.f, h = u.f, m = 0; m < v.length; m++) {
                         var g = v[m];
-                        o(c, g) || p(c, g, h(d, g))
+                        o(f, g) || p(f, g, h(d, g))
                     }
                 }
             },
             e8b5: function(r, s, t) {
                 var o = t("c6b6");
                 r.exports = Array.isArray || function(u) {
                     return o(u) == "Array"
                 }
             },
             e95a: function(r, s, t) {
                 var o = t("b622"),
                     l = t("3f8c"),
                     u = o("iterator"),
-                    f = Array.prototype;
-                r.exports = function(c) {
-                    return c !== void 0 && (l.Array === c || f[u] === c)
+                    c = Array.prototype;
+                r.exports = function(f) {
+                    return f !== void 0 && (l.Array === f || c[u] === f)
                 }
             },
             f5df: function(r, s, t) {
                 var o = t("00ee"),
                     l = t("c6b6"),
                     u = t("b622"),
-                    f = u("toStringTag"),
-                    c = l(function() {
+                    c = u("toStringTag"),
+                    f = l(function() {
                         return arguments
                     }()) == "Arguments",
                     d = function(v, p) {
                         try {
                             return v[p]
                         } catch {}
                     };
                 r.exports = o ? l : function(v) {
                     var p, h, m;
-                    return v === void 0 ? "Undefined" : v === null ? "Null" : typeof(h = d(p = Object(v), f)) == "string" ? h : c ? l(p) : (m = l(p)) == "Object" && typeof p.callee == "function" ? "Arguments" : m
+                    return v === void 0 ? "Undefined" : v === null ? "Null" : typeof(h = d(p = Object(v), c)) == "string" ? h : f ? l(p) : (m = l(p)) == "Object" && typeof p.callee == "function" ? "Arguments" : m
                 }
             },
             f772: function(r, s, t) {
                 var o = t("5692"),
                     l = t("90e3"),
                     u = o("keys");
-                r.exports = function(f) {
-                    return u[f] || (u[f] = l(f))
+                r.exports = function(c) {
+                    return u[c] || (u[c] = l(c))
                 }
             },
             fb15: function(r, s, t) {
                 if (t.r(s), typeof window < "u") {
                     var o = window.document.currentScript; {
                         var l = t("8875");
                         o = l(), "currentScript" in document || Object.defineProperty(document, "currentScript", {
@@ -4440,40 +4440,40 @@
                         })
                     }
                     var u = o && o.src.match(/(.+\/)[^/]+\.js(\?.*)?$/);
                     u && (t.p = u[1])
                 }
                 t("99af"), t("4de4"), t("4160"), t("c975"), t("d81d"), t("a434"), t("159b"), t("a4d3"), t("e439"), t("dbb4"), t("b64b");
 
-                function f(S, b, x) {
+                function c(S, b, x) {
                     return b in S ? Object.defineProperty(S, b, {
                         value: x,
                         enumerable: !0,
                         configurable: !0,
                         writable: !0
                     }) : S[b] = x, S
                 }
 
-                function c(S, b) {
+                function f(S, b) {
                     var x = Object.keys(S);
                     if (Object.getOwnPropertySymbols) {
                         var A = Object.getOwnPropertySymbols(S);
                         b && (A = A.filter(function(V) {
                             return Object.getOwnPropertyDescriptor(S, V).enumerable
                         })), x.push.apply(x, A)
                     }
                     return x
                 }
 
                 function d(S) {
                     for (var b = 1; b < arguments.length; b++) {
                         var x = arguments[b] != null ? arguments[b] : {};
-                        b % 2 ? c(Object(x), !0).forEach(function(A) {
-                            f(S, A, x[A])
-                        }) : Object.getOwnPropertyDescriptors ? Object.defineProperties(S, Object.getOwnPropertyDescriptors(x)) : c(Object(x)).forEach(function(A) {
+                        b % 2 ? f(Object(x), !0).forEach(function(A) {
+                            c(S, A, x[A])
+                        }) : Object.getOwnPropertyDescriptors ? Object.defineProperties(S, Object.getOwnPropertyDescriptors(x)) : f(Object(x)).forEach(function(A) {
                             Object.defineProperty(S, A, Object.getOwnPropertyDescriptor(x, A))
                         })
                     }
                     return S
                 }
 
                 function v(S) {
@@ -4553,23 +4553,23 @@
                 function j(S, b, x) {
                     var A = x === 0 ? S.children[0] : S.children[x - 1].nextSibling;
                     S.insertBefore(b, A)
                 }
                 var P = t("dbf1");
                 t("13d5"), t("4fad"), t("ac1f"), t("5319");
 
-                function M(S) {
+                function w(S) {
                     var b = Object.create(null);
                     return function(A) {
                         var V = b[A];
                         return V || (b[A] = S(A))
                     }
                 }
                 var D = /-(\w)/g,
-                    R = M(function(S) {
+                    R = w(function(S) {
                         return S.replace(D, function(b, x) {
                             return x.toUpperCase()
                         })
                     });
                 t("5db7"), t("73d9");
                 var H = ["Start", "Add", "Remove", "Update", "End"],
                     F = ["Choose", "Unchoose", "Sort", "Filter", "Clone"],
@@ -4744,28 +4744,28 @@
                         }, {
                             key: "_isRootComponent",
                             get: function() {
                                 return this.externalComponent || this.rootTransition
                             }
                         }]), S
                     }(),
-                    Zt = t("8bbf");
+                    kt = t("8bbf");
 
-                function kt(S, b) {
+                function qt(S, b) {
                     var x = S[b];
                     return x ? x() : []
                 }
 
                 function Je(S) {
                     var b = S.$slots,
                         x = S.realList,
                         A = S.getKey,
                         V = x || [],
                         J = ["header", "footer"].map(function(Y) {
-                            return kt(b, Y)
+                            return qt(b, Y)
                         }),
                         _ = y(J, 2),
                         at = _[0],
                         yt = _[1],
                         Q = b.item;
                     if (!Q) throw new Error("draggable element must have an item slot");
                     var B = V.flatMap(function(Y, nt) {
@@ -4788,15 +4788,15 @@
 
                 function mn(S) {
                     var b = Ot(S),
                         x = !pt(S) && !b;
                     return {
                         transition: b,
                         externalComponent: x,
-                        tag: x ? Object(Zt.resolveComponent)(S) : b ? Zt.TransitionGroup : S
+                        tag: x ? Object(kt.resolveComponent)(S) : b ? kt.TransitionGroup : S
                     }
                 }
 
                 function Wt(S) {
                     var b = S.$slots,
                         x = S.tag,
                         A = S.realList,
@@ -4812,15 +4812,15 @@
                         root: _,
                         realList: A
                     })
                 }
 
                 function le(S, b) {
                     var x = this;
-                    Object(Zt.nextTick)(function() {
+                    Object(kt.nextTick)(function() {
                         return x.$emit(S.toLowerCase(), b)
                     })
                 }
 
                 function ye(S) {
                     var b = this;
                     return function(x, A) {
@@ -4870,15 +4870,15 @@
                             required: !1,
                             default: null
                         }
                     },
                     Ae = ["update:modelValue", "change"].concat(T([].concat(T(ot.manageAndEmit), T(ot.emit)).map(function(S) {
                         return S.toLowerCase()
                     }))),
-                    Re = Object(Zt.defineComponent)({
+                    Re = Object(kt.defineComponent)({
                         name: "draggable",
                         inheritAttrs: !1,
                         props: De,
                         emits: Ae,
                         data: function() {
                             return {
                                 error: !1
@@ -4900,17 +4900,17 @@
                                         getKey: _
                                     });
                                 this.componentStructure = at;
                                 var yt = st({
                                     $attrs: x,
                                     componentData: V
                                 });
-                                return at.render(Zt.h, yt)
+                                return at.render(kt.h, yt)
                             } catch (Q) {
-                                return this.error = !0, Object(Zt.h)("pre", {
+                                return this.error = !0, Object(kt.h)("pre", {
                                     style: {
                                         color: "red"
                                     }
                                 }, Q.stack)
                             }
                         },
                         created: function() {
@@ -4978,15 +4978,15 @@
                                 return this.componentStructure.getUnderlyingVm(b) || null
                             },
                             getUnderlyingPotencialDraggableComponent: function(b) {
                                 return b.__draggable_component__
                             },
                             emitChanges: function(b) {
                                 var x = this;
-                                Object(Zt.nextTick)(function() {
+                                Object(kt.nextTick)(function() {
                                     return x.$emit("change", b)
                                 })
                             },
                             alterList: function(b) {
                                 if (this.list) {
                                     b(this.list);
                                     return
@@ -5110,16 +5110,16 @@
                     we = Re;
                 s.default = we
             },
             fb6a: function(r, s, t) {
                 var o = t("23e7"),
                     l = t("861d"),
                     u = t("e8b5"),
-                    f = t("23cb"),
-                    c = t("50c4"),
+                    c = t("23cb"),
+                    f = t("50c4"),
                     d = t("fc6a"),
                     v = t("8418"),
                     p = t("b622"),
                     h = t("1dde"),
                     m = t("ae40"),
                     g = h("slice"),
                     y = m("slice", {
@@ -5133,20 +5133,20 @@
                 o({
                     target: "Array",
                     proto: !0,
                     forced: !g || !y
                 }, {
                     slice: function($, L) {
                         var I = d(this),
-                            j = c(I.length),
-                            P = f($, j),
-                            M = f(L === void 0 ? j : L, j),
+                            j = f(I.length),
+                            P = c($, j),
+                            w = c(L === void 0 ? j : L, j),
                             D, R, H;
-                        if (u(I) && (D = I.constructor, typeof D == "function" && (D === Array || u(D.prototype)) ? D = void 0 : l(D) && (D = D[O], D === null && (D = void 0)), D === Array || D === void 0)) return E.call(I, P, M);
-                        for (R = new(D === void 0 ? Array : D)(C(M - P, 0)), H = 0; P < M; P++, H++) P in I && v(R, H, I[P]);
+                        if (u(I) && (D = I.constructor, typeof D == "function" && (D === Array || u(D.prototype)) ? D = void 0 : l(D) && (D = D[O], D === null && (D = void 0)), D === Array || D === void 0)) return E.call(I, P, w);
+                        for (R = new(D === void 0 ? Array : D)(C(w - P, 0)), H = 0; P < w; P++, H++) P in I && v(R, H, I[P]);
                         return R.length = H, R
                     }
                 })
             },
             fc6a: function(r, s, t) {
                 var o = t("44ad"),
                     l = t("1d80");
@@ -5271,15 +5271,15 @@
         },
         emits: ["update:modelValue"],
         setup(a) {
             return (e, n) => (U(), W("label", Xi, [X("input", {
                 type: "checkbox",
                 checked: a.modelValue,
                 onInput: n[0] || (n[0] = i => e.$emit("update:modelValue", i.target.checked))
-            }, null, 40, Yi), zi, Qt(e.$slots, "default", {}, void 0, !0)]))
+            }, null, 40, Yi), zi, Zt(e.$slots, "default", {}, void 0, !0)]))
         }
     },
     or = ne(Ji, [
         ["__scopeId", "data-v-c95e23ce"]
     ]);
 const Qi = {
         class: "segmented-control"
@@ -5300,30 +5300,30 @@
                 class: We({
                     selected: a.modelValue === i
                 })
             }, [X("input", {
                 type: "radio",
                 onInput: r => e.$emit("update:modelValue", i),
                 checked: a.modelValue === i
-            }, null, 40, Zi), X("span", null, [Qt(e.$slots, "default", {
+            }, null, 40, Zi), X("span", null, [Zt(e.$slots, "default", {
                 option: i
             }, () => [Bt(it(i), 1)], !0)])], 2))), 128))]))
         }
     },
     qi = ne(ki, [
         ["__scopeId", "data-v-3ae3bbf6"]
     ]),
     _i = {
         props: ["parameter", "modelValue"],
         emits: ["update:modelValue"]
     },
     tl = ["value", "min", "max"];
 
 function el(a, e, n, i, r, s) {
-    return U(), W(bt, null, [Qt(a.$slots, "default"), X("input", Te({
+    return U(), W(bt, null, [Zt(a.$slots, "default"), X("input", Te({
         type: "number"
     }, a.$attrs, {
         value: n.modelValue,
         onInput: e[0] || (e[0] = t => a.$emit("update:modelValue", t.target.value)),
         min: n.parameter.min,
         max: n.parameter.max,
         step: 1
@@ -5335,15 +5335,15 @@
     nl = {
         props: ["parameter", "modelValue"],
         emits: ["update:modelValue"]
     },
     rl = ["value", "min", "max", "step"];
 
 function ol(a, e, n, i, r, s) {
-    return U(), W(bt, null, [Qt(a.$slots, "default"), X("input", Te({
+    return U(), W(bt, null, [Zt(a.$slots, "default"), X("input", Te({
         type: "number"
     }, a.$attrs, {
         value: n.modelValue,
         onInput: e[0] || (e[0] = t => a.$emit("update:modelValue", t.target.value)),
         min: n.parameter.min,
         max: n.parameter.max,
         step: .1
@@ -5357,15 +5357,15 @@
         emits: ["update:modelValue"]
     },
     il = ["value"],
     ll = ["value"],
     sl = ["value"];
 
 function ul(a, e, n, i, r, s) {
-    return U(), W(bt, null, [Qt(a.$slots, "default"), n.parameter.allowed_values ? (U(), W("select", Te({
+    return U(), W(bt, null, [Zt(a.$slots, "default"), n.parameter.allowed_values ? (U(), W("select", Te({
         key: 0
     }, a.$attrs, {
         value: n.modelValue,
         onInput: e[0] || (e[0] = t => a.$emit("update:modelValue", t.target.value))
     }), [(U(!0), W(bt, null, Gt(n.parameter.allowed_values, t => (U(), W("option", {
         value: t,
         key: t
@@ -5380,22 +5380,22 @@
 const Wn = ne(al, [
         ["render", ul]
     ]),
     fl = {
         props: ["parameter", "modelValue"],
         emits: ["update:modelValue"]
     },
-    cl = ["value"];
+    cl = ["checked"];
 
 function dl(a, e, n, i, r, s) {
-    return U(), W(bt, null, [Qt(a.$slots, "default"), X("input", Te({
+    return U(), W(bt, null, [Zt(a.$slots, "default"), X("input", Te({
         type: "checkbox"
     }, a.$attrs, {
-        value: n.modelValue,
-        onInput: e[0] || (e[0] = t => a.$emit("update:modelValue", t.target.value))
+        checked: n.modelValue,
+        onInput: e[0] || (e[0] = t => a.$emit("update:modelValue", t.target.checked))
     }), null, 16, cl)], 64)
 }
 const Xn = ne(fl, [
         ["render", dl]
     ]),
     vl = {
         class: "property-list"
@@ -5409,15 +5409,15 @@
             const e = {
                     int: Kn,
                     float: Hn,
                     str: Wn,
                     bool: Xn
                 },
                 n = Ln();
-            return (i, r) => (U(), W("fieldset", vl, [X("legend", null, [Qt(i.$slots, "default")]), (U(!0), W(bt, null, Gt(a.parameter.parameters || [], (s, t) => (U(), W("div", {
+            return (i, r) => (U(), W("fieldset", vl, [X("legend", null, [Zt(i.$slots, "default")]), (U(!0), W(bt, null, Gt(a.parameter.parameters || [], (s, t) => (U(), W("div", {
                 key: t
             }, [(U(), ce(Xe(e[s.type]), {
                 id: `tuple-${K(n)}-${t}`,
                 parameter: s,
                 modelValue: a.modelValue[t],
                 "onUpdate:modelValue": o => i.$emit("update:modelValue", [...a.modelValue.slice(0, t), o, ...a.modelValue.slice(t + 1)])
             }, {
@@ -5444,15 +5444,15 @@
                     tuple: wr,
                     list: void 0
                 };
 
             function i(r) {
                 return e.modelValue.indexOf(r).toString()
             }
-            return (r, s) => (U(), W("fieldset", null, [X("legend", null, [Qt(r.$slots, "default", {}, void 0, !0)]), Tt(K(Nn), {
+            return (r, s) => (U(), W("fieldset", null, [X("legend", null, [Zt(r.$slots, "default", {}, void 0, !0)]), Tt(K(Nn), {
                 tag: "ol",
                 class: "parameter-list",
                 "item-key": i,
                 modelValue: e.modelValue,
                 "onUpdate:modelValue": s[1] || (s[1] = t => r.$emit("update:modelValue", t))
             }, {
                 item: Nt(({
@@ -5515,15 +5515,15 @@
                 n = Ln();
             return (i, r) => {
                 var s;
                 return U(), W("li", null, [X("details", {
                     class: "property-list",
                     onToggle: r[1] || (r[1] = t => i.$emit("update:open", t.target.open)),
                     open: a.open
-                }, [X("summary", null, [Qt(i.$slots, "header")]), K(Rr)(a.modelValue) ? (U(), W("div", bl, [X("label", {
+                }, [X("summary", null, [Zt(i.$slots, "header")]), K(Rr)(a.modelValue) ? (U(), W("div", bl, [X("label", {
                     for: `step-${K(n)}-column`
                 }, "Column", 8, Sl), X("select", {
                     id: `step-${K(n)}-column`,
                     value: a.modelValue.language,
                     onInput: r[0] || (r[0] = t => i.$emit("update:modelValue", {
                         ...a.modelValue,
                         language: t.target.value
@@ -5544,15 +5544,15 @@
                         }
                     })
                 }, {
                     default: Nt(() => [X("label", {
                         for: `step-${K(n)}-${o}`
                     }, it(o), 9, xl)]),
                     _: 2
-                }, 1032, ["id", "parameter", "modelValue", "onUpdate:modelValue"])), t.help ? (U(), W("small", Ol, it(t.help), 1)) : _t("", !0)]))), 128)), X("footer", null, [Qt(i.$slots, "footer")])], 40, yl)])
+                }, 1032, ["id", "parameter", "modelValue", "onUpdate:modelValue"])), t.help ? (U(), W("small", Ol, it(t.help), 1)) : _t("", !0)]))), 128)), X("footer", null, [Zt(i.$slots, "footer")])], 40, yl)])
             }
         }
     };
 
 function Mr(a, e, n = {
     equals(i, r) {
         return i == r
@@ -5570,26 +5570,26 @@
         l = ar(n, o[0], e, a, 0);
     if (o[0].newPos + 1 >= i && l + 1 >= r) return [{
         value: e,
         count: e.length
     }];
     for (s = 1; s <= t; ++s)
         for (let u = -1 * s; u <= s; u += 2) {
-            let f, c = o[u - 1],
+            let c, f = o[u - 1],
                 d = o[u + 1],
                 v = (d ? d.newPos : 0) - u;
-            c && (o[u - 1] = void 0);
-            let p = c && c.newPos + 1 < i,
+            f && (o[u - 1] = void 0);
+            let p = f && f.newPos + 1 < i,
                 h = d && 0 <= v && v < r;
             if (!p && !h) {
                 o[u] = void 0;
                 continue
             }
-            if (!p || h && c.newPos < d.newPos ? (f = Pl(d), ir(f.components, void 0, !0)) : (f = c, f.newPos++, ir(f.components, !0, void 0)), v = ar(n, f, e, a, u), f.newPos + 1 >= i && v + 1 >= r) return Il(n, f.components, e, a);
-            o[u] = f
+            if (!p || h && f.newPos < d.newPos ? (c = Pl(d), ir(c.components, void 0, !0)) : (c = f, c.newPos++, ir(c.components, !0, void 0)), v = ar(n, c, e, a, u), c.newPos + 1 >= i && v + 1 >= r) return Il(n, c.components, e, a);
+            o[u] = c
         }
 }
 
 function ar({
     equals: a
 }, e, n, i, r) {
     let s = n.length,
@@ -5621,29 +5621,29 @@
     useLongestToken: e
 }, n, i, r) {
     let s = 0,
         t = n.length,
         o = 0,
         l = 0;
     for (; s < t; s++) {
-        let f = n[s];
-        if (f.removed) {
-            if (f.value = r.slice(l, l + f.count), l += f.count, s && n[s - 1].added) {
-                let c = n[s - 1];
-                n[s - 1] = n[s], n[s] = c
+        let c = n[s];
+        if (c.removed) {
+            if (c.value = r.slice(l, l + c.count), l += c.count, s && n[s - 1].added) {
+                let f = n[s - 1];
+                n[s - 1] = n[s], n[s] = f
             }
         } else {
-            if (!f.added && e) {
-                let c = i.slice(o, o + f.count);
-                c = c.map(function(d, v) {
+            if (!c.added && e) {
+                let f = i.slice(o, o + c.count);
+                f = f.map(function(d, v) {
                     let p = r[l + v];
                     return p.length > d.length ? p : d
-                }), f.value = c
-            } else f.value = i.slice(o, o + f.count);
-            o += f.count, f.added || (l += f.count)
+                }), c.value = f
+            } else c.value = i.slice(o, o + c.count);
+            o += c.count, c.added || (l += c.count)
         }
     }
     let u = n[t - 1];
     return t > 1 && typeof u.value == "string" && (u.added || u.removed) && a("", u.value) && (n[t - 2].value += u.value, n.pop()), n
 }
 
 function Pl(a) {
@@ -5673,23 +5673,23 @@
             continue
         }
         for (u = l + 1; u < s[o].value.length && !r(e[t + u], s[o].value[u]); ++u);
         if (console.assert(u <= s[o].value.length), l > 0 && (s.splice(o, 0, {
                 count: l,
                 value: s[o].value.slice(0, l)
             }), ++o), s[o].value = s[o].value.slice(l), s[o].count = u - l, s[o].changed = !0, u - l < s[o].value.length) {
-            const f = s[o].value.length - (u - l);
+            const c = s[o].value.length - (u - l);
             s.splice(o + 1, 0, {
-                count: f,
+                count: c,
                 value: s[o].value.slice(u - l)
             }), s[o].value = s[o].value.slice(0, u - l)
         }
-        console.assert(s[o].value.every((f, c) => !r(e[t + l + c], f))), s[o].differences = s[o].value.map((f, c) => ({
-            previous: e[t + l + c],
-            current: f
+        console.assert(s[o].value.every((c, f) => !r(e[t + l + f], c))), s[o].differences = s[o].value.map((c, f) => ({
+            previous: e[t + l + f],
+            current: c
         })), t += u
     }
     return s
 }
 const Dl = {
         key: 0
     },
@@ -5708,15 +5708,15 @@
                 required: !0
             }
         },
         setup(a) {
             const {
                 current: e,
                 previous: n
-            } = a, i = qt(() => Mr(n.split(""), e.split(""), {
+            } = a, i = Qt(() => Mr(n.split(""), e.split(""), {
                 equals: (r, s) => r == s,
                 maxEditLength: Math.max(n.length, e.length) * .5
             }));
             return (r, s) => K(i) ? (U(), W("span", Al, [(U(!0), W(bt, null, Gt(K(i), t => (U(), W(bt, null, [t.added || t.removed ? (U(), ce(Xe(t.added ? "ins" : "del"), {
                 key: 0
             }, {
                 default: Nt(() => [Bt(it(t.value.join("")), 1)]),
@@ -5770,17 +5770,17 @@
                 type: Boolean,
                 default: !1
             }
         },
         setup(a) {
             const e = a,
                 n = zt(),
-                i = qt(() => e.refRows !== null),
-                r = qt(() => pn(e.refRows !== null ? Cl(e.languages, e.refRows, e.rows) : [])),
-                s = qt(() => {
+                i = Qt(() => e.refRows !== null),
+                r = Qt(() => pn(e.refRows !== null ? Cl(e.languages, e.refRows, e.rows) : [])),
+                s = Qt(() => {
                     let p = 0,
                         h = 0,
                         m = 0;
                     return r.value.forEach(({
                         added: g,
                         removed: y,
                         changed: O,
@@ -5834,27 +5834,27 @@
                     changed: "yellow"
                 };
                 n.value.querySelectorAll("tbody tr:is(.added, .removed, .changed)").forEach(E => {
                     m.fillStyle = O[E.className], m.fillRect(0, E.offsetTop / h * p, g, Math.max(E.offsetHeight / h * p, 1))
                 })
             }
             cr(u);
-            const f = new ResizeObserver(u);
-            jn(() => f.observe(n.value)), ur(() => f.unobserve(n.value));
-            const c = {
+            const c = new ResizeObserver(u);
+            jn(() => c.observe(n.value)), ur(() => c.unobserve(n.value));
+            const f = {
                     "\xA0": "\u2423",
                     "\u202F": "\u2423",
                     "\u2007": "\u2423",
                     "\u2060": "\u2423",
                     " ": "\xB7"
                 },
-                d = new RegExp(Object.keys(c).join("|"), "g");
+                d = new RegExp(Object.keys(f).join("|"), "g");
 
             function v(p) {
-                return e.displayWhitespace ? p.replace(d, h => c[h]) : p
+                return e.displayWhitespace ? p.replace(d, h => f[h]) : p
             }
             return (p, h) => (U(), W("div", wl, [X("div", {
                 ref_key: "outputElement",
                 ref: n,
                 class: We(["sample", {
                     "display-as-rows": e.displayAsRows
                 }])
@@ -5894,15 +5894,15 @@
                 width: "16"
             }, null, 512)], 2)]))
         }
     },
     Bl = ne(Gl, [
         ["__scopeId", "data-v-7fccf6d5"]
     ]);
-const Kl = a => ($n("data-v-d9732d88"), a = a(), Fn(), a),
+const Kl = a => ($n("data-v-b2568139"), a = a(), Fn(), a),
     Hl = {
         class: "clean-corpus-container"
     },
     Wl = {
         class: "output-panel"
     },
     Xl = {
@@ -5955,41 +5955,43 @@
         __name: "FilterEditor",
         props: {
             dataset: Object
         },
         setup(a) {
             const {
                 dataset: e
-            } = a, n = navigator.platform.match(/^(Mac|iPhone$)/) ? "Meta" : "Control", i = 1e3, r = zt(!1), s = zt(!1), t = ["original", "clean", "changes"], o = zt("clean"), l = zt(!1), u = Hi(), f = Ja(e), c = qt(() => {
-                if (!(e != null && e.columns)) return [];
-                const P = Array.from(Object.keys(e.columns)).sort();
-                return e.name.includes(P.reverse().join("-")) || P.reverse(), P
-            }), d = zt([]), v = qt(() => d.value.length > 0 ? d.value[d.value.length - 1] : null), p = qt(() => d.value.length > 0 ? d.value[0] : null);
-            async function h(P, M, {
+            } = a, n = navigator.platform.match(/^(Mac|iPhone$)/) ? "Meta" : "Control", i = 1e3, r = zt(!1), s = zt(!1), t = ["original", "clean", "changes"], o = zt("clean"), l = zt(!1), u = Qt(() => ((e == null ? void 0 : e.columns) || []).map(({
+                lang: P
+            }) => P)), c = Qt(() => {
+                var w;
+                let P = Hi().value || [];
+                return ((w = u.value) == null ? void 0 : w.length) === 1 && (P = P.filter(D => D.type === "monolingual")), P
+            }), f = Ja(e), d = zt([]), v = Qt(() => d.value.length > 0 ? d.value[d.value.length - 1] : null), p = Qt(() => d.value.length > 0 ? d.value[0] : null);
+            async function h(P, w, {
                 signal: D
             }) {
                 l.value = !0, d.value = [];
                 try {
                     const R = Bi(`/api/datasets/${encodeURIComponent(P.name)}/sample`, {
                         method: "POST",
                         signal: D,
                         headers: {
                             "Content-Type": "application/json",
                             Accept: "application/json"
                         },
-                        body: JSON.stringify(M, null, 2)
+                        body: JSON.stringify(w, null, 2)
                     });
                     for await (let H of R) D.aborted || d.value.push(pn(H))
                 } catch (R) {
                     if (R.toString().indexOf("The operation was aborted") === -1 && R.toString().indexOf("The user aborted a request") === -1) throw R
                 } finally {
                     l.value = !1
                 }
             }
-            vr([f.steps, e], (P, M, D) => {
+            vr([f.steps, e], (P, w, D) => {
                 const R = () => {
                     const H = new AbortController;
                     D(() => H.abort()), h(e, f.steps.value, H)
                 };
                 if (d.value.length === 0) R();
                 else {
                     const H = setTimeout(R, i);
@@ -6001,56 +6003,56 @@
 
             function m(P) {
                 return {
                     id: Ln(),
                     filter: P.name,
                     language: Rr({
                         filter: P.name
-                    }) ? c.value[0] : null,
-                    parameters: Object.fromEntries(Object.entries(P.parameters).map(([M, D]) => [M, hr(D)]))
+                    }) ? u.value[0] : null,
+                    parameters: Object.fromEntries(Object.entries(P.parameters).map(([w, D]) => [w, hr(D)]))
                 }
             }
 
             function g(P) {
-                const M = m(P);
-                f.update([...f.steps.value, M]), j.get(M).value = !0
+                const w = m(P);
+                f.update([...f.steps.value, w]), j.get(w).value = !0
             }
 
             function y(P) {
                 f.update([...f.steps.value.slice(0, P), ...f.steps.value.slice(P + 1)])
             }
 
-            function O(P, M) {
-                f.update([...f.steps.value.slice(0, P), M, ...f.steps.value.slice(P + 1)])
+            function O(P, w) {
+                f.update([...f.steps.value.slice(0, P), w, ...f.steps.value.slice(P + 1)])
             }
 
-            function E(P, M) {
-                P.setData("text/plain", JSON.stringify(m(M.__draggable_context.element), null, 2))
+            function E(P, w) {
+                P.setData("text/plain", JSON.stringify(m(w.__draggable_context.element), null, 2))
             }
 
-            function C(P, M) {
-                P.setData("text/plain", JSON.stringify(M.__draggable_context.element, null, 2))
+            function C(P, w) {
+                P.setData("text/plain", JSON.stringify(w.__draggable_context.element, null, 2))
             }
 
             function T(P) {
                 return d.value.length < P + 1 ? "pending" : d.value.length === P + 1 ? "loading" : d.value[P + 1].returncode === 0 ? "loaded" : "failed"
             }
 
-            function $(P, M) {
-                return M.length === 0 ? P : P.filter(({
+            function $(P, w) {
+                return w.length === 0 ? P : P.filter(({
                     name: D,
                     description: R
-                }) => D.toLowerCase().indexOf(M.toLowerCase()) !== -1 || R && R.toLowerCase().indexOf(M.toLowerCase()) !== -1)
+                }) => D.toLowerCase().indexOf(w.toLowerCase()) !== -1 || R && R.toLowerCase().indexOf(w.toLowerCase()) !== -1)
             }
             zt();
-            const L = qt(() => {
-                var P, M;
+            const L = Qt(() => {
+                var P, w;
                 return {
                     original: d.value.length > 0 ? (P = d.value[0].stdout) == null ? void 0 : P.length : null,
-                    clean: d.value.length === f.steps.value.length + 1 ? (M = d.value[f.steps.value.length].stdout) == null ? void 0 : M.length : null,
+                    clean: d.value.length === f.steps.value.length + 1 ? (w = d.value[f.steps.value.length].stdout) == null ? void 0 : w.length : null,
                     changes: null
                 }
             });
 
             function I(P) {
                 (n === "Meta" ? P.metaKey : P.ctrlKey) && P.keyCode === 90 && (P.shiftKey ? f.canRedo.value && f.redo() : f.canUndo.value && f.undo(), P.preventDefault())
             }
@@ -6063,58 +6065,58 @@
                 constructor() {
                     this.map = new Map
                 }
                 get(P) {
                     return this.map.has(P.id) || this.map.set(P.id, zt(!1)), this.map.get(P.id)
                 }
             };
-            return (P, M) => {
+            return (P, w) => {
                 var D, R, H, F;
                 return U(), W("div", Hl, [X("div", Wl, [X("header", Xl, [Tt(or, {
                     modelValue: r.value,
-                    "onUpdate:modelValue": M[0] || (M[0] = N => r.value = N)
+                    "onUpdate:modelValue": w[0] || (w[0] = N => r.value = N)
                 }, {
                     default: Nt(() => [Bt("Display as rows")]),
                     _: 1
                 }, 8, ["modelValue"]), Tt(or, {
                     modelValue: s.value,
-                    "onUpdate:modelValue": M[1] || (M[1] = N => s.value = N)
+                    "onUpdate:modelValue": w[1] || (w[1] = N => s.value = N)
                 }, {
                     default: Nt(() => [Bt("Display whitespace")]),
                     _: 1
                 }, 8, ["modelValue"]), X("div", Yl, [X("button", {
                     class: "icon-button",
                     title: "Undo",
-                    onClick: M[2] || (M[2] = N => K(f).undo()),
+                    onClick: w[2] || (w[2] = N => K(f).undo()),
                     disabled: !K(f).canUndo.value
                 }, [Tt(K(Ha))], 8, zl), X("button", {
                     class: "icon-button",
                     title: "Redo",
-                    onClick: M[3] || (M[3] = N => K(f).redo()),
+                    onClick: w[3] || (w[3] = N => K(f).redo()),
                     disabled: !K(f).canRedo.value
                 }, [Tt(K(Wa))], 8, Jl)]), Tt(qi, {
                     class: "table-buttons",
                     modelValue: o.value,
-                    "onUpdate:modelValue": M[4] || (M[4] = N => o.value = N),
+                    "onUpdate:modelValue": w[4] || (w[4] = N => o.value = N),
                     options: t
                 }, {
                     default: Nt(({
                         option: N
                     }) => [Bt(it(N) + " ", 1), K(L)[N] !== null ? (U(), W("small", Ql, it(K(L)[N]), 1)) : _t("", !0)]),
                     _: 1
                 }, 8, ["modelValue"])]), X("div", Zl, [Tt(Bl, {
                     class: "filter-output-table",
-                    languages: K(c),
+                    languages: K(u),
                     rows: o.value === "original" ? (D = K(p)) == null ? void 0 : D.stdout : (R = K(v)) == null ? void 0 : R.stdout,
                     "ref-rows": o.value === "changes" ? (H = K(p)) == null ? void 0 : H.stdout : null,
                     "display-as-rows": r.value,
                     "display-whitespace": s.value
                 }, null, 8, ["languages", "rows", "ref-rows", "display-as-rows", "display-whitespace"]), (F = K(v)) != null && F.stderr ? (U(), W("div", kl, [X("pre", null, it(K(v).stderr), 1)])) : _t("", !0)])]), X("div", ql, [X("div", _l, [Tt(K(ka), {
                     filter: $,
-                    options: K(u),
+                    options: K(c),
                     label: "name",
                     placeholder: "Search filters\u2026",
                     "onOption:selected": g
                 }, {
                     option: Nt(({
                         name: N,
                         description: k
@@ -6124,28 +6126,28 @@
                     }, [Bt(it(N), 1), es, X("small", null, it(k), 1)], 8, ts)]),
                     _: 1
                 }, 8, ["options"])]), Tt(K(Nn), {
                     tag: "ol",
                     class: "filter-steps",
                     "item-key": "id",
                     modelValue: K(f).steps.value,
-                    "onUpdate:modelValue": M[5] || (M[5] = N => K(f).update(N)),
+                    "onUpdate:modelValue": w[5] || (w[5] = N => K(f).update(N)),
                     group: {
                         name: "filters"
                     },
                     "multi-drag": !0,
                     "set-data": C,
                     "multi-drag-key": K(n)
                 }, {
                     item: Nt(({
                         element: N,
                         index: k
                     }) => [Tt(Tl, {
                         class: "filter-step",
-                        languages: K(c),
+                        languages: K(u),
                         modelValue: N,
                         "onUpdate:modelValue": ot => O(k, ot),
                         open: K(j).get(N).value,
                         "onUpdate:open": ot => K(j).get(N).value = ot
                     }, {
                         header: Nt(() => {
                             var ot, St;
@@ -6162,16 +6164,16 @@
                         }),
                         _: 2
                     }, 1032, ["languages", "modelValue", "onUpdate:modelValue", "open", "onUpdate:open"])]),
                     _: 1
                 }, 8, ["modelValue", "multi-drag-key"]), Tt(K(Nn), {
                     tag: "ul",
                     class: "available-filters",
-                    modelValue: K(u),
-                    "onUpdate:modelValue": M[6] || (M[6] = N => lr(u) ? u.value = N : null),
+                    modelValue: K(c),
+                    "onUpdate:modelValue": w[6] || (w[6] = N => lr(c) ? c.value = N : null),
                     "item-key": "name",
                     group: {
                         name: "filters",
                         pull: "clone",
                         put: !1
                     },
                     sort: !1,
@@ -6190,24 +6192,24 @@
                     }, [Tt(K(pr))], 8, ss)]), X("p", null, it(N.description), 1)])])]),
                     _: 1
                 }, 8, ["modelValue"])])])
             }
         }
     },
     fs = ne(us, [
-        ["__scopeId", "data-v-d9732d88"]
+        ["__scopeId", "data-v-b2568139"]
     ]);
 const cs = {
         class: "filter-editor"
     },
     ds = {
         __name: "EditFiltersView",
         setup(a) {
             const e = Ya(),
-                n = qt(() => Za(e.params.datasetName));
+                n = Qt(() => Za(e.params.datasetName));
             return (i, r) => {
                 const s = dr("RouterLink");
                 return U(), W("div", cs, [X("header", null, [X("h2", null, [Bt("Dataset: "), X("em", null, it(K(n).name), 1)]), Tt(Qa, {
                     dataset: K(n)
                 }, null, 8, ["dataset"])]), K(n) ? (U(), ce(fs, {
                     key: 0,
                     dataset: K(n)
```

### Comparing `opuscleaner-0.2.2/opuscleaner/frontend/assets/ListDatasetsView.0c61d7cc.js` & `opuscleaner-0.3.0/opuscleaner/frontend/assets/ListDatasetsView.576d1862.js`

 * *Files 17% similar despite different names*

#### js-beautify {}

```diff
@@ -1,136 +1,137 @@
 import {
-    _ as g,
+    _ as f,
     o,
     c as n,
-    a as y,
-    b as s,
-    w as i,
+    a as g,
+    b as a,
+    w as c,
     u as e,
-    R as c,
-    T as b,
+    R as i,
+    T as y,
     d as t,
-    F as k,
+    F as b,
     r as w,
     e as I,
     f as _,
-    U as v,
+    U as k,
     t as u,
-    C as N,
-    g as D,
-    P as S,
-    p as V,
-    h as x
-} from "./index.6cc31f0d.js";
+    C as v,
+    g as N,
+    P as D,
+    p as S,
+    h as V
+} from "./index.aa84b8f1.js";
 import {
-    g as h,
-    T as C,
-    a as F
-} from "./TagsEditor.23cf196f.js";
-import "./hacks.1ae1ba64.js";
-const L = "/frontend/assets/data-cuate.84693c76.svg";
-const d = l => (V("data-v-45560305"), l = l(), x(), l),
-    T = {
+    g as m,
+    T as x,
+    a as C
+} from "./TagsEditor.3f956450.js";
+import "./hacks.175c31f5.js";
+const F = "/frontend/assets/data-cuate.84693c76.svg";
+const d = l => (S("data-v-1788c3f7"), l = l(), V(), l),
+    L = {
         class: "table-container-first-screen"
     },
-    B = d(() => t("h2", {
+    T = d(() => t("h2", {
         class: "table-title"
     }, "Your datasets", -1)),
-    E = {
+    B = {
         key: 0,
         class: "datasets-table"
     },
-    R = d(() => t("thead", null, [t("tr", null, [t("th", null, "Name"), t("th", null, "Languages"), t("th", null, "Categories"), t("th", null, "Filter steps"), t("th", null, "Actions")])], -1)),
-    j = {
+    E = d(() => t("thead", null, [t("tr", null, [t("th", null, "Name"), t("th", null, "Languages"), t("th", null, "Categories"), t("th", null, "Filter steps"), t("th", null, "Actions")])], -1)),
+    R = {
         class: "tags"
     },
     P = {
         class: "filter-steps"
     },
     U = {
         key: 1,
         class: "illustration-container"
     },
-    A = ["src"],
-    O = d(() => t("p", null, "No datasets yet. Click on the import data button on the right to get started.", -1)),
+    j = ["src"],
+    A = d(() => t("p", null, "No datasets yet. Click on the import data button on the right to get started.", -1)),
     Y = d(() => t("p", {
         class: "credits"
     }, [_("Image by "), t("a", {
         href: "https://www.freepik.com/free-vector/no-data-concept-illustration_8961448.htm",
         target: "_blank"
     }, "storyset on Freepik"), _(".")], -1)),
     q = {
         __name: "ListDatasetsView",
         setup(l) {
-            function f(r) {
-                const p = Object.keys((r == null ? void 0 : r.columns) || {}),
-                    a = new Intl.DisplayNames([], {
-                        type: "language"
-                    });
-                return p.map(m => {
+            function h(r) {
+                const p = new Intl.DisplayNames([], {
+                    type: "language"
+                });
+                return ((r == null ? void 0 : r.columns) || []).map(({
+                    lang: s
+                }) => {
                     try {
-                        return a.of(m.replace("_", "-"))
+                        return p.of(s.replace("_", "-"))
                     } catch {
-                        return m
+                        return s
                     }
                 })
             }
-            return (r, p) => (o(), n("div", T, [(o(), y(b, {
+            return (r, p) => (o(), n("div", L, [(o(), g(y, {
                 to: ".navbar"
-            }, [s(e(c), {
+            }, [a(e(i), {
                 class: "import-data-button",
                 to: {
                     name: "add-dataset"
                 }
             }, {
-                default: i(() => [_(" Import dataset "), s(e(v), {
+                default: c(() => [_(" Import dataset "), a(e(k), {
                     class: "import-data-icon"
                 })]),
                 _: 1
-            })])), B, e(h)().length > 0 ? (o(), n("table", E, [R, t("tbody", null, [(o(!0), n(k, null, w(e(h)(), a => (o(), n("tr", {
-                key: a.id
-            }, [t("td", null, u(a.name), 1), t("td", null, u(f(a).join("\u2013")), 1), t("td", j, [s(C, {
-                dataset: a
-            }, null, 8, ["dataset"])]), t("td", P, u(e(F)(a).steps.value.length), 1), t("td", null, [s(e(c), {
+            })])), T, e(m)().length > 0 ? (o(), n("table", B, [E, t("tbody", null, [(o(!0), n(b, null, w(e(m)(), s => (o(), n("tr", {
+                key: s.id
+            }, [t("td", null, u(s.name), 1), t("td", null, u(h(s).join("\u2013")), 1), t("td", R, [a(x, {
+                dataset: s
+            }, null, 8, ["dataset"])]), t("td", P, u(e(C)(s).steps.value.length), 1), t("td", null, [a(e(i), {
                 class: "icon-button",
                 title: "Show filter yaml",
                 to: {
                     name: "edit-filters-yaml",
                     params: {
-                        datasetName: a.name,
+                        datasetName: s.name,
                         format: "configuration-for-opusfilter.yaml"
                     }
                 }
             }, {
-                default: i(() => [s(e(N))]),
+                default: c(() => [a(e(v))]),
                 _: 2
-            }, 1032, ["to"]), s(e(c), {
+            }, 1032, ["to"]), a(e(i), {
                 class: "icon-button",
                 title: "Edit filters",
                 to: {
                     name: "edit-filters",
                     params: {
-                        datasetName: a.name
+                        datasetName: s.name
                     }
                 }
             }, {
-                default: i(() => [s(e(D))]),
+                default: c(() => [a(e(N))]),
                 _: 2
-            }, 1032, ["to"]), s(e(c), {
+            }, 1032, ["to"]), a(e(i), {
                 class: "icon-button",
                 title: "Show dataset statistics",
                 to: {}
             }, {
-                default: i(() => [s(e(S))]),
+                default: c(() => [a(e(D))]),
                 _: 1
             })])]))), 128))])])) : (o(), n("div", U, [t("img", {
-                src: e(L)
-            }, null, 8, A), O, Y])), s(e(I))]))
+                src: e(F)
+            }, null, 8, j), A, Y])), a(e(I))]))
         }
     },
-    K = g(q, [
-        ["__scopeId", "data-v-45560305"]
+    K = f(q, [
+        ["__scopeId", "data-v-1788c3f7"]
     ]);
 export {
     K as
     default
 };
```

### Comparing `opuscleaner-0.2.2/opuscleaner/frontend/assets/TagsEditor.23cf196f.js` & `opuscleaner-0.3.0/opuscleaner/frontend/assets/TagsEditor.3f956450.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -38,18 +38,18 @@
     y as Z,
     T as ee,
     p as te,
     h as se,
     b as T,
     z as ae,
     E as ne
-} from "./index.6cc31f0d.js";
+} from "./index.aa84b8f1.js";
 import {
     g as ie
-} from "./hacks.1ae1ba64.js";
+} from "./hacks.175c31f5.js";
 
 function oe(t, e, s) {
     const a = new Map(t.map(i => [s(i), i])),
         o = e.map(i => a.has(s(i)) ? Object.assign(a.get(s(i)), i) : i);
     t.splice(0, t.length, ...o)
 }
 const w = v([]);
```

### Comparing `opuscleaner-0.2.2/opuscleaner/frontend/assets/TagsEditor.ccc03a15.css` & `opuscleaner-0.3.0/opuscleaner/frontend/assets/TagsEditor.ccc03a15.css`

 * *Files identical despite different names*

### Comparing `opuscleaner-0.2.2/opuscleaner/frontend/assets/data-cuate.84693c76.svg` & `opuscleaner-0.3.0/opuscleaner/frontend/assets/data-cuate.84693c76.svg`

 * *Files identical despite different names*

### Comparing `opuscleaner-0.2.2/opuscleaner/frontend/assets/datailor-logo.fbfa6008.svg` & `opuscleaner-0.3.0/opuscleaner/frontend/assets/datailor-logo.fbfa6008.svg`

 * *Files identical despite different names*

### Comparing `opuscleaner-0.2.2/opuscleaner/frontend/assets/eu.24cff2c1.png` & `opuscleaner-0.3.0/opuscleaner/frontend/assets/eu.24cff2c1.png`

 * *Files identical despite different names*

### Comparing `opuscleaner-0.2.2/opuscleaner/frontend/assets/horizon-europe.80625b0c.png` & `opuscleaner-0.3.0/opuscleaner/frontend/assets/horizon-europe.80625b0c.png`

 * *Files identical despite different names*

### Comparing `opuscleaner-0.2.2/opuscleaner/frontend/assets/index.47848488.css` & `opuscleaner-0.3.0/opuscleaner/frontend/assets/index.47848488.css`

 * *Files identical despite different names*

### Comparing `opuscleaner-0.2.2/opuscleaner/frontend/assets/index.6cc31f0d.js` & `opuscleaner-0.3.0/opuscleaner/frontend/assets/index.aa84b8f1.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -7043,32 +7043,32 @@
         ["__scopeId", "data-v-1e8f5c6b"]
     ]),
     Lf = uf({
         history: Pu("/frontend/"),
         routes: [{
             path: "/",
             name: "list-datasets",
-            component: () => Un(() => import("./ListDatasetsView.0c61d7cc.js"), ["assets/ListDatasetsView.0c61d7cc.js", "assets/ListDatasetsView.79aac80d.css", "assets/TagsEditor.23cf196f.js", "assets/TagsEditor.ccc03a15.css", "assets/hacks.1ae1ba64.js"]),
+            component: () => Un(() => import("./ListDatasetsView.576d1862.js"), ["assets/ListDatasetsView.576d1862.js", "assets/ListDatasetsView.b8eb7e79.css", "assets/TagsEditor.3f956450.js", "assets/TagsEditor.ccc03a15.css", "assets/hacks.175c31f5.js"]),
             children: [{
                 name: "edit-filters-yaml",
                 path: "/datasets/:datasetName/:format",
                 component: Nf,
                 props: {
-                    component: () => Un(() => import("./EditFiltersYamlView.28a1a7c9.js"), ["assets/EditFiltersYamlView.28a1a7c9.js", "assets/hacks.1ae1ba64.js"]),
+                    component: () => Un(() => import("./EditFiltersYamlView.5763c641.js"), ["assets/EditFiltersYamlView.5763c641.js", "assets/hacks.175c31f5.js"]),
                     format: "configuration-for-opusfilter.yaml"
                 }
             }]
         }, {
             path: "/datasets/:datasetName/configuration",
             name: "edit-filters",
-            component: () => Un(() => import("./EditFiltersView.bc0dd7c3.js"), ["assets/EditFiltersView.bc0dd7c3.js", "assets/EditFiltersView.a7795492.css", "assets/TagsEditor.23cf196f.js", "assets/TagsEditor.ccc03a15.css", "assets/hacks.1ae1ba64.js", "assets/vue-select.9ddbca8a.js", "assets/vue-select.b0fac2a1.css"])
+            component: () => Un(() => import("./EditFiltersView.877cfb0b.js"), ["assets/EditFiltersView.877cfb0b.js", "assets/EditFiltersView.fa7331b7.css", "assets/TagsEditor.3f956450.js", "assets/TagsEditor.ccc03a15.css", "assets/hacks.175c31f5.js", "assets/vue-select.973ce47f.js", "assets/vue-select.b0fac2a1.css"])
         }, {
             path: "/download/",
             name: "add-dataset",
-            component: () => Un(() => import("./AddDatasetView.ff526466.js"), ["assets/AddDatasetView.ff526466.js", "assets/AddDatasetView.4182f0f7.css", "assets/vue-select.9ddbca8a.js", "assets/vue-select.b0fac2a1.css"])
+            component: () => Un(() => import("./AddDatasetView.8b79ed74.js"), ["assets/AddDatasetView.8b79ed74.js", "assets/AddDatasetView.1967bdb7.css", "assets/vue-select.973ce47f.js", "assets/vue-select.b0fac2a1.css"])
         }]
     });
 const hl = cu(Rf);
 hl.use(Lf);
 hl.mount("#app");
 export {
     lc as $, Qf as A, Nd as B, Ld as C, $i as D, $d as E, be as F, us as G, Kf as H, jf as I, $f as J, Bf as K, Zi as L, Ut as M, Yt as N, Qn as O, jd as P, Gi as Q, fl as R, Hf as S, fa as T, Wd as U, no as V, Uf as W, eo as X, Df as Y, te as Z, Sf as _, es as a, yc as a$, Fe as a0, zf as a1, He as a2, as as a3, os as a4, wl as a5, zn as a6, go as a7, Pe as a8, Zf as a9, ud as aA, Ot as aB, _d as aC, pa as aD, ur as aE, Nc as aF, $c as aG, mr as aH, Bc as aI, Lc as aJ, Uc as aK, On as aL, Dc as aM, jc as aN, Hc as aO, ws as aP, gr as aQ, Wn as aR, lo as aS, ad as aT, rd as aU, ed as aV, td as aW, Kc as aX, Cd as aY, En as aZ, Xr as a_, Wt as aa, Yf as ab, Cn as ac, Be as ad, nt as ae, rt as af, Rd as ag, oa as ah, vd as ai, ia as aj, sd as ak, ld as al, Xf as am, ys as an, dd as ao, hd as ap, fd as aq, sn as ar, Nt as as, pr as at, ko as au, Re as av, tn as aw, wd as ax, Ve as ay, Ea as az, ce as b, Qt as b0, xa as b1, Ed as b2, id as b3, od as b4, md as b5, bd as b6, gd as b7, po as b8, Ca as b9, Vd as bA, Dd as bB, Ud as bC, zd as bD, Hd as bE, Fd as bF, uc as ba, Oc as bb, Jf as bc, yd as bd, pd as be, xd as bf, qf as bg, jo as bh, Sd as bi, Er as bj, cu as bk, Id as bl, Ua as bm, Td as bn, lu as bo, Md as bp, pi as bq, Pd as br, Ad as bs, eu as bt, Yo as bu, Ga as bv, Xs as bw, iu as bx, kd as by, Od as bz, da as c, xe as d, dl as e, Io as f, Bd as g, Wf as h, Kn as i, ve as j, Vt as k, Xi as l, Y as m, Gf as n, Jt as o, Vf as p, _e as q, nd as r, nc as s, Ff as t, Ne as u, qo as v, fr as w, is as x, cd as y, Kd as z
```

### Comparing `opuscleaner-0.2.2/opuscleaner/frontend/assets/vue-select.9ddbca8a.js` & `opuscleaner-0.3.0/opuscleaner/frontend/assets/vue-select.973ce47f.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -18,15 +18,15 @@
     n as v,
     bx as L,
     b as E,
     w as M,
     bz as B,
     a4 as A,
     bh as j
-} from "./index.6cc31f0d.js";
+} from "./index.aa84b8f1.js";
 var I = Object.defineProperty,
     N = Object.defineProperties,
     K = Object.getOwnPropertyDescriptors,
     D = Object.getOwnPropertySymbols,
     z = Object.prototype.hasOwnProperty,
     R = Object.prototype.propertyIsEnumerable,
     P = (e, t, s) => t in e ? I(e, t, {
```

### Comparing `opuscleaner-0.2.2/opuscleaner/frontend/assets/vue-select.b0fac2a1.css` & `opuscleaner-0.3.0/opuscleaner/frontend/assets/vue-select.b0fac2a1.css`

 * *Files identical despite different names*

### Comparing `opuscleaner-0.2.2/README.md` & `opuscleaner-0.3.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -22,24 +22,24 @@
 - [FastAPI](https://fastapi.tiangolo.com) as the base for the backend part.
 - [Pydantic](https://pydantic-docs.helpmanual.io/) for conversion of untyped JSON to typed objects. And because FastAPI automatically supports it and gives you useful error messages if you mess up things.
 - [Vue](https://vuejs.org/guide/introduction.html) for frontend
 
 ### Screenshots
 
 List and categorize the datasets you are going to use for training.
-[<img src=".github/screenshots/list-datasets.png" width="100%">](.github/screenshots/list-datasets.png)
+[<img src="https://github.com/hplt-project/OpusCleaner/raw/main/.github/screenshots/list-datasets.png" width="100%">](https://github.com/hplt-project/OpusCleaner/blob/main/.github/screenshots/list-datasets.png)
 
 Download more datasets right from the interface.
-[<img src=".github/screenshots/add-datasets.png" width="100%">](.github/screenshots/add-datasets.png)
+[<img src="https://github.com/hplt-project/OpusCleaner/raw/main/.github/screenshots/add-datasets.png" width="100%">](https://github.com/hplt-project/OpusCleaner/blob/main/.github/screenshots/add-datasets.png)
 
 Filter each individual dataset, showing you the results immediately.
-[<img src=".github/screenshots/filter-datasets.png" width="100%">](.github/screenshots/filter-datasets.png)
+[<img src="https://github.com/hplt-project/OpusCleaner/raw/main/.github/screenshots/filter-datasets.png" width="100%">](https://github.com/hplt-project/OpusCleaner/blob/main/.github/screenshots/filter-datasets.png)
 
 Compare the dataset at different stages of filtering to see what the impact is of each filter.
-[<img src=".github/screenshots/diff-filter-output.png" width="100%">](.github/screenshots/diff-filter-output.png)
+[<img src="https://github.com/hplt-project/OpusCleaner/raw/main/.github/screenshots/diff-filter-output.png" width="100%">](https://github.com/hplt-project/OpusCleaner/blob/main/.github/screenshots/diff-filter-output.png)
 
 
 ### Paths
 - `data/train-parts` is scanned for datasets. You can change this by setting the `DATA_PATH` environment variable, the default is `data/train-parts/*.*.gz`.
 - `filters` should contain filter json files. You can change the `FILTER_PATH` environment variable, the default is `<PYTHON_PACKAGE>/filters/*.json`.
 
 ### Installation for development
```

### Comparing `opuscleaner-0.2.2/pyproject.toml` & `opuscleaner-0.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `opuscleaner-0.2.2/PKG-INFO` & `opuscleaner-0.3.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opuscleaner
-Version: 0.2.2
+Version: 0.3.0
 Project-URL: Documentation, https://github.com/hplt-project/opuscleaner#readme
 Project-URL: Issues, https://github.com/hplt-project/opuscleaner/issues
 Project-URL: Source, https://github.com/hplt-project/opuscleaner
 Author-email: Jelmer van der Linde <jelmer@ikhoefgeen.nl>
 License-Expression: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
@@ -59,24 +59,24 @@
 - [FastAPI](https://fastapi.tiangolo.com) as the base for the backend part.
 - [Pydantic](https://pydantic-docs.helpmanual.io/) for conversion of untyped JSON to typed objects. And because FastAPI automatically supports it and gives you useful error messages if you mess up things.
 - [Vue](https://vuejs.org/guide/introduction.html) for frontend
 
 ### Screenshots
 
 List and categorize the datasets you are going to use for training.
-[<img src=".github/screenshots/list-datasets.png" width="100%">](.github/screenshots/list-datasets.png)
+[<img src="https://github.com/hplt-project/OpusCleaner/raw/main/.github/screenshots/list-datasets.png" width="100%">](https://github.com/hplt-project/OpusCleaner/blob/main/.github/screenshots/list-datasets.png)
 
 Download more datasets right from the interface.
-[<img src=".github/screenshots/add-datasets.png" width="100%">](.github/screenshots/add-datasets.png)
+[<img src="https://github.com/hplt-project/OpusCleaner/raw/main/.github/screenshots/add-datasets.png" width="100%">](https://github.com/hplt-project/OpusCleaner/blob/main/.github/screenshots/add-datasets.png)
 
 Filter each individual dataset, showing you the results immediately.
-[<img src=".github/screenshots/filter-datasets.png" width="100%">](.github/screenshots/filter-datasets.png)
+[<img src="https://github.com/hplt-project/OpusCleaner/raw/main/.github/screenshots/filter-datasets.png" width="100%">](https://github.com/hplt-project/OpusCleaner/blob/main/.github/screenshots/filter-datasets.png)
 
 Compare the dataset at different stages of filtering to see what the impact is of each filter.
-[<img src=".github/screenshots/diff-filter-output.png" width="100%">](.github/screenshots/diff-filter-output.png)
+[<img src="https://github.com/hplt-project/OpusCleaner/raw/main/.github/screenshots/diff-filter-output.png" width="100%">](https://github.com/hplt-project/OpusCleaner/blob/main/.github/screenshots/diff-filter-output.png)
 
 
 ### Paths
 - `data/train-parts` is scanned for datasets. You can change this by setting the `DATA_PATH` environment variable, the default is `data/train-parts/*.*.gz`.
 - `filters` should contain filter json files. You can change the `FILTER_PATH` environment variable, the default is `<PYTHON_PACKAGE>/filters/*.json`.
 
 ### Installation for development
```

