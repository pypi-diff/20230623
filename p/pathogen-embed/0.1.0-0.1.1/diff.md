# Comparing `tmp/pathogen-embed-0.1.0.tar.gz` & `tmp/pathogen-embed-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/jlhudd/projects/cartography/source/dist/tmp9clnm8ru/pathogen-embed-0.1.0.tar", last modified: Fri Mar  4 23:02:47 2022, max compression
+gzip compressed data, was "pathogen-embed-0.1.1.tar", last modified: Thu Jun 22 23:30:59 2023, max compression
```

## Comparing `pathogen-embed-0.1.0.tar` & `pathogen-embed-0.1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 jlhudd     (501) staff       (20)        0 2022-03-04 23:02:47.000000 pathogen-embed-0.1.0/
--rw-r--r--   0 jlhudd     (501) staff       (20)     1068 2022-03-04 22:43:49.000000 pathogen-embed-0.1.0/LICENSE
--rw-r--r--   0 jlhudd     (501) staff       (20)     3430 2022-03-04 23:02:47.000000 pathogen-embed-0.1.0/PKG-INFO
--rw-r--r--   0 jlhudd     (501) staff       (20)     2478 2022-03-04 22:43:49.000000 pathogen-embed-0.1.0/README.md
--rw-r--r--   0 jlhudd     (501) staff       (20)      103 2022-03-04 22:43:49.000000 pathogen-embed-0.1.0/pyproject.toml
--rw-r--r--   0 jlhudd     (501) staff       (20)       38 2022-03-04 23:02:47.000000 pathogen-embed-0.1.0/setup.cfg
--rw-r--r--   0 jlhudd     (501) staff       (20)     1766 2022-03-04 22:57:30.000000 pathogen-embed-0.1.0/setup.py
-drwxr-xr-x   0 jlhudd     (501) staff       (20)        0 2022-03-04 23:02:47.000000 pathogen-embed-0.1.0/src/
-drwxr-xr-x   0 jlhudd     (501) staff       (20)        0 2022-03-04 23:02:47.000000 pathogen-embed-0.1.0/src/embed/
--rw-r--r--   0 jlhudd     (501) staff       (20)     4867 2022-03-04 22:45:45.000000 pathogen-embed-0.1.0/src/embed/__init__.py
--rw-r--r--   0 jlhudd     (501) staff       (20)      337 2022-03-04 22:43:49.000000 pathogen-embed-0.1.0/src/embed/__main__.py
--rw-r--r--   0 jlhudd     (501) staff       (20)     9681 2022-03-04 22:45:45.000000 pathogen-embed-0.1.0/src/embed/embed.py
-drwxr-xr-x   0 jlhudd     (501) staff       (20)        0 2022-03-04 23:02:47.000000 pathogen-embed-0.1.0/src/pathogen_embed.egg-info/
--rw-r--r--   0 jlhudd     (501) staff       (20)     3430 2022-03-04 23:02:46.000000 pathogen-embed-0.1.0/src/pathogen_embed.egg-info/PKG-INFO
--rw-r--r--   0 jlhudd     (501) staff       (20)      358 2022-03-04 23:02:47.000000 pathogen-embed-0.1.0/src/pathogen_embed.egg-info/SOURCES.txt
--rw-r--r--   0 jlhudd     (501) staff       (20)        1 2022-03-04 23:02:46.000000 pathogen-embed-0.1.0/src/pathogen_embed.egg-info/dependency_links.txt
--rw-r--r--   0 jlhudd     (501) staff       (20)       46 2022-03-04 23:02:46.000000 pathogen-embed-0.1.0/src/pathogen_embed.egg-info/entry_points.txt
--rw-r--r--   0 jlhudd     (501) staff       (20)       74 2022-03-04 23:02:47.000000 pathogen-embed-0.1.0/src/pathogen_embed.egg-info/requires.txt
--rw-r--r--   0 jlhudd     (501) staff       (20)        6 2022-03-04 23:02:47.000000 pathogen-embed-0.1.0/src/pathogen_embed.egg-info/top_level.txt
+drwxrwxrwx   0 nandsra   (1000) nandsra   (1000)        0 2023-06-22 23:30:59.665323 pathogen-embed-0.1.1/
+-rwxrwxrwx   0 nandsra   (1000) nandsra   (1000)     1068 2023-06-21 05:19:15.000000 pathogen-embed-0.1.1/LICENSE
+-rwxrwxrwx   0 nandsra   (1000) nandsra   (1000)     4810 2023-06-22 23:30:59.658745 pathogen-embed-0.1.1/PKG-INFO
+-rwxrwxrwx   0 nandsra   (1000) nandsra   (1000)     3879 2023-06-22 23:23:27.000000 pathogen-embed-0.1.1/README.md
+-rwxrwxrwx   0 nandsra   (1000) nandsra   (1000)      103 2022-01-21 05:41:32.000000 pathogen-embed-0.1.1/pyproject.toml
+-rwxrwxrwx   0 nandsra   (1000) nandsra   (1000)       38 2023-06-22 23:30:59.667792 pathogen-embed-0.1.1/setup.cfg
+-rwxrwxrwx   0 nandsra   (1000) nandsra   (1000)     1764 2023-06-22 23:26:13.000000 pathogen-embed-0.1.1/setup.py
+drwxrwxrwx   0 nandsra   (1000) nandsra   (1000)        0 2023-06-22 23:30:58.639024 pathogen-embed-0.1.1/src/
+drwxrwxrwx   0 nandsra   (1000) nandsra   (1000)        0 2023-06-22 23:30:59.136146 pathogen-embed-0.1.1/src/embed/
+-rwxrwxrwx   0 nandsra   (1000) nandsra   (1000)     5341 2023-06-21 15:35:01.000000 pathogen-embed-0.1.1/src/embed/__init__.py
+-rwxrwxrwx   0 nandsra   (1000) nandsra   (1000)      337 2022-01-21 05:41:32.000000 pathogen-embed-0.1.1/src/embed/__main__.py
+-rwxrwxrwx   0 nandsra   (1000) nandsra   (1000)    13721 2023-01-12 19:45:51.000000 pathogen-embed-0.1.1/src/embed/embed.py
+drwxrwxrwx   0 nandsra   (1000) nandsra   (1000)        0 2023-06-22 23:30:59.591062 pathogen-embed-0.1.1/src/pathogen_embed.egg-info/
+-rwxrwxrwx   0 nandsra   (1000) nandsra   (1000)     4810 2023-06-22 23:30:58.000000 pathogen-embed-0.1.1/src/pathogen_embed.egg-info/PKG-INFO
+-rwxrwxrwx   0 nandsra   (1000) nandsra   (1000)      358 2023-06-22 23:30:58.000000 pathogen-embed-0.1.1/src/pathogen_embed.egg-info/SOURCES.txt
+-rwxrwxrwx   0 nandsra   (1000) nandsra   (1000)        1 2023-06-22 23:30:58.000000 pathogen-embed-0.1.1/src/pathogen_embed.egg-info/dependency_links.txt
+-rwxrwxrwx   0 nandsra   (1000) nandsra   (1000)       46 2023-06-22 23:30:58.000000 pathogen-embed-0.1.1/src/pathogen_embed.egg-info/entry_points.txt
+-rwxrwxrwx   0 nandsra   (1000) nandsra   (1000)       74 2023-06-22 23:30:58.000000 pathogen-embed-0.1.1/src/pathogen_embed.egg-info/requires.txt
+-rwxrwxrwx   0 nandsra   (1000) nandsra   (1000)        6 2023-06-22 23:30:58.000000 pathogen-embed-0.1.1/src/pathogen_embed.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pathogen-embed-0.1.0/LICENSE` & `pathogen-embed-0.1.1/LICENSE`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2019 Bedford Lab
+Copyright (c) 2023 Bedford Lab
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `pathogen-embed-0.1.0/PKG-INFO` & `pathogen-embed-0.1.1/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,53 +1,76 @@
-Metadata-Version: 2.1
-Name: pathogen-embed
-Version: 0.1.0
-Summary: Reduced dimension embeddings for pathogen sequences
-Home-page: https://github.com/blab/cartography/
-Author: Sravani Nanduri <nandsra@cs.washington.edu> , John Huddleston <huddlej@gmail.com>
-Author-email: nandsra@cs.washington.edu
-License: MIT License
-Project-URL: Documentation, https://blab.github.io/cartography/
-Project-URL: Bug Reports, https://github.com/blab/cartography/issues
-Project-URL: Source Code, https://github.com/blab/cartography/tree/master/source
-Project-URL: Change Log, https://github.com/blab/cartography/tree/master/source/CHANGES.md
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: OS Independent
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
+# pathogen-embed
+Create reduced dimension embeddings for pathogen sequences
 
-# Cartography
-Reduced dimension embeddings for pathogen sequences
 
+pathogen-embed is an open-source software for scientists, epidemiologists, etc. to run reduced dimension embeddings (PCA, MDS, t-SNE, and UMAP) on viral populations. This is the source code from the paper Cartography written by Sravani Nanduri and John Huddleston.
+
+[Documentation](https://blab.github.io/pathogen-embed/)\
+[Source Code](https://github.com/blab/pathogen-embed/tree/main)\
+[Bug reports](https://github.com/blab/pathogen-embed/issues)
+
+# Build documentation  
+Build the [Documentation](https://blab.github.io/pathogen-embed/):
+
+``` make -C /docs html ```
+
+Clean the docs.
+
+``` make -C /docs clean ```
+
+# Releasing a new version
+
+### Information about each file
+
+#### README.md
+
+contains the description of the package pathogen-embed.
+
+#### setup.py
+
+Gives PyPi the instructions about where to find dependent packages, the authors and relevant links, etc. Also gives the entry points for the console script, which tells Pypi to call the main function of __main__.py. 
+
+#### __init__.py
+
+Initializes the package, creates the parser to parse the command line arguments and pass them into the embed.py function.
 
-Cartography is an open-source software for scientists, epidemiologists, etc. to run reduced dimension embeddings (PCA, MDS, t-SNE, and UMAP) on viral populations. This is the source code from the paper Cartography written by Sravani Nanduri and John Huddleston.
+#### __main__.py
 
-[Documentation](https://blab.github.io/cartography/)\
-[Source Code](https://github.com/blab/cartography/tree/master/source)\
-[Bug reports](https://github.com/blab/cartography/issues)
+Calls the "run" function in __init__.py, which calls embed.py. 
 
+#### embed.py
+
+The main code for the package.
+
+# To create new version 
+
+Run 
+
+``` python3 -m build ``` 
+
+This creates the dist folder that gets uploaded to pypi.
+
+``` python3 -m twine upload dist/* ```
+
+Input the username and password, upload new dist files to pypi. Make sure the version of the dist folders does not already exist within pypi. 
 
 
 ## Installing the package
 
 Simply install the package using pip.
 
 ```
 pip install pathogen-embed
 ```
 
 # src.embed module
 
 ## Command line interface
 
-The full [Documentation](https://blab.github.io/cartography/). 
+The full [Documentation](https://blab.github.io/pathogen-embed/). 
 
 The below documentation does not detail the named and positional arguments. 
 
 Reduced dimension embeddings for pathogen sequences
 
 
 ```
@@ -125,8 +148,19 @@
 >>> get_hamming_distances(genomes)
 [0, 1, 1]
 >>> genomes = ["AT-GCT", "AT--CT", "AC--CT"]
 >>> get_hamming_distances(genomes)
 [0, 1, 1]
 ```
 
+# Issues and fixes:
+
+Issue/Fix: Used sphinx-book-theme version 0.3.3 for backwards compatibility (wouldn't render otherwise)
+
+Issue: index.rst: Module "src" has no attribute "make_parser"
+Incorrect argparse :module: or :func: values?
+
+Fix: changed module from src to src.embed
+
+
+
```

### Comparing `pathogen-embed-0.1.0/setup.py` & `pathogen-embed-0.1.1/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,27 +3,27 @@
 
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='pathogen-embed',
-    version='0.1.0',
+    version='0.1.1',
     description='Reduced dimension embeddings for pathogen sequences',
-    url='https://github.com/blab/cartography/',
+    url='https://github.com/blab/pathogen-embed/',
     author='Sravani Nanduri <nandsra@cs.washington.edu> , John Huddleston <huddlej@gmail.com>',
     author_email='nandsra@cs.washington.edu',
     long_description=long_description,
     long_description_content_type="text/markdown",
     license='MIT License',
     project_urls = {
-        "Documentation": "https://blab.github.io/cartography/",
-        "Bug Reports": "https://github.com/blab/cartography/issues",
-        "Source Code": "https://github.com/blab/cartography/tree/master/source",
-		"Change Log": "https://github.com/blab/cartography/tree/master/source/CHANGES.md",
+        "Documentation": "https://blab.github.io/pathogen-embed/",
+        "Bug Reports": "https://github.com/blab/pathogen-embed/issues",
+        "Source Code": "https://github.com/blab/pathogen-embed/tree/main",
+	"Change Log": "https://github.com/blab/pathogen-embed/tree/master/CHANGES.md",
     },
     package_dir={"": "src"},
 	packages = find_packages(where="src", exclude=['test']),
     #packages=['seaborn', 'scikit-learn', 'umap-learn', 'matplotlib', 'pandas', 'numpy', 'hdbscan'],
     install_requires=['numpy',
                       'pandas',
                       "biopython",
```

### Comparing `pathogen-embed-0.1.0/src/embed/__init__.py` & `pathogen-embed-0.1.1/src/embed/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 """
 pathogen-embed.
 
 Reduced dimension embeddings for pathogen sequences.
 """
 
-__version__ = "0.0.2"
+__version__ = "0.1.0"
 __author__ = 'Sravani Nanduri, John Huddleston'
 __credits__ = 'Bedford Lab, Vaccine and Infectious Disease Division, Fred Hutchinson Cancer Research Center, Seattle, WA, USA'
 
 import argparse
 import sys
-from .embed import embed
+from .embed import embed, get_hamming_distances
 
 def make_parser():
     parser = argparse.ArgumentParser(description = "Reduced dimension embeddings for pathogen sequences", formatter_class=argparse.ArgumentDefaultsHelpFormatter)
 
     parser.add_argument("--distance-matrix", help="a distance matrix that can be read in by pandas, index column as row 0")
     parser.add_argument("--separator", default=",", help="separator between columns in the given distance matrix")
     parser.add_argument("--alignment", help="an aligned FASTA file to create a distance matrix with. Make sure the strain order in this file matches the order in the distance matrix.")
     parser.add_argument("--cluster-data", help="The file (same separator as distance-matrix) that contains the distance threshold by which to cluster data in the embedding and assign labels given via HDBSCAN (https://hdbscan.readthedocs.io/en/latest/how_hdbscan_works.html). If no value is given in cluster-data or cluster-threshold, the default distance threshold of 0.0 will be used. If any additional columns in this file match embedding-specific parameters (e.g., 'n_components' or 'learning_rate'), the values from the first record of this file will override default values or values provided by the command line arguments.")
+    parser.add_argument("--cluster-min-size", type=int, default=5, help="minimum cluster size for HDBSCAN")
+    parser.add_argument("--cluster-min-samples", type=int, default=5, help="minimum number of sample to seed a cluster for HDBSCAN. Lowering this value reduces number of samples that do not get clustered.")
     parser.add_argument("--cluster-threshold", type=float, help="The float value for the distance threshold by which to cluster data in the embedding and assign labels via HDBSCAN. If no value is given in cluster-data or cluster-threshold, the default distance threshold of 0.0 will be used.")
     parser.add_argument("--random-seed", default = 314159, type=int, help="an integer used for reproducible results.")
+    parser.add_argument("--indel-distance", action="store_true", help="include insertions/deletions in genetic distance calculations")
     parser.add_argument("--output-dataframe", help="a csv file outputting the embedding with the strain name and its components.")
     parser.add_argument("--output-figure", help="outputs a PNG plot of the embedding")
 
     subparsers = parser.add_subparsers(
         dest="command",
         required=True
     )
@@ -51,8 +54,8 @@
 
 def run(argv):
     args = make_parser().parse_args(argv)
     try:
         return embed(args)
     except Exception as error:
         print(error, file=sys.stderr)
-        sys.exit(1)
+        sys.exit(1)
```

### Comparing `pathogen-embed-0.1.0/src/embed/embed.py` & `pathogen-embed-0.1.1/src/embed/embed.py`

 * *Files 21% similar despite different names*

```diff
@@ -11,42 +11,113 @@
 import seaborn as sns
 from sklearn.decomposition import PCA
 from sklearn.manifold import TSNE, MDS
 import sys
 from umap import UMAP
 
 
-def get_hamming_distances(genomes):
+def find_ranges(positions):
+    """
+    Find ranges of adjacent integers in the given list of integers and
+    return a dictionary of gap lengths indexed by start position.
+
+    >>> find_ranges([])
+    {}
+    >>> find_ranges([0])
+    {0: 1}
+    >>> find_ranges([0, 2, 3, 4])
+    {0: 1, 2: 3}
+    >>> find_ranges([2, 3, 4])
+    {2: 3}
+    >>> find_ranges([2, 3, 4, 6, 7, 9])
+    {2: 3, 6: 2, 9: 1}
+
+    """
+    ranges = {}
+    start = 0
+    end = 0
+    for i in range(len(positions)):
+        # If the next position is one greater than the current position, update
+        # the end point to the next position.
+        if i < len(positions) - 1 and positions[i] + 1 == positions[i + 1]:
+            end = i + 1
+        # Otherwise, if the next position is more than one away or we're at the
+        # end of the list, save the current range and set the next range to
+        # start and end at the next position.
+        else:
+            # If the range is a singleton, output only that value. Otherwise,
+            # output the range from start to end.
+            ranges[positions[start]] = end - start + 1
+
+            start = i + 1
+            end = i + 1
+
+    return ranges
+
+
+def get_hamming_distances(genomes, count_indels=False):
     """Calculate pairwise Hamming distances between the given list of genomes
     and return the nonredundant array of values for use with scipy's squareform function.
-    Bases other than standard nucleotides (A, T, C, G) are ignored.
+    Bases other than standard nucleotides (A, T, C, G) are ignored. Treat indels as a single event.
 
     Parameters
     ----------
     genomes : list
         a list of strings corresponding to genomes that should be compared
+    count_indels : boolean
+        true means indels are counted in the distance calculation, false if not.
+        the default value is false.
 
     Returns
     -------
     list
         a list of distinct Hamming distances as a vector-form distance vector
 
+    >>> genomes = ["ATGCT", "ATGCT", "ACGCT"]
+    >>> get_hamming_distances(genomes, True)
+    [0, 1, 1]
+    >>> get_hamming_distances(["AT--CT", "AC--CT"], True)
+    [1]
+    >>> genomes = ["AT-GCT", "AT--CT", "AC--CT"]
+    >>> get_hamming_distances(genomes, True)
+    [1, 2, 1]
+    >>> genomes = ["ACTGG", "A--GN", "A-NGG"]
+    >>> get_hamming_distances(genomes, True)
+    [1, 1, 1]
+
+    When counting indels, we ignore leading and trailing gaps that indicate
+    different sequence lengths and not biological events.
+
+    >>> genomes = ["ACTGTA", "A--CCA", "A--GT-"]
+    >>> get_hamming_distances(genomes, True)
+    [3, 1, 2]
+    >>> genomes = ["ACTGTA", "A--CCA", "---GT-"]
+    >>> get_hamming_distances(genomes, True)
+    [3, 0, 2]
+
+    When not counting indels, we ignore gaps altogether.
 
     >>> genomes = ["ATGCT", "ATGCT", "ACGCT"]
     >>> get_hamming_distances(genomes)
     [0, 1, 1]
     >>> genomes = ["AT-GCT", "AT--CT", "AC--CT"]
     >>> get_hamming_distances(genomes)
     [0, 1, 1]
+    >>> genomes = ["ACTGG", "A--GN", "A-NGG"]
+    >>> get_hamming_distances(genomes)
+    [0, 0, 0]
+    >>> genomes = ["ACTGTA", "A--CCA", "A--GT-"]
+    >>> get_hamming_distances(genomes)
+    [2, 0, 2]
 
     """
+
     # Define an array of valid nucleotides to use in pairwise distance calculations.
     # Using a numpy array of byte strings allows us to apply numpy.isin later.
-
-    nucleotides = np.array([b'A', b'T', b'C', b'G', b'a', b't', b'c', b'g']) # take into account lowercase letters as well as uppercase
+    nucleotides = np.array([b'A', b'T', b'C', b'G'])
 
     # Convert genome strings into numpy arrays to enable vectorized comparisons.
     genome_arrays = [
         np.frombuffer(genome.encode(), dtype="S1")
         for genome in genomes
     ]
 
@@ -56,35 +127,64 @@
         for genome_array in genome_arrays
     ]
 
     # Calculate Hamming distance between all distinct pairs of genomes at valid bases.
     # The resulting list is a reduced representation of a symmetric matrix that can be
     # converted to a square matrix with scipy's squareform function:
     # https://docs.scipy.org/doc/scipy/reference/generated/scipy.spatial.distance.squareform.html
+    total_genomes = len(genomes)
+    alignment_length = len(genomes[0])
     hamming_distances = []
-    for i in range(len(genomes)):
+    for i in range(total_genomes):
         # Only compare the current genome, i, with all later genomes.
         # This avoids repeating comparisons or comparing each genome to itself.
-        for j in range(i + 1, len(genomes)):
-            # Find all mismatches between these two genomes.
-            mismatches = genome_arrays[i] != genome_arrays[j]
+        if count_indels:
+            i_gaps = np.where(genome_arrays[i] == b"-")
+            i_gap_ranges = find_ranges(i_gaps[0])
+
+        for j in range(i + 1, total_genomes):
+            # Find all mismatches at valid nucleotide bases.
+            distance = ((genome_arrays[i] != genome_arrays[j]) & valid_bases[i] & valid_bases[j]).sum()
+
+            if count_indels:
+                j_gaps = np.where(genome_arrays[j] == b"-")
+                j_gap_ranges = find_ranges(j_gaps[0])
+
+                # Mismatched gaps include total number of different start
+                # positions plus the number of the same start positions with
+                # different lengths. Note that we ignore gaps that start at the
+                # beginning of the alignment which occur because of differing
+                # sequence lengths and not necessarily a biological event.
+                num_indel = 0
+                for gap_start, gap_length  in j_gap_ranges.items():
+                    # Skip leading gaps.
+                    if gap_start == 0:
+                        continue
+
+                    # Skip trailing gaps.
+                    if gap_start + gap_length == alignment_length:
+                        continue
+
+                    if gap_start not in i_gap_ranges or i_gap_ranges[gap_start] != gap_length:
+                        num_indel += 1
+
+                distance += num_indel
 
-            # Count the number of mismatches where both genomes have valid bases.
-            hamming_distances.append((mismatches & valid_bases[i] & valid_bases[j]).sum())
+            hamming_distances.append(distance)
 
     return hamming_distances
 
 
 def embed(args):
     # TODO: Create a default cluster distance threshold if none given.
 
     # Setting Random seed for numpy
     np.random.seed(seed=args.random_seed)
 
-    if args.output_dataframe is None:
+    if args.output_dataframe is None and args.output_figure is None:
         print("You must specify one of the outputs", file=sys.stderr)
         sys.exit(1)
 
     if args.alignment is None and args.command == "pca":
         print("You must specify an alignment for pca, not a distance matrix", file=sys.stderr)
         sys.exit(1)
 
@@ -99,42 +199,56 @@
         for sequence in Bio.SeqIO.parse(args.alignment, "fasta"):
             sequences_by_name[sequence.id] = str(sequence.seq)
 
         sequence_names = list(sequences_by_name.keys())
         if args.command != "pca" and distance_matrix is None:
             # Calculate Distance Matrix
             hamming_distances = get_hamming_distances(
-                sequences_by_name.values()
+                sequences_by_name.values(),
+                args.indel_distance,
             )
             distance_matrix = pd.DataFrame(squareform(hamming_distances))
             distance_matrix.index = sequence_names
 
     # Calculate Embedding
+    clusterer = None
+
+    if args.cluster_threshold is not None:
+        cluster_threshold = float(args.cluster_threshold)
+        clusterer = hdbscan.HDBSCAN(
+            min_cluster_size=args.cluster_min_size,
+            min_samples=args.cluster_min_samples,
+            cluster_selection_epsilon=cluster_threshold,
+        )
 
     # Load embedding and cluster parameters from an external CSV file, if
     # possible.
-    clusterer = None
     cluster_data = None
     if args.cluster_data is not None:
         max_df = pd.read_csv(args.cluster_data)
-        clusterer = hdbscan.HDBSCAN(cluster_selection_epsilon=float(max_df.where(max_df["method"] == args.command).dropna(subset = ['distance_threshold'])[["distance_threshold"]].values.tolist()[0][0]))
+
+        # Look for cluster distance threshold in the cluster data, if the user
+        # has not provided a value from the command line.
+        if args.cluster_threshold is None:
+            clusterer = hdbscan.HDBSCAN(
+                min_cluster_size=args.cluster_min_size,
+                min_samples=args.cluster_min_samples,
+                cluster_selection_epsilon=float(max_df.where(max_df["method"] == args.command).dropna(subset = ['distance_threshold'])[["distance_threshold"]].values.tolist()[0][0])
+            )
 
         # Get a dictionary of additional parameters provided by the cluster data
         # to override defaults for the current method.
         cluster_data = max_df.to_dict("records")[0]
 
-    if cluster_data is not None and "n_components" in cluster_data:
-        n_components = cluster_data["n_components"]
+    if cluster_data is not None and "components" in cluster_data:
+        n_components = int(cluster_data["components"])
+        cluster_data["n_components"] = n_components
     else:
         n_components = args.components
 
-    if args.cluster_threshold is not None:
-        cluster_threshold = float(args.cluster_threshold)
-        clusterer = hdbscan.HDBSCAN(cluster_selection_epsilon=cluster_threshold)
-
     # Use PCA as its own embedding or as an initialization for t-SNE.
     if args.command == "pca" or args.command == "t-sne":
         sequence_names = list(sequences_by_name.keys())
 
         numbers = list(sequences_by_name.values())[:]
         for i in range(0,len(list(sequences_by_name.values()))):
             numbers[i] = re.sub(r'[^AGCT]', '5', numbers[i])
```

