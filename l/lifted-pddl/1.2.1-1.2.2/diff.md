# Comparing `tmp/lifted-pddl-1.2.1.tar.gz` & `tmp/lifted-pddl-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lifted-pddl-1.2.1.tar", last modified: Thu Jun 22 00:23:16 2023, max compression
+gzip compressed data, was "lifted-pddl-1.2.2.tar", last modified: Fri Jun 23 17:21:26 2023, max compression
```

## Comparing `lifted-pddl-1.2.1.tar` & `lifted-pddl-1.2.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 00:23:16.363217 lifted-pddl-1.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-22 00:23:05.000000 lifted-pddl-1.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-22 00:23:05.000000 lifted-pddl-1.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5174 2023-06-22 00:23:16.363217 lifted-pddl-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4680 2023-06-22 00:23:05.000000 lifted-pddl-1.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 00:23:16.363217 lifted-pddl-1.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-06-22 00:23:05.000000 lifted-pddl-1.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 00:23:16.359217 lifted-pddl-1.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 00:23:16.359217 lifted-pddl-1.2.1/src/lifted_pddl/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-22 00:23:05.000000 lifted-pddl-1.2.1/src/lifted_pddl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7941 2023-06-22 00:23:05.000000 lifted-pddl-1.2.1/src/lifted_pddl/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 00:23:16.359217 lifted-pddl-1.2.1/src/lifted_pddl/data/
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-06-22 00:23:05.000000 lifted-pddl-1.2.1/src/lifted_pddl/data/blocksworld-domain.pddl
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-06-22 00:23:05.000000 lifted-pddl-1.2.1/src/lifted_pddl/data/blocksworld-problem.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-06-22 00:23:05.000000 lifted-pddl-1.2.1/src/lifted_pddl/data/logistics-domain-exists.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-06-22 00:23:05.000000 lifted-pddl-1.2.1/src/lifted_pddl/data/logistics-domain.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     2426 2023-06-22 00:23:05.000000 lifted-pddl-1.2.1/src/lifted_pddl/data/logistics-problem.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     3492 2023-06-22 00:23:05.000000 lifted-pddl-1.2.1/src/lifted_pddl/data/sokoban-domain-no-clear.pddl
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-06-22 00:23:05.000000 lifted-pddl-1.2.1/src/lifted_pddl/data/sokoban-problem.pddl
--rw-r--r--   0 runner    (1001) docker     (123)    34186 2023-06-22 00:23:05.000000 lifted-pddl-1.2.1/src/lifted_pddl/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 00:23:16.359217 lifted-pddl-1.2.1/src/lifted_pddl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5174 2023-06-22 00:23:16.000000 lifted-pddl-1.2.1/src/lifted_pddl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-06-22 00:23:16.000000 lifted-pddl-1.2.1/src/lifted_pddl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 00:23:16.000000 lifted-pddl-1.2.1/src/lifted_pddl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-22 00:23:16.000000 lifted-pddl-1.2.1/src/lifted_pddl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-22 00:23:16.000000 lifted-pddl-1.2.1/src/lifted_pddl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-22 00:23:16.000000 lifted-pddl-1.2.1/src/lifted_pddl.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 17:21:26.575081 lifted-pddl-1.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-23 17:21:17.000000 lifted-pddl-1.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-23 17:21:17.000000 lifted-pddl-1.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5174 2023-06-23 17:21:26.575081 lifted-pddl-1.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4680 2023-06-23 17:21:17.000000 lifted-pddl-1.2.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 17:21:26.575081 lifted-pddl-1.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-06-23 17:21:17.000000 lifted-pddl-1.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 17:21:26.571081 lifted-pddl-1.2.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 17:21:26.575081 lifted-pddl-1.2.2/src/lifted_pddl/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-23 17:21:17.000000 lifted-pddl-1.2.2/src/lifted_pddl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7941 2023-06-23 17:21:17.000000 lifted-pddl-1.2.2/src/lifted_pddl/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 17:21:26.575081 lifted-pddl-1.2.2/src/lifted_pddl/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-06-23 17:21:17.000000 lifted-pddl-1.2.2/src/lifted_pddl/data/blocksworld-domain.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-06-23 17:21:17.000000 lifted-pddl-1.2.2/src/lifted_pddl/data/blocksworld-problem.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-06-23 17:21:17.000000 lifted-pddl-1.2.2/src/lifted_pddl/data/logistics-domain-exists.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-06-23 17:21:17.000000 lifted-pddl-1.2.2/src/lifted_pddl/data/logistics-domain.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     2426 2023-06-23 17:21:17.000000 lifted-pddl-1.2.2/src/lifted_pddl/data/logistics-problem.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     3492 2023-06-23 17:21:17.000000 lifted-pddl-1.2.2/src/lifted_pddl/data/sokoban-domain-no-clear.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-06-23 17:21:17.000000 lifted-pddl-1.2.2/src/lifted_pddl/data/sokoban-problem.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)    34496 2023-06-23 17:21:17.000000 lifted-pddl-1.2.2/src/lifted_pddl/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 17:21:26.575081 lifted-pddl-1.2.2/src/lifted_pddl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5174 2023-06-23 17:21:26.000000 lifted-pddl-1.2.2/src/lifted_pddl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-06-23 17:21:26.000000 lifted-pddl-1.2.2/src/lifted_pddl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 17:21:26.000000 lifted-pddl-1.2.2/src/lifted_pddl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-23 17:21:26.000000 lifted-pddl-1.2.2/src/lifted_pddl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-23 17:21:26.000000 lifted-pddl-1.2.2/src/lifted_pddl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-23 17:21:26.000000 lifted-pddl-1.2.2/src/lifted_pddl.egg-info/top_level.txt
```

### Comparing `lifted-pddl-1.2.1/LICENSE` & `lifted-pddl-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `lifted-pddl-1.2.1/PKG-INFO` & `lifted-pddl-1.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lifted-pddl
-Version: 1.2.1
+Version: 1.2.2
 Summary: A lightweight framework for parsing PDDL in lifted form.
 Home-page: https://github.com/AI-Planning/lifted-pddl
 Author: Carlos Núñez Molina
 Author-email: ccaarlos@ugr.es
 License: MIT
 Keywords: automated_planning PDDL parser
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `lifted-pddl-1.2.1/README.md` & `lifted-pddl-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `lifted-pddl-1.2.1/setup.py` & `lifted-pddl-1.2.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(name='lifted-pddl',
-      version='1.2.1',
+      version='1.2.2',
       description='A lightweight framework for parsing PDDL in lifted form.',
       long_description=long_description,
       long_description_content_type="text/markdown",
       url='https://github.com/AI-Planning/lifted-pddl',
       author='Carlos Núñez Molina',
       author_email='ccaarlos@ugr.es',
       license='MIT',
```

### Comparing `lifted-pddl-1.2.1/src/lifted_pddl/__main__.py` & `lifted-pddl-1.2.2/src/lifted_pddl/__main__.py`

 * *Files identical despite different names*

### Comparing `lifted-pddl-1.2.1/src/lifted_pddl/data/blocksworld-domain.pddl` & `lifted-pddl-1.2.2/src/lifted_pddl/data/blocksworld-domain.pddl`

 * *Files identical despite different names*

### Comparing `lifted-pddl-1.2.1/src/lifted_pddl/data/blocksworld-problem.pddl` & `lifted-pddl-1.2.2/src/lifted_pddl/data/blocksworld-problem.pddl`

 * *Files identical despite different names*

### Comparing `lifted-pddl-1.2.1/src/lifted_pddl/data/logistics-domain-exists.pddl` & `lifted-pddl-1.2.2/src/lifted_pddl/data/logistics-domain-exists.pddl`

 * *Files identical despite different names*

### Comparing `lifted-pddl-1.2.1/src/lifted_pddl/data/logistics-domain.pddl` & `lifted-pddl-1.2.2/src/lifted_pddl/data/logistics-domain.pddl`

 * *Files identical despite different names*

### Comparing `lifted-pddl-1.2.1/src/lifted_pddl/data/logistics-problem.pddl` & `lifted-pddl-1.2.2/src/lifted_pddl/data/logistics-problem.pddl`

 * *Files identical despite different names*

### Comparing `lifted-pddl-1.2.1/src/lifted_pddl/data/sokoban-domain-no-clear.pddl` & `lifted-pddl-1.2.2/src/lifted_pddl/data/sokoban-domain-no-clear.pddl`

 * *Files identical despite different names*

### Comparing `lifted-pddl-1.2.1/src/lifted_pddl/data/sokoban-problem.pddl` & `lifted-pddl-1.2.2/src/lifted_pddl/data/sokoban-problem.pddl`

 * *Files identical despite different names*

### Comparing `lifted-pddl-1.2.1/src/lifted_pddl/parser.py` & `lifted-pddl-1.2.2/src/lifted_pddl/parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -242,17 +242,23 @@
 		atoms = problem.init.as_atoms()
 		self.atoms = set([(atom.predicate.name, tuple([self.object_names.index(obj.name) for obj in atom.subterms])) for atom in atoms])
 
 		# Goals, as a set containing each goal
 		# Each goal is represented as a tuple (is_true, pred_name, object_indexes)
 		# object_indexes is a tuple containing the index of each object the atom of the goal is instantiated on
 		# is_true equals False if the goal is negative (e.g., (not (at t1 l1)) ) and True otherwise
-		subformulas = problem.goal.subformulas
-		self.goals = set([(True, x.predicate.name, tuple(self.object_names.index(obj.name) for obj in x.subterms)) if isinstance(x, Atom) else \
-					  (False, x.subformulas[0].predicate.name, tuple(self.object_names.index(obj.name) for obj in x.subformulas[0].subterms)) for x in subformulas])
+		
+		# The goal contains a single atom (e.g., ( :goal (and (on b2 b1))) )
+		if isinstance(problem.goal, Atom):
+			self.goals = set([(True, problem.goal.predicate.name, tuple(self.object_names.index(obj.name) for obj in problem.goal.subterms))])			
+
+		else: # The goal contains more than a single atom
+			subformulas = problem.goal.subformulas
+			self.goals = set([(True, x.predicate.name, tuple(self.object_names.index(obj.name) for obj in x.subterms)) if isinstance(x, Atom) else \
+						  (False, x.subformulas[0].predicate.name, tuple(self.object_names.index(obj.name) for obj in x.subformulas[0].subterms)) for x in subformulas])
 
 	# Returns the name of the object whose index is @obj_ind
 	def get_object_name(self, obj_ind):
 		assert type(obj_ind) == int, "@obj_ind must be an integer"
 
 		return self.object_names[obj_ind]
```

### Comparing `lifted-pddl-1.2.1/src/lifted_pddl.egg-info/PKG-INFO` & `lifted-pddl-1.2.2/src/lifted_pddl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lifted-pddl
-Version: 1.2.1
+Version: 1.2.2
 Summary: A lightweight framework for parsing PDDL in lifted form.
 Home-page: https://github.com/AI-Planning/lifted-pddl
 Author: Carlos Núñez Molina
 Author-email: ccaarlos@ugr.es
 License: MIT
 Keywords: automated_planning PDDL parser
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `lifted-pddl-1.2.1/src/lifted_pddl.egg-info/SOURCES.txt` & `lifted-pddl-1.2.2/src/lifted_pddl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

