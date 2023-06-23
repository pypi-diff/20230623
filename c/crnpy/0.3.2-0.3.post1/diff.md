# Comparing `tmp/crnpy-0.3.2.tar.gz` & `tmp/crnpy-0.3.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crnpy-0.3.2.tar", last modified: Fri Jun 23 17:07:23 2023, max compression
+gzip compressed data, was "crnpy-0.3.post1.tar", last modified: Fri Jun 16 23:49:30 2023, max compression
```

## Comparing `crnpy-0.3.2.tar` & `crnpy-0.3.post1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 17:07:23.601242 crnpy-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-23 17:07:11.000000 crnpy-0.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3351 2023-06-23 17:07:23.601242 crnpy-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2968 2023-06-23 17:07:11.000000 crnpy-0.3.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 17:07:23.601242 crnpy-0.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-06-23 17:07:11.000000 crnpy-0.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 17:07:23.597242 crnpy-0.3.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 17:07:23.601242 crnpy-0.3.2/src/crnpy/
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-23 17:07:11.000000 crnpy-0.3.2/src/crnpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    55997 2023-06-23 17:07:11.000000 crnpy-0.3.2/src/crnpy/crnpy.py
--rw-r--r--   0 runner    (1001) docker     (123)     9161 2023-06-23 17:07:11.000000 crnpy-0.3.2/src/crnpy/data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 17:07:23.601242 crnpy-0.3.2/src/crnpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3351 2023-06-23 17:07:23.000000 crnpy-0.3.2/src/crnpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-23 17:07:23.000000 crnpy-0.3.2/src/crnpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 17:07:23.000000 crnpy-0.3.2/src/crnpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-23 17:07:23.000000 crnpy-0.3.2/src/crnpy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 23:49:30.905187 crnpy-0.3.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-16 23:49:21.000000 crnpy-0.3.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2643 2023-06-16 23:49:30.905187 crnpy-0.3.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-06-16 23:49:21.000000 crnpy-0.3.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 23:49:30.905187 crnpy-0.3.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-06-16 23:49:21.000000 crnpy-0.3.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 23:49:30.901188 crnpy-0.3.post1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 23:49:30.905187 crnpy-0.3.post1/src/crnpy/
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-16 23:49:21.000000 crnpy-0.3.post1/src/crnpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53443 2023-06-16 23:49:21.000000 crnpy-0.3.post1/src/crnpy/crnpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9161 2023-06-16 23:49:21.000000 crnpy-0.3.post1/src/crnpy/data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 23:49:30.905187 crnpy-0.3.post1/src/crnpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2643 2023-06-16 23:49:30.000000 crnpy-0.3.post1/src/crnpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-16 23:49:30.000000 crnpy-0.3.post1/src/crnpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 23:49:30.000000 crnpy-0.3.post1/src/crnpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-16 23:49:30.000000 crnpy-0.3.post1/src/crnpy.egg-info/top_level.txt
```

### Comparing `crnpy-0.3.2/LICENSE` & `crnpy-0.3.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `crnpy-0.3.2/README.md` & `crnpy-0.3.post1/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,40 +1,30 @@
-![GitHub Workflow Status (building)](https://img.shields.io/github/actions/workflow/status/soilwater/crnpy/python-package.yml)
-![GitHub Workflow Status (publish)](https://img.shields.io/github/actions/workflow/status/soilwater/crnpy/python-publish.yml?label=publish)
-[![PyPI - Status](https://img.shields.io/pypi/v/crnpy)](https://pypi.org/project/crnpy/)
-![GitHub commits since latest release (by SemVer including pre-releases)](https://img.shields.io/github/commits-since/soilwater/crnpy/latest/main)
-
 # Cosmic-Ray Neutron Python (CRNPy) Library
 
-<img src="https://raw.githubusercontent.com/soilwater/crnpy/main/docs/img/logo/crnpy-logo.png" alt="CRNPY logo" width="250"/>
+<img src="/docs/img/logo/crnpy-logo.png" alt="CRNPY logo" width="250"/>
 
 ## Overview
 
 Welcome to the homepage of the CRNPy (Cosmic-Ray Neutron Python) library, an open-source Python library designed for the processing and conversion of raw neutron counts from Cosmic-Ray Neutron Probes (CRNP) into accurate field-level soil moisture data.
 
 This library has been developed with the intent of providing a comprehensive yet easy-to-use workflow for processing raw data from a variety of CRNP, encompassing multiple manufacturers and models.
 
 ## Key Features
 - Versatility: CRNPy can handle data from various CRNP manufacturers and models. It has been successfully tested on both roving and stationary CRNP.
 - Modularity: The library is designed to be modular, allowing users to easily customize the processing workflow to their needs.
-- Instrument agnostic: It can be used with any CRNP, allowing users to process data from multiple instruments with their own workflow.
+- Accuracy: The library shows excellent agreement with ground-based measurements, making it a reliable tool for scientific research and practical applications.
+- Correction Routines: The correction functions of the library have been effectively used to represent field and watershed scale soil moisture conditions.
 
-![CRNPy Processing Workflow](https://raw.githubusercontent.com/soilwater/crnpy/main/docs/img/workflow.png)
+![CRNPy Processing Workflow](docs/img/workflow.png)
 Overview of the proposed CRNPy processing workflow. Final user can choose to use the entire workflow, part of it, or build functions on top of it depending on their needs, dashed lines indicate optional steps.
 
 
 ## Installation
 
 To install the CRNPy library, you can use Python's package manager, pip. Simply open your command line or terminal and type:
 
 ```pip install crnpy```
 
 ## Authors
+The CRNPy library was conceived and developed by Joaquin Peraza and Andres Patrignani in the Soil Water Processes Lab at Kansas State University. The team's passion for making soil moisture data more accessible and easier to process culminated in this powerful tool.
 
-The CRNPy library was developed by:
-
-- Joaquin Peraza
-- Andres Patrignani
-
-in the Soil Water Processes Lab at Kansas State University. The team's passion for making soil moisture data more accessible and easier to process culminated in this powerful tool.
-
-The Soil Water Processes Lab at Kansas State University is a leading research group focused on understanding and modeling soil water processes. The lab combines a range of experimental and computational approaches to tackle some of the most pressing issues in soil and water research. The development of the CRNPy library is a testament to the lab's commitment to pushing the boundaries of soil science through the innovative use of technology. The authors would like to acknowledge the contributions of the wider scientific community in testing and providing feedback on the library, which has been instrumental in its ongoing development.
+The Soil Water Processes Lab at Kansas State University is a leading research group focused on understanding and modeling soil water processes. The lab combines a range of experimental and computational approaches to tackle some of the most pressing issues in soil and water research. The development of the CRNPy library is a testament to the lab's commitment to pushing the boundaries of soil science through the innovative use of technology. like to acknowledge the contributions of the wider scientific community in testing and providing feedback on the library, which has been instrumental in its ongoing development.
```

### Comparing `crnpy-0.3.2/src/crnpy/crnpy.py` & `crnpy-0.3.post1/src/crnpy/crnpy.py`

 * *Files 5% similar despite different names*

```diff
@@ -70,61 +70,48 @@
             source = pd.concat([df,new_line])
 
     df.sort_values(by=col, inplace=True)
     df.reset_index(drop=True, inplace=True)
     df.set_index(col, inplace=True)
     return df
 
-def count_time(counts=None, timestamp_col=None):
+def count_time(df):
     """Approximate counting time.
 
     Args:
-        counts (pandas.DataFrame): DataFrame with neutron counts, might have DateTimeIndex.
-        timestamp_col (pandas.Series): Series with timestamps. If counts has a DateTimeIndex, timestamp_col is not needed.
+        df (pandas.DataFrame): Dataframe containing only the columns with neutron counts and timestamp in the index.
 
     Returns:
-        (pandas.Series): Series with the approximate counting time for each observation.
+        (pandas.DataFrame): Dataframe with the approximate counting time for each observation.
 
     Examples:
         Using `count_time` in a console environment:
 
         >>> df = pd.DataFrame(...)
-        >>> count_time(timestamp_col=df['timestamp'])
+        >>> count_time(df)
         0   3600.0
         1   3600.0
         2   3600.0
     """
-    if timestamp_col is not None:
-        if not isinstance(timestamp_col, pd.Series):
-            raise TypeError('timestamp_col must be a pandas Series.')
-        if timestamp_col.dtype != 'datetime64[ns]':
-            raise TypeError('timestamp_col must be a pandas Series with datetime64[ns] dtype.')
 
-        count_time = timestamp_col.diff().dt.total_seconds()
-        return count_time
+    # Check that index is a timestamp
+    if type(df.index) != pd.core.indexes.datetimes.DatetimeIndex:
+        raise ValueError('Index must be a timestamp.')
 
-    if counts is not None:
-        if not isinstance(counts, pd.DataFrame):
-            raise TypeError('counts must be a pandas DataFrame.')
+    # Calculate time difference between rows
+    count_time = df.index.to_series().diff().dt.total_seconds()
 
-        if not counts.index.dtype == 'datetime64[ns]':
-            raise TypeError('counts must have a DateTimeIndex.')
+    return count_time
 
-        count_time = counts.index.to_series().diff().dt.total_seconds()
-        return count_time
-
-    raise TypeError('Either counts or timestamp_col must be provided.')
-
-def fill_counts(counts, count_times=None, timestamp_col=None, expected_time=False, threshold=0.25, limit=3):
+def fill_counts(counts, count_times=None, expected_time=False, threshold=0.25, limit=3):
     """Fill missing neutron counts. Observation periods shorter than threshold are discarded (replaced with NaN).
     
     Args:
-        counts (pandas.DataFrame): DataFrame with neutron counts, might have DateTimeIndex.
-        count_time (pandas.Series or pandas.DataFrame): Counting time in seconds. If a DataFrame is provided, it must have the same number of columns as `counts`.
-        timestamp_col (pandas.Series): Series with timestamps. If counts has a DateTimeIndex, timestamp_col is not needed.
+        counts (pandas.DataFrame): DataFrame with neutron counts, might have count_time column(s).
+        count_time (pandas.Series or pandas.DataFrame): Counting time in seconds. If a DataFrame is provided, it must have the same number of columns as df.
         expected_time (int): Expected counting time in seconds. If not provided, it is calculated as the median of the counting times.
         threshold (float): Minimum fraction of the neutron integration time. Default is 0.25.
 
     Returns:
         (pandas.DataFrame): DataFrame with linearly interpolated neutron counts.
 
     Examples:
@@ -138,27 +125,18 @@
         3   102.0
     """
 
     counts=counts.copy()
 
     if type(counts.index) == pd.core.indexes.datetimes.DatetimeIndex and isinstance(count_times, type(None)):
         print("No count time columns provided. Using timestamp index to compute count time.")
-        count_times = count_time(timestamp_col=counts.index.to_series())
-
-    elif not isinstance(timestamp_col, type(None)) and isinstance(count_times, type(None)):
-        if timestamp_col.dtype != 'datetime64[ns]':
-            if len(timestamp_col) != len(counts):
-                raise ValueError('Timestamp column length does not match number of readings.')
-            print("No count time columns provided. Using timestamp column to compute count time.")
-            count_times = count_time(timestamp_col=timestamp_col)
-        else:
-            raise TypeError('Timestamp column must be a pandas Series with datetime64[ns] dtype.')
+        count_times = counts.index.to_series().diff().dt.total_seconds()
 
-    if type(counts.index) != pd.core.indexes.datetimes.DatetimeIndex and isinstance(count_times, type(None)) and isinstance(timestamp_col, type(None)):
-        raise ValueError('Count_times must be provided, or timestamp_col must be provided, or counts must have a DatetimeIndex.')
+    if type(counts.index) != pd.core.indexes.datetimes.DatetimeIndex and isinstance(count_times, type(None)):
+        raise ValueError('Index must be a timestamp or count times must be provided.')
 
     if len(counts) != len(count_times):
         raise ValueError('Count times length does not match number of readings.')
 
     if expected_time is False:
         expected_time = count_times.median()
         print('Using median count time as expected count time:', expected_time)
@@ -181,84 +159,70 @@
         idx_nan = np.where(count_times < time_threshold)
         counts.loc[idx_nan] = np.nan
 
     # Fill missing values with linear interpolation and round to nearest integer
     counts = counts.interpolate(method='linear', limit=limit, limit_direction='both').round()
     return counts
 
-def normalize_counts(counts, count_time=3600, count_times=None, timestamp_col=None):
+def normalize_counts(counts, count_time=3600, count_times=None):
     """Normalize neutron counts to the desired counting time.
     
     Args:
         counts (pandas.DataFrame): Dataframe containing only the columns with neutron counts.
         count_time (int): Count time in seconds for normalization. Default is 3600 seconds.
-        count_times (pandas.Series or pandas.DataFrame): Counting time in seconds. If a DataFrame is provided, it must have the same number of columns as counts.
-        timestamp_col (pandas.Series): Timestamp column, used to calculate count time if count_times is not provided, it must have the same number of rows as counts.
+        count_times (pandas.Series or pandas.DataFrame): Counting time in seconds. If a DataFrame is provided, it must have the same number of columns as df.
         
     Returns:
         (pandas.DataFrame): Normalized neutron counts.
 
     """
 
     if count_times is None and type(counts.index) == pd.core.indexes.datetimes.DatetimeIndex:
         print("No count_times columns provided. Using timestamp index to compute count time.")
         count_times = counts.index.to_series().diff().dt.total_seconds()
 
-    elif count_times is None and not isinstance(timestamp_col, type(None)):
-        if len(timestamp_col) != len(counts):
-            raise ValueError('Timestamp column length does not match number of readings.')
-        print("No count_times columns provided. Using timestamp column to compute count time.")
-        if timestamp_col.dtype != 'datetime64[ns]':
-            raise TypeError('Timestamp column must be a pandas Series with datetime64[ns] dtype.')
-        count_times = count_time(timestamp_col=timestamp_col)
-
-
     if isinstance(count_times, type(None)):
-        raise ValueError('Count time must be provided, or `timestamp_col` must be provided, or counts must have a DatetimeIndex.')
+        raise ValueError('Count time must be provided or index must be a timestamp.')
 
     if len(counts) != len(count_times):
         raise ValueError('Count times length does not match number of readings.')
 
+
     #Normalize counts rounded to integer
     if type(count_times) == pd.core.series.Series or len(count_times.columns) == 1:
         normalized_counts = counts.div(count_times, axis=0).mul(count_time).round()
         return normalized_counts
     else:
         normalized_counts = counts.copy()
         count_times = count_times.copy()
         for i in range(len(count_times.columns)):
             normalized_counts[normalized_counts.columns[i]] = normalized_counts.iloc[:,i].div(count_times.iloc[:,i], axis=0).mul(count_time).round()
         return normalized_counts
 
 
-def compute_total_raw_counts(counts, nan_strategy=None, timestamp_col=None):
+
+def compute_total_raw_counts(counts, nan_strategy=None):
     """Compute the sum of uncorrected neutron counts for all detectors.
 
     Args:
         counts (pandas.DataFrame): Dataframe containing only the columns with neutron counts.
         nan_strategy (str): Strategy to use for NaN values. Options are 'interpolate', 'average', or None. Default is None.
 
     Returns:
         (pandas.DataFrame): Dataframe with the sum of uncorrected neutron counts for all detectors.
     """
-
     counts=counts.copy()
 
     if counts.isnull().values.any():
         if nan_strategy is None:
             raise ValueError('NaN values found. Please fill missing values or provide a strategy. See documentation for more information.')
         elif nan_strategy == 'interpolate':
             print('NaN values found. Interpolating missing values using fill_counts().')
-            if not isinstance(timestamp_col, type(None)):
-                if type(timestamp_col) != pd.core.series.Series:
-                    if timestamp_col.dtype != 'datetime64[ns]':
-                        raise TypeError('Timestamp column must be a pandas Series with datetime64[ns] dtype.')
-                counts = fill_counts(counts, timestamp_col)
-            elif type(counts.index) != pd.core.indexes.datetimes.DatetimeIndex:
-                raise ValueError('`timestamp_col` must be provided if `counts` does not have a DatetimeIndex.')
+            if type(counts.index) != pd.core.indexes.datetimes.DatetimeIndex:
+                raise ValueError('Index must be a timestamp to use interpolation strategy.')
             counts = fill_counts(counts)
         elif nan_strategy == 'average':
             if len(counts.columns) == 1:
                 raise ValueError('Only one detector found. Cannot use average strategy.')
             print('NaN values found. Replacing missing values with average of other detectors before summing.')
             counts = counts.apply(lambda x: x.fillna(counts.mean(axis=1)),axis=0)
         else:
@@ -286,14 +250,15 @@
         or
         (pandas.DataFrame, pandas.DataFrame): Dataframe without outliers and dataframe with outliers.
 
     References:
         Iglewicz, B. and Hoaglin, D.C., 1993. How to detect and handle outliers (Vol. 16). Asq Press.
     """
 
+
     if min_counts is not None:
         lower_count = np.sum(raw_counts < min_counts)
         if lower_count > len(raw_counts) * 0.25:
             print(f"WARNING: Discarded {lower_count} counts below {min_counts}. This is more than 25% of the total number of readings. Consider increasing the minimum counts threshold.")
         else:
             print(f"Discarded counts below {min_counts}: {lower_count}")
         raw_counts = raw_counts[raw_counts >= min_counts]
@@ -520,15 +485,15 @@
     # Interpolate nan values
     df_flux = df_flux['counts'].interpolate(method='nearest', limit_direction='both')
 
     # Retur only the values for the selected timestamps
     return df_flux.loc[timestamps]
 
 
-def smooth_1d(corrected_counts, window=5, order=3, method='moving_median'):
+def smooth_1D(corrected_counts,window=5,order=3, method='moving_median'):
     """Use a Savitzky-Golay filter to smooth the signal of corrected neutron counts or another one-dimensional array (e.g. computed volumetric water content).
 
     Args:
         corrected_counts (pd.DataFrame): Dataframe containing the corrected neutron counts.
         window (int): Window size for the Savitzky-Golay filter. Default is 5.
         method (str): Method to use for smoothing the data. Default is 'moving_median'.
             Options are 'moving_average', 'moving_median' and 'savitzky_golay'.
@@ -984,15 +949,15 @@
 
 
 def estimate_lattice_water(clay_content, total_carbon=None):
     r"""Estimate the amount of water in the lattice of clay minerals.
 
     ![img1](img/lattice_water_simple.png) | ![img2](img/lattice_water_multiple.png)
     :-------------------------:|:-------------------------:
-    $\omega_{lat} = 0.097 * clay(\%)$ | $\omega_{lat} = -0.028 + 0.077 * clay(\%) + 0.459 * carbon(\%)$
+    $\omega_{lat} = 1.241 + 0.069 * clay(\%)$ | $\omega_{lat} = -0.028 + 0.077 * clay(\%) + 0.459 * carbon(\%)$
     Linear regression [lattice water (%) as a function of clay (%)] done with data from Soil Water Processes Lab and Dong and Ochsner (2018) |  Multiple linear regression [lattice water (%) as a function of clay (%) and soil carbon (%)] done with data from Soil Water Processes Lab.
 
     Args:
         clay_content (float): Clay content in the soil in percent.
         total_carbon (float, optional): Total carbon content in the soil in percent.
             If None, the amount of water is estimated based on clay content only.
 
@@ -1002,15 +967,15 @@
     References:
         Dong, J., & Ochsner, T. E. (2018). Soil texture often exerts a stronger influence than precipitation
          on mesoscale soil moisture patterns. Water Resources Research, 54, 2199– 2211.
          https://doi.org/10.1002/2017WR021692
 
     """
     if total_carbon is None:
-        lattice_water = 0.097 * clay_content
+        lattice_water = 1.241 + 0.069 * clay_content
     else:
         lattice_water = -0.028 + 0.077 * clay_content + 0.459 * total_carbon
     return lattice_water
 
 
 def latlon_to_utm(lat, lon, utm_zone_number, missing_values=None):
     """Convert geographic coordinates (lat, lon) to projected coordinates (utm) using the Military Grid Reference System.
@@ -1112,15 +1077,15 @@
     Returns:
         (ndarray): Numpy array of distances from the point (px,py) to all the points in x and y vectors.
     """
     d = np.sqrt((px - x) ** 2 + (py - y) ** 2)
     return d
 
 
-def smooth_2d(x, y, z, buffer=100, min_neighbours=3, method='mean', rnd=False):
+def smooth_2D(x, y, z, buffer=100, min_neighbours=3, method='mean', rnd=False):
     """Moving buffer filter to smooth georeferenced two-dimensional data.
 
     Args:
         x (list or array): UTM x coordinates in meters.
         y (list or array): UTM y coordinates in meters.
         z (list or array): Values to be smoothed.
         buffer (float): Radial buffer distance in meters.
@@ -1187,15 +1152,15 @@
         neighborhood (float): Only points within this radius in meters are considered for the interpolation.
         p (int): Exponent of the inverse distance weight formula. Typically, p=1 or p=2.
 
     Returns:
         (array): Interpolated values.
 
     References:
-        [https://en.wikipedia.org/wiki/Inverse_distance_weighting](https://en.wikipedia.org/wiki/Inverse_distance_weighting)
+        [https://soilwater.github.io/pynotes-agriscience/notebooks/inverse_distance_weighting.html](https://soilwater.github.io/pynotes-agriscience/notebooks/inverse_distance_weighting.html)
 
 
     """
 
     # Flatten arrays to handle 1D and 2D arrays with the same code
     s = X_pred.shape  # Save shape
     X_pred = X_pred.flatten()
@@ -1204,24 +1169,24 @@
     # Pre-allocate output array
     Z_pred = np.full_like(X_pred, np.nan)
 
     for n in range(X_pred.size):
         # Distance between current and observed points
         d = euclidean_distance(X_pred[n], Y_pred[n], x, y)
 
-        # Select points within neighborhood only for interpolation
+        # Select points within neighborhood only for interpolateion
         idx_neighbors = d < neighborhood
 
         # Compute interpolated value at point of interest
         Z_pred[n] = np.sum(z[idx_neighbors] / d[idx_neighbors] ** p) / np.sum(1 / d[idx_neighbors] ** p)
 
     return np.reshape(Z_pred, s)
 
 
-def interpolate_2d(x, y, z, dx=100, dy=100, method='cubic', neighborhood=1000):
+def interpolate_2D(x, y, z, dx=100, dy=100, method='cubic', neighborhood=1000):
     """Function for interpolating irregular spatial data into a regular grid.
 
     Args:
         x (list or array): UTM x coordinates in meters.
         y (list or array): UTM y coordinates in meters.
         z (list or array): Values to be interpolated.
         dx (float): Pixel width in meters.
```

### Comparing `crnpy-0.3.2/src/crnpy/data.py` & `crnpy-0.3.post1/src/crnpy/data.py`

 * *Files identical despite different names*

