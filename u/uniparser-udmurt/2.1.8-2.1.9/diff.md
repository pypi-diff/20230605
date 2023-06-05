# Comparing `tmp/uniparser-udmurt-2.1.8.tar.gz` & `tmp/uniparser-udmurt-2.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uniparser-udmurt-2.1.8.tar", last modified: Fri Nov 19 11:07:49 2021, max compression
+gzip compressed data, was "uniparser-udmurt-2.1.9.tar", last modified: Mon Nov 22 10:26:56 2021, max compression
```

## Comparing `uniparser-udmurt-2.1.8.tar` & `uniparser-udmurt-2.1.9.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2021-11-19 11:07:49.840947 uniparser-udmurt-2.1.8/
--rw-rw-rw-   0        0        0     1167 2021-09-30 12:32:07.000000 uniparser-udmurt-2.1.8/LICENSE
--rw-rw-rw-   0        0        0      186 2021-03-22 10:35:22.000000 uniparser-udmurt-2.1.8/MANIFEST.in
--rw-rw-rw-   0        0        0     5458 2021-11-19 11:07:49.840947 uniparser-udmurt-2.1.8/PKG-INFO
--rw-rw-rw-   0        0        0     4749 2021-03-22 10:35:22.000000 uniparser-udmurt-2.1.8/README.md
--rw-rw-rw-   0        0        0      108 2021-03-22 10:35:22.000000 uniparser-udmurt-2.1.8/pyproject.toml
--rw-rw-rw-   0        0        0      818 2021-11-19 11:07:49.842937 uniparser-udmurt-2.1.8/setup.cfg
-drwxrwxrwx   0        0        0        0 2021-11-19 11:07:49.749798 uniparser-udmurt-2.1.8/uniparser_udmurt/
--rw-rw-rw-   0        0        0     2406 2021-03-22 10:35:22.000000 uniparser-udmurt-2.1.8/uniparser_udmurt/__init__.py
-drwxrwxrwx   0        0        0        0 2021-11-19 11:07:49.784923 uniparser-udmurt-2.1.8/uniparser_udmurt/data_nodiacritics/
--rw-rw-rw-   0        0        0        0 2021-03-22 10:35:22.000000 uniparser-udmurt-2.1.8/uniparser_udmurt/data_nodiacritics/__init__.py
--rw-rw-rw-   0        0        0     5848 2021-11-19 10:51:13.000000 uniparser-udmurt-2.1.8/uniparser_udmurt/data_nodiacritics/bad_analyses.txt
--rw-rw-rw-   0        0        0   753297 2021-11-19 10:53:49.000000 uniparser-udmurt-2.1.8/uniparser_udmurt/data_nodiacritics/lex_rules.txt
--rw-rw-rw-   0        0        0  6697381 2021-11-19 10:53:49.000000 uniparser-udmurt-2.1.8/uniparser_udmurt/data_nodiacritics/lexemes.txt
--rw-rw-rw-   0        0        0   185884 2021-11-19 10:53:49.000000 uniparser-udmurt-2.1.8/uniparser_udmurt/data_nodiacritics/paradigms.txt
--rw-rw-rw-   0        0        0    14194 2021-09-30 12:32:07.000000 uniparser-udmurt-2.1.8/uniparser_udmurt/data_nodiacritics/udmurt_disambiguation.cg3
-drwxrwxrwx   0        0        0        0 2021-11-19 11:07:49.838947 uniparser-udmurt-2.1.8/uniparser_udmurt/data_strict/
--rw-rw-rw-   0        0        0        0 2021-03-22 10:35:22.000000 uniparser-udmurt-2.1.8/uniparser_udmurt/data_strict/__init__.py
--rw-rw-rw-   0        0        0     5848 2021-11-19 10:51:13.000000 uniparser-udmurt-2.1.8/uniparser_udmurt/data_strict/bad_analyses.txt
--rw-rw-rw-   0        0        0   753297 2021-11-19 10:53:49.000000 uniparser-udmurt-2.1.8/uniparser_udmurt/data_strict/lex_rules.txt
--rw-rw-rw-   0        0        0  6614374 2021-11-19 10:53:48.000000 uniparser-udmurt-2.1.8/uniparser_udmurt/data_strict/lexemes.txt
--rw-rw-rw-   0        0        0   179589 2021-11-19 10:53:49.000000 uniparser-udmurt-2.1.8/uniparser_udmurt/data_strict/paradigms.txt
--rw-rw-rw-   0        0        0    14194 2021-09-30 12:32:07.000000 uniparser-udmurt-2.1.8/uniparser_udmurt/data_strict/udmurt_disambiguation.cg3
-drwxrwxrwx   0        0        0        0 2021-11-19 11:07:49.759698 uniparser-udmurt-2.1.8/uniparser_udmurt.egg-info/
--rw-rw-rw-   0        0        0     5458 2021-11-19 11:07:49.000000 uniparser-udmurt-2.1.8/uniparser_udmurt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      856 2021-11-19 11:07:49.000000 uniparser-udmurt-2.1.8/uniparser_udmurt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-11-19 11:07:49.000000 uniparser-udmurt-2.1.8/uniparser_udmurt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2021-11-19 11:07:49.000000 uniparser-udmurt-2.1.8/uniparser_udmurt.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2021-11-19 11:07:49.000000 uniparser-udmurt-2.1.8/uniparser_udmurt.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2021-11-22 10:26:56.709051 uniparser-udmurt-2.1.9/
+-rw-rw-rw-   0        0        0     1167 2021-09-30 12:32:07.000000 uniparser-udmurt-2.1.9/LICENSE
+-rw-rw-rw-   0        0        0      186 2021-03-22 10:35:22.000000 uniparser-udmurt-2.1.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     5458 2021-11-22 10:26:56.710048 uniparser-udmurt-2.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0     4749 2021-03-22 10:35:22.000000 uniparser-udmurt-2.1.9/README.md
+-rw-rw-rw-   0        0        0      108 2021-03-22 10:35:22.000000 uniparser-udmurt-2.1.9/pyproject.toml
+-rw-rw-rw-   0        0        0      818 2021-11-22 10:26:56.711045 uniparser-udmurt-2.1.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2021-11-22 10:26:56.635248 uniparser-udmurt-2.1.9/uniparser_udmurt/
+-rw-rw-rw-   0        0        0     2406 2021-03-22 10:35:22.000000 uniparser-udmurt-2.1.9/uniparser_udmurt/__init__.py
+drwxrwxrwx   0        0        0        0 2021-11-22 10:26:56.673160 uniparser-udmurt-2.1.9/uniparser_udmurt/data_nodiacritics/
+-rw-rw-rw-   0        0        0        0 2021-03-22 10:35:22.000000 uniparser-udmurt-2.1.9/uniparser_udmurt/data_nodiacritics/__init__.py
+-rw-rw-rw-   0        0        0     5903 2021-11-22 09:50:01.000000 uniparser-udmurt-2.1.9/uniparser_udmurt/data_nodiacritics/bad_analyses.txt
+-rw-rw-rw-   0        0        0   753297 2021-11-22 10:07:58.000000 uniparser-udmurt-2.1.9/uniparser_udmurt/data_nodiacritics/lex_rules.txt
+-rw-rw-rw-   0        0        0  6701367 2021-11-22 10:07:58.000000 uniparser-udmurt-2.1.9/uniparser_udmurt/data_nodiacritics/lexemes.txt
+-rw-rw-rw-   0        0        0   190524 2021-11-22 10:07:58.000000 uniparser-udmurt-2.1.9/uniparser_udmurt/data_nodiacritics/paradigms.txt
+-rw-rw-rw-   0        0        0    14194 2021-09-30 12:32:07.000000 uniparser-udmurt-2.1.9/uniparser_udmurt/data_nodiacritics/udmurt_disambiguation.cg3
+drwxrwxrwx   0        0        0        0 2021-11-22 10:26:56.708053 uniparser-udmurt-2.1.9/uniparser_udmurt/data_strict/
+-rw-rw-rw-   0        0        0        0 2021-03-22 10:35:22.000000 uniparser-udmurt-2.1.9/uniparser_udmurt/data_strict/__init__.py
+-rw-rw-rw-   0        0        0     5903 2021-11-22 09:50:01.000000 uniparser-udmurt-2.1.9/uniparser_udmurt/data_strict/bad_analyses.txt
+-rw-rw-rw-   0        0        0   753297 2021-11-22 10:07:58.000000 uniparser-udmurt-2.1.9/uniparser_udmurt/data_strict/lex_rules.txt
+-rw-rw-rw-   0        0        0  6618243 2021-11-22 10:07:58.000000 uniparser-udmurt-2.1.9/uniparser_udmurt/data_strict/lexemes.txt
+-rw-rw-rw-   0        0        0   183442 2021-11-22 10:07:58.000000 uniparser-udmurt-2.1.9/uniparser_udmurt/data_strict/paradigms.txt
+-rw-rw-rw-   0        0        0    14194 2021-09-30 12:32:07.000000 uniparser-udmurt-2.1.9/uniparser_udmurt/data_strict/udmurt_disambiguation.cg3
+drwxrwxrwx   0        0        0        0 2021-11-22 10:26:56.645231 uniparser-udmurt-2.1.9/uniparser_udmurt.egg-info/
+-rw-rw-rw-   0        0        0     5458 2021-11-22 10:26:56.000000 uniparser-udmurt-2.1.9/uniparser_udmurt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      856 2021-11-22 10:26:56.000000 uniparser-udmurt-2.1.9/uniparser_udmurt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2021-11-22 10:26:56.000000 uniparser-udmurt-2.1.9/uniparser_udmurt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2021-11-22 10:26:56.000000 uniparser-udmurt-2.1.9/uniparser_udmurt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2021-11-22 10:26:56.000000 uniparser-udmurt-2.1.9/uniparser_udmurt.egg-info/top_level.txt
```

### Comparing `uniparser-udmurt-2.1.8/LICENSE` & `uniparser-udmurt-2.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `uniparser-udmurt-2.1.8/PKG-INFO` & `uniparser-udmurt-2.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uniparser-udmurt
-Version: 2.1.8
+Version: 2.1.9
 Summary: Rule-based morphological analysis for Udmurt
 Home-page: https://github.com/timarkh/uniparser-grammar-udm
 Author: Timofey Arkhangelskiy
 Author-email: timarkh@gmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/timarkh/uniparser-grammar-udm/issues
 Platform: UNKNOWN
```

### Comparing `uniparser-udmurt-2.1.8/README.md` & `uniparser-udmurt-2.1.9/README.md`

 * *Files identical despite different names*

### Comparing `uniparser-udmurt-2.1.8/setup.cfg` & `uniparser-udmurt-2.1.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2075 6e69 7061 7273 6572 2d75 646d   = uniparser-udm
 00000020: 7572 740d 0a76 6572 7369 6f6e 203d 2032  urt..version = 2
-00000030: 2e31 2e38 0d0a 6175 7468 6f72 203d 2054  .1.8..author = T
+00000030: 2e31 2e39 0d0a 6175 7468 6f72 203d 2054  .1.9..author = T
 00000040: 696d 6f66 6579 2041 726b 6861 6e67 656c  imofey Arkhangel
 00000050: 736b 6979 0d0a 6175 7468 6f72 5f65 6d61  skiy..author_ema
 00000060: 696c 203d 2074 696d 6172 6b68 4067 6d61  il = timarkh@gma
 00000070: 696c 2e63 6f6d 0d0a 6465 7363 7269 7074  il.com..descript
 00000080: 696f 6e20 3d20 5275 6c65 2d62 6173 6564  ion = Rule-based
 00000090: 206d 6f72 7068 6f6c 6f67 6963 616c 2061   morphological a
 000000a0: 6e61 6c79 7369 7320 666f 7220 5564 6d75  nalysis for Udmu
```

### Comparing `uniparser-udmurt-2.1.8/uniparser_udmurt/__init__.py` & `uniparser-udmurt-2.1.9/uniparser_udmurt/__init__.py`

 * *Files identical despite different names*

### Comparing `uniparser-udmurt-2.1.8/uniparser_udmurt/data_nodiacritics/bad_analyses.txt` & `uniparser-udmurt-2.1.9/uniparser_udmurt/data_nodiacritics/bad_analyses.txt`

 * *Files 1% similar despite different names*

```diff
@@ -98,10 +98,11 @@
   {"wf": "^.*ын(гес)?$", "gramm": ".*rel_n.*sg.*,ins.*"},
   {"wf": "^.*ы(гес)?$", "gramm": ".*rel_n.*,1sg.*", "lemma": "^([^п]|п[^а]).*$"},
   {"gramm": "V.*intr(.(?!caus))*pass,([12]|3,pl).*", "lemma": "^.*(?<!пырын|оскын|азьын|уккын|юлман|уттын|чигын|бусан|анжан|шайян|ртъян|рттын)ы$"},
   {"gramm": ".*,vn,.*attr_o.*"},
   {"wfGlossed": ".*ӟ-е-?м?[еы]?$", "gramm": ".*(fut(?!,neg)|3,pl,prs).*"},
   {"wfGlossed": "^[^-]*з-?ь($|-.*)", "lemma": ".*ӟ$"},
   {"wfGlossed": ".*-CAUS-CAUS-.*", "lemma": ".*уттыны"},
-  {"wfGlossed": ".*-[еэ]сь(-гес)?", "gramm": "^ADJ.*,pl,adj_nmlz,nom(,comp)?$"}
+  {"wfGlossed": ".*-[еэ]сь(-гес)?", "gramm": "^ADJ.*,pl,adj_nmlz,nom(,comp)?$"},
+  {"wf": "сиенъёслы", "gramm": ".*pl_comp"}
 ]
```

### Comparing `uniparser-udmurt-2.1.8/uniparser_udmurt/data_nodiacritics/lex_rules.txt` & `uniparser-udmurt-2.1.9/uniparser_udmurt/data_nodiacritics/lex_rules.txt`

 * *Files identical despite different names*

### Comparing `uniparser-udmurt-2.1.8/uniparser_udmurt/data_nodiacritics/lexemes.txt` & `uniparser-udmurt-2.1.9/uniparser_udmurt/data_nodiacritics/lexemes.txt`

 * *Files 0% similar despite different names*

```diff
@@ -37563,14 +37563,21 @@
  lex: Лоенгриновна
  stem: лоенгриновна.
  gramm: N,PN,patrn
  paradigm: Noun-num-vowel
  trans_ru: Лоенгриновна
 
 -lexeme
+ lex: Ложкари
+ gramm: N,PN
+ stem: ложкари.
+ paradigm: Noun-num-vowel
+ trans_ru: Ложкари (название ансамбля)
+
+-lexeme
  lex: Ложкин
  stem: ложкин.
  gramm: N,PN,famn
  paradigm: Noun-num-consonant
  trans_ru: Ложкин
 
 -lexeme
@@ -82402,14 +82409,21 @@
  lex: ализарин
  stem: ализарин.
  gramm: N,rus
  paradigm: Noun-num-consonant
  trans_ru: ализарин
 
 -lexeme
+ lex: алилы
+ stem: алилы.
+ gramm: ADV,dat
+ paradigm: connect_adverbs
+ trans_ru: на сейчас, до настоящего времени
+
+-lexeme
  lex: алимент
  stem: алимент.
  gramm: N,rus
  paradigm: Noun-num-consonant
  trans_ru: алимент
 
 -lexeme
@@ -85931,28 +85945,31 @@
  trans_ru: сам, свой
 
 -lexeme
  lex: ас
  stem: аслад.
  gramm: PRO,2sg,gen
  paradigm: Noun-case-compounding
+ paradigm: Noun-case-compounding-pl-consonant
  trans_ru: сам, свой
 
 -lexeme
  lex: ас
  stem: аслаз.
  gramm: PRO,3sg,gen
  paradigm: Noun-case-compounding
+ paradigm: Noun-case-compounding-pl-consonant
  trans_ru: сам, свой
 
 -lexeme
  lex: ас
  stem: аслам.
  gramm: PRO,1sg,gen
  paradigm: Noun-case-compounding
+ paradigm: Noun-case-compounding-pl-consonant
  trans_ru: сам, свой
 
 -lexeme
  lex: ас
  stem: аслыд.
  gramm: PRO,2sg,dat
  paradigm: Comparative
@@ -85970,31 +85987,37 @@
  stem: аслым.
  gramm: PRO,1sg,dat
  paradigm: Comparative
  trans_ru: сам, свой
 
 -lexeme
  lex: ас
- stem: аслэсьтыд.
+ stem: аслэсьтыд.//асьлэсьтыд.
  gramm: PRO,2sg,abl
  paradigm: Comparative
+ paradigm: Noun-case-compounding
+ paradigm: Noun-case-compounding-pl-consonant
  trans_ru: сам, свой
 
 -lexeme
  lex: ас
- stem: аслэсьтыз.
+ stem: аслэсьтыз.//асьлэсьтыз.
  gramm: PRO,3sg,abl
  paradigm: Comparative
+ paradigm: Noun-case-compounding
+ paradigm: Noun-case-compounding-pl-consonant
  trans_ru: сам, свой
 
 -lexeme
  lex: ас
- stem: аслэсьтым.
+ stem: аслэсьтым.//асьлэсьтым.
  gramm: PRO,1sg,abl
  paradigm: Comparative
+ paradigm: Noun-case-compounding
+ paradigm: Noun-case-compounding-pl-consonant
  trans_ru: сам, свой
 
 -lexeme
  lex: ас
  stem: асме.//асьме.//ащме.
  gramm: PRO,1sg,acc,nom
  paradigm: Comparative
@@ -86026,15 +86049,15 @@
  stem: астэ.//асьтэ.//ащтэ.
  gramm: PRO,2sg,acc,nom
  paradigm: Comparative
  trans_ru: сам, свой
 
 -lexeme
  lex: ас
- stem: астэс.//астэос.//ачидэс.//асьтэс.//ащтэс.
+ stem: астэс.//астэос.//астӥос.//астиос.//ачидэс.//асьтэс.//ащтэс.
  gramm: PRO,2pl,nom
  paradigm: Comparative
  trans_ru: сам, свой
 
 -lexeme
  lex: ас
  stem: асьме.
@@ -86064,14 +86087,24 @@
  trans_ru: сам, свой
 
 -lexeme
  lex: ас
  stem: асьмелэн.//асьмен.//асьмэн.
  gramm: PRO,1pl,gen
  paradigm: Comparative
+ paradigm: Noun-case-compounding
+ paradigm: Noun-case-compounding-pl-consonant
+ trans_ru: сам, свой
+
+-lexeme
+ lex: ас
+ stem: асьмелэс.
+ gramm: PRO,1pl,abl
+ paradigm: Noun-case-compounding-soft
+ paradigm: Noun-case-compounding-pl-soft
  trans_ru: сам, свой
 
 -lexeme
  lex: ас
  stem: асьмелэсь.
  gramm: PRO,1pl,abl
  paradigm: Comparative
@@ -86117,15 +86150,15 @@
  stem: асьсэдыз.//асьсэдыс.
  gramm: PRO,3pl,acc
  paradigm: Comparative
  trans_ru: сам, свой
 
 -lexeme
  lex: ас
- stem: асьсэзыз.
+ stem: асьсэзыз.//асьсэзыс.
  gramm: PRO,3pl,acc
  paradigm: Comparative
  trans_ru: сам, свой
 
 -lexeme
  lex: ас
  stem: асьсэлы.
@@ -86133,22 +86166,32 @@
  paradigm: Noun-num-vowel
  trans_ru: сам, свой
 
 -lexeme
  lex: ас
  stem: асьсэлэн.
  gramm: PRO,3pl,gen
- paradigm: Noun-num-consonant
+ paradigm: Comparative
+ paradigm: Noun-case-compounding
+ paradigm: Noun-case-compounding-pl-consonant
+ trans_ru: сам, свой
+
+-lexeme
+ lex: ас
+ stem: асьсэлэс.
+ gramm: PRO,3pl,abl
+ paradigm: Noun-case-compounding-soft
+ paradigm: Noun-case-compounding-pl-soft
  trans_ru: сам, свой
 
 -lexeme
  lex: ас
  stem: асьсэлэсь.
  gramm: PRO,3pl,abl
- paradigm: Noun-num-vowel
+ paradigm: Comparative
  trans_ru: сам, свой
 
 -lexeme
  lex: ас
  stem: асьсэос.//асьсэс.//асьсэёс.//асьсэес.
  gramm: PRO,3pl,nom
  paradigm: Noun-num-consonant
@@ -86187,36 +86230,46 @@
  stem: асьтэдыз.//асьтэдыс.
  gramm: PRO,2pl,acc
  paradigm: Comparative
  trans_ru: сам, свой
 
 -lexeme
  lex: ас
- stem: асьтэлы.
+ stem: асьтэлы.//асьтӥлы.//асьтилы.
  gramm: PRO,2pl,dat
  paradigm: Comparative
  trans_ru: сам, свой
 
 -lexeme
  lex: ас
- stem: асьтэлэн.
+ stem: асьтэлэн.//асьтӥлэн.//асьтилэн.
  gramm: PRO,2pl,gen
  paradigm: Comparative
+ paradigm: Noun-case-compounding
+ paradigm: Noun-case-compounding-pl-consonant
+ trans_ru: сам, свой
+
+-lexeme
+ lex: ас
+ stem: асьтэлэс.//асьтӥлэс.//асьтилэс.
+ gramm: PRO,2pl,abl
+ paradigm: Noun-case-compounding-soft
+ paradigm: Noun-case-compounding-pl-soft
  trans_ru: сам, свой
 
 -lexeme
  lex: ас
- stem: асьтэлэсь.
+ stem: асьтэлэсь.//асьтӥлэсь.//асьтилэсь.
  gramm: PRO,2pl,abl
  paradigm: Comparative
  trans_ru: сам, свой
 
 -lexeme
  lex: ас
- stem: асьтэос.//асьтэс.//асьтэёс.//асьтэес.
+ stem: асьтэос.//асьтӥос.//асьтиос.//асьтэс.//асьтэёс.//асьтэес.
  gramm: PRO,2pl,nom
  paradigm: Comparative
  trans_ru: сам, свой
 
 -lexeme
  lex: ас
  stem: асьтэтэк.
@@ -86229,35 +86282,56 @@
  stem: асьтэя.
  gramm: PRO,2pl,adv
  paradigm: Comparative
  trans_ru: сам, свой
 
 -lexeme
  lex: ас
- stem: асэныд.
+ stem: асэныд.//асьсэныд.
  gramm: PRO,2sg,ins
  paradigm: Comparative
  trans_ru: сам, свой
 
 -lexeme
  lex: ас
- stem: асэныз.
+ stem: асэныды.//асьсэныды.
+ gramm: PRO,2pl,ins
+ paradigm: Comparative
+ trans_ru: сам, свой
+
+-lexeme
+ lex: ас
+ stem: асэныз.//асьсэныз.
  gramm: PRO,3sg,ins
  paradigm: Comparative
  trans_ru: сам, свой
 
 -lexeme
  lex: ас
- stem: асэным.
+ stem: асэнызы.//асьсэнызы.
+ gramm: PRO,3pl,ins
+ paradigm: Comparative
+ trans_ru: сам, свой
+
+-lexeme
+ lex: ас
+ stem: асэным.//асьсэным.
  gramm: PRO,1sg,ins
  paradigm: Comparative
  trans_ru: сам, свой
 
 -lexeme
  lex: ас
+ stem: асэнымы.//асьмемын.//асьсэнымы.
+ gramm: PRO,1pl,ins
+ paradigm: Comparative
+ trans_ru: сам, свой
+
+-lexeme
+ lex: ас
  stem: ачид.
  gramm: PRO,2sg,nom
  paradigm: Comparative
  trans_ru: сам, свой
 
 -lexeme
  lex: ас
@@ -86710,14 +86784,21 @@
  lex: ассамблея
  stem: ассамблея.
  gramm: N,rus
  paradigm: Noun-num-vowel
  trans_ru: ассамблея
 
 -lexeme
+ lex: ассигнация
+ stem: ассигнация.
+ gramm: N,rus
+ paradigm: Noun-num-ija
+ trans_ru: ассигнация
+
+-lexeme
  lex: ассимилировать
  stem: ассимилировать.
  gramm: V,rus,rus_inf,rus_pfv_ipfv
  paradigm: Comparative
  trans_ru: ассимилировать
 
 -lexeme
@@ -121045,26 +121126,26 @@
  paradigm: Noun-num-consonant
  paradigm: Noun-num-consonant-y
  trans_ru: честь, слава, почёт, авторитет, достоинство
 
 -lexeme
  lex: данак
  stem: данак.
- gramm: ADJ
- paradigm: connect_adjectives
- trans_ru: порядочный, значительный, изрядный
-
--lexeme
- lex: данак
- stem: данак.
  gramm: ADV
  paradigm: connect_adverbs
  trans_ru: значительно, изрядно
 
 -lexeme
+ lex: данак
+ stem: данак.//данаг.
+ gramm: ADJ
+ paradigm: connect_adjectives
+ trans_ru: порядочный, значительный, изрядный
+
+-lexeme
  lex: данаклы
  stem: данаклы.
  gramm: ADV,dat
  paradigm: connect_adverbs
  trans_ru: намного, значительно
 
 -lexeme
@@ -128024,14 +128105,23 @@
  gramm: POST,missp
  paradigm: Comparative
  paradigm: poss-sg
  paradigm: poss-pl
  trans_ru: во время
 
 -lexeme
+ lex: дыръяку
+ stem: дыръяку.//дыръякы.
+ gramm: POST
+ paradigm: Comparative
+ paradigm: poss-sg
+ paradigm: poss-pl
+ trans_ru: во время
+
+-lexeme
  lex: дырын-дырын
  stem: дырын-дырын.
  gramm: ADV
  paradigm: connect_adverbs
  trans_ru: временами, иногда
 
 -lexeme
@@ -133267,14 +133357,21 @@
  lex: заморозить
  stem: заморозить.
  gramm: V,rus,rus_inf,rus_pfv
  paradigm: Comparative
  trans_ru: заморозить
 
 -lexeme
+ lex: заморозка
+ stem: заморозка.
+ gramm: N,rus
+ paradigm: Noun-num-vowel
+ trans_ru: заморозка
+
+-lexeme
  lex: замороченной
  stem: замороченно.//замороченны.
  gramm: ADJ,rus
  paradigm: connect_adjectives-j
  trans_ru: замороченный
 
 -lexeme
@@ -186947,14 +187044,21 @@
  lex: морозильник
  stem: морозильник.
  gramm: N,rus
  paradigm: Noun-num-consonant
  trans_ru: морозильник
 
 -lexeme
+ lex: морозить
+ stem: морозить.
+ gramm: V,rus,rus_inf,rus_ipfv
+ paradigm: Comparative
+ trans_ru: морозить
+
+-lexeme
  lex: моросить
  stem: моросить.
  gramm: V,rus,rus_inf,rus_ipfv
  paradigm: Comparative
  trans_ru: моросить
 
 -lexeme
@@ -196345,15 +196449,15 @@
  lex: номофобия
  stem: номофоби.
  gramm: N,rus
  paradigm: Noun-num-ija
  trans_ru: номофобия
 
 -lexeme
- lex: номыре
+ lex: номыр
  stem: номыр.
  gramm: PRO
  paradigm: Noun-mar
  trans_ru: ничто
 
 -lexeme
  lex: номыртэм
@@ -202115,14 +202219,21 @@
  lex: огмындаен
  stem: огмындаен.
  gramm: ADV
  paradigm: connect_adverbs
  trans_ru: поровну, одинаково [по количеству]
 
 -lexeme
+ lex: огмыр
+ stem: огмыр.
+ gramm: PRO
+ paradigm: Noun-mar
+ trans_ru: ничто
+
+-lexeme
  lex: огмытэмен
  gramm: ADV
  stem: огмытэмен.
  paradigm: connect_adverbs
  trans_ru: заодно, заодним (с начинанием)
 
 -lexeme
@@ -213691,14 +213802,21 @@
  lex: переиздать
  stem: переиздать.
  gramm: V,rus,rus_inf,rus_pfv
  paradigm: Comparative
  trans_ru: переиздать
 
 -lexeme
+ lex: переименовать
+ stem: переименовать.
+ gramm: V,rus,rus_inf,rus_pfv
+ paradigm: Comparative
+ trans_ru: переименовать
+
+-lexeme
  lex: перекантоваться
  stem: перекантоваться.
  gramm: V,rus,rus_inf,refl,rus_pfv
  paradigm: Comparative
  trans_ru: перекантоваться
 
 -lexeme
@@ -230380,14 +230498,21 @@
  lex: пумкыл
  stem: пумкыл.
  gramm: N
  paradigm: Noun-num-consonant
  trans_ru: 1. приговор, решение 2. суждение
 
 -lexeme
+ lex: пумкылъян
+ stem: пумкылъян.
+ gramm: N
+ paradigm: Noun-num-consonant
+ trans_ru: решение
+
+-lexeme
  lex: пумнала
  stem: пумнала.
  gramm: ADV
  paradigm: connect_adverbs
  trans_ru: беспрерывно, постоянно
 
 -lexeme
@@ -235097,14 +235222,28 @@
  lex: разбудить
  stem: разбудить.
  gramm: V,rus,rus_inf,rus_ipfv
  paradigm: Comparative
  trans_ru: разбудить
 
 -lexeme
+ lex: разваливать
+ stem: разваливать.
+ gramm: V,rus,rus_inf,rus_ipfv
+ paradigm: Comparative
+ trans_ru: разваливать
+
+-lexeme
+ lex: разваливаться
+ stem: разваливаться.
+ gramm: V,rus,rus_inf,refl,rus_ipfv
+ paradigm: Comparative
+ trans_ru: разваливаться
+
+-lexeme
  lex: развалить
  stem: развалить.
  gramm: V,rus,rus_inf,rus_pfv
  paradigm: Comparative
  trans_ru: развалить
 
 -lexeme
@@ -272351,14 +272490,21 @@
  lex: удысчи
  stem: удысчи.
  gramm: N,anim,hum
  paradigm: Noun-num-vowel
  trans_ru: специалист
 
 -lexeme
+ lex: удысэт
+ stem: удысэт.
+ gramm: N
+ paradigm: Noun-num-consonant
+ trans_ru: ведомство
+
+-lexeme
  lex: удысэто
  stem: удысэто.
  gramm: ADJ
  paradigm: connect_adjectives
  trans_ru: ведомственный
 
 -lexeme
@@ -274134,21 +274280,23 @@
  trans_ru: этикет
 
 -lexeme
  lex: улос
  stem: улос.
  gramm: N
  paradigm: Noun-num-consonant
- trans_ru: родная сторона, местность, область, округ, семья, общество, житьё
+ paradigm: Noun-num-consonant-y
+ trans_ru: родная сторона; область; житьё
 
 -lexeme
  lex: улосвыл
  stem: улосвыл.
  gramm: N
  paradigm: Noun-num-consonant
+ paradigm: Noun-num-consonant-y
  trans_ru: территория, область, пространство, площадь
 
 -lexeme
  lex: улоскыл
  stem: улоскыл.
  gramm: N
  paradigm: Noun-num-consonant
@@ -306500,17 +306648,24 @@
  gramm: V,I,tr
  paradigm: connect_verbs-I-CC
  trans_ru: сообразить, догадаться, прийти на ум, припомнить
 
 -lexeme
  lex: ятыр
  stem: ятыр.
+ gramm: ADJ
+ paradigm: connect_adjectives
+ trans_ru: значительный, излишний
+
+-lexeme
+ lex: ятыр
+ stem: ятыр.
  gramm: ADV
  paradigm: connect_adverbs
- trans_ru: 1. излишек, много, порядочно 2. Як-Бодьин. больше, более
+ trans_ru: много, излишек
 
 -lexeme
  lex: яукал
  stem: яукал.
  gramm: N,anim,hum
  paradigm: Noun-num-consonant
  trans_ru: лодырь, тунеядец
@@ -311556,14 +311711,21 @@
  lex: ӧрекчи
  stem: ӧрекчи.//орекчи.
  gramm: N,anim,hum
  paradigm: Noun-num-vowel
  trans_ru: обманщик
 
 -lexeme
+ lex: ӧри
+ stem: ӧри.//ори.
+ gramm: N
+ paradigm: Noun-num-vowel
+ trans_ru: комитет
+
+-lexeme
  lex: ӧрланыны
  stem: ӧрлан.//орлан.
  gramm: V,I,intr
  paradigm: connect_verbs-I
  trans_ru: войти в раж, войти во вкус
 
 -lexeme
```

### Comparing `uniparser-udmurt-2.1.8/uniparser_udmurt/data_nodiacritics/paradigms.txt` & `uniparser-udmurt-2.1.9/uniparser_udmurt/data_nodiacritics/paradigms.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1816,14 +1816,104 @@
   gramm: case_comp,poss_comp,term
   gloss: TERM|P.3SG
  -flex: .етӥ|з<.>//.ети|з<.>//.ьытӥ|з<.>//.ьыти|з<.>//.ьтӥ|з<.>//.ьти|з<.>//.ети|з<.>//.ьыти|з<.>//.ьти|з<.>
   gramm: case_comp,poss_comp,prol
   gloss: PROL|P.3SG
  paradigm: Comparative
 
+-paradigm: Noun-case-compounding-pl-consonant
+ -flex: .ъёс|ыз<.>//.ъес|ыз<.>
+  gramm: case_comp,pl_comp,pl,acc
+  gloss: PL|ACC
+ -flex: .ъёс|ты<.>//.ъес|ты<.>
+  gramm: case_comp,pl_comp,pl,acc
+  gloss: PL|ACC.PL
+ -flex: .ъёс|лэн<.>//.ъес|лэн<.>
+  gramm: case_comp,pl_comp,pl,gen
+  gloss: PL|GEN
+ -flex: .ъёс|лэсь<.>//.ъес|лэсь<.>
+  gramm: case_comp,pl_comp,pl,abl
+  gloss: PL|ABL
+ -flex: .ъёс|лы<.>//.ъес|лы<.>
+  gramm: case_comp,pl_comp,pl,dat
+  gloss: PL|DAT
+ -flex: .ъёс|тэк<.>//.ъес|тэк<.>
+  gramm: case_comp,pl_comp,pl,car
+  gloss: PL|CAR
+ -flex: .ъёс|ъя<.>//.ъес|ъя<.>
+  gramm: case_comp,pl_comp,pl,adv
+  gloss: PL|ADV
+ -flex: .ъёс|ын<.>//.ъес|ын<.>
+  gramm: case_comp,pl_comp,pl,loc
+  gloss: PL|LOC
+ -flex: .ъёс|ы<.>//.ъес|ы<.>
+  gramm: case_comp,pl_comp,pl,ill
+  gloss: PL|ILL
+ -flex: .ъёс|ысь<.>//.ъес|ысь<.>
+  gramm: case_comp,pl_comp,pl,el
+  gloss: PL|EL
+ -flex: .ъёс|ысен<.>//.ъес|ысен<.>
+  gramm: case_comp,pl_comp,pl,egr
+  gloss: PL|EGR
+ -flex: .ъёс|озь<.>//.ъес|озь<.>
+  gramm: case_comp,pl_comp,pl,term
+  gloss: PL|TERM
+ -flex: .ъёс|ытӥ<.>//.ъес|ыти<.>//.ъёс|тӥ<.>//.ъес|ти<.>//.ъёс|этӥ<.>//.ъес|эти<.>//.ъёс|ыти<.>//.ъес|ыти<.>//.ъёс|ти<.>//.ъес|ти<.>//.ъёс|эти<.>//.ъес|эти<.>
+  gramm: case_comp,pl_comp,pl,prol
+  gloss: PL|PROL
+ -flex: .ъёс|лань<.>//.ъес|лань<.>
+  gramm: case_comp,pl_comp,pl,app
+  gloss: PL|APP
+ -flex: .ъёс|ыз<.>//.ъес|ыз<.>
+  gramm: case_comp,pl_comp,pl,poss_comp,nom
+  gloss: PL|P.3SG
+ -flex: .ъёс|ыз|лэн<.>//.ъес|ыз|лэн<.>
+  gramm: case_comp,pl_comp,pl,poss_comp,gen
+  gloss: PL|P.3SG|GEN
+ -flex: .ъёс|ыз|лэсь<.>//.ъес|ыз|лэсь<.>
+  gramm: case_comp,pl_comp,pl,poss_comp,abl
+  gloss: PL|P.3SG|ABL
+ -flex: .ъёс|ыз|лы<.>//.ъес|ыз|лы<.>
+  gramm: case_comp,pl_comp,pl,poss_comp,dat
+  gloss: PL|P.3SG|DAT
+ -flex: .ъёс|ыз|тэк<.>//.ъес|ыз|тэк<.>
+  gramm: case_comp,pl_comp,pl,poss_comp,car
+  gloss: PL|P.3SG|CAR
+ -flex: .ъёс|ыз|ъя<.>//.ъес|ыз|ъя<.>
+  gramm: case_comp,pl_comp,pl,poss_comp,adv
+  gloss: PL|P.3SG|ADV
+ -flex: .ъёс|ыз|лань<.>//.ъес|ыз|лань<.>
+  gramm: case_comp,pl_comp,pl,poss_comp,app
+  gloss: PL|P.3SG|APP
+ -flex: .ъёс|сэ<.>//.ъес|сэ<.>
+  gramm: case_comp,pl_comp,pl,poss_comp,acc
+  gloss: PL|P.3SG.ACC
+ -flex: .ъёс|ын|ыз<.>//.ъес|ын|ыз<.>
+  gramm: case_comp,pl_comp,pl,poss_comp,ins
+  gloss: PL|INS|P.3SG
+ -flex: .ъёс|а|з<.>//.ъес|а|з<.>
+  gramm: case_comp,pl_comp,pl,poss_comp,loc
+  gloss: PL|LOC|P.3SG
+ -flex: .ъёс|а|з<.>//.ъес|а|з<.>
+  gramm: case_comp,pl_comp,pl,poss_comp,ill
+  gloss: PL|ILL|P.3SG
+ -flex: .ъёс|ысьт|ыз<.>//.ъес|ысьт|ыз<.>
+  gramm: case_comp,pl_comp,pl,poss_comp,el
+  gloss: PL|EL|P.3SG
+ -flex: .ъёс|ысен|ыз<.>//.ъес|ысен|ыз<.>
+  gramm: case_comp,pl_comp,pl,poss_comp,egr
+  gloss: PL|EGR|P.3SG
+ -flex: .ъёс|озя|з<.>//.ъес|озя|з<.>
+  gramm: case_comp,pl_comp,pl,poss_comp,term
+  gloss: PL|TERM|P.3SG
+ -flex: .ъёс|ытӥ|з<.>//.ъес|ыти|з<.>//.ъёс|тӥ|з<.>//.ъес|ти|з<.>//.ъёс|этӥ|з<.>//.ъес|эти|з<.>//.ъёс|ыти|з<.>//.ъес|ыти|з<.>//.ъёс|ти|з<.>//.ъес|ти|з<.>//.ъёс|эти|з<.>//.ъес|эти|з<.>
+  gramm: case_comp,pl_comp,pl,poss_comp,prol
+  gloss: PL|PROL|P.3SG
+ paradigm: Comparative
+
 -paradigm: Noun-case-compounding-pl-soft
  -flex: .ьёс|ыз<.>//.ьес|ыз<.>
   gramm: case_comp,pl_comp,pl,acc
   gloss: PL|ACC
  -flex: .ьёс|ты<.>//.ьес|ты<.>
   gramm: case_comp,pl_comp,pl,acc
   gloss: PL|ACC.PL
@@ -2039,15 +2129,15 @@
  -flex: .эз<.>
   gramm: acc
   gloss: ACC
   paradigm: Comparative
  -flex: .ыз<.>
   gramm: acc
   gloss: ACC
-  regex-gramm: ^.*pl.*$
+  regex-prev-gramm: ^.*pl.*$
   paradigm: Comparative
  -flex: .ез<.>
   gramm: acc
   gloss: ACC
   regex-prev: ^.*[бвгжӟӝйкмпрфхцчӵшщаеёиӥоӧуыэюя][<>.]*$
   paradigm: Comparative
  -flex: .ты<.>
@@ -2055,52 +2145,59 @@
   gloss: ACC.PL
   regex-prev-gramm: ^.*pl.*$
   paradigm: Comparative
  -flex: .лэн<.>
   gramm: gen
   gloss: GEN
   paradigm: Noun-case-compounding
+  paradigm: Noun-case-compounding-pl-consonant
  -flex: .лэс<.>
   gramm: abl
   gloss: ABL
   paradigm: Noun-case-compounding-soft
+  paradigm: Noun-case-compounding-pl-soft
  -flex: .лэсь<.>
   gramm: abl
   gloss: ABL
   paradigm: Comparative
  -flex: .лы<.>
   gramm: dat
   gloss: DAT
   paradigm: Noun-case-compounding
+  paradigm: Noun-case-compounding-pl-consonant
  -flex: .эн<.>
   gramm: ins
   gloss: INS
   paradigm: Noun-case-compounding
+  paradigm: Noun-case-compounding-pl-consonant
  -flex: .ен<.>
   gramm: ins
   gloss: INS
   regex-prev: ^.*[бвгжӟӝйкмпрфхцчӵшщаеёиӥоӧуыэюя][<>.]*$
   paradigm: Noun-case-compounding
+  paradigm: Noun-case-compounding-pl-consonant
  -flex: .тэк<.>
   gramm: car
   gloss: CAR
   paradigm: Noun-case-compounding
+  paradigm: Noun-case-compounding-pl-consonant
  -flex: .ъя<.>
   gramm: adv
   gloss: ADV
   paradigm: Comparative
  -flex: .я<.>
   gramm: adv
   gloss: ADV
   paradigm: Comparative
   regex-prev: ^.*[ьйаеёиӥоӧуыэюя][<>.]*$
  -flex: .ын<.>
   gramm: loc
   gloss: LOC
   paradigm: Noun-case-compounding
+  paradigm: Noun-case-compounding-pl-consonant
  -flex: .э<.>
   gramm: ill
   gloss: ILL
   paradigm: Comparative
  -flex: .е<.>
   gramm: ill
   gloss: ILL
@@ -2135,23 +2232,26 @@
   gloss: EL
   paradigm: Comparative
   regex-prev: ^.*[бвгжӟӝйкмпрфхцчӵшщаеёиӥоӧуыэюя][<>.]*$
  -flex: .ысен<.>
   gramm: egr
   gloss: EGR
   paradigm: Noun-case-compounding
+  paradigm: Noun-case-compounding-pl-consonant
  -flex: .исен<.>
   gramm: egr,nonst
   gloss: EGR
   paradigm: Noun-case-compounding
+  paradigm: Noun-case-compounding-pl-consonant
   regex-prev: ^.*[бвгжӟӝйкмпрфхцчӵшщаеёиӥоӧуыэюя][<>.]*$
  -flex: .ӥсен<.>//.исен<.>
   gramm: egr,nonst
   gloss: EGR
   paradigm: Noun-case-compounding
+  paradigm: Noun-case-compounding-pl-consonant
  -flex: .оз<.>
   gramm: term
   gloss: TERM
   paradigm: Noun-case-compounding-soft
  -flex: .озь<.>
   gramm: term
   gloss: TERM
@@ -2196,22 +2296,24 @@
   gramm: acc
   gloss: ACC
   paradigm: Comparative
  -flex: .ен<.>
   gramm: ins
   gloss: INS
   paradigm: Noun-case-compounding
+  paradigm: Noun-case-compounding-pl-consonant
  -flex: .я<.>
   gramm: adv
   gloss: ADV
   paradigm: Comparative
  -flex: .ын<.>
   gramm: loc
   gloss: LOC
   paradigm: Noun-case-compounding
+  paradigm: Noun-case-compounding-pl-consonant
  -flex: .е<.>
   gramm: ill
   gloss: ILL
   paradigm: Comparative
  -flex: .ыс<.>
   gramm: el
   gloss: EL
@@ -2232,18 +2334,20 @@
   gloss: EL
   paradigm: Comparative
   regex-prev: ^.*[бвгжӟӝйкмпрфхцчӵшщаеёиӥоӧуыэюя][<>.]*$
  -flex: .ысен<.>
   gramm: egr
   gloss: EGR
   paradigm: Noun-case-compounding
+  paradigm: Noun-case-compounding-pl-consonant
  -flex: .исен<.>
   gramm: egr,nonst
   gloss: EGR
   paradigm: Noun-case-compounding
+  paradigm: Noun-case-compounding-pl-consonant
   regex-prev: ^.*[бвгжӟӝйкмпрфхцчӵшщаеёиӥоӧуыэюя][<>.]*$
  -flex: .оз<.>
   gramm: term
   gloss: TERM
   paradigm: Noun-case-compounding-soft
  -flex: .озь<.>
   gramm: term
@@ -2360,21 +2464,21 @@
   gloss: APP
   paradigm: Comparative
 
 -paradigm: Noun-case-mar
  -flex: .е<.>
   gramm: nom
   gloss: NOM
-  regex-lex: ^номыре$
+  regex-lex: ^номыр$
  -flex: .<.>
   gramm: nom
  -flex: .е<.>//.э<.>
   gramm: acc
   gloss: ACC
-  regex-lex: ^.*(мар?|кин|со|та|номыре)$
+  regex-lex: ^.*(мар?|кин|со|та|номыр|огмыр)$
  -flex: .ты<.>
   gramm: acc
   gloss: ACC.PL
   regex-gramm: ^.*pl.*$
  -flex: .лэн<.>
   gramm: gen
   gloss: GEN
@@ -2440,42 +2544,48 @@
   gloss: ACC.PL
   regex-gramm: ^.*pl.*$
   paradigm: Comparative
  -flex: .лэн<.>
   gramm: gen
   gloss: GEN
   paradigm: Noun-case-compounding
+  paradigm: Noun-case-compounding-pl-consonant
  -flex: .лэс<.>
   gramm: abl
   gloss: ABL
   paradigm: Noun-case-compounding-soft
+  paradigm: Noun-case-compounding-pl-soft
  -flex: .лэсь<.>
   gramm: abl
   gloss: ABL
   paradigm: Comparative
  -flex: .лы<.>
   gramm: dat
   gloss: DAT
   paradigm: Noun-case-compounding
+  paradigm: Noun-case-compounding-pl-consonant
  -flex: .эн<.>//.ын<.>
   gramm: ins
   gloss: INS
   paradigm: Noun-case-compounding
+  paradigm: Noun-case-compounding-pl-consonant
  -flex: .тэк<.>
   gramm: car
   gloss: CAR
   paradigm: Noun-case-compounding
+  paradigm: Noun-case-compounding-pl-consonant
  -flex: .ъя<.>
   gramm: adv
   gloss: ADV
   paradigm: Comparative
  -flex: .ан<.>
   gramm: loc
   gloss: LOC
   paradigm: Noun-case-compounding
+  paradigm: Noun-case-compounding-pl-consonant
  -flex: .а<.>
   gramm: ill
   gloss: ILL
   paradigm: Comparative
  -flex: .ас<.>//.ыс<.>
   gramm: el
   gloss: EL
@@ -2485,14 +2595,15 @@
   gramm: el
   gloss: EL
   paradigm: Comparative
  -flex: .асен<.>//.ысен<.>
   gramm: egr
   gloss: EGR
   paradigm: Noun-case-compounding
+  paradigm: Noun-case-compounding-pl-consonant
  -flex: .оз<.>
   gramm: term
   gloss: TERM
   paradigm: Noun-case-compounding-soft
  -flex: .озь<.>
   gramm: term
   gloss: TERM
```

### Comparing `uniparser-udmurt-2.1.8/uniparser_udmurt/data_nodiacritics/udmurt_disambiguation.cg3` & `uniparser-udmurt-2.1.9/uniparser_udmurt/data_nodiacritics/udmurt_disambiguation.cg3`

 * *Files identical despite different names*

### Comparing `uniparser-udmurt-2.1.8/uniparser_udmurt/data_strict/bad_analyses.txt` & `uniparser-udmurt-2.1.9/uniparser_udmurt/data_strict/bad_analyses.txt`

 * *Files 1% similar despite different names*

```diff
@@ -98,10 +98,11 @@
   {"wf": "^.*ын(гес)?$", "gramm": ".*rel_n.*sg.*,ins.*"},
   {"wf": "^.*ы(гес)?$", "gramm": ".*rel_n.*,1sg.*", "lemma": "^([^п]|п[^а]).*$"},
   {"gramm": "V.*intr(.(?!caus))*pass,([12]|3,pl).*", "lemma": "^.*(?<!пырын|оскын|азьын|уккын|юлман|уттын|чигын|бусан|анжан|шайян|ртъян|рттын)ы$"},
   {"gramm": ".*,vn,.*attr_o.*"},
   {"wfGlossed": ".*ӟ-е-?м?[еы]?$", "gramm": ".*(fut(?!,neg)|3,pl,prs).*"},
   {"wfGlossed": "^[^-]*з-?ь($|-.*)", "lemma": ".*ӟ$"},
   {"wfGlossed": ".*-CAUS-CAUS-.*", "lemma": ".*уттыны"},
-  {"wfGlossed": ".*-[еэ]сь(-гес)?", "gramm": "^ADJ.*,pl,adj_nmlz,nom(,comp)?$"}
+  {"wfGlossed": ".*-[еэ]сь(-гес)?", "gramm": "^ADJ.*,pl,adj_nmlz,nom(,comp)?$"},
+  {"wf": "сиенъёслы", "gramm": ".*pl_comp"}
 ]
```

### Comparing `uniparser-udmurt-2.1.8/uniparser_udmurt/data_strict/lex_rules.txt` & `uniparser-udmurt-2.1.9/uniparser_udmurt/data_strict/lex_rules.txt`

 * *Files identical despite different names*

### Comparing `uniparser-udmurt-2.1.8/uniparser_udmurt/data_strict/lexemes.txt` & `uniparser-udmurt-2.1.9/uniparser_udmurt/data_strict/lexemes.txt`

 * *Files 0% similar despite different names*

```diff
@@ -37563,14 +37563,21 @@
  lex: Лоенгриновна
  stem: лоенгриновна.
  gramm: N,PN,patrn
  paradigm: Noun-num-vowel
  trans_ru: Лоенгриновна
 
 -lexeme
+ lex: Ложкари
+ gramm: N,PN
+ stem: ложкари.
+ paradigm: Noun-num-vowel
+ trans_ru: Ложкари (название ансамбля)
+
+-lexeme
  lex: Ложкин
  stem: ложкин.
  gramm: N,PN,famn
  paradigm: Noun-num-consonant
  trans_ru: Ложкин
 
 -lexeme
@@ -82401,14 +82408,21 @@
  lex: ализарин
  stem: ализарин.
  gramm: N,rus
  paradigm: Noun-num-consonant
  trans_ru: ализарин
 
 -lexeme
+ lex: алилы
+ stem: алилы.
+ gramm: ADV,dat
+ paradigm: connect_adverbs
+ trans_ru: на сейчас, до настоящего времени
+
+-lexeme
  lex: алимент
  stem: алимент.
  gramm: N,rus
  paradigm: Noun-num-consonant
  trans_ru: алимент
 
 -lexeme
@@ -85929,28 +85943,31 @@
  trans_ru: сам, свой
 
 -lexeme
  lex: ас
  stem: аслад.
  gramm: PRO,2sg,gen
  paradigm: Noun-case-compounding
+ paradigm: Noun-case-compounding-pl-consonant
  trans_ru: сам, свой
 
 -lexeme
  lex: ас
  stem: аслаз.
  gramm: PRO,3sg,gen
  paradigm: Noun-case-compounding
+ paradigm: Noun-case-compounding-pl-consonant
  trans_ru: сам, свой
 
 -lexeme
  lex: ас
  stem: аслам.
  gramm: PRO,1sg,gen
  paradigm: Noun-case-compounding
+ paradigm: Noun-case-compounding-pl-consonant
  trans_ru: сам, свой
 
 -lexeme
  lex: ас
  stem: аслыд.
  gramm: PRO,2sg,dat
  paradigm: Comparative
@@ -85968,31 +85985,37 @@
  stem: аслым.
  gramm: PRO,1sg,dat
  paradigm: Comparative
  trans_ru: сам, свой
 
 -lexeme
  lex: ас
- stem: аслэсьтыд.
+ stem: аслэсьтыд.//асьлэсьтыд.
  gramm: PRO,2sg,abl
  paradigm: Comparative
+ paradigm: Noun-case-compounding
+ paradigm: Noun-case-compounding-pl-consonant
  trans_ru: сам, свой
 
 -lexeme
  lex: ас
- stem: аслэсьтыз.
+ stem: аслэсьтыз.//асьлэсьтыз.
  gramm: PRO,3sg,abl
  paradigm: Comparative
+ paradigm: Noun-case-compounding
+ paradigm: Noun-case-compounding-pl-consonant
  trans_ru: сам, свой
 
 -lexeme
  lex: ас
- stem: аслэсьтым.
+ stem: аслэсьтым.//асьлэсьтым.
  gramm: PRO,1sg,abl
  paradigm: Comparative
+ paradigm: Noun-case-compounding
+ paradigm: Noun-case-compounding-pl-consonant
  trans_ru: сам, свой
 
 -lexeme
  lex: ас
  stem: асме.//асьме.//ащме.
  gramm: PRO,1sg,acc,nom
  paradigm: Comparative
@@ -86024,15 +86047,15 @@
  stem: астэ.//асьтэ.//ащтэ.
  gramm: PRO,2sg,acc,nom
  paradigm: Comparative
  trans_ru: сам, свой
 
 -lexeme
  lex: ас
- stem: астэс.//астэос.//ачидэс.//асьтэс.//ащтэс.
+ stem: астэс.//астэос.//астӥос.//ачидэс.//асьтэс.//ащтэс.
  gramm: PRO,2pl,nom
  paradigm: Comparative
  trans_ru: сам, свой
 
 -lexeme
  lex: ас
  stem: асьме.
@@ -86062,14 +86085,24 @@
  trans_ru: сам, свой
 
 -lexeme
  lex: ас
  stem: асьмелэн.//асьмен.//асьмэн.
  gramm: PRO,1pl,gen
  paradigm: Comparative
+ paradigm: Noun-case-compounding
+ paradigm: Noun-case-compounding-pl-consonant
+ trans_ru: сам, свой
+
+-lexeme
+ lex: ас
+ stem: асьмелэс.
+ gramm: PRO,1pl,abl
+ paradigm: Noun-case-compounding-soft
+ paradigm: Noun-case-compounding-pl-soft
  trans_ru: сам, свой
 
 -lexeme
  lex: ас
  stem: асьмелэсь.
  gramm: PRO,1pl,abl
  paradigm: Comparative
@@ -86115,15 +86148,15 @@
  stem: асьсэдыз.//асьсэдыс.
  gramm: PRO,3pl,acc
  paradigm: Comparative
  trans_ru: сам, свой
 
 -lexeme
  lex: ас
- stem: асьсэзыз.
+ stem: асьсэзыз.//асьсэзыс.
  gramm: PRO,3pl,acc
  paradigm: Comparative
  trans_ru: сам, свой
 
 -lexeme
  lex: ас
  stem: асьсэлы.
@@ -86131,22 +86164,32 @@
  paradigm: Noun-num-vowel
  trans_ru: сам, свой
 
 -lexeme
  lex: ас
  stem: асьсэлэн.
  gramm: PRO,3pl,gen
- paradigm: Noun-num-consonant
+ paradigm: Comparative
+ paradigm: Noun-case-compounding
+ paradigm: Noun-case-compounding-pl-consonant
+ trans_ru: сам, свой
+
+-lexeme
+ lex: ас
+ stem: асьсэлэс.
+ gramm: PRO,3pl,abl
+ paradigm: Noun-case-compounding-soft
+ paradigm: Noun-case-compounding-pl-soft
  trans_ru: сам, свой
 
 -lexeme
  lex: ас
  stem: асьсэлэсь.
  gramm: PRO,3pl,abl
- paradigm: Noun-num-vowel
+ paradigm: Comparative
  trans_ru: сам, свой
 
 -lexeme
  lex: ас
  stem: асьсэос.//асьсэс.//асьсэёс.
  gramm: PRO,3pl,nom
  paradigm: Noun-num-consonant
@@ -86185,36 +86228,46 @@
  stem: асьтэдыз.//асьтэдыс.
  gramm: PRO,2pl,acc
  paradigm: Comparative
  trans_ru: сам, свой
 
 -lexeme
  lex: ас
- stem: асьтэлы.
+ stem: асьтэлы.//асьтӥлы.
  gramm: PRO,2pl,dat
  paradigm: Comparative
  trans_ru: сам, свой
 
 -lexeme
  lex: ас
- stem: асьтэлэн.
+ stem: асьтэлэн.//асьтӥлэн.
  gramm: PRO,2pl,gen
  paradigm: Comparative
+ paradigm: Noun-case-compounding
+ paradigm: Noun-case-compounding-pl-consonant
+ trans_ru: сам, свой
+
+-lexeme
+ lex: ас
+ stem: асьтэлэс.//асьтӥлэс.
+ gramm: PRO,2pl,abl
+ paradigm: Noun-case-compounding-soft
+ paradigm: Noun-case-compounding-pl-soft
  trans_ru: сам, свой
 
 -lexeme
  lex: ас
- stem: асьтэлэсь.
+ stem: асьтэлэсь.//асьтӥлэсь.
  gramm: PRO,2pl,abl
  paradigm: Comparative
  trans_ru: сам, свой
 
 -lexeme
  lex: ас
- stem: асьтэос.//асьтэс.//асьтэёс.
+ stem: асьтэос.//асьтӥос.//асьтэс.//асьтэёс.
  gramm: PRO,2pl,nom
  paradigm: Comparative
  trans_ru: сам, свой
 
 -lexeme
  lex: ас
  stem: асьтэтэк.
@@ -86227,35 +86280,56 @@
  stem: асьтэя.
  gramm: PRO,2pl,adv
  paradigm: Comparative
  trans_ru: сам, свой
 
 -lexeme
  lex: ас
- stem: асэныд.
+ stem: асэныд.//асьсэныд.
  gramm: PRO,2sg,ins
  paradigm: Comparative
  trans_ru: сам, свой
 
 -lexeme
  lex: ас
- stem: асэныз.
+ stem: асэныды.//асьсэныды.
+ gramm: PRO,2pl,ins
+ paradigm: Comparative
+ trans_ru: сам, свой
+
+-lexeme
+ lex: ас
+ stem: асэныз.//асьсэныз.
  gramm: PRO,3sg,ins
  paradigm: Comparative
  trans_ru: сам, свой
 
 -lexeme
  lex: ас
- stem: асэным.
+ stem: асэнызы.//асьсэнызы.
+ gramm: PRO,3pl,ins
+ paradigm: Comparative
+ trans_ru: сам, свой
+
+-lexeme
+ lex: ас
+ stem: асэным.//асьсэным.
  gramm: PRO,1sg,ins
  paradigm: Comparative
  trans_ru: сам, свой
 
 -lexeme
  lex: ас
+ stem: асэнымы.//асьмемын.//асьсэнымы.
+ gramm: PRO,1pl,ins
+ paradigm: Comparative
+ trans_ru: сам, свой
+
+-lexeme
+ lex: ас
  stem: ачид.
  gramm: PRO,2sg,nom
  paradigm: Comparative
  trans_ru: сам, свой
 
 -lexeme
  lex: ас
@@ -86708,14 +86782,21 @@
  lex: ассамблея
  stem: ассамблея.
  gramm: N,rus
  paradigm: Noun-num-vowel
  trans_ru: ассамблея
 
 -lexeme
+ lex: ассигнация
+ stem: ассигнация.
+ gramm: N,rus
+ paradigm: Noun-num-ija
+ trans_ru: ассигнация
+
+-lexeme
  lex: ассимилировать
  stem: ассимилировать.
  gramm: V,rus,rus_inf,rus_pfv_ipfv
  paradigm: Comparative
  trans_ru: ассимилировать
 
 -lexeme
@@ -121036,26 +121117,26 @@
  paradigm: Noun-num-consonant
  paradigm: Noun-num-consonant-y
  trans_ru: честь, слава, почёт, авторитет, достоинство
 
 -lexeme
  lex: данак
  stem: данак.
- gramm: ADJ
- paradigm: connect_adjectives
- trans_ru: порядочный, значительный, изрядный
-
--lexeme
- lex: данак
- stem: данак.
  gramm: ADV
  paradigm: connect_adverbs
  trans_ru: значительно, изрядно
 
 -lexeme
+ lex: данак
+ stem: данак.//данаг.
+ gramm: ADJ
+ paradigm: connect_adjectives
+ trans_ru: порядочный, значительный, изрядный
+
+-lexeme
  lex: данаклы
  stem: данаклы.
  gramm: ADV,dat
  paradigm: connect_adverbs
  trans_ru: намного, значительно
 
 -lexeme
@@ -128015,14 +128096,23 @@
  gramm: POST,missp
  paradigm: Comparative
  paradigm: poss-sg
  paradigm: poss-pl
  trans_ru: во время
 
 -lexeme
+ lex: дыръяку
+ stem: дыръяку.//дыръякы.
+ gramm: POST
+ paradigm: Comparative
+ paradigm: poss-sg
+ paradigm: poss-pl
+ trans_ru: во время
+
+-lexeme
  lex: дырын-дырын
  stem: дырын-дырын.
  gramm: ADV
  paradigm: connect_adverbs
  trans_ru: временами, иногда
 
 -lexeme
@@ -133258,14 +133348,21 @@
  lex: заморозить
  stem: заморозить.
  gramm: V,rus,rus_inf,rus_pfv
  paradigm: Comparative
  trans_ru: заморозить
 
 -lexeme
+ lex: заморозка
+ stem: заморозка.
+ gramm: N,rus
+ paradigm: Noun-num-vowel
+ trans_ru: заморозка
+
+-lexeme
  lex: замороченной
  stem: замороченно.//замороченны.
  gramm: ADJ,rus
  paradigm: connect_adjectives-j
  trans_ru: замороченный
 
 -lexeme
@@ -186927,14 +187024,21 @@
  lex: морозильник
  stem: морозильник.
  gramm: N,rus
  paradigm: Noun-num-consonant
  trans_ru: морозильник
 
 -lexeme
+ lex: морозить
+ stem: морозить.
+ gramm: V,rus,rus_inf,rus_ipfv
+ paradigm: Comparative
+ trans_ru: морозить
+
+-lexeme
  lex: моросить
  stem: моросить.
  gramm: V,rus,rus_inf,rus_ipfv
  paradigm: Comparative
  trans_ru: моросить
 
 -lexeme
@@ -196325,15 +196429,15 @@
  lex: номофобия
  stem: номофоби.
  gramm: N,rus
  paradigm: Noun-num-ija
  trans_ru: номофобия
 
 -lexeme
- lex: номыре
+ lex: номыр
  stem: номыр.
  gramm: PRO
  paradigm: Noun-mar
  trans_ru: ничто
 
 -lexeme
  lex: номыртэм
@@ -202090,14 +202194,21 @@
  lex: огмындаен
  stem: огмындаен.
  gramm: ADV
  paradigm: connect_adverbs
  trans_ru: поровну, одинаково [по количеству]
 
 -lexeme
+ lex: огмыр
+ stem: огмыр.
+ gramm: PRO
+ paradigm: Noun-mar
+ trans_ru: ничто
+
+-lexeme
  lex: огмытэмен
  gramm: ADV
  stem: огмытэмен.
  paradigm: connect_adverbs
  trans_ru: заодно, заодним (с начинанием)
 
 -lexeme
@@ -213665,14 +213776,21 @@
  lex: переиздать
  stem: переиздать.
  gramm: V,rus,rus_inf,rus_pfv
  paradigm: Comparative
  trans_ru: переиздать
 
 -lexeme
+ lex: переименовать
+ stem: переименовать.
+ gramm: V,rus,rus_inf,rus_pfv
+ paradigm: Comparative
+ trans_ru: переименовать
+
+-lexeme
  lex: перекантоваться
  stem: перекантоваться.
  gramm: V,rus,rus_inf,refl,rus_pfv
  paradigm: Comparative
  trans_ru: перекантоваться
 
 -lexeme
@@ -230352,14 +230470,21 @@
  lex: пумкыл
  stem: пумкыл.
  gramm: N
  paradigm: Noun-num-consonant
  trans_ru: 1. приговор, решение 2. суждение
 
 -lexeme
+ lex: пумкылъян
+ stem: пумкылъян.
+ gramm: N
+ paradigm: Noun-num-consonant
+ trans_ru: решение
+
+-lexeme
  lex: пумнала
  stem: пумнала.
  gramm: ADV
  paradigm: connect_adverbs
  trans_ru: беспрерывно, постоянно
 
 -lexeme
@@ -235066,14 +235191,28 @@
  lex: разбудить
  stem: разбудить.
  gramm: V,rus,rus_inf,rus_ipfv
  paradigm: Comparative
  trans_ru: разбудить
 
 -lexeme
+ lex: разваливать
+ stem: разваливать.
+ gramm: V,rus,rus_inf,rus_ipfv
+ paradigm: Comparative
+ trans_ru: разваливать
+
+-lexeme
+ lex: разваливаться
+ stem: разваливаться.
+ gramm: V,rus,rus_inf,refl,rus_ipfv
+ paradigm: Comparative
+ trans_ru: разваливаться
+
+-lexeme
  lex: развалить
  stem: развалить.
  gramm: V,rus,rus_inf,rus_pfv
  paradigm: Comparative
  trans_ru: развалить
 
 -lexeme
@@ -272311,14 +272450,21 @@
  lex: удысчи
  stem: удысчи.
  gramm: N,anim,hum
  paradigm: Noun-num-vowel
  trans_ru: специалист
 
 -lexeme
+ lex: удысэт
+ stem: удысэт.
+ gramm: N
+ paradigm: Noun-num-consonant
+ trans_ru: ведомство
+
+-lexeme
  lex: удысэто
  stem: удысэто.
  gramm: ADJ
  paradigm: connect_adjectives
  trans_ru: ведомственный
 
 -lexeme
@@ -274094,21 +274240,23 @@
  trans_ru: этикет
 
 -lexeme
  lex: улос
  stem: улос.
  gramm: N
  paradigm: Noun-num-consonant
- trans_ru: родная сторона, местность, область, округ, семья, общество, житьё
+ paradigm: Noun-num-consonant-y
+ trans_ru: родная сторона; область; житьё
 
 -lexeme
  lex: улосвыл
  stem: улосвыл.
  gramm: N
  paradigm: Noun-num-consonant
+ paradigm: Noun-num-consonant-y
  trans_ru: территория, область, пространство, площадь
 
 -lexeme
  lex: улоскыл
  stem: улоскыл.
  gramm: N
  paradigm: Noun-num-consonant
@@ -306452,17 +306600,24 @@
  gramm: V,I,tr
  paradigm: connect_verbs-I-CC
  trans_ru: сообразить, догадаться, прийти на ум, припомнить
 
 -lexeme
  lex: ятыр
  stem: ятыр.
+ gramm: ADJ
+ paradigm: connect_adjectives
+ trans_ru: значительный, излишний
+
+-lexeme
+ lex: ятыр
+ stem: ятыр.
  gramm: ADV
  paradigm: connect_adverbs
- trans_ru: 1. излишек, много, порядочно 2. Як-Бодьин. больше, более
+ trans_ru: много, излишек
 
 -lexeme
  lex: яукал
  stem: яукал.
  gramm: N,anim,hum
  paradigm: Noun-num-consonant
  trans_ru: лодырь, тунеядец
@@ -311507,14 +311662,21 @@
  lex: ӧрекчи
  stem: ӧрекчи.
  gramm: N,anim,hum
  paradigm: Noun-num-vowel
  trans_ru: обманщик
 
 -lexeme
+ lex: ӧри
+ stem: ӧри.
+ gramm: N
+ paradigm: Noun-num-vowel
+ trans_ru: комитет
+
+-lexeme
  lex: ӧрланыны
  stem: ӧрлан.
  gramm: V,I,intr
  paradigm: connect_verbs-I
  trans_ru: войти в раж, войти во вкус
 
 -lexeme
```

### Comparing `uniparser-udmurt-2.1.8/uniparser_udmurt/data_strict/paradigms.txt` & `uniparser-udmurt-2.1.9/uniparser_udmurt/data_strict/paradigms.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1816,14 +1816,104 @@
   gramm: case_comp,poss_comp,term
   gloss: TERM|P.3SG
  -flex: .етӥ|з<.>//.ьытӥ|з<.>//.ьтӥ|з<.>//.ети|з<.>//.ьыти|з<.>//.ьти|з<.>
   gramm: case_comp,poss_comp,prol
   gloss: PROL|P.3SG
  paradigm: Comparative
 
+-paradigm: Noun-case-compounding-pl-consonant
+ -flex: .ъёс|ыз<.>
+  gramm: case_comp,pl_comp,pl,acc
+  gloss: PL|ACC
+ -flex: .ъёс|ты<.>
+  gramm: case_comp,pl_comp,pl,acc
+  gloss: PL|ACC.PL
+ -flex: .ъёс|лэн<.>
+  gramm: case_comp,pl_comp,pl,gen
+  gloss: PL|GEN
+ -flex: .ъёс|лэсь<.>
+  gramm: case_comp,pl_comp,pl,abl
+  gloss: PL|ABL
+ -flex: .ъёс|лы<.>
+  gramm: case_comp,pl_comp,pl,dat
+  gloss: PL|DAT
+ -flex: .ъёс|тэк<.>
+  gramm: case_comp,pl_comp,pl,car
+  gloss: PL|CAR
+ -flex: .ъёс|ъя<.>
+  gramm: case_comp,pl_comp,pl,adv
+  gloss: PL|ADV
+ -flex: .ъёс|ын<.>
+  gramm: case_comp,pl_comp,pl,loc
+  gloss: PL|LOC
+ -flex: .ъёс|ы<.>
+  gramm: case_comp,pl_comp,pl,ill
+  gloss: PL|ILL
+ -flex: .ъёс|ысь<.>
+  gramm: case_comp,pl_comp,pl,el
+  gloss: PL|EL
+ -flex: .ъёс|ысен<.>
+  gramm: case_comp,pl_comp,pl,egr
+  gloss: PL|EGR
+ -flex: .ъёс|озь<.>
+  gramm: case_comp,pl_comp,pl,term
+  gloss: PL|TERM
+ -flex: .ъёс|ытӥ<.>//.ъёс|тӥ<.>//.ъёс|этӥ<.>//.ъёс|ыти<.>//.ъёс|ти<.>//.ъёс|эти<.>
+  gramm: case_comp,pl_comp,pl,prol
+  gloss: PL|PROL
+ -flex: .ъёс|лань<.>
+  gramm: case_comp,pl_comp,pl,app
+  gloss: PL|APP
+ -flex: .ъёс|ыз<.>
+  gramm: case_comp,pl_comp,pl,poss_comp,nom
+  gloss: PL|P.3SG
+ -flex: .ъёс|ыз|лэн<.>
+  gramm: case_comp,pl_comp,pl,poss_comp,gen
+  gloss: PL|P.3SG|GEN
+ -flex: .ъёс|ыз|лэсь<.>
+  gramm: case_comp,pl_comp,pl,poss_comp,abl
+  gloss: PL|P.3SG|ABL
+ -flex: .ъёс|ыз|лы<.>
+  gramm: case_comp,pl_comp,pl,poss_comp,dat
+  gloss: PL|P.3SG|DAT
+ -flex: .ъёс|ыз|тэк<.>
+  gramm: case_comp,pl_comp,pl,poss_comp,car
+  gloss: PL|P.3SG|CAR
+ -flex: .ъёс|ыз|ъя<.>
+  gramm: case_comp,pl_comp,pl,poss_comp,adv
+  gloss: PL|P.3SG|ADV
+ -flex: .ъёс|ыз|лань<.>
+  gramm: case_comp,pl_comp,pl,poss_comp,app
+  gloss: PL|P.3SG|APP
+ -flex: .ъёс|сэ<.>
+  gramm: case_comp,pl_comp,pl,poss_comp,acc
+  gloss: PL|P.3SG.ACC
+ -flex: .ъёс|ын|ыз<.>
+  gramm: case_comp,pl_comp,pl,poss_comp,ins
+  gloss: PL|INS|P.3SG
+ -flex: .ъёс|а|з<.>
+  gramm: case_comp,pl_comp,pl,poss_comp,loc
+  gloss: PL|LOC|P.3SG
+ -flex: .ъёс|а|з<.>
+  gramm: case_comp,pl_comp,pl,poss_comp,ill
+  gloss: PL|ILL|P.3SG
+ -flex: .ъёс|ысьт|ыз<.>
+  gramm: case_comp,pl_comp,pl,poss_comp,el
+  gloss: PL|EL|P.3SG
+ -flex: .ъёс|ысен|ыз<.>
+  gramm: case_comp,pl_comp,pl,poss_comp,egr
+  gloss: PL|EGR|P.3SG
+ -flex: .ъёс|озя|з<.>
+  gramm: case_comp,pl_comp,pl,poss_comp,term
+  gloss: PL|TERM|P.3SG
+ -flex: .ъёс|ытӥ|з<.>//.ъёс|тӥ|з<.>//.ъёс|этӥ|з<.>//.ъёс|ыти|з<.>//.ъёс|ти|з<.>//.ъёс|эти|з<.>
+  gramm: case_comp,pl_comp,pl,poss_comp,prol
+  gloss: PL|PROL|P.3SG
+ paradigm: Comparative
+
 -paradigm: Noun-case-compounding-pl-soft
  -flex: .ьёс|ыз<.>
   gramm: case_comp,pl_comp,pl,acc
   gloss: PL|ACC
  -flex: .ьёс|ты<.>
   gramm: case_comp,pl_comp,pl,acc
   gloss: PL|ACC.PL
@@ -2039,15 +2129,15 @@
  -flex: .эз<.>
   gramm: acc
   gloss: ACC
   paradigm: Comparative
  -flex: .ыз<.>
   gramm: acc
   gloss: ACC
-  regex-gramm: ^.*pl.*$
+  regex-prev-gramm: ^.*pl.*$
   paradigm: Comparative
  -flex: .ез<.>
   gramm: acc
   gloss: ACC
   regex-prev: ^.*[бвгжӟӝйкмпрфхцчӵшщаеёиӥоӧуыэюя][<>.]*$
   paradigm: Comparative
  -flex: .ты<.>
@@ -2055,52 +2145,59 @@
   gloss: ACC.PL
   regex-prev-gramm: ^.*pl.*$
   paradigm: Comparative
  -flex: .лэн<.>
   gramm: gen
   gloss: GEN
   paradigm: Noun-case-compounding
+  paradigm: Noun-case-compounding-pl-consonant
  -flex: .лэс<.>
   gramm: abl
   gloss: ABL
   paradigm: Noun-case-compounding-soft
+  paradigm: Noun-case-compounding-pl-soft
  -flex: .лэсь<.>
   gramm: abl
   gloss: ABL
   paradigm: Comparative
  -flex: .лы<.>
   gramm: dat
   gloss: DAT
   paradigm: Noun-case-compounding
+  paradigm: Noun-case-compounding-pl-consonant
  -flex: .эн<.>
   gramm: ins
   gloss: INS
   paradigm: Noun-case-compounding
+  paradigm: Noun-case-compounding-pl-consonant
  -flex: .ен<.>
   gramm: ins
   gloss: INS
   regex-prev: ^.*[бвгжӟӝйкмпрфхцчӵшщаеёиӥоӧуыэюя][<>.]*$
   paradigm: Noun-case-compounding
+  paradigm: Noun-case-compounding-pl-consonant
  -flex: .тэк<.>
   gramm: car
   gloss: CAR
   paradigm: Noun-case-compounding
+  paradigm: Noun-case-compounding-pl-consonant
  -flex: .ъя<.>
   gramm: adv
   gloss: ADV
   paradigm: Comparative
  -flex: .я<.>
   gramm: adv
   gloss: ADV
   paradigm: Comparative
   regex-prev: ^.*[ьйаеёиӥоӧуыэюя][<>.]*$
  -flex: .ын<.>
   gramm: loc
   gloss: LOC
   paradigm: Noun-case-compounding
+  paradigm: Noun-case-compounding-pl-consonant
  -flex: .э<.>
   gramm: ill
   gloss: ILL
   paradigm: Comparative
  -flex: .е<.>
   gramm: ill
   gloss: ILL
@@ -2135,23 +2232,26 @@
   gloss: EL
   paradigm: Comparative
   regex-prev: ^.*[бвгжӟӝйкмпрфхцчӵшщаеёиӥоӧуыэюя][<>.]*$
  -flex: .ысен<.>
   gramm: egr
   gloss: EGR
   paradigm: Noun-case-compounding
+  paradigm: Noun-case-compounding-pl-consonant
  -flex: .исен<.>
   gramm: egr,nonst
   gloss: EGR
   paradigm: Noun-case-compounding
+  paradigm: Noun-case-compounding-pl-consonant
   regex-prev: ^.*[бвгжӟӝйкмпрфхцчӵшщаеёиӥоӧуыэюя][<>.]*$
  -flex: .ӥсен<.>
   gramm: egr,nonst
   gloss: EGR
   paradigm: Noun-case-compounding
+  paradigm: Noun-case-compounding-pl-consonant
  -flex: .оз<.>
   gramm: term
   gloss: TERM
   paradigm: Noun-case-compounding-soft
  -flex: .озь<.>
   gramm: term
   gloss: TERM
@@ -2196,22 +2296,24 @@
   gramm: acc
   gloss: ACC
   paradigm: Comparative
  -flex: .ен<.>
   gramm: ins
   gloss: INS
   paradigm: Noun-case-compounding
+  paradigm: Noun-case-compounding-pl-consonant
  -flex: .я<.>
   gramm: adv
   gloss: ADV
   paradigm: Comparative
  -flex: .ын<.>
   gramm: loc
   gloss: LOC
   paradigm: Noun-case-compounding
+  paradigm: Noun-case-compounding-pl-consonant
  -flex: .е<.>
   gramm: ill
   gloss: ILL
   paradigm: Comparative
  -flex: .ыс<.>
   gramm: el
   gloss: EL
@@ -2232,18 +2334,20 @@
   gloss: EL
   paradigm: Comparative
   regex-prev: ^.*[бвгжӟӝйкмпрфхцчӵшщаеёиӥоӧуыэюя][<>.]*$
  -flex: .ысен<.>
   gramm: egr
   gloss: EGR
   paradigm: Noun-case-compounding
+  paradigm: Noun-case-compounding-pl-consonant
  -flex: .исен<.>
   gramm: egr,nonst
   gloss: EGR
   paradigm: Noun-case-compounding
+  paradigm: Noun-case-compounding-pl-consonant
   regex-prev: ^.*[бвгжӟӝйкмпрфхцчӵшщаеёиӥоӧуыэюя][<>.]*$
  -flex: .оз<.>
   gramm: term
   gloss: TERM
   paradigm: Noun-case-compounding-soft
  -flex: .озь<.>
   gramm: term
@@ -2360,21 +2464,21 @@
   gloss: APP
   paradigm: Comparative
 
 -paradigm: Noun-case-mar
  -flex: .е<.>
   gramm: nom
   gloss: NOM
-  regex-lex: ^номыре$
+  regex-lex: ^номыр$
  -flex: .<.>
   gramm: nom
  -flex: .е<.>//.э<.>
   gramm: acc
   gloss: ACC
-  regex-lex: ^.*(мар?|кин|со|та|номыре)$
+  regex-lex: ^.*(мар?|кин|со|та|номыр|огмыр)$
  -flex: .ты<.>
   gramm: acc
   gloss: ACC.PL
   regex-gramm: ^.*pl.*$
  -flex: .лэн<.>
   gramm: gen
   gloss: GEN
@@ -2440,42 +2544,48 @@
   gloss: ACC.PL
   regex-gramm: ^.*pl.*$
   paradigm: Comparative
  -flex: .лэн<.>
   gramm: gen
   gloss: GEN
   paradigm: Noun-case-compounding
+  paradigm: Noun-case-compounding-pl-consonant
  -flex: .лэс<.>
   gramm: abl
   gloss: ABL
   paradigm: Noun-case-compounding-soft
+  paradigm: Noun-case-compounding-pl-soft
  -flex: .лэсь<.>
   gramm: abl
   gloss: ABL
   paradigm: Comparative
  -flex: .лы<.>
   gramm: dat
   gloss: DAT
   paradigm: Noun-case-compounding
+  paradigm: Noun-case-compounding-pl-consonant
  -flex: .эн<.>//.ын<.>
   gramm: ins
   gloss: INS
   paradigm: Noun-case-compounding
+  paradigm: Noun-case-compounding-pl-consonant
  -flex: .тэк<.>
   gramm: car
   gloss: CAR
   paradigm: Noun-case-compounding
+  paradigm: Noun-case-compounding-pl-consonant
  -flex: .ъя<.>
   gramm: adv
   gloss: ADV
   paradigm: Comparative
  -flex: .ан<.>
   gramm: loc
   gloss: LOC
   paradigm: Noun-case-compounding
+  paradigm: Noun-case-compounding-pl-consonant
  -flex: .а<.>
   gramm: ill
   gloss: ILL
   paradigm: Comparative
  -flex: .ас<.>//.ыс<.>
   gramm: el
   gloss: EL
@@ -2485,14 +2595,15 @@
   gramm: el
   gloss: EL
   paradigm: Comparative
  -flex: .асен<.>//.ысен<.>
   gramm: egr
   gloss: EGR
   paradigm: Noun-case-compounding
+  paradigm: Noun-case-compounding-pl-consonant
  -flex: .оз<.>
   gramm: term
   gloss: TERM
   paradigm: Noun-case-compounding-soft
  -flex: .озь<.>
   gramm: term
   gloss: TERM
```

### Comparing `uniparser-udmurt-2.1.8/uniparser_udmurt/data_strict/udmurt_disambiguation.cg3` & `uniparser-udmurt-2.1.9/uniparser_udmurt/data_strict/udmurt_disambiguation.cg3`

 * *Files identical despite different names*

### Comparing `uniparser-udmurt-2.1.8/uniparser_udmurt.egg-info/PKG-INFO` & `uniparser-udmurt-2.1.9/uniparser_udmurt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uniparser-udmurt
-Version: 2.1.8
+Version: 2.1.9
 Summary: Rule-based morphological analysis for Udmurt
 Home-page: https://github.com/timarkh/uniparser-grammar-udm
 Author: Timofey Arkhangelskiy
 Author-email: timarkh@gmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/timarkh/uniparser-grammar-udm/issues
 Platform: UNKNOWN
```

### Comparing `uniparser-udmurt-2.1.8/uniparser_udmurt.egg-info/SOURCES.txt` & `uniparser-udmurt-2.1.9/uniparser_udmurt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

