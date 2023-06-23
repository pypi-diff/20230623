# Comparing `tmp/qiskit-xyz2pdb-0.1.1.tar.gz` & `tmp/qiskit-xyz2pdb-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qiskit-xyz2pdb-0.1.1.tar", last modified: Thu Jun 22 18:09:38 2023, max compression
+gzip compressed data, was "qiskit-xyz2pdb-0.1.2.tar", last modified: Fri Jun 23 21:32:08 2023, max compression
```

## Comparing `qiskit-xyz2pdb-0.1.1.tar` & `qiskit-xyz2pdb-0.1.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 raubenb  (871252294) CC\Domain Users (465374370)        0 2023-06-22 18:09:38.782122 qiskit-xyz2pdb-0.1.1/
--rw-r--r--   0 raubenb  (871252294) CC\Domain Users (465374370)     1075 2023-03-24 16:27:34.000000 qiskit-xyz2pdb-0.1.1/LICENSE
--rw-r--r--   0 raubenb  (871252294) CC\Domain Users (465374370)     2592 2023-06-22 18:09:38.781978 qiskit-xyz2pdb-0.1.1/PKG-INFO
--rw-r--r--   0 raubenb  (871252294) CC\Domain Users (465374370)     1665 2023-04-07 19:51:16.000000 qiskit-xyz2pdb-0.1.1/README.md
-drwxr-xr-x   0 raubenb  (871252294) CC\Domain Users (465374370)        0 2023-06-22 18:09:38.781550 qiskit-xyz2pdb-0.1.1/qiskit_xyz2pdb.egg-info/
--rw-r--r--   0 raubenb  (871252294) CC\Domain Users (465374370)     2592 2023-06-22 18:09:38.000000 qiskit-xyz2pdb-0.1.1/qiskit_xyz2pdb.egg-info/PKG-INFO
--rw-r--r--   0 raubenb  (871252294) CC\Domain Users (465374370)      295 2023-06-22 18:09:38.000000 qiskit-xyz2pdb-0.1.1/qiskit_xyz2pdb.egg-info/SOURCES.txt
--rw-r--r--   0 raubenb  (871252294) CC\Domain Users (465374370)        1 2023-06-22 18:09:38.000000 qiskit-xyz2pdb-0.1.1/qiskit_xyz2pdb.egg-info/dependency_links.txt
--rw-r--r--   0 raubenb  (871252294) CC\Domain Users (465374370)       56 2023-06-22 18:09:38.000000 qiskit-xyz2pdb-0.1.1/qiskit_xyz2pdb.egg-info/entry_points.txt
--rw-r--r--   0 raubenb  (871252294) CC\Domain Users (465374370)        1 2023-06-22 18:09:38.000000 qiskit-xyz2pdb-0.1.1/qiskit_xyz2pdb.egg-info/not-zip-safe
--rw-r--r--   0 raubenb  (871252294) CC\Domain Users (465374370)        8 2023-06-22 18:09:38.000000 qiskit-xyz2pdb-0.1.1/qiskit_xyz2pdb.egg-info/top_level.txt
--rw-r--r--   0 raubenb  (871252294) CC\Domain Users (465374370)       38 2023-06-22 18:09:38.782172 qiskit-xyz2pdb-0.1.1/setup.cfg
--rw-r--r--   0 raubenb  (871252294) CC\Domain Users (465374370)     1675 2023-04-07 19:39:33.000000 qiskit-xyz2pdb-0.1.1/setup.py
-drwxr-xr-x   0 raubenb  (871252294) CC\Domain Users (465374370)        0 2023-06-22 18:09:38.781796 qiskit-xyz2pdb-0.1.1/xyz2pdb/
--rw-r--r--   0 raubenb  (871252294) CC\Domain Users (465374370)        0 2023-03-24 16:27:34.000000 qiskit-xyz2pdb-0.1.1/xyz2pdb/__init__.py
--rw-r--r--   0 raubenb  (871252294) CC\Domain Users (465374370)    11212 2023-06-22 18:08:33.000000 qiskit-xyz2pdb-0.1.1/xyz2pdb/xyz2pdb.py
+drwxr-xr-x   0 raubenb  (871252294) CC\Domain Users (465374370)        0 2023-06-23 21:32:08.077980 qiskit-xyz2pdb-0.1.2/
+-rw-r--r--   0 raubenb  (871252294) CC\Domain Users (465374370)     1075 2023-03-24 16:27:34.000000 qiskit-xyz2pdb-0.1.2/LICENSE
+-rw-r--r--   0 raubenb  (871252294) CC\Domain Users (465374370)     2612 2023-06-23 21:32:08.077802 qiskit-xyz2pdb-0.1.2/PKG-INFO
+-rw-r--r--   0 raubenb  (871252294) CC\Domain Users (465374370)     1665 2023-04-07 19:51:16.000000 qiskit-xyz2pdb-0.1.2/README.md
+drwxr-xr-x   0 raubenb  (871252294) CC\Domain Users (465374370)        0 2023-06-23 21:32:08.077316 qiskit-xyz2pdb-0.1.2/qiskit_xyz2pdb.egg-info/
+-rw-r--r--   0 raubenb  (871252294) CC\Domain Users (465374370)     2612 2023-06-23 21:32:07.000000 qiskit-xyz2pdb-0.1.2/qiskit_xyz2pdb.egg-info/PKG-INFO
+-rw-r--r--   0 raubenb  (871252294) CC\Domain Users (465374370)      295 2023-06-23 21:32:08.000000 qiskit-xyz2pdb-0.1.2/qiskit_xyz2pdb.egg-info/SOURCES.txt
+-rw-r--r--   0 raubenb  (871252294) CC\Domain Users (465374370)        1 2023-06-23 21:32:07.000000 qiskit-xyz2pdb-0.1.2/qiskit_xyz2pdb.egg-info/dependency_links.txt
+-rw-r--r--   0 raubenb  (871252294) CC\Domain Users (465374370)       56 2023-06-23 21:32:07.000000 qiskit-xyz2pdb-0.1.2/qiskit_xyz2pdb.egg-info/entry_points.txt
+-rw-r--r--   0 raubenb  (871252294) CC\Domain Users (465374370)        1 2023-06-23 21:32:07.000000 qiskit-xyz2pdb-0.1.2/qiskit_xyz2pdb.egg-info/not-zip-safe
+-rw-r--r--   0 raubenb  (871252294) CC\Domain Users (465374370)        8 2023-06-23 21:32:08.000000 qiskit-xyz2pdb-0.1.2/qiskit_xyz2pdb.egg-info/top_level.txt
+-rw-r--r--   0 raubenb  (871252294) CC\Domain Users (465374370)       38 2023-06-23 21:32:08.078050 qiskit-xyz2pdb-0.1.2/setup.cfg
+-rw-r--r--   0 raubenb  (871252294) CC\Domain Users (465374370)     1675 2023-04-07 19:39:33.000000 qiskit-xyz2pdb-0.1.2/setup.py
+drwxr-xr-x   0 raubenb  (871252294) CC\Domain Users (465374370)        0 2023-06-23 21:32:08.077562 qiskit-xyz2pdb-0.1.2/xyz2pdb/
+-rw-r--r--   0 raubenb  (871252294) CC\Domain Users (465374370)        0 2023-03-24 16:27:34.000000 qiskit-xyz2pdb-0.1.2/xyz2pdb/__init__.py
+-rw-r--r--   0 raubenb  (871252294) CC\Domain Users (465374370)    12306 2023-06-23 21:19:27.000000 qiskit-xyz2pdb-0.1.2/xyz2pdb/xyz2pdb.py
```

### Comparing `qiskit-xyz2pdb-0.1.1/LICENSE` & `qiskit-xyz2pdb-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `qiskit-xyz2pdb-0.1.1/PKG-INFO` & `qiskit-xyz2pdb-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: qiskit-xyz2pdb
-Version: 0.1.1
+Version: 0.1.2
 Summary: A simple Python package to convert XYZ files from Qiskit output into PDB structures
 Home-page: http://github.com/thepineapplepirate/qiskit-xyz2pdb
 Download-URL: https://pypi.org/project/qiskit-xyz2pdb/
 Author: Bryan Raubenolt
 Author-email: raubenb@ccf.org
 License: MIT
 Project-URL: Issues, https://github.com/thepineapplepirate/qiskit-xyz2pdb/issues
 Project-URL: Source, https://github.com/thepineapplepirate/qiskit-xyz2pdb
 Keywords: bioinformatics,chemistry,pdb,proteins,qiskit,quantum
+Platform: UNKNOWN
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Requires-Python: >=3.6
@@ -45,7 +46,9 @@
 ```
 
 The conventional alpha carbon trace format is more versatile and can be used for further research beyond visualization - such as reconstructing the full backbone and sidechains, adding a force field, and then performing molecular dynamics simulations. How to run with this option:
 
 ```
 $ qiskit-xyz2pdb --in-xyz inputfile.xyz --out-pdb outputfile.pdb --alpha-c-traces
 ```
+
+
```

### Comparing `qiskit-xyz2pdb-0.1.1/README.md` & `qiskit-xyz2pdb-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `qiskit-xyz2pdb-0.1.1/qiskit_xyz2pdb.egg-info/PKG-INFO` & `qiskit-xyz2pdb-0.1.2/qiskit_xyz2pdb.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: qiskit-xyz2pdb
-Version: 0.1.1
+Version: 0.1.2
 Summary: A simple Python package to convert XYZ files from Qiskit output into PDB structures
 Home-page: http://github.com/thepineapplepirate/qiskit-xyz2pdb
 Download-URL: https://pypi.org/project/qiskit-xyz2pdb/
 Author: Bryan Raubenolt
 Author-email: raubenb@ccf.org
 License: MIT
 Project-URL: Issues, https://github.com/thepineapplepirate/qiskit-xyz2pdb/issues
 Project-URL: Source, https://github.com/thepineapplepirate/qiskit-xyz2pdb
 Keywords: bioinformatics,chemistry,pdb,proteins,qiskit,quantum
+Platform: UNKNOWN
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Requires-Python: >=3.6
@@ -45,7 +46,9 @@
 ```
 
 The conventional alpha carbon trace format is more versatile and can be used for further research beyond visualization - such as reconstructing the full backbone and sidechains, adding a force field, and then performing molecular dynamics simulations. How to run with this option:
 
 ```
 $ qiskit-xyz2pdb --in-xyz inputfile.xyz --out-pdb outputfile.pdb --alpha-c-traces
 ```
+
+
```

### Comparing `qiskit-xyz2pdb-0.1.1/setup.py` & `qiskit-xyz2pdb-0.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `qiskit-xyz2pdb-0.1.1/xyz2pdb/xyz2pdb.py` & `qiskit-xyz2pdb-0.1.2/xyz2pdb/xyz2pdb.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,22 +4,24 @@
 """
 
 __authors__ = ("Bryan Raubenolt (raubenb@ccf.org)",
                "Fabio Cumbo (cumbof@ccf.org)",
                "Jayadev Joshi (joshij@ccf.org)",
                "Daniel Blankenberg (blanked2@ccf.org)")
 
-__version__ = "0.1.1"
-__date__ = "Jun 22, 2023"
+__version__ = "0.1.2"
+__date__ = "Jun 23, 2023"
 
 import argparse as ap
 import errno
 import os
 from functools import partial
-from typing import List, Union
+from typing import List, Union, Optional
+
+import numpy as np
 
 TOOL_ID = "qiskit-xyz2pdb"
 
 # Residue names
 # Used in case of --alpha-c-traces only
 RESIDUES = {
     "A": "ALA",
@@ -61,19 +63,24 @@
         "--in-xyz",
         type=os.path.abspath,
         required=True,
         dest="in_xyz",
         help="Path to the XYZ input file from Qiskit output",
     )
     p.add_argument(
-        "--out-pdb",
+        "--out-name",
+        type=str,
+        dest="out_name",
+        help="Name of the output PDB file",
+    )
+    p.add_argument(
+        "--out-folder",
         type=os.path.abspath,
-        required=True,
-        dest="out_pdb",
-        help="Path to the output PDB file",
+        dest="out_folder",
+        help="Path to the output folder",
     )
     p.add_argument(
         "--alpha-c-traces",
         action="store_true",
         default=False,
         dest="alpha_c_trace",
         help="Add C(alpha) traces",
@@ -169,47 +176,64 @@
         occupancy,
         temperature_factor,
         element_symbol,
         charge_on_the_atom
     )
 
 
-def load_xyz_data(xyz_filepath: os.path.abspath) -> List[List[Union[str, int, float]]]:
+def load_xyz_data(xyz_filepath: os.path.abspath) -> np.ndarray:
     """
     Load a XYZ file as defined by qiskit
 
     :param xyz_filepath:    Path to the XYZ file
-    :return:                A list of lists with the content of the XYZ file
+    :return:                A list of lists as numpy.ndarray with the content of the XYZ file
     """
 
     if not os.path.isfile(xyz_filepath):
         raise FileNotFoundError(errno.ENOENT, os.strerror(errno.ENOENT), xyz_filepath)
 
-    return [line.strip().split(" ") for line in open(xyz_filepath).readlines() if line.strip() and len(line.strip().split(" ")) == 4]
+    return np.array([line.strip().split(" ") for line in open(xyz_filepath).readlines() if line.strip() and len(line.strip().split(" ")) == 4])
 
 
 def build_pdb(
-    xyz_list: List[List[Union[str, int, float]]],
-    out_pdb: os.path.abspath,
+    xyz_list: Union[List[List[Union[str, int, float]]], np.ndarray],
+    out_pdb_name: Optional[str]=None,
+    out_pdb_folder: Optional[os.path.abspath]=None,
     alpha_c_trace: bool=False,
-    hetero_atoms: bool=False
+    hetero_atoms: bool=False,
+    replace: bool=False
 ) -> None:
     """
-    Convert an XYZ list to a PDB file
+    Convert an XYZ list to a PDB file.
+    The output PDB file name is optional. In case of None, it is automatically defined based on the series on aminoacids in xyz_list.
+    The output folder path is also optional. In case of None, the output file is saved into the current working directory.
 
     :param xyz_list:        List of lists with the content of the XYZ file (see load_xyz_data)
-    :param out_pdb:         Path to the output PDB file
+    :param out_pdb_name:    Name of the output PDB file. Optional
+    :param out_pdb_folder:  Path to the folder of the output PDB file. Optional
     :param alpha_c_trace:   Add C(alpha) traces
     :param hetero_atoms:    Add hetero atoms
+    :param replace:         Overwrite the output file if it exists
     """
 
+    if isinstance(xyz_list, np.ndarray):
+        xyz_list = xyz_list.tolist()
+
     if not xyz_list:
-        raise ValueError("The XYZ list is empty!")
+        raise ValueError("The input XYZ is empty!")
 
-    if os.path.isfile(out_pdb):
+    if not out_pdb_name:
+        out_pdb_name = "".join([str(values[0]) for values in xyz_list])
+
+    if not out_pdb_folder:
+        out_pdb_folder = os.getcwd()
+
+    out_pdb = os.path.join(out_pdb_folder, "{}.pdb".format(out_pdb_name))
+
+    if os.path.isfile(out_pdb) and not replace:
         raise Exception("The output PDB file already exists")
 
     if (alpha_c_trace and hetero_atoms) or (not alpha_c_trace and not hetero_atoms):
         raise Exception(
             ("Please use one of the following flags: [--alpha-c-traces; --hetero-atoms]\n"
              "Use --help for additional details")
         )
@@ -326,12 +350,18 @@
 def main() -> None:
     args = read_params()
 
     # Load the XYZ file into a list of lists
     xyz_list = load_xyz_data(args.in_xyz)
 
     # Convert the XYZ list to PDB
-    build_pdb(xyz_list, args.out_pdb, alpha_c_trace=args.alpha_c_trace, hetero_atoms=args.hetero_atoms)
+    build_pdb(
+        xyz_list,
+        out_pdb_name=args.out_name,
+        out_pdb_folder=args.out_folder,
+        alpha_c_trace=args.alpha_c_trace,
+        hetero_atoms=args.hetero_atoms
+    )
 
 
 if __name__ == "__main__":
     main()
```

