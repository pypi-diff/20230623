# Comparing `tmp/bytecodemanipulation-0.3.1.tar.gz` & `tmp/bytecodemanipulation-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bytecodemanipulation-0.3.1.tar", last modified: Sun Jun  4 20:18:54 2023, max compression
+gzip compressed data, was "bytecodemanipulation-0.3.3.tar", last modified: Fri Jun 23 14:20:57 2023, max compression
```

## Comparing `bytecodemanipulation-0.3.1.tar` & `bytecodemanipulation-0.3.3.tar`

### file list

```diff
@@ -1,159 +1,165 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 20:18:54.046816 bytecodemanipulation-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6352 2023-06-04 20:18:54.046816 bytecodemanipulation-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5652 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 20:18:54.018816 bytecodemanipulation-0.3.1/bytecodemanipulation/
--rw-r--r--   0 runner    (1001) docker     (123)    22008 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/Emulator.py
--rw-r--r--   0 runner    (1001) docker     (123)    20025 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/Mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)    16723 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/MutableFunction.py
--rw-r--r--   0 runner    (1001) docker     (123)     9926 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/MutableFunctionHelpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    27097 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/Optimiser.py
--rw-r--r--   0 runner    (1001) docker     (123)    11629 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/Specialization.py
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/TypeEnforcer.py
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/annotated_std.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 20:18:54.022816 bytecodemanipulation-0.3.1/bytecodemanipulation/assembler/
--rw-r--r--   0 runner    (1001) docker     (123)    10355 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/assembler/AbstractBase.py
--rw-r--r--   0 runner    (1001) docker     (123)    12032 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/assembler/Emitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5355 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/assembler/Lexer.py
--rw-r--r--   0 runner    (1001) docker     (123)    19883 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/assembler/Parser.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/assembler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/assembler/hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     2842 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/assembler/syntax_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     3858 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/assembler/target.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 20:18:54.022816 bytecodemanipulation-0.3.1/bytecodemanipulation/assembler/util/
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/assembler/util/CommonUtil.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/assembler/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10940 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/assembler/util/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     8373 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/assembler/util/tokenizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 20:18:54.022816 bytecodemanipulation-0.3.1/bytecodemanipulation/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 20:18:54.022816 bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15893 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/builtin_spec.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 20:18:54.026816 bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/expressions/
--rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/expressions/AttributeAccessExpression.py
--rw-r--r--   0 runner    (1001) docker     (123)     3550 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/expressions/CompoundExpression.py
--rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/expressions/ConstantAccessExpression.py
--rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/expressions/DerefAccessExpression.py
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/expressions/DiscardValueExpression.py
--rw-r--r--   0 runner    (1001) docker     (123)     2983 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/expressions/DynamicAccessExpression.py
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/expressions/GlobalAccessExpression.py
--rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/expressions/GlobalStaticAccessExpression.py
--rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/expressions/LocalAccessExpression.py
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/expressions/MacroAccessExpression.py
--rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/expressions/MacroParameterAcessExpression.py
--rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/expressions/ModuleAccessExpression.py
--rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/expressions/StaticAttributeAcccessExpression.py
--rw-r--r--   0 runner    (1001) docker     (123)     3979 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/expressions/SubscriptionAccessExpression.py
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/expressions/TopOfStackAccessExpression.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/expressions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 20:18:54.034816 bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/instructions/
--rw-r--r--   0 runner    (1001) docker     (123)     4251 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/instructions/AbstractInstruction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/instructions/AssertAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/instructions/AssertStaticInstruction.py
--rw-r--r--   0 runner    (1001) docker     (123)    12361 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/instructions/CallAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     3433 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/instructions/ClassDefinitionAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     4885 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/instructions/ForEachAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     7519 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/instructions/FunctionDefinitionAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     3830 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/instructions/IfAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/instructions/JumpAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/instructions/LabelAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     3226 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/instructions/LoadAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     2998 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/instructions/LoadConstAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/instructions/LoadFastAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     3113 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/instructions/LoadGlobalAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)    22721 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/instructions/MacroAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     4442 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/instructions/MacroImportAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     2760 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/instructions/MacroPasteAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/instructions/MacroReturnAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/instructions/NamespaceAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)    19409 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/instructions/OpAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/instructions/PopElementAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/instructions/PythonCodeAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/instructions/RaiseAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/instructions/RawAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/instructions/ReturnAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/instructions/StoreAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/instructions/StoreFastAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/instructions/StoreGlobalAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     3796 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/instructions/WhileAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/instructions/YieldAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/instructions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 20:18:54.034816 bytecodemanipulation-0.3.1/bytecodemanipulation/data/v3_10/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/v3_10/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/v3_10/assembly_instructions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 20:18:54.038816 bytecodemanipulation-0.3.1/bytecodemanipulation/data/v3_10/instructions/
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/v3_10/instructions/AssertAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     6817 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/v3_10/instructions/CallAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/v3_10/instructions/ClassDefinitionAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     3750 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/v3_10/instructions/ForEachAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     5056 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/v3_10/instructions/FunctionDefinitionAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/v3_10/instructions/IfAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/v3_10/instructions/JumpAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/v3_10/instructions/LoadConstAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/v3_10/instructions/LoadFastAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/v3_10/instructions/LoadGlobalAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)    13485 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/v3_10/instructions/OpAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/v3_10/instructions/PopElementAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/v3_10/instructions/RaiseAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/v3_10/instructions/ReturnAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/v3_10/instructions/StoreFastAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/v3_10/instructions/StoreGlobalAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/v3_10/instructions/WhileAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/v3_10/instructions/YieldAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/v3_10/instructions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/v3_10/specialize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 20:18:54.038816 bytecodemanipulation-0.3.1/bytecodemanipulation/data/v3_11/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/v3_11/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/v3_11/assembly_instructions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 20:18:54.042816 bytecodemanipulation-0.3.1/bytecodemanipulation/data/v3_11/instructions/
--rw-r--r--   0 runner    (1001) docker     (123)     6817 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/v3_11/instructions/CallAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/v3_11/instructions/ClassDefinitionAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     3750 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/v3_11/instructions/ForEachAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     5006 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/v3_11/instructions/FunctionDefinitionAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/v3_11/instructions/IfAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/v3_11/instructions/JumpAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/v3_11/instructions/LoadConstAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/v3_11/instructions/LoadFastAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/v3_11/instructions/LoadGlobalAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/v3_11/instructions/OpAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/v3_11/instructions/PopElementAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/v3_11/instructions/RaiseAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/v3_11/instructions/ReturnAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/v3_11/instructions/StoreFastAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/v3_11/instructions/StoreGlobalAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/v3_11/instructions/WhileAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/v3_11/instructions/YieldAssembly.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/v3_11/instructions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data/v3_11/specialize.py
--rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/data_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     4176 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/mixin_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 20:18:54.046816 bytecodemanipulation-0.3.1/bytecodemanipulation/opcodes/
--rw-r--r--   0 runner    (1001) docker     (123)    12756 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/opcodes/AbstractOpcodeTransformerStage.py
--rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/opcodes/CodeObjectBuilder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/opcodes/ExceptionTable.py
--rw-r--r--   0 runner    (1001) docker     (123)    24591 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/opcodes/Instruction.py
--rw-r--r--   0 runner    (1001) docker     (123)     5632 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/opcodes/Opcodes.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/opcodes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/optimise_self.py
--rw-r--r--   0 runner    (1001) docker     (123)    17376 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/optimiser_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/bytecodemanipulation/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 20:18:54.022816 bytecodemanipulation-0.3.1/bytecodemanipulation.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6352 2023-06-04 20:18:53.000000 bytecodemanipulation-0.3.1/bytecodemanipulation.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7761 2023-06-04 20:18:54.000000 bytecodemanipulation-0.3.1/bytecodemanipulation.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 20:18:54.000000 bytecodemanipulation-0.3.1/bytecodemanipulation.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-04 20:18:54.000000 bytecodemanipulation-0.3.1/bytecodemanipulation.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-04 20:18:54.046816 bytecodemanipulation-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-06-04 20:18:47.000000 bytecodemanipulation-0.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 20:18:54.046816 bytecodemanipulation-0.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    52921 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/tests/test_Assembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/tests/test_InlineSystem.py
--rw-r--r--   0 runner    (1001) docker     (123)     3126 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/tests/test_Mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/tests/test_MutableFunction.py
--rw-r--r--   0 runner    (1001) docker     (123)     8115 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/tests/test_Operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     7217 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/tests/test_Optimiser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/tests/test_Specializations.py
--rw-r--r--   0 runner    (1001) docker     (123)     5353 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/tests/test_StandardLibrary.py
--rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-06-04 20:18:35.000000 bytecodemanipulation-0.3.1/tests/test_issues.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 14:20:57.368648 bytecodemanipulation-0.3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6420 2023-06-23 14:20:57.368648 bytecodemanipulation-0.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5720 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 14:20:57.352648 bytecodemanipulation-0.3.3/bytecodemanipulation/
+-rw-r--r--   0 runner    (1001) docker     (123)    22008 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/Emulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20025 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/Mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19747 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/MutableFunction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9803 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/MutableFunctionHelpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27037 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/Optimiser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11255 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/Specialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/TypeEnforcer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/annotated_std.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 14:20:57.352648 bytecodemanipulation-0.3.3/bytecodemanipulation/assembler/
+-rw-r--r--   0 runner    (1001) docker     (123)    10506 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/assembler/AbstractBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12247 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/assembler/Emitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5356 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/assembler/Lexer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20042 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/assembler/Parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/assembler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/assembler/hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/assembler/syntax_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3883 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/assembler/target.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 14:20:57.352648 bytecodemanipulation-0.3.3/bytecodemanipulation/assembler/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/assembler/util/CommonUtil.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/assembler/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10940 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/assembler/util/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8373 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/assembler/util/tokenizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 14:20:57.352648 bytecodemanipulation-0.3.3/bytecodemanipulation/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 14:20:57.352648 bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15377 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/builtin_spec.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 14:20:57.356648 bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/expressions/
+-rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/expressions/AttributeAccessExpression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3550 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/expressions/CompoundExpression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/expressions/ConstantAccessExpression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/expressions/DerefAccessExpression.py
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/expressions/DiscardValueExpression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/expressions/DynamicAccessExpression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/expressions/GlobalAccessExpression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/expressions/GlobalStaticAccessExpression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/expressions/LocalAccessExpression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/expressions/MacroAccessExpression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/expressions/MacroParameterAcessExpression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/expressions/ModuleAccessExpression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/expressions/StaticAttributeAcccessExpression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3839 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/expressions/SubscriptionAccessExpression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/expressions/TopOfStackAccessExpression.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/expressions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 14:20:57.360648 bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/instructions/
+-rw-r--r--   0 runner    (1001) docker     (123)     4244 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/instructions/AbstractInstruction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/instructions/AssertAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3441 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/instructions/AssertStaticInstruction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14138 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/instructions/CallAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3412 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/instructions/ClassDefinitionAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4808 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/instructions/ForEachAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9234 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/instructions/FunctionDefinitionAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3809 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/instructions/IfAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/instructions/JumpAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/instructions/LabelAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3205 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/instructions/LoadAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/instructions/LoadConstAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/instructions/LoadFastAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/instructions/LoadGlobalAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25406 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/instructions/MacroAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4442 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/instructions/MacroImportAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/instructions/MacroPasteAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/instructions/MacroReturnAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/instructions/NamespaceAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19276 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/instructions/OpAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/instructions/PopElementAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/instructions/PythonCodeAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/instructions/RaiseAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/instructions/RawAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/instructions/ReturnAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2842 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/instructions/StoreAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/instructions/StoreFastAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/instructions/StoreGlobalAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3775 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/instructions/WhileAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/instructions/YieldAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/instructions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 14:20:57.360648 bytecodemanipulation-0.3.3/bytecodemanipulation/data/v3_10/
+-rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/v3_10/ExceptionInstructionCodec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/v3_10/LocationInformationHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/v3_10/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/v3_10/assembly_instructions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 14:20:57.364648 bytecodemanipulation-0.3.3/bytecodemanipulation/data/v3_10/instructions/
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/v3_10/instructions/AssertAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6503 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/v3_10/instructions/CallAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2657 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/v3_10/instructions/ClassDefinitionAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3292 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/v3_10/instructions/ForEachAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5781 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/v3_10/instructions/FunctionDefinitionAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/v3_10/instructions/IfAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/v3_10/instructions/JumpAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/v3_10/instructions/LoadConstAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/v3_10/instructions/LoadFastAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/v3_10/instructions/LoadGlobalAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13524 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/v3_10/instructions/OpAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/v3_10/instructions/PopElementAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/v3_10/instructions/RaiseAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/v3_10/instructions/ReturnAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/v3_10/instructions/StoreFastAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/v3_10/instructions/StoreGlobalAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/v3_10/instructions/WhileAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/v3_10/instructions/YieldAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/v3_10/instructions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/v3_10/specialize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 14:20:57.364648 bytecodemanipulation-0.3.3/bytecodemanipulation/data/v3_11/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/v3_11/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/v3_11/assembly_instructions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 14:20:57.364648 bytecodemanipulation-0.3.3/bytecodemanipulation/data/v3_11/instructions/
+-rw-r--r--   0 runner    (1001) docker     (123)     6599 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/v3_11/instructions/CallAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/v3_11/instructions/ClassDefinitionAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3292 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/v3_11/instructions/ForEachAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4912 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/v3_11/instructions/FunctionDefinitionAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/v3_11/instructions/IfAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/v3_11/instructions/JumpAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/v3_11/instructions/LoadConstAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/v3_11/instructions/LoadFastAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/v3_11/instructions/LoadGlobalAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2799 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/v3_11/instructions/OpAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/v3_11/instructions/PopElementAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/v3_11/instructions/RaiseAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/v3_11/instructions/ReturnAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/v3_11/instructions/StoreFastAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/v3_11/instructions/StoreGlobalAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/v3_11/instructions/WhileAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/v3_11/instructions/YieldAssembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/v3_11/instructions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/v3_11/specialize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 14:20:57.364648 bytecodemanipulation-0.3.3/bytecodemanipulation/data/v3_12/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data/v3_12/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3183 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/data_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4176 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/mixin_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 14:20:57.368648 bytecodemanipulation-0.3.3/bytecodemanipulation/opcodes/
+-rw-r--r--   0 runner    (1001) docker     (123)    12784 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/opcodes/AbstractOpcodeTransformerStage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/opcodes/CacheEntryCreation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/opcodes/CodeObjectBuilder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/opcodes/ExceptionTable.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25688 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/opcodes/Instruction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3139 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/opcodes/OpcodeReplacer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5599 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/opcodes/Opcodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/opcodes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/optimise_self.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17426 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/optimiser_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/bytecodemanipulation/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 14:20:57.352648 bytecodemanipulation-0.3.3/bytecodemanipulation.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6420 2023-06-23 14:20:57.000000 bytecodemanipulation-0.3.3/bytecodemanipulation.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8026 2023-06-23 14:20:57.000000 bytecodemanipulation-0.3.3/bytecodemanipulation.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 14:20:57.000000 bytecodemanipulation-0.3.3/bytecodemanipulation.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-23 14:20:57.000000 bytecodemanipulation-0.3.3/bytecodemanipulation.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 14:20:57.368648 bytecodemanipulation-0.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-06-23 14:20:50.000000 bytecodemanipulation-0.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 14:20:57.368648 bytecodemanipulation-0.3.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    54986 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/tests/test_Assembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/tests/test_InlineSystem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3126 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/tests/test_Mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/tests/test_MutableFunction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8827 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/tests/test_Operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7282 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/tests/test_Optimiser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/tests/test_Specializations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5229 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/tests/test_StandardLibrary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-06-23 14:20:39.000000 bytecodemanipulation-0.3.3/tests/test_issues.py
```

### Comparing `bytecodemanipulation-0.3.1/LICENSE` & `bytecodemanipulation-0.3.3/LICENSE`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 uuk0
+Copyright (c) 2022-2023 uuk0
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `bytecodemanipulation-0.3.1/PKG-INFO` & `bytecodemanipulation-0.3.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bytecodemanipulation
-Version: 0.3.1
+Version: 0.3.3
 Summary: High level python bytecode manipulation
 Home-page: https://github.com/uuk0/PyBytecodeManipulator
 Author: uuk
 Author-email: uuk1301@gmail.com
 Project-URL: Bug Tracker, https://github.com/uuk0/PyBytecodeManipulator/issues
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -160,8 +160,9 @@
 # TODO's
 
 - abstract opcode affect away into a .json file describing all opcodes
 - create a json file for defining certain bytecode sequences
 - write more library-specific optimisations
 - write generating bytecode system for emulator, constructing a function pointing to the
   .json file for exception printing, and optimizing wherever possible
+- add optimisation: JUMP on condition for some operators (e.g. NOT)
```

### Comparing `bytecodemanipulation-0.3.1/README.md` & `bytecodemanipulation-0.3.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -142,8 +142,9 @@
 # TODO's
 
 - abstract opcode affect away into a .json file describing all opcodes
 - create a json file for defining certain bytecode sequences
 - write more library-specific optimisations
 - write generating bytecode system for emulator, constructing a function pointing to the
   .json file for exception printing, and optimizing wherever possible
+- add optimisation: JUMP on condition for some operators (e.g. NOT)
```

### Comparing `bytecodemanipulation-0.3.1/bytecodemanipulation/Emulator.py` & `bytecodemanipulation-0.3.3/bytecodemanipulation/Emulator.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.3.1/bytecodemanipulation/Mixin.py` & `bytecodemanipulation-0.3.3/bytecodemanipulation/Mixin.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.3.1/bytecodemanipulation/MutableFunctionHelpers.py` & `bytecodemanipulation-0.3.3/bytecodemanipulation/MutableFunctionHelpers.py`

 * *Files 3% similar despite different names*

```diff
@@ -186,16 +186,15 @@
     if len(args) > 0 and args[0].opcode != Opcodes.LOAD_CONST:
         return False
 
     # In case we have no args, we need to add a LOAD_CONST(None)
     if len(args) == 0:
         instruction.change_opcode(Opcodes.LOAD_CONST)
         instruction.change_arg_value(None)
-        return_instr = Instruction.create(Opcodes.RETURN_VALUE)
-        return_instr.update_owner(mutable, -1)
+        return_instr = Instruction.create_with_same_info(instruction, Opcodes.RETURN_VALUE)
         return_instr.next_instruction = instruction.next_instruction
         instruction.next_instruction = return_instr
 
     return True
 
 
 def insert_method_into(
@@ -207,15 +206,15 @@
 ):
     """
     Inserts the function AFTER the given offset / Instruction.
     If wanted at HEAD, set offset to -1
     """
 
     if entry_point == -1:
-        HEAD_INSTRUCTION = Instruction.create("NOP")
+        HEAD_INSTRUCTION = Instruction("NOP")
         HEAD_INSTRUCTION.function = body
         HEAD_INSTRUCTION.next_instruction = body.instruction_entry_point
         body.instruction_entry_point = HEAD_INSTRUCTION
 
     elif isinstance(entry_point, int):
         head = body.instruction_entry_point
 
@@ -261,32 +260,27 @@
         nonlocal previous
 
         if previous is not None:
             previous.next_instruction = instr
 
         if instr.opcode == Opcodes.INTERMEDIATE_INNER_RETURN:
             if drop_return_result:
-                previous.insert_after(Instruction(to_insert, -1, Opcodes.POP_TOP))
+                previous.insert_after(Instruction.create_with_same_info(previous, Opcodes.POP_TOP))
 
             instr.change_opcode(
                 Opcodes.JUMP_ABSOLUTE, HEAD_INSTRUCTION.next_instruction
             )
 
         previous = instr
 
     to_insert.walk_instructions(visit)
 
     if instr is not None and instr.next_instruction is None:
         instr.next_instruction = HEAD_INSTRUCTION.next_instruction
 
-    def visit(instr):
-        instr.update_owner(body, -1, False)
-
-    to_insert.walk_instructions(visit)
-
     replace_const_func_call_with_opcode(
         to_insert,
         capture_local,
         Opcodes.LOAD_FAST,
         _inline_capture_local,
     )
     replace_const_func_call_with_opcode(
@@ -316,15 +310,15 @@
             container = _OptimisationContainer.get_for_target(target)
             if not container.try_inline_calls:
                 return
 
             instr.change_opcode(Opcodes.NOP)
             insert_method_into(
                 mutable,
-                instr.offset,
+                instr,
                 MutableFunction(target),
                 drop_return_result=False,
             )
             source.change_opcode(Opcodes.NOP)
             nonlocal dirty
             dirty = True
```

### Comparing `bytecodemanipulation-0.3.1/bytecodemanipulation/Optimiser.py` & `bytecodemanipulation-0.3.3/bytecodemanipulation/Optimiser.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 from bytecodemanipulation.opcodes.Opcodes import Opcodes
 from bytecodemanipulation.optimiser_util import inline_const_value_pop_pairs
 from bytecodemanipulation.optimiser_util import inline_constant_binary_ops
 from bytecodemanipulation.optimiser_util import inline_constant_method_invokes
 from bytecodemanipulation.optimiser_util import inline_static_attribute_access
 from bytecodemanipulation.optimiser_util import remove_branch_on_constant
 from bytecodemanipulation.optimiser_util import remove_local_var_assign_without_use
-from bytecodemanipulation.optimiser_util import remove_nops
 from bytecodemanipulation.Specialization import SpecializationContainer
 from bytecodemanipulation.util import _is_parent_of
 
 BUILTIN_CACHE = builtins.__dict__.copy()
 
 DISABLE_OPTIMISATION_APPLY = os.environ.setdefault("DISABLE_OPTIMISATION_APPLY", "")
```

### Comparing `bytecodemanipulation-0.3.1/bytecodemanipulation/Specialization.py` & `bytecodemanipulation-0.3.3/bytecodemanipulation/Specialization.py`

 * *Files 2% similar despite different names*

```diff
@@ -182,29 +182,25 @@
             using ArgDescriptor as instructions impossible!
         """
 
         if not leave_args_on_stack:
             # Store values in temporary variables
             bytecode = [
                 Instruction(
-                    self.target,
-                    -1,
                     Opcodes.STORE_FAST,
                     f"&fast_tmp_specialize_local::{i}",
                 )
                 for i in range(self.method_call_descriptor.call_method_instr.arg)
             ]
 
             bytecode += [
                 (
-                    instruction.update_owner(self.target, -1)
+                    instruction
                     if isinstance(instruction, Instruction)
                     else Instruction(
-                        self.target,
-                        -1,
                         Opcodes.LOAD_FAST,
                         f"&fast_tmp_specialize_local::{instruction.arg_id}",
                     )
                 )
                 for instruction in opcodes
             ]
         else:
@@ -257,26 +253,20 @@
             if self.invoke_before:
                 self.method_call_descriptor.lookup_method_instr.change_opcode(
                     Opcodes.LOAD_CONST
                 )
                 self.method_call_descriptor.lookup_method_instr.change_arg_value(
                     self.invoke_before
                 )
-                self.method_call_descriptor.call_method_instr.change_arg(arg_count)
+                call = self.method_call_descriptor.call_method_instr
+                call.change_arg(arg_count)
 
-                self.method_call_descriptor.call_method_instr.insert_after(
-                    Instruction(
-                        self.underlying_function, -1, opcode_or_name=Opcodes.POP_TOP
-                    ),
-                    Instruction(
-                        self.underlying_function,
-                        -1,
-                        opcode_or_name=Opcodes.LOAD_CONST,
-                        arg_value=self.constant_value[0],
-                    ),
+                call.insert_after(
+                    Instruction.create_with_same_info(call, Opcodes.POP_TOP),
+                    Instruction.create_with_same_info(call, Opcodes.LOAD_CONST, self.constant_value[0]),
                 )
 
             else:
                 self.method_call_descriptor.lookup_method_instr.change_opcode(
                     Opcodes.NOP
                 )
                 self.method_call_descriptor.call_method_instr.change_opcode(
```

### Comparing `bytecodemanipulation-0.3.1/bytecodemanipulation/assembler/AbstractBase.py` & `bytecodemanipulation-0.3.3/bytecodemanipulation/assembler/AbstractBase.py`

 * *Files 6% similar despite different names*

```diff
@@ -44,14 +44,15 @@
         self.global_scope = {}
         self.scope_path: typing.List[str] = []
         self._name_counter = 1
         self.globals_dict = {}
         self.module_file: str = None
         self.last_base_token: AbstractToken = None
         self.macro_parameter_namespace: typing.Dict[str] = {}
+        self.filled_locals = set()
 
     def scope_name_generator(self, suffix="") -> str:
         name = f"%INTERNAL:{self._name_counter}"
         self._name_counter += 1
 
         if suffix:
             name += "/" + suffix
@@ -109,14 +110,15 @@
         return False
 
     def copy(
         self,
         sub_scope_name: str | list = None,
         copy_labels=False,
         keep_scope_name_generator: bool = None,
+        shared_locals=True,
     ):
         instance = ParsingScope()
         if copy_labels:
             instance.labels = self.labels
         instance.global_scope = self.global_scope
         instance.scope_path = self.scope_path.copy()
         instance.module_file = self.module_file
@@ -127,14 +129,17 @@
                 instance.scope_path.append(sub_scope_name)
             else:
                 instance.scope_path += sub_scope_name
 
         elif keep_scope_name_generator:
             instance.scope_name_generator = self.scope_name_generator
 
+        if shared_locals:
+            instance.filled_locals = self.filled_locals
+
         return instance
 
     def insert_into_scope(
         self, name: typing.List[str], data: typing.Any, override_existing=False
     ):
         if not name:
             raise ValueError("'name' must have at least one element!")
@@ -267,15 +272,15 @@
         return False
 
     def __repr__(self):
         return f"&{self.macro_name}"
 
     def __call__(self, scope: ParsingScope):
         from bytecodemanipulation.assembler.syntax_errors import (
-            throw_positioned_syntax_error,
+            throw_positioned_error,
         )
         from bytecodemanipulation.data.shared.expressions.ConstantAccessExpression import (
             ConstantAccessExpression,
         )
         from bytecodemanipulation.data.shared.expressions.DerefAccessExpression import (
             DerefAccessExpression,
         )
@@ -286,25 +291,25 @@
             LocalAccessExpression,
         )
 
         if scope is None:
             raise SyntaxError("no scope provided")
 
         if self.token[1].text not in scope.macro_parameter_namespace:
-            raise throw_positioned_syntax_error(
+            raise throw_positioned_error(
                 scope,
                 self.token,
                 "Could not find name in macro parameter space",
             )
 
         value = scope.macro_parameter_namespace[self.token[1].text]
 
         if isinstance(value, ConstantAccessExpression):
             if not isinstance(value.value, str):
-                raise throw_positioned_syntax_error(
+                raise throw_positioned_error(
                     scope,
                     self.token,
                     f"Expected 'string' for name de-referencing, got {value}",
                 )
 
             return value.value
 
@@ -314,34 +319,35 @@
                 GlobalAccessExpression,
                 LocalAccessExpression,
                 DerefAccessExpression,
             ),
         ):
             return value.get_name(scope)
 
-        raise throw_positioned_syntax_error(
+        raise throw_positioned_error(
             scope,
             self.token,
             f"Expected <static evaluated expression> for getting the name for storing, got {value}",
         )
 
 
 class StaticIdentifier(IIdentifierAccessor):
     def __init__(self, name: str, token: AbstractToken = None):
         self.name = name
+        self.token = token
 
     def __eq__(self, other):
         return (
             isinstance(other, StaticIdentifier) and self.name == other.name
         ) or self.name == other
 
     def __hash__(self):
         return hash(self.name)
 
     def __repr__(self):
-        return repr(self.name)
+        return "!" + repr(self.name)
 
     def __call__(self, scope: ParsingScope):
         return self.name
 
     def get_tokens(self) -> typing.Iterable[AbstractToken]:
         return (self.token,)
```

### Comparing `bytecodemanipulation-0.3.1/bytecodemanipulation/assembler/Emitter.py` & `bytecodemanipulation-0.3.3/bytecodemanipulation/assembler/Emitter.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,21 @@
-import dis
 import string
 import types
 import typing
 
-from bytecodemanipulation.assembler.AbstractBase import StaticIdentifier
+from bytecodemanipulation.assembler.AbstractBase import IIdentifierAccessor, StaticIdentifier
 from bytecodemanipulation.assembler.Lexer import Lexer
 from bytecodemanipulation.MutableFunction import MutableFunction
-from bytecodemanipulation.opcodes.CodeObjectBuilder import CodeObjectBuilder
 from bytecodemanipulation.opcodes.Instruction import Instruction
 from bytecodemanipulation.opcodes.Opcodes import Opcodes
 from bytecodemanipulation.assembler.Parser import (
     Parser as AssemblyParser,
 )
-from bytecodemanipulation.assembler.AbstractBase import JumpToLabel
-from bytecodemanipulation.assembler.AbstractBase import ParsingScope
+from bytecodemanipulation.assembler.AbstractBase import JumpToLabel, ParsingScope
 from bytecodemanipulation.assembler import target as assembly_targets
-from bytecodemanipulation.util import LambdaInstructionWalker
 
 
 def _visit_for_stack_effect(
     ins: Instruction,
     eff_a: typing.Tuple[int, int] | None,
     eff_b: typing.Tuple[int, int] | None,
 ) -> typing.Tuple[int, int]:
@@ -46,93 +42,116 @@
     return eff, max_size
 
 
 GLOBAL_SCOPE_CACHE: typing.Dict[str, dict] = {}
 
 
 def apply_inline_assemblies(
-    target: MutableFunction | typing.Callable, builder: CodeObjectBuilder = None, store_at_target: bool = None
+    target: MutableFunction | typing.Callable, store_at_target: bool = None
 ):
     """
-    Processes all assembly() calls and label() calls in 'target'
+    Processes all assembly() calls, label() calls and jump() calls in 'target'
     """
     if not isinstance(target, MutableFunction):
         target = MutableFunction(target)
         if store_at_target is None:
             store_at_target = True
 
-    builder = builder or target.create_filled_builder()
-
-    labels = set()
+    labels: typing.Set[IIdentifierAccessor] = set()
+    label_targets: typing.Dict[str, Instruction] = {}
     insertion_points: typing.List[typing.Tuple[str, Instruction]] = []
 
-    for instr in builder.temporary_instructions[:]:
+    def visit(instr: Instruction):
         if instr.opcode == Opcodes.LOAD_GLOBAL:
             try:
                 value = target.target.__globals__.get(instr.arg_value)
             except KeyError:
-                continue
+                return
 
             if value == assembly_targets.assembly:
                 invoke = next(instr.trace_stack_position_use(0))
                 arg = next(invoke.trace_stack_position(0))
-                assert (
-                    arg.opcode == Opcodes.LOAD_CONST
-                ), "only constant assembly code is allowed!"
+
+                if arg.opcode != Opcodes.LOAD_CONST:
+                    raise SyntaxError("<assembly> must be constant!")
 
                 if invoke.next_instruction.opcode == Opcodes.POP_TOP:
-                    insertion_points.append((arg.arg_value, invoke.next_instruction))
+                    insertion_points.append((typing.cast(str, arg.arg_value), invoke.next_instruction))
                 else:
-                    insertion_points.append((arg.arg_value, invoke))
+                    insertion_points.append((typing.cast(str, arg.arg_value), invoke))
 
                 instr.change_opcode(Opcodes.NOP)
                 arg.change_opcode(Opcodes.NOP)
                 invoke.change_opcode(Opcodes.LOAD_CONST, None)
 
             elif value == assembly_targets.jump:
                 invoke = next(instr.trace_stack_position_use(0))
-                arg = next(invoke.trace_stack_position(0))
-                assert (
-                    arg.opcode == Opcodes.LOAD_CONST
-                ), "only constant assembly code is allowed!"
-                assert all(
-                    e in string.ascii_letters + string.digits for e in arg.arg_value
-                ), "only characters and digits are allowed for label names!"
+
+                if invoke.arg not in (1, 2):
+                    raise SyntaxError(f"expected one to two args, not {invoke.arg} for <jump>")
+
+                label_name = next(invoke.trace_stack_position(0))
+
+                if label_name.opcode != Opcodes.LOAD_CONST:
+                    raise SyntaxError(f"expected <constant>, got {label_name}")
+
+                condition = None
+                if invoke.arg == 2:
+                    condition = label_name
+                    label_name = next(invoke.trace_stack_position(0))
+
+                    if label_name.opcode != Opcodes.LOAD_CONST:
+                        raise SyntaxError(f"expected <constant>, got {label_name}")
+
+                    raise NotImplementedError("<condition> on jump() target")
+
+                if not typing.cast(str, label_name.arg_value).isalnum():
+                    raise SyntaxError("label name only characters and digits are allowed for label names!")
 
                 if invoke.next_instruction.opcode == Opcodes.POP_TOP:
                     insertion_points.append(
-                        (f"JUMP {arg.arg_value}", invoke.next_instruction)
+                        (f"JUMP {label_name.arg_value}", invoke.next_instruction)
                     )
                 else:
-                    insertion_points.append((f"JUMP {arg.arg_value}", invoke))
+                    raise SyntaxError(invoke.next_instruction)
 
                 instr.change_opcode(Opcodes.NOP)
-                arg.change_opcode(Opcodes.NOP)
+                label_name.change_opcode(Opcodes.NOP)
                 invoke.change_opcode(Opcodes.LOAD_CONST, None)
 
             elif value == assembly_targets.label:
                 invoke = next(instr.trace_stack_position_use(0))
                 arg = next(invoke.trace_stack_position(0))
-                assert (
-                    arg.opcode == Opcodes.LOAD_CONST
-                ), "only constant label names are allowed!"
 
-                labels.add(StaticIdentifier(arg.arg_value))
+                if arg.opcode != Opcodes.LOAD_CONST:
+                    raise SyntaxError("<label name> must be constant")
+
+                labels.add(StaticIdentifier(typing.cast(str, arg.arg_value)))
                 invoke.change_opcode(Opcodes.BYTECODE_LABEL, arg.arg_value)
-                invoke.insert_after(Instruction(target, -1, Opcodes.LOAD_CONST, None))
+                invoke.insert_after(Instruction.create_with_same_info(invoke, Opcodes.LOAD_CONST, None))
                 instr.change_opcode(Opcodes.NOP)
-                # print(type(arg))
                 arg.change_opcode(Opcodes.NOP)
+                label_targets[typing.cast(str, invoke.arg_value)] = invoke.next_instruction
+
+    target.walk_instructions(visit)
 
     if not insertion_points:
         raise RuntimeError("no target found!")
 
     scope = ParsingScope()
     scope.globals_dict = target.target.__globals__
     scope.module_file = target.target.__globals__["__file__"]
+    scope.filled_locals = set(target.argument_names)
+
+    def visit(instr: Instruction):
+        if instr.opcode == Opcodes.STORE_FAST:
+            scope.filled_locals.add(instr.arg_value)
+
+
+    target.walk_instructions(visit)
 
     if target.target.__module__ in GLOBAL_SCOPE_CACHE:
         scope.global_scope = GLOBAL_SCOPE_CACHE[target.target.__module__]
     else:
         GLOBAL_SCOPE_CACHE[target.target.__module__] = scope.global_scope
 
     assemblies = [
@@ -140,139 +159,127 @@
             Lexer(code).add_line_offset(instr.source_location[0] + 1).lex(),
             scope.scope_path.clear() or scope,
         ).parse()
         for code, instr in insertion_points
     ]
 
     for asm in assemblies:
-        labels.update(asm.collect_label_info(scope))
+        asm_labels = asm.collect_label_info(scope)
+        labels.update({StaticIdentifier(e) for e in asm_labels})
 
     scope.labels |= labels
 
     max_stack_effects = []
 
-    label_targets: typing.Dict[str, Instruction] = {}
-
     # for asm in assemblies:
     #     asm.fill_scope_complete(scope)
 
     scope.scope_path.clear()
 
     for (_, instr), asm in zip(insertion_points, assemblies):
-        bytecode = asm.create_bytecode(target, scope)
+        _create_fragment_bytecode(asm, instr, label_targets, max_stack_effects, scope, target)
 
-        for i, ins in enumerate(bytecode[:-1]):
-            ins.next_instruction = bytecode[i + 1]
-
-        # print("---- start ----")
-        # for e in bytecode:
-        #     print(e)
-        # print("---- end ----")
-
-        if bytecode:
-            try:
-                stack_effect, max_stack_effect = bytecode[0].apply_value_visitor(
-                    _visit_for_stack_effect
-                )
-            except RuntimeError:
-                stack_effect = 0
-                max_stack_effect = 0
-        else:
-            stack_effect = max_stack_effect = 0
-
-        if (
-            stack_effect != 0
-            and bytecode
-            and not (
-                bytecode[-1].has_unconditional_jump() or bytecode[-1].has_stop_flow()
-            )
-        ):
-            print(asm)
-
-            total = 0
-
-            for e in enumerate(bytecode):
-                add, subtract, _ = e[1].get_stack_affect()
-                total += add - subtract
-                print(*e, total)
-
-            print(stack_effect)
-
-            raise RuntimeError(
-                f"Inline assembly code mustn't change overall stack size at exit, got a delta of {stack_effect}!"
-            )
-
-        max_stack_effects.append(max_stack_effect)
-
-        if bytecode:
-            for i, ins in enumerate(bytecode[:-1]):
-                if not ins.has_stop_flow() and not ins.has_unconditional_jump():
-                    ins.next_instruction = bytecode[i + 1]
-
-            bytecode[-1].next_instruction = following_instr = instr.next_instruction
-
-            # print("inserting AFTER", instr)
-            instr.insert_after(bytecode)
-        # else:
-        #     print("empty bytecode block")
-        #     print(asm)
-
-        for i, ins in enumerate(bytecode):
-            if ins.opcode == Opcodes.BYTECODE_LABEL:
-                label_targets[ins.arg_value] = ins.next_instruction
-
-                if not isinstance(ins, Instruction):
-                    print("error: ", ins)
-
-                ins.change_opcode(Opcodes.NOP)
-                ins.next_instruction = (
-                    bytecode[i + 1] if i < len(bytecode) - 1 else following_instr
-                )
-
-    for i, ins in enumerate(builder.temporary_instructions):
-        if ins.opcode == Opcodes.BYTECODE_LABEL:
-            label_targets[ins.arg_value] = ins.next_instruction
-            ins.change_opcode(Opcodes.NOP)
-            ins.next_instruction = builder.temporary_instructions[i + 1]
+    target.walk_instructions(visit)
 
     pending: typing.List[Instruction] = []
 
-    def resolve_special_code(ins: Instruction, *_):
+    def resolve_special_code(ins: Instruction):
         # print(ins)
         if ins.has_jump() and isinstance(ins.arg_value, JumpToLabel):
+            if ins.arg_value.name not in label_targets:
+                print(label_targets)
+                raise NameError(f"Label '{ins.arg_value.name}' not found!")
+
             ins.change_arg_value(label_targets[ins.arg_value.name])
             pending.append(ins.arg_value)
 
         elif ins.opcode == Opcodes.STATIC_ATTRIBUTE_ACCESS:
             source = next(ins.trace_stack_position(0))
 
             if source.opcode != Opcodes.LOAD_CONST:
                 raise RuntimeError("expected 'constant' for constant attribute access!")
 
             obj = source.arg_value
-            source.change_opcode(Opcodes.NOP, update_next=False)
+            source.change_opcode(Opcodes.NOP)
             ins.change_opcode(
-                Opcodes.LOAD_CONST, getattr(obj, ins.arg_value), update_next=False
+                Opcodes.LOAD_CONST, getattr(obj, ins.arg_value)
             )
 
     target.walk_instructions(resolve_special_code)
 
-    while pending:
-        pending.pop().apply_value_visitor(resolve_special_code)
-
-    # target.instructions[0].apply_value_visitor(lambda instr, *_: print(instr))
-
-    # target.assemble_instructions_from_tree(target.instructions[0])
-
     if store_at_target:
         target.reassign_to_function()
 
     return target
 
 
+def _create_fragment_bytecode(asm, insertion_point: Instruction, label_targets: typing.Dict[str, Instruction], max_stack_effects: typing.List, scope: ParsingScope, target: MutableFunction):
+    bytecode = asm.create_bytecode(target, scope)
+
+    if bytecode:
+        # link the instructions to each other
+        for i, ins in enumerate(bytecode[:-1]):
+            ins.next_instruction = bytecode[i + 1]
+
+        try:
+            stack_effect, max_stack_effect = bytecode[0].apply_value_visitor(
+                _visit_for_stack_effect
+            )
+        except RuntimeError:
+            stack_effect = 0
+            max_stack_effect = 0
+
+    else:
+        max_stack_effects.append(0)
+        return
+
+    if (
+        stack_effect != 0
+        and not (
+            bytecode[-1].has_unconditional_jump() or bytecode[-1].has_stop_flow()
+        )
+    ):
+        # print(asm)
+
+        total = 0
+
+        for e in enumerate(bytecode):
+            add, subtract, _ = e[1].get_stack_affect()
+            total += add - subtract
+            print(*e, total)
+
+        print(stack_effect)
+
+        raise RuntimeError(
+            f"Inline assembly code mustn't change overall stack size at exit, got a delta of {stack_effect}!"
+        )
+
+    max_stack_effects.append(max_stack_effect)
+
+    for i, ins in enumerate(bytecode[:-1]):
+        if not ins.has_stop_flow() and not ins.has_unconditional_jump():
+            ins.next_instruction = bytecode[i + 1]
+
+    bytecode[-1].next_instruction = following_instr = insertion_point.next_instruction
+
+    insertion_point.insert_after(bytecode)
+
+    for i, ins in enumerate(bytecode):
+        if ins.opcode == Opcodes.BYTECODE_LABEL:
+            label_targets[ins.arg_value] = ins.next_instruction
+
+            if not isinstance(ins, Instruction):
+                print("error: ", ins)
+
+            ins.change_opcode(Opcodes.NOP)
+            ins.next_instruction = (
+                bytecode[i + 1] if i < len(bytecode) - 1 else following_instr
+            )
+
+
 def execute_module_in_instance(
     asm_code: str, module: types.ModuleType, file: str = None
 ):
     scope = ParsingScope()
 
     try:
         scope.module_file = file or module.__file__
@@ -306,51 +313,44 @@
     for i, ins in enumerate(bytecode[:-1]):
         ins.next_instruction = bytecode[i + 1]
 
     def resolve_jump_to_label(ins: Instruction):
         if ins.has_jump() and isinstance(ins.arg_value, JumpToLabel):
             ins.change_arg_value(label_targets[ins.arg_value.name])
 
-    for instr in bytecode:
-        instr.update_owner(
-            target, -1, force_change_arg_index=True, update_following=False
-        )
-
     if not bytecode:
-        bytecode.append(Instruction(target, -1, "NOP"))
+        bytecode.append(Instruction(Opcodes.NOP))
 
     bytecode[-1].next_instruction = target.instruction_entry_point
+    target.instruction_entry_point = bytecode[0]
+    target.prepare_previous_instructions()
 
     target.walk_instructions(resolve_jump_to_label)
 
-    for instr in bytecode:
+    def visit(instr):
         if instr.opcode == Opcodes.STORE_FAST:
-            load_module = Instruction(target, -1, Opcodes.LOAD_FAST, "$module$")
-            store = Instruction(target, -1, Opcodes.STORE_ATTR, instr.arg_value)
+            load_module = Instruction.create_with_same_info(instr, Opcodes.LOAD_FAST, "$module$")
+            store = Instruction.create_with_same_info(instr, Opcodes.STORE_ATTR, instr.arg_value)
 
             instr.change_opcode(Opcodes.NOP)
             instr.insert_after([load_module, store])
 
         elif instr.opcode == Opcodes.LOAD_FAST:
-            load_module = Instruction(target, -1, Opcodes.LOAD_FAST, "$module$")
-            load = Instruction(target, -1, Opcodes.LOAD_ATTR, instr.arg_value)
+            load_module = Instruction.create_with_same_info(instr, Opcodes.LOAD_FAST, "$module$")
+            load = Instruction.create_with_same_info(instr, Opcodes.LOAD_ATTR, instr.arg_value)
 
             instr.change_opcode(Opcodes.NOP)
             instr.insert_after([load_module, load])
 
         elif instr.opcode == Opcodes.DELETE_FAST:
-            load_module = Instruction(target, -1, Opcodes.LOAD_FAST, "$module$")
-            delete = Instruction(target, -1, Opcodes.DELETE_ATTR, instr.arg_value)
+            load_module = Instruction.create_with_same_info(instr, Opcodes.LOAD_FAST, "$module$")
+            delete = Instruction.create_with_same_info(instr, Opcodes.DELETE_ATTR, instr.arg_value)
 
             instr.change_opcode(Opcodes.NOP)
             instr.insert_after([load_module, delete])
 
-    target.function_name = module.__name__
-
-    target.instruction_entry_point = bytecode[0]
-    target.prepare_previous_instructions()
+    target.walk_instructions_stable(visit)
 
+    target.function_name = module.__name__
     target.reassign_to_function()
 
-    # dis.dis(target)
-
     create_function(module)
```

### Comparing `bytecodemanipulation-0.3.1/bytecodemanipulation/assembler/Lexer.py` & `bytecodemanipulation-0.3.3/bytecodemanipulation/assembler/Lexer.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         IdentifierToken,
         StringLiteralToken,
         CommentToken,
         AbstractToken,
     )
 
 
-SPECIAL_CHARS = "@$+-~/%?;[]{}()<>=!,.*':§&\\"
+SPECIAL_CHARS = "@$+-~/%?;[]{}()<>=!,.*':§&\\|"
 
 
 class SpecialToken(AbstractToken):
     pass
 
 
 class PythonCodeToken(AbstractToken):
```

### Comparing `bytecodemanipulation-0.3.1/bytecodemanipulation/assembler/Parser.py` & `bytecodemanipulation-0.3.3/bytecodemanipulation/assembler/Parser.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from bytecodemanipulation.assembler.AbstractBase import (
     IIdentifierAccessor,
     MacroExpandedIdentifier,
     StaticIdentifier,
 )
 from bytecodemanipulation.assembler.AbstractBase import ParsingScope
 from bytecodemanipulation.assembler.syntax_errors import _syntax_wrapper
-from bytecodemanipulation.assembler.syntax_errors import throw_positioned_syntax_error
+from bytecodemanipulation.assembler.syntax_errors import throw_positioned_error
 from bytecodemanipulation.data.shared.instructions.AbstractInstruction import (
     AbstractAssemblyInstruction,
 )
 from bytecodemanipulation.data.shared.expressions.AttributeAccessExpression import (
     AttributeAccessExpression,
 )
 from bytecodemanipulation.data.shared.instructions.CallAssembly import (
@@ -172,15 +172,15 @@
         if namespace_part is not None:
             if isinstance(namespace_part, str):
                 scope.scope_path.append(namespace_part)
             else:
                 scope.scope_path += namespace_part
 
         if not self.try_consume(SpecialToken("{")):
-            raise throw_positioned_syntax_error(
+            raise throw_positioned_error(
                 scope, self.try_inspect(), "expected '{'"
             )
 
         body = self.parse_while_predicate(
             lambda: not self.try_consume(SpecialToken("}")),
             eof_error="Expected '}', got EOF",
             scope=scope,
@@ -207,24 +207,24 @@
         root = CompoundExpression()
 
         while predicate():
             if self.try_consume(CommentToken):
                 continue
 
             if not (instr_token := self.try_consume(IdentifierToken)):
-                raise throw_positioned_syntax_error(
+                raise throw_positioned_error(
                     scope, self.try_inspect(), "expected identifier"
                 )
 
             if scope:
                 scope.last_base_token = instr_token
 
             if instr_token.text not in self.INSTRUCTIONS:
                 if not (instr := self.try_parse_custom_assembly(instr_token, scope)):
-                    raise throw_positioned_syntax_error(
+                    raise throw_positioned_error(
                         scope,
                         instr_token,
                         "expected <assembly instruction name> or <assembly macro name>",
                     )
             else:
                 instr = self.INSTRUCTIONS[instr_token.text].consume(self, scope)
 
@@ -247,21 +247,21 @@
             if self[-1].line != expr.line:
                 continue
 
             if not predicate():
                 if eof_error and self.try_inspect() is None:
                     print(self.try_inspect())
                     print(repr(root))
-                    raise throw_positioned_syntax_error(scope, self[-1], eof_error)
+                    raise throw_positioned_error(scope, self[-1], eof_error)
 
                 break
 
             print(self[-1].line, self[-1], expr.line)
 
-            raise throw_positioned_syntax_error(
+            raise throw_positioned_error(
                 scope,
                 self.try_inspect(),
                 "Expected <newline> or ';' after assembly instruction",
             )
 
         return root
 
@@ -352,15 +352,25 @@
             else:
                 expr = GlobalAccessExpression(
                     self.parse_identifier_like(scope), start_token
                 )
 
         elif start_token.text == "$":
             self.consume(SpecialToken("$"), err_arg=scope)
-            expr = LocalAccessExpression(self.parse_identifier_like(scope), start_token)
+
+            prefix = ""
+
+            while self.try_consume(SpecialToken("|")):
+                prefix += "|"
+
+            if prefix == "":
+                while self.try_consume(SpecialToken(":")):
+                    prefix += ":"
+
+            expr = LocalAccessExpression(self.parse_identifier_like(scope), start_token, prefix=prefix)
 
         elif start_token.text == "§":
             self.consume(SpecialToken("§"), err_arg=scope)
             expr = DerefAccessExpression(self.parse_identifier_like(scope), start_token)
 
         elif start_token.text == "&":
             self.consume(SpecialToken("&"), err_arg=scope)
@@ -393,24 +403,24 @@
             and allow_op
             and "OP" in self.INSTRUCTIONS
             and AbstractOpAssembly.IMPLEMENTATION is not None
         ):
             self.consume(start_token, err_arg=scope)
 
             if not (opening := self.try_consume(SpecialToken("("))):
-                raise throw_positioned_syntax_error(
+                raise throw_positioned_error(
                     scope,
                     self[-1:1],
                     "expected '(' after OP when used in expressions",
                 )
 
             expr = AbstractOpAssembly.IMPLEMENTATION.consume(self, scope)
 
             if not self.try_consume(SpecialToken(")")):
-                raise throw_positioned_syntax_error(
+                raise throw_positioned_error(
                     scope,
                     [opening, self[0]],
                     "expected ')' after operation",
                 )
 
         else:
             return
@@ -423,27 +433,27 @@
                         index := self.try_consume_access_to_value(
                             allow_primitives=True,
                             allow_tos=allow_tos,
                             allow_op=allow_op,
                             scope=scope,
                         )
                     ):
-                        raise throw_positioned_syntax_error(
+                        raise throw_positioned_error(
                             scope,
                             self.try_inspect() or self[-1],
                             "expected <expression>"
                             + (
                                 ""
                                 if not isinstance(self.try_inspect(), IdentifierToken)
                                 else " (did you forget a prefix?)"
                             ),
                         )
 
                     if not self.try_consume(SpecialToken("]")):
-                        raise throw_positioned_syntax_error(
+                        raise throw_positioned_error(
                             scope, self.try_inspect() or self[-1], "expected ']''"
                         )
 
                     expr = SubscriptionAccessExpression(
                         expr,
                         index,
                     )
@@ -455,29 +465,29 @@
                                 allow_primitives=True,
                                 allow_tos=allow_tos,
                                 allow_op=allow_op,
                                 scope=scope,
                                 allow_calls=allow_calls,
                             )
                         ):
-                            raise throw_positioned_syntax_error(
+                            raise throw_positioned_error(
                                 scope,
                                 self.try_inspect() or self[-1],
                                 "expected <expression>"
                                 + (
                                     ""
                                     if not isinstance(
                                         self.try_inspect(), IdentifierToken
                                     )
                                     else " (did you forget a prefix?)"
                                 ),
                             )
 
                         if not self.try_consume(SpecialToken(")")):
-                            raise throw_positioned_syntax_error(
+                            raise throw_positioned_error(
                                 scope,
                                 [opening_bracket, self.try_inspect()],
                                 "expected ')'",
                             )
 
                         expr = DynamicAttributeAccessExpression(expr, index)
 
@@ -549,14 +559,14 @@
         if expr := self.try_consume(IdentifierToken):
             return StaticIdentifier(expr.text, expr)
 
     def parse_identifier_like(self, scope: ParsingScope) -> IIdentifierAccessor:
         identifier = self.try_parse_identifier_like()
 
         if identifier is None:
-            raise throw_positioned_syntax_error(
+            raise throw_positioned_error(
                 scope,
                 self[0],
                 "expected <identifier> or &<identifier>",
             )
 
         return identifier
```

### Comparing `bytecodemanipulation-0.3.1/bytecodemanipulation/assembler/hook.py` & `bytecodemanipulation-0.3.3/bytecodemanipulation/assembler/hook.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.3.1/bytecodemanipulation/assembler/target.py` & `bytecodemanipulation-0.3.3/bytecodemanipulation/assembler/target.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     raise RuntimeError("Function must be annotated first!")
 
 
 def label(name: str):
     raise RuntimeError("Function must be annotated first!")
 
 
-def jump(label_name: str):
+def jump(label_name: str, cond: typing.Any = None):
     raise RuntimeError("Function must be annotated first!")
 
 
 def _raise_macro_direct_call_error():
     raise RuntimeError("Cannot call <macro> with normal call!")
```

### Comparing `bytecodemanipulation-0.3.1/bytecodemanipulation/assembler/util/parser.py` & `bytecodemanipulation-0.3.3/bytecodemanipulation/assembler/util/parser.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.3.1/bytecodemanipulation/assembler/util/tokenizer.py` & `bytecodemanipulation-0.3.3/bytecodemanipulation/assembler/util/tokenizer.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/builtin_spec.py` & `bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/builtin_spec.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,45 +11,45 @@
 
 @register(typing.cast)
 def specialize_typing_cast(container: SpecializationContainer):
     # typing.cast(<type>, <obj>) -> <obj>
     data_type, value = container.get_arg_specifications()
 
     if ASSERT_TYPE_CASTS:
-        nop = Instruction(container.target, -1, Opcodes.NOP)
+        nop = Instruction(Opcodes.NOP)
 
         bytecode = [
             value,
-            Instruction(container.target, -1, Opcodes.DUP_TOP),
-            Instruction(container.target, -1, Opcodes.LOAD_CONST, isinstance),
-            Instruction(container.target, -1, Opcodes.ROT_TWO),
+            Instruction(Opcodes.DUP_TOP),
+            Instruction(Opcodes.LOAD_CONST, isinstance),
+            Instruction(Opcodes.ROT_TWO),
             data_type,
-            Instruction(container.target, -1, Opcodes.CALL_FUNCTION, arg=2),
-            Instruction(container.target, -1, Opcodes.POP_JUMP_IF_TRUE, nop),
+            Instruction(Opcodes.CALL_FUNCTION, arg=2),
+            Instruction(Opcodes.POP_JUMP_IF_TRUE, nop),
             Instruction(
-                container.target, -1, Opcodes.LOAD_CONST, "expected data type '"
+                Opcodes.LOAD_CONST, "expected data type '"
             ),
-            Instruction(container.target, -1, Opcodes.LOAD_CONST, repr),
+            Instruction(Opcodes.LOAD_CONST, repr),
             data_type,
-            Instruction(container.target, -1, Opcodes.CALL_FUNCTION, arg=1),
-            Instruction(container.target, -1, Opcodes.BINARY_ADD),
-            Instruction(container.target, -1, Opcodes.LOAD_CONST, "', but got '"),
-            Instruction(container.target, -1, Opcodes.BINARY_ADD),
-            Instruction(container.target, -1, Opcodes.LOAD_CONST, repr),
-            Instruction(container.target, -1, Opcodes.LOAD_CONST, type),
+            Instruction(Opcodes.CALL_FUNCTION, arg=1),
+            Instruction(Opcodes.BINARY_ADD),
+            Instruction(Opcodes.LOAD_CONST, "', but got '"),
+            Instruction(Opcodes.BINARY_ADD),
+            Instruction(Opcodes.LOAD_CONST, repr),
+            Instruction(Opcodes.LOAD_CONST, type),
             value,
-            Instruction(container.target, -1, Opcodes.CALL_FUNCTION, arg=1),
-            Instruction(container.target, -1, Opcodes.CALL_FUNCTION, arg=1),
-            Instruction(container.target, -1, Opcodes.BINARY_ADD),
-            Instruction(container.target, -1, Opcodes.LOAD_CONST, "'"),
-            Instruction(container.target, -1, Opcodes.BINARY_ADD),
-            Instruction(container.target, -1, Opcodes.LOAD_CONST, ValueError),
-            Instruction(container.target, -1, Opcodes.ROT_TWO),
-            Instruction(container.target, -1, Opcodes.CALL_FUNCTION, arg=1),
-            Instruction(container.target, -1, Opcodes.RAISE_VARARGS, arg=1),
+            Instruction(Opcodes.CALL_FUNCTION, arg=1),
+            Instruction(Opcodes.CALL_FUNCTION, arg=1),
+            Instruction(Opcodes.BINARY_ADD),
+            Instruction(Opcodes.LOAD_CONST, "'"),
+            Instruction(Opcodes.BINARY_ADD),
+            Instruction(Opcodes.LOAD_CONST, ValueError),
+            Instruction(Opcodes.ROT_TWO),
+            Instruction(Opcodes.CALL_FUNCTION, arg=1),
+            Instruction(Opcodes.RAISE_VARARGS, arg=1),
             nop,
         ]
 
         container.replace_call_with_opcodes(bytecode)
         return
 
     container.replace_call_with_arg(value)
@@ -465,10 +465,10 @@
                         )
                     )
                     return
 
             count = args[0].get_normalized_data_instr().arg
             args[0].get_normalized_data_instr().change_opcode(Opcodes.NOP)
             container.replace_call_with_opcodes(
-                [Instruction(None, -1, Opcodes.BINARY_ADD) for _ in range(count - 1)],
+                [Instruction(Opcodes.BINARY_ADD) for _ in range(count - 1)],
                 leave_args_on_stack=True,
             )
```

### Comparing `bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/expressions/AttributeAccessExpression.py` & `bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/expressions/AttributeAccessExpression.py`

 * *Files 5% similar despite different names*

```diff
@@ -32,22 +32,22 @@
     def copy(self) -> "AttributeAccessExpression":
         return AttributeAccessExpression(self.root.copy(), self.name)
 
     def emit_bytecodes(
         self, function: MutableFunction, scope: ParsingScope
     ) -> typing.List[Instruction]:
         return self.root.emit_bytecodes(function, scope) + [
-            Instruction(function, -1, "LOAD_ATTR", self.name(scope))
+            Instruction("LOAD_ATTR", self.name(scope))
         ]
 
     def emit_store_bytecodes(
         self, function: MutableFunction, scope: ParsingScope
     ) -> typing.List[Instruction]:
         return self.root.emit_bytecodes(function, scope) + [
-            Instruction(function, -1, "STORE_ATTR", self.name(scope))
+            Instruction("STORE_ATTR", self.name(scope))
         ]
 
     def visit_parts(
         self,
         visitor: typing.Callable[
             [IAssemblyStructureVisitable, tuple, typing.List[AbstractExpression]],
             typing.Any,
```

### Comparing `bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/expressions/CompoundExpression.py` & `bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/expressions/CompoundExpression.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/expressions/ConstantAccessExpression.py` & `bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/expressions/ConstantAccessExpression.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import copy
 import typing
 
 from bytecodemanipulation.assembler.AbstractBase import AbstractAccessExpression
 from bytecodemanipulation.assembler.AbstractBase import ParsingScope
-from bytecodemanipulation.assembler.syntax_errors import throw_positioned_syntax_error
+from bytecodemanipulation.assembler.syntax_errors import throw_positioned_error
 from bytecodemanipulation.assembler.util.tokenizer import AbstractToken
 from bytecodemanipulation.opcodes.Instruction import Instruction
 from bytecodemanipulation.MutableFunction import MutableFunction
 
 
 class ConstantAccessExpression(AbstractAccessExpression):
     IS_STATIC = True
@@ -24,20 +24,20 @@
 
     def copy(self) -> "AbstractAccessExpression":
         return type(self)(copy.deepcopy(self.value))
 
     def emit_bytecodes(
         self, function: MutableFunction, scope: ParsingScope
     ) -> typing.List[Instruction]:
-        return [Instruction(function, -1, "LOAD_CONST", self.value)]
+        return [Instruction("LOAD_CONST", self.value)]
 
     def emit_store_bytecodes(
         self, function: MutableFunction, scope: ParsingScope
     ) -> typing.List[Instruction]:
-        raise throw_positioned_syntax_error(
+        raise throw_positioned_error(
             scope, self.token, f"Cannot assign to a constant: {self}"
         )
 
     def get_tokens(self) -> typing.Iterable[AbstractToken]:
         return (self.token,)
 
     def evaluate_static_value(self, scope: ParsingScope) -> typing.Any:
```

### Comparing `bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/expressions/DerefAccessExpression.py` & `bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/expressions/GlobalAccessExpression.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,44 +1,45 @@
 import typing
 
 from bytecodemanipulation.assembler.AbstractBase import AbstractAccessExpression
 from bytecodemanipulation.assembler.AbstractBase import ParsingScope
 from bytecodemanipulation.assembler.util.tokenizer import AbstractToken
 from bytecodemanipulation.opcodes.Instruction import Instruction
 from bytecodemanipulation.MutableFunction import MutableFunction
+from bytecodemanipulation.opcodes.Opcodes import Opcodes
 
 
-class DerefAccessExpression(AbstractAccessExpression):
-    PREFIX = "§"
+class GlobalAccessExpression(AbstractAccessExpression):
+    PREFIX = "@"
 
     def emit_bytecodes(
         self, function: MutableFunction, scope: ParsingScope
     ) -> typing.List[Instruction]:
         value = self.get_name(scope)
 
         if value.isdigit():
             value = int(value)
 
         return [
             Instruction.create_with_token(
-                self.token, function, -1, "LOAD_DEREF", value, _decode_next=False
+                self.token, Opcodes.LOAD_GLOBAL, value
             )
         ]
 
     def emit_store_bytecodes(
         self, function: MutableFunction, scope: ParsingScope
     ) -> typing.List[Instruction]:
         value = self.get_name(scope)
 
         if value.isdigit():
             value = int(value)
 
         return [
             Instruction.create_with_token(
-                self.token, function, -1, "STORE_DEREF", value
+                self.token, Opcodes.STORE_GLOBAL, value
             )
         ]
 
     def evaluate_static_value(self, scope: ParsingScope) -> typing.Any:
         raise NotImplementedError  # todo: implement in some cases
 
     def get_tokens(self) -> typing.Iterable[AbstractToken]:
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/expressions/DiscardValueExpression.py` & `bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/expressions/DiscardValueExpression.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,11 +16,11 @@
         self, function: MutableFunction, scope: ParsingScope
     ) -> typing.List[Instruction]:
         raise RuntimeError
 
     def emit_store_bytecodes(
         self, function: MutableFunction, scope: ParsingScope
     ) -> typing.List[Instruction]:
-        return [Instruction(function, -1, Opcodes.POP_TOP)]
+        return [Instruction(Opcodes.POP_TOP)]
 
     def get_tokens(self) -> typing.Iterable[AbstractToken]:
         return (self.token,)
```

### Comparing `bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/expressions/DynamicAccessExpression.py` & `bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/expressions/DynamicAccessExpression.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,30 +31,30 @@
     def copy(self) -> "DynamicAttributeAccessExpression":
         return DynamicAttributeAccessExpression(self.root.copy(), self.name_expr.copy())
 
     def emit_bytecodes(
         self, function: MutableFunction, scope: ParsingScope
     ) -> typing.List[Instruction]:
         return (
-            [Instruction(function, -1, Opcodes.LOAD_CONST, getattr)]
+            [Instruction(Opcodes.LOAD_CONST, getattr)]
             + self.root.emit_bytecodes(function, scope)
             + self.name_expr.emit_bytecodes(function, scope)
-            + [Instruction(function, -1, Opcodes.CALL_FUNCTION, arg=2)]
+            + [Instruction(Opcodes.CALL_FUNCTION, arg=2)]
         )
 
     def emit_store_bytecodes(
         self, function: MutableFunction, scope: ParsingScope
     ) -> typing.List[Instruction]:
         return (
-            [Instruction(function, -1, Opcodes.LOAD_CONST, setattr)]
+            [Instruction(Opcodes.LOAD_CONST, setattr)]
             + self.root.emit_bytecodes(function, scope)
             + self.name_expr.emit_bytecodes(function, scope)
             + [
-                Instruction(function, -1, Opcodes.ROT_THREE),
-                Instruction(function, -1, Opcodes.CALL_FUNCTION, arg=2),
+                Instruction(Opcodes.ROT_THREE),
+                Instruction(Opcodes.CALL_FUNCTION, arg=2),
             ]
         )
 
     def visit_parts(
         self,
         visitor: typing.Callable[
             [IAssemblyStructureVisitable, tuple, typing.List[AbstractExpression]],
```

### Comparing `bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/expressions/GlobalAccessExpression.py` & `bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/expressions/DerefAccessExpression.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,44 +1,45 @@
 import typing
 
 from bytecodemanipulation.assembler.AbstractBase import AbstractAccessExpression
 from bytecodemanipulation.assembler.AbstractBase import ParsingScope
 from bytecodemanipulation.assembler.util.tokenizer import AbstractToken
 from bytecodemanipulation.opcodes.Instruction import Instruction
 from bytecodemanipulation.MutableFunction import MutableFunction
+from bytecodemanipulation.opcodes.Opcodes import Opcodes
 
 
-class GlobalAccessExpression(AbstractAccessExpression):
-    PREFIX = "@"
+class DerefAccessExpression(AbstractAccessExpression):
+    PREFIX = "§"
 
     def emit_bytecodes(
         self, function: MutableFunction, scope: ParsingScope
     ) -> typing.List[Instruction]:
         value = self.get_name(scope)
 
         if value.isdigit():
             value = int(value)
 
         return [
             Instruction.create_with_token(
-                self.token, function, -1, "LOAD_GLOBAL", value
+                self.token, Opcodes.LOAD_DEREF, value
             )
         ]
 
     def emit_store_bytecodes(
         self, function: MutableFunction, scope: ParsingScope
     ) -> typing.List[Instruction]:
         value = self.get_name(scope)
 
         if value.isdigit():
             value = int(value)
 
         return [
             Instruction.create_with_token(
-                self.token, function, -1, "STORE_GLOBAL", value
+                self.token, Opcodes.STORE_DEREF, value
             )
         ]
 
     def evaluate_static_value(self, scope: ParsingScope) -> typing.Any:
         raise NotImplementedError  # todo: implement in some cases
 
     def get_tokens(self) -> typing.Iterable[AbstractToken]:
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/expressions/GlobalStaticAccessExpression.py` & `bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/expressions/GlobalStaticAccessExpression.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import builtins
 import typing
 
 from bytecodemanipulation.assembler.AbstractBase import AbstractAccessExpression
 from bytecodemanipulation.assembler.AbstractBase import ParsingScope
-from bytecodemanipulation.assembler.syntax_errors import throw_positioned_syntax_error
+from bytecodemanipulation.assembler.syntax_errors import throw_positioned_error
 from bytecodemanipulation.assembler.util.tokenizer import AbstractToken
 from bytecodemanipulation.opcodes.Instruction import Instruction
 from bytecodemanipulation.MutableFunction import MutableFunction
+from bytecodemanipulation.opcodes.Opcodes import Opcodes
 
 
 class GlobalStaticAccessExpression(AbstractAccessExpression):
     PREFIX = "@!"
     IS_STATIC = True
 
     def emit_bytecodes(
@@ -20,27 +21,27 @@
         global_dict = function.target.__globals__
         if key not in global_dict and hasattr(builtins, key):
             value = getattr(builtins, key)
         else:
             value = global_dict.get(key)
 
         return [
-            Instruction.create_with_token(self.name, function, -1, "LOAD_CONST", value)
+            Instruction.create_with_token(tuple(self.name.get_tokens())[0], Opcodes.LOAD_CONST, value)
         ]
 
     def emit_store_bytecodes(
         self, function: MutableFunction, scope: ParsingScope
     ) -> typing.List[Instruction]:
         raise RuntimeError("Cannot assign to a constant global")
 
     def evaluate_static_value(self, scope: ParsingScope) -> typing.Any:
         if self.get_name(scope) in scope.globals_dict:
             return scope.globals_dict[self.get_name(scope)]
 
-        raise throw_positioned_syntax_error(
+        raise throw_positioned_error(
             scope,
             self.token,
             f"Name {self.get_name(scope)} not found!",
             NameError,
         )
 
     def get_tokens(self) -> typing.Iterable[AbstractToken]:
```

### Comparing `bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/expressions/LocalAccessExpression.py` & `bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/expressions/MacroAccessExpression.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,43 +1,38 @@
 import typing
 
 from bytecodemanipulation.assembler.AbstractBase import AbstractAccessExpression
 from bytecodemanipulation.assembler.AbstractBase import ParsingScope
 from bytecodemanipulation.assembler.util.tokenizer import AbstractToken
+from bytecodemanipulation.assembler.util.tokenizer import IdentifierToken
 from bytecodemanipulation.opcodes.Instruction import Instruction
 from bytecodemanipulation.MutableFunction import MutableFunction
 
 
-class LocalAccessExpression(AbstractAccessExpression):
-    PREFIX = "$"
-
+class MacroAccessExpression(AbstractAccessExpression):
     def emit_bytecodes(
         self, function: MutableFunction, scope: ParsingScope
     ) -> typing.List[Instruction]:
-        value = self.get_name(scope)
-
-        if value.isdigit():
-            value = int(value)
-
-        return [
-            Instruction.create_with_token(
-                self.token, function, -1, "LOAD_FAST", value, _decode_next=False
-            )
-        ]
+        raise RuntimeError
 
     def emit_store_bytecodes(
         self, function: MutableFunction, scope: ParsingScope
     ) -> typing.List[Instruction]:
-        value = self.get_name(scope)
+        raise RuntimeError
+
+    def __init__(self, name: typing.List[IdentifierToken]):
+        self.name = name
+
+    def __eq__(self, other):
+        return type(self) is type(other) and self.name == other.name
 
-        if value.isdigit():
-            value = int(value)
+    def __repr__(self):
+        return f"MACRO-LINK({':'.join(map(lambda e: e.text, self.name))})"
 
-        return [
-            Instruction.create_with_token(self.token, function, -1, "STORE_FAST", value)
-        ]
+    def copy(self) -> "MacroAccessExpression":
+        return type(self)(self.name.copy())
 
     def evaluate_static_value(self, scope: ParsingScope) -> typing.Any:
         raise NotImplementedError  # todo: implement in some cases
 
     def get_tokens(self) -> typing.Iterable[AbstractToken]:
-        return (self.token,)
+        return self.name
```

### Comparing `bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/expressions/MacroAccessExpression.py` & `bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/expressions/ModuleAccessExpression.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,38 +1,45 @@
+import builtins
+import types
 import typing
 
 from bytecodemanipulation.assembler.AbstractBase import AbstractAccessExpression
 from bytecodemanipulation.assembler.AbstractBase import ParsingScope
 from bytecodemanipulation.assembler.util.tokenizer import AbstractToken
-from bytecodemanipulation.assembler.util.tokenizer import IdentifierToken
 from bytecodemanipulation.opcodes.Instruction import Instruction
 from bytecodemanipulation.MutableFunction import MutableFunction
+from bytecodemanipulation.opcodes.Opcodes import Opcodes
 
 
-class MacroAccessExpression(AbstractAccessExpression):
+class ModuleAccessExpression(AbstractAccessExpression):
+    IS_STATIC = True
+    PREFIX = "~"
+    _CACHE = builtins.__dict__.copy()
+
+    @classmethod
+    def _cached_lookup(cls, module_name: str) -> types.ModuleType:
+        if module_name not in cls._CACHE:
+            module = cls._CACHE[module_name] = __import__(module_name)
+            return module
+
+        return cls._CACHE[module_name]
+
     def emit_bytecodes(
         self, function: MutableFunction, scope: ParsingScope
     ) -> typing.List[Instruction]:
-        raise RuntimeError
+        value = self._cached_lookup(self.get_name(scope))
+        return [
+            Instruction.create_with_token(
+                self.token, Opcodes.LOAD_CONST, value
+            )
+        ]
 
     def emit_store_bytecodes(
         self, function: MutableFunction, scope: ParsingScope
     ) -> typing.List[Instruction]:
         raise RuntimeError
 
-    def __init__(self, name: typing.List[IdentifierToken]):
-        self.name = name
-
-    def __eq__(self, other):
-        return type(self) is type(other) and self.name == other.name
-
-    def __repr__(self):
-        return f"MACRO-LINK({':'.join(map(lambda e: e.text, self.name))})"
-
-    def copy(self) -> "MacroAccessExpression":
-        return type(self)(self.name.copy())
-
     def evaluate_static_value(self, scope: ParsingScope) -> typing.Any:
-        raise NotImplementedError  # todo: implement in some cases
+        return self._cached_lookup(self.get_name(scope))
 
     def get_tokens(self) -> typing.Iterable[AbstractToken]:
-        return self.name
+        return (self.token,)
```

### Comparing `bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/expressions/MacroParameterAcessExpression.py` & `bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/expressions/MacroParameterAcessExpression.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import typing
 
 from bytecodemanipulation.assembler.AbstractBase import AbstractAccessExpression
 from bytecodemanipulation.assembler.AbstractBase import ParsingScope
-from bytecodemanipulation.assembler.syntax_errors import throw_positioned_syntax_error
+from bytecodemanipulation.assembler.syntax_errors import throw_positioned_error
 from bytecodemanipulation.assembler.util.tokenizer import AbstractToken
 from bytecodemanipulation.opcodes.Instruction import Instruction
 from bytecodemanipulation.MutableFunction import MutableFunction
 from bytecodemanipulation.opcodes.Opcodes import Opcodes
 
 
 class MacroParameterAccessExpression(AbstractAccessExpression):
@@ -14,51 +14,63 @@
 
     def emit_bytecodes(
         self, function: MutableFunction, scope: ParsingScope
     ) -> typing.List[Instruction]:
         value = self.get_name(scope)
 
         if value not in scope.macro_parameter_namespace:
-            raise throw_positioned_syntax_error(
+            raise throw_positioned_error(
                 scope, self.token, "Name not found in macro var space"
             )
 
         if scope.macro_parameter_namespace[value] != self and hasattr(
             scope.macro_parameter_namespace[value], "emit_bytecodes"
         ):
-            return scope.macro_parameter_namespace[value].emit_bytecodes(
+            instructions = scope.macro_parameter_namespace[value].emit_bytecodes(
                 function, scope
             )
 
+            for instr in instructions:
+                if instr.has_local():
+                    instr.change_arg_value(":" + instr.arg_value)
+
+            return instructions
+
         return [
             Instruction.create_with_token(
-                self.token, function, -1, Opcodes.MACRO_LOAD_PARAMETER, value
+                self.token, Opcodes.MACRO_LOAD_PARAMETER, value
             )
         ]
 
     def emit_store_bytecodes(
         self, function: MutableFunction, scope: ParsingScope
     ) -> typing.List[Instruction]:
         value = self.get_name(scope)
 
         if value not in scope.macro_parameter_namespace:
-            raise throw_positioned_syntax_error(
+            raise throw_positioned_error(
                 scope, self.token, "Name not found in macro var space"
             )
 
         if scope.macro_parameter_namespace[value] != self and hasattr(
             scope.macro_parameter_namespace[value], "emit_bytecodes"
         ):
-            return scope.macro_parameter_namespace[value].emit_store_bytecodes(
+            instructions = scope.macro_parameter_namespace[value].emit_store_bytecodes(
                 function, scope
             )
 
+            for instr in instructions:
+                if instr.has_local():
+                    instr.change_arg_value(":" + instr.arg_value)
+
+            return instructions
+
         return [
             Instruction.create_with_token(
-                self.token, function, -1, Opcodes.MACRO_STORE_PARAMETER, value
+                self.token, Opcodes.MACRO_STORE_PARAMETER, value
             )
         ]
 
     def evaluate_static_value(self, scope: ParsingScope) -> typing.Any:
         name = self.name(scope)
 
         if name not in scope.macro_parameter_namespace:
```

### Comparing `bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/expressions/ModuleAccessExpression.py` & `bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/instructions/LabelAssembly.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,45 +1,50 @@
-import builtins
-import types
 import typing
 
-from bytecodemanipulation.assembler.AbstractBase import AbstractAccessExpression
+from bytecodemanipulation.assembler.AbstractBase import IIdentifierAccessor
 from bytecodemanipulation.assembler.AbstractBase import ParsingScope
-from bytecodemanipulation.assembler.util.tokenizer import AbstractToken
+from bytecodemanipulation.assembler.AbstractBase import StaticIdentifier
+from bytecodemanipulation.assembler.Parser import Parser
+from bytecodemanipulation.assembler.syntax_errors import throw_positioned_error
+from bytecodemanipulation.data.shared.instructions.AbstractInstruction import (
+    AbstractAssemblyInstruction,
+)
 from bytecodemanipulation.opcodes.Instruction import Instruction
 from bytecodemanipulation.MutableFunction import MutableFunction
 from bytecodemanipulation.opcodes.Opcodes import Opcodes
 
 
-class ModuleAccessExpression(AbstractAccessExpression):
-    IS_STATIC = True
-    PREFIX = "~"
-    _CACHE = builtins.__dict__.copy()
+@Parser.register
+class LabelAssembly(AbstractAssemblyInstruction):
+    # LABEL <name>
+    NAME = "LABEL"
 
     @classmethod
-    def _cached_lookup(cls, module_name: str) -> types.ModuleType:
-        if module_name not in cls._CACHE:
-            module = cls._CACHE[module_name] = __import__(module_name)
-            return module
+    def consume(cls, parser: "Parser", scope: ParsingScope) -> "LabelAssembly":
+        name = parser.try_parse_identifier_like()
 
-        return cls._CACHE[module_name]
-
-    def emit_bytecodes(
-        self, function: MutableFunction, scope: ParsingScope
-    ) -> typing.List[Instruction]:
-        value = self._cached_lookup(self.get_name(scope))
-        return [
-            Instruction.create_with_token(
-                self.token, function, -1, Opcodes.LOAD_CONST, value
+        if name is None:
+            raise throw_positioned_error(
+                scope, parser[0], "expected <identifier like>"
             )
-        ]
 
-    def emit_store_bytecodes(
+        return cls(name)
+
+    def __init__(self, name: IIdentifierAccessor | str):
+        self.name = name if not isinstance(name, str) else StaticIdentifier(name)
+
+    def __repr__(self):
+        return f"LABEL({self.name})"
+
+    def __eq__(self, other):
+        return type(self) == type(other) and self.name == other.name
+
+    def emit_bytecodes(
         self, function: MutableFunction, scope: ParsingScope
     ) -> typing.List[Instruction]:
-        raise RuntimeError
+        return [Instruction(Opcodes.BYTECODE_LABEL, self.name(scope))]
 
-    def evaluate_static_value(self, scope: ParsingScope) -> typing.Any:
-        return self._cached_lookup(self.get_name(scope))
+    def copy(self) -> "LabelAssembly":
+        return type(self)(self.name)
 
-    def get_tokens(self) -> typing.Iterable[AbstractToken]:
-        return (self.token,)
+    def get_labels(self, scope: ParsingScope) -> typing.Set[StaticIdentifier]:
+        return {StaticIdentifier(self.name(scope))}
```

### Comparing `bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/expressions/StaticAttributeAcccessExpression.py` & `bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/expressions/StaticAttributeAcccessExpression.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import typing
 
 from bytecodemanipulation.assembler.AbstractBase import AbstractAccessExpression
 from bytecodemanipulation.assembler.AbstractBase import IAssemblyStructureVisitable
 from bytecodemanipulation.assembler.AbstractBase import ParsingScope
 from bytecodemanipulation.assembler.util.parser import AbstractExpression
 from bytecodemanipulation.assembler.util.tokenizer import AbstractToken
-from bytecodemanipulation.assembler.util.tokenizer import IdentifierToken
 from bytecodemanipulation.opcodes.Instruction import Instruction
 from bytecodemanipulation.MutableFunction import MutableFunction
 from bytecodemanipulation.assembler.AbstractBase import (
     IIdentifierAccessor,
     StaticIdentifier,
 )
+from bytecodemanipulation.opcodes.Opcodes import Opcodes
 
 
 class StaticAttributeAccessExpression(AbstractAccessExpression):
     IS_STATIC = True
 
     def __init__(
         self,
@@ -39,18 +39,16 @@
         return StaticAttributeAccessExpression(self.root.copy(), self.name)
 
     def emit_bytecodes(
         self, function: MutableFunction, scope: ParsingScope
     ) -> typing.List[Instruction]:
         return self.root.emit_bytecodes(function, scope) + [
             Instruction.create_with_token(
-                self.name(scope),
-                function,
-                -1,
-                "STATIC_ATTRIBUTE_ACCESS",
+                tuple(self.name.get_tokens())[0],
+                Opcodes.STATIC_ATTRIBUTE_ACCESS,
                 self.name(scope),
             )
         ]
 
     def emit_store_bytecodes(
         self, function: MutableFunction, scope: ParsingScope
     ) -> typing.List[Instruction]:
```

### Comparing `bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/expressions/SubscriptionAccessExpression.py` & `bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/expressions/SubscriptionAccessExpression.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,45 +42,41 @@
             self.base_expr.emit_bytecodes(function, scope)
             + (
                 self.index_expr.emit_bytecodes(function, scope)
                 if isinstance(self.index_expr, AbstractAccessExpression)
                 else [
                     Instruction.create_with_token(
                         self.index_expr,
-                        function,
-                        -1,
-                        "LOAD_CONST",
+                        Opcodes.LOAD_CONST,
                         int(self.index_expr.text),
                     )
                 ]
             )
-            + [Instruction(function, -1, Opcodes.BINARY_SUBSCR)]
+            + [Instruction(Opcodes.BINARY_SUBSCR)]
         )
 
     def emit_store_bytecodes(
         self, function: MutableFunction, scope: ParsingScope
     ) -> typing.List[Instruction]:
         return (
             self.base_expr.emit_bytecodes(function, scope)
             + (
                 self.index_expr.emit_bytecodes(function, scope)
                 if isinstance(self.index_expr, AbstractAccessExpression)
                 else [
                     Instruction.create_with_token(
                         self.index_expr,
-                        function,
-                        -1,
-                        "LOAD_CONST",
+                        Opcodes.LOAD_CONST,
                         int(self.index_expr.text),
                     )
                 ]
             )
             + [
                 Instruction.create_with_token(
-                    self.name(scope), function, -1, Opcodes.STORE_SUBSCR
+                    self.name(scope), Opcodes.STORE_SUBSCR
                 )
             ]
         )
 
     def visit_parts(
         self,
         visitor: typing.Callable[
```

### Comparing `bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/expressions/TopOfStackAccessExpression.py` & `bytecodemanipulation-0.3.3/bytecodemanipulation/data/v3_11/instructions/IfAssembly.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,52 +1,46 @@
-import typing
-
-from bytecodemanipulation.assembler.util.tokenizer import AbstractToken
-from bytecodemanipulation.opcodes.Opcodes import Opcodes
-
-from bytecodemanipulation.assembler.AbstractBase import AbstractAccessExpression
+from bytecodemanipulation.assembler.Parser import Parser
 from bytecodemanipulation.assembler.AbstractBase import ParsingScope
+from bytecodemanipulation.data.shared.instructions.IfAssembly import AbstractIFAssembly
 from bytecodemanipulation.opcodes.Instruction import Instruction
 from bytecodemanipulation.MutableFunction import MutableFunction
+from bytecodemanipulation.opcodes.Opcodes import Opcodes
 
 
-class TopOfStackAccessExpression(AbstractAccessExpression):
-    PREFIX = "%"
-
-    def __init__(self, token=None, offset=0):
-        self.token = token
-        self.offset = offset
-
-    def __eq__(self, other):
-        return type(self) == type(other)
-
-    def __repr__(self):
-        return f"%"
-
-    def copy(self) -> "AbstractAccessExpression":
-        return type(self)(self.token)
-
-    def emit_bytecodes(
-        self, function: MutableFunction, scope: ParsingScope
-    ) -> typing.List[Instruction]:
-        if self.offset != 0:
-            return [
-                Instruction(function, -1, Opcodes.ROT_N, arg=self.offset)
-                for _ in range(self.offset - 1)
-            ] + [
-                Instruction(function, -1, Opcodes.DUP_TOP),
-                Instruction(function, -1, Opcodes.ROT_TWO),
-                Instruction(function, -1, Opcodes.ROT_N, arg=self.offset),
-            ]
-
-        return []
-
-    def emit_store_bytecodes(
-        self, function: MutableFunction, scope: ParsingScope
-    ) -> typing.List[Instruction]:
-        if self.offset != 0:
-            raise NotImplementedError("%<n> as store target")
-
-        return []
-
-    def get_tokens(self) -> typing.Iterable[AbstractToken]:
-        return (self.token,)
+@Parser.register
+class IFAssembly(AbstractIFAssembly):
+    def emit_bytecodes(self, function: MutableFunction, scope: ParsingScope):
+
+        if self.label_name is None:
+            end = Instruction("NOP")
+        else:
+            end = Instruction(
+                function, -1, Opcodes.BYTECODE_LABEL, self.label_name.text + "_END"
+            )
+
+        return (
+            (
+                []
+                if self.label_name is None
+                else [
+                    Instruction(
+                        function,
+                        -1,
+                        Opcodes.BYTECODE_LABEL,
+                        self.label_name.text + "_HEAD",
+                    )
+                ]
+            )
+            + self.source.emit_bytecodes(function, scope)
+            + [Instruction("POP_JUMP_IF_FALSE", end)]
+            + (
+                []
+                if self.label_name is None
+                else [
+                    Instruction(
+                        function, -1, Opcodes.BYTECODE_LABEL, self.label_name.text
+                    )
+                ]
+            )
+            + self.body.emit_bytecodes(function, scope)
+            + [end]
+        )
```

### Comparing `bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/instructions/AbstractInstruction.py` & `bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/instructions/AbstractInstruction.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,15 @@
     ) -> "AbstractAssemblyInstruction":
         """
         Tries to consume the instruction from the token stream in 'parser'
         in the given 'scope', and returns the instruction instance
 
         TODO: do we want to allow to return multiple instructions without using an CompoundExpression?
 
-        For coders implementing this function: use the throw_positioned_syntax_error(...) function
+        For coders implementing this function: use the throw_positioned_error(...) function
         for printing fancy error messages with source code location (use e.g. parser[0] for the token)
 
         :param parser: the Parser instance to use
         :param scope: the ParsingScope to use
         :return: the AbstractAssemblyInstruction instance
         :raises SyntaxError: when syntactically errors occurred
         :raises NameError: when a name is accessed which is not known (e.g. macro names)
```

### Comparing `bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/instructions/AssertAssembly.py` & `bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/instructions/AssertAssembly.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from abc import ABC
 
 from bytecodemanipulation.assembler.AbstractBase import (
     ParsingScope,
     AbstractSourceExpression,
 )
-from bytecodemanipulation.assembler.syntax_errors import throw_positioned_syntax_error
+from bytecodemanipulation.assembler.syntax_errors import throw_positioned_error
 from bytecodemanipulation.data.shared.instructions.AbstractInstruction import (
     AbstractAssemblyInstruction,
 )
 from bytecodemanipulation.assembler.Parser import Parser
 
 
 class AbstractAssertAssembly(AbstractAssemblyInstruction, ABC):
@@ -16,15 +16,15 @@
     NAME = "ASSERT"
 
     @classmethod
     def consume(cls, parser: "Parser", scope: ParsingScope) -> "AbstractAssertAssembly":
         target = parser.try_consume_access_to_value(scope=scope, allow_primitives=True)
 
         if target is None:
-            raise throw_positioned_syntax_error(
+            raise throw_positioned_error(
                 scope, parser[0], "expected <expression>"
             )
 
         return cls(
             target,
             parser.try_consume_access_to_value(scope=scope, allow_primitives=True),
         )
```

### Comparing `bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/instructions/AssertStaticInstruction.py` & `bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/instructions/AssertStaticInstruction.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,42 +1,54 @@
 import typing
+import warnings
 
 from bytecodemanipulation.assembler.AbstractBase import AbstractSourceExpression
 from bytecodemanipulation.assembler.AbstractBase import ParsingScope
-from bytecodemanipulation.assembler.syntax_errors import throw_positioned_syntax_error
+from bytecodemanipulation.assembler.syntax_errors import print_positional_warning
+from bytecodemanipulation.assembler.syntax_errors import throw_positioned_error
+from bytecodemanipulation.assembler.util.tokenizer import AbstractToken
 from bytecodemanipulation.data.shared.instructions.AbstractInstruction import (
     AbstractAssemblyInstruction,
 )
 from bytecodemanipulation.opcodes.Instruction import Instruction
 from bytecodemanipulation.MutableFunction import MutableFunction
 
 
+if typing.TYPE_CHECKING:
+    from bytecodemanipulation.assembler.Parser import Parser
+    from bytecodemanipulation.data.shared.instructions.AbstractInstruction import AbstractAssemblyInstruction
+
+
 class AssertStaticInstruction(AbstractAssemblyInstruction):
     # ASSERT_STATIC <expression> [<message>]
     NAME = "ASSERT_STATIC"
 
     @classmethod
     def consume(cls, parser: "Parser", scope: ParsingScope) -> "AbstractAssertAssembly":
         target = parser.try_consume_access_to_value(scope=scope, allow_primitives=True)
 
         if target is None:
-            raise throw_positioned_syntax_error(
+            raise throw_positioned_error(
                 scope, parser[0], "expected <expression>"
             )
 
         return cls(
             target,
             parser.try_consume_access_to_value(scope=scope, allow_primitives=True),
+            base_token=scope.last_base_token,
         )
 
     def __init__(
-        self, source: AbstractSourceExpression, text: AbstractSourceExpression = None
+        self, source: AbstractSourceExpression,
+        text: AbstractSourceExpression = None,
+        base_token: AbstractToken = None,
     ):
         self.source = source
         self.text = text
+        self.base_token = base_token
 
     def __repr__(self):
         return f"ASSERT({self.source}, {self.text})"
 
     def __eq__(self, other):
         return (
             type(self) == type(other)
@@ -49,31 +61,39 @@
 
     def emit_bytecodes(
         self, function: MutableFunction, scope: ParsingScope
     ) -> typing.List[Instruction]:
         try:
             value = self.source.evaluate_static_value(scope)
         except NotImplementedError:
-            raise throw_positioned_syntax_error(
+            print("<target>:", self.source)
+
+            raise throw_positioned_error(
                 scope,
-                list(self.source.get_tokens()),
-                "Expected <static evaluate-able>",
+                self.base_token or list(self.source.get_tokens()),
+                "Expected <static evaluate-able at 'expression'>",
             ) from None
 
         if not value:
             try:
                 message = (
                     "expected <true-ish value>"
                     if self.text is None
                     else self.text.evaluate_static_value(scope)
                 )
             except NotImplementedError:
+                print_positional_warning(
+                    scope,
+                    list(self.source.get_tokens()),
+                    f"<message> could not be evaluated (got syntax element: {self.text})",
+                )
+
                 message = "expected <true-ish value> (message not arrival)"
 
-            raise throw_positioned_syntax_error(
+            raise throw_positioned_error(
                 scope,
                 list(self.source.get_tokens()),
                 f"assertion failed: {message}",
                 AssertionError,
             )
 
         return []
```

### Comparing `bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/instructions/CallAssembly.py` & `bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/instructions/CallAssembly.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 import typing
 from abc import ABC
 
 from bytecodemanipulation.assembler.AbstractBase import AbstractAccessExpression
+from bytecodemanipulation.assembler.AbstractBase import IIdentifierAccessor, StaticIdentifier
 from bytecodemanipulation.assembler.AbstractBase import ParsingScope
+from bytecodemanipulation.assembler.util.tokenizer import AbstractToken
 from bytecodemanipulation.data.shared.instructions.AbstractInstruction import (
     AbstractAssemblyInstruction,
 )
 from bytecodemanipulation.assembler.util.tokenizer import IdentifierToken
 from bytecodemanipulation.assembler.AbstractBase import IAssemblyStructureVisitable
 from bytecodemanipulation.MutableFunction import MutableFunction
 from bytecodemanipulation.opcodes.Instruction import Instruction
 from bytecodemanipulation.assembler.AbstractBase import AbstractSourceExpression
 from bytecodemanipulation.assembler.Lexer import SpecialToken
 from bytecodemanipulation.data.shared.expressions.MacroAccessExpression import (
     MacroAccessExpression,
 )
-from bytecodemanipulation.assembler.syntax_errors import throw_positioned_syntax_error
+from bytecodemanipulation.assembler.syntax_errors import throw_positioned_error
 from bytecodemanipulation.assembler.util.parser import AbstractExpression
 
 
 if typing.TYPE_CHECKING:
     from bytecodemanipulation.assembler.Parser import Parser
 
 
@@ -33,19 +35,21 @@
         Nothing is abstract, but most requires a special subclass
         """
 
         __slots__ = ("source", "is_dynamic")
 
         def __init__(
             self,
-            source: typing.Union["AbstractAccessExpression", IdentifierToken],
+            source: typing.Union["AbstractAccessExpression", IIdentifierAccessor],
             is_dynamic: bool = False,
+            token: AbstractToken =None,
         ):
             self.source = source
             self.is_dynamic = is_dynamic
+            self.token = token
 
         def __repr__(self):
             return f"{type(self).__name__}{'' if not self.is_dynamic else 'Dynamic'}({self.source})"
 
         def __eq__(self, other):
             return (
                 type(self) == type(other)
@@ -88,23 +92,24 @@
         pass
 
     class KwArg(IArg):
         __slots__ = ("key", "source", "is_dynamic")
 
         def __init__(
             self,
-            key: IdentifierToken | str,
+            key: IIdentifierAccessor | str,
             source: typing.Union["AbstractAccessExpression", IdentifierToken],
             is_dynamic: bool = False,
+            token: AbstractToken = None,
         ):
-            self.key = key if isinstance(key, IdentifierToken) else IdentifierToken(key)
-            super().__init__(source, is_dynamic=is_dynamic)
+            self.key = key if not isinstance(key, str) else StaticIdentifier(key)
+            super().__init__(source, is_dynamic=is_dynamic, token=token)
 
         def __repr__(self):
-            return f"{type(self).__name__}{'' if not self.is_dynamic else 'Dynamic'}({self.key.text} = {self.source})"
+            return f"{type(self).__name__}{'' if not self.is_dynamic else 'Dynamic'}({self.key(None)} = {self.source})"
 
         def __eq__(self, other):
             return (
                 type(self) == type(other)
                 and self.source == other.source
                 and self.key == other.key
                 and self.is_dynamic == other.is_dynamic
@@ -142,14 +147,15 @@
     def consume(cls, parser: "Parser", scope) -> "AbstractCallAssembly":
         """
         The normal consumer for the instruction
         Optionally consumes the PARTIAL and MACRO prefixes
         """
         is_partial = bool(parser.try_consume(IdentifierToken("PARTIAL")))
         is_macro = not is_partial and bool(parser.try_consume(IdentifierToken("MACRO")))
+
         return cls.consume_inner(parser, is_partial, is_macro, scope)
 
     @classmethod
     def consume_inner(
         cls,
         parser: "Parser",
         is_partial: bool,
@@ -164,46 +170,77 @@
         if call_target is None:
             if not is_macro:
                 call_target = parser.try_parse_data_source(
                     include_bracket=False, scope=scope, allow_calls=False
                 )
 
                 if isinstance(call_target, AbstractCallAssembly):
-                    raise RuntimeError
+                    # should not be reachable
+
+                    raise throw_positioned_error(
+                        scope,
+                        list(call_target.get_tokens()),
+                        "Must be not <call assembly> (internal error)",
+                        RuntimeError,
+                    )
 
             else:
                 name = [parser.consume(IdentifierToken, err_arg=scope)]
 
-                while parser.try_consume(SpecialToken(":")):
-                    name.append(parser.consume(IdentifierToken, err_arg=scope))
+                while expr := parser.try_consume(SpecialToken(":")):
+                    # todo: allow identifier-like
+                    part = parser.try_consume(IdentifierToken)
+
+                    if part is None:
+                        raise throw_positioned_error(
+                            scope,
+                            [expr, parser[0]],
+                            "<identifier> expected after '.'",
+                        )
+
+                    name.append(part)
 
                 call_target = MacroAccessExpression(name)
 
         if call_target is None:
-            raise throw_positioned_syntax_error(
+            # should be unreachable
+
+            raise throw_positioned_error(
                 scope,
                 parser.try_inspect(),
                 "expected <expression> to be called (did you forget the prefix?)"
                 if not is_macro
                 else "expected <macro name>",
             )
 
         args: typing.List[AbstractCallAssembly.IArg] = []
 
-        parser.consume(SpecialToken("("), err_arg=scope)
+        if not (opening_bracket := parser.try_consume(SpecialToken("("))):
+            raise throw_positioned_error(
+                scope,
+                parser[0],
+                "Expected '(' after <call target>",
+            )
 
         has_seen_keyword_arg = False
 
         while not (bracket := parser.try_consume(SpecialToken(")"))):
-            if (
-                isinstance(parser[0], IdentifierToken)
-                and parser[1] == SpecialToken("=")
-                and not is_macro
-            ):
-                key = parser.consume(IdentifierToken)
+            parser.save()
+
+            identifier = parser.try_parse_identifier_like()
+            is_keyword = identifier and parser.try_inspect() == SpecialToken("=") and not is_macro
+
+            if is_keyword:
+                parser.discard_save()
+            else:
+                parser.rollback()
+
+            if is_keyword:
+                key = identifier
+
                 parser.consume(SpecialToken("="))
 
                 is_dynamic = is_partial and bool(parser.try_consume(SpecialToken("?")))
 
                 expr = parser.try_parse_data_source(
                     allow_primitives=True, include_bracket=False
                 )
@@ -226,63 +263,77 @@
                     parser.consume(SpecialToken("*"))
                     expr = parser.try_parse_data_source(
                         allow_primitives=True, include_bracket=False
                     )
                     args.append(AbstractCallAssembly.StarArg(expr))
 
                 else:
-                    raise throw_positioned_syntax_error(
+                    raise throw_positioned_error(
                         scope,
                         parser.try_inspect(),
                         "*<arg> only allowed before keyword arguments!",
                     )
 
             elif not has_seen_keyword_arg:
+                # todo: maybe parse here also partial variable names
                 if is_macro and parser[0] == SpecialToken("{"):
                     expr = parser.parse_body(scope=scope)
                     is_dynamic = False
+
                 else:
                     is_dynamic = is_partial and bool(
                         parser.try_consume(SpecialToken("?"))
                     )
 
                     expr = parser.try_consume_access_to_value(allow_primitives=True)
 
                     if expr is None:
                         if parser[0] == SpecialToken(")"):
                             break
 
-                        raise throw_positioned_syntax_error(
+                        raise throw_positioned_error(
                             scope, parser[0], "<expression> expected"
                         )
 
                 args.append(AbstractCallAssembly.Arg(expr, is_dynamic))
 
             else:
-                raise throw_positioned_syntax_error(
+                raise throw_positioned_error(
                     scope,
                     parser.try_inspect(),
                     "pure <arg> only allowed before keyword arguments",
                 )
 
             if not parser.try_consume(SpecialToken(",")):
                 break
 
         if bracket is None and not parser.try_consume(SpecialToken(")")):
-            raise throw_positioned_syntax_error(
-                scope, parser.try_inspect(), "expected ')'"
+            raise throw_positioned_error(
+                scope,
+                [opening_bracket, parser[0]],
+                "expected ')' matching '('",
             )
 
-        if allow_target and parser.try_consume_multi(
-            [
-                SpecialToken("-"),
-                SpecialToken(">"),
-            ]
-        ):
+        if allow_target and (arrow_0 := parser.try_consume(SpecialToken("-"))):
+
+            if not (arrow_1 := parser.try_consume(SpecialToken(">"))):
+                raise throw_positioned_error(
+                    scope,
+                    [arrow_0, parser[0]],
+                    "expected '>' after '-' to fill out <target> expression",
+                )
+
             target = parser.try_consume_access_to_value(scope=scope)
+
+            if target is None:
+                raise throw_positioned_error(
+                    scope,
+                    [arrow_0, arrow_1],
+                    "expected <target> expression after '->'",
+                )
         else:
             target = None
 
         return cls(call_target, args, target, is_partial, is_macro)
 
     def __init__(
         self,
```

### Comparing `bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/instructions/ClassDefinitionAssembly.py` & `bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/instructions/ClassDefinitionAssembly.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from bytecodemanipulation.assembler.AbstractBase import (
     ParsingScope,
     IAssemblyStructureVisitable,
     AbstractExpression,
 )
 from bytecodemanipulation.assembler.Lexer import SpecialToken
 from bytecodemanipulation.assembler.Parser import Parser
-from bytecodemanipulation.assembler.syntax_errors import throw_positioned_syntax_error
+from bytecodemanipulation.assembler.syntax_errors import throw_positioned_error
 from bytecodemanipulation.assembler.util.tokenizer import IdentifierToken
 from bytecodemanipulation.data.shared.expressions.ConstantAccessExpression import (
     ConstantAccessExpression,
 )
 from bytecodemanipulation.data.shared.instructions.AbstractInstruction import (
     AbstractAssemblyInstruction,
 )
@@ -51,23 +51,23 @@
 
                 while parser.try_consume(SpecialToken(",")):
                     if parser[0] == SpecialToken(")"):
                         break
 
                     parent = parser.try_consume_access_to_value()
                     if parent is None:
-                        raise throw_positioned_syntax_error(
+                        raise throw_positioned_error(
                             scope,
                             parser[0],
                             "Expected <expression>",
                         )
                     parents.append(parent)
 
             if not parser.try_consume(SpecialToken(")")):
-                raise throw_positioned_syntax_error(scope, parser[0], "Expected ')'")
+                raise throw_positioned_error(scope, parser[0], "Expected ')'")
 
         if not parents:
             parents = [ConstantAccessExpression(object)]
 
         code_block = parser.parse_body(scope=scope, namespace_part=namespace)
         return cls(
             name,
```

### Comparing `bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/instructions/ForEachAssembly.py` & `bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/instructions/ForEachAssembly.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import abc
 import itertools
 import typing
 
 from bytecodemanipulation.assembler.AbstractBase import ParsingScope
 from bytecodemanipulation.assembler.Lexer import SpecialToken
 from bytecodemanipulation.assembler.Parser import Parser
-from bytecodemanipulation.assembler.syntax_errors import throw_positioned_syntax_error
+from bytecodemanipulation.assembler.syntax_errors import throw_positioned_error
 from bytecodemanipulation.assembler.util.tokenizer import IdentifierToken
 from bytecodemanipulation.data.shared.instructions.AbstractInstruction import (
     AbstractAssemblyInstruction,
 )
 from bytecodemanipulation.assembler.AbstractBase import AbstractAccessExpression
 from bytecodemanipulation.MutableFunction import MutableFunction
 from bytecodemanipulation.opcodes.Instruction import Instruction
@@ -27,64 +27,64 @@
         def __init__(self, *items: AbstractAccessExpression):
             self.items = list(items)
 
         def emit_bytecodes(
             self, function: MutableFunction, scope: ParsingScope
         ) -> typing.List[Instruction]:
             bytecode = [
-                Instruction(function, -1, Opcodes.LOAD_CONST, itertools.product),
+                Instruction(Opcodes.LOAD_CONST, itertools.product),
             ]
 
             for item in self.items:
                 bytecode += item.emit_bytecodes(function, scope)
 
             bytecode += [
-                Instruction(function, -1, Opcodes.CALL_FUNCTION, arg=len(self.items)),
+                Instruction(Opcodes.CALL_FUNCTION, arg=len(self.items)),
             ]
             return bytecode
 
     @classmethod
     def consume(
         cls, parser: "Parser", scope: ParsingScope
     ) -> "AbstractForEachAssembly":
         initial = parser.try_consume_access_to_value()
         if initial is None:
-            raise throw_positioned_syntax_error(
+            raise throw_positioned_error(
                 scope, parser[0], "<expression> expected"
             )
         variables = [initial]
 
         while parser.try_consume(SpecialToken(",")):
 
             expr = parser.try_consume_access_to_value()
 
             if expr is None:
-                raise throw_positioned_syntax_error(
+                raise throw_positioned_error(
                     scope, parser[0], "<expression> expected"
                 )
 
             variables.append(expr)
 
         if not parser.try_consume(IdentifierToken("IN")):
-            raise throw_positioned_syntax_error(scope, parser[0], "'IN' expected")
+            raise throw_positioned_error(scope, parser[0], "'IN' expected")
 
         source = parser.try_consume_access_to_value()
         if not source:
-            raise throw_positioned_syntax_error(
+            raise throw_positioned_error(
                 scope, parser[0], "<expression> expected"
             )
         sources = [source]
 
         multi = None
         while parser.try_consume(SpecialToken(",")) or (
             multi := parser.try_consume(SpecialToken("*"))
         ):
             source = parser.try_consume_access_to_value()
             if not source:
-                raise throw_positioned_syntax_error(
+                raise throw_positioned_error(
                     scope, parser[0], "<expression> expected"
                 )
 
             if multi:
                 s = sources[-1]
 
                 if isinstance(s, cls.ForEachMultiplier):
@@ -93,15 +93,15 @@
                     sources[-1] = cls.ForEachMultiplier(s, source)
 
                 multi = None
             else:
                 sources.append(source)
 
         if len(variables) != len(sources):
-            raise throw_positioned_syntax_error(
+            raise throw_positioned_error(
                 scope,
                 scope.last_base_token,
                 f"Number of Variables ({len(variables)}) must equal number of Sources ({len(sources)})",
             )
 
         body = parser.parse_body(scope=scope)
         return cls(
```

### Comparing `bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/instructions/FunctionDefinitionAssembly.py` & `bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/instructions/FunctionDefinitionAssembly.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from bytecodemanipulation.assembler.AbstractBase import IAssemblyStructureVisitable
 from bytecodemanipulation.assembler.AbstractBase import IIdentifierAccessor
 from bytecodemanipulation.assembler.AbstractBase import ParsingScope
 from bytecodemanipulation.assembler.AbstractBase import StaticIdentifier
 from bytecodemanipulation.assembler.Lexer import SpecialToken
 from bytecodemanipulation.assembler.Parser import Parser
-from bytecodemanipulation.assembler.syntax_errors import throw_positioned_syntax_error
+from bytecodemanipulation.assembler.syntax_errors import throw_positioned_error
 from bytecodemanipulation.assembler.util.parser import AbstractExpression
 from bytecodemanipulation.assembler.util.tokenizer import IdentifierToken
 from bytecodemanipulation.data.shared.instructions.AbstractInstruction import (
     AbstractAssemblyInstruction,
 )
 from bytecodemanipulation.data.shared.instructions.CallAssembly import (
     AbstractCallAssembly,
@@ -26,14 +26,23 @@
     # DEF [<func name>] ['<' ['!'] <bound variables> '>'] '(' <signature> ')' ['->' <target>] '{' <body> '}'
     NAME = "DEF"
 
     @classmethod
     def consume(
         cls, parser: "Parser", scope: ParsingScope
     ) -> "AbstractFunctionDefinitionAssembly":
+        prefix = ""
+
+        while parser.try_consume(SpecialToken("|")):
+            prefix += "|"
+
+        if prefix == "":
+            while parser.try_consume(SpecialToken(":")):
+                prefix += ":"
+
         func_name = parser.parse_identifier_like(scope)
 
         bound_variables: typing.List[typing.Tuple[IIdentifierAccessor, bool]] = []
         args = []
 
         if parser.try_consume(SpecialToken("<")):
             is_static = bool(parser.try_consume(SpecialToken("!")))
@@ -49,93 +58,132 @@
                     ):
                         break
 
                     bound_variables.append((expr, is_static))
 
             parser.consume(SpecialToken(">"), err_arg=scope)
 
-        parser.consume(SpecialToken("("), err_arg=scope)
+        if (opening_bracket := parser.try_consume(SpecialToken("("))) is None:
+            raise throw_positioned_error(
+                scope,
+                parser[0],
+                "expected '(' after <identifier>"
+            )
 
         while parser.try_inspect() != SpecialToken(")"):
             arg = None
 
             star = parser.try_consume(SpecialToken("*"))
             star_star = parser.try_consume(SpecialToken("*"))
-            identifier = parser.try_consume(IdentifierToken)
+            identifier = parser.try_parse_identifier_like()
 
             if not identifier:
                 if star:
-                    raise throw_positioned_syntax_error(
+                    raise throw_positioned_error(
                         scope,
                         [star, star_star],
-                        "Expected <expression> after '*'"
+                        "Expected <identifier> after '*'"
                         if not star_star
-                        else "Expected <expression> after '**'",
+                        else "Expected <identifier> after '**'",
                     )
 
                 break
 
             if not star:
-                if parser.try_consume(SpecialToken("=")):
+                if equal_sign := parser.try_consume(SpecialToken("=")):
                     default_value = parser.try_parse_data_source(
                         allow_primitives=True, include_bracket=False, allow_op=True
                     )
 
                     if default_value is None:
-                        raise SyntaxError
+                        raise throw_positioned_error(
+                            scope,
+                            [identifier, equal_sign, parser[0]],
+                            "expected <expression>",
+                        )
 
-                    arg = AbstractCallAssembly.KwArg(identifier, default_value)
+                    arg = AbstractCallAssembly.KwArg(identifier, default_value, token=identifier)
 
             if not arg:
                 if star_star:
-                    arg = AbstractCallAssembly.KwArgStar(identifier)
+                    arg = AbstractCallAssembly.KwArgStar(identifier, token=identifier)
+
                 elif star:
-                    arg = AbstractCallAssembly.StarArg(identifier)
+                    arg = AbstractCallAssembly.StarArg(identifier, token=identifier)
+
                 else:
-                    arg = AbstractCallAssembly.Arg(identifier)
+                    arg = AbstractCallAssembly.Arg(identifier, token=identifier)
 
             args.append(arg)
 
             if not parser.try_consume(SpecialToken(",")):
                 break
 
-        parser.consume(SpecialToken(")"))
+        if not parser.try_consume(SpecialToken(")")):
+            raise throw_positioned_error(
+                scope,
+                [opening_bracket, parser[0]],
+                "expected ')' matching '(' in function definition",
+            )
 
         if expr := parser.try_consume(SpecialToken("<")):
-            raise throw_positioned_syntax_error(
+            if bound_variables:
+                raise throw_positioned_error(
+                    scope,
+                    expr,
+                    "got '<' after '(' ... ')' expression, where a '{' ... '}' (code block) was expected"
+                )
+
+            raise throw_positioned_error(
                 scope,
                 expr,
                 "Respect ordering (got 'args' before 'captured'): DEF ['name'] ['captured'] ('args') [-> 'target'] { code }",
             )
 
-        if parser.try_consume(SpecialToken("-")) and parser.try_consume(
+        if (arrow_0 := parser.try_consume(SpecialToken("-"))) and (arrow_1 := parser.try_consume(
             SpecialToken(">")
-        ):
+        )):
             target = parser.try_consume_access_to_value(scope=scope)
+
+            if target is None:
+                raise throw_positioned_error(
+                    scope,
+                    [arrow_0, arrow_1, parser[0]],
+                    "expected <expression> after '->' as target"
+                )
+
+        elif arrow_0:
+            raise throw_positioned_error(
+                scope,
+                [arrow_0, parser[0]],
+                "expected '>' after '-' to complete <target> expression",
+            )
+
         else:
             target = None
 
         body = parser.parse_body(scope=scope)
 
         if expr := parser.try_consume(SpecialToken("-")):
-            raise throw_positioned_syntax_error(
+            raise throw_positioned_error(
                 scope,
                 expr,
                 "Respect ordering (got 'code' before 'target'): DEF ['name'] ['captured'] ('args') [-> 'target'] { code }",
             )
 
-        return cls(func_name, bound_variables, args, body, target)
+        return cls(func_name, bound_variables, args, body, target, prefix=prefix)
 
     def __init__(
         self,
         func_name: IIdentifierAccessor | str | None,
         bound_variables: typing.List[typing.Tuple[IIdentifierAccessor, bool] | str],
         args: typing.List[AbstractCallAssembly.IArg],
         body: CompoundExpression,
         target: AbstractAccessExpression | None = None,
+        prefix="",
     ):
         self.func_name = (
             func_name if not isinstance(func_name, str) else StaticIdentifier(func_name)
         )
         self.bound_variables: typing.List[typing.Tuple[IIdentifierAccessor, bool]] = []
         # var if isinstance(var, IdentifierToken) else IdentifierToken(var) for var in bound_variables]
 
@@ -159,14 +207,15 @@
                     self.bound_variables.append(element)
             else:
                 raise ValueError(element)
 
         self.args = args
         self.body = body
         self.target = target
+        self.prefix = prefix
 
     def visit_parts(
         self,
         visitor: typing.Callable[
             [IAssemblyStructureVisitable, tuple, typing.List[AbstractExpression]],
             typing.Any,
         ],
@@ -188,17 +237,18 @@
             and self.bound_variables == other.bound_variables
             and self.args == other.args
             and self.body == other.body
             and self.target == other.target
         )
 
     def __repr__(self):
-        return f"DEF({self.func_name}<{repr([(name[0](None), name[1]) for name in self.bound_variables])[1:-1]}>({repr(self.args)[1:-1]}){'-> ' + repr(self.target) if self.target else ''} {{ {self.body} }})"
+        return f"DEF({self.prefix}{self.func_name}<{repr([('!:' if name[1] else '') + name[0](None) for name in self.bound_variables])[1:-1]}>({repr(self.args)[1:-1]}){'-> ' + repr(self.target) if self.target else ''} {{ {self.body} }})"
 
     def copy(self) -> "AbstractFunctionDefinitionAssembly":
         return type(self)(
             self.func_name,
             self.bound_variables.copy(),
             [arg.copy() for arg in self.args],
             self.body.copy(),
-            self.target.copy() if self.target else None,
+            target=self.target.copy() if self.target else None,
+            prefix=self.prefix,
         )
```

### Comparing `bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/instructions/IfAssembly.py` & `bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/instructions/WhileAssembly.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,61 +4,62 @@
 from bytecodemanipulation.assembler.AbstractBase import AbstractSourceExpression
 from bytecodemanipulation.assembler.AbstractBase import IAssemblyStructureVisitable
 from bytecodemanipulation.assembler.AbstractBase import IIdentifierAccessor
 from bytecodemanipulation.assembler.AbstractBase import ParsingScope
 from bytecodemanipulation.assembler.AbstractBase import StaticIdentifier
 from bytecodemanipulation.assembler.Lexer import SpecialToken
 from bytecodemanipulation.assembler.Parser import Parser
-from bytecodemanipulation.assembler.syntax_errors import throw_positioned_syntax_error
+from bytecodemanipulation.assembler.syntax_errors import throw_positioned_error
 from bytecodemanipulation.assembler.util.parser import AbstractExpression
+from bytecodemanipulation.assembler.util.tokenizer import IdentifierToken
 from bytecodemanipulation.data.shared.expressions.CompoundExpression import (
     CompoundExpression,
 )
 from bytecodemanipulation.data.shared.instructions.AbstractInstruction import (
     AbstractAssemblyInstruction,
 )
 
 
-class AbstractIFAssembly(AbstractAssemblyInstruction, abc.ABC):
-    # IF <expression> ['\'' <label name> '\''] '{' <body> '}'
-    NAME = "IF"
+class AbstractWhileAssembly(AbstractAssemblyInstruction, abc.ABC):
+    # # WHILE <expression> ['\'' <label name> '\''] '{' <body> '}'
+    NAME = "WHILE"
 
     @classmethod
-    def consume(cls, parser: "Parser", scope: ParsingScope) -> "AbstractIFAssembly":
-        source = parser.try_parse_data_source(
+    def consume(cls, parser: "Parser", scope: ParsingScope) -> "AbstractWhileAssembly":
+        condition = parser.try_parse_data_source(
             allow_primitives=True, include_bracket=False, scope=scope
         )
 
-        if source is None:
-            raise throw_positioned_syntax_error(
+        if condition is None:
+            raise throw_positioned_error(
                 scope, parser.try_inspect(), "expected <expression>"
             )
 
         if parser.try_consume(SpecialToken("'")):
             label_name = parser.parse_identifier_like(scope)
             if not parser.try_consume(SpecialToken("'")):
-                raise throw_positioned_syntax_error(
+                raise throw_positioned_error(
                     scope, parser.try_inspect(), "expected '"
                 )
         else:
             label_name = None
 
         body = parser.parse_body(scope=scope)
 
         return cls(
-            source,
+            condition,
             body,
             label_name,
         )
 
     def __init__(
         self,
         source: AbstractSourceExpression,
         body: CompoundExpression,
-        label_name: IIdentifierAccessor | str = None,
+        label_name: IIdentifierAccessor | None = None,
     ):
         self.source = source
         self.body = body
         self.label_name = (
             label_name
             if not isinstance(label_name, str)
             else StaticIdentifier(label_name)
@@ -73,41 +74,36 @@
             and self.source == other.source
             and self.body == other.body
             and self.label_name == other.label_name
         )
 
     def __repr__(self):
         c = "'"
-        return f"IF({self.source}{'' if self.label_name is None else ', label='+c+repr(self.label_name)+c}) -> {{{self.body}}}"
+        return f"WHILE({self.source}{'' if self.label_name is None else ', label='+c+repr(self.label_name)+c}) -> {{{self.body}}}"
 
     def visit_parts(
         self,
         visitor: typing.Callable[
             [IAssemblyStructureVisitable, tuple, typing.List[AbstractExpression]],
             typing.Any,
         ],
         parents: list,
     ):
         return visitor(
-            self,
-            (
-                self.source.visit_parts(visitor, parents + [self]),
-                self.body.visit_parts(visitor, parents + [self]),
-            ),
-            parents,
+            self, (self.source.visit_parts(visitor), self.body.visit_parts(visitor))
         )
 
     def visit_assembly_instructions(
         self, visitor: typing.Callable[[IAssemblyStructureVisitable, tuple], typing.Any]
     ):
         return visitor(self, (self.body.visit_assembly_instructions(visitor),))
 
-    def get_labels(self, scope: ParsingScope) -> typing.Set[str]:
+    def get_labels(self, scope: ParsingScope):
         return (
             set()
             if self.label_name is None
             else {
                 self.label_name(scope),
                 self.label_name(scope) + "_END",
-                self.label_name(scope) + "_HEAD",
+                self.label_name(scope) + "_INNER",
             }
         ) | self.body.get_labels(scope)
```

### Comparing `bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/instructions/JumpAssembly.py` & `bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/instructions/JumpAssembly.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/instructions/LabelAssembly.py` & `bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/instructions/StoreFastAssembly.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,50 +1,68 @@
+import abc
 import typing
 
-from bytecodemanipulation.assembler.AbstractBase import IIdentifierAccessor
-from bytecodemanipulation.assembler.AbstractBase import ParsingScope
-from bytecodemanipulation.assembler.AbstractBase import StaticIdentifier
+from bytecodemanipulation.assembler.AbstractBase import AbstractSourceExpression
+from bytecodemanipulation.assembler.AbstractBase import IAssemblyStructureVisitable
+from bytecodemanipulation.assembler.Lexer import SpecialToken
 from bytecodemanipulation.assembler.Parser import Parser
-from bytecodemanipulation.assembler.syntax_errors import throw_positioned_syntax_error
+from bytecodemanipulation.assembler.util.parser import AbstractExpression
+from bytecodemanipulation.assembler.util.tokenizer import IdentifierToken
+from bytecodemanipulation.assembler.util.tokenizer import IntegerToken
 from bytecodemanipulation.data.shared.instructions.AbstractInstruction import (
     AbstractAssemblyInstruction,
 )
-from bytecodemanipulation.opcodes.Instruction import Instruction
-from bytecodemanipulation.MutableFunction import MutableFunction
-from bytecodemanipulation.opcodes.Opcodes import Opcodes
 
 
-@Parser.register
-class LabelAssembly(AbstractAssemblyInstruction):
-    # LABEL <name>
-    NAME = "LABEL"
-
-    @classmethod
-    def consume(cls, parser: "Parser", scope: ParsingScope) -> "LabelAssembly":
-        name = parser.try_parse_identifier_like()
-
-        if name is None:
-            raise throw_positioned_syntax_error(
-                scope, parser[0], "expected <identifier like>"
+class AbstractStoreFastAssembly(AbstractAssemblyInstruction, abc.ABC):
+    # STORE_FAST <name> [<source>]
+    NAME = "STORE_FAST"
+
+    def __init__(
+        self,
+        name_token: IdentifierToken | IntegerToken | str | int,
+        source: AbstractSourceExpression | None = None,
+    ):
+        self.name_token = (
+            name_token
+            if not isinstance(name_token, (str, int))
+            else (
+                IdentifierToken(name_token)
+                if isinstance(name_token, str)
+                else IntegerToken(str(name_token))
             )
+        )
+        self.source = source
 
-        return cls(name)
+    @classmethod
+    def consume(cls, parser: "Parser", scope) -> "AbstractStoreFastAssembly":
+        parser.try_consume(SpecialToken("$"))
+        name = parser.consume([IdentifierToken, IntegerToken])
 
-    def __init__(self, name: IIdentifierAccessor | str):
-        self.name = name if not isinstance(name, str) else StaticIdentifier(name)
+        source = parser.try_parse_data_source()
 
-    def __repr__(self):
-        return f"LABEL({self.name})"
+        return cls(name, source)
 
     def __eq__(self, other):
-        return type(self) == type(other) and self.name == other.name
+        return (
+            type(self) == type(other)
+            and self.name_token == other.name_token
+            and self.source == other.source
+        )
 
-    def emit_bytecodes(
-        self, function: MutableFunction, scope: ParsingScope
-    ) -> typing.List[Instruction]:
-        return [Instruction(function, -1, Opcodes.BYTECODE_LABEL, self.name(scope))]
+    def __repr__(self):
+        return f"STORE_FAST({self.name_token}, source={self.source or 'TOS'})"
 
-    def copy(self) -> "LabelAssembly":
-        return type(self)(self.name)
+    def copy(self) -> "AbstractStoreFastAssembly":
+        return type(self)(self.name, self.source.copy() if self.source else None)
 
-    def get_labels(self, scope: ParsingScope) -> typing.Set[StaticIdentifier]:
-        return {StaticIdentifier(self.name(scope))}
+    def visit_parts(
+        self,
+        visitor: typing.Callable[
+            [IAssemblyStructureVisitable, tuple, typing.List[AbstractExpression]],
+            typing.Any,
+        ],
+        parents: list,
+    ):
+        return visitor(
+            self, (self.source.visit_parts(visitor) if self.target else None,)
+        )
```

### Comparing `bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/instructions/LoadAssembly.py` & `bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/instructions/LoadAssembly.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from bytecodemanipulation.assembler.AbstractBase import AbstractAccessExpression
 from bytecodemanipulation.data.shared.instructions.AbstractInstruction import (
     AbstractAssemblyInstruction,
 )
 from bytecodemanipulation.assembler.AbstractBase import IAssemblyStructureVisitable
 from bytecodemanipulation.assembler.Parser import Parser
 from bytecodemanipulation.assembler.AbstractBase import ParsingScope
-from bytecodemanipulation.assembler.syntax_errors import throw_positioned_syntax_error
+from bytecodemanipulation.assembler.syntax_errors import throw_positioned_error
 from bytecodemanipulation.assembler.util.parser import AbstractExpression
 from bytecodemanipulation.opcodes.Instruction import Instruction
 from bytecodemanipulation.MutableFunction import MutableFunction
 
 
 @Parser.register
 class LoadAssembly(AbstractAssemblyInstruction):
@@ -22,21 +22,21 @@
     @classmethod
     def consume(cls, parser: "Parser", scope: ParsingScope) -> "LoadAssembly":
         access_expr = parser.try_consume_access_to_value(
             allow_tos=False, allow_primitives=True, scope=scope
         )
 
         if access_expr is None:
-            raise throw_positioned_syntax_error(
+            raise throw_positioned_error(
                 scope, parser.try_inspect(), "expected <expression>"
             )
 
         if parser.try_consume(SpecialToken("-")):
             if not parser.try_consume(SpecialToken(">")):
-                raise throw_positioned_syntax_error(
+                raise throw_positioned_error(
                     scope,
                     parser[-1:1] + [scope.last_base_token],
                     "expected '>' after '-' to complete '->'",
                 )
 
             target = parser.try_consume_access_to_value(scope=scope)
         else:
```

### Comparing `bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/instructions/LoadConstAssembly.py` & `bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/instructions/LoadConstAssembly.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import abc
 import typing
 
 from bytecodemanipulation.assembler.AbstractBase import AbstractAccessExpression
 from bytecodemanipulation.assembler.AbstractBase import IAssemblyStructureVisitable
 from bytecodemanipulation.assembler.Lexer import SpecialToken
 from bytecodemanipulation.assembler.Parser import Parser
-from bytecodemanipulation.assembler.syntax_errors import throw_positioned_syntax_error
+from bytecodemanipulation.assembler.syntax_errors import throw_positioned_error
 from bytecodemanipulation.assembler.util.parser import AbstractExpression
 from bytecodemanipulation.data.shared.expressions.ConstantAccessExpression import (
     ConstantAccessExpression,
 )
 from bytecodemanipulation.data.shared.expressions.GlobalAccessExpression import (
     GlobalAccessExpression,
 )
@@ -37,15 +37,15 @@
     @classmethod
     def consume(cls, parser: "Parser", scope) -> "AbstractLoadConstAssembly":
         value = parser.try_parse_data_source(
             allow_primitives=True, include_bracket=False
         )
 
         if not isinstance(value, (ConstantAccessExpression, GlobalAccessExpression)):
-            raise throw_positioned_syntax_error(
+            raise throw_positioned_error(
                 scope, parser.try_inspect(), "expected <constant epxression>"
             )
 
         if parser.try_consume_multi(
             [
                 SpecialToken("-"),
                 SpecialToken(">"),
```

### Comparing `bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/instructions/LoadFastAssembly.py` & `bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/instructions/LoadFastAssembly.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/instructions/LoadGlobalAssembly.py` & `bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/instructions/LoadGlobalAssembly.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import abc
 import typing
 
 from bytecodemanipulation.assembler.AbstractBase import AbstractAccessExpression
 from bytecodemanipulation.assembler.AbstractBase import IAssemblyStructureVisitable
 from bytecodemanipulation.assembler.Lexer import SpecialToken
 from bytecodemanipulation.assembler.Parser import Parser
-from bytecodemanipulation.assembler.syntax_errors import throw_positioned_syntax_error
+from bytecodemanipulation.assembler.syntax_errors import throw_positioned_error
 from bytecodemanipulation.assembler.util.parser import AbstractExpression
 from bytecodemanipulation.assembler.util.tokenizer import IdentifierToken
 from bytecodemanipulation.assembler.util.tokenizer import IntegerToken
 from bytecodemanipulation.data.shared.instructions.AbstractInstruction import (
     AbstractAssemblyInstruction,
 )
 
@@ -37,30 +37,30 @@
     @classmethod
     def consume(cls, parser: "Parser", scope) -> "AbstractLoadGlobalAssembly":
         parser.try_consume(SpecialToken("@"))
 
         name = parser.try_consume([IdentifierToken, IntegerToken])
 
         if name is None:
-            raise throw_positioned_syntax_error(
+            raise throw_positioned_error(
                 scope, parser.try_inspect(), "expected <name> or <integer>"
             )
 
         if parser.try_consume(SpecialToken("-")):
             if not parser.try_consume(SpecialToken(">")):
-                raise throw_positioned_syntax_error(
+                raise throw_positioned_error(
                     scope,
                     parser[-1:1] + [scope.last_base_token],
                     "expected '>' after '-'",
                 )
 
             target = parser.try_consume_access_to_value(scope=scope)
 
             if target is None:
-                raise throw_positioned_syntax_error(
+                raise throw_positioned_error(
                     scope, parser.try_inspect(), "expected <expression>"
                 )
         else:
             target = None
 
         return cls(name, target)
```

### Comparing `bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/instructions/MacroAssembly.py` & `bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/instructions/MacroAssembly.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,20 @@
+import traceback
 import typing
 from abc import ABC
 
+from bytecodemanipulation.MutableFunctionHelpers import capture_local
+
+from bytecodemanipulation.MutableFunctionHelpers import outer_return
+
 from bytecodemanipulation.assembler.AbstractBase import AbstractAccessExpression
 from bytecodemanipulation.assembler.AbstractBase import JumpToLabel
 from bytecodemanipulation.assembler.AbstractBase import ParsingScope
 from bytecodemanipulation.assembler.Lexer import SpecialToken
-from bytecodemanipulation.assembler.syntax_errors import throw_positioned_syntax_error
+from bytecodemanipulation.assembler.syntax_errors import throw_positioned_error
 from bytecodemanipulation.assembler.util.tokenizer import IdentifierToken
 from bytecodemanipulation.data.shared.instructions.AbstractInstruction import (
     AbstractAssemblyInstruction,
 )
 from bytecodemanipulation.data.shared.expressions.CompoundExpression import (
     CompoundExpression,
 )
@@ -33,14 +38,28 @@
 
 LOCAL_TO_DEREF_OPCODES = {
     Opcodes.LOAD_FAST: Opcodes.MACRO_LOAD_PARAMETER,
     Opcodes.STORE_FAST: Opcodes.MACRO_STORE_PARAMETER,
 }
 
 
+def _manipulate_stack_trace(exc: Exception, file: str, func_name: str, line: int, column: int, span: int):
+    trace = traceback.extract_stack()
+
+    entry = traceback.FrameSummary(
+        filename=file,
+        lineno=line,
+        name=func_name,
+    )
+
+    trace.append(entry)
+
+    # exc.__traceback__ = traceback.TracebackException(*trace).__traceback__
+
+
 class MacroAssembly(AbstractAssemblyInstruction):
     # 'MACRO' ['ASSEMBLY'] [{<namespace> ':'}] <name> ['(' <param> \[{',' <param>}] ')'] ['->' <data type>] '{' <assembly code> '}', where param is ['!'] \<name> [<data type>]
     NAME = "MACRO"
 
     @classmethod
     def register(cls):
         from bytecodemanipulation.assembler.Parser import Parser
@@ -138,15 +157,15 @@
             if not isinstance(args, list):
                 raise ValueError(f"args must be list, got {args}!")
 
             bytecode = []
             for arg in args:
                 bytecode += arg.emit_bytecodes(function, scope)
 
-            bytecode += [Instruction(function, -1, "BUILD_LIST", arg=len(args))]
+            bytecode += [Instruction("BUILD_LIST", arg=len(args))]
             return bytecode
 
     class MacroArg:
         def __init__(self, name: IdentifierToken, is_static=False):
             self.name = name
             self.is_static = is_static
             self.index = -1
@@ -262,15 +281,15 @@
 
                     if error:
                         continue
 
                     args[:] = prefix + [inner] + postfix
                     return macro, args
 
-            raise throw_positioned_syntax_error(
+            raise throw_positioned_error(
                 scope,
                 self.name_token,
                 f"Could not find overloaded variant of {':'.join(self.name)} with args {args}!",
                 NameError,
             )
 
         def add_definition(self, macro: "MacroAssembly", override=False):
@@ -439,33 +458,29 @@
                 if arg_decl.data_type_annotation is not None:
                     arg_names.append(var_name := scope.scope_name_generator(f"arg_{i}"))
                     bytecode += arg_decl.data_type_annotation.emit_for_arg(
                         arg_code, function, scope
                     )
                     bytecode.append(
                         Instruction(
-                            function,
-                            -1,
                             Opcodes.STORE_FAST,
                             var_name,
-                            _decode_next=False,
                         )
                     )
+
                 else:
                     arg_names.append(var_name := scope.scope_name_generator(f"arg_{i}"))
                     bytecode += arg_code.emit_bytecodes(function, scope)
                     bytecode.append(
                         Instruction(
-                            function,
-                            -1,
                             Opcodes.STORE_FAST,
                             var_name,
-                            _decode_next=False,
                         )
                     )
+
             else:
                 arg_names.append(None)
 
         local_prefix = scope.scope_name_generator("macro_local")
         end_target = scope.scope_name_generator("macro_end")
         requires_none_load = (
             self.return_type is not None
@@ -477,15 +492,15 @@
             bytecode.append(instr)
 
             if instr.opcode in (
                 Opcodes.MACRO_LOAD_PARAMETER,
                 Opcodes.MACRO_PARAMETER_EXPANSION,
             ):
                 if instr.arg_value not in arg_decl_lookup:
-                    raise throw_positioned_syntax_error(
+                    raise throw_positioned_error(
                         scope,
                         self.name,
                         f"macro name {instr.arg_value} not found in scope",
                     )
 
                 arg_decl: MacroAssembly.MacroArg = arg_decl_lookup[instr.arg_value]
 
@@ -515,15 +530,15 @@
                             function, scope
                         )
                         instr.insert_after(instructions)
                         bytecode += instructions
 
             elif instr.opcode == Opcodes.MACRO_STORE_PARAMETER:
                 if instr.arg_value not in arg_decl_lookup:
-                    raise throw_positioned_syntax_error(
+                    raise throw_positioned_error(
                         scope,
                         self.name,
                         f"macro name {instr.arg_value} not found in scope",
                     )
 
                 arg_decl = arg_decl_lookup[instr.arg_value]
 
@@ -537,38 +552,60 @@
 
                         if instructions is not None:
                             instr.change_opcode(Opcodes.NOP)
                             instr.insert_after(instructions)
                             bytecode += instructions
                             continue
 
-                    raise throw_positioned_syntax_error(
+                    raise throw_positioned_error(
                         scope,
                         self.name,
                         f"Tried to override non-static MACRO parameter '{instr.arg_value}'; This is not allowed as the parameter will be evaluated on each access!",
                         RuntimeError,
                     )
 
-            elif instr.has_local() and instr.arg_value.startswith("MACRO_"):
+            elif instr.has_local() and instr.arg_value.startswith(":"):
                 instr.change_arg_value(
-                    local_prefix + ":" + instr.arg_value.removeprefix("MACRO_")
+                    instr.arg_value.removeprefix(":")
                 )
 
+            elif instr.has_local():
+                instr.change_arg_value(local_prefix + ":" + instr.arg_value)
+
             elif instr.opcode == Opcodes.MACRO_RETURN_VALUE:
                 if self.return_type is None:
                     raise SyntaxError(
                         "'MACRO_RETURN' only allowed in assembly if return type declared!"
                     )
 
                 instr.change_opcode(Opcodes.JUMP_ABSOLUTE, JumpToLabel(end_target))
 
         if requires_none_load:
-            bytecode.append(Instruction(function, -1, Opcodes.LOAD_CONST, None))
+            bytecode.append(Instruction(Opcodes.LOAD_CONST, None))
+
+        bytecode.append(Instruction(Opcodes.BYTECODE_LABEL, end_target))
 
-        bytecode.append(Instruction(function, -1, Opcodes.BYTECODE_LABEL, end_target))
+        # handle = Instruction(Opcodes.NOP)
+        # handle.insert_after(
+        #     [
+        #         Instruction(Opcodes.POP_TOP),
+        #         Instruction(Opcodes.ROT_TWO),  # TOS would be the exception
+        #         Instruction(Opcodes.POP_TOP),
+        #         Instruction(Opcodes.LOAD_CONST, _manipulate_stack_trace),
+        #         Instruction(Opcodes.ROT_TWO),
+        #         Instruction(Opcodes.LOAD_CONST, scope.module_file),
+        #         Instruction(Opcodes.LOAD_CONST, "".join(map(lambda e: e.text, self.name))),
+        #         Instruction(Opcodes.LOAD_CONST, 0),  # todo: load position info (line)
+        #         Instruction(Opcodes.LOAD_CONST, 0),  # todo: load position info (column)
+        #         Instruction(Opcodes.LOAD_CONST, 0),  # todo: load position info (span)
+        #         Instruction(Opcodes.CALL_FUNCTION, arg=6),
+        #         Instruction(Opcodes.RAISE_VARARGS, arg=0),
+        #     ]
+        # )
+        # function.exception_table.add_handle(handle, inner_bytecode)
 
         return bytecode
 
     def fill_scope(self, scope: ParsingScope):
         name = scope.scope_path + list(map(lambda e: e.text, self.name))
         namespace = name[:-1]
         inner_name = name[-1]
@@ -597,28 +634,62 @@
         def emit_bytecodes(
             self, function: MutableFunction, scope: ParsingScope
         ) -> typing.List[Instruction]:
             macro_exit_label = scope.scope_name_generator("macro_exit")
 
             builder = self.function.create_filled_builder()
 
-            return [
+            instructions = [
                 (
-                    instr.copy(owner=function)
+                    instr
                     if instr.opcode != Opcodes.RETURN_VALUE
-                    else instr.copy(owner=function)
+                    else instr
                     .change_opcode(Opcodes.POP_TOP)
                     .insert_after(
                         Instruction(
-                            function,
-                            -1,
                             Opcodes.JUMP_ABSOLUTE,
                             JumpToLabel(macro_exit_label),
                         )
                     )
                 )
                 if not instr.has_local() or instr.arg_value not in self.scoped_names
-                else instr.copy(owner=function).change_opcode(
+                else instr.copy().change_opcode(
                     LOCAL_TO_DEREF_OPCODES[instr.opcode]
                 )
                 for instr in builder.temporary_instructions
-            ] + [Instruction(function, -1, Opcodes.BYTECODE_LABEL, macro_exit_label)]
+            ]
+
+            captured_locals = set()
+            for instr in instructions:
+                if instr.opcode == Opcodes.LOAD_GLOBAL:
+                    target = self.function.target.__globals__.get(instr.arg_value, None)
+
+                    if target == capture_local:
+                        call = next(instr.trace_stack_position_use(0))
+
+                        if call.opcode != Opcodes.CALL_FUNCTION:
+                            raise ValueError(call)
+
+                        arg = next(call.trace_stack_position(0))
+
+                        if arg.opcode != Opcodes.LOAD_CONST:
+                            raise ValueError(arg)
+
+                        captured_locals.add(arg.arg_value)
+                        arg.change_opcode(Opcodes.NOP)
+                        call.change_opcode(Opcodes.LOAD_CONST, None)
+                        instr.change_opcode(Opcodes.NOP)
+
+            for instr in instructions:
+                if instr.opcode == Opcodes.LOAD_GLOBAL:
+                    target = self.function.target.__globals__.get(instr.arg_value, None)
+
+                    if target == outer_return:
+                        call = next(instr.trace_stack_position_use(0))
+
+                        instr.change_opcode(Opcodes.NOP)
+                        call.change_opcode(Opcodes.RETURN_VALUE)
+
+                elif instr.has_local() and instr.arg_value in captured_locals:
+                    instr.change_arg_value(":" + instr.arg_value)
+
+            return instructions + [Instruction(Opcodes.BYTECODE_LABEL, macro_exit_label)]
```

### Comparing `bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/instructions/MacroImportAssembly.py` & `bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/instructions/MacroImportAssembly.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/instructions/MacroPasteAssembly.py` & `bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/instructions/MacroPasteAssembly.py`

 * *Files 7% similar despite different names*

```diff
@@ -56,22 +56,31 @@
 
     def emit_bytecodes(
         self, function: MutableFunction, scope: ParsingScope
     ) -> typing.List[Instruction]:
         if self.name.text in scope.macro_parameter_namespace and hasattr(
             scope.macro_parameter_namespace[self.name.text], "emit_bytecodes"
         ):
-            return scope.macro_parameter_namespace[self.name.text].emit_bytecodes(
+            instructions = scope.macro_parameter_namespace[self.name.text].emit_bytecodes(
                 function, scope
-            ) + (
+            )
+
+            for instr in instructions:
+                if instr.has_local():
+                    if instr.arg_value.startswith("|"):
+                        instr.change_arg_value(instr.arg_value[1:])
+                    else:
+                        instr.change_arg_value(":" + instr.arg_value)
+
+            return instructions + (
                 []
                 if self.target is None
                 else self.target.emit_store_bytecodes(function, scope)
             )
 
         return [
-            Instruction(function, -1, Opcodes.MACRO_PARAMETER_EXPANSION, self.name.text)
+            Instruction(Opcodes.MACRO_PARAMETER_EXPANSION, self.name.text)
         ] + (
             []
             if self.target is None
             else self.target.emit_store_bytecodes(function, scope)
         )
```

### Comparing `bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/instructions/MacroReturnAssembly.py` & `bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/instructions/MacroReturnAssembly.py`

 * *Files 6% similar despite different names*

```diff
@@ -52,8 +52,8 @@
         return MacroReturnAssembly(self.expr.copy())
 
     def emit_bytecodes(
         self, function: MutableFunction, scope: ParsingScope
     ) -> typing.List[Instruction]:
         expr_bytecode = self.expr.emit_bytecodes(function, scope) if self.expr else []
 
-        return expr_bytecode + [Instruction(function, -1, Opcodes.MACRO_RETURN_VALUE)]
+        return expr_bytecode + [Instruction(Opcodes.MACRO_RETURN_VALUE)]
```

### Comparing `bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/instructions/NamespaceAssembly.py` & `bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/instructions/NamespaceAssembly.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/instructions/OpAssembly.py` & `bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/instructions/OpAssembly.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import typing
 from collections import namedtuple
 
 from bytecodemanipulation.assembler.AbstractBase import AbstractSourceExpression
 from bytecodemanipulation.assembler.util.tokenizer import AbstractToken
 from bytecodemanipulation.assembler.Lexer import SpecialToken
 from bytecodemanipulation.assembler.AbstractBase import IAssemblyStructureVisitable
-from bytecodemanipulation.assembler.syntax_errors import throw_positioned_syntax_error
+from bytecodemanipulation.assembler.syntax_errors import throw_positioned_error
 from bytecodemanipulation.assembler.util.parser import AbstractExpression
 from bytecodemanipulation.assembler.AbstractBase import AbstractAccessExpression
 from bytecodemanipulation.data.shared.instructions.AbstractInstruction import (
     AbstractAssemblyInstruction,
 )
 from bytecodemanipulation.MutableFunction import MutableFunction
 from bytecodemanipulation.opcodes.Instruction import Instruction
@@ -61,27 +61,27 @@
         bytecode = []
         if not any(isinstance(param, OperatorArgValue) for param in self.opcodes):
             for param in parameters:
                 bytecode += param.emit_bytecodes(function, scope)
 
         for opcode in self.opcodes:
             if isinstance(opcode, (int, str)):
-                bytecode.append(Instruction(function, -1, opcode))
+                bytecode.append(Instruction(opcode))
             elif isinstance(opcode, tuple):
                 if isinstance(opcode[1], typing.Callable):
                     bytecode.append(
                         Instruction(
                             function,
                             -1,
                             opcode[0],
                             arg=opcode[1](function, scope, list(parameters)),
                         )
                     )
                 else:
-                    bytecode.append(Instruction(function, -1, opcode[0], arg=opcode[1]))
+                    bytecode.append(Instruction(opcode[0], arg=opcode[1]))
             elif isinstance(opcode, OperatorArgValue):
                 bytecode += parameters[opcode.index].emit_bytecodes(function, scope)
             elif hasattr(opcode, "emit_bytecodes"):
                 bytecode += opcode.emit_bytecodes(function, scope)
             else:
                 raise ValueError(opcode)
 
@@ -171,15 +171,15 @@
             self, function: MutableFunction, scope: ParsingScope
         ) -> typing.List[Instruction]:
             try:
                 return self.base.SINGLE_OPS[self.operator].emit_bytecodes(
                     function, scope, self.expression
                 )
             except:
-                raise throw_positioned_syntax_error(
+                raise throw_positioned_error(
                     scope,
                     self.operator_token,
                     "during emitting bytecode of singleton operator",
                 )
 
         def visit_parts(
             self,
@@ -239,15 +239,15 @@
             self, function: MutableFunction, scope: ParsingScope
         ) -> typing.List[Instruction]:
             try:
                 return self.base.BINARY_OPS[self.operator].emit_bytecodes(
                     function, scope, self.lhs, self.rhs
                 )
             except:
-                raise throw_positioned_syntax_error(
+                raise throw_positioned_error(
                     scope,
                     self.operator_token,
                     "during emitting bytecode of binary operation",
                 )
 
         def visit_parts(
             self,
@@ -301,15 +301,15 @@
             self, function: MutableFunction, scope: ParsingScope
         ) -> typing.List[Instruction]:
             try:
                 return self.base.PREFIX_OPERATORS[self.operator][0].emit_bytecodes(
                     function, scope, *self.args
                 )
             except:
-                raise throw_positioned_syntax_error(
+                raise throw_positioned_error(
                     scope,
                     self.operator_token,
                     "during emitting bytecode of binary operation",
                 )
 
         def visit_parts(
             self,
@@ -339,15 +339,15 @@
 
         if expr := cls.try_consume_single(parser, scope):
             return cls(expr, cls.try_consume_arrow(parser, scope))
 
         if expr := cls.try_consume_prefix(parser, scope):
             return cls(expr, cls.try_consume_arrow(parser, scope))
 
-        raise throw_positioned_syntax_error(
+        raise throw_positioned_error(
             scope,
             parser.try_inspect(),
             "expected <operator> or <expression> <operator> ...",
         )
 
     @classmethod
     def try_consume_operator_name(
@@ -364,15 +364,15 @@
 
     @classmethod
     def try_consume_arrow(
         cls, parser: "Parser", scope: ParsingScope
     ) -> AbstractAccessExpression | None:
         if parser.try_consume(SpecialToken("-")):
             if not parser.try_consume(SpecialToken(">")):
-                raise throw_positioned_syntax_error(
+                raise throw_positioned_error(
                     scope,
                     parser[-1:1] + [scope.last_base_token],
                     "expected '>' after '-' to complete '->'",
                 )
 
             return parser.try_consume_access_to_value(scope=scope)
 
@@ -446,17 +446,17 @@
         operator_def, arg_count, has_brackets, has_coma_sep = cls.PREFIX_OPERATORS[
             operator
         ]
 
         bracket = parser.try_consume(SpecialToken("("))
 
         if bracket is None and has_brackets is True:
-            raise throw_positioned_syntax_error(scope, parser[0], "expected '('")
+            raise throw_positioned_error(scope, parser[0], "expected '('")
         elif bracket is not None and has_brackets is False:
-            raise throw_positioned_syntax_error(
+            raise throw_positioned_error(
                 scope,
                 operator_tokens + [parser[0]],
                 "did not expect '(' after operator name",
             )
 
         args = []
 
@@ -468,67 +468,67 @@
                     allow_tos=True,
                     allow_primitives=True,
                     allow_op=True,
                     allow_advanced_access=True,
                 )
 
                 if expr is None:
-                    raise throw_positioned_syntax_error(
+                    raise throw_positioned_error(
                         scope, parser[0], "expected <expression>"
                     )
 
                 args.append(expr)
 
                 coma = parser.try_consume(SpecialToken(","))
 
                 if coma is None and has_coma_sep is True:
-                    raise throw_positioned_syntax_error(
+                    raise throw_positioned_error(
                         scope, parser[0], "expected ','"
                     )
 
                 elif coma is not None and has_coma_sep is False:
-                    raise throw_positioned_syntax_error(
+                    raise throw_positioned_error(
                         scope, coma, "did not expect ',' for separation of args"
                     )
         else:
             while not parser.try_inspect() == SpecialToken(")"):
                 expr = parser.try_consume_access_to_value(
                     scope=scope,
                     allow_calls=True,
                     allow_tos=True,
                     allow_primitives=True,
                     allow_op=True,
                     allow_advanced_access=True,
                 )
 
                 if expr is None:
-                    raise throw_positioned_syntax_error(
+                    raise throw_positioned_error(
                         scope, parser[0], "expected <expression>"
                     )
 
                 args.append(expr)
 
                 coma = parser.try_consume(SpecialToken(","))
 
                 if (
                     coma is None
                     and has_coma_sep is True
                     and parser[0] != SpecialToken(")")
                 ):
-                    raise throw_positioned_syntax_error(
+                    raise throw_positioned_error(
                         scope, parser[0], "expected ','"
                     )
 
                 elif coma is not None and has_coma_sep is False:
-                    raise throw_positioned_syntax_error(
+                    raise throw_positioned_error(
                         scope, coma, "did not expect ',' for separation of args"
                     )
 
         if bracket and not parser.try_consume(SpecialToken(")")):
-            raise throw_positioned_syntax_error(scope, parser[0], "expected ')'")
+            raise throw_positioned_error(scope, parser[0], "expected ')'")
 
         return cls.PrefixOperator(operator, operator_tokens, args, base=cls)
 
     def __init__(
         self, operation: IOperation, target: AbstractAccessExpression | None = None
     ):
         if operation is None:
```

### Comparing `bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/instructions/PopElementAssembly.py` & `bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/instructions/PopElementAssembly.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/instructions/PythonCodeAssembly.py` & `bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/instructions/PythonCodeAssembly.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/instructions/RaiseAssembly.py` & `bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/instructions/RaiseAssembly.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/instructions/RawAssembly.py` & `bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/instructions/RawAssembly.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,13 +48,11 @@
 
         if opcode.isdigit():
             opcode = int(opcode)
 
         return [
             Instruction.create_with_token(
                 self.opcode_or_name,
-                function,
-                -1,
                 opcode,
                 arg=0 if self.arg is None else int(self.arg.text),
             ),
         ]
```

### Comparing `bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/instructions/ReturnAssembly.py` & `bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/instructions/ReturnAssembly.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/instructions/StoreAssembly.py` & `bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/instructions/StoreAssembly.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from bytecodemanipulation.data.shared.instructions.AbstractInstruction import (
     AbstractAssemblyInstruction,
 )
 from bytecodemanipulation.assembler.AbstractBase import AbstractSourceExpression
 from bytecodemanipulation.assembler.AbstractBase import IAssemblyStructureVisitable
 from bytecodemanipulation.assembler.Parser import Parser
 from bytecodemanipulation.assembler.AbstractBase import ParsingScope
-from bytecodemanipulation.assembler.syntax_errors import throw_positioned_syntax_error
+from bytecodemanipulation.assembler.syntax_errors import throw_positioned_error
 from bytecodemanipulation.assembler.util.parser import AbstractExpression
 from bytecodemanipulation.opcodes.Instruction import Instruction
 from bytecodemanipulation.MutableFunction import MutableFunction
 
 
 @Parser.register
 class StoreAssembly(AbstractAssemblyInstruction):
@@ -22,15 +22,15 @@
     @classmethod
     def consume(cls, parser: "Parser", scope: ParsingScope) -> "StoreAssembly":
         access = parser.try_consume_access_to_value(
             allow_tos=False, scope=scope, allow_calls=False
         )
 
         if access is None:
-            raise throw_positioned_syntax_error(
+            raise throw_positioned_error(
                 scope, parser.try_inspect(), "expected <expression>"
             )
 
         source = parser.try_parse_data_source()
 
         return cls(access, source)
```

### Comparing `bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/instructions/StoreFastAssembly.py` & `bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/instructions/StoreGlobalAssembly.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 import abc
 import typing
 
 from bytecodemanipulation.assembler.AbstractBase import AbstractSourceExpression
 from bytecodemanipulation.assembler.AbstractBase import IAssemblyStructureVisitable
 from bytecodemanipulation.assembler.Lexer import SpecialToken
 from bytecodemanipulation.assembler.Parser import Parser
+from bytecodemanipulation.assembler.syntax_errors import throw_positioned_error
 from bytecodemanipulation.assembler.util.parser import AbstractExpression
 from bytecodemanipulation.assembler.util.tokenizer import IdentifierToken
 from bytecodemanipulation.assembler.util.tokenizer import IntegerToken
 from bytecodemanipulation.data.shared.instructions.AbstractInstruction import (
     AbstractAssemblyInstruction,
 )
 
 
-class AbstractStoreFastAssembly(AbstractAssemblyInstruction, abc.ABC):
-    # STORE_FAST <name> [<source>]
-    NAME = "STORE_FAST"
+class AbstractStoreGlobalAssembly(AbstractAssemblyInstruction, abc.ABC):
+    # STORE_GLOBAL <name> [<source>]
+    NAME = "STORE_GLOBAL"
 
     def __init__(
         self,
         name_token: IdentifierToken | IntegerToken | str | int,
         source: AbstractSourceExpression | None = None,
     ):
         self.name_token = (
@@ -30,39 +31,44 @@
                 if isinstance(name_token, str)
                 else IntegerToken(str(name_token))
             )
         )
         self.source = source
 
     @classmethod
-    def consume(cls, parser: "Parser", scope) -> "AbstractStoreFastAssembly":
-        parser.try_consume(SpecialToken("$"))
-        name = parser.consume([IdentifierToken, IntegerToken])
+    def consume(cls, parser: "Parser", scope) -> "AbstractStoreGlobalAssembly":
+        parser.try_consume(SpecialToken("@"))
+        name = parser.try_consume([IdentifierToken, IntegerToken])
+
+        if name is None:
+            raise throw_positioned_error(
+                scope, parser.try_inspect(), "expected <name> or <integer>"
+            )
 
         source = parser.try_parse_data_source()
 
         return cls(name, source)
 
     def __eq__(self, other):
         return (
             type(self) == type(other)
             and self.name_token == other.name_token
             and self.source == other.source
         )
 
     def __repr__(self):
-        return f"STORE_FAST({self.name_token}, source={self.source or 'TOS'})"
+        return f"STORE_GLOBAL({self.name_token}, source={self.source or 'TOS'})"
 
-    def copy(self) -> "AbstractStoreFastAssembly":
-        return type(self)(self.name, self.source.copy() if self.source else None)
+    def copy(self) -> "AbstractStoreGlobalAssembly":
+        return type(self)(self.name_token, self.source.copy() if self.source else None)
 
     def visit_parts(
         self,
         visitor: typing.Callable[
             [IAssemblyStructureVisitable, tuple, typing.List[AbstractExpression]],
             typing.Any,
         ],
         parents: list,
     ):
         return visitor(
-            self, (self.source.visit_parts(visitor) if self.target else None,)
+            self, (self.source.visit_parts(visitor, []) if self.source else None,)
         )
```

### Comparing `bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/instructions/StoreGlobalAssembly.py` & `bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/instructions/YieldAssembly.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,74 +1,92 @@
 import abc
 import typing
 
 from bytecodemanipulation.assembler.AbstractBase import AbstractSourceExpression
 from bytecodemanipulation.assembler.AbstractBase import IAssemblyStructureVisitable
 from bytecodemanipulation.assembler.Lexer import SpecialToken
 from bytecodemanipulation.assembler.Parser import Parser
-from bytecodemanipulation.assembler.syntax_errors import throw_positioned_syntax_error
+from bytecodemanipulation.assembler.syntax_errors import throw_positioned_error
 from bytecodemanipulation.assembler.util.parser import AbstractExpression
-from bytecodemanipulation.assembler.util.tokenizer import IdentifierToken
-from bytecodemanipulation.assembler.util.tokenizer import IntegerToken
 from bytecodemanipulation.data.shared.instructions.AbstractInstruction import (
     AbstractAssemblyInstruction,
 )
 
 
-class AbstractStoreGlobalAssembly(AbstractAssemblyInstruction, abc.ABC):
-    # STORE_GLOBAL <name> [<source>]
-    NAME = "STORE_GLOBAL"
+class AbstractYieldAssembly(AbstractAssemblyInstruction, abc.ABC):
+    # YIELD [*] [<expr>] [-> <target>]
+    NAME = "YIELD"
 
     def __init__(
         self,
-        name_token: IdentifierToken | IntegerToken | str | int,
-        source: AbstractSourceExpression | None = None,
+        expr: AbstractSourceExpression | None = None,
+        is_star: bool = False,
+        target: AbstractSourceExpression | None = None,
     ):
-        self.name_token = (
-            name_token
-            if not isinstance(name_token, (str, int))
-            else (
-                IdentifierToken(name_token)
-                if isinstance(name_token, str)
-                else IntegerToken(str(name_token))
-            )
-        )
-        self.source = source
+        self.expr = expr
+        self.is_star = is_star
+        self.target = target
 
     @classmethod
-    def consume(cls, parser: "Parser", scope) -> "AbstractStoreGlobalAssembly":
-        parser.try_consume(SpecialToken("@"))
-        name = parser.try_consume([IdentifierToken, IntegerToken])
-
-        if name is None:
-            raise throw_positioned_syntax_error(
-                scope, parser.try_inspect(), "expected <name> or <integer>"
-            )
+    def consume(cls, parser: "Parser", scope) -> "AbstractYieldAssembly":
+        is_star = bool(parser.try_consume(SpecialToken("*")))
 
-        source = parser.try_parse_data_source()
+        expr = parser.try_parse_data_source(
+            allow_primitives=True, allow_op=True, include_bracket=False
+        )
 
-        return cls(name, source)
+        if parser.try_consume(SpecialToken("-")) and parser.try_consume(
+            SpecialToken(">")
+        ):
+            target = parser.try_parse_data_source(
+                allow_primitives=True, allow_op=True, include_bracket=False
+            )
 
-    def __eq__(self, other):
-        return (
-            type(self) == type(other)
-            and self.name_token == other.name_token
-            and self.source == other.source
-        )
+            if target is None:
+                raise throw_positioned_error(
+                    scope, parser.try_inspect(), "expected <expression>"
+                )
 
-    def __repr__(self):
-        return f"STORE_GLOBAL({self.name_token}, source={self.source or 'TOS'})"
+        else:
+            target = None
 
-    def copy(self) -> "AbstractStoreGlobalAssembly":
-        return type(self)(self.name_token, self.source.copy() if self.source else None)
+        return cls(expr, is_star, target)
 
     def visit_parts(
         self,
         visitor: typing.Callable[
             [IAssemblyStructureVisitable, tuple, typing.List[AbstractExpression]],
             typing.Any,
         ],
         parents: list,
     ):
         return visitor(
-            self, (self.source.visit_parts(visitor, []) if self.source else None,)
+            self,
+            (
+                self.expr.visit_parts(visitor, parents + [self]) if self.expr else None,
+                self.target.visit_parts(
+                    visitor,
+                    parents + [self],
+                )
+                if self.target
+                else None,
+            ),
+            parents,
+        )
+
+    def __eq__(self, other):
+        return (
+            type(self) == type(other)
+            and self.expr == other.expr
+            and self.is_star == other.is_star
+            and self.target == other.target
+        )
+
+    def __repr__(self):
+        return f"YIELD{'' if not self.is_star else '*'}({self.expr if self.expr else ''}{(', ' if self.expr else '->') + repr(self.target) if self.target else ''})"
+
+    def copy(self) -> "AbstractYieldAssembly":
+        return type(self)(
+            self.expr.copy() if self.expr else None,
+            self.is_star,
+            self.target.copy() if self.target else None,
         )
```

### Comparing `bytecodemanipulation-0.3.1/bytecodemanipulation/data/shared/instructions/WhileAssembly.py` & `bytecodemanipulation-0.3.3/bytecodemanipulation/data/shared/instructions/IfAssembly.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,62 +4,61 @@
 from bytecodemanipulation.assembler.AbstractBase import AbstractSourceExpression
 from bytecodemanipulation.assembler.AbstractBase import IAssemblyStructureVisitable
 from bytecodemanipulation.assembler.AbstractBase import IIdentifierAccessor
 from bytecodemanipulation.assembler.AbstractBase import ParsingScope
 from bytecodemanipulation.assembler.AbstractBase import StaticIdentifier
 from bytecodemanipulation.assembler.Lexer import SpecialToken
 from bytecodemanipulation.assembler.Parser import Parser
-from bytecodemanipulation.assembler.syntax_errors import throw_positioned_syntax_error
+from bytecodemanipulation.assembler.syntax_errors import throw_positioned_error
 from bytecodemanipulation.assembler.util.parser import AbstractExpression
-from bytecodemanipulation.assembler.util.tokenizer import IdentifierToken
 from bytecodemanipulation.data.shared.expressions.CompoundExpression import (
     CompoundExpression,
 )
 from bytecodemanipulation.data.shared.instructions.AbstractInstruction import (
     AbstractAssemblyInstruction,
 )
 
 
-class AbstractWhileAssembly(AbstractAssemblyInstruction, abc.ABC):
-    # # WHILE <expression> ['\'' <label name> '\''] '{' <body> '}'
-    NAME = "WHILE"
+class AbstractIFAssembly(AbstractAssemblyInstruction, abc.ABC):
+    # IF <expression> ['\'' <label name> '\''] '{' <body> '}'
+    NAME = "IF"
 
     @classmethod
-    def consume(cls, parser: "Parser", scope: ParsingScope) -> "AbstractWhileAssembly":
-        condition = parser.try_parse_data_source(
+    def consume(cls, parser: "Parser", scope: ParsingScope) -> "AbstractIFAssembly":
+        source = parser.try_parse_data_source(
             allow_primitives=True, include_bracket=False, scope=scope
         )
 
-        if condition is None:
-            raise throw_positioned_syntax_error(
+        if source is None:
+            raise throw_positioned_error(
                 scope, parser.try_inspect(), "expected <expression>"
             )
 
         if parser.try_consume(SpecialToken("'")):
             label_name = parser.parse_identifier_like(scope)
             if not parser.try_consume(SpecialToken("'")):
-                raise throw_positioned_syntax_error(
+                raise throw_positioned_error(
                     scope, parser.try_inspect(), "expected '"
                 )
         else:
             label_name = None
 
         body = parser.parse_body(scope=scope)
 
         return cls(
-            condition,
+            source,
             body,
             label_name,
         )
 
     def __init__(
         self,
         source: AbstractSourceExpression,
         body: CompoundExpression,
-        label_name: IIdentifierAccessor | None = None,
+        label_name: IIdentifierAccessor | str = None,
     ):
         self.source = source
         self.body = body
         self.label_name = (
             label_name
             if not isinstance(label_name, str)
             else StaticIdentifier(label_name)
@@ -74,36 +73,41 @@
             and self.source == other.source
             and self.body == other.body
             and self.label_name == other.label_name
         )
 
     def __repr__(self):
         c = "'"
-        return f"WHILE({self.source}{'' if self.label_name is None else ', label='+c+repr(self.label_name)+c}) -> {{{self.body}}}"
+        return f"IF({self.source}{'' if self.label_name is None else ', label='+c+repr(self.label_name)+c}) -> {{{self.body}}}"
 
     def visit_parts(
         self,
         visitor: typing.Callable[
             [IAssemblyStructureVisitable, tuple, typing.List[AbstractExpression]],
             typing.Any,
         ],
         parents: list,
     ):
         return visitor(
-            self, (self.source.visit_parts(visitor), self.body.visit_parts(visitor))
+            self,
+            (
+                self.source.visit_parts(visitor, parents + [self]),
+                self.body.visit_parts(visitor, parents + [self]),
+            ),
+            parents,
         )
 
     def visit_assembly_instructions(
         self, visitor: typing.Callable[[IAssemblyStructureVisitable, tuple], typing.Any]
     ):
         return visitor(self, (self.body.visit_assembly_instructions(visitor),))
 
-    def get_labels(self, scope: ParsingScope):
+    def get_labels(self, scope: ParsingScope) -> typing.Set[str]:
         return (
             set()
             if self.label_name is None
             else {
                 self.label_name(scope),
                 self.label_name(scope) + "_END",
-                self.label_name(scope) + "_INNER",
+                self.label_name(scope) + "_HEAD",
             }
         ) | self.body.get_labels(scope)
```

### Comparing `bytecodemanipulation-0.3.1/bytecodemanipulation/data/v3_10/assembly_instructions.py` & `bytecodemanipulation-0.3.3/bytecodemanipulation/data/v3_10/assembly_instructions.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.3.1/bytecodemanipulation/data/v3_10/instructions/AssertAssembly.py` & `bytecodemanipulation-0.3.3/bytecodemanipulation/data/v3_10/instructions/WhileAssembly.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,41 +1,46 @@
-import typing
-
-from bytecodemanipulation.assembler.AbstractBase import JumpToLabel
-from bytecodemanipulation.opcodes.Opcodes import Opcodes
-from bytecodemanipulation.assembler.AbstractBase import ParsingScope
-from bytecodemanipulation.MutableFunction import MutableFunction
-from bytecodemanipulation.opcodes.Instruction import Instruction
 from bytecodemanipulation.assembler.Parser import Parser
-from bytecodemanipulation.data.shared.instructions.AssertAssembly import (
-    AbstractAssertAssembly,
+from bytecodemanipulation.assembler.AbstractBase import ParsingScope
+from bytecodemanipulation.data.shared.instructions.WhileAssembly import (
+    AbstractWhileAssembly,
 )
+from bytecodemanipulation.opcodes.Instruction import Instruction
+from bytecodemanipulation.MutableFunction import MutableFunction
+from bytecodemanipulation.opcodes.Opcodes import Opcodes
 
 
 @Parser.register
-class AssertAssembly(AbstractAssertAssembly):
-    def emit_bytecodes(
-        self, function: MutableFunction, scope: ParsingScope
-    ) -> typing.List[Instruction]:
-        bytecode = self.source.emit_bytecodes(function, scope)
-
-        end_label = scope.scope_name_generator("assert_success")
-
-        bytecode += [
-            Instruction(function, -1, Opcodes.POP_JUMP_IF_TRUE, JumpToLabel(end_label)),
-        ]
-
-        if self.text:
-            bytecode += self.text.emit_bytecodes(function, scope)
+class WHILEAssembly(AbstractWhileAssembly):
+    def emit_bytecodes(self, function: MutableFunction, scope: ParsingScope):
+        if self.label_name is None:
+            end = Instruction("NOP")
         else:
-            bytecode += [
-                Instruction(function, -1, Opcodes.LOAD_CONST, "assertion failed")
-            ]
-
-        bytecode += [
-            Instruction(function, -1, Opcodes.LOAD_CONST, AssertionError),
-            Instruction(function, -1, Opcodes.ROT_TWO),
-            Instruction(function, -1, Opcodes.CALL_FUNCTION, arg=1),
-            Instruction(function, -1, Opcodes.RAISE_VARARGS, arg=1),
-            Instruction(function, -1, Opcodes.BYTECODE_LABEL, end_label),
-        ]
-        return bytecode
+            end = Instruction(
+                function, -1, Opcodes.BYTECODE_LABEL, self.label_name.text + "_END"
+            )
+
+        CONDITION = self.source.emit_bytecodes(function, scope)
+
+        if self.label_name:
+            CONDITION.insert(
+                0,
+                Instruction(Opcodes.BYTECODE_LABEL, self.label_name.text),
+            )
+
+        HEAD = Instruction("POP_JUMP_IF_FALSE", end)
+
+        BODY = self.body.emit_bytecodes(function, scope)
+
+        if self.label_name:
+            BODY.insert(
+                0,
+                Instruction(
+                    function,
+                    -1,
+                    Opcodes.BYTECODE_LABEL,
+                    self.label_name.text + "_INNER",
+                ),
+            )
+
+        JUMP_BACK = Instruction("JUMP_ABSOLUTE", CONDITION[0])
+
+        return CONDITION + [HEAD] + BODY + [JUMP_BACK, end]
```

### Comparing `bytecodemanipulation-0.3.1/bytecodemanipulation/data/v3_10/instructions/CallAssembly.py` & `bytecodemanipulation-0.3.3/bytecodemanipulation/data/v3_10/instructions/CallAssembly.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 )
 from bytecodemanipulation.data.shared.expressions.MacroAccessExpression import (
     MacroAccessExpression,
 )
 from bytecodemanipulation.data.shared.instructions.MacroAssembly import MacroAssembly
 from bytecodemanipulation.assembler.Parser import Parser
 from bytecodemanipulation.assembler.AbstractBase import ParsingScope
-from bytecodemanipulation.assembler.syntax_errors import throw_positioned_syntax_error
+from bytecodemanipulation.assembler.syntax_errors import throw_positioned_error
 from bytecodemanipulation.opcodes.Instruction import Instruction
 from bytecodemanipulation.MutableFunction import MutableFunction
 from bytecodemanipulation.opcodes.Opcodes import Opcodes
 
 
 @Parser.register
 class CallAssembly(AbstractCallAssembly):
@@ -37,112 +37,108 @@
 
             elif isinstance(arg, CallAssembly.StarArg):
                 has_seen_star = True
 
         if not has_seen_kw_arg and not has_seen_star and not has_seen_star_star:
             if self.is_partial:
                 bytecode = [
-                    Instruction(function, -1, Opcodes.LOAD_CONST, functools.partial)
+                    Instruction(Opcodes.LOAD_CONST, functools.partial)
                 ]
                 extra_args = 1
             else:
                 bytecode = []
                 extra_args = 0
 
             bytecode += self.call_target.emit_bytecodes(function, scope)
 
             for arg in self.args:
                 bytecode += arg.source.emit_bytecodes(function, scope)
 
             bytecode += [
                 Instruction(
-                    function, -1, "CALL_FUNCTION", arg=len(self.args) + extra_args
+                    "CALL_FUNCTION", arg=len(self.args) + extra_args
                 ),
             ]
 
         elif has_seen_kw_arg and not has_seen_star and not has_seen_star_star:
             if self.is_partial:
                 bytecode = [
-                    Instruction(function, -1, Opcodes.LOAD_CONST, functools.partial)
+                    Instruction(Opcodes.LOAD_CONST, functools.partial)
                 ]
                 extra_args = 1
             else:
                 bytecode = []
                 extra_args = 0
 
             bytecode += self.call_target.emit_bytecodes(function, scope)
 
             kw_arg_keys = []
 
             for arg in reversed(self.args):
                 bytecode += arg.source.emit_bytecodes(function, scope)
 
                 if isinstance(arg, CallAssembly.KwArg):
-                    kw_arg_keys.append(arg.key.text)
+                    kw_arg_keys.append(arg.key(scope))
 
                 kw_const = tuple(reversed(kw_arg_keys))
 
                 bytecode += [
-                    Instruction(function, -1, "LOAD_CONST", kw_const),
+                    Instruction(Opcodes.LOAD_CONST, kw_const),
                     Instruction(
-                        function,
-                        -1,
-                        "CALL_FUNCTION_KW",
+                        Opcodes.CALL_FUNCTION_KW,
                         arg=len(self.args) + extra_args,
                     ),
                 ]
 
         else:
             bytecode = self.call_target.emit_bytecodes(function, scope)
 
-            bytecode += [Instruction(function, -1, "BUILD_LIST", arg=0)]
+            bytecode += [Instruction("BUILD_LIST", arg=0)]
 
             if self.is_partial:
                 bytecode += [
-                    Instruction(function, -1, Opcodes.LOAD_CONST, functools.partial),
-                    Instruction(function, -1, "LIST_APPEND"),
+                    Instruction(Opcodes.LOAD_CONST, functools.partial),
+                    Instruction(Opcodes.LIST_APPEND),
                 ]
 
             i = -1
             for i, arg in enumerate(self.args):
                 bytecode += arg.source.emit_bytecodes(function, scope)
 
                 if isinstance(arg, CallAssembly.Arg):
-                    bytecode += [Instruction(function, -1, "LIST_APPEND", arg=1)]
+                    bytecode += [Instruction("LIST_APPEND", arg=1)]
                 elif isinstance(arg, CallAssembly.StarArg):
-                    bytecode += [Instruction(function, -1, "LIST_EXTEND", arg=1)]
+                    bytecode += [Instruction("LIST_EXTEND", arg=1)]
                 else:
                     break
 
             bytecode += [
-                Instruction(function, -1, "LIST_TO_TUPLE"),
+                Instruction("LIST_TO_TUPLE"),
             ]
 
             if has_seen_kw_arg or has_seen_star_star:
-                bytecode += [Instruction(function, -1, "BUILD_MAP", arg=0)]
+                bytecode += [Instruction("BUILD_MAP", arg=0)]
 
                 for arg in self.args[i + 1 :]:
                     if isinstance(arg, CallAssembly.KwArg):
                         bytecode += (
-                            [Instruction(function, -1, "LOAD_CONST", arg.key.text)]
+                            [Instruction("LOAD_CONST", arg.key.text)]
                             + arg.source.emit_bytecodes(function, scope)
                             + [
-                                Instruction(function, -1, "BUILD_MAP", arg=1),
-                                Instruction(function, -1, "DICT_MERGE", arg=1),
+                                Instruction("BUILD_MAP", arg=1),
+                                Instruction("DICT_MERGE", arg=1),
                             ]
                         )
                     else:
                         bytecode += arg.source.emit_bytecodes(function, scope) + [
-                            Instruction(function, -1, "DICT_MERGE", arg=1)
+                            Instruction("DICT_MERGE", arg=1)
                         ]
 
             bytecode += [
                 Instruction(
-                    function,
-                    -1,
                     "CALL_FUNCTION_EX",
                     arg=int(has_seen_kw_arg or has_seen_star_star),
                 ),
             ]
 
         if self.target:
             bytecode += self.target.emit_store_bytecodes(function, scope)
@@ -152,15 +148,15 @@
     def emit_macro_bytecode(self, function: MutableFunction, scope: ParsingScope):
         access = typing.cast(MacroAccessExpression, self.call_target)
         name = access.name
 
         macro_declaration = scope.lookup_name_in_scope(name[0].text)
 
         if macro_declaration is None:
-            raise throw_positioned_syntax_error(
+            raise throw_positioned_error(
                 scope,
                 typing.cast(MacroAccessExpression, self.call_target).name,
                 f"Macro '{':'.join(map(lambda e: e.text, name))}' not found!",
                 NameError,
             )
 
         if len(name) > 1:
@@ -178,10 +174,10 @@
             raise RuntimeError(
                 f"Expected <return type> declaration at macro if using '->' in call"
             )
 
         bytecode = macro.emit_call_bytecode(function, scope, args)
 
         if self.target:
-            bytecode += self.target.emit_bytecodes(function, scope)
+            bytecode += self.target.emit_store_bytecodes(function, scope)
 
         return bytecode
```

### Comparing `bytecodemanipulation-0.3.1/bytecodemanipulation/data/v3_10/instructions/ClassDefinitionAssembly.py` & `bytecodemanipulation-0.3.3/bytecodemanipulation/data/v3_11/instructions/ClassDefinitionAssembly.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,18 +16,18 @@
         self, function: MutableFunction, scope: ParsingScope
     ) -> typing.List[Instruction]:
         inner_scope = scope.copy(sub_scope_name=self.name(scope))
 
         target = MutableFunction(lambda: None)
 
         inner_bytecode = [
-            Instruction(target, -1, Opcodes.LOAD_NAME, "__name__"),
-            Instruction(target, -1, Opcodes.STORE_NAME, "__module__"),
-            Instruction(target, -1, Opcodes.LOAD_CONST, self.name(scope)),
-            Instruction(target, -1, Opcodes.STORE_NAME, "__qualname__"),
+            Instruction(Opcodes.LOAD_NAME, "__name__"),
+            Instruction(Opcodes.STORE_NAME, "__module__"),
+            Instruction(Opcodes.LOAD_CONST, self.name(scope)),
+            Instruction(Opcodes.STORE_NAME, "__qualname__"),
         ]
 
         raw_inner_code = self.code_block.emit_bytecodes(target, inner_scope)
 
         for instr in raw_inner_code:
             if instr.opcode == Opcodes.LOAD_FAST:
                 instr.change_opcode(Opcodes.LOAD_NAME, arg_value=instr.arg_value)
@@ -35,36 +35,36 @@
                 instr.change_opcode(Opcodes.STORE_NAME, arg_value=instr.arg_value)
             elif instr.opcode == Opcodes.DELETE_FAST:
                 instr.change_opcode(Opcodes.DELETE_NAME, arg_value=instr.arg_value)
 
         inner_bytecode += raw_inner_code
 
         if inner_bytecode:
-            inner_bytecode[-1].next_instruction = target.instruction_entry_point
+            inner_bytecode[-1].next_instruction = target.instructions[0]
 
         for i, instr in enumerate(inner_bytecode[:-1]):
             instr.next_instruction = inner_bytecode[i + 1]
 
-        target.instruction_entry_point = inner_bytecode[0]
+        target.assemble_instructions_from_tree(inner_bytecode[0])
         target.reassign_to_function()
 
         code_obj = target.target.__code__
 
         bytecode = [
-            Instruction(function, -1, Opcodes.LOAD_BUILD_CLASS),
-            Instruction(function, -1, Opcodes.LOAD_CONST, code_obj),
-            Instruction(function, -1, Opcodes.LOAD_CONST, self.name(scope)),
-            Instruction(function, -1, Opcodes.MAKE_FUNCTION, arg=0),
-            Instruction(function, -1, Opcodes.LOAD_CONST, self.name(scope)),
+            Instruction(Opcodes.LOAD_BUILD_CLASS),
+            Instruction(Opcodes.LOAD_CONST, code_obj),
+            Instruction(Opcodes.LOAD_CONST, self.name(scope)),
+            Instruction(Opcodes.MAKE_FUNCTION, arg=0),
+            Instruction(Opcodes.LOAD_CONST, self.name(scope)),
         ]
 
         for parent in self.parents:
             bytecode += parent.emit_bytecodes(
                 function,
                 scope,
             )
 
         bytecode += [
-            Instruction(function, -1, Opcodes.CALL_FUNCTION, arg=2 + len(self.parents)),
-            Instruction(function, -1, Opcodes.STORE_FAST, self.name(scope)),
+            Instruction(Opcodes.CALL_FUNCTION, arg=2 + len(self.parents)),
+            Instruction(Opcodes.STORE_FAST, self.name(scope)),
         ]
         return bytecode
```

### Comparing `bytecodemanipulation-0.3.1/bytecodemanipulation/data/v3_10/instructions/ForEachAssembly.py` & `bytecodemanipulation-0.3.3/bytecodemanipulation/data/v3_10/instructions/ForEachAssembly.py`

 * *Files 13% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 class ForEachAssembly(AbstractForEachAssembly):
     def emit_bytecodes(
         self, function: MutableFunction, scope: ParsingScope
     ) -> typing.List[Instruction]:
         if len(self.variables) != 1:
             bytecode = [
                 Instruction.create_with_token(
-                    self.base_token, function, -1, Opcodes.LOAD_CONST, zip
+                    self.base_token, Opcodes.LOAD_CONST, zip
                 ),
             ]
         else:
             bytecode = []
 
         for source in self.sources:
             bytecode += source.emit_bytecodes(function, scope)
@@ -31,81 +31,65 @@
         loop_label_name_enter = scope.scope_name_generator("foreach_loop_enter")
         loop_label_name_exit = scope.scope_name_generator("foreach_loop_exit")
 
         if len(self.variables) != 1:
             bytecode += [
                 Instruction.create_with_token(
                     self.base_token,
-                    function,
-                    -1,
                     Opcodes.CALL_FUNCTION,
                     arg=len(self.sources),
                 ),
                 Instruction.create_with_token(
-                    self.base_token, function, -1, Opcodes.GET_ITER
+                    self.base_token, Opcodes.GET_ITER
                 ),
                 Instruction.create_with_token(
                     self.base_token,
-                    function,
-                    -1,
                     Opcodes.BYTECODE_LABEL,
                     loop_label_name_enter,
                 ),
                 Instruction.create_with_token(
                     self.base_token,
-                    function,
-                    -1,
                     Opcodes.FOR_ITER,
                     JumpToLabel(loop_label_name_exit),
                 ),
                 Instruction.create_with_token(
                     self.base_token,
-                    function,
-                    -1,
                     Opcodes.UNPACK_SEQUENCE,
                     arg=len(self.sources),
                 ),
             ]
         else:
             bytecode += [
                 Instruction.create_with_token(
-                    self.base_token, function, -1, Opcodes.GET_ITER
+                    self.base_token, Opcodes.GET_ITER
                 ),
                 Instruction.create_with_token(
                     self.base_token,
-                    function,
-                    -1,
                     Opcodes.BYTECODE_LABEL,
                     loop_label_name_enter,
                 ),
                 Instruction.create_with_token(
                     self.base_token,
-                    function,
-                    -1,
                     Opcodes.FOR_ITER,
                     JumpToLabel(loop_label_name_exit),
                 ),
             ]
 
         for var in self.variables:
             bytecode += var.emit_store_bytecodes(function, scope)
 
         bytecode += self.body.emit_bytecodes(function, scope)
 
         bytecode += [
             Instruction.create_with_token(
                 self.base_token,
-                function,
-                -1,
                 Opcodes.JUMP_ABSOLUTE,
                 JumpToLabel(loop_label_name_enter),
             ),
             Instruction.create_with_token(
                 self.base_token,
-                function,
-                -1,
                 Opcodes.BYTECODE_LABEL,
                 loop_label_name_exit,
             ),
         ]
 
         return bytecode
```

### Comparing `bytecodemanipulation-0.3.1/bytecodemanipulation/data/v3_10/instructions/FunctionDefinitionAssembly.py` & `bytecodemanipulation-0.3.3/bytecodemanipulation/data/v3_11/instructions/FunctionDefinitionAssembly.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,22 +42,22 @@
             tar = lambda: None
 
         target = MutableFunction(tar)
         inner_bytecode = []
 
         if self.bound_variables:
             for name, is_static in self.bound_variables:
-                # print(name, name(scope), is_static)
+                print(name, name(scope), is_static)
                 inner_bytecode += [
-                    Instruction(target, -1, Opcodes.LOAD_DEREF, name(scope) + "%inner"),
-                    Instruction(target, -1, Opcodes.STORE_DEREF, name(scope)),
+                    Instruction(Opcodes.LOAD_DEREF, name(scope) + "%inner"),
+                    Instruction(Opcodes.STORE_DEREF, name(scope)),
                 ]
 
         inner_bytecode += self.body.emit_bytecodes(target, inner_scope)
-        inner_bytecode[-1].next_instruction = target.instruction_entry_point
+        inner_bytecode[-1].next_instruction = target.instructions[0]
 
         for i, instr in enumerate(inner_bytecode[:-1]):
             instr.next_instruction = inner_bytecode[i + 1]
 
         def walk_label(instruction: Instruction):
             if instruction.opcode == Opcodes.BYTECODE_LABEL:
                 # print(instruction, instruction.next_instruction)
@@ -72,15 +72,15 @@
 
         def resolve_jump_to_label(ins: Instruction):
             if ins.has_jump() and isinstance(ins.arg_value, JumpToLabel):
                 ins.change_arg_value(label_targets[ins.arg_value.name])
 
         inner_bytecode[0].apply_visitor(LambdaInstructionWalker(resolve_jump_to_label))
 
-        target.instruction_entry_point = inner_bytecode[0]
+        target.assemble_instructions_from_tree(inner_bytecode[0])
         del inner_bytecode
 
         has_kwarg = False
         for arg in self.args:
             if isinstance(arg, AbstractCallAssembly.IMPLEMENTATION.KwArg):
                 has_kwarg = True
                 break
@@ -93,46 +93,45 @@
             if any(map(lambda e: e[1], self.bound_variables)):
                 raise NotImplementedError("Static variables")
 
             flags |= 0x08
 
             for name, is_static in self.bound_variables:
                 bytecode += [
-                    Instruction(function, -1, Opcodes.LOAD_FAST, name(scope)),
+                    Instruction(Opcodes.LOAD_FAST, name(scope)),
                     Instruction(
                         function, -1, Opcodes.STORE_DEREF, name(scope) + "%inner"
                     ),
                 ]
 
             bytecode += [
-                Instruction(function, -1, Opcodes.LOAD_CLOSURE, name(scope) + "%inner")
+                Instruction(Opcodes.LOAD_CLOSURE, name(scope) + "%inner")
                 for name, is_static in self.bound_variables
             ]
             bytecode.append(
                 Instruction(
                     function, -1, Opcodes.BUILD_TUPLE, arg=len(self.bound_variables)
                 )
             )
 
         target.argument_count = len(self.args)
-        target.prepare_previous_instructions()
         code_object = target.create_code_obj()
 
         bytecode += [
-            Instruction(function, -1, "LOAD_CONST", code_object),
+            Instruction("LOAD_CONST", code_object),
             Instruction(
                 function,
                 -1,
                 "LOAD_CONST",
                 self.func_name(scope) if self.func_name else "<lambda>",
             ),
-            Instruction(function, -1, "MAKE_FUNCTION", arg=flags),
+            Instruction("MAKE_FUNCTION", arg=flags),
         ]
 
         if self.target:
             bytecode += self.target.emit_store_bytecodes(function, scope)
         else:
             bytecode += [
-                Instruction(function, -1, Opcodes.STORE_FAST, self.func_name(scope)),
+                Instruction(Opcodes.STORE_FAST, self.func_name(scope)),
             ]
 
         return bytecode
```

### Comparing `bytecodemanipulation-0.3.1/bytecodemanipulation/data/v3_10/instructions/IfAssembly.py` & `bytecodemanipulation-0.3.3/bytecodemanipulation/data/v3_11/instructions/WhileAssembly.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,46 +1,46 @@
 from bytecodemanipulation.assembler.Parser import Parser
 from bytecodemanipulation.assembler.AbstractBase import ParsingScope
-from bytecodemanipulation.data.shared.instructions.IfAssembly import AbstractIFAssembly
+from bytecodemanipulation.data.shared.instructions.WhileAssembly import (
+    AbstractWhileAssembly,
+)
 from bytecodemanipulation.opcodes.Instruction import Instruction
 from bytecodemanipulation.MutableFunction import MutableFunction
 from bytecodemanipulation.opcodes.Opcodes import Opcodes
 
 
 @Parser.register
-class IFAssembly(AbstractIFAssembly):
+class WHILEAssembly(AbstractWhileAssembly):
     def emit_bytecodes(self, function: MutableFunction, scope: ParsingScope):
-
         if self.label_name is None:
-            end = Instruction(function, -1, "NOP")
+            end = Instruction("NOP")
         else:
             end = Instruction(
                 function, -1, Opcodes.BYTECODE_LABEL, self.label_name.text + "_END"
             )
 
-        return (
-            (
-                []
-                if self.label_name is None
-                else [
-                    Instruction(
-                        function,
-                        -1,
-                        Opcodes.BYTECODE_LABEL,
-                        self.label_name.text + "_HEAD",
-                    )
-                ]
+        CONDITION = self.source.emit_bytecodes(function, scope)
+
+        if self.label_name:
+            CONDITION.insert(
+                0,
+                Instruction(Opcodes.BYTECODE_LABEL, self.label_name.text),
             )
-            + self.source.emit_bytecodes(function, scope)
-            + [Instruction(function, -1, "POP_JUMP_IF_FALSE", end)]
-            + (
-                []
-                if self.label_name is None
-                else [
-                    Instruction(
-                        function, -1, Opcodes.BYTECODE_LABEL, self.label_name.text
-                    )
-                ]
+
+        HEAD = Instruction("POP_JUMP_IF_FALSE", end)
+
+        BODY = self.body.emit_bytecodes(function, scope)
+
+        if self.label_name:
+            BODY.insert(
+                0,
+                Instruction(
+                    function,
+                    -1,
+                    Opcodes.BYTECODE_LABEL,
+                    self.label_name.text + "_INNER",
+                ),
             )
-            + self.body.emit_bytecodes(function, scope)
-            + [end]
-        )
+
+        JUMP_BACK = Instruction("JUMP_ABSOLUTE", CONDITION[0])
+
+        return CONDITION + [HEAD] + BODY + [JUMP_BACK, end]
```

### Comparing `bytecodemanipulation-0.3.1/bytecodemanipulation/data/v3_10/instructions/JumpAssembly.py` & `bytecodemanipulation-0.3.3/bytecodemanipulation/data/v3_10/instructions/JumpAssembly.py`

 * *Files 9% similar despite different names*

```diff
@@ -22,22 +22,18 @@
             raise ValueError(
                 f"Label '{self.label_name_token.text}' is not valid in this context!"
             )
 
         if self.condition is None:
             return [
                 Instruction(
-                    function,
-                    -1,
                     Opcodes.JUMP_ABSOLUTE,
                     JumpToLabel(self.label_name_token.text),
                 )
             ]
 
         return self.condition.emit_bytecodes(function, scope) + [
             Instruction(
-                function,
-                -1,
                 Opcodes.POP_JUMP_IF_TRUE,
                 JumpToLabel(self.label_name_token.text),
             )
         ]
```

### Comparing `bytecodemanipulation-0.3.1/bytecodemanipulation/data/v3_10/instructions/LoadConstAssembly.py` & `bytecodemanipulation-0.3.3/bytecodemanipulation/data/v3_10/instructions/LoadConstAssembly.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.3.1/bytecodemanipulation/data/v3_10/instructions/LoadFastAssembly.py` & `bytecodemanipulation-0.3.3/bytecodemanipulation/data/v3_10/instructions/LoadFastAssembly.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,10 +15,10 @@
         self, function: MutableFunction, scope: ParsingScope
     ) -> typing.List[Instruction]:
         value = self.name_token.text
 
         if value.isdigit():
             value = int(value)
 
-        return [Instruction(function, -1, "LOAD_FAST", value)] + (
+        return [Instruction("LOAD_FAST", value)] + (
             self.target.emit_bytecodes(function, scope) if self.target else []
         )
```

### Comparing `bytecodemanipulation-0.3.1/bytecodemanipulation/data/v3_10/instructions/LoadGlobalAssembly.py` & `bytecodemanipulation-0.3.3/bytecodemanipulation/data/v3_10/instructions/LoadGlobalAssembly.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,10 +15,10 @@
         self, function: MutableFunction, scope: ParsingScope
     ) -> typing.List[Instruction]:
         value = self.name_token.text
 
         if value.isdigit():
             value = int(value)
 
-        return [Instruction(function, -1, "LOAD_GLOBAL", value)] + (
+        return [Instruction("LOAD_GLOBAL", value)] + (
             self.target.emit_bytecodes(function, scope) if self.target else []
         )
```

### Comparing `bytecodemanipulation-0.3.1/bytecodemanipulation/data/v3_10/instructions/OpAssembly.py` & `bytecodemanipulation-0.3.3/bytecodemanipulation/data/v3_10/instructions/OpAssembly.py`

 * *Files 19% similar despite different names*

```diff
@@ -23,38 +23,57 @@
         lhs: AbstractSourceExpression,
         rhs: AbstractSourceExpression,
     ) -> typing.List[Instruction]:
         label_name = scope.scope_name_generator("and_skip_second")
 
         bytecode = lhs.emit_bytecodes(function, scope)
         bytecode += [
-            Instruction(function, -1, Opcodes.DUP_TOP),
+            Instruction(Opcodes.DUP_TOP),
             Instruction(
-                function, -1, Opcodes.POP_JUMP_IF_FALSE, JumpToLabel(label_name)
+                Opcodes.POP_JUMP_IF_FALSE, JumpToLabel(label_name)
             ),
-            Instruction(function, -1, Opcodes.POP_TOP),
+            Instruction(Opcodes.POP_TOP),
         ]
         bytecode += rhs.emit_bytecodes(function, scope)
         bytecode += [
-            Instruction(function, -1, Opcodes.BYTECODE_LABEL, label_name),
-            Instruction(function, -1, Opcodes.UNARY_NOT, bool),
+            Instruction(Opcodes.BYTECODE_LABEL, label_name),
+            Instruction(Opcodes.UNARY_NOT, bool),
         ]
         return bytecode
 
 
 class AndOperator(NandOperator):
     def emit_bytecodes(
         self,
         function: MutableFunction,
         scope: ParsingScope,
         lhs: AbstractSourceExpression,
         rhs: AbstractSourceExpression,
     ) -> typing.List[Instruction]:
         return super().emit_bytecodes(function, scope, lhs, rhs) + [
-            Instruction(function, -1, Opcodes.UNARY_NOT, bool)
+            Instruction(Opcodes.UNARY_NOT, bool)
+        ]
+
+
+class AndEvalOperator(NandOperator):
+    def emit_bytecodes(
+        self,
+        function: MutableFunction,
+        scope: ParsingScope,
+        lhs: AbstractSourceExpression,
+        rhs: AbstractSourceExpression,
+    ) -> typing.List[Instruction]:
+        inner_label = scope.scope_name_generator("and_eval_swap_skip")
+
+        return lhs.emit_bytecodes(function, scope) + rhs.emit_bytecodes(function, scope) + [
+            Instruction(Opcodes.DUP_TOP),
+            Instruction(Opcodes.POP_JUMP_IF_TRUE, JumpToLabel(inner_label)),
+            Instruction(Opcodes.ROT_TWO),
+            Instruction(Opcodes.BYTECODE_LABEL, inner_label),
+            Instruction(Opcodes.POP_TOP),
         ]
 
 
 class NorOperator(AbstractOperator):
     def emit_bytecodes(
         self,
         function: MutableFunction,
@@ -62,117 +81,111 @@
         lhs: AbstractSourceExpression,
         rhs: AbstractSourceExpression,
     ) -> typing.List[Instruction]:
         label_name = scope.scope_name_generator("or_skip_second")
 
         bytecode = lhs.emit_bytecodes(function, scope)
         bytecode += [
-            Instruction(function, -1, Opcodes.DUP_TOP),
+            Instruction(Opcodes.DUP_TOP),
             Instruction(
-                function, -1, Opcodes.POP_JUMP_IF_TRUE, JumpToLabel(label_name)
+                Opcodes.POP_JUMP_IF_TRUE, JumpToLabel(label_name)
             ),
-            Instruction(function, -1, Opcodes.POP_TOP),
+            Instruction(Opcodes.POP_TOP),
         ]
         bytecode += rhs.emit_bytecodes(function, scope)
         bytecode += [
-            Instruction(function, -1, Opcodes.BYTECODE_LABEL, label_name),
-            Instruction(function, -1, Opcodes.UNARY_NOT, bool),
+            Instruction(Opcodes.BYTECODE_LABEL, label_name),
+            Instruction(Opcodes.UNARY_NOT, bool),
         ]
         return bytecode
 
 
 class OrOperator(NorOperator):
     def emit_bytecodes(
         self,
         function: MutableFunction,
         scope: ParsingScope,
         lhs: AbstractSourceExpression,
         rhs: AbstractSourceExpression,
     ) -> typing.List[Instruction]:
         return super().emit_bytecodes(function, scope, lhs, rhs) + [
-            Instruction(function, -1, Opcodes.UNARY_NOT, bool)
+            Instruction(Opcodes.UNARY_NOT, bool)
         ]
 
 
 class OrEvalOperator(AbstractOperator):
     def emit_bytecodes(
         self,
         function: MutableFunction,
         scope: ParsingScope,
         lhs: AbstractSourceExpression,
         rhs: AbstractSourceExpression,
     ) -> typing.List[Instruction]:
-        label_name = scope.scope_name_generator("or_skip_second")
+        inner_label = scope.scope_name_generator("or_eval_swap_skip")
 
-        bytecode = lhs.emit_bytecodes(function, scope)
-        bytecode += [
-            Instruction(function, -1, Opcodes.DUP_TOP),
-            Instruction(
-                function, -1, Opcodes.POP_JUMP_IF_TRUE, JumpToLabel(label_name)
-            ),
-            Instruction(function, -1, Opcodes.POP_TOP),
+        return lhs.emit_bytecodes(function, scope) + rhs.emit_bytecodes(function, scope) + [
+            Instruction(Opcodes.DUP_TOP),
+            Instruction(Opcodes.POP_JUMP_IF_FALSE, JumpToLabel(inner_label)),
+            Instruction(Opcodes.ROT_TWO),
+            Instruction(Opcodes.BYTECODE_LABEL, inner_label),
+            Instruction(Opcodes.POP_TOP),
         ]
-        bytecode += rhs.emit_bytecodes(function, scope)
-        bytecode += [
-            Instruction(function, -1, Opcodes.BYTECODE_LABEL, label_name),
-        ]
-        return bytecode
 
 
 class XOROperator(AbstractOperator):
     def emit_bytecodes(
         self,
         function: MutableFunction,
         scope: ParsingScope,
         lhs: AbstractSourceExpression,
         rhs: AbstractSourceExpression,
     ) -> typing.List[Instruction]:
         bytecode = lhs.emit_bytecodes(function, scope)
         bytecode += [
-            Instruction(function, -1, Opcodes.UNARY_NOT),
+            Instruction(Opcodes.UNARY_NOT),
         ]
         bytecode += rhs.emit_bytecodes(function, scope)
         bytecode += [
-            Instruction(function, -1, Opcodes.UNARY_NOT),
-            Instruction(function, -1, Opcodes.COMPARE_OP, arg=3),
+            Instruction(Opcodes.UNARY_NOT),
+            Instruction(Opcodes.COMPARE_NEQ),
         ]
         return bytecode
 
 
 class XNOROperator(AbstractOperator):
     def emit_bytecodes(
         self,
         function: MutableFunction,
         scope: ParsingScope,
         lhs: AbstractSourceExpression,
         rhs: AbstractSourceExpression,
     ) -> typing.List[Instruction]:
         bytecode = lhs.emit_bytecodes(function, scope)
         bytecode += [
-            Instruction(function, -1, Opcodes.UNARY_NOT),
+            Instruction(Opcodes.UNARY_NOT),
         ]
         bytecode += rhs.emit_bytecodes(function, scope)
         bytecode += [
-            Instruction(function, -1, Opcodes.UNARY_NOT),
-            Instruction(function, -1, Opcodes.COMPARE_OP, arg=2),
+            Instruction(Opcodes.UNARY_NOT),
+            Instruction(Opcodes.COMPARE_EQ),
         ]
         return bytecode
 
 
 class WalrusOperator(AbstractOperator):
     def emit_bytecodes(
         self,
         function: MutableFunction,
         scope: ParsingScope,
         lhs: AbstractSourceExpression,
         rhs: AbstractSourceExpression,
     ) -> typing.List[Instruction]:
         bytecode = rhs.emit_bytecodes(function, scope)
         bytecode += [
-            Instruction(function, -1, Opcodes.DUP_TOP),
+            Instruction(Opcodes.DUP_TOP),
         ]
         bytecode += lhs.emit_store_bytecodes(function, scope)
         return bytecode
 
 
 class InverseWalrusOperator(AbstractOperator):
     def emit_bytecodes(
@@ -180,15 +193,15 @@
         function: MutableFunction,
         scope: ParsingScope,
         lhs: AbstractSourceExpression,
         rhs: AbstractSourceExpression,
     ) -> typing.List[Instruction]:
         bytecode = lhs.emit_bytecodes(function, scope)
         bytecode += [
-            Instruction(function, -1, Opcodes.DUP_TOP),
+            Instruction(Opcodes.DUP_TOP),
         ]
         bytecode += rhs.emit_store_bytecodes(function, scope)
         return bytecode
 
 
 class InstanceOfChecker(AbstractOperator):
     def emit_bytecodes(
@@ -198,17 +211,17 @@
         lhs: AbstractSourceExpression,
         rhs: AbstractSourceExpression,
     ) -> typing.List[Instruction]:
         bytecode = lhs.emit_bytecodes(function, scope) + rhs.emit_bytecodes(
             function, scope
         )
         bytecode += [
-            Instruction(function, -1, Opcodes.LOAD_CONST, isinstance),
-            Instruction(function, -1, Opcodes.ROT_THREE),
-            Instruction(function, -1, Opcodes.CALL_FUNCTION, arg=2),
+            Instruction(Opcodes.LOAD_CONST, isinstance),
+            Instruction(Opcodes.ROT_THREE),
+            Instruction(Opcodes.CALL_FUNCTION, arg=2),
         ]
         return bytecode
 
 
 class SubclassOfChecker(AbstractOperator):
     def emit_bytecodes(
         self,
@@ -217,17 +230,17 @@
         lhs: AbstractSourceExpression,
         rhs: AbstractSourceExpression,
     ) -> typing.List[Instruction]:
         bytecode = lhs.emit_bytecodes(function, scope) + rhs.emit_bytecodes(
             function, scope
         )
         bytecode += [
-            Instruction(function, -1, Opcodes.LOAD_CONST, issubclass),
-            Instruction(function, -1, Opcodes.ROT_THREE),
-            Instruction(function, -1, Opcodes.CALL_FUNCTION, arg=2),
+            Instruction(Opcodes.LOAD_CONST, issubclass),
+            Instruction(Opcodes.ROT_THREE),
+            Instruction(Opcodes.CALL_FUNCTION, arg=2),
         ]
         return bytecode
 
 
 class HasattrChecker(AbstractOperator):
     def emit_bytecodes(
         self,
@@ -236,17 +249,17 @@
         lhs: AbstractSourceExpression,
         rhs: AbstractSourceExpression,
     ) -> typing.List[Instruction]:
         bytecode = lhs.emit_bytecodes(function, scope) + rhs.emit_bytecodes(
             function, scope
         )
         bytecode += [
-            Instruction(function, -1, Opcodes.LOAD_CONST, hasattr),
-            Instruction(function, -1, Opcodes.ROT_THREE),
-            Instruction(function, -1, Opcodes.CALL_FUNCTION, arg=2),
+            Instruction(Opcodes.LOAD_CONST, hasattr),
+            Instruction(Opcodes.ROT_THREE),
+            Instruction(Opcodes.CALL_FUNCTION, arg=2),
         ]
         return bytecode
 
 
 class SumOperator(AbstractOperator):
     def emit_bytecodes(
         self,
@@ -257,15 +270,15 @@
         if len(parameters) == 0:
             raise SyntaxError("expected at least one parameter")
 
         bytecode = parameters[0].emit_bytecodes(function, scope)
 
         for param in parameters[1:]:
             bytecode += param.emit_bytecodes(function, scope)
-            bytecode.append(Instruction(function, -1, Opcodes.BINARY_ADD))
+            bytecode.append(Instruction(Opcodes.BINARY_ADD))
 
         return bytecode
 
 
 class ProdOperator(AbstractOperator):
     def emit_bytecodes(
         self,
@@ -276,15 +289,15 @@
         if len(parameters) == 0:
             raise SyntaxError("expected at least one parameter")
 
         bytecode = parameters[0].emit_bytecodes(function, scope)
 
         for param in parameters[1:]:
             bytecode += param.emit_bytecodes(function, scope)
-            bytecode.append(Instruction(function, -1, Opcodes.BINARY_MULTIPLY))
+            bytecode.append(Instruction(Opcodes.BINARY_MULTIPLY))
 
         return bytecode
 
 
 class AvgOperator(AbstractOperator):
     def emit_bytecodes(
         self,
@@ -295,19 +308,19 @@
         if len(parameters) == 0:
             raise SyntaxError("expected at least one parameter")
 
         bytecode = parameters[0].emit_bytecodes(function, scope)
 
         for param in parameters[1:]:
             bytecode += param.emit_bytecodes(function, scope)
-            bytecode.append(Instruction(function, -1, Opcodes.BINARY_ADD))
+            bytecode.append(Instruction(Opcodes.BINARY_ADD))
 
         bytecode += [
-            Instruction(function, -1, Opcodes.LOAD_CONST, len(parameters)),
-            Instruction(function, -1, Opcodes.BINARY_TRUE_DIVIDE),
+            Instruction(Opcodes.LOAD_CONST, len(parameters)),
+            Instruction(Opcodes.BINARY_TRUE_DIVIDE),
         ]
 
         return bytecode
 
 
 class AvgIOperator(AbstractOperator):
     def emit_bytecodes(
@@ -319,19 +332,19 @@
         if len(parameters) == 0:
             raise SyntaxError("expected at least one parameter")
 
         bytecode = parameters[0].emit_bytecodes(function, scope)
 
         for param in parameters[1:]:
             bytecode += param.emit_bytecodes(function, scope)
-            bytecode.append(Instruction(function, -1, Opcodes.BINARY_ADD))
+            bytecode.append(Instruction(Opcodes.BINARY_ADD))
 
         bytecode += [
-            Instruction(function, -1, Opcodes.LOAD_CONST, len(parameters)),
-            Instruction(function, -1, Opcodes.BINARY_FLOOR_DIVIDE),
+            Instruction(Opcodes.LOAD_CONST, len(parameters)),
+            Instruction(Opcodes.BINARY_FLOOR_DIVIDE),
         ]
 
         return bytecode
 
 
 @Parser.register
 class OpAssembly(AbstractOpAssembly):
@@ -349,31 +362,32 @@
         ">>": OpcodeBaseOperator(Opcodes.BINARY_RSHIFT),
         "<<": OpcodeBaseOperator(Opcodes.BINARY_LSHIFT),
         "@": OpcodeBaseOperator(Opcodes.BINARY_MATRIX_MULTIPLY),
         "is": OpcodeBaseOperator((Opcodes.IS_OP, 0)),
         "!is": OpcodeBaseOperator((Opcodes.IS_OP, 1)),
         "in": OpcodeBaseOperator((Opcodes.CONTAINS_OP, 0)),
         "!in": OpcodeBaseOperator((Opcodes.CONTAINS_OP, 1)),
-        "<": OpcodeBaseOperator((Opcodes.COMPARE_OP, 0)),
-        "<=": OpcodeBaseOperator((Opcodes.COMPARE_OP, 1)),
-        "==": OpcodeBaseOperator((Opcodes.COMPARE_OP, 2)),
-        "!=": OpcodeBaseOperator((Opcodes.COMPARE_OP, 3)),
-        ">": OpcodeBaseOperator((Opcodes.COMPARE_OP, 4)),
-        ">=": OpcodeBaseOperator((Opcodes.COMPARE_OP, 5)),
+        "<": OpcodeBaseOperator(Opcodes.COMPARE_LT),
+        "<=": OpcodeBaseOperator(Opcodes.COMPARE_LE),
+        "==": OpcodeBaseOperator(Opcodes.COMPARE_EQ),
+        "!=": OpcodeBaseOperator(Opcodes.COMPARE_NEQ),
+        ">": OpcodeBaseOperator(Opcodes.COMPARE_GT),
+        ">=": OpcodeBaseOperator(Opcodes.COMPARE_GE),
         "xor": XOROperator(),
         "!xor": XNOROperator(),
         "xnor": XNOROperator(),
         ":=": WalrusOperator(),
         "=:": InverseWalrusOperator(),
         "isinstance": InstanceOfChecker(),
         "instanceof": InstanceOfChecker(),
         "issubclass": SubclassOfChecker(),
         "subclassof": SubclassOfChecker(),
         "hasattr": HasattrChecker(),
         "and": AndOperator(),
+        "andeval": AndEvalOperator(),
         "!and": NandOperator(),
         "nand": NandOperator(),
         "or": OrOperator(),
         "oreval": OrEvalOperator(),
         "!or": NorOperator(),
         "nor": NorOperator(),
     }
```

### Comparing `bytecodemanipulation-0.3.1/bytecodemanipulation/data/v3_10/instructions/PopElementAssembly.py` & `bytecodemanipulation-0.3.3/bytecodemanipulation/data/v3_10/instructions/PopElementAssembly.py`

 * *Files 17% similar despite different names*

```diff
@@ -11,10 +11,10 @@
 
 @Parser.register
 class PopElementAssembly(AbstractPopElementAssembly):
     def emit_bytecodes(
         self, function: MutableFunction, scope: ParsingScope
     ) -> typing.List[Instruction]:
         return [
-            Instruction(function, -1, "POP_TOP", int(self.count.text))
+            Instruction("POP_TOP", int(self.count.text))
             for _ in range(int(self.count.text))
         ]
```

### Comparing `bytecodemanipulation-0.3.1/bytecodemanipulation/data/v3_10/instructions/RaiseAssembly.py` & `bytecodemanipulation-0.3.3/bytecodemanipulation/data/v3_10/instructions/RaiseAssembly.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,8 +13,8 @@
 @Parser.register
 class RaiseAssembly(AbstractRaiseAssembly):
     def emit_bytecodes(
         self, function: MutableFunction, scope: ParsingScope
     ) -> typing.List[Instruction]:
         return (
             [] if self.source is None else self.source.emit_bytecodes(function, scope)
-        ) + [Instruction(function, -1, Opcodes.RAISE_VARARGS, arg=1)]
+        ) + [Instruction(Opcodes.RAISE_VARARGS, arg=1)]
```

### Comparing `bytecodemanipulation-0.3.1/bytecodemanipulation/data/v3_10/instructions/ReturnAssembly.py` & `bytecodemanipulation-0.3.3/bytecodemanipulation/data/v3_10/instructions/ReturnAssembly.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,17 +3,18 @@
 from bytecodemanipulation.assembler.Parser import Parser
 from bytecodemanipulation.assembler.AbstractBase import ParsingScope
 from bytecodemanipulation.data.shared.instructions.ReturnAssembly import (
     AbstractReturnAssembly,
 )
 from bytecodemanipulation.opcodes.Instruction import Instruction
 from bytecodemanipulation.MutableFunction import MutableFunction
+from bytecodemanipulation.opcodes.Opcodes import Opcodes
 
 
 @Parser.register
 class ReturnAssembly(AbstractReturnAssembly):
     def emit_bytecodes(
         self, function: MutableFunction, scope: ParsingScope
     ) -> typing.List[Instruction]:
         expr_bytecode = self.expr.emit_bytecodes(function, scope) if self.expr else []
 
-        return expr_bytecode + [Instruction(function, -1, "RETURN_VALUE")]
+        return expr_bytecode + [Instruction(Opcodes.RETURN_VALUE)]
```

### Comparing `bytecodemanipulation-0.3.1/bytecodemanipulation/data/v3_10/instructions/StoreFastAssembly.py` & `bytecodemanipulation-0.3.3/bytecodemanipulation/data/v3_10/instructions/StoreFastAssembly.py`

 * *Files 15% similar despite different names*

```diff
@@ -17,8 +17,8 @@
         value = self.name_token.text
 
         if value.isdigit():
             value = int(value)
 
         return (
             [] if self.source is None else self.source.emit_bytecodes(function, scope)
-        ) + [Instruction(function, -1, "STORE_FAST", value)]
+        ) + [Instruction("STORE_FAST", value)]
```

### Comparing `bytecodemanipulation-0.3.1/bytecodemanipulation/data/v3_10/instructions/StoreGlobalAssembly.py` & `bytecodemanipulation-0.3.3/bytecodemanipulation/data/v3_11/instructions/LoadGlobalAssembly.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import typing
 
 from bytecodemanipulation.assembler.Parser import Parser
 from bytecodemanipulation.assembler.AbstractBase import ParsingScope
-from bytecodemanipulation.data.shared.instructions.StoreGlobalAssembly import (
-    AbstractStoreGlobalAssembly,
+from bytecodemanipulation.data.shared.instructions.LoadGlobalAssembly import (
+    AbstractLoadGlobalAssembly,
 )
 from bytecodemanipulation.opcodes.Instruction import Instruction
 from bytecodemanipulation.MutableFunction import MutableFunction
 
 
 @Parser.register
-class StoreGlobalAssembly(AbstractStoreGlobalAssembly):
+class LoadGlobalAssembly(AbstractLoadGlobalAssembly):
     def emit_bytecodes(
         self, function: MutableFunction, scope: ParsingScope
     ) -> typing.List[Instruction]:
         value = self.name_token.text
 
         if value.isdigit():
             value = int(value)
 
-        return (
-            [] if self.source is None else self.source.emit_bytecodes(function, scope)
-        ) + [Instruction(function, -1, "STORE_GLOBAL", value)]
+        return [Instruction("LOAD_GLOBAL", value)] + (
+            self.target.emit_bytecodes(function, scope) if self.target else []
+        )
```

### Comparing `bytecodemanipulation-0.3.1/bytecodemanipulation/data/v3_10/instructions/WhileAssembly.py` & `bytecodemanipulation-0.3.3/bytecodemanipulation/data/v3_11/instructions/JumpAssembly.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,46 +1,39 @@
+import typing
+
+from bytecodemanipulation.assembler.AbstractBase import JumpToLabel
 from bytecodemanipulation.assembler.Parser import Parser
 from bytecodemanipulation.assembler.AbstractBase import ParsingScope
-from bytecodemanipulation.data.shared.instructions.WhileAssembly import (
-    AbstractWhileAssembly,
+from bytecodemanipulation.data.shared.instructions.JumpAssembly import (
+    AbstractJumpAssembly,
 )
 from bytecodemanipulation.opcodes.Instruction import Instruction
 from bytecodemanipulation.MutableFunction import MutableFunction
 from bytecodemanipulation.opcodes.Opcodes import Opcodes
 
 
 @Parser.register
-class WHILEAssembly(AbstractWhileAssembly):
-    def emit_bytecodes(self, function: MutableFunction, scope: ParsingScope):
-        if self.label_name is None:
-            end = Instruction(function, -1, "NOP")
-        else:
-            end = Instruction(
-                function, -1, Opcodes.BYTECODE_LABEL, self.label_name.text + "_END"
-            )
+class JumpAssembly(AbstractJumpAssembly):
+    # JUMP <label name> [(IF <condition access>) | ('(' <expression> | <op expression> ')')]
 
-        CONDITION = self.source.emit_bytecodes(function, scope)
-
-        if self.label_name:
-            CONDITION.insert(
-                0,
-                Instruction(function, -1, Opcodes.BYTECODE_LABEL, self.label_name.text),
+    def emit_bytecodes(
+        self, function: MutableFunction, scope: ParsingScope
+    ) -> typing.List[Instruction]:
+        if not scope.exists_label(self.label_name_token.text):
+            raise ValueError(
+                f"Label '{self.label_name_token.text}' is not valid in this context!"
             )
 
-        HEAD = Instruction(function, -1, "POP_JUMP_IF_FALSE", end)
-
-        BODY = self.body.emit_bytecodes(function, scope)
-
-        if self.label_name:
-            BODY.insert(
-                0,
+        if self.condition is None:
+            return [
                 Instruction(
-                    function,
-                    -1,
-                    Opcodes.BYTECODE_LABEL,
-                    self.label_name.text + "_INNER",
-                ),
+                    Opcodes.JUMP_ABSOLUTE,
+                    JumpToLabel(self.label_name_token.text),
+                )
+            ]
+
+        return self.condition.emit_bytecodes(function, scope) + [
+            Instruction(
+                Opcodes.POP_JUMP_IF_TRUE,
+                JumpToLabel(self.label_name_token.text),
             )
-
-        JUMP_BACK = Instruction(function, -1, "JUMP_ABSOLUTE", CONDITION[0])
-
-        return CONDITION + [HEAD] + BODY + [JUMP_BACK, end]
+        ]
```

### Comparing `bytecodemanipulation-0.3.1/bytecodemanipulation/data/v3_10/instructions/YieldAssembly.py` & `bytecodemanipulation-0.3.3/bytecodemanipulation/data/v3_10/instructions/YieldAssembly.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,26 +18,26 @@
         bytecode = []
 
         if self.expr:
             bytecode += self.expr.emit_bytecodes(function, scope)
 
         if self.is_star:
             bytecode += [
-                Instruction(function, -1, Opcodes.GET_YIELD_FROM_ITER),
-                Instruction(function, -1, Opcodes.LOAD_CONST, None),
-                Instruction(function, -1, Opcodes.YIELD_FROM),
+                Instruction(Opcodes.GET_YIELD_FROM_ITER),
+                Instruction(Opcodes.LOAD_CONST, None),
+                Instruction(Opcodes.YIELD_FROM),
             ]
 
         else:
             bytecode += [
-                Instruction(function, -1, Opcodes.YIELD_VALUE),
+                Instruction(Opcodes.YIELD_VALUE),
             ]
 
         if self.target:
             bytecode += self.target.emit_store_bytecodes(function, scope)
 
         else:
-            bytecode += [Instruction(function, -1, Opcodes.POP_TOP)]
+            bytecode += [Instruction(Opcodes.POP_TOP)]
 
         # print(bytecode)
 
         return bytecode
```

### Comparing `bytecodemanipulation-0.3.1/bytecodemanipulation/data/v3_11/assembly_instructions.py` & `bytecodemanipulation-0.3.3/bytecodemanipulation/data/v3_11/assembly_instructions.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.3.1/bytecodemanipulation/data/v3_11/instructions/CallAssembly.py` & `bytecodemanipulation-0.3.3/bytecodemanipulation/data/v3_11/instructions/CallAssembly.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 )
 from bytecodemanipulation.data.shared.expressions.MacroAccessExpression import (
     MacroAccessExpression,
 )
 from bytecodemanipulation.data.shared.instructions.MacroAssembly import MacroAssembly
 from bytecodemanipulation.assembler.Parser import Parser
 from bytecodemanipulation.assembler.AbstractBase import ParsingScope
-from bytecodemanipulation.assembler.syntax_errors import throw_positioned_syntax_error
+from bytecodemanipulation.assembler.syntax_errors import throw_positioned_error
 from bytecodemanipulation.opcodes.Instruction import Instruction
 from bytecodemanipulation.MutableFunction import MutableFunction
 from bytecodemanipulation.opcodes.Opcodes import Opcodes
 
 
 @Parser.register
 class CallAssembly(AbstractCallAssembly):
@@ -37,36 +37,36 @@
 
             elif isinstance(arg, CallAssembly.StarArg):
                 has_seen_star = True
 
         if not has_seen_kw_arg and not has_seen_star and not has_seen_star_star:
             if self.is_partial:
                 bytecode = [
-                    Instruction(function, -1, Opcodes.LOAD_CONST, functools.partial)
+                    Instruction(Opcodes.LOAD_CONST, functools.partial)
                 ]
                 extra_args = 1
             else:
                 bytecode = []
                 extra_args = 0
 
             bytecode += self.call_target.emit_bytecodes(function, scope)
 
             for arg in self.args:
                 bytecode += arg.source.emit_bytecodes(function, scope)
 
             bytecode += [
                 Instruction(
-                    function, -1, "CALL_FUNCTION", arg=len(self.args) + extra_args
+                    Opcodes.CALL_FUNCTION, arg=len(self.args) + extra_args
                 ),
             ]
 
         elif has_seen_kw_arg and not has_seen_star and not has_seen_star_star:
             if self.is_partial:
                 bytecode = [
-                    Instruction(function, -1, Opcodes.LOAD_CONST, functools.partial)
+                    Instruction(Opcodes.LOAD_CONST, functools.partial)
                 ]
                 extra_args = 1
             else:
                 bytecode = []
                 extra_args = 0
 
             bytecode += self.call_target.emit_bytecodes(function, scope)
@@ -78,65 +78,65 @@
 
                 if isinstance(arg, CallAssembly.KwArg):
                     kw_arg_keys.append(arg.key.text)
 
                 kw_const = tuple(reversed(kw_arg_keys))
 
                 bytecode += [
-                    Instruction(function, -1, "LOAD_CONST", kw_const),
+                    Instruction("LOAD_CONST", kw_const),
                     Instruction(
                         function,
                         -1,
                         "CALL_FUNCTION_KW",
                         arg=len(self.args) + extra_args,
                     ),
                 ]
 
         else:
             bytecode = self.call_target.emit_bytecodes(function, scope)
 
-            bytecode += [Instruction(function, -1, "BUILD_LIST", arg=0)]
+            bytecode += [Instruction("BUILD_LIST", arg=0)]
 
             if self.is_partial:
                 bytecode += [
-                    Instruction(function, -1, Opcodes.LOAD_CONST, functools.partial),
-                    Instruction(function, -1, "LIST_APPEND"),
+                    Instruction(Opcodes.LOAD_CONST, functools.partial),
+                    Instruction("LIST_APPEND"),
                 ]
 
             i = -1
             for i, arg in enumerate(self.args):
                 bytecode += arg.source.emit_bytecodes(function, scope)
 
                 if isinstance(arg, CallAssembly.Arg):
-                    bytecode += [Instruction(function, -1, "LIST_APPEND", arg=1)]
+                    bytecode += [Instruction("LIST_APPEND", arg=1)]
                 elif isinstance(arg, CallAssembly.StarArg):
-                    bytecode += [Instruction(function, -1, "LIST_EXTEND", arg=1)]
+                    bytecode += [Instruction("LIST_EXTEND", arg=1)]
                 else:
                     break
 
             bytecode += [
-                Instruction(function, -1, "LIST_TO_TUPLE"),
+                Instruction("LIST_TO_TUPLE"),
             ]
 
             if has_seen_kw_arg or has_seen_star_star:
-                bytecode += [Instruction(function, -1, "BUILD_MAP", arg=0)]
+                bytecode += [Instruction("BUILD_MAP", arg=0)]
 
                 for arg in self.args[i + 1 :]:
                     if isinstance(arg, CallAssembly.KwArg):
                         bytecode += (
-                            [Instruction(function, -1, "LOAD_CONST", arg.key.text)]
+                            [Instruction("LOAD_CONST", arg.key.text)]
                             + arg.source.emit_bytecodes(function, scope)
                             + [
-                                Instruction(function, -1, "BUILD_MAP", arg=1),
-                                Instruction(function, -1, "DICT_MERGE", arg=1),
+                                Instruction("BUILD_MAP", arg=1),
+                                Instruction("DICT_MERGE", arg=1),
                             ]
                         )
                     else:
                         bytecode += arg.source.emit_bytecodes(function, scope) + [
-                            Instruction(function, -1, "DICT_MERGE", arg=1)
+                            Instruction("DICT_MERGE", arg=1)
                         ]
 
             bytecode += [
                 Instruction(
                     function,
                     -1,
                     "CALL_FUNCTION_EX",
@@ -152,15 +152,15 @@
     def emit_macro_bytecode(self, function: MutableFunction, scope: ParsingScope):
         access = typing.cast(MacroAccessExpression, self.call_target)
         name = access.name
 
         macro_declaration = scope.lookup_name_in_scope(name[0].text)
 
         if macro_declaration is None:
-            raise throw_positioned_syntax_error(
+            raise throw_positioned_error(
                 scope,
                 typing.cast(MacroAccessExpression, self.call_target).name,
                 f"Macro '{':'.join(map(lambda e: e.text, name))}' not found!",
                 NameError,
             )
 
         if len(name) > 1:
```

### Comparing `bytecodemanipulation-0.3.1/bytecodemanipulation/data/v3_11/instructions/ClassDefinitionAssembly.py` & `bytecodemanipulation-0.3.3/bytecodemanipulation/data/v3_11/instructions/ForEachAssembly.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,70 +1,95 @@
 import typing
 
+from bytecodemanipulation.assembler.AbstractBase import JumpToLabel
 from bytecodemanipulation.assembler.Parser import Parser
 from bytecodemanipulation.assembler.AbstractBase import ParsingScope
-from bytecodemanipulation.data.shared.instructions.ClassDefinitionAssembly import (
-    AbstractClassDefinitionAssembly,
+from bytecodemanipulation.data.shared.instructions.ForEachAssembly import (
+    AbstractForEachAssembly,
 )
 from bytecodemanipulation.opcodes.Instruction import Instruction
 from bytecodemanipulation.MutableFunction import MutableFunction
 from bytecodemanipulation.opcodes.Opcodes import Opcodes
 
 
 @Parser.register
-class ClassDefinitionAssembly(AbstractClassDefinitionAssembly):
+class ForEachAssembly(AbstractForEachAssembly):
     def emit_bytecodes(
         self, function: MutableFunction, scope: ParsingScope
     ) -> typing.List[Instruction]:
-        inner_scope = scope.copy(sub_scope_name=self.name(scope))
+        if len(self.variables) != 1:
+            bytecode = [
+                Instruction.create_with_token(
+                    self.base_token, Opcodes.LOAD_CONST, zip
+                ),
+            ]
+        else:
+            bytecode = []
+
+        for source in self.sources:
+            bytecode += source.emit_bytecodes(function, scope)
+
+        loop_label_name_enter = scope.scope_name_generator("foreach_loop_enter")
+        loop_label_name_exit = scope.scope_name_generator("foreach_loop_exit")
+
+        if len(self.variables) != 1:
+            bytecode += [
+                Instruction.create_with_token(
+                    self.base_token,
+                    Opcodes.CALL_FUNCTION,
+                    arg=len(self.sources),
+                ),
+                Instruction.create_with_token(
+                    self.base_token, Opcodes.GET_ITER
+                ),
+                Instruction.create_with_token(
+                    self.base_token,
+                    Opcodes.BYTECODE_LABEL,
+                    loop_label_name_enter,
+                ),
+                Instruction.create_with_token(
+                    self.base_token,
+                    Opcodes.FOR_ITER,
+                    JumpToLabel(loop_label_name_exit),
+                ),
+                Instruction.create_with_token(
+                    self.base_token,
+                    Opcodes.UNPACK_SEQUENCE,
+                    arg=len(self.sources),
+                ),
+            ]
+        else:
+            bytecode += [
+                Instruction.create_with_token(
+                    self.base_token, Opcodes.GET_ITER
+                ),
+                Instruction.create_with_token(
+                    self.base_token,
+                    Opcodes.BYTECODE_LABEL,
+                    loop_label_name_enter,
+                ),
+                Instruction.create_with_token(
+                    self.base_token,
+                    Opcodes.FOR_ITER,
+                    JumpToLabel(loop_label_name_exit),
+                ),
+            ]
 
-        target = MutableFunction(lambda: None)
+        for var in self.variables:
+            bytecode += var.emit_store_bytecodes(function, scope)
 
-        inner_bytecode = [
-            Instruction(target, -1, Opcodes.LOAD_NAME, "__name__"),
-            Instruction(target, -1, Opcodes.STORE_NAME, "__module__"),
-            Instruction(target, -1, Opcodes.LOAD_CONST, self.name(scope)),
-            Instruction(target, -1, Opcodes.STORE_NAME, "__qualname__"),
-        ]
-
-        raw_inner_code = self.code_block.emit_bytecodes(target, inner_scope)
-
-        for instr in raw_inner_code:
-            if instr.opcode == Opcodes.LOAD_FAST:
-                instr.change_opcode(Opcodes.LOAD_NAME, arg_value=instr.arg_value)
-            elif instr.opcode == Opcodes.STORE_FAST:
-                instr.change_opcode(Opcodes.STORE_NAME, arg_value=instr.arg_value)
-            elif instr.opcode == Opcodes.DELETE_FAST:
-                instr.change_opcode(Opcodes.DELETE_NAME, arg_value=instr.arg_value)
-
-        inner_bytecode += raw_inner_code
-
-        if inner_bytecode:
-            inner_bytecode[-1].next_instruction = target.instructions[0]
-
-        for i, instr in enumerate(inner_bytecode[:-1]):
-            instr.next_instruction = inner_bytecode[i + 1]
-
-        target.assemble_instructions_from_tree(inner_bytecode[0])
-        target.reassign_to_function()
-
-        code_obj = target.target.__code__
-
-        bytecode = [
-            Instruction(function, -1, Opcodes.LOAD_BUILD_CLASS),
-            Instruction(function, -1, Opcodes.LOAD_CONST, code_obj),
-            Instruction(function, -1, Opcodes.LOAD_CONST, self.name(scope)),
-            Instruction(function, -1, Opcodes.MAKE_FUNCTION, arg=0),
-            Instruction(function, -1, Opcodes.LOAD_CONST, self.name(scope)),
-        ]
-
-        for parent in self.parents:
-            bytecode += parent.emit_bytecodes(
-                function,
-                scope,
-            )
+        bytecode += self.body.emit_bytecodes(function, scope)
 
         bytecode += [
-            Instruction(function, -1, Opcodes.CALL_FUNCTION, arg=2 + len(self.parents)),
-            Instruction(function, -1, Opcodes.STORE_FAST, self.name(scope)),
+            Instruction.create_with_token(
+                self.base_token,
+                Opcodes.JUMP_ABSOLUTE,
+                JumpToLabel(loop_label_name_enter),
+            ),
+            Instruction.create_with_token(
+                self.base_token,
+                Opcodes.BYTECODE_LABEL,
+                loop_label_name_exit,
+            ),
         ]
+
         return bytecode
```

### Comparing `bytecodemanipulation-0.3.1/bytecodemanipulation/data/v3_11/instructions/ForEachAssembly.py` & `bytecodemanipulation-0.3.3/bytecodemanipulation/mixin_util.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,111 +1,110 @@
 import typing
 
-from bytecodemanipulation.assembler.AbstractBase import JumpToLabel
-from bytecodemanipulation.assembler.Parser import Parser
-from bytecodemanipulation.assembler.AbstractBase import ParsingScope
-from bytecodemanipulation.data.shared.instructions.ForEachAssembly import (
-    AbstractForEachAssembly,
-)
-from bytecodemanipulation.opcodes.Instruction import Instruction
 from bytecodemanipulation.MutableFunction import MutableFunction
 from bytecodemanipulation.opcodes.Opcodes import Opcodes
 
 
-@Parser.register
-class ForEachAssembly(AbstractForEachAssembly):
-    def emit_bytecodes(
-        self, function: MutableFunction, scope: ParsingScope
-    ) -> typing.List[Instruction]:
-        if len(self.variables) != 1:
-            bytecode = [
-                Instruction.create_with_token(
-                    self.base_token, function, -1, Opcodes.LOAD_CONST, zip
-                ),
-            ]
-        else:
-            bytecode = []
-
-        for source in self.sources:
-            bytecode += source.emit_bytecodes(function, scope)
-
-        loop_label_name_enter = scope.scope_name_generator("foreach_loop_enter")
-        loop_label_name_exit = scope.scope_name_generator("foreach_loop_exit")
-
-        if len(self.variables) != 1:
-            bytecode += [
-                Instruction.create_with_token(
-                    self.base_token,
-                    function,
-                    -1,
-                    Opcodes.CALL_FUNCTION,
-                    arg=len(self.sources),
-                ),
-                Instruction.create_with_token(
-                    self.base_token, function, -1, Opcodes.GET_ITER
-                ),
-                Instruction.create_with_token(
-                    self.base_token,
-                    function,
-                    -1,
-                    Opcodes.BYTECODE_LABEL,
-                    loop_label_name_enter,
-                ),
-                Instruction.create_with_token(
-                    self.base_token,
-                    function,
-                    -1,
-                    Opcodes.FOR_ITER,
-                    JumpToLabel(loop_label_name_exit),
-                ),
-                Instruction.create_with_token(
-                    self.base_token,
-                    function,
-                    -1,
-                    Opcodes.UNPACK_SEQUENCE,
-                    arg=len(self.sources),
-                ),
-            ]
-        else:
-            bytecode += [
-                Instruction.create_with_token(
-                    self.base_token, function, -1, Opcodes.GET_ITER
-                ),
-                Instruction.create_with_token(
-                    self.base_token,
-                    function,
-                    -1,
-                    Opcodes.BYTECODE_LABEL,
-                    loop_label_name_enter,
-                ),
-                Instruction.create_with_token(
-                    self.base_token,
-                    function,
-                    -1,
-                    Opcodes.FOR_ITER,
-                    JumpToLabel(loop_label_name_exit),
-                ),
-            ]
-
-        for var in self.variables:
-            bytecode += var.emit_store_bytecodes(function, scope)
-
-        bytecode += self.body.emit_bytecodes(function, scope)
-
-        bytecode += [
-            Instruction.create_with_token(
-                self.base_token,
-                function,
-                -1,
-                Opcodes.JUMP_ABSOLUTE,
-                JumpToLabel(loop_label_name_enter),
-            ),
-            Instruction.create_with_token(
-                self.base_token,
-                function,
-                -1,
-                Opcodes.BYTECODE_LABEL,
-                loop_label_name_exit,
-            ),
-        ]
+def resolve_accesses(
+    inject_target: MutableFunction, injected: MutableFunction
+) -> typing.List[str]:
+    BOUND_LOCALS = {}
+    BOUND_CELL_VARIABLES = {}
+
+    def visit(instruction):
+        if instruction.has_local():
+            instruction.change_arg_value(
+                injected.function_name + "::" + instruction.arg_value
+            )
+
+    inject_target.walk_instructions(visit)
+
+    def visit(instruction):
+        if (
+            instruction.opcode in (Opcodes.CALL_METHOD, Opcodes.CALL_FUNCTION)
+            and instruction.arg <= 1
+        ):
+            source = next(instruction.trace_stack_position(instruction.arg))
+
+            if source.opcode == Opcodes.LOAD_CONST:
+                target = source.arg_value
+
+                if not isinstance(target, classmethod):
+                    return
+
+                func_name = target.__name__
+                is_const = True
+                source_source = None
+            elif source.opcode in (Opcodes.LOAD_ATTR, Opcodes.LOAD_METHOD):
+                source_source = next(source.trace_stack_position(0))
+
+                if (
+                    source_source.opcode == Opcodes.LOAD_FAST
+                    and source_source.arg_value in ("self", "cls")
+                ):
+                    func_name = source.arg_value
+                    is_const = False
+                else:
+                    return
+            else:
+                return
+
+            if func_name == "resolve_local":
+                assert (
+                    instruction.arg == 1
+                ), f"resolve_local() must be invoked with exactly one arg, got {instruction.arg}"
+
+                variable_name = next(instruction.trace_stack_position(0))
+
+                assert (
+                    variable_name.opcode == Opcodes.LOAD_CONST
+                ), f"resolve_local(<xy>) MUST be invoked with a constant, got {instruction}"
+
+                target = next(instruction.trace_stack_position_use(0))
+
+                if target.opcode == Opcodes.STORE_FAST:
+                    BOUND_LOCALS[target.arg_value] = variable_name.arg_value
+                else:
+                    instruction.change_opcode(Opcodes.LOAD_FAST)
+                    instruction.change_arg_value(variable_name.arg_value)
+                    source.change_opcode(Opcodes.NOP)
+
+                    if not is_const:
+                        source_source.change_opcode(Opcodes.NOP)
+
+            elif func_name == "resolve_cell_variable":
+                assert (
+                    instruction.arg == 1
+                ), f"resolve_cell_variable() must be invoked with exactly one arg, got {instruction.arg}"
+
+                variable_name = next(instruction.trace_stack_position(0))
+
+                assert (
+                    variable_name.opcode == Opcodes.LOAD_CONST
+                ), f"resolve_cell_variable(<xy>) MUST be invoked with a constant, got {instruction}"
+
+                target = next(instruction.trace_stack_position_use(0))
+
+                if target.opcode == Opcodes.STORE_FAST:
+                    BOUND_CELL_VARIABLES[target.arg_value] = variable_name
+                else:
+                    instruction.change_opcode(Opcodes.LOAD_DEREF)
+                    instruction.change_arg_value(variable_name.arg_value)
+
+                    instruction.change_arg_value(variable_name.arg_value)
+                    source.change_opcode(Opcodes.NOP)
+
+                    if not is_const:
+                        source_source.change_opcode(Opcodes.NOP)
+
+        elif instruction.has_local():
+            if instruction.arg_value in BOUND_LOCALS:
+                instruction.change_arg_value(BOUND_LOCALS[instruction.arg_value])
+            elif instruction.arg_value in BOUND_CELL_VARIABLES:
+                instruction.change_opcode(instruction.opname.replace("FAST", "DEREF"))
+                instruction.change_arg_value(
+                    BOUND_CELL_VARIABLES[instruction.arg_value]
+                )
 
-        return bytecode
+    injected.walk_instructions(visit)
+
+    return list(BOUND_LOCALS.keys())
```

### Comparing `bytecodemanipulation-0.3.1/bytecodemanipulation/data/v3_11/instructions/FunctionDefinitionAssembly.py` & `bytecodemanipulation-0.3.3/bytecodemanipulation/data/v3_10/instructions/FunctionDefinitionAssembly.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import typing
 
 from bytecodemanipulation.data.shared.instructions.FunctionDefinitionAssembly import (
     AbstractFunctionDefinitionAssembly,
 )
+from bytecodemanipulation.data.v3_10.instructions.CallAssembly import CallAssembly
 from bytecodemanipulation.opcodes.Instruction import Instruction
 from bytecodemanipulation.assembler.AbstractBase import JumpToLabel
 from bytecodemanipulation.assembler.Parser import Parser
 from bytecodemanipulation.assembler.AbstractBase import ParsingScope
 from bytecodemanipulation.data.shared.instructions.CallAssembly import (
     AbstractCallAssembly,
 )
@@ -22,15 +23,19 @@
     ) -> typing.List[Instruction]:
         flags = 0
         bytecode = []
 
         inner_labels = self.body.collect_label_info(scope)
         label_targets = {}
 
-        inner_scope = scope.copy()
+        inner_scope = scope.copy(shared_locals=False)
+
+        for arg in self.args:
+            if not isinstance(arg, (CallAssembly.Arg, CallAssembly.KwArg)):
+                inner_scope.filled_locals.add(arg.name(scope))
 
         if self.bound_variables:
             if any(map(lambda e: e[1], self.bound_variables)):
                 raise NotImplementedError("Static variables")
 
             names = [e[0](scope) for e in self.bound_variables]
             s = {}
@@ -42,96 +47,115 @@
             tar = lambda: None
 
         target = MutableFunction(tar)
         inner_bytecode = []
 
         if self.bound_variables:
             for name, is_static in self.bound_variables:
-                print(name, name(scope), is_static)
+                # print(name, name(scope), is_static)
                 inner_bytecode += [
-                    Instruction(target, -1, Opcodes.LOAD_DEREF, name(scope) + "%inner"),
-                    Instruction(target, -1, Opcodes.STORE_DEREF, name(scope)),
+                    Instruction(Opcodes.LOAD_DEREF, name(scope) + "%inner"),
+                    Instruction(Opcodes.STORE_DEREF, name(scope)),
                 ]
 
         inner_bytecode += self.body.emit_bytecodes(target, inner_scope)
-        inner_bytecode[-1].next_instruction = target.instructions[0]
+        inner_bytecode[-1].next_instruction = target.instruction_entry_point
 
         for i, instr in enumerate(inner_bytecode[:-1]):
             instr.next_instruction = inner_bytecode[i + 1]
 
         def walk_label(instruction: Instruction):
             if instruction.opcode == Opcodes.BYTECODE_LABEL:
                 # print(instruction, instruction.next_instruction)
                 label_targets[instruction.arg_value] = (
                     instruction.next_instruction
                     if instruction.next_instruction is not None
                     else instruction
                 )
-                instruction.change_opcode(Opcodes.NOP, update_next=False)
+                instruction.change_opcode(Opcodes.NOP)
 
         inner_bytecode[0].apply_visitor(LambdaInstructionWalker(walk_label))
 
         def resolve_jump_to_label(ins: Instruction):
             if ins.has_jump() and isinstance(ins.arg_value, JumpToLabel):
                 ins.change_arg_value(label_targets[ins.arg_value.name])
 
         inner_bytecode[0].apply_visitor(LambdaInstructionWalker(resolve_jump_to_label))
 
-        target.assemble_instructions_from_tree(inner_bytecode[0])
+        target.instruction_entry_point = inner_bytecode[0]
         del inner_bytecode
 
         has_kwarg = False
         for arg in self.args:
             if isinstance(arg, AbstractCallAssembly.IMPLEMENTATION.KwArg):
                 has_kwarg = True
                 break
 
         if has_kwarg:
-            flags |= 0x02
-            raise NotImplementedError("Kwarg defaults")
+            flags |= 0x01
+
+            defaults = []
+            c = 0
+
+            for arg in self.args:
+                if isinstance(arg, CallAssembly.KwArg):
+                    defaults += typing.cast(CallAssembly.KwArg, arg).source.emit_bytecodes(function, scope)
+                    c += 1
+
+            defaults += [
+                Instruction(Opcodes.BUILD_TUPLE, arg=c),
+            ]
+
+            bytecode += defaults
 
         if self.bound_variables:
             if any(map(lambda e: e[1], self.bound_variables)):
                 raise NotImplementedError("Static variables")
 
             flags |= 0x08
 
             for name, is_static in self.bound_variables:
                 bytecode += [
-                    Instruction(function, -1, Opcodes.LOAD_FAST, name(scope)),
+                    Instruction(Opcodes.LOAD_FAST, name(scope)),
                     Instruction(
-                        function, -1, Opcodes.STORE_DEREF, name(scope) + "%inner"
+                        Opcodes.STORE_DEREF, name(scope) + "%inner"
                     ),
                 ]
 
             bytecode += [
-                Instruction(function, -1, Opcodes.LOAD_CLOSURE, name(scope) + "%inner")
+                Instruction(Opcodes.LOAD_CLOSURE, name(scope) + "%inner")
                 for name, is_static in self.bound_variables
             ]
             bytecode.append(
                 Instruction(
-                    function, -1, Opcodes.BUILD_TUPLE, arg=len(self.bound_variables)
+                    Opcodes.BUILD_TUPLE, arg=len(self.bound_variables)
                 )
             )
 
         target.argument_count = len(self.args)
+
+        for arg in self.args:
+            if isinstance(arg, CallAssembly.Arg):
+                target.argument_names.append(arg.source(scope))
+            elif isinstance(arg, CallAssembly.KwArg):
+                target.argument_names.append(arg.key(scope))
+
+        target.prepare_previous_instructions()
         code_object = target.create_code_obj()
 
         bytecode += [
-            Instruction(function, -1, "LOAD_CONST", code_object),
+            Instruction(Opcodes.LOAD_CONST, code_object),
             Instruction(
-                function,
-                -1,
-                "LOAD_CONST",
+                Opcodes.LOAD_CONST,
                 self.func_name(scope) if self.func_name else "<lambda>",
             ),
-            Instruction(function, -1, "MAKE_FUNCTION", arg=flags),
+            Instruction(Opcodes.MAKE_FUNCTION, arg=flags),
         ]
 
         if self.target:
             bytecode += self.target.emit_store_bytecodes(function, scope)
         else:
             bytecode += [
-                Instruction(function, -1, Opcodes.STORE_FAST, self.func_name(scope)),
+                Instruction(Opcodes.STORE_FAST, self.prefix + self.func_name(scope)),
             ]
 
         return bytecode
```

### Comparing `bytecodemanipulation-0.3.1/bytecodemanipulation/data/v3_11/instructions/IfAssembly.py` & `bytecodemanipulation-0.3.3/bytecodemanipulation/data/v3_10/instructions/IfAssembly.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,40 +7,38 @@
 
 
 @Parser.register
 class IFAssembly(AbstractIFAssembly):
     def emit_bytecodes(self, function: MutableFunction, scope: ParsingScope):
 
         if self.label_name is None:
-            end = Instruction(function, -1, "NOP")
+            end = Instruction(Opcodes.NOP)
         else:
             end = Instruction(
-                function, -1, Opcodes.BYTECODE_LABEL, self.label_name.text + "_END"
+                Opcodes.BYTECODE_LABEL, self.label_name.text + "_END"
             )
 
         return (
             (
                 []
                 if self.label_name is None
                 else [
                     Instruction(
-                        function,
-                        -1,
                         Opcodes.BYTECODE_LABEL,
                         self.label_name.text + "_HEAD",
                     )
                 ]
             )
             + self.source.emit_bytecodes(function, scope)
-            + [Instruction(function, -1, "POP_JUMP_IF_FALSE", end)]
+            + [Instruction("POP_JUMP_IF_FALSE", end)]
             + (
                 []
                 if self.label_name is None
                 else [
                     Instruction(
-                        function, -1, Opcodes.BYTECODE_LABEL, self.label_name.text
+                        Opcodes.BYTECODE_LABEL, self.label_name.text
                     )
                 ]
             )
             + self.body.emit_bytecodes(function, scope)
             + [end]
         )
```

### Comparing `bytecodemanipulation-0.3.1/bytecodemanipulation/data/v3_11/instructions/LoadConstAssembly.py` & `bytecodemanipulation-0.3.3/bytecodemanipulation/data/v3_11/instructions/LoadConstAssembly.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.3.1/bytecodemanipulation/data/v3_11/instructions/LoadFastAssembly.py` & `bytecodemanipulation-0.3.3/bytecodemanipulation/data/v3_11/instructions/LoadFastAssembly.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,10 +15,10 @@
         self, function: MutableFunction, scope: ParsingScope
     ) -> typing.List[Instruction]:
         value = self.name_token.text
 
         if value.isdigit():
             value = int(value)
 
-        return [Instruction(function, -1, "LOAD_FAST", value)] + (
+        return [Instruction("LOAD_FAST", value)] + (
             self.target.emit_bytecodes(function, scope) if self.target else []
         )
```

### Comparing `bytecodemanipulation-0.3.1/bytecodemanipulation/data/v3_11/instructions/LoadGlobalAssembly.py` & `bytecodemanipulation-0.3.3/bytecodemanipulation/data/v3_10/instructions/StoreGlobalAssembly.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 import typing
 
 from bytecodemanipulation.assembler.Parser import Parser
 from bytecodemanipulation.assembler.AbstractBase import ParsingScope
-from bytecodemanipulation.data.shared.instructions.LoadGlobalAssembly import (
-    AbstractLoadGlobalAssembly,
+from bytecodemanipulation.data.shared.instructions.StoreGlobalAssembly import (
+    AbstractStoreGlobalAssembly,
 )
 from bytecodemanipulation.opcodes.Instruction import Instruction
 from bytecodemanipulation.MutableFunction import MutableFunction
+from bytecodemanipulation.opcodes.Opcodes import Opcodes
 
 
 @Parser.register
-class LoadGlobalAssembly(AbstractLoadGlobalAssembly):
+class StoreGlobalAssembly(AbstractStoreGlobalAssembly):
     def emit_bytecodes(
         self, function: MutableFunction, scope: ParsingScope
     ) -> typing.List[Instruction]:
         value = self.name_token.text
 
         if value.isdigit():
             value = int(value)
 
-        return [Instruction(function, -1, "LOAD_GLOBAL", value)] + (
-            self.target.emit_bytecodes(function, scope) if self.target else []
-        )
+        return (
+            [] if self.source is None else self.source.emit_bytecodes(function, scope)
+        ) + [Instruction(Opcodes.STORE_GLOBAL, value)]
```

### Comparing `bytecodemanipulation-0.3.1/bytecodemanipulation/data/v3_11/instructions/OpAssembly.py` & `bytecodemanipulation-0.3.3/bytecodemanipulation/data/v3_11/instructions/OpAssembly.py`

 * *Files 12% similar despite different names*

```diff
@@ -20,50 +20,50 @@
         ">>": Opcodes.BINARY_RSHIFT,
         "<<": Opcodes.BINARY_LSHIFT,
         "@": Opcodes.BINARY_MATRIX_MULTIPLY,
         "is": (Opcodes.IS_OP, 0),
         "!is": (Opcodes.IS_OP, 1),
         "in": (Opcodes.CONTAINS_OP, 0),
         "!in": (Opcodes.CONTAINS_OP, 1),
-        "<": (Opcodes.COMPARE_OP, 0),
-        "<=": (Opcodes.COMPARE_OP, 1),
-        "==": (Opcodes.COMPARE_OP, 2),
-        "!=": (Opcodes.COMPARE_OP, 3),
-        ">": (Opcodes.COMPARE_OP, 4),
-        ">=": (Opcodes.COMPARE_OP, 5),
+        "<": Opcodes.COMPARE_LT,
+        "<=": Opcodes.COMPARE_LE,
+        "==": Opcodes.COMPARE_EQ,
+        "!=": Opcodes.COMPARE_NEQ,
+        ">": Opcodes.COMPARE_GT,
+        ">=": Opcodes.COMPARE_GE,
         # todo: is there a better way?
-        "xor": (Opcodes.COMPARE_OP, 3),
-        "!xor": (Opcodes.COMPARE_OP, 2),
+        "xor": Opcodes.COMPARE_NEQ,
+        "!xor": Opcodes.COMPARE_EQ,
         ":=": lambda lhs, rhs, function, scope: rhs.emit_bytecodes(function, scope)
-        + [Instruction(function, -1, Opcodes.DUP_TOP)]
+        + [Instruction(Opcodes.DUP_TOP)]
         + lhs.emit_store_bytecodes(function, scope),
         "isinstance": lambda lhs, rhs, function, scope: [
-            Instruction(function, -1, Opcodes.LOAD_CONST, isinstance)
+            Instruction(Opcodes.LOAD_CONST, isinstance)
         ]
         + lhs.emit_bytecodes(function, scope)
         + rhs.emit_bytecodes(function, scope)
-        + [Instruction(function, -1, Opcodes.CALL_FUNCTION, arg=2)],
+        + [Instruction(Opcodes.CALL_FUNCTION, arg=2)],
         "issubclass": lambda lhs, rhs, function, scope: [
-            Instruction(function, -1, Opcodes.LOAD_CONST, issubclass)
+            Instruction(Opcodes.LOAD_CONST, issubclass)
         ]
         + lhs.emit_bytecodes(function, scope)
         + rhs.emit_bytecodes(function, scope)
-        + [Instruction(function, -1, Opcodes.CALL_FUNCTION, arg=2)],
+        + [Instruction(Opcodes.CALL_FUNCTION, arg=2)],
         "hasattr": lambda lhs, rhs, function, scope: [
-            Instruction(function, -1, Opcodes.LOAD_CONST, hasattr)
+            Instruction(Opcodes.LOAD_CONST, hasattr)
         ]
         + lhs.emit_bytecodes(function, scope)
         + rhs.emit_bytecodes(function, scope)
-        + [Instruction(function, -1, Opcodes.CALL_FUNCTION, arg=2)],
+        + [Instruction(Opcodes.CALL_FUNCTION, arg=2)],
         "getattr": lambda lhs, rhs, function, scope: [
-            Instruction(function, -1, Opcodes.LOAD_CONST, getattr)
+            Instruction(Opcodes.LOAD_CONST, getattr)
         ]
         + lhs.emit_bytecodes(function, scope)
         + rhs.emit_bytecodes(function, scope)
-        + [Instruction(function, -1, Opcodes.CALL_FUNCTION, arg=2)],
+        + [Instruction(Opcodes.CALL_FUNCTION, arg=2)],
     }
 
     SINGLE_OPS = {
         "-": Opcodes.UNARY_NEGATIVE,
         "+": Opcodes.UNARY_POSITIVE,
         "~": Opcodes.UNARY_INVERT,
         "not": Opcodes.UNARY_NOT,
```

### Comparing `bytecodemanipulation-0.3.1/bytecodemanipulation/data/v3_11/instructions/PopElementAssembly.py` & `bytecodemanipulation-0.3.3/bytecodemanipulation/data/v3_11/instructions/PopElementAssembly.py`

 * *Files 17% similar despite different names*

```diff
@@ -11,10 +11,10 @@
 
 @Parser.register
 class PopElementAssembly(AbstractPopElementAssembly):
     def emit_bytecodes(
         self, function: MutableFunction, scope: ParsingScope
     ) -> typing.List[Instruction]:
         return [
-            Instruction(function, -1, "POP_TOP", int(self.count.text))
+            Instruction("POP_TOP", int(self.count.text))
             for _ in range(int(self.count.text))
         ]
```

### Comparing `bytecodemanipulation-0.3.1/bytecodemanipulation/data/v3_11/instructions/RaiseAssembly.py` & `bytecodemanipulation-0.3.3/bytecodemanipulation/data/v3_11/instructions/RaiseAssembly.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,8 +13,8 @@
 @Parser.register
 class RaiseAssembly(AbstractRaiseAssembly):
     def emit_bytecodes(
         self, function: MutableFunction, scope: ParsingScope
     ) -> typing.List[Instruction]:
         return (
             [] if self.source is None else self.source.emit_bytecodes(function, scope)
-        ) + [Instruction(function, -1, Opcodes.RAISE_VARARGS, arg=1)]
+        ) + [Instruction(Opcodes.RAISE_VARARGS, arg=1)]
```

### Comparing `bytecodemanipulation-0.3.1/bytecodemanipulation/data/v3_11/instructions/ReturnAssembly.py` & `bytecodemanipulation-0.3.3/bytecodemanipulation/data/v3_11/instructions/ReturnAssembly.py`

 * *Files 18% similar despite different names*

```diff
@@ -12,8 +12,8 @@
 @Parser.register
 class ReturnAssembly(AbstractReturnAssembly):
     def emit_bytecodes(
         self, function: MutableFunction, scope: ParsingScope
     ) -> typing.List[Instruction]:
         expr_bytecode = self.expr.emit_bytecodes(function, scope) if self.expr else []
 
-        return expr_bytecode + [Instruction(function, -1, "RETURN_VALUE")]
+        return expr_bytecode + [Instruction("RETURN_VALUE")]
```

### Comparing `bytecodemanipulation-0.3.1/bytecodemanipulation/data/v3_11/instructions/StoreFastAssembly.py` & `bytecodemanipulation-0.3.3/bytecodemanipulation/data/v3_11/instructions/StoreFastAssembly.py`

 * *Files 15% similar despite different names*

```diff
@@ -17,8 +17,8 @@
         value = self.name_token.text
 
         if value.isdigit():
             value = int(value)
 
         return (
             [] if self.source is None else self.source.emit_bytecodes(function, scope)
-        ) + [Instruction(function, -1, "STORE_FAST", value)]
+        ) + [Instruction("STORE_FAST", value)]
```

### Comparing `bytecodemanipulation-0.3.1/bytecodemanipulation/data/v3_11/instructions/StoreGlobalAssembly.py` & `bytecodemanipulation-0.3.3/bytecodemanipulation/data/v3_11/instructions/StoreGlobalAssembly.py`

 * *Files 13% similar despite different names*

```diff
@@ -17,8 +17,8 @@
         value = self.name_token.text
 
         if value.isdigit():
             value = int(value)
 
         return (
             [] if self.source is None else self.source.emit_bytecodes(function, scope)
-        ) + [Instruction(function, -1, "STORE_GLOBAL", value)]
+        ) + [Instruction("STORE_GLOBAL", value)]
```

### Comparing `bytecodemanipulation-0.3.1/bytecodemanipulation/data/v3_11/instructions/YieldAssembly.py` & `bytecodemanipulation-0.3.3/bytecodemanipulation/data/v3_11/instructions/YieldAssembly.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,26 +18,26 @@
         bytecode = []
 
         if self.expr:
             bytecode += self.expr.emit_bytecodes(function, scope)
 
         if self.is_star:
             bytecode += [
-                Instruction(function, -1, Opcodes.GET_YIELD_FROM_ITER),
-                Instruction(function, -1, Opcodes.LOAD_CONST, None),
-                Instruction(function, -1, Opcodes.YIELD_FROM),
+                Instruction(Opcodes.GET_YIELD_FROM_ITER),
+                Instruction(Opcodes.LOAD_CONST, None),
+                Instruction(Opcodes.YIELD_FROM),
             ]
 
         else:
             bytecode += [
-                Instruction(function, -1, Opcodes.YIELD_VALUE),
+                Instruction(Opcodes.YIELD_VALUE),
             ]
 
         if self.target:
             bytecode += self.target.emit_store_bytecodes(function, scope)
 
         else:
-            bytecode += [Instruction(function, -1, Opcodes.POP_TOP)]
+            bytecode += [Instruction(Opcodes.POP_TOP)]
 
         # print(bytecode)
 
         return bytecode
```

### Comparing `bytecodemanipulation-0.3.1/bytecodemanipulation/data_loader.py` & `bytecodemanipulation-0.3.3/bytecodemanipulation/data_loader.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,14 +15,19 @@
 sys.path.append(os.path.dirname(local))
 
 
 INIT_ASSEMBLY = True
 
 
 def load_opcode_data():
+    if load_opcode_data.loaded:
+        return
+
+    load_opcode_data.loaded = True
+
     opcode_data: dict = json.load(open(folder + "/opcodes.json"))
 
     valid_opcode_names = [
         key
         for key, value in Opcodes.__dict__.items()
         if isinstance(value, int) and not key.startswith("__") and value != -1
     ]
@@ -40,14 +45,17 @@
     virtual_opcode = 256
     for key, value in Opcodes.__dict__.items():
         if not key.startswith("__") and value == -1:
             setattr(Opcodes, key, virtual_opcode)
             virtual_opcode += 1
 
 
+load_opcode_data.loaded = False
+
+
 def load_instruction_spec():
     spec_data = json.load(open(folder + "/instruction_spec.json"))
 
     for key, opcodes in spec_data.items():
         getattr(OpcodesM, key)[:] = map(OPNAME2CODE.__getitem__, opcodes)
```

### Comparing `bytecodemanipulation-0.3.1/bytecodemanipulation/opcodes/AbstractOpcodeTransformerStage.py` & `bytecodemanipulation-0.3.3/bytecodemanipulation/opcodes/AbstractOpcodeTransformerStage.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import sys
 from abc import ABC
 import typing
 
 from bytecodemanipulation.opcodes.Instruction import Instruction
 from bytecodemanipulation.opcodes.Opcodes import Opcodes
 from bytecodemanipulation.opcodes.CodeObjectBuilder import CodeObjectBuilder
 
@@ -13,52 +14,57 @@
     @classmethod
     def apply(cls, function: "MutableFunction", metadata: typing.Any) -> typing.Any:
         raise NotImplementedError
 
 
 class InstructionDecoder(AbstractOpcodeTransformerStage):
     @classmethod
-    def apply(cls, function: "MutableFunction", metadata: typing.Any) -> typing.Any:
+    def apply(cls, function: "MutableFunction", metadata: list) -> typing.Any:
         line = function.code_object.co_firstlineno
         lnotab = list(function.code_object.co_lnotab)
 
         instructions = []
 
         extra: int = 0
         for i in range(0, len(function.get_raw_code_unsafe()), 2):
             opcode, arg = function.get_raw_code_unsafe()[i: i + 2]
 
             if opcode == Opcodes.EXTENDED_ARG:
                 extra = extra * 256 + arg
-                instr = Instruction(function, i // 2, "NOP", _decode_next=False)
+                instr = Instruction(Opcodes.NOP)
+                instr.offset = i // 2
 
             else:
                 arg += extra * 256
                 extra = 0
 
                 if opcode in (Opcodes.FOR_ITER, Opcodes.SETUP_FINALLY):
                     arg += 1
 
-                instr = Instruction(function, i // 2, opcode, _decode_next=False)
+                instr = Instruction(opcode)
+                instr.offset = i // 2
 
                 if instr.has_local():
                     instr.arg_value = function.code_object.co_varnames[arg]
+                elif sys.version_info[1] >= 11 and opcode == Opcodes.LOAD_GLOBAL:
+                    instr.arg_value = function.code_object.co_names[arg >> 1]
                 elif instr.has_name():
                     instr.arg_value = function.code_object.co_names[arg]
                 elif instr.has_constant():
                     instr.arg_value = function.code_object.co_consts[arg]
                 elif instr.has_cell_variable():
+                    # todo: py-3.10 could need special handling here!
                     instr.arg_value = function.code_object.co_cellvars[arg]
                 else:
                     instr.arg = arg
 
             if lnotab:
                 lnotab[0] -= 1
 
-                if lnotab[0] == 0:
+                if lnotab[0] <= 0:
                     line_incr = lnotab[1]
                     del lnotab[:2]
 
                     line += line_incr
 
             instr.source_location = (line, None, None)
             instr.offset = i // 2
@@ -77,35 +83,39 @@
                 instr.arg = None
 
         for i, instr in enumerate(instructions[:-1]):
             if not instr.has_stop_flow() and not instr.has_unconditional_jump():
                 instr.next_instruction = instructions[i+1]
 
         function.instruction_entry_point = instructions[0]
+        metadata[:] = instructions
 
 
 class AbstractInstructionWalkerTransform(AbstractOpcodeTransformerStage):
     @classmethod
-    def apply(cls, function: "MutableFunction", metadata: typing.Any) -> typing.Any:
+    def apply(cls, function: "MutableFunction", metadata: typing.Any):
         visiting = {function.get_instruction_entry_point()} | set(function.exception_table.table.keys())
         visited = set()
 
         while visiting:
             instr = visiting.pop()
 
             if instr in visited or instr is None:
                 continue
 
             visited.add(instr)
 
-            cls.visit(
-                function,
-                metadata,
-                instr,
-            )
+            try:
+                cls.visit(
+                    function,
+                    metadata,
+                    instr,
+                )
+            except StopIteration:
+                return
 
             if not instr.has_stop_flow() and not instr.has_unconditional_jump():
                 visiting.add(instr.next_instruction)
 
             if instr.has_jump():
                 visiting.add(instr.arg_value)
 
@@ -180,17 +190,14 @@
             while instruction not in visited:
                 if not isinstance(instruction, Instruction):
                     print(f"Invalid task instruction: {instruction}")
                     break
 
                 # If it branches off, it needs to be visited later on
                 if instruction.has_jump():
-                    if instruction.arg_value is None:
-                        instruction.update_owner(function, instruction.offset)
-
                     assert instruction.arg_value is not None, instruction
 
                     pending_instructions.add(instruction.arg_value)
 
                 instructions.append(instruction)
                 visited.add(instruction)
 
@@ -198,17 +205,14 @@
                     instruction.has_stop_flow()
                     or instruction in breaks_flow
                     or instruction.opcode in breaks_flow
                     or instruction.has_unconditional_jump()
                 ):
                     break
 
-                if instruction.next_instruction is None:
-                    instruction.update_owner(function, instruction.offset)
-
                 # The next instruction MUST be set if it does NOT end the control flow
                 if instruction.next_instruction is None:
                     print("---- start dump")
                     for instr in instructions:
                         print(instr)
                     print("---- end dump")
                     raise RuntimeError(f"next instruction is None: {instruction}")
@@ -239,31 +243,27 @@
             if instruction.has_stop_flow() or instruction.has_unconditional_jump():
                 continue
 
             # FOR_ITER can only jump FORWARD, so insert a new jump absolute to jump there
             # TODO: insert the JUMP somewhere else than here!
             if instruction.opcode == Opcodes.FOR_ITER:
                 jump = Instruction(
-                    function,
-                    -1,
-                    "JUMP_ABSOLUTE",
+                    Opcodes.JUMP_ABSOLUTE,
                     instruction.next_instruction,
                 )
                 jump.change_arg_value(instruction.arg_value)
                 instruction.change_arg_value(jump)
                 builder.temporary_instructions.append(jump)
 
             if (
                 instruction.next_instruction is not None
                 and instruction.offset + 1 != instruction.next_instruction.offset
             ):
                 jump = Instruction(
-                    function,
-                    -1,
-                    "JUMP_ABSOLUTE",
+                    Opcodes.JUMP_ABSOLUTE,
                     instruction.next_instruction,
                 )
                 jump.next_instruction = instruction
                 instruction.next_instruction = jump
                 builder.temporary_instructions.insert(builder.temporary_instructions.index(instruction) + 1, jump)
 
         for i, instruction in enumerate(builder.temporary_instructions):
@@ -272,16 +272,14 @@
     @classmethod
     def update_jump_args(cls, function: "MutableFunction", builder: CodeObjectBuilder):
         # Update the raw arg for jumps
         for i, instruction in enumerate(builder.temporary_instructions):
             if instruction.next_instruction is None:
                 continue
 
-            instruction.update_owner(function, i)
-
             if instruction.has_jump_absolute():
                 instruction.change_arg(instruction.arg_value.offset)
 
             elif instruction.opcode in (Opcodes.FOR_ITER, Opcodes.SETUP_FINALLY):
                 instruction.change_arg(instruction.arg_value.offset - instruction.offset - 2)
 
             elif instruction.has_jump_forward():
@@ -303,14 +301,17 @@
         function._raw_code.clear()
         for i, instruction in enumerate(builder.temporary_instructions):
             if instruction.opcode > 255:
                 raise ValueError(f"invalid instruction at result level: {instruction}")
 
             arg = instruction.get_arg()
 
+            if instruction.opcode == Opcodes.SETUP_FINALLY:
+                arg += 1
+
             if arg > 255:
                 extend = arg // 256
                 arg %= 256
 
                 offset = 1
                 while extend > 0:
                     iarg = extend % 256
```

### Comparing `bytecodemanipulation-0.3.1/bytecodemanipulation/opcodes/CodeObjectBuilder.py` & `bytecodemanipulation-0.3.3/bytecodemanipulation/opcodes/CodeObjectBuilder.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,14 +13,17 @@
 
         self.shared_variable_names = function.argument_names.copy()
         self.constants = []
         self.shared_names = []
         self.free_variables = []
         self.cell_variables = []
 
+        self.first_line_number = 0
+        self.line_info_table = bytes()
+
     def prepare_previous_instructions(self):
         for instruction in self.temporary_instructions:
             if instruction.previous_instructions:
                 instruction.previous_instructions.clear()
 
         for instruction in self.temporary_instructions:
             if instruction.has_stop_flow() or instruction.has_unconditional_jump():
```

### Comparing `bytecodemanipulation-0.3.1/bytecodemanipulation/opcodes/ExceptionTable.py` & `bytecodemanipulation-0.3.3/bytecodemanipulation/opcodes/ExceptionTable.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.3.1/bytecodemanipulation/opcodes/Instruction.py` & `bytecodemanipulation-0.3.3/bytecodemanipulation/opcodes/Instruction.py`

 * *Files 8% similar despite different names*

```diff
@@ -41,65 +41,57 @@
         "_next_instruction",
         "previous_instructions",
         "source_location",
         "_max_stack_size_at",
     )
 
     @classmethod
-    def create(cls, *args, **kwargs):
-        return cls(None, -1, *args, **kwargs)
-
-    @classmethod
     def create_with_token(
         cls,
         token: AbstractToken,
-        function: typing.Optional["MutableFunction"],
-        offset: int | None,
         opcode_or_name: int | str,
         arg_value: object = None,
         arg: int = None,
-        _decode_next=True,
     ) -> "Instruction":
         raise NotImplementedError("not bound!")
 
+    @classmethod
+    def create_with_same_info(cls, instruction: "Instruction", opname_or_code: int | str, arg_value: object = None, arg: int = None) -> "Instruction":
+        instr = cls(opname_or_code, arg_value, arg)
+        instr.offset = instruction.offset
+        instr.source_location = instruction.source_location
+
+        return instr
+
     def __init__(
         self,
-        function: typing.Optional["MutableFunction"],
-        offset: int | None,
         opcode_or_name: int | str,
         arg_value: object = None,
         arg: int = None,
-        _decode_next=True,
         pos_info=None,
     ):
-        self.function = function
-        self.offset = offset
+        self.offset = None
         self.opcode, self.opname = self._pair_instruction(opcode_or_name)
         self.arg_value = arg_value
         self.arg = arg
         self.source_location = pos_info
         self._max_stack_size_at = 0
 
         # Reference to the next instruction
         self._next_instruction: typing.Optional[Instruction] = None
 
         self.previous_instructions: typing.List["Instruction"] | None = None
 
-    def copy(self, owner: "MutableFunction" = None) -> "Instruction":
+    def copy(self) -> "Instruction":
         instance = type(self)(
-            self.function,
-            self.offset,
             self.opcode,
             self.arg_value,
             self.arg,
         )
 
-        if owner:
-            instance.update_owner(owner, -1, force_change_arg_index=True)
-
         return instance
 
     def copy_deep(self, copied: dict = None) -> "Instruction":
         copied = copied or {}
 
         c = self.copy()
         copied[self] = c
@@ -188,25 +180,17 @@
             self.previous_instructions.remove(instruction)
 
     def get_previous_instructions(self) -> typing.List["Instruction"]:
         if self.has_stop_flow():
             return []
 
         if self.previous_instructions is None:
-            if self.function is None:
-                raise ValueError(
-                    f"Instruction {self} is not bound to a MutableFunction object, making retrieving the previous instruction list impossible!!"
-                )
-
-            self.function.prepare_previous_instructions()
-
-            if self.previous_instructions is None:
-                raise RuntimeError(
-                    f"Could not find previous instructions for {self}. This should NOT happen, as we asked the method which MUST yield results. (See MutableFunction.prepare_previous_instructions())"
-                )
+            raise RuntimeError(
+                f"Could not find previous instructions for {self}. This should NOT happen, as we asked the method which MUST yield results. (See MutableFunction.prepare_previous_instructions())"
+            )
 
         return self.previous_instructions
 
     def set_next_instruction(self, instruction: typing.Optional["Instruction"]):
         if self._next_instruction is not None:
             self._next_instruction.remove_previous_instruction(self)
 
@@ -220,25 +204,24 @@
 
     def get_next_instruction(self) -> typing.Optional["Instruction"]:
         return self._next_instruction
 
     next_instruction = property(get_next_instruction, set_next_instruction)
 
     def __repr__(self):
-        assert self.function is None or isinstance(self.function.function_name, str)
-        assert isinstance(self.offset, int)
+        assert isinstance(self.offset, int) or self.offset is None
         assert isinstance(self.opcode, int)
         assert isinstance(self.arg, int) or self.arg is None
         if id(self) == id(self.arg_value):
             return self.repr_safe() + "@self_arg_value"
 
-        return f"Instruction(function={self.function.function_name if self.function else '{Not Bound}'}, position={self.offset}, opcode={self.opcode}, opname={self.opname}, arg={self.arg}, arg_value={self.arg_value.repr_safe() if self.arg_value is not None and isinstance(self.arg_value, Instruction) else self.arg_value}, has_next={self.next_instruction is not None})"
+        return f"Instruction(position={self.offset}, opcode={self.opcode}, opname={self.opname}, arg={self.arg}, arg_value={self.arg_value.repr_safe() if self.arg_value is not None and isinstance(self.arg_value, Instruction) else self.arg_value}, has_next={self.next_instruction is not None})"
 
     def repr_safe(self):
-        return f"Instruction(function={self.function.function_name if self.function else '{Not Bound}'}, position={self.offset}, opcode={self.opcode}, opname={self.opname}, arg={self.arg}, arg_value=..., has_next={self.next_instruction is not None})"
+        return f"Instruction(position={self.offset}, opcode={self.opcode}, opname={self.opname}, arg={self.arg}, arg_value={'... (' + str(type(self.arg_value)) + ')' if self.arg_value is not None else None}, has_next={self.next_instruction is not None})"
 
     def __eq__(self, other):
         if not isinstance(other, Instruction):
             return False
 
         return (
             self.opcode == other.opcode
@@ -252,14 +235,17 @@
                 if not isinstance(self.arg_value, Instruction)
                 else (id(self.arg_value) == id(other.arg_value))
                 if self.arg_value is not None and other.arg_value is not None
                 else True
             )
         )
 
+    def __hash__(self):
+        return id(self)
+
     def lossy_eq(self, other: "Instruction") -> bool:
         if not isinstance(other, Instruction):
             return False
 
         return self.opcode == other.opcode and (
             (
                 (self.arg_value == other.arg_value)
@@ -267,28 +253,25 @@
                 else self.arg_value.lossy_eq(other.arg_value)
             )
             if (self.arg_value is not None and other.arg_value is not None)
             or self.opcode == Opcodes.LOAD_CONST
             else True
         )
 
-    def __hash__(self):
-        return id(self)
-
     def get_arg(self):
         return 0 if self.arg is None else self.arg
 
     def change_opcode(self, opcode: int | str, arg_value=None):
         self.opcode, self.opname = self._pair_instruction(opcode)
 
         if self.opcode < dis.HAVE_ARGUMENT:
-            self.arg = 0
+            self.arg = None
             self.arg_value = None
 
-        if arg_value:
+        if arg_value is not None or self.opcode == Opcodes.LOAD_CONST:
             self.arg_value = arg_value
 
         return self
 
     # todo: remove
     def change_arg_value(self, value: object):
         self.arg_value = value
@@ -326,57 +309,49 @@
 
     def has_unconditional_jump(self):
         return self.opcode in UNCONDITIONAL_JUMPS
 
     def has_stop_flow(self):
         return self.opcode in END_CONTROL_FLOW
 
-    # todo: remove args not required
-    def update_owner(
-        self,
-        function: "MutableFunction",
-        offset: int,
-        update_following=True,
-        force_change_arg_index=False,
-    ):
-        self.function = function
-        self.offset = offset
-        return self
-
     def optimise_tree(self, visited: typing.Set["Instruction"] = None) -> "Instruction":
         """
         Optimises the instruction tree, removing NOP's and inlining unconditional jumps
         WARNING: this WILL invalidate the linearity of any instruction list, you MUST use assemble_instructions_from_tree()
         for inserting it back into the Function.
 
         Requires next_instruction's to be set, meaning it must be owned at some point by a function
         """
 
         if self.has_unconditional_jump():
-            return self.arg_value.optimise_tree(visited)
+            return typing.cast(Instruction, self.arg_value).optimise_tree(visited)
 
         if visited is None:
             visited = set()
 
         if self in visited:
             return self
 
         visited.add(self)
 
-        if self.opcode == Opcodes.NOP and self.next_instruction is not None:
+        if self.opcode in (Opcodes.NOP, Opcodes.CACHE, Opcodes.PRECALL):
+            if self.next_instruction is None:
+                print("WARN: no next_instruction:", self)
+                return self
+
             return self.next_instruction.optimise_tree(visited)
 
         while self.next_instruction is not None:
             assert isinstance(self.next_instruction, Instruction)
 
-            if self.next_instruction.opname == "NOP":
+            if self.next_instruction.opcode in (Opcodes.NOP, Opcodes.CACHE, Opcodes.PRECALL):
                 self.next_instruction = self.next_instruction.next_instruction
                 continue
 
-            if self.next_instruction.opname in ("JUMP_ABSOLUTE", "JUMP_FORWARD"):
+            if self.next_instruction.has_unconditional_jump():
                 self.next_instruction = self.next_instruction.arg_value
                 continue
 
             break
 
         if (
             self.next_instruction is not None
@@ -386,15 +361,15 @@
             self.next_instruction = self.next_instruction.optimise_tree(visited)
 
         if (
             self.has_jump_absolute()
             or self.has_jump_forward()
             or self.has_jump_backward()
         ) and self.arg_value is not None:
-            assert isinstance(self.arg_value, Instruction)
+            assert isinstance(self.arg_value, Instruction), self.repr_safe()
             self.change_arg_value(self.arg_value.optimise_tree(visited))
 
         return self
 
     def trace_variable_set(
         self, name: str, visited: typing.Set[str] = None
     ) -> typing.Iterator["Instruction"]:
@@ -416,15 +391,15 @@
 
         for prev in self.previous_instructions:
             yield from prev.trace_variable_set(name, visited)
 
     def trace_stack_position(
         self, stack_position: int
     ) -> typing.Iterator["Instruction"]:
-        for instr in self.get_priorities_previous():
+        for instr in self.previous_instructions: # self.get_priorities_previous():
             yield from instr._trace_stack_position(stack_position, set(), self)
 
     def get_priorities_previous(self) -> typing.List["Instruction"]:
         if not self.previous_instructions:
             return []
 
         real_previous = [
@@ -511,15 +486,15 @@
             return
 
         stack_position -= pushed
         stack_position += popped
 
         yielded.add(self)
 
-        for instr in self.get_priorities_previous():
+        for instr in self.previous_instructions:  # self.get_priorities_previous():
             try:
                 yield from instr._trace_stack_position(stack_position, yielded, self)
             except:
                 # print(self, instr)
                 raise
 
         if additional_pos:
@@ -590,17 +565,17 @@
             Opcodes.POP_EXCEPT,
             Opcodes.SETUP_FINALLY,
             Opcodes.GEN_START,
             Opcodes.JUMP_ABSOLUTE,
             Opcodes.BYTECODE_LABEL,
             Opcodes.JUMP_FORWARD,
             Opcodes.RERAISE,
-            # Opcodes.CACHE,
-            # Opcodes.PRECALL,
-            # Opcodes.RESUME,
+            Opcodes.CACHE,
+            Opcodes.PRECALL,
+            Opcodes.RESUME,
         ):
             return 0, 0, None
 
         if self.opcode == Opcodes.DUP_TOP:
             return 2, 1, None
 
         if self.opcode == Opcodes.GET_ITER:
@@ -638,32 +613,40 @@
 
         if self.opcode in (Opcodes.FORMAT_VALUE,):
             return 1, (2 if (self.arg & 0x04) == 0x04 else 1), None
 
         if self.opcode in (
             Opcodes.CALL_FUNCTION,
             Opcodes.CALL_METHOD,
-            Opcodes.CALL_FUNCTION_KW,
-            # Opcodes.CALL,
+            Opcodes.CALL,
         ):
             return 1, self.arg + 1, None
 
+        if self.opcode == Opcodes.CALL_FUNCTION_KW:
+            return 1, self.arg + 2, None
+
         if self.opcode in (Opcodes.CALL_FUNCTION_EX,):
             count = 2
 
             if self.arg & 0x01:
                 count += 1
 
             return 1, count, None
 
         if self.opcode == Opcodes.BUILD_MAP:
             return 1, self.arg * 2, None
 
         if self.opcode in (
             Opcodes.COMPARE_OP,
+            Opcodes.COMPARE_LT,
+            Opcodes.COMPARE_LE,
+            Opcodes.COMPARE_EQ,
+            Opcodes.COMPARE_NEQ,
+            Opcodes.COMPARE_GT,
+            Opcodes.COMPARE_GE,
             Opcodes.IS_OP,
             Opcodes.BINARY_SUBSCR,
             Opcodes.CONTAINS_OP,
             Opcodes.LIST_EXTEND,
             Opcodes.LIST_APPEND,
             Opcodes.SET_ADD,
             Opcodes.SET_UPDATE,
@@ -765,7 +748,62 @@
         instructions[0].next_instruction = self.next_instruction
         self.next_instruction = instructions[0]
 
         if len(instructions) > 1:
             instructions[0].insert_after(instructions[1:])
 
         return self
+
+    def insert_after_arg(self, *instructions: "Instruction" | typing.List["Instruction"]):
+        if not self.has_jump():
+            raise ValueError("expected <jump>")
+
+        if not instructions:
+            return self
+
+        if isinstance(instructions[0], (list, tuple)):
+            if len(instructions) > 1:
+                raise ValueError
+
+            instructions = instructions[0]
+
+        if len(instructions) == 0:
+            return self
+
+        instructions[-1].next_instruction = self.arg_value
+        self.arg_value = instructions[0]
+
+        self.arg_value.insert_after(instructions[1:])
+        return self
+
+    def insert_before(self, *instructions: "Instruction" | typing.List["Instruction"]) -> "Instruction":
+        if not instructions:
+            return self
+
+        if isinstance(instructions[0], (list, tuple)):
+            if len(instructions) > 1:
+                raise ValueError
+
+            instructions = instructions[0]
+
+        if len(instructions) == 0:
+            return self
+
+        new_self = self.copy()
+        self.change_opcode(Opcodes.NOP)
+
+        self.insert_after(new_self)
+        self.insert_after(instructions)
+        return new_self
+
+    def get_following_instructions(self) -> typing.Iterable["Instruction"]:
+        if self.has_unconditional_jump():
+            yield self.arg_value
+            return
+
+        if self.has_stop_flow():
+            return
+
+        yield self.next_instruction
+
+        if self.has_jump():
+            yield self.arg_value
```

### Comparing `bytecodemanipulation-0.3.1/bytecodemanipulation/opcodes/Opcodes.py` & `bytecodemanipulation-0.3.3/bytecodemanipulation/opcodes/Opcodes.py`

 * *Files 7% similar despite different names*

```diff
@@ -148,44 +148,51 @@
     CALL_METHOD = 161
     LIST_EXTEND = 162
     SET_UPDATE = 163
     DICT_MERGE = 164
     DICT_UPDATE = 165
 
     # Since python 3.11
-    if sys.version_info.minor >= 11 or typing.TYPE_CHECKING:
-        CACHE = 166
-        PUSH_NULL = 167
-        PUSH_EXC_INFO = 168
-        CHECK_EXC_MATCH = 169
-        CHECK_EG_MATCH = 170
-        BEFORE_WITH = 171
-        RETURN_GENERATOR = 172
-        ASYNC_GEN_WRAP = 173
-        PREP_RERAISE_STAR = 174
-        SWAP = 175
-        POP_JUMP_FORWARD_IF_FALSE = 176
-        POP_JUMP_FORWARD_IF_TRUE = 177
-        COPY = 178
-        BINARY_OP = 179
-        SEND = 180
-        POP_JUMP_FORWARD_IF_NOT_NONE = 181
-        POP_JUMP_FORWARD_IF_NONE = 182
-        JUMP_BACKWARD_NO_INTERRUPT = 183
-        MAKE_CELL = 184
-        JUMP_BACKWARD = 185
-        COPY_FREE_VARS = 186
-        RESUME = 187
-        PRECALL = 188
-        CALL = 189
-        KW_NAMES = 190
-        POP_JUMP_BACKWARD_IF_NOT_NONE = 191
-        POP_JUMP_BACKWARD_IF_NONE = 192
-        POP_JUMP_BACKWARD_IF_FALSE = 193
-        POP_JUMP_BACKWARD_IF_TRUE = 194
+    CACHE = 166
+    PUSH_NULL = 167
+    PUSH_EXC_INFO = 168
+    CHECK_EXC_MATCH = 169
+    CHECK_EG_MATCH = 170
+    BEFORE_WITH = 171
+    RETURN_GENERATOR = 172
+    ASYNC_GEN_WRAP = 173
+    PREP_RERAISE_STAR = 174
+    SWAP = 175
+    POP_JUMP_FORWARD_IF_FALSE = 176
+    POP_JUMP_FORWARD_IF_TRUE = 177
+    COPY = 178
+    BINARY_OP = 179
+    SEND = 180
+    POP_JUMP_FORWARD_IF_NOT_NONE = 181
+    POP_JUMP_FORWARD_IF_NONE = 182
+    JUMP_BACKWARD_NO_INTERRUPT = 183
+    MAKE_CELL = 184
+    JUMP_BACKWARD = 185
+    COPY_FREE_VARS = 186
+    RESUME = 187
+    PRECALL = 188
+    CALL = 189
+    KW_NAMES = 190
+    POP_JUMP_BACKWARD_IF_NOT_NONE = 191
+    POP_JUMP_BACKWARD_IF_NONE = 192
+    POP_JUMP_BACKWARD_IF_FALSE = 193
+    POP_JUMP_BACKWARD_IF_TRUE = 194
+
+    # virtual opcodes
+    COMPARE_LT = -1
+    COMPARE_LE = -1
+    COMPARE_EQ = -1
+    COMPARE_NEQ = -1
+    COMPARE_GT = -1
+    COMPARE_GE = -1
 
     INTERMEDIATE_INNER_RETURN = -1
     INTERMEDIATE_OUTER_RETURN = -1
     INTERMEDIATE_LOAD_FAST = -1
     BYTECODE_LABEL = -1
     MACRO_PARAMETER_EXPANSION = -1
     STATIC_ATTRIBUTE_ACCESS = -1
```

### Comparing `bytecodemanipulation-0.3.1/bytecodemanipulation/optimiser_util.py` & `bytecodemanipulation-0.3.3/bytecodemanipulation/optimiser_util.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,20 +42,20 @@
     Opcodes.BINARY_RSHIFT: "__rshift__",
     Opcodes.INPLACE_RSHIFT: "__irshift__",
     Opcodes.BINARY_AND: "__and__",
     Opcodes.BINARY_XOR: "__xor__",
     Opcodes.BINARY_OR: "__or__",
     (Opcodes.IS_OP, 0): lambda a, b: a is b,
     (Opcodes.IS_OP, 1): lambda a, b: a is not b,
-    (Opcodes.COMPARE_OP, 0): lambda a, b: a < b,
-    (Opcodes.COMPARE_OP, 1): lambda a, b: a <= b,
-    (Opcodes.COMPARE_OP, 2): lambda a, b: a == b,
-    (Opcodes.COMPARE_OP, 3): lambda a, b: a != b,
-    (Opcodes.COMPARE_OP, 4): lambda a, b: a > b,
-    (Opcodes.COMPARE_OP, 5): lambda a, b: a >= b,
+    Opcodes.COMPARE_LT: lambda a, b: a < b,
+    Opcodes.COMPARE_LE: lambda a, b: a <= b,
+    Opcodes.COMPARE_EQ: lambda a, b: a == b,
+    Opcodes.COMPARE_NEQ: lambda a, b: a != b,
+    Opcodes.COMPARE_GT: lambda a, b: a > b,
+    Opcodes.COMPARE_GE: lambda a, b: a >= b,
 }
 
 
 def inline_const_value_pop_pairs(mutable: MutableFunction, builder) -> bool:
     dirty = False
 
     def visit(instruction: Instruction):
@@ -98,15 +98,15 @@
                         func_resolve.change_opcode(Opcodes.POP_TOP)
                         pops -= 1
 
                         if not pops:
                             return
 
                         for _ in range(pops):
-                            nop = Instruction.create(Opcodes.NOP)
+                            nop = Instruction.create_with_same_info(func_resolve, Opcodes.NOP)
                             nop.next_instruction = func_resolve.next_instruction
                             func_resolve.next_instruction = nop
 
                         return True
 
             if source.opcode in (
                 Opcodes.BUILD_LIST,
@@ -130,15 +130,15 @@
                 if count == 1:
                     dirty = True
                     return
 
                 count -= 1
 
                 for _ in range(count):
-                    nop = Instruction.create(Opcodes.NOP)
+                    nop = Instruction.create_with_same_info(source, Opcodes.NOP)
                     nop.next_instruction = source.next_instruction
                     source.next_instruction = nop
 
     mutable.walk_instructions(visit)
 
     return dirty
 
@@ -205,14 +205,15 @@
     return dirty
 
 
 def inline_constant_binary_ops(mutable: MutableFunction, builder) -> bool:
     dirty = False
 
     def visit(instruction: Instruction):
+        print(instruction)
         nonlocal dirty
 
         if (
             instruction.opcode in OPCODE_TO_ATTR_SINGLE
             or (instruction.opcode, instruction.arg) in OPCODE_TO_ATTR_SINGLE
         ):
             method = OPCODE_TO_ATTR_SINGLE[
```

### Comparing `bytecodemanipulation-0.3.1/bytecodemanipulation/util.py` & `bytecodemanipulation-0.3.3/bytecodemanipulation/util.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.3.1/bytecodemanipulation.egg-info/PKG-INFO` & `bytecodemanipulation-0.3.3/bytecodemanipulation.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bytecodemanipulation
-Version: 0.3.1
+Version: 0.3.3
 Summary: High level python bytecode manipulation
 Home-page: https://github.com/uuk0/PyBytecodeManipulator
 Author: uuk
 Author-email: uuk1301@gmail.com
 Project-URL: Bug Tracker, https://github.com/uuk0/PyBytecodeManipulator/issues
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -160,8 +160,9 @@
 # TODO's
 
 - abstract opcode affect away into a .json file describing all opcodes
 - create a json file for defining certain bytecode sequences
 - write more library-specific optimisations
 - write generating bytecode system for emulator, constructing a function pointing to the
   .json file for exception printing, and optimizing wherever possible
+- add optimisation: JUMP on condition for some operators (e.g. NOT)
```

### Comparing `bytecodemanipulation-0.3.1/bytecodemanipulation.egg-info/SOURCES.txt` & `bytecodemanipulation-0.3.3/bytecodemanipulation.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -78,14 +78,16 @@
 bytecodemanipulation/data/shared/instructions/ReturnAssembly.py
 bytecodemanipulation/data/shared/instructions/StoreAssembly.py
 bytecodemanipulation/data/shared/instructions/StoreFastAssembly.py
 bytecodemanipulation/data/shared/instructions/StoreGlobalAssembly.py
 bytecodemanipulation/data/shared/instructions/WhileAssembly.py
 bytecodemanipulation/data/shared/instructions/YieldAssembly.py
 bytecodemanipulation/data/shared/instructions/__init__.py
+bytecodemanipulation/data/v3_10/ExceptionInstructionCodec.py
+bytecodemanipulation/data/v3_10/LocationInformationHandler.py
 bytecodemanipulation/data/v3_10/__init__.py
 bytecodemanipulation/data/v3_10/assembly_instructions.py
 bytecodemanipulation/data/v3_10/specialize.py
 bytecodemanipulation/data/v3_10/instructions/AssertAssembly.py
 bytecodemanipulation/data/v3_10/instructions/CallAssembly.py
 bytecodemanipulation/data/v3_10/instructions/ClassDefinitionAssembly.py
 bytecodemanipulation/data/v3_10/instructions/ForEachAssembly.py
@@ -121,18 +123,21 @@
 bytecodemanipulation/data/v3_11/instructions/RaiseAssembly.py
 bytecodemanipulation/data/v3_11/instructions/ReturnAssembly.py
 bytecodemanipulation/data/v3_11/instructions/StoreFastAssembly.py
 bytecodemanipulation/data/v3_11/instructions/StoreGlobalAssembly.py
 bytecodemanipulation/data/v3_11/instructions/WhileAssembly.py
 bytecodemanipulation/data/v3_11/instructions/YieldAssembly.py
 bytecodemanipulation/data/v3_11/instructions/__init__.py
+bytecodemanipulation/data/v3_12/__init__.py
 bytecodemanipulation/opcodes/AbstractOpcodeTransformerStage.py
+bytecodemanipulation/opcodes/CacheEntryCreation.py
 bytecodemanipulation/opcodes/CodeObjectBuilder.py
 bytecodemanipulation/opcodes/ExceptionTable.py
 bytecodemanipulation/opcodes/Instruction.py
+bytecodemanipulation/opcodes/OpcodeReplacer.py
 bytecodemanipulation/opcodes/Opcodes.py
 bytecodemanipulation/opcodes/__init__.py
 tests/test_Assembly.py
 tests/test_InlineSystem.py
 tests/test_Mixin.py
 tests/test_MutableFunction.py
 tests/test_Operators.py
```

### Comparing `bytecodemanipulation-0.3.1/setup.py` & `bytecodemanipulation-0.3.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 
 setuptools.setup(
     name="bytecodemanipulation",
-    version="0.3.1",
+    version="0.3.3",
     author="uuk",
     author_email="uuk1301@gmail.com",
     description="High level python bytecode manipulation",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/uuk0/PyBytecodeManipulator",
     project_urls={
```

### Comparing `bytecodemanipulation-0.3.1/tests/test_Assembly.py` & `bytecodemanipulation-0.3.3/tests/test_Assembly.py`

 * *Files 8% similar despite different names*

```diff
@@ -56,14 +56,16 @@
 from bytecodemanipulation.assembler.target import (
     assembly,
     label,
     jump as asm_jump,
     make_macro,
 )
 from bytecodemanipulation.assembler.Emitter import apply_inline_assemblies
+from bytecodemanipulation.MutableFunctionHelpers import outer_return
+from bytecodemanipulation.MutableFunctionHelpers import capture_local
 
 try:
     from code_parser.parsers.common import IdentifierExpression
     from code_parser.lexers.common import IdentifierToken
 except ImportError:
     from bytecodemanipulation.assembler.util.parser import IdentifierExpression
     from bytecodemanipulation.assembler.util.tokenizer import IdentifierToken
@@ -146,16 +148,16 @@
         expr = Parser(
             "STORE_GLOBAL test\nSTORE_GLOBAL @test\nSTORE_GLOBAL test (@test)\nSTORE_GLOBAL test ($test)\nSTORE_GLOBAL test (%)"
         ).parse()
 
         self.assertEqualList(
             CompoundExpression(
                 [
-                    AbstractStoreGlobalAssembly.IMPLEMENTATION(IdentifierToken("test")),
-                    AbstractStoreGlobalAssembly.IMPLEMENTATION(IdentifierToken("test")),
+                    AbstractStoreGlobalAssembly.IMPLEMENTATION("test"),
+                    AbstractStoreGlobalAssembly.IMPLEMENTATION("test"),
                     AbstractStoreGlobalAssembly.IMPLEMENTATION(
                         "test",
                         GlobalAccessExpression("test"),
                     ),
                     AbstractStoreGlobalAssembly.IMPLEMENTATION(
                         "test",
                         LocalAccessExpression("test"),
@@ -719,23 +721,23 @@
                     ),
                     AbstractFunctionDefinitionAssembly.IMPLEMENTATION(
                         "test", ["test", "test2"], [], CompoundExpression([])
                     ),
                     AbstractFunctionDefinitionAssembly.IMPLEMENTATION(
                         "test",
                         ["test"],
-                        [AbstractCallAssembly.Arg(IdentifierToken("a"))],
+                        [AbstractCallAssembly.Arg("a")],
                         CompoundExpression([]),
                     ),
                     AbstractFunctionDefinitionAssembly.IMPLEMENTATION(
                         "test",
                         ["test"],
                         [
-                            AbstractCallAssembly.Arg(IdentifierToken("a")),
-                            AbstractCallAssembly.Arg(IdentifierToken("b")),
+                            AbstractCallAssembly.Arg("a"),
+                            AbstractCallAssembly.Arg("b"),
                         ],
                         CompoundExpression([]),
                     ),
                     AbstractFunctionDefinitionAssembly.IMPLEMENTATION(
                         "test",
                         ["test"],
                         [AbstractCallAssembly.KwArg("c", GlobalAccessExpression("d"))],
@@ -909,22 +911,24 @@
 
         def target(x):
             assembly(
                 """
 CALL PARTIAL @print ("Hello World!") -> $x
 """
             )
+            return x
 
         mutable = MutableFunction(target)
         apply_inline_assemblies(mutable)
         mutable.reassign_to_function()
 
         @cache_global_name("functools")
         def compare():
             x = functools.partial(print, "Hello World!")
+            return x
 
         compare_optimized_results(self, target, compare, opt_ideal=2)
 
         _OptimisationContainer.get_for_target(functools).is_static = False
 
     def test_call_assembly(self):
         def target(x):
@@ -974,36 +978,65 @@
 
         code = "import tests.test\nself.assertEqual(10, tests.test.test)"
         exec(code, {"self": self})
 
         bytecodemanipulation.assembler.hook.unhook()
 
     def test_dynamic_attribute_access(self):
+        @apply_operations
         def target(t):
             assembly(
                 """
-RETURN $t.("test_dynamic_attribute_access")
+RETURN $t.("attr")
+"""
+            )
+
+        class H:
+            attr = {}
+
+        x = H()
+
+        self.assertEqual(target(x), x.attr)
+
+    def test_static_attribute_access(self):
+        class H:
+            attr = {}
+
+        global x
+        x = H()
+
+        def target():
+            assembly(
+                """
+RETURN @!x.!attr
 """
             )
 
         mutable = MutableFunction(target)
         apply_inline_assemblies(mutable)
         mutable.reassign_to_function()
 
-        self.assertEqual(target(self), self.test_dynamic_attribute_access)
+        dis.dis(target)
+
+        value = x.attr
+        x.attr = None
+        self.assertEqual(target(), value)
+
+        x = None
+        self.assertEqual(target(), value)
 
 
 class TestMacro(TestCase):
     def test_basic(self):
         def target():
             assembly(
                 """
     LOAD 1 -> $x
     MACRO test_basic {
-        LOAD 0 -> $x
+        LOAD 0 -> $:x
     }
     
     CALL MACRO test_basic()
     RETURN $x
     """
             )
             return -1
@@ -1015,15 +1048,15 @@
         self.assertEqual(target(), 0)
 
     def test_macro_local_access(self):
         def target():
             assembly(
                 """
         MACRO test_macro_local_access {
-            LOAD 1 -> $local
+            LOAD 1 -> $:local
         }
 
         LOAD 0 -> $local
         CALL MACRO test_macro_local_access()
         RETURN $local
         """
             )
@@ -1036,15 +1069,15 @@
         self.assertEqual(target(), 1)
 
     def test_macro_parameter_resolver(self):
         def target():
             assembly(
                 """
         MACRO test_macro_parameter_resolver (!param) {
-            LOAD &param -> $local
+            LOAD &param -> $:local
             LOAD 0 -> &param
         }
 
         LOAD 0 -> $local
         CALL MACRO test_macro_parameter_resolver(1)
         RETURN $local
         """
@@ -1054,33 +1087,32 @@
         mutable = MutableFunction(target)
         apply_inline_assemblies(mutable)
         mutable.reassign_to_function()
 
         self.assertEqual(target(), 1)
 
     def test_macro_parameter_duplicated_access_static(self):
+        @apply_operations
         def target():
             assembly(
                 """
         MACRO test_macro_parameter_duplicated_access_static (!param) {
-            LOAD &param -> $local
+            LOAD &param -> $:local
             LOAD 2 -> &param
-            LOAD &param -> $local
+            LOAD &param -> $:local
         }
 
         LOAD 0 -> $local
         CALL MACRO test_macro_parameter_duplicated_access_static(1)
         RETURN $local
         """
             )
             return -1
 
-        mutable = MutableFunction(target)
-        apply_inline_assemblies(mutable)
-        mutable.reassign_to_function()
+        dis.dis(target)
 
         self.assertEqual(target(), 2)
 
     def test_macro_parameter_static_invalid(self):
         def target():
             assembly(
                 """
@@ -1098,15 +1130,15 @@
         self.assertRaises(SyntaxError, lambda: apply_inline_assemblies(mutable))
 
     def test_macro_local_name_override(self):
         def target():
             assembly(
                 """
         MACRO test_macro_local_name_override (!param) {
-            LOAD 10 -> $test
+            LOAD 10 -> $:test
         }
 
         LOAD 0 -> $test
         CALL MACRO test_macro_local_name_override(1)
         RETURN $test
         """
             )
@@ -1119,15 +1151,15 @@
         self.assertEqual(target(), 10)
 
     def test_macro_local_name_escape(self):
         def target():
             assembly(
                 """
         MACRO test_macro_local_name_escape (!param) {
-            LOAD 10 -> $MACRO_test
+            LOAD 10 -> $test
         }
 
         LOAD 0 -> $test
         CALL MACRO test_macro_local_name_escape(1)
         RETURN $test
         """
             )
@@ -1283,33 +1315,52 @@
             )
             return -1
 
         mutable = MutableFunction(target)
         self.assertRaises(NameError, lambda: apply_inline_assemblies(mutable))
 
     def test_macro_paste_use(self):
+        @apply_operations
         def target():
             assembly(
                 """
         MACRO test_macro_paste_use (param) {
-            MACRO_PASTE param -> $test
+            MACRO_PASTE param -> $:test
         }
 
         LOAD 0 -> $test
         CALL MACRO test_macro_paste_use({
             LOAD 10
         })
         RETURN $test
         """
             )
             return -1
 
-        mutable = MutableFunction(target)
-        apply_inline_assemblies(mutable)
-        mutable.reassign_to_function()
+        self.assertEqual(target(), 10)
+
+    def test_macro_paste_use_vbar_prefix(self):
+        @apply_operations
+        def target():
+            assembly(
+                """
+        MACRO test_macro_paste_use_vbar (param) {
+            LOAD 0 -> $test
+            
+            MACRO_PASTE param
+            
+            RETURN $test
+        }
+
+        CALL MACRO test_macro_paste_use_vbar({
+            LOAD 10 -> $|test
+        })
+        """
+            )
+            return -1
 
         self.assertEqual(target(), 10)
 
     def test_macro_overload(self):
         def target():
             assembly(
                 """
@@ -1377,14 +1428,111 @@
 
         mutable = MutableFunction(target)
         apply_inline_assemblies(mutable)
         mutable.reassign_to_function()
 
         self.assertEqual(target(), 1)
 
+    def test_macro_capture_arg_in_inner_func(self):
+        def target():
+            tar = lambda: 0
+            assembly(
+                """
+MACRO test_macro_capture_arg_in_inner_func(a)
+{
+    DEF :tar()
+    {
+        RETURN &a
+    }
+}
+
+CALL MACRO test_macro_capture_arg_in_inner_func(2)
+"""
+            )
+            return tar
+
+        mutable = MutableFunction(target)
+        apply_inline_assemblies(mutable)
+        mutable.reassign_to_function()
+
+        # dis.dis(target)
+
+        self.assertEqual(target()(), 2)
+
+    def test_macro_capture_arg_in_inner_func_2(self):
+        def target():
+            tar = lambda: 0
+            assembly(
+                """
+MACRO test_macro_capture_arg_in_inner_func_2(a CODE_BLOCK)
+{
+    DEF :tar()
+    {
+        MACRO_PASTE a
+    }
+}
+
+CALL MACRO test_macro_capture_arg_in_inner_func_2({ RETURN 2 })
+"""
+            )
+            return tar
+
+        mutable = MutableFunction(target)
+        apply_inline_assemblies(mutable)
+        mutable.reassign_to_function()
+
+        # dis.dis(target)
+
+        self.assertEqual(target()(), 2)
+
+    def test_macro_func_definition_keyword_expansion(self):
+        @apply_operations
+        def target():
+            assembly("""
+MACRO test_macro_func_definition_keyword_expansion(keyword) -> ANY
+{
+    DEF export(&keyword=0)
+    {
+        RETURN $&keyword
+    }
+    
+    MACRO_RETURN $export
+}
+
+CALL MACRO test_macro_func_definition_keyword_expansion("key") -> $func
+RETURN $func
+""")
+            return 0
+
+        inter = target()
+
+        self.assertEqual(inter.__defaults__, (0,))
+
+        self.assertEqual(inter(key=10), 10)
+
+    def test_macro_func_call_keyword_expansion(self):
+        @apply_operations
+        def target():
+            assembly("""
+
+DEF xy(a=0)
+{
+    RETURN $a
+}            
+
+MACRO test_macro_func_call_keyword_expansion(keyword)
+{
+    RETURN $xy(&keyword=4)
+}
+
+CALL MACRO test_macro_func_call_keyword_expansion("key")
+""")
+            return 0
+
+class TestClassAssembly(TestCase):
     def test_class_assembly(self):
         def target():
             test = None
             assembly(
                 """
 CLASS test{}"""
             )
@@ -1452,139 +1600,101 @@
 
         mutable = MutableFunction(target)
         apply_inline_assemblies(mutable)
         mutable.reassign_to_function()
 
         self.assertEqual(target(), 1)
 
+
+class TestFunc2Macro(TestCase):
     def test_transform_to_macro(self):
         @make_macro("TestMacro:test_transform_to_macro")
         def test_transform_to_macro():
+            capture_local("test")
             test = 1
 
+        @apply_operations
         def target():
             test = -1
             assembly(
                 """
 LOAD 0 -> $test
 CALL MACRO TestMacro:test_transform_to_macro()
 """
             )
             return test
 
-        mutable = MutableFunction(target)
-        apply_inline_assemblies(mutable)
-        mutable.reassign_to_function()
-
         self.assertEqual(target(), 1)
 
     def test_transform_to_macro_2(self):
         @make_macro("TestMacro:test_transform_to_macro_2")
         def test_transform_to_macro(a):
+            capture_local("test")
             test = a
 
+        @apply_operations
         def target():
             test = -1
             assembly(
                 """
 LOAD 0 -> $test
 CALL MACRO TestMacro:test_transform_to_macro_2(1)
 """
             )
             return test
 
-        mutable = MutableFunction(target)
-        apply_inline_assemblies(mutable)
-        mutable.reassign_to_function()
-
         self.assertEqual(target(), 1)
 
     def test_transform_to_macro_3(self):
         @make_macro("TestMacro:test_transform_to_macro_3")
         def test_transform_to_macro(a):
+            capture_local("test")
             test = a + a
 
+        @apply_operations
         def target():
             test = -1
             value = [1, 2]
             assembly(
                 """
 LOAD 0 -> $test
 CALL MACRO TestMacro:test_transform_to_macro_3({ CALL $value.pop() })
 """
             )
             return test
 
-        mutable = MutableFunction(target)
-        apply_inline_assemblies(mutable)
-        mutable.reassign_to_function()
-
         self.assertEqual(target(), 3)
 
     def test_transform_to_macro_or_else_error(self):
         @make_macro(
             "TestMacro:test_transform_to_macro_or_else_error", prevent_direct_calls=True
         )
         def test_transform_to_macro():
             pass
 
         self.assertRaises(RuntimeError, test_transform_to_macro)
 
-    def test_macro_capture_arg_in_inner_func(self):
-        def target():
-            tar = lambda: 0
-            assembly(
-                """
-MACRO test_macro_capture_arg_in_inner_func(a)
-{
-    DEF tar()
-    {
-        RETURN &a
-    }
-}
-
-CALL MACRO test_macro_capture_arg_in_inner_func(2)
-"""
-            )
-            return tar
-
-        mutable = MutableFunction(target)
-        apply_inline_assemblies(mutable)
-        mutable.reassign_to_function()
-
-        # dis.dis(target)
-
-        self.assertEqual(target()(), 2)
+    def test_transform_to_macro_inner_return(self):
+        @make_macro("TestMacro:test_transform_to_macro_inner_return")
+        def test_transform_to_macro():
+            outer_return(1)
 
-    def test_macro_capture_arg_in_inner_func_2(self):
+        @apply_operations
         def target():
-            tar = lambda: 0
             assembly(
                 """
-MACRO test_macro_capture_arg_in_inner_func_2(a CODE_BLOCK)
-{
-    DEF tar()
-    {
-        MACRO_PASTE a
-    }
-}
-
-CALL MACRO test_macro_capture_arg_in_inner_func_2({ RETURN 2 })
+CALL MACRO TestMacro:test_transform_to_macro_inner_return()
 """
             )
-            return tar
-
-        mutable = MutableFunction(target)
-        apply_inline_assemblies(mutable)
-        mutable.reassign_to_function()
+            return 0
 
-        # dis.dis(target)
+        self.assertEqual(target(), 1)
 
-        self.assertEqual(target()(), 2)
 
+class TestForLoopAssembly(TestCase):
     def test_for_loop_basic(self):
         def target():
             iterable = [0, 1, 2, 3]
             result = []
             assembly(
                 """
 FOREACH $p IN $iterable
@@ -1735,15 +1845,16 @@
         try:
             apply_operations(target)
         except AssertionError as e:
             self.assertEqual(e.args, ("assertion failed: hello world",))
 
     def test_assert_static_fail_message_invalid(self):
         def target():
-            assembly("ASSERT_STATIC 0 $x")
+            assembly("""
+ASSERT_STATIC 0 $x""")
 
         try:
             apply_operations(target)
         except AssertionError as e:
             self.assertEqual(
                 e.args,
                 ("assertion failed: expected <true-ish value> (message not arrival)",),
@@ -1752,15 +1863,15 @@
     def test_assert_static_dynamic_expression(self):
         def target():
             assembly("ASSERT_STATIC $a")
 
         try:
             apply_operations(target)
         except SyntaxError as e:
-            self.assertEqual(e.args, ("Expected <static evaluate-able>",))
+            self.assertEqual(e.args, ("Expected <static evaluate-able at 'expression'>",))
 
     def test_assert_static_macro_static_parameter(self):
         @apply_operations
         def target():
             assembly(
                 """
 MACRO test_assert_static_macro_static_parameter(a)
```

### Comparing `bytecodemanipulation-0.3.1/tests/test_InlineSystem.py` & `bytecodemanipulation-0.3.3/tests/test_InlineSystem.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,9 +81,11 @@
             call()
             call()
 
         apply_now()(target)
 
         call = None
 
+        dis.dis(target)
+
         target()
         self.assertEqual(counter, 2)
```

### Comparing `bytecodemanipulation-0.3.1/tests/test_Mixin.py` & `bytecodemanipulation-0.3.3/tests/test_Mixin.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.3.1/tests/test_Operators.py` & `bytecodemanipulation-0.3.3/tests/test_Operators.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import dis
 from unittest import TestCase
 
+from bytecodemanipulation.MutableFunction import MutableFunction
 from bytecodemanipulation.assembler.target import apply_operations
 from bytecodemanipulation.assembler.target import assembly
 
 
 class TestOperators(TestCase):
     def test_simple_and_true(self):
         @apply_operations
@@ -52,14 +53,28 @@
     def test_and_short(self):
         @apply_operations
         def target(tar):
             assembly("""RETURN OP (0 and $tar())""")
 
         self.assertFalse(target(self.fail))
 
+    def test_and_eval_not_short(self):
+        @apply_operations
+        def target(tar):
+            assembly("""RETURN OP (0 andeval $tar())""")
+
+        CALLED = False
+
+        def success():
+            nonlocal CALLED
+            CALLED = True
+
+        self.assertFalse(target(success))
+        self.assertTrue(CALLED)
+
     def test_simple_nand_true(self):
         @apply_operations
         def target():
             assembly("""RETURN OP (1 nand 1)""")
 
         self.assertFalse(target())
 
@@ -152,14 +167,28 @@
     def test_or_short(self):
         @apply_operations
         def target(tar):
             assembly("""RETURN OP (1 or $tar())""")
 
         self.assertTrue(target(self.fail))
 
+    def test_or_eval_not_short(self):
+        @apply_operations
+        def target(tar):
+            assembly("""RETURN OP (1 oreval $tar())""")
+
+        CALLED = False
+
+        def success():
+            nonlocal CALLED
+            CALLED = True
+
+        self.assertTrue(target(success))
+        self.assertTrue(CALLED)
+
     def test_simple_nor_true_true(self):
         @apply_operations
         def target():
             assembly("""RETURN OP (1 nor 1)""")
 
         self.assertFalse(target())
```

### Comparing `bytecodemanipulation-0.3.1/tests/test_Optimiser.py` & `bytecodemanipulation-0.3.3/tests/test_Optimiser.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import math
 import random
 from unittest import TestCase
 
+from bytecodemanipulation.MutableFunction import MutableFunction
 from bytecodemanipulation.optimiser_util import *
 from bytecodemanipulation.Optimiser import (
     guarantee_constant_result,
     cache_global_name,
     _OptimisationContainer,
 )
 from tests.util import compare_optimized_results
```

### Comparing `bytecodemanipulation-0.3.1/tests/test_Specializations.py` & `bytecodemanipulation-0.3.3/tests/test_Specializations.py`

 * *Files identical despite different names*

### Comparing `bytecodemanipulation-0.3.1/tests/test_StandardLibrary.py` & `bytecodemanipulation-0.3.3/tests/test_StandardLibrary.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 
         target()
 
     # todo: can we test somehow the input system
 
     def test_type_check_raise(self):
         def target():
-            assembly("""std:check_type(@int, "test", "exception")""")
+            assembly("""std:check_type(~int, "test", "exception")""")
 
         mutable = MutableFunction(target)
         apply_inline_assemblies(mutable)
         mutable.reassign_to_function()
 
         self.assertRaises(ValueError, target)
 
@@ -136,14 +136,16 @@
         mutable = MutableFunction(target)
         apply_inline_assemblies(mutable)
         mutable.reassign_to_function()
 
         self.assertEqual(target(), 3)
 
     def test_stream_simple_filter(self):
+
+        @apply_operations
         def target():
             data = (0, 1, 2)
             stream = None
             output = None
             assembly(
                 """
 std:stream:initialize($stream)
@@ -154,20 +156,14 @@
 })
 std:print($stream)
 std:stream:to_list($stream, $output)
 """
             )
             return output
 
-        mutable = MutableFunction(target)
-        apply_inline_assemblies(mutable)
-        mutable.reassign_to_function()
-
-        # dis.dis(target)
-
         self.assertEqual(target(), [0, 1])
 
     def test_stream_simple_map(self):
         def target():
             data = (0, 1, 2)
             stream = None
             output = None
@@ -185,15 +181,14 @@
 
         mutable = MutableFunction(target)
         apply_inline_assemblies(mutable)
         mutable.reassign_to_function()
 
         self.assertEqual(target(), [1, 2, 3])
 
-
 #     def test_comprehension_list(self):
 #         def target():
 #             l = [1, 2, 3, 4]
 #             assembly("""
 # std:comprehension:list($l, $value, { OP $value + 1 -> % }) -> %
 # RETURN %""")
 #
```

### Comparing `bytecodemanipulation-0.3.1/tests/test_issues.py` & `bytecodemanipulation-0.3.3/tests/test_issues.py`

 * *Files identical despite different names*

