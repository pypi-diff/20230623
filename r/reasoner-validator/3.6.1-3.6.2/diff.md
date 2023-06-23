# Comparing `tmp/reasoner_validator-3.6.1.tar.gz` & `tmp/reasoner_validator-3.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reasoner_validator-3.6.1.tar", max compression
+gzip compressed data, was "reasoner_validator-3.6.2.tar", max compression
```

## Comparing `reasoner_validator-3.6.1.tar` & `reasoner_validator-3.6.2.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0     1153 2023-06-20 02:01:01.984228 reasoner_validator-3.6.1/LICENSE
--rw-r--r--   0        0        0    12621 2023-06-20 02:01:01.984228 reasoner_validator-3.6.1/README.md
--rw-r--r--   0        0        0      131 2023-06-20 02:01:01.984228 reasoner_validator-3.6.1/docs/.nojekyll
--rw-r--r--   0        0        0      634 2023-06-20 02:01:01.984228 reasoner_validator-3.6.1/docs/Makefile
--rw-r--r--   0        0        0     2291 2023-06-20 02:01:01.988228 reasoner_validator-3.6.1/docs/conf.py
--rw-r--r--   0        0        0    19641 2023-06-20 02:01:01.988228 reasoner_validator-3.6.1/docs/index.rst
--rw-r--r--   0        0        0      795 2023-06-20 02:01:01.988228 reasoner_validator-3.6.1/docs/make.bat
--rw-r--r--   0        0        0      136 2023-06-20 02:01:01.988228 reasoner_validator-3.6.1/docs/reasoner_validator.biolink.rst
--rw-r--r--   0        0        0      135 2023-06-20 02:01:01.988228 reasoner_validator-3.6.1/docs/reasoner_validator.report.rst
--rw-r--r--   0        0        0      142 2023-06-20 02:01:01.988228 reasoner_validator-3.6.1/docs/reasoner_validator.rst
--rw-r--r--   0        0        0      146 2023-06-20 02:01:01.988228 reasoner_validator-3.6.1/docs/reasoner_validator.trapi.mapping.rst
--rw-r--r--   0        0        0      144 2023-06-20 02:01:01.988228 reasoner_validator-3.6.1/docs/reasoner_validator.trapi.rst
--rw-r--r--   0        0        0      163 2023-06-20 02:01:01.988228 reasoner_validator-3.6.1/docs/reasoner_validator.validation_codes.rst
--rw-r--r--   0        0        0      157 2023-06-20 02:01:01.988228 reasoner_validator-3.6.1/docs/reasoner_validator.versioning.rst
--rw-r--r--   0        0        0    35703 2023-06-20 02:01:01.988228 reasoner_validator-3.6.1/docs/validation_codes_dictionary.md
--rw-r--r--   0        0        0     2093 2023-06-20 02:01:01.988228 reasoner_validator-3.6.1/pyproject.toml
--rw-r--r--   0        0        0    36530 2023-06-20 02:01:01.988228 reasoner_validator-3.6.1/reasoner_validator/__init__.py
--rw-r--r--   0        0        0    62655 2023-06-20 02:01:01.988228 reasoner_validator-3.6.1/reasoner_validator/biolink/__init__.py
--rw-r--r--   0        0        0    38969 2023-06-20 02:01:01.988228 reasoner_validator-3.6.1/reasoner_validator/codes.yaml
--rw-r--r--   0        0        0    28533 2023-06-20 02:01:01.988228 reasoner_validator-3.6.1/reasoner_validator/report.py
--rw-r--r--   0        0        0        0 2023-06-20 02:01:01.988228 reasoner_validator-3.6.1/reasoner_validator/sri/__init__.py
--rw-r--r--   0        0        0     4350 2023-06-20 02:01:01.988228 reasoner_validator-3.6.1/reasoner_validator/sri/util.py
--rw-r--r--   0        0        0     9721 2023-06-20 02:01:01.988228 reasoner_validator-3.6.1/reasoner_validator/trapi/__init__.py
--rw-r--r--   0        0        0     1105 2023-06-20 02:01:01.988228 reasoner_validator-3.6.1/reasoner_validator/trapi/mapping.py
--rw-r--r--   0        0        0    14009 2023-06-20 02:01:01.988228 reasoner_validator-3.6.1/reasoner_validator/validation_codes.py
--rw-r--r--   0        0        0    10707 2023-06-20 02:01:01.988228 reasoner_validator-3.6.1/reasoner_validator/versioning.py
--rw-r--r--   0        0        0      361 2023-06-20 02:01:01.988228 reasoner_validator-3.6.1/tests/__init__.py
--rw-r--r--   0        0        0       37 2023-06-20 02:01:01.988228 reasoner_validator-3.6.1/tests/conftest.py
--rw-r--r--   0        0        0   114356 2023-06-20 02:01:01.992229 reasoner_validator-3.6.1/tests/test_biolink_compliance_validation.py
--rw-r--r--   0        0        0    62095 2023-06-20 02:01:01.992229 reasoner_validator-3.6.1/tests/test_data/sample_trapi_schema_v3.2.1-beta5.yaml
--rw-r--r--   0        0        0    34156 2023-06-20 02:01:01.992229 reasoner_validator-3.6.1/tests/test_response_validator.py
--rw-r--r--   0        0        0     5508 2023-06-20 02:01:01.992229 reasoner_validator-3.6.1/tests/test_semver.py
--rw-r--r--   0        0        0     1521 2023-06-20 02:01:01.992229 reasoner_validator-3.6.1/tests/test_trapi_versioning.py
--rw-r--r--   0        0        0    26543 2023-06-20 02:01:01.992229 reasoner_validator-3.6.1/tests/test_validate.py
--rw-r--r--   0        0        0    20400 2023-06-20 02:01:01.992229 reasoner_validator-3.6.1/tests/test_validation_report.py
--rw-r--r--   0        0        0     2061 2023-06-20 02:01:01.992229 reasoner_validator-3.6.1/tests/test_workflows.py
--rw-r--r--   0        0        0    14660 1970-01-01 00:00:00.000000 reasoner_validator-3.6.1/PKG-INFO
+-rw-r--r--   0        0        0     1153 2023-06-23 06:40:38.034146 reasoner_validator-3.6.2/LICENSE
+-rw-r--r--   0        0        0    12621 2023-06-23 06:40:38.034146 reasoner_validator-3.6.2/README.md
+-rw-r--r--   0        0        0      131 2023-06-23 06:40:38.034146 reasoner_validator-3.6.2/docs/.nojekyll
+-rw-r--r--   0        0        0      634 2023-06-23 06:40:38.034146 reasoner_validator-3.6.2/docs/Makefile
+-rw-r--r--   0        0        0     2291 2023-06-23 06:40:38.034146 reasoner_validator-3.6.2/docs/conf.py
+-rw-r--r--   0        0        0    19641 2023-06-23 06:40:38.034146 reasoner_validator-3.6.2/docs/index.rst
+-rw-r--r--   0        0        0      795 2023-06-23 06:40:38.034146 reasoner_validator-3.6.2/docs/make.bat
+-rw-r--r--   0        0        0      136 2023-06-23 06:40:38.034146 reasoner_validator-3.6.2/docs/reasoner_validator.biolink.rst
+-rw-r--r--   0        0        0      135 2023-06-23 06:40:38.038147 reasoner_validator-3.6.2/docs/reasoner_validator.report.rst
+-rw-r--r--   0        0        0      142 2023-06-23 06:40:38.038147 reasoner_validator-3.6.2/docs/reasoner_validator.rst
+-rw-r--r--   0        0        0      146 2023-06-23 06:40:38.038147 reasoner_validator-3.6.2/docs/reasoner_validator.trapi.mapping.rst
+-rw-r--r--   0        0        0      144 2023-06-23 06:40:38.038147 reasoner_validator-3.6.2/docs/reasoner_validator.trapi.rst
+-rw-r--r--   0        0        0      163 2023-06-23 06:40:38.038147 reasoner_validator-3.6.2/docs/reasoner_validator.validation_codes.rst
+-rw-r--r--   0        0        0      157 2023-06-23 06:40:38.038147 reasoner_validator-3.6.2/docs/reasoner_validator.versioning.rst
+-rw-r--r--   0        0        0    35958 2023-06-23 06:40:38.038147 reasoner_validator-3.6.2/docs/validation_codes_dictionary.md
+-rw-r--r--   0        0        0     2093 2023-06-23 06:40:38.038147 reasoner_validator-3.6.2/pyproject.toml
+-rw-r--r--   0        0        0    37715 2023-06-23 06:40:38.038147 reasoner_validator-3.6.2/reasoner_validator/__init__.py
+-rw-r--r--   0        0        0    63014 2023-06-23 06:40:38.038147 reasoner_validator-3.6.2/reasoner_validator/biolink/__init__.py
+-rw-r--r--   0        0        0    39199 2023-06-23 06:40:38.038147 reasoner_validator-3.6.2/reasoner_validator/codes.yaml
+-rw-r--r--   0        0        0    28533 2023-06-23 06:40:38.038147 reasoner_validator-3.6.2/reasoner_validator/report.py
+-rw-r--r--   0        0        0        0 2023-06-23 06:40:38.038147 reasoner_validator-3.6.2/reasoner_validator/sri/__init__.py
+-rw-r--r--   0        0        0     4592 2023-06-23 06:40:38.038147 reasoner_validator-3.6.2/reasoner_validator/sri/util.py
+-rw-r--r--   0        0        0     9721 2023-06-23 06:40:38.038147 reasoner_validator-3.6.2/reasoner_validator/trapi/__init__.py
+-rw-r--r--   0        0        0     1105 2023-06-23 06:40:38.038147 reasoner_validator-3.6.2/reasoner_validator/trapi/mapping.py
+-rw-r--r--   0        0        0    14009 2023-06-23 06:40:38.038147 reasoner_validator-3.6.2/reasoner_validator/validation_codes.py
+-rw-r--r--   0        0        0    10707 2023-06-23 06:40:38.038147 reasoner_validator-3.6.2/reasoner_validator/versioning.py
+-rw-r--r--   0        0        0      361 2023-06-23 06:40:38.042147 reasoner_validator-3.6.2/tests/__init__.py
+-rw-r--r--   0        0        0       37 2023-06-23 06:40:38.042147 reasoner_validator-3.6.2/tests/conftest.py
+-rw-r--r--   0        0        0   114356 2023-06-23 06:40:38.042147 reasoner_validator-3.6.2/tests/test_biolink_compliance_validation.py
+-rw-r--r--   0        0        0    62095 2023-06-23 06:40:38.042147 reasoner_validator-3.6.2/tests/test_data/sample_trapi_schema_v3.2.1-beta5.yaml
+-rw-r--r--   0        0        0    34174 2023-06-23 06:40:38.042147 reasoner_validator-3.6.2/tests/test_response_validator.py
+-rw-r--r--   0        0        0     5508 2023-06-23 06:40:38.042147 reasoner_validator-3.6.2/tests/test_semver.py
+-rw-r--r--   0        0        0     1521 2023-06-23 06:40:38.042147 reasoner_validator-3.6.2/tests/test_trapi_versioning.py
+-rw-r--r--   0        0        0    26543 2023-06-23 06:40:38.042147 reasoner_validator-3.6.2/tests/test_validate.py
+-rw-r--r--   0        0        0    20406 2023-06-23 06:40:38.042147 reasoner_validator-3.6.2/tests/test_validation_report.py
+-rw-r--r--   0        0        0     2061 2023-06-23 06:40:38.042147 reasoner_validator-3.6.2/tests/test_workflows.py
+-rw-r--r--   0        0        0    14660 1970-01-01 00:00:00.000000 reasoner_validator-3.6.2/PKG-INFO
```

### Comparing `reasoner_validator-3.6.1/LICENSE` & `reasoner_validator-3.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.6.1/README.md` & `reasoner_validator-3.6.2/README.md`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.6.1/docs/Makefile` & `reasoner_validator-3.6.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.6.1/docs/conf.py` & `reasoner_validator-3.6.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.6.1/docs/index.rst` & `reasoner_validator-3.6.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.6.1/docs/make.bat` & `reasoner_validator-3.6.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.6.1/docs/validation_codes_dictionary.md` & `reasoner_validator-3.6.2/docs/validation_codes_dictionary.md`

 * *Files 0% similar despite different names*

```diff
@@ -70,14 +70,20 @@
 
 **Message:** Knowledge Graph of TRAPI Response Message is missing expected Edge
 
 **Context:** identifier
 
 **Description:** The given TRAPI Response is expected to return specific edge(s) relating to the original (test edge?) data used to prepare the TRAPI Request!
 
+### error.trapi.response.knowledge_graph.empty
+
+**Message:** Response returned an empty Message Knowledge Graph, which is an error in this context!
+
+**Description:** An empty Knowledge Graph is considered an error in this validation context!
+
 ### error.trapi.response.results.missing
 
 **Message:** TRAPI Message is missing its Results component!
 
 **Description:** TRAPI response should generally have a TRAPI request message Request key value in its reply.
 
 ### error.trapi.response.results.non_array
@@ -776,14 +782,26 @@
 
 **Message:** TRAPI Response has unrecognized status code
 
 **Context:** identifier
 
 **Description:** The TRAPI Response status code should be one of a standardized set of short codes, e.g. Success, QueryNotTraversable, KPsNotAvailable
 
+### warning.trapi.response.knowledge_graph.empty
+
+**Message:** Response returned an empty Message Knowledge Graph?
+
+**Description:** An empty Knowledge Graph is allowed but merits a boundary response warning?
+
+### warning.trapi.response.results.empty
+
+**Message:** Response returned empty Message.results?
+
+**Description:** Empty Results is allowed but merits a boundary response warning?
+
 ### warning.trapi.response.workflow.runner_parameters.null
 
 **Message:** TRAPI Response.workflow.runner_parameters property is missing?
 
 **Description:** If a 'runner_parameters' property value is given for a workflow step specification, it should not be null. This field will be ignored?
 
 ### warning.trapi.response.workflow.parameters.null
@@ -796,26 +814,14 @@
 
 **Message:** Empty graph
 
 **Context:** identifier
 
 **Description:** An empty graph in this particular context is allowed but merits a boundary response warning?
 
-### warning.response.knowledge_graph.empty
-
-**Message:** Response returned an empty Message Knowledge Graph?
-
-**Description:** An empty Knowledge Graph is allowed but merits a boundary response warning?
-
-### warning.response.results.empty
-
-**Message:** Response returned empty Message.results?
-
-**Description:** Empty Results is allowed but merits a boundary response warning?
-
 ### warning.input_edge.node.category.deprecated
 
 **Message:** Node category had deprecated category
 
 **Context:** node_id, identifier
 
 **Description:** Node category is deprecated in the current model, to be removed in the future. Review Biolink Model for suitable replacement?
```

### Comparing `reasoner_validator-3.6.1/pyproject.toml` & `reasoner_validator-3.6.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "reasoner-validator"
-version = "3.6.1"
+version = "3.6.2"
 description = "Validation tools for Reasoner API"
 authors = [
     "Richard Bruskiewich <richard.bruskiewich@delphinai.com>",
     "Patrick Wang <patrickelvin@gmail.com>"
 ]
 maintainers = [
     "Richard Bruskiewich <richard.bruskiewich@delphinai.com>",
```

### Comparing `reasoner_validator-3.6.1/reasoner_validator/__init__.py` & `reasoner_validator-3.6.2/reasoner_validator/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 from typing import Optional, List, Dict
 
+from bmt import Toolkit
 from reasoner_validator.report import ValidationReporter
 from reasoner_validator.biolink import (
     check_biolink_model_compliance_of_query_graph,
     check_biolink_model_compliance_of_knowledge_graph,
+    BMTWrapper,
     BiolinkValidator,
     get_biolink_model_toolkit,
-    BiolinkValidator, TRAPIGraphType
+    TRAPIGraphType
 )
 
 # Maximum number of data points to scrutinize
 # in various parts TRAPI Query Response.Message
 from reasoner_validator.trapi import check_trapi_validity, TRAPISchemaValidator
 from reasoner_validator.trapi.mapping import MappingValidator, check_node_edge_mappings
 from reasoner_validator.versioning import SemVer, SemVerError
+from reasoner_validator.sri.util import get_aliases
 
 import logging
 logger = logging.getLogger(__name__)
 
 # Unspoken assumption here is that validation of results returned for
 # Biolink Model release compliance only needs to be superficial
 RESULT_TEST_DATA_SAMPLE_SIZE = 10
@@ -310,15 +313,15 @@
                     knowledge_graph and len(knowledge_graph) > 0 and
                     "nodes" in knowledge_graph and knowledge_graph["nodes"] and
                     "edges" in knowledge_graph and knowledge_graph["edges"]
             ):
                 # An empty knowledge graph (warning) does not generally invalidate
                 # the whole Message, but no more validation tests are needed
                 if not self.suppress_empty_data_warnings:
-                    self.report(code="warning.response.knowledge_graph.empty")
+                    self.report(code="warning.trapi.response.knowledge_graph.empty")
             else:
                 mapping_validator: MappingValidator = check_node_edge_mappings(knowledge_graph)
                 if mapping_validator.has_messages():
                     self.merge(mapping_validator)
 
                 # ...then if not empty, validate a subgraph sample of the associated
                 # Knowledge Graph (since some TRAPI response kg's may be huge!)
@@ -378,15 +381,15 @@
             if not self.suppress_empty_data_warnings:
                 self.report(code="error.trapi.response.results.missing")
         else:
             results = message['results']
 
             if not (results and len(results) > 0):
                 if not self.suppress_empty_data_warnings:
-                    self.report(code="warning.response.results.empty")
+                    self.report(code="warning.trapi.response.results.empty")
                     # An empty result (warning) does not generally invalidate
                     # the whole Message, but no more validation tests are needed
 
             elif not isinstance(results, List):
                 # The Message.results should be an array of Result objects
                 # TODO: Is this test unnecessary, since TRAPI schema
                 #       validation (below) should normally catch this?
@@ -442,43 +445,43 @@
                     #         # data_dump=f"Resolved aliases:\n{','.join(output_aliases)}\n" +
                     #         #           f"Result object IDs:\n{_output(object_ids,flat=True)}"
 
         # Only 'error' but not 'info' nor 'warning' messages invalidate the overall Message
         return False if self.has_errors() else True
 
     @staticmethod
-    def case_node_found(target: str, identifier: str, case: Dict, nodes: Dict) -> bool:
+    def case_node_found(target: str, identifiers: List[str], case: Dict, nodes: Dict) -> bool:
         """
         Check for presence of the target identifier,
         with expected categories, in the "nodes" catalog.
 
         :param target: 'subject' or 'object'
-        :param identifier: (CURIE) identifier of the node
+        :param identifiers: List of node (CURIE) identifiers to be checked in the "nodes" catalog
         :param case: Dict, full test case (to access the target node 'category')
         :param nodes: Dict, nodes category indexed by node identifiers.
         :return:
         """
         #
         #     "nodes": {
         #         "MONDO:0005148": {"name": "type-2 diabetes"},
         #         "CHEBI:6801": {"name": "metformin", "categories": ["biolink:Drug"]}
         #     }
         #
 
         # Sanity check
         assert target in ["subject", "object"]
-
-        if identifier in nodes.keys():
-            # Found the target node identifier,
-            # but is the expected category present?
-            node_details = nodes[identifier]
-            if "categories" in node_details:
-                category = case[f"{target}_category"]
-                if category in node_details["categories"]:
-                    return True
+        for identifier in identifiers:
+            if identifier in nodes.keys():
+                # Found the target node identifier,
+                # but is the expected category present?
+                node_details = nodes[identifier]
+                if "categories" in node_details:
+                    category = case[f"{target}_category"]
+                    if category in node_details["categories"]:
+                        return True
 
         # Target node identifier or categories is missing,
         # or not annotated with the expected category?
         return False
 
     @staticmethod
     def case_edge_bindings(target_edge_id: str, data: Dict) -> bool:
@@ -537,15 +540,15 @@
             object_id_found: bool = False
             edge_id_found: bool = False
             for node in node_bindings.values():
                 for details in node:
                     if "id" in details:
                         if subject_id == details["id"]:
                             subject_id_found = True
-                        elif object_id == details["id"]:
+                        if object_id == details["id"]:
                             object_id_found = True
 
             # However, TRAPI 1.4.0 Message 'Results' 'edge_bindings' are reported differently
             #          from 1.3.0, rather, embedded in 'Analysis' objects (and 'Auxiliary Graphs')
             if trapi_1_4_0:
                 #
                 #     "auxiliary_graphs": {
@@ -717,21 +720,23 @@
         #         "CHEBI:6801": {"name": "metformin", "categories": ["biolink:Drug"]}
         #     }
         #
         # Check for case 'subject_id' and 'object_id',
         # with expected categories, in nodes catalog
         nodes: Dict = knowledge_graph["nodes"]
         subject_id = case["subject_id"] if "subject_id" in case else case["subject"]
-        if not self.case_node_found("subject", subject_id, case, nodes):
-            # 'subject' node not found?
+        subject_aliases = get_aliases(subject_id)
+        if not self.case_node_found("subject", subject_aliases, case, nodes):
+            # 'subject' node identifier not found?
             return False
 
         object_id = case["object_id"] if "object_id" in case else case["object"]
-        if not self.case_node_found("object", object_id, case, nodes):
-            # 'object' node not found?
+        object_aliases = get_aliases(object_id)
+        if not self.case_node_found("object", object_aliases, case, nodes):
+            # 'object' node identifier not found?
             return False
 
         # In the Knowledge Graph:
         #
         #     "edges": {
         #         "df87ff82": {
         #             "subject": "CHEBI:6801",
@@ -740,40 +745,57 @@
         #         }
         #     }
         #
         # Check in the edges catalog for an edge containing
         # the case 'subject_id', 'predicate' and 'object_id'
         edges: Dict = knowledge_graph["edges"]
 
+        bmtw = BMTWrapper(biolink_version=self.biolink_version)
+
         predicate = case["predicate"]
 
-        validator = BiolinkValidator(TRAPIGraphType.Knowledge_Graph, biolink_version=self.biolink_version)
-        inverse_predicate = validator.get_inverse_predicate(predicate)
+        bmt: Optional[Toolkit] = bmtw.get_bmt()
+        predicate_descendants: List[str]
+        inverse_predicate_descendants: List[str] = list()  # may sometimes remain empty...
+        if bmt is not None:
+            predicate_descendants = bmt.get_descendants(predicate, formatted=True)
+            inverse_predicate = bmtw.get_inverse_predicate(predicate)
+            if inverse_predicate:
+                inverse_predicate_descendants = bmt.get_descendants(inverse_predicate, formatted=True)
+        else:
+            # simpler case in which we are ignoring deep Biolink Model validation
+            predicate_descendants = [predicate]
 
-        edge_id_found: Optional[str] = None
+        edge_id_match: Optional[str] = None
+        subject_match: Optional[str] = None
+        object_match: Optional[str] = None
         for edge_id, edge in edges.items():
             # Note: this edge search could be arduous on a big knowledge graph?
-            if edge["subject"] == subject_id and \
-                    edge["predicate"] == predicate and \
-                    edge["object"] == object_id:
-                edge_id_found = edge_id
+            if edge["subject"] in subject_aliases and \
+                    edge["predicate"] in predicate_descendants and \
+                    edge["object"] in object_aliases:
+                edge_id_match = edge_id
+                subject_match = edge["subject"]
+                object_match = edge["object"]
                 break
-            elif edge["subject"] == object_id and \
-                    edge["predicate"] == inverse_predicate and \
-                    edge["object"] == subject_id:
+            elif edge["subject"] in object_aliases and \
+                    edge["predicate"] in inverse_predicate_descendants and \
+                    edge["object"] in subject_aliases:
                 # observation of the inverse edge is also counted as a match?
-                edge_id_found = edge_id
+                subject_match = edge["subject"]
+                object_match = edge["object"]
+                edge_id_match = edge_id
                 break
 
-        if edge_id_found is None:
+        if edge_id_match is None:
             # Test case S--P->O edge not found?
             return False
 
         results: List = message["results"]
-        if not self.case_result_found(subject_id, object_id, edge_id_found, results, trapi_version):
+        if not self.case_result_found(subject_match, object_match, edge_id_match, results, trapi_version):
             # Some components of test case S--P->O edge
             # NOT bound within any Results?
             return False
 
         # By this point, the case data assumed to be
         # successfully validated in the TRAPI Response?
         return True
```

### Comparing `reasoner_validator-3.6.1/reasoner_validator/biolink/__init__.py` & `reasoner_validator-3.6.2/reasoner_validator/biolink/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -79,15 +79,68 @@
 class TRAPIGraphType(Enum):
     """ Enum type of Biolink Model compliant graph data being validated."""
     Input_Edge = "Input Edge"
     Query_Graph = "Query Graph"
     Knowledge_Graph = "Knowledge Graph"
 
 
-class BiolinkValidator(ValidationReporter):
+class BMTWrapper:
+    def __init__(self, biolink_version: Optional[str] = None):
+        self.bmt: Optional[Toolkit] = None
+        if biolink_version != "suppress":
+            # Here, the Biolink Model version is validated, and the relevant Toolkit pulled.
+            self.bmt = get_biolink_model_toolkit(biolink_version=biolink_version)
+            self.resolved_biolink_version = self.bmt.get_model_version()
+        else:
+            self.resolved_biolink_version = "suppress"
+
+    def get_resolved_biolink_version(self) -> Optional[str]:
+        return self.resolved_biolink_version
+
+    def get_bmt(self) -> Optional[Toolkit]:
+        return self.bmt
+
+    def is_symmetric(self, name: str) -> bool:
+        """
+        Checks if a given element identified by name, is a symmetric (predicate) slot.
+        :param name: name of the element
+        :return: True if element is a symmetric (predicate) slot.
+        """
+        # TODO: perhaps this method ought to be in the Biolink Model Toolkit?
+        if not name:
+            return False
+        element: Optional[Element] = self.bmt.get_element(name)
+        if element['symmetric']:
+            return True
+        else:
+            return False
+
+    def get_inverse_predicate(self, predicate: Optional[str]) -> Optional[str]:
+        """
+        Utility wrapper of logic to robustly test if a predicate exists and has an inverse.
+        :param predicate: CURIE or string name of predicate for which the inverse is sought.
+        :return: CURIE string of inverse predicate, if it exists; None otherwise
+        """
+        # TODO: perhaps this method ought to be in the Biolink Model Toolkit?
+        if predicate and self.bmt.is_predicate(predicate):
+            predicate_name = utils.parse_name(predicate)
+            inverse_predicate_name = self.bmt.get_inverse(predicate_name)
+            if not inverse_predicate_name:
+                if self.is_symmetric(predicate_name):
+                    inverse_predicate_name = predicate_name
+                else:
+                    inverse_predicate_name = None
+
+            if inverse_predicate_name:
+                ip = self.bmt.get_element(inverse_predicate_name)
+                return utils.format_element(ip)
+        return None
+
+
+class BiolinkValidator(ValidationReporter, BMTWrapper):
     """
     Wrapper class for Biolink Model validation.
     """
     def __init__(
         self,
         graph_type: TRAPIGraphType,
         trapi_version: Optional[str] = None,
@@ -103,26 +156,20 @@
         :param trapi_version: caller specified Biolink Model version (default: None, which takes the TRAPI 'latest')
         :type trapi_version: Optional[str] or None
         :param biolink_version: caller specified Biolink Model version (default: None, which takes the BMT 'latest')
         :type biolink_version: Optional[str] or None
         :param sources: Dictionary of validation context identifying the ARA and KP for provenance attribute validation
         :type sources: Optional[Dict[str,str]]
         """
-        self.bmt: Optional[Toolkit] = None
-        if biolink_version != "suppress":
-            # Here, the Biolink Model version is validated, and the relevant Toolkit pulled.
-            self.bmt = get_biolink_model_toolkit(biolink_version=biolink_version)
-            resolved_biolink_version = self.bmt.get_model_version()
-        else:
-            resolved_biolink_version = "suppress"
+        BMTWrapper.__init__(self, biolink_version=biolink_version)
         ValidationReporter.__init__(
             self,
             prefix=f"Biolink Validation of {graph_type.value}",
             trapi_version=trapi_version,
-            biolink_version=resolved_biolink_version,
+            biolink_version=self.get_resolved_biolink_version(),
             sources=sources,
             strict_validation=strict_validation
         )
         self.graph_type: TRAPIGraphType = graph_type
         self.nodes: Set[str] = set()
 
     def minimum_required_biolink_version(self, version: str) -> bool:
@@ -134,50 +181,14 @@
             current: SemVer = SemVer.from_string(self.biolink_version)
             target: SemVer = SemVer.from_string(version)
             return current >= target
         except SemVerError as sve:
             logger.error(f"minimum_required_biolink_version() error: {str(sve)}")
             return False
 
-    def is_symmetric(self, name: str) -> bool:
-        """
-        Checks if a given element identified by name, is a symmetric (predicate) slot.
-        :param name: name of the element
-        :return: True if element is a symmetric (predicate) slot.
-        """
-        # TODO: perhaps this method ought to be in the Biolink Model Toolkit?
-        if not name:
-            return False
-        element: Optional[Element] = self.bmt.get_element(name)
-        if element['symmetric']:
-            return True
-        else:
-            return False
-
-    def get_inverse_predicate(self, predicate: Optional[str]) -> Optional[str]:
-        """
-        Utility wrapper of logic to robustly test if a predicate exists and has an inverse.
-        :param predicate: CURIE or string name of predicate for which the inverse is sought.
-        :return: CURIE string of inverse predicate, if it exists; None otherwise
-        """
-        # TODO: perhaps this method ought to be in the Biolink Model Toolkit?
-        if predicate and self.bmt.is_predicate(predicate):
-            predicate_name = utils.parse_name(predicate)
-            inverse_predicate_name = self.bmt.get_inverse(predicate_name)
-            if not inverse_predicate_name:
-                if self.is_symmetric(predicate_name):
-                    inverse_predicate_name = predicate_name
-                else:
-                    inverse_predicate_name = None
-
-            if inverse_predicate_name:
-                ip = self.bmt.get_element(inverse_predicate_name)
-                return utils.format_element(ip)
-        return None
-
     def get_result(self) -> Tuple[str, Optional[Dict[str, Dict[str, Optional[List[Dict[str, str]]]]]]]:
         """
         Get result of validation.
 
         :return: model version of the validation and dictionary of reported validation messages.
         :rtype Tuple[str, Optional[Dict[str, Set[str]]]]
         """
```

### Comparing `reasoner_validator-3.6.1/reasoner_validator/codes.yaml` & `reasoner_validator-3.6.2/reasoner_validator/codes.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -59,14 +59,17 @@
           $message: "TRAPI Message is missing its Knowledge Graph component!"
           $description: "TRAPI response should generally have a TRAPI request message Knowledge Graph key value in its reply."
         missing_expected_edge:
           $message: "Knowledge Graph of TRAPI Response Message is missing expected Edge"
           $context:
             - identifier
           $description: "The given TRAPI Response is expected to return specific edge(s) relating to the original (test edge?) data used to prepare the TRAPI Request!"
+        empty:
+          $message: "Response returned an empty Message Knowledge Graph, which is an error in this context!"
+          $description: "An empty Knowledge Graph is considered an error in this validation context!"
       results:
         missing:
           $message: "TRAPI Message is missing its Results component!"
           $description: "TRAPI response should generally have a TRAPI request message Request key value in its reply."
         non_array:
           $message: "Response returned a non-array Message.Results!"
           $description: "TRAPI Message.Results must be an array data type (even if empty)"
@@ -598,14 +601,22 @@
     response:
       status:
         unknown:
           $message: "TRAPI Response has unrecognized status code"
           $context:
             - identifier
           $description:  "The TRAPI Response status code should be one of a standardized set of short codes, e.g. Success, QueryNotTraversable, KPsNotAvailable"
+      knowledge_graph:
+        empty:
+          $message: "Response returned an empty Message Knowledge Graph?"
+          $description: "An empty Knowledge Graph is allowed but merits a boundary response warning?"
+      results:
+        empty:
+          $message: "Response returned empty Message.results?"
+          $description: "Empty Results is allowed but merits a boundary response warning?"
       workflow:
         runner_parameters:
           null:
             $message: "TRAPI Response.workflow.runner_parameters property is missing?"
             $description: "If a 'runner_parameters' property value is given for a workflow step specification, it should not be null. This field will be ignored?"
         parameters:
           null:
@@ -613,23 +624,14 @@
             $description: "If a 'parameters' property value is given for a workflow step specification, it should not be null. This field will be ignored?"
   graph:
     empty:
       $message: "Empty graph"
       $context:
         - identifier
       $description: "An empty graph in this particular context is allowed but merits a boundary response warning?"
-  response:
-    knowledge_graph:
-      empty:
-        $message: "Response returned an empty Message Knowledge Graph?"
-        $description: "An empty Knowledge Graph is allowed but merits a boundary response warning?"
-    results:
-      empty:
-        $message: "Response returned empty Message.results?"
-        $description: "Empty Results is allowed but merits a boundary response warning?"
   input_edge:
     node:
       category:
         deprecated:
           $message: "Node category had deprecated category"
           $context:
             - node_id
```

### Comparing `reasoner_validator-3.6.1/reasoner_validator/report.py` & `reasoner_validator-3.6.2/reasoner_validator/report.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.6.1/reasoner_validator/sri/util.py` & `reasoner_validator-3.6.2/reasoner_validator/sri/util.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,122 +9,102 @@
 
 import requests
 
 logger = logging.getLogger(__name__)
 
 # Endpoint for the Translator Normalizer service
 NODE_NORMALIZER_URL = 'https://nodenormalization-sri.renci.org/get_normalized_nodes'
+CURIE_PATTERN = re.compile(r"^[^ <()>:]*:[^/ :]+$")
 
 
-@lru_cache()
 def is_curie(s: str) -> bool:
     """
     Check if a given string is a CURIE.
 
-    Parameters
-    ----------
-    s: str
-        A string
-
-    Returns
-    -------
-    bool
-        Whether or not the given string is a CURIE
-
+    :param s: str, string to be validated as a CURIE
+    :return: bool, whether the given string is a CURIE
     """
+    # Method copied from kgx.prefix_manager.PrefixManager...
     if isinstance(s, str):
-        m = re.match(r"^[^ <()>:]*:[^/ :]+$", s)
+        m = CURIE_PATTERN.match(s)
         return bool(m)
     else:
         return False
 
 
-
-# TODO: not sure to what maxsize for LRU cache
-#       should be set so we just take the default
-@lru_cache()
-def get_aliases(identifier: str):
+# TODO: not sure to what maxsize for LRU cache but saving 1K identifiers for now
+@lru_cache(maxsize=1024)
+def get_aliases(identifier: str) -> List[str]:
     """
     Get clique of related identifiers from the Node Normalizer
     """
     if not identifier:
         raise RuntimeError("get_aliases(): empty input identifier?")
 
+    aliases: Optional[List[str]] = None
     #
     # TODO: maybe check for IRI's here and attempt to translate
     #       (Q: now do we access the prefix map from BMT to do this?)
     # if PrefixManager.is_iri(identifier):
     #     identifier = PrefixManager.contract(identifier)
 
     # We won't raise a RuntimeError for other various
     # erroneous runtime conditions but simply report warnings
     if not is_curie(identifier):
-
         logging.warning(f"get_aliases(): identifier '{identifier}' is not a CURIE thus cannot resolve its aliases?")
-        return list()
-
-    # Use the Translator Node Normalizer service to resolve the identifier clique
-    response = requests.get(NODE_NORMALIZER_URL, params={'curie': identifier})
-
-    if response.status_code != 200:
-        logging.warning(f"get_aliases(): unsuccessful Node Normalizer HTTP call, status code: {response.status_code}")
-        return list()
     else:
-        try:
-            result: Dict = response.json()
-        except (JSONDecodeError, UnicodeDecodeError) as je:
-            logging.warning(f"get_aliases(): Node Normalizer response JSON could not be decoded: {str(je)}?")
-            return list()
-
-    if result and identifier not in result.keys():
-        logging.warning(f"get_aliases(): Node Normalizer didn't return the identifier '{identifier}' clique?")
-        return list()
-
-    clique = result[identifier]
-
-    aliases: List[str] = list()
-    if clique:
-        if "id" in clique.keys():
-            # TODO: Don't need the canonical identifier for method
-            #       but when you do, this is how you'll get it?
-            # clique_id = clique["id"]
-            # preferred_curie = preferred_id["identifier"]
-            # preferred_name = preferred_id["label"]
-            if "equivalent_identifiers" in clique.keys():
-                aliases: List[str] = [entry["identifier"] for entry in clique["equivalent_identifiers"]]
-                aliases.remove(identifier)
-                # print(dumps(aliases, indent=2))
-            else:
-                logging.warning(f"get_aliases(): missing the 'equivalent identifiers' for the '{identifier}' clique?")
+        # Use the Translator Node Normalizer service to resolve the identifier clique
+        response = requests.get(NODE_NORMALIZER_URL, params={'curie': identifier})
+
+        result: Optional[Dict] = None
+        if response.status_code != 200:
+            logging.warning(
+                f"get_aliases(): unsuccessful Node Normalizer HTTP call, status code: {response.status_code}"
+            )
         else:
-            logging.warning(f"get_aliases(): missing the preferred 'id' for the '{identifier}' clique?")
-    else:
-        logging.warning(f"get_aliases(): '{identifier}' is a singleton in its clique thus has no aliases...")
+            try:
+                result = response.json()
+            except (JSONDecodeError, UnicodeDecodeError) as je:
+                logging.warning(f"get_aliases(): Node Normalizer response JSON could not be decoded: {str(je)}?")
+
+        if result:
+            if identifier not in result.keys():
+                logging.warning(f"get_aliases(): Node Normalizer didn't return the identifier '{identifier}' clique?")
+            else:
+                clique = result[identifier]
+                if clique:
+                    if "id" in clique.keys():
+                        # TODO: Don't need the canonical identifier for method
+                        #       but when you do, this is how you'll get it?
+                        # clique_id = clique["id"]
+                        # preferred_curie = preferred_id["identifier"]
+                        # preferred_name = preferred_id["label"]
+                        if "equivalent_identifiers" in clique.keys():
+                            aliases = [entry["identifier"] for entry in clique["equivalent_identifiers"]]
+                            #
+                            # Decided that it was a bad idea to remove
+                            # the original identifier from the aliases...
+                            # aliases.remove(identifier)
+                            #
+                            # print(dumps(aliases, indent=2))
+                        else:
+                            logging.warning(f"get_aliases(): missing the 'equivalent identifiers' for the '{identifier}' clique?")
+                    else:
+                        logging.warning(f"get_aliases(): missing the preferred 'id' for the '{identifier}' clique?")
+                else:
+                    logging.warning(f"get_aliases(): '{identifier}' is a singleton in its clique thus has no aliases...")
+
+    if not aliases:
+        # Logging various errors but always
+        # return the identifier as its own alias
+        aliases = [identifier]
 
     return aliases
 
 
-CURIE_PATTERN = re.compile(r"^[^ <()>:]*:[^/ :]+$")
-
-
-def is_curie(s: str) -> bool:
-    """
-    Check if a given string is a CURIE.
-
-    :param s: str, string to be validated as a CURIE
-    :return: bool, whether or not the given string is a CURIE
-    """
-    # Method copied from kgx.prefix_manager.PrefixManager...
-    if isinstance(s, str):
-        m = CURIE_PATTERN.match(s)
-        return bool(m)
-    else:
-        return False
-
-
 def get_reference(curie: str) -> Optional[str]:
     """
     Get the object_id reference of a given CURIE.
 
     Parameters
     ----------
     curie: str
```

### Comparing `reasoner_validator-3.6.1/reasoner_validator/trapi/__init__.py` & `reasoner_validator-3.6.2/reasoner_validator/trapi/__init__.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.6.1/reasoner_validator/trapi/mapping.py` & `reasoner_validator-3.6.2/reasoner_validator/trapi/mapping.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.6.1/reasoner_validator/validation_codes.py` & `reasoner_validator-3.6.2/reasoner_validator/validation_codes.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.6.1/reasoner_validator/versioning.py` & `reasoner_validator-3.6.2/reasoner_validator/versioning.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.6.1/tests/test_biolink_compliance_validation.py` & `reasoner_validator-3.6.2/tests/test_biolink_compliance_validation.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.6.1/tests/test_data/sample_trapi_schema_v3.2.1-beta5.yaml` & `reasoner_validator-3.6.2/tests/test_data/sample_trapi_schema_v3.2.1-beta5.yaml`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.6.1/tests/test_response_validator.py` & `reasoner_validator-3.6.2/tests/test_response_validator.py`

 * *Files 1% similar despite different names*

```diff
@@ -461,15 +461,15 @@
                 }
             },
             PRE_TRAPI_1_4_0,  # trapi_version
             None,
             None,
             False,
             # "Validate TRAPI Response: WARNING - Response returned an empty Message Knowledge Graph?"
-            "warning.response.knowledge_graph.empty"
+            "warning.trapi.response.knowledge_graph.empty"
         ),
         (
             # Query 5 - Partly empty Response.Message with a modest but workable
             #           query and knowledge graphs? Missing Results detected next?
             {
                 "message": {
                     "query_graph": _TEST_QG_1,
@@ -495,15 +495,15 @@
                 }
             },
             PRE_TRAPI_1_4_0,  # trapi_version
             None,
             None,
             False,
             # "Validate TRAPI Response: WARNING -Response returned empty Message.results?"
-            "warning.response.results.empty"
+            "warning.trapi.response.results.empty"
         ),
         (
             # Query 7 - Partly empty Response.Message with a modest but workable
             #           query and knowledge graphs? Non-array Results detected next?
             {
                 "message": {
                     "query_graph": _TEST_QG_1,
@@ -530,15 +530,15 @@
                 }
             },
             PRE_TRAPI_1_4_0,  # trapi_version
             None,
             None,
             False,
             # "Validate TRAPI Response: ERROR - Response returned empty Message.results?"
-            "warning.response.results.empty"
+            "warning.trapi.response.results.empty"
         ),
         (
             # Query 9 - Full Message, without 'sources' and 'strict_validation': False - should pass?
             {
                 "message": {
                     "query_graph": _TEST_QG_1,
                     "knowledge_graph": _TEST_KG_1,
```

### Comparing `reasoner_validator-3.6.1/tests/test_semver.py` & `reasoner_validator-3.6.2/tests/test_semver.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.6.1/tests/test_trapi_versioning.py` & `reasoner_validator-3.6.2/tests/test_trapi_versioning.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.6.1/tests/test_validate.py` & `reasoner_validator-3.6.2/tests/test_validate.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.6.1/tests/test_validation_report.py` & `reasoner_validator-3.6.2/tests/test_validation_report.py`

 * *Files 0% similar despite different names*

```diff
@@ -233,15 +233,15 @@
     assert reporter2.get_trapi_version() == TEST_TRAPI_VERSION
     assert reporter2.get_biolink_version() == TEST_BIOLINK_VERSION
     reporter2.report(
         code="info.query_graph.edge.predicate.mixin",
         identifier="biolink:this_is_a_mixin",
         edge_id="a-biolink:this_is_a_mixin->b"
     )
-    reporter2.report("warning.response.results.empty")
+    reporter2.report("warning.trapi.response.results.empty")
     reporter2.report("error.knowledge_graph.edges.empty")
     reporter1.merge(reporter2)
     assert reporter1.get_trapi_version() == TEST_TRAPI_VERSION
     assert reporter1.get_biolink_version() == TEST_BIOLINK_VERSION
     
     # No prefix...
     reporter3 = ValidationReporter()
```

### Comparing `reasoner_validator-3.6.1/tests/test_workflows.py` & `reasoner_validator-3.6.2/tests/test_workflows.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.6.1/PKG-INFO` & `reasoner_validator-3.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reasoner-validator
-Version: 3.6.1
+Version: 3.6.2
 Summary: Validation tools for Reasoner API
 Home-page: https://github.com/NCATSTranslator
 License: MIT
 Keywords: NCATS,Biomedical Data Translator,Translator,ReasonerAPI,TRAPI,validation,Biolink Model
 Author: Richard Bruskiewich
 Author-email: richard.bruskiewich@delphinai.com
 Maintainer: Richard Bruskiewich
```

