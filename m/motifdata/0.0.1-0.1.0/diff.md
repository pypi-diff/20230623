# Comparing `tmp/motifdata-0.0.1.tar.gz` & `tmp/motifdata-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "motifdata-0.0.1.tar", max compression
+gzip compressed data, was "motifdata-0.1.0.tar", max compression
```

## Comparing `motifdata-0.0.1.tar` & `motifdata-0.1.0.tar`

### file list

```diff
@@ -1,21 +1,20 @@
--rw-r--r--   0        0        0     1065 2023-01-31 23:19:36.000000 motifdata-0.0.1/LICENSE
--rw-r--r--   0        0        0     2456 2023-02-02 22:17:57.000000 motifdata-0.0.1/motifdata/_Motif.py
--rw-r--r--   0        0        0        0 2023-02-02 22:17:57.000000 motifdata-0.0.1/motifdata/__init__.py
--rw-r--r--   0        0        0     3776 2023-02-02 22:17:58.000000 motifdata-0.0.1/motifdata/_convert.py
--rw-r--r--   0        0        0     4102 2023-02-02 22:17:57.000000 motifdata-0.0.1/motifdata/_fimo.py
--rw-r--r--   0        0        0        0 2023-02-02 22:17:57.000000 motifdata-0.0.1/motifdata/_homer.py
--rw-r--r--   0        0        0    10382 2023-02-02 22:17:57.000000 motifdata-0.0.1/motifdata/_io.py
--rw-r--r--   0        0        0       43 2023-02-02 22:17:57.000000 motifdata-0.0.1/motifdata/_memesuite.py
--rw-r--r--   0        0        0        0 2023-02-02 22:17:58.000000 motifdata-0.0.1/motifdata/_plot.py
--rw-r--r--   0        0        0     5015 2023-02-02 22:17:57.000000 motifdata-0.0.1/motifdata/_utils.py
--rw-r--r--   0        0        0     2857 2023-02-02 22:17:57.000000 motifdata-0.0.1/motifdata/resources/CPEs.meme
--rw-r--r--   0        0        0      240 2023-02-02 22:17:57.000000 motifdata-0.0.1/motifdata/resources/MA0037.3.pfm
--rw-r--r--   0        0        0      183 2023-02-02 22:17:57.000000 motifdata-0.0.1/motifdata/resources/MA0098.1.pfm
--rw-r--r--   0        0        0      269 2023-02-02 22:17:58.000000 motifdata-0.0.1/motifdata/resources/TATA.meme
--rw-r--r--   0        0        0     4392 2023-02-02 22:17:58.000000 motifdata-0.0.1/motifdata/resources/known.motifs
--rw-r--r--   0        0        0    21084 2023-02-02 22:17:57.000000 motifdata-0.0.1/motifdata/resources/model_filters.meme
--rw-r--r--   0        0        0      959 2023-02-02 22:17:57.000000 motifdata-0.0.1/motifdata/resources/motifs.meme
--rw-r--r--   0        0        0      189 2023-02-02 22:17:57.000000 motifdata-0.0.1/motifdata/resources/sample.sites
--rw-r--r--   0        0        0      360 2023-02-02 22:36:20.000000 motifdata-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      668 2023-02-02 22:38:27.941383 motifdata-0.0.1/setup.py
--rw-r--r--   0        0        0      435 2023-02-02 22:38:27.941655 motifdata-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-01-31 23:19:36.000000 motifdata-0.1.0/LICENSE
+-rw-r--r--   0        0        0      479 2023-05-23 17:49:32.000000 motifdata-0.1.0/README.md
+-rw-r--r--   0        0        0     4914 2023-05-31 22:01:20.000000 motifdata-0.1.0/motifdata/_Motif.py
+-rw-r--r--   0        0        0      550 2023-06-08 17:03:25.000000 motifdata-0.1.0/motifdata/__init__.py
+-rw-r--r--   0        0        0     7957 2023-06-23 19:05:33.000000 motifdata-0.1.0/motifdata/_convert.py
+-rw-r--r--   0        0        0    12831 2023-06-23 19:12:38.000000 motifdata-0.1.0/motifdata/_io.py
+-rw-r--r--   0        0        0     1919 2023-05-31 22:01:20.000000 motifdata-0.1.0/motifdata/_transform.py
+-rw-r--r--   0        0        0     7139 2023-06-23 19:02:07.000000 motifdata-0.1.0/motifdata/_utils.py
+-rw-r--r--   0        0        0   111006 2023-05-31 22:01:20.000000 motifdata-0.1.0/motifdata/resources/filters_out.meme
+-rw-r--r--   0        0        0  1632317 2023-05-31 22:01:20.000000 motifdata-0.1.0/motifdata/resources/jaspar_out.meme
+-rw-r--r--   0        0        0     2857 2023-05-31 22:01:20.000000 motifdata-0.1.0/motifdata/resources/sample.meme
+-rw-r--r--   0        0        0     4392 2023-05-31 22:01:20.000000 motifdata-0.1.0/motifdata/resources/sample.motifs
+-rw-r--r--   0        0        0      424 2023-05-31 22:01:20.000000 motifdata-0.1.0/motifdata/resources/sample.pfm
+-rw-r--r--   0        0        0      189 2023-02-02 22:17:57.000000 motifdata-0.1.0/motifdata/resources/sample.sites
+-rw-r--r--   0        0        0      269 2023-05-31 22:01:20.000000 motifdata-0.1.0/motifdata/resources/sample_filter.meme
+-rw-r--r--   0        0        0    21084 2023-05-31 22:01:20.000000 motifdata-0.1.0/motifdata/resources/sample_filters.meme
+-rw-r--r--   0        0        0     2194 2023-05-31 22:01:20.000000 motifdata-0.1.0/motifdata/resources/sample_out.meme
+-rw-r--r--   0        0        0     3482 2023-05-31 22:01:20.000000 motifdata-0.1.0/motifdata/resources/sample_out.motifs
+-rw-r--r--   0        0        0      524 2023-06-23 19:12:30.000000 motifdata-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1244 1970-01-01 00:00:00.000000 motifdata-0.1.0/PKG-INFO
```

### Comparing `motifdata-0.0.1/LICENSE` & `motifdata-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `motifdata-0.0.1/motifdata/_io.py` & `motifdata-0.1.0/motifdata/_io.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,22 +1,23 @@
+import h5py
 from os import PathLike
 import numpy as np
 from ._Motif import Motif, MotifSet
 from ._convert import (
-    _from_biopython
+    from_biopython
 )
 from ._utils import (
     _parse_version, 
     _parse_alphabet, 
     _parse_strands, 
     _parse_background, 
     _parse_motif, 
 )
-from ...preprocess import decode_seq
-from ...preprocess._utils import _token2one_hot
+from ._utils import decode_seq
+from ._utils import _token2one_hot
 
 def _read_meme_pymemesuite(
     filename: PathLike
 ):
     """Read motifs from a MEME file into pymemesuite.common.Motif objects.
 
     Parameters
@@ -78,15 +79,15 @@
                 if strands is None:
                     strands = _parse_strands(line)
                     line = meme_file.readline()
                 else:
                     raise RuntimeError("Multiple strand definitions encountered in MEME file")
             elif line.startswith("Background letter frequencies"):
                 if background is None:
-                    line = _parse_background(line, meme_file)
+                    line, background = _parse_background(line, meme_file)
                 else:
                     raise RuntimeError("Multiple background frequency definitions encountered in MEME file")
             elif line.startswith("MOTIF"):
                 motif = _parse_motif(line, meme_file)
                 if motif.identifier in motifs:
                     raise RuntimeError("Motif identifiers not unique within file")
                 motifs[motif.identifier] = motif
@@ -98,38 +99,98 @@
         version=version,
         alphabet=alphabet,
         strands=strands,
         background=background,
         background_source=background_source,
     )
 
-READER_REGISTRY = {
+MEME_READER_REGISTRY = {
     "pymemesuite": _read_meme_pymemesuite,
     "MotifSet": _read_meme_MotifSet,
 }
 
 def read_meme(
-    filename,
-    return_type="MotifSet"
+    filename: PathLike,
+    return_type: str = "MotifSet"
 ):
     """Read motifs from a MEME file into a MotifSet object.
     
     Parameters
     ----------
     filename : str
         MEME filename
     
     Returns
     -------
     MotifSet
         MotifSet object
     """
-    return READER_REGISTRY[return_type](filename)
+    return MEME_READER_REGISTRY[return_type](filename)
 
-    
+def read_homer(
+    filename: PathLike,
+    transpose: bool = False,
+    counts: bool = False,
+    alphabet: str = "ACGT",
+    background: dict = None,
+):
+    """Read motifs from a .motif file into a MotifSet object.
+
+    Parameters
+    ----------
+    filename : str
+        .motif filename
+    transpose : bool, optional
+        whether to transpose the matrices, by default True
+    counts : bool, optional
+        whether the input matrices are counts and should be converted to pfm, by default True
+
+    Returns
+    -------
+    MotifSet
+        MotifSet object
+    """
+    with open(filename) as motif_file:
+        data = motif_file.readlines()
+    pfm_rows, pfms, ids, names = [], [], [], []
+    for line in data:
+        line = line.rstrip()
+        if line.startswith(">"):
+            ids.append(line.split()[0].replace(">", ""))
+            names.append(line.split()[1])
+            if len(pfm_rows) > 0:
+                pfms.append(np.vstack(pfm_rows))
+                pfm_rows = []
+        else:
+            pfm_row = np.array(list(map(float, line.split())))
+            pfm_rows.append(pfm_row)
+    pfms.append(np.vstack(pfm_rows))
+    motifs = {}
+    for i in range(len(pfms)):
+        if transpose:
+            pfms[i] = pfms[i].T
+        if counts:
+            pfms[i] = np.divide(pfms[i], pfms[i].sum(axis=1)[:,None])
+        consensus = decode_seq(_token2one_hot(pfms[i].argmax(axis=1)))
+        motif = Motif(
+            pfm=pfms[i],
+            identifier=ids[i],
+            name=names[i],
+            consensus=consensus,
+            length=len(consensus)
+        )
+        motifs[ids[i]] = motif
+    if background is None:
+        uniform = 1/len(alphabet) if background is None else background
+        background = {a: uniform for a in alphabet}
+    return MotifSet(
+        motifs=motifs,
+        alphabet=alphabet,
+        background=background,
+    )
 
 def read_motifs(
     filename,
     transpose=True,
     counts=True
 ):
     """Read motifs from a .motif file into a MotifSet object.
@@ -154,14 +215,17 @@
         line = line.rstrip()
         if line.startswith(">"):
             ids.append(line.split()[0])
             names.append(line.split()[1])
             if len(pfm_rows) > 0:
                 pfms.append(np.vstack(pfm_rows))
                 pfm_rows = []
+        # elif the line is only a newline
+        elif not line.strip():
+            continue
         else:
             pfm_row = np.array(list(map(float, line.split())))
             pfm_rows.append(pfm_row)
     pfms.append(np.vstack(pfm_rows))
     motifs = {}
     for i in range(len(pfms)):
         if transpose:
@@ -224,15 +288,14 @@
     return motifs
 
 def load_jaspar(
     motif_accs=None,
     motif_names=None,
     collection=None,
     release="JASPAR2022",
-    identifier_number=0,
     verbose=False,
     **kwargs,   
 ):
     """Load motifs from JASPAR database into a MotifSet object
 
     Parameters
     ----------
@@ -256,113 +319,118 @@
     motifs = _load_jaspar(
         motif_accs=motif_accs,
         motif_names=motif_names,
         collection=collection,
         release=release,
         **kwargs,
     )
-    motif_set = _from_biopython(
+    motif_set = from_biopython(
         motifs, 
-        identifier_number=identifier_number, 
         verbose=verbose
     )
     return motif_set
 
-def read_array(
-    filename,
-    transpose=True,
-):
-    """Read from a NumPy array file into a MotifSet object.
-    TODO: test this with a real case
-    """
-    pass
+def read_h5(filename):
+    motif_set = MotifSet()
+    with h5py.File(filename, "r") as f:
+        for key in f.keys():
+            pfm = f[key][:]
+            consensus = decode_seq(_token2one_hot(pfm.argmax(axis=1)))
+            motif_set.add_motif(
+                Motif(
+                    identifier=key,
+                    name=key,
+                    pfm=pfm,
+                    consensus=consensus,
+                    length=len(consensus)
+                )
+            )
+    return motif_set
 
-def write_meme( 
-    motif_set,
-    filename,
-    background=[0.25, 0.25, 0.25, 0.25],
-    **kwargs,
+def write_meme(
+    motif_set: MotifSet,
+    filename: str
 ):
-    """Write a MotifSet object to a MEME file.
+    """Write MotifSet object to MEME file
 
     Parameters
     ----------
     motif_set : MotifSet
         MotifSet object
     filename : str
-        Output filename
-    background : list of float, optional
-        Background frequencies, by default [0.25, 0.25, 0.25, 0.25]
+        filename to write to
     """
-    pass
+    alphabet = motif_set.alphabet
+    version = motif_set.version
+    background = motif_set.background
+    strands = motif_set.strands
+    meme_file = open(filename, "w")
+    meme_file.write(f"MEME version {version}\n\n")
+    meme_file.write(f"ALPHABET= {alphabet}\n\n")
+    meme_file.write(f"strands: {strands}\n\n")
+    meme_file.write("Background letter frequencies\n")
+    meme_file.write(
+        f"{alphabet[0]} {background[alphabet[0]]} " \
+        f"{alphabet[1]} {background[alphabet[1]]} " \
+        f"{alphabet[2]} {background[alphabet[2]]} " \
+        f"{alphabet[3]} {background[alphabet[3]]}" \
+        f"\n"
+    )
+    for motif in motif_set:
+        ident = motif.identifier
+        name = motif.name
+        pfm = motif.pfm
+        if np.sum(pfm) > 0:
+            meme_file.write("\n")
+            meme_file.write(f"MOTIF {ident} {name} \n")
+            meme_file.write(f"letter-probability matrix: alength= 4 w= {len(pfm)} \n")
+        for j in range(0, len(pfm)):
+            if np.sum(pfm[j]) > 0:
+                meme_file.write("\t".join(pfm[j].astype(str)) + "\n")
+    meme_file.close()
+    print("Saved pfm in MEME format as: {}".format(filename))
 
-def write_motifs(
-    motif_set,
-    filename,
-    format="homer",
-    **kwargs,
+def write_homer(
+    motif_set: MotifSet,
+    filename: PathLike,
+    log_odds_threshold: np.ndarray = None
 ):
-    """Write a MotifSet object to a file.
+    """Write MotifSet object to HOMER file format
 
     Parameters
     ----------
     motif_set : MotifSet
         MotifSet object
     filename : str
-        Output filename
-    format : str, optional
-        Output format, by default "homer"
+        filename to write to
     """
-    pass
+    motif_file = open(filename, "w")
+    log_odds_threshold = np.zeros(len(motif_set)) if log_odds_threshold is None else log_odds_threshold 
+    for i, motif in enumerate(motif_set):
+        ident = motif.identifier
+        name = motif.name
+        pfm = motif.pfm
+        motif_file.write(f">{ident}\t{name}\t{log_odds_threshold[i]}\n")
+        for j in range(0, len(pfm)):
+            if np.sum(pfm) > 0:
+                motif_file.write("\t".join(pfm[j].astype(str)) + "\n")
+    motif_file.close()
+    print("Saved pfms in .motifs format as: {}".format(filename))
 
-def write_meme_from_array(
-    array,
-    outfile,
-    vocab="DNA",
-    background=[0.25, 0.25, 0.25, 0.25],
+def write_h5(
+    motif_set: MotifSet,
+    filename: PathLike
 ):
-    """
-    Function to convert pwm as ndarray to meme file
-    Adapted from:: nnexplain GitHub:
-    TODO: Depracate in favor of first converting to MotifSet and then writing to file
+    """Write MotifSet object to h5 file format
 
     Parameters
     ----------
-    array:
-        numpy.array, often pwm matrices, shape (U, 4, filter_size), where U - number of units
-    outfile:
-        string, the name of the output meme file
+    motif_set : MotifSet
+        MotifSet object
+    filename : str
+        filename to write to
     """
-    from ...preprocess._utils import _get_vocab
-
-    vocab = "".join(_get_vocab(vocab))
-    n_filters = array.shape[0]
-    filter_size = array.shape[2]
-    meme_file = open(outfile, "w")
-    meme_file.write("MEME version 4\n\n")
-    meme_file.write(f"ALPHABET= {vocab}\n\n")
-    meme_file.write("strands: + -\n\n")
-    meme_file.write("Background letter frequencies\n")
-    meme_file.write(f"{vocab[0]} {background[0]} {vocab[1]} {background[1]} {vocab[2]} {background[2]} {vocab[3]} {background[3]}\n")
-
-    for i in range(0, n_filters):
-        if np.sum(array[i, :, :]) > 0:
-            meme_file.write("\n")
-            meme_file.write("MOTIF filter%s\n" % i)
-            meme_file.write(
-                "letter-probability matrix: alength= 4 w= %d \n"
-                % np.count_nonzero(np.sum(array[i, :, :], axis=0))
-            )
-        for j in range(0, filter_size):
-            if np.sum(array[i, :, j]) > 0:
-                meme_file.write(
-                    str(array[i, 0, j])
-                    + "\t"
-                    + str(array[i, 1, j])
-                    + "\t"
-                    + str(array[i, 2, j])
-                    + "\t"
-                    + str(array[i, 3, j])
-                    + "\n"
-                )
-    meme_file.close()
-    print("Saved array in as : {}".format(outfile))
+    with h5py.File(filename, "w") as f:
+        for motif in motif_set.motifs.values():
+            f.create_dataset(motif.identifier, data=motif.pfm)
+    print("Saved pfm in h5 format as: {}".format(filename))
+
```

### Comparing `motifdata-0.0.1/motifdata/resources/CPEs.meme` & `motifdata-0.1.0/motifdata/resources/sample.meme`

 * *Files identical despite different names*

### Comparing `motifdata-0.0.1/motifdata/resources/known.motifs` & `motifdata-0.1.0/motifdata/resources/sample.motifs`

 * *Files identical despite different names*

### Comparing `motifdata-0.0.1/motifdata/resources/model_filters.meme` & `motifdata-0.1.0/motifdata/resources/sample_filters.meme`

 * *Files identical despite different names*

