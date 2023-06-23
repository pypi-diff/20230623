# Comparing `tmp/actuarialmath-0.0.8.tar.gz` & `tmp/actuarialmath-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "actuarialmath-0.0.8.tar", last modified: Thu Jun  8 18:51:56 2023, max compression
+gzip compressed data, was "actuarialmath-0.0.9.tar", last modified: Mon Jun 19 13:00:41 2023, max compression
```

## Comparing `actuarialmath-0.0.8.tar` & `actuarialmath-0.0.9.tar`

### file list

```diff
@@ -1,37 +1,39 @@
-drwxrwxr-x   0 terence   (1000) terence   (1000)        0 2023-06-08 18:51:56.667060 actuarialmath-0.0.8/
--rw-rw-r--   0 terence   (1000) terence   (1000)     1073 2023-05-29 19:44:46.000000 actuarialmath-0.0.8/LICENSE
--rw-rw-r--   0 terence   (1000) terence   (1000)     4370 2023-06-08 18:51:56.667060 actuarialmath-0.0.8/PKG-INFO
--rw-rw-r--   0 terence   (1000) terence   (1000)     4827 2023-06-08 18:15:03.000000 actuarialmath-0.0.8/README.md
--rw-rw-r--   0 terence   (1000) terence   (1000)     3845 2023-06-08 18:21:02.000000 actuarialmath-0.0.8/index.rst
--rw-rw-r--   0 terence   (1000) terence   (1000)      712 2023-06-08 18:51:24.000000 actuarialmath-0.0.8/pyproject.toml
--rw-rw-r--   0 terence   (1000) terence   (1000)       38 2023-06-08 18:51:56.667060 actuarialmath-0.0.8/setup.cfg
-drwxrwxr-x   0 terence   (1000) terence   (1000)        0 2023-06-08 18:51:56.663060 actuarialmath-0.0.8/src/
-drwxrwxr-x   0 terence   (1000) terence   (1000)        0 2023-06-08 18:51:56.667060 actuarialmath-0.0.8/src/actuarialmath/
--rw-rw-r--   0 terence   (1000) terence   (1000)        0 2023-05-25 13:19:02.000000 actuarialmath-0.0.8/src/actuarialmath/__init__.py
--rw-rw-r--   0 terence   (1000) terence   (1000)     4942 2023-06-08 13:33:30.000000 actuarialmath-0.0.8/src/actuarialmath/actuarial.py
--rw-rw-r--   0 terence   (1000) terence   (1000)    14876 2023-06-08 17:49:44.000000 actuarialmath-0.0.8/src/actuarialmath/annuity.py
--rw-rw-r--   0 terence   (1000) terence   (1000)     9400 2023-06-08 15:51:43.000000 actuarialmath-0.0.8/src/actuarialmath/constantforce.py
--rw-rw-r--   0 terence   (1000) terence   (1000)     3638 2023-06-04 15:05:12.000000 actuarialmath-0.0.8/src/actuarialmath/extrarisk.py
--rw-rw-r--   0 terence   (1000) terence   (1000)     9482 2023-06-04 12:58:13.000000 actuarialmath-0.0.8/src/actuarialmath/fractional.py
--rw-rw-r--   0 terence   (1000) terence   (1000)    21113 2023-06-08 18:01:14.000000 actuarialmath-0.0.8/src/actuarialmath/insurance.py
--rw-rw-r--   0 terence   (1000) terence   (1000)     5973 2023-06-06 01:23:38.000000 actuarialmath-0.0.8/src/actuarialmath/interest.py
--rw-rw-r--   0 terence   (1000) terence   (1000)     6906 2023-06-04 12:26:59.000000 actuarialmath-0.0.8/src/actuarialmath/life.py
--rw-rw-r--   0 terence   (1000) terence   (1000)    12187 2023-06-08 17:34:26.000000 actuarialmath-0.0.8/src/actuarialmath/lifetable.py
--rw-rw-r--   0 terence   (1000) terence   (1000)     2706 2023-06-04 12:39:39.000000 actuarialmath-0.0.8/src/actuarialmath/lifetime.py
--rw-rw-r--   0 terence   (1000) terence   (1000)    12048 2023-06-04 14:53:49.000000 actuarialmath-0.0.8/src/actuarialmath/mortalitylaws.py
--rw-rw-r--   0 terence   (1000) terence   (1000)    12454 2023-06-04 15:08:44.000000 actuarialmath-0.0.8/src/actuarialmath/mthly.py
--rw-rw-r--   0 terence   (1000) terence   (1000)    21134 2023-06-04 14:09:48.000000 actuarialmath-0.0.8/src/actuarialmath/policyvalues.py
--rw-rw-r--   0 terence   (1000) terence   (1000)     8833 2023-06-04 13:33:45.000000 actuarialmath-0.0.8/src/actuarialmath/premiums.py
--rw-rw-r--   0 terence   (1000) terence   (1000)    60817 2023-06-08 13:24:50.000000 actuarialmath-0.0.8/src/actuarialmath/recursion.py
--rw-rw-r--   0 terence   (1000) terence   (1000)    11689 2023-06-04 14:13:35.000000 actuarialmath-0.0.8/src/actuarialmath/reserves.py
--rw-rw-r--   0 terence   (1000) terence   (1000)    19575 2023-06-04 14:36:57.000000 actuarialmath-0.0.8/src/actuarialmath/selectlife.py
--rw-rw-r--   0 terence   (1000) terence   (1000)     7296 2023-06-08 13:41:59.000000 actuarialmath-0.0.8/src/actuarialmath/sult.py
--rw-rw-r--   0 terence   (1000) terence   (1000)     8390 2023-06-04 12:50:08.000000 actuarialmath-0.0.8/src/actuarialmath/survival.py
--rw-rw-r--   0 terence   (1000) terence   (1000)     9937 2023-06-04 15:15:45.000000 actuarialmath-0.0.8/src/actuarialmath/udd.py
--rw-rw-r--   0 terence   (1000) terence   (1000)     8112 2023-06-04 15:16:53.000000 actuarialmath-0.0.8/src/actuarialmath/woolhouse.py
-drwxrwxr-x   0 terence   (1000) terence   (1000)        0 2023-06-08 18:51:56.667060 actuarialmath-0.0.8/src/actuarialmath.egg-info/
--rw-rw-r--   0 terence   (1000) terence   (1000)     4370 2023-06-08 18:51:56.000000 actuarialmath-0.0.8/src/actuarialmath.egg-info/PKG-INFO
--rw-rw-r--   0 terence   (1000) terence   (1000)      913 2023-06-08 18:51:56.000000 actuarialmath-0.0.8/src/actuarialmath.egg-info/SOURCES.txt
--rw-rw-r--   0 terence   (1000) terence   (1000)        1 2023-06-08 18:51:56.000000 actuarialmath-0.0.8/src/actuarialmath.egg-info/dependency_links.txt
--rw-rw-r--   0 terence   (1000) terence   (1000)       60 2023-06-08 18:51:56.000000 actuarialmath-0.0.8/src/actuarialmath.egg-info/requires.txt
--rw-rw-r--   0 terence   (1000) terence   (1000)       14 2023-06-08 18:51:56.000000 actuarialmath-0.0.8/src/actuarialmath.egg-info/top_level.txt
+drwxrwxr-x   0 terence   (1000) terence   (1000)        0 2023-06-19 13:00:41.621738 actuarialmath-0.0.9/
+-rw-rw-r--   0 terence   (1000) terence   (1000)     1073 2023-05-29 19:44:46.000000 actuarialmath-0.0.9/LICENSE
+-rw-rw-r--   0 terence   (1000) terence   (1000)     4241 2023-06-19 13:00:41.621738 actuarialmath-0.0.9/PKG-INFO
+-rw-rw-r--   0 terence   (1000) terence   (1000)     4695 2023-06-19 12:18:05.000000 actuarialmath-0.0.9/README.md
+-rw-rw-r--   0 terence   (1000) terence   (1000)     3719 2023-06-19 12:21:56.000000 actuarialmath-0.0.9/index.rst
+-rw-rw-r--   0 terence   (1000) terence   (1000)      720 2023-06-19 13:00:36.000000 actuarialmath-0.0.9/pyproject.toml
+-rw-rw-r--   0 terence   (1000) terence   (1000)       38 2023-06-19 13:00:41.621738 actuarialmath-0.0.9/setup.cfg
+drwxrwxr-x   0 terence   (1000) terence   (1000)        0 2023-06-19 13:00:41.621738 actuarialmath-0.0.9/src/
+drwxrwxr-x   0 terence   (1000) terence   (1000)        0 2023-06-19 13:00:41.621738 actuarialmath-0.0.9/src/actuarialmath/
+-rw-rw-r--   0 terence   (1000) terence   (1000)      709 2023-06-18 20:31:22.000000 actuarialmath-0.0.9/src/actuarialmath/__init__.py
+-rw-rw-r--   0 terence   (1000) terence   (1000)     4060 2023-06-19 03:40:47.000000 actuarialmath-0.0.9/src/actuarialmath/actuarial.py
+-rw-rw-r--   0 terence   (1000) terence   (1000)    14866 2023-06-18 20:28:41.000000 actuarialmath-0.0.9/src/actuarialmath/annuity.py
+-rw-rw-r--   0 terence   (1000) terence   (1000)     9386 2023-06-18 20:25:53.000000 actuarialmath-0.0.9/src/actuarialmath/constantforce.py
+-rw-rw-r--   0 terence   (1000) terence   (1000)     3619 2023-06-18 20:25:38.000000 actuarialmath-0.0.9/src/actuarialmath/extrarisk.py
+-rw-rw-r--   0 terence   (1000) terence   (1000)     9473 2023-06-18 20:28:59.000000 actuarialmath-0.0.9/src/actuarialmath/fractional.py
+-rw-rw-r--   0 terence   (1000) terence   (1000)    21102 2023-06-19 02:29:40.000000 actuarialmath-0.0.9/src/actuarialmath/insurance.py
+-rw-rw-r--   0 terence   (1000) terence   (1000)     5963 2023-06-18 20:29:37.000000 actuarialmath-0.0.9/src/actuarialmath/interest.py
+-rw-rw-r--   0 terence   (1000) terence   (1000)     6862 2023-06-18 20:29:30.000000 actuarialmath-0.0.9/src/actuarialmath/life.py
+-rw-rw-r--   0 terence   (1000) terence   (1000)    12178 2023-06-18 20:27:11.000000 actuarialmath-0.0.9/src/actuarialmath/lifetable.py
+-rw-rw-r--   0 terence   (1000) terence   (1000)     2697 2023-06-18 20:29:07.000000 actuarialmath-0.0.9/src/actuarialmath/lifetime.py
+-rw-rw-r--   0 terence   (1000) terence   (1000)    12027 2023-06-18 22:08:50.000000 actuarialmath-0.0.9/src/actuarialmath/mortalitylaws.py
+-rw-rw-r--   0 terence   (1000) terence   (1000)    12437 2023-06-18 20:33:10.000000 actuarialmath-0.0.9/src/actuarialmath/mthly.py
+-rw-rw-r--   0 terence   (1000) terence   (1000)    21095 2023-06-18 20:27:49.000000 actuarialmath-0.0.9/src/actuarialmath/policyvalues.py
+-rw-rw-r--   0 terence   (1000) terence   (1000)     8824 2023-06-18 20:28:06.000000 actuarialmath-0.0.9/src/actuarialmath/premiums.py
+-rw-rw-r--   0 terence   (1000) terence   (1000)    60459 2023-06-19 03:29:25.000000 actuarialmath-0.0.9/src/actuarialmath/recursion.py
+-rw-rw-r--   0 terence   (1000) terence   (1000)    11674 2023-06-18 20:31:54.000000 actuarialmath-0.0.9/src/actuarialmath/reserves.py
+-rw-rw-r--   0 terence   (1000) terence   (1000)    19564 2023-06-18 20:32:44.000000 actuarialmath-0.0.9/src/actuarialmath/selectlife.py
+-rw-rw-r--   0 terence   (1000) terence   (1000)     7286 2023-06-18 20:27:01.000000 actuarialmath-0.0.9/src/actuarialmath/sult.py
+-rw-rw-r--   0 terence   (1000) terence   (1000)     8385 2023-06-18 20:29:12.000000 actuarialmath-0.0.9/src/actuarialmath/survival.py
+-rw-rw-r--   0 terence   (1000) terence   (1000)     9918 2023-06-18 20:24:33.000000 actuarialmath-0.0.9/src/actuarialmath/udd.py
+-rw-rw-r--   0 terence   (1000) terence   (1000)     8098 2023-06-18 20:23:25.000000 actuarialmath-0.0.9/src/actuarialmath/woolhouse.py
+drwxrwxr-x   0 terence   (1000) terence   (1000)        0 2023-06-19 13:00:41.621738 actuarialmath-0.0.9/src/actuarialmath.egg-info/
+-rw-rw-r--   0 terence   (1000) terence   (1000)     4241 2023-06-19 13:00:41.000000 actuarialmath-0.0.9/src/actuarialmath.egg-info/PKG-INFO
+-rw-rw-r--   0 terence   (1000) terence   (1000)      935 2023-06-19 13:00:41.000000 actuarialmath-0.0.9/src/actuarialmath.egg-info/SOURCES.txt
+-rw-rw-r--   0 terence   (1000) terence   (1000)        1 2023-06-19 13:00:41.000000 actuarialmath-0.0.9/src/actuarialmath.egg-info/dependency_links.txt
+-rw-rw-r--   0 terence   (1000) terence   (1000)       60 2023-06-19 13:00:41.000000 actuarialmath-0.0.9/src/actuarialmath.egg-info/requires.txt
+-rw-rw-r--   0 terence   (1000) terence   (1000)       14 2023-06-19 13:00:41.000000 actuarialmath-0.0.9/src/actuarialmath.egg-info/top_level.txt
+drwxrwxr-x   0 terence   (1000) terence   (1000)        0 2023-06-19 13:00:41.621738 actuarialmath-0.0.9/tests/
+-rw-rw-r--   0 terence   (1000) terence   (1000)     2019 2023-06-19 12:37:26.000000 actuarialmath-0.0.9/tests/test_changes.py
```

### Comparing `actuarialmath-0.0.8/LICENSE` & `actuarialmath-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `actuarialmath-0.0.8/PKG-INFO` & `actuarialmath-0.0.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: actuarialmath
-Version: 0.0.8
+Version: 0.0.9
 Summary: A package for actuarial math and life contingent risks
 Author: Terence Lim
-Project-URL: Homepage, https://terence-lim.github.io/actuarialmath-tutorial
+Project-URL: Homepage, https://terence-lim.github.io/actuarialmath-guide
 Project-URL: Bug Tracker, https://github.com/terence-lim/actuarialmath/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/x-rst
 License-File: LICENSE
@@ -27,66 +27,65 @@
    - Basic interest theory and probability laws
 
    - Survival functions, expected future lifetimes and fractional ages
 
    - Insurance, annuity, premiums, policy values, and reserves calculations
 
 
-2. Specify and load a particular form of assumptions
+2. Adjust results for
 
-   - Life table, select life table, or standard ultimate life table
-
-   - Mortality laws, such as constant force of maturity, beta and uniform distributions, or Makeham's and Gompertz's laws
+   - Extra mortality risks
 
-   - Recursion inputs
+   - 1/mthly payment frequency using UDD or Woolhouse approaches
 
-3. Adjust results for
+3. Specify and load a particular form of assumptions
 
-   - Extra mortality risks
+   - Life table, select life table, or standard ultimate life table
 
-   - 1/mthly payment frequency using UDD or Woolhouse approaches
+   - Mortality laws, such as constant force of maturity, beta and uniform distributions, or Makeham's and Gompertz's laws
 
+   - Recursion inputs
+    
+     
 Quick Start
 -----------
 
 1. ``pip install actuarialmath``
    
    - also requires `numpy`, `scipy`, `matplotlib` and `pandas`.
      
 2. Start Python (version >= 3.10) or Jupyter-notebook
 
    - Select a suitable subclass to initialize with your actuarial assumptions, such as `MortalityLaws` (or a special law like `ConstantForce`), `LifeTable`, `SULT`, `SelectLife` or `Recursion`.
       
    - Call appropriate methods to compute intermediate or final results, or to `solve` parameter values implicitly.
 
-   - If needed, adjust the answers with `ExtraRisk` or `Mthly` (or its `UDD` or `Woolhouse`) classes.
+   - Adjust the answers with `ExtraRisk` or `Mthly` (or its `UDD` or `Woolhouse`) classes.
 
 Examples
 --------
 
 ::
 
   # SOA FAM-L sample question 5.7
-  from actuarialmath.recursion import Recursion
-  from actuarialmath.woolhouse import Woolhouse
+  from actuarialmath.recursion import Recursion, Woolhouse
   # initialize Recursion class with actuarial inputs
   life = Recursion().set_interest(i=0.04)\
                     .set_A(0.188, x=35)\
                     .set_A(0.498, x=65)\
                     .set_p(0.883, x=35, t=30)
   # modfy the standard results with Woolhouse mthly approximation
   mthly = Woolhouse(m=2, life=life, three_term=False)
   # compute the desired temporary annuity value
   print(1000 * mthly.temporary_annuity(35, t=30)) #   solution = 17376.7
 
 ::
 
   # SOA FAM-L sample question 7.20
-  from actuarialmath.sult import SULT   # use Standard Ultimate Life Table
-  from actuarialmath.policyvalues import Contract
+  from actuarialmath.sult import SULT, Contract
   life = SULT()
   # compute the required FPT policy value
   S = life.FPT_policy_value(35, t=1, b=1000)  # is always 0 in year 1!
   # input the given policy contract terms
   contract = Contract(benefit=1000,
                       initial_premium=.3,
                       initial_policy=300,
@@ -99,13 +98,13 @@
   print(R-S)   # solution = -277.19
 
 Resources
 ---------
 
 1. `Colab <https://colab.research.google.com/drive/1TcNr1x5HbT2fF3iFMYGXdN_cvRKiSua4?usp=sharing>`_ or `Jupyter notebook <https://terence-lim.github.io/notes/faml.ipynb>`_, to solve all sample SOA FAM-L exam questions
 
-2. `Online tutorial <https://terence-lim.github.io/actuarialmath-tutorial/>`_, or `download pdf <https://terence-lim.github.io/notes/actuarialmath-tutorial.pdf>`_
+2. `User Guide <https://terence-lim.github.io/actuarialmath-guide/>`_, or `download pdf <https://terence-lim.github.io/notes/actuarialmath-guide.pdf>`_
 
 3. `Code documentation <https://actuarialmath.readthedocs.io/en/latest/>`_
 
 4. `Github repo <https://github.com/terence-lim/actuarialmath.git>`_ and `issues <https://github.com/terence-lim/actuarialmath/issues>`_
```

### Comparing `actuarialmath-0.0.8/README.md` & `actuarialmath-0.0.9/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -19,25 +19,24 @@
 2. Start Python (version >= 3.10) or Jupyter-notebook
 
 
    - Select and import a suitable subclass to initialize with your actuarial assumptions, such as `MortalityLaws` (or a special law like `ConstantForce`), `LifeTable`, `SULT`, `SelectLife` or `Recursion`.
 
    - Call appropriate methods to compute intermediate or final results, or to `solve` parameter values implicitly.
 
-   - If needed, adjust the answers with `ExtraRisk` or `Mthly` (or its `UDD` or `Woolhouse`) classes.
+   - Adjust the answers with `ExtraRisk` or `Mthly` (or its `UDD` or `Woolhouse`) classes.
 
 ## Examples
 
 __SOA FAM-L sample question 5.7__: 
 
 Given $A_{35} = 0.188$, $A_{65} = 0.498$, $S_{35}(30) = 0.883$, calculate the EPV of a temporary annuity $\ddot{a}^{(2)}_{35:\overline{30|}}$ paid half-yearly using the Woolhouse approximation.
 
 ```
-from actuarialmath.recursion import Recursion
-from actuarialmath.woolhouse import Woolhouse
+from actuarialmath.recursion import Recursion, Woolhouse
 # initialize Recursion class with actuarial inputs
 life = Recursion().set_interest(i=0.04)\
                   .set_A(0.188, x=35)\
                   .set_A(0.498, x=65)\
                   .set_p(0.883, x=35, t=30)
 # modfy the standard results with Woolhouse mthly approximation
 mthly = Woolhouse(m=2, life=life, three_term=False)
@@ -55,16 +54,15 @@
 - The gross premium policy value at the end of the first policy year is R
 - Using the Full Preliminary Term Method, the modified reserve at the end of the first policy year is S
 - Mortality follows the Standard Ultimate Life Table
 - _i_ = 0.05
 
 Calculate R − S
 ```
-from actuarialmath.sult import SULT   # use Standard Ultimate Life Table
-from actuarialmath.policyvalues import Contract
+from actuarialmath.sult import SULT, Contract
 life = SULT()
 # compute the required FPT policy value
 S = life.FPT_policy_value(35, t=1, b=1000)  # is always 0 in year 1!
 # input the given policy contract terms
 contract = Contract(benefit=1000,
                     initial_premium=.3,
                     initial_policy=300,
@@ -78,15 +76,15 @@
 ```
 
 
 ## Resources
 
 1. [Colab](https://colab.research.google.com/drive/1TcNr1x5HbT2fF3iFMYGXdN_cvRKiSua4?usp=sharing) or [Jupyter notebook](https://terence-lim.github.io/notes/faml.ipynb), to solve all sample SOA FAM-L exam questions
 
-2. [Online tutorial](https://terence-lim.github.io/actuarialmath-tutorial/), or [download pdf](https://terence-lim.github.io/notes/actuarialmath-tutorial.pdf)
+2. [User Guide](https://terence-lim.github.io/actuarialmath-guide/), or [download pdf](https://terence-lim.github.io/notes/actuarialmath-guide.pdf)
 
 3. [Code documentation](https://actuarialmath.readthedocs.io/en/latest/)
 
 4. [Github repo](https://github.com/terence-lim/actuarialmath.git) and [issues](https://github.com/terence-lim/actuarialmath/issues)
```

### Comparing `actuarialmath-0.0.8/index.rst` & `actuarialmath-0.0.9/index.rst`

 * *Files 11% similar despite different names*

```diff
@@ -13,66 +13,65 @@
    - Basic interest theory and probability laws
 
    - Survival functions, expected future lifetimes and fractional ages
 
    - Insurance, annuity, premiums, policy values, and reserves calculations
 
 
-2. Specify and load a particular form of assumptions
+2. Adjust results for
 
-   - Life table, select life table, or standard ultimate life table
-
-   - Mortality laws, such as constant force of maturity, beta and uniform distributions, or Makeham's and Gompertz's laws
+   - Extra mortality risks
 
-   - Recursion inputs
+   - 1/mthly payment frequency using UDD or Woolhouse approaches
 
-3. Adjust results for
+3. Specify and load a particular form of assumptions
 
-   - Extra mortality risks
+   - Life table, select life table, or standard ultimate life table
 
-   - 1/mthly payment frequency using UDD or Woolhouse approaches
+   - Mortality laws, such as constant force of maturity, beta and uniform distributions, or Makeham's and Gompertz's laws
 
+   - Recursion inputs
+    
+     
 Quick Start
 -----------
 
 1. ``pip install actuarialmath``
    
    - also requires `numpy`, `scipy`, `matplotlib` and `pandas`.
      
 2. Start Python (version >= 3.10) or Jupyter-notebook
 
    - Select a suitable subclass to initialize with your actuarial assumptions, such as `MortalityLaws` (or a special law like `ConstantForce`), `LifeTable`, `SULT`, `SelectLife` or `Recursion`.
       
    - Call appropriate methods to compute intermediate or final results, or to `solve` parameter values implicitly.
 
-   - If needed, adjust the answers with `ExtraRisk` or `Mthly` (or its `UDD` or `Woolhouse`) classes.
+   - Adjust the answers with `ExtraRisk` or `Mthly` (or its `UDD` or `Woolhouse`) classes.
 
 Examples
 --------
 
 ::
 
   # SOA FAM-L sample question 5.7
-  from actuarialmath.recursion import Recursion
-  from actuarialmath.woolhouse import Woolhouse
+  from actuarialmath.recursion import Recursion, Woolhouse
   # initialize Recursion class with actuarial inputs
   life = Recursion().set_interest(i=0.04)\
                     .set_A(0.188, x=35)\
                     .set_A(0.498, x=65)\
                     .set_p(0.883, x=35, t=30)
   # modfy the standard results with Woolhouse mthly approximation
   mthly = Woolhouse(m=2, life=life, three_term=False)
   # compute the desired temporary annuity value
   print(1000 * mthly.temporary_annuity(35, t=30)) #   solution = 17376.7
 
 ::
 
   # SOA FAM-L sample question 7.20
-  from actuarialmath.sult import SULT   # use Standard Ultimate Life Table
-  from actuarialmath.policyvalues import Contract
+  from actuarialmath.sult import SULT, Contract
   life = SULT()
   # compute the required FPT policy value
   S = life.FPT_policy_value(35, t=1, b=1000)  # is always 0 in year 1!
   # input the given policy contract terms
   contract = Contract(benefit=1000,
                       initial_premium=.3,
                       initial_policy=300,
@@ -85,13 +84,13 @@
   print(R-S)   # solution = -277.19
 
 Resources
 ---------
 
 1. `Colab <https://colab.research.google.com/drive/1TcNr1x5HbT2fF3iFMYGXdN_cvRKiSua4?usp=sharing>`_ or `Jupyter notebook <https://terence-lim.github.io/notes/faml.ipynb>`_, to solve all sample SOA FAM-L exam questions
 
-2. `Online tutorial <https://terence-lim.github.io/actuarialmath-tutorial/>`_, or `download pdf <https://terence-lim.github.io/notes/actuarialmath-tutorial.pdf>`_
+2. `User Guide <https://terence-lim.github.io/actuarialmath-guide/>`_, or `download pdf <https://terence-lim.github.io/notes/actuarialmath-guide.pdf>`_
 
 3. `Code documentation <https://actuarialmath.readthedocs.io/en/latest/>`_
 
 4. `Github repo <https://github.com/terence-lim/actuarialmath.git>`_ and `issues <https://github.com/terence-lim/actuarialmath/issues>`_
```

### Comparing `actuarialmath-0.0.8/pyproject.toml` & `actuarialmath-0.0.9/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "actuarialmath"
-version = "0.0.8" # "0.0.98" 
+#version =  "0.0.100"
+version = "0.0.9" 
 authors = [
   { name="Terence Lim"},
 ]
 description = "A package for actuarial math and life contingent risks"
 readme = "index.rst"
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 dependencies = [
-  "matplotlib==3.7.1",
-  "numpy==1.24.3",
-  "pandas==2.0.2",
-  "scipy==1.10.1",
+  "matplotlib>=3.7.1",
+  "numpy>=1.24.3",
+  "pandas>=2.0.2",
+  "scipy>=1.10.1",
 ]
 
 [project.urls]
-"Homepage" = "https://terence-lim.github.io/actuarialmath-tutorial"
+"Homepage" = "https://terence-lim.github.io/actuarialmath-guide"
 "Bug Tracker" = "https://github.com/terence-lim/actuarialmath/issues"
```

### Comparing `actuarialmath-0.0.8/src/actuarialmath/actuarial.py` & `actuarialmath-0.0.9/src/actuarialmath/actuarial.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 """Define base class for actuarial math, with utility helpers and constants
 
 MIT License. Copyright (c) 2022-2023 Terence Lim
 """
 import math
 import numpy as np
 import scipy
+import matplotlib.pyplot as plt
 from typing import Callable, Any, Tuple, List
 
+plt.style.use('ggplot')
+
 class Actuarial(object):
     """Define constants and common utility functions
 
     Constants:
       VARIANCE : select variance as the statistical moment to calculate
 
       WHOLE : indicates that term of insurance or annuity is Whole Life
@@ -21,36 +24,14 @@
     _VARIANCE = VARIANCE
     _WHOLE = WHOLE
     _TOL = 1e-6
     _verbose = 0
     _MAXAGE = 130    # default oldest age
     _MINAGE = 0      # default youngest age
 
-    @classmethod
-    def methods(cls, echo: bool = True):
-        """Helper to partially display docstrings from classes and methods
-
-        Args:
-          echo : print if True, else return as text string
-        """
-        s = "\nclass " + cls.__name__ + " - "
-        s += "\n".join([l for l in cls.__doc__.strip().split('\n')]) + "\n"
-        if hasattr(cls, '_methods') and cls._methods:
-            s += '\n    Methods:\n    --------\n\n'
-            for method in cls._methods:
-                meth = getattr(cls, method)
-                desc = meth.__doc__.strip().split('\n')[0]
-                if callable(meth):
-                    args = [str(arg) for arg in signature(meth).parameters.keys()
-                            if str(arg) not in ['cls', 'self']]
-                else:
-                    args = []
-                s += f"    {method}(" + ", ".join(args) + f"):\n{' '*6}{desc}\n\n"
-        return print(s) if echo else s
-
     #
     # Helpers for numerical computations
     #
     @staticmethod
     def integral(fun: Callable[[float], float],
                  lower: float,
                  upper: float) -> float:
@@ -108,15 +89,15 @@
           n : second term to add
         """
         if t == self.WHOLE or n == self.WHOLE:
             return self.WHOLE  # adding any term to WHOLE is still WHOLE
         return t + n
 
     def max_term(self, x: int, t: int, u: int = 0) -> int:
-        """Decrease term t if deferral period u to (x) exceeds maxage
+        """Decrease term t if adding deferral period u to (x) exceeds maxage
 
         Args:
           x : age
           t : term of insurance or annuity, after deferral period
           u : term deferred
 
         Returns:
```

### Comparing `actuarialmath-0.0.8/src/actuarialmath/annuity.py` & `actuarialmath-0.0.9/src/actuarialmath/annuity.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 MIT License. Copyright (c) 2022-2023 Terence Lim
 """
 from typing import Callable, Any
 import math
 import matplotlib.pyplot as plt
 import numpy as np
-from actuarialmath.insurance import Insurance
+from actuarialmath import Insurance
 
 class Annuity(Insurance):
     """Compute present values and relationships of life annuities"""
 
     def a_x(self, x: int, s: int = 0, t: int = Insurance.WHOLE, u: int = 0,
             benefit: Callable = lambda x,t: 1, discrete: bool = True) -> float:
         """Numerically compute EPV of annuities from survival functions
```

### Comparing `actuarialmath-0.0.8/src/actuarialmath/constantforce.py` & `actuarialmath-0.0.9/src/actuarialmath/constantforce.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Constant Force of Mortality - shortcut formulas
 
 MIT License. Copyright 2022-2023 Terence Lim
 """
 import math
 from scipy.stats import norm
-from actuarialmath.mortalitylaws import MortalityLaws
+from actuarialmath import MortalityLaws
 
 class ConstantForce(MortalityLaws):
     """Constant force of mortality - memoryless exponential distribution of lifetime
 
     Args:
       mu : constant value of force of mortality
       udd : assume UDD (True) or CFM (False, default) between integer ages
```

### Comparing `actuarialmath-0.0.8/src/actuarialmath/extrarisk.py` & `actuarialmath-0.0.9/src/actuarialmath/extrarisk.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Extra Risk - Adjusts force of mortality, age rating or mortality rate
 
 MIT License. Copyright 2022-2023 Terence Lim
 """
-from actuarialmath.survival import Survival
-from actuarialmath.actuarial import Actuarial
 from typing import Dict
 import math
+from actuarialmath import Survival
+from actuarialmath import Actuarial
 
 class ExtraRisk(Actuarial):
     """Adjust mortality by extra risk
 
     Args:
       life : original survival and mortality rates
       extra : amount of extra risk to adjust
```

### Comparing `actuarialmath-0.0.8/src/actuarialmath/fractional.py` & `actuarialmath-0.0.9/src/actuarialmath/fractional.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Fractional age assumptions- Computes survival and mortality functions between integer ages.
 
 MIT License. Copyright (c) 2022-2023 Terence Lim
 """
 
 import math
-from actuarialmath.lifetime import Lifetime
+from actuarialmath import Lifetime
 
 class Fractional(Lifetime):
     """Compute survival functions at fractional ages and durations
 
     Args:
       udd : select UDD (True, default) or CFM (False) between integer ages
     """
```

### Comparing `actuarialmath-0.0.8/src/actuarialmath/insurance.py` & `actuarialmath-0.0.9/src/actuarialmath/insurance.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 MIT License. Copyright (c) 2022-2023 Terence Lim
 """
 from typing import Callable, Any, Tuple, List
 import math
 import matplotlib.pyplot as plt
 import numpy as np
-from actuarialmath.fractional import Fractional
+from actuarialmath import Fractional
 
 class Insurance(Fractional):
     """Compute expected present values of life insurance"""
 
     def E_x(self, x: int, s: int = 0, t: int = 1, endowment: int = 1,
             moment: int = 1) -> float:
         """Pure endowment: t_E_x
```

### Comparing `actuarialmath-0.0.8/src/actuarialmath/interest.py` & `actuarialmath-0.0.9/src/actuarialmath/interest.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 MIT License. Copyright (c) 2022-2023 Terence Lim
 """
 import math
 import numpy as np
 import pandas as pd
 from typing import Callable
-from actuarialmath.actuarial import Actuarial
+from actuarialmath import Actuarial
 
 class Interest(Actuarial):
     """Converts interest rates, and computes value of annuity certain
     
     Args:
       i : assumed annual interest rate
       d : or assumed discount rate
```

### Comparing `actuarialmath-0.0.8/src/actuarialmath/life.py` & `actuarialmath-0.0.9/src/actuarialmath/life.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,16 +4,15 @@
 """
 import math
 import numpy as np
 import pandas as pd
 from scipy.special import ndtri
 from scipy.stats import norm
 from typing import Callable, Dict, Any, Tuple, List
-from actuarialmath.interest import Interest
-from actuarialmath.actuarial import Actuarial
+from actuarialmath import Actuarial, Interest
 
 class Life(Actuarial):
     """Compute moments and probabilities"""
 
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
         self.set_interest(i=0)
```

### Comparing `actuarialmath-0.0.8/src/actuarialmath/lifetable.py` & `actuarialmath-0.0.9/src/actuarialmath/lifetable.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 MIT License. Copyright 2022-2023 Terence Lim
 """
 import math
 import numpy as np
 import matplotlib.pyplot as plt
 import pandas as pd
 from typing import Dict
-from actuarialmath.reserves import Reserves
+from actuarialmath import Reserves
 
 class LifeTable(Reserves):
     """Calculate life table, and iteratively fill in missing values
 
     Args:
       udd : assume UDD or constant force of mortality for fractional ages
       verbose : whether to echo update steps
```

### Comparing `actuarialmath-0.0.8/src/actuarialmath/lifetime.py` & `actuarialmath-0.0.9/src/actuarialmath/lifetime.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Future lifetimes - Computes expectations and moments of future lifetime
 
 MIT License. Copyright (c) 2022-2023 Terence Lim
 """
 import math
-from actuarialmath.survival import Survival
+from actuarialmath import Survival
 
 class Lifetime(Survival):
     """Computes expected moments of future lifetime"""
 
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
```

### Comparing `actuarialmath-0.0.8/src/actuarialmath/mortalitylaws.py` & `actuarialmath-0.0.9/src/actuarialmath/mortalitylaws.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Mortality Laws: Applies shortcut formulas for Beta, Uniform, Makeham and Gompertz
 
 MIT License. Copyright 2022-2023 Terence Lim
 """
 import math
-from actuarialmath.reserves import Reserves
+from actuarialmath import Reserves
 
 class MortalityLaws(Reserves):
     """Apply shortcut formulas for special mortality laws"""
 
     #
     # Define fractional age actuarial survival functions
     #
@@ -63,15 +63,15 @@
           s : years after selection
           r : fractional year after selection
           t : mortality at fractional year t
         """
         return self.f(x, s+r, t)
 
     def e_r(self, x: int, s: int = 0, r: float = 0.,
-            t: float = Reserves._WHOLE) -> float:
+            t: float = Reserves.WHOLE) -> float:
         """Fractional age future lifetime given special mortality law
 
         Args:
           x : age of selection
           s : years after selection
           r : fractional year after selection
           t : limited at t years
@@ -107,28 +107,28 @@
         def _f(x: int, s,t : float) -> float:
             return alpha / (omega - (x+s))
 
         self.set_survival(mu=_mu, l=_l, S=_S, f=_f, minage=0, maxage=omega)
         self.omega_ = omega  # store omega parameter
         self.alpha_ = alpha  # store alpha parameter
 
-    def e_r(self, x: int, s: int = 0, t: float = Reserves._WHOLE) -> float:
+    def e_r(self, x: int, s: int = 0, t: float = Reserves.WHOLE) -> float:
         """Expectation of future lifetime through fractional age: e_[x]+s:t
 
         Args:
           x : age of selection
           s : years after selection
           t : limited at t years
         """
         e = (self.omega_ - (x+s)) / (self.alpha_ + 1)
         if t > 0 and self.max_term(x+s, t) > t: # temporary expectation
             return e - self.p_r(x, s=s, t=t) * self.e_r(x, s=s+t)
         return e   # complete expectation
 
-    def e_x(self, x: int, s: int = 0, n: int = MortalityLaws._WHOLE, 
+    def e_x(self, x: int, s: int = 0, n: int = MortalityLaws.WHOLE, 
           curtate: bool = False, moment: int = 1) -> float:
         """Shortcut formula for complete expectation
 
         Args:
           x : age of selection
           s : years after selection
           n : death within next n fractional years
@@ -137,15 +137,15 @@
           moment : whether to compute first (1) or second (2) moment
         """
         if n == 0:
             return 0
         if not curtate:
             if moment == 1:
                 return self.e_r(x, s=s, t=n)
-            if moment == self._VARIANCE and n < 0: # shortcut for complete variance
+            if moment == self.VARIANCE and n < 0: # shortcut for complete variance
                 return ((self.omega_ - (x + s))
                         / ((self.alpha_ + 1)**2 * (self.alpha_ + 1)))
         return super().__init__(x=x, s=s, n=n, curtate=curtate, moment=moment)
 
 class Uniform(Beta):
     """Shortcuts with uniform distribution of deaths aka DeMoivre's Law
 
@@ -154,40 +154,40 @@
       udd : assume UDD (True, default) or CFM (False) between integer ages
     """
 
     def __init__(self, omega: int, udd: bool = True, **kwargs):
         """One parameter: omega = maxage, with mu(x) = 1/(omega - x)"""
         super().__init__(omega=omega, alpha=1, udd=udd, **kwargs)
 
-    def e_x(self, x: int, s: int = 0, t: int = Beta._WHOLE, 
+    def e_x(self, x: int, s: int = 0, t: int = Beta.WHOLE, 
           curtate: bool = False, moment: int = 1) -> float:
         """Shortcut for expected future lifetime
 
         Args:
           x : age of selection
           s : years after selection
           t : limited at t years
           curtate : whether curtate (True) or complete (False) lifetime
           moment : whether to compute first (1) or second (2) moment
         """
-        if moment in [1, self._VARIANCE] and not curtate:
+        if moment in [1, self.VARIANCE] and not curtate:
             if t < 0:
-                if moment == self._VARIANCE:
+                if moment == self.VARIANCE:
                     return (self.omega_ - x)**2 / 12  # complete shortcut
                 else:
                     return (self.omega_ - x) / 2
             elif moment == 1:         # temporary expectation shortcut
                 # (Pr[die within n years] * n/2) plus (Pr[survive n years] * n)
                 t = self.max_term(x+s, t)
                 t_p_x = t / (self.omega_ - x)
                 return t_p_x * t  + (1 - t_p_x) * (t / 2)
         return super().__init__(x=x, s=s, t=t, curtate=curtate, moment=moment)
 
     
-    def E_x(self, x: int, s: int = 0, t: int = Beta._WHOLE, 
+    def E_x(self, x: int, s: int = 0, t: int = Beta.WHOLE, 
             moment: int = 1) -> float:
         """Shortcut for Pure Endowment
 
         Args:
           x : age of selection
           s : years after selection
           t : term of pure endowment
@@ -197,15 +197,15 @@
         assert moment > 0
         if t == 0:
             return 1.
         if t < 0:
             return 0.
         t = self.max_term(x+s, t)
         t_p_x = (self.omega_ - x - t) / (self.omega_ - x)
-        if moment == self._VARIANCE:  # Bernoulli shortcut for variance
+        if moment == self.VARIANCE:  # Bernoulli shortcut for variance
             return self.interest.v_t(t)**2 * t_p_x * (1 - t_p_x)
         return (self.interest.v_t(t)**moment * (self.omega_ - x - t) 
                 / (self.omega_ - x))
 
     def whole_life_insurance(self, x: int, s: int = 0, moment: int = 1, 
                              b: int = 1, discrete: bool = True) -> float:
         """Shortcut for whole life insurance
@@ -215,15 +215,15 @@
           s : years after selection
           b : amount of benefit
           moment : compute first or second moment
           discrete : benefit paid year-end (True) or moment of death (False)
         """
 
         if not discrete:
-            if moment == Beta._VARIANCE:
+            if moment == Beta.VARIANCE:
                 return (self.whole_life_insurance(x, s=s, b=b, moment=2, 
                                                   discrete=False) -
                         self.whole_life_insurance(x, s=s, b=b, moment=1, 
                                                     discrete=False)**2) * b**2
             return self.term_insurance(x, s=s, t=self.omega_-(x+s), b=b,
                                        moment=moment, discrete=False)
         return super().whole_life_insurance(x, s=s, moment=moment, b=b,
@@ -237,16 +237,16 @@
           x : age of selection
           s : years after selection
           t : term of insurance
           b : amount of benefit
           moment : compute first or second moment
           discrete : benefit paid year-end (True) or moment of death (False)
         """
-        if not discrete and moment in [1, Beta._VARIANCE]:
-            if moment == Beta._VARIANCE:
+        if not discrete and moment in [1, Beta.VARIANCE]:
+            if moment == Beta.VARIANCE:
                 return (self.term_insurance(x, s=s, b=b, t=t, moment=2, 
                                             discrete=False) -
                         self.term_insurance(x, s=s, b=b, t=t, 
                                             discrete=False)**2) * b**2
             t = self.max_term(x+s, t)                                        
             return (b * (1 - self.interest.v_t(t)) 
                     / (self.interest.delta * (self.omega_ - (x+s))))
```

### Comparing `actuarialmath-0.0.8/src/actuarialmath/mthly.py` & `actuarialmath-0.0.9/src/actuarialmath/mthly.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """1/Mthly - Calculates m'thly-pay insurance and annuities
 
 MIT License. Copyright 2022-2023 Terence Lim
 """
 from typing import Callable
 import math
 import pandas as pd
-from actuarialmath.annuity import Annuity
-from actuarialmath.life import Actuarial
+from actuarialmath import Annuity
+from actuarialmath import Actuarial
 
 class Mthly(Actuarial):
     """Compute 1/M'thly insurance and annuities
 
     Args:
       m : number of payments per year
       life : original survival and life contingent functions
@@ -157,15 +157,15 @@
         if t < 0 or self.life.max_term(x+s, t) < t:
             return A
         E = self.E_x(x, s=s, t=t, moment=moment)
         A -= E * self.whole_life_insurance(x, s=s+t, b=b, moment=moment)
         return A
 
     def deferred_insurance(self, x: int, s: int = 0, n: int = 0, b: int = 1, 
-                           t: int = Annuity._WHOLE, moment: int = 1) -> float:
+                           t: int = Annuity.WHOLE, moment: int = 1) -> float:
         """Deferred insurance n|_A_x:t^1 = discounted whole life
 
         Args:
           x : year of selection
           s : years after selection
           u : years to defer
           t : term of insurance in years
@@ -248,15 +248,15 @@
         """
         if variance:  # short cut for variance of whole life
             A1 = self.whole_life_insurance(x, s=s, moment=1)
             A2 = self.whole_life_insurance(x, s=s, moment=2)
             return self.annuity_variance(A2=A2, A1=A1, b=b)
         return b * (1 - self.whole_life_insurance(x, s=s)) / self.d
             
-    def temporary_annuity(self, x: int, s: int = 0, t: int = Annuity._WHOLE, 
+    def temporary_annuity(self, x: int, s: int = 0, t: int = Annuity.WHOLE, 
                           b: int = 1, variance: bool = False) -> float:
         """Temporary m'thly life annuity: a_x:t
 
         Args:
           x : year of selection
           s : years after selection
           t : term of annuity in years
@@ -272,29 +272,29 @@
         a = self.whole_life_annuity(x, s=s, b=b)
         if t < 0 or self.max_term(x+s, t) < t:
             return a
         a_t = self.whole_life_annuity(x, s=s+t, b=b)
         return a - (a_t * self.E_x(x, s=s, t=t))
 
     def deferred_annuity(self, x: int, s: int = 0, u: int = 0, 
-                         t: int = Annuity._WHOLE, b: int = 1) -> float:
+                         t: int = Annuity.WHOLE, b: int = 1) -> float:
         """Deferred m'thly life annuity due n|t_a_x =  n+t_a_x - n_a_x
 
         Args:
           x : year of selection
           s : years after selection
           u : years of deferral
           t : term of annuity in years
           b : amount of benefit
         """
         if self.life.max_term(x+s, u) < u:
             return 0.
         return self.E_x(x, s=s, t=u)*self.temporary_annuity(x, s=s+u, t=t, b=b)
 
-    def immediate_annuity(self, x: int, s: int = 0, t: int = Annuity._WHOLE, 
+    def immediate_annuity(self, x: int, s: int = 0, t: int = Annuity.WHOLE, 
                           b: int = 1) -> float:
         """Immediate m'thly annuity
 
         Args:
           x : year of selection
           s : years after selection
           t : term of annuity in years
```

### Comparing `actuarialmath-0.0.8/src/actuarialmath/policyvalues.py` & `actuarialmath-0.0.9/src/actuarialmath/policyvalues.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,16 +3,15 @@
 MIT License. Copyright 2022-2023 Terence Lim
 """
 import math
 import numpy as np
 import scipy
 import matplotlib.pyplot as plt
 from typing import Dict, Any
-from actuarialmath.premiums import Premiums
-from actuarialmath.life import Actuarial
+from actuarialmath import Premiums, Actuarial
 
 class Contract(Actuarial):
     """Set and retrieve policy contract terms
 
     Args:
       premium : level premium amount
       benefit : insurance death benefit amount
```

### Comparing `actuarialmath-0.0.8/src/actuarialmath/premiums.py` & `actuarialmath-0.0.9/src/actuarialmath/premiums.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 """Premiums - Computes net and gross premiums, with the equivalence principle
 
 MIT License. Copyright (c) 2022-2023 Terence Lim
 """
-from actuarialmath.annuity import Annuity
+from actuarialmath import Annuity
 
 class Premiums(Annuity):
     """Compute et and gross premiums under equivalence principle"""
 
     #
     # Net level premiums for special insurances
     #
-    def net_premium(self, x: int, s: int = 0, t: int = Annuity._WHOLE, 
+    def net_premium(self, x: int, s: int = 0, t: int = Annuity.WHOLE, 
                     u: int = 0, n: int = 0, b: int = 1,
                     endowment: int = 0, discrete: bool | None = True, 
                     return_premium: bool = False, annuity: bool = False,
                     initial_cost: float = 0.) -> float:
         """Net level premium for special n-pay, u-deferred t-year term insurance
 
         Args:
```

### Comparing `actuarialmath-0.0.8/src/actuarialmath/recursion.py` & `actuarialmath-0.0.9/src/actuarialmath/recursion.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Recursion - Applies recursion, shortcut and actuarial formulas
 
 MIT License. Copyright 2022-2023 Terence Lim
 """
 from typing import Tuple
-from actuarialmath.reserves import Reserves
+from actuarialmath import Reserves
 
 class Recursion(Reserves):
     """Solve by appling recursive, shortcut and actuarial formulas repeatedly
 
     Args:
       depth : maximum depth of recursions (default is 3)
       verbose : whether to echo recursion steps (True, default)
@@ -20,15 +20,15 @@
       - 'e' : (temporary) expected future lifetime, and moments
       - 'A' : deferred, term, endowment or whole life insurance, and moments
       - 'IA' : decreasing life insurance of t years
       - 'DA' : increasing life insurance of t years
       - 'a' : deferred, temporary or whole life annuity of t years, and moments
     """
 
-    def __init__(self, depth: int = 3, verbose: bool = True, **kwargs):
+    def __init__(self, depth: int = 5, verbose: bool = True, **kwargs):
         super().__init__(**kwargs)
         self.db = {}
         self.maxdepth = depth
         _Blog._verbose = verbose
 
     #
     # helpers to store given input values
@@ -91,15 +91,15 @@
         if found is not None:
             return found
         if t == 0:
             return 0
         if t < 0:
             return 1
         if u > 0:
-            pu = self._p_x(x, s=s, t=u, depth=depth-1) #1-abs(depth))
+            pu = self._p_x(x, s=s, t=u, depth=depth-1) #depth-1)
             qt = self.get_q(x, s=s+u, t=t)
             if pu is not None and qt is not None:
                 self.blog(_Blog.q(x=x, s=s, t=t, u=u), '=',
                           _Blog.p(x=x, s=s, t=u), '*', _Blog.q(x=x, s=s+u, t=t),
                           depth=depth, rule="defer mortality")
                 return pu * qt        # (1) u_p_x * t_q_x+u
             qu = self.get_q(x, s=s, t=u)
@@ -170,42 +170,42 @@
                       depth=depth, rule='complement of mortality')
             return 1 - found  # (1) complement of q_x
         if depth <= 0:
             return None
         
         # (2a) inverse chain rule: p_x(t) = p_x-1(t+1) / p_x-1 
         found = self._p_x(x, s=s-1, t=t+1, depth=depth-1)
-        p = self._p_x(x, s=s-1, t=1, depth=1-abs(depth))
+        p = self._p_x(x, s=s-1, t=1, depth=depth-1)
         if found is not None and p is not None:
             self.blog(_Blog.p(x=x, s=s, t=t), '=',
                       _Blog.p(x=x, s=s-1, t=t+1), '/', _Blog.p(x=x, s=s-1, t=1),
                       depth=depth, rule="survival chain rule")
             return found / p
         
         # (2b) inverse chain rule: p_x(t) = p_x(t+1) / p_x+t 
         found = self._p_x(x, s=s, t=t+1, depth=depth-1)
-        p = self._p_x(x, s=s+t, t=1, depth=1-abs(depth))
+        p = self._p_x(x, s=s+t, t=1, depth=depth-1)
         if found is not None and p is not None:
             self.blog(_Blog.p(x=x, s=s, t=t), '=',
                       _Blog.p(x=x, s=s, t=t+1), '/', _Blog.p(x=x, s=s+t, t=1),
                       depth=depth, rule="survival chain rule")
             return found / p
         if t > 1:
             # (3a) chain rule: p_x(t) = p_x * p_x+1(t-1)
             found = self._p_x(x, s=s+1, t=t-1, depth=depth-1)
-            p = self._p_x(x, s=s, t=1, depth=1-abs(depth))
+            p = self._p_x(x, s=s, t=1, depth=depth-1)
             if found is not None and p is not None:
                 self.blog(_Blog.p(x=x, s=s, t=t), '=',
                           _Blog.p(x=x, s=s+1, t=t-1), '*', _Blog.p(x=x, s=s, t=1),
                           depth=depth, rule="survival chain rule")
                 return found * p
 
             # (3b) chain rule: p_x(t) = p_x+t-1 * p_x(t-1)
             found = self._p_x(x, s=s, t=t-1, depth=depth-1)
-            p = self._p_x(x, s=s+t-1, t=1, depth=1-abs(depth))
+            p = self._p_x(x, s=s+t-1, t=1, depth=depth-1)
             if found is not None and p is not None:
                 self.blog(_Blog.p(x=x, s=s, t=t), '=',
                           _Blog.p(x=x, s=s, t=t-1), '*', _Blog.p(x=x, s=s+t-1, t=1),
                           depth=depth, rule="survival chain rule")
                 return found * p
 
         if t == 1:
@@ -213,27 +213,27 @@
             if E is not None:
                 self.blog(_Blog.p(x=x, s=s, t=1), '=',
                           _Blog.E(x=x, s=s, t=1), "/v",
                           depth=depth, rule="one-year endowment")
                 return E / self.interest.v
 
             # (4a) annuity recursion: p_x = [a_x(t) - 1] / [v a_x+1(t-1)
-            for _t in [self.WHOLE, 2]:  # consider only WL and 2-term
+            for _t in [self.WHOLE, 2, 3]:  # consider only WL and 2-term
                 a = self._a_x(x, s=s, t=_t, depth=depth-1)
                 a1 = self._a_x(x, s=s+1, t=self.add_term(_t, -1), depth=depth-1)
                 if a is not None and a1 is not None:
                     self.blog(_Blog.p(x=x, s=s, t=1), '= [',
                               _Blog.a(x=x, s=s, t=_t), '- 1 ] / [ v *',
                               _Blog.a(x=x, s=s+1, t=_t-1), ']',
                               depth=depth, rule="annuity recursion")
                     return (a - 1) / (self.interest.v * a1)
 
             
             # (4b) insurance recursion: p_x = [v - A_x(t)] / [v (1 - A_x+1(t-1))]
-            for _t in [self.WHOLE, 2]:  # consider only WL and 2-term
+            for _t in [self.WHOLE, 2, 3]:  # consider only WL and 2-term
                 A = self._A_x(x, s=s, t=_t, depth=depth-1)
                 A1 = self._A_x(x, s=s+1, t=self.add_term(_t, -1), depth=depth-1)
                 if A is not None and A1 is not None:
                     self.blog(_Blog.p(x=x, s=s, t=1), '= [ v -',
                               _Blog.A(x=x, s=s, t=_t), '] / [v * [ 1 -',
                               _Blog.A(x=x, s=s+1, t=_t-1), ']]',
                               depth=depth, rule="insurance recursion")
@@ -254,44 +254,44 @@
         if p is not None:
             print(self.blog, end='')
         return p
 
     #
     # Formulas for Expected Future Lifetime: e_x
     #
-    def get_e(self, x: int, s: int = 0, t: int = Reserves._WHOLE, 
+    def get_e(self, x: int, s: int = 0, t: int = Reserves.WHOLE, 
               curtate: bool = False, moment: int = 1) -> float | None:
         """Get expected future lifetime from key-value store
 
         Args:
           x : age of selection
           s : years after selection
           t : limit of expected future lifetime
           curtate : curtate (True) or complete expectation (False)
           moment : first or second moment of expected future lifetime
         """
         key = self.db_key('e', x=x+s, t=t, curtate=curtate, moment=moment)
         return self.db.get(key, None)
 
-    def set_e(self, val: float, x: int, s: int = 0, t: int = Reserves._WHOLE, 
+    def set_e(self, val: float, x: int, s: int = 0, t: int = Reserves.WHOLE, 
               curtate: bool = False, moment: int = 1) -> "Recursion":
         """Set expected future lifetime e_[x]+s:t to given value
 
         Args:
           val : value to set
           x : age of selection
           s : years after selection
           t : limit of expected future lifetime
           curtate : curtate (True) or complete expectation (False)
           moment : first or second moment of expected future lifetime
         """
         return self.db_put(self.db_key('e', x=x+s, t=t, moment=moment,
                                        curtate=curtate), val)
 
-    def _e_x(self, x: int, s: int = 0, t: int = Reserves._WHOLE, 
+    def _e_x(self, x: int, s: int = 0, t: int = Reserves.WHOLE, 
             curtate: bool = False, moment: int = 1, 
             depth: int = 1) -> float | None:
         """Helper to compute from recursive and alternate formulas"""
         found = self.get_e(x, s=s, t=t, curtate=curtate, moment=moment)
         if found is not None:
             return found
         if depth <= 0:
@@ -302,17 +302,17 @@
                 if t == 1 and curtate:
                     self.blog(_Blog.e(x=x, s=s, t=1, curtate=curtate), '=',
                               _Blog.p(x=x, s=s, t=1),
                               #f"e_{x+s}:1",
                               depth=depth, rule='1-year curtate shortcut')
                     return p_t   # (1) if curtate and t=1: e_x:1 = p_x 
                 if t > 1:
-                    e = self._e_x(x, s=s, t=Reserves._WHOLE, curtate=curtate, 
+                    e = self._e_x(x, s=s, t=Reserves.WHOLE, curtate=curtate, 
                                   moment=1, depth=depth-1)
-                    e_t = self._e_x(x, s=s+t, t=Reserves._WHOLE, curtate=curtate,
+                    e_t = self._e_x(x, s=s+t, t=Reserves.WHOLE, curtate=curtate,
                                     moment=1, depth=depth-1)
                     if e is not None and e_t is not None and p_t is not None:
                         self.blog(_Blog.e(x=x, s=s, t=t), '=', _Blog.e(x=x, s=s), '-',
                                   _Blog.p(x=x, s=s), '*', _Blog.e(x=x, s=s+t),
                                   #"e_{x+s}:{t}: e_x - p_x e_x+t",
                                   depth=depth, rule="temporary lifetime")
                         return e - p_t*e_t  # (2) temporary = e_x - t_p_x e_x+t
@@ -337,15 +337,15 @@
                 self.blog(_Blog.e(x=x, s=s, t=t), '=', _Blog.e(x=x ,s=s, t=1), '+',
                           _Blog.p(x=x, s=s), '*', _Blog.e(x=x, s=s+1, t=t-1),
                           #f"backward: e_x:1 + p_x e_x+1:{t}",
                           depth=depth, rule='lifetime backward recursion')
                 return e + p * e_t # (4) backward: e_x:1 + p_x e_x+1:t-1
 
 
-    def e_x(self, x: int, s: int = 0, t: int = Reserves._WHOLE, 
+    def e_x(self, x: int, s: int = 0, t: int = Reserves.WHOLE, 
             curtate: bool = False, moment: int = 1) -> float:
         """Compute expected future lifetime by calling recursion helper
 
         Args:
           x : age of selection
           s : years after selection
           t : limited at t years
@@ -408,37 +408,37 @@
         if moment > 1:
             E = self._E_x(x, s=s, endowment=endowment, depth=depth)
             if E:  # (1) Shortcut: 2E_x = v E_x
                 self.blog(_Blog.E(x=x, s=s, t=t, moment=moment),
                           f"= v(t={t})"+_Blog.m(moment), '*', _Blog.E(x=x, s=s, t=t),
                           depth=depth, rule='moments of pure endowment')
                 return E * self.interest.v**(moment-1) 
-        p = self._p_x(x, s=s, t=t, depth=depth-1)  # 1-abs(depth))
+        p = self._p_x(x, s=s, t=t, depth=depth-1)  # depth-1)
         if p is not None:   # (2) E_x = p_x * v
             #msg = f"pure endowment {t}_E_{x+s} = {t}_p_{x+s} * v^{t}"
             self.blog(_Blog.E(x=x, s=s, t=t), '=', _Blog.p(x=x, s=s, t=t),
                       f"* v(t={t})"+_Blog.m(moment),
                       depth=depth, rule='pure endowment')
             return p * (endowment * self.interest.v_t(t))**moment
         if depth <= 0:
             return None
 
         At = self._A_x(x, s=s, t=t, moment=moment, b=endowment, endowment=0,
-                       depth=depth-1)  #1-abs(depth))
+                       depth=depth-1)  #depth-1)
         A = self._A_x(x, s=s, t=t, b=endowment, endowment=endowment, 
-                      moment=moment, depth=1-abs(depth))        
+                      moment=moment, depth=depth-1)        
         if A is not None and At is not None:
             self.blog(_Blog.E(x=x, s=s, t=t), '=',
                       _Blog.A(x=x, s=s, t=t, endowment=endowment), '-',
                       _Blog.A(x=x, s=s, t=t, endowment=0),
                       #f"endowment - term insurance = {t}_E_{x+s}",
                       depth=depth, rule='endowment insurance minus term')
             return A - At  # (3) endowment insurance - term (helpful SULT)
 
-        E = self._E_x(x, s=s, moment=moment, depth=1-abs(depth))
+        E = self._E_x(x, s=s, moment=moment, depth=depth-1)
         Et = self._E_x(x, s=s+1, t=t-1, moment=moment, depth=depth-1)
         if E is not None and Et is not None:
             msg = f"chain Rule: {t}_E_{x+s} = E_{x+s} * {t-1}_E_{x+s+1}"
             self.blog(_Blog.E(x=x, s=s, t=t, moment=moment), '=',
                       _Blog.E(x=x, s=s, t=1, moment=moment), '*',
                       _Blog.E(x=x, s=s+1, t=t-1, moment=moment), '*',
                       _Blog.m(moment, endow=endowment),
@@ -455,30 +455,30 @@
           t : term of pure endowment
           endowment : amount of pure endowment
           moment : compute first or second moment
         """
         self.blog = _Blog("Pure Endowment",
                          _Blog.E(x=x, s=s, t=t, moment=moment, endowment=endowment),
                          levels=self.maxdepth)
-        if moment == self._VARIANCE:  # Bernoulli shortcut for variance
+        if moment == self.VARIANCE:  # Bernoulli shortcut for variance
             found = self.get_E(x, s=s, t=t, endowment=endowment, moment=moment)
             if found is not None:
                 return found
             t_p_x = self.p_x(x, s=s, t=t)
             return (endowment * self.interest.v_t(t))**2 * t_p_x * (1-t_p_x)
         found = self._E_x(x, s=s, t=t, endowment=endowment, moment=moment,
                           depth=self.maxdepth)
         if found is not None:
             print(self.blog, end='')
             return found
 
     #
     # Formulas for Increasing Insurance: IA_x:t
     #
-    def get_IA(self, x: int, s: int = 0, t: int = Reserves._WHOLE,
+    def get_IA(self, x: int, s: int = 0, t: int = Reserves.WHOLE,
                b: int = 1, discrete: bool = True) -> float | None:
         """Get increasing insurance from key-value store
 
         Args:
           x : age of selection
           s : years after selection
           t : term of increasing insurance
@@ -486,15 +486,15 @@
           discrete : discrete or continuous increasing insurance
         """
         key = self.db_key('IA', x=x+s, t=t, discrete=discrete)
         val = self.db.get(key, None)
         if val is not None:
             return val * b   # stored with benefit=1
 
-    def set_IA(self, val: float, x: int, s: int = 0, t: int = Reserves._WHOLE,
+    def set_IA(self, val: float, x: int, s: int = 0, t: int = Reserves.WHOLE,
                b: int = 1, discrete: bool = True) -> "Recursion":
         """Set increasing insurance IA_[x]+s:t to given value
 
         Args:
           val : value to set
           x : age of selection
           s : years after selection
@@ -502,15 +502,15 @@
           b : benefit after year 1
           discrete : discrete or continuous increasing insurance
         """
         val /= b   # store with benefit=1
         return self.db_put(self.db_key('IA', x=x+s, t=t, 
                                        discrete=discrete), val)
 
-    def _IA_x(self, x: int, s: int = 0, t: int = Reserves._WHOLE, b: int = 1,
+    def _IA_x(self, x: int, s: int = 0, t: int = Reserves.WHOLE, b: int = 1,
               discrete: bool = True, depth: int = 1) -> float | None:
         """Helper to compute from recursive and alternate formulas"""
         if t == 0:
             return 0
         found = self.get_IA(x=x, s=s, t=t, b=b, discrete=discrete)
         if found is not None:
             return found
@@ -526,23 +526,23 @@
                           _Blog.A(x=x, s=s, t=t), '-', _Blog.DA(x=x, s=s, t=t),
                     #f"identity IA_{x+s}:{t}: ({n})A - DA",
                           depth=depth, rule='varying insurance identity')
                 return A * n - DA  # (1) Identity with term and decreasing
 
         A = self._A_x(x=x, s=s, t=1, b=b, discrete=discrete, depth=depth-1)
         IA = self._IA_x(x=x, s=s+1, t=self.add_term(t, -1), b=b, depth=depth-1)
-        p = self._p_x(x, s=s, t=1, depth=1-abs(depth))   # FIXED t=1
+        p = self._p_x(x, s=s, t=1, depth=depth-1)   # FIXED t=1
         if A is not None and IA is not None and p is not None:
             self.blog(_Blog.IA(x=x, s=s, t=t), '=', _Blog.A(x=x, s=s, t=t), '+',
                       _Blog.p(x=x, s=s), f"* v(t={t}) *", _Blog.IA(x=x, s=s+1, t=t-1),
                       #f"backward IA_{x+s}:{t}: A + IA_{x+s+1}:{t-1}",
                       depth=depth, rule='backward recursion')
             return A + p * self.interest.v * IA  # (2) backward recursion
 
-    def increasing_insurance(self, x: int, s: int = 0, t: int = Reserves._WHOLE,
+    def increasing_insurance(self, x: int, s: int = 0, t: int = Reserves.WHOLE,
                              b: int = 1, discrete: bool = True) -> float:
         """Compute increasing insurance with recursive helper
 
         Args:
           x : age of selection
           s : years after selection
           t : term of insurance
@@ -560,15 +560,15 @@
         if IA is not None:
             print(self.blog, end='')
             return IA
 
     #
     # Formulas for Decreasing insurance: DA_x:t
     #
-    def get_DA(self, x: int, s: int = 0, t: int = Reserves._WHOLE,
+    def get_DA(self, x: int, s: int = 0, t: int = Reserves.WHOLE,
                b: int = 1, discrete: bool = True) -> float | None:
         """Get decreasing insurance from key-value store
 
         Args:
           x : age of selection
           s : years after selection
           t : term of decreasing insurance
@@ -576,15 +576,15 @@
           discrete : discrete or continuous decreasing insurance
         """
         key = self.db_key('DA', x=x+s, t=t, discrete=discrete)
         val = self.db.get(key, None)
         if val is not None:
             return val * b   # stored with benefit=1
 
-    def set_DA(self, val: float, x: int, s: int = 0, t: int = Reserves._WHOLE,
+    def set_DA(self, val: float, x: int, s: int = 0, t: int = Reserves.WHOLE,
                b: int = 1, discrete: bool = True) -> "Recursion":
         """Set decreasing insurance DA_[x]+s:t to given value
 
         Args:
           val : value to set
           x : age of selection
           s : years after selection
@@ -592,15 +592,15 @@
           b : benefit after year 1
           discrete : discrete or continuous decreasing insurance
         """
         val /= b     # store with benefit=1
         return self.db_put(self.db_key('DA', x=x+s, t=t, 
                                        discrete=discrete), val)
 
-    def _DA_x(self, x: int, s: int = 0, t: int = Reserves._WHOLE, b: int = 1,
+    def _DA_x(self, x: int, s: int = 0, t: int = Reserves.WHOLE, b: int = 1,
               discrete: bool = True, depth: int = 1) -> float | None:
         """Helper to compute from recursive and alternate formulas"""
         found = self.get_DA(x=x, s=s, t=t, discrete=discrete)
         if found is not None:
             return found
         if t == 0:
             return 0
@@ -615,23 +615,23 @@
         if A is not None and IA is not None:
             self.blog(_Blog.DA(x=x, s=s, t=t), f'= {n}',
                       _Blog.A(x=x, s=s, t=t), '-', _Blog.IA(x=x, s=s, t=t),
                       depth=depth, rule='varying insurance identity')
             return A * n - IA  # (1) identity with term and decreasing
 
         DA = self._IA_x(x=x, s=s+1, t=self.add_term(t, -1), b=b, depth=depth-1)
-        p = self._p_x(x, s=s, depth=1-abs(depth))
+        p = self._p_x(x, s=s, depth=depth-1)
         if DA is not None and p is not None:
             #msg = f"backward DA_{x+s}:{t}: v(t q_{x+s} + p_{x+s} DA_{x+s+1}:{t-1})"
             self.blog(_Blog.DA(x=x, s=s, t=t), f"= v(t={t}) * t *", _Blog.q(x=x, s=s),
                       '+', _Blog.p(x=x, s=s), '*', _Blog.DA(x=x, s=s+1, t=t-1),
                       depth=depth, rule='backward recursion')
             return self.interest.v * ((1-p)*t + p*DA)  # (2) backward recursion
 
-    def decreasing_insurance(self, x: int, s: int = 0, t: int = Reserves._WHOLE,
+    def decreasing_insurance(self, x: int, s: int = 0, t: int = Reserves.WHOLE,
                              b: int = 1, discrete: bool = True) -> float:
         """Compute decreasing insurance by calling recursive helper first
 
         Args:
           x : age of selection
           s : years after selection
           t : term of insurance
@@ -651,15 +651,15 @@
         if A is not None:
             print(self.blog, end='')
             return A
 
     #
     # Formulas for Insurance: A_x:t
     #
-    def get_A(self, x: int, s: int = 0, u: int = 0, t: int = Reserves._WHOLE,
+    def get_A(self, x: int, s: int = 0, u: int = 0, t: int = Reserves.WHOLE,
               b: int = 1, moment: int = 1, endowment: int = 0, 
               discrete: bool = True) -> float | None:
         """Get insurance from key-value store
 
         Args:
           x : age of selection
           s : years after selection
@@ -682,15 +682,15 @@
         key = self.db_key('A', x=x+s, u=u, t=t, moment=moment, 
                           endowment=endowment, discrete=discrete)
         val = self.db.get(key, None)
         if val is not None:
             return val * scale   # stored with benefit=1
 
 
-    def set_A(self, val: float, x: int, s: int = 0, t: int = Reserves._WHOLE,
+    def set_A(self, val: float, x: int, s: int = 0, t: int = Reserves.WHOLE,
               u: int = 0, b: int = 1, moment: int = 1, endowment: int = 0, 
               discrete: bool = True) -> "Recursion":
         """Set insurance u|_A_[x]+s:t to given value
 
         Args:
           val : value to set
           x : age of selection
@@ -711,15 +711,15 @@
             if b != 1:
                 val /= b
                 endowment /= b
         return self.db_put(self.db_key('A', x=x+s, t=t, u=u,
                                        moment=moment, endowment=endowment, 
                                        discrete=discrete), val)
 
-    def _A_x(self, x: int, s: int = 0, t: int = Reserves._WHOLE, u: int = 0,
+    def _A_x(self, x: int, s: int = 0, t: int = Reserves.WHOLE, u: int = 0,
              b: int = 1, discrete: bool = True, endowment: int = 0,
              moment: int = 1, depth: int = 1) -> float | None:
         """Helper to compute from recursive and alternate formulas"""
         
         if endowment == b and t == 1 and discrete: # 1-year endow ins
             return (self.interest.v_t(1) * endowment)**moment
         found = self.get_A(x=x, s=s, t=t, b=b, u=u, discrete=discrete, 
@@ -751,29 +751,29 @@
                           _Blog.E(x=x, s=s-1, moment=moment),
                           depth=depth, rule='forward recursion')
                 return A / E
             return None
 
         if endowment > 0: # (2a) endowment = term + E_x * endowment
             A = self._A_x(x=x, s=s, t=t, b=b, discrete=discrete, 
-                          moment=moment, depth=1-abs(depth))
+                          moment=moment, depth=depth-1)
             E_x = self._E_x(x=x, s=s, t=t, moment=moment, 
-                            endowment=endowment, depth=1-abs(depth))
+                            endowment=endowment, depth=depth-1)
             if A is not None and E_x is not None:
                 # f"term + pure insurance = A_{x+s}:{t}",
                 self.blog(_Blog.A(x=x, s=s, t=t, endowment=endowment, moment=moment),
                           '=', _Blog.A(x=x, s=s, t=t, moment=moment), '+',
                           _Blog.E(x=x, s=s, t=t, endowment=endowment, moment=moment),
                           depth=depth, rule='term plus pure endowment')
                 return A + E_x
         else:             # (2b) term = endowment insurance - E_x * endowment
             A = self._A_x(x=x, s=s, t=t, b=b, discrete=discrete, 
-                          moment=moment, endowment=b, depth=1-abs(depth))
+                          moment=moment, endowment=b, depth=depth-1)
             E_x = self._E_x(x=x, s=s, t=t, moment=moment, endowment=b, 
-                            depth=1-abs(depth))
+                            depth=depth-1)
             if A is not None and E_x is not None:
                 #msg = f"endowment insurance - pure endowment = A_{x+s}^1:{t}"
                 self.blog(_Blog.A(x=x, s=s, t=t, moment=moment), '=',
                           _Blog.A(x=x, s=s, t=t, moment=moment, endowment=b), '-',
                           _Blog.E(x=x, s=s, t=t, endowment=b, moment=moment),
                           depth=depth, rule='endowment insurance - pure')
                 return A - E_x
@@ -798,29 +798,29 @@
                           depth=depth, rule='one-year discrete insurance')
                 return (self.interest.v**moment 
                         * ((1 - p) * b**moment + p * endowment**moment))
     
         A = self._A_x(x=x, s=s+1, t=self.add_term(t, -1), b=b, 
                       discrete=discrete, moment=moment,
                       endowment=endowment, depth=depth-1)
-        p = self._p_x(x, s=s, t=1, depth=1-abs(depth)) # (4) backward recursion
+        p = self._p_x(x, s=s, t=1, depth=depth-1) # (4) backward recursion
         if A is not None and p is not None:
             self.blog(_Blog.A(x=x, s=s, t=t, b=b, moment=moment),
                       f"= v"+_Blog.m(moment), "* [",
                       _Blog.q(x=x,s=s), f"* b"+_Blog.m(moment), "+",
                       _Blog.p(x=x, s=s), '*',
                       _Blog.A(x=x, s=s+1, t=t-1, b=b, moment=moment), ']',
                       #f"backward: A_{x+s} = qv + pvA_{x+s+1}",
                       depth=depth, rule='backward recursion')
             return self.interest.v_t(1)**moment * ((1 - p)*b**moment + p*A)
 
         A = self._A_x(x=x, s=s-1, t=self.add_term(t, 1), b=b, u=u, 
                       discrete=discrete, moment=moment, 
                       endowment=endowment, depth=depth-1)
-        p = self._p_x(x, s=s-1, t=1, depth=1-abs(depth))
+        p = self._p_x(x, s=s-1, t=1, depth=depth-1)
         if A is not None and p is not None:  # (5) forward recursion
             self.blog(_Blog.A(x=x, s=s, t=t, b=b, moment=moment), '= [',
                       _Blog.A(x=x, s=s-1, t=t+1, b=b, moment=moment),
                       f"/v"+_Blog.m(moment), "-", _Blog.q(x=x,s=s),
                       f"* b"+_Blog.m(moment), "] /", _Blog.p(x=x, s=s),
                       #f"forward: A_{x+s} = (A_{x+s-1}/v - q) / p",
                       depth=depth, rule='forward recursion')
@@ -834,15 +834,15 @@
           x : age of selection
           s : years after selection
           b : amount of benefit
           moment : compute first or second moment
           discrete : benefit paid year-end (True) or moment of death (False)
         """
         self.blog = _Blog("Whole Life Insurance",
-                         _Blog.A(x=x, s=s, t=Reserves._WHOLE, b=b, u=0,
+                         _Blog.A(x=x, s=s, t=Reserves.WHOLE, b=b, u=0,
                                 endowment=0, moment=moment, discrete=discrete),
                          levels=self.maxdepth)
         found = self._A_x(x, s=s, b=b, moment=moment, discrete=discrete,
                           depth=self.maxdepth)
         if found is not None:
             print(self.blog, end='')
             return found
@@ -869,29 +869,29 @@
           t : term of insurance
           b : amount of benefit
           moment : compute first or second moment
           discrete : benefit paid year-end (True) or moment of death (False)
         """
         self.blog = _Blog("Term Insurance",
                          _Blog.A(x=x, s=s, t=t, b=b, u=0, discrete=discrete,
-                                endowment=0, moment=moment),
+                                 endowment=0, moment=moment),
                          levels=self.maxdepth)
         found = self._A_x(x, s=s, b=b, t=t, moment=moment, discrete=discrete,
                           depth=self.maxdepth)
         if found is not None:
             print(self.blog, end='')
             return found
         A = super().term_insurance(x, s=s, b=b, t=t, discrete=discrete,
                                    moment=moment)
         if A is not None:
             print(self.blog, end='')
             return A
 
     def deferred_insurance(self, x: int, s: int = 0, b: int = 1, u: int = 0, 
-                           t: int = Reserves._WHOLE, moment: int = 1, 
+                           t: int = Reserves.WHOLE, moment: int = 1, 
                            discrete: bool = True) -> float:
         """Compute deferred life insurance u|A_x:t^1 by calling recursion helper: """
         self.blog = _Blog("Deferred Insurance",
                          _Blog.A(x=x, s=s, t=t, b=b, u=u, discrete=discrete,
                                 endowment=0, moment=moment),
                          levels=self.maxdepth)
         A = self.get_A(x=x, s=s, t=t, b=b, u=u, discrete=discrete, 
@@ -932,15 +932,15 @@
         if A is not None:
             print(self.blog, end='')
             return A
 
     #
     # Formulas for Annuties: a_x:t
     #
-    def get_a(self, x: int, s: int = 0, u: int = 0, t: int = Reserves._WHOLE,
+    def get_a(self, x: int, s: int = 0, u: int = 0, t: int = Reserves.WHOLE,
               b: int = 1, variance: bool = False, 
               discrete: bool = True) -> float | None:
         """Get annuity from key-value store
 
         Args:
           x : age of selection
           s : years after selection
@@ -952,15 +952,15 @@
         """
         key = self.db_key('a', x=x+s, u=u, t=t, 
                           variance=variance, discrete=discrete)
         val = self.db.get(key, None)
         if val is not None:
             return val * b    # stored with benefit=1
 
-    def set_a(self, val: float, x: int, s: int = 0, t: int = Reserves._WHOLE,
+    def set_a(self, val: float, x: int, s: int = 0, t: int = Reserves.WHOLE,
               u: int = 0, b: int = 1, variance: bool = False, 
               discrete: bool = True) -> "Recursion":
         """Set annuity u|_a_[x]+s:t to given value
 
         Args:
           val : value to set
           x : age of selection
@@ -971,15 +971,15 @@
           discrete : whether annuity due (True) or continuous (False)
           variance : whether first moment (False) or variance (True)
         """
         val /= b    # store with benefit=1
         return self.db_put(self.db_key('a', x=x+s, t=t, u=u, 
                            variance=variance, discrete=discrete), val)
 
-    def _a_x(self, x: int, s: int = 0, t: int = Reserves._WHOLE, 
+    def _a_x(self, x: int, s: int = 0, t: int = Reserves.WHOLE, 
              u: int = 0, b: int = 1, discrete: bool = True, 
              variance: bool = False, depth: int = 1) -> float | None:
         """Helper to compute from recursive and alternate formulas"""
         if t == 1 and not u and discrete:
             self.blog(_Blog.a(x=x, s=s, t=1, discrete=discrete), '= 1',
                       depth=depth, rule='one-year discrete annuity')
             return b 
@@ -1050,15 +1050,15 @@
           x : age of selection
           s : years after selection
           b : annuity benefit amount
           variance (bool): return EPV (True) or variance (False)
           discrete : annuity due (True) or continuous (False)
         """
         self.blog = _Blog("Whole Life Annuity",
-                         _Blog.a(x=x, s=s, t=Reserves._WHOLE, b=b, u=0,
+                         _Blog.a(x=x, s=s, t=Reserves.WHOLE, b=b, u=0,
                                 discrete=discrete, variance=False),
                          levels=self.maxdepth)
         found = self._a_x(x, s=s, b=b, variance=variance, 
                           discrete=discrete, depth=self.maxdepth)
         if found is not None:
             print(self.blog, end='')
             return found
@@ -1071,15 +1071,15 @@
                 return self.annuity_twin(A=A, discrete=discrete)
         a = super().whole_life_annuity(x, s=s, b=b, discrete=discrete,
                                        variance=variance)
         if a is not None:
             print(self.blog, end='') 
             return a
 
-    def temporary_annuity(self, x: int, s: int = 0, t: int = Reserves._WHOLE,
+    def temporary_annuity(self, x: int, s: int = 0, t: int = Reserves.WHOLE,
                           b: int = 1, variance: bool = False,
                           discrete: bool = True) -> float:
         """Compute temporary annuity a_x:t by calling recursion then twin first
 
         Args:
           x : age of selection
           s : years after selection
@@ -1109,15 +1109,15 @@
                 return self.annuity_twin(A=A, discrete=discrete)
         a = super().temporary_annuity(x, s=s, b=b, t=t, discrete=discrete,
                                       variance=variance)
         if a is not None:
             print(self.blog, end='')
             return a
 
-    def deferred_annuity(self, x: int, s: int = 0, t: int = Reserves._WHOLE,
+    def deferred_annuity(self, x: int, s: int = 0, t: int = Reserves.WHOLE,
                          u: int = 0, b: int = 1, discrete: bool = True) -> float:
         """Compute deferred annuity u|a_x:t by calling recursion first
 
         Args:
           x : age of selection
           s : years after selection
           u : years deferred
@@ -1194,15 +1194,15 @@
         out = []
         if t != 1:
             out.append(f"t={t}")
         return f"p_{x+s}" + "("*bool(out) + ",".join(out) + ")"*bool(out)
 
 
     @staticmethod
-    def e(x: int, s: int = 0, t: int = Reserves._WHOLE, curtate: bool = False,
+    def e(x: int, s: int = 0, t: int = Reserves.WHOLE, curtate: bool = False,
           moment: int = 1) -> str:
         """Return string representation of expected future lifetime e_x term"""
         out = []
         if t >= 0:
             out.append(f"t={t}")
         if moment != 1:
             out.append(f"mom={moment}")
@@ -1218,25 +1218,25 @@
         if moment != 1:
             out.append(f"mom={moment}")
         if endowment != 1:
             out.append(f"endow={endowment}")
         return f"E_{x+s}" + "("*bool(out) + ",".join(out) + ")"*bool(out)
     
     @staticmethod
-    def IA(x: int, s: int = 0, t: int = Reserves._WHOLE, b: int = 1,
+    def IA(x: int, s: int = 0, t: int = Reserves.WHOLE, b: int = 1,
            discrete: bool = True) -> str:
         """Return string representation of increasing insurance IA_x term"""
         out = []
         out.append(f"t={t if t >= 0 else 'WL'}")  # term or whole life
         if b != 1:
             out.append(f"b={b}")
         return f"IA_{x+s}" + "("*bool(out) + ",".join(out) + ")"*bool(out)
 
     @staticmethod
-    def DA(x: int, s: int = 0, t: int = Reserves._WHOLE, b: int = 1,
+    def DA(x: int, s: int = 0, t: int = Reserves.WHOLE, b: int = 1,
            discrete: bool = True) -> str:
         """Return string representation of decreasing insurance DA_x term"""
         out = []
         out.append(f"t={t if t >= 0 else 'WL'}")  # term or whole life
         if b != 1:
             out.append(f"b={b}")
         return f"DA_{x+s}" + "("*bool(out) + ",".join(out) + ")"*bool(out)
@@ -1281,32 +1281,24 @@
         return ("(" + "*".join(args) + ")")+out if args else "0"
     
 
 if __name__ == "__main__":
     from actuarialmath.constantforce import ConstantForce
     from actuarialmath.policyvalues import Contract
 
-    print("SOA Question 6.10:  ")
+    print("SOA Question 6.10: (D) 0.91")
     x = 0
-    life = Recursion(verbose=True, depth=5).set_interest(i=0.06).set_p(0.975, x=x)
-    a = 152.85/56.05  # solve a_x:3, given net premium and benefit APV
-    life.set_a(a, x=x, t=3)
-    #life.set_A(152.85, x=x, t=3, b=1000)
-
-    p1 = life.p_x(x=x+1)   # buggy
-#    p2 = life.p_x(x=x+2)
-    life.set_p(p1, x=x+1)
-
-    def fun(p): 
-        return life.set_p(p, x=x+2).term_insurance(x=x, t=3, b=1000)
-    p = life.solve(fun, target=152.85, grid=0.975)  # solve p_x+2, given A_x:3
-    print(p)
-
+    life = Recursion().set_interest(i=0.06)\
+                      .set_p(0.975, x=x)\
+                      .set_a(152.85/56.05, x=x, t=3)\
+                      .set_A(152.85, x=x, t=3, b=1000)
+    print(life.p_x(x=x+2))
     #isclose(0.91, p, question="Q6.10")
 
+    raise Exception
     
     print("AMLCR2 Exercise 2.6")
     x = 0
     life = Recursion(depth=3).set_interest(i=0.06)\
                              .set_p(0.99, x=x)\
                              .set_p(0.985, x=x+1)\
                              .set_p(0.95, x=x+1, t=3)\
```

### Comparing `actuarialmath-0.0.8/src/actuarialmath/reserves.py` & `actuarialmath-0.0.9/src/actuarialmath/reserves.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 MIT License. Copyright 2022-2023 Terence Lim
 """
 import math
 import numpy as np
 import pandas as pd
 import matplotlib.pyplot as plt
 from typing import Callable, Dict, Any
-from actuarialmath.policyvalues import PolicyValues, Contract
+from actuarialmath import PolicyValues, Contract
 
 class Reserves(PolicyValues):
     """Compute recursive, interim and modified reserves"""
     
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
         self._reserves = {'V': {}}
@@ -233,15 +233,15 @@
             V -= self.q_r(x, s=s, t=r) * benefit * self.interest.v_t(1-r)
         V /= self.p_r(x, s=s, t=r)
         return V
 
     #
     # Full Preliminary Term (FPT) modified reserves
     #
-    def FPT_premium(self, x: int, s: int = 0, n: int = PolicyValues._WHOLE, 
+    def FPT_premium(self, x: int, s: int = 0, n: int = PolicyValues.WHOLE, 
                     b: int = 1, first: bool = False) -> float:
         """Initial or renewal Full Preliminary Term premiums
 
         Args:
           x : age of selection
           s : years after selection
           n : term of insurance
@@ -250,15 +250,15 @@
         """
         if first:
             return self.net_premium(x, s=s, b=b, t=1)
         else:
             return self.net_premium(x, s=s+1, b=b, t=self.add_term(n, -1))
 
     def FPT_policy_value(self, x: int, s: int = 0, t: int = 0, b: int = 1,
-                         n: int = PolicyValues._WHOLE,
+                         n: int = PolicyValues.WHOLE,
                          endowment: int = 0, discrete: bool = True) -> float:
         """Compute Full Preliminary Term policy value at time t
 
         Args:
           x : age of selection
           s : years after selection
           n : term of insurance
```

### Comparing `actuarialmath-0.0.8/src/actuarialmath/selectlife.py` & `actuarialmath-0.0.9/src/actuarialmath/selectlife.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 MIT License. Copyright 2022-2023 Terence Lim
 """
 from typing import Dict, List
 import math
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
-from actuarialmath.lifetable import LifeTable
+from actuarialmath import LifeTable
 
 class SelectLife(LifeTable):
     """Calculate select life table, and iteratively fill in missing values
 
     Args:
       periods : number of select period years
       verbose : whether to echo update steps
@@ -319,15 +319,15 @@
           x : age of selection
           s : years after selection
           u : survives u years, then
           t : dies within next t years
         """
         return (1. - self.p_x(x, s=s + u, t=t)) * self.p_x(x, s=s, t=u)
 
-    def e_x(self, x: int, s: int = 0, t: int = LifeTable._WHOLE,
+    def e_x(self, x: int, s: int = 0, t: int = LifeTable.WHOLE,
             curtate: int = True) -> float:
         """Returns expected life time computed from select table
 
         Args:
           x : age of selection
           s : years after selection
           t : limit of expected future lifetime
```

### Comparing `actuarialmath-0.0.8/src/actuarialmath/sult.py` & `actuarialmath-0.0.9/src/actuarialmath/sult.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 MIT License. Copyright 2022-2023 Terence Lim
 """
 import math
 import numpy as np
 import pandas as pd
 from typing import Dict, Callable
-from actuarialmath.lifetable import LifeTable
+from actuarialmath import LifeTable
 
 # Makeham's Law parameters from SOA’s Excel Workbook for FAM-L Tables
 _A, _B, _c = 0.00022, 0.0000027, 1.124
 def _faml_sult(x, t: float) -> float:
     return math.exp(-_A*t - (_B*_c**x*(_c**t - 1)) / math.log(_c))
 
 class SULT(LifeTable):
```

### Comparing `actuarialmath-0.0.8/src/actuarialmath/survival.py` & `actuarialmath-0.0.9/src/actuarialmath/survival.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Survival models - Computes survival and mortality functions
 
 MIT License. Copyright (c) 2022-2023 Terence Lim
 """
 from typing import Callable, Tuple, Any, List
 import math
 import numpy as np
-from actuarialmath.life import Life
+from actuarialmath import Life
 
 class Survival(Life):
     """Set and derive basic survival and mortality functions"""
     _RADIX = 100000   # default initial number of lives in life table
 
     def set_survival(self,
                      S: Callable[[int,float,float], float] | None = None,
```

### Comparing `actuarialmath-0.0.8/src/actuarialmath/udd.py` & `actuarialmath-0.0.9/src/actuarialmath/udd.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """UDD - 1/mthly insurance and annuities with uniform distribution of deaths
 
 MIT License. Copyright 2022-2023 Terence Lim
 """
 import pandas as pd
-from actuarialmath.life import Interest
-from actuarialmath.annuity import Annuity
-from actuarialmath.mthly import Mthly
+from actuarialmath import Interest
+from actuarialmath import Annuity
+from actuarialmath import Mthly
 
 class UDD(Mthly):
     """1/mthly shortcuts with UDD assumption
 
     Args:
       m : number of payments per year
       life : original fractional survival and mortality functions
```

### Comparing `actuarialmath-0.0.8/src/actuarialmath/woolhouse.py` & `actuarialmath-0.0.9/src/actuarialmath/woolhouse.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Woolhouse - 1/mthly insurance and annuities with Woolhouse's approximation
 
 MIT License. Copyright 2022-2023 Terence Lim
 """
 import math
 from typing import Callable
-from actuarialmath.mthly import Mthly
-from actuarialmath.annuity import Annuity
+from actuarialmath import Mthly
+from actuarialmath import Annuity
 
 class Woolhouse(Mthly):
     """1/m'thly shortcuts with Woolhouse approximation
 
     Args:
       m : number of payments per year
       life : original fractional survival and mortality functions
```

### Comparing `actuarialmath-0.0.8/src/actuarialmath.egg-info/PKG-INFO` & `actuarialmath-0.0.9/src/actuarialmath.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: actuarialmath
-Version: 0.0.8
+Version: 0.0.9
 Summary: A package for actuarial math and life contingent risks
 Author: Terence Lim
-Project-URL: Homepage, https://terence-lim.github.io/actuarialmath-tutorial
+Project-URL: Homepage, https://terence-lim.github.io/actuarialmath-guide
 Project-URL: Bug Tracker, https://github.com/terence-lim/actuarialmath/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/x-rst
 License-File: LICENSE
@@ -27,66 +27,65 @@
    - Basic interest theory and probability laws
 
    - Survival functions, expected future lifetimes and fractional ages
 
    - Insurance, annuity, premiums, policy values, and reserves calculations
 
 
-2. Specify and load a particular form of assumptions
+2. Adjust results for
 
-   - Life table, select life table, or standard ultimate life table
-
-   - Mortality laws, such as constant force of maturity, beta and uniform distributions, or Makeham's and Gompertz's laws
+   - Extra mortality risks
 
-   - Recursion inputs
+   - 1/mthly payment frequency using UDD or Woolhouse approaches
 
-3. Adjust results for
+3. Specify and load a particular form of assumptions
 
-   - Extra mortality risks
+   - Life table, select life table, or standard ultimate life table
 
-   - 1/mthly payment frequency using UDD or Woolhouse approaches
+   - Mortality laws, such as constant force of maturity, beta and uniform distributions, or Makeham's and Gompertz's laws
 
+   - Recursion inputs
+    
+     
 Quick Start
 -----------
 
 1. ``pip install actuarialmath``
    
    - also requires `numpy`, `scipy`, `matplotlib` and `pandas`.
      
 2. Start Python (version >= 3.10) or Jupyter-notebook
 
    - Select a suitable subclass to initialize with your actuarial assumptions, such as `MortalityLaws` (or a special law like `ConstantForce`), `LifeTable`, `SULT`, `SelectLife` or `Recursion`.
       
    - Call appropriate methods to compute intermediate or final results, or to `solve` parameter values implicitly.
 
-   - If needed, adjust the answers with `ExtraRisk` or `Mthly` (or its `UDD` or `Woolhouse`) classes.
+   - Adjust the answers with `ExtraRisk` or `Mthly` (or its `UDD` or `Woolhouse`) classes.
 
 Examples
 --------
 
 ::
 
   # SOA FAM-L sample question 5.7
-  from actuarialmath.recursion import Recursion
-  from actuarialmath.woolhouse import Woolhouse
+  from actuarialmath.recursion import Recursion, Woolhouse
   # initialize Recursion class with actuarial inputs
   life = Recursion().set_interest(i=0.04)\
                     .set_A(0.188, x=35)\
                     .set_A(0.498, x=65)\
                     .set_p(0.883, x=35, t=30)
   # modfy the standard results with Woolhouse mthly approximation
   mthly = Woolhouse(m=2, life=life, three_term=False)
   # compute the desired temporary annuity value
   print(1000 * mthly.temporary_annuity(35, t=30)) #   solution = 17376.7
 
 ::
 
   # SOA FAM-L sample question 7.20
-  from actuarialmath.sult import SULT   # use Standard Ultimate Life Table
-  from actuarialmath.policyvalues import Contract
+  from actuarialmath.sult import SULT, Contract
   life = SULT()
   # compute the required FPT policy value
   S = life.FPT_policy_value(35, t=1, b=1000)  # is always 0 in year 1!
   # input the given policy contract terms
   contract = Contract(benefit=1000,
                       initial_premium=.3,
                       initial_policy=300,
@@ -99,13 +98,13 @@
   print(R-S)   # solution = -277.19
 
 Resources
 ---------
 
 1. `Colab <https://colab.research.google.com/drive/1TcNr1x5HbT2fF3iFMYGXdN_cvRKiSua4?usp=sharing>`_ or `Jupyter notebook <https://terence-lim.github.io/notes/faml.ipynb>`_, to solve all sample SOA FAM-L exam questions
 
-2. `Online tutorial <https://terence-lim.github.io/actuarialmath-tutorial/>`_, or `download pdf <https://terence-lim.github.io/notes/actuarialmath-tutorial.pdf>`_
+2. `User Guide <https://terence-lim.github.io/actuarialmath-guide/>`_, or `download pdf <https://terence-lim.github.io/notes/actuarialmath-guide.pdf>`_
 
 3. `Code documentation <https://actuarialmath.readthedocs.io/en/latest/>`_
 
 4. `Github repo <https://github.com/terence-lim/actuarialmath.git>`_ and `issues <https://github.com/terence-lim/actuarialmath/issues>`_
```

### Comparing `actuarialmath-0.0.8/src/actuarialmath.egg-info/SOURCES.txt` & `actuarialmath-0.0.9/src/actuarialmath.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -24,8 +24,9 @@
 src/actuarialmath/survival.py
 src/actuarialmath/udd.py
 src/actuarialmath/woolhouse.py
 src/actuarialmath.egg-info/PKG-INFO
 src/actuarialmath.egg-info/SOURCES.txt
 src/actuarialmath.egg-info/dependency_links.txt
 src/actuarialmath.egg-info/requires.txt
-src/actuarialmath.egg-info/top_level.txt
+src/actuarialmath.egg-info/top_level.txt
+tests/test_changes.py
```

