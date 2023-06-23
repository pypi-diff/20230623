# Comparing `tmp/polyglot_piranha-0.3.8.tar.gz` & `tmp/polyglot_piranha-0.3.9.tar.gz`

## Comparing `polyglot_piranha-0.3.8.tar` & `polyglot_piranha-0.3.9.tar`

### file list

```diff
@@ -1,129 +1,130 @@
--rw-r--r--   0        0        0     2385 1970-01-01 00:00:00.000000 polyglot_piranha-0.3.8/Cargo.toml
--rw-r--r--   0     1001      123    36113 2023-06-05 14:57:48.000000 polyglot_piranha-0.3.8/Cargo.lock
--rw-r--r--   0     1001      123    11359 2023-06-05 14:54:18.000000 polyglot_piranha-0.3.8/LICENSE
--rw-r--r--   0     1001      123     3091 2023-06-05 14:54:18.000000 polyglot_piranha-0.3.8/README.md
--rw-r--r--   0     1001      123     1373 2023-06-05 14:54:18.000000 polyglot_piranha-0.3.8/legacy/java/piranha/src/main/java/com/uber/piranha/EnumWithClassSymbol.java
--rw-r--r--   0     1001      123      994 2023-06-05 14:54:18.000000 polyglot_piranha-0.3.8/legacy/java/piranha/src/main/java/com/uber/piranha/PiranhaRuntimeException.java
--rw-r--r--   0     1001      123     5517 2023-06-05 14:54:18.000000 polyglot_piranha-0.3.8/legacy/java/piranha/src/main/java/com/uber/piranha/PiranhaUtils.java
--rw-r--r--   0     1001      123     5621 2023-06-05 14:54:18.000000 polyglot_piranha-0.3.8/legacy/java/piranha/src/main/java/com/uber/piranha/UsageCounter.java
--rw-r--r--   0     1001      123    66915 2023-06-05 14:54:18.000000 polyglot_piranha-0.3.8/legacy/java/piranha/src/main/java/com/uber/piranha/XPFlagCleaner.java
--rw-r--r--   0     1001      123    21518 2023-06-05 14:54:18.000000 polyglot_piranha-0.3.8/legacy/java/piranha/src/main/java/com/uber/piranha/config/Config.java
--rw-r--r--   0     1001      123     5106 2023-06-05 14:54:18.000000 polyglot_piranha-0.3.8/legacy/java/piranha/src/main/java/com/uber/piranha/config/MethodRecord.java
--rw-r--r--   0     1001      123      377 2023-06-05 14:54:18.000000 polyglot_piranha-0.3.8/legacy/java/piranha/src/main/java/com/uber/piranha/config/PiranhaConfigurationException.java
--rw-r--r--   0     1001      123     3615 2023-06-05 14:54:18.000000 polyglot_piranha-0.3.8/legacy/java/piranha/src/main/java/com/uber/piranha/config/PiranhaEnumRecord.java
--rw-r--r--   0     1001      123     5039 2023-06-05 14:54:18.000000 polyglot_piranha-0.3.8/legacy/java/piranha/src/main/java/com/uber/piranha/config/PiranhaMethodRecord.java
--rw-r--r--   0     1001      123     2584 2023-06-05 14:54:18.000000 polyglot_piranha-0.3.8/legacy/java/piranha/src/main/java/com/uber/piranha/config/PiranhaRecord.java
--rw-r--r--   0     1001      123     2605 2023-06-05 14:54:18.000000 polyglot_piranha-0.3.8/legacy/java/piranha/src/main/java/com/uber/piranha/testannotations/AnnotationArgument.java
--rw-r--r--   0     1001      123      550 2023-06-05 14:54:18.000000 polyglot_piranha-0.3.8/legacy/java/piranha/src/main/java/com/uber/piranha/testannotations/AnnotationResolutionException.java
--rw-r--r--   0     1001      123     2456 2023-06-05 14:54:18.000000 polyglot_piranha-0.3.8/legacy/java/piranha/src/main/java/com/uber/piranha/testannotations/ResolvedTestAnnotation.java
--rw-r--r--   0     1001      123    13106 2023-06-05 14:54:18.000000 polyglot_piranha-0.3.8/legacy/java/piranha/src/main/java/com/uber/piranha/testannotations/TestAnnotationResolver.java
--rw-r--r--   0     1001      123     5875 2023-06-05 14:54:18.000000 polyglot_piranha-0.3.8/legacy/java/piranha/src/main/java/com/uber/piranha/testannotations/TestAnnotationSpecRecord.java
--rw-r--r--   0     1001      123    85120 2023-06-05 14:54:18.000000 polyglot_piranha-0.3.8/legacy/java/piranha/src/test/java/com/uber/piranha/ConfigurationTest.java
--rw-r--r--   0     1001      123    55188 2023-06-05 14:54:18.000000 polyglot_piranha-0.3.8/legacy/java/piranha/src/test/java/com/uber/piranha/CorePiranhaTest.java
--rw-r--r--   0     1001      123    48474 2023-06-05 14:54:18.000000 polyglot_piranha-0.3.8/legacy/java/piranha/src/test/java/com/uber/piranha/EnumConstantTest.java
--rw-r--r--   0     1001      123     2304 2023-06-05 14:54:18.000000 polyglot_piranha-0.3.8/legacy/java/piranha/src/test/java/com/uber/piranha/PiranhaTestingHelpers.java
--rw-r--r--   0     1001      123    33367 2023-06-05 14:54:18.000000 polyglot_piranha-0.3.8/legacy/java/piranha/src/test/java/com/uber/piranha/TestCaseCleanUpTest.java
--rw-r--r--   0     1001      123     6780 2023-06-05 14:54:18.000000 polyglot_piranha-0.3.8/legacy/java/piranha/src/test/java/com/uber/piranha/TreatmentGroupsTest.java
--rw-r--r--   0     1001      123     3480 2023-06-05 14:54:18.000000 polyglot_piranha-0.3.8/legacy/java/piranha/src/test/resources/com/uber/piranha/XPFlagCleanerNegativeCases.java
--rw-r--r--   0     1001      123     8540 2023-06-05 14:54:18.000000 polyglot_piranha-0.3.8/legacy/java/piranha/src/test/resources/com/uber/piranha/XPFlagCleanerPositiveCases.java
--rw-r--r--   0     1001      123     4153 2023-06-05 14:54:18.000000 polyglot_piranha-0.3.8/legacy/java/piranha/src/test/resources/com/uber/piranha/XPFlagCleanerPositiveCasesControl.java
--rw-r--r--   0     1001      123     4326 2023-06-05 14:54:18.000000 polyglot_piranha-0.3.8/legacy/java/piranha/src/test/resources/com/uber/piranha/XPFlagCleanerPositiveCasesTreatment.java
--rw-r--r--   0     1001      123     2555 2023-06-05 14:54:18.000000 polyglot_piranha-0.3.8/legacy/java/piranha/src/test/resources/com/uber/piranha/XPMethodChainCases.java
--rw-r--r--   0     1001      123     1490 2023-06-05 14:54:18.000000 polyglot_piranha-0.3.8/legacy/java/piranha/src/test/resources/com/uber/piranha/XPMethodChainCasesControl.java
--rw-r--r--   0     1001      123     2091 2023-06-05 14:54:18.000000 polyglot_piranha-0.3.8/legacy/java/piranha/src/test/resources/com/uber/piranha/XPMethodChainCasesDoNotAllowMethodChain.java
--rw-r--r--   0     1001      123     2194 2023-06-05 14:54:18.000000 polyglot_piranha-0.3.8/legacy/java/piranha/src/test/resources/com/uber/piranha/XPMethodChainCasesDoNotallowArgMatchingAndMethodChain.java
--rw-r--r--   0     1001      123     1550 2023-06-05 14:54:18.000000 polyglot_piranha-0.3.8/legacy/java/piranha/src/test/resources/com/uber/piranha/XPMethodChainCasesTreatment.java
--rw-r--r--   0     1001      123     1618 2023-06-05 14:54:18.000000 polyglot_piranha-0.3.8/legacy/java/piranha/src/test/resources/com/uber/piranha/XPMethodChainCasesTreatmentDoNotAllowMatchingArgMethodInvc.java
--rw-r--r--   0     1001      123     1573 2023-06-05 14:54:18.000000 polyglot_piranha-0.3.8/legacy/java/piranha/src/test/resources/com/uber/piranha/XPTest.java
--rw-r--r--   0     1001      123       75 2023-06-05 14:54:18.000000 polyglot_piranha-0.3.8/legacy/java/piranha/src/test/resources/com/uber/piranha/mock/BoolParam.java
--rw-r--r--   0     1001      123      109 2023-06-05 14:54:18.000000 polyglot_piranha-0.3.8/legacy/java/piranha/src/test/resources/com/uber/piranha/mock/BoolParameter.java
--rw-r--r--   0     1001      123      175 2023-06-05 14:54:18.000000 polyglot_piranha-0.3.8/legacy/java/piranha/src/test/resources/com/uber/piranha/mock/OverlappingNameInterface.java
--rw-r--r--   0     1001      123      103 2023-06-05 14:54:18.000000 polyglot_piranha-0.3.8/legacy/java/piranha/src/test/resources/com/uber/piranha/mock/PVal.java
--rw-r--r--   0     1001      123      154 2023-06-05 14:54:18.000000 polyglot_piranha-0.3.8/legacy/java/piranha/src/test/resources/com/uber/piranha/mock/Parameter.java
--rw-r--r--   0     1001      123      155 2023-06-05 14:54:18.000000 polyglot_piranha-0.3.8/legacy/java/piranha/src/test/resources/com/uber/piranha/mock/SomeOtherInterface.java
--rw-r--r--   0     1001      123      160 2023-06-05 14:54:18.000000 polyglot_piranha-0.3.8/legacy/java/piranha/src/test/resources/com/uber/piranha/mock/SomeParamRev.java
--rw-r--r--   0     1001      123      122 2023-06-05 14:54:18.000000 polyglot_piranha-0.3.8/legacy/java/piranha/src/test/resources/com/uber/piranha/mock/StaticMthds.java
--rw-r--r--   0     1001      123      229 2023-06-05 14:54:18.000000 polyglot_piranha-0.3.8/legacy/java/piranha/src/test/resources/config/invalid/piranha.properties
--rw-r--r--   0     1001      123       97 2023-06-05 14:54:18.000000 polyglot_piranha-0.3.8/legacy/java/piranha/src/test/resources/config/invalid/properties_test_invalid.json
--rw-r--r--   0     1001      123      202 2023-06-05 14:54:18.000000 polyglot_piranha-0.3.8/legacy/java/piranha/src/test/resources/config/invalid/properties_test_invalid_2.json
--rw-r--r--   0     1001      123      213 2023-06-05 14:54:18.000000 polyglot_piranha-0.3.8/legacy/java/piranha/src/test/resources/config/invalid/properties_test_invalid_3.json
--rw-r--r--   0     1001      123      216 2023-06-05 14:54:18.000000 polyglot_piranha-0.3.8/legacy/java/piranha/src/test/resources/config/invalid/properties_test_invalid_4.json
--rw-r--r--   0     1001      123      361 2023-06-05 14:54:18.000000 polyglot_piranha-0.3.8/legacy/java/piranha/src/test/resources/config/properties_enum_no_arg.json
--rw-r--r--   0     1001      123      525 2023-06-05 14:54:18.000000 polyglot_piranha-0.3.8/legacy/java/piranha/src/test/resources/config/properties_method_chain_control.json
--rw-r--r--   0     1001      123      526 2023-06-05 14:54:18.000000 polyglot_piranha-0.3.8/legacy/java/piranha/src/test/resources/config/properties_method_chain_treated.json
--rw-r--r--   0     1001      123      488 2023-06-05 14:54:18.000000 polyglot_piranha-0.3.8/legacy/java/piranha/src/test/resources/config/properties_no_flag_method_name.json
--rw-r--r--   0     1001      123      489 2023-06-05 14:54:18.000000 polyglot_piranha-0.3.8/legacy/java/piranha/src/test/resources/config/properties_no_flag_method_name_no_method_chain.json
--rw-r--r--   0     1001      123      526 2023-06-05 14:54:18.000000 polyglot_piranha-0.3.8/legacy/java/piranha/src/test/resources/config/properties_no_method_chain.json
--rw-r--r--   0     1001      123      704 2023-06-05 14:54:18.000000 polyglot_piranha-0.3.8/legacy/java/piranha/src/test/resources/config/properties_test_argument.json
--rw-r--r--   0     1001      123     1332 2023-06-05 14:54:18.000000 polyglot_piranha-0.3.8/legacy/java/piranha/src/test/resources/config/properties_test_clean_by_setters_ignore_others.json
--rw-r--r--   0     1001      123      192 2023-06-05 14:54:18.000000 polyglot_piranha-0.3.8/legacy/java/piranha/src/test/resources/config/properties_test_noFlag.json
--rw-r--r--   0     1001      123      739 2023-06-05 14:54:18.000000 polyglot_piranha-0.3.8/legacy/java/piranha/src/test/resources/config/properties_test_noTreatmentGroup.json
--rw-r--r--   0     1001      123      652 2023-06-05 14:54:18.000000 polyglot_piranha-0.3.8/legacy/java/piranha/src/test/resources/config/properties_test_receive.json
--rw-r--r--   0     1001      123     1896 2023-06-05 14:54:18.000000 polyglot_piranha-0.3.8/legacy/java/piranha/src/test/resources/config/properties_test_receive_argument.json
--rw-r--r--   0     1001      123      844 2023-06-05 14:54:18.000000 polyglot_piranha-0.3.8/legacy/java/piranha/src/test/resources/config/properties_test_return.json
--rw-r--r--   0     1001      123     1776 2023-06-05 14:54:18.000000 polyglot_piranha-0.3.8/legacy/java/piranha/src/test/resources/config/properties_test_return_argument.json
--rw-r--r--   0     1001      123     1932 2023-06-05 14:54:18.000000 polyglot_piranha-0.3.8/legacy/java/piranha/src/test/resources/config/properties_test_return_receive.json
--rw-r--r--   0     1001      123     4525 2023-06-05 14:54:18.000000 polyglot_piranha-0.3.8/legacy/java/piranha/src/test/resources/config/properties_test_return_receive_argument.json
--rw-r--r--   0     1001      123      251 2023-06-05 14:54:18.000000 polyglot_piranha-0.3.8/legacy/java/piranha/src/test/resources/config/properties_test_with_enum_no_match.json
--rw-r--r--   0     1001      123      246 2023-06-05 14:54:18.000000 polyglot_piranha-0.3.8/legacy/java/piranha/src/test/resources/config/properties_test_with_enum_wrong_arg.json
--rw-r--r--   0     1001      123      142 2023-06-05 14:54:18.000000 polyglot_piranha-0.3.8/legacy/java/piranha/src/test/resources/config/properties_test_without_enum.json
--rw-r--r--   0     1001      123     1637 2023-06-05 14:54:18.000000 polyglot_piranha-0.3.8/legacy/java/piranha/src/test/resources/config/properties_unnecessary_instance_method.json
--rw-r--r--   0     1001      123     1304 2023-06-05 14:54:18.000000 polyglot_piranha-0.3.8/legacy/java/sample/src/main/java/com/uber/mylib/MyClass.java
--rw-r--r--   0     1001      123     1304 2023-06-05 14:54:18.000000 polyglot_piranha-0.3.8/legacy/java/sample/src/main/resources/com/uber/mylib/MyClass.bak
--rw-r--r--   0     1001      123     1107 2023-06-05 14:54:18.000000 polyglot_piranha-0.3.8/legacy/java/sample/src/main/resources/com/uber/mylib/MyClass.expect
--rw-r--r--   0     1001      123     2565 2023-06-05 14:54:18.000000 polyglot_piranha-0.3.8/legacy/javascript/src/config_checker.js
--rw-r--r--   0     1001      123     4304 2023-06-05 14:54:18.000000 polyglot_piranha-0.3.8/legacy/javascript/src/piranha.js
--rw-r--r--   0     1001      123    27988 2023-06-05 14:54:18.000000 polyglot_piranha-0.3.8/legacy/javascript/src/refactor.js
--rw-r--r--   0     1001      123     1445 2023-06-05 14:54:18.000000 polyglot_piranha-0.3.8/legacy/javascript/src/source_checker.js
--rw-r--r--   0     1001      123      646 2023-06-05 14:54:18.000000 polyglot_piranha-0.3.8/legacy/objc/src/XPFlagRefactoring/CMakeLists.txt
--rw-r--r--   0     1001      123     1064 2023-06-05 14:54:18.000000 polyglot_piranha-0.3.8/legacy/objc/src/XPFlagRefactoring/README.txt
--rw-r--r--   0     1001      123    26229 2023-06-05 14:54:18.000000 polyglot_piranha-0.3.8/legacy/objc/src/XPFlagRefactoring/XPFlagRefactoring.cpp
--rw-r--r--   0     1001      123        0 2023-06-05 14:54:18.000000 polyglot_piranha-0.3.8/legacy/objc/src/XPFlagRefactoring/XPFlagRefactoring.exports
--rw-r--r--   0     1001      123      793 2023-06-05 14:54:18.000000 polyglot_piranha-0.3.8/pyproject.toml
--rw-r--r--   0     1001      123     2366 2023-06-05 14:54:18.000000 polyglot_piranha-0.3.8/src/cleanup_rules/go/edges.toml
--rw-r--r--   0     1001      123    12895 2023-06-05 14:54:18.000000 polyglot_piranha-0.3.8/src/cleanup_rules/go/rules.toml
--rw-r--r--   0     1001      123     1466 2023-06-05 14:54:18.000000 polyglot_piranha-0.3.8/src/cleanup_rules/go/scope_config.toml
--rwxr-xr-x   0     1001      123     2241 2023-06-05 14:54:18.000000 polyglot_piranha-0.3.8/src/cleanup_rules/java/edges.toml
--rwxr-xr-x   0     1001      123    17674 2023-06-05 14:54:18.000000 polyglot_piranha-0.3.8/src/cleanup_rules/java/rules.toml
--rwxr-xr-x   0     1001      123     3580 2023-06-05 14:54:18.000000 polyglot_piranha-0.3.8/src/cleanup_rules/java/scope_config.toml
--rwxr-xr-x   0     1001      123     2251 2023-06-05 14:54:18.000000 polyglot_piranha-0.3.8/src/cleanup_rules/kt/edges.toml
--rwxr-xr-x   0     1001      123    19368 2023-06-05 14:54:18.000000 polyglot_piranha-0.3.8/src/cleanup_rules/kt/rules.toml
--rwxr-xr-x   0     1001      123     2142 2023-06-05 14:54:18.000000 polyglot_piranha-0.3.8/src/cleanup_rules/kt/scope_config.toml
--rw-r--r--   0     1001      123     2316 2023-06-05 14:54:18.000000 polyglot_piranha-0.3.8/src/cleanup_rules/swift/edges.toml
--rw-r--r--   0     1001      123    27137 2023-06-05 14:54:18.000000 polyglot_piranha-0.3.8/src/cleanup_rules/swift/rules.toml
--rw-r--r--   0     1001      123     1684 2023-06-05 14:54:18.000000 polyglot_piranha-0.3.8/src/cleanup_rules/swift/scope_config.toml
--rw-r--r--   0     1001      123     7425 2023-06-05 14:54:18.000000 polyglot_piranha-0.3.8/src/lib.rs
--rw-r--r--   0     1001      123     1679 2023-06-05 14:54:18.000000 polyglot_piranha-0.3.8/src/main.rs
--rw-r--r--   0     1001      123     3656 2023-06-05 14:54:18.000000 polyglot_piranha-0.3.8/src/models/default_configs.rs
--rw-r--r--   0     1001      123     4915 2023-06-05 14:54:18.000000 polyglot_piranha-0.3.8/src/models/edit.rs
--rw-r--r--   0     1001      123    13503 2023-06-05 14:54:18.000000 polyglot_piranha-0.3.8/src/models/filter.rs
--rw-r--r--   0     1001      123     7419 2023-06-05 14:54:18.000000 polyglot_piranha-0.3.8/src/models/language.rs
--rw-r--r--   0     1001      123    11128 2023-06-05 14:54:18.000000 polyglot_piranha-0.3.8/src/models/matches.rs
--rw-r--r--   0     1001      123      924 2023-06-05 14:54:18.000000 polyglot_piranha-0.3.8/src/models/mod.rs
--rw-r--r--   0     1001      123     1987 2023-06-05 14:54:18.000000 polyglot_piranha-0.3.8/src/models/outgoing_edges.rs
--rw-r--r--   0     1001      123    14245 2023-06-05 14:54:18.000000 polyglot_piranha-0.3.8/src/models/piranha_arguments.rs
--rw-r--r--   0     1001      123     2091 2023-06-05 14:54:18.000000 polyglot_piranha-0.3.8/src/models/piranha_output.rs
--rw-r--r--   0     1001      123     7801 2023-06-05 14:54:18.000000 polyglot_piranha-0.3.8/src/models/rule.rs
--rw-r--r--   0     1001      123     6286 2023-06-05 14:54:18.000000 polyglot_piranha-0.3.8/src/models/rule_graph.rs
--rw-r--r--   0     1001      123     6288 2023-06-05 14:54:18.000000 polyglot_piranha-0.3.8/src/models/rule_store.rs
--rw-r--r--   0     1001      123     3402 2023-06-05 14:54:18.000000 polyglot_piranha-0.3.8/src/models/scopes.rs
--rw-r--r--   0     1001      123    14473 2023-06-05 14:54:18.000000 polyglot_piranha-0.3.8/src/models/source_code_unit.rs
--rw-r--r--   0     1001      123     1661 2023-06-05 14:54:18.000000 polyglot_piranha-0.3.8/src/models/unit_tests/piranha_arguments_test.rs
--rw-r--r--   0     1001      123     8344 2023-06-05 14:54:18.000000 polyglot_piranha-0.3.8/src/models/unit_tests/rule_test.rs
--rw-r--r--   0     1001      123     6067 2023-06-05 14:54:18.000000 polyglot_piranha-0.3.8/src/models/unit_tests/scopes_test.rs
--rw-r--r--   0     1001      123    16601 2023-06-05 14:54:18.000000 polyglot_piranha-0.3.8/src/models/unit_tests/source_code_unit_test.rs
--rw-r--r--   0     1001      123     8287 2023-06-05 14:54:18.000000 polyglot_piranha-0.3.8/src/tests/mod.rs
--rw-r--r--   0     1001      123     1647 2023-06-05 14:54:18.000000 polyglot_piranha-0.3.8/src/tests/test_piranha_go.rs
--rw-r--r--   0     1001      123    12934 2023-06-05 14:54:18.000000 polyglot_piranha-0.3.8/src/tests/test_piranha_java.rs
--rw-r--r--   0     1001      123     1862 2023-06-05 14:54:18.000000 polyglot_piranha-0.3.8/src/tests/test_piranha_kt.rs
--rw-r--r--   0     1001      123     2423 2023-06-05 14:54:18.000000 polyglot_piranha-0.3.8/src/tests/test_piranha_python.rs
--rw-r--r--   0     1001      123     1459 2023-06-05 14:54:18.000000 polyglot_piranha-0.3.8/src/tests/test_piranha_strings.rs
--rw-r--r--   0     1001      123     3532 2023-06-05 14:54:18.000000 polyglot_piranha-0.3.8/src/tests/test_piranha_swift.rs
--rw-r--r--   0     1001      123      770 2023-06-05 14:54:18.000000 polyglot_piranha-0.3.8/src/tests/test_piranha_thrift.rs
--rw-r--r--   0     1001      123     1138 2023-06-05 14:54:18.000000 polyglot_piranha-0.3.8/src/tests/test_piranha_ts.rs
--rw-r--r--   0     1001      123     1281 2023-06-05 14:54:18.000000 polyglot_piranha-0.3.8/src/tests/test_piranha_tsx.rs
--rw-r--r--   0     1001      123     5629 2023-06-05 14:54:18.000000 polyglot_piranha-0.3.8/src/utilities/mod.rs
--rw-r--r--   0     1001      123    12743 2023-06-05 14:54:18.000000 polyglot_piranha-0.3.8/src/utilities/tree_sitter_utilities.rs
--rw-r--r--   0     1001      123     3681 2023-06-05 14:54:18.000000 polyglot_piranha-0.3.8/src/utilities/unit_tests/tree_sitter_utilities_test.rs
--rw-r--r--   0     1001      123     2237 2023-06-05 14:54:18.000000 polyglot_piranha-0.3.8/src/utilities/unit_tests/utilities_test.rs
--rw-r--r--   0        0        0     3797 1970-01-01 00:00:00.000000 polyglot_piranha-0.3.8/PKG-INFO
+-rw-r--r--   0        0        0     2279 1970-01-01 00:00:00.000000 polyglot_piranha-0.3.9/Cargo.toml
+-rw-r--r--   0     1001      123    33879 2023-06-12 21:05:35.000000 polyglot_piranha-0.3.9/Cargo.lock
+-rw-r--r--   0     1001      123    11359 2023-06-12 21:01:45.000000 polyglot_piranha-0.3.9/LICENSE
+-rw-r--r--   0     1001      123     3091 2023-06-12 21:01:45.000000 polyglot_piranha-0.3.9/README.md
+-rw-r--r--   0     1001      123     1373 2023-06-12 21:01:45.000000 polyglot_piranha-0.3.9/legacy/java/piranha/src/main/java/com/uber/piranha/EnumWithClassSymbol.java
+-rw-r--r--   0     1001      123      994 2023-06-12 21:01:45.000000 polyglot_piranha-0.3.9/legacy/java/piranha/src/main/java/com/uber/piranha/PiranhaRuntimeException.java
+-rw-r--r--   0     1001      123     5517 2023-06-12 21:01:45.000000 polyglot_piranha-0.3.9/legacy/java/piranha/src/main/java/com/uber/piranha/PiranhaUtils.java
+-rw-r--r--   0     1001      123     5621 2023-06-12 21:01:45.000000 polyglot_piranha-0.3.9/legacy/java/piranha/src/main/java/com/uber/piranha/UsageCounter.java
+-rw-r--r--   0     1001      123    66915 2023-06-12 21:01:45.000000 polyglot_piranha-0.3.9/legacy/java/piranha/src/main/java/com/uber/piranha/XPFlagCleaner.java
+-rw-r--r--   0     1001      123    21518 2023-06-12 21:01:45.000000 polyglot_piranha-0.3.9/legacy/java/piranha/src/main/java/com/uber/piranha/config/Config.java
+-rw-r--r--   0     1001      123     5106 2023-06-12 21:01:45.000000 polyglot_piranha-0.3.9/legacy/java/piranha/src/main/java/com/uber/piranha/config/MethodRecord.java
+-rw-r--r--   0     1001      123      377 2023-06-12 21:01:45.000000 polyglot_piranha-0.3.9/legacy/java/piranha/src/main/java/com/uber/piranha/config/PiranhaConfigurationException.java
+-rw-r--r--   0     1001      123     3615 2023-06-12 21:01:45.000000 polyglot_piranha-0.3.9/legacy/java/piranha/src/main/java/com/uber/piranha/config/PiranhaEnumRecord.java
+-rw-r--r--   0     1001      123     5039 2023-06-12 21:01:45.000000 polyglot_piranha-0.3.9/legacy/java/piranha/src/main/java/com/uber/piranha/config/PiranhaMethodRecord.java
+-rw-r--r--   0     1001      123     2584 2023-06-12 21:01:45.000000 polyglot_piranha-0.3.9/legacy/java/piranha/src/main/java/com/uber/piranha/config/PiranhaRecord.java
+-rw-r--r--   0     1001      123     2605 2023-06-12 21:01:45.000000 polyglot_piranha-0.3.9/legacy/java/piranha/src/main/java/com/uber/piranha/testannotations/AnnotationArgument.java
+-rw-r--r--   0     1001      123      550 2023-06-12 21:01:45.000000 polyglot_piranha-0.3.9/legacy/java/piranha/src/main/java/com/uber/piranha/testannotations/AnnotationResolutionException.java
+-rw-r--r--   0     1001      123     2456 2023-06-12 21:01:45.000000 polyglot_piranha-0.3.9/legacy/java/piranha/src/main/java/com/uber/piranha/testannotations/ResolvedTestAnnotation.java
+-rw-r--r--   0     1001      123    13106 2023-06-12 21:01:45.000000 polyglot_piranha-0.3.9/legacy/java/piranha/src/main/java/com/uber/piranha/testannotations/TestAnnotationResolver.java
+-rw-r--r--   0     1001      123     5875 2023-06-12 21:01:45.000000 polyglot_piranha-0.3.9/legacy/java/piranha/src/main/java/com/uber/piranha/testannotations/TestAnnotationSpecRecord.java
+-rw-r--r--   0     1001      123    85120 2023-06-12 21:01:45.000000 polyglot_piranha-0.3.9/legacy/java/piranha/src/test/java/com/uber/piranha/ConfigurationTest.java
+-rw-r--r--   0     1001      123    55188 2023-06-12 21:01:45.000000 polyglot_piranha-0.3.9/legacy/java/piranha/src/test/java/com/uber/piranha/CorePiranhaTest.java
+-rw-r--r--   0     1001      123    48474 2023-06-12 21:01:45.000000 polyglot_piranha-0.3.9/legacy/java/piranha/src/test/java/com/uber/piranha/EnumConstantTest.java
+-rw-r--r--   0     1001      123     2304 2023-06-12 21:01:45.000000 polyglot_piranha-0.3.9/legacy/java/piranha/src/test/java/com/uber/piranha/PiranhaTestingHelpers.java
+-rw-r--r--   0     1001      123    33367 2023-06-12 21:01:45.000000 polyglot_piranha-0.3.9/legacy/java/piranha/src/test/java/com/uber/piranha/TestCaseCleanUpTest.java
+-rw-r--r--   0     1001      123     6780 2023-06-12 21:01:45.000000 polyglot_piranha-0.3.9/legacy/java/piranha/src/test/java/com/uber/piranha/TreatmentGroupsTest.java
+-rw-r--r--   0     1001      123     3480 2023-06-12 21:01:45.000000 polyglot_piranha-0.3.9/legacy/java/piranha/src/test/resources/com/uber/piranha/XPFlagCleanerNegativeCases.java
+-rw-r--r--   0     1001      123     8540 2023-06-12 21:01:45.000000 polyglot_piranha-0.3.9/legacy/java/piranha/src/test/resources/com/uber/piranha/XPFlagCleanerPositiveCases.java
+-rw-r--r--   0     1001      123     4153 2023-06-12 21:01:45.000000 polyglot_piranha-0.3.9/legacy/java/piranha/src/test/resources/com/uber/piranha/XPFlagCleanerPositiveCasesControl.java
+-rw-r--r--   0     1001      123     4326 2023-06-12 21:01:45.000000 polyglot_piranha-0.3.9/legacy/java/piranha/src/test/resources/com/uber/piranha/XPFlagCleanerPositiveCasesTreatment.java
+-rw-r--r--   0     1001      123     2555 2023-06-12 21:01:45.000000 polyglot_piranha-0.3.9/legacy/java/piranha/src/test/resources/com/uber/piranha/XPMethodChainCases.java
+-rw-r--r--   0     1001      123     1490 2023-06-12 21:01:45.000000 polyglot_piranha-0.3.9/legacy/java/piranha/src/test/resources/com/uber/piranha/XPMethodChainCasesControl.java
+-rw-r--r--   0     1001      123     2091 2023-06-12 21:01:45.000000 polyglot_piranha-0.3.9/legacy/java/piranha/src/test/resources/com/uber/piranha/XPMethodChainCasesDoNotAllowMethodChain.java
+-rw-r--r--   0     1001      123     2194 2023-06-12 21:01:45.000000 polyglot_piranha-0.3.9/legacy/java/piranha/src/test/resources/com/uber/piranha/XPMethodChainCasesDoNotallowArgMatchingAndMethodChain.java
+-rw-r--r--   0     1001      123     1550 2023-06-12 21:01:45.000000 polyglot_piranha-0.3.9/legacy/java/piranha/src/test/resources/com/uber/piranha/XPMethodChainCasesTreatment.java
+-rw-r--r--   0     1001      123     1618 2023-06-12 21:01:45.000000 polyglot_piranha-0.3.9/legacy/java/piranha/src/test/resources/com/uber/piranha/XPMethodChainCasesTreatmentDoNotAllowMatchingArgMethodInvc.java
+-rw-r--r--   0     1001      123     1573 2023-06-12 21:01:45.000000 polyglot_piranha-0.3.9/legacy/java/piranha/src/test/resources/com/uber/piranha/XPTest.java
+-rw-r--r--   0     1001      123       75 2023-06-12 21:01:45.000000 polyglot_piranha-0.3.9/legacy/java/piranha/src/test/resources/com/uber/piranha/mock/BoolParam.java
+-rw-r--r--   0     1001      123      109 2023-06-12 21:01:45.000000 polyglot_piranha-0.3.9/legacy/java/piranha/src/test/resources/com/uber/piranha/mock/BoolParameter.java
+-rw-r--r--   0     1001      123      175 2023-06-12 21:01:45.000000 polyglot_piranha-0.3.9/legacy/java/piranha/src/test/resources/com/uber/piranha/mock/OverlappingNameInterface.java
+-rw-r--r--   0     1001      123      103 2023-06-12 21:01:45.000000 polyglot_piranha-0.3.9/legacy/java/piranha/src/test/resources/com/uber/piranha/mock/PVal.java
+-rw-r--r--   0     1001      123      154 2023-06-12 21:01:45.000000 polyglot_piranha-0.3.9/legacy/java/piranha/src/test/resources/com/uber/piranha/mock/Parameter.java
+-rw-r--r--   0     1001      123      155 2023-06-12 21:01:45.000000 polyglot_piranha-0.3.9/legacy/java/piranha/src/test/resources/com/uber/piranha/mock/SomeOtherInterface.java
+-rw-r--r--   0     1001      123      160 2023-06-12 21:01:45.000000 polyglot_piranha-0.3.9/legacy/java/piranha/src/test/resources/com/uber/piranha/mock/SomeParamRev.java
+-rw-r--r--   0     1001      123      122 2023-06-12 21:01:45.000000 polyglot_piranha-0.3.9/legacy/java/piranha/src/test/resources/com/uber/piranha/mock/StaticMthds.java
+-rw-r--r--   0     1001      123      229 2023-06-12 21:01:45.000000 polyglot_piranha-0.3.9/legacy/java/piranha/src/test/resources/config/invalid/piranha.properties
+-rw-r--r--   0     1001      123       97 2023-06-12 21:01:45.000000 polyglot_piranha-0.3.9/legacy/java/piranha/src/test/resources/config/invalid/properties_test_invalid.json
+-rw-r--r--   0     1001      123      202 2023-06-12 21:01:45.000000 polyglot_piranha-0.3.9/legacy/java/piranha/src/test/resources/config/invalid/properties_test_invalid_2.json
+-rw-r--r--   0     1001      123      213 2023-06-12 21:01:45.000000 polyglot_piranha-0.3.9/legacy/java/piranha/src/test/resources/config/invalid/properties_test_invalid_3.json
+-rw-r--r--   0     1001      123      216 2023-06-12 21:01:45.000000 polyglot_piranha-0.3.9/legacy/java/piranha/src/test/resources/config/invalid/properties_test_invalid_4.json
+-rw-r--r--   0     1001      123      361 2023-06-12 21:01:45.000000 polyglot_piranha-0.3.9/legacy/java/piranha/src/test/resources/config/properties_enum_no_arg.json
+-rw-r--r--   0     1001      123      525 2023-06-12 21:01:45.000000 polyglot_piranha-0.3.9/legacy/java/piranha/src/test/resources/config/properties_method_chain_control.json
+-rw-r--r--   0     1001      123      526 2023-06-12 21:01:45.000000 polyglot_piranha-0.3.9/legacy/java/piranha/src/test/resources/config/properties_method_chain_treated.json
+-rw-r--r--   0     1001      123      488 2023-06-12 21:01:45.000000 polyglot_piranha-0.3.9/legacy/java/piranha/src/test/resources/config/properties_no_flag_method_name.json
+-rw-r--r--   0     1001      123      489 2023-06-12 21:01:45.000000 polyglot_piranha-0.3.9/legacy/java/piranha/src/test/resources/config/properties_no_flag_method_name_no_method_chain.json
+-rw-r--r--   0     1001      123      526 2023-06-12 21:01:45.000000 polyglot_piranha-0.3.9/legacy/java/piranha/src/test/resources/config/properties_no_method_chain.json
+-rw-r--r--   0     1001      123      704 2023-06-12 21:01:45.000000 polyglot_piranha-0.3.9/legacy/java/piranha/src/test/resources/config/properties_test_argument.json
+-rw-r--r--   0     1001      123     1332 2023-06-12 21:01:45.000000 polyglot_piranha-0.3.9/legacy/java/piranha/src/test/resources/config/properties_test_clean_by_setters_ignore_others.json
+-rw-r--r--   0     1001      123      192 2023-06-12 21:01:45.000000 polyglot_piranha-0.3.9/legacy/java/piranha/src/test/resources/config/properties_test_noFlag.json
+-rw-r--r--   0     1001      123      739 2023-06-12 21:01:45.000000 polyglot_piranha-0.3.9/legacy/java/piranha/src/test/resources/config/properties_test_noTreatmentGroup.json
+-rw-r--r--   0     1001      123      652 2023-06-12 21:01:45.000000 polyglot_piranha-0.3.9/legacy/java/piranha/src/test/resources/config/properties_test_receive.json
+-rw-r--r--   0     1001      123     1896 2023-06-12 21:01:45.000000 polyglot_piranha-0.3.9/legacy/java/piranha/src/test/resources/config/properties_test_receive_argument.json
+-rw-r--r--   0     1001      123      844 2023-06-12 21:01:45.000000 polyglot_piranha-0.3.9/legacy/java/piranha/src/test/resources/config/properties_test_return.json
+-rw-r--r--   0     1001      123     1776 2023-06-12 21:01:45.000000 polyglot_piranha-0.3.9/legacy/java/piranha/src/test/resources/config/properties_test_return_argument.json
+-rw-r--r--   0     1001      123     1932 2023-06-12 21:01:45.000000 polyglot_piranha-0.3.9/legacy/java/piranha/src/test/resources/config/properties_test_return_receive.json
+-rw-r--r--   0     1001      123     4525 2023-06-12 21:01:45.000000 polyglot_piranha-0.3.9/legacy/java/piranha/src/test/resources/config/properties_test_return_receive_argument.json
+-rw-r--r--   0     1001      123      251 2023-06-12 21:01:45.000000 polyglot_piranha-0.3.9/legacy/java/piranha/src/test/resources/config/properties_test_with_enum_no_match.json
+-rw-r--r--   0     1001      123      246 2023-06-12 21:01:45.000000 polyglot_piranha-0.3.9/legacy/java/piranha/src/test/resources/config/properties_test_with_enum_wrong_arg.json
+-rw-r--r--   0     1001      123      142 2023-06-12 21:01:45.000000 polyglot_piranha-0.3.9/legacy/java/piranha/src/test/resources/config/properties_test_without_enum.json
+-rw-r--r--   0     1001      123     1637 2023-06-12 21:01:45.000000 polyglot_piranha-0.3.9/legacy/java/piranha/src/test/resources/config/properties_unnecessary_instance_method.json
+-rw-r--r--   0     1001      123     1304 2023-06-12 21:01:45.000000 polyglot_piranha-0.3.9/legacy/java/sample/src/main/java/com/uber/mylib/MyClass.java
+-rw-r--r--   0     1001      123     1304 2023-06-12 21:01:45.000000 polyglot_piranha-0.3.9/legacy/java/sample/src/main/resources/com/uber/mylib/MyClass.bak
+-rw-r--r--   0     1001      123     1107 2023-06-12 21:01:45.000000 polyglot_piranha-0.3.9/legacy/java/sample/src/main/resources/com/uber/mylib/MyClass.expect
+-rw-r--r--   0     1001      123     2565 2023-06-12 21:01:45.000000 polyglot_piranha-0.3.9/legacy/javascript/src/config_checker.js
+-rw-r--r--   0     1001      123     4304 2023-06-12 21:01:45.000000 polyglot_piranha-0.3.9/legacy/javascript/src/piranha.js
+-rw-r--r--   0     1001      123    27988 2023-06-12 21:01:45.000000 polyglot_piranha-0.3.9/legacy/javascript/src/refactor.js
+-rw-r--r--   0     1001      123     1445 2023-06-12 21:01:45.000000 polyglot_piranha-0.3.9/legacy/javascript/src/source_checker.js
+-rw-r--r--   0     1001      123      646 2023-06-12 21:01:45.000000 polyglot_piranha-0.3.9/legacy/objc/src/XPFlagRefactoring/CMakeLists.txt
+-rw-r--r--   0     1001      123     1064 2023-06-12 21:01:45.000000 polyglot_piranha-0.3.9/legacy/objc/src/XPFlagRefactoring/README.txt
+-rw-r--r--   0     1001      123    26229 2023-06-12 21:01:45.000000 polyglot_piranha-0.3.9/legacy/objc/src/XPFlagRefactoring/XPFlagRefactoring.cpp
+-rw-r--r--   0     1001      123        0 2023-06-12 21:01:45.000000 polyglot_piranha-0.3.9/legacy/objc/src/XPFlagRefactoring/XPFlagRefactoring.exports
+-rw-r--r--   0     1001      123      793 2023-06-12 21:01:45.000000 polyglot_piranha-0.3.9/pyproject.toml
+-rw-r--r--   0     1001      123     2366 2023-06-12 21:01:45.000000 polyglot_piranha-0.3.9/src/cleanup_rules/go/edges.toml
+-rw-r--r--   0     1001      123    12895 2023-06-12 21:01:45.000000 polyglot_piranha-0.3.9/src/cleanup_rules/go/rules.toml
+-rw-r--r--   0     1001      123     1466 2023-06-12 21:01:45.000000 polyglot_piranha-0.3.9/src/cleanup_rules/go/scope_config.toml
+-rwxr-xr-x   0     1001      123     2241 2023-06-12 21:01:45.000000 polyglot_piranha-0.3.9/src/cleanup_rules/java/edges.toml
+-rwxr-xr-x   0     1001      123    18101 2023-06-12 21:01:45.000000 polyglot_piranha-0.3.9/src/cleanup_rules/java/rules.toml
+-rwxr-xr-x   0     1001      123     3580 2023-06-12 21:01:45.000000 polyglot_piranha-0.3.9/src/cleanup_rules/java/scope_config.toml
+-rwxr-xr-x   0     1001      123     2251 2023-06-12 21:01:45.000000 polyglot_piranha-0.3.9/src/cleanup_rules/kt/edges.toml
+-rwxr-xr-x   0     1001      123    19370 2023-06-12 21:01:45.000000 polyglot_piranha-0.3.9/src/cleanup_rules/kt/rules.toml
+-rwxr-xr-x   0     1001      123     2142 2023-06-12 21:01:45.000000 polyglot_piranha-0.3.9/src/cleanup_rules/kt/scope_config.toml
+-rw-r--r--   0     1001      123     2316 2023-06-12 21:01:45.000000 polyglot_piranha-0.3.9/src/cleanup_rules/swift/edges.toml
+-rw-r--r--   0     1001      123    27505 2023-06-12 21:01:45.000000 polyglot_piranha-0.3.9/src/cleanup_rules/swift/rules.toml
+-rw-r--r--   0     1001      123     1684 2023-06-12 21:01:45.000000 polyglot_piranha-0.3.9/src/cleanup_rules/swift/scope_config.toml
+-rw-r--r--   0     1001      123     7291 2023-06-12 21:01:45.000000 polyglot_piranha-0.3.9/src/lib.rs
+-rw-r--r--   0     1001      123     1679 2023-06-12 21:01:45.000000 polyglot_piranha-0.3.9/src/main.rs
+-rw-r--r--   0     1001      123     3715 2023-06-12 21:01:45.000000 polyglot_piranha-0.3.9/src/models/default_configs.rs
+-rw-r--r--   0     1001      123     4915 2023-06-12 21:01:45.000000 polyglot_piranha-0.3.9/src/models/edit.rs
+-rw-r--r--   0     1001      123    15141 2023-06-12 21:01:45.000000 polyglot_piranha-0.3.9/src/models/filter.rs
+-rw-r--r--   0     1001      123     7447 2023-06-12 21:01:45.000000 polyglot_piranha-0.3.9/src/models/language.rs
+-rw-r--r--   0     1001      123    11128 2023-06-12 21:01:45.000000 polyglot_piranha-0.3.9/src/models/matches.rs
+-rw-r--r--   0     1001      123     1000 2023-06-12 21:01:45.000000 polyglot_piranha-0.3.9/src/models/mod.rs
+-rw-r--r--   0     1001      123     1987 2023-06-12 21:01:45.000000 polyglot_piranha-0.3.9/src/models/outgoing_edges.rs
+-rw-r--r--   0     1001      123    14245 2023-06-12 21:01:45.000000 polyglot_piranha-0.3.9/src/models/piranha_arguments.rs
+-rw-r--r--   0     1001      123     2091 2023-06-12 21:01:45.000000 polyglot_piranha-0.3.9/src/models/piranha_output.rs
+-rw-r--r--   0     1001      123     8106 2023-06-12 21:01:45.000000 polyglot_piranha-0.3.9/src/models/rule.rs
+-rw-r--r--   0     1001      123     6776 2023-06-12 21:01:45.000000 polyglot_piranha-0.3.9/src/models/rule_graph.rs
+-rw-r--r--   0     1001      123     6288 2023-06-12 21:01:45.000000 polyglot_piranha-0.3.9/src/models/rule_store.rs
+-rw-r--r--   0     1001      123     3402 2023-06-12 21:01:45.000000 polyglot_piranha-0.3.9/src/models/scopes.rs
+-rw-r--r--   0     1001      123    14378 2023-06-12 21:01:45.000000 polyglot_piranha-0.3.9/src/models/source_code_unit.rs
+-rw-r--r--   0     1001      123     1661 2023-06-12 21:01:45.000000 polyglot_piranha-0.3.9/src/models/unit_tests/piranha_arguments_test.rs
+-rw-r--r--   0     1001      123     3347 2023-06-12 21:01:45.000000 polyglot_piranha-0.3.9/src/models/unit_tests/rule_graph_validation_test.rs
+-rw-r--r--   0     1001      123    10402 2023-06-12 21:01:45.000000 polyglot_piranha-0.3.9/src/models/unit_tests/rule_test.rs
+-rw-r--r--   0     1001      123     6067 2023-06-12 21:01:45.000000 polyglot_piranha-0.3.9/src/models/unit_tests/scopes_test.rs
+-rw-r--r--   0     1001      123    15227 2023-06-12 21:01:45.000000 polyglot_piranha-0.3.9/src/models/unit_tests/source_code_unit_test.rs
+-rw-r--r--   0     1001      123     8287 2023-06-12 21:01:45.000000 polyglot_piranha-0.3.9/src/tests/mod.rs
+-rw-r--r--   0     1001      123     1647 2023-06-12 21:01:45.000000 polyglot_piranha-0.3.9/src/tests/test_piranha_go.rs
+-rw-r--r--   0     1001      123    13547 2023-06-12 21:01:45.000000 polyglot_piranha-0.3.9/src/tests/test_piranha_java.rs
+-rw-r--r--   0     1001      123     1862 2023-06-12 21:01:45.000000 polyglot_piranha-0.3.9/src/tests/test_piranha_kt.rs
+-rw-r--r--   0     1001      123     2423 2023-06-12 21:01:45.000000 polyglot_piranha-0.3.9/src/tests/test_piranha_python.rs
+-rw-r--r--   0     1001      123     1459 2023-06-12 21:01:45.000000 polyglot_piranha-0.3.9/src/tests/test_piranha_strings.rs
+-rw-r--r--   0     1001      123     3532 2023-06-12 21:01:45.000000 polyglot_piranha-0.3.9/src/tests/test_piranha_swift.rs
+-rw-r--r--   0     1001      123      770 2023-06-12 21:01:45.000000 polyglot_piranha-0.3.9/src/tests/test_piranha_thrift.rs
+-rw-r--r--   0     1001      123     1138 2023-06-12 21:01:45.000000 polyglot_piranha-0.3.9/src/tests/test_piranha_ts.rs
+-rw-r--r--   0     1001      123     1281 2023-06-12 21:01:45.000000 polyglot_piranha-0.3.9/src/tests/test_piranha_tsx.rs
+-rw-r--r--   0     1001      123     5629 2023-06-12 21:01:45.000000 polyglot_piranha-0.3.9/src/utilities/mod.rs
+-rw-r--r--   0     1001      123    13618 2023-06-12 21:01:45.000000 polyglot_piranha-0.3.9/src/utilities/tree_sitter_utilities.rs
+-rw-r--r--   0     1001      123     3681 2023-06-12 21:01:45.000000 polyglot_piranha-0.3.9/src/utilities/unit_tests/tree_sitter_utilities_test.rs
+-rw-r--r--   0     1001      123     2237 2023-06-12 21:01:45.000000 polyglot_piranha-0.3.9/src/utilities/unit_tests/utilities_test.rs
+-rw-r--r--   0        0        0     3797 1970-01-01 00:00:00.000000 polyglot_piranha-0.3.9/PKG-INFO
```

### Comparing `polyglot_piranha-0.3.8/Cargo.toml` & `polyglot_piranha-0.3.9/Cargo.toml`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
   "Ameya Ketkar <ketkara@uber.com>",
   "Lazaro Clapp <lazaro@uber.com>",
   "Murali Krishna Ramanathan",
   "Uber Technologies Inc.",
 ]
 name = "piranha"
 description = "Polyglot Piranha is a library for performing structural find and replace with deep cleanup."
-version = "0.3.8"
+version = "0.3.9"
 edition = "2021"
 include = ["pyproject.toml", "src/"]
 exclude = ["legacy"]
 license-file = "LICENSE"
 categories = [
   "structural find-replace",
   "find-replace",
@@ -45,26 +45,27 @@
 regex = "1.5.5"
 jwalk = "0.8.1"
 clap = { version = "4.0.3", features = ["derive"] }
 log = "0.4.16"
 env_logger = "0.10.0"
 tempdir = "0.3"
 serde_json = "1.0.82"
-# TODO: Update after https://github.com/fwcd/tree-sitter-kotlin/pull/71 lands
-tree-sitter-kotlin = { git = "https://github.com/ketkarameya/tree-sitter-kotlin.git", rev = "a87ddd003368e068563f1cc478a1b2a3f9d73b60" }
+
+tree-sitter-kotlin = { git = "https://github.com/fwcd/tree-sitter-kotlin.git" }
 # TODO: Update after next version is released (https://github.com/tree-sitter/tree-sitter-java/issues/146)
 tree-sitter-java = { git = "https://github.com/tree-sitter/tree-sitter-java.git", rev = "c194ee5e6ede5f26cf4799feead4a8f165dcf14d" }
 # TODO: Update after: https://github.com/alex-pinkus/tree-sitter-swift/issues/278 resolves
 tree-sitter-swift = { git = "https://github.com/satyam1749/tree-sitter-swift.git", rev = "895cd7814488cb32cf73f68a75458b4bc6d50a85" }
 tree-sitter-python = "0.20.2"
 tree-sitter-typescript = "0.20.1"
 # TODO: Update after https://github.com/tree-sitter/tree-sitter-go/pull/103 lands
 tree-sitter-go = { git = "https://github.com/uber/tree-sitter-go.git", rev = "8f807196afab4a1a1256dbf62a011020c6fe7745" }
 tree-sitter-thrift = "0.5.0"
 tree-sitter-strings = { git = "https://github.com/ketkarameya/tree-sitter-strings.git" }
+tree-sitter-query = "0.1.0"
 derive_builder = "0.12.0"
 getset = "0.1.2"
 pyo3 = "0.19.0"
 pyo3-log = "0.8.1"
 glob = "0.3.1"
 
 [features]
```

### Comparing `polyglot_piranha-0.3.8/Cargo.lock` & `polyglot_piranha-0.3.9/Cargo.lock`

 * *Files 6% similar despite different names*

```diff
@@ -43,25 +43,25 @@
 
 [[package]]
 name = "anstyle-query"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5ca11d4be1bab0c8bc8734a9aa7bf4ee8316d462a08c6ac5052f888fef5b494b"
 dependencies = [
- "windows-sys 0.48.0",
+ "windows-sys",
 ]
 
 [[package]]
 name = "anstyle-wincon"
 version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "180abfa45703aebe0093f79badacc01b8fd4ea2e35118747e5811127f926e188"
 dependencies = [
  "anstyle",
- "windows-sys 0.48.0",
+ "windows-sys",
 ]
 
 [[package]]
 name = "arc-swap"
 version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bddcadddf5e9015d310179a59bb28c4d4b9920ad0f11e8e14dbadf654890c9a6"
@@ -126,41 +126,41 @@
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
 name = "clap"
-version = "4.3.1"
+version = "4.3.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b4ed2379f8603fa2b7509891660e802b88c70a79a6427a70abb5968054de2c28"
+checksum = "ca8f255e4b8027970e78db75e78831229c9815fdbfa67eb1a1b777a62e24b4a0"
 dependencies = [
  "clap_builder",
  "clap_derive",
  "once_cell",
 ]
 
 [[package]]
 name = "clap_builder"
-version = "4.3.1"
+version = "4.3.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "72394f3339a76daf211e57d4bcb374410f3965dcc606dd0e03738c7888766980"
+checksum = "acd4f3c17c83b0ba34ffbc4f8bbd74f079413f747f84a6f89292f138057e36ab"
 dependencies = [
  "anstream",
  "anstyle",
  "bitflags",
  "clap_lex",
  "strsim",
 ]
 
 [[package]]
 name = "clap_derive"
-version = "4.3.1"
+version = "4.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "59e9ef9a08ee1c0e1f2e162121665ac45ac3783b0f897db7244ae75ad9a8f65b"
+checksum = "b8cd2b2a819ad6eec39e8f1d6b53001af1e5469f8c177579cdaeb313115b825f"
 dependencies = [
  "heck",
  "proc-macro2",
  "quote",
  "syn 2.0.18",
 ]
 
@@ -220,22 +220,22 @@
  "cfg-if",
  "crossbeam-epoch",
  "crossbeam-utils",
 ]
 
 [[package]]
 name = "crossbeam-epoch"
-version = "0.9.14"
+version = "0.9.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "46bd5f3f85273295a9d14aedfb86f6aadbff6d8f5295c4a9edb08e819dcf5695"
+checksum = "ae211234986c545741a7dc064309f67ee1e5ad243d0e48335adc0484d960bcc7"
 dependencies = [
  "autocfg",
  "cfg-if",
  "crossbeam-utils",
- "memoffset 0.8.0",
+ "memoffset",
  "scopeguard",
 ]
 
 [[package]]
 name = "crossbeam-queue"
 version = "0.3.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -243,17 +243,17 @@
 dependencies = [
  "cfg-if",
  "crossbeam-utils",
 ]
 
 [[package]]
 name = "crossbeam-utils"
-version = "0.8.15"
+version = "0.8.16"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3c063cd8cc95f5c377ed0d4b49a4b21f632396ff690e8470c29b3359b346984b"
+checksum = "5a22b2d63d4d1dc0b7f1b6b2747dd0088008a9be28b6ddf0b1e7d335e3037294"
 dependencies = [
  "cfg-if",
 ]
 
 [[package]]
 name = "darling"
 version = "0.14.4"
@@ -355,15 +355,15 @@
 name = "errno"
 version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4bcfec3a70f97c962c307b2d2c56e358cf1d00b558d74262b5f929ee8cc7e73a"
 dependencies = [
  "errno-dragonfly",
  "libc",
- "windows-sys 0.48.0",
+ "windows-sys",
 ]
 
 [[package]]
 name = "errno-dragonfly"
 version = "0.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "aa68f1b12764fab894d2755d2518754e71b4fd80ecfb822714a1206c2aab39bf"
@@ -479,27 +479,27 @@
 name = "io-lifetimes"
 version = "1.0.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "eae7b9aee968036d54dce06cebaefd919e4472e753296daccd6d344e3e2df0c2"
 dependencies = [
  "hermit-abi 0.3.1",
  "libc",
- "windows-sys 0.48.0",
+ "windows-sys",
 ]
 
 [[package]]
 name = "is-terminal"
 version = "0.4.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "adcf93614601c8129ddf72e2d5633df827ba6551541c6d8c59520a371475be1f"
 dependencies = [
  "hermit-abi 0.3.1",
  "io-lifetimes",
  "rustix",
- "windows-sys 0.48.0",
+ "windows-sys",
 ]
 
 [[package]]
 name = "itertools"
 version = "0.10.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b0fd2260e829bddf4cb6ea802289de2f86d6a7a690192fbe91b3f46e0f2c8473"
@@ -533,57 +533,48 @@
 name = "lazy_static"
 version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e2abad23fbc42b3700f2f279844dc832adb2b2eb069b2df918f455c4e18cc646"
 
 [[package]]
 name = "libc"
-version = "0.2.145"
+version = "0.2.146"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fc86cde3ff845662b8f4ef6cb50ea0e20c524eb3d29ae048287e06a1b3fa6a81"
+checksum = "f92be4933c13fd498862a9e02a3055f8a8d9c039ce33db97306fd5a6caa7f29b"
 
 [[package]]
 name = "linux-raw-sys"
 version = "0.3.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ef53942eb7bf7ff43a617b3e2c1c4a5ecf5944a7c1bc12d7ee39bbb15e5c1519"
 
 [[package]]
 name = "lock_api"
-version = "0.4.9"
+version = "0.4.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "435011366fe56583b16cf956f9df0095b405b82d76425bc8981c0e22e60ec4df"
+checksum = "c1cc9717a20b1bb222f333e6a92fd32f7d8a18ddc5a3191a11af45dcbf4dcd16"
 dependencies = [
  "autocfg",
  "scopeguard",
 ]
 
 [[package]]
 name = "log"
-version = "0.4.18"
+version = "0.4.19"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "518ef76f2f87365916b142844c16d8fefd85039bc5699050210a7778ee1cd1de"
+checksum = "b06a4cde4c0f271a446782e3eff8de789548ce57dbc8eca9292c27f4a42004b4"
 
 [[package]]
 name = "memchr"
 version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2dffe52ecf27772e601905b7522cb4ef790d2cc203488bbd0e2fe85fcb74566d"
 
 [[package]]
 name = "memoffset"
-version = "0.8.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d61c719bcfbcf5d62b3a09efa6088de8c54bc0bfcd3ea7ae39fcc186108b8de1"
-dependencies = [
- "autocfg",
-]
-
-[[package]]
-name = "memoffset"
 version = "0.9.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5a634b1c61a95585bd15607c6ab0c4e5b226e695ff2800ba0cdccddf208c406c"
 dependencies = [
  "autocfg",
 ]
 
@@ -626,28 +617,28 @@
 dependencies = [
  "lock_api",
  "parking_lot_core",
 ]
 
 [[package]]
 name = "parking_lot_core"
-version = "0.9.7"
+version = "0.9.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9069cbb9f99e3a5083476ccb29ceb1de18b9118cafa53e90c9551235de2b9521"
+checksum = "93f00c865fe7cabf650081affecd3871070f26767e7b2070a3ffae14c654b447"
 dependencies = [
  "cfg-if",
  "libc",
  "redox_syscall",
  "smallvec",
- "windows-sys 0.45.0",
+ "windows-targets",
 ]
 
 [[package]]
 name = "piranha"
-version = "0.3.8"
+version = "0.3.9"
 dependencies = [
  "assert_cmd",
  "cc",
  "clap",
  "colored",
  "derive_builder",
  "env_logger",
@@ -667,14 +658,15 @@
  "tempdir",
  "toml",
  "tree-sitter",
  "tree-sitter-go",
  "tree-sitter-java",
  "tree-sitter-kotlin",
  "tree-sitter-python",
+ "tree-sitter-query",
  "tree-sitter-strings",
  "tree-sitter-swift",
  "tree-sitter-thrift",
  "tree-sitter-traversal",
  "tree-sitter-typescript",
 ]
 
@@ -731,31 +723,31 @@
  "proc-macro2",
  "quote",
  "version_check",
 ]
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.59"
+version = "1.0.60"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6aeca18b86b413c660b781aa319e4e2648a3e6f9eadc9b47e9038e6fe9f3451b"
+checksum = "dec2b086b7a862cf4de201096214fa870344cf922b2b30c167badb3af3195406"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
 version = "0.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "cffef52f74ec3b1a1baf295d9b8fcc3070327aefc39a6d00656b13c1d0b8885c"
 dependencies = [
  "cfg-if",
  "indoc",
  "libc",
- "memoffset 0.9.0",
+ "memoffset",
  "parking_lot",
  "pyo3-build-config",
  "pyo3-ffi",
  "pyo3-macros",
  "unindent",
 ]
 
@@ -879,17 +871,17 @@
 checksum = "678054eb77286b51581ba43620cc911abf02758c91f93f479767aed0f90458b2"
 dependencies = [
  "rand_core 0.3.1",
 ]
 
 [[package]]
 name = "redox_syscall"
-version = "0.2.16"
+version = "0.3.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fb5a58c1855b4b6819d59012155603f0b22ad30cad752600aadfcb695265519a"
+checksum = "567664f262709473930a4bf9e51bf2ebf3348f2e748ccc50dea20646858f8f29"
 dependencies = [
  "bitflags",
 ]
 
 [[package]]
 name = "regex"
 version = "1.8.4"
@@ -920,24 +912,24 @@
 checksum = "3acd125665422973a33ac9d3dd2df85edad0f4ae9b00dafb1a05e43a9f5ef8e7"
 dependencies = [
  "winapi",
 ]
 
 [[package]]
 name = "rustix"
-version = "0.37.19"
+version = "0.37.20"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "acf8729d8542766f1b2cf77eb034d52f40d375bb8b615d0b147089946e16613d"
+checksum = "b96e891d04aa506a6d1f318d2771bcb1c7dfda84e126660ace067c9b474bb2c0"
 dependencies = [
  "bitflags",
  "errno",
  "io-lifetimes",
  "libc",
  "linux-raw-sys",
- "windows-sys 0.48.0",
+ "windows-sys",
 ]
 
 [[package]]
 name = "ryu"
 version = "1.0.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f91339c0467de62360649f8d3e185ca8de4224ff281f66000de5eb2a77a79041"
@@ -946,23 +938,23 @@
 name = "scopeguard"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d29ab0c6d3fc0ee92fe66e2d99f700eab17a8d57d1c1d3b748380fb20baa78cd"
 
 [[package]]
 name = "serde"
-version = "1.0.163"
+version = "1.0.164"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2113ab51b87a539ae008b5c6c02dc020ffa39afd2d83cffcb3f4eb2722cebec2"
+checksum = "9e8c8cf938e98f769bc164923b06dce91cea1751522f46f8466461af04c9027d"
 
 [[package]]
 name = "serde_derive"
-version = "1.0.163"
+version = "1.0.164"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8c805777e3930c8883389c602315a24224bcc738b63905ef87cd1420353ea93e"
+checksum = "d9735b638ccc51c28bf6914d90a2e9725b377144fc612c49a611fddd1b631d68"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn 2.0.18",
 ]
 
 [[package]]
@@ -1111,15 +1103,15 @@
  "cc",
  "tree-sitter",
 ]
 
 [[package]]
 name = "tree-sitter-kotlin"
 version = "0.2.11"
-source = "git+https://github.com/ketkarameya/tree-sitter-kotlin.git?rev=a87ddd003368e068563f1cc478a1b2a3f9d73b60#a87ddd003368e068563f1cc478a1b2a3f9d73b60"
+source = "git+https://github.com/fwcd/tree-sitter-kotlin.git#100d79fd96b56a1b99099a8d2f3c114b8687acfb"
 dependencies = [
  "cc",
  "tree-sitter",
 ]
 
 [[package]]
 name = "tree-sitter-python"
@@ -1128,14 +1120,24 @@
 checksum = "dda114f58048f5059dcf158aff691dffb8e113e6d2b50d94263fd68711975287"
 dependencies = [
  "cc",
  "tree-sitter",
 ]
 
 [[package]]
+name = "tree-sitter-query"
+version = "0.1.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "9d4374ba146382b2c9a50290e79283b5035544912c0e1387e3ff08e6137f4cb4"
+dependencies = [
+ "cc",
+ "tree-sitter",
+]
+
+[[package]]
 name = "tree-sitter-strings"
 version = "0.1.0"
 source = "git+https://github.com/ketkarameya/tree-sitter-strings.git#5780e932da66774e4907026e4346091e6e876f54"
 dependencies = [
  "cc",
  "tree-sitter",
 ]
@@ -1240,140 +1242,74 @@
 name = "winapi-x86_64-pc-windows-gnu"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "712e227841d057c1ee1cd2fb22fa7e5a5461ae8e48fa2ca79ec42cfc1931183f"
 
 [[package]]
 name = "windows-sys"
-version = "0.45.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "75283be5efb2831d37ea142365f009c02ec203cd29a3ebecbc093d52315b66d0"
-dependencies = [
- "windows-targets 0.42.2",
-]
-
-[[package]]
-name = "windows-sys"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "677d2418bec65e3338edb076e806bc1ec15693c5d0104683f2efe857f61056a9"
 dependencies = [
- "windows-targets 0.48.0",
-]
-
-[[package]]
-name = "windows-targets"
-version = "0.42.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8e5180c00cd44c9b1c88adb3693291f1cd93605ded80c250a75d472756b4d071"
-dependencies = [
- "windows_aarch64_gnullvm 0.42.2",
- "windows_aarch64_msvc 0.42.2",
- "windows_i686_gnu 0.42.2",
- "windows_i686_msvc 0.42.2",
- "windows_x86_64_gnu 0.42.2",
- "windows_x86_64_gnullvm 0.42.2",
- "windows_x86_64_msvc 0.42.2",
+ "windows-targets",
 ]
 
 [[package]]
 name = "windows-targets"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7b1eb6f0cd7c80c79759c929114ef071b87354ce476d9d94271031c0497adfd5"
 dependencies = [
- "windows_aarch64_gnullvm 0.48.0",
- "windows_aarch64_msvc 0.48.0",
- "windows_i686_gnu 0.48.0",
- "windows_i686_msvc 0.48.0",
- "windows_x86_64_gnu 0.48.0",
- "windows_x86_64_gnullvm 0.48.0",
- "windows_x86_64_msvc 0.48.0",
+ "windows_aarch64_gnullvm",
+ "windows_aarch64_msvc",
+ "windows_i686_gnu",
+ "windows_i686_msvc",
+ "windows_x86_64_gnu",
+ "windows_x86_64_gnullvm",
+ "windows_x86_64_msvc",
 ]
 
 [[package]]
 name = "windows_aarch64_gnullvm"
-version = "0.42.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "597a5118570b68bc08d8d59125332c54f1ba9d9adeedeef5b99b02ba2b0698f8"
-
-[[package]]
-name = "windows_aarch64_gnullvm"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "91ae572e1b79dba883e0d315474df7305d12f569b400fcf90581b06062f7e1bc"
 
 [[package]]
 name = "windows_aarch64_msvc"
-version = "0.42.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e08e8864a60f06ef0d0ff4ba04124db8b0fb3be5776a5cd47641e942e58c4d43"
-
-[[package]]
-name = "windows_aarch64_msvc"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b2ef27e0d7bdfcfc7b868b317c1d32c641a6fe4629c171b8928c7b08d98d7cf3"
 
 [[package]]
 name = "windows_i686_gnu"
-version = "0.42.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c61d927d8da41da96a81f029489353e68739737d3beca43145c8afec9a31a84f"
-
-[[package]]
-name = "windows_i686_gnu"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "622a1962a7db830d6fd0a69683c80a18fda201879f0f447f065a3b7467daa241"
 
 [[package]]
 name = "windows_i686_msvc"
-version = "0.42.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "44d840b6ec649f480a41c8d80f9c65108b92d89345dd94027bfe06ac444d1060"
-
-[[package]]
-name = "windows_i686_msvc"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4542c6e364ce21bf45d69fdd2a8e455fa38d316158cfd43b3ac1c5b1b19f8e00"
 
 [[package]]
 name = "windows_x86_64_gnu"
-version = "0.42.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8de912b8b8feb55c064867cf047dda097f92d51efad5b491dfb98f6bbb70cb36"
-
-[[package]]
-name = "windows_x86_64_gnu"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ca2b8a661f7628cbd23440e50b05d705db3686f894fc9580820623656af974b1"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
-version = "0.42.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "26d41b46a36d453748aedef1486d5c7a85db22e56aff34643984ea85514e94a3"
-
-[[package]]
-name = "windows_x86_64_gnullvm"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7896dbc1f41e08872e9d5e8f8baa8fdd2677f29468c4e156210174edc7f7b953"
 
 [[package]]
 name = "windows_x86_64_msvc"
-version = "0.42.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9aec5da331524158c6d1a4ac0ab1541149c0b9505fde06423b02f5ef0106b9f0"
-
-[[package]]
-name = "windows_x86_64_msvc"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1a515f5799fe4961cb532f983ce2b23082366b898e52ffbce459c86f67c8378a"
 
 [[package]]
 name = "winnow"
 version = "0.4.6"
```

### Comparing `polyglot_piranha-0.3.8/LICENSE` & `polyglot_piranha-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.8/README.md` & `polyglot_piranha-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.8/legacy/java/piranha/src/main/java/com/uber/piranha/EnumWithClassSymbol.java` & `polyglot_piranha-0.3.9/legacy/java/piranha/src/main/java/com/uber/piranha/EnumWithClassSymbol.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.8/legacy/java/piranha/src/main/java/com/uber/piranha/PiranhaRuntimeException.java` & `polyglot_piranha-0.3.9/legacy/java/piranha/src/main/java/com/uber/piranha/PiranhaRuntimeException.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.8/legacy/java/piranha/src/main/java/com/uber/piranha/PiranhaUtils.java` & `polyglot_piranha-0.3.9/legacy/java/piranha/src/main/java/com/uber/piranha/PiranhaUtils.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.8/legacy/java/piranha/src/main/java/com/uber/piranha/UsageCounter.java` & `polyglot_piranha-0.3.9/legacy/java/piranha/src/main/java/com/uber/piranha/UsageCounter.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.8/legacy/java/piranha/src/main/java/com/uber/piranha/XPFlagCleaner.java` & `polyglot_piranha-0.3.9/legacy/java/piranha/src/main/java/com/uber/piranha/XPFlagCleaner.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.8/legacy/java/piranha/src/main/java/com/uber/piranha/config/Config.java` & `polyglot_piranha-0.3.9/legacy/java/piranha/src/main/java/com/uber/piranha/config/Config.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.8/legacy/java/piranha/src/main/java/com/uber/piranha/config/MethodRecord.java` & `polyglot_piranha-0.3.9/legacy/java/piranha/src/main/java/com/uber/piranha/config/MethodRecord.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.8/legacy/java/piranha/src/main/java/com/uber/piranha/config/PiranhaEnumRecord.java` & `polyglot_piranha-0.3.9/legacy/java/piranha/src/main/java/com/uber/piranha/config/PiranhaEnumRecord.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.8/legacy/java/piranha/src/main/java/com/uber/piranha/config/PiranhaMethodRecord.java` & `polyglot_piranha-0.3.9/legacy/java/piranha/src/main/java/com/uber/piranha/config/PiranhaMethodRecord.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.8/legacy/java/piranha/src/main/java/com/uber/piranha/config/PiranhaRecord.java` & `polyglot_piranha-0.3.9/legacy/java/piranha/src/main/java/com/uber/piranha/config/PiranhaRecord.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.8/legacy/java/piranha/src/main/java/com/uber/piranha/testannotations/AnnotationArgument.java` & `polyglot_piranha-0.3.9/legacy/java/piranha/src/main/java/com/uber/piranha/testannotations/AnnotationArgument.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.8/legacy/java/piranha/src/main/java/com/uber/piranha/testannotations/AnnotationResolutionException.java` & `polyglot_piranha-0.3.9/legacy/java/piranha/src/main/java/com/uber/piranha/testannotations/AnnotationResolutionException.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.8/legacy/java/piranha/src/main/java/com/uber/piranha/testannotations/ResolvedTestAnnotation.java` & `polyglot_piranha-0.3.9/legacy/java/piranha/src/main/java/com/uber/piranha/testannotations/ResolvedTestAnnotation.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.8/legacy/java/piranha/src/main/java/com/uber/piranha/testannotations/TestAnnotationResolver.java` & `polyglot_piranha-0.3.9/legacy/java/piranha/src/main/java/com/uber/piranha/testannotations/TestAnnotationResolver.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.8/legacy/java/piranha/src/main/java/com/uber/piranha/testannotations/TestAnnotationSpecRecord.java` & `polyglot_piranha-0.3.9/legacy/java/piranha/src/main/java/com/uber/piranha/testannotations/TestAnnotationSpecRecord.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.8/legacy/java/piranha/src/test/java/com/uber/piranha/ConfigurationTest.java` & `polyglot_piranha-0.3.9/legacy/java/piranha/src/test/java/com/uber/piranha/ConfigurationTest.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.8/legacy/java/piranha/src/test/java/com/uber/piranha/CorePiranhaTest.java` & `polyglot_piranha-0.3.9/legacy/java/piranha/src/test/java/com/uber/piranha/CorePiranhaTest.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.8/legacy/java/piranha/src/test/java/com/uber/piranha/EnumConstantTest.java` & `polyglot_piranha-0.3.9/legacy/java/piranha/src/test/java/com/uber/piranha/EnumConstantTest.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.8/legacy/java/piranha/src/test/java/com/uber/piranha/PiranhaTestingHelpers.java` & `polyglot_piranha-0.3.9/legacy/java/piranha/src/test/java/com/uber/piranha/PiranhaTestingHelpers.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.8/legacy/java/piranha/src/test/java/com/uber/piranha/TestCaseCleanUpTest.java` & `polyglot_piranha-0.3.9/legacy/java/piranha/src/test/java/com/uber/piranha/TestCaseCleanUpTest.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.8/legacy/java/piranha/src/test/java/com/uber/piranha/TreatmentGroupsTest.java` & `polyglot_piranha-0.3.9/legacy/java/piranha/src/test/java/com/uber/piranha/TreatmentGroupsTest.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.8/legacy/java/piranha/src/test/resources/com/uber/piranha/XPFlagCleanerNegativeCases.java` & `polyglot_piranha-0.3.9/legacy/java/piranha/src/test/resources/com/uber/piranha/XPFlagCleanerNegativeCases.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.8/legacy/java/piranha/src/test/resources/com/uber/piranha/XPFlagCleanerPositiveCases.java` & `polyglot_piranha-0.3.9/legacy/java/piranha/src/test/resources/com/uber/piranha/XPFlagCleanerPositiveCases.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.8/legacy/java/piranha/src/test/resources/com/uber/piranha/XPFlagCleanerPositiveCasesControl.java` & `polyglot_piranha-0.3.9/legacy/java/piranha/src/test/resources/com/uber/piranha/XPFlagCleanerPositiveCasesControl.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.8/legacy/java/piranha/src/test/resources/com/uber/piranha/XPFlagCleanerPositiveCasesTreatment.java` & `polyglot_piranha-0.3.9/legacy/java/piranha/src/test/resources/com/uber/piranha/XPFlagCleanerPositiveCasesTreatment.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.8/legacy/java/piranha/src/test/resources/com/uber/piranha/XPMethodChainCases.java` & `polyglot_piranha-0.3.9/legacy/java/piranha/src/test/resources/com/uber/piranha/XPMethodChainCases.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.8/legacy/java/piranha/src/test/resources/com/uber/piranha/XPMethodChainCasesControl.java` & `polyglot_piranha-0.3.9/legacy/java/piranha/src/test/resources/com/uber/piranha/XPMethodChainCasesControl.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.8/legacy/java/piranha/src/test/resources/com/uber/piranha/XPMethodChainCasesDoNotAllowMethodChain.java` & `polyglot_piranha-0.3.9/legacy/java/piranha/src/test/resources/com/uber/piranha/XPMethodChainCasesDoNotAllowMethodChain.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.8/legacy/java/piranha/src/test/resources/com/uber/piranha/XPMethodChainCasesDoNotallowArgMatchingAndMethodChain.java` & `polyglot_piranha-0.3.9/legacy/java/piranha/src/test/resources/com/uber/piranha/XPMethodChainCasesDoNotallowArgMatchingAndMethodChain.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.8/legacy/java/piranha/src/test/resources/com/uber/piranha/XPMethodChainCasesTreatment.java` & `polyglot_piranha-0.3.9/legacy/java/piranha/src/test/resources/com/uber/piranha/XPMethodChainCasesTreatment.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.8/legacy/java/piranha/src/test/resources/com/uber/piranha/XPMethodChainCasesTreatmentDoNotAllowMatchingArgMethodInvc.java` & `polyglot_piranha-0.3.9/legacy/java/piranha/src/test/resources/com/uber/piranha/XPMethodChainCasesTreatmentDoNotAllowMatchingArgMethodInvc.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.8/legacy/java/piranha/src/test/resources/com/uber/piranha/XPTest.java` & `polyglot_piranha-0.3.9/legacy/java/piranha/src/test/resources/com/uber/piranha/XPTest.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.8/legacy/java/piranha/src/test/resources/config/properties_method_chain_control.json` & `polyglot_piranha-0.3.9/legacy/java/piranha/src/test/resources/config/properties_method_chain_control.json`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.8/legacy/java/piranha/src/test/resources/config/properties_method_chain_treated.json` & `polyglot_piranha-0.3.9/legacy/java/piranha/src/test/resources/config/properties_method_chain_treated.json`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.8/legacy/java/piranha/src/test/resources/config/properties_no_method_chain.json` & `polyglot_piranha-0.3.9/legacy/java/piranha/src/test/resources/config/properties_no_method_chain.json`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.8/legacy/java/piranha/src/test/resources/config/properties_test_argument.json` & `polyglot_piranha-0.3.9/legacy/java/piranha/src/test/resources/config/properties_test_argument.json`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.8/legacy/java/piranha/src/test/resources/config/properties_test_clean_by_setters_ignore_others.json` & `polyglot_piranha-0.3.9/legacy/java/piranha/src/test/resources/config/properties_test_clean_by_setters_ignore_others.json`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.8/legacy/java/piranha/src/test/resources/config/properties_test_noTreatmentGroup.json` & `polyglot_piranha-0.3.9/legacy/java/piranha/src/test/resources/config/properties_test_noTreatmentGroup.json`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.8/legacy/java/piranha/src/test/resources/config/properties_test_receive.json` & `polyglot_piranha-0.3.9/legacy/java/piranha/src/test/resources/config/properties_test_receive.json`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.8/legacy/java/piranha/src/test/resources/config/properties_test_receive_argument.json` & `polyglot_piranha-0.3.9/legacy/java/piranha/src/test/resources/config/properties_test_receive_argument.json`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.8/legacy/java/piranha/src/test/resources/config/properties_test_return.json` & `polyglot_piranha-0.3.9/legacy/java/piranha/src/test/resources/config/properties_test_return.json`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.8/legacy/java/piranha/src/test/resources/config/properties_test_return_argument.json` & `polyglot_piranha-0.3.9/legacy/java/piranha/src/test/resources/config/properties_test_return_argument.json`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.8/legacy/java/piranha/src/test/resources/config/properties_test_return_receive.json` & `polyglot_piranha-0.3.9/legacy/java/piranha/src/test/resources/config/properties_test_return_receive.json`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.8/legacy/java/piranha/src/test/resources/config/properties_test_return_receive_argument.json` & `polyglot_piranha-0.3.9/legacy/java/piranha/src/test/resources/config/properties_test_return_receive_argument.json`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.8/legacy/java/piranha/src/test/resources/config/properties_unnecessary_instance_method.json` & `polyglot_piranha-0.3.9/legacy/java/piranha/src/test/resources/config/properties_unnecessary_instance_method.json`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.8/legacy/java/sample/src/main/java/com/uber/mylib/MyClass.java` & `polyglot_piranha-0.3.9/legacy/java/sample/src/main/java/com/uber/mylib/MyClass.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.8/legacy/java/sample/src/main/resources/com/uber/mylib/MyClass.bak` & `polyglot_piranha-0.3.9/legacy/java/sample/src/main/resources/com/uber/mylib/MyClass.bak`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.8/legacy/java/sample/src/main/resources/com/uber/mylib/MyClass.expect` & `polyglot_piranha-0.3.9/legacy/java/sample/src/main/resources/com/uber/mylib/MyClass.expect`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.8/legacy/javascript/src/config_checker.js` & `polyglot_piranha-0.3.9/legacy/javascript/src/config_checker.js`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.8/legacy/javascript/src/piranha.js` & `polyglot_piranha-0.3.9/legacy/javascript/src/piranha.js`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.8/legacy/javascript/src/refactor.js` & `polyglot_piranha-0.3.9/legacy/javascript/src/refactor.js`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.8/legacy/javascript/src/source_checker.js` & `polyglot_piranha-0.3.9/legacy/javascript/src/source_checker.js`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.8/legacy/objc/src/XPFlagRefactoring/CMakeLists.txt` & `polyglot_piranha-0.3.9/legacy/objc/src/XPFlagRefactoring/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.8/legacy/objc/src/XPFlagRefactoring/README.txt` & `polyglot_piranha-0.3.9/legacy/objc/src/XPFlagRefactoring/README.txt`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.8/legacy/objc/src/XPFlagRefactoring/XPFlagRefactoring.cpp` & `polyglot_piranha-0.3.9/legacy/objc/src/XPFlagRefactoring/XPFlagRefactoring.cpp`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.8/pyproject.toml` & `polyglot_piranha-0.3.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.8/src/cleanup_rules/go/edges.toml` & `polyglot_piranha-0.3.9/src/cleanup_rules/go/edges.toml`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.8/src/cleanup_rules/go/rules.toml` & `polyglot_piranha-0.3.9/src/cleanup_rules/go/rules.toml`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.8/src/cleanup_rules/go/scope_config.toml` & `polyglot_piranha-0.3.9/src/cleanup_rules/go/scope_config.toml`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.8/src/cleanup_rules/java/edges.toml` & `polyglot_piranha-0.3.9/src/cleanup_rules/java/edges.toml`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.8/src/cleanup_rules/java/rules.toml` & `polyglot_piranha-0.3.9/src/cleanup_rules/java/rules.toml`

 * *Files 2% similar despite different names*

```diff
@@ -439,14 +439,35 @@
         (block  ((statement)* @pre)
          ((return_statement) @r)
          ((statement)+ @post)) @b)"""
 replace = ""
 replace_node = "post"
 is_seed_rule = false
 
+
+# Before :
+#  condition ? abc() : abc();
+# After :
+#  abc()
+#
+[[rules]]
+groups = ["if_cleanup"]
+name = "simplify_ternary_similar_consequent_alternative"
+query = """
+(
+    (ternary_expression condition: (_)
+        consequence: (_)* @consequence
+        alternative: (_)* @alternative)
+@ternary_expression
+(#eq? @consequence @alternative)
+)"""
+replace = "@consequence"
+replace_node = "ternary_expression"
+is_seed_rule = false
+
 # Before :
 #  true ? abc() : def();
 # After :
 #  abc()
 #
 [[rules]]
 groups = ["if_cleanup"]
```

### Comparing `polyglot_piranha-0.3.8/src/cleanup_rules/java/scope_config.toml` & `polyglot_piranha-0.3.9/src/cleanup_rules/java/scope_config.toml`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.8/src/cleanup_rules/kt/edges.toml` & `polyglot_piranha-0.3.9/src/cleanup_rules/kt/edges.toml`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.8/src/cleanup_rules/kt/rules.toml` & `polyglot_piranha-0.3.9/src/cleanup_rules/kt/rules.toml`

 * *Files 0% similar despite different names*

```diff
@@ -193,15 +193,15 @@
 [[rules]]
 groups = ["boolean_expression_simplify"]
 name = "simplify_not_false"
 query = """
 (
 (prefix_expression (boolean_literal) @exp) @prefix_expression
 (#eq? @exp "false")
-(#match @prefix_expression "!.*")  
+(#match? @prefix_expression "!.*")  
 )
 """
 replace = "true"
 replace_node = "prefix_expression"
 is_seed_rule = false
 
 # Before : 
@@ -212,15 +212,15 @@
 [[rules]]
 groups = ["boolean_expression_simplify"]
 name = "simplify_not_true"
 query = """
 (
 (prefix_expression (boolean_literal) @exp) @prefix_expression
 (#eq? @exp "true")
-(#match @prefix_expression "!.*")  
+(#match? @prefix_expression "!.*")  
 )
 """
 replace = "false"
 replace_node = "prefix_expression"
 is_seed_rule = false
 
 # Before :
```

### Comparing `polyglot_piranha-0.3.8/src/cleanup_rules/kt/scope_config.toml` & `polyglot_piranha-0.3.9/src/cleanup_rules/kt/scope_config.toml`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.8/src/cleanup_rules/swift/edges.toml` & `polyglot_piranha-0.3.9/src/cleanup_rules/swift/edges.toml`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.8/src/cleanup_rules/swift/rules.toml` & `polyglot_piranha-0.3.9/src/cleanup_rules/swift/rules.toml`

 * *Files 2% similar despite different names*

```diff
@@ -467,14 +467,37 @@
 (#eq? @true "true")
 )"""
 groups = ["guard_cleanup"]
 replace_node = "guard_block"
 replace = ""
 is_seed_rule = false
 
+
+#
+# Before
+# var v = true ? x : x
+#
+# After
+# var v = x
+#
+[[rules]]
+name = "ternary_similar_consequent_alternative"
+query = """(
+(ternary_expression
+    if_true:(_) @block_true
+    if_false:(_) @block_false
+    ) @ternary_block
+(#eq? @block_true @block_false)
+)"""
+groups = ["if_cleanup"]
+replace_node = "ternary_block"
+replace = "@block_true"
+is_seed_rule = false
+
+
 #
 # Before
 # var v = true ? x : y
 #
 # After
 # var v = x
 #
```

### Comparing `polyglot_piranha-0.3.8/src/cleanup_rules/swift/scope_config.toml` & `polyglot_piranha-0.3.9/src/cleanup_rules/swift/scope_config.toml`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.8/src/lib.rs` & `polyglot_piranha-0.3.9/src/lib.rs`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,14 @@
 mod tests;
 pub mod utilities;
 
 use std::{collections::HashMap, fs::File, io::Write, path::PathBuf};
 
 use itertools::Itertools;
 use log::{debug, info};
-use tree_sitter::Parser;
 
 use crate::models::rule_store::RuleStore;
 
 use pyo3::prelude::{pyfunction, pymodule, wrap_pyfunction, PyModule, PyResult, Python};
 use tempdir::TempDir;
 
 #[pymodule]
@@ -107,19 +106,17 @@
       .cloned()
       .collect_vec()
   }
 
   /// Performs cleanup related to stale flags
   fn perform_cleanup(&mut self) {
     // Setup the parser for the specific language
-    let mut parser = Parser::new();
     let piranha_args = &self.piranha_arguments;
-    parser
-      .set_language(*piranha_args.language().language())
-      .expect("Could not set the language for the parser.");
+
+    let mut parser = piranha_args.language().parser();
 
     let mut path_to_codebase = self.piranha_arguments.path_to_codebase().to_string();
 
     let temp_dir = if !self.piranha_arguments.code_snippet().is_empty() {
       let td = self.write_code_snippet_to_temp();
       path_to_codebase = td.path().to_str().unwrap_or_default().to_string();
       Some(td)
```

### Comparing `polyglot_piranha-0.3.8/src/main.rs` & `polyglot_piranha-0.3.9/src/main.rs`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.8/src/models/default_configs.rs` & `polyglot_piranha-0.3.9/src/models/default_configs.rs`

 * *Files 2% similar despite different names*

```diff
@@ -147,14 +147,18 @@
   1
 }
 
 pub(crate) fn default_contains_at_most() -> u32 {
   u32::MAX
 }
 
+pub(crate) fn default_child_count() -> u32 {
+  u32::MAX
+}
+
 pub(crate) fn default_enclosing_node() -> TSQuery {
   TSQuery::new(String::new())
 }
 
 pub(crate) fn default_not_enclosing_node() -> TSQuery {
   TSQuery::new(String::new())
 }
```

### Comparing `polyglot_piranha-0.3.8/src/models/edit.rs` & `polyglot_piranha-0.3.9/src/models/edit.rs`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.8/src/models/filter.rs` & `polyglot_piranha-0.3.9/src/models/filter.rs`

 * *Files 7% similar despite different names*

```diff
@@ -22,15 +22,18 @@
 use tree_sitter::Node;
 
 use crate::utilities::{
   gen_py_str_methods,
   tree_sitter_utilities::{get_all_matches_for_query, get_match_for_query, get_node_for_range},
 };
 
-use super::{rule::InstantiatedRule, rule_store::RuleStore, source_code_unit::SourceCodeUnit};
+use super::{
+  default_configs::default_child_count, rule::InstantiatedRule, rule_store::RuleStore,
+  source_code_unit::SourceCodeUnit, Validator,
+};
 
 use crate::utilities::{tree_sitter_utilities::TSQuery, Instantiate};
 
 use super::default_configs::{
   default_contains_at_least, default_contains_at_most, default_contains_query,
   default_enclosing_node, default_not_contains_queries, default_not_enclosing_node,
 };
@@ -71,83 +74,122 @@
   at_least: u32,
   /// Most number of matches we should find for the contains query
   #[builder(default = "default_contains_at_most()")]
   #[get = "pub"]
   #[serde(default = "default_contains_at_most")]
   #[pyo3(get)]
   at_most: u32,
+
+  // number of named children under the primary matched node
+  #[builder(default = "default_contains_at_most()")]
+  #[get = "pub"]
+  #[serde(default = "default_contains_at_most")]
+  #[pyo3(get)]
+  child_count: u32,
 }
 
 #[pymethods]
 impl Filter {
   #[new]
   fn py_new(
     enclosing_node: Option<String>, not_enclosing_node: Option<String>,
     not_contains: Option<Vec<String>>, contains: Option<String>, at_least: Option<u32>,
-    at_most: Option<u32>,
+    at_most: Option<u32>, child_count: Option<u32>,
   ) -> Self {
     FilterBuilder::default()
       .enclosing_node(TSQuery::new(enclosing_node.unwrap_or_default()))
       .not_enclosing_node(TSQuery::new(not_enclosing_node.unwrap_or_default()))
       .not_contains(
         not_contains
           .unwrap_or_default()
           .iter()
           .map(|x| TSQuery::new(x.to_string()))
           .collect_vec(),
       )
       .contains(TSQuery::new(contains.unwrap_or_default()))
       .at_least(at_least.unwrap_or(default_contains_at_least()))
       .at_most(at_most.unwrap_or(default_contains_at_most()))
+      .child_count(child_count.unwrap_or(default_child_count()))
       .build()
   }
   gen_py_str_methods!();
 }
 
-impl FilterBuilder {
-  /// Builds Filter from FilterBuilder
-  /// * create Filter from the builder
-  /// * validates new argument combinations
-  pub fn build(&self) -> Filter {
-    match &self._validate() {
-      Ok(filter) => filter.clone(),
-      Err(e) => panic!("Invalid filter - {}", e),
-    }
-  }
-
-  fn _validate(&self) -> Result<Filter, String> {
-    let _filter: Filter = self.create().unwrap();
-
+impl Validator for Filter {
+  fn validate(&self) -> Result<(), String> {
     // Only allow users to set either contains or not_contains, but not both
-    if !_filter.contains().get_query().is_empty() && !_filter.not_contains().is_empty() {
+    if *self.contains() != default_contains_query()
+      && *self.not_contains() != default_not_contains_queries()
+    {
       return Err(
         "Invalid Filter Argument. `contains` and `not_contains` cannot be set at the same time !!! Please use two filters instead."
           .to_string(),
       );
     }
 
-    if _filter.at_least > _filter.at_most {
+    if self.at_least > self.at_most {
       return Err(
         "Invalid Filter Argument. `at_least` should be less than or equal to `at_most` !!!"
           .to_string(),
       );
     }
 
     // If the user set `at_least` or `at_most`, then the contains query cannot be empty
-    if (_filter.at_least != default_contains_at_least()
-      || _filter.at_most != default_contains_at_most())
-      && _filter.contains().get_query().is_empty()
+    if (self.at_least != default_contains_at_least() || self.at_most != default_contains_at_most())
+      && self.contains().get_query().is_empty()
     {
       return Err(
         "Invalid Filter Argument. `at_least` or `at_most` is set, but `contains` is empty !!!"
           .to_string(),
       );
     }
 
-    Ok(_filter)
+    if *self.enclosing_node() != default_enclosing_node() {
+      self.enclosing_node().validate()?
+    }
+
+    if *self.not_enclosing_node() != default_not_enclosing_node() {
+      self.not_enclosing_node().validate()?
+    }
+
+    if *self.contains() != default_contains_query() {
+      self.contains().validate()?
+    }
+
+    if *self.not_contains() != default_not_contains_queries() {
+      self.not_contains().iter().try_for_each(|x| x.validate())?
+    }
+
+    if *self.child_count() != default_child_count()
+      && (*self.enclosing_node() != default_enclosing_node()
+        || *self.not_enclosing_node() != default_not_enclosing_node()
+        || *self.contains() != default_contains_query()
+        || *self.not_contains() != default_not_contains_queries())
+    {
+      return Err("The child count operator is not compatible with (not) enclosing node and (not) contains operator".to_string());
+    }
+
+    Ok(())
+  }
+}
+
+impl FilterBuilder {
+  /// Builds Filter from FilterBuilder
+  /// * create Filter from the builder
+  /// * validates new argument combinations
+  pub fn build(&self) -> Filter {
+    match &self._validate() {
+      Ok(filter) => filter.clone(),
+      Err(e) => panic!("Invalid filter - {}", e),
+    }
+  }
+
+  fn _validate(&self) -> Result<Filter, String> {
+    let _filter: Filter = self.create().unwrap();
+    _filter.validate().map(|_| _filter)
   }
 }
 
 #[macro_export]
 /// This macro constructs a FilterBuilder for creating filter queries. It provides a more "dynamic" way to use the builder pattern.
 ///
 /// 'enclosing_node' is an optional parameter that specifies the node to be inspected. If it is not provided
@@ -184,22 +226,23 @@
 ///      .contains(TSQuery::new("(parameter_list)"))
 ///      .at_least(1)
 ///      .at_most(10)
 ///      .build().unwrap()
 /// ```
 ///
 macro_rules! filter {
-  ($(enclosing_node = $enclosing_node:expr)? $(, not_enclosing_node=$not_enclosing_node:expr)? $(, not_contains= [$($q:expr,)*])? $(, contains= $p:expr)? $(, at_least=$min:expr)? $(, at_most=$max:expr)?) => {
+  ($(enclosing_node = $enclosing_node:expr)? $(, not_enclosing_node=$not_enclosing_node:expr)? $(, not_contains= [$($q:expr,)*])? $(, contains= $p:expr)? $(, at_least=$min:expr)? $(, at_most=$max:expr)? $(, child_count=$nChildren:expr)?) => {
     $crate::models::filter::FilterBuilder::default()
       $(.enclosing_node($crate::utilities::tree_sitter_utilities::TSQuery::new($enclosing_node.to_string())))?
       $(.not_enclosing_node($crate::utilities::tree_sitter_utilities::TSQuery::new($not_enclosing_node.to_string())))?
       $(.not_contains(vec![$($crate::utilities::tree_sitter_utilities::TSQuery::new($q.to_string()),)*]))?
       $(.contains($crate::utilities::tree_sitter_utilities::TSQuery::new($p.to_string())))?
       $(.at_least($min))?
       $(.at_most($max))?
+      $(.child_count($nChildren))?
       .build()
   };
 }
 
 pub use filter;
 
 impl Instantiate for Filter {
@@ -214,14 +257,15 @@
         .not_contains()
         .iter()
         .map(|x| x.instantiate(substitutions_for_holes))
         .collect_vec(),
       contains: self.contains().instantiate(substitutions_for_holes),
       at_least: self.at_least,
       at_most: self.at_most,
+      child_count: self.child_count,
     }
   }
 }
 
 // Implements instance methods related to applying a filter
 impl SourceCodeUnit {
   pub(crate) fn is_satisfied(
@@ -252,14 +296,18 @@
   fn _check(
     &self, filter: Filter, node: Node, rule_store: &mut RuleStore,
     substitutions: &HashMap<String, String>,
   ) -> bool {
     let mut node_to_check = node;
     let instantiated_filter = filter.instantiate(substitutions);
 
+    if *filter.child_count() != default_child_count() {
+      return node.named_child_count() == (*filter.child_count() as usize);
+    }
+
     // Check if no ancestor matches the query for not_enclosing_node
     if !self._check_not_enclosing_node(rule_store, node_to_check, &instantiated_filter) {
       return false;
     }
     // If an enclosing node is provided
     let query = instantiated_filter.enclosing_node();
     if !query.get_query().is_empty() {
```

### Comparing `polyglot_piranha-0.3.8/src/models/language.rs` & `polyglot_piranha-0.3.9/src/models/language.rs`

 * *Files 1% similar despite different names*

```diff
@@ -159,15 +159,15 @@
           supported_language: SupportedLanguage::Kotlin,
           language: tree_sitter_kotlin::language(),
           rules: Some(rules),
           edges: Some(edges),
           scopes: parse_toml::<ScopeConfig>(include_str!("../cleanup_rules/kt/scope_config.toml"))
             .scopes()
             .to_vec(),
-          comment_nodes: vec!["comment".to_string()],
+          comment_nodes: vec!["comment".to_string(), "line_comment".to_string()],
         })
       }
       PYTHON => Ok(PiranhaLanguage {
         extension: language.to_string(),
         supported_language: SupportedLanguage::Python,
         language: tree_sitter_python::language(),
         rules: None,
```

### Comparing `polyglot_piranha-0.3.8/src/models/matches.rs` & `polyglot_piranha-0.3.9/src/models/matches.rs`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.8/src/models/mod.rs` & `polyglot_piranha-0.3.9/src/models/mod.rs`

 * *Files 11% similar despite different names*

```diff
@@ -20,7 +20,11 @@
 pub mod piranha_arguments;
 pub mod piranha_output;
 pub(crate) mod rule;
 pub(crate) mod rule_graph;
 pub(crate) mod rule_store;
 pub(crate) mod scopes;
 pub(crate) mod source_code_unit;
+
+pub(crate) trait Validator {
+  fn validate(&self) -> Result<(), String>;
+}
```

### Comparing `polyglot_piranha-0.3.8/src/models/outgoing_edges.rs` & `polyglot_piranha-0.3.9/src/models/outgoing_edges.rs`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.8/src/models/piranha_arguments.rs` & `polyglot_piranha-0.3.9/src/models/piranha_arguments.rs`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.8/src/models/piranha_output.rs` & `polyglot_piranha-0.3.9/src/models/piranha_output.rs`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.8/src/models/rule.rs` & `polyglot_piranha-0.3.9/src/models/rule.rs`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 
 use super::{
   default_configs::{
     default_filters, default_groups, default_holes, default_is_seed_rule, default_query,
     default_replace, default_replace_node, default_rule_name,
   },
   filter::Filter,
+  Validator,
 };
 
 #[derive(Deserialize, Debug, Clone, Default, PartialEq)]
 // Represents the `rules.toml` file
 pub(crate) struct Rules {
   pub(crate) rules: Vec<Rule>,
 }
@@ -144,20 +145,25 @@
   };
 }
 
 #[pymethods]
 impl Rule {
   #[new]
   fn py_new(
-    name: String, query: String, replace: Option<String>, replace_node: Option<String>,
+    name: String, query: Option<String>, replace: Option<String>, replace_node: Option<String>,
     holes: Option<HashSet<String>>, groups: Option<HashSet<String>>,
     filters: Option<HashSet<Filter>>, is_seed_rule: Option<bool>,
   ) -> Self {
     let mut rule_builder = RuleBuilder::default();
-    rule_builder.name(name).query(TSQuery::new(query));
+
+    rule_builder.name(name);
+    if let Some(q) = query {
+      rule_builder.query(TSQuery::new(q));
+    }
+
     if let Some(replace) = replace {
       rule_builder.replace(replace);
     }
 
     if let Some(replace_node) = replace_node {
       rule_builder.replace_node(replace_node);
     }
@@ -180,14 +186,24 @@
 
     rule_builder.build().unwrap()
   }
 
   gen_py_str_methods!();
 }
 
+impl Validator for Rule {
+  fn validate(&self) -> Result<(), String> {
+    let validation = self
+      .query()
+      .validate()
+      .and_then(|_: ()| self.filters().iter().try_for_each(|f| f.validate()));
+    validation
+  }
+}
+
 pub use piranha_rule;
 
 #[derive(Debug, Getters, Clone)]
 pub(crate) struct InstantiatedRule {
   #[get = "pub"]
   rule: Rule,
   #[get = "pub"]
```

### Comparing `polyglot_piranha-0.3.8/src/models/rule_graph.rs` & `polyglot_piranha-0.3.9/src/models/rule_graph.rs`

 * *Files 7% similar despite different names*

```diff
@@ -7,28 +7,29 @@
 
  <p>Unless required by applicable law or agreed to in writing, software distributed under the
  License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either
  express or implied. See the License for the specific language governing permissions and
  limitations under the License.
 */
 
-use derive_builder::Builder;
-use getset::{Getters, MutGetters};
-use itertools::Itertools;
-
 use crate::{
   models::{outgoing_edges::OutgoingEdges, rule::Rule},
   utilities::{gen_py_str_methods, read_toml, MapOfVec},
 };
+use colored::Colorize;
+use derive_builder::Builder;
+use getset::{Getters, MutGetters};
+use itertools::Itertools;
 use std::{collections::HashMap, path::Path};
 
 use super::{
   default_configs::{default_edges, default_rule_graph_map, default_rules},
   outgoing_edges::Edges,
   rule::{InstantiatedRule, Rules},
+  Validator,
 };
 use pyo3::prelude::{pyclass, pymethods};
 
 pub(crate) static GLOBAL: &str = "Global";
 pub(crate) static PARENT: &str = "Parent";
 
 #[derive(Debug, Default, Getters, MutGetters, Builder, Clone, PartialEq)]
@@ -50,14 +51,23 @@
   /// The graph itself
   #[builder(default = "default_rule_graph_map()")]
   #[get = "pub(crate)"]
   #[pyo3(get)]
   graph: HashMap<String, Vec<(String, String)>>,
 }
 
+impl Validator for RuleGraph {
+  fn validate(&self) -> Result<(), String> {
+    match self.rules().iter().try_for_each(|rule| rule.validate()) {
+      Ok(()) => Ok(()),
+      Err(e) => Err(format!("Incorrect Rule Graph - {}", e)),
+    }
+  }
+}
+
 #[pymethods]
 impl RuleGraph {
   #[new]
   fn py_new(rules: Vec<Rule>, edges: Vec<OutgoingEdges>) -> Self {
     RuleGraphBuilder::default()
       .rules(rules)
       .edges(edges)
@@ -88,20 +98,26 @@
               (edge.get_scope().to_string(), to_rule.to_string()),
             );
           }
         }
       }
     }
 
-    RuleGraphBuilder::default()
+    let graph = RuleGraphBuilder::default()
       .edges(_rule_graph.edges().clone())
       .rules(_rule_graph.rules().clone())
       .graph(graph)
       .create()
-      .unwrap()
+      .unwrap();
+
+    if let Err(err) = graph.validate() {
+      panic!("{}", err.as_str().red());
+    }
+
+    graph
   }
 }
 
 impl RuleGraph {
   /// Get all the outgoing edges for `rule_name`
   pub(crate) fn get_neighbors(&self, rule_name: &String) -> Vec<(String, String)> {
     self.graph.get(rule_name).cloned().unwrap_or_default()
@@ -185,7 +201,11 @@
   let input_rules: Rules = read_toml(&path_to_config.join("rules.toml"), true);
   let input_edges: Edges = read_toml(&path_to_config.join("edges.toml"), true);
   RuleGraphBuilder::default()
     .rules(input_rules.rules)
     .edges(input_edges.edges)
     .build()
 }
+
+#[cfg(test)]
+#[path = "unit_tests/rule_graph_validation_test.rs"]
+mod rule_graph_validation_test;
```

### Comparing `polyglot_piranha-0.3.8/src/models/rule_store.rs` & `polyglot_piranha-0.3.9/src/models/rule_store.rs`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.8/src/models/scopes.rs` & `polyglot_piranha-0.3.9/src/models/scopes.rs`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.8/src/models/source_code_unit.rs` & `polyglot_piranha-0.3.9/src/models/source_code_unit.rs`

 * *Files 1% similar despite different names*

```diff
@@ -16,20 +16,20 @@
 };
 
 use colored::Colorize;
 use itertools::Itertools;
 use log::{debug, error};
 
 use tree_sitter::{InputEdit, Node, Parser, Range, Tree};
-use tree_sitter_traversal::{traverse, Order};
 
 use crate::{
   models::rule_graph::{GLOBAL, PARENT},
   utilities::tree_sitter_utilities::{
-    get_match_for_query, get_node_for_range, get_replace_range, get_tree_sitter_edit, TSQuery,
+    get_match_for_query, get_node_for_range, get_replace_range, get_tree_sitter_edit,
+    number_of_errors, TSQuery,
   },
 };
 
 use super::{
   edit::Edit, matches::Match, piranha_arguments::PiranhaArguments, rule::InstantiatedRule,
   rule_store::RuleStore,
 };
@@ -354,19 +354,17 @@
     let msg = format!(
       "Produced syntactically incorrect source code {}",
       self.code()
     );
     panic!("{}", msg);
   }
 
-  /// Returns the number of errors in the AST
+  /// Returns the number of errors in this source code unit
   fn _number_of_errors(&self) -> usize {
-    traverse(self.root_node().walk(), Order::Post)
-      .filter(|node| node.is_error() || node.is_missing())
-      .count()
+    number_of_errors(&self.root_node())
   }
 
   // Replaces the content of the current file with the new content and re-parses the AST
   /// # Arguments
   /// * `replacement_content` - new content of file
   /// * `parser`
   /// * `is_current_ast_edited` : have you invoked `edit` on the current AST ?
```

### Comparing `polyglot_piranha-0.3.8/src/models/unit_tests/piranha_arguments_test.rs` & `polyglot_piranha-0.3.9/src/models/unit_tests/piranha_arguments_test.rs`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.8/src/models/unit_tests/rule_test.rs` & `polyglot_piranha-0.3.9/src/models/unit_tests/rule_test.rs`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,29 @@
+use tree_sitter::Point;
+
 /*
 Copyright (c) 2023 Uber Technologies, Inc.
 
  <p>Licensed under the Apache License, Version 2.0 (the "License"); you may not use this file
  except in compliance with the License. You may obtain a copy of the License at
  <p>http://www.apache.org/licenses/LICENSE-2.0
 
  <p>Unless required by applicable law or agreed to in writing, software distributed under the
  License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either
  express or implied. See the License for the specific language governing permissions and
  limitations under the License.
 */
 use crate::{
   filter,
-  models::{default_configs::UNUSED_CODE_PATH, piranha_arguments::PiranhaArgumentsBuilder},
+  models::{
+    default_configs::{JAVA, UNUSED_CODE_PATH},
+    filter::Filter,
+    language::PiranhaLanguage,
+    piranha_arguments::PiranhaArgumentsBuilder,
+  },
   utilities::eq_without_whitespace,
 };
 
 use super::InstantiatedRule;
 use {
   crate::models::{rule_store::RuleStore, source_code_unit::SourceCodeUnit},
   std::collections::HashMap,
@@ -261,7 +268,82 @@
     &args,
   );
   let edit =
     source_code_unit.get_edit_for_context(29_usize, 33_usize, &mut rule_store, &vec![rule]);
   // let edit = rule.get_edit(&source_code_unit, &mut rule_store, node, true);
   assert!(edit.is_none());
 }
+
+// Tests for not_enclosing_node
+fn run_test_satisfies_filters_not_enclosing_node(
+  filter: Filter, // Replace with the filter to test
+  assertion: fn(bool) -> bool,
+) {
+  let _rule = piranha_rule! {
+    name= "test",
+    query= "(
+      ((local_variable_declaration
+                      declarator: (variable_declarator
+                                          name: (_) @variable_name
+                                          )) @variable_declaration)
+      )",
+    replace_node= "variable_declaration",
+    replace= "",
+    filters= [filter,]
+  };
+  let rule = InstantiatedRule::new(&_rule, &HashMap::new());
+  let source_code = "class Test {
+      public void foobar(){
+        if (isFlagTreated) {
+          int testNumber = 0;
+        }
+       }
+      }";
+
+  let mut rule_store = RuleStore::default();
+  let java = PiranhaLanguage::from(JAVA);
+  let mut parser = java.parser();
+  let piranha_args = PiranhaArgumentsBuilder::default()
+    .path_to_codebase(UNUSED_CODE_PATH.to_string())
+    .language(java)
+    .build();
+  let source_code_unit = SourceCodeUnit::new(
+    &mut parser,
+    source_code.to_string(),
+    &HashMap::new(),
+    PathBuf::new().as_path(),
+    &piranha_args,
+  );
+
+  let start = Point::new(3, 10);
+  let end = Point::new(3, 29);
+  let node = &source_code_unit
+    .root_node()
+    .descendant_for_point_range(start, end)
+    .unwrap();
+
+  let map: HashMap<String, String> = HashMap::new();
+  assert!(assertion(source_code_unit.is_satisfied(
+    *node,
+    &rule,
+    &map,
+    &mut rule_store,
+  )));
+}
+
+#[test]
+fn test_satisfies_filter_not_enclosing_node_positive() {
+  run_test_satisfies_filters_not_enclosing_node(
+    filter! {,
+    not_enclosing_node = "(if_statement) @if_stmt"},
+    |result| !result,
+  );
+}
+
+#[test]
+fn test_satisfies_filter_not_enclosing_node_negative() {
+  run_test_satisfies_filters_not_enclosing_node(
+    filter! {,
+    not_enclosing_node = "(while_statement ) @while"},
+    |result| result,
+  );
+}
```

### Comparing `polyglot_piranha-0.3.8/src/models/unit_tests/scopes_test.rs` & `polyglot_piranha-0.3.9/src/models/unit_tests/scopes_test.rs`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.8/src/models/unit_tests/source_code_unit_test.rs` & `polyglot_piranha-0.3.9/src/models/unit_tests/source_code_unit_test.rs`

 * *Files 5% similar despite different names*

```diff
@@ -9,16 +9,14 @@
  License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either
  express or implied. See the License for the specific language governing permissions and
  limitations under the License.
 */
 
 use tree_sitter::{Parser, Point};
 
-use crate::models::filter::FilterBuilder;
-use crate::utilities::tree_sitter_utilities::TSQuery;
 use crate::{
   filter,
   models::{
     default_configs::{JAVA, UNUSED_CODE_PATH},
     filter::Filter,
     language::PiranhaLanguage,
     piranha_arguments::PiranhaArgumentsBuilder,
@@ -406,14 +404,83 @@
       ("variable_name".to_string(), "isFlagTreated".to_string()),
       ("init".to_string(), "true".to_string())
     ]),
     &mut rule_store,
   ));
 }
 
+#[test]
+fn test_satisfies_filters_child_count() {
+  let rule_positive = piranha_rule! {
+    name= "test",
+    query= "(
+      (method_invocation 
+          name: (_) @name
+          arguments: (argument_list)@args) @mi 
+      (#eq? @name \"someOtherFunction\")
+      )",
+    replace_node= "args",
+    replace= "()",
+    filters= [filter!{
+      , child_count = 3
+    }]
+  };
+  let rule_positive = InstantiatedRule::new(&rule_positive, &HashMap::new());
+
+  let rule_neg = piranha_rule! {
+    name= "test",
+    query= "(
+      (method_invocation 
+          name: (_) @name
+          arguments: (argument_list)@args) @mi 
+      (#eq? @name \"someOtherFunction\")
+      )",
+    replace_node= "args",
+    replace= "()",
+    filters= [filter!{
+      , child_count = 2
+    }]
+  };
+  let rule_neg = InstantiatedRule::new(&rule_neg, &HashMap::new());
+
+  let source_code = "class Test {
+      public void foobar(){
+        boolean isFlagTreated = true;
+        isFlagTreated = false;
+        if (isFlagTreated) {
+          someOtherFunction(1, 2, 3);
+        }
+       }
+      }";
+
+  let mut rule_store = RuleStore::default();
+  let java = get_java_tree_sitter_language();
+  let mut parser = java.parser();
+  let piranha_arguments = &PiranhaArgumentsBuilder::default()
+    .path_to_codebase(UNUSED_CODE_PATH.to_string())
+    .language(java)
+    .build();
+  let source_code_unit = SourceCodeUnit::new(
+    &mut parser,
+    source_code.to_string(),
+    &HashMap::new(),
+    PathBuf::new().as_path(),
+    piranha_arguments,
+  );
+
+  let node = &source_code_unit
+    .root_node()
+    .descendant_for_byte_range(167, 175)
+    .unwrap();
+
+  assert!(source_code_unit.is_satisfied(*node, &rule_positive, &HashMap::new(), &mut rule_store,));
+
+  assert!(!source_code_unit.is_satisfied(*node, &rule_neg, &HashMap::new(), &mut rule_store,));
+}
+
 // Tests for contains without providing an enclosing node
 fn run_test_satisfies_filters_without_enclosing(
   filter: Filter, // Replace with the filter to test
   assertion: fn(bool) -> bool,
 ) {
   let _rule = piranha_rule! {
       name= "test",
@@ -489,121 +556,7 @@
                       name: (identifier) @inv) @md
                    (#eq? @inv \"@method_name\")
                       )",
     at_least =2},
     |result| result,
   );
 }
-
-// Tests for not_enclosing_node
-fn run_test_satisfies_filters_not_enclosing_node(
-  filter: Filter, // Replace with the filter to test
-  assertion: fn(bool) -> bool,
-) {
-  let _rule = piranha_rule! {
-    name= "test",
-    query= "(
-      ((local_variable_declaration
-                      declarator: (variable_declarator
-                                          name: (_) @variable_name
-                                          )) @variable_declaration)
-      )",
-    replace_node= "variable_declaration",
-    replace= "",
-    filters= [filter,]
-  };
-  let rule = InstantiatedRule::new(&_rule, &HashMap::new());
-  let source_code = "class Test {
-      public void foobar(){
-        if (isFlagTreated) {
-          int testNumber = 0;
-        }
-       }
-      }";
-
-  let mut rule_store = RuleStore::default();
-  let java = get_java_tree_sitter_language();
-  let mut parser = java.parser();
-  let piranha_args = PiranhaArgumentsBuilder::default()
-    .path_to_codebase(UNUSED_CODE_PATH.to_string())
-    .language(java)
-    .build();
-  let source_code_unit = SourceCodeUnit::new(
-    &mut parser,
-    source_code.to_string(),
-    &HashMap::new(),
-    PathBuf::new().as_path(),
-    &piranha_args,
-  );
-
-  let start = Point::new(3, 10);
-  let end = Point::new(3, 29);
-  let node = &source_code_unit
-    .root_node()
-    .descendant_for_point_range(start, end)
-    .unwrap();
-
-  let map: HashMap<String, String> = HashMap::new();
-  assert!(assertion(source_code_unit.is_satisfied(
-    *node,
-    &rule,
-    &map,
-    &mut rule_store,
-  )));
-}
-
-#[test]
-fn test_satisfies_filter_not_enclosing_node_positive() {
-  run_test_satisfies_filters_not_enclosing_node(
-    filter! {,
-    not_enclosing_node = "(if_statement) @if_stmt"},
-    |result| !result,
-  );
-}
-
-#[test]
-fn test_satisfies_filter_not_enclosing_node_negative() {
-  run_test_satisfies_filters_not_enclosing_node(
-    filter! {,
-    not_enclosing_node = "(while_statement ) @while"},
-    |result| result,
-  );
-}
-
-#[test]
-#[should_panic(
-  expected = "Invalid Filter Argument. `at_least` or `at_most` is set, but `contains` is empty !!!"
-)]
-fn test_filter_bad_arg_at_least() {
-  FilterBuilder::default().at_least(2).build();
-}
-
-#[test]
-#[should_panic(
-  expected = "Invalid Filter Argument. `at_least` or `at_most` is set, but `contains` is empty !!!"
-)]
-fn test_filter_bad_arg_at_most() {
-  FilterBuilder::default().at_least(5).build();
-}
-
-#[test]
-#[should_panic(
-  expected = "Invalid Filter Argument. `contains` and `not_contains` cannot be set at the same time !!! Please use two filters instead."
-)]
-fn test_filter_bad_arguments_contains_not_contains() {
-  FilterBuilder::default()
-    .contains(TSQuery::new(String::from("(if_statement) @if_stmt")))
-    .not_contains(vec![TSQuery::new(String::from("(for_statement) @for"))])
-    .build();
-}
-
-#[test]
-#[should_panic(
-  expected = "Invalid Filter Argument. `at_least` should be less than or equal to `at_most` !!!"
-)]
-fn test_filter_bad_range() {
-  FilterBuilder::default()
-    .contains(TSQuery::new(String::from("(if_statement) @if_stmt")))
-    .at_least(5)
-    .at_most(4)
-    .build();
-}
```

### Comparing `polyglot_piranha-0.3.8/src/tests/mod.rs` & `polyglot_piranha-0.3.9/src/tests/mod.rs`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.8/src/tests/test_piranha_go.rs` & `polyglot_piranha-0.3.9/src/tests/test_piranha_go.rs`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.8/src/tests/test_piranha_java.rs` & `polyglot_piranha-0.3.9/src/tests/test_piranha_java.rs`

 * *Files 3% similar despite different names*

```diff
@@ -372,7 +372,25 @@
     .rule_graph(RuleGraphBuilder::default().rules(vec![rule]).build())
     .build();
 
   execute_piranha_and_check_result(&piranha_arguments, &_path.join("expected"), 1, true);
   // Delete temp_dir
   temp_dir.close().unwrap();
 }
+
+#[test]
+#[should_panic(expected = "Cannot parse")]
+fn test_incorrect_rule() {
+  initialize();
+  let _path = PathBuf::from("test-resources")
+    .join(JAVA)
+    .join("incorrect_rule");
+  let path_to_codebase = _path.join("input").to_str().unwrap().to_string();
+  let path_to_configurations = _path.join("configurations").to_str().unwrap().to_string();
+  let piranha_arguments = PiranhaArgumentsBuilder::default()
+    .path_to_codebase(path_to_codebase)
+    .path_to_configurations(path_to_configurations)
+    .language(PiranhaLanguage::from(JAVA))
+    .build();
+
+  let _ = execute_piranha(&piranha_arguments);
+}
```

### Comparing `polyglot_piranha-0.3.8/src/tests/test_piranha_kt.rs` & `polyglot_piranha-0.3.9/src/tests/test_piranha_kt.rs`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.8/src/tests/test_piranha_python.rs` & `polyglot_piranha-0.3.9/src/tests/test_piranha_python.rs`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.8/src/tests/test_piranha_strings.rs` & `polyglot_piranha-0.3.9/src/tests/test_piranha_strings.rs`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.8/src/tests/test_piranha_swift.rs` & `polyglot_piranha-0.3.9/src/tests/test_piranha_swift.rs`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.8/src/tests/test_piranha_thrift.rs` & `polyglot_piranha-0.3.9/src/tests/test_piranha_thrift.rs`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.8/src/tests/test_piranha_ts.rs` & `polyglot_piranha-0.3.9/src/tests/test_piranha_ts.rs`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.8/src/tests/test_piranha_tsx.rs` & `polyglot_piranha-0.3.9/src/tests/test_piranha_tsx.rs`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.8/src/utilities/mod.rs` & `polyglot_piranha-0.3.9/src/utilities/mod.rs`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.8/src/utilities/tree_sitter_utilities.rs` & `polyglot_piranha-0.3.9/src/utilities/tree_sitter_utilities.rs`

 * *Files 4% similar despite different names*

```diff
@@ -11,23 +11,24 @@
  limitations under the License.
 */
 
 //! Defines the traits containing with utility functions that interface with tree-sitter.
 
 use super::eq_without_whitespace;
 use crate::{
-  models::{edit::Edit, matches::Match},
+  models::{edit::Edit, matches::Match, Validator},
   utilities::MapOfVec,
 };
 use itertools::Itertools;
 use log::debug;
 use pyo3::prelude::pyclass;
 use serde_derive::Deserialize;
 use std::collections::HashMap;
-use tree_sitter::{InputEdit, Node, Point, Query, QueryCapture, QueryCursor, Range};
+use tree_sitter::{InputEdit, Node, Parser, Point, Query, QueryCapture, QueryCursor, Range};
+use tree_sitter_traversal::{traverse, Order};
 
 /// Applies the query upon the given node, and gets all the matches
 /// # Arguments
 /// * `node` - the root node to apply the query upon
 /// * `source_code` - the corresponding source code string for the node.
 /// * `query` - the query to be applied
 /// * `recursive` - if `true` it matches the query to `self` and `self`'s sub-ASTs, else it matches the `query` only to `self`.
@@ -299,24 +300,51 @@
     start_byte: input_edit.start_byte,
     end_byte: input_edit.new_end_byte,
     start_point: input_edit.start_position,
     end_point: input_edit.new_end_position,
   }
 }
 
+/// Returns the (tree-sitter) parser for the tree-sitter query DSL
+pub(crate) fn get_ts_query_parser() -> Parser {
+  let mut parser = Parser::new();
+  parser
+    .set_language(tree_sitter_query::language())
+    .expect("Could not set the language for the parser.");
+  parser
+}
+
+/// Returns the number of errors in the AST
+pub(crate) fn number_of_errors(node: &Node) -> usize {
+  traverse(node.walk(), Order::Post)
+    .filter(|node| node.is_error() || node.is_missing())
+    .count()
+}
+
 #[pyclass]
 #[derive(Deserialize, Debug, Clone, Default, PartialEq, Hash, Eq)]
 pub struct TSQuery(String);
 
 impl TSQuery {
   pub(crate) fn new(query: String) -> Self {
     Self(query)
   }
 
   pub(crate) fn get_query(&self) -> String {
     self.0.to_string()
   }
 }
 
+impl Validator for TSQuery {
+  fn validate(&self) -> Result<(), String> {
+    let mut parser = get_ts_query_parser();
+    parser
+      .parse(self.get_query(), None)
+      .filter(|x| number_of_errors(&x.root_node()) == 0)
+      .map(|_| Ok(()))
+      .unwrap_or(Err(format!("Cannot parse - {}", self.get_query())))
+  }
+}
+
 #[cfg(test)]
 #[path = "unit_tests/tree_sitter_utilities_test.rs"]
 mod tree_sitter_utilities_test;
```

### Comparing `polyglot_piranha-0.3.8/src/utilities/unit_tests/tree_sitter_utilities_test.rs` & `polyglot_piranha-0.3.9/src/utilities/unit_tests/tree_sitter_utilities_test.rs`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.8/src/utilities/unit_tests/utilities_test.rs` & `polyglot_piranha-0.3.9/src/utilities/unit_tests/utilities_test.rs`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.8/PKG-INFO` & `polyglot_piranha-0.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polyglot_piranha
-Version: 0.3.8
+Version: 0.3.9
 License-File: LICENSE
 License-File: LICENSE
 License-File: NOTICE
 Summary: Polyglot Piranha is a library for performing structural find and replace with deep cleanup.
 Keywords: refactoring,code update,structural find-replace,structural search and replace,structural search
 Author: Uber Technologies Inc.
 Author-email: Ameya Ketkar <ketkara@uber.com>, Lazaro Clapp <lazaro@uber.com>
```

