# Comparing `tmp/pyuff_ustb-2.0.0.tar.gz` & `tmp/pyuff_ustb-2.0.1.tar.gz`

## Comparing `pyuff_ustb-2.0.0.tar` & `pyuff_ustb-2.0.1.tar`

### file list

```diff
@@ -1,92 +1,91 @@
--rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.0/.readthedocs.yaml
--rw-r--r--   0        0        0    12112 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.0/my_sector_scan.uff
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.0/requirements.txt
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.0/setup.py
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.0/.vscode/settings.json
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.0/docs/Makefile
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.0/docs/api-reference.rst
--rw-r--r--   0        0        0     1361 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.0/docs/conf.py
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.0/docs/index.rst
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.0/docs/make.bat
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.0/docs/requirements.txt
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.0/docs/_autosummary/pyuff.common.get_class_from_name.rst
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.0/docs/_autosummary/pyuff.common.get_name_from_class.rst
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.0/docs/_autosummary/pyuff.common.rst
--rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.0/docs/_autosummary/pyuff.objects.Apodization.rst
--rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.0/docs/_autosummary/pyuff.objects.BeamformedData.rst
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.0/docs/_autosummary/pyuff.objects.ChannelData.rst
--rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.0/docs/_autosummary/pyuff.objects.CurvilinearArray.rst
--rw-r--r--   0        0        0     1434 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.0/docs/_autosummary/pyuff.objects.CurvilinearMatrixArray.rst
--rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.0/docs/_autosummary/pyuff.objects.LinearArray.rst
--rw-r--r--   0        0        0      825 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.0/docs/_autosummary/pyuff.objects.LinearScan.rst
--rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.0/docs/_autosummary/pyuff.objects.MatrixArray.rst
--rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.0/docs/_autosummary/pyuff.objects.Phantom.rst
--rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.0/docs/_autosummary/pyuff.objects.Point.rst
--rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.0/docs/_autosummary/pyuff.objects.Probe.rst
--rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.0/docs/_autosummary/pyuff.objects.Pulse.rst
--rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.0/docs/_autosummary/pyuff.objects.Scan.rst
--rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.0/docs/_autosummary/pyuff.objects.SectorScan.rst
--rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.0/docs/_autosummary/pyuff.objects.Uff.rst
--rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.0/docs/_autosummary/pyuff.objects.Wave.rst
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.0/docs/_autosummary/pyuff.objects.Wavefront.rst
--rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.0/docs/_autosummary/pyuff.objects.Window.rst
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.0/docs/_autosummary/pyuff.objects.eager_load.rst
--rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.0/docs/_autosummary/pyuff.objects.rst
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.0/docs/_autosummary/pyuff.objects.write_object.rst
--rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.0/docs/_autosummary/pyuff.readers.H5Reader.rst
--rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.0/docs/_autosummary/pyuff.readers.LazyArray.rst
--rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.0/docs/_autosummary/pyuff.readers.LazyScalar.rst
--rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.0/docs/_autosummary/pyuff.readers.NoneReader.rst
--rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.0/docs/_autosummary/pyuff.readers.Reader.rst
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.0/docs/_autosummary/pyuff.readers.ReaderAttrsKeyError.rst
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.0/docs/_autosummary/pyuff.readers.ReaderKeyError.rst
--rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.0/docs/_autosummary/pyuff.readers.lazy_arrays.LazyArray.rst
--rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.0/docs/_autosummary/pyuff.readers.lazy_arrays.LazyScalar.rst
--rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.0/docs/_autosummary/pyuff.readers.lazy_arrays.rst
--rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.0/docs/_autosummary/pyuff.readers.rst
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.0/docs/_autosummary/pyuff.readers.util.read_enum.rst
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.0/docs/_autosummary/pyuff.readers.util.read_list_of_strings.rst
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.0/docs/_autosummary/pyuff.readers.util.read_potentially_list.rst
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.0/docs/_autosummary/pyuff.readers.util.read_probe.rst
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.0/docs/_autosummary/pyuff.readers.util.read_scan.rst
--rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.0/docs/_autosummary/pyuff.readers.util.rst
--rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.0/docs/_templates/class-template.rst
--rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.0/docs/_templates/module-template.rst
--rw-r--r--   0        0        0     2085 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.0/examples/writing_to_file.ipynb
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.0/pyuff_ustb/__init__.py
--rw-r--r--   0        0        0     1458 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.0/pyuff_ustb/common.py
--rw-r--r--   0        0        0     1440 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.0/pyuff_ustb/objects/__init__.py
--rw-r--r--   0        0        0     4492 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.0/pyuff_ustb/objects/apodization.py
--rw-r--r--   0        0        0     2694 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.0/pyuff_ustb/objects/beamformed_data.py
--rw-r--r--   0        0        0     4140 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.0/pyuff_ustb/objects/channel_data.py
--rw-r--r--   0        0        0     2127 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.0/pyuff_ustb/objects/phantom.py
--rw-r--r--   0        0        0     1290 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.0/pyuff_ustb/objects/point.py
--rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.0/pyuff_ustb/objects/pulse.py
--rw-r--r--   0        0        0    16761 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.0/pyuff_ustb/objects/uff.py
--rw-r--r--   0        0        0     2688 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.0/pyuff_ustb/objects/wave.py
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.0/pyuff_ustb/objects/wavefront.py
--rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.0/pyuff_ustb/objects/window.py
--rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.0/pyuff_ustb/objects/probes/__init__.py
--rw-r--r--   0        0        0     1295 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.0/pyuff_ustb/objects/probes/curvilinear_array.py
--rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.0/pyuff_ustb/objects/probes/curvilinear_matrix_array.py
--rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.0/pyuff_ustb/objects/probes/linear_array.py
--rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.0/pyuff_ustb/objects/probes/matrix_array.py
--rw-r--r--   0        0        0     2573 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.0/pyuff_ustb/objects/probes/probe.py
--rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.0/pyuff_ustb/objects/scans/__init__.py
--rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.0/pyuff_ustb/objects/scans/linear_3D_scan.py
--rw-r--r--   0        0        0     2010 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.0/pyuff_ustb/objects/scans/linear_scan.py
--rw-r--r--   0        0        0     1712 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.0/pyuff_ustb/objects/scans/linear_scan_rotated.py
--rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.0/pyuff_ustb/objects/scans/scan.py
--rw-r--r--   0        0        0     3649 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.0/pyuff_ustb/objects/scans/sector_scan.py
--rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.0/pyuff_ustb/readers/__init__.py
--rw-r--r--   0        0        0     4010 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.0/pyuff_ustb/readers/base.py
--rw-r--r--   0        0        0     2214 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.0/pyuff_ustb/readers/util.py
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.0/pyuff_ustb/readers/lazy_arrays/__init__.py
--rw-r--r--   0        0        0     4102 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.0/pyuff_ustb/readers/lazy_arrays/base.py
--rw-r--r--   0        0        0     1990 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.0/pyuff_ustb/readers/lazy_arrays/lazy_operations.py
--rw-r--r--   0        0        0     8253 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.0/tests/test_read_write.py
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.0/tests/pyuff_ustb/readers/lazy_arrays/test_lazy_operations.py
--rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.0/.gitignore
--rw-r--r--   0        0        0     4261 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.0/README.md
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.0/pyproject.toml
--rw-r--r--   0        0        0     4817 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.1/.readthedocs.yaml
+-rw-r--r--   0        0        0    12112 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.1/my_sector_scan.uff
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.1/requirements.txt
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.1/.vscode/settings.json
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.1/docs/Makefile
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.1/docs/api-reference.rst
+-rw-r--r--   0        0        0     1361 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.1/docs/conf.py
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.1/docs/index.rst
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.1/docs/make.bat
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.1/docs/requirements.txt
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.1/docs/_autosummary/pyuff.common.get_class_from_name.rst
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.1/docs/_autosummary/pyuff.common.get_name_from_class.rst
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.1/docs/_autosummary/pyuff.common.rst
+-rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.1/docs/_autosummary/pyuff.objects.Apodization.rst
+-rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.1/docs/_autosummary/pyuff.objects.BeamformedData.rst
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.1/docs/_autosummary/pyuff.objects.ChannelData.rst
+-rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.1/docs/_autosummary/pyuff.objects.CurvilinearArray.rst
+-rw-r--r--   0        0        0     1434 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.1/docs/_autosummary/pyuff.objects.CurvilinearMatrixArray.rst
+-rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.1/docs/_autosummary/pyuff.objects.LinearArray.rst
+-rw-r--r--   0        0        0      825 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.1/docs/_autosummary/pyuff.objects.LinearScan.rst
+-rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.1/docs/_autosummary/pyuff.objects.MatrixArray.rst
+-rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.1/docs/_autosummary/pyuff.objects.Phantom.rst
+-rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.1/docs/_autosummary/pyuff.objects.Point.rst
+-rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.1/docs/_autosummary/pyuff.objects.Probe.rst
+-rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.1/docs/_autosummary/pyuff.objects.Pulse.rst
+-rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.1/docs/_autosummary/pyuff.objects.Scan.rst
+-rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.1/docs/_autosummary/pyuff.objects.SectorScan.rst
+-rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.1/docs/_autosummary/pyuff.objects.Uff.rst
+-rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.1/docs/_autosummary/pyuff.objects.Wave.rst
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.1/docs/_autosummary/pyuff.objects.Wavefront.rst
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.1/docs/_autosummary/pyuff.objects.Window.rst
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.1/docs/_autosummary/pyuff.objects.eager_load.rst
+-rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.1/docs/_autosummary/pyuff.objects.rst
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.1/docs/_autosummary/pyuff.objects.write_object.rst
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.1/docs/_autosummary/pyuff.readers.H5Reader.rst
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.1/docs/_autosummary/pyuff.readers.LazyArray.rst
+-rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.1/docs/_autosummary/pyuff.readers.LazyScalar.rst
+-rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.1/docs/_autosummary/pyuff.readers.NoneReader.rst
+-rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.1/docs/_autosummary/pyuff.readers.Reader.rst
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.1/docs/_autosummary/pyuff.readers.ReaderAttrsKeyError.rst
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.1/docs/_autosummary/pyuff.readers.ReaderKeyError.rst
+-rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.1/docs/_autosummary/pyuff.readers.lazy_arrays.LazyArray.rst
+-rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.1/docs/_autosummary/pyuff.readers.lazy_arrays.LazyScalar.rst
+-rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.1/docs/_autosummary/pyuff.readers.lazy_arrays.rst
+-rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.1/docs/_autosummary/pyuff.readers.rst
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.1/docs/_autosummary/pyuff.readers.util.read_enum.rst
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.1/docs/_autosummary/pyuff.readers.util.read_list_of_strings.rst
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.1/docs/_autosummary/pyuff.readers.util.read_potentially_list.rst
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.1/docs/_autosummary/pyuff.readers.util.read_probe.rst
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.1/docs/_autosummary/pyuff.readers.util.read_scan.rst
+-rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.1/docs/_autosummary/pyuff.readers.util.rst
+-rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.1/docs/_templates/class-template.rst
+-rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.1/docs/_templates/module-template.rst
+-rw-r--r--   0        0        0     2085 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.1/examples/writing_to_file.ipynb
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.1/pyuff_ustb/__init__.py
+-rw-r--r--   0        0        0     1458 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.1/pyuff_ustb/common.py
+-rw-r--r--   0        0        0     1440 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.1/pyuff_ustb/objects/__init__.py
+-rw-r--r--   0        0        0     4492 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.1/pyuff_ustb/objects/apodization.py
+-rw-r--r--   0        0        0     2694 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.1/pyuff_ustb/objects/beamformed_data.py
+-rw-r--r--   0        0        0     4140 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.1/pyuff_ustb/objects/channel_data.py
+-rw-r--r--   0        0        0     2127 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.1/pyuff_ustb/objects/phantom.py
+-rw-r--r--   0        0        0     1290 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.1/pyuff_ustb/objects/point.py
+-rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.1/pyuff_ustb/objects/pulse.py
+-rw-r--r--   0        0        0    16761 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.1/pyuff_ustb/objects/uff.py
+-rw-r--r--   0        0        0     2688 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.1/pyuff_ustb/objects/wave.py
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.1/pyuff_ustb/objects/wavefront.py
+-rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.1/pyuff_ustb/objects/window.py
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.1/pyuff_ustb/objects/probes/__init__.py
+-rw-r--r--   0        0        0     1295 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.1/pyuff_ustb/objects/probes/curvilinear_array.py
+-rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.1/pyuff_ustb/objects/probes/curvilinear_matrix_array.py
+-rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.1/pyuff_ustb/objects/probes/linear_array.py
+-rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.1/pyuff_ustb/objects/probes/matrix_array.py
+-rw-r--r--   0        0        0     2573 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.1/pyuff_ustb/objects/probes/probe.py
+-rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.1/pyuff_ustb/objects/scans/__init__.py
+-rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.1/pyuff_ustb/objects/scans/linear_3D_scan.py
+-rw-r--r--   0        0        0     2010 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.1/pyuff_ustb/objects/scans/linear_scan.py
+-rw-r--r--   0        0        0     1712 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.1/pyuff_ustb/objects/scans/linear_scan_rotated.py
+-rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.1/pyuff_ustb/objects/scans/scan.py
+-rw-r--r--   0        0        0     3649 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.1/pyuff_ustb/objects/scans/sector_scan.py
+-rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.1/pyuff_ustb/readers/__init__.py
+-rw-r--r--   0        0        0     4010 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.1/pyuff_ustb/readers/base.py
+-rw-r--r--   0        0        0     2214 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.1/pyuff_ustb/readers/util.py
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.1/pyuff_ustb/readers/lazy_arrays/__init__.py
+-rw-r--r--   0        0        0     4102 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.1/pyuff_ustb/readers/lazy_arrays/base.py
+-rw-r--r--   0        0        0     1990 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.1/pyuff_ustb/readers/lazy_arrays/lazy_operations.py
+-rw-r--r--   0        0        0     8253 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.1/tests/test_read_write.py
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.1/tests/pyuff_ustb/readers/lazy_arrays/test_lazy_operations.py
+-rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.1/.gitignore
+-rw-r--r--   0        0        0     4261 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.1/README.md
+-rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0     4858 2020-02-02 00:00:00.000000 pyuff_ustb-2.0.1/PKG-INFO
```

### Comparing `pyuff_ustb-2.0.0/.readthedocs.yaml` & `pyuff_ustb-2.0.1/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `pyuff_ustb-2.0.0/my_sector_scan.uff` & `pyuff_ustb-2.0.1/my_sector_scan.uff`

 * *Files identical despite different names*

### Comparing `pyuff_ustb-2.0.0/docs/Makefile` & `pyuff_ustb-2.0.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pyuff_ustb-2.0.0/docs/conf.py` & `pyuff_ustb-2.0.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pyuff_ustb-2.0.0/docs/make.bat` & `pyuff_ustb-2.0.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pyuff_ustb-2.0.0/docs/_autosummary/pyuff.objects.Apodization.rst` & `pyuff_ustb-2.0.1/docs/_autosummary/pyuff.objects.Apodization.rst`

 * *Files identical despite different names*

### Comparing `pyuff_ustb-2.0.0/docs/_autosummary/pyuff.objects.BeamformedData.rst` & `pyuff_ustb-2.0.1/docs/_autosummary/pyuff.objects.BeamformedData.rst`

 * *Files identical despite different names*

### Comparing `pyuff_ustb-2.0.0/docs/_autosummary/pyuff.objects.ChannelData.rst` & `pyuff_ustb-2.0.1/docs/_autosummary/pyuff.objects.ChannelData.rst`

 * *Files identical despite different names*

### Comparing `pyuff_ustb-2.0.0/docs/_autosummary/pyuff.objects.CurvilinearArray.rst` & `pyuff_ustb-2.0.1/docs/_autosummary/pyuff.objects.CurvilinearArray.rst`

 * *Files identical despite different names*

### Comparing `pyuff_ustb-2.0.0/docs/_autosummary/pyuff.objects.CurvilinearMatrixArray.rst` & `pyuff_ustb-2.0.1/docs/_autosummary/pyuff.objects.CurvilinearMatrixArray.rst`

 * *Files identical despite different names*

### Comparing `pyuff_ustb-2.0.0/docs/_autosummary/pyuff.objects.LinearArray.rst` & `pyuff_ustb-2.0.1/docs/_autosummary/pyuff.objects.LinearArray.rst`

 * *Files identical despite different names*

### Comparing `pyuff_ustb-2.0.0/docs/_autosummary/pyuff.objects.LinearScan.rst` & `pyuff_ustb-2.0.1/docs/_autosummary/pyuff.objects.LinearScan.rst`

 * *Files identical despite different names*

### Comparing `pyuff_ustb-2.0.0/docs/_autosummary/pyuff.objects.MatrixArray.rst` & `pyuff_ustb-2.0.1/docs/_autosummary/pyuff.objects.MatrixArray.rst`

 * *Files identical despite different names*

### Comparing `pyuff_ustb-2.0.0/docs/_autosummary/pyuff.objects.Phantom.rst` & `pyuff_ustb-2.0.1/docs/_autosummary/pyuff.objects.Phantom.rst`

 * *Files identical despite different names*

### Comparing `pyuff_ustb-2.0.0/docs/_autosummary/pyuff.objects.Point.rst` & `pyuff_ustb-2.0.1/docs/_autosummary/pyuff.objects.Point.rst`

 * *Files identical despite different names*

### Comparing `pyuff_ustb-2.0.0/docs/_autosummary/pyuff.objects.Probe.rst` & `pyuff_ustb-2.0.1/docs/_autosummary/pyuff.objects.Probe.rst`

 * *Files identical despite different names*

### Comparing `pyuff_ustb-2.0.0/docs/_autosummary/pyuff.objects.Pulse.rst` & `pyuff_ustb-2.0.1/docs/_autosummary/pyuff.objects.Pulse.rst`

 * *Files identical despite different names*

### Comparing `pyuff_ustb-2.0.0/docs/_autosummary/pyuff.objects.Scan.rst` & `pyuff_ustb-2.0.1/docs/_autosummary/pyuff.objects.Scan.rst`

 * *Files identical despite different names*

### Comparing `pyuff_ustb-2.0.0/docs/_autosummary/pyuff.objects.SectorScan.rst` & `pyuff_ustb-2.0.1/docs/_autosummary/pyuff.objects.SectorScan.rst`

 * *Files identical despite different names*

### Comparing `pyuff_ustb-2.0.0/docs/_autosummary/pyuff.objects.Wave.rst` & `pyuff_ustb-2.0.1/docs/_autosummary/pyuff.objects.Wave.rst`

 * *Files identical despite different names*

### Comparing `pyuff_ustb-2.0.0/docs/_autosummary/pyuff.objects.Window.rst` & `pyuff_ustb-2.0.1/docs/_autosummary/pyuff.objects.Window.rst`

 * *Files identical despite different names*

### Comparing `pyuff_ustb-2.0.0/docs/_autosummary/pyuff.objects.rst` & `pyuff_ustb-2.0.1/docs/_autosummary/pyuff.objects.rst`

 * *Files identical despite different names*

### Comparing `pyuff_ustb-2.0.0/docs/_autosummary/pyuff.readers.rst` & `pyuff_ustb-2.0.1/docs/_autosummary/pyuff.readers.rst`

 * *Files identical despite different names*

### Comparing `pyuff_ustb-2.0.0/docs/_templates/class-template.rst` & `pyuff_ustb-2.0.1/docs/_templates/class-template.rst`

 * *Files identical despite different names*

### Comparing `pyuff_ustb-2.0.0/docs/_templates/module-template.rst` & `pyuff_ustb-2.0.1/docs/_templates/module-template.rst`

 * *Files identical despite different names*

### Comparing `pyuff_ustb-2.0.0/examples/writing_to_file.ipynb` & `pyuff_ustb-2.0.1/examples/writing_to_file.ipynb`

 * *Files identical despite different names*

### Comparing `pyuff_ustb-2.0.0/pyuff_ustb/common.py` & `pyuff_ustb-2.0.1/pyuff_ustb/common.py`

 * *Files identical despite different names*

### Comparing `pyuff_ustb-2.0.0/pyuff_ustb/objects/__init__.py` & `pyuff_ustb-2.0.1/pyuff_ustb/objects/__init__.py`

 * *Files identical despite different names*

### Comparing `pyuff_ustb-2.0.0/pyuff_ustb/objects/apodization.py` & `pyuff_ustb-2.0.1/pyuff_ustb/objects/apodization.py`

 * *Files identical despite different names*

### Comparing `pyuff_ustb-2.0.0/pyuff_ustb/objects/beamformed_data.py` & `pyuff_ustb-2.0.1/pyuff_ustb/objects/beamformed_data.py`

 * *Files identical despite different names*

### Comparing `pyuff_ustb-2.0.0/pyuff_ustb/objects/channel_data.py` & `pyuff_ustb-2.0.1/pyuff_ustb/objects/channel_data.py`

 * *Files identical despite different names*

### Comparing `pyuff_ustb-2.0.0/pyuff_ustb/objects/phantom.py` & `pyuff_ustb-2.0.1/pyuff_ustb/objects/phantom.py`

 * *Files identical despite different names*

### Comparing `pyuff_ustb-2.0.0/pyuff_ustb/objects/point.py` & `pyuff_ustb-2.0.1/pyuff_ustb/objects/point.py`

 * *Files identical despite different names*

### Comparing `pyuff_ustb-2.0.0/pyuff_ustb/objects/pulse.py` & `pyuff_ustb-2.0.1/pyuff_ustb/objects/pulse.py`

 * *Files identical despite different names*

### Comparing `pyuff_ustb-2.0.0/pyuff_ustb/objects/uff.py` & `pyuff_ustb-2.0.1/pyuff_ustb/objects/uff.py`

 * *Files identical despite different names*

### Comparing `pyuff_ustb-2.0.0/pyuff_ustb/objects/wave.py` & `pyuff_ustb-2.0.1/pyuff_ustb/objects/wave.py`

 * *Files identical despite different names*

### Comparing `pyuff_ustb-2.0.0/pyuff_ustb/objects/probes/curvilinear_array.py` & `pyuff_ustb-2.0.1/pyuff_ustb/objects/probes/curvilinear_array.py`

 * *Files identical despite different names*

### Comparing `pyuff_ustb-2.0.0/pyuff_ustb/objects/probes/curvilinear_matrix_array.py` & `pyuff_ustb-2.0.1/pyuff_ustb/objects/probes/curvilinear_matrix_array.py`

 * *Files identical despite different names*

### Comparing `pyuff_ustb-2.0.0/pyuff_ustb/objects/probes/linear_array.py` & `pyuff_ustb-2.0.1/pyuff_ustb/objects/probes/linear_array.py`

 * *Files identical despite different names*

### Comparing `pyuff_ustb-2.0.0/pyuff_ustb/objects/probes/matrix_array.py` & `pyuff_ustb-2.0.1/pyuff_ustb/objects/probes/matrix_array.py`

 * *Files identical despite different names*

### Comparing `pyuff_ustb-2.0.0/pyuff_ustb/objects/probes/probe.py` & `pyuff_ustb-2.0.1/pyuff_ustb/objects/probes/probe.py`

 * *Files identical despite different names*

### Comparing `pyuff_ustb-2.0.0/pyuff_ustb/objects/scans/linear_3D_scan.py` & `pyuff_ustb-2.0.1/pyuff_ustb/objects/scans/linear_3D_scan.py`

 * *Files identical despite different names*

### Comparing `pyuff_ustb-2.0.0/pyuff_ustb/objects/scans/linear_scan.py` & `pyuff_ustb-2.0.1/pyuff_ustb/objects/scans/linear_scan.py`

 * *Files identical despite different names*

### Comparing `pyuff_ustb-2.0.0/pyuff_ustb/objects/scans/linear_scan_rotated.py` & `pyuff_ustb-2.0.1/pyuff_ustb/objects/scans/linear_scan_rotated.py`

 * *Files identical despite different names*

### Comparing `pyuff_ustb-2.0.0/pyuff_ustb/objects/scans/scan.py` & `pyuff_ustb-2.0.1/pyuff_ustb/objects/scans/scan.py`

 * *Files identical despite different names*

### Comparing `pyuff_ustb-2.0.0/pyuff_ustb/objects/scans/sector_scan.py` & `pyuff_ustb-2.0.1/pyuff_ustb/objects/scans/sector_scan.py`

 * *Files identical despite different names*

### Comparing `pyuff_ustb-2.0.0/pyuff_ustb/readers/base.py` & `pyuff_ustb-2.0.1/pyuff_ustb/readers/base.py`

 * *Files identical despite different names*

### Comparing `pyuff_ustb-2.0.0/pyuff_ustb/readers/util.py` & `pyuff_ustb-2.0.1/pyuff_ustb/readers/util.py`

 * *Files identical despite different names*

### Comparing `pyuff_ustb-2.0.0/pyuff_ustb/readers/lazy_arrays/base.py` & `pyuff_ustb-2.0.1/pyuff_ustb/readers/lazy_arrays/base.py`

 * *Files identical despite different names*

### Comparing `pyuff_ustb-2.0.0/pyuff_ustb/readers/lazy_arrays/lazy_operations.py` & `pyuff_ustb-2.0.1/pyuff_ustb/readers/lazy_arrays/lazy_operations.py`

 * *Files identical despite different names*

### Comparing `pyuff_ustb-2.0.0/tests/test_read_write.py` & `pyuff_ustb-2.0.1/tests/test_read_write.py`

 * *Files identical despite different names*

### Comparing `pyuff_ustb-2.0.0/tests/pyuff_ustb/readers/lazy_arrays/test_lazy_operations.py` & `pyuff_ustb-2.0.1/tests/pyuff_ustb/readers/lazy_arrays/test_lazy_operations.py`

 * *Files identical despite different names*

### Comparing `pyuff_ustb-2.0.0/.gitignore` & `pyuff_ustb-2.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `pyuff_ustb-2.0.0/README.md` & `pyuff_ustb-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `pyuff_ustb-2.0.0/PKG-INFO` & `pyuff_ustb-2.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 Metadata-Version: 2.1
 Name: pyuff_ustb
-Version: 2.0.0
+Version: 2.0.1
 Summary: An implementation of USTB's ultrasound file format (UFF) in Python.
-Project-URL: Homepage, https://pyuff-ustb.readthedocs.io/en/latest/
 Project-URL: Bug Tracker, https://github.com/magnusdk/pyuff_ustb/issues
+Project-URL: Homepage, https://pyuff-ustb.readthedocs.io/en/latest/
 Author-email: Magnus Dalen Kvalevåg <magnus.kvalevag@ntnu.no>
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
+Requires-Dist: h5py
+Requires-Dist: numpy
 Description-Content-Type: text/markdown
 
 # PyUFF ([USTB](https://www.ustb.no/))
 An implementation of [USTB's](https://www.ustb.no/) [ultrasound file format (UFF)](https://www.ustb.no/examples/uff/) in Python.
 
 _Note that this project only implements USTB's version of UFF, which is considered version `0.0.1`. Multiple versions of UFF exists, for example check out [uff-reader](https://github.com/waltsims/uff-reader). However, if you only planning to use USTB's version of UFF then you have come to the right place :)_
```

