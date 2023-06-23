# Comparing `tmp/uniparser-meadow-mari-1.1.8.tar.gz` & `tmp/uniparser-meadow-mari-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uniparser-meadow-mari-1.1.8.tar", last modified: Fri Jan 28 17:05:41 2022, max compression
+gzip compressed data, was "uniparser-meadow-mari-1.1.9.tar", last modified: Mon Mar  7 16:30:02 2022, max compression
```

## Comparing `uniparser-meadow-mari-1.1.8.tar` & `uniparser-meadow-mari-1.1.9.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2022-01-28 17:05:41.651247 uniparser-meadow-mari-1.1.8/
--rw-rw-rw-   0        0        0     1205 2021-04-01 11:14:34.000000 uniparser-meadow-mari-1.1.8/LICENSE
--rw-rw-rw-   0        0        0      206 2021-03-18 11:40:43.000000 uniparser-meadow-mari-1.1.8/MANIFEST.in
--rw-rw-rw-   0        0        0     5418 2022-01-28 17:05:41.651247 uniparser-meadow-mari-1.1.8/PKG-INFO
--rw-rw-rw-   0        0        0     4683 2021-03-18 11:40:43.000000 uniparser-meadow-mari-1.1.8/README.md
--rw-rw-rw-   0        0        0      108 2021-03-18 11:40:43.000000 uniparser-meadow-mari-1.1.8/pyproject.toml
--rw-rw-rw-   0        0        0      844 2022-01-28 17:05:41.653243 uniparser-meadow-mari-1.1.8/setup.cfg
-drwxrwxrwx   0        0        0        0 2022-01-28 17:05:41.608845 uniparser-meadow-mari-1.1.8/uniparser_meadow_mari/
--rw-rw-rw-   0        0        0     2420 2021-03-18 11:40:43.000000 uniparser-meadow-mari-1.1.8/uniparser_meadow_mari/__init__.py
-drwxrwxrwx   0        0        0        0 2022-01-28 17:05:41.633343 uniparser-meadow-mari-1.1.8/uniparser_meadow_mari/data_nodiacritics/
--rw-rw-rw-   0        0        0        0 2021-03-18 11:40:43.000000 uniparser-meadow-mari-1.1.8/uniparser_meadow_mari/data_nodiacritics/__init__.py
--rw-rw-rw-   0        0        0     1159 2022-01-28 16:43:00.000000 uniparser-meadow-mari-1.1.8/uniparser_meadow_mari/data_nodiacritics/bad_analyses.txt
--rw-rw-rw-   0        0        0    39851 2022-01-28 16:51:48.000000 uniparser-meadow-mari-1.1.8/uniparser_meadow_mari/data_nodiacritics/lex_rules.txt
--rw-rw-rw-   0        0        0  6964215 2022-01-28 16:51:48.000000 uniparser-meadow-mari-1.1.8/uniparser_meadow_mari/data_nodiacritics/lexemes.txt
--rw-rw-rw-   0        0        0     1804 2021-04-07 08:23:22.000000 uniparser-meadow-mari-1.1.8/uniparser_meadow_mari/data_nodiacritics/meadow_mari_disambiguation.cg3
--rw-rw-rw-   0        0        0   206150 2022-01-28 16:51:48.000000 uniparser-meadow-mari-1.1.8/uniparser_meadow_mari/data_nodiacritics/paradigms.txt
-drwxrwxrwx   0        0        0        0 2022-01-28 17:05:41.649253 uniparser-meadow-mari-1.1.8/uniparser_meadow_mari/data_strict/
--rw-rw-rw-   0        0        0        0 2021-03-18 11:40:43.000000 uniparser-meadow-mari-1.1.8/uniparser_meadow_mari/data_strict/__init__.py
--rw-rw-rw-   0        0        0     1159 2022-01-28 16:43:00.000000 uniparser-meadow-mari-1.1.8/uniparser_meadow_mari/data_strict/bad_analyses.txt
--rw-rw-rw-   0        0        0    39851 2022-01-28 16:51:48.000000 uniparser-meadow-mari-1.1.8/uniparser_meadow_mari/data_strict/lex_rules.txt
--rw-rw-rw-   0        0        0  6848225 2022-01-28 16:51:48.000000 uniparser-meadow-mari-1.1.8/uniparser_meadow_mari/data_strict/lexemes.txt
--rw-rw-rw-   0        0        0     1804 2021-04-07 08:23:22.000000 uniparser-meadow-mari-1.1.8/uniparser_meadow_mari/data_strict/meadow_mari_disambiguation.cg3
--rw-rw-rw-   0        0        0   194133 2022-01-28 16:51:48.000000 uniparser-meadow-mari-1.1.8/uniparser_meadow_mari/data_strict/paradigms.txt
-drwxrwxrwx   0        0        0        0 2022-01-28 17:05:41.617357 uniparser-meadow-mari-1.1.8/uniparser_meadow_mari.egg-info/
--rw-rw-rw-   0        0        0     5418 2022-01-28 17:05:41.000000 uniparser-meadow-mari-1.1.8/uniparser_meadow_mari.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      956 2022-01-28 17:05:41.000000 uniparser-meadow-mari-1.1.8/uniparser_meadow_mari.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-01-28 17:05:41.000000 uniparser-meadow-mari-1.1.8/uniparser_meadow_mari.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2022-01-28 17:05:41.000000 uniparser-meadow-mari-1.1.8/uniparser_meadow_mari.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2022-01-28 17:05:41.000000 uniparser-meadow-mari-1.1.8/uniparser_meadow_mari.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2022-03-07 16:30:02.755739 uniparser-meadow-mari-1.1.9/
+-rw-rw-rw-   0        0        0     1205 2021-04-01 11:14:34.000000 uniparser-meadow-mari-1.1.9/LICENSE
+-rw-rw-rw-   0        0        0      206 2021-03-18 11:40:43.000000 uniparser-meadow-mari-1.1.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     5418 2022-03-07 16:30:02.755739 uniparser-meadow-mari-1.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0     4683 2021-03-18 11:40:43.000000 uniparser-meadow-mari-1.1.9/README.md
+-rw-rw-rw-   0        0        0      108 2021-03-18 11:40:43.000000 uniparser-meadow-mari-1.1.9/pyproject.toml
+-rw-rw-rw-   0        0        0      844 2022-03-07 16:30:02.756736 uniparser-meadow-mari-1.1.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2022-03-07 16:30:02.707025 uniparser-meadow-mari-1.1.9/uniparser_meadow_mari/
+-rw-rw-rw-   0        0        0     2420 2021-03-18 11:40:43.000000 uniparser-meadow-mari-1.1.9/uniparser_meadow_mari/__init__.py
+drwxrwxrwx   0        0        0        0 2022-03-07 16:30:02.736790 uniparser-meadow-mari-1.1.9/uniparser_meadow_mari/data_nodiacritics/
+-rw-rw-rw-   0        0        0        0 2021-03-18 11:40:43.000000 uniparser-meadow-mari-1.1.9/uniparser_meadow_mari/data_nodiacritics/__init__.py
+-rw-rw-rw-   0        0        0     1202 2022-03-07 16:18:52.000000 uniparser-meadow-mari-1.1.9/uniparser_meadow_mari/data_nodiacritics/bad_analyses.txt
+-rw-rw-rw-   0        0        0    39851 2022-03-07 16:19:03.000000 uniparser-meadow-mari-1.1.9/uniparser_meadow_mari/data_nodiacritics/lex_rules.txt
+-rw-rw-rw-   0        0        0  6968930 2022-03-07 16:19:03.000000 uniparser-meadow-mari-1.1.9/uniparser_meadow_mari/data_nodiacritics/lexemes.txt
+-rw-rw-rw-   0        0        0     1804 2021-04-07 08:23:22.000000 uniparser-meadow-mari-1.1.9/uniparser_meadow_mari/data_nodiacritics/meadow_mari_disambiguation.cg3
+-rw-rw-rw-   0        0        0   206150 2022-03-07 16:19:03.000000 uniparser-meadow-mari-1.1.9/uniparser_meadow_mari/data_nodiacritics/paradigms.txt
+drwxrwxrwx   0        0        0        0 2022-03-07 16:30:02.753744 uniparser-meadow-mari-1.1.9/uniparser_meadow_mari/data_strict/
+-rw-rw-rw-   0        0        0        0 2021-03-18 11:40:43.000000 uniparser-meadow-mari-1.1.9/uniparser_meadow_mari/data_strict/__init__.py
+-rw-rw-rw-   0        0        0     1202 2022-03-07 16:18:52.000000 uniparser-meadow-mari-1.1.9/uniparser_meadow_mari/data_strict/bad_analyses.txt
+-rw-rw-rw-   0        0        0    39851 2022-03-07 16:19:03.000000 uniparser-meadow-mari-1.1.9/uniparser_meadow_mari/data_strict/lex_rules.txt
+-rw-rw-rw-   0        0        0  6852867 2022-03-07 16:19:03.000000 uniparser-meadow-mari-1.1.9/uniparser_meadow_mari/data_strict/lexemes.txt
+-rw-rw-rw-   0        0        0     1804 2021-04-07 08:23:22.000000 uniparser-meadow-mari-1.1.9/uniparser_meadow_mari/data_strict/meadow_mari_disambiguation.cg3
+-rw-rw-rw-   0        0        0   194133 2022-03-07 16:19:03.000000 uniparser-meadow-mari-1.1.9/uniparser_meadow_mari/data_strict/paradigms.txt
+drwxrwxrwx   0        0        0        0 2022-03-07 16:30:02.716906 uniparser-meadow-mari-1.1.9/uniparser_meadow_mari.egg-info/
+-rw-rw-rw-   0        0        0     5418 2022-03-07 16:30:02.000000 uniparser-meadow-mari-1.1.9/uniparser_meadow_mari.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      956 2022-03-07 16:30:02.000000 uniparser-meadow-mari-1.1.9/uniparser_meadow_mari.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-03-07 16:30:02.000000 uniparser-meadow-mari-1.1.9/uniparser_meadow_mari.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2022-03-07 16:30:02.000000 uniparser-meadow-mari-1.1.9/uniparser_meadow_mari.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2022-03-07 16:30:02.000000 uniparser-meadow-mari-1.1.9/uniparser_meadow_mari.egg-info/top_level.txt
```

### Comparing `uniparser-meadow-mari-1.1.8/LICENSE` & `uniparser-meadow-mari-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `uniparser-meadow-mari-1.1.8/PKG-INFO` & `uniparser-meadow-mari-1.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uniparser-meadow-mari
-Version: 1.1.8
+Version: 1.1.9
 Summary: Rule-based morphological analysis for Meadow Mari
 Home-page: https://github.com/timarkh/uniparser-grammar-meadow-mari
 Author: Timofey Arkhangelskiy
 Author-email: timarkh@gmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/timarkh/uniparser-grammar-meadow-mari/issues
 Platform: UNKNOWN
```

### Comparing `uniparser-meadow-mari-1.1.8/README.md` & `uniparser-meadow-mari-1.1.9/README.md`

 * *Files identical despite different names*

### Comparing `uniparser-meadow-mari-1.1.8/setup.cfg` & `uniparser-meadow-mari-1.1.9/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2075 6e69 7061 7273 6572 2d6d 6561   = uniparser-mea
 00000020: 646f 772d 6d61 7269 0d0a 7665 7273 696f  dow-mari..versio
-00000030: 6e20 3d20 312e 312e 380d 0a61 7574 686f  n = 1.1.8..autho
+00000030: 6e20 3d20 312e 312e 390d 0a61 7574 686f  n = 1.1.9..autho
 00000040: 7220 3d20 5469 6d6f 6665 7920 4172 6b68  r = Timofey Arkh
 00000050: 616e 6765 6c73 6b69 790d 0a61 7574 686f  angelskiy..autho
 00000060: 725f 656d 6169 6c20 3d20 7469 6d61 726b  r_email = timark
 00000070: 6840 676d 6169 6c2e 636f 6d0d 0a64 6573  h@gmail.com..des
 00000080: 6372 6970 7469 6f6e 203d 2052 756c 652d  cription = Rule-
 00000090: 6261 7365 6420 6d6f 7270 686f 6c6f 6769  based morphologi
 000000a0: 6361 6c20 616e 616c 7973 6973 2066 6f72  cal analysis for
```

### Comparing `uniparser-meadow-mari-1.1.8/uniparser_meadow_mari/__init__.py` & `uniparser-meadow-mari-1.1.9/uniparser_meadow_mari/__init__.py`

 * *Files identical despite different names*

### Comparing `uniparser-meadow-mari-1.1.8/uniparser_meadow_mari/data_nodiacritics/bad_analyses.txt` & `uniparser-meadow-mari-1.1.9/uniparser_meadow_mari/data_nodiacritics/bad_analyses.txt`

 * *Files 7% similar despite different names*

```diff
@@ -10,15 +10,16 @@
   {"wf": "^тӱҥал.*", "lemma": "тӱҥаш"},
   {"wf": "^кӱлеш.*", "lemma": "кӱ"},
   {"wf": "^-?олан(ат)?$", "gramm": ".*PN.*"},
   {"wf": "^тораш[кт][еы].*", "gramm": ".*PN.*"},
   {"gramm": ".*,imp.*", "lemma": "эргаш"},
   {"gramm": ".*,(imp|desid|neg).*3sg"},
   {"gramm": "^CONJ.*3sg"},
-  {"gramm": "(.*,(?:persn|patrn|famn|anim|lang_name).*|^[^N].*)", "gloss": ".*PL\\.SHORT($|(-[^LI]|-L[^O]|-I[^L]|-LO[^C]|-IL[^L]).*)"},
+  {"gramm": ".*,(?:persn|patrn|famn|anim|lang_name).*", "gloss": ".*PL\\.SHORT($|(-[^LI]|-L[^O]|-I[^L]|-LO[^C]|-IL[^L]).*)"},
+  {"gramm": "^[^VN].*", "gloss": ".*PL\\.SHORT.*"},
   {"gramm": "^(.(?!,nation))+$", "gloss": ".*SIM-(ACC|GEN|DAT|LAT|LOC|ILL|SIM|COM).*"},
   {"wf": "тӱрлӧ.*", "lemma": "^(тӱрлаш|тӱр)$"},
   {"gramm": ".*,(nom|acc|gen|dat|com|case_comp).*", "lemma": "ку-"},
   {"gramm": "^.*nmlz(.(?!,sg))+$", "wf": ".*маш$"},
   {"gramm": "CONJ.*", "wf": "^дена[тк]$"}
 ]
```

### Comparing `uniparser-meadow-mari-1.1.8/uniparser_meadow_mari/data_nodiacritics/lex_rules.txt` & `uniparser-meadow-mari-1.1.9/uniparser_meadow_mari/data_nodiacritics/lex_rules.txt`

 * *Files identical despite different names*

### Comparing `uniparser-meadow-mari-1.1.8/uniparser_meadow_mari/data_nodiacritics/lexemes.txt` & `uniparser-meadow-mari-1.1.9/uniparser_meadow_mari/data_nodiacritics/lexemes.txt`

 * *Files 0% similar despite different names*

```diff
@@ -8787,14 +8787,21 @@
  lex: Баркалов
  stem: баркалов.
  gramm: N,PN,famn
  paradigm: N_consonant
  trans_ru: Баркалов
 
 -lexeme
+ lex: Баркас
+ gramm: N,PN,persn
+ stem: баркас.
+ paradigm: N_consonant
+ trans_ru: Баркас
+
+-lexeme
  lex: Барклай-де-толли
  stem: барклай-де-толли.
  gramm: N,PN,famn
  paradigm: N_paroxyton_v_weak
  trans_ru: Барклай-де-толли
 
 -lexeme
@@ -29612,14 +29619,21 @@
  lex: Кажаева
  gramm: N,PN,famn
  stem: кажаева.|кажаевы.|кажаев.
  paradigm: N_paroxyton_v_weak
  trans_ru: Кажаева
 
 -lexeme
+ lex: Кажай
+ gramm: N,persn,PN
+ stem: кажай.|кажа.
+ paradigm: N_j
+ trans_ru: Кажай
+
+-lexeme
  lex: Кажвеле
  stem: кажвеле.
  gramm: N,PN,topn
  paradigm: N_paroxyton_v_weak
  trans_ru: Кажвеле
 
 -lexeme
@@ -29956,14 +29970,21 @@
  stem: какшамбал.
  gramm: N,PN,topn
  paradigm: N_consonant
  trans_ru: Кокшамбал
 
 -lexeme
  lex: Какшан
+ gramm: N,PN,topn
+ stem: какшан.
+ paradigm: N_consonant
+ trans_ru: Кокшага
+
+-lexeme
+ lex: Какшан
  stem: какшан.
  gramm: N,PN,topn
  paradigm: N_consonant
  trans_ru: Кокшайск
 
 -lexeme
  lex: Какшанмучаш
@@ -32188,14 +32209,21 @@
  lex: Керей
  stem: керей.|кере.
  gramm: N,PN,persn
  paradigm: N_j
  trans_ru: Керей
 
 -lexeme
+ lex: Керемлак
+ gramm: N,PN,topn
+ stem: керемлак.
+ paradigm: N_consonant
+ trans_ru: Керемлак
+
+-lexeme
  lex: Керенский
  stem: керенский.|керенски.
  gramm: N,PN,famn
  paradigm: N_j
  trans_ru: Керенский
 
 -lexeme
@@ -34232,14 +34260,21 @@
  lex: Колпакова
  stem: колпакова.|колпаковы.//колпакова.|колпаков.//колпакова.
  gramm: N,PN,famn
  paradigm: N_paroxyton_v_weak
  trans_ru: Колпакова
 
 -lexeme
+ lex: Колтак
+ gramm: N,PN,topn
+ stem: колтак.
+ paradigm: N_consonant
+ trans_ru: Колтак
+
+-lexeme
  lex: Колтаков
  stem: колтаков.
  gramm: N,PN,famn
  paradigm: N_consonant
  trans_ru: Колтаков
 
 -lexeme
@@ -36696,14 +36731,21 @@
  lex: Кувакин
  stem: кувакин.
  gramm: N,PN,famn
  paradigm: N_consonant
  trans_ru: Кувакин
 
 -lexeme
+ lex: Куван
+ gramm: N,topn,PN
+ stem: куван.
+ paradigm: N_consonant
+ trans_ru: Куван
+
+-lexeme
  lex: Кувшинов
  stem: кувшинов.
  gramm: N,PN,famn
  paradigm: N_consonant
  trans_ru: Кувшинов
 
 -lexeme
@@ -37970,14 +38012,21 @@
  lex: Кури
  stem: кури.
  gramm: N,PN,persn
  paradigm: N_paroxyton_v_strong
  trans_ru: Кури
 
 -lexeme
+ lex: Курий
+ gramm: N,persn,PN
+ stem: курий.|кури.
+ paradigm: N_j
+ trans_ru: Курий, Гурий
+
+-lexeme
  lex: Курилов
  stem: курилов.
  gramm: N,PN,famn
  paradigm: N_consonant
  trans_ru: Курилов
 
 -lexeme
@@ -43703,14 +43752,21 @@
  lex: Марткия
  stem: марткия.
  gramm: N,PN,persn
  paradigm: N_paroxyton_v_strong
  trans_ru: Марткия
 
 -lexeme
+ lex: Мартын
+ gramm: N,PN,topn
+ stem: мартын.
+ paradigm: N_consonant
+ trans_ru: Мартын (озеро)
+
+-lexeme
  lex: Мартыненко
  stem: мартыненко.|мартыненкы.//мартыненко.|мартыненк.//мартыненко.
  gramm: N,PN,famn
  paradigm: N_paroxyton_v_weak
  trans_ru: Мартыненко
 
 -lexeme
@@ -45040,14 +45096,21 @@
  lex: Микал
  stem: микал.
  gramm: N,PN,persn
  paradigm: N_consonant
  trans_ru: Микал (Михаил)
 
 -lexeme
+ lex: Микале
+ gramm: N,PN,persn
+ stem: микале.|микалы.|микал.
+ paradigm: N_paroxyton_v_weak
+ trans_ru: Микале, Михаил
+
+-lexeme
  lex: Микальмихайлов
  stem: микальмихайлов.
  gramm: N,PN,famn
  paradigm: N_consonant
  trans_ru: Микальмихайлов
 
 -lexeme
@@ -77961,14 +78024,21 @@
  lex: Чаркаю
  stem: чаркаю.
  gramm: N,PN,topn
  paradigm: N_paroxyton_v_weak
  trans_ru: Чаркаю
 
 -lexeme
+ lex: Чарла
+ gramm: N,topn,PN
+ stem: чарла.
+ paradigm: N_consonant
+ trans_ru: Царевококшайск
+
+-lexeme
  lex: Чарнур
  stem: чарнур.
  gramm: N,PN,topn
  paradigm: N_consonant
  trans_ru: Большой Царанур; Малый Царанур
 
 -lexeme
@@ -80593,14 +80663,21 @@
  lex: Шанцора
  stem: шанцора.|шанцоры.//шанцора.|шанцор.//шанцора.
  gramm: N,PN,persn
  paradigm: N_paroxyton_v_weak
  trans_ru: Шанцора
 
 -lexeme
+ lex: Шап
+ gramm: N,PN,topn
+ stem: шап.
+ paradigm: N_consonant
+ trans_ru: Шап
+
+-lexeme
  lex: Шаплак
  stem: шаплак.
  gramm: N,PN,topn
  paradigm: N_consonant
  trans_ru: Большой Шаплак
 
 -lexeme
@@ -82197,14 +82274,21 @@
  gramm: N,PN,topn
  stem: шолаҥыш.//шоланыш.
  paradigm: N_consonant
  trans_ru: Шоланыш
 
 -lexeme
  lex: Шолеҥер
+ gramm: N,PN,topn
+ stem: шолеҥер.//шоленер.
+ paradigm: N_consonant
+ trans_ru: Шелангер
+
+-lexeme
+ lex: Шолеҥер
  gramm: N,topn,PN
  stem: шолеҥер.//шоленер.
  paradigm: N_consonant
  trans_ru: Шолнер
 
 -lexeme
  lex: Шолкадур
@@ -84822,14 +84906,21 @@
  stem: юкчи.
  gramm: N,PN,persn
  paradigm: N_paroxyton_v_strong
  trans_ru: Юкчи
 
 -lexeme
  lex: Юл
+ gramm: N,topn,PN
+ stem: юл.
+ paradigm: N_consonant
+ trans_ru: Волга
+
+-lexeme
+ lex: Юл
  stem: юл.
  gramm: N,PN,topn
  paradigm: N_consonant
  trans_ru: Юл
 
 -lexeme
  lex: Юлавий
@@ -90016,14 +90107,21 @@
  lex: ай
  gramm: INTRJ
  stem: ай.
  paradigm: Clitics
  trans_ru: ах, эх
 
 -lexeme
+ lex: ай-ай
+ gramm: INTRJ
+ stem: ай-ай.//ай-яй.
+ paradigm: Clitics
+ trans_ru: ах, эх
+
+-lexeme
  lex: айва
  stem: айва.|айвы.//айва.|айв.//айва.
  gramm: N,rus
  paradigm: N_paroxyton_v_weak
  trans_ru: айва
 
 -lexeme
@@ -91879,14 +91977,21 @@
  lex: амал
  stem: амал.
  gramm: N
  paradigm: N_consonant
  trans_ru: причина, повод; форма; случай
 
 -lexeme
+ lex: амалаш
+ gramm: V,intr
+ stem: амал.
+ paradigm: V_e
+ trans_ru: ловчить, изловчиться
+
+-lexeme
  lex: амалгаш
  stem: амалг.
  gramm: V
  paradigm: V_e
  trans_ru: закоснеть
 
 -lexeme
@@ -95517,14 +95622,21 @@
  lex: ать-уть
  gramm: INTRJ
  stem: ать-уть.
  paradigm: Clitics
  trans_ru: ать-уть
 
 -lexeme
+ lex: ау
+ gramm: INTRJ,rus
+ stem: а-у-у.
+ paradigm: Clitics
+ trans_ru: ау, отклик на зов, окрик при поиске
+
+-lexeme
  lex: аудио
  stem: аудио.|аудиы.//аудио.|ауди.//аудио.
  gramm: N,rus
  paradigm: N_paroxyton_v_weak
  trans_ru: аудио
 
 -lexeme
@@ -104637,14 +104749,21 @@
  stem: верховный.//вэрховный.|верховны.//вэрховны.
  gramm: A,rus
  paradigm: A_j
  trans_ru: верховный
 
 -lexeme
  lex: верч
+ gramm: POST
+ stem: верч.
+ paradigm: POST_ADV_Poss
+ trans_ru: для, ради, из-за
+
+-lexeme
+ lex: верч
  stem: верч.//вэрч.
  gramm: ADV
  paradigm: POST_ADV_Poss
  trans_ru: для, ради, из-за
 
 -lexeme
  lex: вершок
@@ -115419,14 +115538,21 @@
  stem: гофрированный.|гофрированны.
  gramm: A,rus
  paradigm: A_j
  trans_ru: гофрированный
 
 -lexeme
  lex: гоч
+ gramm: POST
+ stem: коч.
+ paradigm: POST_ADV_Poss
+ trans_ru: через; пока
+
+-lexeme
+ lex: гоч
  stem: гоч.
  gramm: POST
  paradigm: POST_ADV_Poss
  trans_ru: через; пока
 
 -lexeme
  lex: граб
@@ -131078,14 +131204,21 @@
  stem: йол.
  gramm: N,body
  paradigm: N_consonant
  trans_ru: нога, ножка
 
 -lexeme
  lex: йола
+ gramm: ADV
+ stem: йола.
+ paradigm: POST_ADV_Poss
+ trans_ru: на ногах
+
+-lexeme
+ lex: йола
  stem: йола.
  gramm: N
  paradigm: N_oxyton
  trans_ru: вина
 
 -lexeme
  lex: йола-вала
@@ -133514,14 +133647,21 @@
  stem: йып.
  gramm: N
  paradigm: N_consonant
  trans_ru: пика, копьё
 
 -lexeme
  lex: йып-йып
+ gramm: ADV
+ stem: йып.
+ paradigm: POST_ADV_Poss
+ trans_ru: совершенно, совсем
+
+-lexeme
+ lex: йып-йып
  stem: йып-йып.
  gramm: ADV
  paradigm: POST_ADV_Poss
  trans_ru: совершенно
 
 -lexeme
  lex: йыпар
@@ -134500,14 +134640,21 @@
  lex: йӧрал
  stem: йӧрал.//йорал.
  gramm: A
  paradigm: A_consonant
  trans_ru: пригодный
 
 -lexeme
+ lex: йӧралаш
+ gramm: V,tr
+ stem: йӧрал.//йорал.
+ paradigm: V_a
+ trans_ru: свалить
+
+-lexeme
  lex: йӧралташ
  stem: йӧралт.//йоралт.
  gramm: V
  paradigm: V_a
  trans_ru: валиться; умирать
 
 -lexeme
@@ -151514,14 +151661,21 @@
  lex: кочмывер
  stem: кочмывер.//кочмывэр.
  gramm: N
  paradigm: N_consonant
  trans_ru: столовая
 
 -lexeme
+ lex: кочо
+ gramm: A
+ stem: кочо.|кочы.|коч.
+ paradigm: A_paroxyton_v_weak
+ trans_ru: горький
+
+-lexeme
  lex: кочо-йӧсӧ
  stem: кочо-йӧсӧ.//кочо-йосо.|кочо-йӧсы.//кочо-йосы.|кочо-йӧс.//кочо-йос.
  gramm: N
  paradigm: N_paroxyton_v_weak
  trans_ru: несчастье
 
 -lexeme
@@ -157526,14 +157680,21 @@
  stem: кутузко.|кутузкы.|кутузк.
  gramm: N,rus
  paradigm: N_paroxyton_v_weak
  trans_ru: кутузка
 
 -lexeme
  lex: кутынек
+ gramm: ADV
+ stem: кутынек.
+ paradigm: POST_ADV_Poss
+ trans_ru: вдоль, по
+
+-lexeme
+ lex: кутынек
  stem: кутынек.
  gramm: POST
  paradigm: POST_ADV_Poss
  trans_ru: вдоль, по
 
 -lexeme
  lex: кутынь
@@ -158366,14 +158527,21 @@
  stem: кыж.
  gramm: IMIT
  paradigm: Clitics
  trans_ru: о бесшумном, малозаметном движении
 
 -lexeme
  lex: кыж-гож
+ gramm: IMIT
+ stem: кыж-кож.
+ paradigm: Clitics
+ trans_ru: о звуке шороха, шелеста
+
+-lexeme
+ lex: кыж-гож
  stem: кыж-гож.
  gramm: IMIT
  paradigm: Clitics
  trans_ru: о звуке шороха, шелеста
 
 -lexeme
  lex: кыжга
@@ -158939,14 +159107,21 @@
  lex: кыр-гор
  stem: кыр-гор.
  gramm: IMIT
  paradigm: Clitics
  trans_ru: о скребущем звуке или быстром движении
 
 -lexeme
+ lex: кыр-лук
+ gramm: IMIT
+ stem: кыр-лук.
+ paradigm: Clitics
+ trans_ru: о крике журавля
+
+-lexeme
  lex: кыра-сара
  stem: кыра-сара.
  gramm: N
  paradigm: N_oxyton
  trans_ru: негодное, нерадивое
 
 -lexeme
@@ -161187,14 +161362,21 @@
  lex: кӱлеш
  gramm: A
  stem: кӱлеш.//кулеш.
  paradigm: A_consonant
  trans_ru: нужный
 
 -lexeme
+ lex: кӱлеш
+ gramm: PREDIC
+ stem: кӱлеш.//кулеш.
+ paradigm: Clitics
+ trans_ru: нужно
+
+-lexeme
  lex: кӱлеш-оккӱл
  gramm: N
  stem: кӱлеш-огыл.//кулеш-огыл.
  paradigm: N_consonant
  trans_ru: нелепость
 
 -lexeme
@@ -162224,14 +162406,21 @@
  stem: кӱшклат.//кушклат.
  gramm: N
  paradigm: N_consonant
  trans_ru: верхняя клеть, второй этаж клети
 
 -lexeme
  lex: кӱшкыла
+ gramm: ADV
+ stem: кӱшкыла.//кушкыла.
+ paradigm: POST_ADV_Poss
+ trans_ru: наверх
+
+-lexeme
+ lex: кӱшкыла
  stem: кӱшкыла.//кушкыла.
  gramm: POST
  paradigm: POST_ADV_Poss
  trans_ru: наверх
 
 -lexeme
  lex: кӱшкӧ
@@ -163449,14 +163638,21 @@
  stem: ласа.
  gramm: PART
  paradigm: Clitics
  trans_ru: ведь, же
 
 -lexeme
  lex: ласка
+ gramm: ADV,rus
+ stem: ласка.
+ paradigm: POST_ADV_Poss
+ trans_ru: cпокойно, приятно
+
+-lexeme
+ lex: ласка
  stem: ласка.
  gramm: A,rus
  paradigm: A_oxyton
  trans_ru: ласковый
 
 -lexeme
  lex: ласка
@@ -164660,14 +164856,21 @@
  stem: леп.//лэп.
  gramm: N,body
  paradigm: N_consonant
  trans_ru: селезёнка
 
 -lexeme
  lex: леп-леве
+ gramm: A
+ stem: леп-леп.
+ paradigm: A_consonant
+ trans_ru: тёплый
+
+-lexeme
+ lex: леп-леве
  stem: леп-леве.//леп-левэ.|леп-левы.//леп-лэвы.|леп-лев.//леп-лэв.
  gramm: A
  paradigm: A_paroxyton_v_weak
  trans_ru: тёплый-тёплый
 
 -lexeme
  lex: лепене
@@ -180330,14 +180533,21 @@
  stem: мучката.
  gramm: A
  paradigm: A_oxyton
  trans_ru: полный, тучный, толстый
 
 -lexeme
  lex: мучко
+ gramm: ADV
+ stem: мучко.
+ paradigm: POST_ADV_Poss
+ trans_ru: целиком; сплошь; вдоль
+
+-lexeme
+ lex: мучко
  stem: мучко.
  gramm: POST
  paradigm: POST_ADV_Poss
  trans_ru: целиком; сплошь; вдоль
 
 -lexeme
  lex: мучко-мучко
@@ -210083,14 +210293,21 @@
  stem: почерк.//почэрк.
  gramm: N,rus
  paradigm: N_consonant
  trans_ru: почерк
 
 -lexeme
  lex: почеш
+ gramm: ADV
+ stem: почеш.
+ paradigm: POST_ADV_Poss
+ trans_ru: следом
+
+-lexeme
+ lex: почеш
  gramm: POST
  stem: почеш.
  paradigm: POST_ADV_Poss
  trans_ru: за, по, вслед, после
 
 -lexeme
  lex: почеш
@@ -219841,14 +220058,21 @@
  lex: пышкыраш
  stem: пышкыр.
  gramm: V
  paradigm: V_e
  trans_ru: фыркать
 
 -lexeme
+ lex: пышт
+ gramm: IMIT
+ stem: пышт.
+ paradigm: Clitics
+ trans_ru: о пыхтении
+
+-lexeme
  lex: пышт-пошт
  stem: пышт-пошт.
  gramm: IMIT
  paradigm: Clitics
  trans_ru: о сухом негромком звуке
 
 -lexeme
@@ -252474,14 +252698,21 @@
  stem: торец.//торэц.
  gramm: N,rus
  paradigm: N_consonant
  trans_ru: торец
 
 -lexeme
  lex: тореш
+ gramm: ADV
+ stem: тореш.
+ paradigm: POST_ADV_Poss
+ trans_ru: напротив; поперёк
+
+-lexeme
+ lex: тореш
  gramm: POST
  stem: тореш.
  paradigm: POST_ADV_Poss
  trans_ru: напротив; поперёк
 
 -lexeme
  lex: тореш
@@ -256320,14 +256551,21 @@
  stem: тур.
  gramm: N,rus
  paradigm: N_consonant
  trans_ru: тур
 
 -lexeme
  lex: тура
+ gramm: ADV
+ stem: тура.
+ paradigm: POST_ADV_Poss
+ trans_ru: круто
+
+-lexeme
+ lex: тура
  gramm: N,supernat
  stem: тура.
  paradigm: N_oxyton
  trans_ru: полуденица (миф. существо, являющееся в полдень)
 
 -lexeme
  lex: тура
@@ -270085,14 +270323,21 @@
  lex: фуфик
  stem: фуфик.
  gramm: N,rus,anim,hum
  paradigm: N_consonant
  trans_ru: фуфик
 
 -lexeme
+ lex: фыр
+ gramm: IMIT,rus
+ stem: фыр.
+ paradigm: Clitics
+ trans_ru: фыр, о выходе воздуха, пара
+
+-lexeme
  lex: фыр-р
  stem: фыр-р.
  gramm: IMIT
  paradigm: Clitics
  trans_ru: о звуке фырканья
 
 -lexeme
@@ -272956,14 +273201,21 @@
  stem: чап.
  gramm: N
  paradigm: N_consonant
  trans_ru: слава; уважение
 
 -lexeme
  lex: чап-чап
+ gramm: IMIT
+ stem: чап-чап.
+ paradigm: Clitics
+ trans_ru: о крике синицы
+
+-lexeme
+ lex: чап-чап
  stem: чап-чап.
  gramm: IMIT
  paradigm: Clitics
  trans_ru: об ударах веником в бане
 
 -lexeme
  lex: чап-чара
@@ -294861,14 +295113,21 @@
  lex: шӱштӱштӧ
  stem: шӱштӱштӧ.//шуштушто.|шӱштӱшты.//шуштушты.|шӱштӱшт.//шуштушт.
  gramm: N
  paradigm: N_paroxyton_v_weak
  trans_ru: ремень, кожаный пояс
 
 -lexeme
+ lex: шӱялташ
+ gramm: V,tr
+ stem: шӱялт.//шуялт.
+ paradigm: V_e
+ trans_ru: полоскать
+
+-lexeme
  lex: шӱяш
  stem: шӱ.//шу.|шӱй.//шуй.
  gramm: V
  paradigm: V_ya
  trans_ru: гнить
 
 -lexeme
@@ -305201,15 +305460,15 @@
  trans_ru: сметана
 
 -lexeme
  lex: ӱмбал
  stem: ӱмбал.//умбал.|ӱмба.//умба.
  gramm: N,rel_n
  paradigm: POST
- trans_ru: поверхность; наверху
+ trans_ru: верх, поверхность; наверху
 
 -lexeme
  lex: ӱмбала
  stem: ӱмбала.//умбала.
  gramm: ADV
  paradigm: POST_ADV_Poss
  trans_ru: друг на друга; двухэтажный; многократно; поверх, один на другой
```

### Comparing `uniparser-meadow-mari-1.1.8/uniparser_meadow_mari/data_nodiacritics/meadow_mari_disambiguation.cg3` & `uniparser-meadow-mari-1.1.9/uniparser_meadow_mari/data_nodiacritics/meadow_mari_disambiguation.cg3`

 * *Files identical despite different names*

### Comparing `uniparser-meadow-mari-1.1.8/uniparser_meadow_mari/data_nodiacritics/paradigms.txt` & `uniparser-meadow-mari-1.1.9/uniparser_meadow_mari/data_nodiacritics/paradigms.txt`

 * *Files identical despite different names*

### Comparing `uniparser-meadow-mari-1.1.8/uniparser_meadow_mari/data_strict/bad_analyses.txt` & `uniparser-meadow-mari-1.1.9/uniparser_meadow_mari/data_strict/bad_analyses.txt`

 * *Files 7% similar despite different names*

```diff
@@ -10,15 +10,16 @@
   {"wf": "^тӱҥал.*", "lemma": "тӱҥаш"},
   {"wf": "^кӱлеш.*", "lemma": "кӱ"},
   {"wf": "^-?олан(ат)?$", "gramm": ".*PN.*"},
   {"wf": "^тораш[кт][еы].*", "gramm": ".*PN.*"},
   {"gramm": ".*,imp.*", "lemma": "эргаш"},
   {"gramm": ".*,(imp|desid|neg).*3sg"},
   {"gramm": "^CONJ.*3sg"},
-  {"gramm": "(.*,(?:persn|patrn|famn|anim|lang_name).*|^[^N].*)", "gloss": ".*PL\\.SHORT($|(-[^LI]|-L[^O]|-I[^L]|-LO[^C]|-IL[^L]).*)"},
+  {"gramm": ".*,(?:persn|patrn|famn|anim|lang_name).*", "gloss": ".*PL\\.SHORT($|(-[^LI]|-L[^O]|-I[^L]|-LO[^C]|-IL[^L]).*)"},
+  {"gramm": "^[^VN].*", "gloss": ".*PL\\.SHORT.*"},
   {"gramm": "^(.(?!,nation))+$", "gloss": ".*SIM-(ACC|GEN|DAT|LAT|LOC|ILL|SIM|COM).*"},
   {"wf": "тӱрлӧ.*", "lemma": "^(тӱрлаш|тӱр)$"},
   {"gramm": ".*,(nom|acc|gen|dat|com|case_comp).*", "lemma": "ку-"},
   {"gramm": "^.*nmlz(.(?!,sg))+$", "wf": ".*маш$"},
   {"gramm": "CONJ.*", "wf": "^дена[тк]$"}
 ]
```

### Comparing `uniparser-meadow-mari-1.1.8/uniparser_meadow_mari/data_strict/lex_rules.txt` & `uniparser-meadow-mari-1.1.9/uniparser_meadow_mari/data_strict/lex_rules.txt`

 * *Files identical despite different names*

### Comparing `uniparser-meadow-mari-1.1.8/uniparser_meadow_mari/data_strict/lexemes.txt` & `uniparser-meadow-mari-1.1.9/uniparser_meadow_mari/data_strict/lexemes.txt`

 * *Files 0% similar despite different names*

```diff
@@ -8787,14 +8787,21 @@
  lex: Баркалов
  stem: баркалов.
  gramm: N,PN,famn
  paradigm: N_consonant
  trans_ru: Баркалов
 
 -lexeme
+ lex: Баркас
+ gramm: N,PN,persn
+ stem: баркас.
+ paradigm: N_consonant
+ trans_ru: Баркас
+
+-lexeme
  lex: Барклай-де-толли
  stem: барклай-де-толли.
  gramm: N,PN,famn
  paradigm: N_paroxyton_v_weak
  trans_ru: Барклай-де-толли
 
 -lexeme
@@ -29612,14 +29619,21 @@
  lex: Кажаева
  gramm: N,PN,famn
  stem: кажаева.|кажаевы.|кажаев.
  paradigm: N_paroxyton_v_weak
  trans_ru: Кажаева
 
 -lexeme
+ lex: Кажай
+ gramm: N,persn,PN
+ stem: кажай.|кажа.
+ paradigm: N_j
+ trans_ru: Кажай
+
+-lexeme
  lex: Кажвеле
  stem: кажвеле.
  gramm: N,PN,topn
  paradigm: N_paroxyton_v_weak
  trans_ru: Кажвеле
 
 -lexeme
@@ -29956,14 +29970,21 @@
  stem: какшамбал.
  gramm: N,PN,topn
  paradigm: N_consonant
  trans_ru: Кокшамбал
 
 -lexeme
  lex: Какшан
+ gramm: N,PN,topn
+ stem: какшан.
+ paradigm: N_consonant
+ trans_ru: Кокшага
+
+-lexeme
+ lex: Какшан
  stem: какшан.
  gramm: N,PN,topn
  paradigm: N_consonant
  trans_ru: Кокшайск
 
 -lexeme
  lex: Какшанмучаш
@@ -32188,14 +32209,21 @@
  lex: Керей
  stem: керей.|кере.
  gramm: N,PN,persn
  paradigm: N_j
  trans_ru: Керей
 
 -lexeme
+ lex: Керемлак
+ gramm: N,PN,topn
+ stem: керемлак.
+ paradigm: N_consonant
+ trans_ru: Керемлак
+
+-lexeme
  lex: Керенский
  stem: керенский.|керенски.
  gramm: N,PN,famn
  paradigm: N_j
  trans_ru: Керенский
 
 -lexeme
@@ -34232,14 +34260,21 @@
  lex: Колпакова
  stem: колпакова.|колпаковы.//колпакова.|колпаков.//колпакова.
  gramm: N,PN,famn
  paradigm: N_paroxyton_v_weak
  trans_ru: Колпакова
 
 -lexeme
+ lex: Колтак
+ gramm: N,PN,topn
+ stem: колтак.
+ paradigm: N_consonant
+ trans_ru: Колтак
+
+-lexeme
  lex: Колтаков
  stem: колтаков.
  gramm: N,PN,famn
  paradigm: N_consonant
  trans_ru: Колтаков
 
 -lexeme
@@ -36696,14 +36731,21 @@
  lex: Кувакин
  stem: кувакин.
  gramm: N,PN,famn
  paradigm: N_consonant
  trans_ru: Кувакин
 
 -lexeme
+ lex: Куван
+ gramm: N,topn,PN
+ stem: куван.
+ paradigm: N_consonant
+ trans_ru: Куван
+
+-lexeme
  lex: Кувшинов
  stem: кувшинов.
  gramm: N,PN,famn
  paradigm: N_consonant
  trans_ru: Кувшинов
 
 -lexeme
@@ -37970,14 +38012,21 @@
  lex: Кури
  stem: кури.
  gramm: N,PN,persn
  paradigm: N_paroxyton_v_strong
  trans_ru: Кури
 
 -lexeme
+ lex: Курий
+ gramm: N,persn,PN
+ stem: курий.|кури.
+ paradigm: N_j
+ trans_ru: Курий, Гурий
+
+-lexeme
  lex: Курилов
  stem: курилов.
  gramm: N,PN,famn
  paradigm: N_consonant
  trans_ru: Курилов
 
 -lexeme
@@ -43703,14 +43752,21 @@
  lex: Марткия
  stem: марткия.
  gramm: N,PN,persn
  paradigm: N_paroxyton_v_strong
  trans_ru: Марткия
 
 -lexeme
+ lex: Мартын
+ gramm: N,PN,topn
+ stem: мартын.
+ paradigm: N_consonant
+ trans_ru: Мартын (озеро)
+
+-lexeme
  lex: Мартыненко
  stem: мартыненко.|мартыненкы.//мартыненко.|мартыненк.//мартыненко.
  gramm: N,PN,famn
  paradigm: N_paroxyton_v_weak
  trans_ru: Мартыненко
 
 -lexeme
@@ -45040,14 +45096,21 @@
  lex: Микал
  stem: микал.
  gramm: N,PN,persn
  paradigm: N_consonant
  trans_ru: Микал (Михаил)
 
 -lexeme
+ lex: Микале
+ gramm: N,PN,persn
+ stem: микале.|микалы.|микал.
+ paradigm: N_paroxyton_v_weak
+ trans_ru: Микале, Михаил
+
+-lexeme
  lex: Микальмихайлов
  stem: микальмихайлов.
  gramm: N,PN,famn
  paradigm: N_consonant
  trans_ru: Микальмихайлов
 
 -lexeme
@@ -77961,14 +78024,21 @@
  lex: Чаркаю
  stem: чаркаю.
  gramm: N,PN,topn
  paradigm: N_paroxyton_v_weak
  trans_ru: Чаркаю
 
 -lexeme
+ lex: Чарла
+ gramm: N,topn,PN
+ stem: чарла.
+ paradigm: N_consonant
+ trans_ru: Царевококшайск
+
+-lexeme
  lex: Чарнур
  stem: чарнур.
  gramm: N,PN,topn
  paradigm: N_consonant
  trans_ru: Большой Царанур; Малый Царанур
 
 -lexeme
@@ -80593,14 +80663,21 @@
  lex: Шанцора
  stem: шанцора.|шанцоры.//шанцора.|шанцор.//шанцора.
  gramm: N,PN,persn
  paradigm: N_paroxyton_v_weak
  trans_ru: Шанцора
 
 -lexeme
+ lex: Шап
+ gramm: N,PN,topn
+ stem: шап.
+ paradigm: N_consonant
+ trans_ru: Шап
+
+-lexeme
  lex: Шаплак
  stem: шаплак.
  gramm: N,PN,topn
  paradigm: N_consonant
  trans_ru: Большой Шаплак
 
 -lexeme
@@ -82197,14 +82274,21 @@
  gramm: N,PN,topn
  stem: шолаҥыш.
  paradigm: N_consonant
  trans_ru: Шоланыш
 
 -lexeme
  lex: Шолеҥер
+ gramm: N,PN,topn
+ stem: шолеҥер.
+ paradigm: N_consonant
+ trans_ru: Шелангер
+
+-lexeme
+ lex: Шолеҥер
  gramm: N,topn,PN
  stem: шолеҥер.
  paradigm: N_consonant
  trans_ru: Шолнер
 
 -lexeme
  lex: Шолкадур
@@ -84822,14 +84906,21 @@
  stem: юкчи.
  gramm: N,PN,persn
  paradigm: N_paroxyton_v_strong
  trans_ru: Юкчи
 
 -lexeme
  lex: Юл
+ gramm: N,topn,PN
+ stem: юл.
+ paradigm: N_consonant
+ trans_ru: Волга
+
+-lexeme
+ lex: Юл
  stem: юл.
  gramm: N,PN,topn
  paradigm: N_consonant
  trans_ru: Юл
 
 -lexeme
  lex: Юлавий
@@ -90016,14 +90107,21 @@
  lex: ай
  gramm: INTRJ
  stem: ай.
  paradigm: Clitics
  trans_ru: ах, эх
 
 -lexeme
+ lex: ай-ай
+ gramm: INTRJ
+ stem: ай-ай.//ай-яй.
+ paradigm: Clitics
+ trans_ru: ах, эх
+
+-lexeme
  lex: айва
  stem: айва.|айвы.//айва.|айв.//айва.
  gramm: N,rus
  paradigm: N_paroxyton_v_weak
  trans_ru: айва
 
 -lexeme
@@ -91879,14 +91977,21 @@
  lex: амал
  stem: амал.
  gramm: N
  paradigm: N_consonant
  trans_ru: причина, повод; форма; случай
 
 -lexeme
+ lex: амалаш
+ gramm: V,intr
+ stem: амал.
+ paradigm: V_e
+ trans_ru: ловчить, изловчиться
+
+-lexeme
  lex: амалгаш
  stem: амалг.
  gramm: V
  paradigm: V_e
  trans_ru: закоснеть
 
 -lexeme
@@ -95517,14 +95622,21 @@
  lex: ать-уть
  gramm: INTRJ
  stem: ать-уть.
  paradigm: Clitics
  trans_ru: ать-уть
 
 -lexeme
+ lex: ау
+ gramm: INTRJ,rus
+ stem: а-у-у.
+ paradigm: Clitics
+ trans_ru: ау, отклик на зов, окрик при поиске
+
+-lexeme
  lex: аудио
  stem: аудио.|аудиы.//аудио.|ауди.//аудио.
  gramm: N,rus
  paradigm: N_paroxyton_v_weak
  trans_ru: аудио
 
 -lexeme
@@ -104637,14 +104749,21 @@
  stem: верховный.//вэрховный.|верховны.//вэрховны.
  gramm: A,rus
  paradigm: A_j
  trans_ru: верховный
 
 -lexeme
  lex: верч
+ gramm: POST
+ stem: верч.
+ paradigm: POST_ADV_Poss
+ trans_ru: для, ради, из-за
+
+-lexeme
+ lex: верч
  stem: верч.//вэрч.
  gramm: ADV
  paradigm: POST_ADV_Poss
  trans_ru: для, ради, из-за
 
 -lexeme
  lex: вершок
@@ -115419,14 +115538,21 @@
  stem: гофрированный.|гофрированны.
  gramm: A,rus
  paradigm: A_j
  trans_ru: гофрированный
 
 -lexeme
  lex: гоч
+ gramm: POST
+ stem: коч.
+ paradigm: POST_ADV_Poss
+ trans_ru: через; пока
+
+-lexeme
+ lex: гоч
  stem: гоч.
  gramm: POST
  paradigm: POST_ADV_Poss
  trans_ru: через; пока
 
 -lexeme
  lex: граб
@@ -131078,14 +131204,21 @@
  stem: йол.
  gramm: N,body
  paradigm: N_consonant
  trans_ru: нога, ножка
 
 -lexeme
  lex: йола
+ gramm: ADV
+ stem: йола.
+ paradigm: POST_ADV_Poss
+ trans_ru: на ногах
+
+-lexeme
+ lex: йола
  stem: йола.
  gramm: N
  paradigm: N_oxyton
  trans_ru: вина
 
 -lexeme
  lex: йола-вала
@@ -133514,14 +133647,21 @@
  stem: йып.
  gramm: N
  paradigm: N_consonant
  trans_ru: пика, копьё
 
 -lexeme
  lex: йып-йып
+ gramm: ADV
+ stem: йып.
+ paradigm: POST_ADV_Poss
+ trans_ru: совершенно, совсем
+
+-lexeme
+ lex: йып-йып
  stem: йып-йып.
  gramm: ADV
  paradigm: POST_ADV_Poss
  trans_ru: совершенно
 
 -lexeme
  lex: йыпар
@@ -134500,14 +134640,21 @@
  lex: йӧрал
  stem: йӧрал.
  gramm: A
  paradigm: A_consonant
  trans_ru: пригодный
 
 -lexeme
+ lex: йӧралаш
+ gramm: V,tr
+ stem: йӧрал.
+ paradigm: V_a
+ trans_ru: свалить
+
+-lexeme
  lex: йӧралташ
  stem: йӧралт.
  gramm: V
  paradigm: V_a
  trans_ru: валиться; умирать
 
 -lexeme
@@ -151514,14 +151661,21 @@
  lex: кочмывер
  stem: кочмывер.//кочмывэр.
  gramm: N
  paradigm: N_consonant
  trans_ru: столовая
 
 -lexeme
+ lex: кочо
+ gramm: A
+ stem: кочо.|кочы.|коч.
+ paradigm: A_paroxyton_v_weak
+ trans_ru: горький
+
+-lexeme
  lex: кочо-йӧсӧ
  stem: кочо-йӧсӧ.|кочо-йӧсы.|кочо-йӧс.
  gramm: N
  paradigm: N_paroxyton_v_weak
  trans_ru: несчастье
 
 -lexeme
@@ -157526,14 +157680,21 @@
  stem: кутузко.|кутузкы.|кутузк.
  gramm: N,rus
  paradigm: N_paroxyton_v_weak
  trans_ru: кутузка
 
 -lexeme
  lex: кутынек
+ gramm: ADV
+ stem: кутынек.
+ paradigm: POST_ADV_Poss
+ trans_ru: вдоль, по
+
+-lexeme
+ lex: кутынек
  stem: кутынек.
  gramm: POST
  paradigm: POST_ADV_Poss
  trans_ru: вдоль, по
 
 -lexeme
  lex: кутынь
@@ -158366,14 +158527,21 @@
  stem: кыж.
  gramm: IMIT
  paradigm: Clitics
  trans_ru: о бесшумном, малозаметном движении
 
 -lexeme
  lex: кыж-гож
+ gramm: IMIT
+ stem: кыж-кож.
+ paradigm: Clitics
+ trans_ru: о звуке шороха, шелеста
+
+-lexeme
+ lex: кыж-гож
  stem: кыж-гож.
  gramm: IMIT
  paradigm: Clitics
  trans_ru: о звуке шороха, шелеста
 
 -lexeme
  lex: кыжга
@@ -158939,14 +159107,21 @@
  lex: кыр-гор
  stem: кыр-гор.
  gramm: IMIT
  paradigm: Clitics
  trans_ru: о скребущем звуке или быстром движении
 
 -lexeme
+ lex: кыр-лук
+ gramm: IMIT
+ stem: кыр-лук.
+ paradigm: Clitics
+ trans_ru: о крике журавля
+
+-lexeme
  lex: кыра-сара
  stem: кыра-сара.
  gramm: N
  paradigm: N_oxyton
  trans_ru: негодное, нерадивое
 
 -lexeme
@@ -161187,14 +161362,21 @@
  lex: кӱлеш
  gramm: A
  stem: кӱлеш.
  paradigm: A_consonant
  trans_ru: нужный
 
 -lexeme
+ lex: кӱлеш
+ gramm: PREDIC
+ stem: кӱлеш.
+ paradigm: Clitics
+ trans_ru: нужно
+
+-lexeme
  lex: кӱлеш-оккӱл
  gramm: N
  stem: кӱлеш-огыл.
  paradigm: N_consonant
  trans_ru: нелепость
 
 -lexeme
@@ -162224,14 +162406,21 @@
  stem: кӱшклат.
  gramm: N
  paradigm: N_consonant
  trans_ru: верхняя клеть, второй этаж клети
 
 -lexeme
  lex: кӱшкыла
+ gramm: ADV
+ stem: кӱшкыла.
+ paradigm: POST_ADV_Poss
+ trans_ru: наверх
+
+-lexeme
+ lex: кӱшкыла
  stem: кӱшкыла.
  gramm: POST
  paradigm: POST_ADV_Poss
  trans_ru: наверх
 
 -lexeme
  lex: кӱшкӧ
@@ -163449,14 +163638,21 @@
  stem: ласа.
  gramm: PART
  paradigm: Clitics
  trans_ru: ведь, же
 
 -lexeme
  lex: ласка
+ gramm: ADV,rus
+ stem: ласка.
+ paradigm: POST_ADV_Poss
+ trans_ru: cпокойно, приятно
+
+-lexeme
+ lex: ласка
  stem: ласка.
  gramm: A,rus
  paradigm: A_oxyton
  trans_ru: ласковый
 
 -lexeme
  lex: ласка
@@ -164660,14 +164856,21 @@
  stem: леп.//лэп.
  gramm: N,body
  paradigm: N_consonant
  trans_ru: селезёнка
 
 -lexeme
  lex: леп-леве
+ gramm: A
+ stem: леп-леп.
+ paradigm: A_consonant
+ trans_ru: тёплый
+
+-lexeme
+ lex: леп-леве
  stem: леп-леве.//леп-левэ.|леп-левы.//леп-лэвы.|леп-лев.//леп-лэв.
  gramm: A
  paradigm: A_paroxyton_v_weak
  trans_ru: тёплый-тёплый
 
 -lexeme
  lex: лепене
@@ -180330,14 +180533,21 @@
  stem: мучката.
  gramm: A
  paradigm: A_oxyton
  trans_ru: полный, тучный, толстый
 
 -lexeme
  lex: мучко
+ gramm: ADV
+ stem: мучко.
+ paradigm: POST_ADV_Poss
+ trans_ru: целиком; сплошь; вдоль
+
+-lexeme
+ lex: мучко
  stem: мучко.
  gramm: POST
  paradigm: POST_ADV_Poss
  trans_ru: целиком; сплошь; вдоль
 
 -lexeme
  lex: мучко-мучко
@@ -210083,14 +210293,21 @@
  stem: почерк.//почэрк.
  gramm: N,rus
  paradigm: N_consonant
  trans_ru: почерк
 
 -lexeme
  lex: почеш
+ gramm: ADV
+ stem: почеш.
+ paradigm: POST_ADV_Poss
+ trans_ru: следом
+
+-lexeme
+ lex: почеш
  gramm: POST
  stem: почеш.
  paradigm: POST_ADV_Poss
  trans_ru: за, по, вслед, после
 
 -lexeme
  lex: почеш
@@ -219841,14 +220058,21 @@
  lex: пышкыраш
  stem: пышкыр.
  gramm: V
  paradigm: V_e
  trans_ru: фыркать
 
 -lexeme
+ lex: пышт
+ gramm: IMIT
+ stem: пышт.
+ paradigm: Clitics
+ trans_ru: о пыхтении
+
+-lexeme
  lex: пышт-пошт
  stem: пышт-пошт.
  gramm: IMIT
  paradigm: Clitics
  trans_ru: о сухом негромком звуке
 
 -lexeme
@@ -252474,14 +252698,21 @@
  stem: торец.//торэц.
  gramm: N,rus
  paradigm: N_consonant
  trans_ru: торец
 
 -lexeme
  lex: тореш
+ gramm: ADV
+ stem: тореш.
+ paradigm: POST_ADV_Poss
+ trans_ru: напротив; поперёк
+
+-lexeme
+ lex: тореш
  gramm: POST
  stem: тореш.
  paradigm: POST_ADV_Poss
  trans_ru: напротив; поперёк
 
 -lexeme
  lex: тореш
@@ -256320,14 +256551,21 @@
  stem: тур.
  gramm: N,rus
  paradigm: N_consonant
  trans_ru: тур
 
 -lexeme
  lex: тура
+ gramm: ADV
+ stem: тура.
+ paradigm: POST_ADV_Poss
+ trans_ru: круто
+
+-lexeme
+ lex: тура
  gramm: N,supernat
  stem: тура.
  paradigm: N_oxyton
  trans_ru: полуденица (миф. существо, являющееся в полдень)
 
 -lexeme
  lex: тура
@@ -270085,14 +270323,21 @@
  lex: фуфик
  stem: фуфик.
  gramm: N,rus,anim,hum
  paradigm: N_consonant
  trans_ru: фуфик
 
 -lexeme
+ lex: фыр
+ gramm: IMIT,rus
+ stem: фыр.
+ paradigm: Clitics
+ trans_ru: фыр, о выходе воздуха, пара
+
+-lexeme
  lex: фыр-р
  stem: фыр-р.
  gramm: IMIT
  paradigm: Clitics
  trans_ru: о звуке фырканья
 
 -lexeme
@@ -272956,14 +273201,21 @@
  stem: чап.
  gramm: N
  paradigm: N_consonant
  trans_ru: слава; уважение
 
 -lexeme
  lex: чап-чап
+ gramm: IMIT
+ stem: чап-чап.
+ paradigm: Clitics
+ trans_ru: о крике синицы
+
+-lexeme
+ lex: чап-чап
  stem: чап-чап.
  gramm: IMIT
  paradigm: Clitics
  trans_ru: об ударах веником в бане
 
 -lexeme
  lex: чап-чара
@@ -294861,14 +295113,21 @@
  lex: шӱштӱштӧ
  stem: шӱштӱштӧ.|шӱштӱшты.|шӱштӱшт.
  gramm: N
  paradigm: N_paroxyton_v_weak
  trans_ru: ремень, кожаный пояс
 
 -lexeme
+ lex: шӱялташ
+ gramm: V,tr
+ stem: шӱялт.
+ paradigm: V_e
+ trans_ru: полоскать
+
+-lexeme
  lex: шӱяш
  stem: шӱ.|шӱй.
  gramm: V
  paradigm: V_ya
  trans_ru: гнить
 
 -lexeme
@@ -305201,15 +305460,15 @@
  trans_ru: сметана
 
 -lexeme
  lex: ӱмбал
  stem: ӱмбал.|ӱмба.
  gramm: N,rel_n
  paradigm: POST
- trans_ru: поверхность; наверху
+ trans_ru: верх, поверхность; наверху
 
 -lexeme
  lex: ӱмбала
  stem: ӱмбала.
  gramm: ADV
  paradigm: POST_ADV_Poss
  trans_ru: друг на друга; двухэтажный; многократно; поверх, один на другой
```

### Comparing `uniparser-meadow-mari-1.1.8/uniparser_meadow_mari/data_strict/meadow_mari_disambiguation.cg3` & `uniparser-meadow-mari-1.1.9/uniparser_meadow_mari/data_strict/meadow_mari_disambiguation.cg3`

 * *Files identical despite different names*

### Comparing `uniparser-meadow-mari-1.1.8/uniparser_meadow_mari/data_strict/paradigms.txt` & `uniparser-meadow-mari-1.1.9/uniparser_meadow_mari/data_strict/paradigms.txt`

 * *Files identical despite different names*

### Comparing `uniparser-meadow-mari-1.1.8/uniparser_meadow_mari.egg-info/PKG-INFO` & `uniparser-meadow-mari-1.1.9/uniparser_meadow_mari.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uniparser-meadow-mari
-Version: 1.1.8
+Version: 1.1.9
 Summary: Rule-based morphological analysis for Meadow Mari
 Home-page: https://github.com/timarkh/uniparser-grammar-meadow-mari
 Author: Timofey Arkhangelskiy
 Author-email: timarkh@gmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/timarkh/uniparser-grammar-meadow-mari/issues
 Platform: UNKNOWN
```

### Comparing `uniparser-meadow-mari-1.1.8/uniparser_meadow_mari.egg-info/SOURCES.txt` & `uniparser-meadow-mari-1.1.9/uniparser_meadow_mari.egg-info/SOURCES.txt`

 * *Files identical despite different names*

