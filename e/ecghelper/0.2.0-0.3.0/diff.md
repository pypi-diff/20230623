# Comparing `tmp/ecghelper-0.2.0.tar.gz` & `tmp/ecghelper-0.3.0.tar.gz`

## Comparing `ecghelper-0.2.0.tar` & `ecghelper-0.3.0.tar`

### file list

```diff
@@ -1,15 +1,31 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ecghelper-0.2.0/src/ecghelper/__init__.py
--rw-r--r--   0        0        0    15731 2020-02-02 00:00:00.000000 ecghelper-0.2.0/src/ecghelper/io.py
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 ecghelper-0.2.0/src/ecghelper/utils.py
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 ecghelper-0.2.0/tests/conftest.py
--rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 ecghelper-0.2.0/tests/test_io.py
--rw-r--r--   0        0        0     2087 2020-02-02 00:00:00.000000 ecghelper-0.2.0/tests/test_timing.py
--rw-r--r--   0        0        0   149083 2020-02-02 00:00:00.000000 ecghelper-0.2.0/tests/data/82000.xml
--rw-r--r--   0        0        0   185294 2020-02-02 00:00:00.000000 ecghelper-0.2.0/tests/data/A0001.edf
--rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 ecghelper-0.2.0/tests/data/A0001.hea
--rw-r--r--   0        0        0   180024 2020-02-02 00:00:00.000000 ecghelper-0.2.0/tests/data/A0001.mat
--rw-r--r--   0        0        0   247499 2020-02-02 00:00:00.000000 ecghelper-0.2.0/tests/data/A0001.xml
--rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 ecghelper-0.2.0/.gitignore
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 ecghelper-0.2.0/README.md
--rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 ecghelper-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 ecghelper-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    46579 2020-02-02 00:00:00.000000 ecghelper-0.3.0/82000.csv
+-rw-r--r--   0        0        0     9600 2020-02-02 00:00:00.000000 ecghelper-0.3.0/82000.dat
+-rw-r--r--   0        0        0    18788 2020-02-02 00:00:00.000000 ecghelper-0.3.0/82000.edf
+-rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 ecghelper-0.3.0/82000.hea
+-rw-r--r--   0        0        0    18048 2020-02-02 00:00:00.000000 ecghelper-0.3.0/82000.xml
+-rw-r--r--   0        0        0     9600 2020-02-02 00:00:00.000000 ecghelper-0.3.0/82000_wfdb.dat
+-rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 ecghelper-0.3.0/82000_wfdb.hea
+-rw-r--r--   0        0        0    82282 2020-02-02 00:00:00.000000 ecghelper-0.3.0/Untitled.ipynb
+-rw-r--r--   0        0        0     2030 2020-02-02 00:00:00.000000 ecghelper-0.3.0/debug.py
+-rw-r--r--   0        0        0    33302 2020-02-02 00:00:00.000000 ecghelper-0.3.0/.ipynb_checkpoints/Untitled-checkpoint.ipynb
+-rw-r--r--   0        0        0     2030 2020-02-02 00:00:00.000000 ecghelper-0.3.0/.ipynb_checkpoints/debug-checkpoint.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ecghelper-0.3.0/src/ecghelper/__init__.py
+-rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 ecghelper-0.3.0/src/ecghelper/__main__.py
+-rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 ecghelper-0.3.0/src/ecghelper/convert.py
+-rw-r--r--   0        0        0    17124 2020-02-02 00:00:00.000000 ecghelper-0.3.0/src/ecghelper/io.py
+-rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 ecghelper-0.3.0/src/ecghelper/utils.py
+-rw-r--r--   0        0        0    21595 2020-02-02 00:00:00.000000 ecghelper-0.3.0/src/ecghelper/waveform.py
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 ecghelper-0.3.0/tests/conftest.py
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 ecghelper-0.3.0/tests/test_io.py
+-rw-r--r--   0        0        0     2087 2020-02-02 00:00:00.000000 ecghelper-0.3.0/tests/test_timing.py
+-rw-r--r--   0        0        0     3028 2020-02-02 00:00:00.000000 ecghelper-0.3.0/tests/test_waveform.py
+-rw-r--r--   0        0        0   149083 2020-02-02 00:00:00.000000 ecghelper-0.3.0/tests/data/82000.xml
+-rw-r--r--   0        0        0   185294 2020-02-02 00:00:00.000000 ecghelper-0.3.0/tests/data/A0001.edf
+-rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 ecghelper-0.3.0/tests/data/A0001.hea
+-rw-r--r--   0        0        0   180024 2020-02-02 00:00:00.000000 ecghelper-0.3.0/tests/data/A0001.mat
+-rw-r--r--   0        0        0   247499 2020-02-02 00:00:00.000000 ecghelper-0.3.0/tests/data/A0001.xml
+-rw-r--r--   0        0        0   108785 2020-02-02 00:00:00.000000 ecghelper-0.3.0/tests/data/binary.csv
+-rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 ecghelper-0.3.0/.gitignore
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 ecghelper-0.3.0/README.md
+-rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 ecghelper-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      840 2020-02-02 00:00:00.000000 ecghelper-0.3.0/PKG-INFO
```

### Comparing `ecghelper-0.2.0/src/ecghelper/io.py` & `ecghelper-0.3.0/src/ecghelper/io.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 import warnings
 
 import lxml.etree as ET
 import numpy as np
 import wfdb
 import pyedflib
 
-_LEADS = [
+_LEADS = (
     'I', 'II', 'III', 'aVR', 'aVL', 'aVF', 'V1', 'V2', 'V3', 'V4', 'V5', 'V6'
-]
+)
 
 # === EDF === #
 def load_edf(record_filename: Path) -> np.ndarray:
     """Load an EDF/EDF+ record."""
     f = pyedflib.EdfReader(str(record_filename.resolve()))
     n = f.signals_in_file
     signal = np.zeros((f.getNSamples()[0], n))
@@ -78,15 +78,15 @@
 def load_edfz(record_name: Path) -> np.ndarray:
     """Load an EDFZ record."""
     # with gzip.open(record_name, 'rb') as f:
     #     signal = f.read()
     # pyedflib expects a filename as input, not a file-like object :(
     raise NotImplementedError()
 
-def write_edfz(record_name: Path) -> np.ndarray:
+def write_edfz(record_name: Path):
     """Write an EDFZ record."""
     raise NotImplementedError()
 
 # === WFDB === #
 
 def load_wfdb(record_filename: Path) -> np.ndarray:
     """Load a WFDB record."""
@@ -98,29 +98,29 @@
 
     record = wfdb.rdrecord(record_filename)
     if record.p_signal is None:
         raise ValueError(f'No signal found in {record_filename}')
 
     return record.p_signal
 
-def write_wfdb(record_filename: Path, signal: np.ndarray, sampling_frequency: int = 500) -> np.ndarray:
-    """Load a WFDB record."""
+def write_wfdb(record_filename: Path, signal: np.ndarray, sampling_frequency: int = 500):
+    """Write a WFDB record to format 16 (2-bytes per sample)."""
     # As of WFDB 4.1.1, wrsamp expects there to be no extension in record name,
     # so we remove it if it exists
     if record_filename.suffix not in ('.dat', '.hea'):
         warnings.warn(f'Saved WFDB records will use .dat/.hea, not {record_filename.suffix}')
 
     wfdb.wrsamp(
         record_filename.stem,
         fs=sampling_frequency,
         sig_name=_LEADS,
         p_signal=signal,
         fmt=['16'] * 12,
         units=['mV'] * 12,
-        write_dir = record_filename.parent
+        write_dir = str(record_filename.parent.resolve())
     )
 
 def load_wfdb_metadata(record_filename: Path) -> dict:
     """
     Load metadata from a WFDB (WaveForm DataBase) record file.
 
     Args:
@@ -248,15 +248,15 @@
             raise ValueError(f'unknown units of measure: {units}')
         signal.append(lead_data)
     
     # stack lead data column-wise
     signal = np.stack(signal, axis=1)
     return signal
 
-def write_xml(record_filename: Path, signal: np.ndarray, sampling_frequency: int = 500) -> None:
+def write_xml(record_filename: Path, signal: np.ndarray, sampling_frequency: int = 500):
 
     """Write waveform data to an XML record. Assumes the signal is stored
     as 16-bit integers in millivolts.
     
     This function writes the waveform data to an XML file with the following structure:
         <Waveform>
             <LeadData>
@@ -385,23 +385,62 @@
         header = header[1:]
         data = data[:, 1:]
     elif len(header) != 12:
         raise ValueError('CSV must have 12 or 13 columns')
     
     return data
 
+def load_csv_metadata(record_name: Path) -> dict:
+    """Load metadata for a CSV record.
+
+    This includes (1) the sampling frequency, and (2) the lead names.
+    """
+    with open(record_name, 'r') as f:
+        reader = csv.reader(f)
+        header = next(reader)
+        sample_0 = float(next(reader)[0])
+        sample_1 = float(next(reader)[0])
+        sample_2 = float(next(reader)[0])
+    
+    
+    # verify that the first column have evenly spaced samples
+    # i.e. that it is a time column
+    if sample_2 - sample_1 != sample_1 - sample_0:
+        raise ValueError('First column of CSV must be time')
+
+    # get sampling frequency
+    sampling_frequency = 1 / (sample_1 - sample_0)
+
+    # get lead names
+    leads = header[1:]
+
+    return {'sampling_frequency': sampling_frequency, 'leads': leads}
+
+
+def write_csv(record_name: Path, signal: np.ndarray, sampling_frequency: int = 500, leads=_LEADS):
+    """Write a CSV record.
+    
+    The CSV will have a header row. The first column will be the time of the sample,
+    in seconds. The remaining columns will be the leads of the ECG.
+    """
+    with open(record_name, 'w') as f:
+        writer = csv.writer(f)
+        writer.writerow(['Time'] + list(leads))
+        for i in range(signal.shape[0]):
+            writer.writerow([i / sampling_frequency] + list(signal[i, :]))
 
 # === Record Loading === #
 # The following functions are used to load records from various formats.
 
 load_functions = {
     "wfdb": (load_wfdb, load_wfdb_metadata),
     "edf": (load_edf, load_edf_metadata),
     "edfz": (load_edfz, load_edfz_metadata),
     "xml": (load_xml, load_xml_metadata),
+    "csv": (load_csv, load_csv_metadata),
 }
 
 def get_file_function(format: str) -> tuple[Callable, Callable]:
     if format in load_functions:
         return load_functions[format]
     else:
         raise ValueError(f"Unsupported file format: {format}")
```

### Comparing `ecghelper-0.2.0/tests/test_io.py` & `ecghelper-0.3.0/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `ecghelper-0.2.0/tests/test_timing.py` & `ecghelper-0.3.0/tests/test_timing.py`

 * *Files identical despite different names*

### Comparing `ecghelper-0.2.0/tests/data/82000.xml` & `ecghelper-0.3.0/tests/data/82000.xml`

 * *Files identical despite different names*

### Comparing `ecghelper-0.2.0/tests/data/A0001.edf` & `ecghelper-0.3.0/tests/data/A0001.edf`

 * *Files identical despite different names*

### Comparing `ecghelper-0.2.0/tests/data/A0001.hea` & `ecghelper-0.3.0/tests/data/A0001.hea`

 * *Files identical despite different names*

### Comparing `ecghelper-0.2.0/tests/data/A0001.mat` & `ecghelper-0.3.0/tests/data/A0001.mat`

 * *Files identical despite different names*

### Comparing `ecghelper-0.2.0/tests/data/A0001.xml` & `ecghelper-0.3.0/tests/data/A0001.xml`

 * *Files identical despite different names*

### Comparing `ecghelper-0.2.0/.gitignore` & `ecghelper-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `ecghelper-0.2.0/pyproject.toml` & `ecghelper-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "ecghelper"
-version = "0.2.0"
+version = "0.3.0"
 description = "Tools to load and process electrocardiogram data."
 author = "Alistair Johnson"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "Operating System :: OS Independent",
@@ -17,15 +17,15 @@
     "joblib>=1.2.0",
     "cython>=0.29.34",
     "scikit-learn>=1.2.2",
     "scipy>=1.10.1",
     "tqdm>=4.65.0",
     "xgboost>=1.7.4",
     "pip>=23.1.2",
-    "wfdb>=4.1.1",
+    "wfdb>=4.1.2",
     "pyEDFlib>=0.1.32",
     "lxml>=4.9.2"
 ]
 
 [tool.hatchling]
 src = "src/ecghelper"
```

