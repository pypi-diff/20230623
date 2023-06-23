# Comparing `tmp/QuantStats-0.0.8.tar.gz` & `tmp/QuantStats-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/QuantStats-0.0.8.tar", last modified: Sun May 12 15:54:22 2019, max compression
+gzip compressed data, was "dist/QuantStats-0.0.9.tar", last modified: Sun May 19 19:59:33 2019, max compression
```

## Comparing `QuantStats-0.0.8.tar` & `QuantStats-0.0.9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 ran        (501) staff       (20)        0 2019-05-12 15:54:22.000000 QuantStats-0.0.8/
--rw-r--r--   0 ran        (501) staff       (20)    11358 2018-09-03 18:24:08.000000 QuantStats-0.0.8/LICENSE.txt
--rw-r--r--   0 ran        (501) staff       (20)      129 2019-05-07 14:29:23.000000 QuantStats-0.0.8/MANIFEST.in
--rw-r--r--   0 ran        (501) staff       (20)    10512 2019-05-12 15:54:22.000000 QuantStats-0.0.8/PKG-INFO
-drwxr-xr-x   0 ran        (501) staff       (20)        0 2019-05-12 15:54:22.000000 QuantStats-0.0.8/QuantStats.egg-info/
--rw-r--r--   0 ran        (501) staff       (20)    10512 2019-05-12 15:54:21.000000 QuantStats-0.0.8/QuantStats.egg-info/PKG-INFO
--rw-r--r--   0 ran        (501) staff       (20)      472 2019-05-12 15:54:21.000000 QuantStats-0.0.8/QuantStats.egg-info/SOURCES.txt
--rw-r--r--   0 ran        (501) staff       (20)        1 2019-05-12 15:54:21.000000 QuantStats-0.0.8/QuantStats.egg-info/dependency_links.txt
--rw-r--r--   0 ran        (501) staff       (20)       40 2019-05-12 15:54:21.000000 QuantStats-0.0.8/QuantStats.egg-info/entry_points.txt
--rw-r--r--   0 ran        (501) staff       (20)      117 2019-05-12 15:54:21.000000 QuantStats-0.0.8/QuantStats.egg-info/requires.txt
--rw-r--r--   0 ran        (501) staff       (20)       11 2019-05-12 15:54:21.000000 QuantStats-0.0.8/QuantStats.egg-info/top_level.txt
--rw-r--r--   0 ran        (501) staff       (20)     7043 2019-05-08 17:45:09.000000 QuantStats-0.0.8/README.rst
-drwxr-xr-x   0 ran        (501) staff       (20)        0 2019-05-12 15:54:22.000000 QuantStats-0.0.8/quantstats/
--rw-r--r--   0 ran        (501) staff       (20)     4714 2019-05-12 15:47:26.000000 QuantStats-0.0.8/quantstats/__init__.py
-drwxr-xr-x   0 ran        (501) staff       (20)        0 2019-05-12 15:54:22.000000 QuantStats-0.0.8/quantstats/_plotting/
--rw-r--r--   0 ran        (501) staff       (20)      713 2019-05-07 14:00:24.000000 QuantStats-0.0.8/quantstats/_plotting/__init__.py
--rw-r--r--   0 ran        (501) staff       (20)    22575 2019-05-12 15:52:28.000000 QuantStats-0.0.8/quantstats/_plotting/core.py
--rw-r--r--   0 ran        (501) staff       (20)    21333 2019-05-12 15:52:23.000000 QuantStats-0.0.8/quantstats/_plotting/wrappers.py
--rw-r--r--   0 ran        (501) staff       (20)      758 2019-05-07 14:00:24.000000 QuantStats-0.0.8/quantstats/plots.py
--rw-r--r--   0 ran        (501) staff       (20)     3601 2019-05-11 12:16:55.000000 QuantStats-0.0.8/quantstats/report.html
--rw-r--r--   0 ran        (501) staff       (20)    23351 2019-05-12 15:51:47.000000 QuantStats-0.0.8/quantstats/reports.py
--rw-r--r--   0 ran        (501) staff       (20)    21877 2019-05-12 15:51:57.000000 QuantStats-0.0.8/quantstats/stats.py
--rw-r--r--   0 ran        (501) staff       (20)     9496 2019-05-12 15:52:02.000000 QuantStats-0.0.8/quantstats/utils.py
--rw-r--r--   0 ran        (501) staff       (20)       38 2019-05-12 15:54:22.000000 QuantStats-0.0.8/setup.cfg
--rw-r--r--   0 ran        (501) staff       (20)     2651 2019-05-12 15:47:31.000000 QuantStats-0.0.8/setup.py
+drwxr-xr-x   0 ran        (501) staff       (20)        0 2019-05-19 19:59:33.000000 QuantStats-0.0.9/
+-rw-r--r--   0 ran        (501) staff       (20)    11358 2018-09-03 18:24:08.000000 QuantStats-0.0.9/LICENSE.txt
+-rw-r--r--   0 ran        (501) staff       (20)      129 2019-05-07 14:29:23.000000 QuantStats-0.0.9/MANIFEST.in
+-rw-r--r--   0 ran        (501) staff       (20)    10512 2019-05-19 19:59:33.000000 QuantStats-0.0.9/PKG-INFO
+drwxr-xr-x   0 ran        (501) staff       (20)        0 2019-05-19 19:59:33.000000 QuantStats-0.0.9/QuantStats.egg-info/
+-rw-r--r--   0 ran        (501) staff       (20)    10512 2019-05-19 19:59:33.000000 QuantStats-0.0.9/QuantStats.egg-info/PKG-INFO
+-rw-r--r--   0 ran        (501) staff       (20)      472 2019-05-19 19:59:33.000000 QuantStats-0.0.9/QuantStats.egg-info/SOURCES.txt
+-rw-r--r--   0 ran        (501) staff       (20)        1 2019-05-19 19:59:33.000000 QuantStats-0.0.9/QuantStats.egg-info/dependency_links.txt
+-rw-r--r--   0 ran        (501) staff       (20)       40 2019-05-19 19:59:33.000000 QuantStats-0.0.9/QuantStats.egg-info/entry_points.txt
+-rw-r--r--   0 ran        (501) staff       (20)      117 2019-05-19 19:59:33.000000 QuantStats-0.0.9/QuantStats.egg-info/requires.txt
+-rw-r--r--   0 ran        (501) staff       (20)       11 2019-05-19 19:59:33.000000 QuantStats-0.0.9/QuantStats.egg-info/top_level.txt
+-rw-r--r--   0 ran        (501) staff       (20)     7043 2019-05-08 17:45:09.000000 QuantStats-0.0.9/README.rst
+drwxr-xr-x   0 ran        (501) staff       (20)        0 2019-05-19 19:59:33.000000 QuantStats-0.0.9/quantstats/
+-rw-r--r--   0 ran        (501) staff       (20)     4685 2019-05-19 19:53:01.000000 QuantStats-0.0.9/quantstats/__init__.py
+drwxr-xr-x   0 ran        (501) staff       (20)        0 2019-05-19 19:59:33.000000 QuantStats-0.0.9/quantstats/_plotting/
+-rw-r--r--   0 ran        (501) staff       (20)      713 2019-05-13 12:22:54.000000 QuantStats-0.0.9/quantstats/_plotting/__init__.py
+-rw-r--r--   0 ran        (501) staff       (20)    22575 2019-05-12 15:52:28.000000 QuantStats-0.0.9/quantstats/_plotting/core.py
+-rw-r--r--   0 ran        (501) staff       (20)    21350 2019-05-19 19:51:34.000000 QuantStats-0.0.9/quantstats/_plotting/wrappers.py
+-rw-r--r--   0 ran        (501) staff       (20)      875 2019-05-13 12:23:03.000000 QuantStats-0.0.9/quantstats/plots.py
+-rw-r--r--   0 ran        (501) staff       (20)     3601 2019-05-11 12:16:55.000000 QuantStats-0.0.9/quantstats/report.html
+-rw-r--r--   0 ran        (501) staff       (20)    23351 2019-05-12 15:51:47.000000 QuantStats-0.0.9/quantstats/reports.py
+-rw-r--r--   0 ran        (501) staff       (20)    21877 2019-05-12 15:51:57.000000 QuantStats-0.0.9/quantstats/stats.py
+-rw-r--r--   0 ran        (501) staff       (20)    10092 2019-05-19 19:51:41.000000 QuantStats-0.0.9/quantstats/utils.py
+-rw-r--r--   0 ran        (501) staff       (20)       38 2019-05-19 19:59:33.000000 QuantStats-0.0.9/setup.cfg
+-rw-r--r--   0 ran        (501) staff       (20)     2651 2019-05-19 19:53:05.000000 QuantStats-0.0.9/setup.py
```

### Comparing `QuantStats-0.0.8/LICENSE.txt` & `QuantStats-0.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `QuantStats-0.0.8/PKG-INFO` & `QuantStats-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: QuantStats
-Version: 0.0.8
+Version: 0.0.9
 Summary: Portfolio analytics for quants
 Home-page: https://github.com/ranaroussi/quantstats
 Author: Ran Aroussi
 Author-email: ran@aroussi.com
 License: Apache Software License
 Description: .. image:: https://img.shields.io/badge/python-3.5+-blue.svg?style=flat
             :target: https://pypi.python.org/pypi/quantstats
```

### Comparing `QuantStats-0.0.8/QuantStats.egg-info/PKG-INFO` & `QuantStats-0.0.9/QuantStats.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: QuantStats
-Version: 0.0.8
+Version: 0.0.9
 Summary: Portfolio analytics for quants
 Home-page: https://github.com/ranaroussi/quantstats
 Author: Ran Aroussi
 Author-email: ran@aroussi.com
 License: Apache Software License
 Description: .. image:: https://img.shields.io/badge/python-3.5+-blue.svg?style=flat
             :target: https://pypi.python.org/pypi/quantstats
```

### Comparing `QuantStats-0.0.8/README.rst` & `QuantStats-0.0.9/README.rst`

 * *Files identical despite different names*

### Comparing `QuantStats-0.0.8/quantstats/__init__.py` & `QuantStats-0.0.9/quantstats/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,34 +14,29 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "0.0.08"
+__version__ = "0.0.09"
 __author__ = "Ran Aroussi"
 
-from pandas.core.base import PandasObject as _po
 from . import stats, utils, plots, reports
 
-try:
-    from pandas.plotting import register_matplotlib_converters as _rmc
-    _rmc()
-except ImportError:
-    pass
-
 __all__ = ['stats', 'plots', 'reports', 'utils', 'extend_pandas']
 
 
 def extend_pandas():
     """
     extends pandas by exposing methods to be used like:
     df.sharpe(), df.best('day'), ...
     """
+    from pandas.core.base import PandasObject as _po
+
     _po.compsum = stats.compsum
     _po.comp = stats.comp
     _po.expected_return = stats.expected_return
     _po.geometric_mean = stats.geometric_mean
     _po.ghpr = stats.ghpr
     _po.outliers = stats.outliers
     _po.remove_outliers = stats.remove_outliers
@@ -97,14 +92,16 @@
     _po.to_log_returns = utils.to_log_returns
     _po.log_returns = utils.log_returns
     _po.exponential_stdev = utils.exponential_stdev
     _po.rebase = utils.rebase
     _po.aggregate_returns = utils.aggregate_returns
     _po.to_excess_returns = utils.to_excess_returns
     _po.multi_shift = utils.multi_shift
+    _po.curr_month = utils._pandas_current_month
+    _po.date = utils._pandas_date
 
     # methods that requires benchmark stats
     _po.r_squared = stats.r_squared
     _po.r2 = stats.r2
     _po.information_ratio = stats.information_ratio
     _po.greeks = stats.greeks
     _po.rolling_greeks = stats.rolling_greeks
```

### Comparing `QuantStats-0.0.8/quantstats/_plotting/__init__.py` & `QuantStats-0.0.9/quantstats/_plotting/__init__.py`

 * *Files identical despite different names*

### Comparing `QuantStats-0.0.8/quantstats/_plotting/core.py` & `QuantStats-0.0.9/quantstats/_plotting/core.py`

 * *Files identical despite different names*

### Comparing `QuantStats-0.0.8/quantstats/_plotting/wrappers.py` & `QuantStats-0.0.9/quantstats/_plotting/wrappers.py`

 * *Files 1% similar despite different names*

```diff
@@ -152,24 +152,24 @@
 
     _plt.close()
 
     if not show:
         return fig
 
 
-def earnings(returns, start_balance=1e5,
+def earnings(returns, start_balance=1e5, mode="sum",
              grayscale=False, figsize=(10, 6),
              title='Portfolio Earnings',
              fontname='Arial', lw=1.5,
              subtitle=True, savefig=None, show=True):
 
     colors = _GRAYSCALE_COLORS if grayscale else _FLATUI_COLORS
     alpha = .5 if grayscale else .8
 
-    returns = _utils._make_portfolio(returns, start_balance)
+    returns = _utils.make_portfolio(returns, start_balance, mode)
 
     if figsize is None:
         size = list(_plt.gcf().get_size_inches())
         figsize = (size[0], size[0]*.55)
 
     fig, ax = _plt.subplots(figsize=figsize)
     fig.suptitle(title, fontsize=14, y=.995,
```

### Comparing `QuantStats-0.0.8/quantstats/plots.py` & `QuantStats-0.0.9/quantstats/plots.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,8 +14,14 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+try:
+    from pandas.plotting import register_matplotlib_converters as _rmc
+    _rmc()
+except ImportError:
+    pass
+
 from quantstats._plotting.wrappers import *
```

### Comparing `QuantStats-0.0.8/quantstats/report.html` & `QuantStats-0.0.9/quantstats/report.html`

 * *Files identical despite different names*

### Comparing `QuantStats-0.0.8/quantstats/reports.py` & `QuantStats-0.0.9/quantstats/reports.py`

 * *Files identical despite different names*

### Comparing `QuantStats-0.0.8/quantstats/stats.py` & `QuantStats-0.0.9/quantstats/stats.py`

 * *Files identical despite different names*

### Comparing `QuantStats-0.0.8/quantstats/utils.py` & `QuantStats-0.0.9/quantstats/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,20 +14,33 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import io as _io
+import datetime as _dt
 import pandas as _pd
 import numpy as _np
 import fix_yahoo_finance as _yf
 from . import stats as _stats
 
 
+def _pandas_date(df, dates):
+    if not isinstance(dates, list):
+        dates = [dates]
+    return df[df.index.isin(dates)]
+
+
+def _pandas_current_month(df):
+    n = _dt.datetime.now()
+    daterange = _pd.date_range(_dt.date(n.year, n.month, 1), n)
+    return df[df.index.isin(daterange)]
+
+
 def multi_shift(df, shift=3):
     """
     get last N rows relative to another row in pandas
     """
     if isinstance(df, _pd.Series):
         df = _pd.DataFrame(df)
     dfs = [df.shift(i) for i in _np.arange(shift)]
@@ -272,21 +285,28 @@
 def _score_str(val):
     """
     Returns + sign for positive values (used in plots)
     """
     return ("" if "-" in val else "+") + str(val)
 
 
-def _make_portfolio(returns, start_balance=1e5, round_to=None):
+def make_portfolio(returns, start_balance=1e5,
+                   mode="sum", round_to=None):
     """
     Calculates compounded value of portfolio
     """
-    comp_rev = (start_balance + start_balance *
-                returns.shift(1)).fillna(start_balance) * returns
-    p1 = start_balance + comp_rev.cumsum()
+    if mode.lower() in ["cumsum", "sum"]:
+        p1 = start_balance + start_balance * returns.cumsum()
+    elif mode.lower() in ["compsum", "comp"]:
+        p1 = to_prices(returns, start_balance)
+    else:
+        # fixed amount every day
+        comp_rev = (start_balance + start_balance *
+                    returns.shift(1)).fillna(start_balance) * returns
+        p1 = start_balance + comp_rev.cumsum()
 
     # add day before with starting balance
     p0 = _pd.Series(data=start_balance,
                     index=p1.index + _pd.Timedelta(days=-1))[:1]
 
     portfolio = _pd.concat([p0, p1])
```

### Comparing `QuantStats-0.0.8/setup.py` & `QuantStats-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 # Get the long description from the README file
 with open(path.join(here, 'README.rst'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='QuantStats',
-    version='0.0.08',
+    version='0.0.09',
     description='Portfolio analytics for quants',
     long_description=long_description,
     url='https://github.com/ranaroussi/quantstats',
     author='Ran Aroussi',
     author_email='ran@aroussi.com',
     license='Apache Software License',
     classifiers=[
```

