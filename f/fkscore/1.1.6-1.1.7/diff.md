# Comparing `tmp/fkscore-1.1.6.tar.gz` & `tmp/fkscore-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/fkscore-1.1.6.tar", last modified: Sun Apr 14 16:32:10 2019, max compression
+gzip compressed data, was "fkscore-1.1.7.tar", last modified: Fri Jun 23 21:13:59 2023, max compression
```

## Comparing `fkscore-1.1.6.tar` & `fkscore-1.1.7.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxr-xr-x   0 randallshane   (501) staff       (20)        0 2019-04-14 16:32:10.000000 fkscore-1.1.6/
--rw-r--r--   0 randallshane   (501) staff       (20)     3015 2019-04-14 16:32:10.000000 fkscore-1.1.6/PKG-INFO
--rw-r--r--   0 randallshane   (501) staff       (20)     1642 2019-04-14 16:31:19.000000 fkscore-1.1.6/README.md
-drwxr-xr-x   0 randallshane   (501) staff       (20)        0 2019-04-14 16:32:10.000000 fkscore-1.1.6/fkscore/
--rw-r--r--   0 randallshane   (501) staff       (20)       76 2019-01-26 02:25:42.000000 fkscore-1.1.6/fkscore/__init__.py
--rw-r--r--   0 randallshane   (501) staff       (20)     3832 2019-04-14 15:51:15.000000 fkscore-1.1.6/fkscore/fkscore.py
-drwxr-xr-x   0 randallshane   (501) staff       (20)        0 2019-04-14 16:32:10.000000 fkscore-1.1.6/fkscore.egg-info/
--rw-r--r--   0 randallshane   (501) staff       (20)     3015 2019-04-14 16:32:10.000000 fkscore-1.1.6/fkscore.egg-info/PKG-INFO
--rw-r--r--   0 randallshane   (501) staff       (20)      181 2019-04-14 16:32:10.000000 fkscore-1.1.6/fkscore.egg-info/SOURCES.txt
--rw-r--r--   0 randallshane   (501) staff       (20)        1 2019-04-14 16:32:10.000000 fkscore-1.1.6/fkscore.egg-info/dependency_links.txt
--rw-r--r--   0 randallshane   (501) staff       (20)        8 2019-04-14 16:32:10.000000 fkscore-1.1.6/fkscore.egg-info/top_level.txt
--rw-r--r--   0 randallshane   (501) staff       (20)       38 2019-04-14 16:32:10.000000 fkscore-1.1.6/setup.cfg
--rw-r--r--   0 randallshane   (501) staff       (20)     1617 2019-04-14 16:31:31.000000 fkscore-1.1.6/setup.py
+drwxr-xr-x   0 randall    (501) staff       (20)        0 2023-06-23 21:13:59.998543 fkscore-1.1.7/
+-rw-r--r--   0 randall    (501) staff       (20)     1075 2023-06-23 20:54:49.000000 fkscore-1.1.7/LICENSE
+-rw-r--r--   0 randall    (501) staff       (20)     2671 2023-06-23 21:13:59.998439 fkscore-1.1.7/PKG-INFO
+-rw-r--r--   0 randall    (501) staff       (20)     1634 2023-06-23 21:07:16.000000 fkscore-1.1.7/README.md
+drwxr-xr-x   0 randall    (501) staff       (20)        0 2023-06-23 21:13:59.997694 fkscore-1.1.7/fkscore/
+-rw-r--r--   0 randall    (501) staff       (20)       76 2023-06-23 20:54:49.000000 fkscore-1.1.7/fkscore/__init__.py
+-rw-r--r--   0 randall    (501) staff       (20)     3894 2023-06-23 21:11:20.000000 fkscore-1.1.7/fkscore/fkscore.py
+drwxr-xr-x   0 randall    (501) staff       (20)        0 2023-06-23 21:13:59.998253 fkscore-1.1.7/fkscore.egg-info/
+-rw-r--r--   0 randall    (501) staff       (20)     2671 2023-06-23 21:13:59.000000 fkscore-1.1.7/fkscore.egg-info/PKG-INFO
+-rw-r--r--   0 randall    (501) staff       (20)      189 2023-06-23 21:13:59.000000 fkscore-1.1.7/fkscore.egg-info/SOURCES.txt
+-rw-r--r--   0 randall    (501) staff       (20)        1 2023-06-23 21:13:59.000000 fkscore-1.1.7/fkscore.egg-info/dependency_links.txt
+-rw-r--r--   0 randall    (501) staff       (20)        8 2023-06-23 21:13:59.000000 fkscore-1.1.7/fkscore.egg-info/top_level.txt
+-rw-r--r--   0 randall    (501) staff       (20)       38 2023-06-23 21:13:59.998581 fkscore-1.1.7/setup.cfg
+-rw-r--r--   0 randall    (501) staff       (20)     1698 2023-06-23 21:07:10.000000 fkscore-1.1.7/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `fkscore-1.1.6/PKG-INFO` & `fkscore-1.1.7/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,77 +1,82 @@
 Metadata-Version: 2.1
 Name: fkscore
-Version: 1.1.6
+Version: 1.1.7
 Summary: Flesch Kincaid readability scoring algorithm
 Home-page: https://github.com/RandallShanePhD/fkscore
-Author: Randall Shane, PhD <Randall.Shane@CodeIntelligence.IO>
-Author-email: Randall.Shane@CodeIntelligence.IO
+Author: Randall Shane PhD <Randall@NumbersAndTech.com>
+Author-email: Randall@NumbersAndTech.com
 License: MIT
-Description: fkscore
-        ====
-        
-        Flesch Kincaid readability score for text
-        
-        A Python module implementation of the Flesch Kincaid readability score algorithm.
-        
-        The source code is released under the MIT License.
-        
-        ### Installation ###
-            pip3 install fkscore
-        
-        ### Usage ###
-        For text in python represented as a string.
-        
-        Takes text as string datatype.  Words can be on same or different lines.  Current version is English language only.  Email for support.
-        
-            import fkscore
-            text = '...blah blah blah...'
-            f = fkscore.fkscore(text)
-            print(f.stats)
-            print(f.score)
-        
-            OR
-        
-            from fkscore import fkscore
-            text = '...blah blah blah...'
-            f = fkscore(text)
-            print(f.stats)
-            print(f.score)
-        
-        ### Output ###
-        Output includes 2 dictionaries of information as follows:
-        * stats:
-          * stats['num_words']
-          * stats['num_syllables']
-          * stats['num_sentences']
-        * score:
-          * score['readability']  # Calculated F-K Readability Score
-          * score['grade']        # Permuted F-K Grade Reading Level
-        
-        ### Releases ###
-        Releases and additions will push to PyPi periodically, but if there is a feature in master not built/pushed and you want it to be, just ping me.
-        
-        ### History ###
-        This is a maintained as an implementation of the Flesch-Kincaid readability algorithm which was initially developed in 1948 by Rudolph Flesch and later revised by the U.S. Navy in 1975.  This module is pure python and works with 3.5+.
-        
-        ### Questions ###
-        Feel free to ping for questions, comments, concerns or interact directly via the GitHub repository.
-        
-        Randall Shane, PhD<br />
-        Randall.Shane@CodeIntelligence.IO<br />
-        https://github.com/RandallShanePhD/fkscore<br />
-        Thank you!
-        
 Keywords: nlp,linguistics,nltk,text processing
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Text Processing :: Linguistic
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Text Processing :: Indexing
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+fkscore
+====
+
+Flesch Kincaid readability score for text
+
+A Python module implementation of the Flesch Kincaid readability score algorithm.
+
+The source code is released under the MIT License.
+
+### Installation ###
+    pip3 install fkscore
+
+### Usage ###
+For text in python represented as a string.
+
+Takes text as string datatype.  Words can be on same or different lines.  Current version is English language only.  Email for support.
+
+    import fkscore
+    text = '...blah blah blah...'
+    f = fkscore.fkscore(text)
+    print(f.stats)
+    print(f.score)
+
+    OR
+
+    from fkscore import fkscore
+    text = '...blah blah blah...'
+    f = fkscore(text)
+    print(f.stats)
+    print(f.score)
+
+### Output ###
+Output includes 2 dictionaries of information as follows:
+* stats:
+  * stats['num_words']
+  * stats['num_syllables']
+  * stats['num_sentences']
+* score:
+  * score['readability']  # Calculated F-K Readability Score
+  * score['grade']        # Permuted F-K Grade Reading Level
+
+### Releases ###
+Releases and additions will push to PyPi periodically, but if there is a feature in master not built/pushed and you want it to be, just ping me.
+
+### History ###
+This is a maintained as an implementation of the Flesch-Kincaid readability algorithm which was initially developed in 1948 by Rudolph Flesch and later revised by the U.S. Navy in 1975.  This module is pure python and works with 3.5+.
+
+### Questions ###
+Feel free to ping for questions, comments, concerns or interact directly via the GitHub repository.
+
+Randall Shane PhD<br />
+Randall@NumbersAndTech.com<br />
+https://github.com/RandallShanePhD/fkscore<br />
+Thank you!
+
+
```

### Comparing `fkscore-1.1.6/README.md` & `fkscore-1.1.7/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -44,11 +44,11 @@
 
 ### History ###
 This is a maintained as an implementation of the Flesch-Kincaid readability algorithm which was initially developed in 1948 by Rudolph Flesch and later revised by the U.S. Navy in 1975.  This module is pure python and works with 3.5+.
 
 ### Questions ###
 Feel free to ping for questions, comments, concerns or interact directly via the GitHub repository.
 
-Randall Shane, PhD<br />
-Randall.Shane@CodeIntelligence.IO<br />
+Randall Shane PhD<br />
+Randall@NumbersAndTech.com<br />
 https://github.com/RandallShanePhD/fkscore<br />
 Thank you!
```

### Comparing `fkscore-1.1.6/fkscore/fkscore.py` & `fkscore-1.1.7/fkscore/fkscore.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,18 +3,21 @@
 import re
 import string
 
 
 class fkscore():
     ''' Flesch Kincaid Readability Score
     test = "The quick red fox jumped over the lazy brown dog."
-    sentences = 1
-    words = 10
-    syllables = 12
-    score =
+    stats:
+     sentences = 1
+     words = 10
+     syllables = 12
+    score
+     readability' = 86.705
+     grade = 6th Grade
     '''
 
     def __init__(self, text):
         '''
         Input: UTF-8 text as str
 
         Output (stats):
```

### Comparing `fkscore-1.1.6/fkscore.egg-info/PKG-INFO` & `fkscore-1.1.7/fkscore.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,77 +1,82 @@
 Metadata-Version: 2.1
 Name: fkscore
-Version: 1.1.6
+Version: 1.1.7
 Summary: Flesch Kincaid readability scoring algorithm
 Home-page: https://github.com/RandallShanePhD/fkscore
-Author: Randall Shane, PhD <Randall.Shane@CodeIntelligence.IO>
-Author-email: Randall.Shane@CodeIntelligence.IO
+Author: Randall Shane PhD <Randall@NumbersAndTech.com>
+Author-email: Randall@NumbersAndTech.com
 License: MIT
-Description: fkscore
-        ====
-        
-        Flesch Kincaid readability score for text
-        
-        A Python module implementation of the Flesch Kincaid readability score algorithm.
-        
-        The source code is released under the MIT License.
-        
-        ### Installation ###
-            pip3 install fkscore
-        
-        ### Usage ###
-        For text in python represented as a string.
-        
-        Takes text as string datatype.  Words can be on same or different lines.  Current version is English language only.  Email for support.
-        
-            import fkscore
-            text = '...blah blah blah...'
-            f = fkscore.fkscore(text)
-            print(f.stats)
-            print(f.score)
-        
-            OR
-        
-            from fkscore import fkscore
-            text = '...blah blah blah...'
-            f = fkscore(text)
-            print(f.stats)
-            print(f.score)
-        
-        ### Output ###
-        Output includes 2 dictionaries of information as follows:
-        * stats:
-          * stats['num_words']
-          * stats['num_syllables']
-          * stats['num_sentences']
-        * score:
-          * score['readability']  # Calculated F-K Readability Score
-          * score['grade']        # Permuted F-K Grade Reading Level
-        
-        ### Releases ###
-        Releases and additions will push to PyPi periodically, but if there is a feature in master not built/pushed and you want it to be, just ping me.
-        
-        ### History ###
-        This is a maintained as an implementation of the Flesch-Kincaid readability algorithm which was initially developed in 1948 by Rudolph Flesch and later revised by the U.S. Navy in 1975.  This module is pure python and works with 3.5+.
-        
-        ### Questions ###
-        Feel free to ping for questions, comments, concerns or interact directly via the GitHub repository.
-        
-        Randall Shane, PhD<br />
-        Randall.Shane@CodeIntelligence.IO<br />
-        https://github.com/RandallShanePhD/fkscore<br />
-        Thank you!
-        
 Keywords: nlp,linguistics,nltk,text processing
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Text Processing :: Linguistic
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Text Processing :: Indexing
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+fkscore
+====
+
+Flesch Kincaid readability score for text
+
+A Python module implementation of the Flesch Kincaid readability score algorithm.
+
+The source code is released under the MIT License.
+
+### Installation ###
+    pip3 install fkscore
+
+### Usage ###
+For text in python represented as a string.
+
+Takes text as string datatype.  Words can be on same or different lines.  Current version is English language only.  Email for support.
+
+    import fkscore
+    text = '...blah blah blah...'
+    f = fkscore.fkscore(text)
+    print(f.stats)
+    print(f.score)
+
+    OR
+
+    from fkscore import fkscore
+    text = '...blah blah blah...'
+    f = fkscore(text)
+    print(f.stats)
+    print(f.score)
+
+### Output ###
+Output includes 2 dictionaries of information as follows:
+* stats:
+  * stats['num_words']
+  * stats['num_syllables']
+  * stats['num_sentences']
+* score:
+  * score['readability']  # Calculated F-K Readability Score
+  * score['grade']        # Permuted F-K Grade Reading Level
+
+### Releases ###
+Releases and additions will push to PyPi periodically, but if there is a feature in master not built/pushed and you want it to be, just ping me.
+
+### History ###
+This is a maintained as an implementation of the Flesch-Kincaid readability algorithm which was initially developed in 1948 by Rudolph Flesch and later revised by the U.S. Navy in 1975.  This module is pure python and works with 3.5+.
+
+### Questions ###
+Feel free to ping for questions, comments, concerns or interact directly via the GitHub repository.
+
+Randall Shane PhD<br />
+Randall@NumbersAndTech.com<br />
+https://github.com/RandallShanePhD/fkscore<br />
+Thank you!
+
+
```

### Comparing `fkscore-1.1.6/setup.py` & `fkscore-1.1.7/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="fkscore",
-    version="1.1.6",
+    version="1.1.7",
 
     description="Flesch Kincaid readability scoring algorithm",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/RandallShanePhD/fkscore",
 
     # Author Info
-    author="Randall Shane, PhD <Randall.Shane@CodeIntelligence.IO>",
-    author_email="Randall.Shane@CodeIntelligence.IO",
+    author="Randall Shane PhD <Randall@NumbersAndTech.com>",
+    author_email="Randall@NumbersAndTech.com",
 
 
     # License
     license='MIT',
 
     classifiers=[
         # How mature is this project? Common values are
@@ -37,16 +37,16 @@
         'License :: OSI Approved :: MIT License',
 
         # Specify the Python versions you support here. In particular, ensure
         # that you indicate whether you support Python 2, Python 3 or both.
         'Programming Language :: Python :: 3.5',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
-
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
         "Operating System :: OS Independent",
-
     ],
 
     keywords=["nlp", 'linguistics', 'nltk', 'text processing'],
     packages=setuptools.find_packages(),
     python_requires='>=3.5',
 )
```

