# Comparing `tmp/decoratory-0.1.5.6.tar.gz` & `tmp/decoratory-0.9.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "decoratory-0.1.5.6.tar", last modified: Wed Jun 21 11:44:41 2023, max compression
+gzip compressed data, was "decoratory-0.9.0.6.tar", last modified: Fri Jun 23 07:10:45 2023, max compression
```

## Comparing `decoratory-0.1.5.6.tar` & `decoratory-0.9.0.6.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-06-21 11:44:41.931054 decoratory-0.1.5.6/
--rw-rw-rw-   0        0        0     2550 2023-06-21 06:11:12.000000 decoratory-0.1.5.6/License.txt
--rw-rw-rw-   0        0        0    46030 2023-06-21 11:44:41.931054 decoratory-0.1.5.6/PKG-INFO
--rw-rw-rw-   0        0        0    44405 2023-06-21 10:46:42.000000 decoratory-0.1.5.6/Readme.rst
--rw-rw-rw-   0        0        0        0 2023-06-21 06:11:12.000000 decoratory-0.1.5.6/Requirements.txt
-drwxrwxrwx   0        0        0        0 2023-06-21 11:44:41.830328 decoratory-0.1.5.6/Sources/
-drwxrwxrwx   0        0        0        0 2023-06-21 11:44:41.890770 decoratory-0.1.5.6/Sources/decoratory/
--rw-rw-rw-   0        0        0      249 2023-06-07 18:32:49.000000 decoratory-0.1.5.6/Sources/decoratory/__init__.py
--rw-rw-rw-   0        0        0     5466 2023-06-21 11:44:05.000000 decoratory-0.1.5.6/Sources/decoratory/__main__.py
--rw-rw-rw-   0        0        0     5490 2023-06-19 15:55:21.000000 decoratory-0.1.5.6/Sources/decoratory/banner.py
--rw-rw-rw-   0        0        0    14152 2023-06-19 15:55:21.000000 decoratory-0.1.5.6/Sources/decoratory/basic.py
--rw-rw-rw-   0        0        0    12412 2023-06-21 10:46:45.000000 decoratory-0.1.5.6/Sources/decoratory/multiton.py
--rw-rw-rw-   0        0        0    37318 2023-06-21 10:46:45.000000 decoratory-0.1.5.6/Sources/decoratory/observer.py
--rw-rw-rw-   0        0        0     7993 2023-06-21 10:46:45.000000 decoratory-0.1.5.6/Sources/decoratory/singleton.py
--rw-rw-rw-   0        0        0    10853 2023-06-21 10:48:51.000000 decoratory-0.1.5.6/Sources/decoratory/wrapper.py
-drwxrwxrwx   0        0        0        0 2023-06-21 11:44:41.900859 decoratory-0.1.5.6/Sources/decoratory.egg-info/
--rw-rw-rw-   0        0        0    46030 2023-06-21 11:44:41.000000 decoratory-0.1.5.6/Sources/decoratory.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      586 2023-06-21 11:44:41.000000 decoratory-0.1.5.6/Sources/decoratory.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-21 11:44:41.000000 decoratory-0.1.5.6/Sources/decoratory.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-06-21 11:44:41.000000 decoratory-0.1.5.6/Sources/decoratory.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-21 11:44:41.920957 decoratory-0.1.5.6/Unittest/
--rw-rw-rw-   0        0        0    24037 2023-06-19 16:25:39.000000 decoratory-0.1.5.6/Unittest/test_basic.py
--rw-rw-rw-   0        0        0    23858 2023-06-21 11:37:48.000000 decoratory-0.1.5.6/Unittest/test_multiton.py
--rw-rw-rw-   0        0        0    40092 2023-06-19 16:25:39.000000 decoratory-0.1.5.6/Unittest/test_observer.py
--rw-rw-rw-   0        0        0    10729 2023-06-21 11:37:48.000000 decoratory-0.1.5.6/Unittest/test_singleton.py
--rw-rw-rw-   0        0        0    10193 2023-06-21 11:37:48.000000 decoratory-0.1.5.6/Unittest/test_wrapper.py
--rw-rw-rw-   0        0        0       42 2023-06-21 11:44:41.931054 decoratory-0.1.5.6/setup.cfg
--rw-rw-rw-   0        0        0     4446 2023-06-21 11:44:05.000000 decoratory-0.1.5.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-23 07:10:45.369796 decoratory-0.9.0.6/
+-rw-rw-rw-   0        0        0     2588 2023-06-22 16:28:01.000000 decoratory-0.9.0.6/License.txt
+-rw-rw-rw-   0        0        0    48944 2023-06-23 07:10:45.369796 decoratory-0.9.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0    47319 2023-06-23 07:04:18.000000 decoratory-0.9.0.6/Readme.rst
+-rw-rw-rw-   0        0        0        0 2023-06-21 06:11:12.000000 decoratory-0.9.0.6/Requirements.txt
+drwxrwxrwx   0        0        0        0 2023-06-23 07:10:45.285134 decoratory-0.9.0.6/Sources/
+drwxrwxrwx   0        0        0        0 2023-06-23 07:10:45.322920 decoratory-0.9.0.6/Sources/decoratory/
+-rw-rw-rw-   0        0        0      249 2023-06-07 18:32:49.000000 decoratory-0.9.0.6/Sources/decoratory/__init__.py
+-rw-rw-rw-   0        0        0     7626 2023-06-23 07:10:15.000000 decoratory-0.9.0.6/Sources/decoratory/__main__.py
+-rw-rw-rw-   0        0        0     5888 2023-06-23 06:53:08.000000 decoratory-0.9.0.6/Sources/decoratory/banner.py
+-rw-rw-rw-   0        0        0    14152 2023-06-22 10:12:45.000000 decoratory-0.9.0.6/Sources/decoratory/basic.py
+-rw-rw-rw-   0        0        0    12412 2023-06-21 10:46:45.000000 decoratory-0.9.0.6/Sources/decoratory/multiton.py
+-rw-rw-rw-   0        0        0    36898 2023-06-21 17:34:08.000000 decoratory-0.9.0.6/Sources/decoratory/observer.py
+-rw-rw-rw-   0        0        0     7993 2023-06-21 10:46:45.000000 decoratory-0.9.0.6/Sources/decoratory/singleton.py
+-rw-rw-rw-   0        0        0    10853 2023-06-21 10:48:51.000000 decoratory-0.9.0.6/Sources/decoratory/wrapper.py
+drwxrwxrwx   0        0        0        0 2023-06-23 07:10:45.338549 decoratory-0.9.0.6/Sources/decoratory.egg-info/
+-rw-rw-rw-   0        0        0    48944 2023-06-23 07:10:45.000000 decoratory-0.9.0.6/Sources/decoratory.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      586 2023-06-23 07:10:45.000000 decoratory-0.9.0.6/Sources/decoratory.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-23 07:10:45.000000 decoratory-0.9.0.6/Sources/decoratory.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-06-23 07:10:45.000000 decoratory-0.9.0.6/Sources/decoratory.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-23 07:10:45.354195 decoratory-0.9.0.6/Unittest/
+-rw-rw-rw-   0        0        0    24037 2023-06-21 16:42:40.000000 decoratory-0.9.0.6/Unittest/test_basic.py
+-rw-rw-rw-   0        0        0    23858 2023-06-21 11:37:48.000000 decoratory-0.9.0.6/Unittest/test_multiton.py
+-rw-rw-rw-   0        0        0    40107 2023-06-23 06:53:08.000000 decoratory-0.9.0.6/Unittest/test_observer.py
+-rw-rw-rw-   0        0        0    10729 2023-06-21 11:37:48.000000 decoratory-0.9.0.6/Unittest/test_singleton.py
+-rw-rw-rw-   0        0        0    10193 2023-06-21 11:37:48.000000 decoratory-0.9.0.6/Unittest/test_wrapper.py
+-rw-rw-rw-   0        0        0       42 2023-06-23 07:10:45.369796 decoratory-0.9.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     4515 2023-06-23 07:10:15.000000 decoratory-0.9.0.6/setup.py
```

### Comparing `decoratory-0.1.5.6/License.txt` & `decoratory-0.9.0.6/License.txt`

 * *Files 27% similar despite different names*

```diff
@@ -1,45 +1,45 @@
-PSF LICENSE AGREEMENT FOR PYTHON 3.10.9
-=======================================
+ PSF LICENSE AGREEMENT FOR PYTHON 3.10.9
+ =======================================
 
-1. This LICENSE AGREEMENT is between the Python Software Foundation ("PSF"),
-   and the Individual or Organization ("Licensee") accessing and otherwise
-   using Python 3.10.9 software in source or binary form and its associated
-   documentation.
-
-2. Subject to the terms and conditions of this License Agreement, PSF hereby
-   grants Licensee a nonexclusive, royalty-free, world-wide license to repro-
-   duce, analyze, test, perform and/or display publicly, prepare derivative
-   works, distribute, and otherwise use Python 3.10.9 alone or in any deriva-
-   tive version, provided, however, that PSF's License Agreement and PSF's
-   notice of copyright, i.e., "Copyright © 2001-2022 Python Software Founda-
-   tion; All Rights Reserved" are retained in Python 3.10.9 alone or in any
-   derivative version prepared by Licensee.
-
-3. In the event Licensee prepares a derivative work that is based on or
-   incorporates Python 3.10.9 or any part thereof, and wants to make the
-   derivative work available to others as provided herein, then Licensee hereby
-   agrees to include in any such work a brief summary of the changes made to
-   Python 3.10.9.
-
-4. PSF is making Python 3.10.9 available to Licensee on an "AS IS" basis.
-   PSF MAKES NO REPRESENTATIONS OR WARRANTIES, EXPRESS OR IMPLIED.  BY WAY OF
-   EXAMPLE, BUT NOT LIMITATION, PSF MAKES NO AND DISCLAIMS ANY REPRESENTATION
-   OR WARRANTY OF MERCHANTABILITY OR FITNESS FOR ANY PARTICULAR PURPOSE OR
-   THAT THE USE OF PYTHON 3.10.9 WILL NOT INFRINGE ANY THIRD PARTY RIGHTS.
-
-5. PSF SHALL NOT BE LIABLE TO LICENSEE OR ANY OTHER USERS OF PYTHON 3.10.9
-   FOR ANY INCIDENTAL, SPECIAL, OR CONSEQUENTIAL DAMAGES OR LOSS AS A RESULT
-   OF MODIFYING, DISTRIBUTING, OR OTHERWISE USING PYTHON 3.10.9, OR ANY
-   DERIVATIVE THEREOF, EVEN IF ADVISED OF THE POSSIBILITY THEREOF.
-
-6. This License Agreement will automatically terminate upon a material breach
-   of its terms and conditions.
-
-7. Nothing in this License Agreement shall be deemed to create any relationship
-   of agency, partnership, or joint venture between PSF and Licensee.  This
-   License Agreement does not grant permission to use PSF trademarks or trade
-   name in a trademark sense to endorse or promote products or services of
-   Licensee, or any third party.
+ 1. This LICENSE AGREEMENT is between the Python Software Foundation ("PSF"),
+    and the Individual or Organization ("Licensee") accessing and otherwise
+    using Python 3.10.9 software in source or binary form and its associated
+    documentation.
+
+ 2. Subject to the terms and conditions of this License Agreement, PSF hereby
+    grants Licensee a nonexclusive, royalty-free, world-wide license to repro-
+    duce, analyze, test, perform and/or display publicly, prepare derivative
+    works, distribute, and otherwise use Python 3.10.9 alone or in any deriva-
+    tive version, provided, however, that PSF's License Agreement and PSF's
+    notice of copyright, i.e., "Copyright © 2001-2022 Python Software Founda-
+    tion; All Rights Reserved" are retained in Python 3.10.9 alone or in any
+    derivative version prepared by Licensee.
+
+ 3. In the event Licensee prepares a derivative work that is based on or
+    incorporates Python 3.10.9 or any part thereof, and wants to make the
+    derivative work available to others as provided herein, then Licensee
+    hereby agrees to include in any such work a brief summary of the changes
+    made to Python 3.10.9.
+
+ 4. PSF is making Python 3.10.9 available to Licensee on an "AS IS" basis.
+    PSF MAKES NO REPRESENTATIONS OR WARRANTIES, EXPRESS OR IMPLIED.  BY WAY OF
+    EXAMPLE, BUT NOT LIMITATION, PSF MAKES NO AND DISCLAIMS ANY REPRESENTATION
+    OR WARRANTY OF MERCHANTABILITY OR FITNESS FOR ANY PARTICULAR PURPOSE OR
+    THAT THE USE OF PYTHON 3.10.9 WILL NOT INFRINGE ANY THIRD PARTY RIGHTS.
+
+ 5. PSF SHALL NOT BE LIABLE TO LICENSEE OR ANY OTHER USERS OF PYTHON 3.10.9
+    FOR ANY INCIDENTAL, SPECIAL, OR CONSEQUENTIAL DAMAGES OR LOSS AS A RESULT
+    OF MODIFYING, DISTRIBUTING, OR OTHERWISE USING PYTHON 3.10.9, OR ANY
+    DERIVATIVE THEREOF, EVEN IF ADVISED OF THE POSSIBILITY THEREOF.
+
+ 6. This License Agreement will automatically terminate upon a material breach
+    of its terms and conditions.
+
+ 7. Nothing in this License Agreement shall be deemed to create any relation-
+    ship of agency, partnership, or joint venture between PSF and Licensee.
+    This License Agreement does not grant permission to use PSF trademarks or
+    trade name in a trademark sense to endorse or promote products or services
+    of Licensee, or any third party.
 
-8. By copying, installing or otherwise using Python 3.10.9, Licensee agrees
-   to be bound by the terms and conditions of this License Agreement.
+ 8. By copying, installing or otherwise using Python 3.10.9, Licensee agrees
+    to be bound by the terms and conditions of this License Agreement.
```

### Comparing `decoratory-0.1.5.6/PKG-INFO` & `decoratory-0.9.0.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: decoratory
-Version: 0.1.5.6
+Version: 0.9.0.6
 Summary: Decorators: Singleton, Multiton, Observer, Observable, generic Wrapper.
 Home-page: http://evation.eu
 Download-URL: http://evation.eu
 Author: Martin Abel
 Author-email: Martin Abel <python@evation.eu>
 Maintainer: Martin Abel
 Maintainer-email: Martin Abel <python@evation.eu>
@@ -36,14 +36,34 @@
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: License.txt
 
 
 .. _top:
 
+..  --------------------------------------------------------------------------
+    Documentation for the decoratory package
+    --------------------------------------------------------------------------
+    __title__ = "Readme"
+    __module__ = "Readme.rst"
+    __author__ = "Martin Abel"
+    __maintainer__ = "Martin Abel"
+    __credits__ = ["Martin Abel"]
+    __company__ = "eVation"
+    __email__ = "python@evation.eu"
+    __url__ = "http://evation.eu"
+    __copyright__ = f"(c) copyright 2020-2023, {__company__}"
+    __created__ = "2020-01-01"
+    __version__ = "0.9.0.7"
+    __date__ = "2023-06-23"
+    __time__ = "09:04:18"
+    __state__ = "Beta"
+    __license__ = "PSF"
+    --------------------------------------------------------------------------
+
 
 ==============================================================================
 Decoratory
 ==============================================================================
 
 
 **Introduction**
@@ -595,28 +615,39 @@
 Observer
 ******************************************************************************
 
 The `observer pattern`_ is generally used to inform one or more registered
 objects (observers, subscribers, objects) about selected actions of an
 observed object (observable, publisher, subject).
 
+The time of activation is set to ``AFTER`` by default, i.e. the observable
+performs its own activity and then activates all registered observers in the
+specified order. This setting can be adjusted to before, after, both or even
+no activation at all via the parameter ``activate`` of ``Observable``.
+
 This implementation provides several ways to decorate a function or class
 as an observable or observer.
 
 * `Observable Decoration`_
 * `Observer Decoration`_
 * `Class Decoration`_
 * `Instance Decoration`_
 
 
 Observable Decoration
 ---------------------
 
 The simplest and at the same time the most pythonic variant of decoration
-is to decorate only the *observed* entities.
+is to decorate only the *observed entities* as a ``Observable``.
+
+This is possible because all observer pattern functionalities are concentrated
+in the ``Observable.BaseClass = BaseObservable`` of the observable decorator,
+while the ``Observer.BaseClass = BaseObserver`` of the observer decorator
+remains empty here. If necessary, it is possible to inherit from both
+BaseClasses to modify their functionalities.
 
 .. code-block:: python
 
     # *** example_observer.py - observable decoration
 
     from decoratory.observer import Observable
     from decoratory.basic import F
@@ -625,27 +656,27 @@
         print(f"{person.__name__} says '{say}'")
 
     @Observable(observers=F(person, 'Hey, dog!'))
     def dog(act: str = "Woof!"):
         print(f"{dog.__name__} acts '{act}'")
 
     # Case 1: Observable decoration
-    #    ---> Person as an observer to dog
-    person()                        # person says 'Hello?'
+    #    ---> Person as an observer to observable dog
+    person()                        # person says 'Hello?'    (person acting)
     dog()                           # dog acts 'Woof!'        (dog acting)
                                     # person says 'Hey, dog!' (observer to dog)
 
 Obviously, the addressed observer, the person, must be declared before
 the observed dog. With the simpler decoration
 ``@Observable(observers=person)`` the person would always respond with their
 default action and say ``'Hello?'``. The usage of ``F`` enables the transfer
 of individual parameters to the observer.
 
 Due to hierarchies in stacked observer patterns, a more detailed management
-of the observed objects may be necessary.
+of observed vs. observing objects may be necessary.
 
 .. code-block:: python
 
     # *** example_observer.py - observable decoration
 
     def person(say: str = "Hello?"):
         print(f"{person.__name__} says '{say}'")
@@ -687,15 +718,15 @@
                                     # person says 'Hey, dog!' (observer to dog)
                                     # cat acts 'Roar!'        (observer to dog)
                                     # person says 'Hey, cat!' (observer to cat)
 
 Calling ``dog()`` results in three activities at the observers, because
 ``dog()`` observes the *observed cat*, which informs the person about its own
 action. If this behavior is not desired, ``dog()`` can instead address the
-*original cat* using the cat substitute callee, i.e.
+*original cat* using the ``cat.substitute.callee``, i.e.
 
 .. code-block:: python
 
     # *** example_observer.py - observable decoration
 
     @Observable(observers=[F(cat.substitute.callee, 'Roar!'),
                            F(person, 'Hey, dog!')])
@@ -704,28 +735,32 @@
 
     # Case 4: Stacked observable decoration
     #    ---> Original cat observes dog, person observes dog and cat
     dog()                           # dog acts 'Woof!'        (dog acting)
                                     # cat acts 'Roar!'        (observer to dog)
                                     # person says 'Hey, dog!' (observer to dog)
 
-And again, cat acts before person because of the order of the observer
-list.
+Again, cat acts before person because of the order of the observer list and
+because the *original cat* observes dog the ``Hey, cat!`` statement of person
+is missing.
 
 
 Observer Decoration
 -------------------
 
 In this reversed decoration scheme, the observer decorator collects its
-observables. Because an observer decoration uses observable methods, all
+observables. This seems more elaborate at first glance, but some prefer to
+explicitly designate the ``Observer`` and ``Observable`` roles in their code.
+
+Because an observer decoration uses observable methods, all
 observable(s) must always be declared before their observer(s).
 
     **1. Rule:** Declare *Observables before Observers*
 
-Thus, the initial example ``Case 1`` from above is as follows:
+Thus, the initial example ``Case 1`` from `Observable Decoration`_ translates to:
 
 .. code-block:: python
 
     # *** example_observer.py - observer decoration
 
     from decoratory.observer import Observer, Observable
     from decoratory.basic import X
@@ -735,39 +770,40 @@
         print(f"{dog.__name__} acts '{act}'")
 
     @Observer(observables=X(dog, 'Hey, dog!'))
     def person(say: str = "Hello?"):
         print(f"{person.__name__} says '{say}'")
 
     # Case 1: Observer decoration
-    #    ---> Person as an observer to dog
+    #    ---> Person as an observer to observable dog
     person()                        # person says 'Hello?'
     dog()                           # dog acts 'Woof!'        (dog acting)
                                     # person says 'Hey, dog!' (observer to dog)
 
 The use of the semantic ``X`` instead of ``F`` indicates that ``dog`` is the
-observable, but the ``X`` arguments are for the observer ``person``.
+observable, but the ``X`` arguments apply for the observer ``person``.
 
-For multiple decorations, the *order of decoration* is relevant. Each
-observable must be decorated before it is used by the observer.
+For multiple decorations, the *order of decoration* is also relevant here.
+Each observable must be decorated before it is used by an observer.
 
-    **2. Rule:** Decorate *@Observer before @Observable*
+    **2. Rule:** Decorating as *@Observable* before using in an *@Observer*
 
-The above situation with person, dog and cat would then look like this:
+The situation ``Case 2`` from `Observable Decoration`_ with person,
+dog and cat would then look like:
 
 .. code-block:: python
 
     # *** example_observer.py - observer decoration
 
-    @Observable                     # 2. Rule: dog before cat, person
-    def dog(act: str = "Woof!"):    # 1. Rule: dog before cat, person
+    @Observable                     # 2. Rule: dog before cat & person
+    def dog(act: str = "Woof!"):    # 1. Rule: dog before cat & person
         print(f"{dog.__name__} acts '{act}'")
 
     @Observer(observables=X(dog, 'Roar!'))
-    @Observable                     # 2. Rule: cat before person
+    @Observable                     # 2. Rule: observable cat before person
     def cat(act: str = "Meow!"):    # 1. Rule: cat before person
         print(f"{cat.__name__} acts '{act}'")
 
     @Observer(observables=[X(dog, 'Hey, dog!'),
                            X(cat.substitute.callee, say='Hey, cat!')])
     def person(say: str = "Hello?"):
         print(f"{person.__name__} says '{say}'")
@@ -780,58 +816,58 @@
                                     # person says 'Hey, cat!' (observer to cat)
 
     dog()                           # dog acts 'Woof!'        (dog acting)
                                     # cat acts 'Roar!'        (observer to dog)
                                     # person says 'Hey, cat!' (observer to cat)
                                     # person says 'Hey, dog!' (observer to dog)
 
-Here, the *observed cat* observes the dog, reacts and triggers the person
-observing the *original cat*. This situation reflects the ``Case 2`` from above.
+Here, cat becomes an observer but its callee ``cat.substitute.callee`` is an
+observable which can be observed by person! This *observed cat* observes
+the dog, reacts and triggers the person.
 
-To reproduce ``Case 3`` above, simply swap the order of the decorations at the
-cat and the person then looks at the *observed cat*.
+To reproduce also ``Case 4`` from above, simply swap the order of the
+decorations at the cat and the person then looks at the *observed cat*.
 
 .. code-block:: python
 
     # *** example_observer.py - observer decoration
 
-    @Observable                     # 2. Rule: dog before cat, person
-    def dog(act: str = "Woof!"):    # 1. Rule: dog before cat, person
+    @Observable                     # 2. Rule: dog before cat & person
+    def dog(act: str = "Woof!"):    # 1. Rule: dog before cat & person
         print(f"{dog.__name__} acts '{act}'")
 
     @Observable                     # 2. Rule: cat before person
     @Observer(observables=X(dog, 'Roar!'))
     def cat(act: str = "Meow!"):    # 1. Rule: cat before person
         print(f"{cat.__name__} acts '{act}'")
 
     @Observer(observables=[X(dog, 'Hey, dog!'), X(cat, say='Hey, cat!')])
-    def person(say: str = "Hello?"):        # 1) Rule: dog, cat before person
+    def person(say: str = "Hello?"):
         print(f"{person.__name__} says '{say}'")
 
     # Case 3: Stacked observer decoration
     #    ---> Cat observes dog, person observes cat and dog
     person()                        # person says 'Hello?'    (person acting)
 
     cat()                           # cat acts 'Meow!'        (cat acting)
                                     # person says 'Hey, cat!' (observer to cat)
 
     dog()                           # dog acts 'Woof!'        (dog acting)
                                     # cat acts 'Roar!'        (observer to dog)
                                     # person says 'Hey, dog!' (observer to dog)
 
-Note the difference: in ``Case 2``, the cat ends up as an ``Observer``, not as
-an ``Observable``. So the person observes the *original cat*. Whereas in
-``case 3``, the cat actually ends up as an ``Observable`` and person can observe
-the *observed cat*.
+Now, both dog and cat end up being observers, observed by the person. But the
+cat observing the dog is the *original cat*, which does not inform the person
+of its activities, and so its statement ``Hey, cat!`` is missing.
 
 
 Class Decoration
 ----------------
 
-Both above techniques, `Observable Decoration`_ and `Observer Decoration`_,
+Both techniques, `Observable Decoration`_ and `Observer Decoration`_,
 are static, in the sense, decorations are done e.g. in @-notation evaluated
 at compile time. They are applied to *static functions*.
 
 *Decoration of a class* by default addresses decoration of the
 *class constructor*, this means
 
 .. code-block:: python
@@ -852,14 +888,16 @@
 
 But this behavior is insidious, e.g.
 
 .. code-block:: python
 
     # *** example_observer.py - class decoration
 
+    from decoratory.observer import Observable
+
     class Person:
         def __init__(self, name: str = "Jane Doe"):
             print(f"{name} arrived.")
 
     @Observable(observers=Person)
     class Dog:
         def __init__(self, name: str = "Teddy"):
@@ -870,17 +908,18 @@
     dog = Dog()                     # Dog Teddy arrived.
                                     # Jane Doe arrived.
 
 The instantiation of ``Dog`` induced an instantiation of ``Person``.
 
     **Hint** --- Take care when decorating a class constructor
 
-    *Calling* ``__init__`` *results in a new instance! This means calling
-    the observable induces instantiation of a new observer object, surely
-    in not any case this is the desired behavior ...*
+    *Notifying the* ``__init__`` *method of an observer results in a new
+    instance! This means calling the observable induces instantiation of
+    a new observer object, surely in not any case this is the desired
+    behavior ...*
 
 So the decoration should not address a class but one (or more) target
 methods of the class. As already mentioned, this is easy if this callback
 function is a ``@staticmethod`` or ``@classmethod``.
 
 .. code-block:: python
 
@@ -911,25 +950,32 @@
 
 This is how it usually works: *one action of the observable*, here it's
 the instantiation of ``Dog``, triggers *one to many actions at each observer*,
 here ``Person``.
 
 .. _Class Decoration, Case 3:
 
-But often an instance method is also interesting as a callback function.
-If a *particular instance* ``prs = Person(name="John Doe")`` of a person
-is meant, a decoration like ``@Observable(observers=prs.action)``
-can be applied to ``Dog``. And for *any instance*
-``@Observable(observers=Person().action)`` works. Even a list of ``F``
-structures would be possible to submit different parameters.
+But often an instance method is also interesting as a callback function:
+
+- If a *particular instance* ``prs = Person(name="John Doe")`` of a
+  person is meant, a decoration like ``@Observable(observers=prs.action)``
+  with the *instance method* can be applied to ``Dog``.
+- For *any instance* of a person ``@Observable(observers=Person().action)``
+  works.
+
+Even a list of ``F`` structures would be possible to optionally submit
+different parameters.
 
 .. code-block:: python
 
     # *** example_observer.py - class decoration
 
+    from decoratory.observer import Observable
+    from decoratory.basic import F
+
     class Person:
         def __init__(self, name: str = "Jane Doe"):
             self.name = name
             print(f"{name} arrived.")
 
         def action(self, act: str = "Hello?"):
             print(f"{self.name} says {act}")
@@ -1011,48 +1057,51 @@
 
 
 Instance Decoration
 -------------------
 
 The classic way to exchange information between objects with the observer
 pattern is through the active use of the ``register``, ``dispatch``, and
-``unregister`` interface methods that an observable exposes. Information can
+``unregister`` *interface methods that an observable exposes*. Information can
 be given to the right recipients at relevant places in the code. For this,
 the classes are not decorated and `dynamic decoration <#dynamic-decoration>`_
-comes into play. Dynamic decoration is used, often also in connection with
-getter/setter/property constructions, since data changes take place
+comes into play. Dynamic decoration is used often also in connection with
+getter/setter/property constructions since data changes take place
 meaningfully over these methods.
 
 Let's consider two simple classes:
 
 .. code-block:: python
 
     # *** example_observer.py - instance decoration
 
     class Note:                             # Observer without decoration!
         def info(self, thing):
             print(f"Note.info: val = {thing.a}")
 
     class Thing:                            # Observable without decoration!
-        def __init__(self, a=0):
+        def __init__(self, a=0):            # Constructor, defining variabe 'a'
             self._a = a
-        def inc(self):
+        def inc(self):                      # Instance method, modifying 'a'
             self._a += 1
-        def get_a(self):
-            return self._a
+        def get_a(self):                    # Getter, setter, property,
+            return self._a                  # modifying variable 'a'
         def set_a(self, value):
             self._a = value
         a = property(get_a, set_a)
 
-Initially, they are undecorated and typical actions might be:
+Initially, all these classes are undecorated and typical actions might be:
 
 .. code-block:: python
 
     # *** example_observer.py - instance decoration
 
+    from decoratory.observer import Observable
+    from decoratory.basic import F
+
     # (1) Setup instances
     nti = Note()                    # Note instance
     tgi = Thing()                   # Thing instance
 
     # (2) Dynamic decoration of some methods: Late binding
     tgi.inc = Observable(tgi.inc)           # Late method decoration
     Thing.set_a = Observable(Thing.set_a)   # Late property decoration
@@ -1085,22 +1134,36 @@
     print(tgi.set_a.observable.observers(classbased=True))
     # ---> {'Note': ['F(info, thing=<__main__.Thing object at ..)']}
 
     # Case 7: Unregister nti.info from tgi
     tgi.inc.observable.unregister(nti.info)
     print(tgi.inc.observable.observers(classbased=True))    # {}
 
-This method of instance decoration is certainly the most flexible. However,
-it bears the risk of losing track of all dependencies.
+In contrast to `Class Decoration`_, this `Instance Decoration`_
+
+(1) instantiates the native classes (1), then
+(2) decorates the relevant instance methods (2), and then
+(3) registers the observers with the associated observables (3).
+
+This method of instance decoration is certainly the most flexible.
+However, it bears the risk of losing track of all dependencies.
 
 
 ******************************************************************************
 Version History
 ******************************************************************************
 
+**Version: 0.9.0.*, Build: 2023-06-23**
+
+- Unit test integration for Windows, Linux (and probably MacOS - feedback?)
+- Pre production state, version 0.9.* for module
+    - observer [ ``python -m decoratory.observer --version`` ]
+- Pre production state, version 0.9.* for package
+    - decoratory [ ``python -m decoratory --version`` ]
+
 **Version: 0.1.5.*, Build: 2023-06-21**
 
 - Pre production state, version 0.9.* for module
     - wrapper [ ``python -m decoratory.wrapper --version`` ]
 
 **Version: 0.1.4.*, Build: 2023-06-21**
```

### Comparing `decoratory-0.1.5.6/Readme.rst` & `decoratory-0.9.0.6/Sources/decoratory.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,69 @@
+Metadata-Version: 2.1
+Name: decoratory
+Version: 0.9.0.6
+Summary: Decorators: Singleton, Multiton, Observer, Observable, generic Wrapper.
+Home-page: http://evation.eu
+Download-URL: http://evation.eu
+Author: Martin Abel
+Author-email: Martin Abel <python@evation.eu>
+Maintainer: Martin Abel
+Maintainer-email: Martin Abel <python@evation.eu>
+License: PSF
+Project-URL: Projekt, http://evation.eu
+Project-URL: Release Notes, http://evation.eu
+Project-URL: Download, http://evation.eu
+Keywords: decorator singleton multiton observer observable wrapper
+Platform: Operating System :: OS Independent
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Education
+Classifier: Intended Audience :: Science/Research
+Classifier: Intended Audience :: Information Technology
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: Implementation
+Classifier: License :: OSI Approved :: Python Software Foundation License
+Classifier: Operating System :: OS Independent
+Classifier: Topic :: Education
+Classifier: Topic :: Software Development
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Utilities
+Requires-Python: >=3.7
+Description-Content-Type: text/x-rst
+License-File: License.txt
+
 
 .. _top:
 
+..  --------------------------------------------------------------------------
+    Documentation for the decoratory package
+    --------------------------------------------------------------------------
+    __title__ = "Readme"
+    __module__ = "Readme.rst"
+    __author__ = "Martin Abel"
+    __maintainer__ = "Martin Abel"
+    __credits__ = ["Martin Abel"]
+    __company__ = "eVation"
+    __email__ = "python@evation.eu"
+    __url__ = "http://evation.eu"
+    __copyright__ = f"(c) copyright 2020-2023, {__company__}"
+    __created__ = "2020-01-01"
+    __version__ = "0.9.0.7"
+    __date__ = "2023-06-23"
+    __time__ = "09:04:18"
+    __state__ = "Beta"
+    __license__ = "PSF"
+    --------------------------------------------------------------------------
+
 
 ==============================================================================
 Decoratory
 ==============================================================================
 
 
 **Introduction**
@@ -556,28 +615,39 @@
 Observer
 ******************************************************************************
 
 The `observer pattern`_ is generally used to inform one or more registered
 objects (observers, subscribers, objects) about selected actions of an
 observed object (observable, publisher, subject).
 
+The time of activation is set to ``AFTER`` by default, i.e. the observable
+performs its own activity and then activates all registered observers in the
+specified order. This setting can be adjusted to before, after, both or even
+no activation at all via the parameter ``activate`` of ``Observable``.
+
 This implementation provides several ways to decorate a function or class
 as an observable or observer.
 
 * `Observable Decoration`_
 * `Observer Decoration`_
 * `Class Decoration`_
 * `Instance Decoration`_
 
 
 Observable Decoration
 ---------------------
 
 The simplest and at the same time the most pythonic variant of decoration
-is to decorate only the *observed* entities.
+is to decorate only the *observed entities* as a ``Observable``.
+
+This is possible because all observer pattern functionalities are concentrated
+in the ``Observable.BaseClass = BaseObservable`` of the observable decorator,
+while the ``Observer.BaseClass = BaseObserver`` of the observer decorator
+remains empty here. If necessary, it is possible to inherit from both
+BaseClasses to modify their functionalities.
 
 .. code-block:: python
 
     # *** example_observer.py - observable decoration
 
     from decoratory.observer import Observable
     from decoratory.basic import F
@@ -586,27 +656,27 @@
         print(f"{person.__name__} says '{say}'")
 
     @Observable(observers=F(person, 'Hey, dog!'))
     def dog(act: str = "Woof!"):
         print(f"{dog.__name__} acts '{act}'")
 
     # Case 1: Observable decoration
-    #    ---> Person as an observer to dog
-    person()                        # person says 'Hello?'
+    #    ---> Person as an observer to observable dog
+    person()                        # person says 'Hello?'    (person acting)
     dog()                           # dog acts 'Woof!'        (dog acting)
                                     # person says 'Hey, dog!' (observer to dog)
 
 Obviously, the addressed observer, the person, must be declared before
 the observed dog. With the simpler decoration
 ``@Observable(observers=person)`` the person would always respond with their
 default action and say ``'Hello?'``. The usage of ``F`` enables the transfer
 of individual parameters to the observer.
 
 Due to hierarchies in stacked observer patterns, a more detailed management
-of the observed objects may be necessary.
+of observed vs. observing objects may be necessary.
 
 .. code-block:: python
 
     # *** example_observer.py - observable decoration
 
     def person(say: str = "Hello?"):
         print(f"{person.__name__} says '{say}'")
@@ -648,15 +718,15 @@
                                     # person says 'Hey, dog!' (observer to dog)
                                     # cat acts 'Roar!'        (observer to dog)
                                     # person says 'Hey, cat!' (observer to cat)
 
 Calling ``dog()`` results in three activities at the observers, because
 ``dog()`` observes the *observed cat*, which informs the person about its own
 action. If this behavior is not desired, ``dog()`` can instead address the
-*original cat* using the cat substitute callee, i.e.
+*original cat* using the ``cat.substitute.callee``, i.e.
 
 .. code-block:: python
 
     # *** example_observer.py - observable decoration
 
     @Observable(observers=[F(cat.substitute.callee, 'Roar!'),
                            F(person, 'Hey, dog!')])
@@ -665,28 +735,32 @@
 
     # Case 4: Stacked observable decoration
     #    ---> Original cat observes dog, person observes dog and cat
     dog()                           # dog acts 'Woof!'        (dog acting)
                                     # cat acts 'Roar!'        (observer to dog)
                                     # person says 'Hey, dog!' (observer to dog)
 
-And again, cat acts before person because of the order of the observer
-list.
+Again, cat acts before person because of the order of the observer list and
+because the *original cat* observes dog the ``Hey, cat!`` statement of person
+is missing.
 
 
 Observer Decoration
 -------------------
 
 In this reversed decoration scheme, the observer decorator collects its
-observables. Because an observer decoration uses observable methods, all
+observables. This seems more elaborate at first glance, but some prefer to
+explicitly designate the ``Observer`` and ``Observable`` roles in their code.
+
+Because an observer decoration uses observable methods, all
 observable(s) must always be declared before their observer(s).
 
     **1. Rule:** Declare *Observables before Observers*
 
-Thus, the initial example ``Case 1`` from above is as follows:
+Thus, the initial example ``Case 1`` from `Observable Decoration`_ translates to:
 
 .. code-block:: python
 
     # *** example_observer.py - observer decoration
 
     from decoratory.observer import Observer, Observable
     from decoratory.basic import X
@@ -696,39 +770,40 @@
         print(f"{dog.__name__} acts '{act}'")
 
     @Observer(observables=X(dog, 'Hey, dog!'))
     def person(say: str = "Hello?"):
         print(f"{person.__name__} says '{say}'")
 
     # Case 1: Observer decoration
-    #    ---> Person as an observer to dog
+    #    ---> Person as an observer to observable dog
     person()                        # person says 'Hello?'
     dog()                           # dog acts 'Woof!'        (dog acting)
                                     # person says 'Hey, dog!' (observer to dog)
 
 The use of the semantic ``X`` instead of ``F`` indicates that ``dog`` is the
-observable, but the ``X`` arguments are for the observer ``person``.
+observable, but the ``X`` arguments apply for the observer ``person``.
 
-For multiple decorations, the *order of decoration* is relevant. Each
-observable must be decorated before it is used by the observer.
+For multiple decorations, the *order of decoration* is also relevant here.
+Each observable must be decorated before it is used by an observer.
 
-    **2. Rule:** Decorate *@Observer before @Observable*
+    **2. Rule:** Decorating as *@Observable* before using in an *@Observer*
 
-The above situation with person, dog and cat would then look like this:
+The situation ``Case 2`` from `Observable Decoration`_ with person,
+dog and cat would then look like:
 
 .. code-block:: python
 
     # *** example_observer.py - observer decoration
 
-    @Observable                     # 2. Rule: dog before cat, person
-    def dog(act: str = "Woof!"):    # 1. Rule: dog before cat, person
+    @Observable                     # 2. Rule: dog before cat & person
+    def dog(act: str = "Woof!"):    # 1. Rule: dog before cat & person
         print(f"{dog.__name__} acts '{act}'")
 
     @Observer(observables=X(dog, 'Roar!'))
-    @Observable                     # 2. Rule: cat before person
+    @Observable                     # 2. Rule: observable cat before person
     def cat(act: str = "Meow!"):    # 1. Rule: cat before person
         print(f"{cat.__name__} acts '{act}'")
 
     @Observer(observables=[X(dog, 'Hey, dog!'),
                            X(cat.substitute.callee, say='Hey, cat!')])
     def person(say: str = "Hello?"):
         print(f"{person.__name__} says '{say}'")
@@ -741,58 +816,58 @@
                                     # person says 'Hey, cat!' (observer to cat)
 
     dog()                           # dog acts 'Woof!'        (dog acting)
                                     # cat acts 'Roar!'        (observer to dog)
                                     # person says 'Hey, cat!' (observer to cat)
                                     # person says 'Hey, dog!' (observer to dog)
 
-Here, the *observed cat* observes the dog, reacts and triggers the person
-observing the *original cat*. This situation reflects the ``Case 2`` from above.
+Here, cat becomes an observer but its callee ``cat.substitute.callee`` is an
+observable which can be observed by person! This *observed cat* observes
+the dog, reacts and triggers the person.
 
-To reproduce ``Case 3`` above, simply swap the order of the decorations at the
-cat and the person then looks at the *observed cat*.
+To reproduce also ``Case 4`` from above, simply swap the order of the
+decorations at the cat and the person then looks at the *observed cat*.
 
 .. code-block:: python
 
     # *** example_observer.py - observer decoration
 
-    @Observable                     # 2. Rule: dog before cat, person
-    def dog(act: str = "Woof!"):    # 1. Rule: dog before cat, person
+    @Observable                     # 2. Rule: dog before cat & person
+    def dog(act: str = "Woof!"):    # 1. Rule: dog before cat & person
         print(f"{dog.__name__} acts '{act}'")
 
     @Observable                     # 2. Rule: cat before person
     @Observer(observables=X(dog, 'Roar!'))
     def cat(act: str = "Meow!"):    # 1. Rule: cat before person
         print(f"{cat.__name__} acts '{act}'")
 
     @Observer(observables=[X(dog, 'Hey, dog!'), X(cat, say='Hey, cat!')])
-    def person(say: str = "Hello?"):        # 1) Rule: dog, cat before person
+    def person(say: str = "Hello?"):
         print(f"{person.__name__} says '{say}'")
 
     # Case 3: Stacked observer decoration
     #    ---> Cat observes dog, person observes cat and dog
     person()                        # person says 'Hello?'    (person acting)
 
     cat()                           # cat acts 'Meow!'        (cat acting)
                                     # person says 'Hey, cat!' (observer to cat)
 
     dog()                           # dog acts 'Woof!'        (dog acting)
                                     # cat acts 'Roar!'        (observer to dog)
                                     # person says 'Hey, dog!' (observer to dog)
 
-Note the difference: in ``Case 2``, the cat ends up as an ``Observer``, not as
-an ``Observable``. So the person observes the *original cat*. Whereas in
-``case 3``, the cat actually ends up as an ``Observable`` and person can observe
-the *observed cat*.
+Now, both dog and cat end up being observers, observed by the person. But the
+cat observing the dog is the *original cat*, which does not inform the person
+of its activities, and so its statement ``Hey, cat!`` is missing.
 
 
 Class Decoration
 ----------------
 
-Both above techniques, `Observable Decoration`_ and `Observer Decoration`_,
+Both techniques, `Observable Decoration`_ and `Observer Decoration`_,
 are static, in the sense, decorations are done e.g. in @-notation evaluated
 at compile time. They are applied to *static functions*.
 
 *Decoration of a class* by default addresses decoration of the
 *class constructor*, this means
 
 .. code-block:: python
@@ -813,14 +888,16 @@
 
 But this behavior is insidious, e.g.
 
 .. code-block:: python
 
     # *** example_observer.py - class decoration
 
+    from decoratory.observer import Observable
+
     class Person:
         def __init__(self, name: str = "Jane Doe"):
             print(f"{name} arrived.")
 
     @Observable(observers=Person)
     class Dog:
         def __init__(self, name: str = "Teddy"):
@@ -831,17 +908,18 @@
     dog = Dog()                     # Dog Teddy arrived.
                                     # Jane Doe arrived.
 
 The instantiation of ``Dog`` induced an instantiation of ``Person``.
 
     **Hint** --- Take care when decorating a class constructor
 
-    *Calling* ``__init__`` *results in a new instance! This means calling
-    the observable induces instantiation of a new observer object, surely
-    in not any case this is the desired behavior ...*
+    *Notifying the* ``__init__`` *method of an observer results in a new
+    instance! This means calling the observable induces instantiation of
+    a new observer object, surely in not any case this is the desired
+    behavior ...*
 
 So the decoration should not address a class but one (or more) target
 methods of the class. As already mentioned, this is easy if this callback
 function is a ``@staticmethod`` or ``@classmethod``.
 
 .. code-block:: python
 
@@ -872,25 +950,32 @@
 
 This is how it usually works: *one action of the observable*, here it's
 the instantiation of ``Dog``, triggers *one to many actions at each observer*,
 here ``Person``.
 
 .. _Class Decoration, Case 3:
 
-But often an instance method is also interesting as a callback function.
-If a *particular instance* ``prs = Person(name="John Doe")`` of a person
-is meant, a decoration like ``@Observable(observers=prs.action)``
-can be applied to ``Dog``. And for *any instance*
-``@Observable(observers=Person().action)`` works. Even a list of ``F``
-structures would be possible to submit different parameters.
+But often an instance method is also interesting as a callback function:
+
+- If a *particular instance* ``prs = Person(name="John Doe")`` of a
+  person is meant, a decoration like ``@Observable(observers=prs.action)``
+  with the *instance method* can be applied to ``Dog``.
+- For *any instance* of a person ``@Observable(observers=Person().action)``
+  works.
+
+Even a list of ``F`` structures would be possible to optionally submit
+different parameters.
 
 .. code-block:: python
 
     # *** example_observer.py - class decoration
 
+    from decoratory.observer import Observable
+    from decoratory.basic import F
+
     class Person:
         def __init__(self, name: str = "Jane Doe"):
             self.name = name
             print(f"{name} arrived.")
 
         def action(self, act: str = "Hello?"):
             print(f"{self.name} says {act}")
@@ -972,48 +1057,51 @@
 
 
 Instance Decoration
 -------------------
 
 The classic way to exchange information between objects with the observer
 pattern is through the active use of the ``register``, ``dispatch``, and
-``unregister`` interface methods that an observable exposes. Information can
+``unregister`` *interface methods that an observable exposes*. Information can
 be given to the right recipients at relevant places in the code. For this,
 the classes are not decorated and `dynamic decoration <#dynamic-decoration>`_
-comes into play. Dynamic decoration is used, often also in connection with
-getter/setter/property constructions, since data changes take place
+comes into play. Dynamic decoration is used often also in connection with
+getter/setter/property constructions since data changes take place
 meaningfully over these methods.
 
 Let's consider two simple classes:
 
 .. code-block:: python
 
     # *** example_observer.py - instance decoration
 
     class Note:                             # Observer without decoration!
         def info(self, thing):
             print(f"Note.info: val = {thing.a}")
 
     class Thing:                            # Observable without decoration!
-        def __init__(self, a=0):
+        def __init__(self, a=0):            # Constructor, defining variabe 'a'
             self._a = a
-        def inc(self):
+        def inc(self):                      # Instance method, modifying 'a'
             self._a += 1
-        def get_a(self):
-            return self._a
+        def get_a(self):                    # Getter, setter, property,
+            return self._a                  # modifying variable 'a'
         def set_a(self, value):
             self._a = value
         a = property(get_a, set_a)
 
-Initially, they are undecorated and typical actions might be:
+Initially, all these classes are undecorated and typical actions might be:
 
 .. code-block:: python
 
     # *** example_observer.py - instance decoration
 
+    from decoratory.observer import Observable
+    from decoratory.basic import F
+
     # (1) Setup instances
     nti = Note()                    # Note instance
     tgi = Thing()                   # Thing instance
 
     # (2) Dynamic decoration of some methods: Late binding
     tgi.inc = Observable(tgi.inc)           # Late method decoration
     Thing.set_a = Observable(Thing.set_a)   # Late property decoration
@@ -1046,22 +1134,36 @@
     print(tgi.set_a.observable.observers(classbased=True))
     # ---> {'Note': ['F(info, thing=<__main__.Thing object at ..)']}
 
     # Case 7: Unregister nti.info from tgi
     tgi.inc.observable.unregister(nti.info)
     print(tgi.inc.observable.observers(classbased=True))    # {}
 
-This method of instance decoration is certainly the most flexible. However,
-it bears the risk of losing track of all dependencies.
+In contrast to `Class Decoration`_, this `Instance Decoration`_
+
+(1) instantiates the native classes (1), then
+(2) decorates the relevant instance methods (2), and then
+(3) registers the observers with the associated observables (3).
+
+This method of instance decoration is certainly the most flexible.
+However, it bears the risk of losing track of all dependencies.
 
 
 ******************************************************************************
 Version History
 ******************************************************************************
 
+**Version: 0.9.0.*, Build: 2023-06-23**
+
+- Unit test integration for Windows, Linux (and probably MacOS - feedback?)
+- Pre production state, version 0.9.* for module
+    - observer [ ``python -m decoratory.observer --version`` ]
+- Pre production state, version 0.9.* for package
+    - decoratory [ ``python -m decoratory --version`` ]
+
 **Version: 0.1.5.*, Build: 2023-06-21**
 
 - Pre production state, version 0.9.* for module
     - wrapper [ ``python -m decoratory.wrapper --version`` ]
 
 **Version: 0.1.4.*, Build: 2023-06-21**
```

### Comparing `decoratory-0.1.5.6/Sources/decoratory/__main__.py` & `decoratory-0.9.0.6/Sources/decoratory/__main__.py`

 * *Files 26% similar despite different names*

```diff
@@ -13,74 +13,122 @@
 __maintainer__ = "Martin Abel"
 __credits__ = ["Martin Abel"]
 __company__ = "eVation"
 __email__ = "python@evation.eu"
 __url__ = "http://evation.eu"
 __copyright__ = f"(c) copyright 2020-2023, {__company__}"
 __created__ = "2020-01-01"
-__version__ = "0.1.5.6"
-__date__ = "2023-06-21"
-__time__ = "13:44:05"
+__version__ = "0.9.0.6"
+__date__ = "2023-06-23"
+__time__ = "09:10:15"
 __state__ = "Beta"
 __license__ = "PSF"
 
-__all__ = []
+__all__ = ["get_file_location"]
 
 # -----------------------------------------------------------------------------
 # Libraries & Modules
 import unittest
+import sys
 
-from sys import argv
 from os.path import dirname, join, basename
 from glob import glob
+from site import getsitepackages, getusersitepackages
 from importlib import import_module
 
 # -----------------------------------------------------------------------------
 # Parameters
 module = __title__.lower()
 name = __title__.capitalize()
 
 
 # -----------------------------------------------------------------------------
+# Functions
+def get_file_location(filename: str = "License.txt"):
+    """Finds an installed data file in any OS dependent installation"""
+    # Look in all possible site package locations, global and user
+    if isinstance(getsitepackages(), list):
+        package_locations = getsitepackages()
+    else:
+        package_locations = [getsitepackages()]
+    if isinstance(getusersitepackages(), list):
+        package_locations.extend(getusersitepackages())
+    else:
+        package_locations.append(getusersitepackages())
+    # Try to find the RECORD file in dist/version folder in package_location
+    target_path = None
+    for package_location in package_locations:
+        try:
+            # Read RECORD file
+            record = join(package_location,
+                          f"{__title__.lower()}-{__version__}.dist-info",
+                          "RECORD")
+            with open(record, "r") as f_rec:
+                rec_lines = f_rec.readlines()
+            # Search in lines for the given filename
+            for rec_line in rec_lines:
+                file_path, sep, *skip = rec_line.partition(",")
+                if file_path and str(file_path).endswith(filename):
+                    try:
+                        path = join(package_location, file_path)
+                        with open(path, "r") as fp:
+                            fp.read(1)  # something to read...?
+                        target_path = path
+                        break
+                    except (FileNotFoundError, Exception):
+                        continue
+        except (FileNotFoundError, Exception):
+            continue
+    return target_path
+
+
+# -----------------------------------------------------------------------------
 # A Module Entry Point
 def main():
     """Package information"""
-    arg = argv[1].strip().lower() if len(argv) > 1 else "message"
+    arg = sys.argv[1].strip().lower() if len(sys.argv) > 1 else "message"
     if arg in "--version":
         print(f"{module}: Version {__version__}, "
               f"Build {__date__} {__time__}, State '{__state__}'")
     elif arg in "--copyright":
         print(f"{__copyright__}")
     elif arg in "--license" or arg in "--licence":
         print(f"\n{'-' * 79}")
         print(f"{__title__} ships under the license: {__license__}".center(79))
         print(f"{'-' * 79}")
-        try:
-            with open(join(dirname(__file__), "data", "License.txt"),
-                      "r") as f:
-                txt = f.read()
+        file_path = get_file_location("License.txt")
+        if file_path is not None:
+            with open(file_path, "r") as fp:
+                txt = fp.read()
             print("\n" + txt)
-        except (FileNotFoundError, Exception):
-            print("*** No additional data accessible. "
-                  f"Please look for file 'License.txt' ***".center(79, " "))
+        else:
+            print("*** No additional data accessible. Please look for "
+                  "file 'License.txt' ***".center(79, " "))
+        # print(f"{'-' * 79}")
+        # print(f"File: {file_path}".center(79, " "))
         print(f"{'-' * 79}")
     elif arg in "--test":
         try:
             print(f"\n{'-' * 70}")
             print(f" Running unit tests for all modules ".center(70, '-'))
             print(f"{'-' * 70}\n")
             loader = unittest.TestLoader().loadTestsFromModule
-            for mdl in glob(join(dirname(__file__), "tests", "test_*.py")):
+            sys_path = dirname(get_file_location(f"test_basic.py"))
+            if sys_path and sys_path not in sys.path:
+                sys.path.insert(0, sys_path)
+            for mdl in glob(join(sys_path, "test_*.py")):
                 mdl = basename(mdl)[:-3].lower()
                 print(f"\n{' ' + mdl + ' ' :-^70s}\n")
-                mdl = import_module(f"decoratory.tests.{mdl}")
+                mdl = import_module(mdl)
                 suite = loader(mdl)
                 unittest.TextTestRunner(verbosity=2).run(suite)
-        except (ModuleNotFoundError, ImportError, Exception) as ex:
-            print(ex)
+        except (ModuleNotFoundError, ImportError, NameError, Exception):
+            print(f"*** No unit test available for package "
+                  f"{module} ***\n".center(70, " "))
+        print(f"{'-' * 70}")
     elif arg in "--information":
         print(f"\nPeople and contact information for package {module}:\n")
         print(f"Author    : {__author__}")
         print(f"Maintainer: {__maintainer__}")
         print(f"Company   : {__company__}")
         print(f"Email     : {__email__}")
         print(f"Web       : {__url__}")
@@ -113,21 +161,21 @@
 For information about the whole package the module command can be left empty, 
 for special module information one of the following modules can be addressed:
 
 {'singleton, multiton, wrapper, observer': ^79s}
 
 Possible options are:
 
-  -h, --help            show this help message
-  -v, --version         show {module}[.module] version information      
-  -c, --copyright       show {module}[.module] copyright statement
-  -l, --license         show {module}[.module] license statement (License.txt)
-      --licence         an alias to --license
-  -t, --test            run unit tests for {module}[.module]
-  -i, --info            people and contact information
+  -h, --help           show this help message
+  -v, --version        show {module}[.module] version information      
+  -c, --copyright      show {module}[.module] copyright statement
+  -l, --license        show {module}[.module] license statement (License.txt)
+      --licence        an alias to --license
+  -t, --test           run unit tests for {module}[.module]
+  -i, --info           people and contact information
 
 Example: Display license statement for the multiton module:
 
 {'python -m decoratory.multiton --license': ^79s}
          
 -------------------------------------------------------------------------------
 {__copyright__: <69s}{__date__: >10s}
```

### Comparing `decoratory-0.1.5.6/Sources/decoratory/banner.py` & `decoratory-0.9.0.6/Sources/decoratory/banner.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,68 +13,72 @@
 __maintainer__ = "Martin Abel"
 __credits__ = ["Martin Abel"]
 __company__ = "eVation"
 __email__ = "python@evation.eu"
 __url__ = "http://evation.eu"
 __copyright__ = f"(c) copyright 2020-2023, {__company__}"
 __created__ = "2020-01-01"
-__version__ = "0.1.3.23"
-__date__ = "2023-06-19"
-__time__ = "17:55:21"
+__version__ = "0.9.0.12"
+__date__ = "2023-06-23"
+__time__ = "08:53:07"
 __state__ = "Beta"
 __license__ = "PSF"
 
 __all__ = ["__banner"]
 
 # -----------------------------------------------------------------------------
 # Libraries & Modules
 import unittest
+import sys
 
-from sys import argv
-from os.path import dirname, join
+from os.path import dirname
 from importlib import import_module
+from decoratory.__main__ import get_file_location
 
 
 # -----------------------------------------------------------------------------
 # Banner Display
 def __banner(title, version, date, time, docs,
              author: str = __author__,
              maintainer: str = __maintainer__,
              company: str = __company__,
              email: str = __email__,
              url: str = __url__,
              copyright: str = __copyright__,
              state: str = __state__,
              license: str = __license__,
-             file_license: str = join("data", "License.txt")):
+             file_license: str = "License.txt"):
     """**Banner**
 
     Banner is an auxiliary module for displaying package and module
     information.
     """
     module = title.lower()
     name = title.capitalize()
 
-    arg = argv[1].strip().lower() if len(argv) > 1 else "message"
+    arg = sys.argv[1].strip().lower() if len(sys.argv) > 1 else "message"
     if arg in "--version":
         print(f"{module}: Version {version}, "
               f"Build {date} {time}, State '{state}'")
     elif arg in "--copyright":
         print(f"{copyright}")
     elif arg in "--license" or arg in "--licence":
         print(f"\n{'-' * 79}")
         print(f"{title} ships under the license: {license}".center(79))
         print(f"{'-' * 79}")
-        try:
-            with open(join(dirname(__file__), file_license), "r") as f:
-                txt = f.read()
+        file_path = get_file_location(file_license)
+        if file_path is not None:
+            with open(file_path, "r") as fp:
+                txt = fp.read()
             print("\n" + txt)
-        except (FileNotFoundError, Exception):
-            print("*** No additional data accessible. "
-                  f"Please look for file '{file_license}' ***".center(79, " "))
+        else:
+            print("*** No additional data accessible. Please look for "
+                  f"file '{file_license}' ***".center(79, " "))
+        # print(f"{'-' * 79}")
+        # print(f"File: {file_path}".center(79, " "))
         print(f"{'-' * 79}")
     elif arg in "--documentation":
         print()
         for doc in docs:
             print(f"{' ' + doc.__name__ + ' ':-^79s}\n")
             print(doc.__doc__)  # print(help(doc))
         print(f"{'-' * 79}")
@@ -86,20 +90,25 @@
         print(f"Email     : {email}")
         print(f"Web       : {url}")
     elif arg in "--test":
         try:
             print(f"\n{'-' * 70}")
             print(f" Running unit test for module: {module} ".center(70, '-'))
             print(f"{'-' * 70}\n")
+            sys_path = dirname(get_file_location(f"test_{module}.py"))
+            if sys_path and sys_path not in sys.path:
+                sys.path.insert(0, sys_path)
             loader = unittest.TestLoader().loadTestsFromModule
-            mdl = import_module(f"decoratory.tests.test_{module.lower()}")
+            mdl = import_module(f"test_{module}")
             suite = loader(mdl)
             unittest.TextTestRunner(verbosity=2).run(suite)
-        except (ModuleNotFoundError, ImportError, Exception) as ex:
-            print(ex)
+        except (ModuleNotFoundError, ImportError, NameError, Exception):
+            print(f"*** No unit test available for module "
+                  f"{module} ***\n".center(70, " "))
+        print(f"{'-' * 70}")
     else:
         print(f"""
 -------------------------------------------------------------------------------
 {title.upper(): ^79}
 -------------------------------------------------------------------------------
 
 {module} is a Python module you cannot execute directly from command line.
@@ -115,22 +124,22 @@
 The current version of the installed package is:
 {module}: Version {version}, Build {date} {time}, State '{state}'
 
 Syntax:   python -m decoratory.{module} [option]
 
 Possible options are:
 
-  -h, --help            show this help message
-  -v, --version         show module {module} version information      
-  -c, --copyright       show module {module} copyright statement
-  -l, --license         show module {module} license statement (License.txt)
-      --licence         an alias to --license
-  -d, --documentation   display selected module code documentation
-  -t, --test            run unit test for module {module}
-  -i, --info            people and contact information
+  -h, --help           show this help message
+  -v, --version        show module {module} version information      
+  -c, --copyright      show module {module} copyright statement
+  -l, --license        show module {module} license statement (License.txt)
+      --licence        an alias to --license
+  -d, --documentation  display selected module code documentation
+  -t, --test           run unit test for module {module}
+  -i, --info           people and contact information
 
 -------------------------------------------------------------------------------
 {copyright: <69s}{date: >10s}
 -------------------------------------------------------------------------------
 """)
```

### Comparing `decoratory-0.1.5.6/Sources/decoratory/basic.py` & `decoratory-0.9.0.6/Sources/decoratory/basic.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,17 +37,17 @@
 __maintainer__ = "Martin Abel"
 __credits__ = ["Martin Abel"]
 __company__ = "eVation"
 __email__ = "python@evation.eu"
 __url__ = "http://evation.eu"
 __copyright__ = f"(c) copyright 2020-2023, {__company__}"
 __created__ = "2020-01-01"
-__version__ = "0.1.3.3"
-__date__ = "2023-06-19"
-__time__ = "17:55:21"
+__version__ = "0.9.0.4"
+__date__ = "2023-06-22"
+__time__ = "12:12:42"
 __state__ = "Beta"
 __license__ = "PSF"
 
 __all__ = ["Activation", "Parser", "F", "X"]
 
 # -----------------------------------------------------------------------------
 # Libraries & Modules
```

### Comparing `decoratory-0.1.5.6/Sources/decoratory/multiton.py` & `decoratory-0.9.0.6/Sources/decoratory/multiton.py`

 * *Files identical despite different names*

### Comparing `decoratory-0.1.5.6/Sources/decoratory/observer.py` & `decoratory-0.9.0.6/Sources/decoratory/observer.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,16 +5,26 @@
 # Document Description
 """**Observer**
 
     The observer pattern is generally used to inform one or more registered
     objects (observers, subscribers, objects) about selected actions of an
     observed object (observable, publisher, subject).
 
+    The time of activation is set to AFTER by default, i.e. the observable
+    performs its own activity and then activates all registered observers in
+    the specified order. This setting can be adjusted to before, after, both
+    or even no activation at all via the parameter activate of Observable.
+
     This implementation provides several ways to decorate a function or class
-    as an Observable or Observer.
+    as an observable or observer.
+
+        -   Observable Decoration
+        -   Observer Decoration
+        -   Class Decoration
+        -   Instance Decoration
 
     Attributes
     ----------
     Observer (class):                           (uses BaseObserver)
         Creates an observer instance as a callable object.
 
     Observable (class):                         (uses BaseObservable)
@@ -31,50 +41,40 @@
         None.
 
     Examples
     --------
 
     A) Observable Decoration
 
-    The simplest and at the same time the most Pythonic variant of decoration
-    is to decorate only the *observed* entities. This is possible because all
-    observer pattern functionalities are concentrated in the BaseClass
-    (=BaseObservable) of the observable decorator, while the BaseClass
-    (=BaseObserver) of the observer decorator remains empty here. If
-    necessary, it is possible to inherit from both BaseClasses to extend
-    their functionalities.
+    The simplest and at the same time the most pythonic variant of decoration
+    is to decorate only the observed entities as a Observable.
+
+    This is possible because all observer pattern functionalities are
+    concentrated in the Observable.BaseClass = BaseObservable of the observable
+    decorator, while the Observer.BaseClass = BaseObserver of the observer
+    decorator remains empty here. If necessary, it is possible to inherit from
+    both BaseClasses to modify their functionalities.
 
+    ---------------------------------------------------------------------------
     from decoratory.observer import Observable
+    from decoratory.basic import F
 
     def person(say: str = "Hello?"):
         print(f"{person.__name__} says '{say}'")
 
     @Observable(observers=F(person, 'Hey, dog!'))
     def dog(act: str = "Woof!"):
         print(f"{dog.__name__} acts '{act}'")
 
     # Case 1: Observable decoration
-    #    ---> Person as an observer to dog
-    person()                        # person says 'Hello?'
+    #    ---> Person as an observer to observable dog
+    person()                        # person says 'Hello?'    (person acting)
     dog()                           # dog acts 'Woof!'        (dog acting)
                                     # person says 'Hey, dog!' (observer to dog)
 
-    Obviously, the addressed observer, the person, must be specified before
-    the observed, the dog. To make the observers more visible in the code, an
-    (optional) observer decoration is supported, i.e.
-
-    @Observer                       # Just for the clarity of the code!
-    def person(say: str = "Hello?"):
-        print(f"{person.__name__} says '{say}'")
-
-    This makes person an observer, but here with the same result as above.
-
-    Due to hierarchies in stacked observer patterns, a more detailed management
-    of the observed objects may be necessary.
-
     def person(say: str = "Hello?"):
         print(f"{person.__name__} says '{say}'")
 
     @Observable(observers=F(person, 'Hey, cat!'))
     def cat(act: str = "Meow!"):
         print(f"{cat.__name__} acts '{act}'")
 
@@ -90,91 +90,77 @@
                                     # person says 'Hey, cat!' (observer to cat)
 
     dog()                           # dog acts 'Woof!'        (dog acting)
                                     # cat acts 'Roar!'        (observer to dog)
                                     # person says 'Hey, cat!' (observer to cat)
                                     # person says 'Hey, dog!' (observer to dog)
 
-    The order of reactions is determined by the order in the list in which
-    the cat observes the dog prior to the person. If this order is reversed:
-
     @Observable(observers=[F(person, 'Hey, dog!'), F(cat, 'Roar!')])
     def dog(act: str = "Woof!"):
         print(f"{dog.__name__} acts '{act}'")
 
     # Case 3: Stacked observable decoration
     #    ---> Cat observes dog, person observes dog and cat
     dog()                           # dog acts 'Woof!'        (dog acting)
                                     # person says 'Hey, dog!' (observer to dog)
                                     # cat acts 'Roar!'        (observer to dog)
                                     # person says 'Hey, cat!' (observer to cat)
 
-    Calling dog() results in three activities at the observers, because dog()
-    observes the 'observed cat', which informs the person about its own action.
-    If this behavior is not desired, dog() can instead address the
-    'original cat' using the cat substitute, i.e.
-
     @Observable(observers=[F(cat.substitute.callee, 'Roar!'),
                            F(person, 'Hey, dog!')])
     def dog(act: str = "Woof!"):
         print(f"{dog.__name__} acts '{act}'")
 
     # Case 4: Stacked observable decoration
     #    ---> Original cat observes dog, person observes dog and cat
     dog()                           # dog acts 'Woof!'        (dog acting)
                                     # cat acts 'Roar!'        (observer to dog)
                                     # person says 'Hey, dog!' (observer to dog)
 
-    And again, cat acts before person because of the order of the observer
-    list.
-
 
     B) Observer Decoration
 
-    In this reverse decoration, the observer decorator defines its observables.
+    In this reversed decoration scheme, the observer decorator collects its
+    observables. This seems more elaborate at first glance, but some prefer to
+    explicitly designate the Observer and Observable roles in their code.
+
     Because an observer decoration uses observable methods, all observable(s)
     must always be declared before their observer(s).
 
-    1. Rule: Declare Observables before Observers
+        1. Rule: Declare Observables before Observers
+
+    For multiple decorations, the order of decoration is also relevant here.
+    Each observable must be decorated before it is used by an observer.
 
-    Thus, the initial example Case 1 from above is as follows:
+        2. Rule: Decorating as @Observable before using in an @Observer
 
+    ---------------------------------------------------------------------------
     from decoratory.observer import Observer, Observable
     from decoratory.basic import X
 
     @Observable
     def dog(act: str = "Woof!"):    # 1. Rule: declare dog before person!
         print(f"{dog.__name__} acts '{act}'")
 
     @Observer(observables=X(dog, 'Hey, dog!'))
     def person(say: str = "Hello?"):
         print(f"{person.__name__} says '{say}'")
 
     # Case 1: Observer decoration
-    #    ---> Person as an observer to dog
+    #    ---> Person as an observer to observable dog
     person()                        # person says 'Hello?'
     dog()                           # dog acts 'Woof!'        (dog acting)
                                     # person says 'Hey, dog!' (observer to dog)
 
-    The use of the semantic X instead of F indicates that dog is the
-    observable, but the X arguments are for person.
-
-    For multiple decorations, the order of decoration is relevant. Each
-    observable must be decorated before it is used by the observer.
-
-    2. Rule: Decorate @Observer before @Observable
-
-    The above situation with person, dog and cat would then look like this:
-
-    @Observable                     # 2. Rule: dog before cat, person
-    def dog(act: str = "Woof!"):    # 1. Rule: dog before cat, person
+    @Observable                     # 2. Rule: dog before cat & person
+    def dog(act: str = "Woof!"):    # 1. Rule: dog before cat & person
         print(f"{dog.__name__} acts '{act}'")
 
     @Observer(observables=X(dog, 'Roar!'))
-    @Observable                     # 2. Rule: cat before person
+    @Observable                     # 2. Rule: observable cat before person
     def cat(act: str = "Meow!"):    # 1. Rule: cat before person
         print(f"{cat.__name__} acts '{act}'")
 
     @Observer(observables=[X(dog, 'Hey, dog!'),
                            X(cat.substitute.callee, say='Hey, cat!')])
     def person(say: str = "Hello?"):
         print(f"{person.__name__} says '{say}'")
@@ -187,55 +173,44 @@
                                     # person says 'Hey, cat!' (observer to cat)
 
     dog()                           # dog acts 'Woof!'        (dog acting)
                                     # cat acts 'Roar!'        (observer to dog)
                                     # person says 'Hey, cat!' (observer to cat)
                                     # person says 'Hey, dog!' (observer to dog)
 
-    Here, the observed cat observes the dog, reacts and triggers the person
-    observing the original cat. This situation reflects the Case 2 from above.
-
-    To reproduce Case 3 above, simply swap the order of the decorations at the
-    cat and the person then looks at the observed cat.
-
-    @Observable                     # 2. Rule: dog before cat, person
-    def dog(act: str = "Woof!"):    # 1. Rule: dog before cat, person
+    @Observable                     # 2. Rule: dog before cat & person
+    def dog(act: str = "Woof!"):    # 1. Rule: dog before cat & person
         print(f"{dog.__name__} acts '{act}'")
 
     @Observable                     # 2. Rule: cat before person
     @Observer(observables=X(dog, 'Roar!'))
     def cat(act: str = "Meow!"):    # 1. Rule: cat before person
         print(f"{cat.__name__} acts '{act}'")
 
     @Observer(observables=[X(dog, 'Hey, dog!'), X(cat, say='Hey, cat!')])
-    def person(say: str = "Hello?"):        # 1) Rule: dog, cat before person
+    def person(say: str = "Hello?"):
         print(f"{person.__name__} says '{say}'")
 
     # Case 3: Stacked observer decoration
     #    ---> Cat observes dog, person observes cat and dog
     person()                        # person says 'Hello?'    (person acting)
 
     cat()                           # cat acts 'Meow!'        (cat acting)
                                     # person says 'Hey, cat!' (observer to cat)
 
     dog()                           # dog acts 'Woof!'        (dog acting)
                                     # cat acts 'Roar!'        (observer to dog)
                                     # person says 'Hey, dog!' (observer to dog)
 
-    Note the difference: in Case 2, the cat ends up as an Observer, not as an
-    Observable. So the person observes the original cat. Whereas in case 3,
-    the cat actually ends up as an Observable and person can observe the
-    observed cat.
-
 
     C) Static Class Decoration
 
-    Both techniques, observable and observer decoration, are static, in the
-    sense, decorations are done in @-notation evaluated at compile time. They
-    are applied to *static functions*.
+    Both techniques, Observable Decoration and Observer Decoration, are static,
+    in the sense, decorations are done e.g. in @-notation evaluated at compile
+    time. They are applied to static functions.
 
     Decoration of a class by default addresses decoration of the class
     constructor, this means
 
     @Observable
     class Dog:
         def __init__(self):
@@ -244,105 +219,129 @@
     should be understood as
 
     class Dog:
         @Observable
         def __init__(self):
             pass                    # Some code ...
 
-    But this behavior is insidious.
+    ---------------------------------------------------------------------------
+    from decoratory.observer import Observable
 
-    WARNING: Calling __init__() results in a new instance! This means calling
-             the observable induces instantiation of a new observer object,
-             surely in not any case this is the desired action...
-
-    These previous two techniques can be used to decorate @staticmethod and
-    @classmethod that are declared and available at compile time. Things are
-    different for instance methods, because instances are not available at
-    compile time. They are not available until class instantiation. Therefore,
-    instance methods are best decorated dynamically in the class constructor.
+    class Person:
+        def __init__(self, name: str = "Jane Doe"):
+            print(f"{name} arrived.")
 
-    from decoratory.observer import Observable
-    from decoratory.basic import F
+    @Observable(observers=Person)
+    class Dog:
+        def __init__(self, name: str = "Teddy"):
+            print(f"Dog {name} arrived.")
+
+    # Case 1: Dog is an observable to Person
+    prs = Person()                  # Jane Doe arrived.
+    dog = Dog()                     # Dog Teddy arrived.
+                                    # Jane Doe arrived.
+
+    class Person:
+        def __init__(self, name: str = "Jane Doe"):
+            print(f"{name} arrived.")
+
+        @staticmethod
+        def action1(act: str = "Hello?"):
+            print(f"Person says {act}")
 
-    class Agent:
         @classmethod
-        def inform(cls, value):
-            print(f"Informed value is: {value}")
+        def action2(cls, act: str = "What's up?"):
+            print(f"Person says {act}")
 
-        def report(self, value):
-            print(f"Reported value is: {value}")
+    @Observable(observers=[Person.action1, Person.action2])
+    class Dog:
+        def __init__(self, name: str = "Teddy"):
+            print(f"Dog {name} arrived.")
 
-    class Actor:
-        def __init__(self):
-            self.a = 1              # Dynamic decoration, static data
-            print(f"Initialization: a = {self.a}")
-            self.modify = Observable(observers=[
-                F(Agent.inform, 'unknown'),
-                F(Agent().report, 'undefined')])(self.modify)
-
-        def modify(self, value=1):
-            self.a += value
-            print(f"Modification  : a = {self.a}")
-
-    Each Actor instance defines its modify method as an observable, which
-    informs about each change of self.a both the class method Agent.inform
-    and the Agent().report instance method. But at the time of execution of
-    __init__ no (current) values or data are available yet, so only static
-    reporting is possible in this way.
-
-    # Case 1: Dynamic decoration, static data
-    a = Actor()                     # Initialization: a = 1
-    a.modify(13)                    # Modification  : a = 14
-                                    # Informed value is: unknown
-                                    # Reported value is: undefined
-
-    However, the problem can be tackled i.e. adding the attribute
-    activate=Activation.NONE to the Observable definition in __init__ to
-    switch off default Activation.AFTER and add an individualized dispatch
-    within the modify method
+    # Case 2: Dog is an observable to Person.action
+    prs = Person()                  # Jane Doe arrived.
+    dog = Dog()                     # Dog Teddy arrived.
+                                    # Person says Hello?
+                                    # Person says What's up?
 
+    ---------------------------------------------------------------------------
     from decoratory.observer import Observable
-    from decoratory.basic import F, Activation
+    from decoratory.basic import F
 
-    class Actor:
-        def __init__(self):
-            self.a = 1
-            print(f"Initialization: a = {self.a}")
-            self.modify = Observable(observers=[
-                F(Agent.inform, 'unknown'),
-                F(Agent().report, 'undefined')],
-            # (1) Switch off default activation
-                activate=Activation.NONE)(self.modify)
-
-        def modify(self, value=1):
-            self.a += value
-            print(f"Modification  : a = {self.a}")
-            # (2) Add individual dispatch
-            self.modify.observable.dispatch(value=self.a)
-
-    # Case 2: Dynamic decoration, dynamic data
-    a = Actor()                     # Initialization: a = 1
-    a.modify(13)                    # Modification  : a = 14
-                                    # Informed value is: 14
-                                    # Reported value is: 14
+    class Person:
+        def __init__(self, name: str = "Jane Doe"):
+            self.name = name
+            print(f"{name} arrived.")
+
+        def action(self, act: str = "Hello?"):
+            print(f"{self.name} says {act}")
+
+    prs1 = Person()                 # Jane Doe arrived.
+    prs2 = Person("John Doe")       # John Doe arrived.
+
+    @Observable(observers=[prs1.action, F(prs2.action, "What's up?")])
+    class Dog:
+        def __init__(self, name: str = "Teddy"):
+            print(f"Dog {name} arrived.")
+
+    # Case 3: Dog is an observable to actions of various person instances.
+    dog = Dog()                     # Dog Teddy arrived.
+                                    # Jane Doe says Hello?
+                                    # John Doe says What's up?
+
+    class Person:
+        def __init__(self, name: str = "Jane Doe"):
+            self.name = name
+            print(f"{name} arrived.")
+
+        @classmethod
+        def actionA(cls, act: str = "Hello?"):
+            print(f"Person says {act}")
+
+        def actionB(self, act: str = "Hello?"):
+            print(f"{self.name} says {act}")
+
+    @Observable(methods=["action1", "action2"],
+                observers=[Person.actionA, Person("Any Doe").actionB])
+    class Dog:
+        def __init__(self, name: str = "Teddy"):
+            self.name = name
+            print(f"Dog {name} arrived.")
+
+        @staticmethod
+        def action1(act: str = "Woof!"):
+            print(f"Dog acts {act}")
+
+        def action2(self, act: str = "Brrr!"):
+            print(f"{self.name} acts {act}")
+
+    # Case 4: Dog is an observable with selected actions.
+                                    # Any Doe arrived.
+    prs = Person()                  # Jane Doe arrived.
+    dog = Dog()                     # Dog Teddy arrived.
+
+    dog.action1()                   # Dog acts Woof!        (@staticmethod)
+                                    # Person says Hello?    (@classmethod)
+                                    # Any Doe says Hello?   (Instance 'Any')
+
+    Dog.action2(dog)                # Teddy acts Brrr!      (Instance 'Teddy')
+                                    # Person says Hello?    (@classmethod)
+                                    # Any Doe says Hello?   (Instance 'Any')
 
 
     D) Dynamic Class Decoration
 
     The classic way to exchange information between objects with the observer
     pattern is through the active use of the register, dispatch, and unregister
-    methods that an observable exports. This way, information can be given to
-    the right recipients at the right places in the code. For this, the
-    classes are not decorated. The dynamic decoration comes into play.
-
-    For this, the classes remain undecorated. Dynamic decoration is used,
-    often also in connection with getter/setter/property constructions, since
-    data changes take place meaningfully over these methods.
-
-    Let’s start with the simple classes:
+    interface methods that an observable exposes. Information can be given to
+    the right recipients at relevant places in the code. For this, the classes
+    are not decorated and dynamic decoration comes into play. Dynamic
+    decoration is used, often also in connection with getter/setter/property
+    constructions, since data changes take place meaningfully over these
+    methods.
 
     class Note:                             # Observer without decoration!
         def info(self, thing):
             print(f"Note.info: val = {thing.a}")
 
     class Thing:                            # Observable without decoration!
         def __init__(self, a=0):
@@ -351,75 +350,74 @@
             self._a += 1
         def get_a(self):
             return self._a
         def set_a(self, value):
             self._a = value
         a = property(get_a, set_a)
 
-    Well, some typical actions might be:
-
+    ---------------------------------------------------------------------------
     from decoratory.observer import Observable
     from decoratory.basic import F
 
     # (1) Setup instances
     nti = Note()                    # Note instance
-    thg = Thing()                   # Thing instance
+    tgi = Thing()                   # Thing instance
 
     # (2) Dynamic decoration of some methods: Late binding
-    thg.inc = Observable(thg.inc)           # Late method decoration
+    tgi.inc = Observable(tgi.inc)           # Late method decoration
     Thing.set_a = Observable(Thing.set_a)   # Late property decoration
     Thing.a = property(Thing.get_a, Thing.set_a)
 
     # (3) Register the observer (Note) with the observable (Thing)
-    thg.inc.observable.register(F(nti.info, thg))
-    thg.set_a.observable.register(F(nti.info, thing=thg))
+    tgi.inc.observable.register(F(nti.info, tgi))
+    tgi.set_a.observable.register(F(nti.info, thing=tgi))
 
     # Case 1: Change self.a = 0 using inc()
-    thg.inc()                       # Note.info: val = 1
+    tgi.inc()                       # Note.info: val = 1
 
     # Case 2: Change self.a = 1 using setter via property
-    thg.a = 2                       # Note.info: val = 2
+    tgi.a = 2                       # Note.info: val = 2
 
     # Case 3: Notification from inc() to nti.info() about Thing(3)
-    thg.inc.observable.dispatch(nti.info, Thing(3))
+    tgi.inc.observable.dispatch(nti.info, Thing(3))
                                     # Note.info: val = 3
 
     # Case 4: Notification from set_a() to nti.info() about Thing(4)
-    thg.set_a.observable.dispatch(nti.info, Thing(4))
+    tgi.set_a.observable.dispatch(nti.info, Thing(4))
                                     # Note.info: val = 4
 
-    # Case 5: Print the current value of thg.a
-    print(f"a = {thg.a}")           # a = 2     (no changes by notifications)
+    # Case 5: Print the current value of tgi.a
+    print(f"a = {tgi.a}")           # a = 2     (no changes by notification)
 
     # Case 6: Print list of all observers
-    print(thg.inc.observable.observers(classbased=True))
+    print(tgi.inc.observable.observers(classbased=True))
     # ---> {'Note': ['F(info, <__main__.Thing object at ..)']}
-    print(thg.set_a.observable.observers(classbased=True))
+    print(tgi.set_a.observable.observers(classbased=True))
     # ---> {'Note': ['F(info, thing=<__main__.Thing object at ..)']}
 
-    # Case 7: Unregister nti.info from thg
-    thg.inc.observable.unregister(nti.info)
-    print(thg.inc.observable.observers(classbased=True))    # {}
+    # Case 7: Unregister nti.info from tgi
+    tgi.inc.observable.unregister(nti.info)
+    print(tgi.inc.observable.observers(classbased=True))    # {}
 """
 
 # -----------------------------------------------------------------------------
 # Module Level Dunders
 __title__ = "Observer"
 __module__ = "observer.py"
 __author__ = "Martin Abel"
 __maintainer__ = "Martin Abel"
 __credits__ = ["Martin Abel"]
 __company__ = "eVation"
 __email__ = "python@evation.eu"
 __url__ = "http://evation.eu"
 __copyright__ = f"(c) copyright 2020-2023, {__company__}"
 __created__ = "2020-01-01"
-__version__ = "0.1.3.3"
+__version__ = "0.9.0.2"
 __date__ = "2023-06-21"
-__time__ = "12:46:42"
+__time__ = "19:34:05"
 __state__ = "Beta"
 __license__ = "PSF"
 
 __all__ = ["Observer", "BaseObserver", "Observable", "BaseObservable"]
 
 # -----------------------------------------------------------------------------
 # Libraries & Modules
@@ -457,16 +455,16 @@
         self.kwargs = kwargs or dict()
 
         self.__observers = dict()  # dict of F-type observers: callee is key!
 
     # Methods of the Observer Pattern
     def register(self,
                  observer: Union[F, callable, str],
-                 *observer_args,
-                 **observer_kwargs) -> None:
+                 *observer_args: object,
+                 **observer_kwargs: object) -> None:
         """Register a function (callable) or method (str) for callback.
 
         Parameters:
             observer (F|callable|str): Callback function|method of the observer
             observer_args (object): Callback (default) positional arguments
             observer_kwargs (object): Callback (default) keyword arguments
 
@@ -504,16 +502,16 @@
         elif callable(observer) or isinstance(observer, str):
             self.__observers.pop(observer, None)  # Quiet mode
         else:
             raise TypeError(f"'{observer}' cannot be unregistered.")
 
     def dispatch(self,
                  observer: Union[F, callable, str, None] = None,
-                 *observer_args,
-                 **observer_kwargs) -> None:
+                 *observer_args: object,
+                 **observer_kwargs: object) -> None:
         """Dispatch an observer.
 
         If the observer parameter is omitted (None), all registered observers
         will be dispatched.
 
         Parameters:
             observer (F|callable|str|None): Callback to be dispatched
@@ -546,15 +544,15 @@
             if observer_args or observer_kwargs:
                 F(observer.callee, *observer_args, **observer_kwargs).eval()
             else:
                 observer.eval()
         else:
             raise TypeError(f"'{observer}' cannot be dispatched.")
 
-    def observers(self, classbased=False) -> dict:
+    def observers(self, classbased: bool = False) -> dict:
         """Listing of all observers.
 
         Observers are collected in a dict, which is returned by default with
         classbased=False. Calling with classbased=True returns a dictionary
         with key-value-pair syntax {classname: list(methods)}.
 
         Parameters:
@@ -583,21 +581,21 @@
     if present, like the callable to be substituted, observers, methods and
     activation point in time.
 
     Observable(substitute, *args, observers, methods, activate, **kwargs)
 
     Attributes
     ----------
-    substitute (callable|type):
+    substitute (callable|type|None):
         A type to be made an observable
 
-    observers (list|F|callable|str):
+    observers (list|F|callable|str|None):
         (List of) callable(s) of observers
 
-    methods (list|F|callable|str):
+    methods (list|F|callable|str|None):
         (List of) callable(s) of as method name strings
 
     activate (Activation):
         Dispatch activation point in time
 
     Methods
     -------
@@ -612,15 +610,15 @@
                  observers: Union[list, callable, F, str, None] = None,
                  methods: Union[list, callable, F, str, None] = None,
                  activate: Activation = Activation.AFTER,
                  **kwargs: object) -> None:
         """Observable (Publisher, Subject).
 
         Parameters:
-            substitute (callable|type: Callable|Type to be made an observable
+            substitute (callable|type): Callable|Type to be made an observable
             observers (list|F|callable|str): (List of) callable(s) of observers
             methods (list|F|callable|str): (List of) callable(s) of as strings
             activate (Activation): Dispatch activation point in time
 
         Returns:
             None.
         """
@@ -768,21 +766,21 @@
     original decorator arguments, if present, like the callable to be
     substituted, observables and methods.
 
     Observer(substitute, *args, observables, methods, **kwargs)
 
     Attributes
     ----------
-    substitute (callable|type):
+    substitute (callable|type|None):
         A type to be made an observer
 
-    observables (list|X|callable|str):
+    observables (list|X|callable|str|None):
         (List of) callable(s) of observables
 
-    methods (list|X|callable|str):
+    methods (list|X|callable|str|None):
         (List of) callable(s) of as method name strings
 
     Methods
     -------
         None.
    """
 
@@ -793,15 +791,15 @@
                  *args: object,
                  observables: Union[list, callable, X, str, None] = None,
                  methods: Union[list, callable, X, str, None] = None,
                  **kwargs: object) -> None:
         """**Observer** (Subscriber, Object)
 
         Parameters:
-            substitute (callable|type: Callable|Type to be made an observable
+            substitute (callable|type): Callable|Type to be made an observable
             observables (list|X|callable|str): (List of) callable(s) of observables
             methods (list|X|callable|str): (List of) callable(s) of as strings
 
         Returns:
             None.
         """
         self.__set__substitute(substitute)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `decoratory-0.1.5.6/Sources/decoratory/singleton.py` & `decoratory-0.9.0.6/Sources/decoratory/singleton.py`

 * *Files identical despite different names*

### Comparing `decoratory-0.1.5.6/Sources/decoratory/wrapper.py` & `decoratory-0.9.0.6/Sources/decoratory/wrapper.py`

 * *Files identical despite different names*

### Comparing `decoratory-0.1.5.6/Sources/decoratory.egg-info/PKG-INFO` & `decoratory-0.9.0.6/Readme.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,49 +1,30 @@
-Metadata-Version: 2.1
-Name: decoratory
-Version: 0.1.5.6
-Summary: Decorators: Singleton, Multiton, Observer, Observable, generic Wrapper.
-Home-page: http://evation.eu
-Download-URL: http://evation.eu
-Author: Martin Abel
-Author-email: Martin Abel <python@evation.eu>
-Maintainer: Martin Abel
-Maintainer-email: Martin Abel <python@evation.eu>
-License: PSF
-Project-URL: Projekt, http://evation.eu
-Project-URL: Release Notes, http://evation.eu
-Project-URL: Download, http://evation.eu
-Keywords: decorator singleton multiton observer observable wrapper
-Platform: Operating System :: OS Independent
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Education
-Classifier: Intended Audience :: Science/Research
-Classifier: Intended Audience :: Information Technology
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: Implementation
-Classifier: License :: OSI Approved :: Python Software Foundation License
-Classifier: Operating System :: OS Independent
-Classifier: Topic :: Education
-Classifier: Topic :: Software Development
-Classifier: Topic :: Software Development :: Libraries
-Classifier: Topic :: Utilities
-Requires-Python: >=3.7
-Description-Content-Type: text/x-rst
-License-File: License.txt
-
 
 .. _top:
 
+..  --------------------------------------------------------------------------
+    Documentation for the decoratory package
+    --------------------------------------------------------------------------
+    __title__ = "Readme"
+    __module__ = "Readme.rst"
+    __author__ = "Martin Abel"
+    __maintainer__ = "Martin Abel"
+    __credits__ = ["Martin Abel"]
+    __company__ = "eVation"
+    __email__ = "python@evation.eu"
+    __url__ = "http://evation.eu"
+    __copyright__ = f"(c) copyright 2020-2023, {__company__}"
+    __created__ = "2020-01-01"
+    __version__ = "0.9.0.7"
+    __date__ = "2023-06-23"
+    __time__ = "09:04:18"
+    __state__ = "Beta"
+    __license__ = "PSF"
+    --------------------------------------------------------------------------
+
 
 ==============================================================================
 Decoratory
 ==============================================================================
 
 
 **Introduction**
@@ -595,28 +576,39 @@
 Observer
 ******************************************************************************
 
 The `observer pattern`_ is generally used to inform one or more registered
 objects (observers, subscribers, objects) about selected actions of an
 observed object (observable, publisher, subject).
 
+The time of activation is set to ``AFTER`` by default, i.e. the observable
+performs its own activity and then activates all registered observers in the
+specified order. This setting can be adjusted to before, after, both or even
+no activation at all via the parameter ``activate`` of ``Observable``.
+
 This implementation provides several ways to decorate a function or class
 as an observable or observer.
 
 * `Observable Decoration`_
 * `Observer Decoration`_
 * `Class Decoration`_
 * `Instance Decoration`_
 
 
 Observable Decoration
 ---------------------
 
 The simplest and at the same time the most pythonic variant of decoration
-is to decorate only the *observed* entities.
+is to decorate only the *observed entities* as a ``Observable``.
+
+This is possible because all observer pattern functionalities are concentrated
+in the ``Observable.BaseClass = BaseObservable`` of the observable decorator,
+while the ``Observer.BaseClass = BaseObserver`` of the observer decorator
+remains empty here. If necessary, it is possible to inherit from both
+BaseClasses to modify their functionalities.
 
 .. code-block:: python
 
     # *** example_observer.py - observable decoration
 
     from decoratory.observer import Observable
     from decoratory.basic import F
@@ -625,27 +617,27 @@
         print(f"{person.__name__} says '{say}'")
 
     @Observable(observers=F(person, 'Hey, dog!'))
     def dog(act: str = "Woof!"):
         print(f"{dog.__name__} acts '{act}'")
 
     # Case 1: Observable decoration
-    #    ---> Person as an observer to dog
-    person()                        # person says 'Hello?'
+    #    ---> Person as an observer to observable dog
+    person()                        # person says 'Hello?'    (person acting)
     dog()                           # dog acts 'Woof!'        (dog acting)
                                     # person says 'Hey, dog!' (observer to dog)
 
 Obviously, the addressed observer, the person, must be declared before
 the observed dog. With the simpler decoration
 ``@Observable(observers=person)`` the person would always respond with their
 default action and say ``'Hello?'``. The usage of ``F`` enables the transfer
 of individual parameters to the observer.
 
 Due to hierarchies in stacked observer patterns, a more detailed management
-of the observed objects may be necessary.
+of observed vs. observing objects may be necessary.
 
 .. code-block:: python
 
     # *** example_observer.py - observable decoration
 
     def person(say: str = "Hello?"):
         print(f"{person.__name__} says '{say}'")
@@ -687,15 +679,15 @@
                                     # person says 'Hey, dog!' (observer to dog)
                                     # cat acts 'Roar!'        (observer to dog)
                                     # person says 'Hey, cat!' (observer to cat)
 
 Calling ``dog()`` results in three activities at the observers, because
 ``dog()`` observes the *observed cat*, which informs the person about its own
 action. If this behavior is not desired, ``dog()`` can instead address the
-*original cat* using the cat substitute callee, i.e.
+*original cat* using the ``cat.substitute.callee``, i.e.
 
 .. code-block:: python
 
     # *** example_observer.py - observable decoration
 
     @Observable(observers=[F(cat.substitute.callee, 'Roar!'),
                            F(person, 'Hey, dog!')])
@@ -704,28 +696,32 @@
 
     # Case 4: Stacked observable decoration
     #    ---> Original cat observes dog, person observes dog and cat
     dog()                           # dog acts 'Woof!'        (dog acting)
                                     # cat acts 'Roar!'        (observer to dog)
                                     # person says 'Hey, dog!' (observer to dog)
 
-And again, cat acts before person because of the order of the observer
-list.
+Again, cat acts before person because of the order of the observer list and
+because the *original cat* observes dog the ``Hey, cat!`` statement of person
+is missing.
 
 
 Observer Decoration
 -------------------
 
 In this reversed decoration scheme, the observer decorator collects its
-observables. Because an observer decoration uses observable methods, all
+observables. This seems more elaborate at first glance, but some prefer to
+explicitly designate the ``Observer`` and ``Observable`` roles in their code.
+
+Because an observer decoration uses observable methods, all
 observable(s) must always be declared before their observer(s).
 
     **1. Rule:** Declare *Observables before Observers*
 
-Thus, the initial example ``Case 1`` from above is as follows:
+Thus, the initial example ``Case 1`` from `Observable Decoration`_ translates to:
 
 .. code-block:: python
 
     # *** example_observer.py - observer decoration
 
     from decoratory.observer import Observer, Observable
     from decoratory.basic import X
@@ -735,39 +731,40 @@
         print(f"{dog.__name__} acts '{act}'")
 
     @Observer(observables=X(dog, 'Hey, dog!'))
     def person(say: str = "Hello?"):
         print(f"{person.__name__} says '{say}'")
 
     # Case 1: Observer decoration
-    #    ---> Person as an observer to dog
+    #    ---> Person as an observer to observable dog
     person()                        # person says 'Hello?'
     dog()                           # dog acts 'Woof!'        (dog acting)
                                     # person says 'Hey, dog!' (observer to dog)
 
 The use of the semantic ``X`` instead of ``F`` indicates that ``dog`` is the
-observable, but the ``X`` arguments are for the observer ``person``.
+observable, but the ``X`` arguments apply for the observer ``person``.
 
-For multiple decorations, the *order of decoration* is relevant. Each
-observable must be decorated before it is used by the observer.
+For multiple decorations, the *order of decoration* is also relevant here.
+Each observable must be decorated before it is used by an observer.
 
-    **2. Rule:** Decorate *@Observer before @Observable*
+    **2. Rule:** Decorating as *@Observable* before using in an *@Observer*
 
-The above situation with person, dog and cat would then look like this:
+The situation ``Case 2`` from `Observable Decoration`_ with person,
+dog and cat would then look like:
 
 .. code-block:: python
 
     # *** example_observer.py - observer decoration
 
-    @Observable                     # 2. Rule: dog before cat, person
-    def dog(act: str = "Woof!"):    # 1. Rule: dog before cat, person
+    @Observable                     # 2. Rule: dog before cat & person
+    def dog(act: str = "Woof!"):    # 1. Rule: dog before cat & person
         print(f"{dog.__name__} acts '{act}'")
 
     @Observer(observables=X(dog, 'Roar!'))
-    @Observable                     # 2. Rule: cat before person
+    @Observable                     # 2. Rule: observable cat before person
     def cat(act: str = "Meow!"):    # 1. Rule: cat before person
         print(f"{cat.__name__} acts '{act}'")
 
     @Observer(observables=[X(dog, 'Hey, dog!'),
                            X(cat.substitute.callee, say='Hey, cat!')])
     def person(say: str = "Hello?"):
         print(f"{person.__name__} says '{say}'")
@@ -780,58 +777,58 @@
                                     # person says 'Hey, cat!' (observer to cat)
 
     dog()                           # dog acts 'Woof!'        (dog acting)
                                     # cat acts 'Roar!'        (observer to dog)
                                     # person says 'Hey, cat!' (observer to cat)
                                     # person says 'Hey, dog!' (observer to dog)
 
-Here, the *observed cat* observes the dog, reacts and triggers the person
-observing the *original cat*. This situation reflects the ``Case 2`` from above.
+Here, cat becomes an observer but its callee ``cat.substitute.callee`` is an
+observable which can be observed by person! This *observed cat* observes
+the dog, reacts and triggers the person.
 
-To reproduce ``Case 3`` above, simply swap the order of the decorations at the
-cat and the person then looks at the *observed cat*.
+To reproduce also ``Case 4`` from above, simply swap the order of the
+decorations at the cat and the person then looks at the *observed cat*.
 
 .. code-block:: python
 
     # *** example_observer.py - observer decoration
 
-    @Observable                     # 2. Rule: dog before cat, person
-    def dog(act: str = "Woof!"):    # 1. Rule: dog before cat, person
+    @Observable                     # 2. Rule: dog before cat & person
+    def dog(act: str = "Woof!"):    # 1. Rule: dog before cat & person
         print(f"{dog.__name__} acts '{act}'")
 
     @Observable                     # 2. Rule: cat before person
     @Observer(observables=X(dog, 'Roar!'))
     def cat(act: str = "Meow!"):    # 1. Rule: cat before person
         print(f"{cat.__name__} acts '{act}'")
 
     @Observer(observables=[X(dog, 'Hey, dog!'), X(cat, say='Hey, cat!')])
-    def person(say: str = "Hello?"):        # 1) Rule: dog, cat before person
+    def person(say: str = "Hello?"):
         print(f"{person.__name__} says '{say}'")
 
     # Case 3: Stacked observer decoration
     #    ---> Cat observes dog, person observes cat and dog
     person()                        # person says 'Hello?'    (person acting)
 
     cat()                           # cat acts 'Meow!'        (cat acting)
                                     # person says 'Hey, cat!' (observer to cat)
 
     dog()                           # dog acts 'Woof!'        (dog acting)
                                     # cat acts 'Roar!'        (observer to dog)
                                     # person says 'Hey, dog!' (observer to dog)
 
-Note the difference: in ``Case 2``, the cat ends up as an ``Observer``, not as
-an ``Observable``. So the person observes the *original cat*. Whereas in
-``case 3``, the cat actually ends up as an ``Observable`` and person can observe
-the *observed cat*.
+Now, both dog and cat end up being observers, observed by the person. But the
+cat observing the dog is the *original cat*, which does not inform the person
+of its activities, and so its statement ``Hey, cat!`` is missing.
 
 
 Class Decoration
 ----------------
 
-Both above techniques, `Observable Decoration`_ and `Observer Decoration`_,
+Both techniques, `Observable Decoration`_ and `Observer Decoration`_,
 are static, in the sense, decorations are done e.g. in @-notation evaluated
 at compile time. They are applied to *static functions*.
 
 *Decoration of a class* by default addresses decoration of the
 *class constructor*, this means
 
 .. code-block:: python
@@ -852,14 +849,16 @@
 
 But this behavior is insidious, e.g.
 
 .. code-block:: python
 
     # *** example_observer.py - class decoration
 
+    from decoratory.observer import Observable
+
     class Person:
         def __init__(self, name: str = "Jane Doe"):
             print(f"{name} arrived.")
 
     @Observable(observers=Person)
     class Dog:
         def __init__(self, name: str = "Teddy"):
@@ -870,17 +869,18 @@
     dog = Dog()                     # Dog Teddy arrived.
                                     # Jane Doe arrived.
 
 The instantiation of ``Dog`` induced an instantiation of ``Person``.
 
     **Hint** --- Take care when decorating a class constructor
 
-    *Calling* ``__init__`` *results in a new instance! This means calling
-    the observable induces instantiation of a new observer object, surely
-    in not any case this is the desired behavior ...*
+    *Notifying the* ``__init__`` *method of an observer results in a new
+    instance! This means calling the observable induces instantiation of
+    a new observer object, surely in not any case this is the desired
+    behavior ...*
 
 So the decoration should not address a class but one (or more) target
 methods of the class. As already mentioned, this is easy if this callback
 function is a ``@staticmethod`` or ``@classmethod``.
 
 .. code-block:: python
 
@@ -911,25 +911,32 @@
 
 This is how it usually works: *one action of the observable*, here it's
 the instantiation of ``Dog``, triggers *one to many actions at each observer*,
 here ``Person``.
 
 .. _Class Decoration, Case 3:
 
-But often an instance method is also interesting as a callback function.
-If a *particular instance* ``prs = Person(name="John Doe")`` of a person
-is meant, a decoration like ``@Observable(observers=prs.action)``
-can be applied to ``Dog``. And for *any instance*
-``@Observable(observers=Person().action)`` works. Even a list of ``F``
-structures would be possible to submit different parameters.
+But often an instance method is also interesting as a callback function:
+
+- If a *particular instance* ``prs = Person(name="John Doe")`` of a
+  person is meant, a decoration like ``@Observable(observers=prs.action)``
+  with the *instance method* can be applied to ``Dog``.
+- For *any instance* of a person ``@Observable(observers=Person().action)``
+  works.
+
+Even a list of ``F`` structures would be possible to optionally submit
+different parameters.
 
 .. code-block:: python
 
     # *** example_observer.py - class decoration
 
+    from decoratory.observer import Observable
+    from decoratory.basic import F
+
     class Person:
         def __init__(self, name: str = "Jane Doe"):
             self.name = name
             print(f"{name} arrived.")
 
         def action(self, act: str = "Hello?"):
             print(f"{self.name} says {act}")
@@ -1011,48 +1018,51 @@
 
 
 Instance Decoration
 -------------------
 
 The classic way to exchange information between objects with the observer
 pattern is through the active use of the ``register``, ``dispatch``, and
-``unregister`` interface methods that an observable exposes. Information can
+``unregister`` *interface methods that an observable exposes*. Information can
 be given to the right recipients at relevant places in the code. For this,
 the classes are not decorated and `dynamic decoration <#dynamic-decoration>`_
-comes into play. Dynamic decoration is used, often also in connection with
-getter/setter/property constructions, since data changes take place
+comes into play. Dynamic decoration is used often also in connection with
+getter/setter/property constructions since data changes take place
 meaningfully over these methods.
 
 Let's consider two simple classes:
 
 .. code-block:: python
 
     # *** example_observer.py - instance decoration
 
     class Note:                             # Observer without decoration!
         def info(self, thing):
             print(f"Note.info: val = {thing.a}")
 
     class Thing:                            # Observable without decoration!
-        def __init__(self, a=0):
+        def __init__(self, a=0):            # Constructor, defining variabe 'a'
             self._a = a
-        def inc(self):
+        def inc(self):                      # Instance method, modifying 'a'
             self._a += 1
-        def get_a(self):
-            return self._a
+        def get_a(self):                    # Getter, setter, property,
+            return self._a                  # modifying variable 'a'
         def set_a(self, value):
             self._a = value
         a = property(get_a, set_a)
 
-Initially, they are undecorated and typical actions might be:
+Initially, all these classes are undecorated and typical actions might be:
 
 .. code-block:: python
 
     # *** example_observer.py - instance decoration
 
+    from decoratory.observer import Observable
+    from decoratory.basic import F
+
     # (1) Setup instances
     nti = Note()                    # Note instance
     tgi = Thing()                   # Thing instance
 
     # (2) Dynamic decoration of some methods: Late binding
     tgi.inc = Observable(tgi.inc)           # Late method decoration
     Thing.set_a = Observable(Thing.set_a)   # Late property decoration
@@ -1085,22 +1095,36 @@
     print(tgi.set_a.observable.observers(classbased=True))
     # ---> {'Note': ['F(info, thing=<__main__.Thing object at ..)']}
 
     # Case 7: Unregister nti.info from tgi
     tgi.inc.observable.unregister(nti.info)
     print(tgi.inc.observable.observers(classbased=True))    # {}
 
-This method of instance decoration is certainly the most flexible. However,
-it bears the risk of losing track of all dependencies.
+In contrast to `Class Decoration`_, this `Instance Decoration`_
+
+(1) instantiates the native classes (1), then
+(2) decorates the relevant instance methods (2), and then
+(3) registers the observers with the associated observables (3).
+
+This method of instance decoration is certainly the most flexible.
+However, it bears the risk of losing track of all dependencies.
 
 
 ******************************************************************************
 Version History
 ******************************************************************************
 
+**Version: 0.9.0.*, Build: 2023-06-23**
+
+- Unit test integration for Windows, Linux (and probably MacOS - feedback?)
+- Pre production state, version 0.9.* for module
+    - observer [ ``python -m decoratory.observer --version`` ]
+- Pre production state, version 0.9.* for package
+    - decoratory [ ``python -m decoratory --version`` ]
+
 **Version: 0.1.5.*, Build: 2023-06-21**
 
 - Pre production state, version 0.9.* for module
     - wrapper [ ``python -m decoratory.wrapper --version`` ]
 
 **Version: 0.1.4.*, Build: 2023-06-21**
```

### Comparing `decoratory-0.1.5.6/Sources/decoratory.egg-info/SOURCES.txt` & `decoratory-0.9.0.6/Sources/decoratory.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `decoratory-0.1.5.6/Unittest/test_basic.py` & `decoratory-0.9.0.6/Unittest/test_basic.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,17 +13,17 @@
 __maintainer__ = "Martin Abel"
 __credits__ = ["Martin Abel"]
 __company__ = "eVation"
 __email__ = "python@evation.eu"
 __url__ = "http://evation.eu"
 __copyright__ = f"(c) copyright 2020-2023, {__company__}"
 __created__ = "2020-01-01"
-__version__ = "0.1.3.6"
-__date__ = "2023-06-19"
-__time__ = "18:25:39"
+__version__ = "0.9.0.1"
+__date__ = "2023-06-21"
+__time__ = "18:42:36"
 __state__ = "Beta"
 __license__ = "PSF"
 
 # -----------------------------------------------------------------------------
 # Libraries & Modules
 import unittest
```

### Comparing `decoratory-0.1.5.6/Unittest/test_multiton.py` & `decoratory-0.9.0.6/Unittest/test_multiton.py`

 * *Files identical despite different names*

### Comparing `decoratory-0.1.5.6/Unittest/test_observer.py` & `decoratory-0.9.0.6/Unittest/test_observer.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,17 +13,17 @@
 __maintainer__ = "Martin Abel"
 __credits__ = ["Martin Abel"]
 __company__ = "eVation"
 __email__ = "python@evation.eu"
 __url__ = "http://evation.eu"
 __copyright__ = f"(c) copyright 2020-2023, {__company__}"
 __created__ = "2020-01-01"
-__version__ = "0.1.3.7"
-__date__ = "2023-06-19"
-__time__ = "18:25:39"
+__version__ = "0.9.0.2"
+__date__ = "2023-06-23"
+__time__ = "08:53:07"
 __state__ = "Beta"
 __license__ = "PSF"
 
 # -----------------------------------------------------------------------------
 # Libraries & Modules
 import unittest
 
@@ -64,15 +64,15 @@
         pass
 
     def tearDown(self):
         """Wrap-up"""
         pass
 
     def test_nodecoration_noparams_without_brackets(self):
-        """Unittest: Functions: no decoration, no parameters, no brackets"""
+        """Unittest: Functions - no decoration, no parameters, no brackets"""
 
         # Result list
         res = list()
 
         # Observable
         def dog(act: str = "Brrr!") -> None:
             """A dog function"""
@@ -139,15 +139,15 @@
         prs_obsr()
         self.assertListEqual(res, ["person says 'Hello?'"])
         res.clear()
         dog_obsl()
         self.assertListEqual(res, ["dog acts 'Brrr!'"])
 
     def test_nodecoration_noparams_with_empty_brackets(self):
-        """Unittest: Functions: no decoration, no parameters, empty brackets"""
+        """Unittest: Functions - no decoration, no parameters, empty brackets"""
 
         # Result list
         res = list()
 
         # Observable
         def dog(act: str = "Brrr!") -> None:
             """A dog function"""
@@ -214,15 +214,15 @@
         prs_obsr()
         self.assertListEqual(res, ["person says 'Hello?'"])
         res.clear()
         dog_obsl()
         self.assertListEqual(res, ["dog acts 'Brrr!'"])
 
     def test_nodecoration_params(self):
-        """Unittest: Functions: no decoration, parameters"""
+        """Unittest: Functions - no decoration, parameters"""
 
         # Result list
         res = list()
 
         # Observable
         def dog(act1: str = "Brrr", act2: str = "!") -> None:
             """A dog function"""
@@ -291,15 +291,15 @@
         prs_obsr()
         self.assertListEqual(res, ["person says 'Ooops!'"])
         res.clear()
         dog_obsl()
         self.assertListEqual(res, ["dog acts 'Woof, Woof!'"])
 
     def test_decoration_noparams(self):
-        """Unittest: Functions: decoration, no parameters"""
+        """Unittest: Functions - decoration, no parameters"""
 
         # Result list
         res = list()
 
         # Observable
         def dog(act: str = "Brrr!") -> None:
             """A dog function"""
@@ -366,15 +366,15 @@
         prs_obsr()
         self.assertListEqual(res, ["person says 'Hello?'"])
         res.clear()
         dog_obsl()
         self.assertListEqual(res, ["dog acts 'Brrr!'"])
 
     def test_decoration_params(self):
-        """Unittest: Functions: decoration, parameters"""
+        """Unittest: Functions - decoration, parameters"""
 
         # Result list
         res = list()
 
         # Observable
         def dog(act1: str = "Brrr", act2: str = "!") -> None:
             """A dog function"""
@@ -445,15 +445,15 @@
         prs_obsr()
         self.assertListEqual(res, ["person says 'Ooops!'"])
         res.clear()
         dog_obsl()
         self.assertListEqual(res, ["dog acts 'Woof, Woof!'"])
 
     def test_observable_activation(self):
-        """Unittest: Functions: Activation"""
+        """Unittest: Functions - Activation"""
 
         # Result list
         res = list()
 
         # Observable
         def dog(act: str = "Brrr!") -> None:
             """A dog function"""
@@ -518,15 +518,15 @@
         res.clear()
         dog_obsl()
         self.assertListEqual(res, ["person says 'Hello?'",
                                    "dog acts 'Brrr!'",
                                    "person says 'Hello?'"])
 
     def test_observable_functions(self):
-        """Unittest: Functions: Interface register, unregister, dispatch"""
+        """Unittest: Functions - Interface register, unregister, dispatch"""
 
         # Result list
         res = list()
 
         # Observable
         def dog(act: str = "Woof!") -> None:
             """A dog function"""
@@ -649,15 +649,15 @@
         # ---------------------------------------------------------------------
         # Test: Decoration via Observer
         dog_obsl = Observable(dog)
         prs_obsr = Observer(observables=X(dog_obsl, say="What's up?"))(person)
         test(prs_obsr, dog_obsl)
 
     def test_observable_class_init(self):
-        """Unittest: Class: init()"""
+        """Unittest: Class - init()"""
 
         # Result list
         res = list()
 
         # Observable
         class Dog:
             """A Dog Type"""
@@ -706,15 +706,15 @@
         p.untouched()
         self.assertEqual(res, ['PERSON is untouched'])
         res.clear()
         d.untouched()
         self.assertEqual(res, ['DOG is untouched'])
 
     def test_observable_class_staticmethod01(self):
-        """Unittest: Class: staticmethod()"""
+        """Unittest: Class - staticmethod()"""
 
         # Result list
         res = list()
 
         # Observable
         class Dog:
             """A Dog Type"""
@@ -770,15 +770,15 @@
         Person.static_untouched()
         self.assertEqual(res, ['Person is untouched'])
         res.clear()
         Dog.static_untouched()
         self.assertEqual(res, ['Dog is untouched'])
 
     def test_observable_class_staticmethod02(self):
-        """Unittest: Class: staticmethod()"""
+        """Unittest: Class -  staticmethod()"""
 
         # Result list
         res = list()
 
         # Observable
         class Dog:
             """A Dog Type"""
@@ -833,15 +833,15 @@
         Person.static_untouched()
         self.assertEqual(res, ['Person is untouched'])
         res.clear()
         Dog.static_untouched()
         self.assertEqual(res, ['Dog is untouched'])
 
     def test_observable_class_classmethod01(self):
-        """Unittest: Class: classmethod()"""
+        """Unittest: Class - classmethod()"""
 
         # Result list
         res = list()
 
         # Observable
         class Dog:
             """A Dog Type"""
@@ -879,15 +879,15 @@
         # Dog with Person as an observer
         res.clear()
         Dog.class_method()
         self.assertListEqual(res, ["Dog act 'Woof!'",
                                    "Person say 'What's up?'"])
 
     def test_observable_class_classmethod02(self):
-        """Unittest: Class: classmethod()"""
+        """Unittest: Class - classmethod()"""
 
         # Result list
         res = list()
 
         # Observable
         class Dog:
             """A Dog Type"""
@@ -924,15 +924,15 @@
         # Dog with Person as an observer
         res.clear()
         Dog.class_method()
         self.assertListEqual(res, ["Dog act 'Woof!'",
                                    "Person say 'What's up?'"])
 
     def test_observable_class_objectmethod01(self):
-        """Unittest: Class: object method()"""
+        """Unittest: Class - object method()"""
 
         # Result list
         res = list()
 
         # Observable
         class Dog:
             """A Dog Type"""
@@ -972,15 +972,15 @@
         # Dog with Person as an observer
         res.clear()
         Dog_obsl.object_method()
         self.assertListEqual(res, ["Dog act 'Woof!'",
                                    "Person say 'What's up?'"])
 
     def test_observable_class_objectmethod02(self):
-        """Unittest: Class: object method()"""
+        """Unittest: Class - object method()"""
 
         # Result list
         res = list()
 
         # Observable
         class Dog:
             """A Dog Type"""
```

### Comparing `decoratory-0.1.5.6/Unittest/test_singleton.py` & `decoratory-0.9.0.6/Unittest/test_singleton.py`

 * *Files identical despite different names*

### Comparing `decoratory-0.1.5.6/Unittest/test_wrapper.py` & `decoratory-0.9.0.6/Unittest/test_wrapper.py`

 * *Files identical despite different names*

### Comparing `decoratory-0.1.5.6/setup.py` & `decoratory-0.9.0.6/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,29 +12,31 @@
 __maintainer__ = "Martin Abel"
 __credits__ = ["Martin Abel"]
 __company__ = "eVation"
 __email__ = "python@evation.eu"
 __url__ = "http://evation.eu"
 __copyright__ = f"(c) copyright 2020-2023, {__company__}"
 __created__ = "2020-01-01"
-__version__ = "0.1.5.6"
-__date__ = "2023-06-21"
-__time__ = "13:44:05"
+__version__ = "0.9.0.6"
+__date__ = "2023-06-23"
+__time__ = "09:10:15"
 __state__ = "Beta"
 __license__ = "PSF"
 
 # -----------------------------------------------------------------------------
 # Libraries
 from os.path import join
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 
 # -----------------------------------------------------------------------------
 # Parameters
 src = "Sources"
+dta = join("lib", "site-packages", __title__, "data")
+tst = join("lib", "site-packages", __title__, "tests")
 
 with open("Readme.rst", "r") as f:
     description = f.read()
 
 with open("Requirements.txt", "r") as f:
     requirements = [str(req) for req in f.read().splitlines() if req]
 
@@ -42,15 +44,15 @@
 def version_check():
     """Keep versions in sync"""
     try:
         # noinspection PyProtectedMember
         from Sources.decoratory.__main__ import __version__ as version
         assert version == __version__, (
             f"\n\n{'':=^79s}\n"
-            f"{' Version mismatch: __main__.version != setup.version ':=^79s}\n"
+            f"{' Version problem: __main__.version != setup.version ':=^79s}\n"
             f"{'':=^79s}")
     except (ModuleNotFoundError, ImportError):
         pass  # Let the AssertionError pass...
 
 
 # -----------------------------------------------------------------------------
 # Excecute
@@ -98,22 +100,22 @@
         'Topic :: Utilities'],
     # Modules, Files and Data
     # https://setuptools.pypa.io/en/latest/userguide/package_discovery.html#finding-simple-packages
     packages=find_packages(where=src),
     package_dir={"": src},
     package_data={},
     py_modules=[],
-    data_files=[(f"./lib/site-packages/{__title__}/data",
-                 ["License.txt", "Readme.rst", "Requirements.txt"]),
-                (f"./lib/site-packages/{__title__}/tests",
-                 ["Unittest/test_basic.py",
-                  "Unittest/test_singleton.py",
-                  "Unittest/test_multiton.py",
-                  "Unittest/test_wrapper.py",
-                  "Unittest/test_observer.py"])],
+    data_files=[(dta, ["License.txt",
+                       "Readme.rst",
+                       "Requirements.txt"]),
+                (tst, ["Unittest/test_basic.py",
+                       "Unittest/test_singleton.py",
+                       "Unittest/test_multiton.py",
+                       "Unittest/test_wrapper.py",
+                       "Unittest/test_observer.py"])],
     entry_points={},
     # Dependencies
     python_requires='>=3.7',
     setup_requires=[],
     install_requires=requirements,
     # Post install
     # cmdclass={'install': CustomInstall},
```

