# Comparing `tmp/feiertage-de-0.1.0.tar.gz` & `tmp/feiertage-de-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "feiertage-de-0.1.0.tar", last modified: Fri Jun 16 00:22:52 2023, max compression
+gzip compressed data, was "feiertage-de-0.1.1.tar", last modified: Thu Jun 22 22:42:58 2023, max compression
```

## Comparing `feiertage-de-0.1.0.tar` & `feiertage-de-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-16 00:22:52.151642 feiertage-de-0.1.0/
--rw-r--r--   0 michael   (1000) michael   (1000)     1075 2023-06-15 13:29:01.000000 feiertage-de-0.1.0/LICENSE
--rw-r--r--   0 michael   (1000) michael   (1000)      834 2023-06-16 00:22:52.151642 feiertage-de-0.1.0/PKG-INFO
--rw-r--r--   0 michael   (1000) michael   (1000)      107 2023-06-15 14:47:17.000000 feiertage-de-0.1.0/README.md
--rw-r--r--   0 michael   (1000) michael   (1000)      769 2023-06-16 00:22:43.000000 feiertage-de-0.1.0/pyproject.toml
--rw-r--r--   0 michael   (1000) michael   (1000)       38 2023-06-16 00:22:52.151642 feiertage-de-0.1.0/setup.cfg
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-16 00:22:52.151642 feiertage-de-0.1.0/src/
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-16 00:22:52.151642 feiertage-de-0.1.0/src/feiertage/
--rw-r--r--   0 michael   (1000) michael   (1000)     7189 2023-06-15 22:53:08.000000 feiertage-de-0.1.0/src/feiertage/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)     1501 2023-06-15 22:47:11.000000 feiertage-de-0.1.0/src/feiertage/easter.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-16 00:22:52.151642 feiertage-de-0.1.0/src/feiertage_de.egg-info/
--rw-r--r--   0 michael   (1000) michael   (1000)      834 2023-06-16 00:22:52.000000 feiertage-de-0.1.0/src/feiertage_de.egg-info/PKG-INFO
--rw-r--r--   0 michael   (1000) michael   (1000)      242 2023-06-16 00:22:52.000000 feiertage-de-0.1.0/src/feiertage_de.egg-info/SOURCES.txt
--rw-r--r--   0 michael   (1000) michael   (1000)        1 2023-06-16 00:22:52.000000 feiertage-de-0.1.0/src/feiertage_de.egg-info/dependency_links.txt
--rw-r--r--   0 michael   (1000) michael   (1000)       10 2023-06-16 00:22:52.000000 feiertage-de-0.1.0/src/feiertage_de.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 22:42:58.251434 feiertage-de-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-06-22 22:42:44.000000 feiertage-de-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-06-22 22:42:58.251434 feiertage-de-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-06-22 22:42:44.000000 feiertage-de-0.1.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-06-22 22:42:44.000000 feiertage-de-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 22:42:58.251434 feiertage-de-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 22:42:58.251434 feiertage-de-0.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 22:42:58.251434 feiertage-de-0.1.1/src/feiertage/
+-rw-r--r--   0 runner    (1001) docker     (123)     8566 2023-06-22 22:42:44.000000 feiertage-de-0.1.1/src/feiertage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-06-22 22:42:44.000000 feiertage-de-0.1.1/src/feiertage/easter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 22:42:58.251434 feiertage-de-0.1.1/src/feiertage_de.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-06-22 22:42:58.000000 feiertage-de-0.1.1/src/feiertage_de.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-22 22:42:58.000000 feiertage-de-0.1.1/src/feiertage_de.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 22:42:58.000000 feiertage-de-0.1.1/src/feiertage_de.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-22 22:42:58.000000 feiertage-de-0.1.1/src/feiertage_de.egg-info/top_level.txt
```

### Comparing `feiertage-de-0.1.0/LICENSE` & `feiertage-de-0.1.1/LICENSE`

 * *Files 12% similar despite different names*

```diff
@@ -15,7 +15,9 @@
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
+
+If you want you can send me a postcard for using this python package and I would be really pleased to receive some. You can find my address at the imprint of my website: https://spice-space.de/inhalt/impressum/
```

### Comparing `feiertage-de-0.1.0/pyproject.toml` & `feiertage-de-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "feiertage-de"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
 	{ name="Michael Hohenstein", email="michael@hohenste.in" },
 ]
 description = ""
-readme = "README.md"
+readme = "README.rst"
 requires-python= ">=3.7"
 classifiers = [
 	"Operating System :: OS Independent",
 	"Programming Language :: Python :: 3",
 	"Natural Language :: German",
 	"Topic :: Office/Business",
 	"Topic :: Office/Business :: Scheduling",
```

### Comparing `feiertage-de-0.1.0/src/feiertage/__init__.py` & `feiertage-de-0.1.1/src/feiertage/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,15 @@
 #!/usr/bin/env python3
-# -*- encoding: utf8 -*-
+
+__docformat__ = "numpy"
+
+"""Calculate the holidays for a specified federal state of Germany within a given year
+
+During the initialisation of a `Holiday` object all the holidays for the given state within the given year will be calculated. These will be assigned by the following table: https://de.wikipedia.org/wiki/Gesetzliche_Feiertage_in_Deutschland#%C3%9Cbersicht_aller_gesetzlichen_Feiertage
+"""
 
 import sys
 from datetime import date, timedelta
 from . import easter
 
 states = {
     'Deutschland':'DE',
@@ -22,32 +28,56 @@
     'Sachsen':'SN',
     'Sachsen-Anhalt':'ST',
     'Schleswig-Holstein':'SH',
     'Thüringen':'TH',
 }
 
 class Holidays:
+    """
+    Parameters
+    ---------
+    state : str
+        The state code for the federal state for which the holidays should be calculated. This parameter can either be the name of the state or a short state code, p.Ex. 'Baden-Württemberg' and 'BW' would both be a valid option. Furthermore the option 'Deutschland' / 'DE' gives a list of only the holidays which all the federal states commonly share. The list of all the valid state codes is stored in the dictionary `feiertage.states`:
+
+            - 'Deutschland' / 'DE',
+            - 'Baden-Württemberg' / 'BW',
+            - 'Bayern' / 'BY',
+            - 'Berlin' / 'BE',
+            - 'Brandenburg' / 'BB',
+            - 'Bremen' / 'HB',
+            - 'Hamburg' / 'HH',
+            - 'Hessen' / 'HE',
+            - 'Mecklenburg-Vorpommern' / 'MV',
+            - 'Niedersachsen' / 'NI',
+            - 'Nordrhein-Westfalen' / 'NW',
+            - 'Rheinland-Pfalz' / 'RP',
+            - 'Saarland' / 'SL',
+            - 'Sachsen' / 'SN',
+            - 'Sachsen-Anhalt' / 'ST',
+            - 'Schleswig-Holstein' / 'SH',
+            - 'Thüringen' / 'TH',
+
+    year : int, optional
+        the year for which the holidays should be calculated
+    regional : boolean, default=False
+        Optionally enable some regional holidays which are only valid in some communities. These would be the following ones:
+
+            - Fronleichnam in SL and TH
+            - Augsburger Hohes Friedensfest in BY
+            - Matiä Himmelfahrt in BY
+
+    school_free : boolean, default=False
+        Optionally enable some days which are not holidays but there is no school. These would be the following ones:
+
+            - Gründonnerstag in BW
+            - Reformationstag in BW
+            - Buß- und Bettag in BY
+    """
 
     def __init__(self, state : str, year : int = date.today().year, regional : bool = False, school_free : bool = False):
-        """
-        Create an object of the class 'Hoiday'
-        During the initialisation a list of all holidays will be calculated. The holidays will only be calculated ones and then stored internally inside a dictionary.
-        Teh national holidays will be assigned to the federal states by the following table: https://de.wikipedia.org/wiki/Gesetzliche_Feiertage_in_Deutschland#%C3%9Cbersicht_aller_gesetzlichen_Feiertage
-
-        Parameters
-        ----------
-        state : str
-            the state code of every federal state of germany. These can be seen in the dictionary states. When 'Deutschland' or 'DE' is selected only national wide holidays will be generated
-        year : int
-            the year for which the holidays should be calculated, default will be the current year. If the year is before 1970 it will be reset to 1970
-        regional : bool
-            also include regional holidays in the list
-        school_free : bool
-            also include school free days which are not national wide holidays
-        """
         # parse the year so it can be stored internally as self.year as an integer
         try:
             self.year = int(year)
             if self.year < 1970:
                 self.year = 1970
                 print(sys.stderr, "Year was reset to 1970") # TODO: throw exception instead
         except ValueError:
@@ -151,8 +181,15 @@
         if ( self.state in ["SN"] ) or ( self.state in ["BY"] and self._school_free == True ):
             day = date(self.year, 11, 22)
             while day.weekday() != 2:
                 day = day - timedelta(days = 1)
             self.holidays.append({'date':day, 'name':'Buß und Bettag'})
 
     def get_holidays_list(self) -> list :
+        """Get a list of only the dates for all holidays stored in a datetime.date object
+
+        Returns
+        -------
+            holidays : list of datetime.date objects
+                Each entry in this list is a `date` object which points to a holiday
+        """
         return [ i['date'] for i in self.holidays]
```

### Comparing `feiertage-de-0.1.0/src/feiertage/easter.py` & `feiertage-de-0.1.1/src/feiertage/easter.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,35 @@
 #!/usr/bin/env python3
 # -*- encoding: utf8 -*-
 
+__docformat__ = "numpy"
+
 from datetime import date
-from math import floor
 
 def calc_easter(year : int) -> date :
-    """
-    Calculating the date of Easter by Karl Friedrich Gauss
-    Detailed description can be read on the following website: https://de.wikipedia.org/wiki/Gau%C3%9Fsche_Osterformel
+    """Calculates the date of easter.
+
+    The calculation of the Easter Sunday by following the formula by Karl Friedrich Gauss.
+    A Detailed description can be read on the following website: https://de.wikipedia.org/wiki/Gau%C3%9Fsche_Osterformel
+
+    Args:
+    -----
+        year : int
+            The year for which the date of Easter should be calculated
+
+    Returns:
+    --------
+        easter_day : date
+            A datetime object which is set to the date of easter
 
-    Parameters
-    ----------
-    year : int
-        the year in which the date of Easter should be calculated
-
-    Returns
-    -------
-    easter_day : date
-        A datetime object which is set to the date of easter
+    Examples:
+    ---------
+        >>> from feiertage import easter
+        >>> easter.calc_easter(2023)    # example year: 2023
+        datetime.date(2023,4,9)
     """
 
     K = year // 100                                 # Säkular-zahl
     M = 15 + (3 * K + 3) // 4 - (8 * K + 13) // 25  # säkulare Mondschaltung
     S = 2 - (3 * K + 3) // 4                        # säkulare Sonnenschaltung
     A = year % 19                                   # Mondparameter
     D = (19 * A + M) % 30                           # Keim für den ersten Vollmond im Frühling
```

