# Comparing `tmp/phone_gen-2.3.2.tar.gz` & `tmp/phone_gen-2.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phone_gen-2.3.2.tar", last modified: Wed Jun 14 08:07:48 2023, max compression
+gzip compressed data, was "phone_gen-2.3.3.tar", last modified: Fri Jun 23 09:12:11 2023, max compression
```

## Comparing `phone_gen-2.3.2.tar` & `phone_gen-2.3.3.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:07:48.430148 phone_gen-2.3.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:07:48.426148 phone_gen-2.3.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:07:48.430148 phone_gen-2.3.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-14 08:07:37.000000 phone_gen-2.3.2/.github/workflows/python-package.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-06-14 08:07:37.000000 phone_gen-2.3.2/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-06-14 08:07:37.000000 phone_gen-2.3.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-14 08:07:37.000000 phone_gen-2.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4727 2023-06-14 08:07:48.430148 phone_gen-2.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-06-14 08:07:37.000000 phone_gen-2.3.2/Pipfile
--rw-r--r--   0 runner    (1001) docker     (123)     3612 2023-06-14 08:07:37.000000 phone_gen-2.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:07:48.430148 phone_gen-2.3.2/dev_tools/
--rw-r--r--   0 runner    (1001) docker     (123)     4859 2023-06-14 08:07:37.000000 phone_gen-2.3.2/dev_tools/patterns_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3871 2023-06-14 08:07:37.000000 phone_gen-2.3.2/dev_tools/update.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:07:48.430148 phone_gen-2.3.2/phone_gen/
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-06-14 08:07:37.000000 phone_gen-2.3.2/phone_gen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-14 08:07:48.000000 phone_gen-2.3.2/phone_gen/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10398 2023-06-14 08:07:37.000000 phone_gen-2.3.2/phone_gen/_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-06-14 08:07:37.000000 phone_gen-2.3.2/phone_gen/alt_patterns.py
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-06-14 08:07:37.000000 phone_gen-2.3.2/phone_gen/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    16602 2023-06-14 08:07:37.000000 phone_gen-2.3.2/phone_gen/country_name.py
--rw-r--r--   0 runner    (1001) docker     (123)     6932 2023-06-14 08:07:37.000000 phone_gen-2.3.2/phone_gen/iso3.py
--rw-r--r--   0 runner    (1001) docker     (123)    87928 2023-06-14 08:07:37.000000 phone_gen-2.3.2/phone_gen/patterns.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:07:48.430148 phone_gen-2.3.2/phone_gen.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4727 2023-06-14 08:07:48.000000 phone_gen-2.3.2/phone_gen.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-06-14 08:07:48.000000 phone_gen-2.3.2/phone_gen.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 08:07:48.000000 phone_gen-2.3.2/phone_gen.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-14 08:07:48.000000 phone_gen-2.3.2/phone_gen.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-14 08:07:48.000000 phone_gen-2.3.2/phone_gen.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-14 08:07:48.430148 phone_gen-2.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-06-14 08:07:37.000000 phone_gen-2.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:07:48.430148 phone_gen-2.3.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-14 08:07:37.000000 phone_gen-2.3.2/tests/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-06-14 08:07:37.000000 phone_gen-2.3.2/tests/test_alt_pattern.py
--rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-06-14 08:07:37.000000 phone_gen-2.3.2/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-06-14 08:07:37.000000 phone_gen-2.3.2/tests/test_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-06-14 08:07:37.000000 phone_gen-2.3.2/tests/test_load_alt_patterns.py
--rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-06-14 08:07:37.000000 phone_gen-2.3.2/tests/test_phone.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:12:11.199633 phone_gen-2.3.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:12:11.195633 phone_gen-2.3.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:12:11.195633 phone_gen-2.3.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-23 09:11:55.000000 phone_gen-2.3.3/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-06-23 09:11:55.000000 phone_gen-2.3.3/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-06-23 09:11:55.000000 phone_gen-2.3.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-23 09:11:55.000000 phone_gen-2.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4727 2023-06-23 09:12:11.199633 phone_gen-2.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-06-23 09:11:55.000000 phone_gen-2.3.3/Pipfile
+-rw-r--r--   0 runner    (1001) docker     (123)     3612 2023-06-23 09:11:55.000000 phone_gen-2.3.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:12:11.199633 phone_gen-2.3.3/dev_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)     4859 2023-06-23 09:11:55.000000 phone_gen-2.3.3/dev_tools/patterns_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3871 2023-06-23 09:11:55.000000 phone_gen-2.3.3/dev_tools/update.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:12:11.199633 phone_gen-2.3.3/phone_gen/
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-06-23 09:11:55.000000 phone_gen-2.3.3/phone_gen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-23 09:12:11.000000 phone_gen-2.3.3/phone_gen/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10398 2023-06-23 09:11:55.000000 phone_gen-2.3.3/phone_gen/_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-06-23 09:11:55.000000 phone_gen-2.3.3/phone_gen/alt_patterns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-06-23 09:11:55.000000 phone_gen-2.3.3/phone_gen/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16602 2023-06-23 09:11:55.000000 phone_gen-2.3.3/phone_gen/country_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6932 2023-06-23 09:11:55.000000 phone_gen-2.3.3/phone_gen/iso3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    87966 2023-06-23 09:11:55.000000 phone_gen-2.3.3/phone_gen/patterns.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:12:11.199633 phone_gen-2.3.3/phone_gen.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4727 2023-06-23 09:12:11.000000 phone_gen-2.3.3/phone_gen.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-06-23 09:12:11.000000 phone_gen-2.3.3/phone_gen.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 09:12:11.000000 phone_gen-2.3.3/phone_gen.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-23 09:12:11.000000 phone_gen-2.3.3/phone_gen.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-23 09:12:11.000000 phone_gen-2.3.3/phone_gen.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-23 09:12:11.203633 phone_gen-2.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-06-23 09:11:55.000000 phone_gen-2.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:12:11.199633 phone_gen-2.3.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-23 09:11:55.000000 phone_gen-2.3.3/tests/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-06-23 09:11:55.000000 phone_gen-2.3.3/tests/test_alt_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-06-23 09:11:55.000000 phone_gen-2.3.3/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-06-23 09:11:55.000000 phone_gen-2.3.3/tests/test_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-06-23 09:11:55.000000 phone_gen-2.3.3/tests/test_load_alt_patterns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-06-23 09:11:55.000000 phone_gen-2.3.3/tests/test_phone.py
```

### Comparing `phone_gen-2.3.2/.github/workflows/python-package.yml` & `phone_gen-2.3.3/.github/workflows/python-package.yml`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v2
         with:
           python-version: ${{ matrix.python-version }}
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
-          python -m pip install flake8 pep8-naming pytest black pytest-cov phonenumbers==8.13.14
+          python -m pip install flake8 pep8-naming pytest black pytest-cov phonenumbers==8.13.15
           python -m pip install -e .
       - name: Flake8
         run: |
           flake8 phone_gen
       - name: Black
         run: |
           black --check phone_gen
```

### Comparing `phone_gen-2.3.2/.github/workflows/python-publish.yml` & `phone_gen-2.3.3/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `phone_gen-2.3.2/.gitignore` & `phone_gen-2.3.3/.gitignore`

 * *Files identical despite different names*

### Comparing `phone_gen-2.3.2/LICENSE` & `phone_gen-2.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `phone_gen-2.3.2/PKG-INFO` & `phone_gen-2.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phone_gen
-Version: 2.3.2
+Version: 2.3.3
 Summary: International phone number generation
 Home-page: https://github.com/tolstislon/phone-gen
 Author: tolstislon
 Author-email: tolstislon@gmail.com
 License: MIT License
 Keywords: testing,test-data,phone-number,phone,test-data-generator
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `phone_gen-2.3.2/README.md` & `phone_gen-2.3.3/README.md`

 * *Files identical despite different names*

### Comparing `phone_gen-2.3.2/dev_tools/patterns_generator.py` & `phone_gen-2.3.3/dev_tools/patterns_generator.py`

 * *Files identical despite different names*

### Comparing `phone_gen-2.3.2/dev_tools/update.py` & `phone_gen-2.3.3/dev_tools/update.py`

 * *Files identical despite different names*

### Comparing `phone_gen-2.3.2/phone_gen/__init__.py` & `phone_gen-2.3.3/phone_gen/__init__.py`

 * *Files identical despite different names*

### Comparing `phone_gen-2.3.2/phone_gen/_generator.py` & `phone_gen-2.3.3/phone_gen/_generator.py`

 * *Files identical despite different names*

### Comparing `phone_gen-2.3.2/phone_gen/alt_patterns.py` & `phone_gen-2.3.3/phone_gen/alt_patterns.py`

 * *Files identical despite different names*

### Comparing `phone_gen-2.3.2/phone_gen/cli.py` & `phone_gen-2.3.3/phone_gen/cli.py`

 * *Files identical despite different names*

### Comparing `phone_gen-2.3.2/phone_gen/country_name.py` & `phone_gen-2.3.3/phone_gen/country_name.py`

 * *Files identical despite different names*

### Comparing `phone_gen-2.3.2/phone_gen/iso3.py` & `phone_gen-2.3.3/phone_gen/iso3.py`

 * *Files identical despite different names*

### Comparing `phone_gen-2.3.2/phone_gen/patterns.py` & `phone_gen-2.3.3/phone_gen/patterns.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # -*- coding: utf-8 -*-
 """
-Auto-generated file 2023-06-14 08:01:41 UTC
-Resource: https://github.com/google/libphonenumber v8.13.14
+Auto-generated file 2023-06-23 09:05:07 UTC
+Resource: https://github.com/google/libphonenumber v8.13.15
 """
 
 
 PATTERNS = {
-    "info": "libphonenumber v8.13.14",
+    "info": "libphonenumber v8.13.15",
     "data": {
         "AC": {
             "code": "247",
             "pattern": "((6[2-467][\\d]{3}))",
             "mobile": "((4[\\d]{4}))",
         },
         "AD": {
@@ -107,15 +107,15 @@
             "code": "32",
             "pattern": "((80[2-8][\\d]{5})|((1[0-69])|([23][2-8])|(4[23])|(5[\\d])|(6[013-57-9])|(71)|(8[1-79])|(9[2-4])[\\d]{6}))",
             "mobile": "((4[5-9][\\d]{7}))",
         },
         "BF": {
             "code": "226",
             "pattern": "((2(0(49)|(5[23])|(6[5-7])|(9[016-9]))|(4(4[569])|(5[4-6])|(6[5-7])|(7[0179]))|(5([34][\\d])|(50)|(6[5-7]))[\\d]{4}))",
-            "mobile": "(((0[1-35-7])|(5[1-8])|([67][\\d])[\\d]{6}))",
+            "mobile": "(((0[1-35-7])|(5[0-8])|([67][\\d])[\\d]{6}))",
         },
         "BG": {
             "code": "359",
             "pattern": "((2[\\d]{5:7})|((43[1-6])|(70[1-9])[\\d]{4:5})|(([36][\\d])|(4[124-7])|([57][1-9])|(8[1-6])|(9[1-7])[\\d]{5:6}))",
             "mobile": "(((43[07-9])|(99[69][\\d])[\\d]{5})|((8[7-9])|(98)[\\d]{7}))",
         },
         "BH": {
@@ -502,15 +502,15 @@
             "code": "353",
             "pattern": "(((1[\\d])|(21)[\\d]{6:7})|((2[24-9])|(4(0[24])|(5[\\d])|(7))|(5(0[45])|(1[\\d])|(8))|(6(1[\\d])|([237-9]))|(9(1[\\d])|([35-9]))[\\d]{5})|((23)|(4([1-469])|(8[\\d]))|(5[23679])|(6[4-6])|(7[14])|(9[04])[\\d]{7}))",
             "mobile": "((8(22)|([35-9][\\d])[\\d]{6}))",
         },
         "IL": {
             "code": "972",
             "pattern": "((153[\\d]{8:9})|(29[1-9][\\d]{5})|((2[0-8])|([3489][\\d])[\\d]{6}))",
-            "mobile": "((5(([02368][\\d])|([19][2-9])|(4[1-9])[\\d])|(5(01)|(1[79])|(2[2-9])|(3[0-3])|(4[34])|(5[015689])|(6[6-8])|(7[0-267])|(8[7-9])|(9[1-9]))[\\d]{5}))",
+            "mobile": "((55410[\\d]{4})|(5(([02368][\\d])|([19][2-9])|(4[1-9])[\\d])|(5(01)|(1[79])|(2[2-9])|(3[0-3])|(4[34])|(5[015689])|(6[6-8])|(7[0-267])|(8[7-9])|(9[1-9]))[\\d]{5}))",
         },
         "IM": {
             "code": "44",
             "pattern": "((1624(230)|([5-8][\\d][\\d])[\\d]{3}))",
             "mobile": "((76245[06][\\d]{4})|(7(4576)|([59]24[\\d])|(624[0-4689])[\\d]{5}))",
         },
         "IN": {
@@ -713,15 +713,15 @@
         "MM": {
             "code": "95",
             "pattern": "(((1((2[\\d])|(3[56])|([89][0-6])[\\d])|(4(2[29])|(62)|(7[0-2])|(83))|(6))|(2(2(00)|(8[34]))|(4(0[\\d])|([26]2)|(7[0-2])|(83))|(51[\\d][\\d]))|(4(2(2[\\d][\\d])|(48[013]))|(3(20[\\d])|(4(70)|(83))|(56))|(420[\\d])|(5470))|(6(0([23])|(88[\\d]))|((124)|([56]2[\\d])[\\d])|(2472)|(3(20[\\d])|(470))|(4(2[04][\\d])|(472))|(7((3[\\d])|(8[01459])[\\d])|(4[67]0)))[\\d]{4})|(5(2(2[\\d]{5:6})|(47[02][\\d]{4}))|((3472)|(4(2(1)|(86))|(470))|(522[\\d])|(6(20[\\d])|(483))|(7(20[\\d])|(48[01]))|(8(20[\\d])|(47[02]))|(9(20[\\d])|(470))[\\d]{4}))|(7((0470)|(4(25[\\d])|(470))|(5(202)|(470)|(96[\\d]))[\\d]{4})|(1(20[\\d]{4:5})|(4(70)|(83)[\\d]{4})))|(8(1(2[\\d]{5:6})|(4(10)|(7[01][\\d])[\\d]{3}))|(2(2[\\d]{5:6})|((320)|(490[\\d])[\\d]{3}))|((3(2[\\d][\\d])|(470))|(4[24-7])|(5((2[\\d])|(51)[\\d])|(4([1-35-9][\\d])|(4[0-57-9])))|(6[23])[\\d]{4}))|((1[2-6][\\d])|(4(2[24-8])|(3[2-7])|([46][2-6])|(5[3-5]))|(5([27][2-8])|(3[2-68])|(4[24-8])|(5[23])|(6[2-4])|(8[24-7])|(9[2-7]))|(6([19]20)|(42[03-6])|((52)|(7[45])[\\d]))|(7([04][24-8])|([15][2-7])|(22)|(3[2-4]))|(8(1[2-689])|(2[2-8])|([35]2[\\d]))[\\d]{4})|(25[\\d]{5:6})|((2[2-9])|(6(1[2356])|([24][2-6])|(3[24-6])|(5[2-4])|(6[2-8])|(7[235-7])|(8[245])|(9[24]))|(8(3[24])|(5[245]))[\\d]{4}))",
             "mobile": "(((17[01])|(9(2([0-4])|([56][\\d][\\d]))|((3([0-36])|(4[\\d]))|((6[\\d])|(8[89])|(9[4-8])[\\d])|(7(3)|(40)|([5-9][\\d]))[\\d])|(4(([0245][\\d])|([1379])[\\d])|(88))|(5[0-6])[\\d])[\\d]{4})|(9[69]1[\\d]{6})|(9([68][\\d])|(9[089])[\\d]{5}))",
         },
         "MN": {
             "code": "976",
-            "pattern": "(([12]2[1-3][\\d]{5:6})|(7(0[0-5][\\d])|(128)[\\d]{4})|(([12](1)|(27))|(5[368])[\\d]{6})|([12](3[2-8])|(4[2-68])|(5[1-4689])[\\d]{6:7}))",
+            "pattern": "(([12]2[1-3][\\d]{5:6})|((([12](1)|(27))|(5[368])[\\d][\\d])|(7(0([0-5][\\d])|(7[078])|(80))|(128))[\\d]{4})|([12](3[2-8])|(4[2-68])|(5[1-4689])[\\d]{6:7}))",
             "mobile": "(((83[01])|(92[039])[\\d]{5})|((5[05])|(6[069])|(8[015689])|(9[013-9])[\\d]{6}))",
         },
         "MO": {
             "code": "853",
             "pattern": "(((28[2-9])|(8(11)|([2-57-9][\\d]))[\\d]{5}))",
             "mobile": "((6800[0-79][\\d]{3})|(6([235][\\d][\\d])|(6(0[0-5])|([1-9][\\d]))|(8(0[1-9])|([14-8][\\d])|(2[5-9])|([39][0-4]))[\\d]{4}))",
         },
@@ -789,15 +789,15 @@
             "code": "687",
             "pattern": "(((2[03-9])|(3[0-5])|(4[1-7])|(88)[\\d]{4}))",
             "mobile": "(((5[0-4])|([79][\\d])|(8[0-79])[\\d]{4}))",
         },
         "NE": {
             "code": "227",
             "pattern": "((2(0(20)|(3[1-8])|(4[13-5])|(5[14])|(6[14578])|(7[1-578]))|(1(4[145])|(5[14])|(6[14-68])|(7[169])|(88))[\\d]{4}))",
-            "mobile": "(((23)|(7[04])|([89][\\d])[\\d]{6}))",
+            "mobile": "(((23)|(7[047])|([89][\\d])[\\d]{6}))",
         },
         "NF": {
             "code": "672",
             "pattern": "(((1(06)|(17)|(28)|(39))|(3[0-2][\\d])[\\d]{3}))",
             "mobile": "(((14)|(3[58])[\\d]{4}))",
         },
         "NG": {
@@ -839,15 +839,15 @@
             "code": "64",
             "pattern": "((24099[\\d]{3})|((3[2-79])|([49][2-9])|(6[235-9])|(7[2-57-9])[\\d]{6}))",
             "mobile": "((2[0-27-9][\\d]{7:8})|(2(1[\\d])|(75)[\\d]{5}))",
         },
         "OM": {
             "code": "968",
             "pattern": "((2[1-6][\\d]{6}))",
-            "mobile": "((1505[\\d]{4})|((7([1289][\\d])|(7[0-5]))|(9(0[1-9])|([1-9][\\d]))[\\d]{5}))",
+            "mobile": "((1505[\\d]{4})|((7([1289][\\d])|(69)|(7[0-5]))|(9(0[1-9])|([1-9][\\d]))[\\d]{5}))",
         },
         "PA": {
             "code": "507",
             "pattern": "(((1(0[\\d])|(1[479])|(2[37])|(3[0137])|(4[17])|(5[05])|(6[58])|(7[0167])|(8[2358])|(9[1389]))|(2([0235-79][\\d])|(1[0-7])|(4[013-9])|(8[02-9]))|(3([089][\\d])|(1[0-7])|(2[0-5])|(33)|(4[0-79])|(5[0-35])|(6[068])|(7[0-8]))|(4(00)|(3[0-579])|(4[\\d])|(7[0-57-9]))|(5([01][\\d])|(2[0-7])|([56]0)|(79))|(7(0[09])|(2[0-26-8])|(3[03])|(4[04])|(5[05-9])|(6[056])|(7[0-24-9])|(8[5-9])|(90))|(8(09)|(2[89])|(3[\\d])|(4[0-24-689])|(5[014])|(8[02]))|(9(0[5-9])|(1[0135-8])|(2[036-9])|(3[35-79])|(40)|(5[0457-9])|(6[05-9])|(7[04-9])|(8[35-8])|(9[\\d]))[\\d]{4}))",
             "mobile": "(((1[16]1)|(21[89])|(6[\\d]{3})|(8(1[01])|(7[23]))[\\d]{4}))",
         },
         "PE": {
@@ -1004,15 +1004,15 @@
             "code": "221",
             "pattern": "((3(0(1[0-2])|(80))|(282)|(3(8[1-9])|(9[3-9]))|(611)[\\d]{5}))",
             "mobile": "((7(([06-8][\\d])|(21)|(90)[\\d])|(5(01)|([19]0)|(25)|([38]3)|([4-7][\\d]))[\\d]{5}))",
         },
         "SO": {
             "code": "252",
             "pattern": "(((1[\\d])|(2[0-79])|(3[0-46-8])|(4[0-7])|(5[57-9])[\\d]{5})|(([134][\\d])|(8[125])[\\d]{4}))",
-            "mobile": "((((15)|((3[59])|(4[89])|(79)|(8[08])[\\d])|(6(0[5-7])|([1-9][\\d]))|(9(0[\\d])|([2-9]))[\\d])|(2(4[\\d])|(8))[\\d]{5})|(([67][\\d][\\d])|(904)[\\d]{5}))",
+            "mobile": "((((15)|((3[59])|(4[89])|(6[\\d])|(79)|(8[08])[\\d])|(9(0[\\d])|([2-9]))[\\d])|(2(4[\\d])|(8))[\\d]{5})|(([67][\\d][\\d])|(904)[\\d]{5}))",
         },
         "SR": {
             "code": "597",
             "pattern": "(((2[1-3])|(3[0-7])|((4)|(68)[\\d])|(5[2-58])[\\d]{4}))",
             "mobile": "(((7[124-7])|(8[124-9])[\\d]{5}))",
         },
         "SS": {
@@ -1023,15 +1023,15 @@
         "ST": {
             "code": "239",
             "pattern": "((22[\\d]{5}))",
             "mobile": "((900[5-9][\\d]{3})|(9(0[1-9])|([89][\\d])[\\d]{4}))",
         },
         "SV": {
             "code": "503",
-            "pattern": "((2([1-6][\\d]{3})|([79]90[034])|(890[0245])[\\d]{3}))",
+            "pattern": "((2(([1-6][\\d][\\d])|(990)[\\d])|(790[034])|(890[0245])[\\d]{3}))",
             "mobile": "((66([02-9][\\d][\\d])|(1([02-9][\\d])|(16))[\\d]{3})|((6[0-57-9])|(7[\\d])[\\d]{6}))",
         },
         "SX": {
             "code": "1",
             "pattern": "((7215(4[2-8])|(8[239])|(9[056])[\\d]{4}))",
             "mobile": "((7215(1[02])|(2[\\d])|(5[034679])|(8[014-8])[\\d]{4}))",
         },
```

### Comparing `phone_gen-2.3.2/phone_gen.egg-info/PKG-INFO` & `phone_gen-2.3.3/phone_gen.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phone-gen
-Version: 2.3.2
+Version: 2.3.3
 Summary: International phone number generation
 Home-page: https://github.com/tolstislon/phone-gen
 Author: tolstislon
 Author-email: tolstislon@gmail.com
 License: MIT License
 Keywords: testing,test-data,phone-number,phone,test-data-generator
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `phone_gen-2.3.2/phone_gen.egg-info/SOURCES.txt` & `phone_gen-2.3.3/phone_gen.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `phone_gen-2.3.2/setup.py` & `phone_gen-2.3.3/setup.py`

 * *Files identical despite different names*

### Comparing `phone_gen-2.3.2/tests/test_alt_pattern.py` & `phone_gen-2.3.3/tests/test_alt_pattern.py`

 * *Files identical despite different names*

### Comparing `phone_gen-2.3.2/tests/test_cli.py` & `phone_gen-2.3.3/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `phone_gen-2.3.2/tests/test_generator.py` & `phone_gen-2.3.3/tests/test_generator.py`

 * *Files identical despite different names*

### Comparing `phone_gen-2.3.2/tests/test_load_alt_patterns.py` & `phone_gen-2.3.3/tests/test_load_alt_patterns.py`

 * *Files identical despite different names*

### Comparing `phone_gen-2.3.2/tests/test_phone.py` & `phone_gen-2.3.3/tests/test_phone.py`

 * *Files identical despite different names*

