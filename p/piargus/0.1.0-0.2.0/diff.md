# Comparing `tmp/piargus-0.1.0-py3-none-any.whl.zip` & `tmp/piargus-0.2.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,24 +1,26 @@
-Zip file size: 27660 bytes, number of entries: 22
--rw-rw-rw-  2.0 fat      739 b- defN 23-Mar-09 12:18 piargus/__init__.py
+Zip file size: 30410 bytes, number of entries: 24
+-rw-rw-rw-  2.0 fat      823 b- defN 23-Jun-19 09:47 piargus/__init__.py
 -rw-rw-rw-  2.0 fat     4108 b- defN 23-Feb-01 17:28 piargus/apriori.py
 -rw-rw-rw-  2.0 fat     2933 b- defN 23-Feb-01 17:28 piargus/argusreport.py
--rw-rw-rw-  2.0 fat     3524 b- defN 23-Mar-09 11:03 piargus/batchwriter.py
+-rw-rw-rw-  2.0 fat     3784 b- defN 23-Jun-20 23:19 piargus/batchwriter.py
 -rw-rw-rw-  2.0 fat     1673 b- defN 23-Feb-01 17:28 piargus/codelist.py
 -rw-rw-rw-  2.0 fat      379 b- defN 23-Jan-20 19:08 piargus/constants.py
--rw-rw-rw-  2.0 fat     4353 b- defN 23-Feb-01 17:28 piargus/hierarchy.py
--rw-rw-rw-  2.0 fat     4564 b- defN 23-Feb-10 16:24 piargus/inputdata.py
--rw-rw-rw-  2.0 fat     8996 b- defN 23-Mar-09 10:54 piargus/job.py
+-rw-rw-rw-  2.0 fat     1251 b- defN 23-Jun-19 21:19 piargus/graphrecode.py
+-rw-rw-rw-  2.0 fat     4353 b- defN 23-Jun-21 10:15 piargus/hierarchy.py
+-rw-rw-rw-  2.0 fat     4550 b- defN 23-Jun-18 22:08 piargus/inputdata.py
+-rw-rw-rw-  2.0 fat    10671 b- defN 23-Jun-19 21:26 piargus/job.py
 -rw-rw-rw-  2.0 fat     5310 b- defN 23-Feb-20 21:51 piargus/metadata.py
 -rw-rw-rw-  2.0 fat     3000 b- defN 23-Feb-10 16:24 piargus/microdata.py
--rw-rw-rw-  2.0 fat     4410 b- defN 23-Feb-20 21:12 piargus/safetyrule.py
--rw-rw-rw-  2.0 fat     5358 b- defN 23-Feb-20 21:12 piargus/table.py
--rw-rw-rw-  2.0 fat     5606 b- defN 23-Feb-22 13:23 piargus/tabledata.py
+-rw-rw-rw-  2.0 fat     5046 b- defN 23-Jun-21 13:50 piargus/safetyrule.py
+-rw-rw-rw-  2.0 fat     5107 b- defN 23-Jun-21 13:46 piargus/table.py
+-rw-rw-rw-  2.0 fat     5606 b- defN 23-Jun-18 22:08 piargus/tabledata.py
 -rw-rw-rw-  2.0 fat     2180 b- defN 23-Feb-01 17:28 piargus/tableresult.py
--rw-rw-rw-  2.0 fat     4237 b- defN 23-Feb-20 21:51 piargus/tauargus.py
--rw-rw-rw-  2.0 fat      328 b- defN 23-Feb-20 21:12 piargus/utils.py
--rw-rw-rw-  2.0 fat    11357 b- defN 23-Mar-09 12:20 piargus-0.1.0.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     3065 b- defN 23-Mar-09 12:20 piargus-0.1.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Mar-09 12:20 piargus-0.1.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        8 b- defN 23-Mar-09 12:20 piargus-0.1.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     1679 b- defN 23-Mar-09 12:20 piargus-0.1.0.dist-info/RECORD
-22 files, 77899 bytes uncompressed, 24994 bytes compressed:  67.9%
+-rw-rw-rw-  2.0 fat     2581 b- defN 23-Jun-18 23:39 piargus/tableset.py
+-rw-rw-rw-  2.0 fat     4311 b- defN 23-Jun-19 18:21 piargus/tauargus.py
+-rw-rw-rw-  2.0 fat     1368 b- defN 23-Jun-19 20:30 piargus/utils.py
+-rw-rw-rw-  2.0 fat    11357 b- defN 23-Jun-23 10:33 piargus-0.2.0.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     3070 b- defN 23-Jun-23 10:33 piargus-0.2.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-23 10:33 piargus-0.2.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        8 b- defN 23-Jun-23 10:33 piargus-0.2.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1836 b- defN 23-Jun-23 10:33 piargus-0.2.0.dist-info/RECORD
+24 files, 85397 bytes uncompressed, 27510 bytes compressed:  67.8%
```

## zipnote {}

```diff
@@ -12,14 +12,17 @@
 
 Filename: piargus/codelist.py
 Comment: 
 
 Filename: piargus/constants.py
 Comment: 
 
+Filename: piargus/graphrecode.py
+Comment: 
+
 Filename: piargus/hierarchy.py
 Comment: 
 
 Filename: piargus/inputdata.py
 Comment: 
 
 Filename: piargus/job.py
@@ -39,29 +42,32 @@
 
 Filename: piargus/tabledata.py
 Comment: 
 
 Filename: piargus/tableresult.py
 Comment: 
 
+Filename: piargus/tableset.py
+Comment: 
+
 Filename: piargus/tauargus.py
 Comment: 
 
 Filename: piargus/utils.py
 Comment: 
 
-Filename: piargus-0.1.0.dist-info/LICENSE
+Filename: piargus-0.2.0.dist-info/LICENSE
 Comment: 
 
-Filename: piargus-0.1.0.dist-info/METADATA
+Filename: piargus-0.2.0.dist-info/METADATA
 Comment: 
 
-Filename: piargus-0.1.0.dist-info/WHEEL
+Filename: piargus-0.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: piargus-0.1.0.dist-info/top_level.txt
+Filename: piargus-0.2.0.dist-info/top_level.txt
 Comment: 
 
-Filename: piargus-0.1.0.dist-info/RECORD
+Filename: piargus-0.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## piargus/__init__.py

```diff
@@ -1,19 +1,21 @@
 from piargus.apriori import Apriori
 from piargus.argusreport import TauArgusException
 from piargus.batchwriter import BatchWriter
 from piargus.codelist import CodeList
 from piargus.constants import *
+from piargus.graphrecode import GraphRecode
 from piargus.hierarchy import Hierarchy
 from piargus.inputdata import InputData
 from piargus.job import Job
 from piargus.job import JobSetupError
 from piargus.metadata import MetaData
 from piargus.microdata import MicroData
 from piargus.safetyrule import dominance_rule, percent_rule, frequency_rule, request_rule, zero_rule, \
     missing_rule, weight_rule, manual_rule, p_rule, nk_rule
 from piargus.table import Table
 from piargus.tabledata import TableData
+from piargus.tableset import TableSet
 from piargus.tauargus import TauArgus
 
 
-__version__ = "0.1.0"
+__version__ = "0.2.0"
```

## piargus/batchwriter.py

```diff
@@ -1,8 +1,9 @@
 from .constants import FREQUENCY_RESPONSE
+from .safetyrule import make_safety_rule
 from .utils import format_argument
 
 
 class BatchWriter:
     """
     Helper to write a batch file for use with TauArgus.
 
@@ -19,30 +20,25 @@
         else:
             self._file.write(f"<{command}>\t{arg}\n")
         return command, arg
 
     def logbook(self, log_file):
         self.write_command('LOGBOOK', format_argument(log_file))
 
-    def open_microdata(self, microdata, sep=','):
-        if hasattr(microdata, 'to_csv'):
-            microdata_file = f'microdata_{id(self)}.csv'
-            microdata.to_csv(microdata_file, sep=sep)
-        else:
-            microdata_file = microdata
-
-        return self.write_command("OPENMICRODATA", format_argument(microdata_file))
+    def open_microdata(self, microdata):
+        return self.write_command("OPENMICRODATA", format_argument(microdata))
 
     def open_tabledata(self, tabledata):
         return self.write_command("OPENTABLEDATA", format_argument(tabledata))
 
     def open_metadata(self, metadata):
         return self.write_command("OPENMETADATA", format_argument(metadata))
 
-    def specify_table(self, explanatory, response=FREQUENCY_RESPONSE, shadow=None, cost=None, labda=None):
+    def specify_table(self, explanatory, response=FREQUENCY_RESPONSE, shadow=None, cost=None,
+                      labda=None):
         explanatory_str = "".join([format_argument(v) for v in explanatory])
         response_str = format_argument(response)
         shadow_str = format_argument(shadow)
         cost_str = format_argument(cost)
         options = f'{explanatory_str}|{response_str}|{shadow_str}|{cost_str}'
         if labda:
             options += f"|{labda}"
@@ -54,25 +50,32 @@
     def read_table(self, compute_totals=None):
         if compute_totals is None:
             return self.write_command("READTABLE")
         else:
             return self.write_command("READTABLE", int(compute_totals))
 
     def apriori(self, filename, table, separator=',', ignore_error=False, expand_trivial=True):
-        ignore_error = int(ignore_error)
-        expand_trivial = int(expand_trivial)
         filename = format_argument(filename)
+        table = format_argument(table)
         separator = format_argument(separator)
+        ignore_error = format_argument(ignore_error)
+        expand_trivial = format_argument(expand_trivial)
         arg = f"{filename}, {table}, {separator}, {ignore_error}, {expand_trivial}"
         return self.write_command("APRIORI", arg)
 
-    def safety_rule(self, rules):
-        if isinstance(rules, str):
-            rules = (rules,)
-        return self.write_command('SAFETYRULE', "|".join(rules))
+    def recode(self, table, variable, file_or_treelevel):
+        table = format_argument(table)
+        variable = format_argument(variable)
+        file_or_treelevel = format_argument(file_or_treelevel)
+        arg = f"{table}, {variable}, {file_or_treelevel}"
+        return self.write_command("RECODE", arg)
+
+    def safety_rule(self, rule="", /, *, individual="", holding=""):
+        rule = make_safety_rule(rule, individual=individual, holding=holding)
+        return self.write_command('SAFETYRULE', rule)
 
     def suppress(self, method, table, *method_args):
         args = ",".join(map(str, [table, *method_args]))
         return self.write_command('SUPPRESS', f"{method}({args})")
 
     def write_table(self, table, kind, options, filename):
         if hasattr(options, 'items'):
```

## piargus/inputdata.py

```diff
@@ -1,8 +1,9 @@
 import abc
+import warnings
 from typing import Dict
 
 from pandas.core.dtypes.common import is_string_dtype, is_categorical_dtype, is_bool_dtype
 
 from .codelist import CodeList
 from .hierarchy import Hierarchy
 from .metadata import MetaData, Column
@@ -20,24 +21,24 @@
         column_lengths: Dict[str, int] = None,
         total_codes: Dict[str, str] = None,
     ):
         """
         Abstract class for input data. Either initialize MicroData or TableData.
 
         :param dataset: The dataset to make tables for.
-        :param name: The name to use when write the data to a file.
+        :param name: (unused)
         :param hierarchies: The hierarchies to use for categorial data in the dataset.
         :param codelists: Codelists (dicts) for categorical data in the dataset.
         :param column_lengths: For each column the length.
         :param total_codes: Codes within explanatory that are used for the totals.
         The lengths can also be derived by calling resolve_column_lengths.
         """
 
-        if name is None:
-            name = f'data_{id(self)}'
+        if name is not None:
+            warnings.warn("Name on input_data is no longer used.")
 
         if hierarchies is None:
             hierarchies = dict()
 
         if codelists is None:
             codelists = dict()
 
@@ -47,15 +48,14 @@
         if total_codes is None:
             total_codes = dict()
         elif isinstance(total_codes, str):
             # This is allowed on TableData, but not in general
             raise TypeError("Total codes must be a dict.")
 
         self.dataset = dataset
-        self.name = name
         self.hierarchies = hierarchies
         self.codelists = codelists
         self.column_lengths = column_lengths
         self.total_codes = total_codes
 
         self.filepath = None
```

## piargus/job.py

```diff
@@ -1,22 +1,26 @@
 from pathlib import Path
 from tempfile import TemporaryDirectory
-from typing import Optional, Union, Iterable
+from typing import Optional, Union, Mapping, Hashable, Iterable
 
 from .batchwriter import BatchWriter
+from .graphrecode import GraphRecode
 from .inputdata import InputData
 from .metadata import MetaData
 from .table import Table
+from .tabledata import TableData
+from .tableset import TableSet
+from .utils import slugify
 
 
 class Job:
     def __init__(
         self,
         input_data: InputData,
-        tables: Optional[Iterable[Table]] = None,
+        tables: Optional[Union[Mapping[Hashable, Table], Iterable[Table]]] = None,
         metadata: Optional[MetaData] = None,
         directory: Optional[Union[str, Path]] = None,
         name: Optional[str] = None,
         logbook: Union[bool, str] = True,
         interactive: bool = False,
         setup: bool = True,
     ):
@@ -39,48 +43,77 @@
         :param directory: Where to write tau-argus files.
         :param name: Name from which to derive the name of some temporary files.
         :param logbook: Whether this job should create its own logging file.
         :param interactive: Whether the gui should be opened.
         :param setup: Whether to set up the job inmediately. (required before run).
         """
 
-        if directory is None:
-            # Prevent the directory from being garbage-collected as long as this job exists
-            self._tmp_directory = TemporaryDirectory(prefix='pyargus_')
-            directory = Path(self._tmp_directory.name)
-
-        if name is None:
-            name = f'job_{id(self)}'
+        if tables is None and isinstance(input_data, TableData):
+            tables = [input_data]
 
-        if not isinstance(input_data, InputData):
-            raise TypeError("Input needs to be MicroData or TableData")
-
-        if tables is None:
-            if isinstance(input_data, Table):
-                tables = [input_data]
-            else:
-                raise ValueError("No outputs specified")
-
-        self.directory = Path(directory)
-        self.directory.mkdir(parents=True, exist_ok=True)
+        self._tmp_directory = None  # Will be used if directory is temporary
+        self.directory = directory
         self.input_data = input_data
         self.tables = tables
         self.metadata = metadata
-        self.directory = Path(directory).absolute()
         self.name = name
         self.logbook = logbook
         self.interactive = interactive
 
         if setup:
             self.setup()
 
     def __str__(self):
         return self.name
 
     @property
+    def name(self):
+        return self._name
+
+    @name.setter
+    def name(self, value):
+        if value is None:
+            value = f'job_{id(self)}'
+        self._name = slugify(value)
+
+    @property
+    def directory(self):
+        return self._directory
+
+    @directory.setter
+    def directory(self, value):
+        if value is None:
+            # Prevent the directory from being garbage-collected as long as this job exists
+            self._tmp_directory = TemporaryDirectory(prefix='piargus_')
+            value = Path(self._tmp_directory.name)
+
+        self._directory = Path(value).absolute()
+
+    @property
+    def input_data(self) -> InputData:
+        return self._input_data
+
+    @input_data.setter
+    def input_data(self, value):
+        if not isinstance(value, InputData):
+            raise TypeError("Input needs to be MicroData or TableData")
+        self._input_data = value
+
+    @property
+    def tables(self) -> TableSet:
+        return self._tables
+
+    @tables.setter
+    def tables(self, value):
+        if not isinstance(value, TableSet):
+            value = TableSet(value)
+
+        self._tables = TableSet(value)
+
+    @property
     def batch_filepath(self):
         return self.directory / f'{self.name}.arb'
 
     @property
     def logbook_filepath(self):
         if self.logbook is True:
             logbook = self.directory / f'{self.name}_logbook.txt'
@@ -96,102 +129,116 @@
     def setup(self, check=True):
         """Generate all files required for TauArgus to run."""
         self._setup_directories()
         self._setup_input_data()
         self._setup_hierarchies()
         self._setup_codelists()
         self._setup_metadata()
-        self._setup_apriories()
         self._setup_tables()
         self._setup_batch()
 
         if check:
             self.check()
 
     def _setup_directories(self):
+        self.directory.mkdir(parents=True, exist_ok=True)
         input_directory = self.directory / 'input'
         output_directory = self.directory / 'output'
         input_directory.mkdir(exist_ok=True)
         output_directory.mkdir(exist_ok=True)
         self.workdir.mkdir(parents=True, exist_ok=True)
 
     def _setup_input_data(self):
-        default = self.directory / 'input' / f"{self.input_data.name}.csv"
+        name = f"{self.name}_{type(self.input_data).__name__.casefold()}"
+        default = self.directory / 'input' / f"{name}.csv"
         if not self.input_data.filepath:
             self.input_data.to_csv(default)
 
     def _setup_metadata(self):
         if not self.metadata:
             self.metadata = self.input_data.generate_metadata()
 
-        default = self.directory / 'input' / f"{self.input_data.name}.rda"
+        name = f"{self.name}_{type(self.input_data).__name__.casefold()}"
+        default = self.directory / 'input' / f"{name}.rda"
         if not self.metadata.filepath:
             self.metadata.to_rda(default)
 
     def _setup_hierarchies(self):
         self.input_data.resolve_column_lengths()
         for col, hierarchy in self.input_data.hierarchies.items():
             if not hierarchy.filepath:
-                default = self.directory / 'input' / f'hierarchy_{col}.hrc'
+                default = self.directory / 'input' / f'{col}_hierarchy.hrc'
                 hierarchy.to_hrc(default, length=self.input_data.column_lengths[col])
 
     def _setup_codelists(self):
         self.input_data.resolve_column_lengths()
         for col, codelist in self.input_data.codelists.items():
             if not codelist.filepath:
-                default = self.directory / 'input' / f'codelist_{col}.cdl'
+                default = self.directory / 'input' / f'{col}_codelist.cdl'
                 codelist.to_cdl(default, length=self.input_data.column_lengths[col])
 
-    def _setup_apriories(self):
-        for table in self.tables:
+    def _setup_tables(self):
+        for t_name, table in self.tables.items():
+            if table.filepath_out is None:
+                tablename = f'{self.name}_{slugify(t_name)}'
+                table.filepath_out = self.directory / 'output' / f"{tablename}.csv"
+
             if table.apriori and table.apriori.filepath is None:
-                default = self.directory / 'input' / f'apriori_{table.name}.hst'
+                tablename = f'{self.name}_{slugify(t_name)}'
+                default = self.directory / 'input' / f'{tablename}_apriori.hst'
                 table.apriori.to_hst(default)
 
-    def _setup_tables(self):
-        for table in self.tables:
-            if table.filepath_out is None:
-                table.filepath_out = Path(self.directory / 'output' / f'{table.name}.csv')
+            for col, recode in table.recodes.items():
+                if isinstance(recode, GraphRecode) and recode.filepath is None:
+                    tablename = f'{self.name}_{slugify(t_name)}'
+                    default = self.directory / 'input' / f"{tablename}_{col}_recode.grc"
+                    recode.to_grc(default, length=self.input_data.column_lengths[col])
 
     def _setup_batch(self):
         with open(self.batch_filepath, 'w') as batch:
             writer = BatchWriter(batch)
 
             if isinstance(self.input_data, Table):
-                writer.open_tabledata(str(self.input_data.filepath))
+                writer.open_tabledata(self.input_data)
             else:
-                writer.open_microdata(str(self.input_data.filepath))
+                writer.open_microdata(self.input_data)
 
-            writer.open_metadata(str(self.metadata.filepath))
+            writer.open_metadata(self.metadata)
 
             for table in self.tables:
                 writer.specify_table(table.explanatory, table.response, table.shadow, table.cost,
                                      table.labda)
-
-                safety_rules = table.safety_rule,
-                writer.safety_rule(safety_rules)
+                writer.safety_rule(table.safety_rule)
 
             if isinstance(self.input_data, Table):
                 writer.read_table()
             else:
                 writer.read_microdata()
 
             for t_index, table in enumerate(self.tables, 1):
                 if table.apriori:
                     writer.apriori(
-                        table.apriori.filepath,
+                        table.apriori,
                         t_index,
                         separator=table.apriori.separator,
                         ignore_error=table.apriori.ignore_error,
                         expand_trivial=table.apriori.expand_trivial,
                     )
 
+                for variable, recode in table.recodes.items():
+                    writer.recode(t_index, variable, recode)
+
                 if table.suppress_method:
                     writer.suppress(table.suppress_method, t_index, *table.suppress_method_args)
 
+            # Linked suppression
+            if self.tables.suppress_method:
+                writer.suppress(self.tables.suppress_method, 0, *self.tables.suppress_method_args)
+
+            for t_index, table in enumerate(self.tables, 1):
                 writer.write_table(t_index, 2, {"AS": True}, str(table.filepath_out))
 
             if self.interactive:
                 writer.go_interactive()
 
     def check(self):
         problems = []
```

## piargus/safetyrule.py

```diff
@@ -1,8 +1,8 @@
-from typing import Union, Collection, Sequence
+from typing import Union, Collection, Sequence, Mapping, TypedDict
 
 
 def safety_rule(code, maximum=None, dummy=None):
     """
     Decorator to add metadata to safety rule.
 
     A safety rule is a function returning a string.
@@ -98,21 +98,40 @@
 ]
 
 # Aliases for consistency with τ-argus-api
 nk_rule = dominance_rule
 p_rule = percent_rule
 
 
-def make_safety_rule(individual: Union[str, Collection[str]],
-                     holding: Union[str, Collection[str]]) -> str:
+class SafetyRuleDict(TypedDict, total=False):
+    individual: Union[str, Collection[str]]
+    holding: Union[str, Collection[str]]
+
+
+def make_safety_rule(
+    rule: Union[str, Collection[str], SafetyRuleDict] = "", /, *,
+    individual: Union[str, Collection[str]] = "",
+    holding: Union[str, Collection[str]] = "",
+) -> str:
     """
     Construct a safety rule from individual and holding parts.
 
     Dummy elements are inserted when necessary.
     """
+    if rule:
+        if individual or holding:
+            raise TypeError("Function should either be called with 1 positional "
+                            "or 2 keyword arguments.")
+        elif isinstance(rule, str):
+            return rule
+        elif isinstance(rule, Mapping):
+            return make_safety_rule(**rule)
+        else:
+            return "|".join(_split_rule(rule))
+
     if isinstance(individual, str):
         individual = _split_rule(individual)
     if isinstance(holding, str):
         holding = _split_rule(holding)
 
     dummy = []
     for rule in RULES:
@@ -134,10 +153,10 @@
     """
     Split a safety rule into parts.
 
     >>> _split_rule(["P(1)|NK(3, 7)", "FREQ(1)|NK(3, 7)", "ZERO(5)", [" P(1,2)", "MIS(1) "]])
     ['P(1)', 'NK(3, 7)', 'FREQ(1)', 'NK(3, 7)', 'ZERO(5)', 'P(1,2)', 'MIS(1)']
     """
     if isinstance(rule, str):
-        return [part.strip() for part in rule.split("|")]
+        return [part.strip() for part in rule.split("|") if part]
     else:
         return [part for subrule in rule for part in _split_rule(subrule)]
```

## piargus/table.py

```diff
@@ -1,31 +1,31 @@
 import warnings
 from typing import Union, Optional, Sequence, Collection, Iterable, Any, Mapping
 
 import pandas as pd
 
 from .apriori import Apriori
 from .constants import FREQUENCY_RESPONSE, OPTIMAL
-from .safetyrule import make_safety_rule
+from .graphrecode import GraphRecode
+from .safetyrule import make_safety_rule, SafetyRuleDict
 from .tableresult import TableResult
 
 
 class Table:
     def __init__(
         self,
         explanatory: Sequence[str],
         response: Union[str, int] = FREQUENCY_RESPONSE,
         shadow: Optional[str] = None,
         cost: Optional[Union[int, str]] = None,
         labda: int = None,
-        name: str = None,
-        safety_rule: Union[str, Collection[str], Mapping[str, Collection[str]]] = (),
-        safety_rules=None,  # Deprecated
-        safety_rules_holding=None,  # Deprecated
+        name: str = None,  # Deprecated
+        safety_rule: Union[str, Collection[str], SafetyRuleDict] = (),
         apriori: Union[Apriori, Iterable[Sequence[Any]]] = (),
+        recodes: Mapping[str, Union[int, GraphRecode]] = None,
         suppress_method: Optional[str] = OPTIMAL,
         suppress_method_args: Sequence = (),
     ):
         """
         A Table instance describes the output of the table.
 
         A simple table can be created from MicroData.
@@ -51,84 +51,82 @@
         Each part can be:
         - "P(p, n=1)": p% rule
         - "NK(n, k)": (n, k)-dominance rule
         - "ZERO(safety_range)": Zero rule
         - "FREQ(minfreq, safety_range)": Frequency rule
         - "REQ(percentage_1, percentage_2, safety_margin)": Request rule
         See the Tau-Argus manual for details on those rules.
-        :param name: Name to use for generated files
+        :param name: (unused)
         :param apriori: Apriori file to change parameters
         :param suppress_method: Method to use for secondary suppression.
         Options are:
         - `GHMITER` ("GH"): Hypercube
         - `MODULAR` ("MOD"): Modular
         - `OPTIMAL` ("OPT"): Optimal [default]
         - `NETWORK` ("NET"): Network
         - `ROUNDING` ("RND"): Controlled rounding
         - `TABULAR_ADJUSTMENT` ("CTA"): Controlled Tabular Adjustment
         - None: No secondary suppression is applied
         See the Tau-Argus manual for details on those rules.
         :param suppress_method_args: Parameters to pass to suppress_method.
         """
 
-        if name is None:
-            name = f'table_{id(self)}'
+        if name is not None:
+            warnings.warn("name is deprecated, pass a dict to Job instead")
 
-        if not isinstance(apriori, Apriori):
-            apriori = Apriori(apriori)
-
-        if safety_rules is not None:
-            warnings.warn("safety_rules is deprecated, use safety_rule instead")
-            safety_rule = safety_rules
-
-        if safety_rules_holding is not None:
-            warnings.warn("safety_rules_holding is deprecated"
-                          'use safety_rule={'
-                          '"individual": individual_rules, '
-                          '"holding": holding_rules} instead')
-            safety_rule = make_safety_rule(safety_rule, safety_rules_holding)
+        if recodes:
+            recodes = {col: (recode if isinstance(recode, (int, GraphRecode))
+                             else GraphRecode(recode))
+                       for col, recode in recodes.items()}
+        else:
+            recodes = dict()
 
         self.explanatory = explanatory
         self.response = response
         self.shadow = shadow
         self.cost = cost
         self.labda = labda
-        self.name = name
         self.filepath_out = None
         self.safety_rule = safety_rule
         self.apriori = apriori
+        self.recodes = recodes
         self.suppress_method = suppress_method
         self.suppress_method_args = suppress_method_args
 
     @property
     def safety_rule(self) -> str:
         return self._safety_rule
 
     @safety_rule.setter
-    def safety_rule(self,
-                    value: Union[str, Collection[str], Mapping[str, Union[str, Collection[str]]]]):
-        if isinstance(value, str):
-            self._safety_rule = value
-        elif isinstance(value, dict):
-            self._safety_rule = make_safety_rule(**value)
-        else:
-            self._safety_rule = "|".join(value)
+    def safety_rule(self, rule: Union[str, Collection[str], SafetyRuleDict] = ""):
+        self._safety_rule = make_safety_rule(rule)
+
+    @property
+    def apriori(self):
+        return self._apriori
+
+    @apriori.setter
+    def apriori(self, value):
+        if not isinstance(value, Apriori):
+            value = Apriori(value)
+        self._apriori = value
 
     def load_result(self) -> TableResult:
         if self.response == FREQUENCY_RESPONSE:
             response = 'Freq'
         else:
             response = self.response
 
         df = pd.read_csv(self.filepath_out, index_col=self.explanatory)
         return TableResult(df, response)
 
     def find_variables(self, categorical=True, numeric=True):
         if categorical:
             yield from self.explanatory
+            yield from self.recodes.keys()
 
         if numeric:
             if self.response != FREQUENCY_RESPONSE:
                 yield self.response
             if self.shadow:
                 yield self.shadow
             if self.cost and isinstance(self.cost, str):
```

## piargus/tauargus.py

```diff
@@ -14,20 +14,22 @@
     def __init__(self, program: Union[str, Path] = 'TauArgus'):
         self.program = str(program)
 
     def run(self, batch_or_job=None, check: bool = True, *args, **kwargs) -> ArgusReport:
         """Run either a batch file or a job."""
         if batch_or_job is None:
             result = self._run_interactively()
+        elif isinstance(batch_or_job, str):
+            result = self._run_batch(batch_or_job, *args, **kwargs)
         elif hasattr(batch_or_job, 'batch_filepath'):
             result = self._run_job(batch_or_job, *args, **kwargs)
         elif hasattr(batch_or_job, '__iter__'):
             result = self._run_parallel(batch_or_job, *args, **kwargs)
         else:
-            result = self._run_batch(batch_or_job, *args, **kwargs)
+            raise TypeError
 
         if check:
             if hasattr(result, '__iter__'):
                 for res in result:
                     res.check()
             else:
                 result.check()
```

## piargus/utils.py

```diff
@@ -1,14 +1,39 @@
+import re
 from pathlib import Path
 
+import unicodedata
 
-def format_argument(text):
-    if text is None:
+
+def format_argument(argument) -> str:
+    if argument is None:
         return ""
-    elif isinstance(text, Path):
-        return f'"{text!s}"'
-    elif isinstance(text, str):
-        return f'"{text!s}"'
-    elif isinstance(text, bool):
-        return str(int(text))
+    elif isinstance(argument, bool):
+        return str(int(argument))
+    elif isinstance(argument, Path):
+        return f'"{argument!s}"'
+    elif isinstance(argument, str):
+        return f'"{argument!s}"'
+    elif hasattr(argument, "filepath"):
+        if argument.filepath is not None:
+            return f'"{argument.filepath!s}"'
+        else:
+            raise ValueError(f"Make sure to save {argument!r} first.")
+    else:
+        return str(argument)
+
+
+def slugify(value, allow_unicode=False) -> str:
+    """
+    Taken from https://github.com/django/django/blob/master/django/utils/text.py
+    Convert to ASCII if 'allow_unicode' is False. Convert spaces or repeated
+    dashes to single dashes. Remove characters that aren't alphanumerics,
+    underscores, or hyphens. Convert to lowercase. Also strip leading and
+    trailing whitespace, dashes, and underscores.
+    """
+    value = str(value)
+    if allow_unicode:
+        value = unicodedata.normalize('NFKC', value)
     else:
-        return str(text)
+        value = unicodedata.normalize('NFKD', value).encode('ascii', 'ignore').decode('ascii')
+    value = re.sub(r'[^\w\s-]', '', value.lower())
+    return re.sub(r'[-\s]+', '-', value).strip('-_')
```

## Comparing `piargus-0.1.0.dist-info/LICENSE` & `piargus-0.2.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `piargus-0.1.0.dist-info/METADATA` & `piargus-0.2.0.dist-info/METADATA`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: piargus
-Version: 0.1.0
+Version: 0.2.0
 Summary: Python wrapper around TauArgus
 Home-page: https://github.com/lverweijen/piargus
 Author: lverweijen
 Author-email: lauwerund@gmail.com
 License: Apache License 2.0
 Keywords: statistical-disclosure-control tau-argus
 Classifier: License :: OSI Approved :: Apache Software License
@@ -29,24 +29,24 @@
 
 For this package to work, it is required to install τ-ARGUS locally first.
 It's also recommended to read the [TauArgus manual](https://research.cbs.nl/casc/Software/TauManualV4.1.pdf) to understand how it should be used.
 
 ## Features
 
 - Generate output tables from microdata or tabledata. It is recommended to generate from microdata.
-- Error checking is done to prevent most errors that make argus hang forever.
 - Metadata can be generated automatically, although using an existing rda-file is also possible.
-- It's possible to create hierarchies, codelists, apriori files all from code or from existing files.
+- It's possible to create hierarchies, codelists, apriori files, recode files all from code or from existing files.
+- Basic error checking of input is done before input is supplied to argus.
 
-Feel free to [contribute](https://github.com/lverweijen/piargus) support for other useful TauArgus-features.
+Feel free to [contribute](https://github.com/lverweijen/piargus) for other TauArgus-features.
 [Feedback](https://github.com/lverweijen/piargus/issues) is welcome too.
 
 ## Installing
 
-- Download and install the latest version of [τ-ARGUS](https://research.cbs.nl/casc/tau.htm).
+- Download and install the latest version of [τ-ARGUS](https://github.com/sdcTools/tauargus/releases).
 - Then use [pip](https://pip.pypa.io/en/stable/getting-started/) to install piargus:
 
 ```sh
 $ pip install --upgrade piargus
 ```
 
 ## Example
```

## Comparing `piargus-0.1.0.dist-info/RECORD` & `piargus-0.2.0.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,24 @@
-piargus/__init__.py,sha256=692EQnaVJH_7LYZwL3UHipw0k0RpDXiAq6XaQWfK_wQ,739
+piargus/__init__.py,sha256=COJ0qitu9ldqdYePX0i5TUqFYZHtavwEX8LPw6hmCWo,823
 piargus/apriori.py,sha256=y8_AdvoOvFxrCw2IQfp2kRIXgGsgxcxJwGyF7rPlffI,4108
 piargus/argusreport.py,sha256=C9v6s0GUcB0Yr-nTKwXnAxj7nGjaNUBnQrbxmC0CJSI,2933
-piargus/batchwriter.py,sha256=QqV7-JTkVjgcns_6rH1EX-HsJG045wcupU_V-Kq3MSY,3524
+piargus/batchwriter.py,sha256=2DLNty8sujtJp_GFmwyrm5yeBrqXVGVoIKiwnTXA9Qw,3784
 piargus/codelist.py,sha256=kSqHbVVvohMThrvtro22Lblh6E4mr04HGSX1HBFmJq4,1673
 piargus/constants.py,sha256=kqLB7aSsrvbOdfVvdSBW1fJuAtrqEbUJLGFksePuaUI,379
+piargus/graphrecode.py,sha256=HyQrxGNxSYVDEEfidhHpn6F4SRwigMmuRyKDOGpkNN8,1251
 piargus/hierarchy.py,sha256=XQfVnMCa3kblSPz3ugrDwpV4F3HsJdbEfaMwauwjmTA,4353
-piargus/inputdata.py,sha256=N7tid5VEnGl61pRMWvtBIPlsir9-5v5anQTX5eRYcnI,4564
-piargus/job.py,sha256=huhas5hqoIEyNAlwkv-r3vcqFLhHt-33vuwA3kSG_1Y,8996
+piargus/inputdata.py,sha256=BV9-k6lXEcE8JfoFbpXeYXiRwSiP-LoAQQuA3psYhIQ,4550
+piargus/job.py,sha256=2DnNeoFg54g_-UcBeCkn1FjrS2yE42ahk926qOEaYLI,10671
 piargus/metadata.py,sha256=Lz8w5Ez3_cT6iLkWp1bZCfs2dRpLg3e3cePVHCju6ao,5310
 piargus/microdata.py,sha256=C1mPk0lP8DkWr11M5c0p9oGzdEY-Mb3UpeVMDirRbDA,3000
-piargus/safetyrule.py,sha256=gT4_pLQrRyN9coFY3ETxCUNyY2i9T4nCqiAuveVln1A,4410
-piargus/table.py,sha256=5feDbWJhc8mHFBCW0Bd22otVOBI14fp6-WaXuFqOwNo,5358
+piargus/safetyrule.py,sha256=iL3kpZVQ9DJz2wP2xiVa2NiG8zq1g8Ps1OLR3lGOI4s,5046
+piargus/table.py,sha256=obk7PXTmn8cfDXK15hGudOCK_5qteiWXKRtwGeCF6BA,5107
 piargus/tabledata.py,sha256=P7ljXNrYPw-H1S-njCxHonhZb20XOY-DI3C4ofCtbNE,5606
 piargus/tableresult.py,sha256=ILH5LGqXxn1pnC4IePosrbsKjUaF7CcCYrvEheMiWG8,2180
-piargus/tauargus.py,sha256=9BvT9IwdhktZs4r2EMjbf-sPWL1yNifkk8MAT0Fw7FU,4237
-piargus/utils.py,sha256=NglZ_kAhDfEY5q_VoQWW3C2r_wOa1OBkeUnDX7-yhbE,328
-piargus-0.1.0.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-piargus-0.1.0.dist-info/METADATA,sha256=VTCQNBO007KYzwsVdOjNqX9vLD3k3-gZkbcnlbLroP0,3065
-piargus-0.1.0.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-piargus-0.1.0.dist-info/top_level.txt,sha256=E-TXcwPPYg39KldgrN17YMMoQspcgu1UFq10wgjMNB8,8
-piargus-0.1.0.dist-info/RECORD,,
+piargus/tableset.py,sha256=03iE9iCbDbkSaxerWvIW_2TNUK0Ahlr-O2ZqYkAJkek,2581
+piargus/tauargus.py,sha256=QnuCROADHwfZluyMlVDpQhq8oI7Os2ybtXNVqNLRnEE,4311
+piargus/utils.py,sha256=XIlWCY1NIucuG3Rl6pe8xtpn1s-tDBUYRdS1l1ubT4c,1368
+piargus-0.2.0.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+piargus-0.2.0.dist-info/METADATA,sha256=YTwd0bjDa264SklpT_8TnklER_5a3cZx-yoB2MNP3Gk,3070
+piargus-0.2.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+piargus-0.2.0.dist-info/top_level.txt,sha256=E-TXcwPPYg39KldgrN17YMMoQspcgu1UFq10wgjMNB8,8
+piargus-0.2.0.dist-info/RECORD,,
```

