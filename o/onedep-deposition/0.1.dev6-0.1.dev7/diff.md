# Comparing `tmp/onedep_deposition-0.1.dev6.tar.gz` & `tmp/onedep_deposition-0.1.dev7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onedep_deposition-0.1.dev6.tar", last modified: Wed Jun 21 13:40:39 2023, max compression
+gzip compressed data, was "onedep_deposition-0.1.dev7.tar", last modified: Fri Jun 23 11:14:01 2023, max compression
```

## Comparing `onedep_deposition-0.1.dev6.tar` & `onedep_deposition-0.1.dev7.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 peisach    (502) staff       (20)        0 2023-06-21 13:40:39.906260 onedep_deposition-0.1.dev6/
--rw-r--r--   0 peisach    (502) staff       (20)      552 2023-06-13 13:04:02.000000 onedep_deposition-0.1.dev6/LICENSE
--rw-r--r--   0 peisach    (502) staff       (20)     5174 2023-06-21 13:40:39.905965 onedep_deposition-0.1.dev6/PKG-INFO
--rw-r--r--   0 peisach    (502) staff       (20)     4641 2023-06-17 15:30:45.000000 onedep_deposition-0.1.dev6/README.md
-drwxr-xr-x   0 peisach    (502) staff       (20)        0 2023-06-21 13:40:39.902060 onedep_deposition-0.1.dev6/onedep_deposition/
--rw-r--r--   0 peisach    (502) staff       (20)       25 2023-06-21 13:40:22.000000 onedep_deposition-0.1.dev6/onedep_deposition/__init__.py
-drwxr-xr-x   0 peisach    (502) staff       (20)        0 2023-06-21 13:40:39.905135 onedep_deposition-0.1.dev6/onedep_deposition/cli/
--rw-r--r--   0 peisach    (502) staff       (20)        0 2023-06-17 17:42:03.000000 onedep_deposition-0.1.dev6/onedep_deposition/cli/__init__.py
--rw-r--r--   0 peisach    (502) staff       (20)    12637 2023-06-20 13:27:14.000000 onedep_deposition-0.1.dev6/onedep_deposition/cli/cli.py
--rw-r--r--   0 peisach    (502) staff       (20)      589 2023-06-20 13:27:14.000000 onedep_deposition-0.1.dev6/onedep_deposition/decorators.py
--rw-r--r--   0 peisach    (502) staff       (20)    15148 2023-06-21 13:40:11.000000 onedep_deposition-0.1.dev6/onedep_deposition/deposit_api.py
--rw-r--r--   0 peisach    (502) staff       (20)     9006 2023-06-15 13:32:19.000000 onedep_deposition-0.1.dev6/onedep_deposition/enum.py
--rw-r--r--   0 peisach    (502) staff       (20)      316 2023-06-20 13:27:14.000000 onedep_deposition-0.1.dev6/onedep_deposition/exceptions.py
--rw-r--r--   0 peisach    (502) staff       (20)    12847 2023-06-19 17:09:13.000000 onedep_deposition-0.1.dev6/onedep_deposition/models.py
--rw-r--r--   0 peisach    (502) staff       (20)     6182 2023-06-20 13:27:14.000000 onedep_deposition-0.1.dev6/onedep_deposition/rest_adapter.py
-drwxr-xr-x   0 peisach    (502) staff       (20)        0 2023-06-21 13:40:39.904502 onedep_deposition-0.1.dev6/onedep_deposition.egg-info/
--rw-r--r--   0 peisach    (502) staff       (20)     5174 2023-06-21 13:40:39.000000 onedep_deposition-0.1.dev6/onedep_deposition.egg-info/PKG-INFO
--rw-r--r--   0 peisach    (502) staff       (20)      558 2023-06-21 13:40:39.000000 onedep_deposition-0.1.dev6/onedep_deposition.egg-info/SOURCES.txt
--rw-r--r--   0 peisach    (502) staff       (20)        1 2023-06-21 13:40:39.000000 onedep_deposition-0.1.dev6/onedep_deposition.egg-info/dependency_links.txt
--rw-r--r--   0 peisach    (502) staff       (20)       68 2023-06-21 13:40:39.000000 onedep_deposition-0.1.dev6/onedep_deposition.egg-info/entry_points.txt
--rw-r--r--   0 peisach    (502) staff       (20)       15 2023-06-21 13:40:39.000000 onedep_deposition-0.1.dev6/onedep_deposition.egg-info/requires.txt
--rw-r--r--   0 peisach    (502) staff       (20)       18 2023-06-21 13:40:39.000000 onedep_deposition-0.1.dev6/onedep_deposition.egg-info/top_level.txt
--rw-r--r--   0 peisach    (502) staff       (20)     1039 2023-06-17 17:50:36.000000 onedep_deposition-0.1.dev6/pyproject.toml
--rw-r--r--   0 peisach    (502) staff       (20)       38 2023-06-21 13:40:39.906349 onedep_deposition-0.1.dev6/setup.cfg
+drwxr-xr-x   0 peisach    (502) staff       (20)        0 2023-06-23 11:14:01.028679 onedep_deposition-0.1.dev7/
+-rw-r--r--   0 peisach    (502) staff       (20)      552 2023-06-13 13:04:02.000000 onedep_deposition-0.1.dev7/LICENSE
+-rw-r--r--   0 peisach    (502) staff       (20)     5174 2023-06-23 11:14:01.028335 onedep_deposition-0.1.dev7/PKG-INFO
+-rw-r--r--   0 peisach    (502) staff       (20)     4641 2023-06-17 15:30:45.000000 onedep_deposition-0.1.dev7/README.md
+drwxr-xr-x   0 peisach    (502) staff       (20)        0 2023-06-23 11:14:01.021743 onedep_deposition-0.1.dev7/onedep_deposition/
+-rw-r--r--   0 peisach    (502) staff       (20)       25 2023-06-23 11:13:09.000000 onedep_deposition-0.1.dev7/onedep_deposition/__init__.py
+drwxr-xr-x   0 peisach    (502) staff       (20)        0 2023-06-23 11:14:01.027718 onedep_deposition-0.1.dev7/onedep_deposition/cli/
+-rw-r--r--   0 peisach    (502) staff       (20)        0 2023-06-17 17:42:03.000000 onedep_deposition-0.1.dev7/onedep_deposition/cli/__init__.py
+-rw-r--r--   0 peisach    (502) staff       (20)    13091 2023-06-23 11:13:00.000000 onedep_deposition-0.1.dev7/onedep_deposition/cli/cli.py
+-rw-r--r--   0 peisach    (502) staff       (20)      589 2023-06-20 13:27:14.000000 onedep_deposition-0.1.dev7/onedep_deposition/decorators.py
+-rw-r--r--   0 peisach    (502) staff       (20)    15606 2023-06-23 11:13:00.000000 onedep_deposition-0.1.dev7/onedep_deposition/deposit_api.py
+-rw-r--r--   0 peisach    (502) staff       (20)     9006 2023-06-15 13:32:19.000000 onedep_deposition-0.1.dev7/onedep_deposition/enum.py
+-rw-r--r--   0 peisach    (502) staff       (20)      316 2023-06-20 13:27:14.000000 onedep_deposition-0.1.dev7/onedep_deposition/exceptions.py
+-rw-r--r--   0 peisach    (502) staff       (20)    13030 2023-06-23 11:13:00.000000 onedep_deposition-0.1.dev7/onedep_deposition/models.py
+-rw-r--r--   0 peisach    (502) staff       (20)     6182 2023-06-20 13:27:14.000000 onedep_deposition-0.1.dev7/onedep_deposition/rest_adapter.py
+drwxr-xr-x   0 peisach    (502) staff       (20)        0 2023-06-23 11:14:01.026226 onedep_deposition-0.1.dev7/onedep_deposition.egg-info/
+-rw-r--r--   0 peisach    (502) staff       (20)     5174 2023-06-23 11:14:01.000000 onedep_deposition-0.1.dev7/onedep_deposition.egg-info/PKG-INFO
+-rw-r--r--   0 peisach    (502) staff       (20)      558 2023-06-23 11:14:01.000000 onedep_deposition-0.1.dev7/onedep_deposition.egg-info/SOURCES.txt
+-rw-r--r--   0 peisach    (502) staff       (20)        1 2023-06-23 11:14:01.000000 onedep_deposition-0.1.dev7/onedep_deposition.egg-info/dependency_links.txt
+-rw-r--r--   0 peisach    (502) staff       (20)       68 2023-06-23 11:14:01.000000 onedep_deposition-0.1.dev7/onedep_deposition.egg-info/entry_points.txt
+-rw-r--r--   0 peisach    (502) staff       (20)       15 2023-06-23 11:14:01.000000 onedep_deposition-0.1.dev7/onedep_deposition.egg-info/requires.txt
+-rw-r--r--   0 peisach    (502) staff       (20)       18 2023-06-23 11:14:01.000000 onedep_deposition-0.1.dev7/onedep_deposition.egg-info/top_level.txt
+-rw-r--r--   0 peisach    (502) staff       (20)     1039 2023-06-17 17:50:36.000000 onedep_deposition-0.1.dev7/pyproject.toml
+-rw-r--r--   0 peisach    (502) staff       (20)       38 2023-06-23 11:14:01.028802 onedep_deposition-0.1.dev7/setup.cfg
```

### Comparing `onedep_deposition-0.1.dev6/LICENSE` & `onedep_deposition-0.1.dev7/LICENSE`

 * *Files identical despite different names*

### Comparing `onedep_deposition-0.1.dev6/PKG-INFO` & `onedep_deposition-0.1.dev7/onedep_deposition.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: onedep_deposition
-Version: 0.1.dev6
+Name: onedep-deposition
+Version: 0.1.dev7
 Summary: Package for wrapping the OneDep deposition API services
 Author-email: Neli Jose da Fonseca Junior <neli@ebi.ac.uk>
 License: apache-2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
```

### Comparing `onedep_deposition-0.1.dev6/README.md` & `onedep_deposition-0.1.dev7/README.md`

 * *Files identical despite different names*

### Comparing `onedep_deposition-0.1.dev6/onedep_deposition/cli/cli.py` & `onedep_deposition-0.1.dev7/onedep_deposition/cli/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 import click
 import re
 import os
 import json
 from typing import List, Union, Dict
 from onedep_deposition.deposit_api import DepositApi
 from onedep_deposition.enum import Country, FileType
-
-VERSION = "1.0.0"
+from onedep_deposition.__init__ import __version__ as VERSION
 
 
 def get_api_key():
     """Get API key from the file system or environment variable"""
     if os.path.isfile(os.path.expanduser("~/onedepapi.jwt")):
         with open(os.path.expanduser("~/onedepapi.jwt"), "r") as f:
             api_key = f.read().strip()
@@ -74,19 +73,20 @@
 @click.option("-t", "--type", "dep_type", help="Experiment type [em, xray, fiber, neutron, ec, nmr, ssnmr]")
 @click.option("-e", "--email", "email", help="Main depositor email")
 @click.option("-u", "--users", "users", multiple=True, help="List of users to add to the deposition")
 @click.option("-c", "--country", "country_string", help="Country of the main depositor")
 @click.option("-s", "--subtype", "subtype", help="Experiment subtype, only valid if type is EM")
 @click.option("-E", "--related_emdb", "related_emdb", help="Related EMDB code. Only valid for EM and EC")
 @click.option("-B", "--related_bmrb", "related_bmrb", help="Related BMRB code. Only valid for NMR")
+@click.option("--no_coordinates", "no_coordinates", is_flag=True, help="Depositing coordinates file? (y/n)")
 @click.option("-p", "--password", "password", help="Deposition password")
 @click.pass_context
 @create_api
 def create(api: DepositApi, ctx: Dict, dep_type: str, email: str, users: List[str], country_string: str, subtype: str,
-           related_emdb: str, related_bmrb: str, password: str):
+           related_emdb: str, related_bmrb: str, password: str, no_coordinates: bool = False):
     """`create` deposition command handler"""
     if subtype:
         if subtype not in ["helical", "single", "subtomogram", "tomography"]:
             raise click.BadParameter("Invalid experiment subtype, options are: helical, single, subtomogram, tomography")
     if not email:
         raise click.BadParameter("Email is required")
     if not re.match(r'^[\w\.-]+@[\w\.-]+\.\w+$', email):
@@ -99,30 +99,34 @@
                 raise click.BadParameter(f"Invalid ORCID: {orcid}")
     if related_bmrb:
         if not re.match(r'^\d+$', related_bmrb):
             raise click.BadParameter("Invalid BMRB code")
     if related_emdb:
         if not re.match(r'^EMD-\d{4,5}$', related_emdb):
             raise click.BadParameter("Invalid EMDB code")
+    if no_coordinates:
+        if dep_type in ["xray", "fiber", "neutron"]:
+            raise click.BadParameter("Coordinates are mandatory for X-ray, fiber and neutron diffraction")
     country = get_country_enum(country_string)
+    coordinates = not no_coordinates
 
     if dep_type == "em":
-        deposition = api.create_em_deposition(email, users, country, subtype, related_emdb, password)
+        deposition = api.create_em_deposition(email, users, country, subtype, coordinates, related_emdb, password)
     elif dep_type == "xray":
         deposition = api.create_xray_deposition(email, users, country, password)
     elif dep_type == "fiber":
         deposition = api.create_fiber_deposition(email, users, country, password)
     elif dep_type == "neutron":
         deposition = api.create_neutron_deposition(email, users, country, password)
     elif dep_type == "ec":
-        deposition = api.create_ec_deposition(email, users, country, related_emdb, password)
+        deposition = api.create_ec_deposition(email, users, country, coordinates, related_emdb, password)
     elif dep_type == "nmr":
-        deposition = api.create_nmr_deposition(email, users, country, related_bmrb, password)
+        deposition = api.create_nmr_deposition(email, users, country, coordinates, related_bmrb, password)
     elif dep_type == "ssnmr":
-        deposition = api.create_ssnmr_deposition(email, users, country, related_bmrb, password)
+        deposition = api.create_ssnmr_deposition(email, users, country, coordinates, related_bmrb, password)
     else:
         raise click.BadParameter("Invalid experiment type, options are: em, xray, fiber, neutron, ec, nmr, ssnmr")
     click.echo(deposition)
 
 
 @deposition_group.command(name="get", help="Get deposition info")
 @click.argument("dep_id")
```

### Comparing `onedep_deposition-0.1.dev6/onedep_deposition/decorators.py` & `onedep_deposition-0.1.dev7/onedep_deposition/decorators.py`

 * *Files identical despite different names*

### Comparing `onedep_deposition-0.1.dev6/onedep_deposition/deposit_api.py` & `onedep_deposition-0.1.dev7/onedep_deposition/deposit_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -69,109 +69,113 @@
             else:
                 raise e
         response.data["dep_id"] = response.data.pop("id")
         deposit = Deposit(**response.data)
         return deposit
 
     def create_em_deposition(self, email: str, users: List[str], country: Country, subtype: Union[EMSubType, str],  # pylint: disable=unused-argument
-                             related_emdb: str = None, password: str = "", **kwargs) -> Deposit:
+                             coordinates: bool, related_emdb: str = None, password: str = "", **kwargs) -> Deposit:
         """
         Create an EM deposition
         :param email: User e-mail
         :param users: List of ORCID ids that can access this deposition
         :param country: Country from enum list
         :param subtype: EM sub type, accepts enum or string
+        :param coordinates: Depositing coordinates file?
         :param related_emdb: Related EMDB id
         :param password: Password
         :return: Response
         """
-        experiment = Experiment(exp_type="em", subtype=subtype, related_emdb=related_emdb)
+        experiment = Experiment(exp_type="em", coordinates=coordinates, subtype=subtype, related_emdb=related_emdb)
         deposit = self.create_deposition(email=email, users=users, country=country, experiments=[experiment], password=password)
         return deposit
 
     def create_xray_deposition(self, email: str, users: List[str], country: Country, password: str = "", **kwargs) -> Deposit:  # pylint: disable=unused-argument
         """
         Create an XRAY deposition
         :param email: User e-mail
         :param users: List of ORCID ids that can access this deposition
         :param country: Country from enum list
         :param password: Password
         :return: Response
         """
-        experiment = Experiment(exp_type="xray")
+        experiment = Experiment(exp_type="xray", coordinates=True)
         deposit = self.create_deposition(email=email, users=users, country=country, experiments=[experiment], password=password)
         return deposit
 
     def create_fiber_deposition(self, email: str, users: List[str], country: Country, password: str = "", **kwargs) -> Deposit:  # pylint: disable=unused-argument
         """
         Create a Fiber diffraction deposition
         :param email: User e-mail
         :param users: List of ORCID ids that can access this deposition
         :param country: Country from enum list
         :param password: Password
         :return: Response
         """
-        experiment = Experiment(exp_type="fiber")
+        experiment = Experiment(exp_type="fiber", coordinates=True)
         deposit = self.create_deposition(email=email, users=users, country=country, experiments=[experiment], password=password)
         return deposit
 
     def create_neutron_deposition(self, email: str, users: List[str], country: Country, password: str = "", **kwargs) -> Deposit:  # pylint: disable=unused-argument
         """
         Create a Neutron diffraction deposition
         :param email: User e-mail
         :param users: List of ORCID ids that can access this deposition
         :param country: Country from enum list
         :param password: Password
         :return: Response
         """
-        experiment = Experiment(exp_type="neutron")
+        experiment = Experiment(exp_type="neutron", coordinates=True)
         deposit = self.create_deposition(email=email, users=users, country=country, experiments=[experiment], password=password)
         return deposit
 
-    def create_ec_deposition(self, email: str, users: List[str], country: Country, password: str = "", related_emdb: str = None, **kwargs) -> Deposit:  # pylint: disable=unused-argument
+    def create_ec_deposition(self, email: str, users: List[str], country: Country, coordinates: bool, password: str = "", related_emdb: str = None, **kwargs) -> Deposit:  # pylint: disable=unused-argument
         """
         Create an Electron crystallography deposition
         :param email: User e-mail
         :param users: List of ORCID ids that can access this deposition
         :param country: Country from enum list
+        :param coordinates: Depositing coordinates file?
         :param password: Password
         :param related_emdb: Related EMDB id
         :return: Response
         """
-        experiment = Experiment(exp_type="ec", related_emdb=related_emdb)
+        experiment = Experiment(exp_type="ec", related_emdb=related_emdb, coordinates=coordinates)
         deposit = self.create_deposition(email=email, users=users, country=country, experiments=[experiment], password=password)
         return deposit
 
-    def create_nmr_deposition(self, email: str, users: List[str], country: Country, password: str = "",  # pylint: disable=unused-argument
+    def create_nmr_deposition(self, email: str, users: List[str], country: Country, coordinates: bool, password: str = "",  # pylint: disable=unused-argument
                               related_bmrb: str = None, **kwargs) -> Deposit:
         """
         Create a NMR deposition
         :param email: User e-mail
         :param users: List of ORCID ids that can access this deposition
         :param country: Country from enum list
+        :param coordinates: Depositing coordinates file?
         :param password: Password
         :param related_bmrb: Related BMRB id
         :return: Response
         """
-        experiment = Experiment(exp_type="nmr", related_bmrb=related_bmrb)
+        experiment = Experiment(exp_type="nmr", related_bmrb=related_bmrb, coordinates=coordinates)
         deposit = self.create_deposition(email=email, users=users, country=country, experiments=[experiment], password=password)
         return deposit
 
-    def create_ssnmr_deposition(self, email: str, users: List[str], country: Country, password: str = "",  # pylint: disable=unused-argument
+    def create_ssnmr_deposition(self, email: str, users: List[str], country: Country, coordinates: bool, password: str = "",  # pylint: disable=unused-argument
                                 related_bmrb: str = None, **kwargs) -> Deposit:
         """
         Create a Solid-state NMR E deposition
         :param email: User e-mail
         :param users: List of ORCID ids that can access this deposition
         :param country: Country from enum list
+        :param coordinates: Depositing coordinates file?
         :param password: Password
         :param related_bmrb: Related BMRB id
         :return: Response
         """
-        experiment = Experiment(exp_type="ssnmr", related_bmrb=related_bmrb)
+        experiment = Experiment(exp_type="ssnmr", related_bmrb=related_bmrb, coordinates=coordinates)
         deposit = self.create_deposition(email=email, users=users, country=country, experiments=[experiment], password=password)
         return deposit
 
     @handle_invalid_deposit_site
     def get_deposition(self, dep_id: str) -> Union[Deposit, None]:
         """
         Get deposition from ID
```

### Comparing `onedep_deposition-0.1.dev6/onedep_deposition/enum.py` & `onedep_deposition-0.1.dev7/onedep_deposition/enum.py`

 * *Files identical despite different names*

### Comparing `onedep_deposition-0.1.dev6/onedep_deposition/models.py` & `onedep_deposition-0.1.dev7/onedep_deposition/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,23 +34,25 @@
         :return: String text
         """
         return f"STATUS: {self._status_code}, MESSAGE: {self._message}\n{self._data}"
 
 
 class Experiment:
     """Class representing an experiment"""
-    def __init__(self, exp_type: Union[ExperimentType, str], subtype: Union[EMSubType, str] = None,
+    def __init__(self, exp_type: Union[ExperimentType, str], coordinates: bool = True, subtype: Union[EMSubType, str] = None,
                  related_emdb: str = None, related_bmrb: str = None):
         """
         Constructor for Experiment
         :param exp_type:
+        :param coordinates:
         :param subtype:
         :param related_emdb:
         :param related_bmrb:
         """
+        self._coordinates = bool(coordinates)
         self._type = None
         self._subtype = None
         self._related_emdb = str(related_emdb) if related_emdb is not None else None
         self._related_bmrb = str(related_bmrb) if related_bmrb is not None else None
 
         if type(exp_type) == ExperimentType:
             self._type = exp_type
@@ -58,14 +60,18 @@
             self._type = ExperimentType(exp_type)
         if type(subtype) == EMSubType:
             self._subtype = subtype
         elif subtype:
             self._subtype = EMSubType(subtype)
 
     @property
+    def coordinates(self) -> bool:
+        return self._coordinates
+
+    @property
     def type(self) -> Union[ExperimentType, None]:
         return self._type
 
     @property
     def subtype(self) -> Union[EMSubType, None]:
         return self._subtype
```

### Comparing `onedep_deposition-0.1.dev6/onedep_deposition/rest_adapter.py` & `onedep_deposition-0.1.dev7/onedep_deposition/rest_adapter.py`

 * *Files identical despite different names*

### Comparing `onedep_deposition-0.1.dev6/onedep_deposition.egg-info/PKG-INFO` & `onedep_deposition-0.1.dev7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: onedep-deposition
-Version: 0.1.dev6
+Name: onedep_deposition
+Version: 0.1.dev7
 Summary: Package for wrapping the OneDep deposition API services
 Author-email: Neli Jose da Fonseca Junior <neli@ebi.ac.uk>
 License: apache-2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
```

### Comparing `onedep_deposition-0.1.dev6/onedep_deposition.egg-info/SOURCES.txt` & `onedep_deposition-0.1.dev7/onedep_deposition.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `onedep_deposition-0.1.dev6/pyproject.toml` & `onedep_deposition-0.1.dev7/pyproject.toml`

 * *Files identical despite different names*

