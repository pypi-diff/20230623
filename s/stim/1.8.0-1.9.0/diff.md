# Comparing `tmp/stim-1.8.0.tar.gz` & `tmp/stim-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stim-1.8.0.tar", last modified: Sun Jan 30 06:34:24 2022, max compression
+gzip compressed data, was "stim-1.9.0.tar", last modified: Sun Jul 10 05:40:17 2022, max compression
```

## Comparing `stim-1.8.0.tar` & `stim-1.9.0.tar`

### file list

```diff
@@ -1,100 +1,267 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-30 06:34:24.828296 stim-1.8.0/
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-01-30 06:34:22.000000 stim-1.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     4178 2022-01-30 06:34:24.828296 stim-1.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3846 2022-01-30 06:34:22.000000 stim-1.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-30 06:34:24.820296 stim-1.8.0/glue/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-30 06:34:24.820296 stim-1.8.0/glue/python/
--rw-r--r--   0 runner    (1001) docker     (121)     3846 2022-01-30 06:34:22.000000 stim-1.8.0/glue/python/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-30 06:34:24.820296 stim-1.8.0/glue/python/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-30 06:34:24.820296 stim-1.8.0/glue/python/src/stim/
--rw-r--r--   0 runner    (1001) docker     (121)      868 2022-01-30 06:34:22.000000 stim-1.8.0/glue/python/src/stim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      109 2022-01-30 06:34:22.000000 stim-1.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-01-30 06:34:24.828296 stim-1.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     3105 2022-01-30 06:34:22.000000 stim-1.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-30 06:34:24.820296 stim-1.8.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-30 06:34:24.820296 stim-1.8.0/src/stim/
--rw-r--r--   0 runner    (1001) docker     (121)    10123 2022-01-30 06:34:22.000000 stim-1.8.0/src/stim/arg_parse.cc
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-30 06:34:24.824296 stim-1.8.0/src/stim/circuit/
--rw-r--r--   0 runner    (1001) docker     (121)    43892 2022-01-30 06:34:22.000000 stim-1.8.0/src/stim/circuit/circuit.cc
--rw-r--r--   0 runner    (1001) docker     (121)    58683 2022-01-30 06:34:22.000000 stim-1.8.0/src/stim/circuit/circuit.pybind.cc
--rw-r--r--   0 runner    (1001) docker     (121)     5347 2022-01-30 06:34:22.000000 stim-1.8.0/src/stim/circuit/circuit_gate_target.pybind.cc
--rw-r--r--   0 runner    (1001) docker     (121)     5907 2022-01-30 06:34:22.000000 stim-1.8.0/src/stim/circuit/circuit_instruction.pybind.cc
--rw-r--r--   0 runner    (1001) docker     (121)     4622 2022-01-30 06:34:22.000000 stim-1.8.0/src/stim/circuit/circuit_repeat_block.pybind.cc
--rw-r--r--   0 runner    (1001) docker     (121)     5472 2022-01-30 06:34:22.000000 stim-1.8.0/src/stim/circuit/gate_data.cc
--rw-r--r--   0 runner    (1001) docker     (121)    13476 2022-01-30 06:34:22.000000 stim-1.8.0/src/stim/circuit/gate_data_annotations.cc
--rw-r--r--   0 runner    (1001) docker     (121)     2097 2022-01-30 06:34:22.000000 stim-1.8.0/src/stim/circuit/gate_data_blocks.cc
--rw-r--r--   0 runner    (1001) docker     (121)    14124 2022-01-30 06:34:22.000000 stim-1.8.0/src/stim/circuit/gate_data_collapsing.cc
--rw-r--r--   0 runner    (1001) docker     (121)    10567 2022-01-30 06:34:22.000000 stim-1.8.0/src/stim/circuit/gate_data_controlled.cc
--rw-r--r--   0 runner    (1001) docker     (121)     3233 2022-01-30 06:34:22.000000 stim-1.8.0/src/stim/circuit/gate_data_hada.cc
--rw-r--r--   0 runner    (1001) docker     (121)    11728 2022-01-30 06:34:22.000000 stim-1.8.0/src/stim/circuit/gate_data_noisy.cc
--rw-r--r--   0 runner    (1001) docker     (121)     3588 2022-01-30 06:34:22.000000 stim-1.8.0/src/stim/circuit/gate_data_pauli.cc
--rw-r--r--   0 runner    (1001) docker     (121)     2491 2022-01-30 06:34:22.000000 stim-1.8.0/src/stim/circuit/gate_data_period_3.cc
--rw-r--r--   0 runner    (1001) docker     (121)     5659 2022-01-30 06:34:22.000000 stim-1.8.0/src/stim/circuit/gate_data_period_4.cc
--rw-r--r--   0 runner    (1001) docker     (121)     6648 2022-01-30 06:34:22.000000 stim-1.8.0/src/stim/circuit/gate_data_pp.cc
--rw-r--r--   0 runner    (1001) docker     (121)     3529 2022-01-30 06:34:22.000000 stim-1.8.0/src/stim/circuit/gate_data_swaps.cc
--rw-r--r--   0 runner    (1001) docker     (121)     5804 2022-01-30 06:34:22.000000 stim-1.8.0/src/stim/circuit/gate_target.cc
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-30 06:34:24.824296 stim-1.8.0/src/stim/dem/
--rw-r--r--   0 runner    (1001) docker     (121)    29857 2022-01-30 06:34:22.000000 stim-1.8.0/src/stim/dem/detector_error_model.cc
--rw-r--r--   0 runner    (1001) docker     (121)    31458 2022-01-30 06:34:22.000000 stim-1.8.0/src/stim/dem/detector_error_model.pybind.cc
--rw-r--r--   0 runner    (1001) docker     (121)     7928 2022-01-30 06:34:22.000000 stim-1.8.0/src/stim/dem/detector_error_model_instruction.pybind.cc
--rw-r--r--   0 runner    (1001) docker     (121)     3690 2022-01-30 06:34:22.000000 stim-1.8.0/src/stim/dem/detector_error_model_repeat_block.pybind.cc
--rw-r--r--   0 runner    (1001) docker     (121)     8379 2022-01-30 06:34:22.000000 stim-1.8.0/src/stim/dem/detector_error_model_target.pybind.cc
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-30 06:34:24.824296 stim-1.8.0/src/stim/gen/
--rw-r--r--   0 runner    (1001) docker     (121)     2887 2022-01-30 06:34:22.000000 stim-1.8.0/src/stim/gen/circuit_gen_main.cc
--rw-r--r--   0 runner    (1001) docker     (121)     4061 2022-01-30 06:34:22.000000 stim-1.8.0/src/stim/gen/circuit_gen_params.cc
--rw-r--r--   0 runner    (1001) docker     (121)     7920 2022-01-30 06:34:22.000000 stim-1.8.0/src/stim/gen/gen_color_code.cc
--rw-r--r--   0 runner    (1001) docker     (121)     3753 2022-01-30 06:34:22.000000 stim-1.8.0/src/stim/gen/gen_rep_code.cc
--rw-r--r--   0 runner    (1001) docker     (121)    13501 2022-01-30 06:34:22.000000 stim-1.8.0/src/stim/gen/gen_surface_code.cc
--rw-r--r--   0 runner    (1001) docker     (121)    44722 2022-01-30 06:34:22.000000 stim-1.8.0/src/stim/help.cc
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-30 06:34:24.824296 stim-1.8.0/src/stim/io/
--rw-r--r--   0 runner    (1001) docker     (121)     1735 2022-01-30 06:34:22.000000 stim-1.8.0/src/stim/io/measure_record.cc
--rw-r--r--   0 runner    (1001) docker     (121)     4259 2022-01-30 06:34:22.000000 stim-1.8.0/src/stim/io/measure_record_batch.cc
--rw-r--r--   0 runner    (1001) docker     (121)     3369 2022-01-30 06:34:22.000000 stim-1.8.0/src/stim/io/measure_record_batch_writer.cc
--rw-r--r--   0 runner    (1001) docker     (121)    20882 2022-01-30 06:34:22.000000 stim-1.8.0/src/stim/io/measure_record_reader.cc
--rw-r--r--   0 runner    (1001) docker     (121)     8352 2022-01-30 06:34:22.000000 stim-1.8.0/src/stim/io/measure_record_writer.cc
--rw-r--r--   0 runner    (1001) docker     (121)     1409 2022-01-30 06:34:22.000000 stim-1.8.0/src/stim/io/sparse_shot.cc
--rw-r--r--   0 runner    (1001) docker     (121)    16267 2022-01-30 06:34:22.000000 stim-1.8.0/src/stim/io/stim_data_formats.cc
--rw-r--r--   0 runner    (1001) docker     (121)    12545 2022-01-30 06:34:22.000000 stim-1.8.0/src/stim/main_namespaced.cc
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-30 06:34:24.824296 stim-1.8.0/src/stim/mem/
--rw-r--r--   0 runner    (1001) docker     (121)      772 2022-01-30 06:34:22.000000 stim-1.8.0/src/stim/mem/bit_ref.cc
--rw-r--r--   0 runner    (1001) docker     (121)    10193 2022-01-30 06:34:22.000000 stim-1.8.0/src/stim/mem/simd_bit_table.cc
--rw-r--r--   0 runner    (1001) docker     (121)     4564 2022-01-30 06:34:22.000000 stim-1.8.0/src/stim/mem/simd_bits.cc
--rw-r--r--   0 runner    (1001) docker     (121)     3921 2022-01-30 06:34:22.000000 stim-1.8.0/src/stim/mem/simd_bits_range_ref.cc
--rw-r--r--   0 runner    (1001) docker     (121)      623 2022-01-30 06:34:22.000000 stim-1.8.0/src/stim/mem/simd_compat.cc
--rw-r--r--   0 runner    (1001) docker     (121)      621 2022-01-30 06:34:22.000000 stim-1.8.0/src/stim/mem/simd_util.cc
--rw-r--r--   0 runner    (1001) docker     (121)      633 2022-01-30 06:34:22.000000 stim-1.8.0/src/stim/mem/sparse_xor_vec.cc
--rw-r--r--   0 runner    (1001) docker     (121)     4622 2022-01-30 06:34:22.000000 stim-1.8.0/src/stim/probability_util.cc
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-30 06:34:24.824296 stim-1.8.0/src/stim/py/
--rw-r--r--   0 runner    (1001) docker     (121)     3607 2022-01-30 06:34:22.000000 stim-1.8.0/src/stim/py/base.pybind.cc
--rw-r--r--   0 runner    (1001) docker     (121)    11708 2022-01-30 06:34:22.000000 stim-1.8.0/src/stim/py/compiled_detector_sampler.pybind.cc
--rw-r--r--   0 runner    (1001) docker     (121)    11734 2022-01-30 06:34:22.000000 stim-1.8.0/src/stim/py/compiled_measurement_sampler.pybind.cc
--rw-r--r--   0 runner    (1001) docker     (121)     1189 2022-01-30 06:34:22.000000 stim-1.8.0/src/stim/py/march.pybind.cc
--rw-r--r--   0 runner    (1001) docker     (121)     7258 2022-01-30 06:34:22.000000 stim-1.8.0/src/stim/py/stim.pybind.cc
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-30 06:34:24.828296 stim-1.8.0/src/stim/simulators/
--rw-r--r--   0 runner    (1001) docker     (121)     7421 2022-01-30 06:34:22.000000 stim-1.8.0/src/stim/simulators/detection_simulator.cc
--rw-r--r--   0 runner    (1001) docker     (121)    50028 2022-01-30 06:34:22.000000 stim-1.8.0/src/stim/simulators/error_analyzer.cc
--rw-r--r--   0 runner    (1001) docker     (121)    13171 2022-01-30 06:34:22.000000 stim-1.8.0/src/stim/simulators/error_matcher.cc
--rw-r--r--   0 runner    (1001) docker     (121)    22561 2022-01-30 06:34:22.000000 stim-1.8.0/src/stim/simulators/frame_simulator.cc
--rw-r--r--   0 runner    (1001) docker     (121)    14238 2022-01-30 06:34:22.000000 stim-1.8.0/src/stim/simulators/matched_error.cc
--rw-r--r--   0 runner    (1001) docker     (121)    23996 2022-01-30 06:34:22.000000 stim-1.8.0/src/stim/simulators/matched_error.pybind.cc
--rw-r--r--   0 runner    (1001) docker     (121)    11347 2022-01-30 06:34:22.000000 stim-1.8.0/src/stim/simulators/measurements_to_detection_events.cc
--rw-r--r--   0 runner    (1001) docker     (121)    15504 2022-01-30 06:34:22.000000 stim-1.8.0/src/stim/simulators/measurements_to_detection_events.pybind.cc
--rw-r--r--   0 runner    (1001) docker     (121)    12182 2022-01-30 06:34:22.000000 stim-1.8.0/src/stim/simulators/min_distance.cc
--rw-r--r--   0 runner    (1001) docker     (121)    35132 2022-01-30 06:34:22.000000 stim-1.8.0/src/stim/simulators/tableau_simulator.cc
--rw-r--r--   0 runner    (1001) docker     (121)    36585 2022-01-30 06:34:22.000000 stim-1.8.0/src/stim/simulators/tableau_simulator.pybind.cc
--rw-r--r--   0 runner    (1001) docker     (121)     6482 2022-01-30 06:34:22.000000 stim-1.8.0/src/stim/simulators/vector_simulator.cc
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-30 06:34:24.828296 stim-1.8.0/src/stim/stabilizers/
--rw-r--r--   0 runner    (1001) docker     (121)     4476 2022-01-30 06:34:22.000000 stim-1.8.0/src/stim/stabilizers/pauli_string.cc
--rw-r--r--   0 runner    (1001) docker     (121)    30540 2022-01-30 06:34:22.000000 stim-1.8.0/src/stim/stabilizers/pauli_string.pybind.cc
--rw-r--r--   0 runner    (1001) docker     (121)     4715 2022-01-30 06:34:22.000000 stim-1.8.0/src/stim/stabilizers/pauli_string_ref.cc
--rw-r--r--   0 runner    (1001) docker     (121)    20248 2022-01-30 06:34:22.000000 stim-1.8.0/src/stim/stabilizers/tableau.cc
--rw-r--r--   0 runner    (1001) docker     (121)    38940 2022-01-30 06:34:22.000000 stim-1.8.0/src/stim/stabilizers/tableau.pybind.cc
--rw-r--r--   0 runner    (1001) docker     (121)     5320 2022-01-30 06:34:22.000000 stim-1.8.0/src/stim/stabilizers/tableau_specialized_prepend.cc
--rw-r--r--   0 runner    (1001) docker     (121)     4495 2022-01-30 06:34:22.000000 stim-1.8.0/src/stim/stabilizers/tableau_transposed_raii.cc
--rw-r--r--   0 runner    (1001) docker     (121)      614 2022-01-30 06:34:22.000000 stim-1.8.0/src/stim.cc
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-30 06:34:24.828296 stim-1.8.0/stim.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4178 2022-01-30 06:34:24.000000 stim-1.8.0/stim.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2872 2022-01-30 06:34:24.000000 stim-1.8.0/stim.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-30 06:34:24.000000 stim-1.8.0/stim.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-01-30 06:34:24.000000 stim-1.8.0/stim.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        5 2022-01-30 06:34:24.000000 stim-1.8.0/stim.egg-info/top_level.txt
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-07-10 05:40:17.590165 stim-1.9.0/
+-rw-r--r--   0 runner     (501) staff       (20)    11357 2022-07-10 05:17:41.000000 stim-1.9.0/LICENSE
+-rw-r--r--   0 runner     (501) staff       (20)      103 2022-07-10 05:17:41.000000 stim-1.9.0/MANIFEST.in
+-rw-r--r--   0 runner     (501) staff       (20)     4196 2022-07-10 05:40:17.589768 stim-1.9.0/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)     3846 2022-07-10 05:17:41.000000 stim-1.9.0/README.md
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-07-10 05:40:17.442047 stim-1.9.0/glue/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-07-10 05:40:17.448296 stim-1.9.0/glue/python/
+-rw-r--r--   0 runner     (501) staff       (20)     3846 2022-07-10 05:17:41.000000 stim-1.9.0/glue/python/README.md
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-07-10 05:40:17.442420 stim-1.9.0/glue/python/src/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-07-10 05:40:17.450164 stim-1.9.0/glue/python/src/stim/
+-rw-r--r--   0 runner     (501) staff       (20)     2357 2022-07-10 05:17:41.000000 stim-1.9.0/glue/python/src/stim/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)   204702 2022-07-10 05:17:41.000000 stim-1.9.0/glue/python/src/stim/__init__.pyi
+-rw-r--r--   0 runner     (501) staff       (20)      134 2022-07-10 05:17:41.000000 stim-1.9.0/glue/python/src/stim/_main_argv.py
+-rw-r--r--   0 runner     (501) staff       (20)      109 2022-07-10 05:17:41.000000 stim-1.9.0/pyproject.toml
+-rw-r--r--   0 runner     (501) staff       (20)       38 2022-07-10 05:40:17.590267 stim-1.9.0/setup.cfg
+-rw-r--r--   0 runner     (501) staff       (20)     3655 2022-07-10 05:17:41.000000 stim-1.9.0/setup.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-07-10 05:40:17.452511 stim-1.9.0/src/
+-rw-r--r--   0 runner     (501) staff       (20)      701 2022-07-10 05:17:41.000000 stim-1.9.0/src/main.cc
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-07-10 05:40:17.462734 stim-1.9.0/src/stim/
+-rw-r--r--   0 runner     (501) staff       (20)    10123 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/arg_parse.cc
+-rw-r--r--   0 runner     (501) staff       (20)     9242 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/arg_parse.h
+-rw-r--r--   0 runner     (501) staff       (20)    11209 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/arg_parse.test.cc
+-rw-r--r--   0 runner     (501) staff       (20)     6036 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/benchmark_main.perf.cc
+-rw-r--r--   0 runner     (501) staff       (20)      627 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/benchmark_util.perf.cc
+-rw-r--r--   0 runner     (501) staff       (20)     3973 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/benchmark_util.perf.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-07-10 05:40:17.479111 stim-1.9.0/src/stim/circuit/
+-rw-r--r--   0 runner     (501) staff       (20)    47320 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/circuit/circuit.cc
+-rw-r--r--   0 runner     (501) staff       (20)    15456 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/circuit/circuit.h
+-rw-r--r--   0 runner     (501) staff       (20)     1431 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/circuit/circuit.perf.cc
+-rw-r--r--   0 runner     (501) staff       (20)    74455 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/circuit/circuit.pybind.cc
+-rw-r--r--   0 runner     (501) staff       (20)     1080 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/circuit/circuit.pybind.h
+-rw-r--r--   0 runner     (501) staff       (20)    36126 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/circuit/circuit.test.cc
+-rw-r--r--   0 runner     (501) staff       (20)      977 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/circuit/circuit.test.h
+-rw-r--r--   0 runner     (501) staff       (20)     5342 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/circuit/circuit_gate_target.pybind.cc
+-rw-r--r--   0 runner     (501) staff       (20)      996 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/circuit/circuit_gate_target.pybind.h
+-rw-r--r--   0 runner     (501) staff       (20)     5902 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/circuit/circuit_instruction.pybind.cc
+-rw-r--r--   0 runner     (501) staff       (20)     1668 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/circuit/circuit_instruction.pybind.h
+-rw-r--r--   0 runner     (501) staff       (20)     4617 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/circuit/circuit_repeat_block.pybind.cc
+-rw-r--r--   0 runner     (501) staff       (20)     1155 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/circuit/circuit_repeat_block.pybind.h
+-rw-r--r--   0 runner     (501) staff       (20)     5472 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/circuit/gate_data.cc
+-rw-r--r--   0 runner     (501) staff       (20)     9837 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/circuit/gate_data.h
+-rw-r--r--   0 runner     (501) staff       (20)     1198 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/circuit/gate_data.perf.cc
+-rw-r--r--   0 runner     (501) staff       (20)     3280 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/circuit/gate_data.test.cc
+-rw-r--r--   0 runner     (501) staff       (20)    13456 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/circuit/gate_data_annotations.cc
+-rw-r--r--   0 runner     (501) staff       (20)     2093 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/circuit/gate_data_blocks.cc
+-rw-r--r--   0 runner     (501) staff       (20)    14084 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/circuit/gate_data_collapsing.cc
+-rw-r--r--   0 runner     (501) staff       (20)    10531 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/circuit/gate_data_controlled.cc
+-rw-r--r--   0 runner     (501) staff       (20)     3221 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/circuit/gate_data_hada.cc
+-rw-r--r--   0 runner     (501) staff       (20)    11977 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/circuit/gate_data_noisy.cc
+-rw-r--r--   0 runner     (501) staff       (20)     3588 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/circuit/gate_data_pauli.cc
+-rw-r--r--   0 runner     (501) staff       (20)     2483 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/circuit/gate_data_period_3.cc
+-rw-r--r--   0 runner     (501) staff       (20)     5635 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/circuit/gate_data_period_4.cc
+-rw-r--r--   0 runner     (501) staff       (20)     6624 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/circuit/gate_data_pp.cc
+-rw-r--r--   0 runner     (501) staff       (20)     3517 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/circuit/gate_data_swaps.cc
+-rw-r--r--   0 runner     (501) staff       (20)     5748 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/circuit/gate_target.cc
+-rw-r--r--   0 runner     (501) staff       (20)     2307 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/circuit/gate_target.h
+-rw-r--r--   0 runner     (501) staff       (20)     6040 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/circuit/gate_target.test.cc
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-07-10 05:40:17.484579 stim-1.9.0/src/stim/dem/
+-rw-r--r--   0 runner     (501) staff       (20)    31371 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/dem/detector_error_model.cc
+-rw-r--r--   0 runner     (501) staff       (20)     7894 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/dem/detector_error_model.h
+-rw-r--r--   0 runner     (501) staff       (20)    36713 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/dem/detector_error_model.pybind.cc
+-rw-r--r--   0 runner     (501) staff       (20)      901 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/dem/detector_error_model.pybind.h
+-rw-r--r--   0 runner     (501) staff       (20)    25490 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/dem/detector_error_model.test.cc
+-rw-r--r--   0 runner     (501) staff       (20)     8077 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/dem/detector_error_model_instruction.pybind.cc
+-rw-r--r--   0 runner     (501) staff       (20)     1437 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/dem/detector_error_model_instruction.pybind.h
+-rw-r--r--   0 runner     (501) staff       (20)     3686 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/dem/detector_error_model_repeat_block.pybind.cc
+-rw-r--r--   0 runner     (501) staff       (20)     1159 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/dem/detector_error_model_repeat_block.pybind.h
+-rw-r--r--   0 runner     (501) staff       (20)     8395 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/dem/detector_error_model_target.pybind.cc
+-rw-r--r--   0 runner     (501) staff       (20)     1221 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/dem/detector_error_model_target.pybind.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-07-10 05:40:17.491515 stim-1.9.0/src/stim/gen/
+-rw-r--r--   0 runner     (501) staff       (20)     2887 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/gen/circuit_gen_main.cc
+-rw-r--r--   0 runner     (501) staff       (20)      249 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/gen/circuit_gen_main.h
+-rw-r--r--   0 runner     (501) staff       (20)     2181 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/gen/circuit_gen_main.test.cc
+-rw-r--r--   0 runner     (501) staff       (20)     4061 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/gen/circuit_gen_params.cc
+-rw-r--r--   0 runner     (501) staff       (20)     1460 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/gen/circuit_gen_params.h
+-rw-r--r--   0 runner     (501) staff       (20)     4762 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/gen/circuit_gen_params.test.cc
+-rw-r--r--   0 runner     (501) staff       (20)     7920 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/gen/gen_color_code.cc
+-rw-r--r--   0 runner     (501) staff       (20)      256 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/gen/gen_color_code.h
+-rw-r--r--   0 runner     (501) staff       (20)     4373 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/gen/gen_color_code.test.cc
+-rw-r--r--   0 runner     (501) staff       (20)     3753 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/gen/gen_rep_code.cc
+-rw-r--r--   0 runner     (501) staff       (20)      250 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/gen/gen_rep_code.h
+-rw-r--r--   0 runner     (501) staff       (20)     2356 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/gen/gen_rep_code.test.cc
+-rw-r--r--   0 runner     (501) staff       (20)    13501 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/gen/gen_surface_code.cc
+-rw-r--r--   0 runner     (501) staff       (20)      262 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/gen/gen_surface_code.h
+-rw-r--r--   0 runner     (501) staff       (20)     9269 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/gen/gen_surface_code.test.cc
+-rw-r--r--   0 runner     (501) staff       (20)    46890 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/help.cc
+-rw-r--r--   0 runner     (501) staff       (20)      808 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/help.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-07-10 05:40:17.503481 stim-1.9.0/src/stim/io/
+-rw-r--r--   0 runner     (501) staff       (20)     1735 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/io/measure_record.cc
+-rw-r--r--   0 runner     (501) staff       (20)     2117 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/io/measure_record.h
+-rw-r--r--   0 runner     (501) staff       (20)     1377 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/io/measure_record.test.cc
+-rw-r--r--   0 runner     (501) staff       (20)     4259 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/io/measure_record_batch.cc
+-rw-r--r--   0 runner     (501) staff       (20)     3858 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/io/measure_record_batch.h
+-rw-r--r--   0 runner     (501) staff       (20)     2210 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/io/measure_record_batch.test.cc
+-rw-r--r--   0 runner     (501) staff       (20)     3508 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/io/measure_record_batch_writer.cc
+-rw-r--r--   0 runner     (501) staff       (20)     2859 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/io/measure_record_batch_writer.h
+-rw-r--r--   0 runner     (501) staff       (20)     1276 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/io/measure_record_batch_writer.test.cc
+-rw-r--r--   0 runner     (501) staff       (20)    13034 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/io/measure_record_reader.cc
+-rw-r--r--   0 runner     (501) staff       (20)    14427 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/io/measure_record_reader.h
+-rw-r--r--   0 runner     (501) staff       (20)     4085 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/io/measure_record_reader.perf.cc
+-rw-r--r--   0 runner     (501) staff       (20)    24778 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/io/measure_record_reader.test.cc
+-rw-r--r--   0 runner     (501) staff       (20)     8042 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/io/measure_record_writer.cc
+-rw-r--r--   0 runner     (501) staff       (20)     4038 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/io/measure_record_writer.h
+-rw-r--r--   0 runner     (501) staff       (20)    14152 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/io/measure_record_writer.test.cc
+-rw-r--r--   0 runner     (501) staff       (20)     1218 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/io/raii_file.cc
+-rw-r--r--   0 runner     (501) staff       (20)      899 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/io/raii_file.h
+-rw-r--r--   0 runner     (501) staff       (20)    16178 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/io/read_write.pybind.cc
+-rw-r--r--   0 runner     (501) staff       (20)     1163 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/io/read_write.pybind.h
+-rw-r--r--   0 runner     (501) staff       (20)     1409 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/io/sparse_shot.cc
+-rw-r--r--   0 runner     (501) staff       (20)     1325 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/io/sparse_shot.h
+-rw-r--r--   0 runner     (501) staff       (20)     1350 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/io/sparse_shot.test.cc
+-rw-r--r--   0 runner     (501) staff       (20)    16245 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/io/stim_data_formats.cc
+-rw-r--r--   0 runner     (501) staff       (20)      558 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/io/stim_data_formats.h
+-rw-r--r--   0 runner     (501) staff       (20)    13925 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/main_namespaced.cc
+-rw-r--r--   0 runner     (501) staff       (20)      822 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/main_namespaced.h
+-rw-r--r--   0 runner     (501) staff       (20)     5958 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/main_namespaced.perf.cc
+-rw-r--r--   0 runner     (501) staff       (20)    23484 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/main_namespaced.test.cc
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-07-10 05:40:17.520695 stim-1.9.0/src/stim/mem/
+-rw-r--r--   0 runner     (501) staff       (20)      772 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/mem/bit_ref.cc
+-rw-r--r--   0 runner     (501) staff       (20)     2520 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/mem/bit_ref.h
+-rw-r--r--   0 runner     (501) staff       (20)     2434 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/mem/bit_ref.test.cc
+-rw-r--r--   0 runner     (501) staff       (20)     4103 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/mem/fixed_cap_vector.h
+-rw-r--r--   0 runner     (501) staff       (20)     3256 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/mem/fixed_cap_vector.test.cc
+-rw-r--r--   0 runner     (501) staff       (20)     6232 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/mem/monotonic_buffer.h
+-rw-r--r--   0 runner     (501) staff       (20)     1486 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/mem/monotonic_buffer.test.cc
+-rw-r--r--   0 runner     (501) staff       (20)     5590 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/mem/pointer_range.h
+-rw-r--r--   0 runner     (501) staff       (20)    10193 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/mem/simd_bit_table.cc
+-rw-r--r--   0 runner     (501) staff       (20)     7148 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/mem/simd_bit_table.h
+-rw-r--r--   0 runner     (501) staff       (20)     1215 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/mem/simd_bit_table.perf.cc
+-rw-r--r--   0 runner     (501) staff       (20)     6374 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/mem/simd_bit_table.test.cc
+-rw-r--r--   0 runner     (501) staff       (20)     4564 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/mem/simd_bits.cc
+-rw-r--r--   0 runner     (501) staff       (20)     6109 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/mem/simd_bits.h
+-rw-r--r--   0 runner     (501) staff       (20)     1340 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/mem/simd_bits.perf.cc
+-rw-r--r--   0 runner     (501) staff       (20)     8004 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/mem/simd_bits.test.cc
+-rw-r--r--   0 runner     (501) staff       (20)     3921 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/mem/simd_bits_range_ref.cc
+-rw-r--r--   0 runner     (501) staff       (20)    12929 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/mem/simd_bits_range_ref.h
+-rw-r--r--   0 runner     (501) staff       (20)    10063 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/mem/simd_bits_range_ref.test.cc
+-rw-r--r--   0 runner     (501) staff       (20)      623 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/mem/simd_compat.cc
+-rw-r--r--   0 runner     (501) staff       (20)      831 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/mem/simd_compat.h
+-rw-r--r--   0 runner     (501) staff       (20)     1254 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/mem/simd_compat.perf.cc
+-rw-r--r--   0 runner     (501) staff       (20)     2541 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/mem/simd_compat.test.cc
+-rw-r--r--   0 runner     (501) staff       (20)     3658 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/mem/simd_compat_avx2.h
+-rw-r--r--   0 runner     (501) staff       (20)     4289 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/mem/simd_compat_polyfill.h
+-rw-r--r--   0 runner     (501) staff       (20)     3485 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/mem/simd_compat_sse2.h
+-rw-r--r--   0 runner     (501) staff       (20)     1522 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/mem/simd_util.cc
+-rw-r--r--   0 runner     (501) staff       (20)     1519 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/mem/simd_util.h
+-rw-r--r--   0 runner     (501) staff       (20)     5551 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/mem/simd_util.test.cc
+-rw-r--r--   0 runner     (501) staff       (20)      633 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/mem/sparse_xor_vec.cc
+-rw-r--r--   0 runner     (501) staff       (20)     6646 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/mem/sparse_xor_vec.h
+-rw-r--r--   0 runner     (501) staff       (20)     1355 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/mem/sparse_xor_vec.perf.cc
+-rw-r--r--   0 runner     (501) staff       (20)     6750 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/mem/sparse_xor_vec.test.cc
+-rw-r--r--   0 runner     (501) staff       (20)     4622 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/probability_util.cc
+-rw-r--r--   0 runner     (501) staff       (20)     2196 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/probability_util.h
+-rw-r--r--   0 runner     (501) staff       (20)     2881 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/probability_util.perf.cc
+-rw-r--r--   0 runner     (501) staff       (20)     2460 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/probability_util.test.cc
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-07-10 05:40:17.527402 stim-1.9.0/src/stim/py/
+-rw-r--r--   0 runner     (501) staff       (20)     3511 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/py/base.pybind.cc
+-rw-r--r--   0 runner     (501) staff       (20)     1720 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/py/base.pybind.h
+-rw-r--r--   0 runner     (501) staff       (20)    12489 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/py/compiled_detector_sampler.pybind.cc
+-rw-r--r--   0 runner     (501) staff       (20)     2182 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/py/compiled_detector_sampler.pybind.h
+-rw-r--r--   0 runner     (501) staff       (20)    11714 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/py/compiled_measurement_sampler.pybind.cc
+-rw-r--r--   0 runner     (501) staff       (20)     2038 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/py/compiled_measurement_sampler.pybind.h
+-rw-r--r--   0 runner     (501) staff       (20)     1655 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/py/march.pybind.cc
+-rw-r--r--   0 runner     (501) staff       (20)      210 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/py/march.pybind.h
+-rw-r--r--   0 runner     (501) staff       (20)    10346 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/py/stim.pybind.cc
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-07-10 05:40:17.528366 stim-1.9.0/src/stim/search/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-07-10 05:40:17.542134 stim-1.9.0/src/stim/search/graphlike/
+-rw-r--r--   0 runner     (501) staff       (20)     3666 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/search/graphlike/algo.cc
+-rw-r--r--   0 runner     (501) staff       (20)     1883 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/search/graphlike/algo.h
+-rw-r--r--   0 runner     (501) staff       (20)     1520 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/search/graphlike/algo.perf.cc
+-rw-r--r--   0 runner     (501) staff       (20)     5967 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/search/graphlike/algo.test.cc
+-rw-r--r--   0 runner     (501) staff       (20)     1598 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/search/graphlike/edge.cc
+-rw-r--r--   0 runner     (501) staff       (20)     1173 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/search/graphlike/edge.h
+-rw-r--r--   0 runner     (501) staff       (20)     1299 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/search/graphlike/edge.test.cc
+-rw-r--r--   0 runner     (501) staff       (20)     4535 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/search/graphlike/graph.cc
+-rw-r--r--   0 runner     (501) staff       (20)     1664 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/search/graphlike/graph.h
+-rw-r--r--   0 runner     (501) staff       (20)     5946 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/search/graphlike/graph.test.cc
+-rw-r--r--   0 runner     (501) staff       (20)     1247 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/search/graphlike/node.cc
+-rw-r--r--   0 runner     (501) staff       (20)     1241 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/search/graphlike/node.h
+-rw-r--r--   0 runner     (501) staff       (20)     1214 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/search/graphlike/node.test.cc
+-rw-r--r--   0 runner     (501) staff       (20)     3824 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/search/graphlike/search_state.cc
+-rw-r--r--   0 runner     (501) staff       (20)     1717 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/search/graphlike/search_state.h
+-rw-r--r--   0 runner     (501) staff       (20)     5135 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/search/graphlike/search_state.test.cc
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-07-10 05:40:17.558324 stim-1.9.0/src/stim/search/hyper/
+-rw-r--r--   0 runner     (501) staff       (20)     4075 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/search/hyper/algo.cc
+-rw-r--r--   0 runner     (501) staff       (20)     3726 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/search/hyper/algo.h
+-rw-r--r--   0 runner     (501) staff       (20)     6614 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/search/hyper/algo.test.cc
+-rw-r--r--   0 runner     (501) staff       (20)     1780 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/search/hyper/edge.cc
+-rw-r--r--   0 runner     (501) staff       (20)     1145 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/search/hyper/edge.h
+-rw-r--r--   0 runner     (501) staff       (20)     1220 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/search/hyper/edge.test.cc
+-rw-r--r--   0 runner     (501) staff       (20)     2764 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/search/hyper/graph.cc
+-rw-r--r--   0 runner     (501) staff       (20)     1460 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/search/hyper/graph.h
+-rw-r--r--   0 runner     (501) staff       (20)     3834 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/search/hyper/graph.test.cc
+-rw-r--r--   0 runner     (501) staff       (20)     1187 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/search/hyper/node.cc
+-rw-r--r--   0 runner     (501) staff       (20)     1061 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/search/hyper/node.h
+-rw-r--r--   0 runner     (501) staff       (20)     1202 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/search/hyper/node.test.cc
+-rw-r--r--   0 runner     (501) staff       (20)     2584 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/search/hyper/search_state.cc
+-rw-r--r--   0 runner     (501) staff       (20)     1319 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/search/hyper/search_state.h
+-rw-r--r--   0 runner     (501) staff       (20)     2764 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/search/hyper/search_state.test.cc
+-rw-r--r--   0 runner     (501) staff       (20)      741 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/search/search.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-07-10 05:40:17.578206 stim-1.9.0/src/stim/simulators/
+-rw-r--r--   0 runner     (501) staff       (20)     8303 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/simulators/detection_simulator.cc
+-rw-r--r--   0 runner     (501) staff       (20)     3491 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/simulators/detection_simulator.h
+-rw-r--r--   0 runner     (501) staff       (20)    13068 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/simulators/detection_simulator.test.cc
+-rw-r--r--   0 runner     (501) staff       (20)    58776 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/simulators/error_analyzer.cc
+-rw-r--r--   0 runner     (501) staff       (20)    19400 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/simulators/error_analyzer.h
+-rw-r--r--   0 runner     (501) staff       (20)     2487 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/simulators/error_analyzer.perf.cc
+-rw-r--r--   0 runner     (501) staff       (20)    93794 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/simulators/error_analyzer.test.cc
+-rw-r--r--   0 runner     (501) staff       (20)    13244 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/simulators/error_matcher.cc
+-rw-r--r--   0 runner     (501) staff       (20)     4113 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/simulators/error_matcher.h
+-rw-r--r--   0 runner     (501) staff       (20)    12959 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/simulators/error_matcher.test.cc
+-rw-r--r--   0 runner     (501) staff       (20)    22561 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/simulators/frame_simulator.cc
+-rw-r--r--   0 runner     (501) staff       (20)     6766 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/simulators/frame_simulator.h
+-rw-r--r--   0 runner     (501) staff       (20)     3090 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/simulators/frame_simulator.perf.cc
+-rw-r--r--   0 runner     (501) staff       (20)    35644 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/simulators/frame_simulator.test.cc
+-rw-r--r--   0 runner     (501) staff       (20)    14238 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/simulators/matched_error.cc
+-rw-r--r--   0 runner     (501) staff       (20)     7006 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/simulators/matched_error.h
+-rw-r--r--   0 runner     (501) staff       (20)    23934 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/simulators/matched_error.pybind.cc
+-rw-r--r--   0 runner     (501) staff       (20)      774 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/simulators/matched_error.pybind.h
+-rw-r--r--   0 runner     (501) staff       (20)     8918 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/simulators/matched_error.test.cc
+-rw-r--r--   0 runner     (501) staff       (20)    12594 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/simulators/measurements_to_detection_events.cc
+-rw-r--r--   0 runner     (501) staff       (20)     5802 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/simulators/measurements_to_detection_events.h
+-rw-r--r--   0 runner     (501) staff       (20)    17724 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/simulators/measurements_to_detection_events.pybind.cc
+-rw-r--r--   0 runner     (501) staff       (20)     2894 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/simulators/measurements_to_detection_events.pybind.h
+-rw-r--r--   0 runner     (501) staff       (20)    17916 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/simulators/measurements_to_detection_events.test.cc
+-rw-r--r--   0 runner     (501) staff       (20)    38340 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/simulators/tableau_simulator.cc
+-rw-r--r--   0 runner     (501) staff       (20)    14965 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/simulators/tableau_simulator.h
+-rw-r--r--   0 runner     (501) staff       (20)     1192 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/simulators/tableau_simulator.perf.cc
+-rw-r--r--   0 runner     (501) staff       (20)    56623 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/simulators/tableau_simulator.pybind.cc
+-rw-r--r--   0 runner     (501) staff       (20)     1014 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/simulators/tableau_simulator.pybind.h
+-rw-r--r--   0 runner     (501) staff       (20)    65265 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/simulators/tableau_simulator.test.cc
+-rw-r--r--   0 runner     (501) staff       (20)     8122 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/simulators/vector_simulator.cc
+-rw-r--r--   0 runner     (501) staff       (20)     3151 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/simulators/vector_simulator.h
+-rw-r--r--   0 runner     (501) staff       (20)     9602 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/simulators/vector_simulator.test.cc
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-07-10 05:40:17.586562 stim-1.9.0/src/stim/stabilizers/
+-rw-r--r--   0 runner     (501) staff       (20)     4476 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/stabilizers/pauli_string.cc
+-rw-r--r--   0 runner     (501) staff       (20)     4282 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/stabilizers/pauli_string.h
+-rw-r--r--   0 runner     (501) staff       (20)     1513 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/stabilizers/pauli_string.perf.cc
+-rw-r--r--   0 runner     (501) staff       (20)    30578 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/stabilizers/pauli_string.pybind.cc
+-rw-r--r--   0 runner     (501) staff       (20)     1991 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/stabilizers/pauli_string.pybind.h
+-rw-r--r--   0 runner     (501) staff       (20)    11945 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/stabilizers/pauli_string.test.cc
+-rw-r--r--   0 runner     (501) staff       (20)     4715 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/stabilizers/pauli_string_ref.cc
+-rw-r--r--   0 runner     (501) staff       (20)     5004 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/stabilizers/pauli_string_ref.h
+-rw-r--r--   0 runner     (501) staff       (20)    22011 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/stabilizers/tableau.cc
+-rw-r--r--   0 runner     (501) staff       (20)     8555 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/stabilizers/tableau.h
+-rw-r--r--   0 runner     (501) staff       (20)     1599 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/stabilizers/tableau.perf.cc
+-rw-r--r--   0 runner     (501) staff       (20)    41497 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/stabilizers/tableau.pybind.cc
+-rw-r--r--   0 runner     (501) staff       (20)      757 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/stabilizers/tableau.pybind.h
+-rw-r--r--   0 runner     (501) staff       (20)    42286 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/stabilizers/tableau.test.cc
+-rw-r--r--   0 runner     (501) staff       (20)     5334 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/stabilizers/tableau_specialized_prepend.cc
+-rw-r--r--   0 runner     (501) staff       (20)     4495 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/stabilizers/tableau_transposed_raii.cc
+-rw-r--r--   0 runner     (501) staff       (20)     1925 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/stabilizers/tableau_transposed_raii.h
+-rw-r--r--   0 runner     (501) staff       (20)     1601 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/str_util.h
+-rw-r--r--   0 runner     (501) staff       (20)     1076 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/str_util.test.cc
+-rw-r--r--   0 runner     (501) staff       (20)     1641 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/test_util.test.cc
+-rw-r--r--   0 runner     (501) staff       (20)      957 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim/test_util.test.h
+-rw-r--r--   0 runner     (501) staff       (20)      614 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim.cc
+-rw-r--r--   0 runner     (501) staff       (20)     2329 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim.h
+-rw-r--r--   0 runner     (501) staff       (20)      925 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim.test.cc
+-rw-r--r--   0 runner     (501) staff       (20)      798 2022-07-10 05:17:41.000000 stim-1.9.0/src/stim_included_twice.test.cc
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-07-10 05:40:17.589162 stim-1.9.0/stim.egg-info/
+-rw-r--r--   0 runner     (501) staff       (20)     4196 2022-07-10 05:40:17.000000 stim-1.9.0/stim.egg-info/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)     8665 2022-07-10 05:40:17.000000 stim-1.9.0/stim.egg-info/SOURCES.txt
+-rw-r--r--   0 runner     (501) staff       (20)        1 2022-07-10 05:40:17.000000 stim-1.9.0/stim.egg-info/dependency_links.txt
+-rw-r--r--   0 runner     (501) staff       (20)       52 2022-07-10 05:40:17.000000 stim-1.9.0/stim.egg-info/entry_points.txt
+-rw-r--r--   0 runner     (501) staff       (20)        6 2022-07-10 05:40:17.000000 stim-1.9.0/stim.egg-info/requires.txt
+-rw-r--r--   0 runner     (501) staff       (20)        5 2022-07-10 05:40:17.000000 stim-1.9.0/stim.egg-info/top_level.txt
```

### Comparing `stim-1.8.0/LICENSE` & `stim-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `stim-1.8.0/PKG-INFO` & `stim-1.9.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: stim
-Version: 1.8.0
-Summary: A fast quantum stabilizer circuit simulator.
+Version: 1.9.0
+Summary: A fast library for analyzing with quantum stabilizer circuits.
 Home-page: https://github.com/quantumlib/stim
 Author: Craig Gidney
 Author-email: craig.gidney@gmail.com
 License: Apache 2
 Platform: UNKNOWN
 Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown
```

### Comparing `stim-1.8.0/README.md` & `stim-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `stim-1.8.0/glue/python/README.md` & `stim-1.9.0/glue/python/README.md`

 * *Files identical despite different names*

### Comparing `stim-1.8.0/setup.py` & `stim-1.9.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,88 +9,106 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from setuptools import setup, Extension
-import pybind11
 import glob
+import pybind11
 
 ALL_SOURCE_FILES = glob.glob("src/**/*.cc", recursive=True)
+MUX_SOURCE_FILES = glob.glob("src/**/march.pybind.cc", recursive=True)
 TEST_FILES = glob.glob("src/**/*.test.cc", recursive=True)
 PERF_FILES = glob.glob("src/**/*.perf.cc", recursive=True)
 MAIN_FILES = glob.glob("src/**/main.cc", recursive=True)
 HEADER_FILES = glob.glob("src/**/*.h", recursive=True)
-RELEVANT_SOURCE_FILES = sorted(set(ALL_SOURCE_FILES) - set(TEST_FILES + PERF_FILES + MAIN_FILES))
+RELEVANT_SOURCE_FILES = sorted(set(ALL_SOURCE_FILES) - set(TEST_FILES + PERF_FILES + MAIN_FILES + MUX_SOURCE_FILES))
 
-version = '1.8.0'
+version = '1.9.0'
 
 common_compile_args = [
     '-std=c++11',
     '-fno-strict-aliasing',
     '-O3',
     '-g0',
     f'-DVERSION_INFO={version}',
 ]
+stim_detect_machine_architecture = Extension(
+    'stim._detect_machine_architecture',
+    sources=MUX_SOURCE_FILES,
+    include_dirs=[pybind11.get_include(), "src"],
+    language='c++',
+    extra_compile_args=[
+        *common_compile_args,
+        '-mno-sse2',
+        '-mno-avx2',
+    ],
+)
 stim_polyfill = Extension(
-    'stim._stim_march_polyfill',
+    'stim._stim_polyfill',
     sources=RELEVANT_SOURCE_FILES,
-    headers=HEADER_FILES,
     include_dirs=[pybind11.get_include(), "src"],
     language='c++',
     extra_compile_args=[
         *common_compile_args,
         # I would specify -mno-sse2 but that causes build failures in non-stim code...?
         '-mno-avx2',
-        '-DSTIM_PYBIND11_MODULE_NAME=_stim_march_polyfill',
+        '-DSTIM_PYBIND11_MODULE_NAME=_stim_polyfill',
     ],
 )
 stim_sse2 = Extension(
-    'stim._stim_march_sse2',
+    'stim._stim_sse2',
     sources=RELEVANT_SOURCE_FILES,
-    headers=HEADER_FILES,
     include_dirs=[pybind11.get_include(), "src"],
     language='c++',
     extra_compile_args=[
         *common_compile_args,
         '-msse2',
         '-mno-avx2',
-        '-DSTIM_PYBIND11_MODULE_NAME=_stim_march_sse2',
+        '-DSTIM_PYBIND11_MODULE_NAME=_stim_sse2',
     ],
 )
 stim_avx2 = Extension(
-    'stim._stim_march_avx2',
+    'stim._stim_avx2',
     sources=RELEVANT_SOURCE_FILES,
-    headers=HEADER_FILES,
     include_dirs=[pybind11.get_include(), "src"],
     language='c++',
     extra_compile_args=[
         *common_compile_args,
         '-msse2',
         '-mavx2',
-        '-DSTIM_PYBIND11_MODULE_NAME=_stim_march_avx2',
+        '-DSTIM_PYBIND11_MODULE_NAME=_stim_avx2',
     ],
 )
 
-with open('glue/python/README.md') as f:
+with open('glue/python/README.md', encoding='UTF-8') as f:
     long_description = f.read()
 
 setup(
     name='stim',
     version=version,
     author='Craig Gidney',
     author_email='craig.gidney@gmail.com',
     url='https://github.com/quantumlib/stim',
     license='Apache 2',
-    description='A fast quantum stabilizer circuit simulator.',
+    description='A fast library for analyzing with quantum stabilizer circuits.',
     long_description=long_description,
     long_description_content_type='text/markdown',
-    ext_modules=[stim_polyfill, stim_sse2, stim_avx2],
+    ext_modules=[
+        stim_detect_machine_architecture,
+        stim_polyfill,
+        stim_sse2,
+        stim_avx2,
+    ],
     python_requires='>=3.6.0',
-    data_files=[('', ['glue/python/README.md', 'pyproject.toml'])],
     packages=['stim'],
     package_dir={'stim': 'glue/python/src/stim'},
+    package_data={'': [*HEADER_FILES, 'glue/python/src/stim/__init__.pyi', 'glue/python/README.md', 'pyproject.toml']},
+    include_package_data=True,
     install_requires=['numpy'],
+    entry_points={
+        'console_scripts': ['stim=stim._main_argv:main_argv'],
+    },
     # Needed on Windows to avoid the default `build` colliding with Bazel's `BUILD`.
     options={'build': {'build_base': 'python_build_stim'}},
 )
```

### Comparing `stim-1.8.0/src/stim/arg_parse.cc` & `stim-1.9.0/src/stim/arg_parse.cc`

 * *Files identical despite different names*

### Comparing `stim-1.8.0/src/stim/circuit/circuit.cc` & `stim-1.9.0/src/stim/circuit/circuit.cc`

 * *Files 3% similar despite different names*

```diff
@@ -780,23 +780,50 @@
     }
 
     Circuit result;
     result.append_repeat_block(repetitions, *this);
     return result;
 }
 
+template <typename T>
+ConstPointerRange<T> mono_extend(
+    MonotonicBuffer<T> &cur, ConstPointerRange<T> original, ConstPointerRange<T> additional) {
+    if (original.ptr_end == cur.tail.ptr_start) {
+        // Try to append new data right after the original data.
+        cur.ensure_available(additional.size());
+        if (original.ptr_end == cur.tail.ptr_start) {
+            cur.append_tail(additional);
+            auto added = cur.commit_tail();
+            return {original.ptr_start, added.ptr_end};
+        }
+    }
+
+    // Ensure necessary space is available, plus some padding to avoid quadratic behavior when repeatedly extending.
+    cur.ensure_available((int)(1.1 * (original.size() + additional.size())) + 10);
+    cur.append_tail(original);
+    cur.append_tail(additional);
+    return cur.commit_tail();
+}
+
 Circuit &Circuit::operator+=(const Circuit &other) {
+    ConstPointerRange<Operation> ops_to_add = other.operations;
+    if (!operations.empty() && !ops_to_add.empty() && operations.back().can_fuse(ops_to_add[0])) {
+        operations.back().target_data.targets =
+            mono_extend(target_buf, operations.back().target_data.targets, ops_to_add[0].target_data.targets);
+        ops_to_add.ptr_start++;
+    }
+
     if (&other == this) {
-        operations.insert(operations.end(), operations.begin(), operations.end());
+        operations.insert(operations.end(), ops_to_add.begin(), ops_to_add.end());
         return *this;
     }
 
     uint32_t block_offset = (uint32_t)blocks.size();
     blocks.insert(blocks.end(), other.blocks.begin(), other.blocks.end());
-    for (const auto &op : other.operations) {
+    for (const auto &op : ops_to_add) {
         assert(op.gate != nullptr);
         auto target_data = append_operation(op);
         if (op.gate->id == gate_name_to_id("REPEAT")) {
             assert(op.target_data.targets.size() == 3);
             target_data[0].data += block_offset;
         }
     }
@@ -1028,14 +1055,73 @@
     }
     for (const auto &block : blocks) {
         result.blocks.push_back(block.aliased_noiseless_circuit());
     }
     return result;
 }
 
+Circuit Circuit::without_noise() const {
+    Circuit result;
+    for (const auto &op : operations) {
+        if (op.gate->flags & GATE_PRODUCES_NOISY_RESULTS) {
+            // Drop result flip probabilities.
+            result.operations.push_back(Operation{op.gate, {{}, result.target_buf.take_copy(op.target_data.targets)}});
+        } else if (!(op.gate->flags & GATE_IS_NOISE)) {
+            // Keep noiseless operations.
+            result.operations.push_back(Operation{
+                op.gate,
+                {result.arg_buf.take_copy(op.target_data.args), result.target_buf.take_copy(op.target_data.targets)}});
+        }
+    }
+    for (const auto &block : blocks) {
+        result.blocks.push_back(block.without_noise());
+    }
+    return result;
+}
+
+void flattened_helper(const Circuit &body, std::vector<double> &cur_coordinate_shift, Circuit &out) {
+    const uint8_t shift = gate_name_to_id("SHIFT_COORDS");
+    const uint8_t rep = gate_name_to_id("REPEAT");
+    const uint8_t qubit_coords = gate_name_to_id("QUBIT_COORDS");
+    const uint8_t detector = gate_name_to_id("DETECTOR");
+    for (const auto &op : body.operations) {
+        uint8_t id = op.gate->id;
+        if (id == shift) {
+            while (cur_coordinate_shift.size() < op.target_data.args.size()) {
+                cur_coordinate_shift.push_back(0);
+            }
+            for (size_t k = 0; k < op.target_data.args.size(); k++) {
+                cur_coordinate_shift[k] += op.target_data.args[k];
+            }
+        } else if (id == rep) {
+            uint64_t reps = op_data_rep_count(op.target_data);
+            const auto &loop_body = op_data_block_body(body, op.target_data);
+            for (uint64_t k = 0; k < reps; k++) {
+                flattened_helper(loop_body, cur_coordinate_shift, out);
+            }
+        } else {
+            auto t = out.target_buf.take_copy(op.target_data.targets);
+            auto a = out.arg_buf.take_copy(op.target_data.args);
+            if (id == qubit_coords || op.gate->id == detector) {
+                for (size_t k = 0; k < a.size() && k < cur_coordinate_shift.size(); k++) {
+                    a[k] += cur_coordinate_shift[k];
+                }
+            }
+            out.operations.push_back({op.gate, {a, t}});
+        }
+    }
+}
+
+Circuit Circuit::flattened() const {
+    Circuit result;
+    std::vector<double> shift;
+    flattened_helper(*this, shift, result);
+    return result;
+}
+
 void stim::vec_pad_add_mul(std::vector<double> &target, ConstPointerRange<double> offset, uint64_t mul) {
     while (target.size() < offset.size()) {
         target.push_back(0);
     }
     for (size_t k = 0; k < offset.size(); k++) {
         target[k] += offset[k] * mul;
     }
@@ -1124,28 +1210,28 @@
     std::set<uint64_t>::const_iterator &iter_desired_detector_index,
     const std::vector<double> &initial_coord_shift,
     uint64_t &next_detector_index,
     std::map<uint64_t, std::vector<double>> &out) {
     if (iter_desired_detector_index == included_detector_indices.end()) {
         return;
     }
-    uint64_t desired_detector_index = *iter_desired_detector_index;
 
     std::vector<double> coord_shift = initial_coord_shift;
     for (const auto &op : circuit.operations) {
         if (op.gate->id == gate_name_to_id("SHIFT_COORDS")) {
             vec_pad_add_mul(coord_shift, op.target_data.args);
         } else if (op.gate->id == gate_name_to_id("REPEAT")) {
             const auto &block = op_data_block_body(circuit, op.target_data);
             auto block_shift = block.final_coord_shift();
             uint64_t per = block.count_detectors();
             uint64_t reps = op_data_rep_count(op.target_data);
             uint64_t used_reps = 0;
             while (used_reps < reps) {
-                uint64_t skip = per == 0 ? reps : std::min(reps, (desired_detector_index - next_detector_index) / per);
+                uint64_t skip =
+                    per == 0 ? reps : std::min(reps, (*iter_desired_detector_index - next_detector_index) / per);
                 used_reps += skip;
                 next_detector_index += per * skip;
                 vec_pad_add_mul(coord_shift, block_shift, skip);
                 if (used_reps < reps) {
                     get_detector_coordinates_helper(
                         block,
                         included_detector_indices,
@@ -1154,33 +1240,31 @@
                         next_detector_index,
                         out);
                     used_reps += 1;
                     vec_pad_add_mul(coord_shift, block_shift);
                     if (iter_desired_detector_index == included_detector_indices.end()) {
                         return;
                     }
-                    desired_detector_index = *iter_desired_detector_index;
                 }
             }
         } else if (op.gate->id == gate_name_to_id("DETECTOR")) {
-            if (next_detector_index == desired_detector_index) {
+            if (next_detector_index == *iter_desired_detector_index) {
                 std::vector<double> det_coords;
                 for (size_t k = 0; k < op.target_data.args.size(); k++) {
                     det_coords.push_back(op.target_data.args[k]);
                     if (k < coord_shift.size()) {
                         det_coords[k] += coord_shift[k];
                     }
                 }
                 out[next_detector_index] = det_coords;
 
                 iter_desired_detector_index++;
                 if (iter_desired_detector_index == included_detector_indices.end()) {
                     return;
                 }
-                desired_detector_index = *iter_desired_detector_index;
             }
             next_detector_index++;
         }
     }
 }
 
 std::vector<double> Circuit::coords_of_detector(uint64_t detector_index) const {
```

### Comparing `stim-1.8.0/src/stim/circuit/circuit.pybind.cc` & `stim-1.9.0/src/stim/circuit/circuit.pybind.cc`

 * *Files 12% similar despite different names*

```diff
@@ -10,31 +10,35 @@
 // distributed under the License is distributed on an "AS IS" BASIS,
 // WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 // See the License for the specific language governing permissions and
 // limitations under the License.
 
 #include "stim/circuit/circuit.pybind.h"
 
+#include <fstream>
+
 #include "stim/circuit/circuit_gate_target.pybind.h"
 #include "stim/circuit/circuit_instruction.pybind.h"
 #include "stim/circuit/circuit_repeat_block.pybind.h"
 #include "stim/dem/detector_error_model_target.pybind.h"
 #include "stim/gen/circuit_gen_params.h"
 #include "stim/gen/gen_color_code.h"
 #include "stim/gen/gen_rep_code.h"
 #include "stim/gen/gen_surface_code.h"
+#include "stim/io/raii_file.h"
 #include "stim/py/base.pybind.h"
 #include "stim/py/compiled_detector_sampler.pybind.h"
 #include "stim/py/compiled_measurement_sampler.pybind.h"
+#include "stim/search/search.h"
 #include "stim/simulators/error_analyzer.h"
 #include "stim/simulators/error_matcher.h"
 #include "stim/simulators/measurements_to_detection_events.pybind.h"
-#include "stim/simulators/min_distance.h"
 
 using namespace stim;
+using namespace stim_pybind;
 
 std::string circuit_repr(const Circuit &self) {
     if (self.operations.empty()) {
         return "stim.Circuit()";
     }
     std::stringstream ss;
     ss << "stim.Circuit('''\n";
@@ -42,19 +46,34 @@
     ss << "\n''')";
     return ss.str();
 }
 
 std::vector<ExplainedError> circuit_shortest_graphlike_error(
     const Circuit &self, bool ignore_ungraphlike_errors, bool reduce_to_representative) {
     DetectorErrorModel dem =
-        ErrorAnalyzer::circuit_to_detector_error_model(self, !ignore_ungraphlike_errors, true, false, 1);
+        ErrorAnalyzer::circuit_to_detector_error_model(self, !ignore_ungraphlike_errors, true, false, 1, false, false);
     DetectorErrorModel filter = shortest_graphlike_undetectable_logical_error(dem, ignore_ungraphlike_errors);
     return ErrorMatcher::explain_errors_from_circuit(self, &filter, reduce_to_representative);
 }
 
+std::vector<ExplainedError> py_find_undetectable_logical_error(
+    const Circuit &self,
+    size_t dont_explore_detection_event_sets_with_size_above,
+    size_t dont_explore_edges_with_degree_above,
+    bool dont_explore_edges_increasing_symptom_degree,
+    bool reduce_to_representative) {
+    DetectorErrorModel dem = ErrorAnalyzer::circuit_to_detector_error_model(self, false, true, false, 1, false, false);
+    DetectorErrorModel filter = stim::find_undetectable_logical_error(
+        dem,
+        dont_explore_detection_event_sets_with_size_above,
+        dont_explore_edges_with_degree_above,
+        dont_explore_edges_increasing_symptom_degree);
+    return ErrorMatcher::explain_errors_from_circuit(self, &filter, reduce_to_representative);
+}
+
 void circuit_append(
     Circuit &self,
     const pybind11::object &obj,
     const pybind11::object &targets,
     const pybind11::object &arg,
     bool backwards_compat) {
     // Extract single target or list of targets.
@@ -124,33 +143,32 @@
     circuit_append(self, obj, targets, arg, false);
 }
 
 pybind11::class_<Circuit> pybind_circuit(pybind11::module &m) {
     auto c = pybind11::class_<Circuit>(
         m,
         "Circuit",
-        pybind11::module_local(),
         clean_doc_string(u8R"DOC(
             A mutable stabilizer circuit.
 
             Examples:
                 >>> import stim
                 >>> c = stim.Circuit()
                 >>> c.append("X", 0)
                 >>> c.append("M", 0)
                 >>> c.compile_sampler().sample(shots=1)
-                array([[1]], dtype=uint8)
+                array([[ True]])
 
                 >>> stim.Circuit('''
                 ...    H 0
                 ...    CNOT 0 1
                 ...    M 0 1
                 ...    DETECTOR rec[-1] rec[-2]
                 ... ''').compile_detector_sampler().sample(shots=1)
-                array([[0]], dtype=uint8)
+                array([[False]])
 
         )DOC")
             .data());
 
     pybind_circuit_repeat_block(m);
     pybind_circuit_gate_target(m);
     pybind_circuit_instruction(m);
@@ -332,15 +350,15 @@
                 >>> import stim
                 >>> c = stim.Circuit('''
                 ...    X 2
                 ...    M 0 1 2
                 ... ''')
                 >>> s = c.compile_sampler()
                 >>> s.sample(shots=1)
-                array([[0, 0, 1]], dtype=uint8)
+                array([[False, False,  True]])
         )DOC")
             .data());
 
     c.def(
         "compile_m2d_converter",
         &py_init_compiled_measurements_to_detection_events_converter,
         pybind11::kw_only(),
@@ -417,15 +435,15 @@
                 ...    H 0
                 ...    CNOT 0 1
                 ...    M 0 1
                 ...    DETECTOR rec[-1] rec[-2]
                 ... ''')
                 >>> s = c.compile_detector_sampler()
                 >>> s.sample(shots=1)
-                array([[0]], dtype=uint8)
+                array([[False]])
         )DOC")
             .data());
 
     c.def(
         "clear",
         &Circuit::clear,
         clean_doc_string(u8R"DOC(
@@ -469,43 +487,32 @@
                     } else {
                         targets.append(pybind11::int_(v));
                     }
                 }
                 for (auto t : op.target_data.args) {
                     args.append(t);
                 }
-                if (op.target_data.args.size() == 0) {
+                if (op.target_data.args.empty()) {
                     // Backwards compatibility.
                     result.append(pybind11::make_tuple(op.gate->name, targets, 0));
                 } else if (op.target_data.args.size() == 1) {
                     // Backwards compatibility.
                     result.append(pybind11::make_tuple(op.gate->name, targets, op.target_data.args[0]));
                 } else {
                     result.append(pybind11::make_tuple(op.gate->name, targets, args));
                 }
             });
             return result;
         },
         clean_doc_string(u8R"DOC(
-            Flattens the circuit's operations into a list.
+            [DEPRECATED]
 
-            The operations within repeat blocks are actually repeated in the output.
-
-            Returns:
-                A List[Tuple[name, targets, arg]] of the operations in the circuit.
-                    name: A string with the gate's name.
-                    targets: A list of things acted on by the gate. Each thing can be:
-                        int: The index of a qubit.
-                        Tuple["inv", int]: The index of a qubit to measure with an inverted result.
-                        Tuple["rec", int]: A measurement record target like `rec[-1]`.
-                        Tuple["X", int]: A Pauli X operation to apply during a correlated error.
-                        Tuple["Y", int]: A Pauli Y operation to apply during a correlated error.
-                        Tuple["Z", int]: A Pauli Z operation to apply during a correlated error.
-                    arg: The gate's numeric argument. For most gates this is just 0. For noisy
-                        gates this is the probability of the noise being applied.
+            Returns a list of tuples encoding the contents of the circuit.
+            Instead of this method, use `for instruction in circuit` or, to
+            avoid REPEAT blocks, `for instruction in circuit.flattened()`.
 
             Examples:
                 >>> import stim
                 >>> stim.Circuit('''
                 ...    H 0
                 ...    X_ERROR(0.125) 1
                 ...    M 0 !1
@@ -666,16 +673,19 @@
     for (size_t k = 0; k < 2; k++) {
         c.def(
             k == 0 ? "append_operation" : "append",
             k == 0 ? &circuit_append_backwards_compat : &circuit_append_strict,
             pybind11::arg("name"),
             pybind11::arg("targets") = pybind11::make_tuple(),
             pybind11::arg("arg") = pybind11::none(),
-            clean_doc_string(u8R"DOC(
+            k == 0 ? "[DEPRECATED] use stim.Circuit.append instead"
+                   : clean_doc_string(u8R"DOC(
                 Appends an operation into the circuit.
+                @overload def append(self, name: str, targets: Union[int, stim.GateTarget, Iterable[Union[int, stim.GateTarget]]], arg: Union[float, Iterable[float]]) -> None:
+                @overload def append(self, name: Union[stim.CircuitOperation, stim.CircuitRepeatBlock]) -> None:
 
                 Note: `stim.Circuit.append_operation` is an alias of `stim.Circuit.append`.
 
                 Examples:
                     >>> import stim
                     >>> c = stim.Circuit()
                     >>> c.append("X", 0)
@@ -711,15 +721,15 @@
                         example, X_ERROR takes a probability, OBSERVABLE_INCLUDE takes an observable index, and
                         PAULI_CHANNEL_1 takes three disjoint probabilities.
 
                         Note: Defaults to no parens arguments. Except, for backwards compatibility reasons,
                         `cirq.append_operation` (but not `cirq.append`) will default to a single 0.0 argument for gates
                         that take exactly one argument.
             )DOC")
-                .data());
+                         .data());
     }
 
     c.def(
         "append_from_stim_program_text",
         [](Circuit &self, const char *text) {
             self.append_from_text(text);
         },
@@ -740,15 +750,15 @@
                 >>> print(c)
                 H 0
                 CX 0 2
                 M 2
                 CX rec[-1] 1
 
             Args:
-                text: The STIM program text containing the circuit operations to append.
+                stim_program_text: The STIM program text containing the circuit operations to append.
         )DOC")
             .data());
 
     c.def(
         "__str__",
         &Circuit::str,
         "Returns stim instructions (that can be saved to a file and parsed by stim) for the current circuit.");
@@ -905,14 +915,142 @@
                 DETECTOR(1, 1) rec[-3] rec[-4] rec[-7]
                 DETECTOR(3, 1) rec[-2] rec[-3] rec[-6]
                 DETECTOR(5, 1) rec[-1] rec[-2] rec[-5]
                 OBSERVABLE_INCLUDE(0) rec[-1]
         )DOC")
             .data());
 
+    c.def_static(
+        "from_file",
+        [](pybind11::object &obj) {
+            try {
+                auto path = pybind11::cast<std::string>(obj);
+                RaiiFile f(path.data(), "r");
+                return Circuit::from_file(f.f);
+            } catch (pybind11::cast_error &ex) {
+            }
+
+            auto py_path = pybind11::module::import("pathlib").attr("Path");
+            if (pybind11::isinstance(obj, py_path)) {
+                auto path = pybind11::cast<std::string>(pybind11::str(obj));
+                RaiiFile f(path.data(), "r");
+                return Circuit::from_file(f.f);
+            }
+
+            auto py_text_io_base = pybind11::module::import("io").attr("TextIOBase");
+            if (pybind11::isinstance(obj, py_text_io_base)) {
+                auto contents = obj.attr("read")();
+                return Circuit(pybind11::cast<std::string>(pybind11::str(contents)).data());
+            }
+
+            throw std::invalid_argument(
+                "Don't know how to read from " + pybind11::cast<std::string>(pybind11::str(obj)));
+        },
+        pybind11::arg("file"),
+        clean_doc_string(u8R"DOC(
+            Args:
+                file: A file path or open file object to read from.
+
+            Returns:
+                The circuit parsed from the file.
+
+            Examples:
+                >>> import stim
+                >>> import tempfile
+
+                >>> with tempfile.TemporaryDirectory() as tmpdir:
+                ...     path = tmpdir + '/tmp.stim'
+                ...     with open(path, 'w') as f:
+                ...         print('H 5', file=f)
+                ...     circuit = stim.Circuit.from_file(path)
+                >>> circuit
+                stim.Circuit('''
+                    H 5
+                ''')
+
+                >>> with tempfile.TemporaryDirectory() as tmpdir:
+                ...     path = tmpdir + '/tmp.stim'
+                ...     with open(path, 'w') as f:
+                ...         print('CNOT 4 5', file=f)
+                ...     with open(path) as f:
+                ...         circuit = stim.Circuit.from_file(path)
+                >>> circuit
+                stim.Circuit('''
+                    CX 4 5
+                ''')
+        )DOC")
+            .data());
+
+    c.def(
+        "to_file",
+        [](const Circuit &self, pybind11::object &obj) {
+            try {
+                auto path = pybind11::cast<std::string>(obj);
+                std::ofstream out(path, std::ofstream::out);
+                if (!out.is_open()) {
+                    throw std::invalid_argument("Failed to open " + path);
+                }
+                out << self << '\n';
+                return;
+            } catch (pybind11::cast_error &ex) {
+            }
+
+            auto py_path = pybind11::module::import("pathlib").attr("Path");
+            if (pybind11::isinstance(obj, py_path)) {
+                auto path = pybind11::cast<std::string>(pybind11::str(obj));
+                std::ofstream out(path, std::ofstream::out);
+                if (!out.is_open()) {
+                    throw std::invalid_argument("Failed to open " + path);
+                }
+                out << self << '\n';
+                return;
+            }
+
+            auto py_text_io_base = pybind11::module::import("io").attr("TextIOBase");
+            if (pybind11::isinstance(obj, py_text_io_base)) {
+                obj.attr("write")(pybind11::str(self.str()));
+                obj.attr("write")(pybind11::str("\n"));
+                return;
+            }
+
+            throw std::invalid_argument(
+                "Don't know how to write to " + pybind11::cast<std::string>(pybind11::str(obj)));
+        },
+        pybind11::arg("file"),
+        clean_doc_string(u8R"DOC(
+            @signature def to_file(self, file: Union[io.TextIOBase, str, pathlib.Path]) -> None:
+            Writes the stim circuit to a file.
+
+            Args:
+                file: A file path or an open file to write to.
+
+            Examples:
+                >>> import stim
+                >>> import tempfile
+                >>> c = stim.Circuit('H 5\nX 0')
+
+                >>> with tempfile.TemporaryDirectory() as tmpdir:
+                ...     path = tmpdir + '/tmp.stim'
+                ...     with open(path, 'w') as f:
+                ...         c.to_file(f)
+                ...     with open(path) as f:
+                ...         contents = f.read()
+                >>> contents
+                'H 5\nX 0\n'
+
+                >>> with tempfile.TemporaryDirectory() as tmpdir:
+                ...     path = tmpdir + '/tmp.stim'
+                ...     c.to_file(path)
+                ...     with open(path) as f:
+                ...         contents = f.read()
+                >>> contents
+                'H 5\nX 0\n'
+        )DOC")
+            .data());
+
     c.def(
         "__len__",
         [](const Circuit &self) {
             return self.operations.size();
         },
         clean_doc_string(u8R"DOC(
             Returns the number of top-level instructions and blocks in the circuit.
@@ -963,19 +1101,25 @@
                 args.push_back(e);
             }
             return pybind11::cast(CircuitInstruction(*op.gate, targets, args));
         },
         pybind11::arg("index_or_slice"),
         clean_doc_string(u8R"DOC(
             Returns copies of instructions from the circuit.
+            @overload def __getitem__(self, index_or_slice: int) -> Union[stim.CircuitInstruction, stim.CircuitRepeatBlock]:
+            @overload def __getitem__(self, index_or_slice: slice) -> stim.Circuit:
 
             Args:
                 index_or_slice: An integer index picking out an instruction to return, or a slice picking out a range
                     of instructions to return as a circuit.
 
+            Returns:
+                If the index was an integer, then an instruction from the circuit.
+                If the index was a slice, then a circuit made up of the instructions in that slice.
+
             Examples:
                 >>> import stim
                 >>> circuit = stim.Circuit('''
                 ...    X 0
                 ...    X_ERROR(0.5) 1 2
                 ...    REPEAT 100 {
                 ...        X 0
@@ -1003,23 +1147,33 @@
 
     c.def(
         "detector_error_model",
         [](const Circuit &self,
            bool decompose_errors,
            bool flatten_loops,
            bool allow_gauge_detectors,
-           double approximate_disjoint_errors) -> DetectorErrorModel {
+           double approximate_disjoint_errors,
+           bool ignore_decomposition_failures,
+           bool block_decomposition_from_introducing_remnant_edges) -> DetectorErrorModel {
             return ErrorAnalyzer::circuit_to_detector_error_model(
-                self, decompose_errors, !flatten_loops, allow_gauge_detectors, approximate_disjoint_errors);
+                self,
+                decompose_errors,
+                !flatten_loops,
+                allow_gauge_detectors,
+                approximate_disjoint_errors,
+                ignore_decomposition_failures,
+                block_decomposition_from_introducing_remnant_edges);
         },
         pybind11::kw_only(),
         pybind11::arg("decompose_errors") = false,
         pybind11::arg("flatten_loops") = false,
         pybind11::arg("allow_gauge_detectors") = false,
         pybind11::arg("approximate_disjoint_errors") = false,
+        pybind11::arg("ignore_decomposition_failures") = false,
+        pybind11::arg("block_decomposition_from_introducing_remnant_edges") = false,
         clean_doc_string(u8R"DOC(
             Returns a stim.DetectorErrorModel describing the error processes in the circuit.
 
             Args:
                 decompose_errors: Defaults to false. When set to true, the error analysis attempts to decompose the
                     components of composite error mechanisms (such as depolarization errors) into simpler errors, and
                     suggest this decomposition via `stim.target_separator()` between the components. For example, in an
@@ -1047,14 +1201,33 @@
                     probabilities. For example, a ``PAULI_CHANNEL_1(0.1, 0.2, 0.0)` becomes equivalent to an
                     `X_ERROR(0.1)` followed by a `Z_ERROR(0.2)`. This assumption is an approximation, but it is a good
                     approximation for small probabilities.
 
                     This argument can also be set to a probability between 0 and 1, setting a threshold below which the
                     approximation is acceptable. Any error mechanisms that have a component probability above the
                     threshold will cause an exception to be thrown.
+                ignore_decomposition_failures: Defaults to False.
+                    When this is set to True, circuit errors that fail to decompose into graphlike
+                    detector error model errors no longer cause the conversion process to abort.
+                    Instead, the undecomposed error is inserted into the output. Whatever tool
+                    the detector error model is then given to is responsible for dealing with the
+                    undecomposed errors (e.g. a tool may choose to simply ignore them).
+
+                    Irrelevant unless decompose_errors=True.
+                block_decomposition_from_introducing_remnant_edges: Defaults to False.
+                    Requires that both A B and C D be present elsewhere in the detector error model
+                    in order to decompose A B C D into A B ^ C D. Normally, only one of A B or C D
+                    needs to appear to allow this decomposition.
+
+                    Remnant edges can be a useful feature for ensuring decomposition succeeds, but
+                    they can also reduce the effective code distance by giving the decoder single
+                    edges that actually represent multiple errors in the circuit (resulting in the
+                    decoder making misinformed choices when decoding).
+
+                    Irrelevant unless decompose_errors=True.
 
             Examples:
                 >>> import stim
 
                 >>> stim.Circuit('''
                 ...     X_ERROR(0.125) 0
                 ...     X_ERROR(0.25) 1
@@ -1251,15 +1424,15 @@
 }
 
 void pybind_circuit_after_types_all_defined(pybind11::class_<Circuit> &c) {
     c.def(
         "shortest_graphlike_error",
         &circuit_shortest_graphlike_error,
         pybind11::kw_only(),
-        pybind11::arg("ignore_ungraphlike_errors") = false,
+        pybind11::arg("ignore_ungraphlike_errors") = true,
         pybind11::arg("canonicalize_circuit_errors") = false,
         clean_doc_string(u8R"DOC(
             Finds a minimum sized set of graphlike errors that produce an undetected logical error.
 
             A "graphlike error" is an error that creates at most two detection events (causes a change in the parity of
             the measurement sets of at most two DETECTOR annotations).
 
@@ -1269,35 +1442,37 @@
 
             This method works by converting the circuit into a `stim.DetectorErrorModel` using
             `circuit.detector_error_model(...)`, computing the shortest graphlike error of the error model, and then
             converting the physical errors making up that logical error back into representative circuit errors.
 
             Args:
                 ignore_ungraphlike_errors:
-                    False (default): Attempt to decompose any ungraphlike errors in the circuit into graphlike parts.
+                    False: Attempt to decompose any ungraphlike errors in the circuit into graphlike parts.
                         If this fails, raise an exception instead of continuing.
                         Note: in some cases, graphlike errors only appear as parts of decomposed ungraphlike errors.
                         This can produce a result that lists DEM errors with zero matching circuit errors, because the
                         only way to achieve those errors is by combining a decomposed error with a graphlike error.
                         As a result, when using this option it is NOT guaranteed that the length of the result is an
                         upper bound on the true code distance. That is only the case if every item in the result lists
                         at least one matching circuit error.
-                    True: Ungraphlike errors are simply skipped as if they weren't present, even if they could become
-                        graphlike if decomposed. This guarantees the length of the result is an upper bound on the true
-                        code distance.
+                    True (default): Ungraphlike errors are simply skipped as if they weren't present, even if they could
+                        become graphlike if decomposed. This guarantees the length of the result is an upper bound on
+                        the true code distance.
                 canonicalize_circuit_errors: Whether or not to use one representative for equal-symptom circuit errors.
                     False (default): Each DEM error lists every possible circuit error that single handedly produces
                         those symptoms as a potential match. This is verbose but gives complete information.
                     True: Each DEM error is matched with one possible circuit error that single handedly produces those
                         symptoms, with a preference towards errors that are simpler (e.g. apply Paulis to fewer qubits).
                         This discards mostly-redundant information about different ways to produce the same symptoms in
                         order to give a succinct result.
 
             Returns:
-                ...
+                A detector error model containing only the error mechanisms that cause the undetectable
+                logical error. The error mechanisms will have their probabilities set to 1 (indicating that
+                they are necessary) and will not suggest a decomposition.
 
             Examples:
                 >>> import stim
 
                 >>> circuit = stim.Circuit.generated(
                 ...     "repetition_code:memory",
                 ...     rounds=10,
@@ -1305,16 +1480,99 @@
                 ...     before_round_data_depolarization=0.01)
                 >>> len(circuit.shortest_graphlike_error())
                 7
         )DOC")
             .data());
 
     c.def(
+        "search_for_undetectable_logical_errors",
+        &py_find_undetectable_logical_error,
+        pybind11::kw_only(),
+        pybind11::arg("dont_explore_detection_event_sets_with_size_above"),
+        pybind11::arg("dont_explore_edges_with_degree_above"),
+        pybind11::arg("dont_explore_edges_increasing_symptom_degree"),
+        pybind11::arg("canonicalize_circuit_errors") = false,
+        clean_doc_string(u8R"DOC(
+            Searches for lists of errors from the model that form an undetectable logical error.
+
+            THIS IS A HEURISTIC METHOD. It does not guarantee that it will find errors of particular
+            sizes, or with particular properties. The errors it finds are a tangled combination of the
+            truncation parameters you specify, internal optimizations which are correct when not
+            truncating, and minutia of the circuit being considered.
+
+            If you want a well behaved method that does provide guarantees of finding errors of a
+            particular type, use `stim.Circuit.shortest_graphlike_error`. This method is more
+            thorough than that (assuming you don't truncate so hard you omit graphlike edges),
+            but exactly how thorough is difficult to describe. It's also not guaranteed that the
+            behavior of this method will not be changed in the future in a way that permutes which
+            logical errors are found and which are missed.
+
+            This search method considers hyper errors, so it has worst case exponential runtime. It is
+            important to carefully consider the arguments you are providing, which truncate the search
+            space and trade cost for quality.
+
+            The search progresses by starting from each error that crosses a logical observable, noting
+            which detection events each error produces, and then iteratively adding in errors touching
+            those detection events attempting to cancel out the detection event with the lowest index.
+
+            Beware that the choice of logical observable can interact with the truncation options. Using
+            different observables can change whether or not the search succeeds, even if those observables
+            are equal modulo the stabilizers of the code. This is because the edges crossing logical
+            observables are used as starting points for the search, and starting from different places along
+            a path will result in different numbers of symptoms in intermediate states as the search
+            progresses. For example, if the logical observable is next to a boundary, then the starting
+            edges are likely boundary edges (degree 1) with 'room to grow', whereas if the observable was
+            running through the bulk then the starting edges will have degree at least 2.
+
+            Args:
+                dont_explore_detection_event_sets_with_size_above: Truncates the search space by refusing to
+                    cross an edge (i.e. add an error) when doing so would produce an intermediate state that
+                    has more detection events than this limit.
+                dont_explore_edges_with_degree_above: Truncates the search space by refusing to consider
+                    errors that cause a lot of detection events. For example, you may only want to consider
+                    graphlike errors which have two or fewer detection events.
+                dont_explore_edges_increasing_symptom_degree: Truncates the search space by refusing to
+                    cross an edge (i.e. add an error) when doing so would produce an intermediate state that
+                    has more detection events that the previous intermediate state. This massively improves
+                    the efficiency of the search because instead of, for example, exploring all n^4 possible
+                    detection event sets with 4 symptoms, the search will attempt to cancel out symptoms one
+                    by one.
+                canonicalize_circuit_errors: Whether or not to use one representative for equal-symptom circuit errors.
+                    False (default): Each DEM error lists every possible circuit error that single handedly produces
+                        those symptoms as a potential match. This is verbose but gives complete information.
+                    True: Each DEM error is matched with one possible circuit error that single handedly produces those
+                        symptoms, with a preference towards errors that are simpler (e.g. apply Paulis to fewer qubits).
+                        This discards mostly-redundant information about different ways to produce the same symptoms in
+                        order to give a succinct result.
+
+            Returns:
+                A detector error model containing only the error mechanisms that cause the undetectable
+                logical error. The error mechanisms will have their probabilities set to 1 (indicating that
+                they are necessary) and will not suggest a decomposition.
+
+            Examples:
+                >>> import stim
+                >>> circuit = stim.Circuit.generated(
+                ...     "surface_code:rotated_memory_x",
+                ...     rounds=5,
+                ...     distance=5,
+                ...     after_clifford_depolarization=0.001)
+                >>> print(len(circuit.search_for_undetectable_logical_errors(
+                ...     dont_explore_detection_event_sets_with_size_above=4,
+                ...     dont_explore_edges_with_degree_above=4,
+                ...     dont_explore_edges_increasing_symptom_degree=True,
+                ... )))
+                5
+        )DOC")
+            .data());
+    c.def(
         "explain_detector_error_model_errors",
-        [](const Circuit &self, const pybind11::object &dem_filter, bool reduce_to_one_representative_error) -> std::vector<ExplainedError> {
+        [](const Circuit &self,
+           const pybind11::object &dem_filter,
+           bool reduce_to_one_representative_error) -> std::vector<ExplainedError> {
             if (dem_filter.is_none()) {
                 return ErrorMatcher::explain_errors_from_circuit(self, nullptr, reduce_to_one_representative_error);
             } else {
                 const DetectorErrorModel &model = dem_filter.cast<const DetectorErrorModel &>();
                 return ErrorMatcher::explain_errors_from_circuit(self, &model, reduce_to_one_representative_error);
             }
         },
@@ -1366,8 +1624,79 @@
                         (after 0 TICKs)
                         at instruction #3 (DEPOLARIZE1) in the circuit
                         at target #1 of the instruction
                         resolving to DEPOLARIZE1(0.01) 0
                 }
         )DOC")
             .data());
+
+    c.def(
+        "without_noise",
+        &Circuit::without_noise,
+        clean_doc_string(u8R"DOC(
+            Returns a copy of the circuit with all noise processes removed.
+
+            Pure noise instructions, such as X_ERROR and DEPOLARIZE2, are not
+            included in the result.
+
+            Noisy measurement instructions, like `M(0.001)`, have their noise
+            parameter removed.
+
+            Returns:
+                A `stim.Circuit` with the same instructions except all noise
+                processes have been removed.
+
+            Examples:
+                >>> import stim
+                >>> stim.Circuit('''
+                ...     X_ERROR(0.25) 0
+                ...     CNOT 0 1
+                ...     M(0.125) 0
+                ... ''').without_noise()
+                stim.Circuit('''
+                    CX 0 1
+                    M 0
+                ''')
+        )DOC")
+            .data());
+
+    c.def(
+        "flattened",
+        &Circuit::flattened,
+        clean_doc_string(u8R"DOC(
+            Creates an equivalent circuit without REPEAT or SHIFT_COORDS.
+
+            Returns:
+                A `stim.Circuit` with the same instructions in the same order,
+                but with loops flattened into repeated instructions and with
+                all coordinate shifts inlined.
+
+            Examples:
+                >>> import stim
+                >>> stim.Circuit('''
+                ...     REPEAT 5 {
+                ...         MR 0 1
+                ...         DETECTOR(0, 0) rec[-2]
+                ...         DETECTOR(1, 0) rec[-1]
+                ...         SHIFT_COORDS(0, 1)
+                ...     }
+                ... ''').flattened()
+                stim.Circuit('''
+                    MR 0 1
+                    DETECTOR(0, 0) rec[-2]
+                    DETECTOR(1, 0) rec[-1]
+                    MR 0 1
+                    DETECTOR(0, 1) rec[-2]
+                    DETECTOR(1, 1) rec[-1]
+                    MR 0 1
+                    DETECTOR(0, 2) rec[-2]
+                    DETECTOR(1, 2) rec[-1]
+                    MR 0 1
+                    DETECTOR(0, 3) rec[-2]
+                    DETECTOR(1, 3) rec[-1]
+                    MR 0 1
+                    DETECTOR(0, 4) rec[-2]
+                    DETECTOR(1, 4) rec[-1]
+                ''')
+        )DOC")
+            .data());
 }
```

### Comparing `stim-1.8.0/src/stim/circuit/circuit_gate_target.pybind.cc` & `stim-1.9.0/src/stim/circuit/circuit_gate_target.pybind.cc`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 
 #include "stim/circuit/circuit_gate_target.pybind.h"
 
 #include "stim/circuit/circuit.h"
 #include "stim/py/base.pybind.h"
 
 using namespace stim;
+using namespace stim_pybind;
 
 GateTarget handle_to_gate_target(const pybind11::handle &obj) {
     try {
         return pybind11::cast<GateTarget>(obj);
     } catch (const pybind11::cast_error &ex) {
     }
     try {
@@ -36,15 +37,14 @@
     return handle_to_gate_target(obj);
 }
 
 void pybind_circuit_gate_target(pybind11::module &m) {
     auto c = pybind11::class_<GateTarget>(
         m,
         "GateTarget",
-        pybind11::module_local(),
         clean_doc_string(u8R"DOC(
             Represents a gate target, like `0` or `rec[-1]`, from a circuit.
 
             Examples:
                 >>> import stim
                 >>> circuit = stim.Circuit('''
                 ...     M 0 !1
```

### Comparing `stim-1.8.0/src/stim/circuit/circuit_instruction.pybind.cc` & `stim-1.9.0/src/stim/circuit/circuit_instruction.pybind.cc`

 * *Files 1% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 
 #include "stim/circuit/circuit_gate_target.pybind.h"
 #include "stim/circuit/gate_data.h"
 #include "stim/py/base.pybind.h"
 #include "stim/str_util.h"
 
 using namespace stim;
+using namespace stim_pybind;
 
 CircuitInstruction::CircuitInstruction(
     const char *name, const std::vector<pybind11::object> &init_targets, const std::vector<double> &gate_args)
     : gate(GATE_DATA.at(name)), gate_args(gate_args) {
     for (const auto &obj : init_targets) {
         targets.push_back(obj_to_gate_target(obj));
     }
@@ -79,15 +80,14 @@
     return gate_args;
 }
 
 void pybind_circuit_instruction(pybind11::module &m) {
     auto c = pybind11::class_<CircuitInstruction>(
         m,
         "CircuitInstruction",
-        pybind11::module_local(),
         clean_doc_string(u8R"DOC(
             An instruction, like `H 0 1` or `CNOT rec[-1] 5`, from a circuit.
 
             Examples:
                 >>> import stim
                 >>> circuit = stim.Circuit('''
                 ...     H 0
```

### Comparing `stim-1.8.0/src/stim/circuit/circuit_repeat_block.pybind.cc` & `stim-1.9.0/src/stim/circuit/circuit_repeat_block.pybind.cc`

 * *Files 1% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 
 #include "stim/circuit/circuit.h"
 #include "stim/circuit/circuit.pybind.h"
 #include "stim/circuit/circuit_instruction.pybind.h"
 #include "stim/py/base.pybind.h"
 
 using namespace stim;
+using namespace stim_pybind;
 
 CircuitRepeatBlock::CircuitRepeatBlock(uint64_t repeat_count, stim::Circuit body)
     : repeat_count(repeat_count), body(body) {
     if (repeat_count == 0) {
         throw std::invalid_argument("Can't repeat 0 times.");
     }
 }
@@ -41,15 +42,14 @@
     return "stim.CircuitRepeatBlock(" + std::to_string(repeat_count) + ", " + circuit_repr(body) + ")";
 }
 
 void pybind_circuit_repeat_block(pybind11::module &m) {
     auto c = pybind11::class_<CircuitRepeatBlock>(
         m,
         "CircuitRepeatBlock",
-        pybind11::module_local(),
         clean_doc_string(u8R"DOC(
             A REPEAT block from a circuit.
 
             Examples:
                 >>> import stim
                 >>> circuit = stim.Circuit('''
                 ...     H 0
```

### Comparing `stim-1.8.0/src/stim/circuit/gate_data.cc` & `stim-1.9.0/src/stim/circuit/gate_data.cc`

 * *Files identical despite different names*

### Comparing `stim-1.8.0/src/stim/circuit/gate_data_annotations.cc` & `stim-1.9.0/src/stim/circuit/gate_data_annotations.cc`

 * *Files 5% similar despite different names*

```diff
@@ -56,22 +56,22 @@
 detectors but `DETECTOR rec[-1] rec[-2]` is not, then under noiseless execution the two gauge detectors would either
 always produce the same result or always produce opposite results.
 
 Detectors can specify coordinates using their parens arguments. Coordinates have no effect on simulations, but can be
 useful to tools consuming the circuit. For example, a tool drawing how the detectors in a circuit relate to each other
 can use the coordinates as hints for where to place the detectors in the drawing.
 
-- Parens Arguments:
+Parens Arguments:
 
     Optional.
     Coordinate metadata, relative to the current coordinate offset accumulated from `SHIFT_COORDS` instructions.
     Can be any number of coordinates from 1 to 16.
     There is no required convention for which coordinate is which.
 
-- Targets:
+Targets:
 
     The measurement records to XOR together to get the deterministic-under-noiseless-execution parity.
 
 - Example:
 
     ```
     R 0
@@ -149,19 +149,19 @@
 means that even though `X` and `X_ERROR(1)` have equivalent effects on the measurements making up an observable, they
 have differing effects on the reported value of an observable when sampling detection events (because `X` is intended,
 determining the expected value, and `X_ERROR` is noise, causing deviations from the expected value).
 
 It is not recommended for the measurement set of an observable to have inconsistent parity. For example, the
 circuit-to-detector-error-model conversion will refuse to operate on circuits containing such observables.
 
-- Parens Arguments:
+Parens Arguments:
 
     A non-negative integer specifying the index of the logical observable to add the measurement records to.
 
-- Targets:
+Targets:
 
     The measurement records to add to the specified observable.
 
 - Example:
 
     ```
     R 0 1
@@ -206,19 +206,19 @@
 This instruction is not necessary, it has no effect on simulations, but it can be used by tools that are transforming or
 visualizing the circuit. For example, a tool that adds noise to a circuit may include cross-talk terms that require
 knowing whether or not operations are happening in the same time step or not.
 
 TICK instructions are added, and checked for, by `stimcirq` in order to preserve the moment structure of cirq circuits
 converted between stim circuits and cirq circuits.
 
-- Parens Arguments:
+Parens Arguments:
 
     This instruction takes no parens arguments.
 
-- Targets:
+Targets:
 
     This instruction takes no targets.
 
 - Example:
 
     ```
     # First time step.
@@ -261,22 +261,22 @@
 `stimcirq` uses `QUBIT_COORDS` instructions to preserve `cirq.LineQubit` and `cirq.GridQubit` coordinates when
 converting between stim circuits and cirq circuits
 
 A qubit's coordinates can be specified multiple times, with the intended interpretation being that the qubit is at the
 location of the most recent assignment. For example, this could be used to indicate a simulated qubit is iteratively
 playing the role of many physical qubits.
 
-- Parens Arguments:
+Parens Arguments:
 
     Optional.
     The latest coordinates of the qubit, relative to accumulated offsets from `SHIFT_COORDS` instructions.
     Can be any number of coordinates from 1 to 16.
     There is no required convention for which coordinate is which.
 
-- Targets:
+Targets:
 
     The qubit or qubits the coordinates apply to.
 
 - Example:
 
     ```
     # Annotate that qubits 0 to 3 are at the corners of a square.
@@ -309,21 +309,21 @@
 Accumulates offsets that affect qubit coordinates and detector coordinates.
 
 Note: when qubit/detector coordinates use fewer dimensions than SHIFT_COORDS, the offsets from the additional dimensions
 are ignored (i.e. not specifying a dimension is different from specifying it to be 0).
 
 See also: `QUBIT_COORDS`, `DETECTOR`.
 
-- Parens Arguments:
+Parens Arguments:
 
     Offsets to add into the current coordinate offset.
     Can be any number of coordinate offsets from 1 to 16.
     There is no required convention for which coordinate is which.
 
-- Targets:
+Targets:
 
     This instruction takes no targets.
 
 - Example:
 
     ```
     SHIFT_COORDS(500.5)
```

### Comparing `stim-1.8.0/src/stim/circuit/gate_data_blocks.cc` & `stim-1.9.0/src/stim/circuit/gate_data_blocks.cc`

 * *Files 9% similar despite different names*

```diff
@@ -35,19 +35,19 @@
                     R"MARKDOWN(
 Repeats the instructions in its body N times.
 
 Currently, repetition counts of 0 are not allowed because they create corner cases with ambiguous resolutions.
 For example, if a logical observable is only given measurements inside a repeat block with a repetition count of 0, it's
 ambiguous whether the output of sampling the logical observables includes a bit for that logical observable.
 
-- Parens Arguments:
+Parens Arguments:
 
     This instruction takes no parens arguments.
 
-- Targets:
+Targets:
 
     A positive integer in [1, 10^18] specifying the number of repetitions.
 
 - Example:
 
     ```
     REPEAT 2 {
```

### Comparing `stim-1.8.0/src/stim/circuit/gate_data_collapsing.cc` & `stim-1.9.0/src/stim/circuit/gate_data_collapsing.cc`

 * *Files 4% similar despite different names*

```diff
@@ -33,20 +33,20 @@
             []() -> ExtraGateData {
                 return {
                     "L_Collapsing Gates",
                     R"MARKDOWN(
 X-basis measurement (optionally noisy).
 Projects each target qubit into `|+>` or `|->` and reports its value (false=`|+>`, true=`|->`).
 
-- Parens Arguments:
+Parens Arguments:
 
     Optional.
     A single float specifying A single float specifying the probability of flipping each reported measurement result.
 
-- Targets:
+Targets:
 
     The qubits to measure in the X basis.
     Prefixing a qubit target with `!` flips its reported measurement result.
 )MARKDOWN",
                     {},
                     {"X -> +m xor chance(p)", "X -> +X"},
                     R"CIRCUIT(
@@ -69,20 +69,20 @@
             []() -> ExtraGateData {
                 return {
                     "L_Collapsing Gates",
                     R"MARKDOWN(
 Y-basis measurement (optionally noisy).
 Projects each target qubit into `|i>` or `|-i>` and reports its value (false=`|i>`, true=`|-i>`).
 
-- Parens Arguments:
+Parens Arguments:
 
     Optional.
     A single float specifying the probability of flipping each reported measurement result.
 
-- Targets:
+Targets:
 
     The qubits to measure in the Y basis.
     Prefixing a qubit target with `!` flips its reported measurement result.
 )MARKDOWN",
                     {},
                     {"Y -> m xor chance(p)", "Y -> +Y"},
                     R"CIRCUIT(
@@ -109,20 +109,20 @@
             []() -> ExtraGateData {
                 return {
                     "L_Collapsing Gates",
                     R"MARKDOWN(
 Z-basis measurement (optionally noisy).
 Projects each target qubit into `|0>` or `|1>` and reports its value (false=`|0>`, true=`|1>`).
 
-- Parens Arguments:
+Parens Arguments:
 
     Optional.
     A single float specifying the probability of flipping each reported measurement result.
 
-- Targets:
+Targets:
 
     The qubits to measure in the Z basis.
     Prefixing a qubit target with `!` flips its reported measurement result.
 )MARKDOWN",
                     {},
                     {"Z -> m xor chance(p)", "Z -> +Z"},
                     R"CIRCUIT(
@@ -146,20 +146,20 @@
             []() -> ExtraGateData {
                 return {
                     "L_Collapsing Gates",
                     R"MARKDOWN(
 X-basis demolition measurement (optionally noisy).
 Projects each target qubit into `|+>` or `|->`, reports its value (false=`|+>`, true=`|->`), then resets to `|+>`.
 
-- Parens Arguments:
+Parens Arguments:
 
     Optional.
     A single float specifying the probability of flipping each reported measurement result.
 
-- Targets:
+Targets:
 
     The qubits to measure and reset in the X basis.
     Prefixing a qubit target with `!` flips its reported measurement result.
 )MARKDOWN",
                     {},
                     {"X -> m xor chance(p)", "1 -> +X"},
                     R"CIRCUIT(
@@ -183,20 +183,20 @@
             []() -> ExtraGateData {
                 return {
                     "L_Collapsing Gates",
                     R"MARKDOWN(
 Y-basis demolition measurement (optionally noisy).
 Projects each target qubit into `|i>` or `|-i>`, reports its value (false=`|i>`, true=`|-i>`), then resets to `|i>`.
 
-- Parens Arguments:
+Parens Arguments:
 
     Optional.
     A single float specifying the probability of flipping each reported measurement result.
 
-- Targets:
+Targets:
 
     The qubits to measure and reset in the Y basis.
     Prefixing a qubit target with `!` flips its reported measurement result.
 )MARKDOWN",
                     {},
                     {"Y -> m xor chance(p)", "1 -> +Y"},
                     R"CIRCUIT(
@@ -224,20 +224,20 @@
             []() -> ExtraGateData {
                 return {
                     "L_Collapsing Gates",
                     R"MARKDOWN(
 Z-basis demolition measurement (optionally noisy).
 Projects each target qubit into `|0>` or `|1>`, reports its value (false=`|0>`, true=`|1>`), then resets to `|0>`.
 
-- Parens Arguments:
+Parens Arguments:
 
     Optional.
     A single float specifying the probability of flipping each reported measurement result.
 
-- Targets:
+Targets:
 
     The qubits to measure and reset in the Z basis.
     Prefixing a qubit target with `!` flips its reported measurement result.
 )MARKDOWN",
                     {},
                     {"Z -> m xor chance(p)", "1 -> +Z"},
                     R"CIRCUIT(
@@ -262,19 +262,19 @@
             []() -> ExtraGateData {
                 return {
                     "L_Collapsing Gates",
                     R"MARKDOWN(
 X-basis reset.
 Forces each target qubit into the `|+>` state by silently measuring it in the X basis and applying a `Z` gate if it ended up in the `|->` state.
 
-- Parens Arguments:
+Parens Arguments:
 
     This instruction takes no parens arguments.
 
-- Targets:
+Targets:
 
     The qubits to reset in the X basis.
 )MARKDOWN",
                     {},
                     {"1 -> +X"},
                     R"CIRCUIT(
 H 0
@@ -296,19 +296,19 @@
             []() -> ExtraGateData {
                 return {
                     "L_Collapsing Gates",
                     R"MARKDOWN(
 Y-basis reset.
 Forces each target qubit into the `|i>` state by silently measuring it in the Y basis and applying an `X` gate if it ended up in the `|-i>` state.
 
-- Parens Arguments:
+Parens Arguments:
 
     This instruction takes no parens arguments.
 
-- Targets:
+Targets:
 
     The qubits to reset in the Y basis.
 )MARKDOWN",
                     {},
                     {"1 -> +Y"},
                     R"CIRCUIT(
 S 0
@@ -334,19 +334,19 @@
             []() -> ExtraGateData {
                 return {
                     "L_Collapsing Gates",
                     R"MARKDOWN(
 Z-basis reset.
 Forces each target qubit into the `|0>` state by silently measuring it in the Z basis and applying an `X` gate if it ended up in the `|1>` state.
 
-- Parens Arguments:
+Parens Arguments:
 
     This instruction takes no parens arguments.
 
-- Targets:
+Targets:
 
     The qubits to reset in the Z basis.
 )MARKDOWN",
                     {},
                     {"1 -> +Z"},
                     R"CIRCUIT(
 R 0
@@ -367,20 +367,20 @@
             (GateFlags)(GATE_PRODUCES_NOISY_RESULTS | GATE_TARGETS_PAULI_STRING | GATE_TARGETS_COMBINERS | GATE_ARGS_ARE_DISJOINT_PROBABILITIES),
             []() -> ExtraGateData {
                 return {
                     "L_Collapsing Gates",
                     R"MARKDOWN(
 Measure Pauli products.
 
-- Parens Arguments:
+Parens Arguments:
 
     Optional.
     A single float specifying the probability of flipping each reported measurement result.
 
-- Targets:
+Targets:
 
     A series of Pauli products to measure.
 
     Each Pauli product is a series of Pauli targets (`[XYZ]#`) separated by combiners (`*`).
     Products can be negated by prefixing a Pauli target in the product with an inverter (`!`)
 
 - Example:
```

### Comparing `stim-1.8.0/src/stim/circuit/gate_data_controlled.cc` & `stim-1.9.0/src/stim/circuit/gate_data_controlled.cc`

 * *Files 3% similar despite different names*

```diff
@@ -40,19 +40,19 @@
 The X-controlled X gate.
 First qubit is the control, second qubit is the target.
 
 Applies an X gate to the target if the control is in the |-> state.
 
 Negates the amplitude of the |->|-> state.
 
-- Parens Arguments:
+Parens Arguments:
 
     This instruction takes no parens arguments.
 
-- Targets:
+Targets:
 
     Qubit pairs to operate on.
 )MARKDOWN",
                     {{0.5f, 0.5f, 0.5f, -0.5f},
                      {0.5f, 0.5f, -0.5f, 0.5f},
                      {0.5f, -0.5f, 0.5f, 0.5f},
                      {-0.5f, 0.5f, 0.5f, 0.5f}},
@@ -82,19 +82,19 @@
 The X-controlled Y gate.
 First qubit is the control, second qubit is the target.
 
 Applies a Y gate to the target if the control is in the |-> state.
 
 Negates the amplitude of the |->|-i> state.
 
-- Parens Arguments:
+Parens Arguments:
 
     This instruction takes no parens arguments.
 
-- Targets:
+Targets:
 
     Qubit pairs to operate on.
 )MARKDOWN",
                     {{0.5f, 0.5f, -0.5f * i, 0.5f * i},
                      {0.5f, 0.5f, 0.5f * i, -0.5f * i},
                      {0.5f * i, -0.5f * i, 0.5f, 0.5f},
                      {-0.5f * i, 0.5f * i, 0.5f, 0.5f}},
@@ -127,19 +127,19 @@
 First qubit is the control, second qubit is the target.
 The second qubit can be replaced by a measurement record.
 
 Applies a Z gate to the target if the control is in the |-> state.
 
 Negates the amplitude of the |->|1> state.
 
-- Parens Arguments:
+Parens Arguments:
 
     This instruction takes no parens arguments.
 
-- Targets:
+Targets:
 
     Qubit pairs to operate on.
 )MARKDOWN",
                     {{1, 0, 0, 0}, {0, 1, 0, 0}, {0, 0, 0, 1}, {0, 0, 1, 0}},
                     {"+XI", "+ZZ", "+XX", "+IZ"},
                     R"CIRCUIT(
 CNOT 1 0
@@ -164,19 +164,19 @@
 The Y-controlled X gate.
 First qubit is the control, second qubit is the target.
 
 Applies an X gate to the target if the control is in the |-i> state.
 
 Negates the amplitude of the |-i>|-> state.
 
-- Parens Arguments:
+Parens Arguments:
 
     This instruction takes no parens arguments.
 
-- Targets:
+Targets:
 
     Qubit pairs to operate on.
 )MARKDOWN",
                     {{0.5f, -i * 0.5f, 0.5f, i * 0.5f},
                      {i * 0.5f, 0.5f, -i * 0.5f, 0.5f},
                      {0.5f, i * 0.5f, 0.5f, -i * 0.5f},
                      {-i * 0.5f, 0.5f, i * 0.5f, 0.5f}},
@@ -208,19 +208,19 @@
 The Y-controlled Y gate.
 First qubit is the control, second qubit is the target.
 
 Applies a Y gate to the target if the control is in the |-i> state.
 
 Negates the amplitude of the |-i>|-i> state.
 
-- Parens Arguments:
+Parens Arguments:
 
     This instruction takes no parens arguments.
 
-- Targets:
+Targets:
 
     Qubit pairs to operate on.
 )MARKDOWN",
                     {{0.5f, -i * 0.5f, -i * 0.5f, 0.5f},
                      {i * 0.5f, 0.5f, -0.5f, -i * 0.5f},
                      {i * 0.5f, -0.5f, 0.5f, -i * 0.5f},
                      {0.5f, i * 0.5f, i * 0.5f, 0.5f}},
@@ -255,19 +255,19 @@
 First qubit is the control, second qubit is the target.
 The second qubit can be replaced by a measurement record.
 
 Applies a Z gate to the target if the control is in the |-i> state.
 
 Negates the amplitude of the |-i>|1> state.
 
-- Parens Arguments:
+Parens Arguments:
 
     This instruction takes no parens arguments.
 
-- Targets:
+Targets:
 
     Qubit pairs to operate on.
 )MARKDOWN",
                     {{1, 0, 0, 0}, {0, 1, 0, 0}, {0, 0, 0, -i}, {0, 0, i, 0}},
                     {"+XZ", "+ZZ", "+YX", "+IZ"},
                     R"CIRCUIT(
 S 0
@@ -297,19 +297,19 @@
 First qubit is the control, second qubit is the target.
 The first qubit can be replaced by a measurement record.
 
 Applies an X gate to the target if the control is in the |1> state.
 
 Negates the amplitude of the |1>|-> state.
 
-- Parens Arguments:
+Parens Arguments:
 
     This instruction takes no parens arguments.
 
-- Targets:
+Targets:
 
     Qubit pairs to operate on.
 )MARKDOWN",
                     {{1, 0, 0, 0}, {0, 0, 0, 1}, {0, 0, 1, 0}, {0, 1, 0, 0}},
                     {"+XX", "+ZI", "+IX", "+ZZ"},
                     R"CIRCUIT(
 CNOT 0 1
@@ -337,19 +337,19 @@
 First qubit is the control, second qubit is the target.
 The first qubit can be replaced by a measurement record.
 
 Applies a Y gate to the target if the control is in the |1> state.
 
 Negates the amplitude of the |1>|-i> state.
 
-- Parens Arguments:
+Parens Arguments:
 
     This instruction takes no parens arguments.
 
-- Targets:
+Targets:
 
     Qubit pairs to operate on.
 )MARKDOWN",
                     {{1, 0, 0, 0}, {0, 0, 0, -i}, {0, 0, 1, 0}, {0, i, 0, 0}},
                     {"+XY", "+ZI", "+ZX", "+ZZ"},
                     R"CIRCUIT(
 S 1
@@ -380,19 +380,19 @@
 First qubit is the control, second qubit is the target.
 Either qubit can be replaced by a measurement record.
 
 Applies a Z gate to the target if the control is in the |1> state.
 
 Negates the amplitude of the |1>|1> state.
 
-- Parens Arguments:
+Parens Arguments:
 
     This instruction takes no parens arguments.
 
-- Targets:
+Targets:
 
     Qubit pairs to operate on.
 )MARKDOWN",
                     {{1, 0, 0, 0}, {0, 1, 0, 0}, {0, 0, 1, 0}, {0, 0, 0, -1}},
                     {"+XZ", "+ZI", "+ZX", "+IZ"},
                     R"CIRCUIT(
 H 1
```

### Comparing `stim-1.8.0/src/stim/circuit/gate_data_hada.cc` & `stim-1.9.0/src/stim/circuit/gate_data_hada.cc`

 * *Files 16% similar despite different names*

```diff
@@ -37,19 +37,19 @@
             []() -> ExtraGateData {
                 return {
                     "B_Single Qubit Clifford Gates",
                     R"MARKDOWN(
 The Hadamard gate.
 Swaps the X and Z axes.
 
-- Parens Arguments:
+Parens Arguments:
 
     This instruction takes no parens arguments.
 
-- Targets:
+Targets:
 
     Qubits to operate on.
 )MARKDOWN",
                     {{s, s}, {s, -s}},
                     {"+Z", "+X"},
                     R"CIRCUIT(
 H 0
@@ -70,19 +70,19 @@
             GATE_IS_UNITARY,
             []() -> ExtraGateData {
                 return {
                     "B_Single Qubit Clifford Gates",
                     R"MARKDOWN(
 A variant of the Hadamard gate that swaps the X and Y axes (instead of X and Z).
 
-- Parens Arguments:
+Parens Arguments:
 
     This instruction takes no parens arguments.
 
-- Targets:
+Targets:
 
     Qubits to operate on.
 )MARKDOWN",
                     {{0, s - i * s}, {s + i * s, 0}},
                     {"+Y", "-Z"},
                     R"CIRCUIT(
 H 0
@@ -106,19 +106,19 @@
             GATE_IS_UNITARY,
             []() -> ExtraGateData {
                 return {
                     "B_Single Qubit Clifford Gates",
                     R"MARKDOWN(
 A variant of the Hadamard gate that swaps the Y and Z axes (instead of X and Z).
 
-- Parens Arguments:
+Parens Arguments:
 
     This instruction takes no parens arguments.
 
-- Targets:
+Targets:
 
     Qubits to operate on.
 )MARKDOWN",
                     {{s, -i * s}, {i * s, -s}},
                     {"-X", "+Y"},
                     R"CIRCUIT(
 H 0
```

### Comparing `stim-1.8.0/src/stim/circuit/gate_data_noisy.cc` & `stim-1.9.0/src/stim/circuit/gate_data_noisy.cc`

 * *Files 5% similar despite different names*

```diff
@@ -33,23 +33,23 @@
                 return {
                     "F_Noise Channels",
                     R"MARKDOWN(
 The single qubit depolarizing channel.
 
 Applies a randomly chosen Pauli with a given probability.
 
-- Parens Arguments:
+Parens Arguments:
 
     A single float specifying the depolarization strength.
 
-- Targets:
+Targets:
 
     Qubits to apply single-qubit depolarizing noise to.
 
-- Pauli Mixture:
+Pauli Mixture:
 
     ```
     1-p: I
     p/3: X
     p/3: Y
     p/3: Z
     ```
@@ -74,23 +74,23 @@
                 return {
                     "F_Noise Channels",
                     R"MARKDOWN(
 The two qubit depolarizing channel.
 
 Applies a randomly chosen two-qubit Pauli product with a given probability.
 
-- Parens Arguments:
+Parens Arguments:
 
     A single float specifying the depolarization strength.
 
-- Targets:
+Targets:
 
     Qubit pairs to apply two-qubit depolarizing noise to.
 
-- Pauli Mixture:
+Pauli Mixture:
 
     ```
      1-p: II
     p/15: IX
     p/15: IY
     p/15: IZ
     p/15: XI
@@ -125,23 +125,23 @@
             (GateFlags)(GATE_IS_NOISE | GATE_ARGS_ARE_DISJOINT_PROBABILITIES),
             []() -> ExtraGateData {
                 return {
                     "F_Noise Channels",
                     R"MARKDOWN(
 Applies a Pauli X with a given probability.
 
-- Parens Arguments:
+Parens Arguments:
 
     A single float specifying the probability of applying an X operation.
 
-- Targets:
+Targets:
 
     Qubits to apply bit flip noise to.
 
-- Pauli Mixture:
+Pauli Mixture:
 
     ```
     1-p: I
      p : X
     ```
 )MARKDOWN",
                     {},
@@ -162,23 +162,23 @@
             (GateFlags)(GATE_IS_NOISE | GATE_ARGS_ARE_DISJOINT_PROBABILITIES),
             []() -> ExtraGateData {
                 return {
                     "F_Noise Channels",
                     R"MARKDOWN(
 Applies a Pauli Y with a given probability.
 
-- Parens Arguments:
+Parens Arguments:
 
     A single float specifying the probability of applying a Y operation.
 
-- Targets:
+Targets:
 
     Qubits to apply Y flip noise to.
 
-- Pauli Mixture:
+Pauli Mixture:
 
     ```
     1-p: I
      p : Y
     ```
 )MARKDOWN",
                     {},
@@ -199,23 +199,23 @@
             (GateFlags)(GATE_IS_NOISE | GATE_ARGS_ARE_DISJOINT_PROBABILITIES),
             []() -> ExtraGateData {
                 return {
                     "F_Noise Channels",
                     R"MARKDOWN(
 Applies a Pauli Z with a given probability.
 
-- Parens Arguments:
+Parens Arguments:
 
     A single float specifying the probability of applying a Z operation.
 
-- Targets:
+Targets:
 
     Qubits to apply phase flip noise to.
 
-- Pauli Mixture:
+Pauli Mixture:
 
     ```
     1-p: I
      p : Z
     ```
 )MARKDOWN",
                     {},
@@ -236,34 +236,34 @@
             (GateFlags)(GATE_IS_NOISE | GATE_ARGS_ARE_DISJOINT_PROBABILITIES),
             []() -> ExtraGateData {
                 return {
                     "F_Noise Channels",
                     R"MARKDOWN(
 A single qubit Pauli error channel with explicitly specified probabilities for each case.
 
-- Parens Arguments:
+Parens Arguments:
 
     Three floats specifying disjoint Pauli case probabilities.
     px: Probability of applying an X operation.
     py: Probability of applying a Y operation.
     pz: Probability of applying a Z operation.
 
-- Targets:
+Targets:
 
     Qubits to apply the custom noise channel to.
 
 - Example:
 
     ```
     # Sample errors from the distribution 10% X, 15% Y, 20% Z, 55% I.
     # Apply independently to qubits 1, 2, 4.
     PAULI_CHANNEL_1(0.1, 0.15, 0.2) 1 2 4
     ```
 
-- Pauli Mixture:
+Pauli Mixture:
 
     ```
     1-px-py-pz: I
     px: X
     py: Y
     pz: Z
     ```
@@ -286,15 +286,15 @@
             (GateFlags)(GATE_IS_NOISE | GATE_ARGS_ARE_DISJOINT_PROBABILITIES),
             []() -> ExtraGateData {
                 return {
                     "F_Noise Channels",
                     R"MARKDOWN(
 A two qubit Pauli error channel with explicitly specified probabilities for each case.
 
-- Parens Arguments:
+Parens Arguments:
 
     Fifteen floats specifying the disjoint probabilities of each possible Pauli pair
     that can occur (except for the non-error double identity case).
     The disjoint probability arguments are (in order):
 
     1. pix: Probability of applying an IX operation.
     2. piy: Probability of applying an IY operation.
@@ -308,28 +308,28 @@
     10. pyy: Probability of applying a YY operation.
     11. pyz: Probability of applying a YZ operation.
     12. pzi: Probability of applying a ZI operation.
     13. pzx: Probability of applying a ZX operation.
     14. pzy: Probability of applying a ZY operation.
     15. pzz: Probability of applying a ZZ operation.
 
-- Targets:
+Targets:
 
     Pairs of qubits to apply the custom noise channel to.
     There must be an even number of targets.
 
 - Example:
 
     ```
     # Sample errors from the distribution 10% XX, 20% YZ, 70% II.
     # Apply independently to qubit pairs (1,2), (5,6), and (8,3)
     PAULI_CHANNEL_2(0,0,0, 0.1,0,0,0, 0,0,0,0.2, 0,0,0,0) 1 2 5 6 8 3
     ```
 
-- Pauli Mixture:
+Pauli Mixture:
 
     ```
     1-pix-piy-piz-pxi-pxx-pxy-pxz-pyi-pyx-pyy-pyz-pzi-pzx-pzy-pzz: II
     pix: IX
     piy: IY
     piz: IZ
     pxi: XI
@@ -368,19 +368,19 @@
                     R"MARKDOWN(
 Probabilistically applies a Pauli product error with a given probability.
 Sets the "correlated error occurred flag" to true if the error occurred.
 Otherwise sets the flag to false.
 
 See also: `ELSE_CORRELATED_ERROR`.
 
-- Parens Arguments:
+Parens Arguments:
 
     A single float specifying the probability of applying the Paulis making up the error.
 
-- Targets:
+Targets:
 
     Pauli targets specifying the Paulis to apply when the error occurs.
     Note that, for backwards compatibility reasons, the targets are not combined using combiners (`*`).
     They are implicitly all combined.
 
 - Example:
 
@@ -411,22 +411,26 @@
                 return {
                     "F_Noise Channels",
                     R"MARKDOWN(
 Probabilistically applies a Pauli product error with a given probability, unless the "correlated error occurred flag" is set.
 If the error occurs, sets the "correlated error occurred flag" to true.
 Otherwise leaves the flag alone.
 
+Note: when converting a circuit into a detector error model, every `ELSE_CORRELATED_ERROR` instruction must be preceded by
+an ELSE_CORRELATED_ERROR instruction or an E instruction. In other words, ELSE_CORRELATED_ERROR instructions should appear
+in contiguous chunks started by a CORRELATED_ERROR.
+
 See also: `CORRELATED_ERROR`.
 
-- Parens Arguments:
+Parens Arguments:
 
     A single float specifying the probability of applying the Paulis making up the error, conditioned on the "correlated
     error occurred flag" being False.
 
-- Targets:
+Targets:
 
     Pauli targets specifying the Paulis to apply when the error occurs.
     Note that, for backwards compatibility reasons, the targets are not combined using combiners (`*`).
     They are implicitly all combined.
 
 - Example:
```

### Comparing `stim-1.8.0/src/stim/circuit/gate_data_pauli.cc` & `stim-1.9.0/src/stim/circuit/gate_data_pauli.cc`

 * *Files 8% similar despite different names*

```diff
@@ -33,22 +33,22 @@
             &FrameSimulator::I,
             &ErrorAnalyzer::I,
             GATE_IS_UNITARY,
             []() -> ExtraGateData {
                 return {
                     "A_Pauli Gates",
                     R"MARKDOWN(
-Identity gate.
+The identity gate.
 Does nothing to the target qubits.
 
-- Parens Arguments:
+Parens Arguments:
 
     This instruction takes no parens arguments.
 
-- Targets:
+Targets:
 
     Qubits to do nothing to.
 )MARKDOWN",
                     {{1, 0}, {0, 1}},
                     {"+X", "+Z"},
                     R"CIRCUIT(
 # (no operations)
@@ -66,22 +66,22 @@
             &FrameSimulator::I,
             &ErrorAnalyzer::I,
             GATE_IS_UNITARY,
             []() -> ExtraGateData {
                 return {
                     "A_Pauli Gates",
                     R"MARKDOWN(
-Pauli X gate.
+The Pauli X gate.
 The bit flip gate.
 
-- Parens Arguments:
+Parens Arguments:
 
     This instruction takes no parens arguments.
 
-- Targets:
+Targets:
 
     Qubits to operate on.
 )MARKDOWN",
                     {{0, 1}, {1, 0}},
                     {"+X", "-Z"},
                     R"CIRCUIT(
 H 0
@@ -102,21 +102,21 @@
             &FrameSimulator::I,
             &ErrorAnalyzer::I,
             GATE_IS_UNITARY,
             []() -> ExtraGateData {
                 return {
                     "A_Pauli Gates",
                     R"MARKDOWN(
-Pauli Y gate.
+The Pauli Y gate.
 
-- Parens Arguments:
+Parens Arguments:
 
     This instruction takes no parens arguments.
 
-- Targets:
+Targets:
 
     Qubits to operate on.
 )MARKDOWN",
                     {{0, -i}, {i, 0}},
                     {"-X", "-Z"},
                     R"CIRCUIT(
 S 0
@@ -139,22 +139,22 @@
             &FrameSimulator::I,
             &ErrorAnalyzer::I,
             GATE_IS_UNITARY,
             []() -> ExtraGateData {
                 return {
                     "A_Pauli Gates",
                     R"MARKDOWN(
-Pauli Z gate.
+The Pauli Z gate.
 The phase flip gate.
 
-- Parens Arguments:
+Parens Arguments:
 
     This instruction takes no parens arguments.
 
-- Targets:
+Targets:
 
     Qubits to operate on.
 )MARKDOWN",
                     {{1, 0}, {0, -1}},
                     {"-X", "+Z"},
                     R"CIRCUIT(
 S 0
```

### Comparing `stim-1.8.0/src/stim/circuit/gate_data_period_3.cc` & `stim-1.9.0/src/stim/circuit/gate_data_period_3.cc`

 * *Files 6% similar despite different names*

```diff
@@ -35,19 +35,19 @@
             GATE_IS_UNITARY,
             []() -> ExtraGateData {
                 return {
                     "B_Single Qubit Clifford Gates",
                     R"MARKDOWN(
 Right handed period 3 axis cycling gate, sending X -> Y -> Z -> X.
 
-- Parens Arguments:
+Parens Arguments:
 
     This instruction takes no parens arguments.
 
-- Targets:
+Targets:
 
     Qubits to operate on.
 )MARKDOWN",
                     {{0.5f - i * 0.5f, -0.5f - 0.5f * i}, {0.5f - 0.5f * i, 0.5f + 0.5f * i}},
                     {"Y", "X"},
                     R"CIRCUIT(
 S 0
@@ -70,19 +70,19 @@
             GATE_IS_UNITARY,
             []() -> ExtraGateData {
                 return {
                     "B_Single Qubit Clifford Gates",
                     R"MARKDOWN(
 Left handed period 3 axis cycling gate, sending Z -> Y -> X -> Z.
 
-- Parens Arguments:
+Parens Arguments:
 
     This instruction takes no parens arguments.
 
-- Targets:
+Targets:
 
     Qubits to operate on.
 )MARKDOWN",
                     {{0.5f + i * 0.5f, 0.5f + 0.5f * i}, {-0.5f + 0.5f * i, 0.5f - 0.5f * i}},
                     {"Z", "Y"},
                     R"CIRCUIT(
 H 0
```

### Comparing `stim-1.8.0/src/stim/circuit/gate_data_period_4.cc` & `stim-1.9.0/src/stim/circuit/gate_data_period_4.cc`

 * *Files 9% similar despite different names*

```diff
@@ -36,19 +36,19 @@
             []() -> ExtraGateData {
                 return {
                     "B_Single Qubit Clifford Gates",
                     R"MARKDOWN(
 Principal square root of X gate.
 Phases the amplitude of |-> by i.
 
-- Parens Arguments:
+Parens Arguments:
 
     This instruction takes no parens arguments.
 
-- Targets:
+Targets:
 
     Qubits to operate on.
 )MARKDOWN",
                     {{0.5f + 0.5f * i, 0.5f - 0.5f * i}, {0.5f - 0.5f * i, 0.5f + 0.5f * i}},
                     {"+X", "-Y"},
                     R"CIRCUIT(
 H 0
@@ -71,19 +71,19 @@
             []() -> ExtraGateData {
                 return {
                     "B_Single Qubit Clifford Gates",
                     R"MARKDOWN(
 Adjoint of the principal square root of X gate.
 Phases the amplitude of |-> by -i.
 
-- Parens Arguments:
+Parens Arguments:
 
     This instruction takes no parens arguments.
 
-- Targets:
+Targets:
 
     Qubits to operate on.
 )MARKDOWN",
                     {{0.5f - 0.5f * i, 0.5f + 0.5f * i}, {0.5f + 0.5f * i, 0.5f - 0.5f * i}},
                     {"+X", "+Y"},
                     R"CIRCUIT(
 S 0
@@ -106,19 +106,19 @@
             []() -> ExtraGateData {
                 return {
                     "B_Single Qubit Clifford Gates",
                     R"MARKDOWN(
 Principal square root of Y gate.
 Phases the amplitude of |-i> by i.
 
-- Parens Arguments:
+Parens Arguments:
 
     This instruction takes no parens arguments.
 
-- Targets:
+Targets:
 
     Qubits to operate on.
 )MARKDOWN",
                     {{0.5f + 0.5f * i, -0.5f - 0.5f * i}, {0.5f + 0.5f * i, 0.5f + 0.5f * i}},
                     {"-Z", "+X"},
                     R"CIRCUIT(
 S 0
@@ -141,19 +141,19 @@
             []() -> ExtraGateData {
                 return {
                     "B_Single Qubit Clifford Gates",
                     R"MARKDOWN(
 Adjoint of the principal square root of Y gate.
 Phases the amplitude of |-i> by -i.
 
-- Parens Arguments:
+Parens Arguments:
 
     This instruction takes no parens arguments.
 
-- Targets:
+Targets:
 
     Qubits to operate on.
 )MARKDOWN",
                     {{0.5f - 0.5f * i, 0.5f - 0.5f * i}, {-0.5f + 0.5f * i, 0.5f - 0.5f * i}},
                     {"+Z", "-X"},
                     R"CIRCUIT(
 H 0
@@ -176,19 +176,19 @@
             []() -> ExtraGateData {
                 return {
                     "B_Single Qubit Clifford Gates",
                     R"MARKDOWN(
 Principal square root of Z gate.
 Phases the amplitude of |1> by i.
 
-- Parens Arguments:
+Parens Arguments:
 
     This instruction takes no parens arguments.
 
-- Targets:
+Targets:
 
     Qubits to operate on.
 )MARKDOWN",
                     {{1, 0}, {0, i}},
                     {"+Y", "+Z"},
                     R"CIRCUIT(
 S 0
@@ -210,19 +210,19 @@
             []() -> ExtraGateData {
                 return {
                     "B_Single Qubit Clifford Gates",
                     R"MARKDOWN(
 Adjoint of the principal square root of Z gate.
 Phases the amplitude of |1> by -i.
 
-- Parens Arguments:
+Parens Arguments:
 
     This instruction takes no parens arguments.
 
-- Targets:
+Targets:
 
     Qubits to operate on.
 )MARKDOWN",
                     {{1, 0}, {0, -i}},
                     {"-Y", "+Z"},
                     R"CIRCUIT(
 S 0
```

### Comparing `stim-1.8.0/src/stim/circuit/gate_data_pp.cc` & `stim-1.9.0/src/stim/circuit/gate_data_pp.cc`

 * *Files 3% similar despite different names*

```diff
@@ -35,19 +35,19 @@
             (GateFlags)(GATE_IS_UNITARY | GATE_TARGETS_PAIRS),
             []() -> ExtraGateData {
                 return {
                     "C_Two Qubit Clifford Gates",
                     R"MARKDOWN(
 Phases the -1 eigenspace of the XX observable by i.
 
-- Parens Arguments:
+Parens Arguments:
 
     This instruction takes no parens arguments.
 
-- Targets:
+Targets:
 
     Qubit pairs to operate on.
 )MARKDOWN",
                     {{0.5f + 0.5f * i, 0, 0, 0.5f - 0.5f * i},
                      {0, 0.5f + 0.5f * i, 0.5f - 0.5f * i, 0},
                      {0, 0.5f - 0.5f * i, 0.5f + 0.5f * i, 0},
                      {0.5f - 0.5f * i, 0, 0, 0.5f + 0.5f * i}},
@@ -73,19 +73,19 @@
             (GateFlags)(GATE_IS_UNITARY | GATE_TARGETS_PAIRS),
             []() -> ExtraGateData {
                 return {
                     "C_Two Qubit Clifford Gates",
                     R"MARKDOWN(
 Phases the -1 eigenspace of the XX observable by -i.
 
-- Parens Arguments:
+Parens Arguments:
 
     This instruction takes no parens arguments.
 
-- Targets:
+Targets:
 
     Qubit pairs to operate on.
 )MARKDOWN",
                     {{0.5f - 0.5f * i, 0, 0, 0.5f + 0.5f * i},
                      {0, 0.5f - 0.5f * i, 0.5f + 0.5f * i, 0},
                      {0, 0.5f + 0.5f * i, 0.5f - 0.5f * i, 0},
                      {0.5f + 0.5f * i, 0, 0, 0.5f - 0.5f * i}},
@@ -112,19 +112,19 @@
             (GateFlags)(GATE_IS_UNITARY | GATE_TARGETS_PAIRS),
             []() -> ExtraGateData {
                 return {
                     "C_Two Qubit Clifford Gates",
                     R"MARKDOWN(
 Phases the -1 eigenspace of the YY observable by i.
 
-- Parens Arguments:
+Parens Arguments:
 
     This instruction takes no parens arguments.
 
-- Targets:
+Targets:
 
     Qubit pairs to operate on.
 )MARKDOWN",
                     {{0.5f + 0.5f * i, 0, 0, -0.5f + 0.5f * i},
                      {0, 0.5f + 0.5f * i, 0.5f - 0.5f * i, 0},
                      {0, 0.5f - 0.5f * i, 0.5f + 0.5f * i, 0},
                      {-0.5f + 0.5f * i, 0, 0, 0.5f + 0.5f * i}},
@@ -152,19 +152,19 @@
             (GateFlags)(GATE_IS_UNITARY | GATE_TARGETS_PAIRS),
             []() -> ExtraGateData {
                 return {
                     "C_Two Qubit Clifford Gates",
                     R"MARKDOWN(
 Phases the -1 eigenspace of the YY observable by -i.
 
-- Parens Arguments:
+Parens Arguments:
 
     This instruction takes no parens arguments.
 
-- Targets:
+Targets:
 
     Qubit pairs to operate on.
 )MARKDOWN",
                     {{0.5f - 0.5f * i, 0, 0, -0.5f - 0.5f * i},
                      {0, 0.5f - 0.5f * i, 0.5f + 0.5f * i, 0},
                      {0, 0.5f + 0.5f * i, 0.5f - 0.5f * i, 0},
                      {-0.5f - 0.5f * i, 0, 0, 0.5f - 0.5f * i}},
@@ -193,19 +193,19 @@
             (GateFlags)(GATE_IS_UNITARY | GATE_TARGETS_PAIRS),
             []() -> ExtraGateData {
                 return {
                     "C_Two Qubit Clifford Gates",
                     R"MARKDOWN(
 Phases the -1 eigenspace of the ZZ observable by i.
 
-- Parens Arguments:
+Parens Arguments:
 
     This instruction takes no parens arguments.
 
-- Targets:
+Targets:
 
     Qubit pairs to operate on.
 )MARKDOWN",
                     {{1, 0, 0, 0}, {0, i, 0, 0}, {0, 0, i, 0}, {0, 0, 0, 1}},
                     {"+YZ", "+ZI", "+ZY", "+IZ"},
                     R"CIRCUIT(
 CNOT 0 1
@@ -226,19 +226,19 @@
             (GateFlags)(GATE_IS_UNITARY | GATE_TARGETS_PAIRS),
             []() -> ExtraGateData {
                 return {
                     "C_Two Qubit Clifford Gates",
                     R"MARKDOWN(
 Phases the -1 eigenspace of the ZZ observable by -i.
 
-- Parens Arguments:
+Parens Arguments:
 
     This instruction takes no parens arguments.
 
-- Targets:
+Targets:
 
     Qubit pairs to operate on.
 )MARKDOWN",
                     {{1, 0, 0, 0}, {0, -i, 0, 0}, {0, 0, -i, 0}, {0, 0, 0, 1}},
                     {"-YZ", "+ZI", "-ZY", "+IZ"},
                     R"CIRCUIT(
 H 1
```

### Comparing `stim-1.8.0/src/stim/circuit/gate_data_swaps.cc` & `stim-1.9.0/src/stim/circuit/gate_data_swaps.cc`

 * *Files 3% similar despite different names*

```diff
@@ -35,19 +35,19 @@
             (GateFlags)(GATE_IS_UNITARY | GATE_TARGETS_PAIRS),
             []() -> ExtraGateData {
                 return {
                     "C_Two Qubit Clifford Gates",
                     R"MARKDOWN(
 Swaps two qubits.
 
-- Parens Arguments:
+Parens Arguments:
 
     This instruction takes no parens arguments.
 
-- Targets:
+Targets:
 
     Qubit pairs to operate on.
 )MARKDOWN",
                     {{1, 0, 0, 0}, {0, 0, 1, 0}, {0, 1, 0, 0}, {0, 0, 0, 1}},
                     {"+IX", "+IZ", "+XI", "+ZI"},
                     R"CIRCUIT(
 CNOT 0 1
@@ -70,19 +70,19 @@
             []() -> ExtraGateData {
                 return {
                     "C_Two Qubit Clifford Gates",
                     R"MARKDOWN(
 Swaps two qubits and phases the -1 eigenspace of the ZZ observable by i.
 Equivalent to `SWAP` then `CZ` then `S` on both targets.
 
-- Parens Arguments:
+Parens Arguments:
 
     This instruction takes no parens arguments.
 
-- Targets:
+Targets:
 
     Qubit pairs to operate on.
 )MARKDOWN",
                     {{1, 0, 0, 0}, {0, 0, i, 0}, {0, i, 0, 0}, {0, 0, 0, 1}},
                     {"+ZY", "+IZ", "+YZ", "+ZI"},
                     R"CIRCUIT(
 CNOT 0 1
@@ -106,19 +106,19 @@
             []() -> ExtraGateData {
                 return {
                     "C_Two Qubit Clifford Gates",
                     R"MARKDOWN(
 Swaps two qubits and phases the -1 eigenspace of the ZZ observable by -i.
 Equivalent to `SWAP` then `CZ` then `S_DAG` on both targets.
 
-- Parens Arguments:
+Parens Arguments:
 
     This instruction takes no parens arguments.
 
-- Targets:
+Targets:
 
     Qubit pairs to operate on.
 )MARKDOWN",
                     {{1, 0, 0, 0}, {0, 0, -i, 0}, {0, -i, 0, 0}, {0, 0, 0, 1}},
                     {"-ZY", "+IZ", "-YZ", "+ZI"},
                     R"CIRCUIT(
 CNOT 0 1
```

### Comparing `stim-1.8.0/src/stim/circuit/gate_target.cc` & `stim-1.9.0/src/stim/circuit/gate_target.cc`

 * *Files 2% similar despite different names*

```diff
@@ -37,16 +37,16 @@
 GateTarget GateTarget::qubit(uint32_t qubit, bool inverted) {
     if (qubit != (qubit & TARGET_VALUE_MASK)) {
         throw std::invalid_argument("qubit target larger than " + std::to_string(TARGET_VALUE_MASK));
     }
     return {qubit | (TARGET_INVERTED_BIT * inverted)};
 }
 GateTarget GateTarget::rec(int32_t lookback) {
-    if (lookback >= 0 || lookback < -(int32_t)TARGET_VALUE_MASK) {
-        throw std::invalid_argument("lookback further than " + std::to_string(-(int32_t)TARGET_VALUE_MASK));
+    if (lookback >= 0 || lookback <= -(1 << 24)) {
+        throw std::out_of_range("Need -16777215 <= lookback <= -1");
     }
     return {((uint32_t)-lookback) | TARGET_RECORD_BIT};
 }
 GateTarget GateTarget::sweep_bit(uint32_t index) {
     return {index | TARGET_SWEEP_BIT};
 }
 GateTarget GateTarget::combiner() {
```

### Comparing `stim-1.8.0/src/stim/dem/detector_error_model.cc` & `stim-1.9.0/src/stim/dem/detector_error_model.cc`

 * *Files 2% similar despite different names*

```diff
@@ -576,14 +576,37 @@
 void DetectorErrorModel::clear() {
     target_buf.clear();
     arg_buf.clear();
     instructions.clear();
     blocks.clear();
 }
 
+DetectorErrorModel DetectorErrorModel::rounded(uint8_t sig_figs) const {
+    double scale = 1;
+    for (size_t k = 0; k < sig_figs; k++) {
+        scale *= 10;
+    }
+
+    DetectorErrorModel result;
+    for (const auto &e : instructions) {
+        if (e.type == DEM_REPEAT_BLOCK) {
+            auto reps = e.target_data[0].data;
+            auto &block = blocks[e.target_data[1].data];
+            result.append_repeat_block(reps, block.rounded(sig_figs));
+        } else {
+            std::vector<double> rounded_args;
+            for (auto a : e.arg_data) {
+                rounded_args.push_back(round(a * scale) / scale);
+            }
+            result.append_dem_instruction({rounded_args, e.target_data, e.type});
+        }
+    }
+    return result;
+}
+
 uint64_t DetectorErrorModel::total_detector_shift() const {
     uint64_t result = 0;
     for (const auto &e : instructions) {
         if (e.type == DEM_SHIFT_DETECTORS) {
             result += e.target_data[0].data;
         } else if (e.type == DEM_REPEAT_BLOCK) {
             result += e.target_data[0].data * blocks[e.target_data[1].data].total_detector_shift();
@@ -765,78 +788,95 @@
     std::vector<double> &coord_shift,
     uint64_t &detector_offset,
     std::map<uint64_t, std::vector<double>> &out,
     bool top) {
     if (iter_desired_detector_index == included_detector_indices.end()) {
         return true;
     }
-    uint64_t smallest_desired_detector_index = *iter_desired_detector_index;
 
-    auto found_result = [&](uint64_t index, ConstPointerRange<double> data) {
-        if (included_detector_indices.find(index) == included_detector_indices.end()) {
+    // Fills in data for a detector that was found while iterating.
+    // Returns true if all data has been filled in.
+    auto fill_in_data = [&](uint64_t fill_index, ConstPointerRange<double> fill_data) {
+        if (included_detector_indices.find(fill_index) == included_detector_indices.end()) {
+            // Not interested in the index for this data.
             return false;
         }
-        if (out.find(index) != out.end()) {
+        if (out.find(fill_index) != out.end()) {
+            // Already have this data. Detector may have been declared twice?
             return false;
         }
 
+        // Write data to result dictionary.
         std::vector<double> det_coords;
-        for (size_t k = 0; k < data.size(); k++) {
-            det_coords.push_back(data[k]);
+        det_coords.reserve(fill_data.size());
+        for (size_t k = 0; k < fill_data.size(); k++) {
+            det_coords.push_back(fill_data[k]);
             if (k < coord_shift.size()) {
                 det_coords[k] += coord_shift[k];
             }
         }
-        out[index] = std::move(det_coords);
+        out[fill_index] = std::move(det_coords);
 
-        while (out.find(smallest_desired_detector_index) != out.end()) {
+        // Advance the iterator past values that have been written in.
+        // If the end has been reached, we're done.
+        while (out.find(*iter_desired_detector_index) != out.end()) {
             iter_desired_detector_index++;
             if (iter_desired_detector_index == included_detector_indices.end()) {
                 return true;
             }
-            smallest_desired_detector_index = *iter_desired_detector_index;
         }
+
         return false;
     };
 
     for (const auto &op : dem.instructions) {
         if (op.type == DEM_SHIFT_DETECTORS) {
             vec_pad_add_mul(coord_shift, op.arg_data);
             detector_offset += op.target_data[0].data;
-            while (smallest_desired_detector_index < detector_offset) {
-                if (found_result(smallest_desired_detector_index, {})) {
+            while (*iter_desired_detector_index < detector_offset) {
+                // Shifting past an index proves that it will never be given data.
+                // So set the coordinate data to the empty list.
+                if (fill_in_data(*iter_desired_detector_index, {})) {
                     return true;
                 }
             }
 
         } else if (op.type == DEM_DETECTOR) {
             for (const auto &t : op.target_data) {
-                if (found_result(t.data + detector_offset, op.arg_data)) {
+                if (fill_in_data(t.data + detector_offset, op.arg_data)) {
                     return true;
                 }
             }
 
         } else if (op.type == DEM_REPEAT_BLOCK) {
             const auto &block = dem.blocks[op.target_data[1].data];
             uint64_t reps = op.target_data[0].data;
 
             // TODO: Finish in time proportional to len(instructions) + len(desired) instead of len(execution).
             for (uint64_t k = 0; k < reps; k++) {
                 if (get_detector_coordinates_helper(
-                    block, included_detector_indices, iter_desired_detector_index, coord_shift, detector_offset, out, false)) {
+                        block,
+                        included_detector_indices,
+                        iter_desired_detector_index,
+                        coord_shift,
+                        detector_offset,
+                        out,
+                        false)) {
                     return true;
                 }
             }
         }
     }
 
+    // If we've reached the end of the detector error model, then all remaining
+    // values should be given empty data.
     if (top && out.size() < included_detector_indices.size()) {
         uint64_t n = dem.count_detectors();
-        while (smallest_desired_detector_index < n) {
-            if (found_result(smallest_desired_detector_index, {})) {
+        while (*iter_desired_detector_index < n) {
+            if (fill_in_data(*iter_desired_detector_index, {})) {
                 return true;
             }
         }
     }
 
     return false;
 }
```

### Comparing `stim-1.8.0/src/stim/dem/detector_error_model.pybind.cc` & `stim-1.9.0/src/stim/dem/detector_error_model.pybind.cc`

 * *Files 6% similar despite different names*

```diff
@@ -10,22 +10,26 @@
 // distributed under the License is distributed on an "AS IS" BASIS,
 // WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 // See the License for the specific language governing permissions and
 // limitations under the License.
 
 #include "stim/dem/detector_error_model.pybind.h"
 
+#include <fstream>
+
 #include "stim/circuit/circuit.pybind.h"
 #include "stim/dem/detector_error_model_instruction.pybind.h"
 #include "stim/dem/detector_error_model_repeat_block.pybind.h"
 #include "stim/dem/detector_error_model_target.pybind.h"
+#include "stim/io/raii_file.h"
 #include "stim/py/base.pybind.h"
-#include "stim/simulators/min_distance.h"
+#include "stim/search/search.h"
 
 using namespace stim;
+using namespace stim_pybind;
 
 std::string detector_error_model_repr(const DetectorErrorModel &self) {
     if (self.instructions.empty()) {
         return "stim.DetectorErrorModel()";
     }
     std::stringstream ss;
     ss << "stim.DetectorErrorModel('''\n";
@@ -66,15 +70,14 @@
     throw std::invalid_argument("Not a non-block detector error model instruction name: " + name);
 }
 
 void pybind_detector_error_model(pybind11::module &m) {
     auto c = pybind11::class_<DetectorErrorModel>(
         m,
         "DetectorErrorModel",
-        pybind11::module_local(),
         clean_doc_string(u8R"DOC(
             A list of instructions describing error mechanisms in terms of the detection events they produce.
 
             Examples:
                 >>> import stim
                 >>> model = stim.DetectorErrorModel('''
                 ...     error(0.125) D0
@@ -317,14 +320,16 @@
             result.arguments.insert(result.arguments.begin(), op.arg_data.begin(), op.arg_data.end());
             result.type = op.type;
             return pybind11::cast(result);
         },
         pybind11::arg("index_or_slice"),
         clean_doc_string(u8R"DOC(
             Returns copies of instructions from the detector error model.
+            @overload def __getitem__(self, index_or_slice: int) -> Union[stim.DemInstruction, stim.DemRepeatBlock]:
+            @overload def __getitem__(self, index_or_slice: slice) -> stim.DetectorErrorModel:
 
             Args:
                 index_or_slice: An integer index picking out an instruction to return, or a slice picking out a range
                     of instructions to return as a detector error model.
 
             Examples:
             Examples:
@@ -754,37 +759,165 @@
                 minimum sized logical error is likely to use Y errors. But each Y error decomposes into two graphlike
                 components (the X part and the Z part). As a result, the graphlike code distance in that context is
                 likely to be nearly twice as large as the true code distance.
 
             Examples:
                 >>> import stim
 
-                >>> stim.DetectorErrorModel("""
+                >>> stim.DetectorErrorModel('''
                 ...     error(0.125) D0
                 ...     error(0.125) D0 D1
                 ...     error(0.125) D1 L55
                 ...     error(0.125) D1
-                ... """).shortest_graphlike_error()
+                ... ''').shortest_graphlike_error()
                 stim.DetectorErrorModel('''
                     error(1) D1
                     error(1) D1 L55
                 ''')
 
-                >>> stim.DetectorErrorModel("""
+                >>> stim.DetectorErrorModel('''
                 ...     error(0.125) D0 D1 D2
                 ...     error(0.125) L0
-                ... """).shortest_graphlike_error(ignore_ungraphlike_errors=True)
+                ... ''').shortest_graphlike_error(ignore_ungraphlike_errors=True)
                 stim.DetectorErrorModel('''
                     error(1) L0
                 ''')
 
                 >>> circuit = stim.Circuit.generated(
                 ...     "repetition_code:memory",
                 ...     rounds=10,
                 ...     distance=7,
                 ...     before_round_data_depolarization=0.01)
                 >>> model = circuit.detector_error_model(decompose_errors=True)
                 >>> len(model.shortest_graphlike_error())
                 7
         )DOC")
             .data());
+
+    c.def_static(
+        "from_file",
+        [](pybind11::object &obj) {
+            try {
+                auto path = pybind11::cast<std::string>(obj);
+                RaiiFile f(path.data(), "r");
+                return DetectorErrorModel::from_file(f.f);
+            } catch (pybind11::cast_error &ex) {
+            }
+
+            auto py_path = pybind11::module::import("pathlib").attr("Path");
+            if (pybind11::isinstance(obj, py_path)) {
+                auto path = pybind11::cast<std::string>(pybind11::str(obj));
+                RaiiFile f(path.data(), "r");
+                return DetectorErrorModel::from_file(f.f);
+            }
+
+            auto py_text_io_base = pybind11::module::import("io").attr("TextIOBase");
+            if (pybind11::isinstance(obj, py_text_io_base)) {
+                auto contents = obj.attr("read")();
+                return DetectorErrorModel(pybind11::cast<std::string>(pybind11::str(contents)).data());
+            }
+
+            throw std::invalid_argument(
+                "Don't know how to read from " + pybind11::cast<std::string>(pybind11::str(obj)));
+        },
+        pybind11::arg("file"),
+        clean_doc_string(u8R"DOC(
+            Args:
+                file: A file path or open file object to read from.
+
+            Returns:
+                The circuit parsed from the file.
+
+            Examples:
+                >>> import stim
+                >>> import tempfile
+
+                >>> with tempfile.TemporaryDirectory() as tmpdir:
+                ...     path = tmpdir + '/tmp.stim'
+                ...     with open(path, 'w') as f:
+                ...         print('error(0.25) D2 D3', file=f)
+                ...     circuit = stim.DetectorErrorModel.from_file(path)
+                >>> circuit
+                stim.DetectorErrorModel('''
+                    error(0.25) D2 D3
+                ''')
+
+                >>> with tempfile.TemporaryDirectory() as tmpdir:
+                ...     path = tmpdir + '/tmp.stim'
+                ...     with open(path, 'w') as f:
+                ...         print('error(0.25) D2 D3', file=f)
+                ...     with open(path) as f:
+                ...         circuit = stim.DetectorErrorModel.from_file(path)
+                >>> circuit
+                stim.DetectorErrorModel('''
+                    error(0.25) D2 D3
+                ''')
+        )DOC")
+            .data());
+
+    c.def(
+        "to_file",
+        [](const DetectorErrorModel &self, pybind11::object &obj) {
+            try {
+                auto path = pybind11::cast<std::string>(obj);
+                std::ofstream out(path, std::ofstream::out);
+                if (!out.is_open()) {
+                    throw std::invalid_argument("Failed to open " + path);
+                }
+                out << self << '\n';
+                return;
+            } catch (pybind11::cast_error &ex) {
+            }
+
+            auto py_path = pybind11::module::import("pathlib").attr("Path");
+            if (pybind11::isinstance(obj, py_path)) {
+                auto path = pybind11::cast<std::string>(pybind11::str(obj));
+                std::ofstream out(path, std::ofstream::out);
+                if (!out.is_open()) {
+                    throw std::invalid_argument("Failed to open " + path);
+                }
+                out << self << '\n';
+                return;
+            }
+
+            auto py_text_io_base = pybind11::module::import("io").attr("TextIOBase");
+            if (pybind11::isinstance(obj, py_text_io_base)) {
+                obj.attr("write")(pybind11::str(self.str()));
+                obj.attr("write")(pybind11::str("\n"));
+                return;
+            }
+
+            throw std::invalid_argument(
+                "Don't know how to write to " + pybind11::cast<std::string>(pybind11::str(obj)));
+        },
+        pybind11::arg("file"),
+        clean_doc_string(u8R"DOC(
+            @signature def to_file(self, file: Union[io.TextIOBase, str, pathlib.Path]) -> None:
+            Writes the stim circuit to a file.
+
+            Args:
+                file: A file path or an open file to write to.
+
+            Examples:
+                >>> import stim
+                >>> import tempfile
+                >>> c = stim.DetectorErrorModel('error(0.25) D2 D3')
+
+                >>> with tempfile.TemporaryDirectory() as tmpdir:
+                ...     path = tmpdir + '/tmp.stim'
+                ...     with open(path, 'w') as f:
+                ...         c.to_file(f)
+                ...     with open(path) as f:
+                ...         contents = f.read()
+                >>> contents
+                'error(0.25) D2 D3\n'
+
+                >>> with tempfile.TemporaryDirectory() as tmpdir:
+                ...     path = tmpdir + '/tmp.stim'
+                ...     c.to_file(path)
+                ...     with open(path) as f:
+                ...         contents = f.read()
+                >>> contents
+                'error(0.25) D2 D3\n'
+        )DOC")
+            .data());
 }
```

### Comparing `stim-1.8.0/src/stim/dem/detector_error_model_instruction.pybind.cc` & `stim-1.9.0/src/stim/dem/detector_error_model_instruction.pybind.cc`

 * *Files 4% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 
 #include "stim/dem/detector_error_model_instruction.pybind.h"
 
 #include "stim/dem/detector_error_model.pybind.h"
 #include "stim/py/base.pybind.h"
 
 using namespace stim;
+using namespace stim_pybind;
 
 DemInstruction ExposedDemInstruction::as_dem_instruction() const {
     return DemInstruction{arguments, targets, type};
 }
 
 std::string ExposedDemInstruction::type_name() const {
     std::stringstream out;
@@ -82,15 +83,14 @@
     return arguments;
 }
 
 void pybind_detector_error_model_instruction(pybind11::module &m) {
     auto c = pybind11::class_<ExposedDemInstruction>(
         m,
         "DemInstruction",
-        pybind11::module_local(),
         clean_doc_string(u8R"DOC(
             An instruction from a detector error model.
 
             Examples:
                 >>> import stim
                 >>> model = stim.DetectorErrorModel('''
                 ...     error(0.125) D0
@@ -174,15 +174,19 @@
     c.def(
         "args_copy",
         &ExposedDemInstruction::args_copy,
         "Returns a copy of the list of numbers parameterizing the instruction (e.g. the probability of an error).");
     c.def(
         "targets_copy",
         &ExposedDemInstruction::targets_copy,
-        "Returns a copy of the list of objects the instruction applies to (e.g. affected detectors.");
+        clean_doc_string(u8R"DOC(
+            Returns a copy of the list of objects the instruction applies to (e.g. affected detectors.
+            @signature def targets_copy(self) -> List[Union[int, stim.DemTarget]]:
+        )DOC")
+            .data());
     c.def_property_readonly(
         "type",
         &ExposedDemInstruction::type_name,
         clean_doc_string(u8R"DOC(
             The name of the instruction type (e.g. "error" or "shift_detectors").
         )DOC")
             .data());
```

### Comparing `stim-1.8.0/src/stim/dem/detector_error_model_repeat_block.pybind.cc` & `stim-1.9.0/src/stim/dem/detector_error_model_repeat_block.pybind.cc`

 * *Files 1% similar despite different names*

```diff
@@ -15,20 +15,20 @@
 #include "stim/dem/detector_error_model_repeat_block.pybind.h"
 
 #include "stim/dem/detector_error_model.pybind.h"
 #include "stim/dem/detector_error_model_instruction.pybind.h"
 #include "stim/py/base.pybind.h"
 
 using namespace stim;
+using namespace stim_pybind;
 
 void pybind_detector_error_model_repeat_block(pybind11::module &m) {
     auto c = pybind11::class_<ExposedDemRepeatBlock>(
         m,
         "DemRepeatBlock",
-        pybind11::module_local(),
         clean_doc_string(u8R"DOC(
             A repeat block from a detector error model.
 
             Examples:
                 >>> import stim
                 >>> model = stim.DetectorErrorModel('''
                 ...     repeat 100 {
@@ -49,15 +49,15 @@
         pybind11::arg("repeat_count"),
         pybind11::arg("block"),
         clean_doc_string(u8R"DOC(
             Creates a stim.DemRepeatBlock.
 
             Args:
                 repeat_count: The number of times the repeat block's body is supposed to execute.
-                body: The body of the repeat block as a DetectorErrorModel containing the instructions to repeat.
+                block: The body of the repeat block as a DetectorErrorModel containing the instructions to repeat.
 
             Examples:
                 >>> import stim
                 >>> repeat_block = stim.DemRepeatBlock(100, stim.DetectorErrorModel('''
                 ...     error(0.125) D0 D1
                 ...     shift_detectors 1
                 ... '''))
```

### Comparing `stim-1.8.0/src/stim/dem/detector_error_model_target.pybind.cc` & `stim-1.9.0/src/stim/dem/detector_error_model_target.pybind.cc`

 * *Files 2% similar despite different names*

```diff
@@ -14,18 +14,19 @@
 
 #include "stim/dem/detector_error_model_target.pybind.h"
 
 #include "stim/dem/detector_error_model.pybind.h"
 #include "stim/py/base.pybind.h"
 
 using namespace stim;
+using namespace stim_pybind;
 
-void pybind_detector_error_model_target(pybind11::module &m) {
+void stim_pybind::pybind_detector_error_model_target(pybind11::module &m) {
     auto c = pybind11::class_<ExposedDemTarget>(
-        m, "DemTarget", pybind11::module_local(), "An instruction target from a detector error model (.dem) file.");
+        m, "DemTarget", "An instruction target from a detector error model (.dem) file.");
 
     m.def(
         "target_relative_detector_id",
         &ExposedDemTarget::relative_detector_id,
         pybind11::arg("index"),
         clean_doc_string(u8R"DOC(
             Returns a relative detector id (e.g. "D5" in a .dem file).
```

### Comparing `stim-1.8.0/src/stim/gen/circuit_gen_main.cc` & `stim-1.9.0/src/stim/gen/circuit_gen_main.cc`

 * *Files identical despite different names*

### Comparing `stim-1.8.0/src/stim/gen/circuit_gen_params.cc` & `stim-1.9.0/src/stim/gen/circuit_gen_params.cc`

 * *Files identical despite different names*

### Comparing `stim-1.8.0/src/stim/gen/gen_color_code.cc` & `stim-1.9.0/src/stim/gen/gen_color_code.cc`

 * *Files identical despite different names*

### Comparing `stim-1.8.0/src/stim/gen/gen_rep_code.cc` & `stim-1.9.0/src/stim/gen/gen_rep_code.cc`

 * *Files identical despite different names*

### Comparing `stim-1.8.0/src/stim/gen/gen_surface_code.cc` & `stim-1.9.0/src/stim/gen/gen_surface_code.cc`

 * *Files identical despite different names*

### Comparing `stim-1.8.0/src/stim/help.cc` & `stim-1.9.0/src/stim/help.cc`

 * *Files 2% similar despite different names*

```diff
@@ -353,14 +353,33 @@
 
 CAUTION: simulation results *MAY NOT* be consistent if you vary other flags and modes. For example,
 `--skip_reference_sample` may result in fewer calls the to the random number generator before reported
 sampling begins. More generally, using the same seed for `stim sample` and `stim detect` will not
 result in detection events corresponding to the measurement results.
 )PARAGRAPH";
 
+    flags["--sweep"] = R"PARAGRAPH(Specifies a per-shot sweep data file.
+
+Sweep bits are used to vary whether certain Pauli gates are included in a circuit, or not, from shot to shot.
+For example, if a circuit contains the instruction "CX sweep[5] 0" then there is an X pauli that is included
+only in shots where the corresponding sweep data has the bit at index 5 set to True.
+)PARAGRAPH";
+
+    flags["--sweep_format"] = R"PARAGRAPH(Specifies the format sweep data is stored in (e.g. b8 or 01).
+)PARAGRAPH";
+
+    flags["--obs_out"] = R"PARAGRAPH(Specifies a file to write observable flip data to.
+
+When sampling detection event data, this is an alternative to --append_observables which has the benefit
+of never mixing the two types of data together.
+)PARAGRAPH";
+
+    flags["--obs_out_format"] = R"PARAGRAPH(The format to use when writing observable flip data (e.g. b8 or 01).
+)PARAGRAPH";
+
     modes["analyze_errors"] = CommandLineSingleModeData{
         "Converts a circuit into a detector error model.",
         R"PARAGRAPH(
 Determines the detectors and logical observables that are flipped by each error channel in the given circuit, and
 summarizes this information as an error model framed entirely in terms of independent error mechanisms that flip sets of
 detectors and observables.
 
@@ -370,16 +389,14 @@
 
 stderr:
     Circuit failed to parse.
     Failed to produce a graphlike detector error model but `--decompose_errors` was set.
     Circuit contained gauge detectors but `--allow_gauge_detectors` wasn't set.
     Circuit contained disjoint error channels but `--approximate_disjoint_errors` wasn't set.
 
-Note: currently, the `ELSE_CORRELATED_ERROR` instruction is not supported by this mode.
-
 - Example:
 
     ```
     >>> stim analyze_errors
     ... # Single-shot X-basis rep code circuit.
     ... RX 0 1 2 3 4 5 6
     ... MPP X0*X1 X1*X2 X2*X3 X3*X4 X4*X5 X5*X6
@@ -400,21 +417,45 @@
     error(0.125) D4 D5
     error(0.125) D5
     ```
 )PARAGRAPH",
         {
             "--allow_gauge_detectors",
             "--approximate_disjoint_errors",
+            "--block_decompose_from_introducing_remnant_edges",
+            "--ignore_decomposition_failures",
             "--decompose_errors",
             "--fold_loops",
             "--out",
             "--in",
         },
     };
 
+    flags["--ignore_decomposition_failures"] = R"PARAGRAPH(
+When this flag is set, circuit errors that fail to decompose into graphlike
+detector error model errors no longer cause the conversion process to abort.
+Instead, the undecomposed error is inserted into the output. Whatever processes
+the detector error model is then responsible for dealing with the undecomposed
+errors (e.g. a tool may choose to simply ignore them).
+
+Irrelevant unless --decompose_errors is specified.
+)PARAGRAPH";
+    flags["--block_decomposition_from_introducing_remnant_edges"] = R"PARAGRAPH(
+Requires that both A B and C D be present elsewhere in the detector error model
+in order to decompose A B C D into A B ^ C D. Normally, only one of A B or C D
+needs to appear to allow this decomposition.
+
+Remnant edges can be a useful feature for ensuring decomposition succeeds, but
+they can also reduce the effective code distance by giving the decoder single
+edges that actually represent multiple errors in the circuit (resulting in the
+decoder making misinformed choices when decoding).
+
+Irrelevant unless --decompose_errors is specified.
+)PARAGRAPH";
+
     flags["--fold_loops"] = R"PARAGRAPH(
 Allows the output error model to contain `repeat` blocks.
 
 Analyzes `REPEAT` blocks in the input circuit using a procedure that solves the loop in O(period) iterations, instead of
 O(total_repetition_count) iterations, by using ["tortoise and hare"](https://en.wikipedia.org/wiki/Cycle_detection#Floyd's_tortoise_and_hare)
 period finding algorithm. The "period" of a loop is the number of iterations required for the logical observables to end
 up back in the same place and for any errors introduced in the current iteration to not affected any detectors defined
@@ -767,15 +808,15 @@
     if (decomposition != nullptr) {
         std::stringstream undecomposed;
         undecomposed << gate.name << " 0";
         if (gate.flags & GATE_TARGETS_PAIRS) {
             undecomposed << " 1";
         }
 
-        out << "- Decomposition (into H, S, CX, M, R):\n";
+        out << "Decomposition (into H, S, CX, M, R):\n";
         out.change_indent(+4);
         out << "```\n";
         out << "# The following circuit is equivalent (up to global phase) to `";
         out << undecomposed.str() << "`";
         out << decomposition;
         if (Circuit(decomposition) == Circuit(undecomposed.str().data())) {
             out << "\n# (The decomposition is trivial because this gate is in the target gate set.)\n";
@@ -783,15 +824,15 @@
         out << "```\n";
         out.change_indent(-4);
     }
 }
 
 void print_stabilizer_generators(Acc &out, const Gate &gate) {
     if (gate.flags & GATE_IS_UNITARY) {
-        out << "- Stabilizer Generators:\n";
+        out << "Stabilizer Generators:\n";
         out.change_indent(+4);
         out << "```\n";
         auto tableau = gate.tableau();
         if (gate.flags & GATE_TARGETS_PAIRS) {
             out << "X_ -> " << tableau.xs[0] << "\n";
             out << "Z_ -> " << tableau.zs[0] << "\n";
             out << "_X -> " << tableau.xs[1] << "\n";
@@ -801,15 +842,15 @@
             out << "Z -> " << tableau.zs[0] << "\n";
         }
         out << "```\n";
         out.change_indent(-4);
     } else {
         auto data = gate.extra_data_func();
         if (data.tableau_data.size()) {
-            out << "- Stabilizer Generators:\n";
+            out << "Stabilizer Generators:\n";
             out.change_indent(+4);
             out << "```\n";
             for (const auto &e : data.tableau_data) {
                 out << e << "\n";
             }
             out << "```\n";
             out.change_indent(-4);
@@ -818,15 +859,15 @@
 }
 
 void print_bloch_vector(Acc &out, const Gate &gate) {
     if (!(gate.flags & GATE_IS_UNITARY) || (gate.flags & GATE_TARGETS_PAIRS)) {
         return;
     }
 
-    out << "- Bloch Rotation:\n";
+    out << "Bloch Rotation:\n";
     out.change_indent(+4);
     out << "```\n";
     auto matrix = gate.unitary();
     auto a = matrix[0][0];
     auto b = matrix[0][1];
     auto c = matrix[1][0];
     auto d = matrix[1][1];
@@ -884,15 +925,15 @@
 }
 
 void print_unitary_matrix(Acc &out, const Gate &gate) {
     if (!(gate.flags & GATE_IS_UNITARY)) {
         return;
     }
     auto matrix = gate.unitary();
-    out << "- Unitary Matrix:\n";
+    out << "Unitary Matrix:\n";
     out.change_indent(+4);
     bool all_halves = true;
     bool all_sqrt_halves = true;
     double s = sqrt(0.5);
     for (const auto &row : matrix) {
         for (const auto &cell : row) {
             all_halves &= cell.real() == 0.5 || cell.real() == 0 || cell.real() == -0.5;
@@ -934,17 +975,21 @@
 }
 
 std::string generate_per_gate_help_markdown(const Gate &alt_gate, int indent, bool anchor) {
     Acc out;
     out.indent = indent;
     const Gate &gate = GATE_DATA.at(alt_gate.name);
     if (anchor) {
-        out << "<a name=\"" << alt_gate.name << "\"></a>";
+        out << "<a name=\"" << alt_gate.name << "\"></a>\n";
+    }
+    if (gate.flags & GATE_IS_UNITARY) {
+        out << "### The '" << alt_gate.name << "' Gate\n";
+    } else {
+        out << "### The '" << alt_gate.name << "' Instruction\n";
     }
-    out << "**`" << alt_gate.name << "`**\n";
     for (const auto &other : GATE_DATA.gates()) {
         if (other.id == alt_gate.id && other.name != alt_gate.name) {
             out << "\nAlternate name: ";
             if (anchor) {
                 out << "<a name=\"" << other.name << "\"></a>";
             }
             out << "`" << other.name << "`\n";
@@ -1185,15 +1230,15 @@
         }
     }
     all << "\n";
     for (auto &category : categories) {
         all << "## " << category.first.substr(2) << "\n\n";
         for (const auto &name : category.second) {
             if (name == GATE_DATA.at(name).name) {
-                all << "- " << generate_per_gate_help_markdown(GATE_DATA.at(name), 4, true) << "\n";
+                all << generate_per_gate_help_markdown(GATE_DATA.at(name), 0, true) << "\n";
             }
         }
     }
     result[std::string("GATES_MARKDOWN")] = all.str();
 
     return result;
 }
```

### Comparing `stim-1.8.0/src/stim/io/measure_record.cc` & `stim-1.9.0/src/stim/io/measure_record.cc`

 * *Files identical despite different names*

### Comparing `stim-1.8.0/src/stim/io/measure_record_batch.cc` & `stim-1.9.0/src/stim/io/measure_record_batch.cc`

 * *Files identical despite different names*

### Comparing `stim-1.8.0/src/stim/io/measure_record_batch_writer.cc` & `stim-1.9.0/src/stim/io/measure_record_batch_writer.cc`

 * *Files 2% similar despite different names*

```diff
@@ -14,23 +14,24 @@
  * limitations under the License.
  */
 
 #include "stim/io/measure_record_batch_writer.h"
 
 #include <algorithm>
 
-#include "stim/io/measure_record_batch.h"
-
 using namespace stim;
 
 MeasureRecordBatchWriter::MeasureRecordBatchWriter(FILE *out, size_t num_shots, SampleFormat output_format)
     : output_format(output_format), out(out) {
     if (num_shots > 768) {
         throw std::out_of_range("num_shots > 768 (safety check to ensure staying away from linux file handle limit)");
     }
+    if (output_format == SAMPLE_FORMAT_PTB64 && num_shots % 64 != 0) {
+        throw std::out_of_range("Number of shots must be a multiple of 64 to use output format ptb64.");
+    }
     auto f = output_format;
     auto s = num_shots;
     if (output_format == SAMPLE_FORMAT_PTB64) {
         f = SAMPLE_FORMAT_B8;
         s += 63;
         s /= 64;
     }
```

### Comparing `stim-1.8.0/src/stim/io/measure_record_writer.cc` & `stim-1.9.0/src/stim/io/measure_record_writer.cc`

 * *Files 3% similar despite different names*

```diff
@@ -226,36 +226,27 @@
     const simd_bits &reference_sample,
     const simd_bit_table &table,
     SampleFormat format,
     char dets_prefix_1,
     char dets_prefix_2,
     size_t dets_prefix_transition) {
     if (format == SAMPLE_FORMAT_PTB64) {
+        if (num_shots % 64 != 0) {
+            throw std::invalid_argument("shots must be a multiple of 64 to use ptb64 format.");
+        }
         auto f64 = num_shots >> 6;
         for (size_t s = 0; s < f64; s++) {
             for (size_t m = 0; m < num_measurements; m++) {
                 uint64_t v = table[m].u64[s];
                 if (m < reference_sample.num_bits_padded() && reference_sample[m]) {
                     v = ~v;
                 }
                 fwrite(&v, 1, 64 >> 3, out);
             }
         }
-        if (num_shots & 63) {
-            uint64_t mask = (uint64_t{1} << (num_shots & 63)) - 1ULL;
-            for (size_t m = 0; m < num_measurements; m++) {
-                uint64_t v = table[m].u64[f64];
-                if (m < reference_sample.num_bits_padded() && reference_sample[m]) {
-                    v = ~v;
-                }
-                v &= mask;
-                fwrite(&v, 1, 64 >> 3, out);
-            }
-        }
-        return;
     } else {
         auto result = transposed_vs_ref(num_shots, table, reference_sample);
         if (dets_prefix_transition == 0) {
             dets_prefix_transition = num_measurements;
             dets_prefix_1 = dets_prefix_2;
         } else if (dets_prefix_1 == dets_prefix_2 || dets_prefix_transition >= num_measurements) {
             dets_prefix_transition = num_measurements;
```

### Comparing `stim-1.8.0/src/stim/io/sparse_shot.cc` & `stim-1.9.0/src/stim/io/sparse_shot.cc`

 * *Files identical despite different names*

### Comparing `stim-1.8.0/src/stim/io/stim_data_formats.cc` & `stim-1.9.0/src/stim/io/stim_data_formats.cc`

 * *Files 18% similar despite different names*

```diff
@@ -140,67 +140,75 @@
 The ptb64 format is a dense SIMD-focused binary format that stores shots as partially transposed bit-packed data.
 
 Each 64 bit word (8 bytes) of the data contains bits from the same measurement result across 64 separate shots. The next
 8 bytes contain bits for the next measurement result from the 64 separate shots. This continues until the 8 bytes
 containing the bits from the last measurement result, and then starts over again with data from the next 64 shots (if
 there are more).
 
-The shots are stored by byte order then significant order. The first shot's data goes into the least significant bit of
-the first byte of each 8 byte group. When the number of shots is not a multiple of 64, the bits corresponding to the
-missing shots are always zero.
+The shots are stored by byte order then significance order. The first shot's data goes into the least significant bit of
+the first byte of each 8 byte group.
 
-This format requires the reader to know the number of bits in each shot.
+This format requires the number of shots to be a multiple of 64.
 This format requires the reader to know the number of shots that were taken.
 
 This format is generally more tedious to work with, but useful for achieving good performance on data processing tasks
 where it is possible to parallelize across shots using SIMD instructions.
 
 *Example of producing ptb64 format data using stim's python API:*
 
     >>> import pathlib
     >>> import stim
     >>> import tempfile
     >>> with tempfile.TemporaryDirectory() as d:
     ...     path = str(pathlib.Path(d) / "tmp.dat")
     ...     stim.Circuit("""
     ...         X 1
-    ...         M 0 0 0 0 1 1 1 1 0 0 1 1 0 1
-    ...     """).compile_sampler().sample_write(shots=10, filepath=path, format="ptb64")
+    ...         M 0 1
+    ...     """).compile_sampler().sample_write(shots=64, filepath=path, format="ptb64")
     ...     with open(path, 'rb') as f:
     ...         print(' '.join(hex(e)[2:] for e in f.read()))
-    0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 ff 3 0 0 0 0 0 0 ff 3 0 0 0 0 0 0 ff 3 0 0 0 0 0 0 ff 3 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 ff 3 0 0 0 0 0 0 ff 3 0 0 0 0 0 0 0 0 0 0 0 0 0 0 ff 3 0 0 0 0 0 0
+    0 0 0 0 0 0 0 0 ff ff ff ff ff ff ff ff
 )HELP",
             R"PYTHON(
 from typing import List
 
 def save_ptb64(shots: List[List[bool]]):
+    if len(shots) % 64 != 0:
+        raise ValueError("Number of shots must be a multiple of 64.")
+
     output = b""
     for shot_offset in range(0, len(shots), 64):
         bits_per_shot = len(shots[0])
         for measure_index in range(bits_per_shot):
             v = 0
-            for k in reversed(range(min(64, len(shots) - shot_offset))):
+            for k in range(64)[::-1]:
                 v <<= 1
                 v += shots[shot_offset + k][measure_index]
             output += v.to_bytes(8, 'little')
     return output
 )PYTHON",
             R"PYTHON(
 from typing import List
 
-def parse_ptb64(data: bytes, bits_per_shot: int, num_shots: int) -> List[List[bool]]:
-    result = [[False] * bits_per_shot for _ in range(num_shots)]
-    group_byte_stride = bits_per_shot * 8
-    for shot_offset in range(num_shots):
-        shot_group = shot_offset // 64
-        shot_stripe = shot_offset % 64
-        for measure_index in range(bits_per_shot):
-            byte_offset = group_byte_stride*shot_group + measure_index * 8 + shot_stripe // 8
-            bit = (data[byte_offset] >> (shot_stripe % 8)) % 2 == 1
-            result[shot_offset][measure_index] = bit
+def parse_ptb64(data: bytes, bits_per_shot: int) -> List[List[bool]]:
+    num_shot_groups = int(len(data) * 8 / bits_per_shot / 64)
+    if len(data) * 8 != num_shot_groups * 64 * bits_per_shot:
+        raise ValueError("Number of shots must be a multiple of 64.")
+
+    result = [[False] * bits_per_shot for _ in range(num_shot_groups * 64)]
+    for group_index in range(num_shot_groups):
+        group_bit_offset = 64 * bits_per_shot * group_index
+        for m in range(bits_per_shot):
+            m_bit_offset = m * 64
+            for shot in range(64):
+                bit_offset = group_bit_offset + m_bit_offset + shot
+                byte_offset = bit_offset // 8
+                bit = data[bit_offset // 8] & (1 << (bit_offset % 8)) != 0
+                s = group_index * 64 + shot
+                result[s][m] = bit
     return result
 )PYTHON",
         },
     },
 
     {
         "hits",
```

### Comparing `stim-1.8.0/src/stim/main_namespaced.cc` & `stim-1.9.0/src/stim/main_namespaced.cc`

 * *Files 10% similar despite different names*

```diff
@@ -61,20 +61,21 @@
         fclose(out);
     }
     return EXIT_SUCCESS;
 }
 
 int main_mode_detect(int argc, const char **argv) {
     check_for_unknown_arguments(
-        {"--seed", "--shots", "--append_observables", "--out_format", "--out", "--in"},
+        {"--seed", "--shots", "--append_observables", "--out_format", "--out", "--in", "--obs_out", "--obs_out_format"},
         {"--detect", "--prepend_observables"},
         "detect",
         argc,
         argv);
     const auto &out_format = find_enum_argument("--out_format", "01", format_name_to_enum_map, argc, argv);
+    const auto &obs_out_format = find_enum_argument("--obs_out_format", "01", format_name_to_enum_map, argc, argv);
     bool prepend_observables = find_bool_argument("--prepend_observables", argc, argv);
     if (prepend_observables) {
         std::cerr << "[DEPRECATION] Avoid using `--prepend_observables`. Data readers assume observables are appended, "
                      "not prepended.\n";
     }
     bool append_observables = find_bool_argument("--append_observables", argc, argv);
     uint64_t num_shots =
@@ -86,20 +87,36 @@
     }
     if (out_format.id == SAMPLE_FORMAT_DETS && !append_observables) {
         prepend_observables = true;
     }
 
     FILE *in = find_open_file_argument("--in", stdin, "r", argc, argv);
     FILE *out = find_open_file_argument("--out", stdout, "w", argc, argv);
+    FILE *obs_out = find_open_file_argument("--obs_out", stdout, "w", argc, argv);
+    if (obs_out == stdout) {
+        obs_out = nullptr;
+    }
     auto circuit = Circuit::from_file(in);
     if (in != stdin) {
         fclose(in);
     }
     auto rng = optionally_seeded_rng(argc, argv);
-    detector_samples_out(circuit, num_shots, prepend_observables, append_observables, out, out_format.id, rng);
+    detector_samples_out(
+        circuit,
+        num_shots,
+        prepend_observables,
+        append_observables,
+        out,
+        out_format.id,
+        rng,
+        obs_out,
+        obs_out_format.id);
+    if (obs_out != nullptr) {
+        fclose(obs_out);
+    }
     if (out != stdout) {
         fclose(out);
     }
     return EXIT_SUCCESS;
 }
 
 int main_mode_sample(int argc, const char **argv) {
@@ -153,77 +170,95 @@
             "--circuit",
             "--in_format",
             "--append_observables",
             "--out_format",
             "--out",
             "--in",
             "--skip_reference_sample",
+            "--sweep",
+            "--sweep_format",
+            "--obs_out",
+            "--obs_out_format",
         },
         {
             "--m2d",
-            // Not deprecated but still experimental:
-            "--sweep_data_in_format",
-            "--sweep_data_in",
         },
         "m2d",
         argc,
         argv);
     const auto &in_format = find_enum_argument("--in_format", nullptr, format_name_to_enum_map, argc, argv);
     const auto &out_format = find_enum_argument("--out_format", "01", format_name_to_enum_map, argc, argv);
-    const auto &frame_in_format =
-        find_enum_argument("--sweep_data_in_format", "01", format_name_to_enum_map, argc, argv);
+    const auto &sweep_format = find_enum_argument("--sweep_format", "01", format_name_to_enum_map, argc, argv);
+    const auto &obs_out_format = find_enum_argument("--obs_out_format", "01", format_name_to_enum_map, argc, argv);
     bool append_observables = find_bool_argument("--append_observables", argc, argv);
     bool skip_reference_sample = find_bool_argument("--skip_reference_sample", argc, argv);
     FILE *circuit_file = find_open_file_argument("--circuit", nullptr, "r", argc, argv);
     auto circuit = Circuit::from_file(circuit_file);
     fclose(circuit_file);
 
     FILE *in = find_open_file_argument("--in", stdin, "r", argc, argv);
     FILE *out = find_open_file_argument("--out", stdout, "w", argc, argv);
-    FILE *frame_in = find_open_file_argument("--sweep_data_in", stdin, "r", argc, argv);
-    if (frame_in == stdin) {
-        frame_in = nullptr;
+    FILE *sweep_in = find_open_file_argument("--sweep", stdin, "r", argc, argv);
+    FILE *obs_out = find_open_file_argument("--obs_out", stdout, "w", argc, argv);
+    if (sweep_in == stdin) {
+        sweep_in = nullptr;
+    }
+    if (obs_out == stdout) {
+        obs_out = nullptr;
     }
 
     stream_measurements_to_detection_events(
         in,
         in_format.id,
-        frame_in,
-        frame_in_format.id,
+        sweep_in,
+        sweep_format.id,
         out,
         out_format.id,
         circuit,
         append_observables,
-        skip_reference_sample);
+        skip_reference_sample,
+        obs_out,
+        obs_out_format.id);
     if (in != stdin) {
         fclose(in);
     }
+    if (sweep_in != nullptr) {
+        fclose(sweep_in);
+    }
+    if (obs_out != nullptr) {
+        fclose(obs_out);
+    }
     if (out != stdout) {
         fclose(out);
     }
     return EXIT_SUCCESS;
 }
 
 int main_mode_analyze_errors(int argc, const char **argv) {
     check_for_unknown_arguments(
         {
             "--allow_gauge_detectors",
             "--approximate_disjoint_errors",
+            "--block_decompose_from_introducing_remnant_edges",
             "--decompose_errors",
             "--fold_loops",
-            "--out",
+            "--ignore_decomposition_failures",
             "--in",
+            "--out",
         },
         {"--analyze_errors", "--detector_hypergraph"},
         "analyze_errors",
         argc,
         argv);
     bool decompose_errors = find_bool_argument("--decompose_errors", argc, argv);
     bool fold_loops = find_bool_argument("--fold_loops", argc, argv);
     bool allow_gauge_detectors = find_bool_argument("--allow_gauge_detectors", argc, argv);
+    bool ignore_decomposition_failures = find_bool_argument("--ignore_decomposition_failures", argc, argv);
+    bool block_decompose_from_introducing_remnant_edges =
+        find_bool_argument("--block_decompose_from_introducing_remnant_edges", argc, argv);
 
     const char *approximate_disjoint_errors_arg = find_argument("--approximate_disjoint_errors", argc, argv);
     float approximate_disjoint_errors_threshold = 0;
     if (approximate_disjoint_errors_arg != nullptr && *approximate_disjoint_errors_arg == '\0') {
         approximate_disjoint_errors_threshold = 1;
     } else {
         approximate_disjoint_errors_threshold =
@@ -234,15 +269,21 @@
     auto out_stream = find_output_stream_argument("--out", true, argc, argv);
     std::ostream &out = out_stream.stream();
     auto circuit = Circuit::from_file(in);
     if (in != stdin) {
         fclose(in);
     }
     out << ErrorAnalyzer::circuit_to_detector_error_model(
-               circuit, decompose_errors, fold_loops, allow_gauge_detectors, approximate_disjoint_errors_threshold)
+               circuit,
+               decompose_errors,
+               fold_loops,
+               allow_gauge_detectors,
+               approximate_disjoint_errors_threshold,
+               ignore_decomposition_failures,
+               block_decompose_from_introducing_remnant_edges)
         << "\n";
     return EXIT_SUCCESS;
 }
 
 int main_mode_repl(int argc, const char **argv) {
     check_for_unknown_arguments({}, {"--repl"}, "repl", argc, argv);
     auto rng = externally_seeded_rng();
```

### Comparing `stim-1.8.0/src/stim/mem/bit_ref.cc` & `stim-1.9.0/src/stim/mem/bit_ref.cc`

 * *Files identical despite different names*

### Comparing `stim-1.8.0/src/stim/mem/simd_bit_table.cc` & `stim-1.9.0/src/stim/mem/simd_bit_table.cc`

 * *Files identical despite different names*

### Comparing `stim-1.8.0/src/stim/mem/simd_bits.cc` & `stim-1.9.0/src/stim/mem/simd_bits.cc`

 * *Files identical despite different names*

### Comparing `stim-1.8.0/src/stim/mem/simd_bits_range_ref.cc` & `stim-1.9.0/src/stim/mem/simd_bits_range_ref.cc`

 * *Files identical despite different names*

### Comparing `stim-1.8.0/src/stim/mem/simd_compat.cc` & `stim-1.9.0/src/stim/mem/simd_compat.cc`

 * *Files identical despite different names*

### Comparing `stim-1.8.0/src/stim/mem/simd_util.cc` & `stim-1.9.0/src/stim/simulators/matched_error.pybind.h`

 * *Files 16% similar despite different names*

```diff
@@ -8,8 +8,15 @@
 //
 // Unless required by applicable law or agreed to in writing, software
 // distributed under the License is distributed on an "AS IS" BASIS,
 // WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 // See the License for the specific language governing permissions and
 // limitations under the License.
 
-#include "stim/mem/simd_util.h"
+#ifndef _STIM_SIMULATORS_MATCHED_ERROR_PYBIND_H
+#define _STIM_SIMULATORS_MATCHED_ERROR_PYBIND_H
+
+#include <pybind11/pybind11.h>
+
+void pybind_matched_error(pybind11::module &m);
+
+#endif
```

### Comparing `stim-1.8.0/src/stim/mem/sparse_xor_vec.cc` & `stim-1.9.0/src/stim/mem/sparse_xor_vec.cc`

 * *Files identical despite different names*

### Comparing `stim-1.8.0/src/stim/probability_util.cc` & `stim-1.9.0/src/stim/probability_util.cc`

 * *Files identical despite different names*

### Comparing `stim-1.8.0/src/stim/py/base.pybind.cc` & `stim-1.9.0/src/stim/py/base.pybind.cc`

 * *Files 10% similar despite different names*

```diff
@@ -16,33 +16,28 @@
 
 #include <memory>
 
 #include "stim/probability_util.h"
 
 using namespace stim;
 
-static std::shared_ptr<std::mt19937_64> shared_rng;
-
-std::shared_ptr<std::mt19937_64> PYBIND_SHARED_RNG(const pybind11::object &seed) {
-    if (seed.is(pybind11::none())) {
-        if (!shared_rng) {
-            shared_rng = std::make_shared<std::mt19937_64>(std::move(externally_seeded_rng()));
-        }
-        return shared_rng;
+std::shared_ptr<std::mt19937_64> stim_pybind::make_py_seeded_rng(const pybind11::object &seed) {
+    if (seed.is_none()) {
+        return std::make_shared<std::mt19937_64>(externally_seeded_rng());
     }
 
     try {
         uint64_t s = pybind11::cast<uint64_t>(seed) ^ INTENTIONAL_VERSION_SEED_INCOMPATIBILITY;
         return std::make_shared<std::mt19937_64>(s);
     } catch (const pybind11::cast_error &) {
         throw std::invalid_argument("Expected seed to be None or a 64 bit unsigned integer.");
     }
 }
 
-std::string clean_doc_string(const char *c) {
+std::string stim_pybind::clean_doc_string(const char *c) {
     // Skip leading empty lines.
     while (*c == '\n') {
         c++;
     }
 
     // Determine indentation using first non-empty line.
     size_t indent = 0;
@@ -67,15 +62,15 @@
             }
         }
     }
 
     return result;
 }
 
-bool normalize_index_or_slice(
+bool stim_pybind::normalize_index_or_slice(
     const pybind11::object &index_or_slice,
     size_t length,
     pybind11::ssize_t *start,
     pybind11::ssize_t *step,
     pybind11::ssize_t *slice_length) {
     try {
         *start = pybind11::cast<pybind11::ssize_t>(index_or_slice);
@@ -101,15 +96,15 @@
     pybind11::ssize_t stop;
     if (!slice.compute(length, start, &stop, step, slice_length)) {
         throw pybind11::error_already_set();
     }
     return true;
 }
 
-SampleFormat format_to_enum(const std::string &format) {
+SampleFormat stim_pybind::format_to_enum(const std::string &format) {
     auto found_format = format_name_to_enum_map.find(format);
     if (found_format == format_name_to_enum_map.end()) {
         std::stringstream msg;
         msg << "Unrecognized output format: '" << format << "'. Recognized formats are:\n";
         for (const auto &kv : format_name_to_enum_map) {
             msg << "    " << kv.first << "\n";
         }
```

### Comparing `stim-1.8.0/src/stim/py/compiled_detector_sampler.pybind.cc` & `stim-1.9.0/src/stim/py/compiled_detector_sampler.pybind.cc`

 * *Files 4% similar despite different names*

```diff
@@ -11,26 +11,29 @@
 // WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 // See the License for the specific language governing permissions and
 // limitations under the License.
 
 #include "stim/py/compiled_detector_sampler.pybind.h"
 
 #include "stim/circuit/circuit.pybind.h"
+#include "stim/io/raii_file.h"
 #include "stim/py/base.pybind.h"
 #include "stim/simulators/detection_simulator.h"
 #include "stim/simulators/frame_simulator.h"
+#include "stim/simulators/measurements_to_detection_events.pybind.h"
 #include "stim/simulators/tableau_simulator.h"
 
 using namespace stim;
+using namespace stim_pybind;
 
 CompiledDetectorSampler::CompiledDetectorSampler(Circuit circuit, std::shared_ptr<std::mt19937_64> prng)
     : dets_obs(circuit), circuit(std::move(circuit)), prng(prng) {
 }
 
-pybind11::array_t<uint8_t> CompiledDetectorSampler::sample(
+pybind11::array_t<bool> CompiledDetectorSampler::sample(
     size_t num_shots, bool prepend_observables, bool append_observables) {
     auto sample =
         detector_samples(circuit, dets_obs, num_shots, prepend_observables, append_observables, *prng).transposed();
 
     const simd_bits &flat = sample.data;
     std::vector<uint8_t> bytes;
     bytes.reserve(flat.num_bits_padded());
@@ -44,15 +47,15 @@
 
     size_t n = dets_obs.detectors.size() + dets_obs.observables.size() * (prepend_observables + append_observables);
 
     void *ptr = bytes.data();
     pybind11::ssize_t itemsize = sizeof(uint8_t);
     std::vector<pybind11::ssize_t> shape{(pybind11::ssize_t)num_shots, (pybind11::ssize_t)n};
     std::vector<pybind11::ssize_t> stride{(pybind11::ssize_t)sample.num_minor_bits_padded(), 1};
-    const std::string &format = pybind11::format_descriptor<uint8_t>::value;
+    const std::string &format = pybind11::format_descriptor<bool>::value;
     bool readonly = true;
     return pybind11::array_t<uint8_t>(pybind11::buffer_info(ptr, itemsize, format, 2, shape, stride, readonly));
 }
 
 pybind11::array_t<uint8_t> CompiledDetectorSampler::sample_bit_packed(
     size_t num_shots, bool prepend_observables, bool append_observables) {
     auto sample =
@@ -69,45 +72,52 @@
 }
 
 void CompiledDetectorSampler::sample_write(
     size_t num_samples,
     const std::string &filepath,
     const std::string &format,
     bool prepend_observables,
-    bool append_observables) {
+    bool append_observables,
+    const char *obs_out_filepath,
+    const std::string &obs_out_format) {
     auto f = format_to_enum(format);
-    FILE *out = fopen(filepath.data(), "w");
-    if (out == nullptr) {
-        throw std::invalid_argument("Failed to open '" + filepath + "' to write.");
-    }
-    detector_samples_out(circuit, num_samples, prepend_observables, append_observables, out, f, *prng);
-    fclose(out);
+    RaiiFile out(filepath.data(), "w");
+    RaiiFile obs_out(obs_out_filepath, "w");
+    auto parsed_obs_out_format = format_to_enum(obs_out_format);
+    detector_samples_out(
+        circuit,
+        num_samples,
+        prepend_observables,
+        append_observables,
+        out.f,
+        f,
+        *prng,
+        obs_out.f,
+        parsed_obs_out_format);
 }
 
 std::string CompiledDetectorSampler::repr() const {
     std::stringstream result;
     result << "stim.CompiledDetectorSampler(";
     result << circuit_repr(circuit);
     result << ")";
     return result.str();
 }
 
-CompiledDetectorSampler py_init_compiled_detector_sampler(const Circuit &circuit, const pybind11::object &seed) {
-    return CompiledDetectorSampler(circuit, PYBIND_SHARED_RNG(seed));
+CompiledDetectorSampler stim_pybind::py_init_compiled_detector_sampler(
+    const Circuit &circuit, const pybind11::object &seed) {
+    return CompiledDetectorSampler(circuit, make_py_seeded_rng(seed));
 }
 
-pybind11::class_<CompiledDetectorSampler> pybind_compiled_detector_sampler_class(pybind11::module &m) {
+pybind11::class_<CompiledDetectorSampler> stim_pybind::pybind_compiled_detector_sampler_class(pybind11::module &m) {
     return pybind11::class_<CompiledDetectorSampler>(
-        m,
-        "CompiledDetectorSampler",
-        pybind11::module_local(),
-        "An analyzed stabilizer circuit whose detection events can be sampled quickly.");
+        m, "CompiledDetectorSampler", "An analyzed stabilizer circuit whose detection events can be sampled quickly.");
 }
 
-void pybind_compiled_detector_sampler_methods(pybind11::class_<CompiledDetectorSampler> &c) {
+void stim_pybind::pybind_compiled_detector_sampler_methods(pybind11::class_<CompiledDetectorSampler> &c) {
     c.def(
         pybind11::init(&py_init_compiled_detector_sampler),
         pybind11::arg("circuit"),
         pybind11::kw_only(),
         pybind11::arg("seed") = pybind11::none(),
         clean_doc_string(u8R"DOC(
             Creates a detector sampler, which can sample the detectors (and optionally observables) in a circuit.
@@ -144,15 +154,15 @@
                 ...    CNOT 0 1
                 ...    X_ERROR(1.0) 0
                 ...    M 0 1
                 ...    DETECTOR rec[-1] rec[-2]
                 ... ''')
                 >>> s = c.compile_detector_sampler()
                 >>> s.sample(shots=1)
-                array([[1]], dtype=uint8)
+                array([[ True]])
         )DOC")
             .data());
 
     c.def(
         "sample",
         &CompiledDetectorSampler::sample,
         pybind11::arg("shots"),
@@ -211,14 +221,16 @@
         &CompiledDetectorSampler::sample_write,
         pybind11::arg("shots"),
         pybind11::kw_only(),
         pybind11::arg("filepath"),
         pybind11::arg("format") = "01",
         pybind11::arg("prepend_observables") = false,
         pybind11::arg("append_observables") = false,
+        pybind11::arg("obs_out_filepath") = nullptr,
+        pybind11::arg("obs_out_format") = "01",
         clean_doc_string(u8R"DOC(
             Samples detection events from the circuit and writes them to a file.
 
             Examples:
                 >>> import stim
                 >>> import tempfile
                 >>> with tempfile.TemporaryDirectory() as d:
@@ -238,14 +250,19 @@
 
             Args:
                 shots: The number of times to sample every measurement in the circuit.
                 filepath: The file to write the results to.
                 format: The output format to write the results with.
                     Valid values are "01", "b8", "r8", "hits", "dets", and "ptb64".
                     Defaults to "01".
+                obs_out_filepath: Sample observables as part of each shot, and write them to this file.
+                    This keeps the observable data separate from the detector data.
+                obs_out_format: If writing the observables to a file, this is the format to write them in.
+                    Valid values are "01", "b8", "r8", "hits", "dets", and "ptb64".
+                    Defaults to "01".
                 prepend_observables: Sample observables as part of each shot, and put them at the start of the detector
                     data.
                 append_observables: Sample observables as part of each shot, and put them at the end of the detector
                     data.
 
             Returns:
                 None.
```

### Comparing `stim-1.8.0/src/stim/py/compiled_measurement_sampler.pybind.cc` & `stim-1.9.0/src/stim/py/compiled_measurement_sampler.pybind.cc`

 * *Files 2% similar despite different names*

```diff
@@ -17,21 +17,22 @@
 #include "stim/circuit/circuit.pybind.h"
 #include "stim/py/base.pybind.h"
 #include "stim/simulators/detection_simulator.h"
 #include "stim/simulators/frame_simulator.h"
 #include "stim/simulators/tableau_simulator.h"
 
 using namespace stim;
+using namespace stim_pybind;
 
 CompiledMeasurementSampler::CompiledMeasurementSampler(
     simd_bits ref_sample, Circuit circuit, bool skip_reference_sample, std::shared_ptr<std::mt19937_64> prng)
     : ref_sample(ref_sample), circuit(circuit), skip_reference_sample(skip_reference_sample), prng(prng) {
 }
 
-pybind11::array_t<uint8_t> CompiledMeasurementSampler::sample(size_t num_samples) {
+pybind11::array_t<bool> CompiledMeasurementSampler::sample(size_t num_samples) {
     auto sample = FrameSimulator::sample(circuit, ref_sample, num_samples, *prng);
 
     const simd_bits &flat = sample.data;
     std::vector<uint8_t> bytes;
     bytes.reserve(flat.num_bits_padded());
     auto *end = flat.u64 + flat.num_u64_padded();
     for (auto u64 = flat.u64; u64 != end; u64++) {
@@ -42,15 +43,15 @@
     }
 
     void *ptr = bytes.data();
     pybind11::ssize_t itemsize = sizeof(uint8_t);
     std::vector<pybind11::ssize_t> shape{
         (pybind11::ssize_t)num_samples, (pybind11::ssize_t)circuit.count_measurements()};
     std::vector<pybind11::ssize_t> stride{(pybind11::ssize_t)sample.num_minor_bits_padded(), 1};
-    const std::string &format = pybind11::format_descriptor<uint8_t>::value;
+    const std::string &format = pybind11::format_descriptor<bool>::value;
     bool readonly = true;
     return pybind11::array_t<uint8_t>(pybind11::buffer_info(ptr, itemsize, format, 2, shape, stride, readonly));
 }
 
 pybind11::array_t<uint8_t> CompiledMeasurementSampler::sample_bit_packed(size_t num_samples) {
     auto sample = FrameSimulator::sample(circuit, ref_sample, num_samples, *prng);
 
@@ -84,25 +85,22 @@
     }
     result << ")";
     return result.str();
 }
 
 pybind11::class_<CompiledMeasurementSampler> pybind_compiled_measurement_sampler_class(pybind11::module &m) {
     return pybind11::class_<CompiledMeasurementSampler>(
-        m,
-        "CompiledMeasurementSampler",
-        pybind11::module_local(),
-        "An analyzed stabilizer circuit whose measurements can be sampled quickly.");
+        m, "CompiledMeasurementSampler", "An analyzed stabilizer circuit whose measurements can be sampled quickly.");
 }
 
 CompiledMeasurementSampler py_init_compiled_sampler(
     const Circuit &circuit, bool skip_reference_sample, const pybind11::object &seed) {
     simd_bits ref_sample = skip_reference_sample ? simd_bits(circuit.count_measurements())
                                                  : TableauSimulator::reference_sample_circuit(circuit);
-    return CompiledMeasurementSampler(ref_sample, circuit, skip_reference_sample, PYBIND_SHARED_RNG(seed));
+    return CompiledMeasurementSampler(ref_sample, circuit, skip_reference_sample, make_py_seeded_rng(seed));
 }
 
 void pybind_compiled_measurement_sampler_methods(pybind11::class_<CompiledMeasurementSampler> &c) {
     c.def(
         pybind11::init(&py_init_compiled_sampler),
         pybind11::arg("circuit"),
         pybind11::kw_only(),
@@ -156,15 +154,15 @@
                 >>> import stim
                 >>> c = stim.Circuit('''
                 ...    X 0   2 3
                 ...    M 0 1 2 3
                 ... ''')
                 >>> s = c.compile_sampler()
                 >>> s.sample(shots=1)
-                array([[1, 0, 1, 1]], dtype=uint8)
+                array([[ True, False,  True,  True]])
         )DOC")
             .data());
 
     c.def(
         "sample",
         &CompiledMeasurementSampler::sample,
         pybind11::arg("shots"),
@@ -175,15 +173,15 @@
                 >>> import stim
                 >>> c = stim.Circuit('''
                 ...    X 0   2 3
                 ...    M 0 1 2 3
                 ... ''')
                 >>> s = c.compile_sampler()
                 >>> s.sample(shots=1)
-                array([[1, 0, 1, 1]], dtype=uint8)
+                array([[ True, False,  True,  True]])
 
             Args:
                 shots: The number of times to sample every measurement in the circuit.
 
             Returns:
                 A numpy array with `dtype=uint8` and `shape=(shots, num_measurements)`.
                 The bit for measurement `m` in shot `s` is at `result[s, m]`.
```

### Comparing `stim-1.8.0/src/stim/py/march.pybind.cc` & `stim-1.9.0/src/stim/py/march.pybind.cc`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,23 @@
-#include "march.pybind.h"
+#include "stim/py/march.pybind.h"
+
+#include <pybind11/pybind11.h>
 
 #ifdef _WIN32
 //  Windows
 #include <intrin.h>
 #define cpuid(info, x) __cpuidex(info, x, 0)
+#elif (defined(__arm64__) && defined(__APPLE__)) || defined(__aarch64__)
+// macOS ARM64 (dummied out)
+void cpuid(int info[4], int infoType) {
+    info[0] = 0;
+    info[1] = 0;
+    info[2] = 0;
+    info[3] = 0;
+}
 #else
 //  GCC Intrinsics
 #include <cpuid.h>
 void cpuid(int info[4], int infoType) {
     __cpuid_count(infoType, 0, info[0], info[1], info[2], info[3]);
 }
 #endif
@@ -39,7 +49,14 @@
         if (regs[EDX] & sse2_bit_in_edx) {
             return "sse2";
         }
     }
 
     return "polyfill";
 }
+
+PYBIND11_MODULE(_detect_machine_architecture, m) {
+    m.doc() = R"pbdoc(
+        Helper code for detecting AVX/SSE instruction support for Stim.
+    )pbdoc";
+    m.def("_UNSTABLE_detect_march", &detect_march);
+}
```

### Comparing `stim-1.8.0/src/stim/py/stim.pybind.cc` & `stim-1.9.0/src/stim/py/stim.pybind.cc`

 * *Files 24% similar despite different names*

```diff
@@ -14,14 +14,16 @@
 
 #include <pybind11/numpy.h>
 #include <pybind11/pybind11.h>
 #include <pybind11/stl.h>
 
 #include "stim/circuit/circuit.pybind.h"
 #include "stim/dem/detector_error_model.pybind.h"
+#include "stim/io/read_write.pybind.h"
+#include "stim/main_namespaced.h"
 #include "stim/py/base.pybind.h"
 #include "stim/py/compiled_detector_sampler.pybind.h"
 #include "stim/py/compiled_measurement_sampler.pybind.h"
 #include "stim/py/march.pybind.h"
 #include "stim/simulators/matched_error.pybind.h"
 #include "stim/simulators/measurements_to_detection_events.pybind.h"
 #include "stim/simulators/tableau_simulator.pybind.h"
@@ -29,40 +31,47 @@
 #include "stim/stabilizers/tableau.h"
 #include "stim/stabilizers/tableau.pybind.h"
 
 #define xstr(s) str(s)
 #define str(s) #s
 
 using namespace stim;
+using namespace stim_pybind;
 
-uint32_t target_rec(int32_t lookback) {
-    if (lookback >= 0 || lookback <= -(1 << 24)) {
-        throw std::out_of_range("Need -16777215 <= lookback <= -1");
-    }
-    return uint32_t(-lookback) | TARGET_RECORD_BIT;
+GateTarget target_rec(int32_t lookback) {
+    return GateTarget::rec(lookback);
 }
 
-uint32_t target_inv(uint32_t qubit) {
-    return GateTarget::qubit(qubit, true).data;
+GateTarget target_inv(uint32_t qubit) {
+    return GateTarget::qubit(qubit, true);
 }
 
-uint32_t target_x(uint32_t qubit, bool invert) {
-    return GateTarget::x(qubit, invert).data;
+GateTarget target_x(uint32_t qubit, bool invert) {
+    return GateTarget::x(qubit, invert);
 }
 
-uint32_t target_y(uint32_t qubit, bool invert) {
-    return GateTarget::y(qubit, invert).data;
+GateTarget target_y(uint32_t qubit, bool invert) {
+    return GateTarget::y(qubit, invert);
 }
 
-uint32_t target_z(uint32_t qubit, bool invert) {
-    return GateTarget::z(qubit, invert).data;
+GateTarget target_z(uint32_t qubit, bool invert) {
+    return GateTarget::z(qubit, invert);
 }
 
-uint32_t target_sweep_bit(uint32_t qubit) {
-    return GateTarget::sweep_bit(qubit).data;
+GateTarget target_sweep_bit(uint32_t qubit) {
+    return GateTarget::sweep_bit(qubit);
+}
+
+int stim_main(const std::vector<std::string> &args) {
+    std::vector<const char *> argv;
+    argv.push_back("stim.main");
+    for (const auto &arg : args) {
+        argv.push_back(arg.data());
+    }
+    return stim::main(argv.size(), argv.data());
 }
 
 pybind11::object raw_gate_data_solo(const Gate &gate) {
     pybind11::dict result;
     auto f = gate.extra_data_func;
     if (f == nullptr) {
         f = GATE_DATA.at(gate.name).extra_data_func;
@@ -105,15 +114,15 @@
     }
     return result;
 }
 
 PYBIND11_MODULE(STIM_PYBIND11_MODULE_NAME, m) {
     m.attr("__version__") = xstr(VERSION_INFO);
     m.doc() = R"pbdoc(
-        Stim: A fast stabilizer circuit simulator library.
+        Stim: A fast stabilizer circuit library.
     )pbdoc";
 
     // CAUTION: The ordering of these is important!
     // If a class references another before it is registered, method signatures can get messed up.
     // For example, if DetectorErrorModel is defined after Circuit then Circuit.detector_error_model's return type is
     // described as `stim::DetectorErrorModel` instead of `stim.DetectorErrorModel`.
 
@@ -126,14 +135,15 @@
     pybind_compiled_detector_sampler_methods(c0);
     pybind_compiled_measurement_sampler_methods(c1);
     pybind_compiled_measurements_to_detection_events_converter_methods(c2);
     pybind_pauli_string(m);
     pybind_tableau(m);
     pybind_tableau_simulator(m);
     pybind_matched_error(m);
+    pybind_read_write(m);
 
     m.def(
         "target_rec",
         &target_rec,
         pybind11::arg("lookback_index"),
         clean_doc_string(u8R"DOC(
             Returns a record target that can be passed into Circuit.append_operation.
@@ -199,12 +209,88 @@
         pybind11::arg("sweep_bit_index"),
         clean_doc_string(u8R"DOC(
             Returns a sweep bit target that can be passed into Circuit.append_operation
             For example, the 'sweep[5]' in 'CNOT sweep[5] 7' is from `stim.target_sweep_bit(5)`.
         )DOC")
             .data());
 
+    m.def(
+        "main",
+        &stim_main,
+        pybind11::kw_only(),
+        pybind11::arg("command_line_args"),
+        clean_doc_string(u8R"DOC(
+            Runs the command line tool version of stim on the given arguments.
+
+            Note that by default any input will be read from stdin, any output
+            will print to stdout (as opposed to being intercepted). For most
+            commands, you can use arguments like `--out` to write to a file
+            instead of stdout and `--in` to read from a file instead of stdin.
+
+            Returns:
+                An exit code (0 means success, not zero means failure).
+
+            Raises:
+                A large variety of errors, depending on what you are doing and
+                how it failed! Beware that many errors are caught by the main
+                method itself and printed to stderr, with the only indication
+                that something went wrong being the return code.
+
+            Example:
+                >>> import stim
+                >>> import tempfile
+                >>> with tempfile.TemporaryDirectory() as d:
+                ...     path = f'{d}/tmp.out'
+                ...     return_code = stim.main(command_line_args=[
+                ...         "gen",
+                ...         "--code=repetition_code",
+                ...         "--task=memory",
+                ...         "--rounds=1000",
+                ...         "--distance=2",
+                ...         "--out",
+                ...         path,
+                ...     ])
+                ...     assert return_code == 0
+                ...     with open(path) as f:
+                ...         print(f.read(), end='')
+                # Generated repetition_code circuit.
+                # task: memory
+                # rounds: 1000
+                # distance: 2
+                # before_round_data_depolarization: 0
+                # before_measure_flip_probability: 0
+                # after_reset_flip_probability: 0
+                # after_clifford_depolarization: 0
+                # layout:
+                # L0 Z1 d2
+                # Legend:
+                #     d# = data qubit
+                #     L# = data qubit with logical observable crossing
+                #     Z# = measurement qubit
+                R 0 1 2
+                TICK
+                CX 0 1
+                TICK
+                CX 2 1
+                TICK
+                MR 1
+                DETECTOR(1, 0) rec[-1]
+                REPEAT 999 {
+                    TICK
+                    CX 0 1
+                    TICK
+                    CX 2 1
+                    TICK
+                    MR 1
+                    SHIFT_COORDS(0, 1)
+                    DETECTOR(1, 0) rec[-1] rec[-2]
+                }
+                M 0 2
+                DETECTOR(1, 1) rec[-1] rec[-2] rec[-3]
+                OBSERVABLE_INCLUDE(0) rec[-1]
+        )DOC")
+            .data());
+
     m.def("_UNSTABLE_raw_gate_data", &raw_gate_data);
     m.def("_UNSTABLE_raw_format_data", &raw_format_data);
-    m.def("_UNSTABLE_detect_march", &detect_march);
     pybind_circuit_after_types_all_defined(c_circuit);
 }
```

### Comparing `stim-1.8.0/src/stim/simulators/detection_simulator.cc` & `stim-1.9.0/src/stim/simulators/detection_simulator.cc`

 * *Files 16% similar despite different names*

```diff
@@ -124,78 +124,116 @@
 void detector_samples_out_in_memory(
     const Circuit &circuit,
     size_t num_shots,
     bool prepend_observables,
     bool append_observables,
     FILE *out,
     SampleFormat format,
-    std::mt19937_64 &rng) {
-    if (prepend_observables && append_observables) {
-        throw std::out_of_range("Can't have both --prepend_observables and --append_observables");
+    std::mt19937_64 &rng,
+    FILE *obs_out,
+    SampleFormat obs_out_format) {
+    bool obs_in_det_output = prepend_observables || append_observables;
+    if (prepend_observables + append_observables + (obs_out != nullptr) > 1) {
+        throw std::out_of_range("Can't combine --prepend_observables, --append_observables, or --obs_out");
     }
 
     DetectorsAndObservables det_obs(circuit);
-    size_t num_sample_locations =
-        det_obs.detectors.size() + det_obs.observables.size() * ((int)prepend_observables + (int)append_observables);
+    size_t no = det_obs.observables.size();
+    size_t nd = det_obs.detectors.size();
 
     char c1, c2;
     size_t ct;
     if (prepend_observables) {
         c1 = 'L';
         c2 = 'D';
-        ct = det_obs.observables.size();
+        ct = no;
     } else if (append_observables) {
         c1 = 'D';
         c2 = 'L';
-        ct = det_obs.detectors.size();
+        ct = nd;
     } else {
         c1 = 'D';
         c2 = 'D';
         ct = 0;
     }
 
-    auto table = detector_samples(circuit, det_obs, num_shots, prepend_observables, append_observables, rng);
-    write_table_data(out, num_shots, num_sample_locations, simd_bits(0), table, format, c1, c2, ct);
+    auto table = detector_samples(
+        circuit, det_obs, num_shots, prepend_observables, append_observables || obs_out != nullptr, rng);
+
+    if (obs_out != nullptr) {
+        simd_bit_table obs_data(no, num_shots);
+        for (size_t k = 0; k < no; k++) {
+            obs_data[k] = table[nd + k];
+            table[nd + k].clear();
+        }
+        write_table_data(obs_out, num_shots, no, simd_bits(0), obs_data, obs_out_format, 'L', 'L', no);
+    }
+
+    write_table_data(out, num_shots, nd + no * obs_in_det_output, simd_bits(0), table, format, c1, c2, ct);
 }
 
 void detector_sample_out_helper(
     const Circuit &circuit,
     FrameSimulator &sim,
     size_t num_shots,
     bool prepend_observables,
     bool append_observables,
     FILE *out,
     SampleFormat format,
-    std::mt19937_64 &rng) {
+    std::mt19937_64 &rng,
+    FILE *obs_out,
+    SampleFormat obs_out_format) {
     uint64_t d = circuit.count_detectors() + circuit.count_observables();
     uint64_t approx_mem_usage = std::max(num_shots, size_t{256}) * std::max(circuit.count_measurements(), d);
-    if (!prepend_observables && should_use_streaming_instead_of_memory(approx_mem_usage)) {
+    if (!prepend_observables && obs_out == nullptr && should_use_streaming_instead_of_memory(approx_mem_usage)) {
         detector_sample_out_helper_stream(circuit, sim, num_shots, append_observables, out, format);
     } else {
-        detector_samples_out_in_memory(circuit, num_shots, prepend_observables, append_observables, out, format, rng);
+        detector_samples_out_in_memory(
+            circuit, num_shots, prepend_observables, append_observables, out, format, rng, obs_out, obs_out_format);
     }
 }
 
 void stim::detector_samples_out(
     const Circuit &circuit,
     size_t num_shots,
     bool prepend_observables,
     bool append_observables,
     FILE *out,
     SampleFormat format,
-    std::mt19937_64 &rng) {
+    std::mt19937_64 &rng,
+    FILE *obs_out,
+    SampleFormat obs_out_format) {
     constexpr size_t GOOD_BLOCK_SIZE = 768;
     size_t num_qubits = circuit.count_qubits();
     size_t max_lookback = circuit.max_lookback();
     if (num_shots >= GOOD_BLOCK_SIZE) {
         auto sim = FrameSimulator(num_qubits, GOOD_BLOCK_SIZE, max_lookback, rng);
         while (num_shots > GOOD_BLOCK_SIZE) {
             detector_sample_out_helper(
-                circuit, sim, GOOD_BLOCK_SIZE, prepend_observables, append_observables, out, format, rng);
+                circuit,
+                sim,
+                GOOD_BLOCK_SIZE,
+                prepend_observables,
+                append_observables,
+                out,
+                format,
+                rng,
+                obs_out,
+                obs_out_format);
             num_shots -= GOOD_BLOCK_SIZE;
         }
     }
     if (num_shots) {
         auto sim = FrameSimulator(num_qubits, num_shots, max_lookback, rng);
-        detector_sample_out_helper(circuit, sim, num_shots, prepend_observables, append_observables, out, format, rng);
+        detector_sample_out_helper(
+            circuit,
+            sim,
+            num_shots,
+            prepend_observables,
+            append_observables,
+            out,
+            format,
+            rng,
+            obs_out,
+            obs_out_format);
     }
 }
```

### Comparing `stim-1.8.0/src/stim/simulators/error_analyzer.cc` & `stim-1.9.0/src/stim/simulators/error_analyzer.cc`

 * *Files 17% similar despite different names*

```diff
@@ -83,40 +83,43 @@
         auto q = dat.targets[k].qubit_value();
         scheduled_measurement_time++;
 
         std::vector<DemTarget> &d = measurement_to_detectors[scheduled_measurement_time];
         xor_sort_measurement_error(d, dat);
         xs[q].xor_sorted_items(d);
         check_for_gauge(zs[q], op, q);
+        measurement_to_detectors.erase(scheduled_measurement_time);
     }
 }
 
 void ErrorAnalyzer::MY_with_context(const OperationData &dat, const char *op) {
     for (size_t k = dat.targets.size(); k-- > 0;) {
         auto q = dat.targets[k].qubit_value();
         scheduled_measurement_time++;
 
         std::vector<DemTarget> &d = measurement_to_detectors[scheduled_measurement_time];
         xor_sort_measurement_error(d, dat);
         xs[q].xor_sorted_items(d);
         zs[q].xor_sorted_items(d);
         check_for_gauge(xs[q], zs[q], op, q);
+        measurement_to_detectors.erase(scheduled_measurement_time);
     }
 }
 
 void ErrorAnalyzer::MZ_with_context(const OperationData &dat, const char *context_op) {
     for (size_t k = dat.targets.size(); k-- > 0;) {
         auto q = dat.targets[k].qubit_value();
         scheduled_measurement_time++;
 
         std::vector<DemTarget> &d = measurement_to_detectors[scheduled_measurement_time];
         xor_sort_measurement_error(d, dat);
 
         zs[q].xor_sorted_items(d);
         check_for_gauge(xs[q], context_op, q);
+        measurement_to_detectors.erase(scheduled_measurement_time);
     }
 }
 
 void ErrorAnalyzer::check_for_gauge(
     SparseXorVec<DemTarget> &potential_gauge_summand_1,
     SparseXorVec<DemTarget> &potential_gauge_summand_2,
     const char *context_op,
@@ -577,33 +580,47 @@
 
 ErrorAnalyzer::ErrorAnalyzer(
     uint64_t num_detectors,
     size_t num_qubits,
     bool decompose_errors,
     bool fold_loops,
     bool allow_gauge_detectors,
-    double approximate_disjoint_errors_threshold)
+    double approximate_disjoint_errors_threshold,
+    bool ignore_decomposition_failures,
+    bool block_decomposition_from_introducing_remnant_edges)
     : total_detectors(num_detectors),
       used_detectors(0),
       xs(num_qubits),
       zs(num_qubits),
       scheduled_measurement_time(0),
       decompose_errors(decompose_errors),
       accumulate_errors(true),
       fold_loops(fold_loops),
       allow_gauge_detectors(allow_gauge_detectors),
-      approximate_disjoint_errors_threshold(approximate_disjoint_errors_threshold) {
+      approximate_disjoint_errors_threshold(approximate_disjoint_errors_threshold),
+      ignore_decomposition_failures(ignore_decomposition_failures),
+      block_decomposition_from_introducing_remnant_edges(block_decomposition_from_introducing_remnant_edges) {
 }
 
 void ErrorAnalyzer::run_circuit(const Circuit &circuit) {
+    std::vector<OperationData> stacked_else_correlated_errors;
     for (size_t k = circuit.operations.size(); k--;) {
         const auto &op = circuit.operations[k];
         assert(op.gate != nullptr);
         try {
-            if (op.gate->id == gate_name_to_id("REPEAT")) {
+            if (op.gate->id == gate_name_to_id("ELSE_CORRELATED_ERROR")) {
+                stacked_else_correlated_errors.push_back(op.target_data);
+            } else if (op.gate->id == gate_name_to_id("E")) {
+                stacked_else_correlated_errors.push_back(op.target_data);
+                correlated_error_block(stacked_else_correlated_errors);
+                stacked_else_correlated_errors.clear();
+            } else if (!stacked_else_correlated_errors.empty()) {
+                throw std::invalid_argument(
+                    "ELSE_CORRELATED_ERROR wasn't preceded by ELSE_CORRELATED_ERROR or CORRELATED_ERROR (E)");
+            } else if (op.gate->id == gate_name_to_id("REPEAT")) {
                 assert(op.target_data.targets.size() == 3);
                 auto b = op.target_data.targets[0].data;
                 assert(op.target_data.targets[0].data < circuit.blocks.size());
                 uint64_t repeats = op_data_rep_count(op.target_data);
                 const auto &block = circuit.blocks[b];
                 run_loop(block, repeats);
             } else {
@@ -630,14 +647,19 @@
             error_msg << '\n' << circuit.describe_instruction_location(k);
             if (p != std::string::npos) {
                 error_msg << "\n    at block's instruction" << body.substr(p + strlen(marker));
             }
             throw std::invalid_argument(error_msg.str());
         }
     }
+
+    if (!stacked_else_correlated_errors.empty()) {
+        throw std::invalid_argument(
+            "ELSE_CORRELATED_ERROR wasn't preceded by ELSE_CORRELATED_ERROR or CORRELATED_ERROR (E)");
+    }
 }
 
 void ErrorAnalyzer::post_check_initialization() {
     for (uint32_t q = 0; q < xs.size(); q++) {
         check_for_gauge(xs[q], "qubit initialization into |0> at the start of the circuit", q);
     }
 }
@@ -675,28 +697,59 @@
     ConstPointerRange<T> in2 = src.range();
     xor_merge_sort_temp_buffer_callback(in1, in2, [&](ConstPointerRange<T> result) {
         dst.discard_tail();
         dst.append_tail(result);
     });
 }
 
-void ErrorAnalyzer::CORRELATED_ERROR(const OperationData &dat) {
+void ErrorAnalyzer::add_composite_error(double probability, ConstPointerRange<GateTarget> targets) {
     if (!accumulate_errors) {
         return;
     }
-    for (auto qp : dat.targets) {
+    for (auto qp : targets) {
         auto q = qp.qubit_value();
         if (qp.data & TARGET_PAULI_Z_BIT) {
             inplace_xor_tail(mono_buf, xs[q]);
         }
         if (qp.data & TARGET_PAULI_X_BIT) {
             inplace_xor_tail(mono_buf, zs[q]);
         }
     }
-    add_error_in_sorted_jagged_tail(dat.args[0]);
+    add_error_in_sorted_jagged_tail(probability);
+}
+
+void ErrorAnalyzer::correlated_error_block(const std::vector<OperationData> &dats) {
+    assert(!dats.empty());
+
+    if (dats.size() == 1) {
+        add_composite_error(dats[0].args[0], dats[0].targets);
+        return;
+    }
+    check_can_approximate_disjoint("ELSE_CORRELATED_ERROR");
+
+    double remaining_p = 1;
+    for (size_t k = dats.size(); k--;) {
+        OperationData dat = dats[k];
+        double actual_p = dat.args[0] * remaining_p;
+        remaining_p *= 1 - dat.args[0];
+        if (actual_p > approximate_disjoint_errors_threshold) {
+            throw std::invalid_argument(
+                "CORRELATED_ERROR/ELSE_CORRELATED_ERROR block has a component probability '" +
+                std::to_string(actual_p) +
+                "' larger than the "
+                "`approximate_disjoint_errors` threshold of "
+                "'" +
+                std::to_string(approximate_disjoint_errors_threshold) + "'.");
+        }
+        add_composite_error(actual_p, dat.targets);
+    }
+}
+
+void ErrorAnalyzer::CORRELATED_ERROR(const OperationData &dat) {
+    add_composite_error(dat.args[0], dat.targets);
 }
 
 void ErrorAnalyzer::DEPOLARIZE1(const OperationData &dat) {
     if (!accumulate_errors) {
         return;
     }
     if (dat.args[0] >= 3.0 / 4.0) {
@@ -732,24 +785,31 @@
                 xs[b.data].range(),
                 zs[b.data].range(),
             });
     }
 }
 
 void ErrorAnalyzer::ELSE_CORRELATED_ERROR(const OperationData &dat) {
-    throw std::invalid_argument(
-        "ELSE_CORRELATED_ERROR operations currently not supported in error analysis (cases may not be "
-        "independent).");
+    throw std::invalid_argument("Failed to analyze ELSE_CORRELATED_ERROR" + dat.str());
 }
 
-void ErrorAnalyzer::PAULI_CHANNEL_1(const OperationData &dat) {
+void ErrorAnalyzer::check_can_approximate_disjoint(const char *op_name) {
     if (approximate_disjoint_errors_threshold == 0) {
-        throw std::invalid_argument(
-            "Handling PAULI_CHANNEL_1 requires `approximate_disjoint_errors` argument to be specified.");
+        std::stringstream msg;
+        msg << "Encountered the operation " << op_name
+            << " during error analysis, but this operation requires the `approximate_disjoint_errors` option to be "
+               "enabled.";
+        msg << "\nIf you're' calling from python, using stim.Circuit.detector_error_model, you need to add the "
+               "argument approximate_disjoint_errors=True.\n";
+        msg << "\nIf you're' calling from the command line, you need to specify --approximate_disjoint_errors.";
+        throw std::invalid_argument(msg.str());
     }
+}
+void ErrorAnalyzer::PAULI_CHANNEL_1(const OperationData &dat) {
+    check_can_approximate_disjoint("PAULI_CHANNEL_1");
     ConstPointerRange<double> args = dat.args;
     std::array<double, 4> probabilities;
     for (size_t k = 0; k < 3; k++) {
         if (args[k] > approximate_disjoint_errors_threshold) {
             throw std::invalid_argument(
                 "PAULI_CHANNEL_1 has a component probability '" + std::to_string(args[k]) +
                 "' larger than the "
@@ -769,18 +829,15 @@
                 zs[q.data].range(),
                 xs[q.data].range(),
             });
     }
 }
 
 void ErrorAnalyzer::PAULI_CHANNEL_2(const OperationData &dat) {
-    if (approximate_disjoint_errors_threshold == 0) {
-        throw std::invalid_argument(
-            "Handling PAULI_CHANNEL_2 requires `approximate_disjoint_errors` argument to be specified.");
-    }
+    check_can_approximate_disjoint("PAULI_CHANNEL_2");
     ConstPointerRange<double> args = dat.args;
     std::array<double, 16> probabilities;
     for (size_t k = 0; k < 15; k++) {
         if (args[k] > approximate_disjoint_errors_threshold) {
             throw std::invalid_argument(
                 "PAULI_CHANNEL_2 has a component probability '" + std::to_string(args[k]) +
                 "' larger than the "
@@ -856,22 +913,26 @@
 }
 
 DetectorErrorModel ErrorAnalyzer::circuit_to_detector_error_model(
     const Circuit &circuit,
     bool decompose_errors,
     bool fold_loops,
     bool allow_gauge_detectors,
-    double approximate_disjoint_errors_threshold) {
+    double approximate_disjoint_errors_threshold,
+    bool ignore_decomposition_failures,
+    bool block_decomposition_from_introducing_remnant_edges) {
     ErrorAnalyzer analyzer(
         circuit.count_detectors(),
         circuit.count_qubits(),
         decompose_errors,
         fold_loops,
         allow_gauge_detectors,
-        approximate_disjoint_errors_threshold);
+        approximate_disjoint_errors_threshold,
+        ignore_decomposition_failures,
+        block_decomposition_from_introducing_remnant_edges);
     analyzer.current_circuit_being_analyzed = &circuit;
     analyzer.run_circuit(circuit);
     analyzer.post_check_initialization();
     analyzer.flush();
     uint64_t t = 0;
     std::set<DemTarget> seen;
     return unreversed(analyzer.flushed_reversed_model, t, seen);
@@ -927,29 +988,49 @@
 ConstPointerRange<DemTarget> ErrorAnalyzer::add_error_in_sorted_jagged_tail(double probability) {
     auto key = mono_dedupe_store_tail();
     auto &old_p = error_class_probabilities[key];
     old_p = old_p * (1 - probability) + (1 - old_p) * probability;
     return key;
 }
 
-bool shifted_equals(int64_t shift, const SparseXorVec<DemTarget> &unshifted, const SparseXorVec<DemTarget> &expected) {
+bool shifted_equals(int64_t shift, ConstPointerRange<DemTarget> unshifted, ConstPointerRange<DemTarget> expected) {
     if (unshifted.size() != expected.size()) {
         return false;
     }
     for (size_t k = 0; k < unshifted.size(); k++) {
-        DemTarget a = unshifted.sorted_items[k];
-        DemTarget e = expected.sorted_items[k];
+        DemTarget a = unshifted[k];
+        DemTarget e = expected[k];
         a.shift_if_detector_id(shift);
         if (a != e) {
             return false;
         }
     }
     return true;
 }
 
+bool shifted_equals(
+    int64_t m_shift,
+    int64_t d_shift,
+    const std::map<uint64_t, std::vector<DemTarget>> &unshifted,
+    const std::map<uint64_t, std::vector<DemTarget>> &expected) {
+    if (unshifted.size() != expected.size()) {
+        return false;
+    }
+    for (const auto &unshifted_entry : unshifted) {
+        const auto &shifted_entry = expected.find(unshifted_entry.first + m_shift);
+        if (shifted_entry == expected.end()) {
+            return false;
+        }
+        if (!shifted_equals(d_shift, unshifted_entry.second, shifted_entry->second)) {
+            return false;
+        }
+    }
+    return true;
+}
+
 void ErrorAnalyzer::run_loop(const Circuit &loop, uint64_t iterations) {
     if (!fold_loops) {
         // If loop folding is disabled, just manually run each iteration.
         for (size_t k = 0; k < iterations; k++) {
             run_circuit(loop);
         }
         return;
@@ -960,34 +1041,40 @@
     uint64_t tortoise_iter = 0;
     ErrorAnalyzer hare(
         total_detectors - used_detectors,
         xs.size(),
         false,
         true,
         allow_gauge_detectors,
-        approximate_disjoint_errors_threshold);
+        approximate_disjoint_errors_threshold,
+        false,
+        false);
     hare.xs = xs;
     hare.zs = zs;
     hare.ticks_seen = ticks_seen;
     hare.measurement_to_detectors = measurement_to_detectors;
     hare.scheduled_measurement_time = scheduled_measurement_time;
     hare.accumulate_errors = false;
 
     auto hare_is_colliding_with_tortoise = [&]() -> bool {
         // When comparing different loop iterations, shift detector ids to account for
         // detectors being introduced during each iteration.
         int64_t dt = -(int64_t)((hare_iter - tortoise_iter) * num_loop_detectors);
+        int64_t mt = hare.scheduled_measurement_time - scheduled_measurement_time;
         for (size_t k = 0; k < hare.xs.size(); k++) {
-            if (!shifted_equals(dt, xs[k], hare.xs[k])) {
+            if (!shifted_equals(dt, xs[k].range(), hare.xs[k].range())) {
                 return false;
             }
-            if (!shifted_equals(dt, zs[k], hare.zs[k])) {
+            if (!shifted_equals(dt, zs[k].range(), hare.zs[k].range())) {
                 return false;
             }
         }
+        if (!shifted_equals(mt, dt, measurement_to_detectors, hare.measurement_to_detectors)) {
+            return false;
+        }
         return true;
     };
 
     // Perform tortoise-and-hare cycle finding.
     while (hare_iter < iterations) {
         try {
             hare.run_circuit(loop);
@@ -1201,15 +1288,15 @@
         if (kv.second != 0 && !is_graphlike(component)) {
             return true;
         }
     }
     return false;
 }
 
-void ErrorAnalyzer::decompose_and_append_component_to_tail(
+bool ErrorAnalyzer::decompose_and_append_component_to_tail(
     ConstPointerRange<DemTarget> component,
     const std::map<FixedCapVector<DemTarget, 2>, ConstPointerRange<DemTarget>> &known_symptoms) {
     std::vector<bool> done(component.size(), false);
 
     size_t num_component_detectors = 0;
     for (size_t k = 0; k < component.size(); k++) {
         if (component[k].is_relative_detector_id()) {
@@ -1217,15 +1304,15 @@
         } else {
             done[k] = true;
         }
     }
     if (num_component_detectors <= 2) {
         mono_buf.append_tail(component);
         mono_buf.append_tail(DemTarget::separator());
-        return;
+        return true;
     }
 
     SparseXorVec<DemTarget> sparse;
     sparse.xor_sorted_items(component);
 
     for (size_t k = 0; k < component.size(); k++) {
         if (!done[k]) {
@@ -1255,25 +1342,109 @@
                 mono_buf.append_tail(DemTarget::separator());
                 sparse.xor_sorted_items(p->second);
             }
         }
         missed += !done[k];
     }
 
-    if (missed > 2) {
-        throw std::invalid_argument(
-            "Failed to decompose errors into graphlike components with at most two symptoms.\n"
-            "The error component that failed to decompose is '" +
-            comma_sep_workaround(component) + "'.");
+    if (missed <= 2) {
+        if (!sparse.empty()) {
+            mono_buf.append_tail({sparse.begin(), sparse.end()});
+            mono_buf.append_tail(DemTarget::separator());
+        }
+        return true;
     }
 
-    if (!sparse.empty()) {
-        mono_buf.append_tail({sparse.begin(), sparse.end()});
-        mono_buf.append_tail(DemTarget::separator());
+    mono_buf.discard_tail();
+    return false;
+}
+
+std::pair<uint64_t, uint64_t> obs_mask_of_targets(ConstPointerRange<DemTarget> targets) {
+    uint64_t obs_mask = 0;
+    uint64_t used_mask = 0;
+    for (size_t k = 0; k < targets.size(); k++) {
+        const auto &t = targets[k];
+        if (t.is_observable_id()) {
+            if (t.val() >= 64) {
+                throw std::invalid_argument("Not implemented: decomposing errors observable ids larger than 63.");
+            }
+            obs_mask |= uint64_t{1} << t.val();
+            used_mask |= uint64_t{1} << k;
+        }
+    }
+    return {obs_mask, used_mask};
+}
+
+bool brute_force_decomp_helper(
+    size_t start,
+    uint64_t used_term_mask,
+    uint64_t remaining_obs_mask,
+    ConstPointerRange<DemTarget> problem,
+    const std::map<FixedCapVector<DemTarget, 2>, ConstPointerRange<DemTarget>> &known_symptoms,
+    std::vector<ConstPointerRange<DemTarget>> &out_result) {
+    while (true) {
+        if (start >= problem.size()) {
+            return remaining_obs_mask == 0;
+        }
+        if (((used_term_mask >> start) & 1) == 0) {
+            break;
+        }
+        start++;
+    }
+    used_term_mask |= 1 << start;
+
+    FixedCapVector<DemTarget, 2> key;
+    key.push_back(problem[start]);
+    for (size_t k = start + 1; k <= problem.size(); k++) {
+        if (k < problem.size()) {
+            if ((used_term_mask >> k) & 1) {
+                continue;
+            }
+            key.push_back(problem[k]);
+            used_term_mask ^= 1 << k;
+        }
+        auto match = known_symptoms.find(key);
+        if (match != known_symptoms.end()) {
+            uint64_t obs_change = obs_mask_of_targets(match->second).first;
+            if (brute_force_decomp_helper(
+                    start + 1, used_term_mask, remaining_obs_mask ^ obs_change, problem, known_symptoms, out_result)) {
+                out_result.push_back(match->second);
+                return true;
+            }
+        }
+        if (k < problem.size()) {
+            key.pop_back();
+            used_term_mask ^= 1 << k;
+        }
     }
+
+    return false;
+}
+
+bool stim::brute_force_decomposition_into_known_graphlike_errors(
+    ConstPointerRange<DemTarget> problem,
+    const std::map<FixedCapVector<DemTarget, 2>, ConstPointerRange<DemTarget>> &known_graphlike_errors,
+    MonotonicBuffer<DemTarget> &output) {
+    if (problem.size() >= 64) {
+        throw std::invalid_argument("Not implemented: decomposing errors with more than 64 terms.");
+    }
+
+    std::vector<ConstPointerRange<DemTarget>> out;
+    out.reserve(problem.size());
+    auto prob_masks = obs_mask_of_targets(problem);
+
+    bool result =
+        brute_force_decomp_helper(0, prob_masks.second, prob_masks.first, problem, known_graphlike_errors, out);
+    if (result) {
+        for (auto r = out.crbegin(); r != out.crend(); r++) {
+            output.append_tail(*r);
+            output.append_tail(DemTarget::separator());
+        }
+    }
+    return result;
 }
 
 void ErrorAnalyzer::do_global_error_decomposition_pass() {
     if (!decompose_errors || !has_unflushed_ungraphlike_errors()) {
         return;
     }
 
@@ -1313,30 +1484,61 @@
         if (is_graphlike(targets)) {
             continue;
         }
 
         size_t start = 0;
         for (size_t k = 0; k <= targets.size(); k++) {
             if (k == targets.size() || targets[k].is_separator()) {
-                decompose_and_append_component_to_tail({&targets[start], &targets[k]}, known_symptoms);
+                ConstPointerRange<DemTarget> problem{&targets[start], &targets[k]};
+                if (brute_force_decomposition_into_known_graphlike_errors(problem, known_symptoms, mono_buf)) {
+                    // Solved using only existing edges.
+                } else if (
+                    !block_decomposition_from_introducing_remnant_edges &&
+                    // We are now *really* desperate.
+                    // We need to start considering decomposing into errors that
+                    // don't exist, as long as they can be formed by xoring
+                    // together errors that do exist. This might impact the
+                    // graphlike code distance.
+                    decompose_and_append_component_to_tail({&targets[start], &targets[k]}, known_symptoms)) {
+                    // Solved using a remnant edge.
+                } else if (ignore_decomposition_failures) {
+                    mono_buf.append_tail(problem);
+                    mono_buf.append_tail(DemTarget::separator());
+                } else {
+                    std::stringstream ss;
+                    ss << "Failed to decompose errors into graphlike components with at most two symptoms.\n";
+                    ss << "The error component that failed to decompose is '" << comma_sep_workaround(problem)
+                       << "'.\n";
+                    ss << "\n";
+                    ss << "In Python, you can ignore this error by passing `ignore_decomposition_failures=True` to "
+                          "`stim.Circuit.detector_error_model(...)`.\n";
+                    ss << "From the command line, you can ignore this error by passing the flag "
+                          "`--ignore_decomposition_failures` to `stim analyze_errors`.";
+                    if (block_decomposition_from_introducing_remnant_edges) {
+                        ss << "\n\nNote: `block_decomposition_from_introducing_remnant_edges` is ON.\n";
+                        ss << "Turning it off may prevent this error.\n";
+                    }
+                    throw std::invalid_argument(ss.str());
+                }
                 start = k + 1;
             }
         }
 
         if (!mono_buf.tail.empty()) {
             // Drop final separator.
             mono_buf.tail.ptr_end -= 1;
         }
 
         rewrites.push_back({kv.first, mono_buf.commit_tail()});
     }
 
     for (const auto &rewrite : rewrites) {
-        add_error(error_class_probabilities[rewrite.first], rewrite.second);
+        double p = error_class_probabilities[rewrite.first];
         error_class_probabilities.erase(rewrite.first);
+        add_error(p, rewrite.second);
     }
 }
 
 template <size_t s>
 void ErrorAnalyzer::add_error_combinations(
     std::array<double, 1 << s> independent_probabilities, std::array<ConstPointerRange<DemTarget>, s> basis_errors) {
     std::array<uint64_t, 1 << s> detector_masks{};
```

### Comparing `stim-1.8.0/src/stim/simulators/error_matcher.cc` & `stim-1.9.0/src/stim/simulators/error_matcher.cc`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 #include <queue>
 #include <sstream>
 
 using namespace stim;
 
 ErrorMatcher::ErrorMatcher(
     const Circuit &circuit, const DetectorErrorModel *init_filter, bool reduce_to_one_representative_error)
-    : error_analyzer(circuit.count_detectors(), circuit.count_qubits(), false, false, true, 1),
+    : error_analyzer(circuit.count_detectors(), circuit.count_qubits(), false, false, true, 1, false, false),
       cur_loc(),
       output_map(),
       allow_adding_new_dem_errors_to_output_map(init_filter == nullptr),
       reduce_to_one_representative_error(reduce_to_one_representative_error),
       dem_coords_map(),
       qubit_coords_map(circuit.get_final_qubit_coords()),
       cur_coord_offset(circuit.final_coord_shift()),
@@ -222,15 +222,15 @@
     } else if (op.gate->id == gate_name_to_id("SHIFT_COORDS")) {
         error_analyzer.SHIFT_COORDS(op.target_data);
         for (size_t k = 0; k < op.target_data.args.size(); k++) {
             cur_coord_offset[k] -= op.target_data.args[k];
         }
     } else if (!(op.gate->flags & (GATE_IS_NOISE | GATE_PRODUCES_NOISY_RESULTS))) {
         (error_analyzer.*op.gate->reverse_error_analyzer_function)(op.target_data);
-    } else if (op.gate->id == gate_name_to_id("E")) {
+    } else if (op.gate->id == gate_name_to_id("E") || op.gate->id == gate_name_to_id("ELSE_CORRELATED_ERROR")) {
         cur_loc.instruction_targets.target_range_start = 0;
         cur_loc.instruction_targets.target_range_end = op.target_data.targets.size();
         resolve_paulis_into(op.target_data.targets, 0, cur_loc.flipped_pauli_product);
         err_atom(op);
         cur_loc.flipped_pauli_product.clear();
     } else if (op.gate->id == gate_name_to_id("X_ERROR")) {
         err_xyz(op, TARGET_PAULI_X_BIT);
```

### Comparing `stim-1.8.0/src/stim/simulators/frame_simulator.cc` & `stim-1.9.0/src/stim/simulators/frame_simulator.cc`

 * *Files identical despite different names*

### Comparing `stim-1.8.0/src/stim/simulators/matched_error.cc` & `stim-1.9.0/src/stim/simulators/matched_error.cc`

 * *Files identical despite different names*

### Comparing `stim-1.8.0/src/stim/simulators/matched_error.pybind.cc` & `stim-1.9.0/src/stim/simulators/matched_error.pybind.cc`

 * *Files 1% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 #include "stim/circuit/gate_data.h"
 #include "stim/circuit/gate_target.h"
 #include "stim/dem/detector_error_model_target.pybind.h"
 #include "stim/py/base.pybind.h"
 #include "stim/simulators/matched_error.h"
 
 using namespace stim;
+using namespace stim_pybind;
 
 std::string CircuitErrorLocationStackFrame_repr(const CircuitErrorLocationStackFrame &self) {
     std::stringstream out;
     out << "stim.CircuitErrorLocationStackFrame";
     out << "(instruction_offset=" << self.instruction_offset;
     out << ", iteration_index=" << self.iteration_index;
     out << ", instruction_repetitions_arg=" << self.instruction_repetitions_arg;
@@ -131,15 +132,14 @@
     return out.str();
 }
 
 void pybind_CircuitErrorLocationStackFrame(pybind11::module &m) {
     auto c = pybind11::class_<CircuitErrorLocationStackFrame>(
         m,
         "CircuitErrorLocationStackFrame",
-        pybind11::module_local(),
         clean_doc_string(u8R"DOC(
             Describes the location of an instruction being executed within a
             circuit or loop, distinguishing between separate loop iterations.
 
             The full location of an instruction is a list of these frames,
             drilling down from the top level circuit to the inner-most loop
             that the instruction is within.
@@ -206,15 +206,14 @@
     c.def("__repr__", &CircuitErrorLocationStackFrame_repr);
 }
 
 void pybind_GateTargetWithCoords(pybind11::module &m) {
     auto c = pybind11::class_<GateTargetWithCoords>(
         m,
         "GateTargetWithCoords",
-        pybind11::module_local(),
         clean_doc_string(u8R"DOC(
             A gate target with associated coordinate information.
 
             For example, if the gate target is a qubit from a circuit with
             QUBIT_COORDS instructions, the coords field will contain the
             coordinate data from the QUBIT_COORDS instruction for the qubit.
 
@@ -264,15 +263,14 @@
     c.def("__repr__", &GateTargetWithCoords_repr);
 }
 
 void pybind_DemTargetWithCoords(pybind11::module &m) {
     auto c = pybind11::class_<DemTargetWithCoords>(
         m,
         "DemTargetWithCoords",
-        pybind11::module_local(),
         clean_doc_string(u8R"DOC(
             A detector error model instruction target with associated coords.
 
             It is also guaranteed that, if the type of the DEM target is a
             relative detector id, it is actually absolute (i.e. relative to
             0).
 
@@ -329,15 +327,14 @@
     c.def("__repr__", DemTargetWithCoords_repr);
 }
 
 void pybind_FlippedMeasurement(pybind11::module &m) {
     auto c = pybind11::class_<FlippedMeasurement>(
         m,
         "FlippedMeasurement",
-        pybind11::module_local(),
         clean_doc_string(u8R"DOC(
             Describes a measurement that was flipped.
 
             Gives the measurement's index in the measurement record, and also
             the observable of the measurement.
         )DOC")
             .data());
@@ -388,15 +385,14 @@
     c.def("__str__", &FlippedMeasurement_repr);
 }
 
 void pybind_CircuitTargetsInsideInstruction(pybind11::module &m) {
     auto c = pybind11::class_<CircuitTargetsInsideInstruction>(
         m,
         "CircuitTargetsInsideInstruction",
-        pybind11::module_local(),
         clean_doc_string(u8R"DOC(
             Describes a range of targets within a circuit instruction.
         )DOC")
             .data());
 
     c.def_property_readonly(
         "gate",
@@ -404,14 +400,15 @@
             if (self.gate == nullptr) {
                 return pybind11::none();
             }
             return pybind11::str(self.gate->name);
         },
         clean_doc_string(u8R"DOC(
             Returns the name of the gate / instruction that was being executed.
+            @signature def gate(self) -> Optional[str]:
         )DOC")
             .data());
 
     c.def_readonly(
         "target_range_start",
         &CircuitTargetsInsideInstruction::target_range_start,
         clean_doc_string(u8R"DOC(
@@ -475,15 +472,14 @@
     c.def("__str__", &CircuitTargetsInsideInstruction::str);
 }
 
 void pybind_CircuitErrorLocation(pybind11::module &m) {
     auto c = pybind11::class_<CircuitErrorLocation>(
         m,
         "CircuitErrorLocation",
-        pybind11::module_local(),
         clean_doc_string(u8R"DOC(
             Describes the location of an error mechanism from a stim circuit.
         )DOC")
             .data());
 
     c.def_readonly(
         "tick_offset",
@@ -510,14 +506,15 @@
                 return pybind11::none();
             }
             return pybind11::cast(self.flipped_measurement);
         },
         clean_doc_string(u8R"DOC(
             The measurement that was flipped by the error mechanism.
             If the error isn't a measurement error, this will be None.
+            @signature def flipped_measurement(self) -> Optional[stim.FlippedMeasurement]:
         )DOC")
             .data());
 
     c.def_readonly(
         "instruction_targets",
         &CircuitErrorLocation::instruction_targets,
         clean_doc_string(u8R"DOC(
@@ -575,15 +572,14 @@
     c.def("__str__", &CircuitErrorLocation::str);
 }
 
 void pybind_MatchedError(pybind11::module &m) {
     auto c = pybind11::class_<ExplainedError>(
         m,
         "ExplainedError",
-        pybind11::module_local(),
         clean_doc_string(u8R"DOC(
             Describes the location of an error mechanism from a stim circuit.
         )DOC")
             .data());
 
     c.def_readonly(
         "dem_error_terms",
```

### Comparing `stim-1.8.0/src/stim/simulators/measurements_to_detection_events.cc` & `stim-1.9.0/src/stim/simulators/measurements_to_detection_events.cc`

 * *Files 4% similar despite different names*

```diff
@@ -36,21 +36,30 @@
     bool append_observables,
     size_t num_measurements,
     size_t num_detectors,
     size_t num_observables,
     size_t num_qubits) {
     // Tables should agree on the batch size.
     size_t batch_size = out_detection_results__minor_shot_index.num_minor_bits_padded();
-    assert(measurements__minor_shot_index.num_minor_bits_padded() == batch_size);
-    assert(sweep_bits__minor_shot_index.num_minor_bits_padded() == batch_size);
+    if (measurements__minor_shot_index.num_minor_bits_padded() != batch_size) {
+        throw std::invalid_argument("measurements__minor_shot_index.num_minor_bits_padded() != batch_size");
+    }
+    if (sweep_bits__minor_shot_index.num_minor_bits_padded() != batch_size) {
+        throw std::invalid_argument("sweep_bits__minor_shot_index.num_minor_bits_padded() != batch_size");
+    }
     // Tables should have the right number of bits per shot.
-    assert(
-        out_detection_results__minor_shot_index.num_major_bits_padded() >=
-        num_detectors + num_observables * append_observables);
-    assert(measurements__minor_shot_index.num_major_bits_padded() >= num_measurements);
+    if (out_detection_results__minor_shot_index.num_major_bits_padded() <
+        num_detectors + num_observables * append_observables) {
+        throw std::invalid_argument(
+            "out_detection_results__minor_shot_index.num_major_bits_padded() < num_detectors + num_observables * "
+            "append_observables");
+    }
+    if (measurements__minor_shot_index.num_major_bits_padded() < num_measurements) {
+        throw std::invalid_argument("measurements__minor_shot_index.num_major_bits_padded() < num_measurements");
+    }
 
     // The frame simulator is used to account for flips in the measurement results that originate from the sweep data.
     // Eg. a `CNOT sweep[5] 0` can bit flip qubit 0, which can invert later measurement results, which will invert the
     // expected parity of detectors involving that measurement. This can vary from shot to shot.
     std::mt19937_64 rng1(0);
     std::mt19937_64 rng2(0);
     FrameSimulator frame_sim(num_qubits, batch_size, num_measurements, rng1);
@@ -74,15 +83,14 @@
         } else {
             measure_count_so_far += op.count_measurement_results();
             (frame_sim.*op.gate->frame_simulator_function)(op.target_data);
             return;
         }
 
         // XOR together the appropriate measurement inversions, using the reference sample as a baseline.
-        out_detection_results__minor_shot_index[out_index].clear();
         for (const auto &t : op.target_data.targets) {
             assert(t.is_measurement_record_target());  // Circuit validation should guarantee this.
             uint32_t lookback = t.data & TARGET_VALUE_MASK;
             if (lookback > measure_count_so_far) {
                 throw std::invalid_argument("Referred to a measurement result before the beginning of time.");
             }
             out_detection_results__minor_shot_index[out_index] ^=
@@ -91,15 +99,17 @@
             if (reference_sample[measure_count_so_far - lookback]) {
                 out_detection_results__minor_shot_index[out_index].invert_bits();
             }
         }
     });
 
     // Safety check verifying no randomness was used by the frame simulator.
-    assert(rng1() == rng2());
+    if (rng1() != rng2()) {
+        throw std::invalid_argument("Something is wrong. Converting measurements consumed entropy, but it shouldn't.");
+    }
 }
 
 simd_bit_table stim::measurements_to_detection_events(
     const simd_bit_table &measurements__minor_shot_index,
     const simd_bit_table &sweep_bits__minor_shot_index,
     const Circuit &circuit,
     bool append_observables,
@@ -133,15 +143,17 @@
     SampleFormat measurements_in_format,
     FILE *optional_initial_error_frames_in,
     SampleFormat initial_error_frames_in_format,
     FILE *results_out,
     SampleFormat results_out_format,
     const Circuit &circuit,
     bool append_observables,
-    bool skip_reference_sample) {
+    bool skip_reference_sample,
+    FILE *obs_out,
+    SampleFormat obs_out_format) {
     // Circuit metadata.
     size_t num_measurements = circuit.count_measurements();
     size_t num_observables = circuit.count_observables();
     size_t num_detectors = circuit.count_detectors();
     size_t num_qubits = circuit.count_qubits();
     size_t num_sweep_bits = circuit.count_sweep_bits();
     simd_bits reference_sample(num_measurements);
@@ -156,14 +168,16 @@
         optional_initial_error_frames_in,
         initial_error_frames_in_format,
         results_out,
         results_out_format,
         noiseless_circuit,
         append_observables,
         reference_sample,
+        obs_out,
+        obs_out_format,
         num_measurements,
         num_observables,
         num_detectors,
         num_qubits,
         num_sweep_bits);
 }
 
@@ -173,26 +187,32 @@
     FILE *optional_sweep_bits_in,
     SampleFormat sweep_bits_in_format,
     FILE *results_out,
     SampleFormat results_out_format,
     const Circuit &noiseless_circuit,
     bool append_observables,
     simd_bits_range_ref reference_sample,
+    FILE *obs_out,
+    SampleFormat obs_out_format,
     size_t num_measurements,
     size_t num_observables,
     size_t num_detectors,
     size_t num_qubits,
     size_t num_sweep_bits) {
     size_t num_out_bits = num_detectors + num_observables * append_observables;
     size_t num_sweep_bits_available = optional_sweep_bits_in == nullptr ? 0 : num_sweep_bits;
     size_t num_buffered_shots = 1024;
 
     // Readers / writers.
     auto reader = MeasureRecordReader::make(measurements_in, measurements_in_format, num_measurements);
     std::unique_ptr<MeasureRecordReader> sweep_data_reader;
+    std::unique_ptr<MeasureRecordWriter> obs_writer;
+    if (obs_out != nullptr) {
+        obs_writer = MeasureRecordWriter::make(obs_out, obs_out_format);
+    }
     auto writer = MeasureRecordWriter::make(results_out, results_out_format);
     if (optional_sweep_bits_in != nullptr) {
         sweep_data_reader = MeasureRecordReader::make(optional_sweep_bits_in, sweep_bits_in_format, num_sweep_bits);
     }
 
     // Buffers and transposed buffers.
     simd_bit_table measurements__minor_shot_index(num_measurements, num_buffered_shots);
@@ -226,21 +246,22 @@
         }
         if (record_count == 0) {
             break;
         }
         total_read += record_count;
 
         // Convert measurement data into detection event data.
+        out__minor_shot_index.clear();
         measurements_to_detection_events_helper(
             measurements__minor_shot_index,
             sweep_bits__minor_shot_index,
             out__minor_shot_index,
             noiseless_circuit,
             reference_sample,
-            append_observables,
+            append_observables || obs_out != nullptr,
             num_measurements,
             num_detectors,
             num_observables,
             num_qubits);
         out__minor_shot_index.transpose_into(out__major_shot_index);
 
         // Write detection event data.
@@ -251,10 +272,18 @@
             if (append_observables) {
                 writer->begin_result_type('L');
                 for (size_t k2 = 0; k2 < num_observables; k2++) {
                     writer->write_bit(record[num_detectors + k2]);
                 }
             }
             writer->write_end();
+
+            if (obs_out != nullptr) {
+                obs_writer->begin_result_type('L');
+                for (size_t k2 = 0; k2 < num_observables; k2++) {
+                    obs_writer->write_bit(record[num_detectors + k2]);
+                }
+                obs_writer->write_end();
+            }
         }
     }
 }
```

### Comparing `stim-1.8.0/src/stim/simulators/measurements_to_detection_events.pybind.cc` & `stim-1.9.0/src/stim/simulators/measurements_to_detection_events.pybind.cc`

 * *Files 14% similar despite different names*

```diff
@@ -11,185 +11,156 @@
 // WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 // See the License for the specific language governing permissions and
 // limitations under the License.
 
 #include "stim/simulators/measurements_to_detection_events.pybind.h"
 
 #include "stim/circuit/circuit.pybind.h"
+#include "stim/io/raii_file.h"
+#include "stim/io/read_write.pybind.h"
 #include "stim/py/base.pybind.h"
 #include "stim/simulators/detection_simulator.h"
 #include "stim/simulators/frame_simulator.h"
 #include "stim/simulators/measurements_to_detection_events.h"
 #include "stim/simulators/tableau_simulator.h"
 
 using namespace stim;
+using namespace stim_pybind;
 
 CompiledMeasurementsToDetectionEventsConverter::CompiledMeasurementsToDetectionEventsConverter(
     simd_bits ref_sample, Circuit circuit, bool skip_reference_sample)
     : skip_reference_sample(skip_reference_sample),
       ref_sample(ref_sample),
-      circuit(circuit),
       circuit_num_measurements(circuit.count_measurements()),
       circuit_num_sweep_bits(circuit.count_sweep_bits()),
       circuit_num_detectors(circuit.count_detectors()),
       circuit_num_observables(circuit.count_observables()),
-      circuit_num_qubits(circuit.count_qubits()) {
+      circuit_num_qubits(circuit.count_qubits()),
+      circuit(std::move(circuit)) {
 }
 std::string CompiledMeasurementsToDetectionEventsConverter::repr() const {
     std::stringstream result;
     result << "stim.CompiledMeasurementsToDetectionEventsConverter(";
     result << circuit_repr(circuit);
     if (skip_reference_sample) {
         result << ", skip_reference_sample=True";
     }
     result << ")";
     return result.str();
 }
 
-struct RaiiFile {
-    FILE *f;
-    RaiiFile(const char *path, const char *mode) {
-        if (path == nullptr) {
-            f = nullptr;
-            return;
-        }
-
-        f = fopen(path, mode);
-        if (f == nullptr) {
-            std::stringstream ss;
-            ss << "Failed to open '";
-            ss << path;
-            ss << "' for ";
-            if (*mode == 'r') {
-                ss << "reading.";
-            } else {
-                ss << "writing.";
-            }
-            throw std::invalid_argument(ss.str());
-        }
-    }
-    RaiiFile(const RaiiFile &other) = delete;
-    RaiiFile(RaiiFile &&other) = delete;
-    ~RaiiFile() {
-        if (f != nullptr) {
-            fclose(f);
-            f = nullptr;
-        }
-    }
-};
-
 void CompiledMeasurementsToDetectionEventsConverter::convert_file(
     const std::string &measurements_filepath,
     const std::string &measurements_format,
     const char *sweep_bits_filepath,
     const std::string &sweep_bits_format,
     const std::string &detection_events_filepath,
     const std::string &detection_events_format,
-    bool append_observables) {
+    bool append_observables,
+    const char *obs_out_filepath,
+    const std::string &obs_out_format) {
     auto format_in = format_to_enum(measurements_format);
     auto format_sweep_bits = format_to_enum(sweep_bits_format);
     auto format_out = format_to_enum(detection_events_format);
     RaiiFile file_in(measurements_filepath.data(), "r");
+    RaiiFile obs_out(obs_out_filepath, "w");
     RaiiFile sweep_bits_in(sweep_bits_filepath, "r");
     RaiiFile detections_out(detection_events_filepath.data(), "w");
+    auto parsed_obs_out_format = format_to_enum(obs_out_format);
 
     stim::stream_measurements_to_detection_events_helper(
         file_in.f,
         format_in,
         sweep_bits_in.f,
         format_sweep_bits,
         detections_out.f,
         format_out,
-        circuit,
+        circuit.aliased_noiseless_circuit(),
         append_observables,
         ref_sample,
+        obs_out.f,
+        parsed_obs_out_format,
         circuit_num_measurements,
         circuit_num_observables,
         circuit_num_detectors,
         circuit_num_qubits,
         circuit_num_sweep_bits);
 }
 
-pybind11::array_t<bool> CompiledMeasurementsToDetectionEventsConverter::convert(
-    const pybind11::array_t<bool> &measurements, const pybind11::array_t<bool> &sweep_bits, bool append_observables) {
-    size_t num_shots = measurements.shape(0);
-    if (measurements.ndim() != 2) {
-        throw std::invalid_argument("Need len(measurements.shape) == 2");
-    }
-    if ((size_t)measurements.shape(1) != circuit_num_measurements) {
-        throw std::invalid_argument("Need measurements.shape[1] == circuit.num_measurements");
+pybind11::object CompiledMeasurementsToDetectionEventsConverter::convert(
+    const pybind11::object &measurements,
+    const pybind11::object &sweep_bits,
+    const pybind11::object &separate_observables_obj,
+    const pybind11::object &append_observables_obj,
+    bool bit_pack_result) {
+    if (separate_observables_obj.is_none() && append_observables_obj.is_none()) {
+        throw std::invalid_argument(
+            "To ignore observable flip data, you must explicitly specify either separate_observables=False or "
+            "append_observables=False.");
     }
-    if (sweep_bits.ndim() != 0) {
-        if (sweep_bits.ndim() != 2) {
-            throw std::invalid_argument("Need len(sweep_bits.shape) == 2");
-        }
-        if ((size_t)sweep_bits.shape(1) != circuit_num_sweep_bits) {
-            throw std::invalid_argument("Need sweep_bits.shape[1] == circuit.num_sweep_bits");
-        }
-        if ((size_t)sweep_bits.shape(0) != num_shots) {
+    bool separate_observables = pybind11::cast<bool>(separate_observables_obj);
+    bool append_observables = pybind11::cast<bool>(append_observables_obj);
+    size_t num_shots;
+    simd_bit_table measurements_minor_shot_index =
+        numpy_array_to_transposed_simd_table(measurements, circuit_num_measurements, &num_shots);
+
+    simd_bit_table sweep_bits_minor_shot_index{0, num_shots};
+    if (!sweep_bits.is_none()) {
+        size_t num_sweep_shots;
+        sweep_bits_minor_shot_index =
+            numpy_array_to_transposed_simd_table(sweep_bits, circuit_num_sweep_bits, &num_sweep_shots);
+        if (num_shots != num_sweep_shots) {
             throw std::invalid_argument("Need sweep_bits.shape[0] == measurements.shape[0]");
         }
     }
 
-    simd_bit_table measurements__minor_shot_index(circuit_num_measurements, num_shots);
-    auto m = measurements.unchecked();
-    for (size_t shot_index = 0; shot_index < num_shots; shot_index++) {
-        for (size_t m_index = 0; m_index < circuit_num_measurements; m_index++) {
-            measurements__minor_shot_index[m_index][shot_index] ^= (bool)m(shot_index, m_index);
-        }
-    }
-
-    simd_bit_table sweep_bits__minor_shot_index(circuit_num_sweep_bits, num_shots);
-    if (sweep_bits.ndim() != 0) {
-        auto s = sweep_bits.unchecked();
-        for (size_t shot_index = 0; shot_index < num_shots; shot_index++) {
-            for (size_t b_index = 0; b_index < circuit_num_sweep_bits; b_index++) {
-                sweep_bits__minor_shot_index[b_index][shot_index] ^= (bool)s(shot_index, b_index);
-            }
-        }
-    }
-
-    size_t num_output_bits = circuit_num_detectors + circuit_num_observables * append_observables;
-    simd_bit_table out_detection_results__minor_shot_index(num_output_bits, num_shots);
+    size_t num_intermediate_bits =
+        circuit_num_detectors + circuit_num_observables * (append_observables || separate_observables);
+    simd_bit_table out_detection_results_minor_shot_index(num_intermediate_bits, num_shots);
     stim::measurements_to_detection_events_helper(
-        measurements__minor_shot_index,
-        sweep_bits__minor_shot_index,
-        out_detection_results__minor_shot_index,
+        measurements_minor_shot_index,
+        sweep_bits_minor_shot_index,
+        out_detection_results_minor_shot_index,
         circuit.aliased_noiseless_circuit(),
         ref_sample,
-        append_observables,
+        append_observables || separate_observables,
         circuit_num_measurements,
         circuit_num_detectors,
         circuit_num_observables,
         circuit_num_qubits);
 
-    std::vector<uint8_t> bytes;
-    bytes.resize(num_output_bits * num_shots);
-    size_t k = 0;
-    for (size_t shot_index = 0; shot_index < num_shots; shot_index++) {
-        for (size_t o_index = 0; o_index < num_output_bits; o_index++) {
-            bytes[k++] = out_detection_results__minor_shot_index[o_index][shot_index];
+    size_t num_output_bits = circuit_num_detectors + circuit_num_observables * append_observables;
+    pybind11::object obs_data = pybind11::none();
+    if (separate_observables) {
+        simd_bit_table obs_table(circuit_num_observables, num_shots);
+        for (size_t obs = 0; obs < circuit_num_observables; obs++) {
+            auto obs_slice = out_detection_results_minor_shot_index[circuit_num_detectors + obs];
+            obs_table[obs] = obs_slice;
+            if (!append_observables) {
+                obs_slice.clear();
+            }
         }
+        obs_data = transposed_simd_bit_table_to_numpy(obs_table, circuit_num_observables, num_shots, bit_pack_result);
     }
 
-    void *ptr = bytes.data();
-    pybind11::ssize_t itemsize = sizeof(uint8_t);
-    std::vector<pybind11::ssize_t> shape{(pybind11::ssize_t)num_shots, (pybind11::ssize_t)num_output_bits};
-    std::vector<pybind11::ssize_t> stride{(pybind11::ssize_t)num_output_bits, 1};
-    const std::string &format = pybind11::format_descriptor<bool>::value;
-    bool readonly = true;
-    return pybind11::array_t<bool>(pybind11::buffer_info(ptr, itemsize, format, 2, shape, stride, readonly));
+    // Caution: only do this after extracting the observable data, lest it leak into the packed bytes.
+    pybind11::object det_data = transposed_simd_bit_table_to_numpy(
+        out_detection_results_minor_shot_index, num_output_bits, num_shots, bit_pack_result);
+
+    if (separate_observables) {
+        return pybind11::make_tuple(det_data, obs_data);
+    }
+    return det_data;
 }
 
 pybind11::class_<CompiledMeasurementsToDetectionEventsConverter>
 pybind_compiled_measurements_to_detection_events_converter_class(pybind11::module &m) {
     return pybind11::class_<CompiledMeasurementsToDetectionEventsConverter>(
         m,
         "CompiledMeasurementsToDetectionEventsConverter",
-        pybind11::module_local(),
         "A tool for quickly converting measurements from an analyzed stabilizer circuit into detection events.");
 }
 
 CompiledMeasurementsToDetectionEventsConverter py_init_compiled_measurements_to_detection_events_converter(
     const Circuit &circuit, bool skip_reference_sample) {
     simd_bits ref_sample = skip_reference_sample ? simd_bits(circuit.count_measurements())
                                                  : TableauSimulator::reference_sample_circuit(circuit);
@@ -247,15 +218,17 @@
         pybind11::kw_only(),
         pybind11::arg("measurements_filepath"),
         pybind11::arg("measurements_format") = "01",
         pybind11::arg("sweep_bits_filepath") = pybind11::none(),
         pybind11::arg("sweep_bits_format") = "01",
         pybind11::arg("detection_events_filepath"),
         pybind11::arg("detection_events_format") = "01",
-        pybind11::arg("append_observables"),
+        pybind11::arg("append_observables") = false,
+        pybind11::arg("obs_out_filepath") = nullptr,
+        pybind11::arg("obs_out_format") = "01",
         clean_doc_string(u8R"DOC(
             Reads measurement data from a file, converts it, and writes the detection events to another file.
 
             Args:
                 measurements_filepath: A file containing measurement data to be converted.
                 measurements_format: The format the measurement data is stored in.
                     Valid values are "01", "b8", "r8", "hits", "dets", and "ptb64".
@@ -267,14 +240,19 @@
                 sweep_bits_filepath: Defaults to None. A file containing sweep data, or None.
                     When specified, sweep data (used for `sweep[k]` controls in the circuit, which can vary from shot to
                     shot) will be read from the given file.
                     When not specified, all sweep bits default to False and no sweep-controlled operations occur.
                 sweep_bits_format: The format the sweep data is stored in.
                     Valid values are "01", "b8", "r8", "hits", "dets", and "ptb64".
                     Defaults to "01".
+                obs_out_filepath: Sample observables as part of each shot, and write them to this file.
+                    This keeps the observable data separate from the detector data.
+                obs_out_format: If writing the observables to a file, this is the format to write them in.
+                    Valid values are "01", "b8", "r8", "hits", "dets", and "ptb64".
+                    Defaults to "01".
                 append_observables: When True, the observables in the circuit are included as part of the detection
                     event data. Specifically, they are treated as if they were additional detectors at the end of the
                     circuit. When False, observable data is not output.
 
             Examples:
                 >>> import stim
                 >>> import tempfile
@@ -301,48 +279,81 @@
 
     c.def(
         "convert",
         &CompiledMeasurementsToDetectionEventsConverter::convert,
         pybind11::kw_only(),
         pybind11::arg("measurements"),
         pybind11::arg("sweep_bits") = pybind11::none(),
-        pybind11::arg("append_observables"),
+        pybind11::arg("separate_observables") = pybind11::none(),
+        pybind11::arg("append_observables") = pybind11::none(),
+        pybind11::arg("bit_pack_result") = false,
         clean_doc_string(u8R"DOC(
-            Reads measurement data from a file, converts it, and writes the detection events to another file.
+            Converts measurement data into detection event data.
+            @signature def convert(self, *, measurements: np.ndarray, sweep_bits: Optional[np.ndarray] = None, separate_observables: bool = False, append_observables: bool = False, bit_pack_result: bool = False) -> Union[np.ndarray, Tuple[np.ndarray, np.ndarray]]:
 
             Args:
-                measurements: A numpy array containing measurement data:
-                    dtype=bool8
-                    shape=(num_shots, circuit.num_measurements)
-                sweep_bits: A numpy array containing sweep data for `sweep[k]` controls in the circuit:
-                    dtype=bool8
-                    shape=(num_shots, circuit.num_sweep_bits)
-                    Defaults to None (all sweep bits False).
-                append_observables: When True, the observables in the circuit are included as part of the detection
-                    event data. Specifically, they are treated as if they were additional detectors at the end of the
-                    circuit. When False, observable data is not output.
+                measurements: A numpy array containing measurement data. The dtype of the array is used
+                    to determine if it is bit packed or not.
+
+                    dtype=np.bool8 (unpacked data):
+                        shape=(num_shots, circuit.num_measurements)
+                    dtype=np.uint8 (bit packed data):
+                        shape=(num_shots, math.ceil(circuit.num_measurements / 8))
+                sweep_bits: Optional. A numpy array containing sweep data for the `sweep[k]` controls in the circuit.
+                    The dtype of the array is used to determine if it is bit packed or not.
+
+                    dtype=np.bool8 (unpacked data):
+                        shape=(num_shots, circuit.num_sweep_bits)
+                    dtype=np.uint8 (bit packed data):
+                        shape=(num_shots, math.ceil(circuit.num_sweep_bits / 8))
+                separate_observables: Defaults to False. When set to True, two numpy arrays are returned instead of one,
+                    with the second array containing the observable flip data.
+                append_observables: Defaults to False. When set to True, the observables in the circuit are treated as
+                    if they were additional detectors. Their results are appended to the end of the detection event
+                    data.
+                bit_pack_result: Defaults to False. When set to True, the returned numpy array contains bit packed
+                    data (dtype=np.uint8 with 8 bits per item) instead of unpacked data (dtype=np.bool8).
 
             Returns:
-                The detection event data in a numpy array:
-                    dtype=bool8
-                    shape=(num_shots, circuit.num_detectors + circuit.num_observables * append_observables)
+                The detection event data and (optionally) observable data.
+                The result is a single numpy array if separate_observables is false, otherwise it's a tuple of two numpy arrays.
+                When returning two numpy arrays, the first array is the detection event data and the second is the observable flip data.
+                The dtype of the returned arrays is np.bool8 if bit_pack_result is false, otherwise they're np.uint8 arrays.
+                shape[0] of the array(s) is the number of shots.
+                shape[1] of the array(s) is the number of bits per shot (divided by 8 if bit packed) (e.g. for just detection event data it would be circuit.num_detectors).
 
             Examples:
                 >>> import stim
                 >>> import numpy as np
                 >>> converter = stim.Circuit('''
                 ...    X 0
-                ...    M 0
+                ...    M 0 1
                 ...    DETECTOR rec[-1]
+                ...    DETECTOR rec[-2]
+                ...    OBSERVABLE_INCLUDE(0) rec[-2]
                 ... ''').compile_m2d_converter()
-                >>> converter.convert(
-                ...     measurements=np.array([[0], [1]], dtype=np.bool8),
-                ...     append_observables=False,
+                >>> dets, obs = converter.convert(
+                ...     measurements=np.array([[1, 0],
+                ...                            [1, 0],
+                ...                            [1, 0],
+                ...                            [0, 0],
+                ...                            [1, 0]], dtype=np.bool8),
+                ...     separate_observables=True,
                 ... )
-                array([[ True],
+                >>> dets
+                array([[False, False],
+                       [False, False],
+                       [False, False],
+                       [False,  True],
+                       [False, False]])
+                >>> obs
+                array([[False],
+                       [False],
+                       [False],
+                       [ True],
                        [False]])
         )DOC")
             .data());
 
     c.def(
         "__repr__",
         &CompiledMeasurementsToDetectionEventsConverter::repr,
```

### Comparing `stim-1.8.0/src/stim/simulators/tableau_simulator.cc` & `stim-1.9.0/src/stim/simulators/tableau_simulator.cc`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 using namespace stim;
 
 TableauSimulator::TableauSimulator(std::mt19937_64 &rng, size_t num_qubits, int8_t sign_bias, MeasureRecord record)
     : inv_state(Tableau::identity(num_qubits)),
       rng(rng),
       sign_bias(sign_bias),
-      measurement_record(record),
+      measurement_record(std::move(record)),
       last_correlated_error_occurred(false) {
 }
 
 bool TableauSimulator::is_deterministic_x(size_t target) const {
     return !inv_state.xs[target].xs.not_zero();
 }
 
@@ -55,14 +55,71 @@
             measure_z(meas);
             ZCX(cnot);
             H_YZ(h_yz);
             H_XZ(h_xz);
         });
 }
 
+void TableauSimulator::postselect_helper(
+    ConstPointerRange<GateTarget> targets,
+    bool desired_result,
+    void (TableauSimulator::*basis_change)(const OperationData &),
+    const char *false_name,
+    const char *true_name) {
+    std::set<GateTarget> unique_targets;
+    unique_targets.insert(targets.begin(), targets.end());
+    std::vector<GateTarget> unique_targets_vec;
+    unique_targets_vec.insert(unique_targets_vec.end(), unique_targets.begin(), unique_targets.end());
+
+    size_t finished = 0;
+    (this->*basis_change)({{}, unique_targets_vec});
+    {
+        uint8_t old_bias = sign_bias;
+        sign_bias = desired_result ? -1 : +1;
+        TableauTransposedRaii temp_transposed(inv_state);
+        while (finished < targets.size()) {
+            size_t q = (size_t)targets[finished].qubit_value();
+            collapse_qubit_z(q, temp_transposed);
+            if (inv_state.zs.signs[q] != desired_result) {
+                break;
+            }
+            finished++;
+        }
+        sign_bias = old_bias;
+    }
+    (this->*basis_change)({{}, unique_targets_vec});
+
+    if (finished < targets.size()) {
+        std::stringstream msg;
+        msg << "The requested postselection was impossible.\n";
+        msg << "Desired state: |" << (desired_result ? true_name : false_name) << ">\n";
+        msg << "Qubit " << targets[finished] << " is in the perpendicular state |"
+            << (desired_result ? false_name : true_name) << ">\n";
+        if (finished > 0) {
+            msg << finished << " of the requested postselections were finished (";
+            for (size_t k = 0; k < finished; k++) {
+                msg << "qubit " << targets[k] << ", ";
+            }
+            msg << "[failed here])\n";
+        }
+        throw std::invalid_argument(msg.str());
+    }
+}
+
+void TableauSimulator::postselect_x(ConstPointerRange<GateTarget> targets, bool desired_result) {
+    postselect_helper(targets, desired_result, &TableauSimulator::H_XZ, "+", "-");
+}
+
+void TableauSimulator::postselect_y(ConstPointerRange<GateTarget> targets, bool desired_result) {
+    postselect_helper(targets, desired_result, &TableauSimulator::H_YZ, "i", "-i");
+}
+void TableauSimulator::postselect_z(ConstPointerRange<GateTarget> targets, bool desired_result) {
+    postselect_helper(targets, desired_result, &TableauSimulator::I, "0", "1");
+}
+
 void TableauSimulator::measure_x(const OperationData &target_data) {
     // Ensure measurement observables are collapsed.
     collapse_x(target_data.targets);
 
     // Record measurement results.
     for (auto t : target_data.targets) {
         auto q = t.qubit_value();
@@ -272,14 +329,29 @@
         result.xs[0] = true;
         result.zs[0] = true;
     }
 
     return result;
 }
 
+int8_t TableauSimulator::peek_x(uint32_t target) const {
+    PauliStringRef x = inv_state.xs[target];
+    return x.xs.not_zero() ? 0 : x.sign ? -1 : +1;
+}
+
+int8_t TableauSimulator::peek_y(uint32_t target) const {
+    PauliString y = inv_state.eval_y_obs(target);
+    return y.xs.not_zero() ? 0 : y.sign ? -1 : +1;
+}
+
+int8_t TableauSimulator::peek_z(uint32_t target) const {
+    PauliStringRef z = inv_state.zs[target];
+    return z.xs.not_zero() ? 0 : z.sign ? -1 : +1;
+}
+
 void TableauSimulator::SQRT_X(const OperationData &target_data) {
     const auto &targets = target_data.targets;
     for (auto q : targets) {
         // Note: inverted because we're tracking the inverse tableau.
         inv_state.prepend_SQRT_X_DAG(q.data);
     }
 }
@@ -697,19 +769,29 @@
 
 VectorSimulator TableauSimulator::to_vector_sim() const {
     auto inv = inv_state.inverse();
     std::vector<PauliStringRef> stabilizers;
     for (size_t k = 0; k < inv.num_qubits; k++) {
         stabilizers.push_back(inv.zs[k]);
     }
-    return VectorSimulator::from_stabilizers(stabilizers, rng);
+    return VectorSimulator::from_stabilizers(stabilizers);
+}
+
+void TableauSimulator::apply_tableau(const Tableau &tableau, const std::vector<size_t> &targets) {
+    inv_state.inplace_scatter_prepend(tableau.inverse(), targets);
 }
 
-std::vector<std::complex<float>> TableauSimulator::to_state_vector() const {
-    return to_vector_sim().state;
+std::vector<std::complex<float>> TableauSimulator::to_state_vector(bool little_endian) const {
+    auto sim = to_vector_sim();
+    if (!little_endian) {
+        for (size_t q = 0; q < inv_state.num_qubits - q - 1; q++) {
+            sim.apply("SWAP", q, inv_state.num_qubits - q - 1);
+        }
+    }
+    return sim.state;
 }
 
 void TableauSimulator::collapse_x(ConstPointerRange<GateTarget> targets) {
     // Find targets that need to be collapsed.
     std::set<GateTarget> unique_collapse_targets;
     for (GateTarget t : targets) {
         t.data &= TARGET_VALUE_MASK;
```

### Comparing `stim-1.8.0/src/stim/simulators/tableau_simulator.pybind.cc` & `stim-1.9.0/src/stim/simulators/tableau_simulator.pybind.cc`

 * *Files 23% similar despite different names*

```diff
@@ -16,67 +16,113 @@
 
 #include "stim/py/base.pybind.h"
 #include "stim/simulators/tableau_simulator.h"
 #include "stim/stabilizers/pauli_string.pybind.h"
 #include "stim/stabilizers/tableau.h"
 
 using namespace stim;
+using namespace stim_pybind;
+
+PyTableauSimulator::PyTableauSimulator(std::shared_ptr<std::mt19937_64> rng)
+    : TableauSimulator(*rng), rng_reference(rng) {
+}
+
+void do_obj(PyTableauSimulator &self, const pybind11::object &obj) {
+    if (pybind11::isinstance<Circuit>(obj)) {
+        self.expand_do_circuit(pybind11::cast<Circuit>(obj));
+    } else if (pybind11::isinstance<PyPauliString>(obj)) {
+        const PyPauliString &pauli_string = pybind11::cast<PyPauliString>(obj);
+        self.ensure_large_enough_for_qubits(pauli_string.value.num_qubits);
+        self.paulis(pauli_string.value);
+    } else {
+        std::stringstream ss;
+        ss << "Don't know how to handle ";
+        ss << obj;
+        throw std::invalid_argument(ss.str());
+    }
+}
 
 struct TempViewableData {
     std::vector<GateTarget> targets;
     TempViewableData(std::vector<GateTarget> targets) : targets(std::move(targets)) {
     }
     operator OperationData() {
         return {{}, targets};
     }
 };
 
-TableauSimulator create_tableau_simulator() {
-    std::shared_ptr<std::mt19937_64> rng = PYBIND_SHARED_RNG(pybind11::none());
-    // Note: there is a global shared_ptr to the unseeded rng so it won't deallocate.
-    return TableauSimulator(*rng, 0);
+PyTableauSimulator create_tableau_simulator() {
+    return PyTableauSimulator(make_py_seeded_rng(pybind11::none()));
 }
 
-TempViewableData args_to_targets(TableauSimulator &self, const pybind11::args &args) {
+std::vector<GateTarget> arg_to_qubit_or_qubits(PyTableauSimulator &self, const pybind11::object &obj) {
+    std::vector<GateTarget> arguments;
+    uint32_t max_q = 0;
+    try {
+        try {
+            uint32_t q = pybind11::cast<uint32_t>(obj);
+            arguments.push_back(GateTarget::qubit(q));
+            max_q = q;
+        } catch (const pybind11::cast_error &) {
+            for (const auto &e : obj) {
+                uint32_t q = e.cast<uint32_t>();
+                max_q = std::max(max_q, q);
+                arguments.push_back(GateTarget::qubit(q));
+            }
+        }
+    } catch (const pybind11::cast_error &) {
+        throw std::out_of_range("'targets' must be a non-negative integer or iterable of non-negative integers.");
+    }
+
+    // Note: quadratic behavior.
+    self.ensure_large_enough_for_qubits(max_q + 1);
+
+    return arguments;
+}
+
+TempViewableData args_to_targets(PyTableauSimulator &self, const pybind11::args &args) {
     std::vector<GateTarget> arguments;
     uint32_t max_q = 0;
     try {
         for (const auto &e : args) {
-            uint32_t q = e.cast<uint32_t>();
-            max_q = std::max(max_q, q & TARGET_VALUE_MASK);
-            arguments.push_back(GateTarget{q});
+            if (pybind11::isinstance<GateTarget>(e)) {
+                arguments.push_back(pybind11::cast<GateTarget>(e));
+            } else {
+                uint32_t q = e.cast<uint32_t>();
+                max_q = std::max(max_q, q & TARGET_VALUE_MASK);
+                arguments.push_back(GateTarget{q});
+            }
         }
     } catch (const pybind11::cast_error &) {
         throw std::out_of_range("Target qubits must be non-negative integers.");
     }
 
     // Note: quadratic behavior.
     self.ensure_large_enough_for_qubits(max_q + 1);
 
     return TempViewableData(arguments);
 }
 
-TempViewableData args_to_target_pairs(TableauSimulator &self, const pybind11::args &args) {
+TempViewableData args_to_target_pairs(PyTableauSimulator &self, const pybind11::args &args) {
     if (pybind11::len(args) & 1) {
         throw std::invalid_argument("Two qubit operation requires an even number of targets.");
     }
     auto result = args_to_targets(self, args);
     for (size_t k = 0; k < result.targets.size(); k += 2) {
         if (result.targets[k] == result.targets[k + 1]) {
             throw std::invalid_argument("Two qubit operation can't target the same qubit twice.");
         }
     }
     return result;
 }
 
 void pybind_tableau_simulator(pybind11::module &m) {
-    auto c = pybind11::class_<TableauSimulator>(
+    auto c = pybind11::class_<PyTableauSimulator>(
         m,
         "TableauSimulator",
-        pybind11::module_local(),
         clean_doc_string(u8R"DOC(
             A quantum stabilizer circuit simulator whose internal state is an inverse stabilizer tableau.
 
             Supports interactive usage, where gates and measurements are applied on demand.
 
             Examples:
                 >>> import stim
@@ -105,15 +151,15 @@
         )DOC")
             .data());
 
     c.def(pybind11::init(&create_tableau_simulator));
 
     c.def(
         "current_inverse_tableau",
-        [](TableauSimulator &self) {
+        [](PyTableauSimulator &self) {
             return self.inv_state;
         },
         clean_doc_string(u8R"DOC(
             Returns a copy of the internal state of the simulator as a stim.Tableau.
 
             Returns:
                 A stim.Tableau copy of the simulator's state.
@@ -144,16 +190,24 @@
                     ],
                 )
         )DOC")
             .data());
 
     c.def(
         "state_vector",
-        [](const TableauSimulator &self) {
-            auto complex_vec = self.to_state_vector();
+        [](const PyTableauSimulator &self, const std::string &endian) {
+            bool little_endian;
+            if (endian == "little") {
+                little_endian = true;
+            } else if (endian == "big") {
+                little_endian = false;
+            } else {
+                throw std::invalid_argument("endian not in ['little', 'big']");
+            }
+            auto complex_vec = self.to_state_vector(little_endian);
             std::vector<float> float_vec;
             float_vec.reserve(complex_vec.size() * 2);
             for (const auto &e : complex_vec) {
                 float_vec.push_back(e.real());
                 float_vec.push_back(e.imag());
             }
             void *ptr = float_vec.data();
@@ -161,48 +215,63 @@
             std::vector<pybind11::ssize_t> shape{(pybind11::ssize_t)complex_vec.size()};
             std::vector<pybind11::ssize_t> stride{itemsize};
             const std::string &format = pybind11::format_descriptor<std::complex<float>>::value;
             bool readonly = true;
             return pybind11::array_t<float>(
                 pybind11::buffer_info(ptr, itemsize, format, shape.size(), shape, stride, readonly));
         },
+        pybind11::kw_only(),
+        pybind11::arg("endian") = "little",
         clean_doc_string(u8R"DOC(
+            @signature def state_vector(self, *, endian: str = 'little') -> np.ndarray[np.complex64]:
             Returns a wavefunction that satisfies the stabilizers of the simulator's current state.
 
             This function takes O(n * 2**n) time and O(2**n) space, where n is the number of qubits. The computation is
             done by initialization a random state vector and iteratively projecting it into the +1 eigenspace of each
-            stabilizer of the state. The global phase of the result is arbitrary (and will vary from call to call).
+            stabilizer of the state. The state is then canonicalized so that zero values are actually exactly 0, and so
+            that the first non-zero entry is positive.
 
-            The result is in little endian order. The amplitude at offset b_0 + b_1*2 + b_2*4 + ... + b_{n-1}*2^{n-1} is
-            the amplitude for the computational basis state where the qubit with index 0 is storing the bit b_0, the
-            qubit with index 1 is storing the bit b_1, etc.
+            Args:
+                endian:
+                    "little" (default): state vector is in little endian order, where higher index qubits
+                        correspond to larger changes in the state index.
+                    "big": state vector is in little endian order, where higher index qubits correspond to
+                        smaller changes in the state index.
 
             Returns:
-                A `numpy.ndarray[numpy.complex64]` of computational basis amplitudes in little endian order.
+                A `numpy.ndarray[numpy.complex64]` of computational basis amplitudes.
+
+                If the result is in little endian order then the amplitude at offset b_0 + b_1*2 + b_2*4 + ... + b_{n-1}*2^{n-1} is
+                the amplitude for the computational basis state where the qubit with index 0 is storing the bit b_0, the
+                qubit with index 1 is storing the bit b_1, etc.
+
+                If the result is in big endian order then the amplitude at offset b_0 + b_1*2 + b_2*4 + ... + b_{n-1}*2^{n-1} is
+                the amplitude for the computational basis state where the qubit with index 0 is storing the bit b_{n-1}, the
+                qubit with index 1 is storing the bit b_{n-2}, etc.
 
             Examples:
                 >>> import stim
                 >>> import numpy as np
-
-                >>> # Check that the qubit-to-amplitude-index ordering is little-endian.
                 >>> s = stim.TableauSimulator()
-                >>> s.x(1)
-                >>> s.x(4)
-                >>> vector = s.state_vector()
-                >>> np.abs(vector[0b_10010]).round(2)
-                1.0
-                >>> tensor = vector.reshape((2, 2, 2, 2, 2))
-                >>> np.abs(tensor[1, 0, 0, 1, 0]).round(2)
-                1.0
+                >>> s.x(2)
+                >>> list(s.state_vector(endian='little'))
+                [0j, 0j, 0j, 0j, (1+0j), 0j, 0j, 0j]
+
+                >>> list(s.state_vector(endian='big'))
+                [0j, (1+0j), 0j, 0j, 0j, 0j, 0j, 0j]
+
+                >>> s.sqrt_x(1, 2)
+                >>> list(s.state_vector())
+                [(0.5+0j), 0j, -0.5j, 0j, 0.5j, 0j, (0.5+0j), 0j]
         )DOC")
             .data());
 
     c.def(
         "canonical_stabilizers",
-        [](const TableauSimulator &self) {
+        [](const PyTableauSimulator &self) {
             auto stabilizers = self.canonical_stabilizers();
             std::vector<PyPauliString> result;
             result.reserve(stabilizers.size());
             for (auto &s : stabilizers) {
                 result.emplace_back(std::move(s), false);
             }
             return result;
@@ -243,15 +312,15 @@
                 >>> s.canonical_stabilizers()
                 [stim.PauliString("+XX_"), stim.PauliString("+ZZ_"), stim.PauliString("-__Z")]
         )DOC")
             .data());
 
     c.def(
         "current_measurement_record",
-        [](TableauSimulator &self) {
+        [](const PyTableauSimulator &self) {
             return self.measurement_record.storage;
         },
         clean_doc_string(u8R"DOC(
             Returns a copy of the record of all measurements performed by the simulator.
 
             Examples:
                 >>> import stim
@@ -272,410 +341,776 @@
             Returns:
                 A list of booleans containing the result of every measurement performed by the simulator so far.
         )DOC")
             .data());
 
     c.def(
         "do",
-        &TableauSimulator::expand_do_circuit,
-        pybind11::arg("circuit"),
+        &do_obj,
+        pybind11::arg("circuit_or_pauli_string"),
         clean_doc_string(u8R"DOC(
-            Applies all the operations in the given stim.Circuit to the simulator's state.
+            Applies a circuit or pauli string to the simulator's state.
+            @overload def do(self, circuit_or_pauli_string: stim.Circuit) -> None:
+            @overload def do(self, circuit_or_pauli_string: stim.PauliString) -> None:
+
+            Args:
+                circuit_or_pauli_string: A stim.Circuit or a stim.PauliString containing operations to apply.
 
             Examples:
                 >>> import stim
                 >>> s = stim.TableauSimulator()
                 >>> s.do(stim.Circuit('''
                 ...     X 0
                 ...     M 0
                 ... '''))
                 >>> s.current_measurement_record()
                 [True]
 
-            Args:
-                circuit: A stim.Circuit containing operations to apply.
+                >>> s = stim.TableauSimulator()
+                >>> s.do(stim.PauliString("IXYZ"))
+                >>> s.measure_many(0, 1, 2, 3)
+                [False, True, True, False]
         )DOC")
             .data());
 
     c.def(
-        "do",
-        [](TableauSimulator &self, const PyPauliString &pauli_string) {
+        "do_pauli_string",
+        [](PyTableauSimulator &self, PyPauliString &pauli_string) {
             self.ensure_large_enough_for_qubits(pauli_string.value.num_qubits);
             self.paulis(pauli_string.value);
         },
         pybind11::arg("pauli_string"),
         clean_doc_string(u8R"DOC(
-            Applies all the Pauli operations in the given stim.PauliString to the simulator's state.
+            Applies the paulis from a pauli string to the simulator's state.
 
-            The Pauli at offset k is applied to the qubit with index k.
+            Args:
+                pauli_string: A stim.PauliString containing Paulis to apply.
 
             Examples:
                 >>> import stim
                 >>> s = stim.TableauSimulator()
-                >>> s.do(stim.PauliString("IXYZ"))
+                >>> s.do_pauli_string(stim.PauliString("IXYZ"))
                 >>> s.measure_many(0, 1, 2, 3)
                 [False, True, True, False]
+        )DOC")
+            .data());
+
+    c.def(
+        "do_circuit",
+        &PyTableauSimulator::expand_do_circuit,
+        pybind11::arg("circuit"),
+        clean_doc_string(u8R"DOC(
+            Applies a circuit to the simulator's state.
+
+            Args:
+                circuit: A stim.Circuit containing operations to apply.
+
+            Examples:
+                >>> import stim
+                >>> s = stim.TableauSimulator()
+                >>> s.do_circuit(stim.Circuit('''
+                ...     X 0
+                ...     M 0
+                ... '''))
+                >>> s.current_measurement_record()
+                [True]
+        )DOC")
+            .data());
+
+    c.def(
+        "do_tableau",
+        [](PyTableauSimulator &self, const Tableau &tableau, const std::vector<size_t> &targets) {
+            if (targets.size() != tableau.num_qubits) {
+                throw std::invalid_argument("len(tableau) != len(targets)");
+            }
+            size_t max_target = 0;
+            for (size_t i = 0; i < targets.size(); i++) {
+                max_target = std::max(max_target, targets[i]);
+                for (size_t j = i + 1; j < targets.size(); j++) {
+                    if (targets[i] == targets[j]) {
+                        std::stringstream ss;
+                        ss << "targets contains duplicates: ";
+                        ss << comma_sep(targets);
+                        throw std::invalid_argument(ss.str());
+                    }
+                }
+            }
+            self.ensure_large_enough_for_qubits(max_target + 1);
+            self.apply_tableau(tableau, targets);
+        },
+        pybind11::arg("tableau"),
+        pybind11::arg("targets"),
+        clean_doc_string(u8R"DOC(
+            Applies a custom tableau operation to qubits in the simulator.
+
+            Note that this method has to compute the inverse of the tableau, because the
+            simulator's internal state is an inverse tableau.
 
             Args:
-                pauli_string: A stim.PauliString containing Pauli operations to apply.
+                tableau: A stim.Tableau representing the Clifford operation to apply.
+                targets: The indices of the qubits to operate on.
+
+            Examples:
+                >>> import stim
+                >>> sim = stim.TableauSimulator()
+                >>> sim.h(1)
+                >>> sim.h_yz(2)
+                >>> [str(sim.peek_bloch(k)) for k in range(4)]
+                ['+Z', '+X', '+Y', '+Z']
+                >>> rot3 = stim.Tableau.from_conjugated_generators(
+                ...     xs=[
+                ...         stim.PauliString("_X_"),
+                ...         stim.PauliString("__X"),
+                ...         stim.PauliString("X__"),
+                ...     ],
+                ...     zs=[
+                ...         stim.PauliString("_Z_"),
+                ...         stim.PauliString("__Z"),
+                ...         stim.PauliString("Z__"),
+                ...     ],
+                ... )
+
+                >>> sim.do_tableau(rot3, [1, 2, 3])
+                >>> [str(sim.peek_bloch(k)) for k in range(4)]
+                ['+Z', '+Z', '+X', '+Y']
+
+                >>> sim.do_tableau(rot3, [1, 2, 3])
+                >>> [str(sim.peek_bloch(k)) for k in range(4)]
+                ['+Z', '+Y', '+Z', '+X']
         )DOC")
             .data());
 
     c.def(
         "h",
-        [](TableauSimulator &self, pybind11::args args) {
+        [](PyTableauSimulator &self, pybind11::args args) {
             self.H_XZ(args_to_targets(self, args));
         },
         clean_doc_string(u8R"DOC(
             Applies a Hadamard gate to the simulator's state.
 
             Args:
                 *targets: The indices of the qubits to target with the gate.
         )DOC")
             .data());
 
     c.def(
+        "h_xz",
+        [](PyTableauSimulator &self, pybind11::args args) {
+            self.H_XZ(args_to_targets(self, args));
+        },
+        clean_doc_string(u8R"DOC(
+            Applies a Hadamard gate to the simulator's state.
+
+            Args:
+                *targets: The indices of the qubits to target with the gate.
+        )DOC")
+            .data());
+
+    c.def(
+        "c_xyz",
+        [](PyTableauSimulator &self, pybind11::args args) {
+            self.C_XYZ(args_to_targets(self, args));
+        },
+        clean_doc_string(u8R"DOC(
+            Applies a C_XYZ gate to the simulator's state.
+
+            Args:
+                *targets: The indices of the qubits to target with the gate.
+        )DOC")
+            .data());
+
+    c.def(
+        "c_zyx",
+        [](PyTableauSimulator &self, pybind11::args args) {
+            self.C_ZYX(args_to_targets(self, args));
+        },
+        clean_doc_string(u8R"DOC(
+            Applies a C_ZYX gate to the simulator's state.
+
+            Args:
+                *targets: The indices of the qubits to target with the gate.
+        )DOC")
+            .data());
+
+    c.def(
         "h_xy",
-        [](TableauSimulator &self, pybind11::args args) {
+        [](PyTableauSimulator &self, pybind11::args args) {
             self.H_XY(args_to_targets(self, args));
         },
         clean_doc_string(u8R"DOC(
             Applies a variant of the Hadamard gate that swaps the X and Y axes to the simulator's state.
 
             Args:
                 *targets: The indices of the qubits to target with the gate.
         )DOC")
             .data());
 
     c.def(
         "h_yz",
-        [](TableauSimulator &self, pybind11::args args) {
+        [](PyTableauSimulator &self, pybind11::args args) {
             self.H_YZ(args_to_targets(self, args));
         },
         clean_doc_string(u8R"DOC(
             Applies a variant of the Hadamard gate that swaps the Y and Z axes to the simulator's state.
 
             Args:
                 *targets: The indices of the qubits to target with the gate.
         )DOC")
             .data());
 
     c.def(
         "x",
-        [](TableauSimulator &self, pybind11::args args) {
+        [](PyTableauSimulator &self, pybind11::args args) {
             self.X(args_to_targets(self, args));
         },
         clean_doc_string(u8R"DOC(
             Applies a Pauli X gate to the simulator's state.
 
             Args:
                 *targets: The indices of the qubits to target with the gate.
         )DOC")
             .data());
 
     c.def(
         "y",
-        [](TableauSimulator &self, pybind11::args args) {
+        [](PyTableauSimulator &self, pybind11::args args) {
             self.Y(args_to_targets(self, args));
         },
         clean_doc_string(u8R"DOC(
             Applies a Pauli Y gate to the simulator's state.
 
             Args:
                 *targets: The indices of the qubits to target with the gate.
         )DOC")
             .data());
 
     c.def(
         "z",
-        [](TableauSimulator &self, pybind11::args args) {
-            self.Z(args_to_targets(self, args));
+        [](PyTableauSimulator &self, pybind11::args targets) {
+            self.Z(args_to_targets(self, targets));
         },
         clean_doc_string(u8R"DOC(
             Applies a Pauli Z gate to the simulator's state.
 
             Args:
                 *targets: The indices of the qubits to target with the gate.
         )DOC")
             .data());
 
     c.def(
         "s",
-        [](TableauSimulator &self, pybind11::args args) {
+        [](PyTableauSimulator &self, pybind11::args args) {
             self.SQRT_Z(args_to_targets(self, args));
         },
         clean_doc_string(u8R"DOC(
             Applies a SQRT_Z gate to the simulator's state.
 
             Args:
                 *targets: The indices of the qubits to target with the gate.
         )DOC")
             .data());
 
     c.def(
         "s_dag",
-        [](TableauSimulator &self, pybind11::args args) {
+        [](PyTableauSimulator &self, pybind11::args args) {
             self.SQRT_Z_DAG(args_to_targets(self, args));
         },
         clean_doc_string(u8R"DOC(
             Applies a SQRT_Z_DAG gate to the simulator's state.
 
             Args:
                 *targets: The indices of the qubits to target with the gate.
         )DOC")
             .data());
 
     c.def(
         "sqrt_x",
-        [](TableauSimulator &self, pybind11::args args) {
+        [](PyTableauSimulator &self, pybind11::args args) {
             self.SQRT_X(args_to_targets(self, args));
         },
         clean_doc_string(u8R"DOC(
             Applies a SQRT_X gate to the simulator's state.
 
             Args:
                 *targets: The indices of the qubits to target with the gate.
         )DOC")
             .data());
 
     c.def(
         "sqrt_x_dag",
-        [](TableauSimulator &self, pybind11::args args) {
+        [](PyTableauSimulator &self, pybind11::args args) {
             self.SQRT_X_DAG(args_to_targets(self, args));
         },
         clean_doc_string(u8R"DOC(
             Applies a SQRT_X_DAG gate to the simulator's state.
 
             Args:
                 *targets: The indices of the qubits to target with the gate.
         )DOC")
             .data());
 
     c.def(
         "sqrt_y",
-        [](TableauSimulator &self, pybind11::args args) {
+        [](PyTableauSimulator &self, pybind11::args args) {
             self.SQRT_Y(args_to_targets(self, args));
         },
         clean_doc_string(u8R"DOC(
             Applies a SQRT_Y gate to the simulator's state.
 
             Args:
                 *targets: The indices of the qubits to target with the gate.
         )DOC")
             .data());
 
     c.def(
         "sqrt_y_dag",
-        [](TableauSimulator &self, pybind11::args args) {
+        [](PyTableauSimulator &self, pybind11::args args) {
             self.SQRT_Y_DAG(args_to_targets(self, args));
         },
         clean_doc_string(u8R"DOC(
             Applies a SQRT_Y_DAG gate to the simulator's state.
 
             Args:
                 *targets: The indices of the qubits to target with the gate.
         )DOC")
             .data());
 
     c.def(
         "swap",
-        [](TableauSimulator &self, pybind11::args args) {
+        [](PyTableauSimulator &self, pybind11::args args) {
             self.SWAP(args_to_target_pairs(self, args));
         },
         clean_doc_string(u8R"DOC(
             Applies a swap gate to the simulator's state.
 
             Args:
                 *targets: The indices of the qubits to target with the gate.
                     Applies the gate to the first two targets, then the next two targets, and so forth.
                     There must be an even number of targets.
         )DOC")
             .data());
 
     c.def(
         "iswap",
-        [](TableauSimulator &self, pybind11::args args) {
+        [](PyTableauSimulator &self, pybind11::args args) {
             self.ISWAP(args_to_target_pairs(self, args));
         },
         clean_doc_string(u8R"DOC(
             Applies an ISWAP gate to the simulator's state.
 
             Args:
                 *targets: The indices of the qubits to target with the gate.
                     Applies the gate to the first two targets, then the next two targets, and so forth.
                     There must be an even number of targets.
         )DOC")
             .data());
 
     c.def(
         "iswap_dag",
-        [](TableauSimulator &self, pybind11::args args) {
+        [](PyTableauSimulator &self, pybind11::args args) {
             self.ISWAP_DAG(args_to_target_pairs(self, args));
         },
         clean_doc_string(u8R"DOC(
             Applies an ISWAP_DAG gate to the simulator's state.
 
             Args:
                 *targets: The indices of the qubits to target with the gate.
                     Applies the gate to the first two targets, then the next two targets, and so forth.
                     There must be an even number of targets.
         )DOC")
             .data());
 
     c.def(
         "cnot",
-        [](TableauSimulator &self, pybind11::args args) {
+        [](PyTableauSimulator &self, pybind11::args args) {
+            self.ZCX(args_to_target_pairs(self, args));
+        },
+        clean_doc_string(u8R"DOC(
+            Applies a controlled X gate to the simulator's state.
+
+            Args:
+                *targets: The indices of the qubits to target with the gate.
+                    Applies the gate to the first two targets, then the next two targets, and so forth.
+                    There must be an even number of targets.
+        )DOC")
+            .data());
+
+    c.def(
+        "zcx",
+        [](PyTableauSimulator &self, pybind11::args args) {
+            self.ZCX(args_to_target_pairs(self, args));
+        },
+        clean_doc_string(u8R"DOC(
+            Applies a controlled X gate to the simulator's state.
+
+            Args:
+                *targets: The indices of the qubits to target with the gate.
+                    Applies the gate to the first two targets, then the next two targets, and so forth.
+                    There must be an even number of targets.
+        )DOC")
+            .data());
+
+    c.def(
+        "cx",
+        [](PyTableauSimulator &self, pybind11::args args) {
             self.ZCX(args_to_target_pairs(self, args));
         },
         clean_doc_string(u8R"DOC(
             Applies a controlled X gate to the simulator's state.
 
             Args:
                 *targets: The indices of the qubits to target with the gate.
                     Applies the gate to the first two targets, then the next two targets, and so forth.
                     There must be an even number of targets.
         )DOC")
             .data());
 
     c.def(
         "cz",
-        [](TableauSimulator &self, pybind11::args args) {
+        [](PyTableauSimulator &self, pybind11::args args) {
+            self.ZCZ(args_to_target_pairs(self, args));
+        },
+        clean_doc_string(u8R"DOC(
+            Applies a controlled Z gate to the simulator's state.
+
+            Args:
+                *targets: The indices of the qubits to target with the gate.
+                    Applies the gate to the first two targets, then the next two targets, and so forth.
+                    There must be an even number of targets.
+        )DOC")
+            .data());
+
+    c.def(
+        "zcz",
+        [](PyTableauSimulator &self, pybind11::args args) {
             self.ZCZ(args_to_target_pairs(self, args));
         },
         clean_doc_string(u8R"DOC(
             Applies a controlled Z gate to the simulator's state.
 
             Args:
                 *targets: The indices of the qubits to target with the gate.
                     Applies the gate to the first two targets, then the next two targets, and so forth.
                     There must be an even number of targets.
         )DOC")
             .data());
 
     c.def(
         "cy",
-        [](TableauSimulator &self, pybind11::args args) {
+        [](PyTableauSimulator &self, pybind11::args args) {
+            self.ZCY(args_to_target_pairs(self, args));
+        },
+        clean_doc_string(u8R"DOC(
+            Applies a controlled Y gate to the simulator's state.
+
+            Args:
+                *targets: The indices of the qubits to target with the gate.
+                    Applies the gate to the first two targets, then the next two targets, and so forth.
+                    There must be an even number of targets.
+        )DOC")
+            .data());
+
+    c.def(
+        "zcy",
+        [](PyTableauSimulator &self, pybind11::args args) {
             self.ZCY(args_to_target_pairs(self, args));
         },
         clean_doc_string(u8R"DOC(
             Applies a controlled Y gate to the simulator's state.
 
             Args:
                 *targets: The indices of the qubits to target with the gate.
                     Applies the gate to the first two targets, then the next two targets, and so forth.
                     There must be an even number of targets.
         )DOC")
             .data());
 
     c.def(
         "xcx",
-        [](TableauSimulator &self, pybind11::args args) {
+        [](PyTableauSimulator &self, pybind11::args args) {
             self.XCX(args_to_target_pairs(self, args));
         },
         clean_doc_string(u8R"DOC(
             Applies an X-controlled X gate to the simulator's state.
 
             Args:
                 *targets: The indices of the qubits to target with the gate.
                     Applies the gate to the first two targets, then the next two targets, and so forth.
                     There must be an even number of targets.
         )DOC")
             .data());
 
     c.def(
         "xcy",
-        [](TableauSimulator &self, pybind11::args args) {
+        [](PyTableauSimulator &self, pybind11::args args) {
             self.XCY(args_to_target_pairs(self, args));
         },
         clean_doc_string(u8R"DOC(
             Applies an X-controlled Y gate to the simulator's state.
 
             Args:
                 *targets: The indices of the qubits to target with the gate.
                     Applies the gate to the first two targets, then the next two targets, and so forth.
                     There must be an even number of targets.
         )DOC")
             .data());
 
     c.def(
         "xcz",
-        [](TableauSimulator &self, pybind11::args args) {
+        [](PyTableauSimulator &self, pybind11::args args) {
             self.XCZ(args_to_target_pairs(self, args));
         },
         clean_doc_string(u8R"DOC(
             Applies an X-controlled Z gate to the simulator's state.
 
             Args:
                 *targets: The indices of the qubits to target with the gate.
                     Applies the gate to the first two targets, then the next two targets, and so forth.
                     There must be an even number of targets.
         )DOC")
             .data());
 
     c.def(
         "ycx",
-        [](TableauSimulator &self, pybind11::args args) {
+        [](PyTableauSimulator &self, pybind11::args args) {
             self.YCX(args_to_target_pairs(self, args));
         },
         clean_doc_string(u8R"DOC(
             Applies a Y-controlled X gate to the simulator's state.
 
             Args:
                 *targets: The indices of the qubits to target with the gate.
                     Applies the gate to the first two targets, then the next two targets, and so forth.
                     There must be an even number of targets.
         )DOC")
             .data());
 
     c.def(
         "ycy",
-        [](TableauSimulator &self, pybind11::args args) {
+        [](PyTableauSimulator &self, pybind11::args args) {
             self.YCY(args_to_target_pairs(self, args));
         },
         clean_doc_string(u8R"DOC(
             Applies a Y-controlled Y gate to the simulator's state.
 
             Args:
                 *targets: The indices of the qubits to target with the gate.
                     Applies the gate to the first two targets, then the next two targets, and so forth.
                     There must be an even number of targets.
         )DOC")
             .data());
 
     c.def(
         "ycz",
-        [](TableauSimulator &self, pybind11::args args) {
+        [](PyTableauSimulator &self, pybind11::args args) {
             self.YCZ(args_to_target_pairs(self, args));
         },
         clean_doc_string(u8R"DOC(
             Applies a Y-controlled Z gate to the simulator's state.
 
             Args:
                 *targets: The indices of the qubits to target with the gate.
                     Applies the gate to the first two targets, then the next two targets, and so forth.
                     There must be an even number of targets.
         )DOC")
             .data());
 
     c.def(
         "reset",
-        [](TableauSimulator &self, pybind11::args args) {
+        [](PyTableauSimulator &self, pybind11::args args) {
+            self.reset_z(args_to_targets(self, args));
+        },
+        clean_doc_string(u8R"DOC(
+            Resets qubits to the |0> state.
+
+            Args:
+                *targets: The indices of the qubits to reset.
+
+            Example:
+                >>> import stim
+                >>> s = stim.TableauSimulator()
+                >>> s.x(0)
+                >>> s.reset(0)
+                >>> s.peek_bloch(0)
+                stim.PauliString("+Z")
+        )DOC")
+            .data());
+
+    c.def(
+        "reset_x",
+        [](PyTableauSimulator &self, pybind11::args args) {
+            self.reset_x(args_to_targets(self, args));
+        },
+        clean_doc_string(u8R"DOC(
+            Resets qubits to the |+> state.
+
+            Args:
+                *targets: The indices of the qubits to reset.
+
+            Example:
+                >>> import stim
+                >>> s = stim.TableauSimulator()
+                >>> s.reset_x(0)
+                >>> s.peek_bloch(0)
+                stim.PauliString("+X")
+        )DOC")
+            .data());
+
+    c.def(
+        "reset_y",
+        [](PyTableauSimulator &self, pybind11::args args) {
+            self.reset_y(args_to_targets(self, args));
+        },
+        clean_doc_string(u8R"DOC(
+            Resets qubits to the |i> state.
+
+            Args:
+                *targets: The indices of the qubits to reset.
+
+            Example:
+                >>> import stim
+                >>> s = stim.TableauSimulator()
+                >>> s.reset_y(0)
+                >>> s.peek_bloch(0)
+                stim.PauliString("+Y")
+        )DOC")
+            .data());
+
+    c.def(
+        "reset_z",
+        [](PyTableauSimulator &self, pybind11::args args) {
             self.reset_z(args_to_targets(self, args));
         },
         clean_doc_string(u8R"DOC(
-            Resets qubits to zero (e.g. by swapping them for zero'd qubit from the environment).
+            Resets qubits to the |0> state.
 
             Args:
                 *targets: The indices of the qubits to reset.
+
+            Example:
+                >>> import stim
+                >>> s = stim.TableauSimulator()
+                >>> s.h(0)
+                >>> s.reset_z(0)
+                >>> s.peek_bloch(0)
+                stim.PauliString("+Z")
+        )DOC")
+            .data());
+
+    c.def(
+        "peek_x",
+        [](PyTableauSimulator &self, uint32_t target) -> int8_t {
+            self.ensure_large_enough_for_qubits(target + 1);
+            return self.peek_x(target);
+        },
+        pybind11::arg("target"),
+        clean_doc_string(u8R"DOC(
+            Returns the expected value of a qubit's X observable (which will always be -1, 0, or +1).
+
+            This is a non-physical operation.
+            It reports information about the quantum state without disturbing it.
+
+            Args:
+                target: The qubit to analyze.
+
+            Returns:
+                +1: Qubit is in the |+> state.
+                -1: Qubit is in the |-> state.
+                0: Qubit is in some other state.
+
+            Example:
+                >>> import stim
+                >>> s = stim.TableauSimulator()
+                >>> s.reset_z(0)
+                >>> s.peek_x(0)
+                0
+                >>> s.reset_x(0)
+                >>> s.peek_x(0)
+                1
+                >>> s.z(0)
+                >>> s.peek_x(0)
+                -1
+        )DOC")
+            .data());
+
+    c.def(
+        "peek_y",
+        [](PyTableauSimulator &self, uint32_t target) -> int8_t {
+            self.ensure_large_enough_for_qubits(target + 1);
+            return self.peek_y(target);
+        },
+        pybind11::arg("target"),
+        clean_doc_string(u8R"DOC(
+            Returns the expected value of a qubit's Y observable (which will always be -1, 0, or +1).
+
+            This is a non-physical operation.
+            It reports information about the quantum state without disturbing it.
+
+            Args:
+                target: The qubit to analyze.
+
+            Returns:
+                +1: Qubit is in the |i> state.
+                -1: Qubit is in the |-i> state.
+                0: Qubit is in some other state.
+
+            Example:
+                >>> import stim
+                >>> s = stim.TableauSimulator()
+                >>> s.reset_z(0)
+                >>> s.peek_y(0)
+                0
+                >>> s.reset_y(0)
+                >>> s.peek_y(0)
+                1
+                >>> s.z(0)
+                >>> s.peek_y(0)
+                -1
+        )DOC")
+            .data());
+
+    c.def(
+        "peek_z",
+        [](PyTableauSimulator &self, uint32_t target) -> int8_t {
+            self.ensure_large_enough_for_qubits(target + 1);
+            return self.peek_z(target);
+        },
+        pybind11::arg("target"),
+        clean_doc_string(u8R"DOC(
+            Returns the expected value of a qubit's Z observable (which will always be -1, 0, or +1).
+
+            This is a non-physical operation.
+            It reports information about the quantum state without disturbing it.
+
+            Args:
+                target: The qubit to analyze.
+
+            Returns:
+                +1: Qubit is in the |0> state.
+                -1: Qubit is in the |1> state.
+                0: Qubit is in some other state.
+
+            Example:
+                >>> import stim
+                >>> s = stim.TableauSimulator()
+                >>> s.reset_x(0)
+                >>> s.peek_z(0)
+                0
+                >>> s.reset_z(0)
+                >>> s.peek_z(0)
+                1
+                >>> s.x(0)
+                >>> s.peek_z(0)
+                -1
         )DOC")
             .data());
 
     c.def(
         "peek_bloch",
-        [](TableauSimulator &self, size_t target) {
+        [](PyTableauSimulator &self, size_t target) {
             self.ensure_large_enough_for_qubits(target + 1);
             return PyPauliString(self.peek_bloch(target));
         },
         pybind11::arg("target"),
         clean_doc_string(u8R"DOC(
             Returns the current bloch vector of the qubit, represented as a stim.PauliString.
 
@@ -711,15 +1146,15 @@
                 >>> s.peek_bloch(0)
                 stim.PauliString("+_")
         )DOC")
             .data());
 
     c.def(
         "peek_observable_expectation",
-        [](const TableauSimulator &self, const PyPauliString &observable) -> int8_t {
+        [](const PyTableauSimulator &self, const PyPauliString &observable) -> int8_t {
             if (observable.imag) {
                 throw std::invalid_argument(
                     "Observable isn't Hermitian; it has imaginary sign. Need observable.sign in [1, -1].");
             }
             return self.peek_observable_expectation(observable.value);
         },
         pybind11::arg("observable"),
@@ -763,15 +1198,15 @@
                 II 1
                 IIZ 1
         )DOC")
             .data());
 
     c.def(
         "measure",
-        [](TableauSimulator &self, uint32_t target) {
+        [](PyTableauSimulator &self, uint32_t target) {
             self.ensure_large_enough_for_qubits(target + 1);
             self.measure_z(TempViewableData({GateTarget{target}}));
             return (bool)self.measurement_record.storage.back();
         },
         pybind11::arg("target"),
         clean_doc_string(u8R"DOC(
             Measures a single qubit.
@@ -788,15 +1223,15 @@
             Returns:
                 The measurement result as a bool.
         )DOC")
             .data());
 
     c.def(
         "measure_many",
-        [](TableauSimulator &self, pybind11::args args) {
+        [](PyTableauSimulator &self, pybind11::args args) {
             auto converted_args = args_to_targets(self, args);
             self.measure_z(converted_args);
             auto e = self.measurement_record.storage.end();
             return std::vector<bool>(e - converted_args.targets.size(), e);
         },
         clean_doc_string(u8R"DOC(
             Measures multiple qubits.
@@ -806,18 +1241,134 @@
 
             Returns:
                 The measurement results as a list of bools.
         )DOC")
             .data());
 
     c.def(
+        "postselect_x",
+        [](PyTableauSimulator &self, const pybind11::object &targets, bool desired_value) {
+            auto gate_targets = arg_to_qubit_or_qubits(self, targets);
+            self.postselect_x(gate_targets, desired_value);
+        },
+        pybind11::arg("targets"),
+        pybind11::kw_only(),
+        pybind11::arg("desired_value"),
+        clean_doc_string(u8R"DOC(
+            @signature def postselect_x(self, targets: Union[int, Iterable[int]], *, desired_value: bool) -> None:
+            Postselects qubits in the X basis, or raises an exception.
+
+            Postselecting a qubit forces it to collapse to a specific state, as
+            if it was measured and that state was the result of the measurement.
+
+            Args:
+                targets: The qubit index or indices to postselect.
+                desired_value:
+                    False: postselect targets into the |+> state.
+                    True: postselect targets into the |-> state.
+
+            Raises:
+                ValueError:
+                    The postselection failed. One of the qubits was in a state
+                    orthogonal to the desired state, so it was literally
+                    impossible for a measurement of the qubit to return the
+                    desired result.
+        )DOC")
+            .data());
+
+    c.def(
+        "postselect_y",
+        [](PyTableauSimulator &self, const pybind11::object &targets, bool desired_value) {
+            auto gate_targets = arg_to_qubit_or_qubits(self, targets);
+            self.postselect_y(gate_targets, desired_value);
+        },
+        pybind11::arg("targets"),
+        pybind11::kw_only(),
+        pybind11::arg("desired_value"),
+        clean_doc_string(u8R"DOC(
+            @signature def postselect_y(self, targets: Union[int, Iterable[int]], *, desired_value: bool) -> None:
+            Postselects qubits in the Y basis, or raises an exception.
+
+            Postselecting a qubit forces it to collapse to a specific state, as
+            if it was measured and that state was the result of the measurement.
+
+            Args:
+                targets: The qubit index or indices to postselect.
+                desired_value:
+                    False: postselect targets into the |i> state.
+                    True: postselect targets into the |-i> state.
+
+            Raises:
+                ValueError:
+                    The postselection failed. One of the qubits was in a state
+                    orthogonal to the desired state, so it was literally
+                    impossible for a measurement of the qubit to return the
+                    desired result.
+        )DOC")
+            .data());
+
+    c.def(
+        "postselect_z",
+        [](PyTableauSimulator &self, const pybind11::object &targets, bool desired_value) {
+            auto gate_targets = arg_to_qubit_or_qubits(self, targets);
+            self.postselect_z(gate_targets, desired_value);
+        },
+        pybind11::arg("targets"),
+        pybind11::kw_only(),
+        pybind11::arg("desired_value"),
+        clean_doc_string(u8R"DOC(
+            @signature def postselect_z(self, targets: Union[int, Iterable[int]], *, desired_value: bool) -> None:
+            Postselects qubits in the Z basis, or raises an exception.
+
+            Postselecting a qubit forces it to collapse to a specific state, as
+            if it was measured and that state was the result of the measurement.
+
+            Args:
+                targets: The qubit index or indices to postselect.
+                desired_value:
+                    False: postselect targets into the |0> state.
+                    True: postselect targets into the |1> state.
+
+            Raises:
+                ValueError:
+                    The postselection failed. One of the qubits was in a state
+                    orthogonal to the desired state, so it was literally
+                    impossible for a measurement of the qubit to return the
+                    desired result.
+        )DOC")
+            .data());
+
+    c.def_property_readonly(
+        "num_qubits",
+        [](const PyTableauSimulator &self) -> size_t {
+            return self.inv_state.num_qubits;
+        },
+        clean_doc_string(u8R"DOC(
+            Returns the number of qubits currently being tracked by the simulator's internal state.
+
+            Note that the number of qubits being tracked will implicitly increase if qubits beyond
+            the current limit are touched. Untracked qubits are always assumed to be in the |0> state.
+
+            Examples:
+                >>> import stim
+                >>> s = stim.TableauSimulator()
+                >>> s.num_qubits
+                0
+                >>> s.h(2)
+                >>> s.num_qubits
+                3
+        )DOC")
+            .data());
+
+    c.def(
         "set_num_qubits",
-        [](TableauSimulator &self, uint32_t new_num_qubits) {
+        [](PyTableauSimulator &self, uint32_t new_num_qubits) {
             self.set_num_qubits(new_num_qubits);
         },
+        pybind11::arg("new_num_qubits"),
         clean_doc_string(u8R"DOC(
             Forces the simulator's internal state to track exactly the qubits whose indices are in range(new_num_qubits).
 
             Note that untracked qubits are always assumed to be in the |0> state. Therefore, calling this method
             will effectively force any qubit whose index is outside range(new_num_qubits) to be reset to |0>.
 
             Note that this method does not prevent future operations from implicitly expanding the size of the
@@ -842,17 +1393,18 @@
                 >>> s.measure_many(0, 1, 2, 3)
                 [True, True, False, False]
         )DOC")
             .data());
 
     c.def(
         "set_inverse_tableau",
-        [](TableauSimulator &self, const Tableau &new_inverse_tableau) {
+        [](PyTableauSimulator &self, const Tableau &new_inverse_tableau) {
             self.inv_state = new_inverse_tableau;
         },
+        pybind11::arg("new_inverse_tableau"),
         clean_doc_string(u8R"DOC(
             Overwrites the simulator's internal state with a copy of the given inverse tableau.
 
             The inverse tableau specifies how Pauli product observables of qubits at the current time transform
             into equivalent Pauli product observables at the beginning of time, when all qubits were in the
             |0> state. For example, if the Z observable on qubit 5 maps to a product of Z observables at the
             start of time then a Z basis measurement on qubit 5 will be deterministic and equal to the sign
@@ -872,16 +1424,16 @@
                 >>> s.current_inverse_tableau() == t
                 True
         )DOC")
             .data());
 
     c.def(
         "copy",
-        [](TableauSimulator &self) {
-            TableauSimulator copy = self;
+        [](const PyTableauSimulator &self) {
+            PyTableauSimulator copy = self;
             return copy;
         },
         clean_doc_string(u8R"DOC(
             Returns a copy of the simulator. A simulator with the same internal state.
 
             Examples:
                 >>> import stim
@@ -907,15 +1459,15 @@
                 >>> s.measure(0)
                 True
         )DOC")
             .data());
 
     c.def(
         "measure_kickback",
-        [](TableauSimulator &self, uint32_t target) {
+        [](PyTableauSimulator &self, uint32_t target) {
             self.ensure_large_enough_for_qubits(target + 1);
             auto result = self.measure_kickback_z({target});
             if (result.second.num_qubits == 0) {
                 return pybind11::make_tuple(result.first, pybind11::none());
             }
             return pybind11::make_tuple(result.first, PyPauliString(result.second));
         },
```

### Comparing `stim-1.8.0/src/stim/simulators/vector_simulator.cc` & `stim-1.9.0/src/stim/simulators/vector_simulator.cc`

 * *Files 15% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 
 #include "stim/simulators/vector_simulator.h"
 
 #include <cassert>
 
 #include "stim/circuit/gate_data.h"
 #include "stim/mem/simd_util.h"
+#include "stim/probability_util.h"
 #include "stim/stabilizers/pauli_string.h"
 
 using namespace stim;
 
 VectorSimulator::VectorSimulator(size_t num_qubits) {
     state.resize(size_t{1} << num_qubits, 0.0f);
     state[0] = 1;
@@ -103,32 +104,43 @@
             apply("X", q);
         } else if (z) {
             apply("Z", q);
         }
     }
 }
 
-VectorSimulator VectorSimulator::from_stabilizers(const std::vector<PauliStringRef> stabilizers, std::mt19937_64 &rng) {
+std::vector<std::complex<float>> VectorSimulator::state_vector_from_stabilizers(
+    const std::vector<PauliStringRef> &stabilizers, float norm2) {
     size_t num_qubits = stabilizers.empty() ? 0 : stabilizers[0].num_qubits;
-    VectorSimulator result(num_qubits);
+    VectorSimulator sim(num_qubits);
 
     // Create an initial state $|A\rangle^{\otimes n}$ which overlaps with all possible stabilizers.
     std::uniform_real_distribution<float> dist(-1.0, +1.0);
-    for (size_t k = 0; k < result.state.size(); k++) {
-        result.state[k] = {dist(rng), dist(rng)};
+
+    auto rng = externally_seeded_rng();
+    for (auto &s : sim.state) {
+        s = {dist(rng), dist(rng)};
     }
 
     // Project out the non-overlapping parts.
     for (const auto &p : stabilizers) {
-        result.project(p);
+        sim.project(p);
     }
     if (stabilizers.empty()) {
-        result.project(PauliString(0));
+        sim.project(PauliString(0));
     }
 
+    sim.canonicalize_assuming_stabilizer_state(norm2);
+
+    return sim.state;
+}
+
+VectorSimulator VectorSimulator::from_stabilizers(const std::vector<PauliStringRef> &stabilizers) {
+    VectorSimulator result(0);
+    result.state = state_vector_from_stabilizers(stabilizers, 1);
     return result;
 }
 
 float VectorSimulator::project(const PauliStringRef &observable) {
     assert(1ULL << observable.num_qubits == state.size());
     auto basis_change = [&]() {
         for (size_t k = 0; k < observable.num_qubits; k++) {
@@ -204,7 +216,46 @@
     out << "VectorSimulator {\n";
     for (size_t k = 0; k < sim.state.size(); k++) {
         out << "    " << k << ": " << sim.state[k] << "\n";
     }
     out << "}";
     return out;
 }
+
+void VectorSimulator::canonicalize_assuming_stabilizer_state(double norm2) {
+    // Find a solid non-zero entry.
+    size_t nz = 0;
+    for (size_t k = 1; k < state.size(); k++) {
+        if (abs(state[k]) > abs(state[nz]) * 2) {
+            nz = k;
+        }
+    }
+
+    // Rescale so that the non-zero entries are 1, -1, 1j, or -1j.
+    size_t num_non_zero = 0;
+    std::complex<float> big_v = state[nz];
+    for (auto &v : state) {
+        v /= big_v;
+        if (abs(v) < 0.1) {
+            v = 0;
+            continue;
+        }
+        num_non_zero++;
+        if (abs(v - std::complex<float>{1, 0}) < 0.1) {
+            v = std::complex<float>{1, 0};
+        } else if (abs(v - std::complex<float>{0, 1}) < 0.1) {
+            v = std::complex<float>{0, 1};
+        } else if (abs(v - std::complex<float>{-1, 0}) < 0.1) {
+            v = std::complex<float>{-1, 0};
+        } else if (abs(v - std::complex<float>{0, -1}) < 0.1) {
+            v = std::complex<float>{0, -1};
+        } else {
+            throw std::invalid_argument("State vector extraction failed. This shouldn't occur.");
+        }
+    }
+
+    // Normalize the entries so the result is a unit vector.
+    std::complex<float> scale = (float)(sqrt(norm2 / (double)num_non_zero));
+    for (auto &v : state) {
+        v *= scale;
+    }
+}
```

### Comparing `stim-1.8.0/src/stim/stabilizers/pauli_string.cc` & `stim-1.9.0/src/stim/stabilizers/pauli_string.cc`

 * *Files identical despite different names*

### Comparing `stim-1.8.0/src/stim/stabilizers/pauli_string.pybind.cc` & `stim-1.9.0/src/stim/stabilizers/pauli_string.pybind.cc`

 * *Files 1% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 #include "stim/py/base.pybind.h"
 #include "stim/simulators/tableau_simulator.h"
 #include "stim/stabilizers/pauli_string.pybind.h"
 #include "stim/stabilizers/tableau.h"
 #include "stim/stabilizers/tableau.pybind.h"
 
 using namespace stim;
+using namespace stim_pybind;
 
 PyPauliString::PyPauliString(const PauliStringRef val, bool imag) : value(val), imag(imag) {
 }
 
 PyPauliString::PyPauliString(PauliString &&val, bool imag) : value(std::move(val)), imag(imag) {
 }
 
@@ -214,15 +215,14 @@
     return value;
 }
 
 void pybind_pauli_string(pybind11::module &m) {
     auto c = pybind11::class_<PyPauliString>(
         m,
         "PauliString",
-        pybind11::module_local(),
         clean_doc_string(u8R"DOC(
             A signed Pauli tensor product (e.g. "+X \u2297 X \u2297 X" or "-Y \u2297 Z".
 
             Represents a collection of Pauli operations (I, X, Y, Z) applied pairwise to a collection of qubits.
 
             Examples:
                 >>> import stim
@@ -337,15 +337,15 @@
                 pauli_indices: A sequence of integers from 0 to 3 (inclusive) indicating paulis.
         )DOC")
             .data());
 
     c.def_static(
         "random",
         [](size_t num_qubits, bool allow_imaginary) {
-            std::shared_ptr<std::mt19937_64> rng = PYBIND_SHARED_RNG(pybind11::none());
+            auto rng = make_py_seeded_rng(pybind11::none());
             return PyPauliString(PauliString::random(num_qubits, *rng), allow_imaginary ? ((*rng)() & 1) : false);
         },
         pybind11::arg("num_qubits"),
         pybind11::kw_only(),
         pybind11::arg("allow_imaginary") = false,
         clean_doc_string(u8R"DOC(
             Samples a uniformly random Hermitian Pauli string over the given number of qubits.
@@ -591,15 +591,15 @@
             return self * lhs;
         },
         pybind11::arg("lhs"),
         clean_doc_string(u8R"DOC(
             Left-multiplies the Pauli string by another Pauli string, a complex unit, or a tensor power.
 
             Args:
-                rhs: The left hand side of the multiplication. This can be:
+                lhs: The left hand side of the multiplication. This can be:
                     - A stim.PauliString to left-multiply term-by-term into the paulis of the pauli string.
                     - A complex unit (1, -1, 1j, -1j) to multiply into the sign of the pauli string.
                     - A non-negative integer indicating the tensor power to raise the pauli string to (how many times to repeat it).
 
             Examples:
                 >>> import stim
 
@@ -670,17 +670,14 @@
                 >>> p = stim.PauliString("X")
                 >>> p *= stim.PauliString("_YY")
                 >>> p
                 stim.PauliString("+XYY")
 
             Returns:
                 The mutated Pauli string.
-
-            Raises:
-                ValueError: The Pauli strings have different lengths.
         )DOC")
             .data());
 
     c.def(
         "__itruediv__",
         &PyPauliString::operator/=,
         pybind11::is_operator(),
@@ -872,14 +869,16 @@
             } else {
                 return pybind11::cast(self.value.py_get_item(start));
             }
         },
         pybind11::arg("index_or_slice"),
         clean_doc_string(u8R"DOC(
             Returns an individual Pauli or Pauli string slice from the pauli string.
+            @overload def __getitem__(self, index_or_slice: int) -> int:
+            @overload def __getitem__(self, index_or_slice: slice) -> stim.PauliString:
 
             Individual Paulis are returned as an int using the encoding 0=I, 1=X, 2=Y, 3=Z.
             Slices are returned as a stim.PauliString (always with positive sign).
 
             Examples:
                 >>> import stim
                 >>> p = stim.PauliString("_XYZ")
```

### Comparing `stim-1.8.0/src/stim/stabilizers/pauli_string_ref.cc` & `stim-1.9.0/src/stim/stabilizers/pauli_string_ref.cc`

 * *Files identical despite different names*

### Comparing `stim-1.8.0/src/stim/stabilizers/tableau.cc` & `stim-1.9.0/src/stim/stabilizers/tableau.cc`

 * *Files 4% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 #include <iostream>
 #include <map>
 #include <random>
 #include <sstream>
 #include <thread>
 
 #include "stim/circuit/gate_data.h"
+#include "stim/simulators/vector_simulator.h"
 #include "stim/stabilizers/pauli_string.h"
 #include "stim/stabilizers/tableau_transposed_raii.h"
 
 using namespace stim;
 
 void Tableau::expand(size_t new_num_qubits) {
     // If the new qubits fit inside the padding, just extend into it.
@@ -594,7 +595,58 @@
         result.zs[k] = xs[k].xs[input_index];
     }
     if (!skip_sign) {
         result.sign = (*this)(result).sign;
     }
     return result;
 }
+
+std::vector<std::complex<float>> Tableau::to_flat_unitary_matrix(bool little_endian) const {
+    VectorSimulator sim(2 * num_qubits);
+
+    std::vector<PauliString> pauli_strings;
+    size_t nw = xs[0].xs.num_simd_words;
+
+    // Add X transformation stabilizers.
+    for (size_t k = 0; k < num_qubits; k++) {
+        PauliString p(num_qubits * 2);
+        p.xs.word_range_ref(0, nw) = xs[k].xs;
+        p.zs.word_range_ref(0, nw) = xs[k].zs;
+        p.sign = xs[k].sign;
+        p.xs[num_qubits + k] ^= true;
+        pauli_strings.push_back(p);
+    }
+
+    // Add Z transformation stabilizers.
+    for (size_t k = 0; k < num_qubits; k++) {
+        PauliString p(num_qubits * 2);
+        p.xs.word_range_ref(0, nw) = zs[k].xs;
+        p.zs.word_range_ref(0, nw) = zs[k].zs;
+        p.sign = zs[k].sign;
+        p.zs[num_qubits + k] ^= true;
+        pauli_strings.push_back(p);
+    }
+
+    for (auto &p : pauli_strings) {
+        for (size_t q = 0; q < num_qubits - q - 1; q++) {
+            size_t q2 = num_qubits - q - 1;
+            if (!little_endian) {
+                p.xs[q].swap_with(p.xs[q2]);
+                p.zs[q].swap_with(p.zs[q2]);
+                p.xs[q + num_qubits].swap_with(p.xs[q2 + num_qubits]);
+                p.zs[q + num_qubits].swap_with(p.zs[q2 + num_qubits]);
+            }
+        }
+        for (size_t q = 0; q < num_qubits; q++) {
+            p.xs[q].swap_with(p.xs[q + num_qubits]);
+            p.zs[q].swap_with(p.zs[q + num_qubits]);
+        }
+    }
+
+    // Turn it into a vector.
+    std::vector<PauliStringRef> refs;
+    for (const auto &e : pauli_strings) {
+        refs.push_back(e.ref());
+    }
+
+    return VectorSimulator::state_vector_from_stabilizers(refs, 1 << num_qubits);
+}
```

### Comparing `stim-1.8.0/src/stim/stabilizers/tableau.pybind.cc` & `stim-1.9.0/src/stim/stabilizers/tableau.pybind.cc`

 * *Files 8% similar despite different names*

```diff
@@ -17,20 +17,20 @@
 #include "stim/py/base.pybind.h"
 #include "stim/simulators/tableau_simulator.h"
 #include "stim/stabilizers/pauli_string.h"
 #include "stim/stabilizers/pauli_string.pybind.h"
 #include "stim/stabilizers/tableau.h"
 
 using namespace stim;
+using namespace stim_pybind;
 
 void pybind_tableau(pybind11::module &m) {
     auto c = pybind11::class_<Tableau>(
         m,
         "Tableau",
-        pybind11::module_local(),
         clean_doc_string(u8R"DOC(
             A stabilizer tableau.
 
             Represents a Clifford operation by explicitly storing how that operation conjugates a list of Pauli
             group generators into composite Pauli products.
 
             Examples:
@@ -82,15 +82,15 @@
                 num_qubits: The number of qubits the tableau's operation acts on.
         )DOC")
             .data());
 
     c.def_static(
         "random",
         [](size_t num_qubits) {
-            return Tableau::random(num_qubits, *PYBIND_SHARED_RNG(pybind11::none()));
+            return Tableau::random(num_qubits, *make_py_seeded_rng(pybind11::none()));
         },
         pybind11::arg("num_qubits"),
         clean_doc_string(u8R"DOC(
             Samples a uniformly random Clifford operation over the given number of qubits and returns its tableau.
 
             Args:
                 num_qubits: The number of qubits the tableau should act on.
@@ -105,14 +105,73 @@
             References:
                 "Hadamard-free circuits expose the structure of the Clifford group"
                 Sergey Bravyi, Dmitri Maslov
                 https://arxiv.org/abs/2003.09412
         )DOC")
             .data());
 
+    c.def(
+        "to_unitary_matrix",
+        [](Tableau &self, const std::string &endian) {
+            bool little_endian;
+            if (endian == "little") {
+                little_endian = true;
+            } else if (endian == "big") {
+                little_endian = false;
+            } else {
+                throw std::invalid_argument("endian not in ['little', 'big']");
+            }
+            auto data = self.to_flat_unitary_matrix(little_endian);
+
+            void *ptr = data.data();
+            pybind11::ssize_t itemsize = sizeof(float) * 2;
+            pybind11::ssize_t n = 1 << self.num_qubits;
+            std::vector<pybind11::ssize_t> shape{n, n};
+            std::vector<pybind11::ssize_t> stride{n * itemsize, itemsize};
+            const std::string &format = pybind11::format_descriptor<std::complex<float>>::value;
+            bool readonly = true;
+            return pybind11::array_t<float>(
+                pybind11::buffer_info(ptr, itemsize, format, shape.size(), shape, stride, readonly));
+        },
+        pybind11::kw_only(),
+        pybind11::arg("endian"),
+        clean_doc_string(u8R"DOC(
+            @signature def to_unitary_matrix(self, *, endian: str) -> np.ndarray[np.complex64]:
+            Converts the tableau into a unitary matrix.
+
+            Args:
+                endian:
+                    "little": The first qubit is the least significant (corresponds
+                        to an offset of 1 in the state vector).
+                    "big": The first qubit is the most significant (corresponds
+                        to an offset of 2**(n - 1) in the state vector).
+
+            Returns:
+                A numpy array with dtype=np.complex64 and shape=(1 << len(tableau), 1 << len(tableau)).
+
+            Example:
+                >>> import stim
+                >>> cnot = stim.Tableau.from_conjugated_generators(
+                ...     xs=[
+                ...         stim.PauliString("XX"),
+                ...         stim.PauliString("_X"),
+                ...     ],
+                ...     zs=[
+                ...         stim.PauliString("Z_"),
+                ...         stim.PauliString("ZZ"),
+                ...     ],
+                ... )
+                >>> cnot.to_unitary_matrix(endian='big')
+                array([[1.+0.j, 0.+0.j, 0.+0.j, 0.+0.j],
+                       [0.+0.j, 1.+0.j, 0.+0.j, 0.+0.j],
+                       [0.+0.j, 0.+0.j, 0.+0.j, 1.+0.j],
+                       [0.+0.j, 0.+0.j, 1.+0.j, 0.+0.j]], dtype=complex64)
+        )DOC")
+            .data());
+
     c.def_static(
         "from_named_gate",
         [](const char *name) {
             const Gate &gate = GATE_DATA.at(name);
             if (!(gate.flags & GATE_IS_UNITARY)) {
                 throw std::out_of_range("Recognized name, but not unitary: " + std::string(name));
             }
@@ -752,15 +811,15 @@
                 >>> import stim
 
                 # Check equivalence with the inverse's x_output.
                 >>> t = stim.Tableau.random(4)
                 >>> expected = t.inverse().x_output(0)
                 >>> t.inverse_x_output(0) == expected
                 True
-                >>> expected.sign = +1;
+                >>> expected.sign = +1
                 >>> t.inverse_x_output(0, unsigned=True) == expected
                 True
         )DOC")
             .data());
 
     c.def(
         "inverse_y_output",
@@ -788,15 +847,15 @@
                 >>> import stim
 
                 # Check equivalence with the inverse's y_output.
                 >>> t = stim.Tableau.random(4)
                 >>> expected = t.inverse().y_output(0)
                 >>> t.inverse_y_output(0) == expected
                 True
-                >>> expected.sign = +1;
+                >>> expected.sign = +1
                 >>> t.inverse_y_output(0, unsigned=True) == expected
                 True
         )DOC")
             .data());
 
     c.def(
         "inverse_z_output",
@@ -826,15 +885,15 @@
                 >>> import stim
 
                 # Check equivalence with the inverse's z_output.
                 >>> t = stim.Tableau.random(4)
                 >>> expected = t.inverse().z_output(0)
                 >>> t.inverse_z_output(0) == expected
                 True
-                >>> expected.sign = +1;
+                >>> expected.sign = +1
                 >>> t.inverse_z_output(0, unsigned=True) == expected
                 True
         )DOC")
             .data());
 
     c.def(
         "copy",
```

### Comparing `stim-1.8.0/src/stim/stabilizers/tableau_specialized_prepend.cc` & `stim-1.9.0/src/stim/stabilizers/tableau_specialized_prepend.cc`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     zs[q].sign ^= 1;
 }
 
 void Tableau::prepend_Z(size_t q) {
     xs[q].sign ^= 1;
 }
 
-void Tableau::prepend(const PauliStringRef &op) {
+void Tableau::prepend_pauli_product(const PauliStringRef &op) {
     assert(op.num_qubits == num_qubits);
     zs.signs ^= op.xs;
     xs.signs ^= op.zs;
 }
 
 struct IgnoreAntiCommute {
     PauliStringRef rhs;
```

### Comparing `stim-1.8.0/src/stim/stabilizers/tableau_transposed_raii.cc` & `stim-1.9.0/src/stim/stabilizers/tableau_transposed_raii.cc`

 * *Files identical despite different names*

### Comparing `stim-1.8.0/src/stim.cc` & `stim-1.9.0/src/stim.cc`

 * *Files identical despite different names*

### Comparing `stim-1.8.0/stim.egg-info/PKG-INFO` & `stim-1.9.0/stim.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: stim
-Version: 1.8.0
-Summary: A fast quantum stabilizer circuit simulator.
+Version: 1.9.0
+Summary: A fast library for analyzing with quantum stabilizer circuits.
 Home-page: https://github.com/quantumlib/stim
 Author: Craig Gidney
 Author-email: craig.gidney@gmail.com
 License: Apache 2
 Platform: UNKNOWN
 Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown
```

