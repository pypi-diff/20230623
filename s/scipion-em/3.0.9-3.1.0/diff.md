# Comparing `tmp/scipion-em-3.0.9.tar.gz` & `tmp/scipion-em-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scipion-em-3.0.9.tar", last modified: Tue Mar 30 10:37:19 2021, max compression
+gzip compressed data, was "scipion-em-3.1.0.tar", last modified: Fri Jun 23 15:12:46 2023, max compression
```

## Comparing `scipion-em-3.0.9.tar` & `scipion-em-3.1.0.tar`

### file list

```diff
@@ -1,148 +1,172 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-30 10:37:19.989638 scipion-em-3.0.9/
--rw-r--r--   0 runner    (1001) docker     (121)       54 2021-03-30 10:31:41.000000 scipion-em-3.0.9/CHANGES.txt
--rw-r--r--   0 runner    (1001) docker     (121)    35147 2021-03-30 10:31:41.000000 scipion-em-3.0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       43 2021-03-30 10:31:41.000000 scipion-em-3.0.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     2257 2021-03-30 10:37:19.989638 scipion-em-3.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1000 2021-03-30 10:31:41.000000 scipion-em-3.0.9/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-30 10:37:19.977636 scipion-em-3.0.9/pwem/
--rw-r--r--   0 runner    (1001) docker     (121)     4916 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2113 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/bibtex.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-30 10:37:19.977636 scipion-em-3.0.9/pwem/cmd/
--rwxr-xr-x   0 runner    (1001) docker     (121)      382 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/cmd/chimera_client.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     4026 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/cmd/convert.py
--rw-r--r--   0 runner    (1001) docker     (121)     1517 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/cmd/program.py
--rw-r--r--   0 runner    (1001) docker     (121)     6375 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-30 10:37:19.977636 scipion-em-3.0.9/pwem/convert/
--rw-r--r--   0 runner    (1001) docker     (121)     1517 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/convert/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    37562 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/convert/atom_struct.py
--rw-r--r--   0 runner    (1001) docker     (121)    14159 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/convert/headers.py
--rw-r--r--   0 runner    (1001) docker     (121)     8688 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/convert/sequence.py
--rw-r--r--   0 runner    (1001) docker     (121)    23840 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/convert/symmetry.py
--rw-r--r--   0 runner    (1001) docker     (121)    65754 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/convert/transformations.py
--rw-r--r--   0 runner    (1001) docker     (121)     4547 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/convert/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-30 10:37:19.977636 scipion-em-3.0.9/pwem/emlib/
--rw-r--r--   0 runner    (1001) docker     (121)     1194 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/emlib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    29660 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/emlib/_libNone.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-30 10:37:19.977636 scipion-em-3.0.9/pwem/emlib/image/
--rw-r--r--   0 runner    (1001) docker     (121)     1198 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/emlib/image/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    21780 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/emlib/image/image_handler.py
--rw-r--r--   0 runner    (1001) docker     (121)     1199 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/emlib/lib.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-30 10:37:19.977636 scipion-em-3.0.9/pwem/emlib/metadata/
--rw-r--r--   0 runner    (1001) docker     (121)     1152 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/emlib/metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    11287 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/emlib/metadata/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-30 10:37:19.977636 scipion-em-3.0.9/pwem/objects/
--rw-r--r--   0 runner    (1001) docker     (121)     1205 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/objects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    71469 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/objects/data.py
--rw-r--r--   0 runner    (1001) docker     (121)     5562 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/objects/data_tiltpairs.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-30 10:37:19.981637 scipion-em-3.0.9/pwem/protocols/
--rw-r--r--   0 runner    (1001) docker     (121)     2454 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/protocols/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4142 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/protocols/parallel.py
--rw-r--r--   0 runner    (1001) docker     (121)    13672 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/protocols/protocol.py
--rw-r--r--   0 runner    (1001) docker     (121)     3902 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/protocols/protocol_2d.py
--rw-r--r--   0 runner    (1001) docker     (121)     3321 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/protocols/protocol_3d.py
--rw-r--r--   0 runner    (1001) docker     (121)    32873 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/protocols/protocol_align_movies.py
--rw-r--r--   0 runner    (1001) docker     (121)     7445 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/protocols/protocol_alignment_assign.py
--rw-r--r--   0 runner    (1001) docker     (121)     4553 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/protocols/protocol_alignment_invertHand.py
--rw-r--r--   0 runner    (1001) docker     (121)    24488 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/protocols/protocol_batch.py
--rw-r--r--   0 runner    (1001) docker     (121)     4585 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/protocols/protocol_classes_consensus.py
--rw-r--r--   0 runner    (1001) docker     (121)    15973 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/protocols/protocol_create_stream_data.py
--rw-r--r--   0 runner    (1001) docker     (121)     8052 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/protocols/protocol_ctf_assign.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-30 10:37:19.981637 scipion-em-3.0.9/pwem/protocols/protocol_export/
--rw-r--r--   0 runner    (1001) docker     (121)     1194 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/protocols/protocol_export/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    12107 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/protocols/protocol_export/protocol_export_DB.py
--rw-r--r--   0 runner    (1001) docker     (121)    16690 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/protocols/protocol_extract_coordinates.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-30 10:37:19.981637 scipion-em-3.0.9/pwem/protocols/protocol_import/
--rw-r--r--   0 runner    (1001) docker     (121)     1692 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/protocols/protocol_import/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    12003 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/protocols/protocol_import/base.py
--rw-r--r--   0 runner    (1001) docker     (121)    25865 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/protocols/protocol_import/coordinates.py
--rw-r--r--   0 runner    (1001) docker     (121)    10122 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/protocols/protocol_import/ctfs.py
--rw-r--r--   0 runner    (1001) docker     (121)     6057 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/protocols/protocol_import/dataimport.py
--rw-r--r--   0 runner    (1001) docker     (121)    23881 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/protocols/protocol_import/images.py
--rw-r--r--   0 runner    (1001) docker     (121)     3649 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/protocols/protocol_import/masks.py
--rw-r--r--   0 runner    (1001) docker     (121)    30302 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/protocols/protocol_import/micrographs.py
--rw-r--r--   0 runner    (1001) docker     (121)    13060 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/protocols/protocol_import/particles.py
--rw-r--r--   0 runner    (1001) docker     (121)    25590 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/protocols/protocol_import/sequence.py
--rw-r--r--   0 runner    (1001) docker     (121)    22524 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/protocols/protocol_import/volumes.py
--rw-r--r--   0 runner    (1001) docker     (121)     3201 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/protocols/protocol_metadata_editor.py
--rw-r--r--   0 runner    (1001) docker     (121)    31529 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/protocols/protocol_micrographs.py
--rw-r--r--   0 runner    (1001) docker     (121)    21203 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/protocols/protocol_movies.py
--rw-r--r--   0 runner    (1001) docker     (121)     7141 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/protocols/protocol_origin_sampling_volume.py
--rw-r--r--   0 runner    (1001) docker     (121)    25437 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/protocols/protocol_particles.py
--rw-r--r--   0 runner    (1001) docker     (121)    25045 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/protocols/protocol_particles_picking.py
--rw-r--r--   0 runner    (1001) docker     (121)     5259 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/protocols/protocol_pdf_report.py
--rw-r--r--   0 runner    (1001) docker     (121)    33673 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/protocols/protocol_sets.py
--rw-r--r--   0 runner    (1001) docker     (121)     7736 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/protocols/protocol_tests.py
--rw-r--r--   0 runner    (1001) docker     (121)    10282 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/protocols/protocol_tiltpairs.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-30 10:37:19.981637 scipion-em-3.0.9/pwem/templates/
--rw-r--r--   0 runner    (1001) docker     (121)     6537 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/templates/demo.json.template
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-30 10:37:19.981637 scipion-em-3.0.9/pwem/tests/
--rw-r--r--   0 runner    (1001) docker     (121)     1239 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-30 10:37:19.985637 scipion-em-3.0.9/pwem/tests/data/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/tests/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    38693 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/tests/data/test_convert_atom_struct.py
--rw-r--r--   0 runner    (1001) docker     (121)    35874 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/tests/data/test_data.py
--rw-r--r--   0 runner    (1001) docker     (121)     3204 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/tests/data/test_metadata.py
--rw-r--r--   0 runner    (1001) docker     (121)    21174 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/tests/data/test_symmetry.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-30 10:37:19.985637 scipion-em-3.0.9/pwem/tests/protocols/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/tests/protocols/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8069 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/tests/protocols/test_extract_particles.py
--rw-r--r--   0 runner    (1001) docker     (121)     6760 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/tests/protocols/test_notifier.py
--rw-r--r--   0 runner    (1001) docker     (121)     6500 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/tests/protocols/test_protocol_alignment_assign.py
--rw-r--r--   0 runner    (1001) docker     (121)    13157 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/tests/protocols/test_protocol_export2DB.py
--rw-r--r--   0 runner    (1001) docker     (121)     2248 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/tests/protocols/test_protocol_extract_coorinates.py
--rw-r--r--   0 runner    (1001) docker     (121)     6065 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/tests/protocols/test_protocol_invert_Hand.py
--rw-r--r--   0 runner    (1001) docker     (121)    11658 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/tests/protocols/test_protocol_volume_homogenizer.py
--rw-r--r--   0 runner    (1001) docker     (121)     8404 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/tests/protocols/test_protocols_assign_orig.py
--rw-r--r--   0 runner    (1001) docker     (121)     9190 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/tests/protocols/test_protocols_import_coords.py
--rw-r--r--   0 runner    (1001) docker     (121)     6635 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/tests/protocols/test_protocols_import_ctfs.py
--rw-r--r--   0 runner    (1001) docker     (121)     2295 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/tests/protocols/test_protocols_import_masks.py
--rw-r--r--   0 runner    (1001) docker     (121)     9168 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/tests/protocols/test_protocols_import_micrographs.py
--rw-r--r--   0 runner    (1001) docker     (121)     6488 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/tests/protocols/test_protocols_import_movies.py
--rw-r--r--   0 runner    (1001) docker     (121)     9670 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/tests/protocols/test_protocols_import_particles.py
--rw-r--r--   0 runner    (1001) docker     (121)    27671 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/tests/protocols/test_protocols_import_sequence.py
--rw-r--r--   0 runner    (1001) docker     (121)    17661 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/tests/protocols/test_protocols_import_volumes.py
--rw-r--r--   0 runner    (1001) docker     (121)    25634 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/tests/protocols/test_protocols_sets.py
--rw-r--r--   0 runner    (1001) docker     (121)     2241 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/tests/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-30 10:37:19.985637 scipion-em-3.0.9/pwem/tests/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)       41 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/tests/workflows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    17332 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/tests/workflows/test_parallel_gpu_queue.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1299 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/tests/workflows/test_workflow.py
--rw-r--r--   0 runner    (1001) docker     (121)    14023 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/tests/workflows/test_workflow_initialvolume.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    12648 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/tests/workflows/test_workflow_mixed.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    13743 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/tests/workflows/test_workflow_mixed_large.py
--rwxr-xr-x   0 runner    (1001) docker     (121)   122820 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/tests/workflows/test_workflow_modeling.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    11926 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/tests/workflows/test_workflow_xmipp.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     4512 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/tests/workflows/test_workflow_xmipp_assignment_tiltpairs.py
--rw-r--r--   0 runner    (1001) docker     (121)    10427 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/tests/workflows/test_workflow_xmipp_ctf_consensus.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     5438 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/tests/workflows/test_workflow_xmipp_rct.py
--rw-r--r--   0 runner    (1001) docker     (121)     3345 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-30 10:37:19.989638 scipion-em-3.0.9/pwem/viewers/
--rw-r--r--   0 runner    (1001) docker     (121)     2529 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/viewers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6991 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/viewers/filehandlers.py
--rw-r--r--   0 runner    (1001) docker     (121)    10409 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/viewers/plotter.py
--rw-r--r--   0 runner    (1001) docker     (121)    12570 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/viewers/showj.py
--rw-r--r--   0 runner    (1001) docker     (121)     5254 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/viewers/viewer_base.py
--rw-r--r--   0 runner    (1001) docker     (121)    19582 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/viewers/viewer_chimera.py
--rw-r--r--   0 runner    (1001) docker     (121)     4770 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/viewers/viewer_fsc.py
--rw-r--r--   0 runner    (1001) docker     (121)     4033 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/viewers/viewer_localres.py
--rw-r--r--   0 runner    (1001) docker     (121)     1538 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/viewers/viewer_pdf.py
--rw-r--r--   0 runner    (1001) docker     (121)     3026 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/viewers/viewer_sequence.py
--rw-r--r--   0 runner    (1001) docker     (121)     2893 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/viewers/viewer_vmd.py
--rw-r--r--   0 runner    (1001) docker     (121)     7854 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/viewers/viewer_volumes.py
--rw-r--r--   0 runner    (1001) docker     (121)    10148 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/viewers/viewers_data.py
--rw-r--r--   0 runner    (1001) docker     (121)     2042 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/viewers/viewers_protocols.py
--rw-r--r--   0 runner    (1001) docker     (121)    16407 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/viewers/views.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-30 10:37:19.989638 scipion-em-3.0.9/pwem/wizards/
--rw-r--r--   0 runner    (1001) docker     (121)     1200 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/wizards/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    49421 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/wizards/wizard.py
--rw-r--r--   0 runner    (1001) docker     (121)     9048 2021-03-30 10:31:41.000000 scipion-em-3.0.9/pwem/wizards/wizards.py
--rw-r--r--   0 runner    (1001) docker     (121)       35 2021-03-30 10:31:41.000000 scipion-em-3.0.9/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-30 10:37:19.989638 scipion-em-3.0.9/scipion_em.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2257 2021-03-30 10:37:19.000000 scipion-em-3.0.9/scipion_em.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4460 2021-03-30 10:37:19.000000 scipion-em-3.0.9/scipion_em.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-03-30 10:37:19.000000 scipion-em-3.0.9/scipion_em.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      161 2021-03-30 10:37:19.000000 scipion-em-3.0.9/scipion_em.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       35 2021-03-30 10:37:19.000000 scipion-em-3.0.9/scipion_em.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        5 2021-03-30 10:37:19.000000 scipion-em-3.0.9/scipion_em.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-03-30 10:37:19.989638 scipion-em-3.0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     3168 2021-03-30 10:31:41.000000 scipion-em-3.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:12:46.467060 scipion-em-3.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     9228 2023-06-23 15:10:58.000000 scipion-em-3.1.0/CHANGES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-06-23 15:10:58.000000 scipion-em-3.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-23 15:10:58.000000 scipion-em-3.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-06-23 15:12:46.467060 scipion-em-3.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-06-23 15:10:58.000000 scipion-em-3.1.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:12:46.443061 scipion-em-3.1.0/pwem/
+-rw-r--r--   0 runner    (1001) docker     (123)     9402 2023-06-23 15:10:58.000000 scipion-em-3.1.0/pwem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-06-23 15:10:58.000000 scipion-em-3.1.0/pwem/bibtex.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:12:46.443061 scipion-em-3.1.0/pwem/cmd/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      382 2023-06-23 15:10:58.000000 scipion-em-3.1.0/pwem/cmd/chimera_client.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4026 2023-06-23 15:10:58.000000 scipion-em-3.1.0/pwem/cmd/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-06-23 15:10:58.000000 scipion-em-3.1.0/pwem/cmd/program.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7207 2023-06-23 15:10:58.000000 scipion-em-3.1.0/pwem/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:12:46.447061 scipion-em-3.1.0/pwem/convert/
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-06-23 15:10:58.000000 scipion-em-3.1.0/pwem/convert/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45637 2023-06-23 15:10:58.000000 scipion-em-3.1.0/pwem/convert/atom_struct.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15240 2023-06-23 15:10:58.000000 scipion-em-3.1.0/pwem/convert/headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10921 2023-06-23 15:10:58.000000 scipion-em-3.1.0/pwem/convert/sequence.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47961 2023-06-23 15:10:58.000000 scipion-em-3.1.0/pwem/convert/symmetry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65807 2023-06-23 15:10:58.000000 scipion-em-3.1.0/pwem/convert/transformations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4547 2023-06-23 15:10:58.000000 scipion-em-3.1.0/pwem/convert/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:12:46.447061 scipion-em-3.1.0/pwem/emlib/
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-06-23 15:10:58.000000 scipion-em-3.1.0/pwem/emlib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29799 2023-06-23 15:10:58.000000 scipion-em-3.1.0/pwem/emlib/_libNone.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:12:46.447061 scipion-em-3.1.0/pwem/emlib/image/
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-06-23 15:10:58.000000 scipion-em-3.1.0/pwem/emlib/image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22832 2023-06-23 15:10:58.000000 scipion-em-3.1.0/pwem/emlib/image/image_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-06-23 15:10:58.000000 scipion-em-3.1.0/pwem/emlib/lib.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:12:46.447061 scipion-em-3.1.0/pwem/emlib/metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-06-23 15:10:58.000000 scipion-em-3.1.0/pwem/emlib/metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11683 2023-06-23 15:10:58.000000 scipion-em-3.1.0/pwem/emlib/metadata/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:12:46.447061 scipion-em-3.1.0/pwem/objects/
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-06-23 15:10:58.000000 scipion-em-3.1.0/pwem/objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    85792 2023-06-23 15:10:58.000000 scipion-em-3.1.0/pwem/objects/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5562 2023-06-23 15:10:58.000000 scipion-em-3.1.0/pwem/objects/data_tiltpairs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:12:46.451061 scipion-em-3.1.0/pwem/protocols/
+-rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-06-23 15:10:58.000000 scipion-em-3.1.0/pwem/protocols/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4142 2023-06-23 15:10:58.000000 scipion-em-3.1.0/pwem/protocols/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13585 2023-06-23 15:10:58.000000 scipion-em-3.1.0/pwem/protocols/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3902 2023-06-23 15:10:58.000000 scipion-em-3.1.0/pwem/protocols/protocol_2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-06-23 15:10:58.000000 scipion-em-3.1.0/pwem/protocols/protocol_3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33322 2023-06-23 15:10:58.000000 scipion-em-3.1.0/pwem/protocols/protocol_align_movies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9395 2023-06-23 15:10:58.000000 scipion-em-3.1.0/pwem/protocols/protocol_alignment_assign.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4553 2023-06-23 15:10:58.000000 scipion-em-3.1.0/pwem/protocols/protocol_alignment_invertHand.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25609 2023-06-23 15:10:58.000000 scipion-em-3.1.0/pwem/protocols/protocol_batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9869 2023-06-23 15:10:58.000000 scipion-em-3.1.0/pwem/protocols/protocol_boxsize_checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15655 2023-06-23 15:10:58.000000 scipion-em-3.1.0/pwem/protocols/protocol_boxsize_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6476 2023-06-23 15:10:58.000000 scipion-em-3.1.0/pwem/protocols/protocol_classes_selector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18773 2023-06-23 15:10:58.000000 scipion-em-3.1.0/pwem/protocols/protocol_create_stream_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8437 2023-06-23 15:10:58.000000 scipion-em-3.1.0/pwem/protocols/protocol_ctf_assign.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:12:46.451061 scipion-em-3.1.0/pwem/protocols/protocol_export/
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-06-23 15:10:58.000000 scipion-em-3.1.0/pwem/protocols/protocol_export/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12110 2023-06-23 15:10:58.000000 scipion-em-3.1.0/pwem/protocols/protocol_export/protocol_export_DB.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16631 2023-06-23 15:10:58.000000 scipion-em-3.1.0/pwem/protocols/protocol_extract_coordinates.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:12:46.451061 scipion-em-3.1.0/pwem/protocols/protocol_import/
+-rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-06-23 15:10:58.000000 scipion-em-3.1.0/pwem/protocols/protocol_import/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12003 2023-06-23 15:10:58.000000 scipion-em-3.1.0/pwem/protocols/protocol_import/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26633 2023-06-23 15:10:58.000000 scipion-em-3.1.0/pwem/protocols/protocol_import/coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10122 2023-06-23 15:10:58.000000 scipion-em-3.1.0/pwem/protocols/protocol_import/ctfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7150 2023-06-23 15:10:58.000000 scipion-em-3.1.0/pwem/protocols/protocol_import/dataimport.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23705 2023-06-23 15:10:58.000000 scipion-em-3.1.0/pwem/protocols/protocol_import/images.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3901 2023-06-23 15:10:58.000000 scipion-em-3.1.0/pwem/protocols/protocol_import/masks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30655 2023-06-23 15:10:58.000000 scipion-em-3.1.0/pwem/protocols/protocol_import/micrographs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13977 2023-06-23 15:10:58.000000 scipion-em-3.1.0/pwem/protocols/protocol_import/particles.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26948 2023-06-23 15:10:58.000000 scipion-em-3.1.0/pwem/protocols/protocol_import/sequence.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28345 2023-06-23 15:10:58.000000 scipion-em-3.1.0/pwem/protocols/protocol_import/volumes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6071 2023-06-23 15:10:58.000000 scipion-em-3.1.0/pwem/protocols/protocol_mathematical_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31783 2023-06-23 15:10:58.000000 scipion-em-3.1.0/pwem/protocols/protocol_micrographs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4770 2023-06-23 15:10:58.000000 scipion-em-3.1.0/pwem/protocols/protocol_movie_eraser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21511 2023-06-23 15:10:58.000000 scipion-em-3.1.0/pwem/protocols/protocol_movies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7681 2023-06-23 15:10:58.000000 scipion-em-3.1.0/pwem/protocols/protocol_origin_sampling_volume.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25734 2023-06-23 15:10:58.000000 scipion-em-3.1.0/pwem/protocols/protocol_particles.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25337 2023-06-23 15:10:58.000000 scipion-em-3.1.0/pwem/protocols/protocol_particles_picking.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5259 2023-06-23 15:10:58.000000 scipion-em-3.1.0/pwem/protocols/protocol_pdf_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17456 2023-06-23 15:10:58.000000 scipion-em-3.1.0/pwem/protocols/protocol_projection_edit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-06-23 15:10:58.000000 scipion-em-3.1.0/pwem/protocols/protocol_set_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12652 2023-06-23 15:10:58.000000 scipion-em-3.1.0/pwem/protocols/protocol_set_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36458 2023-06-23 15:10:58.000000 scipion-em-3.1.0/pwem/protocols/protocol_sets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7707 2023-06-23 15:10:58.000000 scipion-em-3.1.0/pwem/protocols/protocol_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10282 2023-06-23 15:10:58.000000 scipion-em-3.1.0/pwem/protocols/protocol_tiltpairs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4168 2023-06-23 15:10:58.000000 scipion-em-3.1.0/pwem/protocols/protocol_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5883 2023-06-23 15:10:58.000000 scipion-em-3.1.0/pwem/protocols.conf
+-rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-06-23 15:10:58.000000 scipion-em-3.1.0/pwem/scipion_icon.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:12:46.451061 scipion-em-3.1.0/pwem/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     6537 2023-06-23 15:10:58.000000 scipion-em-3.1.0/pwem/templates/demo.json.template
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:12:46.451061 scipion-em-3.1.0/pwem/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    13717 2023-06-23 15:10:58.000000 scipion-em-3.1.0/pwem/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:12:46.459061 scipion-em-3.1.0/pwem/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 15:10:58.000000 scipion-em-3.1.0/pwem/tests/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)  4875359 2023-06-23 15:10:58.000000 scipion-em-3.1.0/pwem/tests/data/hexonAtomStruct.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41865 2023-06-23 15:10:58.000000 scipion-em-3.1.0/pwem/tests/data/test_convert_atom_struct.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38187 2023-06-23 15:10:58.000000 scipion-em-3.1.0/pwem/tests/data/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5834 2023-06-23 15:10:58.000000 scipion-em-3.1.0/pwem/tests/data/test_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49175 2023-06-23 15:10:58.000000 scipion-em-3.1.0/pwem/tests/data/test_symmetry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:12:46.459061 scipion-em-3.1.0/pwem/tests/protocols/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 15:10:58.000000 scipion-em-3.1.0/pwem/tests/protocols/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8069 2023-06-23 15:10:58.000000 scipion-em-3.1.0/pwem/tests/protocols/test_extract_particles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6760 2023-06-23 15:10:58.000000 scipion-em-3.1.0/pwem/tests/protocols/test_notifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-06-23 15:10:58.000000 scipion-em-3.1.0/pwem/tests/protocols/test_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59195 2023-06-23 15:10:58.000000 scipion-em-3.1.0/pwem/tests/protocols/test_projection_edit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6500 2023-06-23 15:10:58.000000 scipion-em-3.1.0/pwem/tests/protocols/test_protocol_alignment_assign.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3642 2023-06-23 15:10:58.000000 scipion-em-3.1.0/pwem/tests/protocols/test_protocol_boxsize_checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6328 2023-06-23 15:10:58.000000 scipion-em-3.1.0/pwem/tests/protocols/test_protocol_boxsize_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13157 2023-06-23 15:10:58.000000 scipion-em-3.1.0/pwem/tests/protocols/test_protocol_export2DB.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2248 2023-06-23 15:10:58.000000 scipion-em-3.1.0/pwem/tests/protocols/test_protocol_extract_coorinates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6065 2023-06-23 15:10:58.000000 scipion-em-3.1.0/pwem/tests/protocols/test_protocol_invert_Hand.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4183 2023-06-23 15:10:58.000000 scipion-em-3.1.0/pwem/tests/protocols/test_protocol_mathematical_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11658 2023-06-23 15:10:58.000000 scipion-em-3.1.0/pwem/tests/protocols/test_protocol_volume_homogenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8404 2023-06-23 15:10:58.000000 scipion-em-3.1.0/pwem/tests/protocols/test_protocols_assign_orig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3545 2023-06-23 15:10:58.000000 scipion-em-3.1.0/pwem/tests/protocols/test_protocols_import_atomstruct.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9883 2023-06-23 15:10:58.000000 scipion-em-3.1.0/pwem/tests/protocols/test_protocols_import_coords.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6635 2023-06-23 15:10:58.000000 scipion-em-3.1.0/pwem/tests/protocols/test_protocols_import_ctfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2295 2023-06-23 15:10:58.000000 scipion-em-3.1.0/pwem/tests/protocols/test_protocols_import_masks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9168 2023-06-23 15:10:58.000000 scipion-em-3.1.0/pwem/tests/protocols/test_protocols_import_micrographs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6488 2023-06-23 15:10:58.000000 scipion-em-3.1.0/pwem/tests/protocols/test_protocols_import_movies.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10826 2023-06-23 15:10:58.000000 scipion-em-3.1.0/pwem/tests/protocols/test_protocols_import_particles.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25854 2023-06-23 15:10:58.000000 scipion-em-3.1.0/pwem/tests/protocols/test_protocols_import_sequence.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17661 2023-06-23 15:10:58.000000 scipion-em-3.1.0/pwem/tests/protocols/test_protocols_import_volumes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6745 2023-06-23 15:10:58.000000 scipion-em-3.1.0/pwem/tests/protocols/test_protocols_set_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7640 2023-06-23 15:10:58.000000 scipion-em-3.1.0/pwem/tests/protocols/test_protocols_set_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28741 2023-06-23 15:10:58.000000 scipion-em-3.1.0/pwem/tests/protocols/test_protocols_sets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-06-23 15:10:58.000000 scipion-em-3.1.0/pwem/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:12:46.463060 scipion-em-3.1.0/pwem/tests/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-23 15:10:58.000000 scipion-em-3.1.0/pwem/tests/workflows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17388 2023-06-23 15:10:58.000000 scipion-em-3.1.0/pwem/tests/workflows/test_parallel_gpu_queue.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1299 2023-06-23 15:10:58.000000 scipion-em-3.1.0/pwem/tests/workflows/test_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14023 2023-06-23 15:10:58.000000 scipion-em-3.1.0/pwem/tests/workflows/test_workflow_initialvolume.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12779 2023-06-23 15:10:58.000000 scipion-em-3.1.0/pwem/tests/workflows/test_workflow_mixed.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13571 2023-06-23 15:10:58.000000 scipion-em-3.1.0/pwem/tests/workflows/test_workflow_mixed_large.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)   123298 2023-06-23 15:10:58.000000 scipion-em-3.1.0/pwem/tests/workflows/test_workflow_modeling.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11413 2023-06-23 15:10:58.000000 scipion-em-3.1.0/pwem/tests/workflows/test_workflow_xmipp.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4512 2023-06-23 15:10:58.000000 scipion-em-3.1.0/pwem/tests/workflows/test_workflow_xmipp_assignment_tiltpairs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10427 2023-06-23 15:10:58.000000 scipion-em-3.1.0/pwem/tests/workflows/test_workflow_xmipp_ctf_consensus.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5438 2023-06-23 15:10:58.000000 scipion-em-3.1.0/pwem/tests/workflows/test_workflow_xmipp_rct.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4607 2023-06-23 15:10:58.000000 scipion-em-3.1.0/pwem/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:12:46.463060 scipion-em-3.1.0/pwem/viewers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-06-23 15:10:58.000000 scipion-em-3.1.0/pwem/viewers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7978 2023-06-23 15:10:58.000000 scipion-em-3.1.0/pwem/viewers/filehandlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11691 2023-06-23 15:10:58.000000 scipion-em-3.1.0/pwem/viewers/plotter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12857 2023-06-23 15:10:58.000000 scipion-em-3.1.0/pwem/viewers/showj.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-06-23 15:10:58.000000 scipion-em-3.1.0/pwem/viewers/viewer_angular_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5254 2023-06-23 15:10:58.000000 scipion-em-3.1.0/pwem/viewers/viewer_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20154 2023-06-23 15:10:58.000000 scipion-em-3.1.0/pwem/viewers/viewer_chimera.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4929 2023-06-23 15:10:58.000000 scipion-em-3.1.0/pwem/viewers/viewer_fsc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19846 2023-06-23 15:10:58.000000 scipion-em-3.1.0/pwem/viewers/viewer_localres.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-06-23 15:10:58.000000 scipion-em-3.1.0/pwem/viewers/viewer_pdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3349 2023-06-23 15:10:58.000000 scipion-em-3.1.0/pwem/viewers/viewer_sequence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-06-23 15:10:58.000000 scipion-em-3.1.0/pwem/viewers/viewer_vmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7851 2023-06-23 15:10:58.000000 scipion-em-3.1.0/pwem/viewers/viewer_volumes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11970 2023-06-23 15:10:58.000000 scipion-em-3.1.0/pwem/viewers/viewers_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-06-23 15:10:58.000000 scipion-em-3.1.0/pwem/viewers/viewers_protocols.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16407 2023-06-23 15:10:58.000000 scipion-em-3.1.0/pwem/viewers/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:12:46.463060 scipion-em-3.1.0/pwem/wizards/
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-06-23 15:10:58.000000 scipion-em-3.1.0/pwem/wizards/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55857 2023-06-23 15:10:58.000000 scipion-em-3.1.0/pwem/wizards/wizard.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19871 2023-06-23 15:10:58.000000 scipion-em-3.1.0/pwem/wizards/wizards.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:12:46.463060 scipion-em-3.1.0/pwem/wizards/wizards_3d/
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-06-23 15:10:58.000000 scipion-em-3.1.0/pwem/wizards/wizards_3d/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5583 2023-06-23 15:10:58.000000 scipion-em-3.1.0/pwem/wizards/wizards_3d/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9201 2023-06-23 15:10:58.000000 scipion-em-3.1.0/pwem/wizards/wizards_3d/mask_structure_wizard.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10999 2023-06-23 15:10:58.000000 scipion-em-3.1.0/pwem/wizards/wizards_3d/mask_volume_wizard.py
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-23 15:10:58.000000 scipion-em-3.1.0/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:12:46.467060 scipion-em-3.1.0/scipion_em.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-06-23 15:12:46.000000 scipion-em-3.1.0/scipion_em.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5442 2023-06-23 15:12:46.000000 scipion-em-3.1.0/scipion_em.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 15:12:46.000000 scipion-em-3.1.0/scipion_em.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-23 15:12:46.000000 scipion-em-3.1.0/scipion_em.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-23 15:12:46.000000 scipion-em-3.1.0/scipion_em.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-23 15:12:46.000000 scipion-em-3.1.0/scipion_em.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 15:12:46.467060 scipion-em-3.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-06-23 15:10:58.000000 scipion-em-3.1.0/setup.py
```

### Comparing `scipion-em-3.0.9/LICENSE` & `scipion-em-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `scipion-em-3.0.9/PKG-INFO` & `scipion-em-3.1.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,60 +1,62 @@
 Metadata-Version: 1.1
 Name: scipion-em
-Version: 3.0.9
+Version: 3.1.0
 Summary: This modules contains classes related with EM
 Home-page: https://github.com/scipion-em/scipion-em
 Author: J.M. De la Rosa Trevin, Roberto Marabini, Grigory Sharov, Josue Gomez Blanco, Pablo Conesa, Yunior Fonseca Reyna
 Author-email: delarosatrevin@scilifelab.se, roberto@cnb.csic.es, gsharov@mrc-lmb.cam.ac.uk, josue.gomez-blanco@mcgill.ca, pconesa@cnb.csic.es, fonsecareyna@cnb.csic.es
 License: UNKNOWN
-Description: ====
+Description: .. image:: https://img.shields.io/badge/Contributor%20Covenant-v2.0%20adopted-ff69b4.svg
+          :width: 200
+          :alt: Contributor Covenant
+          :target: https://www.contributor-covenant.org/version/2/0/code_of_conduct/
+        
+        
         pwem
         ====
         
         **pwem** is a Python module of Scipion framework for image processing in Electron Microscopy
         
-        
         The entire collection is licensed under the terms of the GNU Public License,
         version 3 (GPLv3).
         
-        -------------
         Development
-        -------------
+        -----------
         
         To install **pwem** for development purposes, one can do:
         
-        ::
+        .. code-block:: bash
         
             # Create a clean virtual environment
-            python -m venv ~/myenv
-            source ~/myenv/bin/activate
-            git clone git@github.com:scipion-em/scipion-em.git
+            conda create -n scipion python=3.8
+            conda activate
+            git clone https://github.com/scipion-em/scipion-em.git
             cd scipion-em
-            python -m pip install -e .  # Install in the environment as development
+            pip install -e .
         
-        -------------
         Running tests
         -------------
         
-        First make sure that **pwem** is available as a Python module in your
-        current Python environment. During development, I tend to set the PYTHONPATH:
-        
-        ::
+        .. code-block:: bash
         
+            conda activate scipion
             cd scipion-em
-            # Either you have installed as mentioned above, or modify the PYTHONPATH
-            export PYTHONPATH=$PYTHONPATH:$PWD
-            # After pyworkflow is accessible as a module, then:
-            cd pwem/tests
-        
+            export SCIPION_DOMAIN="pwem"
             python -m unittest discover
         
+        API documentation
+        -----------------
+        
+        https://scipion-em.github.io/docs/release-3.0.0/api/pwem/pwem.html
         
 Keywords: scipion cryoem imageprocessing scipion-3.0
 Platform: UNKNOWN
-Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering
```

### Comparing `scipion-em-3.0.9/pwem/bibtex.py` & `scipion-em-3.1.0/pwem/bibtex.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.0.9/pwem/cmd/convert.py` & `scipion-em-3.1.0/pwem/cmd/convert.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.0.9/pwem/cmd/program.py` & `scipion-em-3.1.0/pwem/cmd/program.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.0.9/pwem/constants.py` & `scipion-em-3.1.0/pwem/constants.py`

 * *Files 8% similar despite different names*

```diff
@@ -37,15 +37,17 @@
 
 RELATION_CTF = 'relation_ctf'
 
 UNIT_PIXEL = 'px'
 UNIT_PIXEL_FOURIER = '1/px'
 UNIT_ANGSTROM = 'A'
 UNIT_ANGSTROM_FOURIER = '1/A'
-UNIT_ANGSTROM_SYMBOL = u"\u212B" # No needed: Å should be valid as long as first line in file has utf-8 directive --> # -*- coding: utf-8 -*-
+# No needed: Å should be valid as long as first line
+# in file has utf-8 directive --> # -*- coding: utf-8 -*-
+UNIT_ANGSTROM_SYMBOL = u"\u212B"
 
 # Fourier Filter options
 FILTER_LOW_PASS = 0
 FILTER_HIGH_PASS = 1
 FILTER_BAND_PASS = 2
 FILTER_GAUSSIAN = 3
 FILTER_LOW_PASS_NO_DECAY = 4
@@ -65,75 +67,89 @@
 COLOR_TERRAIN = 1
 COLOR_GIST_EARTH = 2
 COLOR_GIST_NCAR = 3
 COLOR_GNU_PLOT = 4
 COLOR_GNU_PLOT2 = 5
 COLOR_OTHER = 6
 
-COLOR_CHOICES = ['jet', 'terrain',  'gist_earth', 'gist_ncar', 'gnuplot', 'gnuplot2', 'other']
+COLOR_CHOICES = ['jet', 'terrain', 'gist_earth',
+                 'gist_ncar', 'gnuplot', 'gnuplot2', 'other']
 
 # Axis code
 AX_X = 0
 AX_Y = 1
 AX_Z = 2
 
-
-# SYMMETRY, conventions described atr: https://scipion-em.github.io/docs/docs/developer/symmetries
+# SYMMETRY, conventions described at:
+# https://scipion-em.github.io/docs/docs/developer/symmetries
 # Some notes:
 # Icosahedral
 #   xmipp and relion define I1, I2, I3 and I4 that corerspond to
 #   I222, I222r, In25 and In25z
-#   cryosparc has I1 and I2 
-#   EMAN always puts the highest symmetry axis on Z. 
+#   cryosparc has I1 and I2
+#   EMAN always puts the highest symmetry axis on Z.
 #   and a 2 fold axis in X (so it uses I2n5 or I2n5r, not sure)
 # DIEDRAL: first axis Z, second X (DX) except cryosparc that uses y (DY)
-# Tetraedral, most of the programs use T222, EMAN uses Tz3
-SYM_CYCLIC = 0  # CN cyclic symmetry Cn around z axis
-SYM_DIHEDRAL = 1  # DN cyclic symmetry plus and extra 2fold symmetry axis around X
+# Tetraedral, most of the programs use TZ3
+# CN cyclic symmetry Cn around z axis
+SYM_CYCLIC = 0
+# DN cyclic symmetry plus and extra 2fold symmetry axis around X
+SYM_DIHEDRAL = 1
 SYM_DIHEDRAL_X = SYM_DIHEDRAL
-SYM_DIHEDRAL_Y = 2  # DN cyclic symmetry plus and extra 2fold symmetry axis around Y (cryoSparc)
-SYM_TETRAHEDRAL = 3  # T 222 Tetrahedral symmetry with two-fold symmetry axes along the X, Y,
-# and Z axes, a three-fold along axis (1,1,1)
-SYM_TETRAHEDRAL_Z3 = 4  # T  three-fold symmetry axis along Z, another three-fold axis 
-# in the YZ plane such that rotation about the X axis by ~110°
-# is a symmetry operation (EMAN convention)
+# DN cyclic symmetry plus and extra 2fold symmetry axis around Y (cryoSparc)
+SYM_DIHEDRAL_Y = 2
+# T 222 Tetrahedral symmetry with two-fold symmetry axis along the X, Y and Z
+SYM_TETRAHEDRAL = 3
+SYM_TETRAHEDRAL_222 = SYM_TETRAHEDRAL
+# T  three-fold symmetry axis along Z, another three-fold axis
+# in the YZ plane such that the sign(y) != sign(z)
+SYM_TETRAHEDRAL_Z3 = 4
+# SYM_TETRAHEDRAL222R  is a degenerated symmetry, that is
+# for each symmetry axis (x,y,z)  defined in T222, there is a
+# symmetry axis (-x,-y,-z) in T222R, therefore the produced
+# symmetry matrices are equivalent
+# SYM_TETRAHEDRAL222R = 14
+
+# T  three-fold symmetry axis along Z, another three-fold axis
+# in the YZ plane such that  sign(y) = sign(z)
+SYM_TETRAHEDRAL_Z3R = 5
 
-SYM_OCTAHEDRAL = 5  # O
+SYM_OCTAHEDRAL = 6  # O
 
 # icosahedric IXXX
 # (no crowther 222 and standard in heyman et al 2005 article).
 # 2-fold axes on x,y,z axes. With the positive z-axis pointing at the viewer,
 # the front-most 5-fold vertices are in yz plane, and the front-most 3-fold
 # axes are in the xz plane.
-SYM_I222 = 6
+SYM_I222 = 7
 
 # (crowther) 2-fold axes on x,y,z axes. With the positive z-axis pointing at
 # the viewer, the front-most 5-fold vertices are in xz plane,
 # and the front-most 3-fold axes are in the yz plane.
 # (222 rotated 90 degrees around Z)
-SYM_I222r = 7 
+SYM_I222r = 8
 
-# '2-fold symmetry along y and 5-fold along z 
-SYM_In25 = 8
+# '2-fold symmetry along y and 5-fold along z
+SYM_In25 = 9
 
 # 'n25' with 180 degree rotation about x
-SYM_In25r = 9
-
-SYM_I2n3 = 10  # Two-fold symmetry along X and 3-fold along Z
-SYM_I2n3r = 11  # Idem but rotated 180 degree about Y
-SYM_I2n5 = 12  # Two-fold symmetry along Y and 5-fold along Z
-SYM_I2n5r = 13  # Idem but rotated 180 degree about X
+SYM_In25r = 10
+SYM_I2n3 = 11  # Two-fold symmetry along X and 3-fold along Z
+SYM_I2n3r = 12  # Idem but rotated 180 degree about Y
+SYM_I2n5 = 13  # Two-fold symmetry along Y and 5-fold along Z
+SYM_I2n5r = 14  # Idem but rotated 180 degree about X
 
 # Symmetry dictionary
 SCIPION_SYM_NAME = dict()
 SCIPION_SYM_NAME[SYM_CYCLIC] = 'Cn'
 SCIPION_SYM_NAME[SYM_DIHEDRAL_X] = 'Dxn'
 SCIPION_SYM_NAME[SYM_DIHEDRAL_Y] = 'Dyn'
 SCIPION_SYM_NAME[SYM_TETRAHEDRAL] = 'T222'
 SCIPION_SYM_NAME[SYM_TETRAHEDRAL_Z3] = 'Tz3'
+SCIPION_SYM_NAME[SYM_TETRAHEDRAL_Z3R] = 'Tz3r'
 SCIPION_SYM_NAME[SYM_OCTAHEDRAL] = 'O'
 SCIPION_SYM_NAME[SYM_I222] = 'I222'
 SCIPION_SYM_NAME[SYM_I222r] = 'I222r'
 SCIPION_SYM_NAME[SYM_In25] = 'In25'
 SCIPION_SYM_NAME[SYM_In25r] = 'In25r'
 SCIPION_SYM_NAME[SYM_I2n3] = 'I2n3'
 SCIPION_SYM_NAME[SYM_I2n3r] = 'I2n3r'
@@ -147,22 +163,39 @@
 
 # maxit
 MAXIT_HOME = 'MAXIT_HOME'
 MAXIT = 'maxit'
 
 # Explanation messages for the wizards
 RING_MASK_WIZ_MSG = \
-    'The values of the outer and inner radius can be controlled via both the sliders placed below or ' \
-    'the mousewheel (when the mouse cursor is over the image). The arrow (=>) located at the left of ' \
-    'the sliders is used to indicate which one is active. To change from one to another, simply ' \
+    'The values of the outer and inner radius can be controlled via '\
+    'both the sliders placed below or '\
+    'the mousewheel (when the mouse cursor is over the image). '\
+    'The arrow (=>) located at the left of '\
+    'the sliders is used to indicate which one is active. '\
+    'To change from one to another, simply '\
     'click and drag the corresponding slider or use up and down keys.'
 CIRCLE_MASK_WIZ_MSG = \
-    'The values of the mask radius can be controlled via both the slider or the mousewheel (when ' \
+    'The values of the mask radius can be controlled via '\
+    'both the slider or the mousewheel (when ' \
     'the mouse cursor is over the image).'
-FREQ_BANDPASS_WIZ_MSG = \
-    'The values of the low and high frequencies can be controlled via both the sliders placed below or ' \
-    'the mousewheel (when the mouse cursor is over the image). The arrow (=>) located at the left of ' \
-    'the sliders is used to indicate which one is active. To change from one to another, simply ' \
-    'click and drag the corresponding slider or use up and down keys. Values are shown in both digital ' \
+FREQ_BANDPASS_WIZ_MSG =\
+    'The values of the low and high frequencies can '\
+    'be controlled via both the sliders placed below or '\
+    'the mousewheel (when the mouse cursor is over the image). '\
+    'The arrow (=>) located at the left of '\
+    'the sliders is used to indicate which one is active. '\
+    'To change from one to another, simply '\
+    'click and drag the corresponding slider or use up and down keys. '\
+    'Values are shown in both digital '\
     'frequency and angstroms.'
 
 EM_ROOT_VAR = 'EM_ROOT'
+
+DEFAULT_MAX_PREVIEW_FILE_SIZE = 500  # Unit is MB: 500 MB
+
+RESIDUES3TO1 = {'CYS': 'C', 'ASP': 'D', 'SER': 'S', 'GLN': 'Q', 'LYS': 'K',
+                'ILE': 'I', 'PRO': 'P', 'THR': 'T', 'PHE': 'F', 'ASN': 'N',
+                'GLY': 'G', 'HIS': 'H', 'LEU': 'L', 'ARG': 'R', 'TRP': 'W',
+                'ALA': 'A', 'VAL': 'V', 'GLU': 'E', 'TYR': 'Y', 'MET': 'M'}
+
+RESIDUES1TO3 = {v: k for k, v in RESIDUES3TO1.items()}
```

### Comparing `scipion-em-3.0.9/pwem/convert/__init__.py` & `scipion-em-3.1.0/pwem/convert/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,13 +23,13 @@
 # *  e-mail address 'scipion@cnb.csic.es'
 # *
 # **************************************************************************
 
 from .utils import getSubsetByDefocus, downloadPdb
 from .atom_struct import AtomicStructHandler, toCIF, cifToPdb
 from .headers import Ccp4Header
-from .symmetry import getSymmetryMatrices, Icosahedron
+from .symmetry import (getSymmetryMatrices, Icosahedron, getUnitCell, moveParticlesInsideUnitCell)
 from .transformations import identity_matrix
 from .sequence import *
 from .transformations import (euler_matrix, translation_matrix,
                               concatenate_matrices)
```

### Comparing `scipion-em-3.0.9/pwem/convert/atom_struct.py` & `scipion-em-3.1.0/pwem/protocols/protocol_align_movies.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # **************************************************************************
 # *
-# * Authors:     Roberto Marabini (roberto@cnb.csic.es)
-# *              Marta Martinez (mmmtnez@cnb.csic.es)
+# * Authors:     J.M. De la Rosa Trevin (jmdelarosa@cnb.csic.es)
+# *              Vahid Abrishami (vabrishami@cnb.csic.es)
+# *              Josue Gomez Blanco (josue.gomez-blanco@mcgill.ca)
 # *
 # * Unidad de  Bioinformatica of Centro Nacional de Biotecnologia , CSIC
 # *
 # * This program is free software; you can redistribute it and/or modify
 # * it under the terms of the GNU General Public License as published by
 # * the Free Software Foundation; either version 3 of the License, or
 # * (at your option) any later version.
@@ -20,883 +21,794 @@
 # * Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA
 # * 02111-1307  USA
 # *
 # *  All comments concerning this program package may be sent to the
 # *  e-mail address 'scipion@cnb.csic.es'
 # *
 # **************************************************************************
-#
-# cif to pdb conversion is based on  cif2pdb.py by Spencer Bliven
-# <spencer.bliven@gmail.com>
-#
-# see http://biopython.org/DIST/docs/tutorial/Tutorial.html for a description
-# on the object "structure" and other Bio.xxxx modules
-
-from Bio.PDB.Dice import ChainSelector
-from Bio.PDB.MMCIFParser import MMCIFParser
-from Bio.PDB.PDBParser import PDBParser
-from Bio.PDB import PDBIO, MMCIFIO
-from Bio.PDB.mmcifio import mmcif_order
-
-from Bio.PDB.MMCIF2Dict import MMCIF2Dict
-from Bio.PDB import Entity
-from Bio.PDB import PDBList
-from collections import OrderedDict
-from Bio.PDB.Polypeptide import is_aa
-from Bio.PDB.Polypeptide import three_to_one
-from Bio.Seq import Seq
-from pwem import Plugin, MAXIT_HOME
-from pwem.convert.transformations import translation_from_matrix
-import mmap
-import re
+import enum
 import os
-import numpy
-import pyworkflow.utils as pwutils
-import shutil
-
-
-class OutOfChainsError(Exception):
-    pass
+import warnings
 
+try:
+    from itertools import izip
+except ImportError:
+    izip = zip
+from math import ceil
 
-class scipionMMCIFIO(MMCIFIO):
+import pyworkflow.object as pwobj
+import pyworkflow.utils as pwutils
+from pyworkflow.gui.plotter import Plotter
+import pyworkflow.protocol.params as params
+import pyworkflow.protocol.constants as pwcts
+
+import pwem.objects as emobj
+from pwem import emlib
+
+from pwem.protocols import ProtProcessMovies
+
+OUT_MICS = "outputMicrographs"
+OUT_MICS_DW = "outputMicrographsDoseWeighted"
+OUT_MOVIES = "outputMovies"
+OUT_MICS_ODD = 'outputMicrographsOdd'
+OUT_MICS_EVEN = 'outputMicrographsEven'
+
+
+class ProtAlignMovies(ProtProcessMovies):
+    """
+    Base class for movie alignment protocols such as:
+    motioncorr, crosscorrelation and optical flow
+
+    Alignment parameters are defined in common. For example,
+    the frames range used for alignment and final sum, the binning factor
+    or the cropping options (region of interest)
+    """
+    _possibleOutputs = {OUT_MICS: emobj.SetOfMicrographs,
+                        OUT_MICS_DW: emobj.SetOfMicrographs,
+                        OUT_MICS_ODD: emobj.SetOfMicrographs,
+                        OUT_MICS_EVEN: emobj.SetOfMicrographs,
+                        OUT_MOVIES: emobj.SetOfMovies}
+
+    # Even / odd functionality
+    evenOddCapable = False
+
+    # -------------------------- DEFINE param functions -----------------------
+    def _defineParams(self, form):
+        ProtProcessMovies._defineParams(self, form)
+        self._defineAlignmentParams(form)
+
+    def _defineAlignmentParams(self, form):
+        group = form.addGroup('Alignment')
+        line = group.addLine('Frames to ALIGN',
+                             help='Frames range to ALIGN on each movie. The '
+                                  'first frame is 1. If you set 0 in the final '
+                                  'frame to align, it means that you will '
+                                  'align until the last frame of the movie.')
+        line.addParam('alignFrame0', params.IntParam, default=1,
+                      label='from')
+        line.addParam('alignFrameN', params.IntParam, default=0,
+                      label='to')
+        group.addParam('useAlignToSum', params.BooleanParam, default=True,
+                       label='Use ALIGN frames range to SUM?',
+                       help="If *Yes*, the same frame range will be used to "
+                            "ALIGN and to SUM. If *No*, you can selected a "
+                            "different range for SUM (must be a subset).")
+        line = group.addLine('Frames to SUM', condition="not useAlignToSum",
+                             help='Frames range to SUM on each movie. The '
+                                  'first frame is 1. If you set 0 in the final '
+                                  'frame to sum, it means that you will sum '
+                                  'until the last frame of the movie.')
+        line.addParam('sumFrame0', params.IntParam, default=1,
+                      label='from')
+        line.addParam('sumFrameN', params.IntParam, default=0,
+                      label='to')
+        group.addParam('binFactor', params.FloatParam, default=1.,
+                       label='Binning factor',
+                       help='1x or 2x. Bin stack before processing.')
+
+        line = group.addLine('Crop offsets (px)')
+        line.addParam('cropOffsetX', params.IntParam, default=0, label='X')
+        line.addParam('cropOffsetY', params.IntParam, default=0, label='Y')
+
+        line = group.addLine('Crop dimensions (px)',
+                             help='How many pixels to crop from offset\n'
+                                  'If equal to 0, use maximum size.')
+        line.addParam('cropDimX', params.IntParam, default=0, label='X')
+        line.addParam('cropDimY', params.IntParam, default=0, label='Y')
+
+        form.addParam('doSaveAveMic', params.BooleanParam, default=True,
+                      label="Save aligned micrograph",
+                      expertLevel=pwcts.LEVEL_ADVANCED)
+
+        form.addParam('doSaveMovie', params.BooleanParam, default=False,
+                      label="Save movie", expertLevel=pwcts.LEVEL_ADVANCED,
+                      help="Save Aligned movie")
+
+        if self.evenOddCapable:
+            form.addParam('splitEvenOdd', params.BooleanParam,
+                          default=False,
+                          label='Split & sum odd/even frames?',
+                          expertLevel=params.LEVEL_ADVANCED,
+                          help='Generate odd and even sums using odd and even frames '
+                               'respectively when this option is enabled.')
+
+    # --------------------------- STEPS functions ----------------------------
+    def createOutputStep(self):
+        # validate that we have some output movies
+        for outName, out in self.iterOutputAttributes():
+            output = out
+            break
+
+        if output.getSize() == 0 and len(self.listOfMovies) != 0:
+            raise Exception("All movies failed, didn't create outputMicrographs."
+                            "Please review movie processing steps above.")
+        elif output.getSize() < len(self.listOfMovies):
+            self.warning(pwutils.yellowStr("WARNING - Failed to align %d movies."
+                                           % (len(self.listOfMovies) - output.getSize())))
+
+    def _loadOutputSet(self, SetClass, baseName, fixSampling=True):
+        """
+        Load the output set if it exists or create a new one.
+        fixSampling: correct the output sampling rate if binning was used,
+        except for the case when the original movies are kept and shifts
+        refers to that one.
+        """
+        setFile = self._getPath(baseName)
+
+        if os.path.exists(setFile) and os.path.getsize(setFile) > 0:
+            outputSet = SetClass(filename=setFile)
+            outputSet.loadAllProperties()
+            outputSet.enableAppend()
+        else:
+            outputSet = SetClass(filename=setFile)
+            outputSet.setStreamState(outputSet.STREAM_OPEN)
+
+            inputMovies = self.inputMovies.get()
+            outputSet.copyInfo(inputMovies)
+
+            if fixSampling:
+                newSampling = inputMovies.getSamplingRate() * self._getBinFactor()
+                outputSet.setSamplingRate(newSampling)
+
+        return outputSet
+
+    def _updateOutputMicSet(self, newDone, sqliteFn, getOutputMicName,
+                            outputName, streamMode):
+        """ Updated the output micrographs set with new items found. """
+        micSet = self._loadOutputSet(emobj.SetOfMicrographs, sqliteFn)
+        doneFailed = []
+
+        for movie in newDone:
+            mic = micSet.ITEM_TYPE()
+            mic.copyObjId(movie)
+            mic.setMicName(movie.getMicName())
+            # The subclass protocol is responsible for generating the output
+            # micrograph file in the extra path with the required name
+            extraMicFn = self._getExtraPath(getOutputMicName(movie))
+            mic.setFileName(extraMicFn)
+            if not os.path.exists(extraMicFn):
+                print(pwutils.yellowStr("WARNING: Micrograph %s was not generated, "
+                                        "can't add it to output set." % extraMicFn))
+                doneFailed.append(movie)
+                continue
+            # Tolerate errors here. Usually here some plots are generated.
+            try:
+                self._preprocessOutputMicrograph(mic, movie)
+            except Exception as e:
+                self.error("Couldn't prepare output details: %s" % e)
+                doneFailed.append(movie)
+                continue
+
+            micSet.append(mic)
+
+        self._updateOutputSet(outputName, micSet, streamMode)
+        if doneFailed:
+            self._writeFailedList(doneFailed)
+
+        if self._firstTimeOutput:
+            # We consider that Movies are 'transformed' into the Micrographs
+            # This will allow to extend the CTF associated to a set of
+            # micrographs to another set of micrographs generated from a
+            # different movie alignment
+            self._defineTransformRelation(self.inputMovies, micSet)
+
+    def _updateOutputMovieSet(self, newDone, streamMode):
+        saveMovie = self.getAttributeValue('doSaveMovie', False)
+        movieSet = self._loadOutputSet(emobj.SetOfMovies, 'movies.sqlite',
+                                       fixSampling=saveMovie)
+
+        # If we need to save the movies
+        if saveMovie:
+            movieSet.setGain(None)
+            movieSet.setDark(None)
 
-    # this class was needed before including maxit
-    # as converter.
-    # TODO: Delete it after a more extensive testing period
-    # DATE mar feb 18 17:48:57 CET 2020
-
-    def _save_dict_delete(self, out_file):
-        # Form dictionary where key is first part of mmCIF key and value is list
-        # of corresponding second parts
-        key_lists = {}
-        for key in self.dic:
-            if key == "data_":
-                data_val = self.dic[key]
-            else:
-                s = re.split(r"\.", key)
-                if len(s) == 2:
-                    if s[0] in key_lists:
-                        key_lists[s[0]].append(s[1])
-                    else:
-                        key_lists[s[0]] = [s[1]]
+        for movie in newDone:
+            try:
+                newMovie = self._createOutputMovie(movie)
+                if newMovie.getAlignment().getShifts()[0]:
+                    movieSet.append(newMovie)
                 else:
-                    raise ValueError("Invalid key in mmCIF dictionary: " + key)
-
-        # Re-order lists if an order has been specified
-        # Not all elements from the specified order are necessarily present
-        for key, key_list in key_lists.items():
-            # P3
-            # for key, key_list in list(key_lists.items()):
-            if key in mmcif_order:
-                inds = []
-                for i in key_list:
-                    try:
-                        inds.append(mmcif_order[key].index(i))
-                    # Unrecognised key - add at end
-                    except ValueError:
-                        inds.append(len(mmcif_order[key]))
-                key_lists[key] = [k for _, k in sorted(zip(inds, key_list))]
-
-        # Write out top data_ line
-        if data_val:
-            out_file.write("data_" + data_val + "\n#\n")
-            # ESCRIBIR POLYSEQTABLE
-            out_file.write("""loop_
-_entity_poly_seq.entity_id
-_entity_poly_seq.num
-_entity_poly_seq.mon_id
-_entity_poly_seq.hetero\n#\n""")
-            total_seqs = []
-            counter_chain = 1
-            for model in self.structure:
-                for chain in model:
-                    min_val = int(chain.get_unpacked_list()[0].id[1])
-                    # max_val = min_val + len(chain.get_unpacked_list())
-                    #                    not_are = range(1, min_val-1)
-                    #                    for i in range(min_val)[:-1]:
-                    #                        not_are.append(i + 1)
-                    counter = 1
-                    if min_val > 1:
-                        for counter in range(1, min_val):
-                            if len(chain.get_unpacked_list()[0].resname.strip()) == 3:
-                                total_seqs.append((counter_chain, str(counter), "XAA", "n"))
-                            elif len(chain.get_unpacked_list()[0].resname.strip()) == 2:
-                                total_seqs.append((counter_chain, str(counter), "DX", "n"))
-                            elif len(chain.get_unpacked_list()[0].resname.strip()) == 1:
-                                total_seqs.append((counter_chain, str(counter), "X", "n"))
-                            counter += 1
-                    for residue in chain:
-                        if len(chain.get_unpacked_list()[0].resname.strip()) == 3 and \
-                                is_aa(residue.get_resname(), standard=True):  # aminoacids
-                            total_seqs.append((counter_chain, residue.id[1], residue.get_resname(), "n"))
-                        elif len(chain.get_unpacked_list()[0].resname.strip()) == 2 and \
-                                residue.get_resname()[1] in ['A', 'C', 'G', 'T']:
-                            total_seqs.append((counter_chain, counter, residue.get_resname(), "n"))
-                        elif len(chain.get_unpacked_list()[0].resname.strip()) == 1 and \
-                                residue.get_resname() in ['A', 'C', 'G', 'U']:
-                            total_seqs.append((counter_chain, counter, residue.get_resname(), "n"))
-                        counter += 1
-                    counter_chain += 1
-            for item in total_seqs:
-                item = list(item)
-                out_file.write("""%s %s %s  %s\n""" %
-                               (str(item[0]), item[1], item[2], item[3]))
-
-        for key, key_list in key_lists.items():
-            #  for key, key_list in list(key_lists.items()):
-            # Pick a sample mmCIF value, which can be a list or a single value
-            sample_val = self.dic[key + "." + key_list[0]]
-            n_vals = len(sample_val)
-            # Check the mmCIF dictionary has consistent list sizes
-            for i in key_list:
-                val = self.dic[key + "." + i]
-                if (isinstance(sample_val, list) and (isinstance(val, str) or len(val) != n_vals)) or (
-                        isinstance(sample_val, str) and isinstance(val, list)):
-                    raise ValueError("Inconsistent list sizes in mmCIF dictionary: " + key + "." + i)
-            # If the value is a single value, write as key-value pairs
-            if isinstance(sample_val, str):
-                m = 0
-                # Find the maximum key length
-                for i in key_list:
-                    if len(i) > m:
-                        m = len(i)
-                for i in key_list:
-                    out_file.write(
-                        "{k: <{width}}".format(k=key + "." + i, width=len(key) + m + 4) + self._format_mmcif_col(
-                            self.dic[key + "." + i], len(self.dic[key + "." + i])) + "\n")
-            # If the value is a list, write as keys then a value table
-            elif isinstance(sample_val, list):
-                out_file.write("loop_\n")
-                col_widths = {}
-                # Write keys and find max widths for each set of values
-                for i in key_list:
-                    out_file.write(key + "." + i + "\n")
-                    col_widths[i] = 0
-                    for val in self.dic[key + "." + i]:
-                        len_val = len(val)
-                        # If the value requires quoting it will add 2 characters
-                        if self._requires_quote(val) and not self._requires_newline(val):
-                            len_val += 2
-                        if len_val > col_widths[i]:
-                            col_widths[i] = len_val
-                # Technically the max of the sum of the column widths is 2048
-
-                # Write the values as rows
-                for i in range(n_vals):
-                    for col in key_list:
-                        out_file.write(self._format_mmcif_col(self.dic[key + "." + col][i], col_widths[col] + 1))
-                    out_file.write("\n")
-            else:
-                raise ValueError("Invalid type in mmCIF dictionary: " + str(type(sample_val)))
-            out_file.write("#\n")
-
-
-class AtomicStructHandler:
-    """ Class that contain utilities to handle pdb/cif files"""
-    PDB = 0
-    CIF = 1
-
-    def __init__(self, fileName=None, permissive=1):
-        # The PERMISSIVE flag indicates that a number of common problems
-        # associated with PDB files will be ignored
-        self.permissive = permissive
-        self.pdbParser = None
-        self.cifParser = None
-        self.ioPDB = None
-        self.ioCIF = None
-        self.structure = None
-        self._readDone = False
-        if fileName is not None:
-            self.read(fileName)
-
-    def readFromPDBDatabase(self, pdbID, dir=None, type='mmCif'):
-        """
-        Retrieve structure from PDB
-        :param pdbID:
-        :param dir: save structure in this directory
-        :param type:  mmCif or pdb
-        :return: filename with pdb file
-        """
-        if dir is None:
-            dir = os.getcwd()
-        pdbl = PDBList(pdb=dir)
-        fileName = pdbl.retrieve_pdb_file(pdbID, pdir=dir, file_format=type)
-        return os.path.abspath(fileName)
-
-    def checkLabelInFile(self, fileName, label):
-        with open(fileName, "r") as f:
-            s = mmap.mmap(f.fileno(), 0, access=mmap.ACCESS_READ)
-            if s.find(label) != -1:
-                return True
-            else:
-                return False
-
-    def getStructure(self):
-        """return structure information, model, chain,
-           residues, atoms..."""
-        return self.structure
-
-    def read(self, fileName):
-        """ Read and parse file."""
-        # biopython assigns an ID to any read structure
-        structure_id = os.path.basename(fileName)
-        structure_id = structure_id[:4] if len(structure_id) > 4 else "1xxx"
-
-        if fileName.endswith(".pdb") or fileName.endswith(".ent"):
-            if self.pdbParser is None:
-                self.pdbParser = PDBParser(PERMISSIVE=self.permissive)
-            parser = self.pdbParser
-            self.type = self.PDB
-        else:
-            if self.cifParser is None:
-                self.cifParser = MMCIFParser()
-            parser = self.cifParser
-            self.type = self.CIF
-
-        self.structure = parser.get_structure(structure_id, fileName)
-        self._readDone = True
-
-    def checkRead(self):
-        if self._readDone:
-            return True
-        else:
-            print("you must read the pdb file first")
-            exit(0)
-
-    def getModelsChains(self):
-        """
-        given an atomic structure returns two dictionaries:
-            (1) for all models and respective chains (chainID and length of residues)
-            (2) for each chain list of residues
-        """
-        self.checkRead()
-        listOfChains = OrderedDict()
-        listOfResidues = OrderedDict()
-
-        for model in self.structure:
-            chainDicLength = OrderedDict()
-            chainDicFirstResidue = OrderedDict()
-            for chain in model:
-                if len(chain.get_unpacked_list()[0].resname.strip()) == 1:  # RNA
-                    seq = list()
-                    seq_number = list()
-                    for residue in chain:
-                        if residue.get_resname() in ['A', 'C', 'G', 'U']:
-                            seq.append(residue.get_resname())
-                        else:
-                            seq.append("X")
-                        seq_number.append((residue.get_id()[1], residue.get_resname()))
-                elif len(chain.get_unpacked_list()[0].resname.strip()) == 2:  # DNA
-                    seq = list()
-                    seq_number = list()
-                    for residue in chain:
-                        if residue.get_resname()[1] in ['A', 'C', 'G', 'T']:
-                            seq.append(residue.get_resname()[1])
-                        else:
-                            seq.append("X")
-                        seq_number.append((residue.get_id()[1], residue.get_resname()))
-                elif len(chain.get_unpacked_list()[0].resname.strip()) == 3:  # Protein
-                    seq = list()
-                    seq_number = list()
-                    counter = 0
-                    for residue in chain:
-                        if is_aa(residue.get_resname(), standard=True):  # aminoacids
-                            seq.append(three_to_one(residue.get_resname()))
-                            counter += 1
-                        else:
-                            seq.append("X")
-                        seq_number.append((residue.get_id()[1], residue.get_resname()))
-                    if counter == 0:  # HETAM
-                        for residue in chain:
-                            seq.append(residue.get_resname())
-                while seq[-1] == "X":
-                    del seq[-1]
-                while seq[0] == "X":
-                    del seq[0]
-                chainDicLength[chain.id] = len(seq)
-                chainDicFirstResidue[chain.id] = seq_number
-            listOfChains[model.id] = chainDicLength
-            listOfResidues[model.id] = chainDicFirstResidue
-
-        return listOfChains, listOfResidues
-
-    def getSequenceFromChain(self, modelID, chainID):
-        self.checkRead()
-        seq = list()
-        for model in self.structure:
-            if model.id == modelID:
-                for chain in model:
-                    if str(chain.id) == chainID:
-                        if len(chain.get_unpacked_list()[0].resname) == 1:
-                            print("Your sequence is a nucleotide sequence ("
-                                  "RNA)\n")
-                            # alphabet = IUPAC.IUPACAmbiguousRNA._upper()
-                            for residue in chain:
-                                # Check if the residue belongs to the
-                                # standard RNA and add those residues to the
-                                # seq
-                                if residue.get_resname() in ['A', 'C',
-                                                             'G', 'U']:
-                                    seq.append(residue.get_resname())
-                                else:
-                                    seq.append("X")
-                        elif len(chain.get_unpacked_list()[0].resname) == 2:
-                            print("Your sequence is a nucleotide sequence ("
-                                  "DNA)\n")
-                            # alphabet = IUPAC.ExtendedIUPACDNA._upper()
-                            for residue in chain:
-                                # Check if the residue belongs to the
-                                # standard DNA and add those residues to the
-                                # seq
-                                if residue.get_resname()[1] in ['A', 'C',
-                                                                'G', 'T']:
-                                    seq.append(residue.get_resname()[1])
-                                else:
-                                    seq.append("X")
-                        elif len(chain.get_unpacked_list()[0].resname) == 3:
-                            counter = 0
-                            for residue in chain:
-                                if is_aa(residue.get_resname(), standard=True):
-                                    # alphabet = IUPAC.ExtendedIUPACProtein._upper()
-                                    # The test checks if the amino acid
-                                    # is one of the 20 standard amino acids
-                                    # Some proteins have "UNK" or "XXX", or other symbols
-                                    # for missing or unknown residues
-                                    seq.append(three_to_one(residue.get_resname()))
-                                    counter += 1
-                                else:
-                                    seq.append("X")
-                            if counter != 0:  # aminoacids
-                                print("Your sequence is an aminoacid sequence")
-                            else:  # HETAM
-                                print("Your sequence is a HETAM sequence")
-                                for residue in chain:
-                                    seq.append(residue.get_resname())
-                        while seq[-1] == "X":
-                            del seq[-1]
-                        while seq[0] == "X":
-                            del seq[0]
-                        # return Seq(str(''.join(seq)), alphabet=alphabet)
-                        return Seq(str(''.join(seq)))
-
-    def getFullID(self, model_id='0', chain_id=None):
-        """
-        assign a label to a sequence obtained from a PDB file
-        :parameter
-        model_id
-        chain_id
-        :return: string with label
-        """
-        self.checkRead()  # cehck we have read the structure
-        label = "%s" % self.structure.get_id()  # PDB_ID
-        # check how many model are in sequence if > 1 add to id
-        models = self.getModelsChains()
-        if len(models) > 1:
-            label = label + "__%s" % str(model_id)
-        # if chain_id is None do not add it to te name
-        if chain_id is not None:
-            label = label + "_%s" % str(chain_id)
-        return label
-
-    def readLowLevel(self, fileName):
-        """ Return a dictionary with all mmcif fields. you should parse them
-            Example: get the list of the y coordinates of all atoms
-              dict = readLowLevel("kk.pdb")
-              y_list = dict['_atom_site.Cartn_y']
+                    print(pwutils.yellowStr("WARNING: Movie %s has empty alignment "
+                                            "data, can't add it to output set."
+                                            % movie.getFileName()))
+
+            # Warn about any exception creating the movie
+            except Exception as e:
+                print(pwutils.redStr("ERROR: Movie %s couldn't be "
+                                     "added to the output set.\n%s"
+                                     % (movie.getFileName(), e)))
+
+        self._updateOutputSet(OUT_MOVIES, movieSet, streamMode)
+
+        if self._firstTimeOutput:
+            # Probably is a good idea to store a cached summary for the
+            # first resulting movie of the processing.
+            self._storeSummary(newDone[0])
+            # If the movies are not written out, then dimensions can be
+            # copied from the input movies
+            if not saveMovie:
+                movieSet.setDim(self.inputMovies.get().getDim())
+            self._defineTransformRelation(self.inputMovies, movieSet)
+
+    def _updateOutputSets(self, newDone, streamMode):
+        if self._createOutputMovies():
+            self._updateOutputMovieSet(newDone, streamMode)
+
+        if self._createOutputMicrographs():
+            self._updateOutputMicSet(newDone, 'micrographs.sqlite',
+                                self._getOutputMicName,
+                                OUT_MICS, streamMode)
+
+        if self._createOutputWeightedMicrographs():
+            self._updateOutputMicSet(newDone, 'micrographs_dose-weighted.sqlite',
+                                self._getOutputMicWtName,
+                                OUT_MICS_DW, streamMode)
+
+        if self._doSplitEvenOdd():
+            self._updateOutputMicSet(newDone, 'micrographs_even.sqlite',
+                                self._getOutputMicEvenName,
+                                OUT_MICS_EVEN, streamMode)
+            self._updateOutputMicSet(newDone, 'micrographs_odd.sqlite',
+                                self._getOutputMicOddName,
+                                OUT_MICS_ODD, streamMode)
+
+    def _checkNewOutput(self):
+        if getattr(self, 'finished', False):
+            return
+
+        # Load previously done items (from text file)
+        doneList = self._readDoneList()
+        # Check for newly done items
+        newDone = [m for m in self.listOfMovies
+                   if m.getObjId() not in doneList and self._isMovieDone(m)]
+
+        # Update the file with the newly done movies
+        # or exit from the function if no new done movies
+        self.debug('_checkNewOutput: ')
+        self.debug('   listOfMovies: %s, doneList: %s, newDone: %s'
+                   % (len(self.listOfMovies), len(doneList), len(newDone)))
+
+        self._firstTimeOutput = len(doneList) == 0
+        allDone = len(doneList) + len(newDone)
+        # We have finished when there is not more input movies (stream closed)
+        # and the number of processed movies is equal to the number of inputs
+        self.finished = self.streamClosed and allDone == len(self.listOfMovies)
+        streamMode = pwobj.Set.STREAM_CLOSED if self.finished else pwobj.Set.STREAM_OPEN
+
+        if newDone:
+            self._writeDoneList(newDone)
+
+        elif not self.finished:
+            # If we are not finished and no new output have been produced
+            # it does not make sense to proceed and updated the outputs
+            # so we exit from the function here
+            return
+
+        self.debug('   finished: %s ' % self.finished)
+        self.debug('        self.streamClosed (%s) AND' % self.streamClosed)
+        self.debug('        allDone (%s) == len(self.listOfMovies (%s)'
+                   % (allDone, len(self.listOfMovies)))
+        self.debug('   streamMode: %s' % streamMode)
+
+        self._updateOutputSets(newDone, streamMode)
+
+        if self.finished:  # Unlock createOutputStep if finished all jobs
+            outputStep = self._getFirstJoinStep()
+            if outputStep and outputStep.isWaiting():
+                outputStep.setStatus(pwcts.STATUS_NEW)
+
+    # --------------------------- INFO functions ------------------------------
+    def _validate(self):
+        errors = []
+
+        # Only validate about cropDimensions if the protocol supports them
+        if (hasattr(self, 'cropDimX') and hasattr(self, 'cropDimY')
+                and (self.cropDimX > 0 >= self.cropDimY
+                     or self.cropDimX <= 0 < self.cropDimY)):
+            errors.append("If you give cropDimX, you should also give "
+                          "cropDimY and vice versa")
+
+        inputMovies = self.inputMovies.get()
+
+        # Do not continue if there ar no movies. Validation message will
+        # take place since attribute is a Pointer.
+        if inputMovies is None:
+            return errors
+
+        firstItem = inputMovies.getFirstItem()
+
+        firstFrame, lastFrame, _ = inputMovies.getFramesRange()
+        if lastFrame == 0:
+            # Although getFirstItem is not recommended in general, here it is
+            # used only once, for validation purposes, so performance
+            # problems should not appear.
+            frames = firstItem.getNumberOfFrames()
+            lastFrame = frames
+        else:
+            frames = lastFrame - firstFrame + 1
+
+        if frames is not None:
+            def _validateRange(prefix):
+                # Avoid validation when the range is not defined
+                if not hasattr(self, '%sFrame0' % prefix):
+                    return
+
+                f0, fN = self._getFrameRange(frames, prefix)
+                if fN < firstFrame or fN > lastFrame:
+                    errors.append("Check the selected last frame to *%s*. "
+                                  "Last frame (%d) should be in range: %s "
+                                  % (prefix.upper(), fN, (firstFrame,
+                                                          lastFrame)))
+                if f0 < firstFrame or f0 > lastFrame:
+                    errors.append("Check the selected first frame to *%s*. "
+                                  "First frame (%d) should be in range: %s "
+                                  % (prefix.upper(), f0, (firstFrame,
+                                                          lastFrame)))
+                if fN < f0:
+                    errors.append("Check the selected frames range to *%s*. "
+                                  "Last frame (%d) should be greater or equal "
+                                  "than first frame (%d)"
+                                  % (prefix.upper(), fN, f0))
+
+            _validateRange("align")
+            _validateRange("sum")
+
+        if not emlib.image.ImageHandler().existsLocation(firstItem.getLocation()):
+            errors.append("The input movie files do not exist!!! "
+                          "Since usually input movie files are symbolic links, "
+                          "please check that links are not broken if you "
+                          "moved the project folder. ")
+
+        return errors
+
+    # --------------------------- INFO functions -------------------------------
+    def _summary(self):
+        return [self.summaryVar.get('')]
+
+    # --------------------------- UTILS functions ----------------------------
+    def _doSplitEvenOdd(self):
+        """ Returns if even/odd stuff has to be done"""
+        if not self.evenOddCapable:
+            return False
+        else:
+            return self.splitEvenOdd.get()
+
+    def _useAlignToSum(self):
+        return self.getAttributeValue('useAlignToSum', False)
+
+    def _getFrameRange(self, n, prefix):
+        """
+        Params:
+        :param n: Number of frames of the movies
+        :param prefix: what range we want to consider, either 'align' or 'sum'
+        :return: (i, f) initial and last frame range
+        """
+        # In case that the user select the same range for ALIGN and SUM
+        # we also use the 'align' prefix
+        if self._useAlignToSum():
+            prefix = 'align'
+
+        first = self.getAttributeValue('%sFrame0' % prefix)
+        last = self.getAttributeValue('%sFrameN' % prefix)
+
+        if first <= 1:
+            first = 1
+
+        if last <= 0:
+            last = n
+
+        return first, last
+
+    def _createOutputMovie(self, movie):
+        # Parse the alignment parameters and store the log files
+        alignedMovie = movie.clone()
+        n = movie.getNumberOfFrames()
+        first, last = self._getFrameRange(n, 'align')
+        framesRange = alignedMovie.getFramesRange()
+        framesRange.setFirstFrame(first)
+        framesRange.setLastFrame(last)
+        # Check if user selected to save movie, use the getAttributeValue
+        # function for allow the protocol to not define this flag
+        # and use False as default
+        if self.getAttributeValue('doSaveMovie', False):
+            # The subclass protocol is responsible for generating the output
+            # movie file in the extra path with the required name
+            extraMovieFn = self._getExtraPath(self._getOutputMovieName(movie))
+            alignedMovie.setFileName(extraMovieFn)
+            # When the output movies are saved, the shifts
+            # will be set to zero since they are aligned
+            totalFrames = last - first + 1
+            xshifts = [0] * totalFrames
+            yshifts = xshifts
+            # If we save the movies, we need to modify which are the index
+            # of the first frame in the stack, now is 1 since the stack is
+            # written only with the given frames
+            firstFrameIndex = 1
+        else:
+            xshifts, yshifts = self._getMovieShifts(movie)
+            firstFrameIndex = first
+
+        framesRange.setFirstFrameIndex(firstFrameIndex)
+        alignment = emobj.MovieAlignment(first=first, last=last, xshifts=xshifts,
+                                         yshifts=yshifts)
+
+        roiList = [self.getAttributeValue(s, 0) for s in
+                   ['cropOffsetX', 'cropOffsetY', 'cropDimX', 'cropDimY']]
+        alignment.setRoi(roiList)
+        alignedMovie.setAlignment(alignment)
+
+        return alignedMovie
+
+    # ---------- Hook functions that need to be implemented in subclasses ------
+    def _getBinFactor(self):
+        return self.getAttributeValue('binFactor', 1.0)
+
+    def _getMovieRoot(self, movie):
+        # Try to use the 'original' fileName in case it is present
+        # the original could be different from the current filename if
+        # we are dealing with compressed movies (e.g., movie.mrc.bz2)
+        fn = movie.getAttributeValue('_originalFileName',
+                                     movie.getFileName())
+        # Remove the first extension
+        fnRoot = pwutils.removeBaseExt(fn)
+        # Check if there is a second extension
+        # (Assuming it is only a dot and 3 or 4 characters after it
+        # Do not perform this check if the file name is short
+        if len(fnRoot) > 5:
+            if fnRoot[-4] == '.' or fnRoot[-5] == '.':
+                fnRoot = pwutils.removeExt(fnRoot)
+
+        return fnRoot
+
+    def _getOutputMovieName(self, movie):
+        """ Returns the name of the output movie.
+        (relative to micFolder)
+        """
+        return self._getMovieRoot(movie) + '_aligned_movie.mrcs'
+
+    def _getOutputMicName(self, movie):
+        """ Returns the name of the output micrograph
+        (relative to micFolder)
+        """
+        return self._getMovieRoot(movie) + '_aligned_mic.mrc'
+
+    def _getOutputMicWtName(self, movie):
+        """ Returns the name of the output dose-weighted micrograph
+        (relative to micFolder)
+        """
+        return self._getMovieRoot(movie) + '_aligned_mic_DW.mrc'
+
+    def _getOutputMicEvenName(self, movie):
+        """ Returns the name of the output EVEN micrograph
+        (relative to micFolder)
+        """
+        return self._getMovieRoot(movie) + '_aligned_mic_EVN.mrc'
+
+    def _getOutputMicOddName(self, movie):
+        """ Returns the name of the output EVEN micrograph
+        (relative to micFolder)
+        """
+        return self._getMovieRoot(movie) + '_aligned_mic_ODD.mrc'
+
+    def _getOutputMicThumbnail(self, movie):
+        return self._getExtraPath(self._getMovieRoot(movie) + '_thumbnail.png')
+
+    def _getMovieShifts(self, movie):
+        """ Returns the x and y shifts for the alignment of this movie.
+         The shifts should refer to the original micrograph without any binning.
+         In case of a binning greater than 1, the shifts should be scaled.
+        """
+        return [], []
+
+    def _createOutputMovies(self):
+        """ Returns True if an output set of movies will be generated.
+        The most common case is to always generate output movies,
+        either with alignment only or the binary aligned movie files.
+        Subclasses can override this function to change this behavior.
         """
-
-        if fileName.endswith(".pdb"):
-            print("Low level access to PDB is not implemented")
-        else:
-            dict = MMCIF2Dict(fileName)
-        return dict
-
-    def _write(self, fileName):
-        """ Do not use this function use toPDB or toCIF, they take care of some
-        compatibiity issues"""
-        if fileName.endswith(".pdb") or fileName.endswith(".ent"):
-            if self.ioPDB is None:
-                self.ioPDB = PDBIO()
-            io = self.ioPDB
-        else:
-            if self.ioCIF is None:
-                self.ioCIF = scipionMMCIFIO()
-                # self.ioCIF = MMCIFIO()
-            io = self.ioCIF
-        io.set_structure(self.structure)
-        io.save(fileName)
-
-    def _writeLowLevel(self, fileName, dict):
-        """ write a dictionary as cif file
-        """
-
-        if fileName.endswith(".pdb"):
-            print("Low level access to PDB is not implemented")
-        else:
-            if self.ioCIF is None:
-                self.ioCIF = MMCIFIO()
-            io = self.ioCIF
-        io.set_dict(dict)
-        io.save(fileName)
-
-    def _intToChain(self, i, base=62):
-        """
-        int_to_chain(int,int) -> str
-        Converts a positive integer to a chain ID. Chain IDs include uppercase
-        characters, numbers, and optionally lowercase letters.
-        i = a positive integer to convert
-        base = the alphabet size to include. Typically 36 or 62.
-        """
-        if i < 0:
-            raise ValueError("positive integers only")
-        if base < 0 or 62 < base:
-            raise ValueError("Invalid base")
-
-        quot = int(i) // base
-        rem = i % base
-        if rem < 26:
-            letter = chr(ord("A") + rem)
-        elif rem < 36:
-            letter = str(rem - 26)
-        else:
-            letter = chr(ord("a") + rem - 36)
-        if quot == 0:
-            return letter
-        else:
-            return self._intToChain(quot - 1, base) + letter
-
-    def renameChains(self, structure):
-        """Renames chains to be one-letter chains
-
-        Existing one-letter chains will be kept.
-        Multi-letter chains will be truncated
-        or renamed to the next available letter of the alphabet.
-
-        If more than 62 chains are present in the structure,
-        raises an OutOfChainsError
-
-        Returns a map between new and old chain IDs, as well as modifying
-        the input structure
-
-        """
-        next_chain = 0  #
-        # single-letters stay the same
-        chainmap = {c.id: c.id
-                    for c in structure.get_chains() if len(c.id) == 1}
-        for o in structure.get_chains():
-            if len(o.id) != 1:
-                if o.id[0] not in chainmap:
-                    chainmap[o.id[0]] = o.id
-                    o.id = o.id[0]
-                else:
-                    c = self._intToChain(next_chain)
-                    while c in chainmap:
-                        next_chain += 1
-                        c = self._intToChain(next_chain)
-                        if next_chain >= 62:
-                            raise OutOfChainsError()
-                    chainmap[c] = o.id
-                    o.id = c
-        return chainmap
-
-    def write(self, fileName):
-        if fileName.endswith(".pdb") or fileName.endswith(".ent"):
-            self.writeAsPdb(fileName)
-        else:
-            self.writeAsCif(fileName)
-
-    def writeAsPdb(self, pdbFile):
-        """ Save structure as PDB. Be aware that this is not a lossless conversion
-        Returns False is conversion is not possible. True otherwise
-        """
-        # check input is not PDB
-        if self.type == self.PDB:
-            pass
-        else:
-            # rename long chains
-            try:
-                chainmap = self.renameChains(self.structure)
-            except OutOfChainsError:
-                print("Too many chains to represent in PDB format")
-                return False
-
-            for new, old in chainmap.items():
-                # for new, old in list(chainmap.items()):
-                if new != old:
-                    print("Renaming chain {0} to {1}".format(old, new))
-
-        self._write(pdbFile)
-
         return True
 
-    def writeAsCif(self, cifFile):
-        """ Save structure as CIF.
-            Be aware that this is not a lossless conversion
-        """
-        self._write(cifFile)
-
-    def centerOfMass(self, geometric=False):
-        """
-        Returns gravity [default] or geometric center of mass of an Entity
-        (anything with a get_atoms function in biopython.
-        Geometric assumes all masses are equal (geometric=True)
-        """
-        entity = self.structure
-        # Structure, Model, Chain, Residue
-        if isinstance(entity, Entity.Entity):
-            atom_list = entity.get_atoms()
-        # List of Atoms
-        elif hasattr(entity, '__iter__') and \
-                [x for x in entity if x.level == 'A']:
-            atom_list = entity
-        else:  # Some other weirdo object
-            raise ValueError("Center of Mass can only be calculated "
-                             "from the following objects:\n"
-                             "Structure, Model, Chain, Residue, "
-                             "list of Atoms.")
-
-        masses = []
-        positions = [[], [], []]
-
-        for atom in atom_list:
-            masses.append(atom.mass)
-
-            for i, coord in enumerate(atom.coord.tolist()):
-                positions[i].append(coord)
-
-        # If there is a single atom with undefined mass complain loudly.
-        if 'ukn' in set(masses) and not geometric:
-            raise ValueError("Some Atoms don't have an element assigned.\n"
-                             "Try adding them manually or calculate the "
-                             "geometrical center of mass instead.")
-
-        if geometric:
-            return [sum(coord_list) / len(masses) for coord_list in positions]
-        else:
-            w_pos = [[], [], []]
-            for atom_index, atom_mass in enumerate(masses):
-                w_pos[0].append(positions[0][atom_index] * atom_mass)
-                w_pos[1].append(positions[1][atom_index] * atom_mass)
-                w_pos[2].append(positions[2][atom_index] * atom_mass)
-
-            return [sum(coord_list) / sum(masses) for coord_list in w_pos]
-
-    def transform(self, transformation_matrix, sampling=1.):
-        """ Geometrical transformation of a PDB structure
-
-        :param entity: PDB biopython structure
-        :param transformation_matrix -> 4x4 scipion matrix
-        :param sampling: scipion transform matrix is applied to voxels so
-              length must be multiplied by samplingRate
-
-        internal variables:
-             rotation matrix -> numpy.array(
-                      [[ 0.5, -0.809017,  0.309017],
-                       [ 0.809017,  0.30917,  -0.5     ],
-                       [ 0.309017,  0.5,       0.809017]])
-             translation: translation vector -> numpy.array([1., 0., 0.], 'd')
-        :return: no return, new data overwrites entity
-        """
-        # bioPhython and Scipion conventions do not match
-        rotation_matrix = numpy.transpose(transformation_matrix[:3, :3])
-        # from geometry get euler angles and recreate matrix
-        translation = translation_from_matrix(transformation_matrix)
-        translation = [x * sampling for x in translation]
-        self.structure.transform(rotation_matrix, translation)
-
-    def _renameChainsIfNeed(self, struct2):
-        """Rename chain, we assume that there is a single model per structure"""
-        repeated = False
-
-        def RepresentsInt(s):
-            try:
-                int(s)
-                return True
-            except ValueError:
-                return False
-
-        import uuid
-        chainIDs1 = [chain.id for chain in self.structure.get_chains()]
-        for chain in struct2.get_chains():
-            counter = 2
-            if chain.id in chainIDs1:
-                repeated = True
-                cId = chain.id
-                l = len(cId)
-                if l == 1:
-                    while True:
-                        try:
-                            chain.id = "%s%03d" % (cId, counter)
-                            break
-                        except ValueError:
-                            counter +=1
-                            if counter > 1000:
-                                raise ValueError('Error in _renameChainsIfNeed.')
-                elif RepresentsInt(cId[1:]):  # try to fit a number and increase it by one
-                    chain.id = "%s%03d" % (cId[0], int(cId[1:]) + 1)
-                else:  # generate a 4 byte random string
-                    chain.id = uuid.uuid4().hex[:4]
-        if repeated:
-            self._renameChainsIfNeed(struct2)
-
-    def addStruct(self, secondPDBfileName, outPDBfileName=None, useModel=False):
-        """ Join the second structure to the first one.
-            If cheon numes are the same rename them.
-            if outPDBfileName id provided then new
-            struct is saved to a file"""
-        # read new structure
-        if outPDBfileName is not None:
-            pdbID = (os.path.splitext(os.path.basename(outPDBfileName))[0])[:4]
-        else:
-            pdbID = (os.path.splitext(os.path.basename(secondPDBfileName))[0])[:4]
-
-        if secondPDBfileName.endswith(".pdb") or secondPDBfileName.endswith(".ent"):
-            parser = PDBParser(PERMISSIVE=self.permissive)
-        else:
-            parser = MMCIFParser()
-
-        struct2 = parser.get_structure(pdbID, secondPDBfileName)
-
-        if useModel:
-            modelNumber = 0
-            modelID = 0
-            # model.id = model.serial_num = len(self.structure)?  # not sure this
-            # is valid always
-            for model in self.structure:
-                pass
-            modelNumber = model.serial_num
-            modelID = model.id
-            for model in struct2:
-                modelNumber += 1
-                modelID += 1
-                model.detach_parent()
-                model.serial_num = modelNumber
-                model.id = modelID
-                self.structure.add(model)
-        else:
-            self._renameChainsIfNeed(struct2)
-
-            for model in struct2:
-                for chain in model:
-                    chain.detach_parent()
-                    self.structure[0].add(chain)
-
-        # create new output file
-        if outPDBfileName is not None:
-            self.write(outPDBfileName)
-
-    def extractChain(self, chainID, start=0, end=-1,
-                     modelID='0', filename="output.mmcif"):
-        """Code for chopping  a structure.
-        This module is used internally by the Bio.PDB.extract() function.
-        """
-        sel = ChainSelector(chain_id=chainID, start=start,
-                            end=end, model_id=int(modelID))
-        io = scipionMMCIFIO()
-        io.set_structure(self.structure)
-        io.save(filename, sel)
-
-    def renameChain(self, chainID, newChainName, modelID='0',
-                    filename="output.mmcif"):
-        self.structure[modelID][chainID].id = newChainName
-        self.write(filename)
-
-    def renumberChain(self, chainID, offset=0, modelID='0',
-                      filename="output.mmcif"):
-        # get chain object
-        chain = self.structure[modelID][chainID]
-        # remove chain from model
-        self.structure[modelID].detach_child(chainID)
-        from Bio.PDB.Chain import Chain
-        # create new chain
-        newChain = Chain(chainID)
-        for residue in chain:
-            # remove residue, otherwise we cannot renumber it
-            residue.detach_parent()
-            rId = residue.id
-            res_id = list(rId)
-            res_id[1] = res_id[1] + offset
-            if res_id[1] < 0:
-                raise ValueError('Residue number cant be <= 0')
-            residue.id = tuple(res_id)
-            newChain.add(residue)
-        self.structure[modelID].add(newChain)
-        self.write(filename)
-
-
-def cifToPdb(fnCif, fnPdb):
-    h = AtomicStructHandler()
-    h.read(fnCif)
-    h.writeAsPdb(fnPdb)
-
-
-def pdbToCif(fnPdb, fnCif):
-    h = AtomicStructHandler()
-    h.read(fnPdb)
-    h.writeAsCif(fnCif)
-
-
-def toPdb(inFileName, outPDBFile):
-    if inFileName.endswith(".pdb") or inFileName.endswith(".ent"):
-        return inFileName
-    elif inFileName.endswith(".cif") or inFileName.endswith(".mmcif"):
-        cifToPdb(inFileName, outPDBFile)
-        return outPDBFile
-    else:
-        print("ERROR (toPdb), Unknown file type for file = %s" % inFileName)
-
-
-def toCIF(inFileName, outCIFFile):
-    if inFileName.endswith(".cif") or inFileName.endswith(".mmcif"):
-        return inFileName
-    elif inFileName.endswith(".pdb") or inFileName.endswith(".ent"):
-        pdbToCif(inFileName, outCIFFile)
-        return outCIFFile
-    else:
-        print("ERROR (toCIF), Unknown file type for file = %s" % inFileName)
-
-
-def getEnviron():
-    environ = pwutils.Environ(os.environ)
-    environ.update({'RCSBROOT': os.path.join(Plugin.getMaxitHome())
-                    }, position=pwutils.Environ.REPLACE)
-    environ.update({'PATH': os.path.join(Plugin.getMaxitHome(), 'bin')
-                    }, position=pwutils.Environ.BEGIN)
-    return environ
-
-
-def _frombase(inFileName, outFileName, log, oParam=1):
-    # check if maxit exists,
-    # if it does not then complain
-    # convert pdb to cif using maxit
-    global maxitAvailable
-    try:
-        maxitAvailable
-    except:
-        if not os.path.exists(Plugin.getMaxitBin()):
-            maxitAvailable = False
-            # show error message
-        else:
-            maxitAvailable = True
+    def _createOutputMicrographs(self):
+        """ By default check if the user have selected 'doSaveAveMic'
+        property. Subclasses can override this method to implement different
+        behaviour.
+        """
+        return self.getAttributeValue('doSaveAveMic', True)
+
+    def _createOutputWeightedMicrographs(self):
+        return False
+
+    def _preprocessOutputMicrograph(self, mic, movie):
+        """ Hook function that will be call before adding the micrograph
+        to the output set of micrographs.
+        """
+        pass
+
+    def _doComputeMicThumbnail(self):
+        """ Should be implemented in sub-classes if want to check
+        the generation of thumbnails.
+        """
+        return False
+
+    def _storeSummary(self, movie):
+        """ Implement this method if you want to store the summary. """
+        pass
+
+    def _getCorrectedDose(self, movieSet):
+        """get and correct the pre-exposure dose. It is important for cases
+        in which the first frame is different of one. The method support both
+        movie and sets of movies"""
+
+        firstFrame, _, _ = movieSet.getFramesRange()
+        preExp = movieSet.getAcquisition().getDoseInitial()
+        dose = movieSet.getAcquisition().getDosePerFrame()
+        preExp += dose * (firstFrame - 1)
+
+        return preExp, dose
+
+    def __runXmippProgram(self, program, args):
+        """ Internal shortcut function to launch a Xmipp program. """
+        from pwem import Domain
+        xmipp3 = Domain.importFromPlugin('xmipp3')
+        xmipp3.Plugin.runXmippProgram(program, args)
+
+    def __runEman2Program(self, program, args):
+        """ Internal workaround to launch an EMAN2 program. """
+        from pwem import Domain
+        eman2 = Domain.importFromPlugin('eman2')
+        from pyworkflow.utils.process import runJob
+        runJob(self._log, eman2.Plugin.getProgram(program), args,
+               env=eman2.Plugin.getEnviron())
+
+    def computePSD(self, inputMic, oroot, dim=384,  # 384 = 128 + 256, which should be fast for any Fourier Transformer
+                   overlap=0.4):
+        warnings.warn("Use psd = image.computePSD(overlap=0.4, xdim=384, ydim=384, fftthreads=1) instead",
+                      DeprecationWarning)
+        ih = emlib.image.ImageHandler()
+        psdImg1 = ih.read(inputMic)
+        res = psdImg1.computePSD(overlap, dim, dim)
+        res.write(oroot + ".psd")
+
+    def composePSDImages(self, psdImg1, psdImg2, outputFn,
+                         outputFnUncorrected=None, outputFnCorrected=None):
+        """ Compose a single PSD image:
+         left part from psd1 (uncorrected PSD),
+         right-part from psd2 (corrected PSD)
+        """
+        data1 = psdImg1.getData()  # get the data now, as conversion would change them
+        if outputFnUncorrected is not None:
+            psdImg1.convertPSD()
+            psdImg1.write(outputFnUncorrected)
+
+        data2 = psdImg2.getData()  # get the data now, as conversion would change them
+        if outputFnCorrected is not None:
+            psdImg2.convertPSD()
+            psdImg2.write(outputFnCorrected)
+
+        # Compute middle index
+        x, _, _, _ = psdImg1.getDimensions()
+        m = int(round(x / 2.))
+        data1[:, :m] = data2[:, :m]
+        psdImg1.setData(data1)
+        psdImg1.write(outputFn)
+
+    def composePSD(self, psd1, psd2, outputFn,
+                   outputFnUncorrected=None, outputFnCorrected=None):
+        import warnings
+        warnings.warn("Use composePSDImages() instead", DeprecationWarning)
+        """ Compose a single PSD image:
+         left part from psd1 (uncorrected PSD),
+         right-part from psd2 (corrected PSD)
+        """
+        ih = emlib.image.ImageHandler()
+        self.composePSDImages(ih.read(psd1), ih.read(psd2), outputFn,
+                              outputFnUncorrected, outputFnCorrected)
+
+    def computePSDImages(self, movie, fnUncorrected, fnCorrected,
+                         outputFnUncorrected=None, outputFnCorrected=None):
+        self.composePSDImages(
+            emlib.image.ImageHandler().read(fnUncorrected).computePSD(),
+            emlib.image.ImageHandler().read(fnCorrected).computePSD(),
+            self._getPsdCorr(movie),
+            outputFnUncorrected,
+            outputFnCorrected)
+
+    def computePSDs(self, movie, fnUncorrected, fnCorrected,
+                    outputFnUncorrected=None, outputFnCorrected=None):
+        import warnings
+        warnings.warn("Use computePSDImages() instead", DeprecationWarning)
+        self.computePSDImages(movie, fnUncorrected, fnCorrected,
+                              outputFnUncorrected, outputFnCorrected)
+
+    def computeThumbnail(self, inputFn, scaleFactor=6, outputFn=None):
+        """ Generates a thumbnail of the input file"""
+        outputFn = outputFn or self.getThumbnailFn(inputFn)
+        args = "%s %s " % (inputFn, outputFn)
+        args += "--meanshrink %s --fixintscaling=sane" % scaleFactor
+
+        self.__runEman2Program('e2proc2d.py', args)
+
+        return outputFn
+
+    def correctGain(self, movieFn, outputFn, gainFn=None, darkFn=None):
+        """correct a movie with both gain and dark images"""
+        ih = emlib.image.ImageHandler()
+        _, _, z, n = ih.getDimensions(movieFn)
+        numberOfFrames = max(z, n)  # in case of wrong mrc stacks as volumes
+
+        def _readImgFloat(fn):
+            img = None
+            if fn:
+                img = ih.read(fn)
+                img.convert2DataType(emlib.DT_FLOAT)
+            return img
+
+        gainImg = _readImgFloat(gainFn)
+        darkImg = _readImgFloat(darkFn)
+
+        img = ih.createImage()
+
+        for i in range(1, numberOfFrames + 1):
+            img.read((i, movieFn))
+            img.convert2DataType(emlib.DT_FLOAT)
+
+            if darkImg:
+                img.inplaceSubtract(darkImg)
+            if gainImg:
+                img.inplaceMultiply(gainImg)
+
+            img.write((i, outputFn))
+
+    def getThumbnailFn(self, inputFn):
+        """ Returns the default name for a thumbnail image"""
+        return pwutils.replaceExt(inputFn, "thumb.png")
+
+    def _getPsdCorr(self, movie):
+        """ This should be implemented in subclasses."""
+        pass
+
+    def _writeFailedList(self, movieList):
+        """ Write to a text file the items that have failed. """
+        with open(self._getAllFailed(), 'a') as f:
+            for movie in movieList:
+                f.write('%d\n' % movie.getObjId())
+
+    def _readFailedList(self):
+        """ Read from a text file the id's of the items that have failed. """
+        failedFile = self._getAllFailed()
+        failedList = []
+        if os.path.exists(failedFile):
+            with open(failedFile) as f:
+                failedList += [int(line.strip()) for line in f]
+
+        return failedList
+
+
+def createAlignmentPlot(meanX, meanY):
+    """ Create a plotter with the cumulative shift per frame. """
+    figureSize = (8, 6)
+    plotter = Plotter(*figureSize)
+    figure = plotter.getFigure()
+
+    ax = figure.add_subplot(111)
+    ax.grid()
+    ax.axis('equal')
+    ax.set_title('Cartesian representation')
+    ax.set_xlabel('Drift x (pixels)')
+    ax.set_ylabel('Drift y (pixels)')
+
+    # Max range of the plot of the two coordinates
+    plotRange = max(max(meanX) - min(meanX), max(meanY) - min(meanY))
+    i = 1
+    skipLabels = ceil(len(meanX) / 10.0)
+    for x, y in izip(meanX, meanY):
+        if i % skipLabels == 0:
+            ax.text(x - 0.02 * plotRange, y + 0.02 * plotRange, str(i))
+        i += 1
+
+    ax.plot(meanX, meanY, color='b')
+    ax.plot(meanX, meanY, 'yo')
+
+    # setting the plot windows to properly see the data
+    ax.axis([min(meanX) - 0.1 * plotRange, max(meanX) + 0.1 * plotRange,
+             min(meanY) - 0.1 * plotRange, max(meanY) + 0.1 * plotRange])
+
+    plotter.tightLayout()
+
+    return plotter
+
+
+class ProtAverageFrames(ProtAlignMovies):
+    """
+    Very simple protocol to align all the frames of a given data collection
+    session. It can be used as a sanity check.
+    """
+    _label = 'average frames'
+
+    # -------------------------- DEFINE param functions -----------------------
+    def _defineAlignmentParams(self, form):
+        pass
+
+    def _processMovie(self, movie):
+        allFramesSum = self._getPath('all_frames_sum.mrc')
+        ih = emlib.image.ImageHandler()
+        sumImg = ih.createImage()
+        img = ih.createImage()
+
+        n = movie.getNumberOfFrames()
+        fn = movie.getFileName()
+
+        sumImg.read((1, fn))
+
+        for frame in range(2, n + 1):
+            img.read((frame, fn))
+            sumImg.inplaceAdd(img)
+
+        if os.path.exists(allFramesSum):
+            img.read(allFramesSum)
+            sumImg.inplaceAdd(img)
+
+        sumImg.write(allFramesSum)
+
+    # FIXME: Methods will change when using the streaming for the output
+    def createOutputStep(self):
+        # Really load the input, since in the streaming case we can not
+        # use the self.inputMovies directly
+        allFramesSum = self._getPath('all_frames_sum.mrc')
+        allFramesAvg = self._getPath('all_frames_avg.mrc')
+        self._loadInputList()
+        n = len(self.listOfMovies)
+
+        ih = emlib.image.ImageHandler()
+        sumImg = ih.read(allFramesSum)
+        sumImg.inplaceDivide(float(n))
+        sumImg.write(allFramesAvg)
+
+        outputAvg = emobj.Image()
+        outputAvg.setFileName(allFramesAvg)
+        outputAvg.setSamplingRate(self.listOfMovies[0].getSamplingRate())
+        self._defineOutputs(outputAverage=outputAvg)
+        self._defineSourceRelation(self.inputMovies, outputAvg)
+
+    def _validate(self):
+        return []
+
+    def _summary(self):
+        return []
+
+    def _createOutputMovies(self):
+        """ Returns True if an output set of movies will be generated.
+        The most common case is to always generate output movies,
+        either with alignment only or the binary aligned movie files.
+        Subclasses can override this function to change this behavior.
+        """
+        return False
+
+    def _createOutputMicrographs(self):
+        """ By default check if the user have selected 'doSaveAveMic'
+        property. Subclasses can override this method to implement different
+        behaviour.
+        """
+        return False
 
-    if maxitAvailable:
-        args = ' -input "' + inFileName + '" -output "' + outFileName + \
-               '" -o %d' % oParam
-        log.info('Launching: ' + Plugin.getMaxitBin() + args)
-        # run in the background
-        env = getEnviron()
-        pwutils.runJob(None, Plugin.getMaxitBin(), args, env=env)
-    else:
-        # this is not the ideal conversion but it is better
-        # than nothing
-        aSH = AtomicStructHandler()
-        aSH.read(inFileName)
-        aSH.write(outFileName)
-        # show error message
-        print(pwutils.redStr("Please, install maxit with the command 'scipion installb maxit'"))
-        print(pwutils.redStr("and restart scipion. Packages bison and flex are needed."))
-        print(pwutils.redStr("If maxit is installed check %s in scipion.conf" % MAXIT_HOME))
-
-
-def fromPDBToCIF(inFileName, outFileName, log):
-    _frombase(inFileName, outFileName, log, 1)
-
-
-def fromCIFToPDB(inFileName, outFileName, log):
-    _frombase(inFileName, outFileName, log, 2)
-
-
-def fromCIFTommCIF(inFileName, outFileName, log):
-    _frombase(inFileName, outFileName, log, 8)
-
-
-def retry(runEnvirom, program, args, cwd, listAtomStruct=[], log=None, clean_dir=None):
-    try:
-        runEnvirom(program, args, cwd=cwd)
-    except:
-        # first remove every files or directories in the extra folder,
-        # except maps
-        partiallyCleaningFolder(program, cwd)
-        # something went wrong, may be bad atomStruct format
-        log.info('retry with maxit conversion')
-
-        for i, atomStructName in enumerate(listAtomStruct):
-            if atomStructName.endswith(".pdb.cif"):
-                aSH = AtomicStructHandler()
-                aSH.read(atomStructName)
-                aSH.write(atomStructName)
-
-                runEnvirom(program, args, cwd=cwd)
-            else:
-                try:
-                    if atomStructName.endswith(".pdb"):
-                        newAtomStructName = os.path.abspath(
-                            os.path.join(cwd, "retrypdb%d.cif" % i))
-                        fromPDBToCIF(atomStructName, newAtomStructName, log)
-                        _args = args.replace(atomStructName, newAtomStructName)
-                        try:
-                            runEnvirom(program, _args, cwd=cwd)
-                        except:
-                            fromCIFTommCIF(newAtomStructName, newAtomStructName, log)
-                            runEnvirom(program, _args, cwd=cwd)
-                    elif atomStructName.endswith(".cif"):
-                        newAtomStructName = os.path.abspath(
-                            os.path.join(cwd, "retrycif%d.cif" % i))
-                        fromCIFTommCIF(atomStructName, newAtomStructName, log)
-                        _args = args.replace(atomStructName, newAtomStructName)
-                        try:
-                            runEnvirom(program, _args, cwd=cwd)
-                        except:
-                            newAtomStructName = os.path.abspath(
-                                os.path.join(cwd, "retrycif%d.pdb" % i))
-                            fromCIFToPDB(atomStructName, newAtomStructName, log)
-                            _args = args.replace(atomStructName, newAtomStructName)
-                            runEnvirom(program, _args, cwd=cwd)
-                except:
-                    # first remove files or directories in the extra folder,
-                    # except maps
-                    partiallyCleaningFolder(program, cwd)
-                    # biopython conversion
-                    aSH = AtomicStructHandler()
-                    if atomStructName.endswith(".pdb") or atomStructName.endswith(".ent"):
-                        newAtomStructName = atomStructName.replace(".pdb", ".cif"). \
-                            replace(".ent", ".cif")
-                    else:
-                        newAtomStructName = atomStructName
-                    try:
-                        aSH.read(atomStructName)
-                        aSH.write(newAtomStructName)
-                        _args = args.replace(atomStructName, newAtomStructName)
-                        runEnvirom(program, _args, cwd=cwd)
-                    except:
-                        print("CIF file standardisation failed.")
-                        # atomStructName = newAtomStructName
-
-
-# TODO this should no be here, ROB
-def partiallyCleaningFolder(program, cwd):
-    l1 = os.listdir(cwd)
-    l2 = ['molprobity.out', 'molprobity_probe.txt', 'molprobity_coot.py']
-    l3 = ['validation_cryoem.pkl']
-    l4 = ['placed_model.pdb', 'placed_model.cif']
-
-    for item in l1:
-        if (program.endswith('real_space_refine.py') and
-            (item.endswith('geo') or
-             item.endswith('real_space_refined.log') or
-             item.endswith('real_space_refine.pdb') or
-             item.endswith('real_space_refined.cif'))) or \
-                (program.endswith('molprobity.py') and item in l2) or \
-                (program.endswith('validation_cryoem.py') and item in l3) or \
-                (program.endswith('emringer.py') and
-                 (item.endswith("emringer.csv") or
-                  item.endswith("emringer.pkl") or
-                  item.endswith("emringer_plots") or
-                  item.startswith('emringer_transfer'))) or \
-                (program.endswith('dock_in_map.py') and item in l4):
-            path1 = os.path.join(cwd, item)
-            if os.path.exists(path1):
-                if os.path.isfile(path1) or os.path.islink(path1):
-                    os.remove(path1)
-                elif os.path.isdir(path1):
-                    shutil.rmtree(path1)
+    def _createOutputWeightedMicrographs(self):
+        return False
```

### Comparing `scipion-em-3.0.9/pwem/convert/headers.py` & `scipion-em-3.1.0/pwem/convert/headers.py`

 * *Files 4% similar despite different names*

```diff
@@ -322,15 +322,15 @@
         self.isMovie = False
 
         if ext == '.mrcs':
             self.isMovie = True
         elif ext == '.mrc:mrcs':  # Movie --> dims = [X, Y, Z = 1, N]
             self.isMovie = True
             fileName = fileName.replace(':mrcs', '')
-        elif ext == '.mrc:mrc':  # Volume --> dims = [X, Y, Z, N = 1]
+        elif ext in ['.mrc:mrc', '.map:mrc']:  # Volume --> dims = [X, Y, Z, N = 1]
             fileName = fileName.replace(':mrc', '')
 
         return fileName
 
     @classmethod
     def fixFile(cls, inFileName, outFileName, scipionOriginShifts,
                 sampling=1.0, originField=START):
@@ -344,16 +344,47 @@
         if originField == cls.ORIGIN:
             ccp4header.setOrigin(scipionOriginShifts)
         else:
             ccp4header.setStartAngstrom(scipionOriginShifts, sampling)
 
         ccp4header.writeHeader()
 
+    @classmethod
+    def isCompatible(cls, file):
+        return getFileFormat(file) == MRC
+
 
 def getFileFormat(fileName):
     ext = getExt(fileName)
-    if ext in ['.mrc', '.map', '.mrcs', '.mrc:mrc', '.mrc:mrcs', '.st', '.rec']:
+    if ext in ['.mrc', '.map', '.mrcs', '.mrc:mrc', '.mrc:mrcs', '.st', '.rec', '.ali']:
         return MRC
     elif ext == '.spi' or ext == '.vol':
         return SPIDER
     else:
         return UNKNOWNFORMAT
+
+def fixVolume(paths):
+    """
+    Fixes mrc (any extension) files that are defined as stacks but are meant to be volumes as defined in the mrc 2014
+    specs. Setting ISPG to 1.
+    :param paths: accept a string or a list of strings
+    :return: nothing, but mrc files header end up being updated.
+    """
+    if isinstance(paths, str):
+        paths = [paths]
+    for path in paths:
+        ccp4header = Ccp4Header(path, readHeader=True)
+        ccp4header.setISPG(1)
+        ccp4header.writeHeader()
+
+def setMRCSamplingRate(paths, samplingRate):
+    """
+    Sets the mrc file sampling rate value
+    :param paths: accept a string or a list of strings
+    :return: nothing, but mrc files header end up being updated with the right sampling rate
+    """
+    if isinstance(paths, str):
+        paths = [paths]
+    for path in paths:
+        ccp4header = Ccp4Header(path, readHeader=True)
+        ccp4header.setSampling(samplingRate)
+        ccp4header.writeHeader()
```

### Comparing `scipion-em-3.0.9/pwem/convert/sequence.py` & `scipion-em-3.1.0/pwem/viewers/filehandlers.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,10 @@
-# -*- coding: utf-8 -*-
 # **************************************************************************
 # *
-# * Authors:     Marta Martinez (mmmtnez@cnb.csic.es)
-# *              Roberto Marabini (roberto@cnb.csic.es)
+# * Authors:     Pablo Conesa (pconesa@cnb.csic.es)
 # *
 # * Unidad de  Bioinformatica of Centro Nacional de Biotecnologia , CSIC
 # *
 # * This program is free software; you can redistribute it and/or modify
 # * it under the terms of the GNU General Public License as published by
 # * the Free Software Foundation; either version 3 of the License, or
 # * (at your option) any later version.
@@ -21,212 +19,219 @@
 # * Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA
 # * 02111-1307  USA
 # *
 # *  All comments concerning this program package may be sent to the
 # *  e-mail address 'scipion@cnb.csic.es'
 # *
 # **************************************************************************
-from urllib.error import URLError, HTTPError
-from urllib.request import urlopen
-
-
-# sequence related stuff
-SEQ_TYPE = ['aminoacids', 'nucleotides']
-SEQ_TYPE_AMINOACIDS = 0
-SEQ_TYPE_NUCLEOTIDES = 1
-IUPAC_PROTEIN_ALPHABET = ['Extended Protein', 'Protein']
-EXTENDED_PROTEIN_ALPHABET = 0
-PROTEIN_ALPHABET = 1
-IUPAC_NUCLEOTIDE_ALPHABET = ['Ambiguous DNA', 'Unambiguous DNA',
-                             'Extended DNA', 'Ambiguous RNA',
-                             'Unambiguous RNA']
-EXTENDED_DNA_ALPHABET = 0
-AMBIGOUS_DNA_ALPHABET = 1
-UNAMBIGOUS_DNA_ALPHABET = 2
-AMBIGOUS_RNA_ALPHABET = 3
-UNAMBIGOUS_RNA_ALPHABET = 4
-
-
-from Bio.Seq import Seq
-from Bio.Alphabet import IUPAC
-from Bio import Entrez, SeqIO
-import sys
-from Bio.SeqRecord import SeqRecord
-from Bio.Align.Applications import ClustalOmegaCommandline, MuscleCommandline
-from Bio import pairwise2
-
-
-class SequenceHandler:
-    def __init__(self, sequence=None,
-                 iUPACAlphabet=0,
-                 isAminoacid=True):
-
-        self.isAminoacid = isAminoacid
-        self.alphabet = indexToAlphabet(isAminoacid, iUPACAlphabet)
-
-        if sequence is not None:
-            # sequence = cleanSequence(self.alphabet, sequence)
-            self._sequence = Seq(sequence, alphabet=self.alphabet)
-        else:
-            self._sequence = None
-            # type(self._sequence):  <class 'Bio.Seq.Seq'>
-
-    def saveFile(self, fileName, seqID, sequence=None, name=None,
-                 seqDescription=None, type="fasta"):
-        if sequence is not None:
-            self._sequence = sequence
-        record = SeqRecord(self._sequence, id=seqID, name=name,
-                           description=seqDescription)
-        # type(record): < class 'Bio.SeqRecord.SeqRecord'>
-        with open(fileName, "w") as output_handle:
-            SeqIO.write(record, output_handle, type)
-
-    def downloadSeqFromFile(self, fileName, type="fasta"):
-        record = next(SeqIO.parse(fileName, type))
-        return record
-
-    def downloadSeqFromDatabase(self, seqID):
-        # see http://biopython.org/DIST/docs/api/Bio.SeqIO-module.html
-        # for format/databases
-        print("Connecting to database...")
-        seqID = str(seqID)
-        sys.stdout.flush()
-        counter = 1
-        retries = 5
-        record = None
-        error = ""
-        while counter <= retries:  # retry up to 5 times if server busy
-            try:
-                if self.isAminoacid:
-                    dataBase = 'UnitProt'
-                    url = "http://www.uniprot.org/uniprot/%s.xml"
-                    format = "uniprot-xml"
-                    handle = urlopen(url % seqID)
-                    print("URL", url % seqID)
-                else:
-                    dataBase = 'GeneBank'
-                    Entrez.email = "adam.richards@stat.duke.edu"
-                    format = "fasta"
-                    handle = Entrez.efetch(db="nucleotide", id=seqID,
-                                           rettype=format, retmode="text")
-
-                record = SeqIO.read(handle, format)
-                break
-            except HTTPError as e:
-                error = "%s is a wrong sequence ID" % seqID
-                print(e.code)
-            except URLError as e:
-                error = "Cannot connect to %s" % dataBase
-                print(e.args)
-            except Exception as ex:
-                template = "An exception of type {0} occurred. Arguments:\n{1!r}"
-                message = template.format(type(ex).__name__, ex.args)
-                error = message
-            if counter == retries:
+"""
+This modules contains file handlers to be registered in the scipion file browser
+"""
+import os
+
+import pwem
+import pyworkflow.utils as pwutils
+from pwem.convert import Ccp4Header
+from pyworkflow import gui
+from pyworkflow.gui.browser import FileHandler, isStandardImage
+
+from pwem import emlib
+
+
+class ImageFileHandler(FileHandler):
+    _image = emlib.Image()
+    _index = ''
+
+    def _getImageString(self, filename):
+        if isStandardImage(filename):
+            return "Image file."
+        x, y, z, n = emlib.getImageSize(filename)
+        objType = 'Image'
+        objFileType = "link" if os.path.islink(filename) else "file"
+        dimMsg = "*%(objType)s %(objFileType)s*\n  dimensions: %(x)d x %(y)d"
+        expMsg = "Columns x Rows "
+        if z > 1:
+            dimMsg += " x %(z)d"
+            expMsg += " x Slices"
+            objType = 'Volume'
+        if n > 1:
+            dimMsg += " x %(n)d"
+            expMsg += " x Objects"
+            objType = 'Stack'
+
+        if Ccp4Header.isCompatible(filename):
+            ccp4Reader= Ccp4Header(filename, readHeader=True)
+            expMsg += "\nHeader info: \nSampling rate: %1.2f, %1.2f, %1.2f" % ccp4Reader.getSampling()
+            expMsg += "\nOrigin: %1.2f, %1.2f, %1.2f" % ccp4Reader.getOrigin()
+
+
+        return (dimMsg + "\n" + expMsg) % locals()
+
+    def _getImagePreview(self, filename):
+
+        # If file size if big
+        if pwutils.getFileSize(filename) > (pwem.Config.MAX_PREVIEW_FILE_SIZE * 1024*1024):
+            return
+
+        dim = 128
+
+        if isStandardImage(filename):
+            self.tkImg = gui.getImage(os.path.abspath(filename),
+                                      tkImage=True, maxheight=dim)
+        else:
+            fn = self._index + filename
+            self.tkImg = getTkImage(self._image, fn, dim)
+
+        return self.tkImg
+
+    def getFilePreview(self, objFile):
+        fn = objFile.getPath()
+        return self._getImagePreview(fn), self._getImageString(fn)
+
+    def getFileActions(self, objFile):
+        from .views import DataView
+        fn = objFile.getPath()
+        return [('Open with Xmipp viewer', lambda: DataView(fn).show(),
+                 pwutils.Icon.ACTION_VISUALIZE)]
+
+
+class ParticleFileHandler(ImageFileHandler):
+    def getFileIcon(self, objFile):
+        return 'file_image.gif' if not objFile.isLink() else 'file_image_link.gif'
+
+
+class VolFileHandler(ImageFileHandler):
+    def getFileIcon(self, objFile):
+        return 'file_vol.gif'
+
+class StackHandler(ImageFileHandler):
+    _index = '1@'
+
+    def getFileIcon(self, objFile):
+        return 'file_stack.gif' if not objFile.isLink() else 'file_stack_link.gif'
+
+
+class ChimeraHandler(FileHandler):
+
+    def getFileActions(self, objFile):
+        from .viewer_chimera import ChimeraView
+        fn = objFile.getPath()
+        return [('Open with Chimera', lambda: ChimeraView(fn).show(),
+                 pwutils.Icon.ACTION_VISUALIZE)]
+
+    def getFileIcon(self, objFile):
+        return 'file_text.gif'
+
+
+class MdFileHandler(ImageFileHandler):
+    def getFileIcon(self, objFile):
+        if objFile.isLink():
+            return 'file_md_link.gif'
+        else:
+            return 'file_md.gif'
+
+    def _getImgPath(self, mdFn, imgFn):
+        """ Get ups and ups until finding the relative location to images. """
+        path = os.path.dirname(mdFn)
+        index, fn = emlib.FileName(imgFn).decompose()
+
+        while path and path != '/':
+            newFn = os.path.join(path, fn)
+            if os.path.exists(newFn):
+                if index:
+                    newFn = '%d@%s' % (index, newFn)
+                return newFn
+            path = os.path.dirname(path)
+
+        return None
+
+    def _getMdString(self, filename, block=None):
+        md = emlib.MetaData()
+        if block:
+            md.read(block + '@' + filename)
+        else:
+            md.read(filename, 1)
+        labels = md.getActiveLabels()
+        msg = "Metadata items: *%d*\n" % md.getParsedLines()
+        msg += "Metadata labels: " + ''.join(
+            ["\n   - %s" % emlib.label2Str(l)
+             for l in labels])
+
+        imgPath = None
+        for label in labels:
+            if emlib.labelIsImage(label):
+                imgPath = self._getImgPath(filename,
+                                           md.getValue(label, md.firstObject()))
+                if imgPath is None or not os.path.exists(imgPath):
+                    imgPath = None
                 break
-            counter += 1
-        return record, error
-
-    def alignSeq(self, referenceSeq):
-        if self._sequence is not None:
-            alignments = pairwise2.align.globalds(self._sequence.seq,
-                                                  referenceSeq.seq)
-            return alignments
-        else:
-            print("read the sequence first")
-            exit(0)
-
-
-def sequenceLength(filename, format='fasta'):
-    handler = SequenceHandler()
-    return len(handler.downloadSeqFromFile(filename, format))
-
 
-def cleanSequenceScipion(isAminoacid, iUPACAlphabet, sequence):
-    return cleanSequence(indexToAlphabet(isAminoacid, iUPACAlphabet), sequence)
-
-
-def cleanSequence(alphabet, sequence):
-    str_list = []
-    for item in sequence.upper():
-        if item in alphabet.letters:
-            str_list.append(item)
-    value = ''.join(str_list)
-    return ''.join(str_list)
-
-
-def indexToAlphabet(isAminoacid, iUPACAlphabet):
-    if isAminoacid:
-        if iUPACAlphabet == EXTENDED_PROTEIN_ALPHABET:
-            alphabet = IUPAC.ExtendedIUPACProtein
-        else:
-            alphabet = IUPAC.IUPACProtein
-    else:
-        if iUPACAlphabet == EXTENDED_DNA_ALPHABET:
-            alphabet = IUPAC.ExtendedIUPACDNA
-        elif iUPACAlphabet == AMBIGOUS_DNA_ALPHABET:
-            alphabet = IUPAC.IUPACAmbiguousDNA
-        elif iUPACAlphabet == UNAMBIGOUS_DNA_ALPHABET:
-            alphabet = IUPAC.IUPACUnambiguousDNA
-        elif iUPACAlphabet == AMBIGOUS_RNA_ALPHABET:
-            alphabet = IUPAC.IUPACAmbiguousRNA
-        else:
-            alphabet = IUPAC.IUPACUnambiguousRNA
-    return alphabet
-
-
-def alphabetToIndex(isAminoacid, alphabet):
-    if isAminoacid:
-        if isinstance(alphabet, IUPAC.ExtendedIUPACProtein):
-            return EXTENDED_PROTEIN_ALPHABET
-        else:
-            return PROTEIN_ALPHABET
-    else:
-        if isinstance(alphabet, IUPAC.ExtendedIUPACDNA):
-            return EXTENDED_DNA_ALPHABET
-        elif isinstance(alphabet, IUPAC.IUPACAmbiguousDNA):
-            return AMBIGOUS_DNA_ALPHABET
-        elif isinstance(alphabet, IUPAC.IUPACUnambiguousDNA):
-            return UNAMBIGOUS_DNA_ALPHABET
-        elif isinstance(alphabet, IUPAC.IUPACAmbiguousRNA):
-            return AMBIGOUS_RNA_ALPHABET
-        else:
-            return UNAMBIGOUS_RNA_ALPHABET
+        # If there is an image and is not too big
+        if imgPath and pwutils.getFileSize(imgPath) < (pwem.Config.MAX_PREVIEW_FILE_SIZE * 1024*1024):
 
+            self._imgPreview = self._getImagePreview(imgPath)
+            self._imgInfo = self._getImageString(imgPath)
+        return msg
+
+    def getFilePreview(self, objFile):
+        self._imgPreview = None
+        self._imgInfo = None
+        filename = objFile.getPath()
+        ext = pwutils.getExt(filename)
+
+        if ext == '.xmd' or ext == '.ctfparam' or ext == '.pos' or ext == '.doc':
+            msg = "*Metadata File* "
+            blocks = emlib.getBlocksInMetaDataFile(filename)
+            nblocks = len(blocks)
+            if nblocks <= 1:
+                mdStr = self._getMdString(filename)
+                msg += "  (single block)\n"
+                if self._imgInfo:
+                    msg += "\nFirst item: \n" + self._imgInfo
+                msg += '\n' + mdStr
+            else:
+                mdStr = self._getMdString(filename, blocks[0])
+                msg += "  (%d blocks) " % nblocks
+                if self._imgInfo:
+                    msg += "\nFirst item: \n" + self._imgInfo
+                msg += "\nFirst block: \n" + mdStr
+                msg += "\nAll blocks:" + ''.join(
+                    ["\n  - %s" % b for b in blocks])
+        elif ext == '.star':
+            msg = "*Relion STAR file* \n"
+            msg += self._getMdString(filename)
+
+        return self._imgPreview, msg
+
+
+# Image methods for filehandlers
+def getPILImage(imageXmipp, dim=None, normalize=True):
+    """ Given an image read by Xmipp, convert it to PIL. """
+    from PIL import Image
+
+    if normalize:
+        imageXmipp.convert2DataType(emlib.DT_UCHAR, emlib.CW_ADJUST)
+
+    imageData = imageXmipp.getData()
+    image = Image.fromarray(imageData)
+    if dim:
+        size = int(dim), int(dim)
+        image.thumbnail(size, Image.ANTIALIAS)
+    return image
+
+
+def getTkImage(imageXmipp, filename, dim):
+    from PIL import ImageTk
+    imageXmipp.readPreview(filename, dim)
+    return ImageTk.PhotoImage(getPILImage(imageXmipp))
+
+
+def getImageFromPath(imagePath):
+    """ Read an image using Xmipp, convert to PIL
+    and then return as expected by Tk.
+    """
+    img = emlib.Image(imagePath)
+    imgPIL = getPILImage(img)
+    from PIL import ImageTk
+    imgTk = ImageTk.PhotoImage(imgPIL)
 
-def saveFileSequencesToAlign(SeqDic, inFile, type="fasta"):
-    # Write my sequences to a fasta file
-    with open(inFile, "w") as output_handle:
-        for index, seq in SeqDic.items():
-            record = SeqRecord(seq, id=str(index),
-                               name="", description="")
-            SeqIO.write(record, output_handle, type)
-
-
-def alignClustalSequences(inFile, outFile):
-    # Alignment of sequences with Clustal Omega program
-    clustalomega_cline = ClustalOmegaCommandline(
-            infile=inFile,
-            outfile=outFile,
-            verbose=True, auto=True)
-    return clustalomega_cline
-
-
-def alignMuscleSequences(inFile, outFile):
-    # Alignment of sequences with Muscle program
-    muscle_cline = MuscleCommandline(input=inFile, out=outFile)
-    return muscle_cline
-
-
-def alignBioPairwise2Sequences(structureSequenceId, structureSequence,
-                               userSequenceId, userSequence,
-                               outFileName):
-    """aligns two sequences and saves them to disk using fasta format"""
-    # see alignment_function for globalms parameters
-    alignments = pairwise2.align.globalms(structureSequence,
-                                          userSequence,  3, -1, -3, -2)
-    align1, align2, score, begin, end = alignments[0]
-    with open(outFileName, "w") as handle:
-        handle.write(">%s\n%s\n>%s\n%s\n" % (structureSequenceId,
-                                             align1,
-                                             userSequenceId,
-                                             align2))
+    return imgTk
```

### Comparing `scipion-em-3.0.9/pwem/convert/transformations.py` & `scipion-em-3.1.0/pwem/convert/transformations.py`

 * *Files 0% similar despite different names*

```diff
@@ -182,15 +182,16 @@
 >>> M = rotation_matrix(angle_between_vectors(v0, v1), vector_product(v0, v1))
 >>> v2 = np.dot(v0, M[:3,:3].T)
 >>> np.allclose(unit_vector(v1), unit_vector(v2))
 True
 
 """
 
-import math, sys
+import math
+import sys
 
 import numpy as np
 
 __version__ = '2013.06.29'
 __docformat__ = 'restructuredtext en'
 __all__ = []
 
@@ -361,19 +362,22 @@
     if not len(i):
         raise ValueError("no unit eigenvector corresponding to eigenvalue 1")
     point = np.real(Q[:, i[-1]]).squeeze()
     point /= point[3]
     # rotation angle depending on direction
     cosa = (np.trace(R33) - 1.0) / 2.0
     if abs(direction[2]) > 1e-8:
-        sina = (R[1, 0] + (cosa - 1.0) * direction[0] * direction[1]) / direction[2]
+        sina = (R[1, 0] + (cosa - 1.0) * direction[0] * direction[1]) /\
+             direction[2]
     elif abs(direction[1]) > 1e-8:
-        sina = (R[0, 2] + (cosa - 1.0) * direction[0] * direction[2]) / direction[1]
+        sina = (R[0, 2] + (cosa - 1.0) * direction[0] * direction[2]) /\
+            direction[1]
     else:
-        sina = (R[2, 1] + (cosa - 1.0) * direction[1] * direction[2]) / direction[0]
+        sina = (R[2, 1] + (cosa - 1.0) * direction[1] * direction[2]) /\
+            direction[0]
     angle = math.atan2(sina, cosa)
     return angle, direction, point
 
 
 def scale_matrix(factor, origin=None, direction=None):
     """Return matrix to scale by factor around origin in direction.
 
@@ -1446,59 +1450,66 @@
         return q0
     isin = 1.0 / math.sin(angle)
     q0 *= math.sin((1.0 - fraction) * angle) * isin
     q1 *= math.sin(fraction * angle) * isin
     q0 += q1
     return q0
 
+
 def quaternion_distance(q1, q2):
     '''Return distance between two quaternions'''
     q = q1 - q2
     module2_q = q[0] ** 2 + np.linalg.norm(q[1:]) ** 2
     dist = 2 * np.arccos(1 - module2_q / 2)
     return dist
 
+
 def weighted_tensor(tuple_q):
     '''Compute the Tensor as needed for the mean of quaterniones'''
     T = np.zeros((4, 4))
     w_i = 1 / len(tuple_q)
     for q in tuple_q:
         T += w_i * q.reshape(-1, 1).dot(q.reshape(1, -1))
     return T
 
+
 def normalized_Principal_Eigenvector(T, q_bar):
     '''Normalize the principal eigenvector o a tensor given a quaternion'''
     new_q_bar = T.dot(q_bar.reshape(-1, 1))
     new_q_bar /= np.linalg.norm(new_q_bar)
     return new_q_bar.reshape(-1)
 
+
 def mean_quaternion(T, q_bar_0=None, tol=1e-3):
     '''Compute the mean of a series of quaternions given a weighted Tensor'''
-    if q_bar_0 == None:
+    if q_bar_0 is None:
         q_bar_0 = random_quaternion()
     cost = sys.maxsize
     while (cost > tol):
         q_bar_f = normalized_Principal_Eigenvector(T, q_bar_0)
         cost = quaternion_distance(q_bar_f, q_bar_0)
         q_bar_0 = q_bar_f
     return q_bar_f, cost
 
+
 def listQuaternions(matrices):
     '''Convert a list of transformations matrices into a list of quaternions'''
     quaternions = [quaternion_from_matrix(matrix) for matrix in matrices]
     return np.asarray(quaternions)
 
+
 def qDistMatrix(Q1, Q2):
     '''Returns a Distance matrix from two list of quaternions'''
     ids_1 = range(0, Q1.shape[0])
     ids_2 = range(0, Q2.shape[0])
     dist = [[quaternion_distance(Q1[id_1, :], Q2[id_2, :])
             for id_2 in ids_2] for id_1 in ids_1]
     return np.asarray(dist)
 
+
 def random_quaternion(rand=None):
     """Return uniform random unit quaternion.
 
     rand: array like or None
         Three independent random variables that are uniformly distributed
         between 0 and 1.
```

### Comparing `scipion-em-3.0.9/pwem/convert/utils.py` & `scipion-em-3.1.0/pwem/convert/utils.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.0.9/pwem/emlib/__init__.py` & `scipion-em-3.1.0/pwem/emlib/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.0.9/pwem/emlib/_libNone.py` & `scipion-em-3.1.0/pwem/emlib/_libNone.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,16 +56,18 @@
 
             print("Xmipp bindings registered in Scipion. You will need to restart.")
 
         if os.path.abspath(pw.Config.getLibFolder()) not in os.environ.get("LD_LIBRARY_PATH", ""):
             print("LD_LIBRARY_PATH must contain scipion lib folder (%s).  Please, add it." % os.path.abspath(
                 pw.Config.getLibFolder()))
 
+cancelWarning = os.environ.get("SCIPION_CANCEL_XMIPP_BINDING_WARNING", False)
 
-print(ghostStr)
+if (not cancelWarning) and pw.Config.isScipionRunning():
+    print(ghostStr)
 
 linkXmippBinding()
 
 GHOST_ACTIVATED = True  # Flag to unequivocal identify the Ghost
 
 DT_DEFAULT = None
 DT_UNKNOWN = None
```

### Comparing `scipion-em-3.0.9/pwem/emlib/image/__init__.py` & `scipion-em-3.1.0/pwem/emlib/image/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.0.9/pwem/emlib/image/image_handler.py` & `scipion-em-3.1.0/pwem/emlib/image/image_handler.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,20 +24,21 @@
 # *
 # **************************************************************************
 
 import os
 
 import numpy
 from PIL import Image
+from tifffile import TiffFile
+
 import pyworkflow.utils as pwutils
 import pwem.objects as emobj
 import pwem.constants as emcts
 from .. import lib
 
-
 class ImageHandler(object):
     """ Class to provide several Image manipulation utilities. """
 
     # TODO: remove dependency from Xmipp
 
     def __init__(self):
         # Now it will use Xmipp image library
@@ -252,14 +253,20 @@
                 # or recent .img format
                 # we are opening an Eman2 process to read the dm4 file
                 from pwem import Domain
                 getImageDimensions = Domain.importFromPlugin(
                     'eman2.convert', 'getImageDimensions',
                     doRaise=True)
                 return getImageDimensions(fn)  # we are ignoring index here
+            elif ext in ['.eer', '.gain']:
+                tif = TiffFile(fn)
+                frames = len(tif.pages)  # number of pages in the file
+                page = tif.pages[0]  # get shape and dtype of the image in the first page
+                x, y = page.shape
+                return x, y, frames, 1
             else:
                 self._img.read(location, lib.HEADER)
                 return self._img.getDimensions()
         else:
             return None, None, None, None
 
     def getDataType(self, locationObj):
@@ -371,14 +378,23 @@
         The mask will be stored in 'outputFile'
         """
         inputRef = self.locationToXmipp(refImage)
         self.__runXmippProgram('xmipp_transform_mask',
                                '-i %s --create_mask  %s --mask circular -%d'
                                % (inputRef, outputFile, radius))
 
+    def rotateVolume(self, inputFile, outputFile, transformation):
+        """ Apply geometric transformations to images. You can shift, rotate
+        and scale a group of images/volumes.
+        """
+        elementList = [str(item) for item in transformation.getRotationMatrix().flatten().tolist()]
+        unrolledMatrix = ' '.join(elementList)
+        self.__runXmippProgram('xmipp_transform_geometry',
+                               '-i %s -o %s --rotate_volume matrix %s' % (inputFile, outputFile, unrolledMatrix))
+
     def addNoise(self, inputFile, outputFile, std=1., avg=0.):
         """ Add Gaussian noise to an input image (or stack)
         to produce noisy images.
         Params:
             inputFile: the filename of the input images
             outputFile: the filename of the output noisy images
             noiseStd: standard deviation for the Gaussian noise.
@@ -420,15 +436,19 @@
         lib.createEmptyFile(fnOut, xDim, yDim, zDim, nDim, dt)
 
     @classmethod
     def isImageFile(cls, imgFn):
         """ Check if imgFn has an image extension. The function
         is implemented in the Xmipp binding.
         """
-        return lib.FileName(imgFn).isImage()
+        # Local import to avoid import loop between ImageHandler and Ccp4Header.
+        from pwem.convert import headers
+
+        return (lib.FileName(imgFn).isImage() or
+                headers.getFileFormat(imgFn) == headers.MRC)
 
     def computeThumbnail(self, inputFn, outputFn, scaleFactor=6, flipOnY=False,
                          flipOnX=False):
         """ Compute a thumbnail of inputFn, save to ouptutFn.
         Optionally choose a scale factor eg scaleFactor=6 will make
         a thumbnail 6 times smaller.
         """
```

### Comparing `scipion-em-3.0.9/pwem/emlib/lib.py` & `scipion-em-3.1.0/pwem/emlib/lib.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.0.9/pwem/emlib/metadata/__init__.py` & `scipion-em-3.1.0/pwem/emlib/metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.0.9/pwem/emlib/metadata/utils.py` & `scipion-em-3.1.0/pwem/emlib/metadata/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -86,38 +86,43 @@
 
     def getValueAsObject(self, label, default=None):
         """ Same as getValue, but making an Object wrapping. """
         return ObjectWrap(self.getValue(label, default))
 
     def readFromMd(self, md, objId):
         """ Get all row values from a given id of a metadata. """
-        self._labelDict.clear()
         self._objId = objId
-
-        for label in md.getActiveLabels():
-            self._labelDict[label] = md.getValue(label, objId)
+        try:
+            self._labelDict = md.getRow(objId)
+        except AttributeError:  # can be eventually removed, once we are sure that users have recent Xmipp
+            self._labelDict.clear()
+            for label in md.getActiveLabels():
+                self._labelDict[label] = md.getValue(label, objId)
 
     def addToMd(self, md):
         self.writeToMd(md, md.addObject())
 
     def writeToMd(self, md, objId):
         """ Set back row values to a metadata row. """
-        for label, value in self._labelDict.items():
-            # TODO: Check how to handle correctly unicode type
-            # in Xmipp and Scipion
-            if type(value) is str:
-                value = str(value)
-            try:
-                md.setValue(label, value, objId)
-            except Exception as ex:
-                import sys
-                print("XmippMdRow.writeToMd: Error writing value to metadata.", file=sys.stderr)
-                print("                     label: %s, value: %s, type(value): %s" % (
-                    label2Str(label), value, type(value)), file=sys.stderr)
-                raise ex
+        try:
+            md.setRow(self._labelDict, objId)
+        except AttributeError:  # can be eventually removed, once we are sure that users have recent Xmipp
+            for label, value in self._labelDict.items():
+                # TODO: Check how to handle correctly unicode type
+                # in Xmipp and Scipion
+                if type(value) is str:
+                    value = str(value)
+                try:
+                    md.setValue(label, value, objId)
+                except Exception as ex:
+                    import sys
+                    print("XmippMdRow.writeToMd: Error writing value to metadata.", file=sys.stderr)
+                    print("                     label: %s, value: %s, type(value): %s" % (
+                        label2Str(label), value, type(value)), file=sys.stderr)
+                    raise ex
 
     def readFromFile(self, fn):
         md = MetaData(fn)
         self.readFromMd(md, md.firstObject())
 
     def writeToFile(self, fn):
         md = MetaData()
```

### Comparing `scipion-em-3.0.9/pwem/objects/__init__.py` & `scipion-em-3.1.0/pwem/objects/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.0.9/pwem/objects/data.py` & `scipion-em-3.1.0/pwem/objects/data.py`

 * *Files 15% similar despite different names*

```diff
@@ -24,26 +24,29 @@
 # *  e-mail address 'scipion@cnb.csic.es'
 # *
 # **************************************************************************
 """
 This modules contains basic hierarchy
 for EM data objects like: Image, SetOfImage and others
 """
+import logging
+logger = logging.getLogger(__name__)
 
 import os
 import json
 import numpy as np
 
+import pyworkflow.utils as pwutils
 from pyworkflow.object import (Object, Float, Integer, String,
                                OrderedDict, CsvList, Boolean, Set, Pointer,
                                Scalar)
-
 from pwem.constants import (NO_INDEX, ALIGN_NONE, ALIGN_2D, ALIGN_3D,
                             ALIGN_PROJ, ALIGNMENTS)
 
+
 class EMObject(Object):
     """Base object for all EM classes"""
 
     def __str__(self):
         return self.getClassName()
 
     def getFiles(self):
@@ -112,40 +115,175 @@
         return "\n    mag=%s\n    volt= %s\n    Cs=%s\n    Q0=%s\n\n" % \
                (self._magnification.get(),
                 self._voltage.get(),
                 self._sphericalAberration.get(),
                 self._amplitudeContrast.get())
 
 
+class Transform(EMObject):
+    """ This class will contain a transformation matrix
+    that can be applied to 2D/3D objects like images and volumes.
+    It should contain information about euler angles, translation(or shift)
+    and mirroring.
+    Shifts are stored in pixels as treated in extract coordinates, or assign angles,...
+    """
+
+    # Basic Transformation factory
+    ROT_X_90_CLOCKWISE = 'rotX90c'
+    ROT_Y_90_CLOCKWISE = 'rotY90c'
+    ROT_Z_90_CLOCKWISE = 'rotZ90c'
+    ROT_X_90_COUNTERCLOCKWISE = 'rotX90cc'
+    ROT_Y_90_COUNTERCLOCKWISE = 'rotY90cc'
+    ROT_Z_90_COUNTERCLOCKWISE = 'rotZ90cc'
+
+    def __init__(self, matrix=None, **kwargs):
+        EMObject.__init__(self, **kwargs)
+        self._matrix = Matrix()
+        if matrix is not None:
+            self.setMatrix(matrix)
+
+    def getMatrix(self):
+        return self._matrix.getMatrix()
+
+    def getRotationMatrix(self):
+        M = self.getMatrix()
+        return M[:3, :3]
+
+    def getShifts(self):
+        M = self.getMatrix()
+        return M[1, 4], M[2, 4], M[3, 4]
+
+    def getMatrixAsList(self):
+        """ Return the values of the Matrix as a list. """
+        return self._matrix.getMatrix().flatten().tolist()
+
+    def setMatrix(self, matrix):
+        self._matrix.setMatrix(matrix)
+
+    def __str__(self):
+        return str(self._matrix)
+
+    def scale(self, factor):
+        m = self.getMatrix()
+        m *= factor
+        m[3, 3] = 1.
+
+    def scaleShifts(self, factor):
+        # By default Scipion uses a coordinate system associated with the volume rather than the projection
+        m = self.getMatrix()
+        m[0, 3] *= factor
+        m[1, 3] *= factor
+        m[2, 3] *= factor
+
+    def invert(self):
+        # Local import to avoid loop pwem --> data --> convert --> Plugin (at pwem)
+        from pwem.convert.transformations import inverse_matrix
+
+        self._matrix.setMatrix(inverse_matrix(self._matrix.getMatrix()))
+
+        return self._matrix
+
+    def getShifts(self):
+        m = self.getMatrix()
+        return m[0, 3], m[1, 3], m[2, 3]
+
+    def setShifts(self, x, y, z):
+        m = self.getMatrix()
+        m[0, 3] = x
+        m[1, 3] = y
+        m[2, 3] = z
+
+    def setShiftsTuple(self, shifts):
+        self.setShifts(shifts[0], shifts[1], shifts[2])
+
+    def composeTransform(self, matrix):
+        """Apply a transformation matrix to the current matrix """
+        new_matrix = np.matmul(matrix, self.getMatrix())
+        # new_matrix = matrix * self.getMatrix()
+        self._matrix.setMatrix(new_matrix)
+
+    @classmethod
+    def create(cls, type):
+        if type == cls.ROT_X_90_CLOCKWISE:
+            return Transform(matrix=np.array([
+                [1, 0, 0, 0],
+                [0, 0, 1, 0],
+                [0, -1, 0, 0],
+                [0, 0, 0, 1]]))
+        elif type == cls.ROT_X_90_COUNTERCLOCKWISE:
+            return Transform(matrix=np.array([
+                [1, 0, 0, 0],
+                [0, 0, -1, 0],
+                [0, 1, 0, 0],
+                [0, 0, 0, 1]]))
+        elif type == cls.ROT_Y_90_CLOCKWISE:
+            return Transform(matrix=np.array([
+                [1, 0, -1, 0],
+                [0, 1, 0, 0],
+                [1, 0, 0, 0],
+                [0, 0, 0, 1]]))
+        elif type == cls.ROT_Y_90_COUNTERCLOCKWISE:
+            return Transform(matrix=np.array([
+                [1, 0, 1, 0],
+                [0, 1, 0, 0],
+                [-1, 0, 0, 0],
+                [0, 0, 0, 1]]))
+        elif type == cls.ROT_Z_90_CLOCKWISE:
+            return Transform(matrix=np.array([
+                [0, 1, 0, 0],
+                [-1, 0, 0, 0],
+                [0, 0, 1, 0],
+                [0, 0, 0, 1]]))
+        elif type == cls.ROT_Z_90_COUNTERCLOCKWISE:
+            return Transform(matrix=np.array([
+                [0, -1, 0, 0],
+                [1, 0, 0, 0],
+                [0, 0, 1, 0],
+                [0, 0, 0, 1]]))
+        else:
+            TRANSFORMATION_FACTORY_TYPES = [
+                cls.ROT_X_90_CLOCKWISE,
+                cls.ROT_Y_90_CLOCKWISE,
+                cls.ROT_Z_90_CLOCKWISE,
+                cls.ROT_X_90_COUNTERCLOCKWISE,
+                cls.ROT_Y_90_COUNTERCLOCKWISE,
+                cls.ROT_Z_90_COUNTERCLOCKWISE
+            ]
+            raise Exception('Introduced Transformation type is not recognized.\nAdmitted values are\n'
+                            '%s' % ' '.join(TRANSFORMATION_FACTORY_TYPES))
+
+
 class CTFModel(EMObject):
     """ Represents a generic CTF model. """
 
+    DEFOCUS_V_MINIMUM_VALUE = 0.1
+    DEFOCUS_RATIO_ERROR_VALUE = -1
+
     def __init__(self, **kwargs):
         EMObject.__init__(self, **kwargs)
         self._defocusU = Float(kwargs.get('defocusU', None))
         self._defocusV = Float(kwargs.get('defocusV', None))
         self._defocusAngle = Float(kwargs.get('defocusAngle', None))
         self._defocusRatio = Float()
         self._phaseShift = Float(kwargs['phaseShift']) if 'phaseShift' in kwargs else None
-        self._defocusRatio = Float()
         self._psdFile = String()
         self._micObj = None
         self._resolution = Float()
         self._fitQuality = Float()
 
     def __str__(self):
 
         def strEx(value):
             return "None" if value is None else "%0.2f" % value
 
         ctfStr = "defU={}, defV={}, ast={}, " \
                  "psh={}, res={}, fit={}".format(
             strEx(self._defocusU.get()),
             strEx(self._defocusV.get()),
-            strEx(self._defocusAngle.get()),
+            strEx(self._defocusU.get(0)-self._defocusV.get(0)),
             strEx(self.getPhaseShift()),
             strEx(self._resolution.get()),
             strEx(self._fitQuality.get())
         )
 
         return ctfStr
 
@@ -245,15 +383,19 @@
             self._defocusAngle.sum(90.)
         if self._defocusAngle >= 180.:
             self._defocusAngle.sum(-180.)
         elif self._defocusAngle < 0.:
             self._defocusAngle.sum(180.)
         # At this point defocusU is always greater than defocusV
         # following the EMX standard
-        self._defocusRatio.set(self.getDefocusU() / self.getDefocusV())
+
+        if self.getDefocusV() > self.DEFOCUS_V_MINIMUM_VALUE:
+            self._defocusRatio.set(self.getDefocusU() / self.getDefocusV())
+        else:
+            self._defocusRatio.set(self.DEFOCUS_RATIO_ERROR_VALUE)
 
     def equalAttributes(self, other, ignore=[], verbose=False):
         """ Override default behaviour to compare two
         CTF objects, now ignoring the psdFile.
         """
         return (self._defocusU == other._defocusU and
                 self._defocusV == other._defocusV and
@@ -540,15 +682,15 @@
 
     def setAcquisition(self, acquisition):
         self._acquisition = acquisition
 
     def hasTransform(self):
         return self._transform is not None
 
-    def getTransform(self):
+    def getTransform(self)-> Transform:
         return self._transform
 
     def setTransform(self, newTransform):
         self._transform = newTransform
 
     def hasOrigin(self):
         return self._origin is not None
@@ -580,17 +722,21 @@
         return x, y, z
         # x, y, z are floats in Angstroms
 
     def setShiftsInOrigin(self, x, y, z):
         origin = self.getOrigin(force=True)
         origin.setShifts(x, y, z)
 
-    def setOrigin(self, newOrigin):
-        """shifts in A"""
-        self._origin = newOrigin
+    def setOrigin(self, newOrigin=None):
+        """If None, default origin will be set.
+        Note: shifts are in Angstroms"""
+        if newOrigin:
+            self._origin = newOrigin
+        else:
+            self._origin = self._getDefaultOrigin()
 
     def originResampled(self, originNotResampled, oldSampling):
         factor = self.getSamplingRate() / oldSampling
         shifts = originNotResampled.getShifts()
         origin = self.getOrigin(force=True)
         origin.setShifts(shifts[0] * factor,
                          shifts[1] * factor,
@@ -605,14 +751,18 @@
                                          self.getSamplingRate() or 99999.))
 
     def getFiles(self):
         filePaths = set()
         filePaths.add(self.getFileName())
         return filePaths
 
+    def setMRCSamplingRate(self):
+        """ Sets the sampling rate to the mrc file represented by this image"""
+        from pwem.convert.headers import setMRCSamplingRate
+        setMRCSamplingRate(self.getFileName(), self.getSamplingRate())
 
 class Micrograph(Image):
     """ Represents an EM Micrograph object """
 
     def __init__(self, location=None, **kwargs):
         Image.__init__(self, location, **kwargs)
         self._micName = String()
@@ -717,22 +867,45 @@
     def setClassId(self, classId):
         self._classId.set(classId)
 
     def hasClassId(self):
         return self._classId.hasValue()
 
     def hasHalfMaps(self):
-        return self._halfMapFilenames.hasValue()
+        return not self._halfMapFilenames.isEmpty()
 
-    def getHalfMaps(self):
-        return self._halfMapFilenames.get()
+    def getHalfMaps(self, asList=False):
+        if asList:
+            return self._halfMapFilenames
+        else:
+            return self._halfMapFilenames.get()
 
     def setHalfMaps(self, listFileNames):
         return self._halfMapFilenames.set(listFileNames)
 
+    def fixMRCVolume(self, setSamplingRate=False):
+        """ Fixes the header of the mrc file pointed by this object
+
+        :param setSamplingRate: if true, it will set the header's sampling rate of the MRC file it refers
+
+        """
+        from pwem.convert.headers import fixVolume, setMRCSamplingRate
+        fixVolume(self.getFileName())
+
+        if setSamplingRate:
+            setMRCSamplingRate(self.getFileName(), self.getSamplingRate())
+
+    def __str__(self):
+        """ returns string representation adding halves info to base image.__str__"""
+        imgStr = super().__str__()
+
+        if self.hasHalfMaps():
+            imgStr += " - w/halves"
+
+        return imgStr
 
 class VolumeMask(Volume):
     """ A 3D mask to be used with volumes. """
     pass
 
 
 class EMFile(EMObject):
@@ -746,20 +919,72 @@
         """ Use the _objValue attribute to store filename. """
         return self._filename.get()
 
     def setFileName(self, filename):
         """ Use the _objValue attribute to store filename. """
         self._filename.set(filename)
 
+class Alphabet():
+    """ class with a dictionary of all valid alphabets"""
+    # sequence types
+    AMINOACIDS = 0
+    NUCLEOTIDES = 1
+    
+    SEQ_TYPE = ['aminoacids', 'nucleotides']
+
+    # alphabets for proteins
+    PROTEIN_ALPHABET = 0
+    EXTENDED_PROTEIN_ALPHABET = 1
+
+    # alphabets for nucleotides
+    AMBIGOUS_DNA_ALPHABET = 2
+    UNAMBIGOUS_DNA_ALPHABET = 3
+    EXTENDED_DNA_ALPHABET = 4
+    AMBIGOUS_RNA_ALPHABET = 5
+    UNAMBIGOUS_RNA_ALPHABET = 6 
+    NUCLEOTIDES_ALPHABET = 7
+
+    # dummy alphabet
+    DUMMY_ALPHABET = 8
+
+    # dictionary with all alphabets
+    alphabets = {}; alphabetsLabels = {}
+
+    alphabets[PROTEIN_ALPHABET] = 'ACDEFGHIKLMNPQRSTVWY'
+    alphabets[EXTENDED_PROTEIN_ALPHABET] = 'ACDEFGHIKLMNPQRSTVWYBJOUXZ'
+    alphabets[AMBIGOUS_DNA_ALPHABET] = 'GATCRYWSMKHBVDN'
+    alphabets[UNAMBIGOUS_DNA_ALPHABET] = 'GATC'
+    alphabets[EXTENDED_DNA_ALPHABET] = 'GATCBDSW'
+    alphabets[AMBIGOUS_RNA_ALPHABET] = 'GAUCRYWSMKHBVDN'
+    alphabets[UNAMBIGOUS_RNA_ALPHABET] = 'GAUC'
+    alphabets[NUCLEOTIDES_ALPHABET] = 'GAC'
+    alphabets[DUMMY_ALPHABET] = 'ABCDEFGHIJKLMNOPQRSTUVWXYZ'
+
+    # dictionary with all alphabets labels
+    alphabetsLabels[PROTEIN_ALPHABET] = 'Protein'
+    alphabetsLabels[EXTENDED_PROTEIN_ALPHABET] = 'Extended Protein'
+    alphabetsLabels[AMBIGOUS_DNA_ALPHABET] = 'Ambigous DNA'
+    alphabetsLabels[UNAMBIGOUS_DNA_ALPHABET] = 'Unambigous DNA'
+    alphabetsLabels[EXTENDED_DNA_ALPHABET] = 'Extended DNA'
+    alphabetsLabels[AMBIGOUS_RNA_ALPHABET] = 'Ambigous RNA'
+    alphabetsLabels[UNAMBIGOUS_RNA_ALPHABET] = 'Unambigous RNA'
+
+    
 
 class Sequence(EMObject):
     """Class containing a sequence of aminoacids/nucleotides
        Attribute names follow the biopython default ones
+            param: name: name of the sequence
+            param: sequence: string with the sequence
+            param: alphabet: integer with the alphabet to be used
+            param: isAminoacids: boolean indicating if the sequence is an aminoacid sequence
+            param: id: string with the sequence id
+            param: description: string with the sequence description
+           
     """
-
     def __init__(self, name=None, sequence=None,
                  alphabet=None, isAminoacids=True, id=None, description=None,
                  **kwargs):
         EMObject.__init__(self, **kwargs)
         # sequence Id, usually from a database. E.g: P12345
         self._id = String(id)
         # Descriptive alias provided by the user. E.g: CicloxigenasaB
@@ -805,29 +1030,70 @@
     # after that it makes no sense to change the alphabet
     def getAlphabet(self):
         return self._alphabet.get()
 
     def getIsAminoacids(self):
         return self._isAminoacids
 
+    def importFromFile(self, seqFileName, isAmino=True):
+        '''Fills the sequence attributes from the FIRST sequence found in the specified file'''
+        import pwem.convert as emconv
+        seqHandler = emconv.SequenceHandler()
+        seqDic = seqHandler.readSequenceFromFile(seqFileName, type=None, isAmino=isAmino)
+        self.setSequence(seqDic['sequence']), self.setId(seqDic['seqID'])
+        self.setName(seqDic['name']), self.setDescription(seqDic['description'])
+        self._alphabet.set(Integer(seqDic['alphabet']))
+        self._isAminoacids.set(Boolean(seqDic['isAminoacids']))
+
+    def exportToFile(self, seqFileName, doClean=True):
+        '''Exports the sequence to the specified file'''
+        import pwem.convert as emconv
+        seqHandler = emconv.SequenceHandler(self.getSequence(),
+                                            self._alphabet.get(), doClean)
+        # retrieving  args from scipion object
+        seqID = self.getId() if self.getId() is not None else 'seqID'
+        seqName = self.getSeqName() if self.getSeqName() is not None else 'seqName'
+        seqDescription = self.getDescription() if self.getDescription() is not None else ''
+        seqHandler.saveFile(seqFileName, seqID,
+                            name=seqName, seqDescription=seqDescription,
+                            type=None)
+                            #seqFiP12345 USER_SEQ 
+                            # Aspartate aminotransferase, mitochondrial
+
+    def appendToFile(self, seqFileName, doClean=True):
+        '''Exports the sequence to the specified file. If it already exists,
+        the sequence is appended to the ones in the file'''
+        logger.info("Appending sequence to file: %s" % seqFileName)
+        import pwem.convert as emconv
+        seqHandler = emconv.SequenceHandler(self.getSequence(),
+                                            Alphabet.DUMMY_ALPHABET, doClean)
+        # retrieving  args from scipion object
+        seqID = self.getId() if self.getId() is not None else 'seqID'
+        seqName = self.getSeqName() if self.getSeqName() is not None else 'seqName'
+        seqDescription = self.getDescription() if self.getDescription() is not None else ''
+        seqHandler.appendFile(seqFileName, seqID,
+                            name=seqName, seqDescription=seqDescription,
+                            type=None)
+
+
     def __str__(self):
         return "Sequence (name = {})\n".format(self.getSeqName())
 
 
 class AtomStruct(EMFile):
     """Represents an PDB file. """
 
     def __init__(self, filename=None, pseudoatoms=False, **kwargs):
         EMFile.__init__(self, filename, **kwargs)
         self._pseudoatoms = Boolean(pseudoatoms)
         self._volume = None
         # origin stores a matrix that using as input the point (0,0,0)
         # provides  the position of the actual origin in the system of
         # coordinates of the default origin.
-        # _origin is an object of the class Transformor shifts
+        # _origin is an object of the class Transform shifts
         # units are Angstroms (in Image units are A)
         self._origin = None
 
     def getPseudoAtoms(self):
         return self._pseudoatoms.get()
 
     def setPseudoAtoms(self, value):
@@ -836,15 +1102,15 @@
     def getVolume(self):
         return self._volume
 
     def hasVolume(self):
         return self._volume is not None
 
     def setVolume(self, volume):
-        if type(volume) is Volume:
+        if issubclass(type(volume), Volume):
             self._volume = volume
         else:
             raise Exception('TypeError', 'ERROR: SetVolume, This is not a '
                                          'volume')
 
     def __str__(self):
         return ("%s (pseudoatoms=%s, volume=%s)" %
@@ -936,14 +1202,69 @@
                 # _appendItem to False do not append the item
                 if getattr(newItem, "_appendItem", True):
                     self.append(newItem)
             else:
                 if itemDataIter is not None:
                     next(itemDataIter)  # just skip disabled data row
 
+    @classmethod
+    def create(cls, outputPath,
+               prefix=None, suffix=None, ext=None,
+               **kwargs):
+        """ Create an empty set from the current Set class.
+         Params:
+            outputPath: where the output file will be written.
+            prefix: prefix of the created file, if None, it will be deduced
+                from the ClassName.
+            suffix: additional suffix that will be added to the prefix with a
+                "_" in between.
+            ext: extension of the output file, be default will use .sqlite
+        """
+        fn = prefix or cls.__name__.lower().replace('setof', '')
+
+        if suffix:
+            fn += '_%s' % suffix
+
+        if ext and ext[0] == '.':
+            ext = ext[1:]
+        fn += '.%s' % (ext or 'sqlite')
+
+        setPath = os.path.join(outputPath, fn)
+        pwutils.cleanPath(setPath)
+
+        return cls(filename=setPath, **kwargs)
+
+    def createCopy(self, outputPath,
+                   prefix=None, suffix=None, ext=None,
+                   copyInfo=False, copyItems=False):
+        """ Make a copy of the current set to another location (e.g file).
+        Params:
+            outputPath: where the output file will be written.
+            prefix: prefix of the created file, if None, it will be deduced
+                from the ClassName.
+            suffix: additional suffix that will be added to the prefix with a
+                "_" in between.
+            ext: extension of the output file, be default will use the same
+                extension of this set filename.
+            copyInfo: if True the copyInfo will be called after set creation.
+            copyItems: if True the copyItems function will be called.
+        """
+        setObj = self.create(outputPath,
+                             prefix=prefix,
+                             suffix=suffix,
+                             ext=ext or pwutils.getExt(self.getFileName()))
+
+        if copyInfo:
+            setObj.copyInfo(self)
+
+        if copyItems:
+            setObj.copyItems(self)
+
+        return setObj
+
     def getFiles(self):
         return Set.getFiles(self)
 
 
 class SetOfImages(EMSet):
     """ Represents a set of Images """
     ITEM_TYPE = Image
@@ -1117,25 +1438,28 @@
 
     def getDimensions(self):
         """Return first image dimensions as a tuple: (xdim, ydim, zdim)"""
         return self.getFirstItem().getDim()
 
     def __str__(self):
         """ String representation of a set of images. """
+        s = "%s (%d items, %s, %s%s)" % \
+            (self.getClassName(), self.getSize(),
+             self._dimStr(), self._samplingRateStr(), self._appendStreamState())
+        return s
+    def _samplingRateStr(self):
+        """ Returns how the sampling rate is presented in a 'str' context."""
         sampling = self.getSamplingRate()
 
         if not sampling:
-            print("FATAL ERROR: Object %s has no sampling rate!!!"
+            logger.error("FATAL ERROR: Object %s has no sampling rate!!!"
                   % self.getName())
             sampling = -999.0
 
-        s = "%s (%d items, %s, %0.2f Å/px%s)" % \
-            (self.getClassName(), self.getSize(),
-             self._dimStr(), sampling, self._appendStreamState())
-        return s
+        return "%0.2f Å/px" % sampling
 
     def _dimStr(self):
         """ Return the string representing the dimensions. """
         return str(self._firstDim)
 
     def iterItems(self, orderBy='id', direction='ASC', where='1', limit=None, iterate=True):
         """ Redefine iteration to set the acquisition to images. """
@@ -1232,21 +1556,33 @@
         this SetOfParticles"""
         return self._coordsPointer.get()
 
     def setCoordinates(self, coordinates):
         """ Set the SetOfCoordinates associates with
         this set of particles.
          """
-        self._coordsPointer.set(coordinates)
+        if coordinates.isPointer():
+            self._coordsPointer.copy(coordinates)
+        else:
+            self._coordsPointer.set(coordinates)
+
+        if not self._coordsPointer.hasExtended():
+            logger.warning("FOR DEVELOPERS: Direct pointers to objects should be avoided. "
+                           "They are problematic in complex streaming scenarios. "
+                           "Pass a pointer to a protocol with extended "
+                           "(e.g.: input param are this kind of pointers. Without get()!)")
+
 
     def copyInfo(self, other):
         """ Copy basic information (voltage, spherical aberration and
         sampling rate) from other set of micrographs to current one.
         """
         SetOfImages.copyInfo(self, other)
+        if hasattr(other, '_coordsPointer'):
+            self.copyAttributes(other, "_coordsPointer")
         self.setHasCTF(other.hasCTF())
 
 
 class SetOfAverages(SetOfParticles):
     """Represents a set of Averages.
     It is a SetOfParticles but it is useful to differentiate outputs."""
 
@@ -1323,28 +1659,55 @@
 
 class SetOfAtomStructs(EMSet):
     """ Set containing PDB items. """
     ITEM_TYPE = AtomStruct
     # Hint to GUI components to expose internal items for direct selection
     EXPOSE_ITEMS = True
 
+    def getFiles(self):
+        files = []
+        for atomStruct in self.iterItems():
+            files.append(atomStruct.getFileName())
+
+        return files
 
 class SetOfPDBs(SetOfAtomStructs):
     """ Set containing PDB items. """
 
     def __init__(self):
         SetOfAtomStructs.__init__(self)
-        print("SetOfPDBs class has been renamed to SetOfAtomStructs. "
+        logger.warning("FOR DEVELOPERS: SetOfPDBs class has been renamed to SetOfAtomStructs. "
               "Please update your code.")
 
 
 class SetOfSequences(EMSet):
     """Set containing Sequence items."""
     ITEM_TYPE = Sequence
 
+    def __init__(self, **kwargs):
+        super().__init__(**kwargs)
+        self.aligned = Boolean(kwargs.get('aligned', False))
+
+
+    def exportToFile(self, seqFileName):
+        '''Writes the sequences in the set in the specified file'''
+        for sequence in self:
+            sequence.appendToFile(seqFileName)
+
+    def importFromFile(self, seqFileName, isAmino=True, type=None):
+        '''Appends elements to the set from sequences found in the specified file'''
+        import pwem.convert as emconv
+        seqHandler = emconv.SequenceHandler()
+        seqsDic = seqHandler.readSequencesFromFile(seqFileName, type=type, isAmino=isAmino)
+        for seqDic in seqsDic:
+            newSeq = Sequence(sequence=seqDic['sequence'], id=seqDic['seqID'],
+                              name=seqDic['name'], description=seqDic['description'],
+                              alphabet=seqDic['alphabet'], isAminoacids=seqDic['isAminoacids'])
+            self.append(newSeq)
+
 
 class Coordinate(EMObject):
     """This class holds the (x,y) position and other information
     associated with a coordinate"""
 
     def __init__(self, **kwargs):
         EMObject.__init__(self, **kwargs)
@@ -1491,14 +1854,20 @@
             micrographs: Either a SetOfMicrographs object or a pointer to it.
         """
         if micrographs.isPointer():
             self._micrographsPointer.copy(micrographs)
         else:
             self._micrographsPointer.set(micrographs)
 
+        if not self._micrographsPointer.hasExtended():
+            logger.warning("FOR DEVELOPERS: Direct pointers to objects should be avoided. "
+                         "They are problematic in complex streaming scenarios. "
+                         "Pass a pointer to a protocol with extended "
+                         "(e.g.: input param are this kind of pointers. Without get()!)")
+
     def getFiles(self):
         filePaths = set()
         filePaths.add(self.getFileName())
         return filePaths
 
     def __str__(self):
         """ String representation of a set of coordinates. """
@@ -1554,80 +1923,14 @@
         """ Override the default behaviour of copy
         to also copy array data.
         """
         self.setMatrix(np.copy(other.getMatrix()))
         self._objValue = other._objValue
 
 
-class Transform(EMObject):
-    """ This class will contain a transformation matrix
-    that can be applied to 2D/3D objects like images and volumes.
-    It should contain information about euler angles, translation(or shift)
-    and mirroring.
-    Shifts are stored in pixels as treated in extract coordinates, or assign angles,...
-    """
-
-    def __init__(self, matrix=None, **kwargs):
-        EMObject.__init__(self, **kwargs)
-        self._matrix = Matrix()
-        if matrix is not None:
-            self.setMatrix(matrix)
-
-    def getMatrix(self):
-        return self._matrix.getMatrix()
-
-    def getMatrixAsList(self):
-        """ Return the values of the Matrix as a list. """
-        return self._matrix.getMatrix().flatten().tolist()
-
-    def setMatrix(self, matrix):
-        self._matrix.setMatrix(matrix)
-
-    def __str__(self):
-        return str(self._matrix)
-
-    def scale(self, factor):
-        m = self.getMatrix()
-        m *= factor
-        m[3, 3] = 1.
-
-    def scaleShifts(self, factor):
-        # By default Scipion uses a coordinate system associated with the volume rather than the projection
-        m = self.getMatrix()
-        m[0, 3] *= factor
-        m[1, 3] *= factor
-        m[2, 3] *= factor
-
-    def invert(self):
-        # Local import to avoid loop pwem --> data --> convert --> Plugin (at pwem)
-        from pwem.convert.transformations import inverse_matrix
-
-        self._matrix.setMatrix(inverse_matrix(self._matrix.getMatrix()))
-
-        return self._matrix
-
-    def getShifts(self):
-        m = self.getMatrix()
-        return m[0, 3], m[1, 3], m[2, 3]
-
-    def setShifts(self, x, y, z):
-        m = self.getMatrix()
-        m[0, 3] = x
-        m[1, 3] = y
-        m[2, 3] = z
-
-    def setShiftsTuple(self, shifts):
-        self.setShifts(shifts[0], shifts[1], shifts[2])
-
-    def composeTransform(self, matrix):
-        """Apply a transformation matrix to the current matrix """
-        new_matrix = matrix * self.getMatrix()
-        self._matrix.setMatrix(new_matrix)
-
-
 class Class2D(SetOfParticles):
     """ Represent a Class that groups Particles objects.
     Usually the representative of the class is another Particle
     (some kind of average particle from the particles assigned
     to the class)
     """
 
@@ -1705,19 +2008,36 @@
                     if iterDisabled or img.isEnabled():
                         yield img
 
     def hasRepresentatives(self):
         return self._representatives.get()
 
     def getImages(self):
-        """ Return the SetOFImages used to create the SetOfClasses. """
+        """ Return the SetOfImages used to create the SetOfClasses. """
         return self._imagesPointer.get()
 
+    def getImagesPointer(self):
+        """" Return the pointer to the SetOfImages used to create the SetOfClasses. """
+        return self._imagesPointer
+
     def setImages(self, images):
-        self._imagesPointer.set(images)
+        """ Set the images (particles) 2d associated with this set of classes.
+        Params:
+            images: An indirect pointer (with extended) to a set of images.
+        """
+        if images.isPointer():
+            self._imagesPointer.copy(images)
+        else:
+            self._imagesPointer.set(images)
+
+        if not self._imagesPointer.hasExtended():
+            logger.warning("FOR DEVELOPERS: Direct pointers to objects should be avoided. "
+                         "They are problematic in complex streaming scenarios. "
+                         "Pass a pointer to a protocol with extended "
+                         "(e.g.: input param are this kind of pointers. Without get()!)")
 
     def getDimensions(self):
         """Return first image dimensions as a tuple: (xdim, ydim, zdim)"""
         if self.hasRepresentatives():
             return self.getFirstItem().getRepresentative().getDim()
         return None
 
@@ -1763,14 +2083,21 @@
             if classItem.hasRepresentative():
                 rep = classItem.getRepresentative()
                 rep.setObjId(classItem.getObjId())
                 rep.setSamplingRate(classItem.getSamplingRate())
 
                 yield rep
 
+    def getFiles(self):
+
+        files = []
+        for rep in self.iterRepresentatives():
+            files.append(rep.getFileName())
+        return files
+
     def getSamplingRate(self):
         return self.getImages().getSamplingRate()
 
     def appendFromClasses(self, classesSet, filterClassFunc=None, updateClassCallback=None):
         """ Iterate over the classes and the elements inside each
         class and append classes and items that are enabled.
         """
@@ -1934,14 +2261,19 @@
     def getPdb(self):
         return self._pdbPointer.get()
 
     def copyInfo(self, other):
         self._pdbPointer.copy(other._pdbPointer, copyId=False)
 
 
+class SetOfPrincipalComponents(SetOfNormalModes):
+    "Set of Principal Components is a SetOfNormalModes with a new name"
+    pass
+
+
 class FramesRange(CsvList):
     """ Store first and last frames in a movie. The last element will be
      the index in the stack of the first frame.
     """
 
     def __init__(self, firstFrame=1, lastFrame=0, firstFrameIndex=1):
         """
@@ -2199,11 +2531,26 @@
     def getData(self):
         return self._x, self._y
 
     def setData(self, xData, yData):
         self._x.set(xData)
         self._y.set(yData)
 
+    def calculateResolution(self, threshold=0.143):
+        """
+        Calculate the FSC resolution value
+        """
+        dataLength = len(self._x)
+        for i in range(dataLength):
+            if float(self._y[i]) < threshold or i == dataLength-1:
+                above_res = float(self._x[i-1])
+                above_fsc = float(self._y[i-1])
+                below_res = float(self._x[i])
+                below_fsc = float(self._y[i])
+                break
+        resolution = below_res - ((threshold-below_fsc)/(above_fsc-below_fsc) * (below_res-above_res))
+        return "{0:.1f}".format(1/resolution)
+
 
 class SetOfFSCs(EMSet):
     """Represents a set of FSCs"""
     ITEM_TYPE = FSC
```

### Comparing `scipion-em-3.0.9/pwem/objects/data_tiltpairs.py` & `scipion-em-3.1.0/pwem/objects/data_tiltpairs.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.0.9/pwem/protocols/__init__.py` & `scipion-em-3.1.0/pwem/protocols/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -34,27 +34,37 @@
 from .protocol_align_movies import (ProtAlignMovies, ProtAverageFrames,
                                     createAlignmentPlot)
 from .protocol_particles import *
 from .protocol_particles_picking import *
 from .protocol_2d import *
 from .protocol_3d import *
 from .protocol_sets import *
+from .protocol_projection_edit import *
 from .protocol_pdf_report import *
 from .protocol_tiltpairs import *
 from .protocol_ctf_assign import ProtCTFAssign
 from .protocol_alignment_assign import ProtAlignmentAssign
 from .protocol_alignment_invertHand import ProtAlignmentInvertHand
 from .protocol_batch import *
-from .protocol_classes_consensus import ProtClassesConsensus
 from .protocol_extract_coordinates import ProtExtractCoords
 from .protocol_create_stream_data import ProtCreateStreamData
 from .parallel import ProtTestParallel
 from .protocol_create_stream_data import SET_OF_RANDOM_MICROGRAPHS
 
 from .protocol_import import *
 
 from .protocol_export import *
 from .protocol_tests import *
 
 from .protocol_origin_sampling_volume import ProtOrigSampling
-from .protocol_metadata_editor import ProtMetadataEditor
+from .protocol_projection_edit import ProtProjectionEditor
+from .protocol_set_editor import ProtSetEditor
+from .protocol_set_filter import ProtSetFilter
+from .protocol_movie_eraser import ProtMovieEraser
+from .protocol_classes_selector import ProtClassesSelector
+from .protocol_boxsize_parameters import ProtBoxSizeParameters
+from .protocol_boxsize_checkpoint import ProtBoxSizeCheckpoint
+
+from .protocol_mathematical_operator import ProtMathematicalOperator
+
+from .protocol_tools import *
```

### Comparing `scipion-em-3.0.9/pwem/protocols/parallel.py` & `scipion-em-3.1.0/pwem/protocols/parallel.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.0.9/pwem/protocols/protocol.py` & `scipion-em-3.1.0/pwem/protocols/protocol.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,14 @@
 except ImportError:
     izip = zip
 
 import pyworkflow.object as pwobj
 import pyworkflow.protocol as pwprot
 import pyworkflow.protocol.params as params
 import pyworkflow.utils as pwutils
-import pyworkflow.mapper as pwmapper
 
 import pwem.objects as emobj
 import pwem.constants as emcts
 
 
 class EMProtocol(pwprot.Protocol):
     """ Base class to all EM protocols.
@@ -53,16 +52,14 @@
     def __createSet(self, SetClass, template, suffix, **kwargs):
         """ Create a set and set the filename using the suffix.
         If the file exists, it will be delete. """
         setFn = self._getPath(template % suffix)
         # Close the connection to the database if
         # it is open before deleting the file
         pwutils.cleanPath(setFn)
-
-        pwmapper.SqliteDb.closeConnection(setFn)
         setObj = SetClass(filename=setFn, **kwargs)
         return setObj
 
     def _createSetOfMicrographs(self, suffix=''):
         return self.__createSet(emobj.SetOfMicrographs,
                                 'micrographs%s.sqlite', suffix,
                                 indexes=['_index'])
```

### Comparing `scipion-em-3.0.9/pwem/protocols/protocol_2d.py` & `scipion-em-3.1.0/pwem/protocols/protocol_2d.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.0.9/pwem/protocols/protocol_3d.py` & `scipion-em-3.1.0/pwem/protocols/protocol_3d.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.0.9/pwem/protocols/protocol_align_movies.py` & `scipion-em-3.1.0/pwem/protocols/protocol_micrographs.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 # **************************************************************************
 # *
-# * Authors:     J.M. De la Rosa Trevin (jmdelarosa@cnb.csic.es)
-# *              Vahid Abrishami (vabrishami@cnb.csic.es)
-# *              Josue Gomez Blanco (josue.gomez-blanco@mcgill.ca)
+# * Authors:     Josue Gomez Blanco (josue.gomez-blanco@mcgill.ca)
+# *              Roberto Marabini (roberto@cnb.csic.es)
+# *              Airen Zaldivar Peraza (azaldivar@cnb.csic.es)
+# *              Grigory Sharov (gsharov@mrc-lmb.cam.ac.uk)
+# *
 # *
 # * Unidad de  Bioinformatica of Centro Nacional de Biotecnologia , CSIC
 # *
 # * This program is free software; you can redistribute it and/or modify
 # * it under the terms of the GNU General Public License as published by
 # * the Free Software Foundation; either version 3 of the License, or
 # * (at your option) any later version.
@@ -21,787 +23,730 @@
 # * Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA
 # * 02111-1307  USA
 # *
 # *  All comments concerning this program package may be sent to the
 # *  e-mail address 'scipion@cnb.csic.es'
 # *
 # **************************************************************************
-
-import os
-import warnings
-
-try:
-    from itertools import izip
-except ImportError:
-    izip = zip
-from math import ceil
+import enum
+from os.path import exists, getmtime
+from datetime import datetime
+from collections import OrderedDict
 
 import pyworkflow.object as pwobj
-import pyworkflow.utils as pwutils
-from pyworkflow.gui.plotter import Plotter
-import pyworkflow.protocol.params as params
 import pyworkflow.protocol.constants as pwcts
+import pyworkflow.protocol.params as params
+import pyworkflow.utils as pwutils
 
 import pwem.objects as emobj
-from pwem import emlib
 
-from pwem.protocols import ProtProcessMovies
+from .protocol import EMProtocol
 
 
-class ProtAlignMovies(ProtProcessMovies):
-    """
-    Base class for movie alignment protocols such as:
-    motioncorr, crosscorrelation and optical flow
+class ProtMicrographs(EMProtocol):
+    pass
 
-    Alignment parameters are defined in common. For example,
-    the frames range used for alignment and final sum, the binning factor
-    or the cropping options (region of interest)
-    """
+
+class ProtCTFMicOutputs(enum.Enum):
+    outputCTF = emobj.SetOfCTF
+
+
+class ProtCTFMicrographs(ProtMicrographs):
+    """ Base class for all protocols that estimates the CTF"""
+
+    _possibleOutputs = ProtCTFMicOutputs
+
+    def __init__(self, **kwargs):
+        EMProtocol.__init__(self, **kwargs)
+        self.stepsExecutionMode = pwcts.STEPS_PARALLEL
+        self.isFirstTime = pwobj.Boolean(False)
 
     # -------------------------- DEFINE param functions -----------------------
     def _defineParams(self, form):
-        ProtProcessMovies._defineParams(self, form)
-        self._defineAlignmentParams(form)
+        form.addSection(label=pwutils.Message.LABEL_CTF_ESTI)
+        form.addParam('recalculate', params.BooleanParam, default=False,
+                      condition='recalculate',
+                      label="Do recalculate ctf?")
+
+        form.addParam('continueRun', params.PointerParam, allowsNull=True,
+                      condition='recalculate', label="Input previous run",
+                      pointerClass=self.getClassName())
+        form.addHidden('sqliteFile', params.FileParam, condition='recalculate',
+                       allowsNull=True)
+
+        form.addParam('inputMicrographs', params.PointerParam, important=True,
+                      condition='not recalculate',
+                      label=pwutils.Message.LABEL_INPUT_MIC,
+                      pointerClass='SetOfMicrographs')
+
+        form.addParam('AutoDownsampling', params.BooleanParam, default=False,
+                      label='Automatic Downsampling Factor',
+                      help='Recommended value to downsample')
+
+        form.addParam('ctfDownFactor', params.FloatParam, default=1.,
+                      label='Manual CTF Downsampling factor',
+                      condition='not AutoDownsampling',  # 'not recalculate',
+                      help='Set to 1 for no downsampling. Non-integer downsample '
+                           'factors are possible. This downsampling is only used '
+                           'for estimating the CTF and it does not affect any '
+                           'further calculation. Ideally the estimation of the '
+                           'CTF is optimal when the Thon rings are not too '
+                           'concentrated at the origin (too small to be seen) '
+                           'and not occupying the whole power spectrum (since '
+                           'this downsampling might entail aliasing).')
+
+        self._defineProcessParams(form)
+
+        line = form.addLine('Resolution', condition='not recalculate',
+                            help='Give a value in digital frequency '
+                                 '(i.e. between 0.0 and 0.5). These cut-offs '
+                                 'prevent the typical peak at the center of the'
+                                 ' PSD and high-resolution terms where only '
+                                 'noise exists, to interfere with CTF '
+                                 'estimation. The default lowest value is 0.05 '
+                                 'but for micrographs with a very fine sampling '
+                                 'this may be lowered towards 0. The default '
+                                 'highest value is 0.35, but it should be '
+                                 'increased for micrographs with signals '
+                                 'extending beyond this value. However, if '
+                                 'your micrographs extend further than 0.35, '
+                                 'you should consider sampling them at a finer '
+                                 'rate.')
+        line.addParam('lowRes', params.FloatParam, default=0.05, label='Lowest')
+        line.addParam('highRes', params.FloatParam, default=0.35, label='Highest')
+        line = form.addLine('Defocus search range (microns)',
+                            condition='not recalculate',
+                            expertLevel=pwcts.LEVEL_ADVANCED,
+                            help='Select _minimum_ and _maximum_ values for '
+                                 'defocus search range (in microns). Underfocus'
+                                 ' is represented by a positive number.')
+        line.addParam('minDefocus', params.FloatParam, default=0.25,
+                      label='Min')
+        line.addParam('maxDefocus', params.FloatParam, default=4.,
+                      label='Max')
+
+        form.addParam('windowSize', params.IntParam, default=512,
+                      expertLevel=pwcts.LEVEL_ADVANCED,
+                      label='Window size', condition='not recalculate',
+                      help='The PSD is estimated from small patches of this '
+                           'size. Bigger patches allow identifying more '
+                           'details. However, since there are fewer windows, '
+                           'estimations are noisier.')
+
+        form.addParallelSection(threads=2, mpi=1)
+
+    def _defineProcessParams(self, form):
+        """ This method should be implemented by subclasses
+        to add other parameter relatives to the specific operation."""
+        pass
+
+    # -------------------------- INSERT steps functions -----------------------
+    def _insertAllSteps(self):
+        """ Insert the steps to perform CTF estimation, or re-estimation,
+        on a set of micrographs.
+        """
+        self._defineCtfParamsDict()
+        self.micDict = OrderedDict()
+
+        if not self.recalculate:
+            self.initialIds = self._insertInitialSteps()
+            micDict, self.streamClosed = self._loadInputList()
+            ctfIds = self._insertNewMicsSteps(micDict.values())
+            self._insertFinalSteps(ctfIds)
+            # For the streaming mode, the steps function have a 'wait' flag
+            # that can be turned on/off. For example, here we insert the
+            # createOutputStep but it wait=True, which means that can not be
+            # executed until it is set to False
+            # (when the input micrographs stream is closed)
+            waitCondition = self._getFirstJoinStepName() == 'createOutputStep'
+        else:
+            if self.isFirstTime:
+                # Insert previous estimation or re-estimation an so on...
+                self._insertPreviousSteps()
+                self.isFirstTime.set(False)
+            ctfIds = self._insertRecalculateSteps()
+            # For now the streaming is not allowed for recalculate CTF
+            waitCondition = False
+
+        self._insertFunctionStep('createOutputStep', prerequisites=ctfIds,
+                                 wait=waitCondition)
+
+    def _insertInitialSteps(self):
+        """ Override this function to insert some steps before the
+        estimate ctfs steps.
+        Should return a list of ids of the initial steps. """
+
+        pwutils.makePath(self._getExtraPath('DONE'))
+        return []
+
+    def _insertNewMicsSteps(self, inputMics):
+        """ Insert steps to process new mics (from streaming)
+        Params:
+            inputMics: input mics set to be check
+        """
+        return self._insertNewMics(inputMics,
+                                   lambda mic: mic.getMicName(),
+                                   self._insertCtfStep,
+                                   self._insertCtfListStep,
+                                   *self._getCtfArgs())
+
+    def _insertRecalculateSteps(self):
+        recalDeps = []
+        # For each psd insert the steps to process it
+        self.recalculateSet = emobj.SetOfCTF(filename=self.sqliteFile.get(),
+                                             objDoStore=False)
+        inputMics = self.getInputMicrographs()
+        for ctf in self.recalculateSet:
+            line = ctf.getObjComment()
+            if ctf.isEnabled() and line:
+                # CTF Re-estimation
+                # Make estimation steps independent between them
+                objId = ctf.getObjId()
+                stepId = self._insertFunctionStep('reEstimateCtfStep',
+                                                  objId, prerequisites=[])
+                recalDeps.append(stepId)
+                self.micDict[objId] = inputMics[objId].clone()
+        return recalDeps
+
+    def _insertFinalSteps(self, deps):
+        """ This should be implemented in subclasses"""
+        return deps
+
+    def _getFirstJoinStepName(self):
+        # This function will be used for streaming, to check which is
+        # the first function that need to wait for all micrographs
+        # to have completed, this can be overwritten in subclasses
+        # (e.g., in Xmipp 'sortPSDStep')
+        return 'createOutputStep'
+
+    def _getFirstJoinStep(self):
+        for s in self._steps:
+            if s.funcName == self._getFirstJoinStepName():
+                return s
+        return None
+
+    # -------------------------- STEPS functions ------------------------------
+    def _insertCtfStep(self, mic, prerequisites, *args):
+        """ Basic method to insert an estimation step for a given micrograph. """
+        micStepId = self._insertFunctionStep('estimateCtfStep',
+                                             mic.getMicName(), *args,
+                                             prerequisites=prerequisites)
+        return micStepId
+
+    def estimateCtfStep(self, micName, *args):
+        """ Step function that will be common for all CTF protocols.
+        It will take care of re-building the micrograph object from the micDict
+        argument and perform any conversion if needed. Then, the function
+        _estimateCTF will be called, that should be implemented by each
+        CTF estimation protocol.
+        """
+        mic = self.micDict[micName]
+        micDoneFn = self._getMicrographDone(mic)
+        micFn = mic.getFileName()
+
+        if self.isContinued() and self._isMicDone(mic):
+            self.info("Skipping micrograph: %s, seems to be done" % micFn)
+            return
+
+        # Clean old finished files
+        pwutils.cleanPath(micDoneFn)
+        self.info("Estimating CTF of micrograph: %s " % mic.getObjId())
+        self._estimateCTF(mic, *args)
+
+        # Mark this mic as finished
+        open(micDoneFn, 'w').close()
+
+    def _estimateCTF(self, mic, *args):
+        """ Do the CTF estimation with the specific program
+        and the parameters required.
+        Params:
+         micFn: micrograph filename
+         micDir: micrograph directory
+        """
+        raise Exception(pwutils.Message.ERROR_NO_EST_CTF)
+
+    def reEstimateCtfStep(self, micId):
+        """ CTF - re-estimation that is common for all programs.
+        The _restimateCTF function will be called with proper parameters.
+        """
+        ctf = self.recalculateSet[micId]
+        mic = self.micDict[micId]
+        micDoneFn = self._getMicrographDone(mic)
+        # Clean old finished files
+        pwutils.cleanPath(micDoneFn)
+        self.info("Estimating CTF of micrograph: %s " % mic.getObjId())
+        self._reEstimateCTF(mic, ctf)
+
+        # Mark this mic as finished
+        open(micDoneFn, 'w').close()
+
+    def _reEstimateCTF(self, mic, ctf):
+        """ Do the re-estimation of this mic (original one)
+        and the parameters that comes in the comment field of the ctf object.
+        Params:
+         micFn: micrograph filename
+         micDir: micrograph directory
+        """
+        raise Exception(pwutils.Message.ERROR_NO_EST_CTF)
 
-    def _defineAlignmentParams(self, form):
-        group = form.addGroup('Alignment')
-        line = group.addLine('Frames to ALIGN',
-                             help='Frames range to ALIGN on each movie. The '
-                                  'first frame is 1. If you set 0 in the final '
-                                  'frame to align, it means that you will '
-                                  'align until the last frame of the movie.')
-        line.addParam('alignFrame0', params.IntParam, default=1,
-                      label='from')
-        line.addParam('alignFrameN', params.IntParam, default=0,
-                      label='to')
-        group.addParam('useAlignToSum', params.BooleanParam, default=True,
-                       label='Use ALIGN frames range to SUM?',
-                       help="If *Yes*, the same frame range will be used to "
-                            "ALIGN and to SUM. If *No*, you can selected a "
-                            "different range for SUM (must be a subset).")
-        line = group.addLine('Frames to SUM', condition="not useAlignToSum",
-                             help='Frames range to SUM on each movie. The '
-                                  'first frame is 1. If you set 0 in the final '
-                                  'frame to sum, it means that you will sum '
-                                  'until the last frame of the movie.')
-        line.addParam('sumFrame0', params.IntParam, default=1,
-                      label='from')
-        line.addParam('sumFrameN', params.IntParam, default=0,
-                      label='to')
-        group.addParam('binFactor', params.FloatParam, default=1.,
-                       label='Binning factor',
-                       help='1x or 2x. Bin stack before processing.')
-
-        line = group.addLine('Crop offsets (px)')
-        line.addParam('cropOffsetX', params.IntParam, default=0, label='X')
-        line.addParam('cropOffsetY', params.IntParam, default=0, label='Y')
-
-        line = group.addLine('Crop dimensions (px)',
-                             help='How many pixels to crop from offset\n'
-                                  'If equal to 0, use maximum size.')
-        line.addParam('cropDimX', params.IntParam, default=0, label='X')
-        line.addParam('cropDimY', params.IntParam, default=0, label='Y')
-
-        form.addParam('doSaveAveMic', params.BooleanParam, default=True,
-                      label="Save aligned micrograph",
-                      expertLevel=pwcts.LEVEL_ADVANCED)
-
-        form.addParam('doSaveMovie', params.BooleanParam, default=False,
-                      label="Save movie", expertLevel=pwcts.LEVEL_ADVANCED,
-                      help="Save Aligned movie")
+    # Group of functions to estimate several micrographs if the batch size is
+    # defined. In some programs it might be more efficient to estimate many
+    # at once and not one by one
+
+    def _insertCtfListStep(self, micList, prerequisites, *args):
+        """ Basic method to insert an estimation step for a given micrograph. """
+        micNameList = [mic.getMicName() for mic in micList]
+        micStepId = self._insertFunctionStep('estimateCtfListStep',
+                                             micNameList, *args,
+                                             prerequisites=prerequisites)
+        return micStepId
+
+    def estimateCtfListStep(self, micNameList, *args):
+        micList = []
+
+        for micName in micNameList:
+            mic = self.micDict[micName]
+            micDoneFn = self._getMicrographDone(mic)
+            if self.isContinued() and self._isMicDone(mic):
+                self.info("Skipping micrograph: %s, seems to be done"
+                          % mic.getFileName())
+            else:
+                # Clean old finished files
+                pwutils.cleanPath(micDoneFn)
+                micList.append(mic)
+
+        self.info("Estimating CTF for micrographs: %s"
+                  % [mic.getObjId() for mic in micList])
+        self._estimateCtfList(micList, *args)
+
+        for mic in micList:
+            # Mark this mic as finished
+            open(self._getMicrographDone(mic), 'w').close()
+
+    def _estimateCtfList(self, micList, *args):
+        """ This function can be implemented by subclasses if it is a more
+        efficient way to estimate many micrographs at once.
+         Default implementation will just call the _estimateCTF. """
+        for mic in micList:
+            self._estimateCTF(mic, *args)
+
+    def _createCtfModel(self, mic, updateSampling=False):
+        """ This should be implemented in subclasses
+        in order to create a CTF model from program results.
+        """
+        pass
 
-    # --------------------------- STEPS functions ----------------------------
     def createOutputStep(self):
-        # validate that we have some output movies
-        for outName, out in self.iterOutputAttributes():
-            output = out
-            break
-
-        if output.getSize() == 0 and len(self.listOfMovies) != 0:
-            raise Exception("All movies failed, didn't create outputMicrographs."
-                            "Please review movie processing steps above.")
-        elif output.getSize() < len(self.listOfMovies):
-            self.warning(pwutils.yellowStr("WARNING - Failed to align %d movies."
-                                           % (len(self.listOfMovies) - output.getSize())))
-
-    def _loadOutputSet(self, SetClass, baseName, fixSampling=True):
-        """
-        Load the output set if it exists or create a new one.
-        fixSampling: correct the output sampling rate if binning was used,
-        except for the case when the original movies are kept and shifts
-        refers to that one.
-        """
-        setFile = self._getPath(baseName)
-
-        if os.path.exists(setFile) and os.path.getsize(setFile) > 0:
-            outputSet = SetClass(filename=setFile)
-            outputSet.loadAllProperties()
-            outputSet.enableAppend()
+        """ This function is shared by Xmipp and CTFfind
+        estimation, or recalculate, protocols.
+        if is recalculate, it will iterated for each CTF model, see
+        if was recalculated and update with new defocus values.
+        Else, the function that should be implemented in each subclass.
+        """
+        if self.recalculate:
+            ctfSet = self._createSetOfCTF("_recalculated")
+            prot = self.continueRun.get() or self
+            if hasattr(prot, ProtCTFMicOutputs.outputCTF.name):
+                micSet = prot.outputCTF.getMicrographs()
+                # We suppose this is reading the ctf selection
+                # (with enabled/disabled) to only consider the enabled ones
+                # in the final SetOfCTF
+                # TODO: maybe we can remove the need of the extra text file
+                # with the recalculate parameters
+                newCount = 0
+                for ctfModel in self.recalculateSet:
+                    if ctfModel.isEnabled() and ctfModel.getObjComment():
+                        mic = ctfModel.getMicrograph()
+                        # Update the CTF models that where recalculated and append
+                        # later to the set, we don't want to copy the id here since
+                        # it is already correct
+                        newCtf = self._createCtfModel(mic, updateSampling=False)
+                        ctfModel.copy(newCtf, copyId=False)
+                        ctfModel.setEnabled(True)
+                        newCount += 1
+                    ctfSet.append(ctfModel)
+                ctfSet.setMicrographs(micSet)
+                self._defineOutputs(**{ProtCTFMicOutputs.outputCTF.name:ctfSet})
+                self._defineCtfRelation(micSet, ctfSet)
+                self._computeDefocusRange(ctfSet)
+                self.summaryVar.set("CTF Re-estimation of %d micrographs"
+                                    % newCount)
+            else:
+                raise Exception(
+                    pwutils.redStr("The outputCTF do not exist, all CTFs failed."))
+        else:
+            self._createOutputStep()
+            if self.outputCTF.getSize() == 0:
+                raise Exception(pwutils.redStr("outputCTF has size zero, all CTFs failed."
+                                               "Please review processing steps above."))
+
+    # -------------------------- INFO functions -------------------------------
+    def _summary(self):
+        summary = []
+
+        if self.recalculate:
+            if self.isFinished():
+                if self.summaryVar.hasValue():
+                    summary.append(self.summaryVar.get())
+            else:
+                summary.append(pwutils.Message.TEXT_NO_CTF_READY)
+        else:
+            if not hasattr(self, ProtCTFMicOutputs.outputCTF.name):
+                summary.append(pwutils.Message.TEXT_NO_CTF_READY)
+            else:
+                summary.append("CTF estimation of %d micrographs."
+                               % self.inputMicrographs.get().getSize())
+
+        return summary
+
+    def _methods(self):
+        methods = []
+
+        if hasattr(self, ProtCTFMicOutputs.outputCTF.name) and self.isFinished():
+            methods.append(self.methodsVar.get())
         else:
-            outputSet = SetClass(filename=setFile)
-            outputSet.setStreamState(outputSet.STREAM_OPEN)
+            methods.append(pwutils.Message.TEXT_NO_CTF_READY)
+
+        return methods
+
+    # -------------------------- UTILS functions ------------------------------
+    def _defineCtfParamsDict(self):
+        """ This function define a dictionary with parameters used
+        for CTF estimation that are common for all micrographs. """
+        # Get pointer to input micrographs
+        inputMics = self.getInputMicrographs()
+        acq = inputMics.getAcquisition()
+        sampling = inputMics.getSamplingRate()
+        downFactor = self.getAttributeValue('ctfDownFactor', 1.0)
+        if downFactor != 1.0:
+            sampling *= downFactor
+        self._params = {'voltage': acq.getVoltage(),
+                        'sphericalAberration': acq.getSphericalAberration(),
+                        'magnification': acq.getMagnification(),
+                        'ampContrast': acq.getAmplitudeContrast(),
+                        'samplingRate': sampling,
+                        'scannedPixelSize': inputMics.getScannedPixelSize(),
+                        'windowSize': self.windowSize.get(),
+                        'lowRes': self.lowRes.get(),
+                        'highRes': self.highRes.get(),
+                        # Convert from microns to Angstroms
+                        'minDefocus': self.minDefocus.get() * 1e+4,
+                        'maxDefocus': self.maxDefocus.get() * 1e+4
+                        }
+
+    def getCtfParamsDict(self):
+        """ Return a copy of the global params dict,
+        to avoid overwriting values. """
+        return self._params
+
+    def getRecalCtfParamsDict(self, ctfModel):
+        """ This function get the acquisition info of the micrographs"""
+        mic = ctfModel.getMicrograph()
+
+        acq = mic.getAcquisition()
+        mag = acq.getMagnification()
+        scannedPixelSize = mic.getSamplingRate() * mag / 10000
+        return {'voltage': acq.getVoltage(),
+                'sphericalAberration': acq.getSphericalAberration(),
+                'magnification': mag,
+                'ampContrast': acq.getAmplitudeContrast(),
+                'scannedPixelSize': scannedPixelSize,
+                'samplingRate': mic.getSamplingRate()
+                }
+
+    def _ctfCounter(self, values):
+        """ This function return the number of CTFs that was recalculated.
+        """
+        numberOfCTF = len(values) / 2
+        msg = "CTF Re-estimation of %d micrographs" % numberOfCTF
+        self.summaryVar.set(msg)
+
+    def _getInputCtf(self):
+        if self.continueRecal:
+            sqliteFile = self._getPath()
+        #             return self.outputCTF.get()
+        else:
+            return self.inputCtf.get()
+
+    def _iterMicrographs(self, inputMics=None):
+        """ Iterate over micrographs and yield
+        micrograph name. """
+        if inputMics is None:
+            inputMics = self.getInputMicrographs()
+
+        for mic in inputMics:
+            micFn = mic.getFileName()
+            yield micFn, mic
+
+    def _computeDefocusRange(self, ctfSet):
+        """ Compute the minimum and maximu defocus in a set of CTFs.
+        The protocol methodsVar will be updated with new values.
+
+        Params:
+            ctfSet: the set of CTFs to compute min and max
+        """
+        defocusList = []
+
+        for ctf in ctfSet:
+            defocusList.append(ctf.getDefocusU())
+            defocusList.append(ctf.getDefocusV())
+
+        minD = min(defocusList) / 10000.
+        maxD = max(defocusList) / 10000.
+
+        self.methodsVar.set("Estimated  defocus range defocus was"
+                            " %0.3f - %0.3f microns. " % (minD, maxD))
 
-            inputMovies = self.inputMovies.get()
-            outputSet.copyInfo(inputMovies)
+        self._store(self.methodsVar)
 
-            if fixSampling:
-                newSampling = inputMovies.getSamplingRate() * self._getBinFactor()
-                outputSet.setSamplingRate(newSampling)
+    def _defocusMaxMin(self, defocusList):
+        """ This function return the minimum and maximum of the defocus
+        of a SetOfMicrographs.
+        """
+        raise Exception("DEPRECATED")
+
+    def getInputMicrographsPointer(self):
+        return self.inputMicrographs
 
-        return outputSet
+    def getInputMicrographs(self):
+        return self.getInputMicrographsPointer().get()
+
+    def _getCtfArgs(self):
+        """ Should be implemented in sub-classes to define the argument
+        list that should be passed to the estimation step function.
+        """
+        return []
+
+    # ------ Methods for Streaming CTF --------------
+    def _stepsCheck(self):
+        # To allow streaming ctf estimation we need to detect:
+        #   1) new micrographs ready to be estimated
+        #   2) new output ctfs that have been produced and add then
+        #      to the output set.
+
+        # For now the streaming is not allowed for recalculate CTF
+        if self.recalculate:
+            return
+        self._checkNewInput()
+        self._checkNewOutput()
+
+    def _checkNewInput(self):
+        # Check if there are new micrographs to process from the input set
+        localFile = self.getInputMicrographs().getFileName()
+        now = datetime.now()
+        self.lastCheck = getattr(self, 'lastCheck', now)
+        mTime = datetime.fromtimestamp(getmtime(localFile))
+        self.debug('Last check: %s, modification: %s'
+                   % (pwutils.prettyTime(self.lastCheck),
+                      pwutils.prettyTime(mTime)))
+        # If the input micrographs.sqlite have not changed since our last check,
+        # it does not make sense to check for new input data
+        if self.lastCheck > mTime and hasattr(self, 'listOfMics'):
+            return None
+
+        self.lastCheck = now
+        # Open input micrographs.sqlite and close it as soon as possible
+        micDict, self.streamClosed = self._loadInputList()
+        newMics = micDict.values()
+        outputStep = self._getFirstJoinStep()
+
+        if newMics:
+            fDeps = self._insertNewMicsSteps(newMics)
+            if outputStep is not None:
+                outputStep.addPrerequisites(*fDeps)
+            self.updateSteps()
 
     def _checkNewOutput(self):
         if getattr(self, 'finished', False):
             return
-
         # Load previously done items (from text file)
         doneList = self._readDoneList()
         # Check for newly done items
-        newDone = [m for m in self.listOfMovies
-                   if m.getObjId() not in doneList and self._isMovieDone(m)]
+        listOfMics = self.micDict.values()
+        nMics = len(listOfMics)
+        newDone = [m for m in listOfMics
+                   if m.getObjId() not in doneList and self._isMicDone(m)]
 
-        # Update the file with the newly done movies
-        # or exit from the function if no new done movies
+        # Update the file with the newly done mics
+        # or exit from the function if no new done mics
         self.debug('_checkNewOutput: ')
-        self.debug('   listOfMovies: %s, doneList: %s, newDone: %s'
-                   % (len(self.listOfMovies), len(doneList), len(newDone)))
+        self.debug('   listOfMics: %s, doneList: %s, newDone: %s'
+                   % (nMics, len(doneList), len(newDone)))
 
-        firstTime = len(doneList) == 0
         allDone = len(doneList) + len(newDone)
-        # We have finished when there is not more input movies (stream closed)
-        # and the number of processed movies is equal to the number of inputs
-        self.finished = self.streamClosed and allDone == len(self.listOfMovies)
+        # We have finished when there is not more input mics (stream closed)
+        # and the number of processed mics is equal to the number of inputs
+        self.finished = self.streamClosed and allDone == nMics
         streamMode = pwobj.Set.STREAM_CLOSED if self.finished else pwobj.Set.STREAM_OPEN
+        self.debug('   streamMode: %s newDone: %s' % (streamMode,
+                                                      not (newDone == [])))
 
         if newDone:
-            self._writeDoneList(newDone)
-
+            newDoneUpdated = self._updateOutputCTFSet(newDone, streamMode)
+            self._writeDoneList(newDoneUpdated)
         elif not self.finished:
             # If we are not finished and no new output have been produced
             # it does not make sense to proceed and updated the outputs
             # so we exit from the function here
+
+            # Maybe it would be good idea to take a snap to avoid
+            # so much IO if this protocol does not have much to do now
+            if allDone == nMics:
+                self._streamingSleepOnWait()
+
             return
 
         self.debug('   finished: %s ' % self.finished)
         self.debug('        self.streamClosed (%s) AND' % self.streamClosed)
-        self.debug('        allDone (%s) == len(self.listOfMovies (%s)'
-                   % (allDone, len(self.listOfMovies)))
-        self.debug('   streamMode: %s' % streamMode)
-
-        if self._createOutputMovies():
-            saveMovie = self.getAttributeValue('doSaveMovie', False)
-            movieSet = self._loadOutputSet(emobj.SetOfMovies, 'movies.sqlite',
-                                           fixSampling=saveMovie)
-
-            # If need to save the movie
-            if saveMovie:
-                movieSet.setGain(None)
-                movieSet.setDark(None)
-
-            for movie in newDone:
-                try:
-                    newMovie = self._createOutputMovie(movie)
-                    if newMovie.getAlignment().getShifts()[0]:
-                        movieSet.append(newMovie)
-                    else:
-                        print(pwutils.yellowStr("WARNING: Movie %s has empty alignment "
-                                                "data, can't add it to output set."
-                                                % movie.getFileName()))
-
-                # Warn about any exception creating the movie
-                except Exception as e:
-                    print(pwutils.redStr("ERROR: Movie %s couldn't be "
-                                         "added to the output set.\n%s"
-                                         % (movie.getFileName(), e)))
-
-            self._updateOutputSet('outputMovies', movieSet, streamMode)
-
-            if firstTime:
-                # Probably is a good idea to store a cached summary for the
-                # first resulting movie of the processing.
-                self._storeSummary(newDone[0])
-                # If the movies are not written out, then dimensions can be
-                # copied from the input movies
-                if not saveMovie:
-                    movieSet.setDim(self.inputMovies.get().getDim())
-                self._defineTransformRelation(self.inputMovies, movieSet)
-
-        def _updateOutputMicSet(sqliteFn, getOutputMicName, outputName):
-            """ Updated the output micrographs set with new items found. """
-            micSet = self._loadOutputSet(emobj.SetOfMicrographs, sqliteFn)
-            doneFailed = []
-
-            for movie in newDone:
-                mic = micSet.ITEM_TYPE()
-                mic.copyObjId(movie)
-                mic.setMicName(movie.getMicName())
-                # The subclass protocol is responsible of generating the output
-                # micrograph file in the extra path with the required name
-                extraMicFn = self._getExtraPath(getOutputMicName(movie))
-                mic.setFileName(extraMicFn)
-                if not os.path.exists(extraMicFn):
-                    print(pwutils.yellowStr("WARNING: Micrograph %s was not generated, "
-                                            "can't add it to output set." % extraMicFn))
-                    doneFailed.append(movie)
-                    continue
-                # Tolerate errors here. Usually here some plots are generated.
-                try:
-                    self._preprocessOutputMicrograph(mic, movie)
-                except Exception as e:
-                    self.error("Couldn't prepare output details: %s" % e)
-                    doneFailed.append(movie)
-                    continue
-
-                micSet.append(mic)
-
-            self._updateOutputSet(outputName, micSet, streamMode)
-            if doneFailed:
-                self._writeFailedList(doneFailed)
-
-            if firstTime:
-                # We consider that Movies are 'transformed' into the Micrographs
-                # This will allow to extend the CTF associated to a set of
-                # micrographs to another set of micrographs generated from a
-                # different movie alignment
-                self._defineTransformRelation(self.inputMovies, micSet)
-
-        if self._createOutputMicrographs():
-            _updateOutputMicSet('micrographs.sqlite',
-                                self._getOutputMicName,
-                                'outputMicrographs')
-
-        if self._createOutputWeightedMicrographs():
-            _updateOutputMicSet('micrographs_dose-weighted.sqlite',
-                                self._getOutputMicWtName,
-                                'outputMicrographsDoseWeighted')
+        self.debug('        allDone (%s) == len(self.listOfMics (%s)'
+                   % (allDone, nMics))
 
         if self.finished:  # Unlock createOutputStep if finished all jobs
+            self._updateStreamState(streamMode)
             outputStep = self._getFirstJoinStep()
             if outputStep and outputStep.isWaiting():
                 outputStep.setStatus(pwcts.STATUS_NEW)
 
-    # --------------------------- INFO functions ------------------------------
-    def _validate(self):
-        errors = []
-
-        # Only validate about cropDimensions if the protocol supports them
-        if (hasattr(self, 'cropDimX') and hasattr(self, 'cropDimY')
-                and (self.cropDimX > 0 >= self.cropDimY
-                     or self.cropDimX <= 0 < self.cropDimY)):
-            errors.append("If you give cropDimX, you should also give "
-                          "cropDimY and vice versa")
-
-        inputMovies = self.inputMovies.get()
-
-        # Do not continue if there ar no movies. Validation message will
-        # take place since attribute is a Pointer.
-        if inputMovies is None:
-            return errors
-
-        firstItem = inputMovies.getFirstItem()
-
-        firstFrame, lastFrame, _ = inputMovies.getFramesRange()
-        if lastFrame == 0:
-            # Although getFirstItem is not recommended in general, here it is
-            # used only once, for validation purposes, so performance
-            # problems should not appear.
-            frames = firstItem.getNumberOfFrames()
-            lastFrame = frames
+    def _loadInputList(self):
+        """ Load the input set of micrographs that are ready to be estimated. """
+        return self._loadSet(self.getInputMicrographs(), emobj.SetOfMicrographs,
+                             lambda mic: mic.getMicName())
+
+    def _loadSet(self, inputSet, SetClass, getKeyFunc):
+        """ Load a given input set if their items are not already present
+        in the self.micDict.
+        This can be used to load new micrographs for estimation as well as
+        new CTF (if used) in streaming.
+        """
+        setFn = inputSet.getFileName()
+        self.debug("Loading input db: %s" % setFn)
+        updatedSet = SetClass(filename=setFn)
+        updatedSet.loadAllProperties()
+        newItemDict = OrderedDict()
+        for item in updatedSet:
+            micKey = getKeyFunc(item)
+            if micKey not in self.micDict:
+                newItemDict[micKey] = item.clone()
+        streamClosed = updatedSet.isStreamClosed()
+        updatedSet.close()
+        self.debug("Closed db.")
+
+        return newItemDict, streamClosed
+
+    def _updateOutputCTFSet(self, micList, streamMode):
+        doneFailed = []
+        micDoneList = [mic for mic in micList]
+        # Do no proceed if there is not micrograph ready
+        if not micDoneList:
+            return []
+
+        outputName = ProtCTFMicOutputs.outputCTF.name
+        outputCtf = getattr(self, outputName, None)
+
+        # If there is not outputCTF yet, it means that is the first
+        # time we are updating output CTFs, so we need to first create
+        # the output set
+        firstTime = outputCtf is None
+
+        if firstTime:
+            outputCtf = self._createSetOfCTF()
+            outputCtf.setMicrographs(self.getInputMicrographsPointer())
         else:
-            frames = lastFrame - firstFrame + 1
+            outputCtf.enableAppend()
 
-        if frames is not None:
-            def _validateRange(prefix):
-                # Avoid validation when the range is not defined
-                if not hasattr(self, '%sFrame0' % prefix):
-                    return
-
-                f0, fN = self._getFrameRange(frames, prefix)
-                if fN < firstFrame or fN > lastFrame:
-                    errors.append("Check the selected last frame to *%s*. "
-                                  "Last frame (%d) should be in range: %s "
-                                  % (prefix.upper(), fN, (firstFrame,
-                                                          lastFrame)))
-                if f0 < firstFrame or f0 > lastFrame:
-                    errors.append("Check the selected first frame to *%s*. "
-                                  "First frame (%d) should be in range: %s "
-                                  % (prefix.upper(), f0, (firstFrame,
-                                                          lastFrame)))
-                if fN < f0:
-                    errors.append("Check the selected frames range to *%s*. "
-                                  "Last frame (%d) should be greater or equal "
-                                  "than first frame (%d)"
-                                  % (prefix.upper(), fN, f0))
-
-            _validateRange("align")
-            _validateRange("sum")
-
-        if not emlib.image.ImageHandler().existsLocation(firstItem.getLocation()):
-            errors.append("The input movie files do not exist!!! "
-                          "Since usually input movie files are symbolic links, "
-                          "please check that links are not broken if you "
-                          "moved the project folder. ")
+        for micFn, mic in self._iterMicrographs(micList):
+            try:
+                ctf = self._createCtfModel(mic)
+                outputCtf.append(ctf)
+            except Exception as ex:
+                print(pwutils.yellowStr("Missing CTF?: Couldn't update CTF set with mic: %s" % micFn))
+                doneFailed.append(mic)
+
+        self.debug(" _updateOutputCTFSet Stream Mode: %s " % streamMode)
+        self._updateOutputSet(outputName, outputCtf, streamMode)
+        if doneFailed:
+            self._writeFailedList(doneFailed)
+
+        if firstTime:  # define relation just once
+            # Using a pointer to define the relations is more robust to
+            # scheduling and id changes between the protocol run.db and
+            # the main project database.get
+            self._defineCtfRelation(self.getInputMicrographsPointer(),
+                                    outputCtf)
+
+        return micDoneList
+
+    def _updateStreamState(self, streamMode):
+        outputName = ProtCTFMicOutputs.outputCTF.name
+        outputCtf = getattr(self, outputName, None)
+
+        # If there are not outputCTFs yet, it means that is the first
+        # time we are updating output CTF, so we need to first create
+        # the output set
+        firstTime = outputCtf is None
 
-        return errors
-
-    # --------------------------- INFO functions -------------------------------
-    def _summary(self):
-        return [self.summaryVar.get('')]
-
-    # --------------------------- UTILS functions ----------------------------
-    def _useAlignToSum(self):
-        return self.getAttributeValue('useAlignToSum', False)
-
-    def _getFrameRange(self, n, prefix):
-        """
-        Params:
-        :param n: Number of frames of the movies
-        :param prefix: what range we want to consider, either 'align' or 'sum'
-        :return: (i, f) initial and last frame range
-        """
-        # In case that the user select the same range for ALIGN and SUM
-        # we also use the 'align' prefix
-        if self._useAlignToSum():
-            prefix = 'align'
-
-        first = self.getAttributeValue('%sFrame0' % prefix)
-        last = self.getAttributeValue('%sFrameN' % prefix)
-
-        if first <= 1:
-            first = 1
-
-        if last <= 0:
-            last = n
-
-        return first, last
-
-    def _createOutputMovie(self, movie):
-        movieId = movie.getObjId()
-
-        # Parse the alignment parameters and store the log files
-        alignedMovie = movie.clone()
-        n = movie.getNumberOfFrames()
-        first, last = self._getFrameRange(n, 'align')
-        framesRange = alignedMovie.getFramesRange()
-        framesRange.setFirstFrame(first)
-        framesRange.setLastFrame(last)
-        # Check if user selected to save movie, use the getAttributeValue
-        # function for allow the protocol to not define this flag
-        # and use False as default
-        if self.getAttributeValue('doSaveMovie', False):
-            # The subclass protocol is responsible of generating the output
-            # movie file in the extra path with the required name
-            extraMovieFn = self._getExtraPath(self._getOutputMovieName(movie))
-            alignedMovie.setFileName(extraMovieFn)
-            # When the output movies are saved, the shifts
-            # will be set to zero since they are aligned
-            totalFrames = last - first + 1
-            xshifts = [0] * totalFrames
-            yshifts = xshifts
-            # If we save the movies, we need to modify which are the index
-            # of the first frame in the stack, now is 1 since the stack is
-            # written only with the given frames
-            firstFrameIndex = 1
+        if firstTime:
+            outputCtf = self._createSetOfCTF()
         else:
-            xshifts, yshifts = self._getMovieShifts(movie)
-            firstFrameIndex = first
-
-        framesRange.setFirstFrameIndex(firstFrameIndex)
-        alignment = emobj.MovieAlignment(first=first, last=last, xshifts=xshifts,
-                                         yshifts=yshifts)
-
-        roiList = [self.getAttributeValue(s, 0) for s in
-                   ['cropOffsetX', 'cropOffsetY', 'cropDimX', 'cropDimY']]
-        alignment.setRoi(roiList)
-        alignedMovie.setAlignment(alignment)
-
-        return alignedMovie
-
-    # ---------- Hook functions that need to be implemented in subclasses ------
-    def _getBinFactor(self):
-        return self.getAttributeValue('binFactor', 1.0)
-
-    def _getMovieRoot(self, movie):
-        # Try to use the 'original' fileName in case it is present
-        # the original could be different from the current filename if
-        # we are dealing with compressed movies (e.g., movie.mrc.bz2)
-        fn = movie.getAttributeValue('_originalFileName',
-                                     movie.getFileName())
-        # Remove the first extension
-        fnRoot = pwutils.removeBaseExt(fn)
-        # Check if there is a second extension
-        # (Assuming is is only a dot and 3 or 4 characters after it
-        # Do not perform this check if the file name is short
-        if len(fnRoot) > 5:
-            if fnRoot[-4] == '.' or fnRoot[-5] == '.':
-                fnRoot = pwutils.removeExt(fnRoot)
-
-        return fnRoot
-
-    def _getOutputMovieName(self, movie):
-        """ Returns the name of the output movie.
-        (relative to micFolder)
-        """
-        return self._getMovieRoot(movie) + '_aligned_movie.mrcs'
-
-    def _getOutputMicName(self, movie):
-        """ Returns the name of the output micrograph
-        (relative to micFolder)
-        """
-        return self._getMovieRoot(movie) + '_aligned_mic.mrc'
-
-    def _getOutputMicWtName(self, movie):
-        """ Returns the name of the output dose-weighted micrograph
-        (relative to micFolder)
-        """
-        return self._getMovieRoot(movie) + '_aligned_mic_DW.mrc'
-
-    def _getOutputMicThumbnail(self, movie):
-        return self._getExtraPath(self._getMovieRoot(movie) + '_thumbnail.png')
-
-    def _getMovieShifts(self, movie):
-        """ Returns the x and y shifts for the alignment of this movie.
-         The shifts should refer to the original micrograph without any binning.
-         In case of a binning greater than 1, the shifts should be scaled.
-        """
-        return [], []
-
-    def _createOutputMovies(self):
-        """ Returns True if an output set of movies will be generated.
-        The most common case is to always generate output movies,
-        either with alignment only or the binary aligned movie files.
-        Subclasses can override this function to change this behavior.
-        """
-        return True
-
-    def _createOutputMicrographs(self):
-        """ By default check if the user have selected 'doSaveAveMic'
-        property. Subclasses can override this method to implement different
-        behaviour.
-        """
-        return self.getAttributeValue('doSaveAveMic', True)
-
-    def _createOutputWeightedMicrographs(self):
-        return False
-
-    def _preprocessOutputMicrograph(self, mic, movie):
-        """ Hook function that will be call before adding the micrograph
-        to the output set of micrographs.
-        """
-        pass
-
-    def _doComputeMicThumbnail(self):
-        """ Should be implemented in sub-classes if want to check
-        the generation of thumbnails.
-        """
-        return False
-
-    def _storeSummary(self, movie):
-        """ Implement this method if you want to store the summary. """
-        pass
+            outputCtf.enableAppend()
 
-    def _getCorrectedDose(self, movieSet):
-        """get and correct the pre-exposure dose. It is important for cases
-        in which the first frame is different of one. The method support both
-        movie and sets of movies"""
-
-        firstFrame, _, _ = movieSet.getFramesRange()
-        preExp = movieSet.getAcquisition().getDoseInitial()
-        dose = movieSet.getAcquisition().getDosePerFrame()
-        preExp += dose * (firstFrame - 1)
-
-        return preExp, dose
-
-    def __runXmippProgram(self, program, args):
-        """ Internal shortcut function to launch a Xmipp program. """
-        from pwem import Domain
-        xmipp3 = Domain.importFromPlugin('xmipp3')
-        xmipp3.Plugin.runXmippProgram(program, args)
-
-    def __runEman2Program(self, program, args):
-        """ Internal workaround to launch an EMAN2 program. """
-        from pwem import Domain
-        eman2 = Domain.importFromPlugin('eman2')
-        from pyworkflow.utils.process import runJob
-        runJob(self._log, eman2.Plugin.getProgram(program), args,
-               env=eman2.Plugin.getEnviron())
-
-    def averageMovie(self, movie, inputFn, outputMicFn, binFactor=1, roi=None,
-                     dark=None, gain=None, splineOrder=None):
-        """ Average a movie (using xmipp) taking into account the
-         possible shifts and other alignment parameters.
-         Params:
-            inputFn: input filename, either the movie file or a metadata
-                with the shifts and other info.
-            dark: dark file
-            gain: gain correction file.
-
-         The output will be the averaged micrograph.
-        """
-        args = '-i %s ' % inputFn
-        args += '--sampling %f ' % movie.getSamplingRate()
-        args += '--useInputShifts '
-
-        if binFactor > 1:
-            args += '--bin %f ' % binFactor
-
-        if roi is not None:
-            x, y, _ = movie.getDim()
-            offsetX, offsetY, cropDimX, cropDimY = roi
-            # cropDim value is <= 0 we should take the whole size
-            if cropDimX <= 0:
-                dimX = x - 1
-            else:
-                dimX = offsetX + cropDimX - 1
-
-            if cropDimY <= 0:
-                dimY = y - 1
-            else:
-                dimY = offsetY + cropDimY - 1
-
-            args += '--cropULCorner %d %d ' % (offsetX, offsetY)
-            args += '--cropDRCorner %d %d ' % (dimX, dimY)
+        self.debug(" _updateStreamState Stream Mode: %s " % streamMode)
+        self._updateOutputSet(outputName, outputCtf, streamMode)
 
-        args += ' --oavg %s ' % outputMicFn
-        args += ' --Bspline %d ' % (splineOrder if splineOrder else 1)
-
-        if dark is not None:
-            args += ' --dark ' + dark
-
-        if gain is not None:
-            args += ' --gain ' + gain
-
-        self.__runXmippProgram('xmipp_movie_alignment_correlation', args)
-
-    def computePSD(self, inputMic, oroot, dim=384,  # 384 = 128 + 256, which should be fast for any Fourier Transformer
-                   overlap=0.4):
-        warnings.warn("Use psd = image.computePSD(overlap=0.4, xdim=384, ydim=384, fftthreads=1) instead",
-                      DeprecationWarning)
-        ih = emlib.image.ImageHandler()
-        psdImg1 = ih.read(inputMic)
-        res = psdImg1.computePSD(overlap, dim, dim)
-        res.write(oroot + ".psd")
-
-    def composePSDImages(self, psdImg1, psdImg2, outputFn,
-                         outputFnUncorrected=None, outputFnCorrected=None):
-        """ Compose a single PSD image:
-         left part from psd1 (uncorrected PSD),
-         right-part from psd2 (corrected PSD)
-        """
-        data1 = psdImg1.getData()  # get the data now, as conversion would change them
-        if outputFnUncorrected is not None:
-            psdImg1.convertPSD()
-            psdImg1.write(outputFnUncorrected)
-
-        data2 = psdImg2.getData()  # get the data now, as conversion would change them
-        if outputFnCorrected is not None:
-            psdImg2.convertPSD()
-            psdImg2.write(outputFnCorrected)
-
-        # Compute middle index
-        x, _, _, _ = psdImg1.getDimensions()
-        m = int(round(x / 2.))
-        data1[:, :m] = data2[:, :m]
-        psdImg1.setData(data1)
-        psdImg1.write(outputFn)
-
-    def composePSD(self, psd1, psd2, outputFn,
-                   outputFnUncorrected=None, outputFnCorrected=None):
-        import warnings
-        warnings.warn("Use composePSDImages() instead", DeprecationWarning)
-        """ Compose a single PSD image:
-         left part from psd1 (uncorrected PSD),
-         right-part from psd2 (corrected PSD)
-        """
-        ih = emlib.image.ImageHandler()
-        self.composePSDImages(ih.read(psd1), ih.read(psd2), outputFn,
-                              outputFnUncorrected, outputFnCorrected)
-
-    def computePSDImages(self, movie, fnUncorrected, fnCorrected,
-                         outputFnUncorrected=None, outputFnCorrected=None):
-        self.composePSDImages(
-            emlib.image.ImageHandler().read(fnUncorrected).computePSD(),
-            emlib.image.ImageHandler().read(fnCorrected).computePSD(),
-            self._getPsdCorr(movie),
-            outputFnUncorrected,
-            outputFnCorrected)
-
-    def computePSDs(self, movie, fnUncorrected, fnCorrected,
-                    outputFnUncorrected=None, outputFnCorrected=None):
-        import warnings
-        warnings.warn("Use computePSDImages() instead", DeprecationWarning)
-        self.computePSDImages(movie, fnUncorrected, fnCorrected,
-                              outputFnUncorrected, outputFnCorrected)
-
-    def computeThumbnail(self, inputFn, scaleFactor=6, outputFn=None):
-        """ Generates a thumbnail of the input file"""
-        outputFn = outputFn or self.getThumbnailFn(inputFn)
-        args = "%s %s " % (inputFn, outputFn)
-        args += "--meanshrink %s --fixintscaling=sane" % scaleFactor
-
-        self.__runEman2Program('e2proc2d.py', args)
-
-        return outputFn
-
-    def correctGain(self, movieFn, outputFn, gainFn=None, darkFn=None):
-        """correct a movie with both gain and dark images"""
-        ih = emlib.image.ImageHandler()
-        _, _, z, n = ih.getDimensions(movieFn)
-        numberOfFrames = max(z, n)  # in case of wrong mrc stacks as volumes
-
-        def _readImgFloat(fn):
-            img = None
-            if fn:
-                img = ih.read(fn)
-                img.convert2DataType(emlib.DT_FLOAT)
-            return img
-
-        gainImg = _readImgFloat(gainFn)
-        darkImg = _readImgFloat(darkFn)
-
-        img = ih.createImage()
-
-        for i in range(1, numberOfFrames + 1):
-            img.read((i, movieFn))
-            img.convert2DataType(emlib.DT_FLOAT)
-
-            if darkImg:
-                img.inplaceSubtract(darkImg)
-            if gainImg:
-                img.inplaceMultiply(gainImg)
-
-            img.write((i, outputFn))
-
-    def getThumbnailFn(self, inputFn):
-        """ Returns the default name for a thumbnail image"""
-        return pwutils.replaceExt(inputFn, "thumb.png")
-
-    def _getPsdCorr(self, movie):
-        """ This should be implemented in subclasses."""
-        pass
+    def _readDoneList(self):
+        """ Read from a text file the id's of the items that have been done. """
+        doneFile = self._getAllDone()
+        doneList = []
+        # Check what items have been previously done
+        if exists(doneFile):
+            with open(doneFile) as f:
+                doneList += [int(line.strip()) for line in f]
+        return doneList
+
+    def _writeDoneList(self, micList):
+        """ Write to a text file the items that have been done. """
+        doneFile = self._getAllDone()
+
+        if not exists(doneFile):
+            pwutils.makeFilePath(doneFile)
+
+        with open(doneFile, 'a') as f:
+            for mic in micList:
+                f.write('%d\n' % mic.getObjId())
+
+    def _isMicDone(self, mic):
+        """ A mic is done if the marker file exists. """
+        return exists(self._getMicrographDone(mic))
+
+    def _getAllDone(self):
+        return self._getExtraPath('DONE', 'all.TXT')
+
+    def _getAllFailed(self):
+        return self._getExtraPath('FAILED_all.TXT')
+
+    def _getMicrographDir(self, mic):
+        """ Return an unique dir name for results of the micrograph. """
+        return self._getTmpPath('mic_%04d' % mic.getObjId())
+
+    def _getMicrographDone(self, mic):
+        """ Return the file that is used as a flag of termination. """
+        return self._getExtraPath('DONE', 'mic_%06d.TXT' % mic.getObjId())
 
-    def _writeFailedList(self, movieList):
+    def _writeFailedList(self, micList):
         """ Write to a text file the items that have failed. """
         with open(self._getAllFailed(), 'a') as f:
-            for movie in movieList:
-                f.write('%d\n' % movie.getObjId())
+            for mic in micList:
+                f.write('%d\n' % mic.getObjId())
 
     def _readFailedList(self):
         """ Read from a text file the id's of the items that have failed. """
         failedFile = self._getAllFailed()
         failedList = []
-        if os.path.exists(failedFile):
+        if exists(failedFile):
             with open(failedFile) as f:
                 failedList += [int(line.strip()) for line in f]
 
         return failedList
 
 
-def createAlignmentPlot(meanX, meanY):
-    """ Create a plotter with the cumulative shift per frame. """
-    figureSize = (8, 6)
-    plotter = Plotter(*figureSize)
-    figure = plotter.getFigure()
-
-    ax = figure.add_subplot(111)
-    ax.grid()
-    ax.axis('equal')
-    ax.set_title('Cartesian representation')
-    ax.set_xlabel('Drift x (pixels)')
-    ax.set_ylabel('Drift y (pixels)')
-
-    # Max range of the plot of the two coordinates
-    plotRange = max(max(meanX) - min(meanX), max(meanY) - min(meanY))
-    i = 1
-    skipLabels = ceil(len(meanX) / 10.0)
-    for x, y in izip(meanX, meanY):
-        if i % skipLabels == 0:
-            ax.text(x - 0.02 * plotRange, y + 0.02 * plotRange, str(i))
-        i += 1
-
-    ax.plot(meanX, meanY, color='b')
-    ax.plot(meanX, meanY, 'yo')
-
-    # setting the plot windows to properly see the data
-    ax.axis([min(meanX) - 0.1 * plotRange, max(meanX) + 0.1 * plotRange,
-             min(meanY) - 0.1 * plotRange, max(meanY) + 0.1 * plotRange])
-
-    plotter.tightLayout()
-
-    return plotter
-
-
-class ProtAverageFrames(ProtAlignMovies):
-    """
-    Very simple protocol to align all the frames of a given data collection
-    session. It can be used as a sanity check.
-    """
-    _label = 'average frames'
-
-    # -------------------------- DEFINE param functions -----------------------
-    def _defineAlignmentParams(self, form):
-        pass
-
-    def _processMovie(self, movie):
-        allFramesSum = self._getPath('all_frames_sum.mrc')
-        ih = emlib.image.ImageHandler()
-        sumImg = ih.createImage()
-        img = ih.createImage()
-
-        n = movie.getNumberOfFrames()
-        fn = movie.getFileName()
-
-        sumImg.read((1, fn))
-
-        for frame in range(2, n + 1):
-            img.read((frame, fn))
-            sumImg.inplaceAdd(img)
-
-        if os.path.exists(allFramesSum):
-            img.read(allFramesSum)
-            sumImg.inplaceAdd(img)
-
-        sumImg.write(allFramesSum)
-
-    # FIXME: Methods will change when using the streaming for the output
-    def createOutputStep(self):
-        # Really load the input, since in the streaming case we can not
-        # use the self.inputMovies directly
-        allFramesSum = self._getPath('all_frames_sum.mrc')
-        allFramesAvg = self._getPath('all_frames_avg.mrc')
-        self._loadInputList()
-        n = len(self.listOfMovies)
-
-        ih = emlib.image.ImageHandler()
-        sumImg = ih.read(allFramesSum)
-        sumImg.inplaceDivide(float(n))
-        sumImg.write(allFramesAvg)
-
-        outputAvg = emobj.Image()
-        outputAvg.setFileName(allFramesAvg)
-        outputAvg.setSamplingRate(self.listOfMovies[0].getSamplingRate())
-        self._defineOutputs(outputAverage=outputAvg)
-        self._defineSourceRelation(self.inputMovies, outputAvg)
-
-    def _validate(self):
-        return []
-
-    def _summary(self):
-        return []
-
-    def _createOutputMovies(self):
-        """ Returns True if an output set of movies will be generated.
-        The most common case is to always generate output movies,
-        either with alignment only or the binary aligned movie files.
-        Subclasses can override this function to change this behavior.
-        """
-        return False
-
-    def _createOutputMicrographs(self):
-        """ By default check if the user have selected 'doSaveAveMic'
-        property. Subclasses can override this method to implement different
-        behaviour.
-        """
-        return False
-
-    def _createOutputWeightedMicrographs(self):
-        return False
+class ProtPreprocessMicrographs(ProtMicrographs):
+    pass
```

### Comparing `scipion-em-3.0.9/pwem/protocols/protocol_alignment_assign.py` & `scipion-em-3.1.0/pwem/protocols/protocol_alignment_assign.py`

 * *Files 26% similar despite different names*

```diff
@@ -23,119 +23,142 @@
 # *  e-mail address 'scipion@cnb.csic.es'
 # *
 # **************************************************************************
 
 
 import pyworkflow.protocol.params as params
 from pyworkflow.object import Integer
+from pwem.objects import SetOfParticles
 
 from .protocol_2d import ProtAlign2D
 
 
 class ProtAlignmentAssign(ProtAlign2D):
-    """ Assign a the alignment calculated for a set of particles to another set.
+    """ Assign the alignment calculated for a set of particles to another set.
     This protocol will take into account the differences of pixel size (A/pix)
     between the two sets and multiply by the right factor the shifts.
     The particles with the alignment can also be a subset of the other images
     """
     _label = 'assign alignment'
+    OUTPUT_NAME ='outputParticles'
+    IGNORE_LABEL = 'Ignore fractional shifts'
+    _possibleOutputs = {OUTPUT_NAME: SetOfParticles}
 
     def _defineParams(self, form):
         form.addSection(label='Input')
 
-        form.addParam('inputParticles', params.PointerParam, pointerClass='SetOfParticles',
+        form.addParam('inputParticles', params.PointerParam, pointerClass=SetOfParticles,
                       label='Input particles',
                       help='Select the particles that you want to update the new alignment.')
-        form.addParam('inputAlignment', params.PointerParam, pointerClass='SetOfParticles',
+        form.addParam('inputAlignment', params.PointerParam, pointerClass=SetOfParticles,
                       label="Input alignments",
                       help='Select the particles with alignment to be apply to the other particles.')
         form.addParam('assignRandomSubsets', params.BooleanParam, default=True,
                       expertLevel=params.LEVEL_ADVANCED,
                       label="Assign random subsets?",
                       help="If yes, the random subset information from the "
                            "assignment input will be transferred to the output "
                            "particles.")
+        form.addBooleanParam('ignoreFractionalShift',
+                             label=self.IGNORE_LABEL,
+                             help='When extracting coordinates, the integer part of the shifts from the alignment'
+                                  ' can be transferred to the 2d coordinate. The remaining decimal part is stored'
+                                  ' as xFrac and yFrac in the particles. Leave this active if you want current alignment'
+                                  ' shifts to be used, IGNORING the decimal fraction that might be annotated in case this'
+                                  ' set comes from an "extract coordinates" and you chose to "Apply particle shifts?"',
+                             default=True)
 
         form.addParallelSection(threads=0, mpi=0)
 
 # --------------------------- INSERT steps functions --------------------------
 
     def _insertAllSteps(self):
         """for each ctf insert the steps to compare it
         """
-        self._insertFunctionStep('createOutputStep')
+        self._insertFunctionStep(self.createOutputStep)
 
     def _updateItem(self, item, row):
         """ Implement this function to do some
         update actions over each single item
         that will be stored in the output Set.
         """
-        # Add alignment info from corresponding item on inputAlignment
-        inputAlignment = self.inputAlignment.get()
-        scale = inputAlignment.getSamplingRate()/self.inputParticles.get().getSamplingRate()
 
-        alignedParticle = inputAlignment[item.getObjId()]
+        alignedParticle = self.alignmentData[item.getObjId()]
         # If alignment is found for this particle set the alignment info
         # on the output particle, if not do not write that item
         if alignedParticle is not None:
             alignment = alignedParticle.getTransform()
 
             # If shifts Applied before at extraction coordinate time
-            if item.hasCoordinate() and hasattr(item.getCoordinate(), "xFrac"):
+            if not self.ignoreFractionalShift.get() and self.hasFractions():
                 coord = item.getCoordinate()
 
-                alignedParticle = inputAlignment[item.getObjId()]
-
                 alignment.invert()
                 alignment.setShifts(-coord.xFrac.get(),
                                 -coord.yFrac.get(),
                                 0)
                 alignment.invert()
+
+                # remove the attribute since it has been already applied
+                del coord.xFrac
+                del coord.yFrac
+
             else:
-                alignment.scaleShifts(scale)
+                alignment.scaleShifts(self.scale)
 
             item.setTransform(alignment)
 
             if self.assignRandomSubsets:
                 subset = \
                     alignedParticle.getAttributeValue('_rlnRandomSubset', None)
                 if subset is not None:
                     item._rlnRandomSubset = Integer(subset)
         else:
             item._appendItem = False
 
     def createOutputStep(self):
+
         inputParticles = self.inputParticles.get()
-        inputAlignment = self.inputAlignment.get()
+
+        # Store data to be used in the update item
+        self.alignmentData = self.inputAlignment.get()
+
+        # Trigger the connection to avoid connecting and disconnecting later when using self.alignmentData[23]
+        self.alignmentData.load()
+        self.scale = self.alignmentData.getSamplingRate()/inputParticles.getSamplingRate()
+
+        # Add alignment info from corresponding item on inputAlignment
+        # Output
         outputParticles = self._createSetOfParticles()
         outputParticles.copyInfo(inputParticles)
-        outputParticles.setAlignment(inputAlignment.getAlignment())
+        outputParticles.setAlignment(self.alignmentData.getAlignment())
 
+        self.hasFractions() # Initialize here this to avoid using the set during the loop of copyItems.
         outputParticles.copyItems(inputParticles,
                                   updateItemCallback=self._updateItem)
 
-        self._defineOutputs(outputParticles=outputParticles)
+        self._defineOutputs(**{self.OUTPUT_NAME:outputParticles})
         self._defineSourceRelation(self.inputParticles, outputParticles)
         self._defineSourceRelation(self.inputAlignment, outputParticles)
 
     def _summary(self):
         summary = []
-        if not hasattr(self, 'outputParticles'):
+        if not hasattr(self, self.OUTPUT_NAME):
             summary.append("Output particles not ready yet.")
         else:
             scale = self.inputAlignment.get().getSamplingRate()/self.inputParticles.get().getSamplingRate()
             summary.append("Assigned alignment to %s particles from a total of %s." % (
                 self.outputParticles.getSize(), self.inputParticles.get().getSize()))
             if scale != 1:
                 summary.append("Applied scale of %s." % scale)
         return summary
 
     def _methods(self):
         methods = []
-        if not hasattr(self, 'outputParticles'):
+        if not hasattr(self, self.OUTPUT_NAME):
             methods.append("Output particles not ready yet.")
         else:
             scale = self.inputAlignment.get().getSamplingRate()/self.inputParticles.get().getSamplingRate()
             methods.append("We assigned alignment to %s particles from %s and produced %s."
                            % (self.outputParticles.getSize(), self.getObjectTag('inputParticles'),
                               self.getObjectTag('outputParticles')))
             if scale != 1:
@@ -159,7 +182,23 @@
             if alignment is None:
                 errors.append('Inconsistency detected in *Input alignment* !!!')
                 errors.append('It has alignment: _%s_, but the alignment is missing!!!' %
                               inputAlignmentSet.getAlignment())
             
         # Add some errors if input is not valid
         return errors
+    def hasFractions(self):
+
+        if not hasattr(self, '_hasFractions'):
+            item = self.inputParticles.get().getFirstItem()
+            self._hasFractions = item.hasCoordinate() and hasattr(item.getCoordinate(), "xFrac")
+
+        return self._hasFractions
+
+    def _warnings(self):
+        warnings = []
+        if self.hasFractions() and self.ignoreFractionalShift.get():
+            warnings.append("Your set has residual shifts from a previous 'extract coordinates' protocol."
+                            " And will be ignored. If you want to use them, cancel this and deactivate '%s'."
+                            % self.IGNORE_LABEL)
+
+        return warnings
```

### Comparing `scipion-em-3.0.9/pwem/protocols/protocol_alignment_invertHand.py` & `scipion-em-3.1.0/pwem/protocols/protocol_alignment_invertHand.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.0.9/pwem/protocols/protocol_batch.py` & `scipion-em-3.1.0/pwem/protocols/protocol_batch.py`

 * *Files 6% similar despite different names*

```diff
@@ -65,88 +65,109 @@
         form.addHidden('sqliteFile', FileParam)
         form.addHidden('outputClassName', StringParam)
 
     def _insertAllSteps(self):
         self._insertFunctionStep('createSetStep')
 
     def createSetStep(self):
-        setObj = self.createSetObject()
-        inputObj = self.inputObject.get()
+
+        sourceSet = self.inputObject.get()
+        markedSet = self.createSetObject()  # Set equal to sourceSet but marked with disabled
         other = self.other.get()
+
+        self.info("Source: %s" % sourceSet)
+        self.info("Output type: %s" % self.outputClassName)
+        self.info("Subset (sqlite) file: %s" % self.sqliteFile)
+        if other:
+            self.info("Other: %s" % other)
+
+
+        # New recommended way to create subsets: making the set responsible for his own subset process
+        # Once all Sets implement appendFromSet and the if below is gone we can remove this "if"
+        if getattr(markedSet, "USE_CREATE_COPY_FOR_SUBSET", False):
+            markedSet.loadAllProperties()
+            newSet = markedSet.createCopy(self._getPath(),
+                                          copyInfo=True, copyItems=True)
+
+            # Define outputs, may be use something more specific than "subset"
+            self._defineOutputs(subset=newSet)
+            self._defineSourceRelation(sourceSet, newSet)
+            return
+
         if other and ',Volume' in other:
             volId = int(other.split(',')[0])
 
-            if isinstance(setObj, emobj.SetOfVolumes):
+            if isinstance(markedSet, emobj.SetOfVolumes):
                 volSet = emobj.SetOfVolumes(filename=self._dbName)
                 output = volSet[volId]
             else:
                 classSet = emobj.SetOfClasses3D(filename=self._dbName)
                 output = classSet[volId].getRepresentative()
             self._defineOutputs(outputVolume=output)
 
-        elif isinstance(inputObj, emobj.SetOfImages):
-            self._createSubSetFromImages(inputObj)
+        elif isinstance(sourceSet, emobj.SetOfImages):
+            self._createSubSetFromImages(sourceSet)
 
-        elif isinstance(inputObj, emobj.SetOfClasses):
-            self._createSubSetFromClasses(inputObj)
+        elif isinstance(sourceSet, emobj.SetOfClasses):
+            self._createSubSetFromClasses(sourceSet)
 
-        elif isinstance(inputObj, emobj.SetOfCTF):
+        elif isinstance(sourceSet, emobj.SetOfCTF):
             outputClassName = self.outputClassName.get()
             if outputClassName.startswith('SetOfMicrographs'):
-                self._createMicsSubSetFromCTF(inputObj)
+                self._createMicsSubSetFromCTF(sourceSet)
 
-        elif isinstance(inputObj, emobj.SetOfAtomStructs):
-            self._createSubSetFromAtomStructs(inputObj)
+        elif isinstance(sourceSet, emobj.SetOfAtomStructs):
+            self._createSubSetFromAtomStructs(sourceSet)
 
-        elif isinstance(inputObj, MicrographsTiltPair):
-            self._createSubSetFromMicrographsTiltPair(inputObj)
+        elif isinstance(sourceSet, MicrographsTiltPair):
+            self._createSubSetFromMicrographsTiltPair(sourceSet)
 
-        elif isinstance(inputObj, ParticlesTiltPair):
-            self._createSubSetFromParticlesTiltPair(inputObj)
+        elif isinstance(sourceSet, ParticlesTiltPair):
+            self._createSubSetFromParticlesTiltPair(sourceSet)
 
-        elif isinstance(inputObj, EMProtocol):
+        elif isinstance(sourceSet, EMProtocol):
             if self.other.hasValue():
                 otherid = self.other.get()
                 otherObj = self.getProject().mapper.selectById(int(otherid))
 
-                if isinstance(setObj, emobj.SetOfClasses):
-                    setObj.setImages(otherObj)
-                    self._createSubSetFromClasses(setObj)
-
-                elif isinstance(setObj, emobj.SetOfImages):
-                    setObj.copyInfo(otherObj)  # copy info from original images
-                    self._createSubSetFromImages(setObj)
+                if isinstance(markedSet, emobj.SetOfClasses):
+                    markedSet.setImages(otherObj)
+                    self._createSubSetFromClasses(markedSet)
+
+                elif isinstance(markedSet, emobj.SetOfImages):
+                    markedSet.copyInfo(otherObj)  # copy info from original images
+                    self._createSubSetFromImages(markedSet)
 
-                elif isinstance(setObj, emobj.SetOfNormalModes):
+                elif isinstance(markedSet, emobj.SetOfNormalModes):
                     self._createSimpleSubset(otherObj)
             else:
-                if isinstance(setObj, emobj.SetOfVolumes):
+                if isinstance(markedSet, emobj.SetOfVolumes):
                     volSet = emobj.SetOfVolumes(filename=self._dbName)
                     volSet.loadAllProperties()
                     self._createSimpleSubset(volSet)
 
                 # Go for a generic way of creating the set the the
                 # input set is not registered (typically from viewers)
                 else:
                     # We might want to do this before, inside the createSetObject
-                    setObj.loadAllProperties()
-                    self._createSimpleSubset(setObj)
+                    markedSet.loadAllProperties()
+                    self._createSimpleSubset(markedSet)
 
         else:
-            self._createSimpleSubset(inputObj)
+            self._createSimpleSubset(sourceSet)
 
     def _createSimpleSubset(self, inputObj):
         className = inputObj.getClassName()
         modifiedSet = inputObj.getClass()(filename=self._dbName,
                                           prefix=self._dbPrefix)
         try:
             createFunc = getattr(self, '_create' + className)
             output = createFunc()
         except Exception:
-            output = inputObj.create(self._getPath())
+            output = inputObj.createCopy(self._getPath())
 
         for item in modifiedSet:
             if item.isEnabled():
                 output.append(item)
 
         if hasattr(modifiedSet, 'copyInfo'):
             output.copyInfo(inputObj)
@@ -165,19 +186,19 @@
         setClass = inputImages.getClass()
 
         modifiedSet = setClass(filename=self._dbName, prefix=self._dbPrefix)
         try:
             createFunc = getattr(self, '_create' + className)
             output = createFunc()
         except Exception:
-            output = inputImages.create(self._getPath())
+            output = inputImages.createCopy(self._getPath())
 
         if copyInfoCallback is None:
-            modifiedSet.loadAllProperties()
-            output.copyInfo(modifiedSet)
+            # modifiedSet.loadAllProperties()
+            output.copyInfo(inputImages)
         else:
             copyInfoCallback(output)
 
         output.appendFromImages(modifiedSet)
         # Register outputs
         self._defineOutput(className, output)
 
@@ -324,15 +345,15 @@
         """
         inputImages = inputClasses.getImages()
         className = inputImages.getClassName()
         try:
             createFunc = getattr(self, '_create' + className)
             output = createFunc()
         except Exception as e:
-            output = inputImages.create(self._getPath())
+            output = inputImages.createCopy(self._getPath())
 
         modifiedSet = inputClasses.getClass()(filename=self._dbName, prefix=self._dbPrefix)
         self.info("Creating subset of images from classes, sqlite file: %s" % self._dbName)
         self._copyInfoAndSetAlignment(inputClasses, output)
         output.appendFromClasses(modifiedSet)
         # Register outputs
         self._defineOutput(className, output)
@@ -452,14 +473,16 @@
         outputDict = {'outputParticlesTiltPair': output}
         self._defineOutputs(**outputDict)
         self._defineTransformRelation(particlesTiltPair, output)
         return output
 
     # noinspection PyAttributeOutsideInit
     def createSetObject(self):
+        """ Moves the sqlite with the enable/disable status to its own
+        path to keep it and names it subset.sqlite"""
         _dbName, self._dbPrefix = self.sqliteFile.get().split(',')
         self._dbName = self._getPath('subset.sqlite')
         os.rename(_dbName, self._dbName)
 
         if self._dbPrefix.endswith('_'):
             self._dbPrefix = self._dbPrefix[:-1]
```

### Comparing `scipion-em-3.0.9/pwem/protocols/protocol_create_stream_data.py` & `scipion-em-3.1.0/pwem/protocols/protocol_create_stream_data.py`

 * *Files 14% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 # *
 # *  All comments concerning this program package may be sent to the
 # *  e-mail address 'scipion@cnb.csic.es'
 # *
 # **************************************************************************
 
 from collections import OrderedDict
-from os.path import basename
+from os.path import basename, splitext
 import time
 import random
 
 import pyworkflow.protocol.params as params
 from pyworkflow import VERSION_1_1
 from pyworkflow.protocol.constants import STEPS_PARALLEL
 
@@ -40,14 +40,15 @@
 from pwem import emlib
 
 
 SET_OF_MOVIES = 0
 SET_OF_MICROGRAPHS = 1
 SET_OF_RANDOM_MICROGRAPHS = 2
 SET_OF_PARTICLES = 3
+SET_OF_COORDINATES = 4
 
 
 class ProtCreateStreamData(EMProtocol):
     """ create  setofXXXX in streaming mode.
         micrograph -> read a micrograph in memory and writes it nDim times
         movie      -> read a movie in memory and writes it nDim times
         randomMicrographs -> creates a micrograph with random values
@@ -70,15 +71,15 @@
 
     # -------------------------- DEFINE param functions ----------------------
     def _defineParams(self, form):
         form.addSection(label='Input')
 
         form.addParam('setof', params.EnumParam, default=0,
                       choices=['Movies', 'Micrographs', 'RandomMicrographs',
-                               'Particles'],
+                               'Particles', 'Coordinates'],
                       label='set Of',
                       help='create set of')
         form.addParam('inputMovies', params.PointerParam, pointerClass='SetOfMovies',
                       condition="setof==%d" % SET_OF_MOVIES,
                       label="movie",
                       help='This movie will be copied "number of items" times')
         form.addParam('inputMics', params.PointerParam,
@@ -96,14 +97,19 @@
                       label="ydim",
                       help="Y dim ")
         form.addParam('inputParticles', params.PointerParam,
                       pointerClass='SetOfParticles',
                       condition="setof==%d" % SET_OF_PARTICLES,
                       label="SetOfParticles",
                       help='These particles will be written in streaming')
+        form.addParam('inputCoordinates', params.PointerParam,
+                      pointerClass='SetOfCoordinates',
+                      condition="setof==%d" % SET_OF_COORDINATES,
+                      label="SetOfCoordinates",
+                      help='These Coordinates will be written in streaming')
         form.addParam('groups', params.IntParam, default=50,
                       condition="setof==%d" % SET_OF_PARTICLES,
                       label="groups",
                       help='How many items will be created every iteration')
         form.addParam('nDim', params.IntParam, default=10,
                       label="number of items",
                       help="setofXX size")
@@ -112,54 +118,67 @@
                           SET_OF_MICROGRAPHS, SET_OF_MOVIES),
                       label="samplingRate",
                       help="Sampling rate")
         form.addParam('creationInterval', params.IntParam, default=60,
                       label="Create Object each (sec)",
                       pointerClass='EMProtocol',
                       help="create one object each creationInterval seconds")
+        form.addParam('extraRandomInterval', params.IntParam, default=0,
+                      label='Extra random seconds interval', expertLevel=params.LEVEL_ADVANCED,
+                      help='Each object will be generated in a random time uniformly picked from the interval defined by'
+                           '[baseInterval, baseInterval+extraInterval]')
         form.addParam('delay', params.IntParam, default=0,
                       label="delay (sec)",
                       help="wait this seconds before creating stream data")
 
         form.addParallelSection(threads=1, mpi=1)
 
     # --------------------------- INSERT steps functions ---------------------
     def _insertAllSteps(self):
         self.counter = 0
         deps = []
 
-        if self.delay != 0:
+        if self.delay.get() != 0:
             delayId = self._insertFunctionStep('delayStep')
             deps.append(delayId)
 
         step = None
         if self.setof == SET_OF_MOVIES:
             step = 'createStep'
         elif self.setof == SET_OF_MICROGRAPHS:
             step = 'createStep'
         elif self.setof == SET_OF_RANDOM_MICROGRAPHS:
             step = 'createRandomMicStep'
         elif self.setof == SET_OF_PARTICLES:
             step = 'createParticlesStep'
+        elif self.setof == SET_OF_COORDINATES:
+            step = 'createCoordinatesStep'
         else:
             raise Exception('Unknown data type')
 
         if self.setof == SET_OF_PARTICLES:
             self.nDims = int(min(self.nDim, len(self.inputParticles.get())))
             self.group = int(min(self.nDims, self.groups.get()))
             for mic in range(1, int((self.nDims / self.group) +
                              (self.nDims % self.group > 0) + 1)):
                 self._insertFunctionStep(step, prerequisites=deps)
+
+        elif self.setof == SET_OF_COORDINATES:
+            self.inputMicrographs = self.inputCoordinates.get().getMicrographs()
+            self.nDims = min(self.nDim.get(), len(self.inputMicrographs))
+            for micIdx in range(1, self.nDims + 1):
+                self._insertFunctionStep(step, micIdx, prerequisites=deps)
+
         else:
             for mic in range(1, self.nDim.get() + 1):
                 self._insertFunctionStep(step, mic, prerequisites=deps)
 
-    # -------------------------- STEPS functions -------------------------
+    # -------------------------- STEPS functions ------------------------
     def delayStep(self):
-        time.sleep(self.delay)
+        time.sleep(self.delay.get())
 
     def _checkNewItems(self, objSet):
         """ Check for already computed micrograph/movie and
         update the output set. """
         objDict = {}
         newObj = False
         for obj in objSet:
@@ -268,62 +287,89 @@
         if newObj:
             if endObjs:
                 newObjSet.setStreamState(newObjSet.STREAM_CLOSED)
             self._updateOutput(newObjSet)
         newObjSet.close()
 
     def createStep(self, counter):
-        time.sleep(self.creationInterval.get())
+        time.sleep(self.getTimeInterval())
         if not ProtCreateStreamData.object or self.setof == \
                 SET_OF_MICROGRAPHS or self.setof == SET_OF_MOVIES:
 
             if self.setof == SET_OF_MOVIES:
                 setDim = self.inputMovies.get().getSize()
                 for idx, mov in enumerate(self.inputMovies.get()):
                     if idx == (counter - 1) % setDim:
                         newMov = mov.clone()
                         break
+                _, ext = splitext(newMov.getFileName())
                 ProtCreateStreamData.object = \
                     emlib.image.ImageHandler().read(newMov.getLocation())
                 self.name = "movie"
 
             elif self.setof == SET_OF_MICROGRAPHS:
                 setDim = self.inputMics.get().getSize()
                 for idx, mic in enumerate(self.inputMics.get()):
                     if idx == (counter-1) % setDim:
                         newMic = mic.clone()
                         break
+                _, ext = splitext(newMic.getFileName())
                 ProtCreateStreamData.object = \
                     emlib.image.ImageHandler().read(newMic.getLocation())
                 self.name = "micro"
 
         # save file
-        destFn = self._getExtraPath("%s_%05d" % (self.name, counter))
+        destFn = self._getExtraPath("%s_%05d%s" % (self.name, counter, ext))
         ProtCreateStreamData.object.write(destFn)
         self.dictObj[destFn] = True
         self._checkProcessedData()
 
     def createParticlesStep(self):
         self.name = "particle"
-        time.sleep(self.creationInterval.get())
+        time.sleep(self.getTimeInterval())
 
         for idx, p in enumerate(self.inputParticles.get()):
             if ((idx > self.counter-1) and (idx < self.nDims) and
                     (idx <= self.counter-1 + self.group)):
                 newP = p.clone()
                 ProtCreateStreamData.object = \
                     emlib.image.ImageHandler().read(newP.getLocation())
                 destFn = self._getExtraPath("%s_%05d" % (self.name, idx))
                 ProtCreateStreamData.object.write(destFn)
                 self.dictObj[destFn] = True
         self._checkProcessedData()
 
+    def createCoordinatesStep(self, micIdx):
+        self.name = "coordinate"
+        time.sleep(self.getTimeInterval())
+        inputCoordinates = self.inputCoordinates.get()
+        micrographs = inputCoordinates.getMicrographs()
+        if not hasattr(self, "outputCoordinates"):
+            self.outputCoordinates = self._createSetOfCoordinates(micrographs)
+            self.outputCoordinates.copyInfo(inputCoordinates)
+            self.outputCoordinates.setBoxSize(inputCoordinates.getBoxSize())
+            self.outputCoordinates.setStreamState(emobj.SetOfParticles.STREAM_OPEN)
+            self._defineOutputs(outputCoordinates=self.outputCoordinates)
+            self._defineSourceRelation(inputCoordinates, self.outputCoordinates)
+
+        for idx, mic in enumerate(micrographs):
+            if idx == micIdx - 1:
+                newMic = mic.clone()
+                for newCoord in self.inputCoordinates.get().iterCoordinates(newMic):
+                    self.outputCoordinates.append(newCoord)
+                if micIdx == self.nDims:
+                    self.outputCoordinates.setStreamState(emobj.SetOfParticles.STREAM_CLOSED)
+                self.outputCoordinates.write()
+                self._store(self.outputCoordinates)
+                break
+
+
     def createRandomMicStep(self, mic):
         from pwem import Domain
-        time.sleep(self.creationInterval.get())
+        time.sleep(self.getTimeInterval())
         getEnviron = Domain.importFromPlugin('xmipp3', 'Plugin',
                                              doRaise=True).getEnviron
 
         # create image
         img = emlib.Image()
         img.setDataType(emlib.DT_FLOAT)
         img.resize(self.xDim, self.yDim)
@@ -362,14 +408,21 @@
         args += " -o %s" % baseFnImageCTF
         args += " -f ctf %s" % baseFnCtf
         args += " --sampling %f" % self.samplingRate
         self.runJob("xmipp_transform_filter", args, env=getEnviron())
         self.dictObj[baseFnImageCTF] = True
         self._checkProcessedData()
 
+    # -------------------------- UTILS functions -----------------------------
+    def getTimeInterval(self):
+        baseInterval = self.creationInterval.get()
+        interval = random.randint(baseInterval, baseInterval+self.extraRandomInterval.get())
+        return interval
+
+
     # -------------------------- INFO functions ------------------------------
     def _validate(self):
         return []
 
     def _summary(self):
         return []
```

### Comparing `scipion-em-3.0.9/pwem/protocols/protocol_ctf_assign.py` & `scipion-em-3.1.0/pwem/protocols/protocol_ctf_assign.py`

 * *Files 8% similar despite different names*

```diff
@@ -63,25 +63,24 @@
         self.inputSetsParam = form.addParam('inputSet', params.PointerParam,
                                             pointerClass='EMSet',
                                             label='Input set',
                                             help='Select the images '
                                                  '(micrographs or particles) '
                                                  'that you want to update the '
                                                  'CTF parameters.')        
-        form.addParam('inputCTF', params.PointerParam, pointerClass='SetOfCTF',
+        form.addParam('inputCTF', params.PointerParam,
+                      pointerClass='SetOfCTF, SetOfParticles',
                       label="Input CTF",
-                      help='Select the CTF that will be used to update '
-                           'particles.')  
+                      help='Select the CTFs that will be used to update '
+                           'particles. It can be another set of particles')
         form.addParallelSection(threads=0, mpi=0) 
     
     # --------------------------- INSERT steps functions ----------------------
                                 
     def _insertAllSteps(self):
-        """for each ctf insert the steps to compare it
-        """
         self._insertFunctionStep('createOutputStep')
     
     # --------------------------- STEPS functions -----------------------------
     def createOutputStep(self):
         inputSet = self.inputSet.get()
         inputCTF = self.inputCTF.get()
         
@@ -90,47 +89,52 @@
         else:
             self._micrographsOutputStep(inputSet, inputCTF)
             
     def _particlesOutputStep(self, inputSet, inputCTF):
         outputParts = self._createSetOfParticles()
         outputParts.copyInfo(inputSet)
         outputParts.setHasCTF(True)
-        ctfDict = {}
-        
-        firstCoord = inputSet.getFirstItem().getCoordinate()
-        hasMicName = firstCoord.getMicName() is not None
-        
-        for ctf in inputCTF:
-            if hasMicName:
-                ctfName = ctf.getMicrograph().getMicName()
-            else:
-                ctfName = ctf.getMicrograph().getObjId()
-#             print("ctf: ", ctf.printAll(), ctfName)
-            ctfDict[ctfName] = ctf.clone()
-        
-        missingSet = set()  # Report missing micrographs only once
-        
-        for particle in inputSet:
-            if particle.hasCoordinate():
-                coord = particle.getCoordinate()
-                micKey = coord.getMicName() if hasMicName else particle.getMicId()
-            else:
-                micKey = particle.getMicId()
-           
-            if micKey not in missingSet:
-                ctf = ctfDict.get(micKey, None)
-                
-                if ctf is None:
-                    self.warning("Discarding particles from micrograph with"
-                                 " micName: %s, CTF not found. " % micKey)
-                    missingSet.add(micKey)
+
+        if isinstance(inputCTF, emobj.SetOfParticles):
+            outputParts.copyItems(inputSet,
+                                  itemDataIterator=inputCTF.iterItems(),
+                                  updateItemCallback=self._updateItem)
+        else:
+            ctfDict = {}
+            firstCoord = inputSet.getFirstItem().getCoordinate()
+            hasMicName = firstCoord.getMicName() is not None
+
+            for ctf in inputCTF:
+                if hasMicName:
+                    ctfName = ctf.getMicrograph().getMicName()
+                else:
+                    ctfName = ctf.getMicrograph().getObjId()
+    #             print("ctf: ", ctf.printAll(), ctfName)
+                ctfDict[ctfName] = ctf.clone()
+
+            missingSet = set()  # Report missing micrographs only once
+
+            for particle in inputSet:
+                if particle.hasCoordinate():
+                    coord = particle.getCoordinate()
+                    micKey = coord.getMicName() if hasMicName else particle.getMicId()
                 else:
-                    newParticle = particle.clone()
-                    newParticle.setCTF(ctf)
-                    outputParts.append(newParticle)
+                    micKey = particle.getMicId()
+
+                if micKey not in missingSet:
+                    ctf = ctfDict.get(micKey, None)
+
+                    if ctf is None:
+                        self.warning("Discarding particles from micrograph with"
+                                     " micName: %s, CTF not found. " % micKey)
+                        missingSet.add(micKey)
+                    else:
+                        newParticle = particle.clone()
+                        newParticle.setCTF(ctf)
+                        outputParts.append(newParticle)
         
         self._defineOutputs(outputParticles=outputParts)
         self._defineSourceRelation(self.inputSet, outputParts)
         self._defineSourceRelation(self.inputCTF, outputParts)
 
     def __findCTF(self, inputSet, outputSet, ctfDict, keyFunc):
         for mic in inputSet:
@@ -181,13 +185,17 @@
         # Add some errors if input is not valid
         inputSet = self.inputSet.get()
         if isinstance(inputSet, emobj.SetOfParticles):
             part = inputSet.getFirstItem()
             if not part.hasMicId():
                 errors.append("The input particles doesn't have any micrograph"
                               " assigned.")
+
         # same micrographs in both CTF??
         return errors
     
     # --------------------------- UTILS functions -----------------------------
     def _stepsCheck(self):
         pass
+
+    def _updateItem(self, item, row):
+        item.setCTF(row.getCTF())
```

### Comparing `scipion-em-3.0.9/pwem/protocols/protocol_export/__init__.py` & `scipion-em-3.1.0/pwem/protocols/protocol_export/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.0.9/pwem/protocols/protocol_export/protocol_export_DB.py` & `scipion-em-3.1.0/pwem/protocols/protocol_export/protocol_export_DB.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 
 class ProtExportDataBases(EMProtocol):
     """ generates files for elements to submit structures to EMDB/PDB.
         Since mmcif/pdb is only partially supported by some software
         the protocol creates 4 versions of the atomic struct file with the hope that at least
         one of them will work.
     """
-    _label = 'export emdb/pdb'
+    _label = 'export to emdb/pdb'
     _program = ""
     _lastUpdateVersion = VERSION_1_2
     VOLUMENAME = 'main_map.mrc'
     HALFVOLUMENAME = 'half_map_%d.mrc'
     COORDINATEFILENAME = 'coordinates.cif'
     ADDITIONALVOLUMEDIR = "addMaps"
     ADDITIONALVOLUMENAME = "map_%02d.mrc"
```

### Comparing `scipion-em-3.0.9/pwem/protocols/protocol_extract_coordinates.py` & `scipion-em-3.1.0/pwem/protocols/protocol_extract_coordinates.py`

 * *Files 1% similar despite different names*

```diff
@@ -155,16 +155,16 @@
         inPart = self.getInputParticles()
         inMics = self.getInputMicrographs()
         scale = inPart.getSamplingRate() / inMics.getSamplingRate()
         print("Scaling coordinates by a factor *%0.2f*" % scale)
         alignType = inPart.getAlignment()
 
         suffix = self.getSuffix(partsIds[0]) if partsIds is not None else ''
-        outputCoords = self._createSetOfCoordinates(inMics, suffix=suffix)
-
+        #outputCoords = self._createSetOfCoordinates(inMics, suffix=suffix)
+        outputCoords = self._createSetOfCoordinates(self.getInputMicrographsPointer(), suffix=suffix)
         # Prepare a double key dictionary to do the match: micname and micId
         micDict = dict()
         for mic in inMics.iterItems():
             # Clone the mics! otherwise we will get pointers and
             # will end up with the same mic in the dictionary.
             clonedMic = mic.clone()
             micDict[clonedMic.getObjId()] = clonedMic
@@ -268,18 +268,15 @@
         else:
             outputSet = emobj.SetOfCoordinates(filename=setFile)
             outputSet.setStreamState(outputSet.STREAM_OPEN)
             self._store(outputSet)
             self._defineTransformRelation(self.getInputParticles(), outputSet)
             self._defineSourceRelation(self.getInputMicrographs(), outputSet)
 
-        # copyInfo raise an error since particles has no _boxsize
-        #   copyInfo does not do anything else
-        # outputSet.copyInfo(self.getInputParticles())
-        outputSet.setMicrographs(self.getInputMicrographs())
+        outputSet.setMicrographs(self.getInputMicrographsPointer())
 
         return outputSet
 
     def _getFirstJoinStep(self):
         for s in self._steps:
             if s.funcName == self._getFirstJoinStepName():
                 return s
```

### Comparing `scipion-em-3.0.9/pwem/protocols/protocol_import/__init__.py` & `scipion-em-3.1.0/pwem/protocols/protocol_import/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -32,9 +32,9 @@
 from .base import ProtImport, ProtImportFiles
 from .coordinates import ProtImportCoordinates, ProtImportCoordinatesPairs
 from .ctfs import ProtImportCTF
 from .images import ProtImportImages
 from .masks import ProtImportMask
 from .micrographs import ProtImportMicrographs, ProtImportMovies
 from .particles import ProtImportParticles, ProtImportAverages
-from .volumes import ProtImportVolumes, ProtImportPdb
+from .volumes import ProtImportVolumes, ProtImportPdb, ProtImportSetOfAtomStructs
 from .sequence import ProtImportSequence
```

### Comparing `scipion-em-3.0.9/pwem/protocols/protocol_import/base.py` & `scipion-em-3.1.0/pwem/protocols/protocol_import/base.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.0.9/pwem/protocols/protocol_import/coordinates.py` & `scipion-em-3.1.0/pwem/protocols/protocol_import/coordinates.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,21 +51,22 @@
     _label = 'import coordinates'
 
     IMPORT_FROM_AUTO = 0
     IMPORT_FROM_XMIPP = 1
     IMPORT_FROM_RELION = 2
     IMPORT_FROM_EMAN = 3
     IMPORT_FROM_DOGPICKER = 4
+    IMPORT_FROM_SCIPION = 5
 
     def _getImportChoices(self):
         """ Return a list of possible choices
         from which the import can be done.
         (usually packages formats such as: xmipp3, eman2, relion...etc.
         """
-        return ['auto', 'xmipp', 'relion', 'eman', 'dogpicker']
+        return ['auto', 'xmipp', 'relion', 'eman', 'dogpicker', 'scipion']
 
     def _getDefaultChoice(self):
         return self.IMPORT_FROM_AUTO
 
     def _getFilesCondition(self):
         """ Return an string representing the condition
         when to display the files path and pattern to grab
@@ -84,46 +85,58 @@
                       label='Input micrographs',
                       help='Select the micrographs for which you want to '
                            'import coordinates.')
 
         form.addParam('boxSize', IntParam, label='Box size')
         form.addParam('scale', FloatParam,
                       label='Scale', default=1,
+                      condition='importFrom!=%d' % self.IMPORT_FROM_SCIPION,
                       help='Factor to scale coordinates')
         form.addParam('invertX', BooleanParam, default=False,
+                      condition='importFrom!=%d' % self.IMPORT_FROM_SCIPION,
                       label='Invert X')
         form.addParam('invertY', BooleanParam, default=False,
+                      condition='importFrom!=%d' % self.IMPORT_FROM_SCIPION,
                       label='Invert Y',
                       help='Invert Y for EMAN coordinates taken on dm3 or'
                            ' tif micrographs')
 
     # ------------------- INSERT steps functions ------------------------------
     def _insertAllSteps(self):
         importFrom = self.importFrom.get()
         self._insertFunctionStep('createOutputStep', importFrom,
                                  self.filesPath.get())
 
     # ------------------ STEPS functions --------------------------------------
     def createOutputStep(self, importFrom, *args):
-        inputMics = self.inputMicrographs.get()
-        coordsSet = self._createSetOfCoordinates(inputMics)
-        coordsSet.setBoxSize(self.boxSize.get())
-        ci = self.getImportClass()
-        for coordFile, fileId in self.iterFiles():
-            mic = self.getMatchingMic(coordFile, fileId)
-            if mic is not None:
-                def addCoordinate(coord):
-                    coord.setMicrograph(mic)
-                    self.correctCoordinatePosition(coord)
-                    coordsSet.append(coord)
-                # Parse the coordinates in the given format for this micrograph
-                ci.importCoordinates(coordFile, addCoordinate=addCoordinate)
 
-        self._defineOutputs(outputCoordinates=coordsSet)
-        self._defineSourceRelation(self.inputMicrographs, coordsSet)
+        # scipion imports have a predefined format (see dataimport)
+        if importFrom == self.IMPORT_FROM_SCIPION:
+            from .dataimport import ScipionImport
+            self.importFilePath = self.filesPath.get('').strip()
+            sImport = ScipionImport(self, self.importFilePath)
+            # this function defines outputs and relations
+            sImport.importCoordinates(self.inputMicrographs)
+        else:
+            # Pass the pointer with extended.
+            coordsSet = self._createSetOfCoordinates(self.inputMicrographs)
+            coordsSet.setBoxSize(self.boxSize.get())
+            ci = self.getImportClass()
+            for coordFile, fileId in self.iterFiles():
+                mic = self.getMatchingMic(coordFile, fileId)
+                if mic is not None:
+                    def addCoordinate(coord):
+                        coord.setMicrograph(mic)
+                        self.correctCoordinatePosition(coord)
+                        coordsSet.append(coord)
+                    # Parse the coordinates in the given format for this micrograph
+                    ci.importCoordinates(coordFile, addCoordinate=addCoordinate)
+
+            self._defineOutputs(outputCoordinates=coordsSet)
+            self._defineSourceRelation(self.inputMicrographs, coordsSet)
 
     # ---------------- INFO functions -----------------------------------------
     def _summary(self):
         summary = []
 
         if not hasattr(self, 'outputCoordinates'):
             msg = 'Output coordinates not ready yet'
@@ -173,14 +186,15 @@
 
         elif importFrom == self.IMPORT_FROM_DOGPICKER:
             DogpickerImport = Domain.importFromPlugin('appion.convert', 'DogpickerImport',
                                                       errorMsg='appion plugin is needed to import '
                                                                'dogpicker files',
                                                       doRaise=True)
             return DogpickerImport(self)
+
         else:
             self.importFilePath = ''
             return None
 
     def getImportFrom(self):
         importFrom = self.importFrom.get()
         if importFrom == self.IMPORT_FROM_AUTO:
```

### Comparing `scipion-em-3.0.9/pwem/protocols/protocol_import/ctfs.py` & `scipion-em-3.1.0/pwem/protocols/protocol_import/ctfs.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.0.9/pwem/protocols/protocol_import/dataimport.py` & `scipion-em-3.1.0/pwem/protocols/protocol_import/dataimport.py`

 * *Files 11% similar despite different names*

```diff
@@ -59,14 +59,36 @@
         self.protocol.setSamplingRate(micSet)
         micSet.setIsPhaseFlipped(self.protocol.haveDataBeenPhaseFlipped.get())
         # Read the micrographs from the 'self._sqliteFile' metadata
         # but fixing the filenames with new ones (linked or copy to extraDir)
         micSet.copyItems(inputSet, updateItemCallback=self._updateParticle)
         self.protocol._defineOutputs(outputMicrographs=micSet)
 
+    def importCoordinates(self, inputMics):
+        """ Import a SetOfCoordinates from a given sqlite file. """
+        inputSet = emobj.SetOfCoordinates(filename=self._sqliteFile)
+        # self._findImagesPath(inputSet)
+        
+        coorSet = self.protocol._createSetOfCoordinates(inputMics)
+        coorSet.copyInfo(inputSet)
+        coorSet.setObjComment('Coordinates imported from sqlite file:\n%s'
+                             % self._sqliteFile)
+
+        # Update both samplingRate and acquisition with parameters
+        # selected in the protocol form.
+        # Acquisition should be updated before, just to ensure that
+        # scannedPixedSize will be computed properly when calling
+        # setSamplingRate
+        coorSet.setBoxSize(self.protocol.boxSize.get())
+        # Read the micrographs from the 'self._sqliteFile' metadata
+        # but fixing the filenames with new ones (linked or copy to extraDir)
+        coorSet.copyItems(inputSet)
+        self.protocol._defineOutputs(outputCoordinates=coorSet)
+        self.protocol._defineSourceRelation(inputMics, coorSet)
+
     def importParticles(self):
         """ Import particles from a metadata 'images.xmd' """
         inputSet = emobj.SetOfParticles(filename=self._sqliteFile)
         inputSet.loadProperty('_alignment', emcts.ALIGN_NONE)
         inputSet.loadProperty('_hasCtf', False)
         self._findImagesPath(inputSet)
```

### Comparing `scipion-em-3.0.9/pwem/protocols/protocol_import/images.py` & `scipion-em-3.1.0/pwem/protocols/protocol_import/images.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 
 from os.path import exists, isdir
 import time
 from datetime import timedelta, datetime
 
 import pyworkflow.utils as pwutils
 import pyworkflow.protocol.params as params
+from pwem import cleanFileName
 
 from pwem.emlib.image import ImageHandler
 from pwem.objects import Acquisition
 
 from .base import ProtImportFiles
 
 
@@ -158,15 +159,15 @@
                     img.cleanObjId()
                     img.setMicId(fileId)
                     img.setFileName(dst)
                     img.setIndex(index)
                     self._addImageToSet(img, imgSet)
             else:
                 img.setObjId(fileId)
-                img.setFileName(dst)
+                img.setLocation(dst)
                 # Fill the micName if img is either Micrograph or Movie
                 uniqueFn = uniqueFn.replace(' ', '')
                 self._fillMicName(img, uniqueFn)
                 self._addImageToSet(img, imgSet)
 
             outFiles.append(dst)
             
@@ -242,20 +243,16 @@
             for fileName, uniqueFn, fileId in self.iterNewInputFiles():
                 someNew = True
                 if self.fileModified(fileName, fileTimeout):
                     continue
                 
                 dst = self._getExtraPath(uniqueFn)
                 self.importedFiles.add(uniqueFn)
-                if ' ' in dst:
-                    if not alreadyWarned:
-                        self.warning('Warning: your file names have white spaces!')
-                        self.warning('Removing white spaces from copies/symlinks.')
-                        alreadyWarned = True
-                    dst = dst.replace(' ', '')
+                dst, alreadyWarned = cleanFileName(dst, not alreadyWarned)
+
                 copyOrLink(fileName, dst)
 
                 self.debug('Importing file: %s' % fileName)
                 self.debug("uniqueFn: %s" % uniqueFn)
                 self.debug("dst Fn: %s" % dst)
 
                 if self._checkStacks:
@@ -346,14 +343,15 @@
                 # Exceptions: 
                 #  - Compressed movies (bz2 or tbz extensions)
                 #  - Importing in streaming, since files may be incomplete
                 #  - Bad characters in path [':' ,'%', '#']
                 if (not self.dataStreaming and
                     not (imgFn.endswith('bz2') or
                          imgFn.endswith('tbz') or
+                         imgFn.endswith('eer') or
                          ih.isImageFile(imgFn))):
                     if not errors:  # if empty add the first line
                         errors.append("Error reading the following images:")
                     errors.append('  %s' % imgFn)
                     errors += ProtImportImages.validatePath(imgFn)
 
             break  # validate just first image
```

### Comparing `scipion-em-3.0.9/pwem/protocols/protocol_import/masks.py` & `scipion-em-3.1.0/pwem/protocols/protocol_import/masks.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,29 +23,34 @@
 # *  All comments concerning this program package may be sent to the
 # *  e-mail address 'scipion@cnb.csic.es'
 # *
 # **************************************************************************
 """
 In this module are protocol related to EM imports of Masks...
 """
-
+import enum
 from os.path import exists, basename
 
 import pyworkflow.protocol.params as params
 import pyworkflow.utils as pwutils
 
 from pwem.objects import Mask, VolumeMask
 from pwem.emlib.image import ImageHandler
+from pwem.protocols.protocol_import.images import cleanFileName
 
 from .base import ProtImport
 
+class ImportMaskOutput(enum.Enum):
+    outputMask = VolumeMask
+
 
 class ProtImportMask(ProtImport):
     """ Class for import masks from existing files. """
     _label = 'import mask'
+    _possibleOutputs = ImportMaskOutput
     
     # --------------------------- DEFINE param functions ----------------------
     def _defineParams(self, form):
         
         form.addSection(label='Import')
 
         form.addParam('maskPath', params.PathParam,
@@ -63,14 +68,15 @@
     def importMaskStep(self, path, samplingRate):
         """ Copy mask from maskPath.
         """
         self.info("Using mask path: '%s'" % path)
 
         # Copy the image file into the project
         dst = self._getExtraPath(basename(path))
+        dst, cleaned = cleanFileName(dst)
         pwutils.copyFile(path, dst)
 
         # Retrieve image dimensions
         imgh = ImageHandler()
         _, _, z, n = imgh.getDimensions(dst)
 
         # Create a 2D or 3D Mask, consider the case of n>1
@@ -79,15 +85,15 @@
             mask = VolumeMask()
         else:
             mask = Mask()
 
         mask.setFileName(dst)
         mask.setSamplingRate(samplingRate)
 
-        self._defineOutputs(outputMask=mask)
+        self._defineOutputs(**{self._possibleOutputs.outputMask.name:mask})
 
     # --------------------------- INFO functions ------------------------------
     def _validate(self):
         errors = []
         if not self.maskPath.hasValue():
             errors.append("Mask path cannot be empty.")
         elif not exists(self.maskPath.get()):
```

### Comparing `scipion-em-3.0.9/pwem/protocols/protocol_import/micrographs.py` & `scipion-em-3.1.0/pwem/protocols/protocol_import/micrographs.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,29 +21,29 @@
 # * Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA
 # * 02111-1307  USA
 # *
 # *  All comments concerning this program package may be sent to the
 # *  e-mail address 'scipion@cnb.csic.es'
 # *
 # **************************************************************************
-
-
+import enum
 import os
 from os.path import join, basename
 import re
 from datetime import timedelta, datetime
 
 import pyworkflow.utils as pwutils
 import pyworkflow.protocol.params as params
 
 from pwem import Domain
 from pwem.emlib.image import ImageHandler
 import pwem.constants as emcts
 
 from .images import ProtImportImages
+from ...objects import SetOfMicrographs, SetOfMovies
 
 
 class ProtImportMicBase(ProtImportImages):
     """ Just to have a base class to both 
     ProtImportMicrographs and ProtImportMovies
     """
     _checkStacks = False
@@ -292,19 +292,22 @@
                     return True
             elif fileName in item2blacklist:
                 self.info("Blacklist warning: %s is blacklisted " % fileName)
                 blacklistedItems.add(fileName)
                 return True
         return False
 
+class ImportMicsOutput(enum.Enum):
+    outputMicrographs = SetOfMicrographs
 
 class ProtImportMicrographs(ProtImportMicBase):
     """Protocol to import a set of micrographs to the project"""
     _label = 'import micrographs'
-    _outputClassName = 'SetOfMicrographs'
+    _possibleOutputs = ImportMicsOutput
+    _outputClassName = ImportMicsOutput.outputMicrographs.value.__name__
 
     IMPORT_FROM_EMX = 1
     IMPORT_FROM_XMIPP3 = 2
     IMPORT_FROM_SCIPION = 3
 
     def _getImportChoices(self):
         """ Return a list of possible choices
@@ -424,21 +427,24 @@
             from .dataimport import ScipionImport
             self.importFilePath = self.sqliteFile.get('').strip()
             return ScipionImport(self, self.importFilePath)
         else:
             self.importFilePath = ''
             return None
 
+class ImportMoviesOutput(enum.Enum):
+    outputMovies = SetOfMovies
 
 class ProtImportMovies(ProtImportMicBase):
     """ Protocol to import a set of movies (from direct detector cameras)
     to the project.
     """
     _label = 'import movies'
-    _outputClassName = 'SetOfMovies'
+    _possibleOutputs = ImportMoviesOutput
+    _outputClassName = ImportMoviesOutput.outputMovies.value.__name__
 
     def __init__(self, **kwargs):
         ProtImportMicBase.__init__(self, **kwargs)
         self.serverSocket = None
         self.connectionList = None
 
     def _getBlacklistSetClass(self):
```

### Comparing `scipion-em-3.0.9/pwem/protocols/protocol_import/particles.py` & `scipion-em-3.1.0/pwem/protocols/protocol_import/particles.py`

 * *Files 3% similar despite different names*

```diff
@@ -43,44 +43,48 @@
 
     IMPORT_FROM_EMX = 1
     IMPORT_FROM_XMIPP3 = 2
     IMPORT_FROM_RELION = 3
     IMPORT_FROM_SCIPION = 4
     IMPORT_FROM_FREALIGN = 5
     IMPORT_FROM_EMAN = 6
+    IMPORT_FROM_CRYOSPARC = 7
 
-    importFormats = ['emx', 'xmipp3', 'relion', 'scipion', 'frealign', 'eman']
-    importExts = ['emx', 'xmd', 'star', 'sqlite', 'par', 'lst']
+    importFormats = ['emx', 'xmipp3', 'relion', 'scipion', 'frealign', 'eman', 'cryosparc']
+    importExts = ['emx', 'xmd', 'star', 'sqlite', 'par', 'lst', 'cs']
     alignTypeList = [emcts.ALIGN_2D, emcts.ALIGN_3D, emcts.ALIGN_PROJ,
                      emcts.ALIGN_NONE]
 
     def _getImportChoices(self):
         """ Return a list of possible choices
         from which the import can be done.
-        (usually packages formats such as: xmipp3, eman2, relion...etc.
+        (usually packages formats such as: xmipp3, eman2, relion...etc.)
         """
         choices = ProtImportImages._getImportChoices(self)
         # Do not change the order of this list since
         # it is related to the constants defined
         return choices + self.importFormats
     
     def _defineImportParams(self, form):
-        """ Import files from: emx, xmipp3, relion, scipion  formats. """
+        """
+        Import files from: emx, xmipp3, relion, scipion, cryosparc formats.
+        """
         param = form.getParam('importFrom')
         # Customize the help of this parameter with specific information
         # of the import particles
         param.help.set("You can import particles directly from the binary "
                        "files, or import from other packages formats. \n"
                        "Currently, we can import from: %s \n"
                        "Following are the expected import files for each one:\n"
                        "*emx*: particles.emx\n"
                        "*xmipp3*: images.xmd\n"
                        "*relion*: itXX_data.star\n"
                        "*scipion*: particles.sqlite\n"
                        "*eman*: particleSet.lst\n"
+                       "*cryosparc*: particles.cs\n"
                        "" % ', '.join(self.importFormats))
 
         form.addParam('emxFile', params.FileParam,
                       condition='(importFrom == %d)' % self.IMPORT_FROM_EMX,
                       label='Input EMX file',
                       help="Select the EMX file containing particles "
                            "information.\n See more about \n"
@@ -135,14 +139,21 @@
                       condition='(importFrom == %d)' % self.IMPORT_FROM_FREALIGN,
                       label='Param file',
                       help="Select a Frealign .par file with the refinement information.")
         form.addParam('lstFile', params.FileParam,
                       condition='(importFrom == %d)' % self.IMPORT_FROM_EMAN,
                       label='Lst file',
                       help='Select a *.lst set file from EMAN2 project.')
+
+        form.addParam('csFile', params.FileParam,
+                      condition='(importFrom == %d)' % self.IMPORT_FROM_CRYOSPARC,
+                      label='cs file',
+                      help="Select a .cs file.\n"
+                           "It is usually a .cs file result from cryoSPARC job "
+                           "execution.")
         
     def _defineAcquisitionParams(self, form):
         group = ProtImportImages._defineAcquisitionParams(self, form)
         group.addParam('samplingRate', params.FloatParam,
                        label=pwutils.Message.LABEL_SAMP_RATE)
 
     def _insertAllSteps(self):
@@ -191,14 +202,21 @@
             return GrigorieffLabImportParticles(self, self.parFile.get(),
                                                 self.stackFile.get())
         elif self.importFrom == self.IMPORT_FROM_EMAN:
             self.importFilePath = self.lstFile.get('').strip()
             EmanImport = Domain.importFromPlugin('eman2.convert', 'EmanImport',
                                                  doRaise=True)
             return EmanImport(self, self.lstFile.get())
+
+        elif self.importFrom == self.IMPORT_FROM_CRYOSPARC:
+            cryoSPARCImport = Domain.importFromPlugin('cryosparc2.convert', 'cryoSPARCImport',
+                                                      'cryoSPARC is needed to import .cs files',
+                                                      doRaise=True)
+            self.importFilePath = self.csFile.get('').strip()
+            return cryoSPARCImport(self, self.csFile.get())
         else:
             self.importFilePath = ''
             return None 
                     
     def setSamplingRate(self, imgSet):
         imgSet.setSamplingRate(self.samplingRate.get())
```

### Comparing `scipion-em-3.0.9/pwem/protocols/protocol_import/sequence.py` & `scipion-em-3.1.0/pwem/protocols/protocol_import/sequence.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,100 +26,104 @@
 # *
 # **************************************************************************
 
 from os.path import exists
 import os
 import pyworkflow.protocol.params as params
 
-from pwem.objects.data import Sequence
+from pwem.objects.data import Sequence, Alphabet
 import pwem.convert as emconv
 from pwem.convert import AtomicStructHandler
 
 from .base import ProtImportFiles
 
-
 class ProtImportSequence(ProtImportFiles):
     """ Protocol to import an aminoacid/nucleotide sequence file to the
     project"""
     _label = 'import sequence'
     # SEQUENCEFILENAME = '_sequence.fasta'
+    # proteins
     IMPORT_FROM_PLAIN_TEXT = 0
     IMPORT_FROM_STRUCTURE = 1
     IMPORT_FROM_FILES = 2
     IMPORT_FROM_UNIPROT = 3
+    IMPORT_FROM_PROTEIN_GENEBANK = 4
+    # nucleotics
     IMPORT_FROM_NUCLEOTIDE_PLAIN_TEXT = 0
     IMPORT_FROM_NUCLEOTIDE_STRUCTURE = 1
     IMPORT_FROM_NUCLEOTIDE_FILES = 2
-    IMPORT_FROM_GENEBANK = 3
+    IMPORT_FROM_NUCLEOTIDE_GENEBANK = 3
     IMPORT_STRUCTURE_FROM_ID = 0
     IMPORT_STRUCTURE_FROM_FILES = 1
 
     url = "http://www.uniprot.org/uniprot/"
 
     def __init__(self, **args):
         ProtImportFiles.__init__(self, **args)
 
     def _defineParams(self, form):
 
         form.addSection(label='Input')
         form.addParam('inputSequenceID', params.StringParam,
                       label="Sequence ID", allowsNull=True,
+                      expertLevel=params.LEVEL_ADVANCED,
                       help="Write a sequence ID. Otherwise, if the "
-                           "sequence derives from GeneBank/UniProt/PDB "
+                           "sequence derives from GenBank/UniProt/PDB "
                            "databases, the respective database ID will be "
                            "selected as starting sequence ID; examples: if "
-                           "you select GeneBank accession AJ520101, SCIPION "
+                           "you select GenBank accession AJ520101, SCIPION "
                            "will assign AJ520101 as sequence ID; if "
                            "you select UniProt accession P12345, SCIPION will "
                            "assign P12345 as sequence ID; if you "
                            "select atomic structure 3lqd.cif, chain B, "
                            "SCIPION will assign 3lqd_B as sequence ID. In "
                            "the rest of cases, the Sequence name "
                            "will be selected as starting Sequence ID.")
         form.addParam('inputSequenceName', params.StringParam, important=True,
                       label="Sequence name", allowsNull=False,
                       help="Write a sequence name.")
         form.addParam('inputSequenceDescription', params.StringParam,
                       label="Sequence description",
                       allowsNull=True,
+                      expertLevel=params.LEVEL_ADVANCED,
                       help="Write a description for your sequence. Otherwise, "
                            "if the "
-                           "sequence derives from GeneBank/UniProt/PDB "
+                           "sequence derives from GenBank/UniProt/PDB "
                            "databases, the respective database description "
                            "will be "
                            "selected as starting sequence description. In "
                            "the rest of cases, no sequence description will "
                            "be added.")
         form.addParam('inputSequence', params.EnumParam,
                       pointerClass='Sequence',
-                      choices=emconv.SEQ_TYPE,
+                      choices=Alphabet.SEQ_TYPE,
                       display=params.EnumParam.DISPLAY_HLIST,
                       label="Import sequence of ",
-                      default=emconv.SEQ_TYPE_AMINOACIDS,
+                      default=Alphabet.AMINOACIDS,
                       help='Select the type of sequence to import.')
         form.addParam('inputProteinSequence', params.EnumParam,
                       choices=['plain text', 'atomic structure', 'file',
-                               'UniProt ID'],
+                               'UniProt ID', 'NCBI/GenBank ID'],
                       display=params.EnumParam.DISPLAY_HLIST,
-                      condition='inputSequence == %d' % emconv.SEQ_TYPE_AMINOACIDS,
+                      condition='inputSequence == %d' % Alphabet.AMINOACIDS,
                       label="From ",
                       default=self.IMPORT_FROM_PLAIN_TEXT,
                       help='Select one of the four options: write the '
                            'aminoacid sequence or import it '
                            'from a previously loaded atomic structure, a local '
                            'file or an online server.')
         form.addParam('proteinIUPACalphabet', params.EnumParam,
-                      choices=emconv.IUPAC_PROTEIN_ALPHABET,
+                      choices=list(Alphabet.alphabetsLabels.values())[:Alphabet.AMBIGOUS_DNA_ALPHABET],
                       display=params.EnumParam.DISPLAY_HLIST,
                       condition='inputSequence == %d and '
                                 'inputProteinSequence == %d' %
-                                (emconv.SEQ_TYPE_AMINOACIDS,
+                                ( Alphabet.AMINOACIDS,
                                  self.IMPORT_FROM_PLAIN_TEXT),
                       label="IUPAC Protein alphabet: ",
-                      default=emconv.EXTENDED_PROTEIN_ALPHABET,
+                      default=Alphabet.EXTENDED_PROTEIN_ALPHABET,
                       help='Your raw sequence will be cleaned according '
                            'a certain alphabet, i.e., only the letters '
                            'contained in the alphabet will be maintained in '
                            'the sequence. Select thus the type of protein '
                            'alphabet in order to accomplish the '
                            'cleaning:\n\nProtein alphabet: IUPAC protein '
                            'alphabet of the 20 standard amino acids; uppercase'
@@ -133,45 +137,48 @@
                            'Unknown or other amino acid\n*Z = Glx*; Glutamic '
                            'acid (E) or Glutamine (Q)\n*J = Xle*; Leucine ('
                            'L) or Isoleucine (I), used in mass-spec (NMR)\n'
                            '*U = Sec*; Selenocysteine\n*O = Pyl*; '
                            'Pyrrolysine\nThis alphabet is not intended to be '
                            'used with X for Selenocysteine (an ad-hoc standard'
                            ' prior to the IUPAC adoption of U instead).\n')
+
         form.addParam('uniProtSequence', params.StringParam,
                       condition='inputSequence == %d and '
                                 'inputProteinSequence == %d' %
-                                (emconv.SEQ_TYPE_AMINOACIDS,
+                                (Alphabet.AMINOACIDS,
                                  self.IMPORT_FROM_UNIPROT),
                       label="UniProt name/ID ", allowsNull=True,
                       help='Write a UniProt ID (six or ten alphanumeric '
                            'characters; examples: A2BC19, P12345, '
                            'A0A022YWF9, DGAL_ECOLI).\n You can convert other '
                            'database identifiers to UniProt accession codes '
                            'by using the "ID Mapping" tab on '
                            'https://www.uniprot.org/')
         form.addParam('inputNucleotideSequence', params.EnumParam,
                       choices=['plain text', 'atomic structure', 'file',
-                               'GeneBank'],
+                               'NCBI/GenBank ID'],
                       display=params.EnumParam.DISPLAY_HLIST,
-                      condition='inputSequence == %d' % emconv.SEQ_TYPE_NUCLEOTIDES,
+                      condition='inputSequence == %d' %  Alphabet.NUCLEOTIDES,
                       label="From ",
                       default=self.IMPORT_FROM_NUCLEOTIDE_PLAIN_TEXT,
-                      help='Select one of the four options: write the '
+                      help='Select one of the five options: write the '
                            'nucleic acid sequence or import it '
                            'from a local file or an online server.')
         form.addParam('nucleotideIUPACalphabet', params.EnumParam,
-                      choices=emconv.IUPAC_NUCLEOTIDE_ALPHABET,
+                      # move to first element in label list that is nucleotide 
+                      choices=list(Alphabet.alphabetsLabels.values())[Alphabet.AMBIGOUS_DNA_ALPHABET:],
                       display=params.EnumParam.DISPLAY_HLIST,
                       condition='inputSequence == %d and '
                                 'inputNucleotideSequence == %d' %
-                                (emconv.SEQ_TYPE_NUCLEOTIDES,
+                                (Alphabet.NUCLEOTIDES,
                                  self.IMPORT_FROM_NUCLEOTIDE_PLAIN_TEXT),
                       label="IUPAC Nucleic acid alphabet: ",
-                      default=emconv.EXTENDED_DNA_ALPHABET,
+                      # subtract first element of type nucleotide
+                      default=Alphabet.EXTENDED_DNA_ALPHABET - Alphabet.EXTENDED_DNA_ALPHABET,
                       help='Your raw sequence will be cleaned according '
                            'a certain alphabet, i.e., only the letters '
                            'contained in the alphabet will be maintained in '
                            'the sequence. Select thus the type of nucleic '
                            'acid alphabet in order to accomplish the '
                            'cleaning:\n\n Ambiguous DNA alphabet: Uppercase '
                            'IUPAC ambiguous DNA: *GATCRYWSMKHBVDN*.\n\n'
@@ -185,17 +192,17 @@
                            'RNA alphabet: Generic single letter RNA '
                            'alphabet.\n\n')
         form.addParam('inputRawSequence', params.StringParam,
                       condition='(inputSequence == %d and '
                                 'inputProteinSequence == %d) or '
                                 '(inputSequence == %d and '
                                 'inputNucleotideSequence == %d) ' %
-                                (emconv.SEQ_TYPE_AMINOACIDS,
+                                (Alphabet.AMINOACIDS,
                                  self.IMPORT_FROM_PLAIN_TEXT,
-                                 emconv.SEQ_TYPE_NUCLEOTIDES,
+                                 Alphabet.NUCLEOTIDES,
                                  self.IMPORT_FROM_NUCLEOTIDE_PLAIN_TEXT),
                       label="Write your sequence here:", important=True,
                       help="Write the aminoacid or nucleotide raw sequence.\n")
         form.addParam('inputStructureSequence', params.EnumParam,
                       choices=['id', 'file'],
                       condition='inputProteinSequence == %d or '
                                 'inputNucleotideSequence == %d' %
@@ -243,49 +250,57 @@
                                  self.IMPORT_FROM_NUCLEOTIDE_FILES),
                       allowsNull=True,
                       help='Specify a path to desired aminoacid or '
                            'nucleic acid sequence '
                            'file.\nIf your file contains more than one '
                            'sequence, only the first one will be considered.')
         form.addParam('geneBankSequence', params.StringParam,
-                      condition='inputSequence == %d and '
-                                'inputNucleotideSequence == %d' %
-                                (emconv.SEQ_TYPE_NUCLEOTIDES,
-                                 self.IMPORT_FROM_GENEBANK),
-                      label="GeneBank accession ", allowsNull=True,
-                      help='Write a GeneBank accession.\n')
+                      condition='(inputSequence == %d and '
+                                'inputNucleotideSequence == %d) or '
+                                '(inputSequence == %d and '
+                                'inputProteinSequence == %d)' %
+                                (Alphabet.NUCLEOTIDES,
+                                 self.IMPORT_FROM_NUCLEOTIDE_GENEBANK,
+                                 Alphabet.AMINOACIDS,
+                                 self.IMPORT_FROM_PROTEIN_GENEBANK),
+                      label="GenBank accession ", allowsNull=True,
+                      help='Write a GenBank accession.\n')
+
 
     def _insertAllSteps(self):
         self.name = self.inputSequenceName.get()
-
-        if self.inputSequence == emconv.SEQ_TYPE_AMINOACIDS:
+        if self.inputSequence == Alphabet.AMINOACIDS:
             if self.inputProteinSequence == self.IMPORT_FROM_PLAIN_TEXT:
                 rawSequence = self.inputRawSequence.get()
                 self._insertFunctionStep('getRawSequenceStep', rawSequence)
             elif self.inputProteinSequence == self.IMPORT_FROM_STRUCTURE:
                 chainId = self.inputStructureChain.get()
                 self._insertFunctionStep('getSequenceOfChainStep', chainId)
             elif self.inputProteinSequence == self.IMPORT_FROM_UNIPROT:
                 sequenceDB = self._getUniProtID()
                 self._insertFunctionStep('sequenceDatabaseDownloadStep',
                                          sequenceDB)
+            elif self.inputProteinSequence == self.IMPORT_FROM_PROTEIN_GENEBANK:
+                sequenceDB = self._getGeneBankID()
+                self._insertFunctionStep('sequenceDatabaseDownloadStep',
+                                         sequenceDB)
             elif self.inputProteinSequence == self.IMPORT_FROM_FILES:
                 self.sequenceFile = self.fileSequence.get()
                 sequenceFile = self.sequenceFile
                 self._insertFunctionStep('fileDownloadStep', sequenceFile)
         else:
             if self.inputNucleotideSequence == \
                     self.IMPORT_FROM_NUCLEOTIDE_PLAIN_TEXT:
                 rawSequence = self.inputRawSequence.get()
                 self._insertFunctionStep('getRawSequenceStep', rawSequence)
             elif self.inputNucleotideSequence == \
                     self.IMPORT_FROM_NUCLEOTIDE_STRUCTURE:
                 chainId = self.inputStructureChain.get()
                 self._insertFunctionStep('getSequenceOfChainStep', chainId)
-            elif self.inputNucleotideSequence == self.IMPORT_FROM_GENEBANK:
+            elif self.inputNucleotideSequence == self.IMPORT_FROM_NUCLEOTIDE_GENEBANK:
                 sequenceDB = self._getGeneBankID()
                 self._insertFunctionStep('sequenceDatabaseDownloadStep',
                                          sequenceDB)
             elif self.inputNucleotideSequence == \
                     self.IMPORT_FROM_NUCLEOTIDE_FILES:
                 self.sequenceFile = self.fileSequence.get()
                 sequenceFile = self.sequenceFile
@@ -295,17 +310,21 @@
 
     def getRawSequenceStep(self, rawSequence):
         # user types sequence
         if self.inputSequenceID.get() is not None:
             self.id = self.inputSequenceID.get()
         else:
             self.id = self.name
-        self.alphabet = self._getAlphabet()  # index number
-        self.sequence = emconv.cleanSequenceScipion(self.inputSequence ==
-                                                    emconv.SEQ_TYPE_AMINOACIDS,
+        isAmino = self.inputSequence == Alphabet.AMINOACIDS
+        if isAmino:
+            self.alphabet =  self.proteinIUPACalphabet.get()
+        else:
+            self.alphabet =  self.nucleotideIUPACalphabet.get()
+
+        self.sequence = emconv.cleanSequenceScipion(isAmino, 
                                                     self.alphabet, rawSequence)
 
     def getSequenceOfChainStep(self, chainId):
         # sequece is obtained from PDB file
 
         # form has a wizard that creates label with the format
         # [model: x, chain: x, xxx residues]
@@ -324,106 +343,109 @@
                 # wizard has not used and the file has not been downloaded yet
                 self.structureHandler.readFromPDBDatabase(pdbID, dir="/tmp")
             self.structureHandler.read(tmpFilePath)
         else:
             # PDB from file
             self.structureHandler.read(self.pdbFile.get())
 
-        _sequence = self.structureHandler.getSequenceFromChain(
-            selectedModel, selectedChain)
+        _sequence, alphabet = self.structureHandler.getSequenceFromChain(
+            selectedModel, selectedChain, returnAlphabet =True)
         self.sequence = str(_sequence)
-        self.alphabet = emconv.alphabetToIndex(self.inputSequence ==
-                                               emconv.SEQ_TYPE_AMINOACIDS,
-                                               _sequence.alphabet)
+        self.alphabet = alphabet #emconv.alphabetToIndex(self.inputSequence ==
+                                           #    Alphabet.AMINOACIDS,
+                                           #    _sequence.alphabet)
 
         # Assignation of sequence ID: if the user has provided a specific
         #  ID, this will be adopted by default; otherwise, a sequence ID
         # related with the starting structure will be selected.
         if self.inputSequenceID.get() is not None:
             self.id = self.inputSequenceID.get()
         else:
             self.id = self.structureHandler.getFullID(
                 selectedModel, selectedChain)
 
         print("Selected chain: %s from model: %s from structure: %s" %
               (selectedChain, selectedModel, self.structureHandler.structure.get_id()))
 
     def sequenceDatabaseDownloadStep(self, sequenceDB):
-        """Download UniProt/GeneBank sequence from its respective database
+        """Download UniProt/GenBank sequence from its respective database
         """
         # sequenceDB = str(sequenceDB)
+        isAminoacid=(self.inputSequence == Alphabet.AMINOACIDS)
         if self.uniProtSequence.get() is not None:
-            seqHandler = emconv.SequenceHandler()
+            seqHandler = emconv.SequenceHandler(iUPACAlphabet=Alphabet.EXTENDED_PROTEIN_ALPHABET)
+            dataBase = 'UniProt'
 
         elif self._getGeneBankID() is not None:
-            seqHandler = emconv.SequenceHandler(isAminoacid=False)
-
-        record, error = seqHandler.downloadSeqFromDatabase(sequenceDB)
-        if record is None:
+            if isAminoacid:
+                seqHandler = emconv.SequenceHandler(iUPACAlphabet=Alphabet.EXTENDED_PROTEIN_ALPHABET)
+            else:
+                seqHandler = emconv.SequenceHandler(iUPACAlphabet=Alphabet.NUCLEOTIDES_ALPHABET)
+            dataBase = 'GeneBank'
+        seqDic, error = seqHandler.downloadSeqFromDatabase(seqID = sequenceDB, dataBase=dataBase)
+        if seqDic is None:
             print("Error: ", error)
             self.setAborted()
             exit(0)
 
         if self.inputSequenceID.get() is not None:
             self.id = self.inputSequenceID.get()
         elif sequenceDB != '':
             self.id = sequenceDB
         else:
             self.id = self.name
-        if record.description != '':
-            self.description = record.description
+        if seqDic['description'] != '':
+            self.description = seqDic['description']
 
-        self.sequence = str(record.seq)
-        self.alphabet = emconv.alphabetToIndex(self.inputSequence ==
-                                               emconv.SEQ_TYPE_AMINOACIDS, record.seq.alphabet)
+        self.sequence = seqDic['sequence']
+        self.alphabet = seqDic['alphabet'] 
 
     def fileDownloadStep(self, sequenceFile):
         # If sequencePath contains more than one sequence, only
         # the first one will be considered
         seqHandler = emconv.SequenceHandler()
-        record = seqHandler.downloadSeqFromFile(sequenceFile,
-                                                type="fasta")
+        seqDic = seqHandler.readSequenceFromFile(sequenceFile,
+                                                 type="fasta",
+                                                 isAmino= self.inputSequence.get()==Alphabet.AMINOACIDS)
         if self.inputSequenceID.get() is not None:
             self.id = self.inputSequenceID.get()
-        elif record.id != '':
-            self.id = record.id
+        elif seqDic['seqID'] != '':
+            self.id = seqDic['seqID']
         else:
             self.id = self.name
-        if record.description != '':
-            self.description = record.description
+        if seqDic['description'] != '':
+            self.description = seqDic['description']
 
-        self.sequence = str(record.seq)
-        self.alphabet = emconv.alphabetToIndex(self.inputSequence ==
-                                               emconv.SEQ_TYPE_AMINOACIDS, record.seq.alphabet)
+        self.sequence = seqDic['sequence']
+        self.alphabet = seqDic['alphabet']
 
     def createOutputStep(self):
         """ Register the output object. """
 
         if self.inputSequenceDescription.get() is not None:
             self.description = self.inputSequenceDescription.get()
         elif hasattr(self, 'description'):
             pass
         else:
             self.description = ''
-
         seq = Sequence(name=self.name,
                        sequence=self.sequence,
                        alphabet=self.alphabet,
                        isAminoacids=(self.inputSequence ==
-                                     emconv.SEQ_TYPE_AMINOACIDS),
+                                     Alphabet.AMINOACIDS),
                        id=self.id, description=self.description)
         outputs = {'outputSequence': seq}
         self._defineOutputs(**outputs)
 
     def _summary(self):
         summary = []
         self.name = self.inputSequenceName.get()
         uniProtId = self._getUniProtID()
         geneBankID = self._getGeneBankID()
-        if self.inputSequence == emconv.SEQ_TYPE_AMINOACIDS:
+        if self.inputSequence == Alphabet.AMINOACIDS:
             summary.append('Sequence of aminoacids:\n')
             if self.inputProteinSequence == self.IMPORT_FROM_PLAIN_TEXT:
                 summary.append("Sequence *%s* imported from plain text\n"
                                % self.name)
             elif self.inputProteinSequence == self.IMPORT_FROM_STRUCTURE:
                 if self.inputStructureSequence == \
                         self.IMPORT_STRUCTURE_FROM_ID:
@@ -455,16 +477,16 @@
                     summary.append("Sequence *%s* imported from atomic "
                                    "structure *%s.cif*\n"
                                    % (self.name, self.pdbId.get()))
                 elif self.inputStructureSequence == \
                         self.IMPORT_STRUCTURE_FROM_FILES:
                     summary.append("Sequence *%s* imported from file *%s*\n"
                                    % (self.name, self.pdbFile.get()))
-            elif self.inputNucleotideSequence == self.IMPORT_FROM_GENEBANK:
-                summary.append("Sequence *%s* imported from geneBank ID "
+            elif self.inputNucleotideSequence == self.IMPORT_FROM_NUCLEOTIDE_GENEBANK:
+                summary.append("Sequence *%s* imported from GenBank ID "
                                "*%s*\n"
                                % (self.name, geneBankID))
             elif self.inputNucleotideSequence == \
                     self.IMPORT_FROM_NUCLEOTIDE_FILES:
                 summary.append("Sequence *%s* imported from file name: "
                                "*%s*\n"
                                % (self.name, self.fileSequence.get()))
@@ -480,11 +502,11 @@
     def _getUniProtID(self):
         return self.uniProtSequence.get()
 
     def _getGeneBankID(self):
         return self.geneBankSequence
 
     def _getAlphabet(self):
-        if self.inputSequence == emconv.SEQ_TYPE_AMINOACIDS:
+        if self.inputSequence == Alphabet.AMINOACIDS:
             return self.proteinIUPACalphabet.get()
         else:
-            return self.nucleotideIUPACalphabet.get()
+            return self.nucleotideIUPACalphabet.get() + Alphabet.AMBIGOUS_DNA_ALPHABET
```

### Comparing `scipion-em-3.0.9/pwem/protocols/protocol_import/volumes.py` & `scipion-em-3.1.0/pwem/protocols/protocol_import/volumes.py`

 * *Files 13% similar despite different names*

```diff
@@ -20,35 +20,43 @@
 # * Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA
 # * 02111-1307  USA
 # *
 # *  All comments concerning this program package may be sent to the
 # *  e-mail address 'scipion@cnb.csic.es'
 # *
 # **************************************************************************
+import enum
+import logging
+import os.path
 
-
-from os.path import exists, basename, abspath, relpath, join
+logger = logging.getLogger(__name__)
+from os.path import exists, basename, abspath, relpath, join, splitext
 from os import stat
 from numpy import array
 from numpy.linalg import norm
+import glob
 
 import pyworkflow.utils as pwutils
 import pyworkflow.protocol.params as params
 import pwem.objects as emobj
 import pwem.convert as emconv
 from pwem import emlib
 
 from .base import ProtImportFiles
 from .images import ProtImportImages
 
+class ImportVolumeOutputs(enum.Enum):
+    outputVolume = emobj.Volume
+    outputVolumes = emobj.SetOfVolumes
 
 class ProtImportVolumes(ProtImportImages):
     """Protocol to import a set of volumes to the project"""
     _outputClassName = 'SetOfVolumes'
     _label = 'import volumes'
+    _possibleOutputs = ImportVolumeOutputs
     IMPORT_FROM_EMDB = 1
 
     def __init__(self, **args):
         ProtImportImages.__init__(self, **args)
 
     def _getImportChoices(self):
         """ Return a list of possible choices
@@ -129,125 +137,136 @@
                       label="x", help="offset along x axis (Angstroms)")
         form.addParam('y', params.FloatParam, condition='setOrigCoord',
                       label="y", help="offset along y axis (Angstroms)")
         form.addParam('z', params.FloatParam, condition='setOrigCoord',
                       label="z", help="offset along z axis (Angstroms)")
 
     def _insertAllSteps(self):
-        self._insertFunctionStep('importVolumesStep',
+        if self.importFrom == self.IMPORT_FROM_FILES:
+            self._insertFunctionStep(self.importFromFileStep,
                                  self.getPattern(),
                                  self.samplingRate.get(),
                                  self.setOrigCoord.get())
+        else:
+            self._insertFunctionStep(self.importFromEMDBStep)
 
     # --------------------------- STEPS functions -----------------------------
 
-    def importVolumesStep(self, pattern, samplingRate, setOrigCoord=False):
+    def importFromFileStep(self, pattern, samplingRate, setOrigCoord=False):
         """ Copy images matching the filename pattern
         Register other parameters.
         """
         volSet = self._createSetOfVolumes()
         vol = emobj.Volume()
 
-        if self.importFrom == self.IMPORT_FROM_FILES:
-            self.info("Using pattern: '%s'" % pattern)
+        self.info("Using pattern: '%s'" % pattern)
 
-            # Create a Volume template object
-            vol.setSamplingRate(samplingRate)
+        # Create a Volume template object
+        vol.setSamplingRate(samplingRate)
 
-            imgh = emlib.image.ImageHandler()
+        imgh = emlib.image.ImageHandler()
 
-            volSet.setSamplingRate(samplingRate)
+        volSet.setSamplingRate(samplingRate)
 
-            for fileName, fileId in self.iterFiles():
-                x, y, z, n = imgh.getDimensions(fileName)
-                if fileName.endswith('.mrc') or fileName.endswith('.map'):
-                    fileName += ':mrc'
-                    if z == 1 and n != 1:
-                        zDim = n
-                        n = 1
-                    else:
-                        zDim = z
+        for fileName, fileId in self.iterFiles():
+            x, y, z, n = imgh.getDimensions(fileName)
+            if fileName.endswith('.mrc') or fileName.endswith('.map'):
+                fileName += ':mrc'
+                if z == 1 and n != 1:
+                    zDim = n
+                    n = 1
                 else:
                     zDim = z
-                origin = emobj.Transform()
-                if setOrigCoord:
-                    origin.setShiftsTuple(self._getOrigCoord())
-                else:
-                    origin.setShifts(x / -2. * samplingRate,
-                                     y / -2. * samplingRate,
-                                     zDim / -2. * samplingRate)
-
-                vol.setOrigin(origin)  # read origin from form
-
-                if self.copyFiles or setOrigCoord:
-                    newFileName = abspath(self._getVolumeFileName(fileName, "mrc"))
-                    emconv.Ccp4Header.fixFile(fileName, newFileName, origin.getShifts(),
+            else:
+                zDim = z
+            origin = emobj.Transform()
+            if setOrigCoord:
+                origin.setShiftsTuple(self._getOrigCoord())
+            else:
+                origin.setShifts(x / -2. * samplingRate,
+                                 y / -2. * samplingRate,
+                                 zDim / -2. * samplingRate)
+
+            vol.setOrigin(origin)  # read origin from form
+
+            if self.copyFiles or setOrigCoord:
+                newFileName = abspath(self._getVolumeFileName(fileName, "mrc"))
+                emconv.Ccp4Header.fixFile(fileName, newFileName, origin.getShifts(),
+                                          samplingRate, emconv.Ccp4Header.ORIGIN)
+                if self.setHalfMaps.get():
+                    newFileName1 = abspath(self._getVolumeFileName(self.half1map.get(), "mrc"))
+                    emconv.Ccp4Header.fixFile(self.half1map.get(), newFileName1, origin.getShifts(),
+                                              samplingRate, emconv.Ccp4Header.ORIGIN)
+                    newFileName2 = abspath(self._getVolumeFileName(self.half2map.get(), "mrc"))
+                    emconv.Ccp4Header.fixFile(self.half2map.get(), newFileName2, origin.getShifts(),
                                               samplingRate, emconv.Ccp4Header.ORIGIN)
-                    if self.setHalfMaps.get():
-                        newFileName1 = abspath(self._getVolumeFileName(self.half1map.get(), "mrc"))
-                        emconv.Ccp4Header.fixFile(self.half1map.get(), newFileName1, origin.getShifts(),
-                                                  samplingRate, emconv.Ccp4Header.ORIGIN)
-                        newFileName2 = abspath(self._getVolumeFileName(self.half2map.get(), "mrc"))
-                        emconv.Ccp4Header.fixFile(self.half2map.get(), newFileName2, origin.getShifts(),
-                                                  samplingRate, emconv.Ccp4Header.ORIGIN)
-
-                        vol.setHalfMaps([relpath(newFileName1), relpath(newFileName2)])
-                else:
-                    newFileName = abspath(self._getVolumeFileName(fileName))
-
-                    if fileName.endswith(':mrc'):
-                        fileName = fileName[:-4]
 
-                    pwutils.createAbsLink(fileName, newFileName)
-                    if self.setHalfMaps.get():
-                        pwutils.createAbsLink(self.half1map.get(),
-                                              abspath(self._getVolumeFileName(self.half1map.get())))
-                        pwutils.createAbsLink(self.half2map.get(),
-                                              abspath(self._getVolumeFileName(self.half2map.get())))
-
-                        vol.setHalfMaps([relpath(self._getVolumeFileName(self.half1map.get())),
-                                         relpath(self._getVolumeFileName(self.half2map.get()))
-                                         ])
-
-                # Make newFileName relative
-                # https://github.com/I2PC/scipion/issues/1935
-                newFileName = relpath(newFileName)
-                if n == 1:
+                    vol.setHalfMaps([relpath(newFileName1), relpath(newFileName2)])
+            else:
+                newFileName = abspath(self._getVolumeFileName(fileName))
+
+                if fileName.endswith(':mrc'):
+                    fileName = fileName[:-4]
+
+                pwutils.createAbsLink(fileName, newFileName)
+                if self.setHalfMaps.get():
+                    pwutils.createAbsLink(self.half1map.get(),
+                                          abspath(self._getVolumeFileName(self.half1map.get())))
+                    pwutils.createAbsLink(self.half2map.get(),
+                                          abspath(self._getVolumeFileName(self.half2map.get())))
+
+                    vol.setHalfMaps([relpath(self._getVolumeFileName(self.half1map.get())),
+                                     relpath(self._getVolumeFileName(self.half2map.get()))
+                                     ])
+
+            # Make newFileName relative
+            # https://github.com/I2PC/scipion/issues/1935
+            newFileName = relpath(newFileName)
+            if n == 1:
+                vol.cleanObjId()
+                vol.setFileName(newFileName)
+                vol.setObjComment(vol.getBaseName())
+                volSet.append(vol)
+            else:
+                for index in range(1, n + 1):
                     vol.cleanObjId()
-                    vol.setFileName(newFileName)
+                    vol.setLocation(index, newFileName)
+                    vol.setObjComment("%s@%s" % (index, vol.getBaseName()))
                     volSet.append(vol)
-                else:
-                    for index in range(1, n + 1):
-                        vol.cleanObjId()
-                        vol.setLocation(index, newFileName)
-                        volSet.append(vol)
-        else:  # import from EMDB
-            self.info("Downloading map with ID = %s" % self.emdbId)
-            try:
-                localFileName, sampling, origin = \
-                    fetch_emdb_map(self.emdbId,
-                                   self._getExtraPath(),
-                                   self._getTmpPath())
-            except Exception as e:
-                print(e)
-                return
-            # open volume and fill sampling and origin
-            self.samplingRate.set(sampling)
-            self._store(self.samplingRate)
-            vol.setSamplingRate(sampling)
-            vol.setFileName(localFileName)
-            from pwem.objects.data import Transform
-            originMat = Transform()
-            originMat.setShifts(origin[0], origin[1], origin[2])
-            vol.setOrigin(originMat)
 
         if volSet.getSize() > 1:
-            self._defineOutputs(outputVolumes=volSet)
+            self._defineOutputs(**{ImportVolumeOutputs.outputVolumes.name:volSet})
         else:
-            self._defineOutputs(outputVolume=vol)
+            self._defineOutputs(**{ImportVolumeOutputs.outputVolume.name:vol})
+
+    def importFromEMDBStep(self):
+        """ Copy images matching the filename pattern
+        Register other parameters.
+        """
+        vol = emobj.Volume()
+
+        self.info("Downloading map with ID = %s" % self.emdbId)
+
+        localFileName, sampling, origin = \
+            fetch_emdb_map(self.emdbId,
+                           self._getExtraPath(),
+                           self._getTmpPath())
+
+        # open volume and fill sampling and origin
+        self.samplingRate.set(sampling)
+        self._store(self.samplingRate)
+        vol.setSamplingRate(sampling)
+        vol.setFileName(localFileName)
+        from pwem.objects.data import Transform
+        originMat = Transform()
+        originMat.setShifts(origin[0], origin[1], origin[2])
+        vol.setOrigin(originMat)
+
+        self._defineOutputs(**{ImportVolumeOutputs.outputVolume.name:vol})
+
 
     # --------------------------- INFO functions ------------------------------
 
     def _getVolMessage(self):
         if self.hasAttribute('outputVolume'):
             return "Volume %s" % self.getObjectTag('outputVolume')
         else:
@@ -387,55 +406,187 @@
                 self.pdbFile.get())):
             errors.append("Atomic structure not found at *%s*" %
                           self.pdbFile.get())
         # TODO: maybe also validate that if exists is a valid PDB file
         return errors
 
 
+class ProtImportSetOfAtomStructs(ProtImportFiles):
+    """ Protocol to import a set of atomic structure  to the project.
+    Format may be PDB or MMCIF"""
+    _label = 'import set of atomic structures'
+    _OUTNAME = 'outputAtomStructs'
+    _possibleOutputs = {_OUTNAME: emobj.SetOfAtomStructs}
+
+    IMPORT_FROM_ID = 0
+    IMPORT_FROM_FILES = 1
+
+    def __init__(self, **args):
+      ProtImportFiles.__init__(self, **args)
+
+    def _defineParams(self, form):
+      form.addSection(label='Input')
+      form.addParam('inputPdbData', params.EnumParam, choices=['id', 'file'],
+                    label="Import atomic structures from",
+                    default=self.IMPORT_FROM_ID,
+                    display=params.EnumParam.DISPLAY_HLIST,
+                    help='Import mmCIF data from online server or local files')
+      form.addParam('pdbIds', params.StringParam,
+                    condition='inputPdbData == IMPORT_FROM_ID',
+                    label="Atomic structure IDs ", allowsNull=True,
+                    help='Type a mmCIF ID (four alphanumeric characters, comma-separated)\n'
+                         'i.e: 5ni1, 1ake')
+      form.addParam('filesPath', params.PathParam, label="Files directory path: ",
+                    condition='inputPdbData == IMPORT_FROM_FILES',
+                    allowsNull=True,
+                    help="Specify a path to the directory where the files are stored.\n"
+                         "The path can also contain wildcards to select"
+                         "from several folders. \n\n"
+                         "Examples:\n"
+                         "  ~/project/data/day??_files/\n"
+                         "Each '?' represents one unknown character\n\n"
+                         "  ~/project/data/day*_files/\n"
+                         "'*' represents any number of unknown characters\n\n"
+                         "  ~/project/data/day##_files/\n"
+                         "'##' represents two digits that will be used as "
+                         "file ID\n\n"
+                         "NOTE: wildcard characters ('*', '?', '#') "
+                         "cannot appear in the actual path.)")
+      form.addParam('filesPattern', params.StringParam, condition='inputPdbData == IMPORT_FROM_FILES',
+                    label='Pattern: ',
+                    default="*",
+                    help="Pattern of the files to be imported.\n\n"
+                         "The pattern can contain standard wildcards such as\n"
+                         "*, ?, etc, or special ones like ### to mark some\n"
+                         "digits in the filename as ID.\n\n"
+                         "NOTE: wildcards and special characters "
+                         "('*', '?', '#', ':', '%') cannot appear in the "
+                         "actual path.\n\n"
+                         "You may create AtomStruct from PDB (.pdb) or CIF/mmCIF (.cif)")
+
+    def _insertAllSteps(self):
+      if self.inputPdbData == self.IMPORT_FROM_ID:
+        self._insertFunctionStep('pdbDownloadStep')
+      else:
+        filenames = []
+        for fn in glob.glob(join(self.filesPath.get(), self.filesPattern.get())):
+          filenames.append(fn)
+        self._insertFunctionStep('createOutputStep', filenames)
+
+    def pdbDownloadStep(self):
+      """Download all pdb files in file_list and unzip them.
+      """
+      aSH = emconv.AtomicStructHandler()
+      ASPaths = []
+      for pdbId in self.pdbIds.get().split(','):
+          print("retrieving atomic structure with ID = %s" % pdbId)
+          ASPaths.append(aSH.readFromPDBDatabase(pdbId.strip(), type='mmCif', dir=self._getExtraPath()))
+      self.createOutputStep(ASPaths)
+
+    def createOutputStep(self, atomStructPaths):
+      """ Copy the PDB structures and register the output object.
+      """
+      outASs = emobj.SetOfAtomStructs().create(self._getPath())
+      
+      numStructs = len(atomStructPaths)
+      padding_format_str = '%0' + str(len(str(numStructs))) + 'd'
+
+      for atomStructPath in atomStructPaths:
+          if not exists(atomStructPath):
+              raise Exception("Atomic structure not found at *%s*" % atomStructPath)
+
+          baseName = basename(atomStructPath)
+          localPath = abspath(self._getExtraPath(baseName))
+
+          if str(atomStructPath) != str(localPath):  # from local file
+              if exists(localPath):
+                  localPath = splitext(localPath)[0] + padding_format_str % (i+1) + splitext(localPath)[1]
+                  i += 1
+              else:
+                  i = 0
+                  
+              pwutils.copyFile(atomStructPath, localPath)
+
+          localPath = relpath(localPath)
+
+          outASs.append(emobj.AtomStruct(filename=localPath))
+
+      self._defineOutputs(**{self._OUTNAME:outASs})
+
+
+    def _summary(self):
+      if self.inputPdbData == self.IMPORT_FROM_ID:
+        summary = ['Atomic structure imported from IDs: *%s*' %
+                   self.pdbIds]
+      else:
+        summary = ['Atomic structure imported from files: *%s*' %
+                   self.filesPattern]
+
+      return summary
+
+    def _validate(self):
+      errors = []
+      return errors
+
+
 ######################################
 
 
 def fetch_emdb_map(id, directory, tmpDirectory):
     """ get map from emd
     :param id: 3D MAP ID in EMDB
     :return: local 3Dmap filename
     """
     import socket
 
     # get computer name and select server
-    url_rest_api = "https://www.ebi.ac.uk/pdbe/api/emdb/entry/map/EMD-%d"
+    url_rest_api = "https://www.ebi.ac.uk/emdb/api/entry/map/%s"
     hname = socket.gethostname()
     if hname.endswith('.edu') or hname.endswith('.gov'):
         site = 'ftp.wwpdb.org'
         url_pattern = 'ftp://%s/pub/emdb/structures/EMD-%s/map/%s'
     elif hname.endswith('.cn'):
         site = 'ftp.emdb-china.org'
         url_pattern = 'ftp://%s/structures/EMD-%s/map/%s'
     else:
         site = 'ftp.ebi.ac.uk'
         url_pattern = 'ftp://%s/pub/databases/emdb/structures/EMD-%s/map/%s'
 
+    if len(str(id)) < 4:
+        id = '%04d' % id
+    else:
+        id = '%d' % id
+
     map_name = 'emd_%s.map' % id
     map_gz_name = map_name + '.gz'
     map_url = url_pattern % (site, id, map_gz_name)
-    name = 'EMD-%d' % id
+    name = 'EMD-%s' % id
     minimum_map_size = 8192  # bytes
     url_rest_api = url_rest_api % id
 
-    try:
-        map_path, samplingAPI, originAPI = fetch_file(map_url,
-                                                      url_rest_api,
-                                                      name,
-                                                      minimum_map_size,
-                                                      directory,
-                                                      tmpDirectory,
-                                                      map_name
-                                                      )
-    except Exception as e:
-        raise Exception("Cannot retrieve File from EMDB", e)
+    nTimes = 3
+    for i in range(nTimes):  # if error repeat the fetch file up to nTimes
+        try:
+            # raise Exception("test")  # uncomment to test this loop
+            map_path, samplingAPI, originAPI = fetch_file(map_url,
+                                                          url_rest_api,
+                                                          name,
+                                                          minimum_map_size,
+                                                          directory,
+                                                          tmpDirectory,
+                                                          map_name
+                                                          )
+            break
+        except Exception as e:
+            if i+1<nTimes:
+                logger.info("Retrieving 3D map with id=%s failed retrying (%d/%d)" %
+                  (id, i+1, nTimes))
+            else:
+                logger.error("Cannot retrieve File from EMDB", exc_info=e)
+
 
     originAPI = array(originAPI) * samplingAPI  # convert to Angstrom
     # check consistency between file header and rest API
     ccp4header = emconv.Ccp4Header(map_path, readHeader=True)
     samplingHeader = ccp4header.computeSampling()  # unit = A/px
     originHeader = array(ccp4header.getOrigin())  # unit = A
 
@@ -447,15 +598,15 @@
               "###########################\n" % (samplingAPI, samplingHeader))
 
     if norm(originHeader - originAPI) >= 0.1:
         print("###########################\n"
               "WARNING: origin  stored in EMDB\n"
               "database and 3D map header file do not match\n"
               "API=%f, header=%f\n"
-              "###########################\n" % (originAPI, originHeader))
+              "###########################\n" % (originAPI[0], originHeader[0]))
     return map_path, samplingAPI, originAPI
 
 
 def fetch_file(url, url_rest_api, name,
                minimum_file_size=8192,
                save_dir='',
                tmp_dir='',
@@ -474,44 +625,44 @@
     :return: local file name
     """
     import urllib.request
     import requests
     noCompressName = join(save_dir, save_name)
     compressName = join(tmp_dir, save_name + ".gz")
 
-    try:
+    # If uncompressed file exists
+    if os.path.exists(noCompressName):
+        logger.info("File fetching skip: file %s exists." % noCompressName)
+    else:
+
+        logger.info("Fetching file from %s" % url)
         urllib.request.urlretrieve(url, filename=compressName)
-        # if retrieval fails retry another time
-        if not exists(compressName):
-            urllib.request.urlretrieve(url, filename=compressName)
-            if not exists(compressName):
-                raise Exception("Can not download file from EMDB")
-
-        json_results = requests.get(url_rest_api).json()
-        sampling_tag = "pixel_spacing"
-        sampling_x_tag = "x"
-        origin_tag = "origin"
-        origin_x_tag = "column"
-        origin_y_tag = "row"
-        origin_z_tag = "section"
-
-        # units A/px
-        results = json_results[name][0]['map']
-        sampling = results[sampling_tag][sampling_x_tag]['value']
-        # units unknown may be pixels since this is integer
-        x = results[origin_tag][origin_x_tag]
-        y = results[origin_tag][origin_y_tag]
-        z = results[origin_tag][origin_z_tag]
-    except Exception as e:
-        print("Error retrieving data from EMDB", str(e))
 
     if stat(compressName).st_size < minimum_file_size:
         raise Exception("File Downloaded from EMDB is empty")
 
     gunzip(compressName, noCompressName)
+
+    logger.info("Fetching metadata from %s" % url_rest_api)
+    json_results = requests.get(url_rest_api).json()
+    sampling_tag = "pixel_spacing"
+    sampling_x_tag = "x"
+    origin_tag = "origin"
+    origin_x_tag = "col"
+    origin_y_tag = "row"
+    origin_z_tag = "sec"
+
+    # units A/px
+    results = json_results['map']
+    sampling = float(results[sampling_tag][sampling_x_tag]['valueOf_'])
+    # units unknown may be pixels since this is integer
+    x = float(results[origin_tag][origin_x_tag])
+    y = float(results[origin_tag][origin_y_tag])
+    z = float(results[origin_tag][origin_z_tag])
+
     return noCompressName, sampling, (x, y, z)
 
 
 def gunzip(gzpath, path):
     import gzip
     gzf = gzip.open(gzpath)
     f = open(path, 'wb')
```

### Comparing `scipion-em-3.0.9/pwem/protocols/protocol_metadata_editor.py` & `scipion-em-3.1.0/pwem/protocols/protocol_set_editor.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # **************************************************************************
 # *
 # * Authors:     Pablo Conesa(pconesa@cnb.csic.es)
+# *              Roberto Marabini(roberto@cnb.csic.es)
 # *
 # * Unidad de  Bioinformatica of Centro Nacional de Biotecnologia , CSIC
 # *
 # * This program is free software; you can redistribute it and/or modify
 # * it under the terms of the GNU General Public License as published by
 # * the Free Software Foundation; either version 3 of the License, or
 # * (at your option) any later version.
@@ -21,56 +22,67 @@
 # *
 # *  All comments concerning this program package may be sent to the
 # *  e-mail address 'scipion@cnb.csic.es'
 # *
 # **************************************************************************
 
 import pyworkflow.protocol.params as params
-import pyworkflow.utils as pwutils
 from pwem.protocols import EMProtocol
+from pwem.objects.data import SetOfParticles
 
+import numpy as np
 
-class ProtMetadataEditor(EMProtocol):
+
+class ProtSetEditor(EMProtocol):
     """
     Protocol to edit attributes of all the items of a set using a formula.
-    This could be useful for corrupting your data for testing purposes or
-    editing some values in the set that make sense to do it. Use this with
-    extreme care, you can easily ruin your processing.
+    This could be useful for editing some values in the set. Use this
+    protocol with extreme care, you can easily produce a set that is
+    not consistent.
     """
-    _label = 'metadata editor'
+    _label = 'edit set'
 
     def _defineParams(self, form):
         """
         Defines the parameters the protocol form will show and its behaviour
         :param form:
         """
-
         form.addSection(label='Input')
-        form.addParam('inputSet', params.PointerParam, pointerClass='EMSet',
+        form.addParam('inputSet', params.PointerParam,
+                      pointerClass='EMSet',
                       label='Set to edit',
                       help='Set which items will be modified.')
-        form.addParam('formula', params.StringParam, label="Formula", important=True,
+        # formula
+        form.addParam('formula', params.StringParam, label="Formula",
                       help='A python code compatible with eval, where item represents each of '
                            'the elements of the set. E.g.: item._resolution.set(item._resolution.get() +1).'
                            'You could also use modules like "import numpy;  item._resolution .... "')
 
     def _insertAllSteps(self):
-        self._insertFunctionStep('editItemsStep')
+        self._insertFunctionStep('formulaStep')
 
-    def editItemsStep(self):
+    def formulaStep(self):
         """
         Goes through all items in the input set and applies the formula to each of them using exec.
         Complex python code could be run separating lines with ;  To use numpy you could do
         import numpy; item._resolution.set(numpy.random.randint(10))
         """
         inputSet = self.inputSet.get()
-
-        modifiedSet = inputSet.create(self._getExtraPath())
-        modifiedSet.copyInfo(inputSet)
+        modifiedSet = inputSet.createCopy(self._getExtraPath(), copyInfo=True)
 
         for sourceItem in inputSet.iterItems():
             item = sourceItem.clone()
             exec(self.formula.get())
             modifiedSet.append(item)
 
-        outputArgs = {self.inputSet.getExtended(): modifiedSet}
+        self.createOutput(self.inputSet, modifiedSet)
+
+    def createOutput(self, inputSet, modifiedSet):
+        """ Save the output set."""
+        outputArgs = {inputSet.getExtended(): modifiedSet}
         self._defineOutputs(**outputArgs)
+
+    def _summary(self):
+
+        return ["The this formula (%s) is/was applied to the items of the input set." % self.formula.get()]
+
+
```

### Comparing `scipion-em-3.0.9/pwem/protocols/protocol_micrographs.py` & `scipion-em-3.1.0/pwem/protocols/protocol_sets.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,10 @@
 # **************************************************************************
 # *
-# * Authors:     Josue Gomez Blanco (josue.gomez-blanco@mcgill.ca)
-# *              Roberto Marabini (roberto@cnb.csic.es)
-# *              Airen Zaldivar Peraza (azaldivar@cnb.csic.es)
-# *              Grigory Sharov (gsharov@mrc-lmb.cam.ac.uk)
-# *
+# * Authors:     J.M. De la Rosa Trevin (jmdelarosa@cnb.csic.es)
 # *
 # * Unidad de  Bioinformatica of Centro Nacional de Biotecnologia , CSIC
 # *
 # * This program is free software; you can redistribute it and/or modify
 # * it under the terms of the GNU General Public License as published by
 # * the Free Software Foundation; either version 3 of the License, or
 # * (at your option) any later version.
@@ -23,724 +19,853 @@
 # * Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA
 # * 02111-1307  USA
 # *
 # *  All comments concerning this program package may be sent to the
 # *  e-mail address 'scipion@cnb.csic.es'
 # *
 # **************************************************************************
+"""
+This module contains protocols related to Set operations such us:
+- subsets
+- unions
+- split
+... etc
+"""
 
-from os.path import exists, getmtime
-from datetime import datetime
-from collections import OrderedDict
+import random
+import sys
 
+import pyworkflow.protocol as pwprot
 import pyworkflow.object as pwobj
-import pyworkflow.protocol.constants as pwcts
-import pyworkflow.protocol.params as params
-import pyworkflow.utils as pwutils
 
 import pwem.objects as emobj
+from pwem.protocols import EMProtocol
+from pwem.objects import Volume, EMSet
+from pyworkflow.utils import ProgressBar, getListFromRangeString
+
+
+class ProtSets(EMProtocol):
+    """ Base class for all protocols related to subsets. """
+
+    def _append(self, outputSet, item, sourceItem=None):
+        """ Add an item to the outputSet.
+        If the item is a new copy of sourceItem(case of the join sets),
+        then use a sourceItem since item lost the information related with the
+        mapper
+        """
+        subElemList = []
+        if sourceItem is None:
+            sourceItem = item
+        if isinstance(item, EMSet):
+            for subElem in sourceItem.iterItems():
+                # We need to create a clone because all items have a same _objId
+                subElemList.append(subElem.clone())
+
+        outputSet.append(item)
+        if subElemList:
+            for subElem in subElemList:
+                item.append(subElem)
+
+
+class ProtUnionSet(ProtSets):
+    """ Protocol to join two or more sets of images.
+    This protocol allows to select two or more set of images
+    and will produce another set joining all elements of the 
+    selected sets. It will validate that all sets are of the
+    same type of elements (Micrographs, Particles or Volumes) 
+    """
+    _label = 'join sets'
+    TYPE_CTF = 'CTFs'
+    TYPE_VOLUME='Volumes'
+    TYPE_VOLUME_INDEX = 3
+
+    _unionTypes = ['Particles',
+                   'Micrographs',
+                   TYPE_CTF,
+                   TYPE_VOLUME,
+                   'Averages',
+                   'All']
 
-from .protocol import EMProtocol
+    def __init__(self, **kwargs):
+        ProtSets.__init__(self, **kwargs)
 
+        # We need to trace the changes of 'inputType' to
+        # dynamically modify the property of pointerClass
+        # of the 'inputSets' parameter
+        def onChangeInputType():
+            inputText = self.getEnumText('inputType')
+
+            if inputText == 'All':
+                pointerClass = 'EMSet'
+            # elif inputText == 'CTFs + Micrographs':
+            #     pointerClass = 'SetOfCTF'
+            else:
+                pointerClass = 'SetOf' + inputText
+            # For relatively small set we usually want to include
+            # the single element type, this will allow, for example
+            # to union SetOfVolumes and Volumes in the final set
+            if inputText in [self.TYPE_VOLUME]:
+                pointerClass += ',%s' % inputText[:-1]  # remove last 's'
+            elif inputText in [self.TYPE_CTF]:
+                # remove last 's'
+                pointerClass = '%s,CTFModel' % pointerClass[:-1]
 
-class ProtMicrographs(EMProtocol):
-    pass
+            self.inputSetsParam.setPointerClass(pointerClass)
 
+        self.inputType.trace(onChangeInputType)
 
-class ProtCTFMicrographs(ProtMicrographs):
-    """ Base class for all protocols that estimates the CTF"""
+    # -------------------------- DEFINE param functions ------------------------
+    def _defineParams(self, form):
+        form.addSection(label='Input')
 
-    def __init__(self, **kwargs):
-        EMProtocol.__init__(self, **kwargs)
-        self.stepsExecutionMode = pwcts.STEPS_PARALLEL
-        self.isFirstTime = pwobj.Boolean(False)
+        form.addParam('inputType', pwprot.params.EnumParam,
+                      choices=self._unionTypes, default=5,  # All
+                      label='Input type:',
+                      help='Select the type of objects that you want to union.\n'
+                           'Special case All will allow you to select any type.')
+        self.inputSetsParam = form.addParam('inputSets', pwprot.params.MultiPointerParam,
+                                            label="Input set", important=True,
+                                            pointerClass='EMSet', minNumObjects=2, maxNumObjects=0,
+                                            help='Select two or more sets (of micrographs, particles,'
+                                                 ' volumes, etc.) to be united. If you select 3 sets '
+                                                 'with 100, 200, 200 elements, the final set will '
+                                                 'contain a total of 500 elements.')
+        form.addParam('ignoreDuplicates', pwprot.params.BooleanParam,
+                      default=False,
+                      label='Remove duplicates?',
+                      help='By default, duplicated items found (same ID) '
+                           'within the input sets, will cause renumbering of all the '
+                           'items ids in the output set. '
+                           'This is the case for example when doing several '
+                           'imports (which will cause ids overlapping) '
+                           'but we really want to insert as new items in the '
+                           'output. \n'
+                           'On the other hand, items originated in a previous common '
+                           'protocol (above in the workflow) might have identical items '
+                           'and you would like to remove them. '
+                           'Therefore, set this option to *Yes* to remove duplicates and keep only '
+                           'one copy of the item (the first occurrence).')
+        form.addParam('renumber', pwprot.params.BooleanParam, default=False,
+                      expertLevel=pwprot.LEVEL_ADVANCED,
+                      label="Force new ids",
+                      help='Perform an automatic renumbering of ids to ensure all objects have unique ids. '
+                           'This will mean new objects will not be associated to the old ones.')
 
-    # -------------------------- DEFINE param functions -----------------------
-    def _defineParams(self, form):
-        form.addSection(label=pwutils.Message.LABEL_CTF_ESTI)
-        form.addParam('recalculate', params.BooleanParam, default=False,
-                      condition='recalculate',
-                      label="Do recalculate ctf?")
-
-        form.addParam('continueRun', params.PointerParam, allowsNull=True,
-                      condition='recalculate', label="Input previous run",
-                      pointerClass=self.getClassName())
-        form.addHidden('sqliteFile', params.FileParam, condition='recalculate',
-                       allowsNull=True)
-
-        form.addParam('inputMicrographs', params.PointerParam, important=True,
-                      condition='not recalculate',
-                      label=pwutils.Message.LABEL_INPUT_MIC,
-                      pointerClass='SetOfMicrographs')
-
-        form.addParam('AutoDownsampling', params.BooleanParam, default=False,
-                      label='Automatic Downsampling Factor',
-                      help='Recommended value to downsample')
-
-        form.addParam('ctfDownFactor', params.FloatParam, default=1.,
-                      label='Manual CTF Downsampling factor',
-                      condition='not AutoDownsampling',  # 'not recalculate',
-                      help='Set to 1 for no downsampling. Non-integer downsample '
-                           'factors are possible. This downsampling is only used '
-                           'for estimating the CTF and it does not affect any '
-                           'further calculation. Ideally the estimation of the '
-                           'CTF is optimal when the Thon rings are not too '
-                           'concentrated at the origin (too small to be seen) '
-                           'and not occupying the whole power spectrum (since '
-                           'this downsampling might entail aliasing).')
-
-        self._defineProcessParams(form)
-
-        line = form.addLine('Resolution', condition='not recalculate',
-                            help='Give a value in digital frequency '
-                                 '(i.e. between 0.0 and 0.5). These cut-offs '
-                                 'prevent the typical peak at the center of the'
-                                 ' PSD and high-resolution terms where only '
-                                 'noise exists, to interfere with CTF '
-                                 'estimation. The default lowest value is 0.05 '
-                                 'but for micrographs with a very fine sampling '
-                                 'this may be lowered towards 0. The default '
-                                 'highest value is 0.35, but it should be '
-                                 'increased for micrographs with signals '
-                                 'extending beyond this value. However, if '
-                                 'your micrographs extend further than 0.35, '
-                                 'you should consider sampling them at a finer '
-                                 'rate.')
-        line.addParam('lowRes', params.FloatParam, default=0.05, label='Lowest')
-        line.addParam('highRes', params.FloatParam, default=0.35, label='Highest')
-        line = form.addLine('Defocus search range (microns)',
-                            condition='not recalculate',
-                            expertLevel=pwcts.LEVEL_ADVANCED,
-                            help='Select _minimum_ and _maximum_ values for '
-                                 'defocus search range (in microns). Underfocus'
-                                 ' is represented by a positive number.')
-        line.addParam('minDefocus', params.FloatParam, default=0.25,
-                      label='Min')
-        line.addParam('maxDefocus', params.FloatParam, default=4.,
-                      label='Max')
-
-        form.addParam('windowSize', params.IntParam, default=512,
-                      expertLevel=pwcts.LEVEL_ADVANCED,
-                      label='Window size', condition='not recalculate',
-                      help='The PSD is estimated from small patches of this '
-                           'size. Bigger patches allow identifying more '
-                           'details. However, since there are fewer windows, '
-                           'estimations are noisier.')
-
-        form.addParallelSection(threads=2, mpi=1)
-
-    def _defineProcessParams(self, form):
-        """ This method should be implemented by subclasses
-        to add other parameter relatives to the specific operation."""
-        pass
+        # TODO: See what kind of restrictions we add,
+        # like "All sets should have the same sampling rate."
 
     # -------------------------- INSERT steps functions -----------------------
     def _insertAllSteps(self):
-        """ Insert the steps to perform CTF estimation, or re-estimation,
-        on a set of micrographs.
-        """
-        self._defineCtfParamsDict()
-        self.micDict = OrderedDict()
+        self._insertFunctionStep('createOutputStep')
+
+    # --------------------------- STEPS functions ------------------------------
+    def createOutputStep(self):
+
+        set1 = self.inputSets[0].get()  # 1st set (we use it many times)
 
-        if not self.recalculate:
-            self.initialIds = self._insertInitialSteps()
-            micDict, self.streamClosed = self._loadInputList()
-            ctfIds = self._insertNewMicsSteps(micDict.values())
-            self._insertFinalSteps(ctfIds)
-            # For the streaming mode, the steps function have a 'wait' flag
-            # that can be turned on/off. For example, here we insert the
-            # createOutputStep but it wait=True, which means that can not be
-            # executed until it is set to False
-            # (when the input micrographs stream is closed)
-            waitCondition = self._getFirstJoinStepName() == 'createOutputStep'
+        # Read ClassName and create the corresponding EMSet (SetOfParticles...)
+        try:
+            if str(set1.getClassName()) is not Volume.__name__:
+                outputSetFunction = getattr(self, "_create%s" % set1.getClassName())
+            else:
+                outputSetFunction = self._createSetOfVolumes
+            outputSet = outputSetFunction()
+        except Exception:
+            outputSet = set1.createCopy(self._getPath())
+
+        # Copy info from input sets (sampling rate, etc).
+        if str(set1.getClassName()) is not Volume.__name__:
+            outputSet.copyInfo(set1)  # all sets must have the same info as set1!
         else:
-            if self.isFirstTime:
-                # Insert previous estimation or re-estimation an so on...
-                self._insertPreviousSteps()
-                self.isFirstTime.set(False)
-            ctfIds = self._insertRecalculateSteps()
-            # For now the streaming is not allowed for recalculate CTF
-            waitCondition = False
-
-        self._insertFunctionStep('createOutputStep', prerequisites=ctfIds,
-                                 wait=waitCondition)
-
-    def _insertInitialSteps(self):
-        """ Override this function to insert some steps before the
-        estimate ctfs steps.
-        Should return a list of ids of the initial steps. """
-
-        pwutils.makePath(self._getExtraPath('DONE'))
-        return []
-
-    def _insertNewMicsSteps(self, inputMics):
-        """ Insert steps to process new mics (from streaming)
-        Params:
-            inputMics: input mics set to be check
-        """
-        return self._insertNewMics(inputMics,
-                                   lambda mic: mic.getMicName(),
-                                   self._insertCtfStep,
-                                   self._insertCtfListStep,
-                                   *self._getCtfArgs())
-
-    def _insertRecalculateSteps(self):
-        recalDeps = []
-        # For each psd insert the steps to process it
-        self.recalculateSet = emobj.SetOfCTF(filename=self.sqliteFile.get(),
-                                             objDoStore=False)
-        inputMics = self.getInputMicrographs()
-        for ctf in self.recalculateSet:
-            line = ctf.getObjComment()
-            if ctf.isEnabled() and line:
-                # CTF Re-estimation
-                # Make estimation steps independent between them
-                objId = ctf.getObjId()
-                stepId = self._insertFunctionStep('reEstimateCtfStep',
-                                                  objId, prerequisites=[])
-                recalDeps.append(stepId)
-                self.micDict[objId] = inputMics[objId].clone()
-        return recalDeps
-
-    def _insertFinalSteps(self, deps):
-        """ This should be implemented in subclasses"""
-        return deps
-
-    def _getFirstJoinStepName(self):
-        # This function will be used for streaming, to check which is
-        # the first function that need to wait for all micrographs
-        # to have completed, this can be overwritten in subclasses
-        # (e.g., in Xmipp 'sortPSDStep')
-        return 'createOutputStep'
-
-    def _getFirstJoinStep(self):
-        for s in self._steps:
-            if s.funcName == self._getFirstJoinStepName():
-                return s
-        return None
+            outputSet.setSamplingRate(set1.getSamplingRate())
 
-    # -------------------------- STEPS functions ------------------------------
-    def _insertCtfStep(self, mic, prerequisites, *args):
-        """ Basic method to insert an estimation step for a given micrograph. """
-        micStepId = self._insertFunctionStep('estimateCtfStep',
-                                             mic.getMicName(), *args,
-                                             prerequisites=prerequisites)
-        return micStepId
-
-    def estimateCtfStep(self, micName, *args):
-        """ Step function that will be common for all CTF protocols.
-        It will take care of re-building the micrograph object from the micDict
-        argument and perform any conversion if needed. Then, the function
-        _estimateCTF will be called, that should be implemented by each
-        CTF estimation protocol.
-        """
-        mic = self.micDict[micName]
-        micDoneFn = self._getMicrographDone(mic)
-        micFn = mic.getFileName()
-
-        if self.isContinued() and self._isMicDone(mic):
-            self.info("Skipping micrograph: %s, seems to be done" % micFn)
-            return
-
-        # Clean old finished files
-        pwutils.cleanPath(micDoneFn)
-        self.info("Estimating CTF of micrograph: %s " % mic.getObjId())
-        self._estimateCTF(mic, *args)
-
-        # Mark this mic as finished
-        open(micDoneFn, 'w').close()
-
-    def _estimateCTF(self, mic, *args):
-        """ Do the CTF estimation with the specific program
-        and the parameters required.
-        Params:
-         micFn: micrograph filename
-         micDir: micrograph directory
-        """
-        raise Exception(pwutils.Message.ERROR_NO_EST_CTF)
+        # Renumber from the beginning if either the renumber option is selected
+        # or we find duplicated ids in the sets
+        cleanIds = not self.ignoreDuplicates.get() and self.duplicatedIds()
+
+        # Warn in the log in case attributes will be lost
+        allSetAttributes, commonAttrs = self.commonAttributes()
+        warnings = self._getHeterogeneityWarning(allSetAttributes, commonAttrs)
+        if warnings:
+            self.info(warnings)
+
+        # Always ingnore non common attributtes
+        ignoreExtraAttributes = True
+
+        # Get the 1st level attributes to be used for the copyAttributes
+        copyAttrs = list()
+        for attr in commonAttrs:
+            if "." not in attr:
+                copyAttrs.append(attr)
+
+        self.info("Common attributes to all sets are: %s" % copyAttrs)
+
+        idsList = {}
+        setNum = 0
+        for itemSet in self.inputSets:
+            setNum += 1
+            if str(itemSet.get().getClassName()) is not Volume.__name__:
+                for obj in itemSet.get():
+                    objId = obj.getObjId()
+                    if self.ignoreDuplicates.get():
+                        if objId in idsList:
+                            continue
+                        idsList[objId] =objId
+                    # This is always TRUE, if stable we could remove the if and the else.
+                    if ignoreExtraAttributes:
+                        newObj = itemSet.get().ITEM_TYPE()
+                        newObj.copyAttributes(obj, *copyAttrs)
+
+                        self.cleanExtraAttributes(newObj, commonAttrs)
+                        if not cleanIds or setNum == 1:
+                            newObj.setObjId(objId)
+                    else:
+                        newObj = obj
 
-    def reEstimateCtfStep(self, micId):
-        """ CTF - re-estimation that is common for all programs.
-        The _restimateCTF function will be called with proper parameters.
-        """
-        ctf = self.recalculateSet[micId]
-        mic = self.micDict[micId]
-        micDoneFn = self._getMicrographDone(mic)
-        # Clean old finished files
-        pwutils.cleanPath(micDoneFn)
-        self.info("Estimating CTF of micrograph: %s " % mic.getObjId())
-        self._reEstimateCTF(mic, ctf)
-
-        # Mark this mic as finished
-        open(micDoneFn, 'w').close()
-
-    def _reEstimateCTF(self, mic, ctf):
-        """ Do the re-estimation of this mic (original one)
-        and the parameters that comes in the comment field of the ctf object.
-        Params:
-         micFn: micrograph filename
-         micDir: micrograph directory
-        """
-        raise Exception(pwutils.Message.ERROR_NO_EST_CTF)
+                    if (cleanIds and setNum > 1) or self.renumber.get():
+                        newObj.cleanObjId()
 
-    # Group of functions to estimate several micrographs if the batch size is
-    # defined. In some programs it might be more efficient to estimate many
-    # at once and not one by one
-
-    def _insertCtfListStep(self, micList, prerequisites, *args):
-        """ Basic method to insert an estimation step for a given micrograph. """
-        micNameList = [mic.getMicName() for mic in micList]
-        micStepId = self._insertFunctionStep('estimateCtfListStep',
-                                             micNameList, *args,
-                                             prerequisites=prerequisites)
-        return micStepId
-
-    def estimateCtfListStep(self, micNameList, *args):
-        micList = []
-
-        for micName in micNameList:
-            mic = self.micDict[micName]
-            micDoneFn = self._getMicrographDone(mic)
-            if self.isContinued() and self._isMicDone(mic):
-                self.info("Skipping micrograph: %s, seems to be done"
-                          % mic.getFileName())
-            else:
-                # Clean old finished files
-                pwutils.cleanPath(micDoneFn)
-                micList.append(mic)
-
-        self.info("Estimating CTF for micrographs: %s"
-                  % [mic.getObjId() for mic in micList])
-        self._estimateCtfList(micList, *args)
-
-        for mic in micList:
-            # Mark this mic as finished
-            open(self._getMicrographDone(mic), 'w').close()
-
-    def _estimateCtfList(self, micList, *args):
-        """ This function can be implemented by subclasses if it is a more
-        efficient way to estimate many micrographs at once.
-         Default implementation will just call the _estimateCTF. """
-        for mic in micList:
-            self._estimateCTF(mic, *args)
-
-    def _createCtfModel(self, mic, updateSampling=False):
-        """ This should be implemented in subclasses
-        in order to create a CTF model from program results.
-        """
-        pass
+                    self._append(outputSet, newObj, sourceItem=obj)
 
-    def createOutputStep(self):
-        """ This function is shared by Xmipp and CTFfind
-        estimation, or recalculate, protocols.
-        if is recalculate, it will iterated for each CTF model, see
-        if was recalculated and update with new defocus values.
-        Else, the function that should be implemented in each subclass.
-        """
-        if self.recalculate:
-            ctfSet = self._createSetOfCTF("_recalculated")
-            prot = self.continueRun.get() or self
-            if hasattr(prot, 'outputCTF'):
-                micSet = prot.outputCTF.getMicrographs()
-                # We suppose this is reading the ctf selection
-                # (with enabled/disabled) to only consider the enabled ones
-                # in the final SetOfCTF
-                # TODO: maybe we can remove the need of the extra text file
-                # with the recalculate parameters
-                newCount = 0
-                for ctfModel in self.recalculateSet:
-                    if ctfModel.isEnabled() and ctfModel.getObjComment():
-                        mic = ctfModel.getMicrograph()
-                        # Update the CTF models that where recalculated and append
-                        # later to the set, we don't want to copy the id here since
-                        # it is already correct
-                        newCtf = self._createCtfModel(mic, updateSampling=False)
-                        ctfModel.copy(newCtf, copyId=False)
-                        ctfModel.setEnabled(True)
-                        newCount += 1
-                    ctfSet.append(ctfModel)
-                ctfSet.setMicrographs(micSet)
-                self._defineOutputs(outputCTF=ctfSet)
-                self._defineCtfRelation(micSet, ctfSet)
-                self._computeDefocusRange(ctfSet)
-                self.summaryVar.set("CTF Re-estimation of %d micrographs"
-                                    % newCount)
             else:
-                raise Exception(
-                    pwutils.redStr("The outputCTF do not exist, all CTFs failed."))
-        else:
-            self._createOutputStep()
-            if self.outputCTF.getSize() == 0:
-                raise Exception(pwutils.redStr("outputCTF has size zero, all CTFs failed."
-                                               "Please review processing steps above."))
+                obj = itemSet.get()
+                objId = obj.getObjId()
+                if self.ignoreDuplicates.get():
+                    if objId in idsList:
+                        continue
+                    idsList[objId] = objId
+                newObj = obj
+                if (cleanIds and setNum > 1) or self.renumber.get():
+                    newObj.cleanObjId()
+                outputSet.append(newObj)
+
+        self._defineOutputs(outputSet=outputSet)
+        for itemSet in self.inputSets:
+            self._defineSourceRelation(itemSet, outputSet)
+
+    # Overwrite SetOfCoordinates creation
+    def _createSetOfCoordinates(self, suffix=''):
+        coordSet = self.inputSets[0].get()
+        micSet = coordSet.getMicrographs()
+        return ProtSets._createSetOfCoordinates(self, micSet, suffix)
+
+    def cleanExtraAttributes(self, obj, verifyAttrs, prefix=""):
+
+        for attr, value in obj.getAttributesToStore():
+
+            prefixedAttribute = prefix + attr
+
+            if prefixedAttribute not in verifyAttrs:
+                value._objDoStore = False
+                self.info("%s will be lost." % attr)
 
-    # -------------------------- INFO functions -------------------------------
-    def _summary(self):
-        summary = []
+            else:
+                self.cleanExtraAttributes(value, verifyAttrs,
+                                          prefixedAttribute + ".")
 
-        if self.recalculate:
-            if self.isFinished():
-                if self.summaryVar.hasValue():
-                    summary.append(self.summaryVar.get())
+    def getObjDict(self, includeClass=False, includeBasic=False):
+        return super(ProtUnionSet, self).getObjDict(
+            includeClass=includeClass, includeBasic=includeBasic)
+
+    def duplicatedIds(self):
+        """ Check if there are duplicated ids to renumber from
+        the beginning. """
+        usedIds = set()  # to keep track of the object ids we have already seen
+
+        for item_pointer in self.inputSets:
+            if str(item_pointer.get().getClassName()) is not Volume.__name__:
+                for objId in item_pointer.get().getIdSet():
+                    if objId in usedIds:
+                        return True
             else:
-                summary.append(pwutils.Message.TEXT_NO_CTF_READY)
-        else:
-            if not hasattr(self, 'outputCTF'):
-                summary.append(pwutils.Message.TEXT_NO_CTF_READY)
+                objId = item_pointer.get().getObjId()
+                if objId in usedIds:
+                    return True
+            usedIds.add(objId)
+        return False
+
+    def getAllSetsAttributes(self):
+        allSetsAttributes = list()
+        for itemSet in self.inputSets:
+            if str(itemSet.get().getClassName()) is not Volume.__name__:
+                item = itemSet.get().getFirstItem()
+            else:
+                item = itemSet.get()
+            attrs = set(item.getObjDict().keys())
+            allSetsAttributes.append(attrs)
+
+        return allSetsAttributes
+
+    def commonAttributes(self):
+        """ Compute the set of common attributes to all items within
+        each input set. """
+        commonAttrs = None
+        allSetsAttributes = self.getAllSetsAttributes()
+
+        for attrSet in allSetsAttributes:
+            if commonAttrs is None:  # first time
+                commonAttrs = attrSet
             else:
-                summary.append("CTF estimation of %d micrographs."
-                               % self.inputMicrographs.get().getSize())
+                commonAttrs = commonAttrs & attrSet
 
-        return summary
+        return allSetsAttributes, list(commonAttrs)
 
-    def _methods(self):
-        methods = []
+    # -------------------------- INFO functions -------------------------------
+    def _validate(self):
+        # Are all inputSets from the same class?
+        classes = {x.get().getClassName() for x in self.inputSets}
+        if len(classes) > 1:
+            return ["All objects should have the same type.",
+                    "Types of objects found: %s" % ", ".join(classes)]
+        if issubclass(type(self.inputSets[0].get()), emobj.SetOfClasses):
+            return ["Is not possible to join different sets of classes.\n"
+                    "If you want to join different representative, extract them "
+                    "with the viewer and them run this protocol with the "
+                    "resulting averages."]
+
+        # Validate attributes like sampling rate or dimensions
+        return self._checkSetsCompatibility()
+
+    def _checkSetsCompatibility(self):
+        """ Check if all input sets have a minimum compatible attributes """
+        # Attributes to check
+        attrs = {'sampling rates': 'getSamplingRate',
+                 'dimensions': 'getDimensions'}
+        errors = []
+        # For each attribute
+        for key, attr in attrs.items():
+
+            # Intentional: we need a default value not None, since some
+            # attributes could return None as a valid value.
+            refValue = '?'
+
+            # For pointer to a set
+            for setPointer in self.inputSets:
+
+                # Get the set:
+                inputSet = setPointer.get()
+
+                # If the set has the attribute
+                if not hasattr(inputSet, attr):
+                    break
+
+                # Get the attribute and "call it" --> final ().
+                setValue = getattr(inputSet, attr)()
+
+                if refValue == '?':
+                    refValue = setValue
+                else:
+                    if refValue != setValue:
+                        errors.append("There are different %s among the input"
+                                      " sets: %s and %s" % (key, refValue, setValue))
+                        break
+
+        return errors
+
+    def _warnings(self):
+        """ Warn about loosing info. """
+
+        # Get all attributes "map"
+        allSetsAttributes, commonAttributes = self.commonAttributes()
+
+        return self._getHeterogeneityWarning(allSetsAttributes, commonAttributes)
+
+    def _getHeterogeneityWarning(self, allSetsAttributes, commonAttributes):
+
+        warnings = []
+        # Use a set
+        commonAttributes = set(commonAttributes)
+
+        # Go through all sets attributes
+        for index, setAttributes in enumerate(allSetsAttributes):
+            setAttributes = set(setAttributes)
+            # Get the difference
+            lostAttributes = setAttributes - commonAttributes
+
+            if len(lostAttributes) != 0:
+                warnings.append("Set #%d will loose following "
+                                "attributes:" % index)
+                for attr in lostAttributes:
+                    warnings.append(attr)
+
+        if len(warnings):
+            warnings.append("Your input sets have different attributes. "
+                            "We will keep only the common ones. This may "
+                            "cause the lost of important data like CFT, "
+                            "alignment information,...")
 
-        if hasattr(self, 'outputCTF') and self.isFinished():
-            methods.append(self.methodsVar.get())
+        return  warnings
+
+    def _summary(self):
+        if not hasattr(self, 'outputSet'):
+            return ["Protocol has not finished yet."]
         else:
-            methods.append(pwutils.Message.TEXT_NO_CTF_READY)
+            return ["We have merged the following sets:",
+                    ", ".join(x.get().getNameId() for x in self.inputSets)]
 
-        return methods
+    def _methods(self):
+        return self._summary()
 
-    # -------------------------- UTILS functions ------------------------------
-    def _defineCtfParamsDict(self):
-        """ This function define a dictionary with parameters used
-        for CTF estimation that are common for all micrographs. """
-        # Get pointer to input micrographs
-        inputMics = self.getInputMicrographs()
-        acq = inputMics.getAcquisition()
-        sampling = inputMics.getSamplingRate()
-        downFactor = self.getAttributeValue('ctfDownFactor', 1.0)
-        if downFactor != 1.0:
-            sampling *= downFactor
-        self._params = {'voltage': acq.getVoltage(),
-                        'sphericalAberration': acq.getSphericalAberration(),
-                        'magnification': acq.getMagnification(),
-                        'ampContrast': acq.getAmplitudeContrast(),
-                        'samplingRate': sampling,
-                        'scannedPixelSize': inputMics.getScannedPixelSize(),
-                        'windowSize': self.windowSize.get(),
-                        'lowRes': self.lowRes.get(),
-                        'highRes': self.highRes.get(),
-                        # Convert from microns to Angstroms
-                        'minDefocus': self.minDefocus.get() * 1e+4,
-                        'maxDefocus': self.maxDefocus.get() * 1e+4
-                        }
-
-    def getCtfParamsDict(self):
-        """ Return a copy of the global params dict,
-        to avoid overwriting values. """
-        return self._params
-
-    def getRecalCtfParamsDict(self, ctfModel):
-        """ This function get the acquisition info of the micrographs"""
-        mic = ctfModel.getMicrograph()
-
-        acq = mic.getAcquisition()
-        mag = acq.getMagnification()
-        scannedPixelSize = mic.getSamplingRate() * mag / 10000
-        return {'voltage': acq.getVoltage(),
-                'sphericalAberration': acq.getSphericalAberration(),
-                'magnification': mag,
-                'ampContrast': acq.getAmplitudeContrast(),
-                'scannedPixelSize': scannedPixelSize,
-                'samplingRate': mic.getSamplingRate()
-                }
 
-    def _ctfCounter(self, values):
-        """ This function return the number of CTFs that was recalculated.
-        """
-        numberOfCTF = len(values) / 2
-        msg = "CTF Re-estimation of %d micrographs" % numberOfCTF
-        self.summaryVar.set(msg)
-
-    def _getInputCtf(self):
-        if self.continueRecal:
-            sqliteFile = self._getPath()
-        #             return self.outputCTF.get()
+class ProtSplitSet(ProtSets):
+    """ Protocol to split a set in two or more subsets.
+    """
+    _label = 'split sets'
+
+    # -------------------------- DEFINE param functions -----------------------
+    def _defineParams(self, form):
+        form.addSection(label='Input')
+
+        form.addParam('inputSet', pwprot.params.PointerParam,
+                      pointerClass='EMSet',
+                      label="Input set", important=True,
+                      help='Select the set of elements (images, etc) that you '
+                           'want to split.')
+
+        form.addParam('numberOfSets', pwprot.params.IntParam, default=2,
+                      label="Number of subsets",
+                      help='Select how many subsets do you want to create.')
+
+        form.addParam('randomize', pwprot.params.BooleanParam, default=False,
+                      label="Randomize elements",
+                      help='Put the elements at random in the different '
+                           'subsets.')
+
+    # Overwrite SetOfCoordinates creation
+    def _createSetOfCoordinates(self, suffix=''):
+        coordSet = self.inputSet.get()
+        micSet = coordSet.getMicrographs()
+        return ProtSets._createSetOfCoordinates(self, micSet, suffix)
+
+    # -------------------------- INSERT steps functions -----------------------
+    def _insertAllSteps(self):
+        self._insertFunctionStep('createOutputStep')
+
+    # -------------------------- STEPS functions ------------------------------
+    def createOutputStep(self):
+        inputSet = self.inputSet.get()
+        inputClassName = str(inputSet.getClassName())
+        n = self.numberOfSets.get()
+        # Create as many subsets as requested by the user
+        try:
+            outputSetFunction = getattr(self, "_create%s" % inputClassName)
+            subsets = [outputSetFunction(suffix=str(i)) for i in range(1, n + 1)]
+        except Exception:
+            subsets = [inputSet.createCopy(self._getPath(), suffix=str(i))
+                       for i in range(1, n + 1)]
+
+        # Iterate over the elements in the input set and assign
+        # to different subsets.
+        elements = self.inputSet.get()
+
+        ns = [len(elements) // n + (1 if i < len(elements) % n else 0)
+              for i in range(n)]  # number of elements in each subset
+        pos, i = 0, 0  # index of current subset and index of position inside it
+        orderBy = 'RANDOM()' if self.randomize else 'id'
+
+        for elem in elements.iterItems(orderBy=orderBy, direction='ASC'):
+            if i >= ns[pos]:
+                pos += 1
+                i = 0
+            self._append(subsets[pos], elem)
+            i += 1
+
+        key = 'output' + inputClassName.replace('SetOf', '') + '%02d'
+        for i in range(1, n + 1):
+            subset = subsets[i - 1]
+            subset.copyInfo(inputSet)
+            self._defineOutputs(**{key % i: subset})
+            self._defineTransformRelation(inputSet, subset)
+
+    # -------------------------- INFO functions -------------------------------
+    def _validate(self):
+        errors = []
+        if self.inputSet.get().getSize() < self.numberOfSets:
+            errors.append("The number of subsets requested is greater than")
+            errors.append("the number of elements in the input set.")
+        return errors
+
+    def _summary(self):
+        if not any(x.startswith('output') for x in dir(self)):
+            return ["Protocol has not finished yet."]
         else:
-            return self.inputCtf.get()
+            return ["We have split the set %s in %d sets." %
+                    (self.inputSet.getName(), self.numberOfSets.get())]
 
-    def _iterMicrographs(self, inputMics=None):
-        """ Iterate over micrographs and yield
-        micrograph name. """
-        if inputMics is None:
-            inputMics = self.getInputMicrographs()
-
-        for mic in inputMics:
-            micFn = mic.getFileName()
-            yield micFn, mic
-
-    def _computeDefocusRange(self, ctfSet):
-        """ Compute the minimum and maximu defocus in a set of CTFs.
-        The protocol methodsVar will be updated with new values.
 
-        Params:
-            ctfSet: the set of CTFs to compute min and max
-        """
-        defocusList = []
+class ProtSubSet(ProtSets):
+    """    
+    Create a set with the elements of an original set that are also
+    referenced in another set.
+    
+    Usually there is a bigger set with all the elements, and a smaller
+    one obtained from classification, cleaning, etc. The desired result
+    is a set with the elements from the original set that are also present
+    somehow in the smaller set (in the smaller set they may be downsampled
+    or processed in some other way).
+    
+    Both sets should be of the same kind (micrographs, particles, volumes)
+    or related (micrographs and CTFs for example).
+    """
+    _label = 'subset'
+    SET_INTERSECTION = 0
+    SET_DIFFERENCE = 1
 
-        for ctf in ctfSet:
-            defocusList.append(ctf.getDefocusU())
-            defocusList.append(ctf.getDefocusV())
+    # -------------------------- DEFINE param functions -----------------------
+    def _defineParams(self, form):
+        form.addSection(label='Input')
 
-        minD = min(defocusList) / 10000.
-        maxD = max(defocusList) / 10000.
+        add = form.addParam  # short notation
+        add('inputFullSet', pwprot.params.PointerParam, pointerClass='EMSet',
+            label="Full set of items", important=True,
+            help='Even if the operation can be applied to two arbitrary sets,\n'
+                 'the most common use-case is to retrieve a subset of\n'
+                 'elements from an original full set.\n'
+                 '*Note*: the elements of the resulting set will be the same\n'
+                 'ones as this input set.')
+        add('chooseAtRandom', pwprot.params.BooleanParam, default=False,
+            label="Make random subset",
+            help='Choose elements randomly form the full set.')
+        add('nElements', pwprot.params.IntParam, default=2,
+            condition='chooseAtRandom',
+            label="Number of elements",
+            help='How many elements will be taken from the full set.')
+        add('selectIds', pwprot.params.BooleanParam, default=False,
+            condition='not chooseAtRandom',
+            label="Make a subset from specific IDs",
+            help="Choose specific elements form the full set.")
+        add('range', pwprot.params.NumericRangeParam,
+            label="IDs range or list",
+            condition='selectIds and not chooseAtRandom',
+            allowsNull=True,
+            help='Select the IDs that will be the subset.\n'
+                 'You have several ways to specify the IDs.\n'
+                 'Example: \n'
+                 '"1,3,5-8,17-20" -> [1,3, 5, 6, 7, 8, 17, 18, 19, 20]\n')
+        add('inputSubSet', pwprot.params.PointerParam,
+            pointerClass='EMSet', condition='not (chooseAtRandom or selectIds)',
+            label="Other set",
+            allowsNull=True,
+            help='The elements present in this set will be used to pick \n'
+                 'elements from the input full set.     \n'
+                 'This means that the output set will contain elements with \n'
+                 'exact the same information of input full set.\n\n'
+                 'Set operation: if _intersection_ is used,\n'
+                 'elements that are both in input and other set\n'
+                 'will be included. If _difference_, elements that\n'
+                 'are in input but not in other will picked.')
+        add('setOperation', pwprot.params.EnumParam,
+            condition='not (chooseAtRandom or selectIds)',
+            default=self.SET_INTERSECTION,
+            choices=['intersection', 'difference'],
+            display=pwprot.params.EnumParam.DISPLAY_HLIST,
+            label='Set operation',
+            help='Set operation: if _intersection_ is used,\n'
+                 'elements that are both in input and other set\n'
+                 'will be included. If _difference_, elements that\n'
+                 'are in input but not in other will picked.')
+
+    # -------------------------- INSERT steps functions -----------------------
+    def _insertAllSteps(self):
+        self._insertFunctionStep('createOutputStep')
 
-        self.methodsVar.set("Estimated  defocus range defocus was"
-                            " %0.3f - %0.3f microns. " % (minD, maxD))
+    # -------------------------- STEPS functions ------------------------------
+    def createOutputStep(self):
+        inputFullSet = self.inputFullSet.get()
 
-        self._store(self.methodsVar)
+        inputClassName = inputFullSet.getClassName()
 
-    def _defocusMaxMin(self, defocusList):
-        """ This function return the minimum and maximum of the defocus
-        of a SetOfMicrographs.
-        """
-        raise Exception("DEPRECATED")
+        try:
+            outputSetFunction = getattr(self, "_create%s" % inputClassName)
+            outputSet = outputSetFunction()
+        except Exception:
+            outputSet = inputFullSet.createCopy(self._getPath())
+
+        outputSet.copyInfo(inputFullSet)
+
+        if self.chooseAtRandom or self.selectIds:
+            if self.chooseAtRandom:
+                # Get all ids form iput set
+                self.info("Creating subset from random positions from input set.")
+                ids = set(random.sample(inputFullSet.getIdSet(), self.nElements.get()))
+            else:
+                self.info("Creating subset by range: %s" % self.range)
+                ids = set(getListFromRangeString(self.range.get()))
+        else:
+            # Get the ids from both sets
+            fullSetIds = inputFullSet.getIdSet()
+            smallSetIds = self.inputSubSet.get().getIdSet()
+
+            # The function to include an element or not
+            # depends on the set operation
+            # if it is 'intersection' we want that item is not None (found)
+            # if it is 'difference' we want that item is None
+            # (not found, different)
+            if self.setOperation == self.SET_INTERSECTION:
+                ids = fullSetIds.intersection(smallSetIds)
+            else:
+                ids = fullSetIds.difference(smallSetIds)
 
-    def getInputMicrographsPointer(self):
-        return self.inputMicrographs
+        progress = None
+        nElements = len(ids)
 
-    def getInputMicrographs(self):
-        return self.getInputMicrographsPointer().get()
+        if nElements > 100000:  # show progressBar for large sets
+            progress = ProgressBar(total=nElements, fmt=ProgressBar.NOBAR)
+            progress.start()
+            sys.stdout.flush()
+            step = max(25000, nElements // 25000)
+
+        i = 0
+
+        for elem in inputFullSet.iterItems():
+            if elem.getObjId() in ids:
+                i += 1
+                if progress and i % step == 0:
+                    progress.update(i)
+                self._append(outputSet, elem)
+
+        if progress:
+            progress.finish(printNewLine=True)
+
+        if outputSet.getSize():
+            key = 'output' + inputClassName.replace('SetOf', '')
+            self._defineOutputs(**{key: outputSet})
+            self._defineTransformRelation(inputFullSet, outputSet)
+            if not (self.chooseAtRandom.get() or self.selectIds.get()):
+                self._defineSourceRelation(self.inputSubSet, outputSet)
+        else:
+            self.summaryVar.set('Output was not generated. Resulting set '
+                                'was EMPTY!!!')
 
-    def _getCtfArgs(self):
-        """ Should be implemented in sub-classes to define the argument
-        list that should be passed to the estimation step function.
-        """
-        return []
+    # Overwrite SetOfCoordinates creation
+    def _createSetOfCoordinates(self, suffix=''):
+        coordSet = self.inputFullSet.get()
+        micSet = coordSet.getMicrographs()
+        return ProtSets._createSetOfCoordinates(self, micSet, suffix)
 
-    # ------ Methods for Streaming CTF --------------
-    def _stepsCheck(self):
-        # To allow streaming ctf estimation we need to detect:
-        #   1) new micrographs ready to be estimated
-        #   2) new output ctfs that have been produced and add then
-        #      to the output set.
-
-        # For now the streaming is not allowed for recalculate CTF
-        if self.recalculate:
-            return
-        self._checkNewInput()
-        self._checkNewOutput()
-
-    def _checkNewInput(self):
-        # Check if there are new micrographs to process from the input set
-        localFile = self.getInputMicrographs().getFileName()
-        now = datetime.now()
-        self.lastCheck = getattr(self, 'lastCheck', now)
-        mTime = datetime.fromtimestamp(getmtime(localFile))
-        self.debug('Last check: %s, modification: %s'
-                   % (pwutils.prettyTime(self.lastCheck),
-                      pwutils.prettyTime(mTime)))
-        # If the input micrographs.sqlite have not changed since our last check,
-        # it does not make sense to check for new input data
-        if self.lastCheck > mTime and hasattr(self, 'listOfMics'):
-            return None
-
-        self.lastCheck = now
-        # Open input micrographs.sqlite and close it as soon as possible
-        micDict, self.streamClosed = self._loadInputList()
-        newMics = micDict.values()
-        outputStep = self._getFirstJoinStep()
-
-        if newMics:
-            fDeps = self._insertNewMicsSteps(newMics)
-            if outputStep is not None:
-                outputStep.addPrerequisites(*fDeps)
-            self.updateSteps()
-
-    def _checkNewOutput(self):
-        if getattr(self, 'finished', False):
-            return
-        # Load previously done items (from text file)
-        doneList = self._readDoneList()
-        # Check for newly done items
-        listOfMics = self.micDict.values()
-        nMics = len(listOfMics)
-        newDone = [m for m in listOfMics
-                   if m.getObjId() not in doneList and self._isMicDone(m)]
-
-        # Update the file with the newly done mics
-        # or exit from the function if no new done mics
-        self.debug('_checkNewOutput: ')
-        self.debug('   listOfMics: %s, doneList: %s, newDone: %s'
-                   % (nMics, len(doneList), len(newDone)))
-
-        allDone = len(doneList) + len(newDone)
-        # We have finished when there is not more input mics (stream closed)
-        # and the number of processed mics is equal to the number of inputs
-        self.finished = self.streamClosed and allDone == nMics
-        streamMode = pwobj.Set.STREAM_CLOSED if self.finished else pwobj.Set.STREAM_OPEN
-        self.debug('   streamMode: %s newDone: %s' % (streamMode,
-                                                      not (newDone == [])))
-
-        if newDone:
-            newDoneUpdated = self._updateOutputCTFSet(newDone, streamMode)
-            self._writeDoneList(newDoneUpdated)
-        elif not self.finished:
-            # If we are not finished and no new output have been produced
-            # it does not make sense to proceed and updated the outputs
-            # so we exit from the function here
-
-            # Maybe it would be good idea to take a snap to avoid
-            # so much IO if this protocol does not have much to do now
-            if allDone == nMics:
-                self._streamingSleepOnWait()
-
-            return
-
-        self.debug('   finished: %s ' % self.finished)
-        self.debug('        self.streamClosed (%s) AND' % self.streamClosed)
-        self.debug('        allDone (%s) == len(self.listOfMics (%s)'
-                   % (allDone, nMics))
-
-        if self.finished:  # Unlock createOutputStep if finished all jobs
-            self._updateStreamState(streamMode)
-            outputStep = self._getFirstJoinStep()
-            if outputStep and outputStep.isWaiting():
-                outputStep.setStatus(pwcts.STATUS_NEW)
-
-    def _loadInputList(self):
-        """ Load the input set of micrographs that are ready to be estimated. """
-        return self._loadSet(self.getInputMicrographs(), emobj.SetOfMicrographs,
-                             lambda mic: mic.getMicName())
-
-    def _loadSet(self, inputSet, SetClass, getKeyFunc):
-        """ Load a given input set if their items are not already present
-        in the self.micDict.
-        This can be used to load new micrographs for estimation as well as
-        new CTF (if used) in streaming.
-        """
-        setFn = inputSet.getFileName()
-        self.debug("Loading input db: %s" % setFn)
-        updatedSet = SetClass(filename=setFn)
-        updatedSet.loadAllProperties()
-        newItemDict = OrderedDict()
-        for item in updatedSet:
-            micKey = getKeyFunc(item)
-            if micKey not in self.micDict:
-                newItemDict[micKey] = item.clone()
-        streamClosed = updatedSet.isStreamClosed()
-        updatedSet.close()
-        self.debug("Closed db.")
-
-        return newItemDict, streamClosed
-
-    def _updateOutputCTFSet(self, micList, streamMode):
-        doneFailed = []
-        micDoneList = [mic for mic in micList]
-        # Do no proceed if there is not micrograph ready
-        if not micDoneList:
-            return []
-
-        outputName = 'outputCTF'
-        outputCtf = getattr(self, outputName, None)
-
-        # If there is not outputCTF yet, it means that is the first
-        # time we are updating output CTFs, so we need to first create
-        # the output set
-        firstTime = outputCtf is None
-
-        if firstTime:
-            outputCtf = self._createSetOfCTF()
-            outputCtf.setMicrographs(self.getInputMicrographsPointer())
+    # -------------------------- INFO functions -------------------------------
+    def _validate(self):
+        """Make sure the input data make sense."""
+
+        # Do not allow failing sets:
+        notImplentedClasses = ['SetOfClasses2D', 'SetOfClasses3D',
+                               'CoordinatesTiltPair']
+
+        errors =[]
+        if not self.chooseAtRandom and not self.selectIds and not self.inputSubSet.get():
+            errors.append("Subsetting without ids or random selection needs the 'Other set' parameter.")
+
+        if not self.inputFullSet.get():
+            # Since is mandatory it will not validate
+            # Stop validating since following validations need this set
+            return errors
+
+        c1 = self.inputFullSet.get().getClassName()
+        if c1 in notImplentedClasses:
+            errors.append("%s subset is not implemented." % c1)
+
+        # First dispatch the easy case, where we choose elements at random.
+        if self.chooseAtRandom:
+            if self.nElements > self.inputFullSet.get().getSize():
+                errors.append("Number of elements to choose cannot be bigger than",
+                        "the number of elements in the set.")
+
+
+        # Now the harder case: two sets. Check for compatible classes.
+
+        # self.inputFullSet and self.inputSubSet .get().getClassName()
+        # can be SetOf...:
+        #   Alignment
+        #   Angles
+        #   Averages
+        #   Classes
+        #   ClassesVol
+        #   Coordinates
+        #   CTF
+        #   Micrographs
+        #   MovieParticles
+        #   Movies
+        #   Particles
+        #   Volumes
+
+        if not self.inputSubSet.get():
+            # Stop validating since following validations need this set
+            return errors
+        
+        c2 = self.inputSubSet.get().getClassName()
+        if c2 in notImplentedClasses:
+            errors.append("%s subset is not implemented." % c2)
+
+        if c1 == c2:
+            return errors
+
+        # Avoid combinations that make no sense.
+        for classA, classesIncompatible in [
+            ('SetOfParticles',
+             {'SetOfMicrographs', 'SetOfMovies', 'SetOfVolumes'}),
+            ('SetOfCoordinates',
+             {'SetOfMicrographs', 'SetOfMovies', 'SetOfVolumes'}),
+            ('SetOfVolumes',
+             {'SetOfMicrographs', 'SetOfMovies', 'SetOfParticles', 'SetOfCoordinates'})]:
+            if ((c1 == classA and c2 in classesIncompatible) or
+                    (c2 == classA and c1 in classesIncompatible)):
+                errors.append("The full set and the subset are of incompatible classes",
+                        "%s and %s." % (c1, c2))
+        return errors
+
+    def _summary(self):
+        if self.summaryVar.hasValue():
+            return [self.summaryVar.get()]
+
+        key = 'output' + self.inputFullSet.get().getClassName().replace('SetOf', '')
+
+        if not hasattr(self, key):
+            return ["Protocol has not finished yet."]
         else:
-            outputCtf.enableAppend()
+            if self.setOperation == self.SET_INTERSECTION:
+                return ["The elements of %s that also are referenced in %s" %
+                        (self.inputFullSet.getName(), self.inputSubSet.getName()),
+                        "are now in %s" % getattr(self, key).getName()]
+            else:
+                return ["%s has elements only present in %s." %
+                        (getattr(self, key).getName(),
+                         self.inputFullSet.getName())
+                        ]
 
-        for micFn, mic in self._iterMicrographs(micList):
-            try:
-                ctf = self._createCtfModel(mic)
-                outputCtf.append(ctf)
-            except Exception as ex:
-                print(pwutils.yellowStr("Missing CTF?: Couldn't update CTF set with mic: %s" % micFn))
-                doneFailed.append(mic)
-
-        self.debug(" _updateOutputCTFSet Stream Mode: %s " % streamMode)
-        self._updateOutputSet(outputName, outputCtf, streamMode)
-        if doneFailed:
-            self._writeFailedList(doneFailed)
-
-        if firstTime:  # define relation just once
-            # Using a pointer to define the relations is more robust to
-            # scheduling and id changes between the protocol run.db and
-            # the main project database.get
-            self._defineCtfRelation(self.getInputMicrographsPointer(),
-                                    outputCtf)
-
-        return micDoneList
-
-    def _updateStreamState(self, streamMode):
-        outputName = 'outputCTF'
-        outputCtf = getattr(self, outputName, None)
-
-        # If there are not outputCTFs yet, it means that is the first
-        # time we are updating output CTF, so we need to first create
-        # the output set
-        firstTime = outputCtf is None
 
-        if firstTime:
-            outputCtf = self._createSetOfCTF()
+class ProtSubSetByMic(ProtSets):
+    """
+    Create a subset of those particles that come from a particular set of micrographs
+    """
+    _label = 'particles subset by micrograph'
+
+    # --------------------------- DEFINE param functions ----------------------
+    def _defineParams(self, form):
+        form.addSection(label='Input')
+
+        add = form.addParam  # short notation
+        add('inputParticles', pwprot.params.PointerParam,
+            pointerClass='SetOfParticles', label="Input particles",
+            help='Set of particles from which the subset will be taken')
+        add('inputMicrographs', pwprot.params.PointerParam,
+            pointerClass='SetOfMicrographs', label="Input micrographs",
+            help='Only the particles in this set of micrographs will be output')
+
+    # --------------------------- INSERT steps functions ----------------------
+    def _insertAllSteps(self):
+        self._insertFunctionStep('createOutputStep',
+                                 self.inputParticles.getObjId(),
+                                 self.inputMicrographs.getObjId())
+
+    # --------------------------- STEPS functions -----------------------------
+    def createOutputStep(self, partsId, micsId):
+        inputParticles = self.inputParticles.get()
+        inputMicrographs = self.inputMicrographs.get()
+
+        outputSet = self._createSetOfParticles()
+        outputSet.copyInfo(inputParticles)
+
+        micIds = []
+
+        for mic in inputMicrographs:
+            micIds.append(mic.getObjId())
+
+        for particle in inputParticles:
+            if particle.getMicId() in micIds:
+                outputSet.append(particle)
+
+        self._defineOutputs(outputParticles=outputSet)
+        self._defineTransformRelation(inputParticles, outputSet)
+
+    # --------------------------- INFO functions ------------------------------
+    def _validate(self):
+        """Make sure the input data make sense, i.e. hasMicId.
+        Thus they come from some Mic"""
+        if not self.inputParticles.get().getFirstItem().hasMicId():
+            return ['The _Input Particles_ must come from some Micrographs '
+                    'of the workflow, i.e. particles must have micId.']
+
+    def _summary(self):
+        if not hasattr(self, 'outputParticles'):
+            summary = ["Protocol has not finished yet."]
         else:
-            outputCtf.enableAppend()
+            summary = ['A subset of *%d* particles is made from a total of *%d*'
+                       ' particles.' % (self.outputParticles.getSize(),
+                                        self.inputParticles.get().getSize())]
+        return summary
+
+
+class ProtSubSetByCoord(ProtSets):
+    """
+    Create a subset of those particles that have a particular set of coordinates
+    """
+    _label = 'particles subset by coordinates'
 
-        self.debug(" _updateStreamState Stream Mode: %s " % streamMode)
-        self._updateOutputSet(outputName, outputCtf, streamMode)
+    # --------------------------- DEFINE param functions ----------------------
+    def _defineParams(self, form):
+        form.addSection(label='Input')
 
-    def _readDoneList(self):
-        """ Read from a text file the id's of the items that have been done. """
-        doneFile = self._getAllDone()
-        doneList = []
-        # Check what items have been previously done
-        if exists(doneFile):
-            with open(doneFile) as f:
-                doneList += [int(line.strip()) for line in f]
-        return doneList
-
-    def _writeDoneList(self, micList):
-        """ Write to a text file the items that have been done. """
-        doneFile = self._getAllDone()
-
-        if not exists(doneFile):
-            pwutils.makeFilePath(doneFile)
-
-        with open(doneFile, 'a') as f:
-            for mic in micList:
-                f.write('%d\n' % mic.getObjId())
-
-    def _isMicDone(self, mic):
-        """ A mic is done if the marker file exists. """
-        return exists(self._getMicrographDone(mic))
-
-    def _getAllDone(self):
-        return self._getExtraPath('DONE', 'all.TXT')
-
-    def _getAllFailed(self):
-        return self._getExtraPath('FAILED_all.TXT')
-
-    def _getMicrographDir(self, mic):
-        """ Return an unique dir name for results of the micrograph. """
-        return self._getTmpPath('mic_%04d' % mic.getObjId())
-
-    def _getMicrographDone(self, mic):
-        """ Return the file that is used as a flag of termination. """
-        return self._getExtraPath('DONE', 'mic_%06d.TXT' % mic.getObjId())
-
-    def _writeFailedList(self, micList):
-        """ Write to a text file the items that have failed. """
-        with open(self._getAllFailed(), 'a') as f:
-            for mic in micList:
-                f.write('%d\n' % mic.getObjId())
-
-    def _readFailedList(self):
-        """ Read from a text file the id's of the items that have failed. """
-        failedFile = self._getAllFailed()
-        failedList = []
-        if exists(failedFile):
-            with open(failedFile) as f:
-                failedList += [int(line.strip()) for line in f]
+        add = form.addParam  # short notation
+        add('inputParticles', pwprot.params.PointerParam,
+            pointerClass='SetOfParticles', label="Input particles",
+            help='Set of particles from which the subset will be taken')
+        add('inputCoordinates', pwprot.params.PointerParam,
+            pointerClass='SetOfCoordinates', label="Input coordinates",
+            help='Only the particles with this set of coordinates will be output')
+        add('coordTolerance', pwprot.params.FloatParam,
+            label='Coordinate tolerance (px)', default=0,
+            help='Two coordinates are supposed to be the same if their X and Y distance'
+                 ' is smaller or equal this value')
 
-        return failedList
+    # --------------------------- INSERT steps functions ----------------------
+    def _insertAllSteps(self):
+        self._insertFunctionStep('createOutputStep',
+                                 self.inputParticles.getObjId(),
+                                 self.inputCoordinates.getObjId(),
+                                 self.coordTolerance.get())
+
+    # --------------------------- STEPS functions -----------------------------
+    def createOutputStep(self, partsId, micsId, tolerance):
+        inputParticles = self.inputParticles.get()
+        inputCoordinates = self.inputCoordinates.get()
+
+        outputSet = self._createSetOfParticles()
+        outputSet.copyInfo(inputParticles)
+
+        micCoordinates = {}
+        for coord in inputCoordinates.iterCoordinates():
+            micId = coord.getMicId()
+            x, y = coord.getPosition()
+            if micId not in micCoordinates:
+                micCoordinates[micId] = []
+            micCoordinates[micId].append((x, y))
+
+        for particle in inputParticles:
+            if particle.getMicId() in micCoordinates:
+                x0, y0 = particle.getCoordinate().getPosition()
+                okToAdd = False
+                for x, y in micCoordinates[particle.getMicId()]:
+                    if abs(x - x0) <= tolerance and abs(y - y0) <= tolerance:
+                        okToAdd = True
+                        break
+                if okToAdd:
+                    outputSet.append(particle)
+
+        self._defineOutputs(outputParticles=outputSet)
+        self._defineTransformRelation(inputParticles, outputSet)
+
+    # --------------------------- INFO functions ------------------------------
+    def _validate(self):
+        """Make sure the input data make sense, i.e. hasMicId.
+        Thus they come from some Mic"""
+        if not self.inputParticles.get().getFirstItem().hasCoordinate():
+            return ['The _Input Particles_ must have coordinates']
 
+    def _summary(self):
+        if not hasattr(self, 'outputParticles'):
+            summary = ["Protocol has not finished yet."]
+        else:
+            summary = ['A subset of *%d* particles is made from a total of *%d*'
+                       ' particles.' % (self.outputParticles.getSize(),
+                                        self.inputParticles.get().getSize())]
+        return summary
 
-class ProtPreprocessMicrographs(ProtMicrographs):
-    pass
```

### Comparing `scipion-em-3.0.9/pwem/protocols/protocol_movies.py` & `scipion-em-3.1.0/pwem/protocols/protocol_movies.py`

 * *Files 2% similar despite different names*

```diff
@@ -137,14 +137,21 @@
         # If correctionImage is None, finalName will be None
         if finalName is None:
             return None
 
         elif not os.path.exists(finalName):
             # Conversion never happened...
             print('converting %s to %s' % (correctionImage, finalName))
+
+            if correctionImage.endswith('.gain'):  # treat as tif file
+                fnBase = basename(correctionImage)
+                tmpLink = self._getTmpPath(pwutils.replaceExt(fnBase, 'tif'))
+                pwutils.createAbsLink(correctionImage, tmpLink)
+                correctionImage = tmpLink
+
             emlib.image.ImageHandler().convert(correctionImage, finalName)
 
         # return final name
         return os.path.abspath(finalName)
 
     def getFinalCorrectionImagePath(self, correctionImage):
         """ Returns the final path to the correction image (converted or not)
```

### Comparing `scipion-em-3.0.9/pwem/protocols/protocol_origin_sampling_volume.py` & `scipion-em-3.1.0/pwem/protocols/protocol_origin_sampling_volume.py`

 * *Files 3% similar despite different names*

```diff
@@ -55,15 +55,18 @@
         form.addParam('inVolume', params.PointerParam, label="Input Volume", important=True,
                       pointerClass='Volume',
                       help='A new object volume will be created with the assigned sampling rate and origin. '
                            'No new binary file will be created')
         form.addParam('copyFiles', params.BooleanParam,
                       label="Copy volume",
                       help="Option Yes:\nA new volume file will be copied "
-                           "otherwise a link to the input volume is made\n",
+                           "otherwise a link to the input volume is made\n"
+                           "NOTE: if the copy option is selected the new sampling/origin"
+                           " is stored in the header. Otherwise this information "
+                           " is only stored in Scipion's database",
                       expertLevel=params.LEVEL_ADVANCED,
                       default=False)
         form.addParam('setSampling', params.BooleanParam,
                       label="Set sampling rate",
                       help="Option Yes:\nA new volume object will be created with "
                            "the given SamplingRate. "
                            "This sampling rate will NOT be set in the map file header.\n\n",
@@ -97,37 +100,44 @@
                       label="  z", default=0.,
                       help="offset along z axis (Å)")
 
     # --------------------------- INSERT steps functions ----------------------
     def _insertAllSteps(self):
         self._insertFunctionStep('assignStep')
 
-    # --------------------------- STEPS functions -----------------------------
-
+    # --------------------------- STEPS functions -----------------------------        
+        
     def assignStep(self):
         # Create a Volume object
         self.inVol = self.inVolume.get()
         self.outVol = emobj.Volume()
         self.outVol.copy(self.inVol)
 
         # Set sampling Rate (or copy from input)
+        oldSampling = self.inVol.getSamplingRate()
+        resample = True
         if self.setSampling.get():
             samplingRate = self.samplingRate.get()
         else:
-            samplingRate = self.inVol.getSamplingRate()
+            samplingRate = oldSampling
+            resample = False
 
         self.outVol.setSamplingRate(samplingRate)
 
         # set Origin
         if self.setOrigCoord.get():
             origin = emobj.Transform()
             origin.setShifts(self.x.get(), self.y.get(), self.z.get())
         else:
             origin = self.inVol.getOrigin()
-
+            if resample:
+                x, y, z = origin.getShifts()
+                factor = samplingRate / oldSampling
+                origin.setShifts(x*factor, y*factor, z*factor)
+            
         self.outVol.setOrigin(origin)
 
         # Files system stuff
         fileName = os.path.abspath(self.inVol.getFileName())
         fileName = fileName.replace(':mrc', '')
 
         # copy or link
```

### Comparing `scipion-em-3.0.9/pwem/protocols/protocol_particles.py` & `scipion-em-3.1.0/pwem/protocols/protocol_particles.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,16 +21,15 @@
 # * Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA
 # * 02111-1307  USA
 # *
 # *  All comments concerning this program package may be sent to the
 # *  e-mail address 'scipion@cnb.csic.es'
 # *
 # **************************************************************************
-
-
+import enum
 import os
 from datetime import datetime
 from collections import OrderedDict
 
 import pyworkflow.object as pwobj
 import pyworkflow.protocol as pwprot
 import pyworkflow.protocol.params as params
@@ -97,20 +96,26 @@
 
 
 # Micrograph type constants for particle extraction
 SAME_AS_PICKING = 0
 OTHER = 1
 
 
+class ProtExtractParticlesOutput(enum.Enum):
+    """Predefined outputs for particle extraction protocols"""
+    outputParticles = emobj.SetOfParticles
+
+
+# noinspection SqlDialectInspection
 class ProtExtractParticles(ProtParticles):
     """ Base class for all extract-particles protocols.
      This class will take care of the streaming functionality and
      derived classes should mainly overwrite the '_extractMicrograph' function.
      """
-
+    _possibleOutputs = ProtExtractParticlesOutput
     # --------------------------- DEFINE param functions ------------------------
     def _defineParams(self, form):
         form.addSection(label='Input')
 
         form.addParam('inputCoordinates', params.PointerParam,
                       pointerClass='SetOfCoordinates',
                       important=True,
@@ -132,15 +137,15 @@
                            'If you select _other_ option, you must provide '
                            'a different set of micrographs to extract from. \n'
                            '*Note*: In the _other_ case, ensure that provided '
                            'micrographs and coordinates are related '
                            'by micName or by micId. Difference in pixel size '
                            'will be handled automatically.')
 
-        form.addParam('inputMicrographs', params.PointerParam,
+        form.addParam('inputMicrographs', params.PointerParam, allowsNull=True,
                       pointerClass='SetOfMicrographs',
                       condition='downsampleType != %s' % SAME_AS_PICKING,
                       important=True, label='Input micrographs',
                       help='Select the SetOfMicrographs from which to extract.')
 
         form.addParam('ctfRelations', params.RelationParam, allowsNull=True,
                       condition='inputCoordinates is not None',
@@ -236,15 +241,15 @@
         self._extractMicrograph(mic, *args)
 
         # Mark this mic as finished
         open(micDoneFn, 'w').close()
 
     def _extractMicrograph(self, mic, *args):
         """ This function should be implemented by subclasses in order
-        to picking the given micrograph. """
+        to pick the given micrograph. """
         pass
 
     # ---------- Methods to extract many micrographs at once ------------------
 
     def _insertExtractMicrographListStep(self, micList, prerequisites, *args):
         """ Basic method to insert a picking step for a given micrograph. """
         return self._insertFunctionStep('extractMicrographListStep',
@@ -551,23 +556,23 @@
     def readPartsFromMics(self, micDoneList, outputParts):
         """ This method should be implemented in subclasses to read
         the particles from a given list of micrographs.
         """
         pass
 
     def _updateOutputPartSet(self, micList, streamMode):
-        outputName = 'outputParticles'
+        outputName = ProtExtractParticlesOutput.outputParticles.name
         outputParts = getattr(self, outputName, None)
         firstTime = True
 
         if outputParts is None:
             inputMics = self.getInputMicrographs()
             outputParts = self._createSetOfParticles()
             outputParts.copyInfo(inputMics)
-            outputParts.setCoordinates(self.getCoords())
+            outputParts.setCoordinates(self.inputCoordinates)
 
             if self.getAttributeValue('doFlip', False):
                 outputParts.setIsPhaseFlipped(not inputMics.isPhaseFlipped())
 
             outputParts.setSamplingRate(self._getNewSampling())
             outputParts.setHasCTF(self._useCTF())
         else:
```

### Comparing `scipion-em-3.0.9/pwem/protocols/protocol_particles_picking.py` & `scipion-em-3.1.0/pwem/protocols/protocol_particles_picking.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,31 +19,38 @@
 # * Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA
 # * 02111-1307  USA
 # *
 # *  All comments concerning this program package may be sent to the
 # *  e-mail address 'scipion@cnb.csic.es'
 # *
 # **************************************************************************
-
-
+import enum
 import os
 from datetime import datetime
 from collections import OrderedDict
 
 import pyworkflow.object as pwobj
 import pyworkflow.protocol.params as params
 import pyworkflow.protocol as pwprot
 import pyworkflow.utils as pwutils
 
 import pwem.objects as emobj
 from pwem.protocols import ProtParticles
 
 
+class ProtParticlePickingOutput(enum.Enum):
+    """ Possible outputs for particle picking protocols
+    """
+    outputCoordinates = emobj.SetOfCoordinates
+
+
 class ProtParticlePicking(ProtParticles):
-    OUTPUT_PREFIX = 'outputCoordinates'
+
+    _possibleOutputs = ProtParticlePickingOutput
+    OUTPUT_PREFIX = ProtParticlePickingOutput.outputCoordinates.name
 
     def _defineParams(self, form):
 
         form.addSection(label='Input')
         form.addParam('inputMicrographs', params.PointerParam,
                       pointerClass='SetOfMicrographs',
                       label=pwutils.Message.LABEL_INPUT_MIC, important=True,
@@ -68,15 +75,15 @@
             return ['Input micrographs not available yet.']
 
         methodsMsgs.append("Input micrographs %s of size %d."
                            % (self.getObjectTag(self.getInputMicrographs()),
                               self.getInputMicrographs().getSize()))
 
         if self.getOutputsSize() >= 1:
-            for key, output in self.iterOutputAttributes():
+            for key, output in self.iterOutputAttributes(emobj.SetOfCoordinates):
                 msg = self.getMethods(output)
                 methodsMsgs.append("%s: %s" % (self.getObjectTag(output), msg))
         else:
             methodsMsgs.append(pwutils.Message.TEXT_NO_OUTPUT_CO)
 
         return methodsMsgs
 
@@ -199,15 +206,15 @@
         Should return a list of ids of the initial steps. """
         return []
 
     def _insertFinalSteps(self, micSteps):
         """ Override this function to insert some steps after the
         picking micrograph steps.
         Receive the list of step ids of the picking steps. """
-        self._insertFunctionStep('createOutputStep',
+        self._insertFunctionStep(self.createOutputStep.__name__,
                                  prerequisites=micSteps, wait=True)
 
     def _getPickArgs(self):
         """ Should be implemented in sub-classes to define the argument
         list that should be passed to the picking step function.
         """
         return []
@@ -522,15 +529,15 @@
                 f.write('%d\n' % mic.getObjId())
 
     def _getFirstJoinStepName(self):
         # This function will be used for streaming, to check which is
         # the first function that need to wait for all micrographs
         # to have completed, this can be overwritten in subclasses
         # (eg in Xmipp 'sortPSDStep')
-        return 'createOutputStep'
+        return self.createOutputStep.__name__
 
     def _getFirstJoinStep(self):
         for s in self._steps:
             if s.funcName == self._getFirstJoinStepName():
                 return s
         return None
```

### Comparing `scipion-em-3.0.9/pwem/protocols/protocol_pdf_report.py` & `scipion-em-3.1.0/pwem/protocols/protocol_pdf_report.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.0.9/pwem/protocols/protocol_sets.py` & `scipion-em-3.1.0/pwem/tests/protocols/test_protocols_sets.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,14 @@
-# **************************************************************************
-# *
-# * Authors:     J.M. De la Rosa Trevin (jmdelarosa@cnb.csic.es)
+#!/usr/bin/env python
+
+# ***************************************************************************
+# * Authors:     Roberto Marabini (roberto@cnb.csic.es)
+# *              Jordi Burguet Castell (jburguet@cnb.csic.es)
 # *
-# * Unidad de  Bioinformatica of Centro Nacional de Biotecnologia , CSIC
+# * Unidad de Bioinformatica of Centro Nacional de Biotecnologia, CSIC
 # *
 # * This program is free software; you can redistribute it and/or modify
 # * it under the terms of the GNU General Public License as published by
 # * the Free Software Foundation; either version 3 of the License, or
 # * (at your option) any later version.
 # *
 # * This program is distributed in the hope that it will be useful,
@@ -19,787 +21,668 @@
 # * Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA
 # * 02111-1307  USA
 # *
 # *  All comments concerning this program package may be sent to the
 # *  e-mail address 'scipion@cnb.csic.es'
 # *
 # **************************************************************************
-"""
-This module contains protocols related to Set operations such us:
-- subsets
-- unions
-- split
-... etc
-"""
 
+
+import logging
+logger = logging.getLogger(__name__)
 import random
+import unittest
+
+from pwem.protocols import ProtUserSubSet
+from pyworkflow.tests import DataSet
+
+try:
+    from itertools import izip
+except ImportError:
+    izip = zip
 
-import pyworkflow.protocol as pwprot
-import pyworkflow.object as pwobj
+import pyworkflow.tests as pwtests
+import pyworkflow.utils as pwutils
 
+import pwem.protocols as emprot
 import pwem.objects as emobj
-from pwem.protocols import EMProtocol
-from pwem.objects import Volume
 
+# Used by Roberto's test, where he creates the particles "by hand"
+from pwem.objects.data import Particle, SetOfParticles, Acquisition, CTFModel
+from pyworkflow.utils.utils import prettyDict
+from pyworkflow.object import Float
+
+
+class TestSets(pwtests.BaseTest):
+    """Run different tests related to the set operations."""
+
+    @classmethod
+    def setUpClass(cls):
+        """Prepare the data that we will use later on."""
+
+        logger.info(pwutils.greenStr(" Set Up - Collect data ".center(75, '-')))
+
+        pwtests.setupTestProject(cls)  # defined in BaseTest, creates cls.proj
+
+        cls.dataset_xmipp = pwtests.DataSet.getDataSet('xmipp_tutorial')
+        cls.dataset_mda = pwtests.DataSet.getDataSet('mda')
+        cls.dataset_ribo = pwtests.DataSet.getDataSet('ribo_movies')
+        cls.datasetRelion = pwtests.DataSet.getDataSet('relion_tutorial')
+
+        #
+        # Imports
+        #
+        new = cls.proj.newProtocol  # short notation
+        launch = cls.proj.launchProtocol
+        # Micrographs
+        # NOTE: This dataset has 3 mic with heterogeneous dimensions!! But so
+        # far is not failing, should it?
+        logger.info(pwutils.magentaStr("==> Importing data - micrographs"))
+        p_imp_micros = new(emprot.ProtImportMicrographs,
+                           filesPath=cls.dataset_xmipp.getFile('allMics'),
+                           samplingRate=1.237, voltage=300)
+        launch(p_imp_micros, wait=True)
+        cls.micros = p_imp_micros.outputMicrographs
+
+        # Micrographs SMALL - This is a mic with different dimensions
+        logger.info(pwutils.magentaStr("==> Importing data - micrographs SMALL"))
+        p_imp_micros = new(emprot.ProtImportMicrographs,
+                           filesPath=cls.dataset_xmipp.getFile('mic3'),
+                           samplingRate=1.237, voltage=300)
+        launch(p_imp_micros, wait=True)
+        cls.microsSmall = p_imp_micros.outputMicrographs
+
+        # Volumes
+        logger.info(pwutils.magentaStr("==> Importing data - volumes"))
+        p_imp_volumes = new(emprot.ProtImportVolumes,
+                            filesPath=cls.dataset_xmipp.getFile('volumes'),
+                            samplingRate=9.896)
+        launch(p_imp_volumes, wait=True)
+        cls.vols = p_imp_volumes.outputVolumes
+
+        # Movies
+        logger.info(pwutils.magentaStr("==> Importing data - movies"))
+        p_imp_movies = new(emprot.ProtImportMovies,
+                           filesPath=cls.dataset_ribo.getFile('movies'),
+                           samplingRate=2.37, magnification=59000,
+                           voltage=300, sphericalAberration=2.0,
+                           gainFile=cls.dataset_ribo.getFile('volume'),
+                           darkFile=cls.dataset_ribo.getFile('volume'))
+        launch(p_imp_movies, wait=True)
+        cls.movies = p_imp_movies.outputMovies
+
+        # Particles
+        logger.info(pwutils.magentaStr("==> Importing data - particles"))
+        p_imp_particles = new(emprot.ProtImportParticles,
+                              filesPath=cls.dataset_mda.getFile('particles'),
+                              samplingRate=3.5)
+        launch(p_imp_particles, wait=True)
+        cls.particles = p_imp_particles.outputParticles
+
+        # Particles with micId
+        logger.info(pwutils.magentaStr("==> Importing data - particles with micId"))
+        relionFile = 'import/case2/relion_it015_data.star'
+        pImpPartMicId = new(emprot.ProtImportParticles,
+                            objLabel='from relion (auto-refine 3d)',
+                            importFrom=emprot.ProtImportParticles.IMPORT_FROM_RELION,
+                            starFile=cls.datasetRelion.getFile(relionFile),
+                            magnification=10000,
+                            samplingRate=7.08,
+                            haveDataBeenPhaseFlipped=True)
+        launch(pImpPartMicId, wait=True)
+        cls.partMicId = pImpPartMicId.outputParticles
+        cls.micsMicId = pImpPartMicId.outputMicrographs
+
+        # Coordinates  -  Oh, I don't know of any example of coord. import :(
+
+    #
+    # Helper functions
+    #
+    def split(self, em_set, n, randomize):
+        """Return a run split protocol over input set em_set."""
+
+        p_split = self.proj.newProtocol(emprot.ProtSplitSet, numberOfSets=n)
+        p_split.inputSet.set(em_set)
+        p_split.randomize.set(randomize)
+        self.proj.launchProtocol(p_split, wait=True)
+        return p_split
+
+    @staticmethod
+    def outputs(p):
+        """Iterator over all the elements in the outputs of protocol p."""
+        for key, output in p.iterOutputAttributes():
+            yield output
+
+    #
+    # The tests themselves.
+    #
+    def testSplit(self):
+        """Test that the split operation works as expected."""
+
+        logger.info(pwutils.greenStr(" Test Split ".center(75, '-')))
+
+        def check(set0, n=2, randomize=False):
+            # Simple checks on split sets from set0.
+            logger.info(pwutils.magentaStr("==> Check split of %s" % type(set0).__name__))
+            unsplit_set = [x.strId() for x in set0]
+            p_split = self.split(set0, n=n, randomize=randomize)
+            # Are all output elements of the protocol in the original set?
+            for em_set in self.outputs(p_split):
+                for elem in em_set:
+                    self.assertTrue(elem.strId() in unsplit_set)
+            # Number of elements of all split sets equal to original number?
+            self.assertEqual(sum(len(x) for x in self.outputs(p_split)),
+                             len(set0))
+
+        check(self.micros)
+        check(self.micros, randomize=True)
+        check(self.vols)
+        check(self.movies)
+        check(self.particles)
+        check(self.particles, n=4)
+
+    def testSubsetByParams(self):
+        """Test that the subset operation using parameters works as expected."""
+
+        logger.info(pwutils.greenStr(" Test Subset by params".center(75, '-')))
+
+        # Launch random subset
+        p_subset = self.newProtocol(emprot.ProtSubSet)
+        p_subset.setObjLabel('Random subset')
+        p_subset.inputFullSet.set(self.particles)
+        p_subset.chooseAtRandom.set(True)
+        p_subset.nElements.set(10)
+        self.launchProtocol(p_subset)
+
+        self.assertSetSize(p_subset.outputParticles, 10)
+
+        # Launch subset by ids
+        p_subset = self.newProtocol(emprot.ProtSubSet)
+        p_subset.setObjLabel('Subset by ids')
+        p_subset.inputFullSet.set(self.particles)
+        p_subset.selectIds.set(True)
+        p_subset.range.set("1-4, 8, 1000") # Last one 1000 should be skipped as is missing in the set.
+        self.launchProtocol(p_subset)
+
+        self.assertSetSize(p_subset.outputParticles, 5)
+        self.assertIsNotNone(p_subset.outputParticles[8], "Subset by id did not picked item 8.")
+
+    def testSubsetByRange(self):
+        logger.info(pwutils.greenStr(" Test Subset by Range"))
+
+        particles = [p.clone() for p in self.particles]
+
+        def _equal(part1, part2):
+            return part1.getObjDict() == part2.getObjDict()
+
+        # Launch random subset
+        ps1 = self.newProtocol(emprot.ProtSubSet)
+        ps1.inputFullSet.set(self.particles)
+        ps1.setObjLabel('Range 1')
+        ps1.selectIds.set(True)
+        ps1.range.set('1-10')
+        self.launchProtocol(ps1)
+        self.assertSetSize(ps1.outputParticles, 10)
+        self.assertTrue(_equal(particles[0], ps1.outputParticles.getFirstItem()))
+
+        ps2 = self.newProtocol(emprot.ProtSubSet)
+        ps2.inputFullSet.set(self.particles)
+        ps2.setObjLabel('Range 2')
+        ps2.selectIds.set(True)
+        ps2.range.set('11-20')
+        self.launchProtocol(ps2)
+        self.assertSetSize(ps2.outputParticles, 10)
+        self.assertTrue(_equal(particles[10], ps2.outputParticles.getFirstItem()))
+
+    def testSubsetIntersection(self):
+        """Test that the subset operation works as expected."""
+
+        logger.info(pwutils.greenStr(" Test Subset ".center(75, '-')))
+
+        def check(set0, n1=2, n2=2):
+            """Simple checks on subsets, coming from split sets of set0."""
+            logger.info(pwutils.magentaStr("==> Check subset of %s" % type(set0).__name__))
+            p_split1 = self.split(set0, n=n1, randomize=True)
+            p_split2 = self.split(set0, n=n2, randomize=True)
+
+            setFull = random.choice(list(self.outputs(p_split1)))
+            setSub = random.choice(list(self.outputs(p_split2)))
+
+            label = '%s - %s,%s ' % (set0.getClassName(), n1, n2)
+            # Launch intersection subset
+            p_subset = self.newProtocol(emprot.ProtSubSet)
+            p_subset.setObjLabel(label + 'intersection')
+            p_subset.inputFullSet.set(setFull)
+            p_subset.inputSubSet.set(setSub)
+            self.launchProtocol(p_subset)
+
+            # Launch difference subset
+            p_subset_diff = self.proj.copyProtocol(p_subset)
+            p_subset_diff.setOperation.set(p_subset_diff.SET_DIFFERENCE)
+            p_subset_diff.setObjLabel(label + 'difference')
+            self.launchProtocol(p_subset_diff)
+
+            setFullIds = setFull.getIdSet()
+            setSubIds = setSub.getIdSet()
+            n = len(setFull)
+
+            # Check intersection
+            outputs = [o for o in self.outputs(p_subset)]
+            n1 = 0
+            if outputs:
+                output = outputs[0]
+
+                # Check properties
+                self.assertTrue(set0.equalAttributes(output,
+                                                     ignore=['_mapperPath', '_size'],
+                                                     verbose=True),
+                                "Intersection subset attributes are wrong")
+
+                n1 = len(output)
+                for elem in output:
+                    self.assertTrue(elem.getObjId() in setFullIds)
+                    self.assertTrue(elem.getObjId() in setSubIds,
+                                    'object id %s not in set: %s'
+                                    % (elem.getObjId(), setSubIds))
+
+            # Check difference
+            outputs = [o for o in self.outputs(p_subset_diff)]
+            n2 = 0
+            if outputs:
+                output_diff = outputs[0]
+                # Check properties
+                self.assertTrue(set0.equalAttributes(output_diff,
+                                                     ignore=['_mapperPath', '_size'],
+                                                     verbose=True),
+                                "In subset attributes are wrong")
+
+                n2 = len(output_diff)
+                for elem in output_diff:
+                    self.assertTrue(elem.getObjId() in setFullIds)
+                    self.assertTrue(elem.getObjId() not in setSubIds)
+
+            self.assertTrue(n >= n1)
+            self.assertTrue(n >= n2)
+            self.assertEqual(n, n1 + n2)
+
+        check(self.movies)
+        check(self.particles)
+        check(self.particles, n1=3, n2=5)
+
+    def testSubsetByMic(self):
+        """Test that the subset by Mic operation works as expected."""
+        logger.info( pwutils.greenStr(" Test Subset by Mic".center(75, '-')))
+        "Simple checks on subsets, coming from split sets of setMics."
+        logger.info(pwutils.magentaStr("==> Check subset of %s by %s"
+                                 % (type(self.partMicId).__name__,
+                                    type(self.micsMicId).__name__)))
+
+        # launch the protocol for a certain mics input
+        def launchSubsetByMic(micsSubset):
+            pSubsetbyMic = self.newProtocol(emprot.ProtSubSetByMic)
+            pSubsetbyMic.inputParticles.set(self.partMicId)
+            pSubsetbyMic.inputMicrographs.set(micsSubset)
+            self.launchProtocol(pSubsetbyMic)
+            return pSubsetbyMic.outputParticles
+
+        # Check if the Output is generated, the subset size is correct and
+        #  the micId of the particle with certain partId is correct.
+        def checkAsserts(setParts, size, partId, micId):
+            self.assertIsNotNone(setParts, "Output SetOfParticles"
+                                           " were not created.")
+            self.assertEqual(setParts.getSize(), size,
+                             "The number of created particles is incorrect.")
+            p = setParts[partId]
+            self.assertEqual(p.getMicId(), micId)
+
+        # Whole set of micrographs
+        setMics = self.micsMicId
+        # Create a subsets of Mics to apply the protocol
+        pSplit = self.split(setMics, n=2, randomize=False)
+        setMics2 = pSplit.outputMicrographs02
+        # Create a subset of a single micrograph to apply the protocol
+        pSplit = self.split(setMics, n=20, randomize=False)
+        setMics3 = pSplit.outputMicrographs03
+
+        # Launch subset by mics protocol with the whole set of Mics
+        partByMic1 = launchSubsetByMic(setMics)
+        # Launch subset by mics protocol with a subset of Mics
+        partByMic2 = launchSubsetByMic(setMics2)
+        # Launch subset by mics protocol with a single SetOfMics
+        partByMic3 = launchSubsetByMic(setMics3)
+
+        # Assertions for the three sets
+        checkAsserts(partByMic1, self.partMicId.getSize(), 1885, 7)
+        checkAsserts(partByMic2, 2638, 4330, 16)
+        checkAsserts(partByMic3, 270, 725, 3)
+
+    def testSubsetByCoord(self):
+        """Test that the subset by Coord operation works as expected."""
+        logger.info(pwutils.greenStr(" Test Subset by Coord".center(75, '-')))
+
+        p_extract_coordinates = self.newProtocol(emprot.ProtExtractCoords)
+        p_extract_coordinates.inputParticles.set(self.partMicId)
+        p_extract_coordinates.inputMicrographs.set(self.micsMicId)
+        self.launchProtocol(p_extract_coordinates)
+
+        p_subset_by_coords = self.newProtocol(emprot.ProtSubSetByCoord)
+        p_subset_by_coords.inputParticles.set(self.partMicId)
+        p_subset_by_coords.inputCoordinates.set(p_extract_coordinates.outputCoordinates)
+        self.launchProtocol(p_subset_by_coords)
+        self.assertIsNotNone(p_subset_by_coords.outputParticles, "Output SetOfParticles were not created.")
+        self.assertEqual(p_subset_by_coords.outputParticles.getSize(), 5236,
+                         "The number of created particles is incorrect.")
+
+    def testMerge(self):
+        """Test that the union operation works as expected."""
+
+        logger.info(pwutils.greenStr(" Test Merge ".center(75, '-')))
+
+        def check(set0):
+            # Simple checks on merge, coming from many split sets of set0.
+            logger.info(pwutils.magentaStr("==> Check merge of %s" % type(set0).__name__))
+            p_union = self.proj.newProtocol(emprot.ProtUnionSet)
+
+            setsIds = []
+            for i in range(random.randint(1, 5)):
+                n = random.randint(1, len(set0) // 2)
+                p_split = self.split(set0, n=n, randomize=True)
+                setRandom = random.choice(list(self.outputs(p_split)))
+                setsIds.append([x.strId() for x in setRandom])
+                p_union.inputSets.append(setRandom)
+            self.proj.launchProtocol(p_union, wait=True)
+
+            output = next(self.outputs(p_union))  # first (and only!) output
+            self.assertEqual(len(output), sum(len(x) for x in setsIds))
+            # We might be able to do more interesting tests, using the
+            # collected setsIds.
+
+        check(self.micros)
+        check(self.vols)
+        check(self.movies)
+        check(self.particles)
+
+    def testMergeAlternateColumn(self):
+        """Test that the union operation works as expected.
+        Even if the order of the columns do not match.
+        That is, M1(a,b,c) U M2(a,c,b)"""
+        # Create two sets of particles
+        inFileNameMetadata1 = self.proj.getTmpPath('particles1.sqlite')
+        inFileNameMetadata2 = self.proj.getTmpPath('particles2.sqlite')
+        imgSet1 = SetOfParticles(filename=inFileNameMetadata1)
+        imgSet2 = SetOfParticles(filename=inFileNameMetadata2)
+
+        inFileNameData = self.proj.getTmpPath('particles.stk')
+        img1 = Particle()
+        img2 = Particle()
+        attrb1 = [11, 12, 13, 14]
+        attrb2 = [21, 22, 23, 24]
+        counter = 0
+
+        for i in range(1, 3):
+            img1.cleanObjId()
+            img1.setLocation(i, inFileNameData)
+            img1.setMicId(i % 3)
+            img1.setClassId(i % 5)
+            img1.setSamplingRate(1.)
+            img1._attrb1 = Float(attrb1[counter])
+            img1._attrb2 = Float(attrb2[counter])
+            imgSet1.append(img1)
+            counter += 1
+
+        for i in range(1, 3):
+            img2.cleanObjId()
+            img2.setLocation(i, inFileNameData)
+            img2.setClassId(i % 5)
+            img2.setMicId(i % 3)
+            img2.setSamplingRate(2.)
+            img2._attrb1 = Float(attrb1[counter])
+            img2._attrb2 = Float(attrb2[counter])
+            imgSet2.append(img2)
+            counter += 1
+
+        imgSet1.write()
+        imgSet2.write()
+
+        # import them
+        protImport1 = self.newProtocol(emprot.ProtImportParticles,
+                                       objLabel='import set1',
+                                       importFrom=emprot.ProtImportParticles.IMPORT_FROM_SCIPION,
+                                       sqliteFile=inFileNameMetadata1,
+                                       magnification=10000,
+                                       samplingRate=7.08,
+                                       haveDataBeenPhaseFlipped=True)
+        self.launchProtocol(protImport1)
+
+        protImport2 = self.newProtocol(emprot.ProtImportParticles,
+                                       objLabel='import set2',
+                                       importFrom=emprot.ProtImportParticles.IMPORT_FROM_SCIPION,
+                                       sqliteFile=inFileNameMetadata2,
+                                       magnification=10000,
+                                       samplingRate=7.08,
+                                       haveDataBeenPhaseFlipped=True)
+        self.launchProtocol(protImport2)
+
+        # create merge protocol
+        p_union = self.newProtocol(emprot.ProtUnionSet,
+                                   objLabel='join diff column order',
+                                   ignoreExtraAttributes=True)
+        p_union.inputSets.append(protImport1.outputParticles)
+        p_union.inputSets.append(protImport2.outputParticles)
+        self.proj.launchProtocol(p_union, wait=True)
+        # assert
+        counter = 0
+        for img in p_union.outputSet:
+            self.assertAlmostEqual(attrb1[counter], img._attrb1, 4)
+            self.assertAlmostEqual(attrb2[counter], img._attrb2, 4)
+            counter += 1
+
+    def testMergeDifferentAttrs(self):
+        """ Test merge from subsets with different attributes.
+        That is, M1(a,b,c) U M2(a,b,c,d)"""
+
+        # create two set of particles
+        inFileNameMetadata1 = self.proj.getTmpPath('particles11.sqlite')
+        inFileNameMetadata2 = self.proj.getTmpPath('particles22.sqlite')
+        imgSet1 = SetOfParticles(filename=inFileNameMetadata1)
+        imgSet2 = SetOfParticles(filename=inFileNameMetadata2)
+
+        inFileNameData = self.proj.getTmpPath('particles.stk')
+        # Start ids 4
+        img1 = Particle(objId=4)
+        img2 = Particle(objId=4)
+        attrb1 = [11, 12, 13, 14]
+        attrb2 = [21, 22, 23, 24]
+        attrb3 = [31, 32]
+        counter = 0
+        # Test the join handles different attributes at a second level
+        ctf1 = CTFModel(defocusU=1000, defocusV=1000, defocusAngle=0)
+        ctf2 = CTFModel(defocusU=2000, defocusV=2000, defocusAngle=0)
+        ctf2._myOwnQuality = Float(1.)
+        img1.setCTF(ctf1)
+        img2.setCTF(ctf2)
+
+        for i in range(1, 3):
+            # Increment Id
+            img1.setObjId(img1.getObjId() + 1)
+            img1.setLocation(i, inFileNameData)
+            img1.setMicId(i % 3)
+            img1.setClassId(i % 5)
+            img1.setSamplingRate(1.)
+            img1._attrb1 = Float(attrb1[counter])
+            img1._attrb2 = Float(attrb2[counter])
+            img1._attrb3 = Float(attrb3[counter])
+            imgSet1.append(img1)
+            counter += 1
+
+        for i in range(1, 3):
+            # Increment Id
+            img2.setObjId(img2.getObjId() + 1)
+            img2.setLocation(i, inFileNameData)
+            img2.setClassId(i % 5)
+            img2.setMicId(i % 3)
+            img2.setSamplingRate(2.)
+            img2._attrb1 = Float(attrb1[counter])
+            img2._attrb2 = Float(attrb2[counter])
+            imgSet2.append(img2)
+            counter += 1
+
+        imgSet1.write()
+        imgSet2.write()
+
+        # import them
+        protImport1 = self.newProtocol(emprot.ProtImportParticles,
+                                       objLabel='import set1',
+                                       importFrom=emprot.ProtImportParticles.IMPORT_FROM_SCIPION,
+                                       sqliteFile=inFileNameMetadata1,
+                                       magnification=10000,
+                                       samplingRate=7.08,
+                                       haveDataBeenPhaseFlipped=True
+                                       )
+        self.launchProtocol(protImport1)
+
+        protImport2 = self.newProtocol(emprot.ProtImportParticles,
+                                       objLabel='import set2',
+                                       importFrom=emprot.ProtImportParticles.IMPORT_FROM_SCIPION,
+                                       sqliteFile=inFileNameMetadata2,
+                                       magnification=10000,
+                                       samplingRate=7.08,
+                                       haveDataBeenPhaseFlipped=True
+                                       )
+        self.launchProtocol(protImport2)
+
+        # create merge protocol
+        p_union = self.newProtocol(emprot.ProtUnionSet,
+                                   objLabel='join different attrs',
+                                   ignoreExtraAttributes=True)
+        p_union.inputSets.append(protImport1.outputParticles)
+        p_union.inputSets.append(protImport2.outputParticles)
+        self.proj.launchProtocol(p_union, wait=True)
+
+        counter = 0
+
+        for img in p_union.outputSet:
+            self.assertAlmostEqual(attrb1[counter], img._attrb1, 4)
+            self.assertAlmostEqual(attrb2[counter], img._attrb2, 4)
+            self.assertFalse(hasattr(img, '_attrb3'),
+                             "join should not have attrb3")
+            self.assertTrue(hasattr(img, '_attrb2'),
+                            "join should have attrb2")
+            ctf = img.getCTF()
+            self.assertIsNotNone(ctf, "Image should have CTF after join")
+            self.assertFalse(hasattr(ctf, '_myOwnQuality'),
+                             "CTF should not have non common attributes")
+
+            # Assert ids
+            self.assertEqual(counter + 5, img.getObjId(),
+                             "Object id's not kept.")
+            counter += 1
+
+    def testOrderBy(self):
+        """ create set of particles and orderby a given attribute
+        """
+        # This function was written by Roberto. It does things
+        # differently, so let's keep it for reference.
+
+        # create set of particles
+
+        inFileNameMetadata = self.proj.getTmpPath('particlesOrderBy.sqlite')
+        inFileNameData = self.proj.getTmpPath('particlesOrderBy.stk')
+
+        imgSet = SetOfParticles(filename=inFileNameMetadata)
+        imgSet.setSamplingRate(1.5)
+        acq = Acquisition()
+        acq.setAmplitudeContrast(0.1)
+        acq.setMagnification(10000)
+        acq.setVoltage(200)
+        acq.setSphericalAberration(2.0)
+
+        imgSet.setAcquisition(acq)
+        img = Particle()
+
+        for i in range(1, 10):
+            img.setLocation(i, inFileNameData)
+            img.setMicId(i % 3)
+            img.setClassId(i % 5)
+            imgSet.append(img)
+            img.cleanObjId()
+
+        imgSet.write()
+        # now import the dataset
+        prot1 = self.newProtocol(emprot.ProtImportParticles,
+                                 importFrom=emprot.ProtImportParticles.IMPORT_FROM_SCIPION,
+                                 sqliteFile=inFileNameMetadata,
+                                 magnification=10000,
+                                 samplingRate=1.5
+                                 )
+        prot1.setObjLabel('from sqlite (test-sets)')
+        self.launchProtocol(prot1)
+
+        if prot1.outputParticles is None:
+            raise Exception(
+                'Import of images: %s, failed. outputParticles is None.'
+                % inFileNameMetadata)
+
+        protSplitSet = self.newProtocol(emprot.ProtSplitSet,
+                                        inputSet=prot1.outputParticles,
+                                        numberOfSets=2,
+                                        randomize=True)
+        self.launchProtocol(protSplitSet)
+
+        inputSets = [protSplitSet.outputParticles01,
+                     protSplitSet.outputParticles02]
+        outputSet = SetOfParticles(filename=self.proj.getTmpPath('gold.sqlite'))
+        for itemSet in inputSets:
+            for obj in itemSet:
+                outputSet.append(obj)
+
+        for item1, item2 in izip(imgSet, outputSet):
+            if not item1.equalAttributes(item2):
+                logger.info("Items differ:")
+                prettyDict(item1.getObjDict())
+                prettyDict(item2.getObjDict())
+            self.assertTrue(item1.equalAttributes(item2), )
+
+    def testEmptiness(self):
+
+        self.assertSetSize(self.particles)
+        self.assertSetSize(self.particles, 76)
+
+    def testJoinValidation(self):
+
+        # Create a merge protocol
+        p_union = self.newProtocol(emprot.ProtUnionSet,
+                                   objLabel='invalid join',
+                                   ignoreExtraAttributes=True)
+        p_union.inputSets.append(self.microsSmall)
+        p_union.inputSets.append(self.micros)
+
+        with self.assertRaises(Exception):
+            self.launchProtocol(p_union)
+
+
+class TestUserSubSet(pwtests.BaseTest):
+    @classmethod
+    def setUpClass(cls):
+        cls.dataset = DataSet.getDataSet('model')
+        cls.selectionFn = cls.dataset.getFile('classesSelection')
+        pwtests.setupTestProject(cls)
+
+    def test_2DClasses(self):
+        """ Load an existing SetOfClasses and test basic properties
+        such us: _mapperPath, iteration and others.
+        """
+        emProt = self.newProtocol(emprot.ProtImportParticles)
+        classes2DSet = emobj.SetOfClasses2D(filename=self.selectionFn)
+        emProt._defineOutputs(outputClasses=classes2DSet)
+        emProt.setFinished()
+        emProt._store()
+
+        batchProt = self.newProtocol(ProtUserSubSet,
+                                     inputObject=classes2DSet,
+                                     sqliteFile=self.selectionFn + ',',
+                                     outputClassName='SetOfClasses2D')
+        self.launchProtocol(batchProt)
 
 
-class ProtSets(EMProtocol):
-    """ Base class for all protocols related to subsets. """
-    pass
-
-
-class ProtUnionSet(ProtSets):
-    """ Protocol to join two or more sets of images.
-    This protocol allows to select two or more set of images
-    and will produce another set joining all elements of the 
-    selected sets. It will validate that all sets are of the
-    same type of elements (Micrographs, Particles or Volumes) 
-    """
-    _label = 'join sets'
-    TYPE_CTF = 'CTFs'
-    TYPE_VOLUME='Volumes'
-    TYPE_VOLUME_INDEX = 3
-
-    _unionTypes = ['Particles',
-                   'Micrographs',
-                   TYPE_CTF,
-                   TYPE_VOLUME,
-                   'Averages',
-                   'All']
-
-    def __init__(self, **kwargs):
-        ProtSets.__init__(self, **kwargs)
-
-        # We need to trace the changes of 'inputType' to
-        # dynamically modify the property of pointerClass
-        # of the 'inputSets' parameter
-        def onChangeInputType():
-            inputText = self.getEnumText('inputType')
-
-            if inputText == 'All':
-                pointerClass = 'EMSet'
-            # elif inputText == 'CTFs + Micrographs':
-            #     pointerClass = 'SetOfCTF'
-            else:
-                pointerClass = 'SetOf' + inputText
-            # For relatively small set we usually want to include
-            # the single element type, this will allow, for example
-            # to union SetOfVolumes and Volumes in the final set
-            if inputText in [self.TYPE_VOLUME]:
-                pointerClass += ',%s' % inputText[:-1]  # remove last 's'
-            elif inputText in [self.TYPE_CTF]:
-                # remove last 's'
-                pointerClass = '%s,CTFModel' % pointerClass[:-1]
-
-            self.inputSetsParam.setPointerClass(pointerClass)
-
-        self.inputType.trace(onChangeInputType)
-
-    # -------------------------- DEFINE param functions ------------------------
-    def _defineParams(self, form):
-        form.addSection(label='Input')
-
-        form.addParam('inputType', pwprot.params.EnumParam,
-                      choices=self._unionTypes, default=5,  # All
-                      label='Input type:',
-                      help='Select the type of objects that you want to union.\n'
-                           'Special case All will allow you to select any type.')
-        self.inputSetsParam = form.addParam('inputSets', pwprot.params.MultiPointerParam,
-                                            label="Input set", important=True,
-                                            pointerClass='EMSet', minNumObjects=2, maxNumObjects=0,
-                                            help='Select two or more sets (of micrographs, particles,'
-                                                 ' volumes, etc.) to be united. If you select 3 sets '
-                                                 'with 100, 200, 200 elements, the final set will '
-                                                 'contain a total of 500 elements.')
-        form.addParam('ignoreDuplicates', pwprot.params.BooleanParam,
-                      default=False,
-                      label='Remove duplicates?',
-                      help='By default, duplicated items found (same ID) '
-                           'within the input sets, will cause renumbering of all the '
-                           'items ids in the output set. '
-                           'This is the case for example when doing several '
-                           'imports (which will cause ids overlapping) '
-                           'but we really want to insert as new items in the '
-                           'output. \n'
-                           'On the other hand, items originated in a previous common '
-                           'protocol (above in the workflow) might have identical items'
-                           'and you would like to remove them. '
-                           'Therefore, set this option to *Yes* to remove duplicates and keep only '
-                           'one copy of the item. (the first occurrence)')
-        form.addParam('renumber', pwprot.params.BooleanParam, default=False,
-                      expertLevel=pwprot.LEVEL_ADVANCED,
-                      label="Force new ids",
-                      help='Make an automatic renumbering of the ids, so all '
-                           'new objects will not be associated to the old ones.')
-
-        # TODO: See what kind of restrictions we add,
-        # like "All sets should have the same sampling rate."
-
-    # -------------------------- INSERT steps functions -----------------------
-    def _insertAllSteps(self):
-        self._insertFunctionStep('createOutputStep')
-
-    # --------------------------- STEPS functions ------------------------------
-    def createOutputStep(self):
-        set1 = self.inputSets[0].get()  # 1st set (we use it many times)
-
-        # Read ClassName and create the corresponding EMSet (SetOfParticles...)
-        try:
-            if str(set1.getClassName()) is not Volume.__name__:
-                outputSetFunction = getattr(self, "_create%s" % set1.getClassName())
-            else:
-                outputSetFunction = self._createSetOfVolumes
-            outputSet = outputSetFunction()
-        except Exception:
-            outputSet = set1.create(self._getPath())
-
-        # Copy info from input sets (sampling rate, etc).
-        if str(set1.getClassName()) is not Volume.__name__:
-            outputSet.copyInfo(set1)  # all sets must have the same info as set1!
-        else:
-            outputSet.setSamplingRate(set1.getSamplingRate())
-
-        # Renumber from the beginning if either the renumber option is selected
-        # or we find duplicated ids in the sets
-        cleanIds = not self.ignoreDuplicates.get() and self.duplicatedIds()
-
-        # TODO ROB remove ignoreExtraAttributes condition
-        # or implement it. But this will be for Scipion 1.2
-        self.ignoreExtraAttributes = pwobj.Boolean(True)
-        if self.ignoreExtraAttributes:
-            _, commonAttrs = self.commonAttributes()
-
-            # Get the 1st level attributes to be used for the copyAttributes
-            copyAttrs = list()
-            for attr in commonAttrs:
-                if "." not in attr:
-                    copyAttrs.append(attr)
-
-        idsList = []
-        setNum = 0
-        for itemSet in self.inputSets:
-            setNum += 1
-            if str(itemSet.get().getClassName()) is not Volume.__name__:
-                for obj in itemSet.get():
-                    objId = obj.getObjId()
-                    if self.ignoreDuplicates.get():
-                        if objId in idsList:
-                            continue
-                        idsList.append(objId)
-
-                    if self.ignoreExtraAttributes:
-                        newObj = itemSet.get().ITEM_TYPE()
-                        newObj.copyAttributes(obj, *copyAttrs)
-
-                        self.cleanExtraAttributes(newObj, commonAttrs)
-                        if not cleanIds or setNum == 1:
-                            newObj.setObjId(objId)
-                    else:
-                        newObj = obj
-
-                    if (cleanIds and setNum > 1) or self.renumber.get():
-                        newObj.cleanObjId()
-
-                    outputSet.append(newObj)
-
-            else:
-                obj = itemSet.get()
-                objId = obj.getObjId()
-                if self.ignoreDuplicates.get():
-                    if objId in idsList:
-                        continue
-                    idsList.append(objId)
-                newObj = obj
-                if (cleanIds and setNum > 1) or self.renumber.get():
-                    newObj.cleanObjId()
-                outputSet.append(newObj)
-
-        self._defineOutputs(outputSet=outputSet)
-        for itemSet in self.inputSets:
-            self._defineSourceRelation(itemSet, outputSet)
-
-    # Overwrite SetOfCoordinates creation
-    def _createSetOfCoordinates(self, suffix=''):
-        coordSet = self.inputSets[0].get()
-        micSet = coordSet.getMicrographs()
-        return ProtSets._createSetOfCoordinates(self, micSet, suffix)
-
-    def cleanExtraAttributes(self, obj, verifyAttrs, prefix=""):
-
-        for attr, value in obj.getAttributesToStore():
-
-            prefixedAttribute = prefix + attr
-
-            if prefixedAttribute not in verifyAttrs:
-                value._objDoStore = False
-                print("INFO: %s will be lost." % attr)
-
-            else:
-                self.cleanExtraAttributes(value, verifyAttrs,
-                                          prefixedAttribute + ".")
-
-    def getObjDict(self, includeClass=False):
-        return super(ProtUnionSet, self).getObjDict(includeClass)
-
-    def duplicatedIds(self):
-        """ Check if there are duplicated ids to renumber from
-        the beginning. """
-        usedIds = set()  # to keep track of the object ids we have already seen
-
-        for item_pointer in self.inputSets:
-            if str(item_pointer.get().getClassName()) is not Volume.__name__:
-                # This could be optimised to get just the ids and avoiding Objects
-                for obj in item_pointer.get():
-                    objId = obj.getObjId()
-                    if objId in usedIds:
-                        return True
-                    usedIds.add(objId)
-            else:
-                objId = item_pointer.get().getObjId()
-                if objId in usedIds:
-                    return True
-                usedIds.add(objId)
-        return False
-
-    def getAllSetsAttributes(self):
-        allSetsAttributes = list()
-        for itemSet in self.inputSets:
-            if str(itemSet.get().getClassName()) is not Volume.__name__:
-                item = itemSet.get().getFirstItem()
-            else:
-                item = itemSet.get()
-            attrs = set(item.getObjDict().keys())
-            allSetsAttributes.append(attrs)
-
-        return allSetsAttributes
-
-    def commonAttributes(self):
-        """ Compute the set of common attributes to all items within
-        each input set. """
-        commonAttrs = None
-        allSetsAttributes = self.getAllSetsAttributes()
-
-        for attrSet in allSetsAttributes:
-            if commonAttrs is None:  # first time
-                commonAttrs = attrSet
-            else:
-                commonAttrs = commonAttrs & attrSet
-
-        return allSetsAttributes, list(commonAttrs)
-
-    # -------------------------- INFO functions -------------------------------
-    def _validate(self):
-        # Are all inputSets from the same class?
-        classes = {x.get().getClassName() for x in self.inputSets}
-        if len(classes) > 1:
-            return ["All objects should have the same type.",
-                    "Types of objects found: %s" % ", ".join(classes)]
-        if issubclass(type(self.inputSets[0].get()), emobj.SetOfClasses):
-            return ["Is not possible to join different sets of classes.\n"
-                    "If you want to join different representative, extract them "
-                    "with the viewer and them run this protocol with the "
-                    "resulting averages."]
-
-        # Validate attributes like sampling rate or dimensions
-        return self._checkSetsCompatibility()
-
-    def _checkSetsCompatibility(self):
-        """ Check if all input sets have a minimum compatible attributes """
-        # Attributes to check
-        attrs = {'sampling rates': 'getSamplingRate',
-                 'dimensions': 'getDimensions'}
-        errors = []
-        # For each attribute
-        for key, attr in attrs.items():
-
-            # Intentional: we need a default value not None, since some
-            # attributes could return None as a valid value.
-            refValue = '?'
-
-            # For pointer to a set
-            for setPointer in self.inputSets:
-
-                # Get the set:
-                inputSet = setPointer.get()
-
-                # If the set has the attribute
-                if not hasattr(inputSet, attr):
-                    break
-
-                # Get the attribute and "call it" --> final ().
-                setValue = getattr(inputSet, attr)()
-
-                if refValue == '?':
-                    refValue = setValue
-                else:
-                    if refValue != setValue:
-                        errors.append("There are different %s among the input"
-                                      " sets: %s and %s" % (key, refValue, setValue))
-                        break
-
-        return errors
-
-    def _warnings(self):
-        """ Warn about loosing info. """
-        warnings = []
-        # Get all attributes "map"
-        allSetsAttributes, commonAttributes = self.commonAttributes()
-        # Use a set
-        commonAttributes = set(commonAttributes)
-
-        # Go through all sets attributes
-        for index, setAttributes in enumerate(allSetsAttributes):
-            setAttributes = set(setAttributes)
-            # Get the difference
-            lostAttributes = setAttributes - commonAttributes
-
-            if len(lostAttributes) != 0:
-                warnings.append("Set #%d will loose following "
-                                "attributes:" % index)
-                for attr in lostAttributes:
-                    warnings.append(attr)
-
-        if len(warnings):
-            warnings.append("Your input sets have different attributes. "
-                            "We will keep only the common ones. This may "
-                            "cause the lost of important data like CFT, "
-                            "alignment information,...")
-        return warnings
-
-    def _summary(self):
-        if not hasattr(self, 'outputSet'):
-            return ["Protocol has not finished yet."]
-        else:
-            return ["We have merged the following sets:",
-                    ", ".join(x.get().getNameId() for x in self.inputSets)]
-
-    def _methods(self):
-        return self._summary()
-
-
-class ProtSplitSet(ProtSets):
-    """ Protocol to split a set in two or more subsets.
-    """
-    _label = 'split sets'
-
-    # -------------------------- DEFINE param functions -----------------------
-    def _defineParams(self, form):
-        form.addSection(label='Input')
-
-        form.addParam('inputSet', pwprot.params.PointerParam,
-                      pointerClass='EMSet',
-                      label="Input set", important=True,
-                      help='Select the set of elements (images, etc) that you '
-                           'want to split.')
-
-        form.addParam('numberOfSets', pwprot.params.IntParam, default=2,
-                      label="Number of subsets",
-                      help='Select how many subsets do you want to create.')
-
-        form.addParam('randomize', pwprot.params.BooleanParam, default=False,
-                      label="Randomize elements",
-                      help='Put the elements at random in the different '
-                           'subsets.')
-
-    # Overwrite SetOfCoordinates creation
-    def _createSetOfCoordinates(self, suffix=''):
-        coordSet = self.inputSet.get()
-        micSet = coordSet.getMicrographs()
-        return ProtSets._createSetOfCoordinates(self, micSet, suffix)
-
-    # -------------------------- INSERT steps functions -----------------------
-    def _insertAllSteps(self):
-        self._insertFunctionStep('createOutputStep')
-
-    # -------------------------- STEPS functions ------------------------------
-    def createOutputStep(self):
-        inputSet = self.inputSet.get()
-        inputClassName = str(inputSet.getClassName())
-        n = self.numberOfSets.get()
-        # Create as many subsets as requested by the user
-        try:
-            outputSetFunction = getattr(self, "_create%s" % inputClassName)
-            subsets = [outputSetFunction(suffix=str(i)) for i in range(1, n + 1)]
-        except Exception:
-            subsets = [inputSet.create(self._getPath(), suffix=str(i)) for i in
-                       range(1, n + 1)]
-
-        # Iterate over the elements in the input set and assign
-        # to different subsets.
-        elements = self.inputSet.get()
-
-        ns = [len(elements) // n + (1 if i < len(elements) % n else 0)
-              for i in range(n)]  # number of elements in each subset
-        pos, i = 0, 0  # index of current subset and index of position inside it
-        orderBy = 'RANDOM()' if self.randomize else 'id'
-
-        for elem in elements.iterItems(orderBy=orderBy, direction='ASC'):
-            if i >= ns[pos]:
-                pos += 1
-                i = 0
-            subsets[pos].append(elem)
-            i += 1
-
-        key = 'output' + inputClassName.replace('SetOf', '') + '%02d'
-        for i in range(1, n + 1):
-            subset = subsets[i - 1]
-            subset.copyInfo(inputSet)
-            self._defineOutputs(**{key % i: subset})
-            self._defineTransformRelation(inputSet, subset)
-
-    # -------------------------- INFO functions -------------------------------
-    def _validate(self):
-        errors = []
-        if self.inputSet.get().getSize() < self.numberOfSets:
-            errors.append("The number of subsets requested is greater than")
-            errors.append("the number of elements in the input set.")
-        return errors
-
-    def _summary(self):
-        if not any(x.startswith('output') for x in dir(self)):
-            return ["Protocol has not finished yet."]
-        else:
-            return ["We have split the set %s in %d sets." %
-                    (self.inputSet.getName(), self.numberOfSets.get())]
-
-
-class ProtSubSet(ProtSets):
-    """    
-    Create a set with the elements of an original set that are also
-    referenced in another set.
-    
-    Usually there is a bigger set with all the elements, and a smaller
-    one obtained from classification, cleaning, etc. The desired result
-    is a set with the elements from the original set that are also present
-    somehow in the smaller set (in the smaller set they may be downsampled
-    or processed in some other way).
-    
-    Both sets should be of the same kind (micrographs, particles, volumes)
-    or related (micrographs and CTFs for example).
-    """
-    _label = 'subset'
-    SET_INTERSECTION = 0
-    SET_DIFFERENCE = 1
-
-    # -------------------------- DEFINE param functions -----------------------
-    def _defineParams(self, form):
-        form.addSection(label='Input')
-
-        add = form.addParam  # short notation
-        add('inputFullSet', pwprot.params.PointerParam, pointerClass='EMSet',
-            label="Full set of items", important=True,
-            help='Even if the operation can be applied to two arbitrary sets,\n'
-                 'the most common use-case is to retrieve a subset of\n'
-                 'elements from an original full set.\n'
-                 '*Note*: the elements of the resulting set will be the same\n'
-                 'ones as this input set.')
-        add('chooseAtRandom', pwprot.params.BooleanParam, default=False,
-            label="Make random subset",
-            help='Choose elements randomly form the full set.')
-        add('nElements', pwprot.params.IntParam, default=2,
-            condition='chooseAtRandom',
-            label="Number of elements",
-            help='How many elements will be taken from the full set.')
-        add('inputSubSet', pwprot.params.PointerParam,
-            pointerClass='EMSet', condition='not chooseAtRandom',
-            label="Other set",
-            help='The elements present in this set will be used to pick \n'
-                 'elements from the input full set.     \n'
-                 'This means that the output set will contain elements with \n'
-                 'exact the same information of input full set.\n\n'
-                 'Set operation: if _intersection_ is used,\n'
-                 'elements that are both in input and other set\n'
-                 'will be included. If _difference_, elements that\n'
-                 'are in input but not in other will picked.')
-        add('setOperation', pwprot.params.EnumParam,
-            condition='not chooseAtRandom',
-            default=self.SET_INTERSECTION,
-            choices=['intersection', 'difference'],
-            display=pwprot.params.EnumParam.DISPLAY_HLIST,
-            label='Set operation',
-            help='Set operation: if _intersection_ is used,\n'
-                 'elements that are both in input and other set\n'
-                 'will be included. If _difference_, elements that\n'
-                 'are in input but not in other will picked.')
-
-    # -------------------------- INSERT steps functions -----------------------
-    def _insertAllSteps(self):
-        self._insertFunctionStep('createOutputStep')
-
-    # -------------------------- STEPS functions ------------------------------
-    def createOutputStep(self):
-        inputFullSet = self.inputFullSet.get()
-
-        inputClassName = inputFullSet.getClassName()
-
-        try:
-            outputSetFunction = getattr(self, "_create%s" % inputClassName)
-            outputSet = outputSetFunction()
-        except Exception:
-            outputSet = inputFullSet.create(self._getPath())
-
-        outputSet.copyInfo(inputFullSet)
-
-        if self.chooseAtRandom:
-            chosen = random.sample(range(len(inputFullSet)),
-                                   self.nElements.get())
-            for i, elem in enumerate(inputFullSet):
-                if i in chosen:
-                    outputSet.append(elem)
-        else:
-            # Iterate over the elements in the smaller set
-            # and take the info from the full set
-            inputSubSet = self.inputSubSet.get()
-            # The function to include an element or not
-            # depends on the set operation
-            # if it is 'intersection' we want that item is not None (found)
-            # if it is 'difference' we want that item is None
-            # (not found, different)
-            if self.setOperation == self.SET_INTERSECTION:
-                checkElem = lambda e: e
-            else:
-                checkElem = lambda e: not e
-
-            for origElem in inputFullSet:
-                # TODO: this can be improved if we perform
-                # intersection directly in sqlite
-                exists = origElem.getObjId() in inputSubSet
-                if checkElem(exists):
-                    outputSet.append(origElem)
-
-        if outputSet.getSize():
-            key = 'output' + inputClassName.replace('SetOf', '')
-            self._defineOutputs(**{key: outputSet})
-            self._defineTransformRelation(inputFullSet, outputSet)
-            if not self.chooseAtRandom.get():
-                self._defineSourceRelation(self.inputSubSet, outputSet)
-        else:
-            self.summaryVar.set('Output was not generated. Resulting set '
-                                'was EMPTY!!!')
-
-    # Overwrite SetOfCoordinates creation
-    def _createSetOfCoordinates(self, suffix=''):
-        coordSet = self.inputFullSet.get()
-        micSet = coordSet.getMicrographs()
-        return ProtSets._createSetOfCoordinates(self, micSet, suffix)
-
-    # -------------------------- INFO functions -------------------------------
-    def _validate(self):
-        """Make sure the input data make sense."""
-
-        # Do not allow failing sets:
-        notImplentedClasses = ['SetOfClasses2D', 'SetOfClasses3D',
-                               'CoordinatesTiltPair']
-
-        if not self.inputFullSet.get():
-            # Since is mandatory is will not validate
-            return []
-
-        c1 = self.inputFullSet.get().getClassName()
-        if c1 in notImplentedClasses:
-            return ["%s subset is not implemented." % c1]
-
-        # First dispatch the easy case, where we choose elements at random.
-        if self.chooseAtRandom:
-            if self.nElements <= self.inputFullSet.get().getSize():
-                return []
-            else:
-                return ["Number of elements to choose cannot be bigger than",
-                        "the number of elements in the set."]
-
-        if not self.inputSubSet.get():
-            return []
-
-        # Now the harder case: two sets. Check for compatible classes.
-
-        # self.inputFullSet and self.inputSubSet .get().getClassName()
-        # can be SetOf...:
-        #   Alignment
-        #   Angles
-        #   Averages
-        #   Classes
-        #   ClassesVol
-        #   Coordinates
-        #   CTF
-        #   Micrographs
-        #   MovieParticles
-        #   Movies
-        #   Particles
-        #   Volumes
-
-        c2 = self.inputSubSet.get().getClassName()
-        if c2 in notImplentedClasses:
-            return ["%s subset is not implemented." % c2]
-
-        if c1 == c2:
-            return []
-
-        # Avoid combinations that make no sense.
-        for classA, classesIncompatible in [
-            ('SetOfParticles',
-             {'SetOfMicrographs', 'SetOfMovies', 'SetOfVolumes'}),
-            ('SetOfCoordinates',
-             {'SetOfMicrographs', 'SetOfMovies', 'SetOfVolumes'}),
-            ('SetOfVolumes',
-             {'SetOfMicrographs', 'SetOfMovies', 'SetOfParticles', 'SetOfCoordinates'})]:
-            if ((c1 == classA and c2 in classesIncompatible) or
-                    (c2 == classA and c1 in classesIncompatible)):
-                return ["The full set and the subset are of incompatible classes",
-                        "%s and %s." % (c1, c2)]
-        return []  # no errors
-
-    def _summary(self):
-        if self.summaryVar.hasValue():
-            return [self.summaryVar.get()]
-
-        key = 'output' + self.inputFullSet.get().getClassName().replace('SetOf', '')
-
-        if not hasattr(self, key):
-            return ["Protocol has not finished yet."]
-        else:
-            if self.setOperation == self.SET_INTERSECTION:
-                return ["The elements of %s that also are referenced in %s" %
-                        (self.inputFullSet.getName(), self.inputSubSet.getName()),
-                        "are now in %s" % getattr(self, key).getName()]
-            else:
-                return ["%s has elements only present in %s." %
-                        (getattr(self, key).getName(),
-                         self.inputFullSet.getName())
-                        ]
-
-
-class ProtSubSetByMic(ProtSets):
-    """
-    Create a subset of those particles that come from a particular set of micrographs
-    """
-    _label = 'particles subset by micrograph'
-
-    # --------------------------- DEFINE param functions ----------------------
-    def _defineParams(self, form):
-        form.addSection(label='Input')
-
-        add = form.addParam  # short notation
-        add('inputParticles', pwprot.params.PointerParam,
-            pointerClass='SetOfParticles', label="Input particles",
-            help='Set of particles from which the subset will be taken')
-        add('inputMicrographs', pwprot.params.PointerParam,
-            pointerClass='SetOfMicrographs', label="Input micrographs",
-            help='Only the particles in this set of micrographs will be output')
-
-    # --------------------------- INSERT steps functions ----------------------
-    def _insertAllSteps(self):
-        self._insertFunctionStep('createOutputStep',
-                                 self.inputParticles.getObjId(),
-                                 self.inputMicrographs.getObjId())
-
-    # --------------------------- STEPS functions -----------------------------
-    def createOutputStep(self, partsId, micsId):
-        inputParticles = self.inputParticles.get()
-        inputMicrographs = self.inputMicrographs.get()
-
-        outputSet = self._createSetOfParticles()
-        outputSet.copyInfo(inputParticles)
-
-        micIds = []
-
-        for mic in inputMicrographs:
-            micIds.append(mic.getObjId())
-
-        for particle in inputParticles:
-            if particle.getMicId() in micIds:
-                outputSet.append(particle)
-
-        self._defineOutputs(outputParticles=outputSet)
-        self._defineTransformRelation(inputParticles, outputSet)
-
-    # --------------------------- INFO functions ------------------------------
-    def _validate(self):
-        """Make sure the input data make sense, i.e. hasMicId.
-        Thus they come from some Mic"""
-        if not self.inputParticles.get().getFirstItem().hasMicId():
-            return ['The _Input Particles_ must come from some Micrographs '
-                    'of the workflow, i.e. particles must have micId.']
-
-    def _summary(self):
-        if not hasattr(self, 'outputParticles'):
-            summary = ["Protocol has not finished yet."]
-        else:
-            summary = ['A subset of *%d* particles is made from a total of *%d*'
-                       ' particles.' % (self.outputParticles.getSize(),
-                                        self.inputParticles.get().getSize())]
-        return summary
-
-
-class ProtSubSetByCoord(ProtSets):
-    """
-    Create a subset of those particles that have a particular set of coordinates
-    """
-    _label = 'particles subset by coordinates'
-
-    # --------------------------- DEFINE param functions ----------------------
-    def _defineParams(self, form):
-        form.addSection(label='Input')
-
-        add = form.addParam  # short notation
-        add('inputParticles', pwprot.params.PointerParam,
-            pointerClass='SetOfParticles', label="Input particles",
-            help='Set of particles from which the subset will be taken')
-        add('inputCoordinates', pwprot.params.PointerParam,
-            pointerClass='SetOfCoordinates', label="Input coordinates",
-            help='Only the particles with this set of coordinates will be output')
-        add('coordTolerance', pwprot.params.FloatParam,
-            label='Coordinate tolerance (px)', default=0,
-            help='Two coordinates are supposed to be the same if their X and Y distance'
-                 ' is smaller or equal this value')
-
-    # --------------------------- INSERT steps functions ----------------------
-    def _insertAllSteps(self):
-        self._insertFunctionStep('createOutputStep',
-                                 self.inputParticles.getObjId(),
-                                 self.inputCoordinates.getObjId(),
-                                 self.coordTolerance.get())
-
-    # --------------------------- STEPS functions -----------------------------
-    def createOutputStep(self, partsId, micsId, tolerance):
-        inputParticles = self.inputParticles.get()
-        inputCoordinates = self.inputCoordinates.get()
-
-        outputSet = self._createSetOfParticles()
-        outputSet.copyInfo(inputParticles)
-
-        micCoordinates = {}
-        for coord in inputCoordinates.iterCoordinates():
-            micId = coord.getMicId()
-            x, y = coord.getPosition()
-            if micId not in micCoordinates:
-                micCoordinates[micId] = []
-            micCoordinates[micId].append((x, y))
-
-        for particle in inputParticles:
-            if particle.getMicId() in micCoordinates:
-                x0, y0 = particle.getCoordinate().getPosition()
-                okToAdd = False
-                for x, y in micCoordinates[particle.getMicId()]:
-                    if abs(x - x0) <= tolerance and abs(y - y0) <= tolerance:
-                        okToAdd = True
-                        break
-                if okToAdd:
-                    outputSet.append(particle)
-
-        self._defineOutputs(outputParticles=outputSet)
-        self._defineTransformRelation(inputParticles, outputSet)
-
-    # --------------------------- INFO functions ------------------------------
-    def _validate(self):
-        """Make sure the input data make sense, i.e. hasMicId.
-        Thus they come from some Mic"""
-        if not self.inputParticles.get().getFirstItem().hasCoordinate():
-            return ['The _Input Particles_ must have coordinates']
-
-    def _summary(self):
-        if not hasattr(self, 'outputParticles'):
-            summary = ["Protocol has not finished yet."]
-        else:
-            summary = ['A subset of *%d* particles is made from a total of *%d*'
-                       ' particles.' % (self.outputParticles.getSize(),
-                                        self.inputParticles.get().getSize())]
-        return summary
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `scipion-em-3.0.9/pwem/protocols/protocol_tests.py` & `scipion-em-3.1.0/pwem/protocols/protocol_tests.py`

 * *Files 2% similar despite different names*

```diff
@@ -119,19 +119,19 @@
             if self.extraParams is not None:
                 args += " %s " % self.extraParams
             self.runJob(self._program, args)
 
     # ------------------------ INFO functions ----------------------------------
     def _validate(self):
         message = []
-        from distutils.spawn import find_executable
+        from shutil import which
         if self.noCpu == 0 and self.noIO == 0 and self.noMem == 0:
             pass
         else:
-            if find_executable(self._program) is None:
+            if which(self._program) is None:
                 message = ["Cannot find executable %s" % self._program]
         return message
 
     def _summary(self):
         message = "%d CPU, %d Mem, %d IO stressor" % (self.cpu, self.mem,
                                                       self.io)
         return [message]
```

### Comparing `scipion-em-3.0.9/pwem/protocols/protocol_tiltpairs.py` & `scipion-em-3.1.0/pwem/protocols/protocol_tiltpairs.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.0.9/pwem/templates/demo.json.template` & `scipion-em-3.1.0/pwem/templates/demo.json.template`

 * *Files identical despite different names*

### Comparing `scipion-em-3.0.9/pwem/tests/__init__.py` & `scipion-em-3.1.0/pwem/wizards/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,11 @@
-#!/usr/bin/env python
 # **************************************************************************
 # *
-# * Authors:     J.M. De la Rosa Trevin (jmdelarosa@cnb.csic.es)
-#                Laura del Cano         (ldelcano@cnb.csic.es)
+# * Authors: Yunior C. Fonseca Reyna    (cfonseca@cnb.csic.es)
+# *
 # *
 # * Unidad de  Bioinformatica of Centro Nacional de Biotecnologia , CSIC
 # *
 # * This program is free software; you can redistribute it and/or modify
 # * it under the terms of the GNU General Public License as published by
 # * the Free Software Foundation; either version 3 of the License, or
 # * (at your option) any later version.
@@ -22,8 +21,10 @@
 # * 02111-1307  USA
 # *
 # *  All comments concerning this program package may be sent to the
 # *  e-mail address 'scipion@cnb.csic.es'
 # *
 # **************************************************************************
 
-
+from .wizard import *
+from .wizards import *
+from .wizards_3d import *
```

### Comparing `scipion-em-3.0.9/pwem/tests/data/test_convert_atom_struct.py` & `scipion-em-3.1.0/pwem/tests/data/test_convert_atom_struct.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,23 +26,25 @@
 #
 from copy import deepcopy
 from tempfile import NamedTemporaryFile
 from collections import Counter
 from urllib.request import urlretrieve
 
 import numpy as np
+import os
 
 from pyworkflow.tests import *
 
 import pwem.convert as emconv
 from pwem.emlib.image import ImageHandler
+from pwem.protocols import ProtImportPdb
 
 
 class TestAtomicStructHandler(unittest.TestCase):
-
+    """test atomicstructure handler"""
     def testIntToChain(self):
         aSH = emconv.AtomicStructHandler(self.PDBFileName)
         solString = ['A',  'B',  'C',  'D',  'E',  'F',  'G',
                      'H',  'I',  'J',  'K',  'L',  'M',  'N',
                      'O',  'P',  'Q',  'R',  'S',  'T',  'U',
                      'V',  'W',  'X',  'Y',  'Z',  '0',  '1',
                      '2',  '3',  '4',  '5',  '6',  '7',  '8',
@@ -958,7 +960,73 @@
 HETATM 4 O O  . PRO B 1 . 1 ? 9.466 21.457 19.005 1.00 17.44 ? ? ? ? ? ? ? 1 PRO B O  1 PRO B O  1
 HETATM 5 C CB . PRO B 1 . 1 ? 6.460 21.723 20.211 1.00 22.26 ? ? ? ? ? ? ? 1 PRO B CB 1 PRO B CB 1
 #"""
         f = NamedTemporaryFile(delete=False, suffix=".cif")
         f.write(CIFString.encode('utf8'))
         f.close()
         cls.CIFFileName = f.name
+
+    def testGetTransformMatrix(self):
+        # create and load atom struct
+        from .hexonAtomStruct import saveFiles
+        h1Fn, h2Fn = saveFiles()
+        aSH = emconv.AtomicStructHandler(h1Fn)
+        # should get identity matrix
+        matrix, error = aSH.getTransformMatrix(h1Fn, 100, 300)
+        self.assertTrue(matrix.shape[0] == matrix.shape[1] and\
+               np.allclose(matrix, np.eye(matrix.shape[0])))
+        data = np.array([[1, 2], [3, 4]])
+
+        goldMatrix = np.array(
+            [[ 9.93196087e-01,  2.55599161e-02, -1.13614363e-01, 1.75187864e+00],
+             [-2.25492853e-02,  9.99361764e-01,  2.77054840e-02, 4.47446401e+01],
+             [ 1.14250000e-01, -2.49550556e-02,  9.93138552e-01, 3.95671369e+01],
+             [ 0.00000000e+00,  0.00000000e+00,  0.00000000e+00, 1.00000000e+00]])
+        goldError = 0.8032027904183334
+
+        matrix, error = aSH.getTransformMatrix(h2Fn, -1, -1)
+        self.assertTrue( matrix.shape[0] == matrix.shape[1] and\
+                        np.allclose(matrix, goldMatrix))
+        self.assertAlmostEqual(error, goldError)
+        # DEBUG, next three lines save the transformed
+        # atom struct to file
+        # aSH2 = emconv.AtomicStructHandler(h2Fn)
+        # aSH2.transform(matrix)
+        # aSH2.write("/tmp/kk.cif")
+
+    def testGetBoundingBox(self):
+        # create and load atom struct
+        from .hexonAtomStruct import saveFiles
+        h1Fn, h2Fn = saveFiles()
+        aSH = emconv.AtomicStructHandler(h1Fn)
+        [[x1, y1, z1],[x2, y2, z2]] = aSH.getBoundingBox()
+        self.assertAlmostEqual(x1, 205.438 - 3, places=2)
+        self.assertAlmostEqual(y1, -92.590 - 3, places=2)
+        self.assertAlmostEqual(z1, 240.313 - 3, places=2)
+        self.assertAlmostEqual(x2, 328.960 + 3, places=2)
+        self.assertAlmostEqual(y2,   2.663 + 3, places=2)
+        self.assertAlmostEqual(z2, 352.586 + 3, places=2)
+
+    def testFunctionAddAttribute(self):
+        from .hexonAtomStruct import saveFiles
+        import pwem.convert.atom_struct as convAS
+        h1Fn, h2Fn = saveFiles()
+        outFileName = '/tmp/scipionAttributes.cif'
+        attrName = 'hidrophobicity'
+
+        attrDic = {':asp':	3.49, ':glu': 2.68, ':asn':	2.05, ':gln': 2.36, ':lys':	2.71,
+                	 ':arg':	2.58, ':his':	2.06, ':gly':	0.74, ':pro':	2.23, ':ser':	0.84,
+                   ':thr':	0.52, ':cys':	-0.13, ':met':	-0.10, ':mse':	-0.10, ':ala':	0.11,
+                   ':val':	-0.31, ':ile':	-0.60, ':leu':	-0.55, ':phe':	-0.32, ':trp':	0.30,
+                	 ':tyr':	0.68}
+
+        aSH = emconv.AtomicStructHandler()
+        cifDic = aSH.readLowLevel(h1Fn)
+        cifDic = convAS.addScipionAttribute(cifDic, attrDic, attrName, 'residues')
+        aSH._writeLowLevel(outFileName, cifDic)
+
+        cifDicOut = aSH.readLowLevel(outFileName)
+        self.assertEqual(cifDicOut[convAS.NAME][0], attrName)
+        self.assertEqual(cifDicOut[convAS.RECIP][0], 'residues')
+        self.assertEqual(cifDicOut[convAS.SPEC][0], ':asp')
+        self.assertEqual(cifDicOut[convAS.VALUE][0], '3.49')
+
```

### Comparing `scipion-em-3.0.9/pwem/tests/data/test_data.py` & `scipion-em-3.1.0/pwem/tests/data/test_data.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,14 +13,17 @@
 from pyworkflow import SCIPION_DEBUG_NOCLEAN
 from pyworkflow.tests import *
 import pyworkflow.utils as pwutils
 
 import pwem.objects as emobj
 from pwem import emlib
 from pwem.emlib import metadata as md
+import pwem.protocols as emprot
+import pyworkflow.tests as pwtests
+from pwem.convert import SequenceHandler
 
 # set to true if you want to check how fast is the access to
 # the database
 SPEEDTEST = True
 
 
 def getIndex(fileName):
@@ -51,28 +54,27 @@
     from pwem.protocols import EMProtocol
 
     prot = proj.newProtocol(EMProtocol)
     prot.setObjLabel('dummy protocol')
     try:
         proj.launchProtocol(prot)
     except Exception as e:
-        print(str(e))
+        logger.error("Can't launch EMProtocol", exc_info=e)
     return prot
 
 
 class TestFSC(unittest.TestCase):
     _labels = [SMALL, WEEKLY]
 
     def testIO(self):
         """Test basic FSC object"""
         xList = [0.00, 0.05, 0.10, 0.15, 0.2]
         yList = [1.00, 0.95, 0.90, 0.85, 0.2]
         fsc = emobj.FSC()
         fsc.setData(xList, yList)
-        # fsc.printAll()
         x, y = fsc.getData()
         self.assertEqual(xList, x)
         self.assertEqual(yList, y)
 
     def testMd(self):
         """test create FSC from metadata"""
         xList = [0.00, 0.05, 0.10, 0.15, 0.2]
@@ -229,24 +231,32 @@
         # Labelled as movie
         X, Y, Z, N = ih.getDimensions(sVolFn + movieLabel)
         self.assertEqual([X, Y, Z, N], expectedSize_Mov)
         # Labelled as volume
         X, Y, Z, N = ih.getDimensions(sVolFn + volLabel)
         self.assertEqual([X, Y, Z, N], expectedSize_Svol)
 
+        # eer format (In case we want to cancel the warning)
+        import logging
+        tifffileLogger = logging.getLogger("tifffile.tifffile")
+        tifffileLogger.disabled = True
+
+        X, Y, Z, N = ih.getDimensions(self.dsFormat.getFile("eer"))
+        self.assertEqual([X, Y, Z, N], [4096, 4096, 567, 1])
+
     def test_convertMicrographs(self):
         """ Convert micrographs to different formats.
          EMAN2 required for .img
         """
         micFn = self.dataset.getFile('micrographs/BPV_1386.mrc')
         outSuffix = pwutils.replaceBaseExt(micFn, 'img')
         ih = emlib.image.ImageHandler()
 
         outFn = join('/tmp', outSuffix)
-        print("Converting: \n%s -> %s" % (micFn, outFn))
+        logger.info("Converting: \n%s -> %s" % (micFn, outFn))
 
         ih.convert(micFn, outFn)
 
         self.assertTrue(os.path.exists(outFn))
         self.assertTrue(pwutils.getFileSize(outFn) > 0)
 
         pwutils.cleanPath(outFn)
@@ -262,15 +272,15 @@
         EXPECTED_SIZE = (7676, 7420, 1, 1)
         self.assertEqual(ih.getDimensions(micFn), EXPECTED_SIZE)
 
         # We could even convert to an mrc file:
         outSuffix = pwutils.replaceBaseExt(micFn, 'mrc')
 
         outFn = join('/tmp', outSuffix)
-        print("Converting: \n%s -> %s" % (micFn, outFn))
+        logger.info("Converting: \n%s -> %s" % (micFn, outFn))
 
         ih.convert(micFn, outFn)
 
         self.assertTrue(os.path.exists(outFn))
         self.assertTrue(pwutils.getFileSize(outFn) > 0)
         # Check dimensions are still the same:
         self.assertEqual(ih.getDimensions(outFn), EXPECTED_SIZE)
@@ -288,15 +298,15 @@
         EXPECTED_SIZE = (7676, 7420, 1, 38)
         self.assertEqual(ih.getDimensions(micFn), EXPECTED_SIZE)
 
         # We could even convert to an mrc file:
         outSuffix = pwutils.replaceBaseExt(micFn, 'mrc')
 
         outFn = join('/tmp', outSuffix)
-        print("Converting: \n%s -> %s" % ((1, micFn), outFn))
+        logger.info("Converting: \n%s -> %s" % ((1, micFn), outFn))
 
         ih.convert((1, micFn), outFn)
 
         self.assertTrue(os.path.exists(outFn))
         self.assertTrue(pwutils.getFileSize(outFn) > 0)
         self.assertEqual(ih.getDimensions(outFn), (7676, 7420, 1, 1))
 
@@ -321,15 +331,15 @@
 
         self.assertTrue(os.path.exists(outFn))
         self.assertTrue(pwutils.getFileSize(outFn) > 0)
         self.assertEqual(ih.getDimensions(outFn), (4096, 4096, 1, 5))
         self.assertEqual(ih.getDataType(outFn), EXPECTED_DT)
 
         if pwutils.envVarOn(SCIPION_DEBUG_NOCLEAN):
-            print("Not cleaning output movie: ", outFn)
+            logger.info("Not cleaning output movie: ", outFn)
         else:
             pwutils.cleanPath(outFn)
 
     def test_truncateMask(self):
         ih = emlib.image.ImageHandler()
 
         maskFn = self.dataset.getFile('masks/mask.vol')
@@ -413,15 +423,14 @@
             raise Exception('There are not micrographs matching pattern')
         cls.mics.sort()
 
     def checkSet(self, micSet):
         idCount = 1
 
         for mic1, fn in zip(micSet, self.mics):
-            # traceback.print_stack(file=sys.stdout)
             micFn = mic1.getFileName()
             self.assertEqual(fn, micFn,
                              "micrograph NAME in the set is wrong, \n   expected: '%s'\n        got: '%s'"
                              % (fn, micFn))
             self.assertEqual(idCount, mic1.getObjId(),
                              "micrograph ID in the set is wrong, \n   expected: '%s'\n        got: '%s'"
                              % (idCount, mic1.getObjId()))
@@ -453,15 +462,15 @@
 
         os.chdir(cwd)
 
     def testRead(self):
         """ Read micrographs from a an sqlite file.
         It should contains Acquisition info. """
         micFn = self.dataset.getFile('micsGoldSqlite2')
-        print(">>> Reading gold micrographs from: ", micFn)
+        logger.info(">>> Reading gold micrographs from %s " % micFn)
 
         micSet = emobj.SetOfMicrographs(filename=micFn)
         self.assertEqual(2, micSet.getSize())
         acquisition = emobj.Acquisition()
         acquisition.setMagnification(10000.)
         acquisition.setVoltage(200.)
         acquisition.setSphericalAberration(2.26)
@@ -493,15 +502,14 @@
             mic.setLocation(i, "stack.stk")
             micSet.append(mic)
             mic.cleanObjId()
             micSet.write()
 
         # check defined indexes
         setOfMicrographsFileName = prot._getPath("micrographs.sqlite")
-        # print os.path.abspath(setOfPArticleFileName)
         indexes = sorted([index[1] for index in
                           getIndex(setOfMicrographsFileName)])
         for index, indexName in zip(indexes, indexesNames):
             self.assertEqual(index, 'index_' + indexName)
 
 
 class TestSetOfParticles(BaseTest):
@@ -550,29 +558,29 @@
         imgSet = emobj.SetOfParticles(filename=outFn)
         imgSet.setSamplingRate(1.0)
         imgSet.readStack(inStack)  # This should add 29 new items to the set
 
         self.assertEquals(size, imgSet.getSize())  # Check same size
         self.assertEquals(xdim, imgSet.getDim()[0])  # Check same dimensions
 
-        print("writing particles to: ", outFn)
+        logger.info("writing particles to %s" % outFn)
         imgSet.write()
 
         imgSet2 = emobj.SetOfParticles(filename=':memory:')
         imgSet2.copyInfo(imgSet)
         self.assertAlmostEqual(imgSet.getSamplingRate(), imgSet2.getSamplingRate())
 
     def test_hugeSet(self):
         """ Create a set of a big number of particles to measure
         creation time with sqlite operations. 
         """
         # Allow what huge means to be defined with environment var
         n = int(os.environ.get('SCIPION_TEST_HUGE', 10000))
-        print(">>>> Creating a set of %d particles." % n)
-        print("     (set SCIPION_TEST_HUGE environment var to other value)")
+        logger.info(">>>> Creating a set of %d particles." % n)
+        logger.info("     (set SCIPION_TEST_HUGE environment var to other value)")
 
         dbFn = self.getOutputPath('huge_set.sqlite')
         # dbFn = ':memory:'
 
         img = emobj.Particle()
         imgSet = emobj.SetOfParticles(filename=dbFn)
         imgSet.setSamplingRate(1.0)
@@ -589,45 +597,44 @@
 
         imgSet.write()
 
     def test_hugeSetToMd(self):
         """ Just as a benchrmark comparing to test_hugeSet ."""
         # Allow what huge means to be defined with environment var
         n = int(os.environ.get('SCIPION_TEST_HUGE', 10000))
-        print(">>>> Creating a set of %d particles." % n)
-        print("     (set SCIPION_TEST_HUGE environment var to other value)")
+        logger.info(">>>> Creating a set of %d particles." % n)
+        logger.info("     (set SCIPION_TEST_HUGE environment var to other value)")
 
         imgMd = md.MetaData()
 
         for i in range(1, n + 1):
             # Creating object inside the loop significantly
             # decrease performance
             # img = Particle()
             objId = imgMd.addObject()
             imgMd.setValue(md.MDL_IMAGE, '%06d@images.stk' % (i + 1), objId)
 
         mdFn = self.getOutputPath('huge_set.xmd')
-        print("Writing metadata to: ", mdFn)
+        logger.info("Writing metadata to %s." % mdFn)
         imgMd.write(mdFn)
 
     def test_hugeSetToText(self):
         """ Just as a benchrmark comparing to test_hugeSet ."""
         # Allow what huge means to be defined with environment var
         n = int(os.environ.get('SCIPION_TEST_HUGE', 10000))
-        print(">>>> Creating a set of %d particles." % n)
-        print("     (set SCIPION_TEST_HUGE environment var to other value)")
+        logger.info(">>>> Creating a set of %d particles." % n)
+        logger.info("     (set SCIPION_TEST_HUGE environment var to other value)")
 
         textFn = self.getOutputPath('huge_set.txt')
-        print("Writing to text file: ", textFn)
+        logger.info("Writing to text file %s " % textFn)
         f = open(textFn, 'w')
 
         for i in range(1, n + 1):
             string = '%06d@images.stk' % i
             f.write(string)
-            # print >> f, '%06d@images.stk' % i
 
         f.close()
 
     def test_getFiles(self):
         # create setofImages
         dbFn = self.getOutputPath('multistack_set.sqlite')
         # dbFn = ':memory:'
@@ -668,15 +675,14 @@
             part.setLocation(i, "stack.vol")
             partSet.append(part)
             part.cleanObjId()
         partSet.write()
 
         # check defined indexes
         setOfPArticleFileName = prot._getPath("particles.sqlite")
-        # print os.path.abspath(setOfPArticleFileName)
         indexes = sorted([index[1] for index in
                           getIndex(setOfPArticleFileName)])
         for index, indexName in zip(indexes, indexesNames):
             self.assertEqual(index, 'index_' + indexName)
 
 
 class TestSetOfCoordinates(BaseTest):
@@ -710,15 +716,15 @@
             coordSet.append(coord)
             coord.cleanObjId()
         coordSet.write()
 
         # check defined indexes
         setOfCoordinatesFileName = \
             prot._getPath("coordinates.sqlite")
-        print(os.path.abspath(setOfCoordinatesFileName))
+        logger.info(os.path.abspath(setOfCoordinatesFileName))
         indexes = sorted([index[1] for index in
                           getIndex(setOfCoordinatesFileName)])
         for index, indexName in zip(indexes, indexesNames):
             self.assertEqual(index, 'index_' + indexName)
 
         # Test speed: based on loop in file protocol_extractparticles.py
         # for 600 mic and 100 part the values for the first
@@ -934,15 +940,14 @@
 
         outputSet = emobj.SetOfParticles(filename=outFn)
         outputSet.copyInfo(inputSet)
 
         outputSet.copyItems(inputSet,
                             updateItemCallback=self._updateItem)
 
-        # print("writing particles to: ", outFn)
         outputSet.write()
         outputSet.close()
 
         # Read again the written set of particles
         checkSet = emobj.SetOfParticles(filename=outFn)
 
         # check that the first item (as the rest)
@@ -996,12 +1001,66 @@
         # when this is done then I will finish the test_mapper
 
 
 class TestCTFModel(TestCase):
     def test_stringContext(self):
         ctf = emobj.CTFModel()
         # All values to None should be printable without exception
-        print(ctf)
+        logger.info("Empty Ctf str converts to %s" % ctf)
 
         ctf.setDefocusU(2.4545)
-        print(ctf)
+        logger.info("Ctf with defocusU converts to %s" % ctf)
         self.assertTrue("2.45," in str(ctf))
+
+
+class TestSequenceHandler(pwtests.BaseTest):
+    NAME = 'USER_SEQ'
+    DESCRIPTION = 'User description'
+    UNIPROTID1 = 'P12345'
+    UNIPROTID2 = 'P03252'
+
+    @classmethod
+    def setUpClass(cls):
+        pwtests.setupTestProject(cls)
+
+    def testImportStructureAminoacidSequence1(self):
+        """
+        Import the sequence of chain B of atomic structure 3lqd.cif
+        """
+        args = {'inputSequenceName': self.NAME,
+                'inputProteinSequence':
+                    emprot.ProtImportSequence.IMPORT_FROM_UNIPROT,
+                'uniProtSequence': self.UNIPROTID1,
+                }
+        prot1 = self.newProtocol(emprot.ProtImportSequence, **args)
+        self.launchProtocol(prot1)
+        sequence1 = prot1.outputSequence
+
+        args = {'inputSequenceName': self.NAME,
+                'inputProteinSequence':
+                    emprot.ProtImportSequence.IMPORT_FROM_UNIPROT,
+                'uniProtSequence': self.UNIPROTID2,
+                }
+        prot2 = self.newProtocol(emprot.ProtImportSequence, **args)
+        self.launchProtocol(prot2)
+        sequence2 = prot2.outputSequence
+
+        #Saving Sequences into files
+        outFile = prot1._getPath('sequence.fasta')
+        sequence1.exportToFile(outFile)
+        # sequence2.exportToFile(prot2._getPath('sequence.genbank'))
+
+        #Reading exported sequence
+        readSequence = SequenceHandler()
+        sequencesDics = readSequence.readSequencesFromFile(outFile)
+        self.assertEqual(sequence1.getSequence(), sequencesDics[0]['sequence'])
+
+        #Appending sequence to existing sequence file
+        sequence2.appendToFile(outFile)
+
+        # Reading appended sequences
+        readSequence = SequenceHandler()
+        sequencesDics = readSequence.readSequencesFromFile(outFile)
+        self.assertEqual(sequence1.getSequence(), sequencesDics[0]['sequence'])
+        self.assertEqual(sequence2.getSequence(), sequencesDics[1]['sequence'])
+
+
```

### Comparing `scipion-em-3.0.9/pwem/tests/protocols/test_extract_particles.py` & `scipion-em-3.1.0/pwem/tests/protocols/test_extract_particles.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.0.9/pwem/tests/protocols/test_notifier.py` & `scipion-em-3.1.0/pwem/tests/protocols/test_notifier.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.0.9/pwem/tests/protocols/test_protocol_alignment_assign.py` & `scipion-em-3.1.0/pwem/tests/protocols/test_protocol_alignment_assign.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.0.9/pwem/tests/protocols/test_protocol_export2DB.py` & `scipion-em-3.1.0/pwem/tests/protocols/test_protocol_export2DB.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.0.9/pwem/tests/protocols/test_protocol_extract_coorinates.py` & `scipion-em-3.1.0/pwem/tests/protocols/test_protocol_extract_coorinates.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.0.9/pwem/tests/protocols/test_protocol_invert_Hand.py` & `scipion-em-3.1.0/pwem/tests/protocols/test_protocol_invert_Hand.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.0.9/pwem/tests/protocols/test_protocol_volume_homogenizer.py` & `scipion-em-3.1.0/pwem/tests/protocols/test_protocol_volume_homogenizer.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.0.9/pwem/tests/protocols/test_protocols_assign_orig.py` & `scipion-em-3.1.0/pwem/tests/protocols/test_protocols_assign_orig.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.0.9/pwem/tests/protocols/test_protocols_import_coords.py` & `scipion-em-3.1.0/pwem/tests/protocols/test_protocols_import_coords.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,14 +68,27 @@
         prot1.inputMicrographs.set(protImport.outputMicrographs)
         prot1.setObjLabel('import coords from xmipp ')
         self.launchProtocol(prot1)
         
         # Make sure that all 264 coordinates where correctly imported
         self.assertTrue(prot1.outputCoordinates.getSize() == 264)
 
+        filepath = prot1.outputCoordinates.getFileName()
+        prot2 = self.newProtocol(emprot.ProtImportCoordinates,
+                                 importFrom=emprot.ProtImportCoordinates.IMPORT_FROM_SCIPION,
+                                 filesPath=filepath, 
+                                 filesPattern='',
+                                 boxSize=110,
+                                 )
+        prot2.inputMicrographs.set(protImport.outputMicrographs)
+        prot2.setObjLabel('import coords from scipion ')
+        self.launchProtocol(prot2)
+        # Make sure that all 264 coordinates where correctly imported
+        self.assertTrue(prot2.outputCoordinates.getSize() == 264)
+
         # prot2 = self.newProtocol(ProtImportCoordinates,
         #                          importFrom=ProtImportCoordinates.IMPORT_FROM_RELION,
         #                          filesPath=self.dsXmipp.getFile('boxingDir'),#no dataset with picking
         #                          filesPattern='info/*_info.json',
         #                          boxSize=110,
         #                          scale=2,
         #                          invertX=False,
```

### Comparing `scipion-em-3.0.9/pwem/tests/protocols/test_protocols_import_ctfs.py` & `scipion-em-3.1.0/pwem/tests/protocols/test_protocols_import_ctfs.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.0.9/pwem/tests/protocols/test_protocols_import_masks.py` & `scipion-em-3.1.0/pwem/tests/protocols/test_protocols_import_masks.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.0.9/pwem/tests/protocols/test_protocols_import_micrographs.py` & `scipion-em-3.1.0/pwem/tests/protocols/test_protocols_import_micrographs.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.0.9/pwem/tests/protocols/test_protocols_import_movies.py` & `scipion-em-3.1.0/pwem/tests/protocols/test_protocols_import_movies.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.0.9/pwem/tests/protocols/test_protocols_import_particles.py` & `scipion-em-3.1.0/pwem/tests/protocols/test_protocols_import_particles.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 # *  All comments concerning this program package may be sent to the
 # *  e-mail address 'scipion@cnb.csic.es'
 # ***************************************************************************/
 
 import pyworkflow.tests as pwtests
 
 import pwem.protocols as emprot
+from pyworkflow.object import Pointer
 
 
 class TestImportBase(pwtests.BaseTest):
     @classmethod
     def setUpClass(cls):
         pwtests.setupTestProject(cls)
         cls.dsXmipp = pwtests.DataSet.getDataSet('xmipp_tutorial')
@@ -147,16 +148,40 @@
                                  magnification=10000,
                                  samplingRate=7.08,
                                  haveDataBeenPhaseFlipped=True
                                  )
         self.launchProtocol(prot1)
         self.checkOutput(prot1, 'outputParticles', ['outputParticles.hasAlignment2D()',
                                                     'outputParticles.isPhaseFlipped()'])
-        self.checkOutput(prot1, 'outputClasses')    
- 
+        self.checkOutput(prot1, 'outputClasses')
+
+
+        # Add tests for classes selector. representative
+        classSelector = self.newProtocol(emprot.ProtClassesSelector,
+                                         objLabel='representatives from 2 mayor classes',
+                                         firstNElements=2,
+                                         extractRepresentative=True
+                                         )
+        classSelector.inputClasses = Pointer(prot1, extended='outputClasses')
+        self.launchProtocol(classSelector)
+
+        self.assertSetSize(classSelector.output, size=2)
+
+        # Add tests for classes selector: items
+        classSelector2 = self.newProtocol(emprot.ProtClassesSelector,
+                                         objLabel='items from 3 mayor classes',
+                                         firstNElements=3,
+                                         extractRepresentative=False
+                                         )
+        classSelector2.inputClasses = Pointer(prot1, extended='outputClasses')
+        self.launchProtocol(classSelector2)
+
+        self.assertSetSize(classSelector2.output, size=1739)
+
+
     def test_fromRelionClassify3D(self):
         """ Import an EMX file with Particles and defocus
         """
         prot1 = self.newProtocol(emprot.ProtImportParticles,
                                  objLabel='from relion (classify 3d)',
                                  importFrom=emprot.ProtImportParticles.IMPORT_FROM_RELION,
                                  starFile=self.dsRelion.getFile('import/classify3d/extra/relion_it015_data.star'),
```

### Comparing `scipion-em-3.0.9/pwem/tests/protocols/test_protocols_import_sequence.py` & `scipion-em-3.1.0/pwem/tests/protocols/test_protocols_import_sequence.py`

 * *Files 9% similar despite different names*

```diff
@@ -25,16 +25,15 @@
 # *  e-mail address 'scipion@cnb.csic.es'
 # *
 # **************************************************************************
 
 import pyworkflow.tests as pwtests
 
 import pwem.protocols as emprot
-import pwem.convert as emconv
-
+from pwem.objects.data import Alphabet
 
 class TestImportBase(pwtests.BaseTest):
     @classmethod
     def setUpClass(cls):
         pwtests.setupTestProject(cls)
         cls.dsModBuild = pwtests.DataSet.getDataSet('model_building_tutorial')
 
@@ -48,73 +47,70 @@
     CHAIN1 = '{"model": 0, "chain": "B", "residues": 148}'  # Protein
     CHAIN2 = '{"model": 0, "chain": "A", "residues": 12}'  # RNA
     CHAIN3 = '{"model": 0, "chain": "I", "residues": 146}'  # DNA
     pdbID1 = "3lqd"  # Protein
     pdbID2 = "205d"  # RNA
     pdbID3 = "1aoi"  # DNA and protein
     GENEBANKID = 'AJ520101.1'
+    GENEBANKIDPROT = 'CAE8970392.1'
     UNIPROTID = 'P12345'
 
     def testImportUserNucleotideSequence1(self):
         """
         Import a single nucleotide sequence provided by the user (nucleotide
         alphabet by default)
         """
         args = {'inputSequenceName': self.NAME,
                 'inputSequenceDescription': self.DESCRIPTION,
-                'inputSequence': emconv.SEQ_TYPE_NUCLEOTIDES,
-                'nucleotideIUPACalphabet': emconv.EXTENDED_DNA_ALPHABET,
+                'inputSequence': Alphabet.NUCLEOTIDES,
+                'nucleotideIUPACalphabet': Alphabet.EXTENDED_DNA_ALPHABET,
                 'inputRawSequence': self.NUCLEOTIDESEQ1
                 }
         prot1 = self.newProtocol(emprot.ProtImportSequence, **args)
         prot1.setObjLabel('1_import DNA,\nseq from user\nExtended DNA '
                           'alphabet')
         self.launchProtocol(prot1)
         sequence = prot1.outputSequence
         self.assertEqual("USER_SEQ", sequence.getId())
         self.assertEqual("USER_SEQ", sequence.getSeqName())
         self.assertEqual("User description",
                          sequence.getDescription())
         self.assertEqual("AATGCGGTTG", sequence.getSequence()[:10])
-        self.assertEqual("GATCBDSW",
-                         emconv.indexToAlphabet(sequence.getIsAminoacids(),
-                                                sequence.getAlphabet()).letters)
+        self.assertEqual(Alphabet.EXTENDED_DNA_ALPHABET, sequence.getAlphabet())
 
     def testImportUserNucleotideSequence2(self):
         """
         Import a single nucleotide sequence provided by the user (nucleotide
         alphabet AMBIGOUS_RNA_ALPHABET)
         """
         args = {'inputSequenceName': self.NAME,
                 'inputSequenceDescription': self.DESCRIPTION,
-                'inputSequence': emconv.SEQ_TYPE_NUCLEOTIDES,
-                'nucleotideIUPACalphabet': emconv.AMBIGOUS_RNA_ALPHABET,
+                'inputSequence': Alphabet.NUCLEOTIDES,
+                'nucleotideIUPACalphabet': Alphabet.AMBIGOUS_RNA_ALPHABET,
                 'inputRawSequence': self.NUCLEOTIDESEQ1
                 }
         prot2 = self.newProtocol(emprot.ProtImportSequence, **args)
         prot2.setObjLabel('2_import RNA,\nseq from user\nAmbiguous RNA '
                           'alphabet')
         self.launchProtocol(prot2)
         sequence = prot2.outputSequence
         self.assertEqual("USER_SEQ", sequence.getId())
         self.assertEqual("USER_SEQ", sequence.getSeqName())
         self.assertEqual("User description",
                          sequence.getDescription())
         self.assertEqual("AAGCGGGGGB", sequence.getSequence()[:10])
-        self.assertEqual("GAUCRYWSMKHBVDN",
-                         emconv.indexToAlphabet(sequence.getIsAminoacids(),
-                                                sequence.getAlphabet()).letters)
+        self.assertEqual(Alphabet.AMBIGOUS_RNA_ALPHABET, sequence.getAlphabet())
 
     def testImportStructureNucleotideSequence1(self):
         """
         Import the sequence of chain A of atomic RNA structure 205d.cif
         """
         args = {'inputSequenceName': self.NAME,
                 'inputSequenceDescription': self.DESCRIPTION,
-                'inputSequence': emconv.SEQ_TYPE_NUCLEOTIDES,
+                'inputSequence': Alphabet.NUCLEOTIDES,
                 'inputNucleotideSequence':
                     emprot.ProtImportSequence.IMPORT_FROM_NUCLEOTIDE_STRUCTURE,
                 'inputStructureSequence':
                     emprot.ProtImportSequence.IMPORT_STRUCTURE_FROM_ID,
                 'pdbId': self.pdbID2,
                 'inputStructureChain': self.CHAIN2
                 }
@@ -124,26 +120,24 @@
         self.launchProtocol(prot3)
         sequence = prot3.outputSequence
         self.assertEqual("205d__0_A", sequence.getId())
         self.assertEqual("USER_SEQ", sequence.getSeqName())
         self.assertEqual("User description",
                          sequence.getDescription())
         self.assertEqual("GGACUUUGGU", sequence.getSequence()[:10])
-        self.assertEqual("GAUC",
-                         emconv.indexToAlphabet(sequence.getIsAminoacids(),
-                                                sequence.getAlphabet()).letters)
+        self.assertEqual(Alphabet.UNAMBIGOUS_RNA_ALPHABET, sequence.getAlphabet()) # RNA
 
     def testImportStructureNucleotideSequence2(self):
         """
         Import the sequence of chain A of atomic RNA structure 205d.cif
         """
         args = {'inputSequenceID': self.USERID,
                 'inputSequenceName': self.NAME,
                 'inputSequenceDescription': self.DESCRIPTION,
-                'inputSequence': emconv.SEQ_TYPE_NUCLEOTIDES,
+                'inputSequence': Alphabet.NUCLEOTIDES,
                 'inputNucleotideSequence':
                     emprot.ProtImportSequence.IMPORT_FROM_NUCLEOTIDE_STRUCTURE,
                 'inputStructureSequence':
                     emprot.ProtImportSequence.IMPORT_STRUCTURE_FROM_FILES,
                 'pdbFile': self.dsModBuild.getFile('PDBx_mmCIF/205d.cif'),
                 'inputStructureChain': self.CHAIN2
                 }
@@ -153,25 +147,23 @@
         self.launchProtocol(prot4)
         sequence = prot4.outputSequence
         self.assertEqual("UserID", sequence.getId())
         self.assertEqual("USER_SEQ", sequence.getSeqName())
         self.assertEqual("User description",
                          sequence.getDescription())
         self.assertEqual("GGACUUUGGU", sequence.getSequence()[:10])
-        self.assertEqual("GAUC",
-                         emconv.indexToAlphabet(sequence.getIsAminoacids(),
-                                                sequence.getAlphabet()).letters)
+        self.assertEqual(Alphabet.UNAMBIGOUS_RNA_ALPHABET, sequence.getAlphabet()) # RNA
 
     def testImportStructureNucleotideSequence3(self):
         """
         Import the sequence of chain I of atomic DNA structure 1aoi.cif
         """
         args = {'inputSequenceName': self.NAME,
                 'inputSequenceDescription': self.DESCRIPTION,
-                'inputSequence': emconv.SEQ_TYPE_NUCLEOTIDES,
+                'inputSequence': Alphabet.NUCLEOTIDES,
                 'inputNucleotideSequence':
                     emprot.ProtImportSequence.IMPORT_FROM_NUCLEOTIDE_STRUCTURE,
                 'inputStructureSequence':
                     emprot.ProtImportSequence.IMPORT_STRUCTURE_FROM_ID,
                 'pdbId': self.pdbID3,
                 'inputStructureChain': self.CHAIN3
                 }
@@ -181,26 +173,24 @@
         self.launchProtocol(prot5)
         sequence = prot5.outputSequence
         self.assertEqual("1aoi__0_I", sequence.getId())
         self.assertEqual("USER_SEQ", sequence.getSeqName())
         self.assertEqual("User description",
                          sequence.getDescription())
         self.assertEqual("ATCAATATCC", sequence.getSequence()[:10])
-        self.assertEqual("GAUC",
-                         emconv.indexToAlphabet(sequence.getIsAminoacids(),
-                                                sequence.getAlphabet()).letters)
+        self.assertEqual(Alphabet.UNAMBIGOUS_DNA_ALPHABET, sequence.getAlphabet()) # DNA
 
     def testImportStructureNucleotideSequence4(self):
         """
         Import the sequence of chain I of atomic DNA structure 1aoi.cif
         """
         args = {'inputSequenceID': self.USERID,
                 'inputSequenceName': self.NAME,
                 'inputSequenceDescription': self.DESCRIPTION,
-                'inputSequence': emconv.SEQ_TYPE_NUCLEOTIDES,
+                'inputSequence': Alphabet.NUCLEOTIDES,
                 'inputNucleotideSequence':
                     emprot.ProtImportSequence.IMPORT_FROM_NUCLEOTIDE_STRUCTURE,
                 'inputStructureSequence':
                     emprot.ProtImportSequence.IMPORT_STRUCTURE_FROM_FILES,
                 'pdbFile': self.dsModBuild.getFile('PDBx_mmCIF/1aoi.cif'),
                 'inputStructureChain': self.CHAIN3
                 }
@@ -210,24 +200,22 @@
         self.launchProtocol(prot6)
         sequence = prot6.outputSequence
         self.assertEqual("UserID", sequence.getId())
         self.assertEqual("USER_SEQ", sequence.getSeqName())
         self.assertEqual("User description",
                          sequence.getDescription())
         self.assertEqual("ATCAATATCC", sequence.getSequence()[:10])
-        self.assertEqual("GAUC",
-                         emconv.indexToAlphabet(sequence.getIsAminoacids(),
-                                                sequence.getAlphabet()).letters)
+        self.assertEqual(Alphabet.UNAMBIGOUS_DNA_ALPHABET, sequence.getAlphabet()) # DNA
 
     def testImportFileNucleotideSequence1(self):
         """
         Import a single nucleotide sequence from a text file
         """
         args = {'inputSequenceName': self.NAME,
-                'inputSequence': emconv.SEQ_TYPE_NUCLEOTIDES,
+                'inputSequence': Alphabet.NUCLEOTIDES,
                 'inputNucleotideSequence':
                     emprot.ProtImportSequence.IMPORT_FROM_NUCLEOTIDE_FILES,
                 'fileSequence': self.dsModBuild.getFile(
                     'Sequences/AJ520101.fasta')
                 }
         prot7 = self.newProtocol(emprot.ProtImportSequence, **args)
         prot7.setObjLabel('7_import nucleotide,\nseq from file')
@@ -237,146 +225,131 @@
         self.assertEqual('USER_SEQ', sequence.getSeqName())
         self.assertEqual("AJ520101.1 Rhizobium leguminosarum bv. viciae "
                          "plasmid "
                          "partial fixC gene, fixX gene, nifA gene "
                          "and nifB gene",
                          sequence.getDescription())
         self.assertEqual("GGATCCGAGA", sequence.getSequence()[:10])
-        self.assertEqual("GAUC",
-                         emconv.indexToAlphabet(sequence.getIsAminoacids(),
-                                                sequence.getAlphabet()).letters)
+        self.assertEqual(Alphabet.UNAMBIGOUS_DNA_ALPHABET, sequence.getAlphabet()) # DNA
 
     def testImportFileNucleotideSequence2(self):
         """
         Import a single nucleotide sequence from a text file
         """
         args = {'inputSequenceID': self.USERID,
                 'inputSequenceName': self.NAME,
                 'inputSequenceDescription': self.DESCRIPTION,
-                'inputSequence': emconv.SEQ_TYPE_NUCLEOTIDES,
+                'inputSequence': Alphabet.NUCLEOTIDES,
                 'inputNucleotideSequence':
                     emprot.ProtImportSequence.IMPORT_FROM_NUCLEOTIDE_FILES,
                 'fileSequence': self.dsModBuild.getFile(
                     'Sequences/AJ520101.fasta')
                 }
         prot8 = self.newProtocol(emprot.ProtImportSequence, **args)
         prot8.setObjLabel('8_import nucleotide,\nseq from file')
         self.launchProtocol(prot8)
         sequence = prot8.outputSequence
         self.assertEqual("UserID", sequence.getId())
         self.assertEqual('USER_SEQ', sequence.getSeqName())
         self.assertEqual("User description",
                          sequence.getDescription())
         self.assertEqual("GGATCCGAGA", sequence.getSequence()[:10])
-        self.assertEqual("GAUC",
-                         emconv.indexToAlphabet(sequence.getIsAminoacids(),
-                                                sequence.getAlphabet()).letters)
+        self.assertEqual(Alphabet.UNAMBIGOUS_DNA_ALPHABET, sequence.getAlphabet()) # DNA
 
     def testImportFileNucleotideSequence3(self):
         """
         Import a single nucleotide sequence from a text file
         """
         args = {'inputSequenceName': self.NAME,
-                'inputSequence': emconv.SEQ_TYPE_NUCLEOTIDES,
+                'inputSequence': Alphabet.NUCLEOTIDES,
                 'inputNucleotideSequence':
                     emprot.ProtImportSequence.IMPORT_FROM_NUCLEOTIDE_FILES,
                 'fileSequence': self.dsModBuild.getFile(
                     'Sequences/Several_sequences.fasta')
                 }
         prot9 = self.newProtocol(emprot.ProtImportSequence, **args)
         prot9.setObjLabel('9_import nucleotide,\nseq from file')
         self.launchProtocol(prot9)
         sequence = prot9.outputSequence
         self.assertEqual("Seq1", sequence.getId())
         self.assertEqual('USER_SEQ', sequence.getSeqName())
         self.assertEqual("Seq1 This is the sequence number one",
                          sequence.getDescription())
         self.assertEqual("TGGCTAAATA", sequence.getSequence()[:10])
-        self.assertEqual("GAUC",
-                         emconv.indexToAlphabet(sequence.getIsAminoacids(),
-                                                sequence.getAlphabet()).letters)
+        self.assertEqual(Alphabet.UNAMBIGOUS_DNA_ALPHABET, sequence.getAlphabet()) # DNA
 
     def testImportFileNucleotideSequence4(self):
         """
         Import a single nucleotide sequence from a text file that contains
         several sequences
         """
         args = {'inputSequenceID': self.USERID,
                 'inputSequenceName': self.NAME,
                 'inputSequenceDescription': self.DESCRIPTION,
-                'inputSequence': emconv.SEQ_TYPE_NUCLEOTIDES,
+                'inputSequence': Alphabet.NUCLEOTIDES,
                 'inputNucleotideSequence':
                     emprot.ProtImportSequence.IMPORT_FROM_NUCLEOTIDE_FILES,
                 'fileSequence': self.dsModBuild.getFile(
                     'Sequences/Several_sequences.fasta')
                 }
         prot10 = self.newProtocol(emprot.ProtImportSequence, **args)
         prot10.setObjLabel('10_import nucleotide,\nseq from file')
         self.launchProtocol(prot10)
         sequence = prot10.outputSequence
         self.assertEqual("UserID", sequence.getId())
         self.assertEqual('USER_SEQ', sequence.getSeqName())
         self.assertEqual("User description",
                          sequence.getDescription())
         self.assertEqual("TGGCTAAATA", sequence.getSequence()[:10])
-        self.assertEqual("GAUC",
-                         emconv.indexToAlphabet(sequence.getIsAminoacids(),
-                                                sequence.getAlphabet()).letters)
+        self.assertEqual(Alphabet.UNAMBIGOUS_DNA_ALPHABET, sequence.getAlphabet()) # DNA
 
     def testImportGeneBankNucleotideSequence1(self):
         """
         Import a single nucleotide sequence from GeneBank
         """
         args = {'inputSequenceName': self.NAME,
-                'inputSequence': emconv.SEQ_TYPE_NUCLEOTIDES,
+                'inputSequence': Alphabet.NUCLEOTIDES,
                 'inputNucleotideSequence':
-                    emprot.ProtImportSequence.IMPORT_FROM_GENEBANK,
+                    emprot.ProtImportSequence.IMPORT_FROM_NUCLEOTIDE_GENEBANK,
                 'geneBankSequence': self.GENEBANKID
                 }
         prot11 = self.newProtocol(emprot.ProtImportSequence, **args)
         prot11.setObjLabel('11_import nucleotide,\nseq from '
                            'GeneBank')
         self.launchProtocol(prot11)
         sequence = prot11.outputSequence
         self.assertEqual("AJ520101.1", sequence.getId())
         self.assertEqual('USER_SEQ', sequence.getSeqName())
         self.assertEqual("AJ520101.1 Rhizobium leguminosarum bv. viciae "
                          "plasmid partial fixC gene, fixX gene, nifA gene "
                          "and nifB gene",
                          sequence.getDescription())
         self.assertEqual("GGATCCGAGA", sequence.getSequence()[:10])
-        self.assertEqual("GAUC",
-                         emconv.indexToAlphabet(sequence.getIsAminoacids(),
-                                                sequence.getAlphabet()).letters)
+        self.assertEqual(Alphabet.NUCLEOTIDES_ALPHABET, sequence.getAlphabet()) # DNA
 
     def testImportGeneBankNucleotideSequence2(self):
         """
         Import a single nucleotide sequence from GeneBank
         """
-        args = {'inputSequenceID': self.USERID,
-                'inputSequenceName': self.NAME,
-                'inputSequenceDescription': self.DESCRIPTION,
-                'inputSequence': emconv.SEQ_TYPE_NUCLEOTIDES,
-                'inputNucleotideSequence':
-                    emprot.ProtImportSequence.IMPORT_FROM_GENEBANK,
-                'geneBankSequence': self.GENEBANKID
+        args = {'inputSequenceName': self.NAME,
+                'inputProteinSequence':
+                    emprot.ProtImportSequence.IMPORT_FROM_PROTEIN_GENEBANK,
+                'geneBankSequence': self.GENEBANKIDPROT
                 }
         prot12 = self.newProtocol(emprot.ProtImportSequence, **args)
-        prot12.setObjLabel('12_import nucleotide,\nseq from '
+        prot12.setObjLabel('12.5_import protein,\nseq from '
                            'GeneBank')
         self.launchProtocol(prot12)
         sequence = prot12.outputSequence
-        self.assertEqual("UserID", sequence.getId())
+        self.assertEqual(self.GENEBANKIDPROT, sequence.getId())
         self.assertEqual('USER_SEQ', sequence.getSeqName())
-        self.assertEqual("User description",
+        self.assertEqual('CAE8970392.1 unnamed protein product, partial [Tetraselmis striata]',
                          sequence.getDescription())
-        self.assertEqual("GGATCCGAGA", sequence.getSequence()[:10])
-        self.assertEqual("GAUC",
-                         emconv.indexToAlphabet(sequence.getIsAminoacids(),
-                                                sequence.getAlphabet()).letters)
+        self.assertEqual("MPDHHLRYFR", sequence.getSequence()[:10])
+        self.assertEqual(Alphabet.EXTENDED_PROTEIN_ALPHABET, sequence.getAlphabet()) # Protein
 
     def testImportUserAminoacidSequence1(self):
         """
         Import a single aminoacid sequence provided by the user (protein
         alphabet by default)
         """
         args = {'inputSequenceName': self.NAME,
@@ -389,42 +362,36 @@
         self.launchProtocol(prot13)
 
         sequence = prot13.outputSequence
         self.assertEqual("USER_SEQ", sequence.getId())
         self.assertEqual("USER_SEQ", sequence.getSeqName())
         self.assertEqual("User description", sequence.getDescription())
         self.assertEqual("LARKJLAKPA", sequence.getSequence()[:10])
-        self.assertEqual("ACDEFGHIKLMNPQRSTVWYBXZJUO",
-                         emconv.indexToAlphabet(sequence.getIsAminoacids(),
-                                                sequence.getAlphabet()).letters
-                         )
+        self.assertEqual(Alphabet.EXTENDED_PROTEIN_ALPHABET, sequence.getAlphabet()) # Extended protein
 
     def testImportUserAminoacidSequence2(self):
         """
         Import a single aminoacid sequence provided by the user (protein
         alphabet PROTEIN_ALPHABET
         """
         args = {'inputSequenceName': self.NAME,
                 'inputSequenceDescription': self.DESCRIPTION,
-                'proteinIUPACalphabet': emconv.PROTEIN_ALPHABET,
+                'proteinIUPACalphabet': Alphabet.AMINOACIDS,
                 'inputRawSequence': self.AMINOACIDSSEQ1
                 }
         prot14 = self.newProtocol(emprot.ProtImportSequence, **args)
         prot14.setObjLabel('14_import aminoacid seq,\n from user\nProtein '
                            'alphabet')
         self.launchProtocol(prot14)
         sequence = prot14.outputSequence
         self.assertEqual("USER_SEQ", sequence.getId())
         self.assertEqual("USER_SEQ", sequence.getSeqName())
         self.assertEqual("User description", sequence.getDescription())
         self.assertEqual("LARKLAKPAV", sequence.getSequence()[:10])
-        self.assertEqual("ACDEFGHIKLMNPQRSTVWY",
-                         emconv.indexToAlphabet(sequence.getIsAminoacids(),
-                                                sequence.getAlphabet()).letters
-                         )
+        self.assertEqual(Alphabet.PROTEIN_ALPHABET, sequence.getAlphabet()) # Protein
 
     def testImportStructureAminoacidSequence1(self):
         """
         Import the sequence of chain B of atomic structure 3lqd.cif
         """
         args = {'inputSequenceName': self.NAME,
                 'inputSequenceDescription': self.DESCRIPTION,
@@ -441,17 +408,15 @@
         self.launchProtocol(prot15)
         sequence = prot15.outputSequence
 
         self.assertEqual("3lqd__0_B", sequence.getId())
         self.assertEqual("USER_SEQ", sequence.getSeqName())
         self.assertEqual("User description", sequence.getDescription())
         self.assertEqual("VHLSGEEKSA", sequence.getSequence()[:10])
-        self.assertEqual("ACDEFGHIKLMNPQRSTVWY",
-                         emconv.indexToAlphabet(sequence.getIsAminoacids(),
-                                                sequence.getAlphabet()).letters)
+        self.assertEqual(Alphabet.EXTENDED_PROTEIN_ALPHABET, sequence.getAlphabet()) # Protein
 
     def testImportStructureAminoacidSequence2(self):
         """
         Import the sequence of chain B of atomic structure 3lqd.cif
         """
         args = {'inputSequenceID': self.USERID,
                 'inputSequenceName': self.NAME,
@@ -468,17 +433,15 @@
                            'structure')
         self.launchProtocol(prot16)
         sequence = prot16.outputSequence
         self.assertEqual("UserID", sequence.getId())
         self.assertEqual("USER_SEQ", sequence.getSeqName())
         self.assertEqual("User description", sequence.getDescription())
         self.assertEqual("VHLSGEEKSA", sequence.getSequence()[:10])
-        self.assertEqual("ACDEFGHIKLMNPQRSTVWY",
-                         emconv.indexToAlphabet(sequence.getIsAminoacids(),
-                                                sequence.getAlphabet()).letters)
+        self.assertEqual(Alphabet.EXTENDED_PROTEIN_ALPHABET, sequence.getAlphabet()) # Protein
 
     def testImportFileAminoacidSequence1(self):
         """
         Import a single aminoacid sequence from a text file
         """
         args = {'inputSequenceName': self.NAME,
                 'inputProteinSequence':
@@ -493,17 +456,15 @@
 
         self.assertEqual("YP_003024028.1", sequence.getId())
         self.assertEqual('USER_SEQ', sequence.getSeqName())
         self.assertEqual('YP_003024028.1 cytochrome c oxidase '
                          'subunit I (mitochondrion) [Homo sapiens]',
                          sequence.getDescription())
         self.assertEqual("MFADRWLFST", sequence.getSequence()[:10])
-        self.assertEqual("ACDEFGHIKLMNPQRSTVWY",
-                         emconv.indexToAlphabet(sequence.getIsAminoacids(),
-                                                sequence.getAlphabet()).letters)
+        self.assertEqual(Alphabet.EXTENDED_PROTEIN_ALPHABET, sequence.getAlphabet()) # Protein
 
     def testImportFileAminoacidSequence2(self):
         """
         Import a single aminoacid sequence from a text file
         """
         args = {'inputSequenceID': self.USERID,
                 'inputSequenceName': self.NAME,
@@ -518,17 +479,15 @@
         self.launchProtocol(prot18)
         sequence = prot18.outputSequence
         self.assertEqual("UserID", sequence.getId())
         self.assertEqual('USER_SEQ', sequence.getSeqName())
         self.assertEqual('User description',
                          sequence.getDescription())
         self.assertEqual("MFADRWLFST", sequence.getSequence()[:10])
-        self.assertEqual("ACDEFGHIKLMNPQRSTVWY",
-                         emconv.indexToAlphabet(sequence.getIsAminoacids(),
-                                                sequence.getAlphabet()).letters)
+        self.assertEqual(Alphabet.EXTENDED_PROTEIN_ALPHABET, sequence.getAlphabet()) # Protein
 
     def testImportUniprotAminoacidSequence1(self):
         """
         Import a single aminoacid sequence from UniProt
         """
         args = {'inputSequenceName': self.NAME,
                 'inputProteinSequence':
@@ -538,20 +497,18 @@
         prot19 = self.newProtocol(emprot.ProtImportSequence, **args)
         prot19.setObjLabel('19_import aminoacids,\nseq from '
                            'UniProt')
         self.launchProtocol(prot19)
         sequence = prot19.outputSequence
         self.assertEqual("P12345", sequence.getId())
         self.assertEqual('USER_SEQ', sequence.getSeqName())
-        self.assertEqual('Aspartate aminotransferase, mitochondrial',
+        self.assertEqual('sp|P12345.2|AATM_RABIT RecName: Full=Aspartate aminotransferase, mitochondrial; Short=mAspAT; AltName: Full=Fatty acid-binding protein; Short=FABP-1; AltName: Full=Glutamate oxaloacetate transaminase 2; AltName: Full=Kynurenine aminotransferase 4; AltName: Full=Kynurenine aminotransferase IV; AltName: Full=Kynurenine--oxoglutarate transaminase 4; AltName: Full=Kynurenine--oxoglutarate transaminase IV; AltName: Full=Plasma membrane-associated fatty acid-binding protein; Short=FABPpm; AltName: Full=Transaminase A; Flags: Precursor',
                          sequence.getDescription())
         self.assertEqual("MALLHSARVL", sequence.getSequence()[:10])
-        self.assertEqual("ACDEFGHIKLMNPQRSTVWY",
-                         emconv.indexToAlphabet(sequence.getIsAminoacids(),
-                                                sequence.getAlphabet()).letters)
+        self.assertEqual(Alphabet.EXTENDED_PROTEIN_ALPHABET, sequence.getAlphabet()) # Protein
 
     def testImportUniprotAminoacidSequence2(self):
         """
         Import a single aminoacid sequence from UniProt
         """
         args = {'inputSequenceID': self.USERID,
                 'inputSequenceName': self.NAME,
@@ -566,10 +523,8 @@
         self.launchProtocol(prot20)
         sequence = prot20.outputSequence
         self.assertEqual("UserID", sequence.getId())
         self.assertEqual('USER_SEQ', sequence.getSeqName())
         self.assertEqual('User description',
                          sequence.getDescription())
         self.assertEqual("MALLHSARVL", sequence.getSequence()[:10])
-        self.assertEqual("ACDEFGHIKLMNPQRSTVWY",
-                         emconv.indexToAlphabet(sequence.getIsAminoacids(),
-                                                sequence.getAlphabet()).letters)
+        self.assertEqual(Alphabet.EXTENDED_PROTEIN_ALPHABET, sequence.getAlphabet()) # Protein
```

### Comparing `scipion-em-3.0.9/pwem/tests/protocols/test_protocols_import_volumes.py` & `scipion-em-3.1.0/pwem/tests/protocols/test_protocols_import_volumes.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.0.9/pwem/tests/utils.py` & `scipion-em-3.1.0/pwem/tests/utils.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.0.9/pwem/tests/workflows/test_parallel_gpu_queue.py` & `scipion-em-3.1.0/pwem/tests/workflows/test_parallel_gpu_queue.py`

 * *Files 1% similar despite different names*

```diff
@@ -162,14 +162,15 @@
             :param useQueue: Use the queue system or not
             :return: the launched protocol
         """
         relionProtocols = Domain.importFromPlugin('relion.protocols',
                                                   doRaise=True)
         prot2D = self.newProtocol(relionProtocols.ProtRelionClassify2D,
                                   doCTF=False, maskDiameterA=340,
+                                  useGradientAlg=False,
                                   numberOfMpi=MPI, numberOfThreads=threads)
         prot2D.numberOfClasses.set(4)
         prot2D.numberOfIterations.set(3)
         prot2D.inputParticles.set(previousRun.outputParticles)
         prot2D.setObjLabel(label)
 
         if useQueue:
```

### Comparing `scipion-em-3.0.9/pwem/tests/workflows/test_workflow.py` & `scipion-em-3.1.0/pwem/tests/workflows/test_workflow.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.0.9/pwem/tests/workflows/test_workflow_initialvolume.py` & `scipion-em-3.1.0/pwem/tests/workflows/test_workflow_initialvolume.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.0.9/pwem/tests/workflows/test_workflow_mixed.py` & `scipion-em-3.1.0/pwem/tests/workflows/test_workflow_mixed.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,14 +17,16 @@
 # * Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA
 # * 02111-1307  USA
 # *
 # *  All comments concerning this program package may be sent to the
 # *  e-mail address 'scipion@cnb.csic.es'
 # *
 # **************************************************************************
+import  logging
+logger = logging.getLogger(__name__)
 
 import pyworkflow.tests as pwtests
 
 from pwem import Domain
 import pwem.protocols as emprot
 
 from .test_workflow import TestWorkflow
@@ -50,38 +52,38 @@
                                       samplingRate=1.237, voltage=300)
         self.launchProtocol(protImport)
         self.assertIsNotNone(protImport.outputMicrographs,
                              "There was a problem with the import")
         #         self.validateFiles('protImport', protImport)
 
         # Import a set of volumes
-        print("Import Volume")
+        logger.info("Import Volume")
         protImportVol = self.newProtocol(emprot.ProtImportVolumes, filesPath=self.vol1,
                                          samplingRate=9.896)
         self.launchProtocol(protImportVol)
         self.assertIsNotNone(protImportVol.getFiles(),
                              "There was a problem with the import")
         #        self.validateFiles('protImportVol', protImportVol)
 
         # Perform a downsampling on the micrographs
-        print("Downsampling...")
+        logger.info("Downsampling...")
         XmippProtPreprocessMicrographs = Domain.importFromPlugin('xmipp3.protocols',
                                                                  'XmippProtPreprocessMicrographs',
                                                                  doRaise=True)
         protDownsampling = self.newProtocol(XmippProtPreprocessMicrographs,
                                             doDownsample=True, downFactor=5,
                                             doCrop=False, runMode=1)
         protDownsampling.inputMicrographs.set(protImport.outputMicrographs)
         self.launchProtocol(protDownsampling)
         self.assertIsNotNone(protDownsampling.outputMicrographs,
                              "There was a problem with the downsampling")
         #         self.validateFiles('protDownsampling', protDownsampling)
 
         # Estimate CTF on the downsampled micrographs
-        print("Performing CTFfind...")
+        logger.info("Performing CTFfind...")
         ProtCTFFind = Domain.importFromPlugin('cistem.protocols',
                                               'CistemProtCTFFind', doRaise=True)
         protCTF = self.newProtocol(ProtCTFFind, numberOfThreads=4,
                                    minDefocus=22000, maxDefocus=25000)
         protCTF.inputMicrographs.set(protDownsampling.outputMicrographs)
         self.launchProtocol(protCTF)
         self.assertIsNotNone(protCTF.outputCTF,
@@ -92,26 +94,26 @@
             self.assertAlmostEquals(ctfModel.getDefocusU(), values[0], delta=1000)
             self.assertAlmostEquals(ctfModel.getDefocusV(), values[1], delta=1000)
             self.assertAlmostEquals(ctfModel.getMicrograph().getSamplingRate(),
                                     6.185, delta=0.001)
 
         #         self.validateFiles('protCTF', protCTF)
 
-        print("Running Eman import coordinates...")
+        logger.info("Running Eman import coordinates...")
         protPP = self.newProtocol(emprot.ProtImportCoordinates,
                                   importFrom=emprot.ProtImportCoordinates.IMPORT_FROM_EMAN,
                                   filesPath=self.crdsDir,
                                   filesPattern='*_info.json', boxSize=110)
         protPP.inputMicrographs.set(protDownsampling.outputMicrographs)
         self.launchProtocol(protPP)
         self.assertIsNotNone(protPP.outputCoordinates,
                              "There was a problem with the Eman import coordinates")
 
         # Extract the SetOfParticles.
-        print("Run extract particles with other downsampling factor")
+        logger.info("Run extract particles with other downsampling factor")
         XmippProtExtractParticles = Domain.importFromPlugin(
             'xmipp3.protocols',
             'XmippProtExtractParticles')
         OTHER = Domain.importFromPlugin('xmipp3.constants', 'OTHER')
         protExtract = self.newProtocol(XmippProtExtractParticles,
                                        boxSize=64,
                                        downsampleType=OTHER,
@@ -143,60 +145,60 @@
                                       samplingRate=1.237, voltage=300)
         self.launchProtocol(protImport)
         self.assertIsNotNone(protImport.outputMicrographs,
                              "There was a problem with the import")
         #         self.validateFiles('protImport', protImport)
 
         # Import a set of volumes
-        print("Import Volume")
+        logger.info("Import Volume")
         protImportVol = self.newProtocol(emprot.ProtImportVolumes, filesPath=self.vol1,
                                          samplingRate=9.896)
         self.launchProtocol(protImportVol)
         self.assertIsNotNone(protImportVol.getFiles(),
                              "There was a problem with the import")
         #        self.validateFiles('protImportVol', protImportVol)
 
         # Perform a downsampling on the micrographs
-        print("Downsampling...")
+        logger.info("Downsampling...")
         XmippProtPreprocessMicrographs = Domain.importFromPlugin(
             'xmipp3.protocols',
             'XmippProtPreprocessMicrographs',
             doRaise=True)
         protDownsampling = self.newProtocol(XmippProtPreprocessMicrographs,
                                             doDownsample=True, downFactor=5,
                                             doCrop=False, runMode=1)
         protDownsampling.inputMicrographs.set(protImport.outputMicrographs)
         self.launchProtocol(protDownsampling)
         self.assertIsNotNone(protDownsampling.outputMicrographs,
                              "There was a problem with the downsampling")
         #         self.validateFiles('protDownsampling', protDownsampling)
 
         # Estimate CTF on the downsampled micrographs
-        print("Performing CTFfind...")
+        logger.info("Performing CTFfind...")
         ProtCTFFind = Domain.importFromPlugin('cistem.protocols',
                                               'CistemProtCTFFind', doRaise=True)
         protCTF = self.newProtocol(ProtCTFFind, numberOfThreads=4,
                                    minDefocus=22000, maxDefocus=25000)
         protCTF.inputMicrographs.set(protImport.outputMicrographs)
         self.launchProtocol(protCTF)
         self.assertIsNotNone(protCTF.outputCTF,
                              "There was a problem with the CTF estimation")
         #         self.validateFiles('protCTF', protCTF)
 
-        print("Running Eman import coordinates...")
+        logger.info("Running Eman import coordinates...")
         protPP = self.newProtocol(emprot.ProtImportCoordinates,
                                   importFrom=emprot.ProtImportCoordinates.IMPORT_FROM_EMAN,
                                   filesPath=self.crdsDir,
                                   filesPattern='*_info.json', boxSize=110)
         protPP.inputMicrographs.set(protDownsampling.outputMicrographs)
         self.launchProtocol(protPP)
         self.assertIsNotNone(protPP.outputCoordinates,
                              "There was a problem with the Eman import coordinates")
 
-        print("<Run extract particles with Same as picking>")
+        logger.info("<Run extract particles with Same as picking>")
         XmippProtExtractParticles = Domain.importFromPlugin(
             'xmipp3.protocols',
             'XmippProtExtractParticles')
 
         SAME_AS_PICKING = Domain.importFromPlugin('xmipp3.constants',
                                                   'SAME_AS_PICKING')
         protExtract = self.newProtocol(XmippProtExtractParticles, boxSize=110,
@@ -205,42 +207,42 @@
         protExtract.inputCoordinates.set(protPP.outputCoordinates)
         protExtract.ctfRelations.set(protCTF.outputCTF)
         self.launchProtocol(protExtract)
         self.assertIsNotNone(protExtract.outputParticles,
                              "There was a problem with the extract particles")
         # self.validateFiles('protExtract', protExtract)
 
-        print("Run Preprocess particles")
+        logger.info("Run Preprocess particles")
         XmippProtCropResizeParticles = Domain.importFromPlugin(
             'xmipp3.protocols',
             'XmippProtCropResizeParticles')
         protCropResize = self.newProtocol(XmippProtCropResizeParticles,
                                           doResize=True, resizeOption=1,
                                           resizeDim=110)
         protCropResize.inputParticles.set(protExtract.outputParticles)
         self.launchProtocol(protCropResize)
 
         self.assertIsNotNone(protCropResize.outputParticles,
                              "There was a problem with resize/crop the particles")
 
-        print("Run ML2D")
+        logger.info("Run ML2D")
         XmippProtML2D = Domain.importFromPlugin('xmipp3.protocols',
                                                 'XmippProtML2D')
         protML2D = self.newProtocol(XmippProtML2D, numberOfClasses=8, maxIters=2,
                                     numberOfMpi=2, numberOfThreads=2)
         protML2D.inputParticles.set(protCropResize.outputParticles)
         self.launchProtocol(protML2D)
         self.assertIsNotNone(protML2D.outputClasses,
                              "There was a problem with ML2D")
         # self.validateFiles('protML2D', protML2D)
 
         #         #FIXME: Check the initial model with EMAn and restore the next step
         #         return
 
-        print("Run Initial Model")
+        logger.info("Run Initial Model")
 
         EmanProtInitModel = Domain.importFromPlugin('eman2.protocols',
                                                     'EmanProtInitModel',
                                                     doRaise=True)
         protIniModel = self.newProtocol(EmanProtInitModel, numberOfIterations=1,
                                         numberOfModels=2,
                                         shrink=5, symmetry='icos',
```

### Comparing `scipion-em-3.0.9/pwem/tests/workflows/test_workflow_mixed_large.py` & `scipion-em-3.1.0/pwem/tests/workflows/test_workflow_mixed_large.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,15 +87,15 @@
         # Now estimate CTF on the micrographs with ctffind 
         print("Performing CTFfind...")
         grigorieffLabProtocols = Domain.importFromPlugin(
             'cistem.protocols',
             doRaise=True)
         protCTF = self.newProtocol(grigorieffLabProtocols.CistemProtCTFFind,
                                    minDefocus=12000, maxDefocus=30000,
-                                   runMode=1, numberOfMpi=1, numberOfThreads=16)
+                                   numberOfThreads=16)
         protCTF.inputMicrographs.set(protPreprocess.outputMicrographs)
         protCTF.setObjLabel('CTF ctffind')
         self.launchProtocol(protCTF)
 
         print("Run extract particles with <Same as picking> option")
         protExtract = self.newProtocol(xmippProtocols.XmippProtExtractParticles,
                                        boxSize=60,
@@ -155,19 +155,17 @@
         self.launchProtocol(protExtract2)
         self.assertIsNotNone(protExtract2.outputParticles,
                              "There was a problem with the extract particles")
 
         print("Run Relion Classification2d")
         relionProtocols = Domain.importFromPlugin('relion.protocols',
                                                   doRaise=True)
-        prot2D = relionProtocols.ProtRelionClassify2D(regularisationParamT=2,
-                                                      numberOfMpi=4,
+        prot2D = relionProtocols.ProtRelionClassify2D(numberOfMpi=1,
                                                       numberOfThreads=4)
         prot2D.numberOfClasses.set(50)
-        prot2D.numberOfIterations.set(25)
         prot2D.inputParticles.set(protExtract2.outputParticles)
         prot2D.setObjLabel('relion 2D')
         self.launchProtocol(prot2D)
         self.assertIsNotNone(prot2D.outputClasses,
                              "There was a problem with Relion 2D:\n" + (prot2D.getErrorMessage() or "No error set"))
 
         print("Run Relion Refine")
@@ -239,15 +237,15 @@
         # Now estimate CTF on the micrographs with ctffind 
         print("Performing CTFfind...")
         grigorieffLabProtocols = Domain.importFromPlugin(
             'cistem.protocols',
             doRaise=True)
         protCTF = self.newProtocol(grigorieffLabProtocols.CistemProtCTFFind,
                                    minDefocus=12000, maxDefocus=30000,
-                                   runMode=1, numberOfMpi=1, numberOfThreads=16)
+                                   numberOfThreads=16)
         protCTF.inputMicrographs.set(protPreprocess.outputMicrographs)
         protCTF.setObjLabel('CTF ctffind')
         self.launchProtocol(protCTF)
 
         print("Run extract particles with <Same as picking> option")
         protExtract = self.newProtocol(xmippProtocols.XmippProtExtractParticles,
                                        boxSize=60,
```

### Comparing `scipion-em-3.0.9/pwem/tests/workflows/test_workflow_modeling.py` & `scipion-em-3.1.0/pwem/tests/workflows/test_workflow_modeling.py`

 * *Files 1% similar despite different names*

```diff
@@ -1003,18 +1003,21 @@
         newExtraCommands = self._createExtraCommandLine(0., 0., 0.)
         protCoot.extraCommands.set(newExtraCommands)
 
         try:
             self.launchProtocol(protCoot)
         except Exception as ex:
             print("second call to coot ended")
-        self.assertIsNotNone(protCoot.coot_001138_Imol_0000_version_0002.getFileName(),
+
+        PDB_output = eval("protCoot.coot_%06d_Imol_0000_version_0002"
+                          % protCoot.getObjId())
+        self.assertIsNotNone(PDB_output.getFileName(),
                              "There was a problem with the alignment")
         self.assertTrue(os.path.exists(
-            protCoot.coot_001138_Imol_0000_version_0002.getFileName()))
+            PDB_output.getFileName()))
         self.assertTrue(
             os.path.exists(protCoot.output3DMap_0001.getFileName()))
 
         # third coot
         protCoot.doInteractive.set(False)
         label = 'lastTestLabel'
         lastExtraCommands = self._createExtraCommandLine(0., 0., 0., label)
@@ -1758,15 +1761,16 @@
 
         protCoot.doInteractive.set(False)
         newExtraCommands = self._createExtraCommandLine(0., 0., 0.)
         protCoot.extraCommands.set(newExtraCommands)
         self.launchProtocol(protCoot)
 
         # EMRinger
-        coot_PDB = protCoot.coot_000730_Imol_0000_version_0002
+        coot_PDB = eval("protCoot.coot_%06d_Imol_0000_version_0002"
+                        % protCoot.getObjId())
         args = {'inputVolume': volume,
                 'inputStructure': coot_PDB,
                 'doTest': True
                 }
         PhenixProtRunEMRinger = Domain.importFromPlugin('phenix.protocols',
                                                         'PhenixProtRunEMRinger',
                                                         doRaise=True)
@@ -1779,15 +1783,16 @@
                           rotRatio=0.6756756756756757,
                           maxZscore=2.313625586144688,
                           modLength=121,
                           EMScore=2.103295987404262,
                           protEMRinger=protEMRinger)
 
         # refmac withouth mask
-        coot_PDB = protCoot.coot_000730_Imol_0000_version_0002
+        coot_PDB = eval("protCoot.coot_%06d_Imol_0000_version_0002"
+                        % protCoot.getObjId())
         args = {'inputVolume': volume,
                 'inputStructure': coot_PDB,
                 'generateMaskedVolume': False
                 }
         CCP4ProtRunRefmac = Domain.importFromPlugin('ccp4.protocols',
                                                     'CCP4ProtRunRefmac')
         protRefmac = self.newProtocol(CCP4ProtRunRefmac, **args)
@@ -1883,15 +1888,16 @@
 
         protCoot.doInteractive.set(False)
         newExtraCommands = self._createExtraCommandLine(0., 0., 0.)
         protCoot.extraCommands.set(newExtraCommands)
         self.launchProtocol(protCoot)
 
         # EMRinger
-        coot_PDB = protCoot.coot_001030_Imol_0000_version_0002
+        coot_PDB = eval("protCoot.coot_%06d_Imol_0000_version_0002"
+                        % protCoot.getObjId())
         args = {'inputVolume': volume,
                 'inputStructure': coot_PDB,
                 'doTest': True
                 }
         PhenixProtRunEMRinger = Domain.importFromPlugin('phenix.protocols',
                                                         'PhenixProtRunEMRinger',
                                                         doRaise=True)
@@ -1904,15 +1910,16 @@
                           rotRatio=0.6756756756756757,
                           maxZscore=2.313625586144688,
                           modLength=121,
                           EMScore=2.103295987404262,
                           protEMRinger=protEMRinger)
 
         # refmac with mask
-        coot_PDB = protCoot.coot_001030_Imol_0000_version_0002
+        coot_PDB = eval("protCoot.coot_%06d_Imol_0000_version_0002"
+                          % protCoot.getObjId())
         args = {'inputVolume': volume,
                 'inputStructure': coot_PDB,
                 'generateMaskedVolume': True
                 }
         CCP4ProtRunRefmac = Domain.importFromPlugin('ccp4.protocols',
                                                     'CCP4ProtRunRefmac')
         protRefmac = self.newProtocol(CCP4ProtRunRefmac, **args)
@@ -2503,15 +2510,16 @@
 
         protCoot.doInteractive.set(False)
         newExtraCommands = self._createExtraCommandLine(0., 0., 0.)
         protCoot.extraCommands.set(newExtraCommands)
         self.launchProtocol(protCoot)
 
         # MolProbity
-        coot_PDB = protCoot.coot_000754_Imol_0000_version_0002
+        coot_PDB = eval("protCoot.coot_%06d_Imol_0000_version_0002"
+                          % protCoot.getObjId())
         args = {'inputVolume': volume,
                 'resolution': 3.5,
                 'inputStructure': coot_PDB
                 }
 
         PhenixProtRunMolprobity = Domain.importFromPlugin('phenix.protocols',
                                                           'PhenixProtRunMolprobity')
@@ -2525,15 +2533,16 @@
                           rotOutliers=3.98,
                           cbetaOutliers=0,
                           clashScore=4.77,
                           overallScore=2.42,
                           protMolProbity=protMolProbity)
 
         # refmac withouth mask
-        coot_PDB = protCoot.coot_000754_Imol_0000_version_0002
+        coot_PDB = eval("protCoot.coot_%06d_Imol_0000_version_0002"
+                        % protCoot.getObjId())
         args = {'inputVolume': volume,
                 'inputStructure': coot_PDB,
                 'generateMaskedVolume': False
                 }
 
         CCP4ProtRunRefmac = Domain.importFromPlugin('ccp4.protocols',
                                                     'CCP4ProtRunRefmac')
@@ -2629,15 +2638,16 @@
 
         protCoot.doInteractive.set(False)
         newExtraCommands = self._createExtraCommandLine(0., 0., 0.)
         protCoot.extraCommands.set(newExtraCommands)
         self.launchProtocol(protCoot)
 
         # MolProbity
-        coot_PDB = protCoot.coot_001066_Imol_0000_version_0002
+        coot_PDB = eval("protCoot.coot_%06d_Imol_0000_version_0002"
+                          % protCoot.getObjId())
         args = {'inputVolume': volume,
                 'resolution': 3.5,
                 'inputStructure': coot_PDB
                 }
 
         PhenixProtRunMolprobity = Domain.importFromPlugin('phenix.protocols',
                                                           'PhenixProtRunMolprobity')
@@ -2651,15 +2661,16 @@
                           rotOutliers=3.98,
                           cbetaOutliers=0,
                           clashScore=4.77,
                           overallScore=2.42,
                           protMolProbity=protMolProbity)
 
         # refmac with mask
-        coot_PDB = protCoot.coot_001066_Imol_0000_version_0002
+        coot_PDB = eval("protCoot.coot_%06d_Imol_0000_version_0002"
+                          % protCoot.getObjId())
         args = {'inputVolume': volume,
                 'inputStructure': coot_PDB,
                 'generateMaskedVolume': True
                 }
 
         CCP4ProtRunRefmac = Domain.importFromPlugin('ccp4.protocols',
                                                     'CCP4ProtRunRefmac')
```

### Comparing `scipion-em-3.0.9/pwem/tests/workflows/test_workflow_xmipp.py` & `scipion-em-3.1.0/pwem/tests/workflows/test_workflow_xmipp.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,16 +20,17 @@
 # * 02111-1307  USA
 # *
 # *  All comments concerning this program package may be sent to the
 # *  e-mail address 'scipion@cnb.csic.es'
 # *
 # **************************************************************************
 
-import pyworkflow.tests as pwtests
+import numpy as np
 
+import pyworkflow.tests as pwtests
 from pwem import Domain
 import pwem.protocols as emprot
 
 from .test_workflow import TestWorkflow
 
 
 class TestXmippWorkflow(TestWorkflow):
@@ -127,16 +128,16 @@
         self.assertSetSize(protExtractCoords.outputCoordinates,
                            size=protExtract.outputParticles.getSize(),
                            msg="There was a problem with the coordinates extraction")
         # Check if the scaling factor is being calculated and applied correctly
         scale = protExtract.outputParticles.getSamplingRate() / protImport.outputMicrographs.getSamplingRate()
         inParticleCoord = protExtract.outputParticles.getFirstItem().getCoordinate()
         x, y = inParticleCoord.getPosition()
-        self.assertAlmostEqual(protExtractCoords.outputCoordinates.getFirstItem().getPosition(),
-                               (int(x * scale), int(y * scale)))
+        np.testing.assert_allclose(protExtractCoords.outputCoordinates.getFirstItem().getPosition(),
+                                   (int(x * scale), int(y * scale)), rtol=0.5)
 
         print("Run Screen Particles")
         protScreen = self.newProtocol(xmippProtcols.XmippProtScreenParticles,
                                       autoParRejection=xmippProtcols.XmippProtScreenParticles.REJ_MAXZSCORE,
                                       maxZscore=3.0)
         protScreen.inputParticles.set(protExtract.outputParticles)
         self.launchProtocol(protScreen)
@@ -191,31 +192,23 @@
         # Check if the scaling factor is being calculated and applied correctly
         scale = inputParticles.getSamplingRate() / protDownsampling.outputMicrographs.getSamplingRate()
         inParticleCoord = inputParticles.getFirstItem().getCoordinate()
         shifts = protExtractCoordsShifts.getShifts(inputParticles.getFirstItem().getTransform(),
                                                    inputParticles.getAlignment())
         x, y = inParticleCoord.getPosition()
         xCoor, yCoor = x - int(shifts[0]), y - int(shifts[1])
-        self.assertAlmostEqual(protExtractCoordsShifts.outputCoordinates.getFirstItem().getPosition(),
-                               (int(xCoor * scale), int(yCoor * scale)))
+        np.testing.assert_allclose(protExtractCoordsShifts.outputCoordinates.getFirstItem().getPosition(),
+                                   (int(xCoor * scale), int(yCoor * scale)), rtol=0.5)
 
         print("Run kerdensom")
         ProtKerdensom = self.newProtocol(xmippProtcols.XmippProtKerdensom,
                                          useMask=False, SomXdim=2, SomYdim=2,
                                          SomReg0=800, SomReg1=400, SomSteps=2)
         ProtKerdensom.inputParticles.set(protOnlyAlign.outputParticles)
         self.launchProtocol(ProtKerdensom)
         self.assertIsNotNone(ProtKerdensom.outputClasses, "There was a problem with kerdensom")
         # self.validateFiles('ProtKerdensom', ProtKerdensom)
 
-        print("Run Rotational Spectra")
-        xmippProtRotSpectra = self.newProtocol(xmippProtcols.XmippProtRotSpectra,
-                                               SomXdim=2, SomYdim=2,
-                                               spectraInnerRadius=4,
-                                               spectraOuterRadius=24)
-        xmippProtRotSpectra.inputParticles.set(protOnlyAlign.outputParticles)
-        self.launchProtocol(xmippProtRotSpectra)
-        self.assertIsNotNone(xmippProtRotSpectra.outputClasses, "There was a problem with Rotational Spectra")
 
 
 if __name__ == "__main__":
     pwtests.unittest.main()
```

### Comparing `scipion-em-3.0.9/pwem/tests/workflows/test_workflow_xmipp_assignment_tiltpairs.py` & `scipion-em-3.1.0/pwem/tests/workflows/test_workflow_xmipp_assignment_tiltpairs.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.0.9/pwem/tests/workflows/test_workflow_xmipp_ctf_consensus.py` & `scipion-em-3.1.0/pwem/tests/workflows/test_workflow_xmipp_ctf_consensus.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,15 +64,15 @@
 
         if not avgCTF:
             refCTF = refCTFs.getFirstItem()
             self.assertTrue(firstCTF.equalAttributes(refCTF),
                             "The outputCTF%s has different attributes "
                             "than the input." % label)
         else:
-            self.assertAlmostEqual(avgCTF['defocusU'], firstCTF.getDefocusU(), delta=100,
+            self.assertAlmostEqual(avgCTF['defocusU'], firstCTF.getDefocusU(), delta=200,
                                    msg="DefocusU doesn't match when defocus averaging.")
             self.assertAlmostEqual(avgCTF['defocusV'], firstCTF.getDefocusV(), delta=100,
                                    msg="DefocusV doesn't match when defocus averaging.")
             self.assertAlmostEqual(avgCTF['defocusAngle'], firstCTF.getDefocusAngle(), delta=1,
                                    msg="DefocusAngle doesn't match when defocus averaging.")
 
         if MDmerging:
@@ -176,17 +176,17 @@
                                         averageDefocus=True)
         protCTFcons3.inputCTF.set(protCTF1.outputCTF)
         protCTFcons3.inputCTF2.set(protCTF2.outputCTF)
         self.launchProtocol(protCTFcons3)
 
         protCTF1.outputCTF.load()  # Needed to update the set
         protCTF2.outputCTF.load()  # Needed to update the set
-        ctfAveraged = {'defocusU': 24140.0898,
-                       'defocusV': 23569.0801,
-                       'defocusAngle': 58.3429}
+        ctfAveraged = {'defocusU': 24025.6729,
+                       'defocusV': 23610.2071,
+                       'defocusAngle': 57.1943}
         self.checkCTFs(protCTFcons3,
                        refMics=protImport.outputMicrographs,
                        refCTFs=protCTF1.outputCTF,
                        avgCTF=ctfAveraged)
 
         # merging Metadata columns
         protCTFcons4 = self.newProtocol(XmippProtCTFConsensus,
```

### Comparing `scipion-em-3.0.9/pwem/tests/workflows/test_workflow_xmipp_rct.py` & `scipion-em-3.1.0/pwem/tests/workflows/test_workflow_xmipp_rct.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.0.9/pwem/viewers/__init__.py` & `scipion-em-3.1.0/pwem/viewers/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -21,36 +21,27 @@
 # *
 # *  All comments concerning this program package may be sent to the
 # *  e-mail address 'scipion@cnb.csic.es'
 # *
 # **************************************************************************
 
 # Expose many basic views
-from pyworkflow.gui.browser import FileTreeProvider, STANDARD_IMAGE_EXTENSIONS
 from .views import (DataView, ObjectView, MicrographsView, CtfView,
                     ClassesView, Classes3DView, CoordinatesObjectView,
                     ImageView, TableView)
 from .viewer_base import EmProtocolViewer
 from .plotter import EmPlotter
 from .viewers_data import DataViewer
 
-from .viewer_localres import LocalResolutionViewer
+from .viewer_localres import LocalResolutionViewer, ChimeraAttributeViewer
 from .viewer_vmd import Vmd, VmdView, VmdViewer
 from .viewer_fsc import FscViewer
 from .viewer_pdf import PDFReportViewer
-from .viewer_chimera import (Chimera, ChimeraView, ChimeraClientView,
-                             ChimeraDataView, ChimeraViewer, ChimeraAngDist)
+from .viewer_chimera import (Chimera, ChimeraView, ChimeraViewer, ChimeraAngDist)
 from .viewer_sequence import SequenceViewer
 from .viewer_volumes import viewerProtImportVolumes
+from .viewer_angular_dist import AngularDistributionViewer
+
 from .showj import *
 
-# register file handlers to preview info in the Filebrowser....
-from .filehandlers import *
-register = FileTreeProvider.registerFileHandler
-register(MdFileHandler(), '.xmd', '.star', '.pos', '.ctfparam', '.doc')
-register(ParticleFileHandler(),
-         '.xmp', '.tif', '.tiff', '.spi', '.mrc', '.map', '.raw',
-         '.inf', '.dm3', '.em', '.pif', '.psd', '.spe', '.ser', '.img',
-         '.hed', *STANDARD_IMAGE_EXTENSIONS)
-register(VolFileHandler(), '.vol')
-register(StackHandler(), '.stk', '.mrcs', '.st', '.pif', '.dm4')
-register(ChimeraHandler(), '.bild')
+if emConfig.CHIMERA_OLD_BINARY_PATH:
+    from .viewer_chimera import ChimeraOldViewer
```

### Comparing `scipion-em-3.0.9/pwem/viewers/filehandlers.py` & `scipion-em-3.1.0/pwem/viewers/viewer_volumes.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # **************************************************************************
 # *
-# * Authors:     Pablo Conesa (pconesa@cnb.csic.es)
+# * Authors:     Marta Martinez (mmmtnez@cnb.csic.es)
+# *              Roberto Marabini (roberto@cnb.csic.es)
 # *
 # * Unidad de  Bioinformatica of Centro Nacional de Biotecnologia , CSIC
 # *
 # * This program is free software; you can redistribute it and/or modify
 # * it under the terms of the GNU General Public License as published by
 # * the Free Software Foundation; either version 3 of the License, or
 # * (at your option) any later version.
@@ -19,197 +20,173 @@
 # * Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA
 # * 02111-1307  USA
 # *
 # *  All comments concerning this program package may be sent to the
 # *  e-mail address 'scipion@cnb.csic.es'
 # *
 # **************************************************************************
-"""
-This modules contains file handlers to be registered in the scipion file browser
-"""
-import os
-
-import pyworkflow.utils as pwutils
-from pyworkflow import gui
-from pyworkflow.gui.browser import FileHandler, isStandardImage
-
-from pwem import emlib
-
-
-class ImageFileHandler(FileHandler):
-    _image = emlib.Image()
-    _index = ''
-
-    def _getImageString(self, filename):
-        if isStandardImage(filename):
-            return "Image file."
-        x, y, z, n = emlib.getImageSize(filename)
-        objType = 'Image'
-        dimMsg = "*%(objType)s file*\n  dimensions: %(x)d x %(y)d"
-        expMsg = "Columns x Rows "
-        if z > 1:
-            dimMsg += " x %(z)d"
-            expMsg += " x Slices"
-            objType = 'Volume'
-        if n > 1:
-            dimMsg += " x %(n)d"
-            expMsg += " x Objects"
-            objType = 'Stack'
-        return (dimMsg + "\n" + expMsg) % locals()
-
-    def _getImagePreview(self, filename):
-        dim = 128
-
-        if isStandardImage(filename):
-            self.tkImg = gui.getImage(os.path.abspath(filename),
-                                      tkImage=True, maxheight=dim)
-        else:
-            fn = self._index + filename
-            self.tkImg = getTkImage(self._image, fn, dim)
-
-        return self.tkImg
-
-    def getFilePreview(self, objFile):
-        fn = objFile.getPath()
-        return self._getImagePreview(fn), self._getImageString(fn)
-
-    def getFileActions(self, objFile):
-        from .views import DataView
-        fn = objFile.getPath()
-        return [('Open with Xmipp viewer', lambda: DataView(fn).show(),
-                 pwutils.Icon.ACTION_VISUALIZE)]
-
-
-class ParticleFileHandler(ImageFileHandler):
-    def getFileIcon(self, objFile):
-        return 'file_image.gif'
-
-
-class VolFileHandler(ImageFileHandler):
-    def getFileIcon(self, objFile):
-        return 'file_vol.gif'
 
 
-class StackHandler(ImageFileHandler):
-    _index = '1@'
-
-    def getFileIcon(self, objFile):
-        return 'file_stack.gif'
-
-
-class ChimeraHandler(FileHandler):
-
-    def getFileActions(self, objFile):
-        from .viewer_chimera import ChimeraView
-        fn = objFile.getPath()
-        return [('Open with Chimera', lambda: ChimeraView(fn).show(),
-                 pwutils.Icon.ACTION_VISUALIZE)]
-
-    def getFileIcon(self, objFile):
-        return 'file_text.gif'
-
-
-class MdFileHandler(ImageFileHandler):
-    def getFileIcon(self, objFile):
-        return 'file_md.gif'
+"""
+This module implements visualization program
+for input volumes.
+"""
 
-    def _getImgPath(self, mdFn, imgFn):
-        """ Get ups and ups until finding the relative location to images. """
-        path = os.path.dirname(mdFn)
-        index, fn = emlib.FileName(imgFn).decompose()
+import os
+from shutil import which
+from tkinter.messagebox import showerror
 
-        while path and path != '/':
-            newFn = os.path.join(path, fn)
-            if os.path.exists(newFn):
-                if index:
-                    newFn = '%d@%s' % (index, newFn)
-                return newFn
-            path = os.path.dirname(path)
+import pyworkflow.protocol.params as params
+import pyworkflow.viewer as pwviewer
 
-        return None
+import pwem.objects as emobj
+import pwem.protocols as emprot
+from pwem.viewers import Chimera, ChimeraView, EmProtocolViewer
+from pwem.emlib import image
+
+VOLUME_SLICES = 1
+VOLUME_CHIMERA = 0
+
+
+class viewerProtImportVolumes(EmProtocolViewer):
+    """ Wrapper to visualize different type of objects
+    with the Xmipp program xmipp_showj. """
+
+    _label = 'viewer input volume'
+    _targets = [emprot.ProtImportVolumes, emprot.ProtOrigSampling]
+    _environments = [pwviewer.DESKTOP_TKINTER, pwviewer.WEB_DJANGO]
+
+    def _defineParams(self, form):
+        form.addSection(label='Visualization of input volumes')
+        form.addParam('displayVol', params.EnumParam,
+                      choices=['chimerax', 'slices'],
+                      default=VOLUME_CHIMERA,
+                      display=params.EnumParam.DISPLAY_HLIST,
+                      label='Display volume with',
+                      help='*chimerax*: display volumes as surfaces with '
+                           'ChimeraX.\n *slices*: display volumes as 2D slices '
+                           'along z axis.\n If the number of volumes is equal to 1, '
+                           'a system of coordinates is shown'
+                      )
+
+    def _getVisualizeDict(self):
+        return {
+            'displayVol': self._showVolumes,
+        }
+
+    def _validate(self):
+        if (self.displayVol == VOLUME_CHIMERA
+                and which(Chimera.getProgram()) is None):
+            return ["chimera is not available. "
+                    "Either install it or choose option 'slices'. "]
+        return []
+
+    # =========================================================================
+    # ShowVolumes
+    # =========================================================================
+
+    def _showVolumes(self, paramName=None):
+        if self.displayVol == VOLUME_CHIMERA:
+            return self._showVolumesChimera()
+
+        elif self.displayVol == VOLUME_SLICES:
+            return self._showVolumesSlices()
+
+    def _createSetOfVolumes(self):
+        try:
+            setOfVolumes = self.protocol.outputVolumes
+            sampling = self.protocol.outputVolumes.getSamplingRate()
+        except Exception as ex:
+            setOfVolumes = self.protocol._createSetOfVolumes()
+            setOfVolumes.append(self.protocol.outputVolume)
+            sampling = self.protocol.outputVolume.getSamplingRate()
+
+        return sampling, setOfVolumes
+
+    def _showVolumesChimera(self):
+        """ Create a chimera script to visualize selected volumes. """
+        tmpFileNameCMD = self.protocol._getExtraPath("chimera.cxc")
+        f = open(tmpFileNameCMD, "w")
+        sampling, _setOfVolumes = self._createSetOfVolumes()
+        count = 1  # chimeraX stars counting in 1 (chimera in 0)
+
+        if len(_setOfVolumes) == 1:
+            # if we have a single volume then create axis
+            # as bild file. Chimera must read the bild file first
+            # otherwise system of coordinates will not
+            # be in the center of the window
+
+            dim = self.protocol.outputVolume.getDim()[0]
+            tmpFileNameBILD = os.path.abspath(self.protocol._getExtraPath(
+                "axis.bild"))
+            Chimera.createCoordinateAxisFile(dim,
+                                             bildFileName=tmpFileNameBILD,
+                                             sampling=sampling)
+            f.write("open %s\n" % tmpFileNameBILD)
+            f.write("cofr 0,0,0\n")  # set center of coordinates
+            count = 2  # skip first model because is not a 3D map
+
+        for vol in _setOfVolumes:
+            localVol = os.path.abspath(image.ImageHandler.removeFileType(
+                vol.getFileName()))
+            if localVol.endswith("stk"):
+                errorWindow(None, "Extension .stk is not supported")
+            f.write("open %s\n" % localVol)
+            f.write("volume #%d style surface level 0.001 voxelSize %f\n" %
+                    (count, sampling))
+            count += 1
 
-    def _getMdString(self, filename, block=None):
-        md = emlib.MetaData()
-        if block:
-            md.read(block + '@' + filename)
+        if len(_setOfVolumes) > 1:
+            f.write('tile\n')
         else:
-            md.read(filename, 1)
-        labels = md.getActiveLabels()
-        msg = "Metadata items: *%d*\n" % md.getParsedLines()
-        msg += "Metadata labels: " + ''.join(
-            ["\n   - %s" % emlib.label2Str(l)
-             for l in labels])
-
-        imgPath = None
-        for label in labels:
-            if emlib.labelIsImage(label):
-                imgPath = self._getImgPath(filename,
-                                           md.getValue(label, md.firstObject()))
-                break
-        if imgPath:
-            self._imgPreview = self._getImagePreview(imgPath)
-            self._imgInfo = self._getImageString(imgPath)
-        return msg
-
-    def getFilePreview(self, objFile):
-        self._imgPreview = None
-        self._imgInfo = None
-        filename = objFile.getPath()
-        ext = pwutils.getExt(filename)
-
-        if ext == '.xmd' or ext == '.ctfparam' or ext == '.pos' or ext == '.doc':
-            msg = "*Metadata File* "
-            blocks = emlib.getBlocksInMetaDataFile(filename)
-            nblocks = len(blocks)
-            if nblocks <= 1:
-                mdStr = self._getMdString(filename)
-                msg += "  (single block)\n"
-                if self._imgInfo:
-                    msg += "\nFirst item: \n" + self._imgInfo
-                msg += '\n' + mdStr
+            x, y, z = vol.getShiftsFromOrigin()
+            f.write("volume #2 origin %0.2f,%0.2f,%0.2f\n" % (x, y, z))
+            if vol.getHalfMaps():
+                for halfMap in vol.getHalfMaps().split(','):
+                    if not os.path.abspath(halfMap).endswith(".mrc"):
+                        f.write("open %s\n" % (os.path.abspath(halfMap).split(".")[0] + ".mrc"))
+                    else:
+                        f.write("open %s\n" % os.path.abspath(halfMap))
+                    f.write("volume #%d style surface level 0.001 voxelSize %f\n" %
+                            (count, sampling))
+                    f.write("volume #%d origin %0.2f,%0.2f,%0.2f\n" %
+                            (count, x, y, z))
+                    f.write("tile\n")
+                    count += 1
+        f.write("view\n")
+        f.close()
+        return [ChimeraView(tmpFileNameCMD)]
+
+    def _showVolumesSlices(self):
+        # Write an sqlite with all volumes selected for visualization.
+        sampling, setOfVolumes = self._createSetOfVolumes()
+        # setOfVolumes.setSamplingRate(sampling)
+        if len(setOfVolumes) == 1:
+            if self.protocol.outputVolume.getHalfMaps():
+                setOfVolumes = self.protocol._createSetOfVolumes(suffix='tmp')
+                vol = emobj.Volume()
+                vol.setFileName(self.protocol.outputVolume.getFileName())
+                vol.setSamplingRate(sampling)
+                setOfVolumes.append(vol)
+                for halfMap in self.protocol.outputVolume.getHalfMaps().split(','):
+                    volHalf = emobj.Volume()
+                    volHalf.setSamplingRate(sampling)
+                    if not halfMap.endswith(".mrc"):
+                        volHalf.setFileName(halfMap.split(".")[0] + ".mrc")
+                    else:
+                        volHalf.setFileName(halfMap)
+                    setOfVolumes.append(volHalf)
+                setOfVolumes.write()
+                return [self.objectView(setOfVolumes)]
             else:
-                mdStr = self._getMdString(filename, blocks[0])
-                msg += "  (%d blocks) " % nblocks
-                if self._imgInfo:
-                    msg += "\nFirst item: \n" + self._imgInfo
-                msg += "\nFirst block: \n" + mdStr
-                msg += "\nAll blocks:" + ''.join(
-                    ["\n  - %s" % b for b in blocks])
-        elif ext == '.star':
-            msg = "*Relion STAR file* \n"
-            msg += self._getMdString(filename)
-
-        return self._imgPreview, msg
-
-
-# Image methods for filehandlers
-def getPILImage(imageXmipp, dim=None, normalize=True):
-    """ Given an image read by Xmipp, convert it to PIL. """
-    from PIL import Image
-
-    if normalize:
-        imageXmipp.convert2DataType(emlib.DT_UCHAR, emlib.CW_ADJUST)
-
-    imageData = imageXmipp.getData()
-    image = Image.fromarray(imageData)
-    if dim:
-        size = int(dim), int(dim)
-        image.thumbnail(size, Image.ANTIALIAS)
-    return image
-
-
-def getTkImage(imageXmipp, filename, dim):
-    from PIL import ImageTk
-    imageXmipp.readPreview(filename, dim)
-    return ImageTk.PhotoImage(getPILImage(imageXmipp))
-
-
-def getImageFromPath(imagePath):
-    """ Read an image using Xmipp, convert to PIL
-    and then return as expected by Tk.
-    """
-    img = emlib.Image(imagePath)
-    imgPIL = getPILImage(img)
-    from PIL import ImageTk
-    imgTk = ImageTk.PhotoImage(imgPIL)
+                return [self.objectView(self.protocol.outputVolume)]
+        return [self.objectView(setOfVolumes)]
+
+
+def errorWindow(tkParent, msg):
+    try:
+        showerror("Error",  # bar title
+                  msg,  # message
+                  parent=tkParent)
+    except Exception as ex:
+        print("Error:", msg)
 
-    return imgTk
```

### Comparing `scipion-em-3.0.9/pwem/viewers/plotter.py` & `scipion-em-3.1.0/pwem/viewers/plotter.py`

 * *Files 9% similar despite different names*

```diff
@@ -19,66 +19,104 @@
 # * Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA
 # * 02111-1307  USA
 # *
 # *  All comments concerning this program package may be sent to the
 # *  e-mail address 'scipion@cnb.csic.es'
 # *
 # **************************************************************************
-
-from math import radians
+import logging
+logger = logging.getLogger(__name__)
+from math import radians, degrees
 import numpy as np
 import matplotlib.cm as cm
 from scipy.ndimage.filters import gaussian_filter
 
+from pwem.convert.transformations import euler_from_matrix
 from pyworkflow.gui.plotter import Plotter, plt
 import pwem.emlib.metadata as md
 import numbers
 
 
 class EmPlotter(Plotter):
     """ Class to create several plots. """
 
     def __init__(self, x=1, y=1, mainTitle="", **kwargs):
         Plotter.__init__(self, x, y, mainTitle, **kwargs)
 
     def plotAngularDistribution(self, title, rot,
                                 tilt, weight=[], max_p=40,
                                 min_p=5, color='blue'):
-        """ Create an special type of subplot, representing the angular
+        """ Create a special type of subplot, representing the angular
         distribution of weight projections. """
         if weight:
             max_w = max(weight)
             min_w = min(weight)
             a = self.createSubPlot(title,
                                    'Min weight=%(min_w).2f, Max weight=%(max_w).2f'
                                    % locals(), '', projection='polar')
+
+            pointSizes = []
             for r, t, w in zip(rot, tilt, weight):
-                pointsize = int((w - min_w) / (max_w - min_w + 0.001) * (max_p - min_p) + min_p)
-                a.plot(r, t, markerfacecolor=color, marker='.', markersize=pointsize)
+                 pointsize = int((w - min_w) / (max_w - min_w + 0.001) * (max_p - min_p) + min_p)
+                 pointSizes.append(pointsize)
+
+            a.scatter(rot, tilt, s=pointSizes, c=color, marker='.')
         else:
-            a = self.createSubPlot(title, 'Empty plot', '', projection='polar')
-            for r, t in zip(rot, tilt):
-                a.plot(r, t, markerfacecolor=color, marker='.', markersize=10)
+            a = self.createSubPlot(title, 'Non weighted plot', '', projection='polar')
+            a.scatter(rot, tilt, s=10, c=color, marker='.')
         return a
 
     def plotAngularDistributionHistogram(self, title, rot, tilt):
-        """ Create an special type of subplot, representing the angular
+        """ Create a special type of subplot, representing the angular
         distribution of weight projections. """
         heatmap, xedges, yedges = np.histogram2d(rot, tilt, bins=100)
         sigma = min(max(xedges) - min(xedges), max(yedges) - min(yedges)) / 20
         heatmap = gaussian_filter(heatmap, sigma=sigma)
         heatmapImage = heatmap.T
         extent = [xedges[0], xedges[-1], yedges[0], yedges[-1]]
 
         a = self.createSubPlot(title, 'Angular distribution', '')
         mappable = a.imshow(heatmapImage, extent=extent, origin='lower', cmap=cm.jet, aspect='auto')
         a.set_xlabel('Rotational angle')
         a.set_ylabel('Tilt angle')
         return mappable
 
+
+    def plotAngularDistributionFromSet(self, mdSet, title, weightAttr=None, histogram=False, **kwargs):
+        """ Read the values of the transformation matrix
+         and plot its histogram or its angular distribution.
+
+         :param mdSet: Set with alignment information at with item.getTransform()
+         :param title: Title of the plot
+        """
+        rots = []
+        tilts = []
+        weights = []
+
+        if histogram:
+            for item in mdSet:
+                rot, tilt, psi = euler_from_matrix(item.getTransform().getMatrix())
+                rots.append(rot)
+                tilts.append(tilt)
+
+            return self.plotAngularDistributionHistogram(title, rots, tilts)
+        else:
+            for item in mdSet:
+                psi, tilt, rot = euler_from_matrix(item.getTransform().getMatrix(), axes="szyz" )
+
+                rots.append(rot)
+                tilts.append(degrees(tilt))
+
+                if weightAttr:
+                    weight = getattr(item, weightAttr).get()
+                    weights.append(weight)
+
+
+            return self.plotAngularDistribution(title, rots, tilts, weights, **kwargs)
+
     def plotAngularDistributionFromMd(self, mdFile, title, **kwargs):
         """ Read the values of rot, tilt and weights from
         the metadata and plot the angular distribution.
         ANGLES are in DEGREES
         In the metadata:
             rot: MDL_ANGLE_ROT
             tilt: MDL_ANGLE_TILT
@@ -116,17 +154,17 @@
                    , vmaxData
                    , cmap='jet'
                    , xticksLablesMajor=None
                    , yticksLablesMajor=None
                    , rotationX=90.
                    , rotationY=0.
                    , **kwargs):
-        interpolation = kwargs.get('interpolation', "none")
+        interpolation = kwargs.pop('interpolation', "none")
         plot = img.imshow(matrix, interpolation=interpolation, cmap=cmap,
-                          vmin=vminData, vmax=vmaxData)
+                          vmin=vminData, vmax=vmaxData, **kwargs)
         if xticksLablesMajor is not None:
             plt.xticks(range(len(xticksLablesMajor)),
                        xticksLablesMajor[:len(xticksLablesMajor)],
                        rotation=rotationX)
         if yticksLablesMajor is not None:
             plt.yticks(range(len(yticksLablesMajor)),
                        yticksLablesMajor[:len(yticksLablesMajor)],
```

### Comparing `scipion-em-3.0.9/pwem/viewers/showj.py` & `scipion-em-3.1.0/pwem/viewers/showj.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,29 +25,32 @@
 # **************************************************************************
 """
 Configuration definition for launching the ShowJ visualization utility.
 The name of ShowJ is due historical reasons. This data visualization tools
 was first called xmipp_show. And later was re-written using Java and 
 became xmipp_showj.
 """
+import logging
+logger = logging.getLogger(__name__)
 
 import os
 import sys
 from os.path import join
 from collections import OrderedDict
 import subprocess
 
 from pyworkflow import Config
-from pyworkflow.utils import getFreePort
+from pyworkflow.utils import getFreePort, runCommand
 from pwem import Config as emConfig
 import threading
 import shlex
 import socketserver
 from pyworkflow.constants import SCIPION_DOMAIN, SCIPION_HOME_VAR, SCIPION_DEBUG
 
+javaVersion = None
 
 # ----------------------- Showj constants ---------------------------
 COL_RENDER_NONE = 0
 COL_RENDER_ID = 1
 COL_RENDER_TEXT = 2
 COL_RENDER_IMAGE = 3
 COL_RENDER_CHECKBOX = 4
@@ -249,14 +252,28 @@
     import platform
     arch = platform.architecture()[0]
     for a in ['32', '64']:
         if a in arch:
             return a
     return 'NO_ARCH'
 
+def getJavaVersion():
+    global javaVersion
+
+    if javaVersion is None:
+        version = subprocess.check_output([getJavaBin(), '-version'], stderr=subprocess.STDOUT)
+        javaVersion = int(version.decode("utf-8").split('"')[1].split('.')[0])
+
+    return javaVersion
+def getJavaBin():
+
+    if emConfig.JAVA_HOME:
+        return join(emConfig.JAVA_HOME, "bin", "java")
+    else:
+        return  "java"
 
 def getJavaIJappArguments(memory, appName, appArgs):
     """ Build the command line arguments to launch
     a Java application based on ImageJ.
     memory: the amount of memory passed to the JVM.
     appName: the qualified name of the java application.
     appArgs: the arguments specific to the application.
@@ -268,18 +285,15 @@
     javaBind = join(emConfig.XMIPP_HOME, "bindings", "java")
     imagej_home = join(javaBind, "imagej")
     lib = join(emConfig.XMIPP_HOME, "lib")
     javaLib = join(javaBind, 'lib')
     plugins_dir = os.path.join(imagej_home, "plugins")
     arch = getArchitecture()
 
-    import subprocess
-    version = subprocess.check_output(['java', '-version'], stderr=subprocess.STDOUT)
-    majorVersion = int(version.decode("utf-8").split('"')[1].split('.')[0])
-    if majorVersion > 9:
+    if getJavaVersion() > 9:
         args = "-Xmx%(memory)sg -Djava.library.path=%(lib)s -Dplugins.dir=%(plugins_dir)s -cp %(jdkLib)s/*:%(imagej_home)s/*:%(javaLib)s/* %(appName)s %(appArgs)s" % locals()
     else:
         args = "-Xmx%(memory)sg -d%(arch)s -Djava.library.path=%(lib)s -Dplugins.dir=%(plugins_dir)s -cp %(jdkLib)s/*:%(imagej_home)s/*:%(javaLib)s/* %(appName)s %(appArgs)s" % locals()
 
     return args
 
 
@@ -301,17 +315,18 @@
     try:
         chimeraPlugin = Config.getDomain().importFromPlugin('chimera', 'Plugin', doRaise=True)
         env["CHIMERA_LAUNCHER"] = chimeraPlugin.getProgram() + " %s"
     except Exception as e:
         pass
 
     args = getJavaIJappArguments(memory, appName, args)
-    print('java %s' % args)
-    # return subprocess.Popen('java ' + args, shell=True, env=env)
-    cmd = ['java'] + shlex.split(args)
+    javaBin = getJavaBin()
+    logger.info('%s %s' % (javaBin, args))
+    cmd = [javaBin] + shlex.split(args)
+
     return subprocess.Popen(cmd, env=env)
 
 
 def launchSupervisedPickerGUI(micsFn, outputDir, protocol,
                               mode=None, memory=None,
                               pickerProps=None, inTmpFolder=False):
     app = "xmipp.viewer.particlepicker.training.SupervisedPickerRunner"
```

### Comparing `scipion-em-3.0.9/pwem/viewers/viewer_base.py` & `scipion-em-3.1.0/pwem/viewers/viewer_base.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.0.9/pwem/viewers/viewer_chimera.py` & `scipion-em-3.1.0/pwem/viewers/viewer_chimera.py`

 * *Files 7% similar despite different names*

```diff
@@ -22,24 +22,23 @@
 # *
 # *  All comments concerning this program package may be sent to the
 # *  e-mail address 'scipion@cnb.csic.es'
 # *
 # **************************************************************************
 
 import os
-from multiprocessing.connection import Client
-import threading
 
 import pyworkflow.utils as pwutils
 import pyworkflow.viewer as pwviewer
 import pwem.constants as emcts
 import pwem.emlib.metadata as md
 import pwem.objects as emobj
 from pwem import emlib
 from pwem import Config as emConfig
+from pwem.objects import SetOfAtomStructs
 
 chimeraPdbTemplateFileName = "Atom_struct__%06d.cif"
 chimeraMapTemplateFileName = "Map__%06d.mrc"
 chimeraScriptFileName = "chimeraScript.cxc"
 chimeraConfigFileName = "chimera.ini"
 sessionFile = "SESSION.cxs"
 
@@ -80,15 +79,20 @@
     @classmethod
     def getSymmetry(cls, scipionSym):
         """ Return the equivalent Chimera symmetry from Scipion one. """
         return cls._symmetryMap[scipionSym]
 
     @classmethod
     def getHome(cls):
-        return emConfig.CHIMERA_HOME
+        """ Returns chimera home, trying first to take it from chimera plugin. If it fails it will return, the default value in the config"""
+        with pwutils.weakImport("chimera"):
+            from chimera import Plugin as chimeraPlugin
+            return chimeraPlugin.getHome()
+
+        return os.path.join(emConfig.EM_ROOT, 'chimerax-1.2.5')
 
     @classmethod
     def getEnviron(cls):
         """ Return the proper environ to launch chimera.
         CHIMERA_HOME variable is read from the ~/.config/scipion.conf file.
         """
         environ = pwutils.Environ(os.environ)
@@ -127,33 +131,27 @@
         arrowDict = {}
         arrowDict["x"] = arrowDict["y"] = arrowDict["z"] = \
             sampling * dim * 1. / 2.
         arrowDict["r1"] = r1 * dim / 50.
         arrowDict["r2"] = 2 * arrowDict["r1"]
         arrowDict["rho"] = 0.75  # axis thickness
 
-        ff.write(".color 1 0 0\n"
+        ff.write(".color red\n" # red
                  ".arrow 0 0 0 %(x)f 0 0 %(r1)f %(r2)f %(rho)f\n"
                  ".color 0 0 0\n.sphere -%(x)f 0 0 0.00001\n"
-                 ".color 1 1 0\n"
+                 ".color yellow\n" # yellow
                  ".arrow 0 0 0 0 %(y)f 0 %(r1)f %(r2)f %(rho)f\n"
                  ".color 0 0 0\n.sphere 0 -%(y)f 0 0.00001\n"
-                 ".color 0 0 1\n"
+                 ".color blue\n"
                  ".arrow 0 0 0 0 0 %(z)f %(r1)f %(r2)f %(rho)f\n"
                  ".color 0 0 0\n.sphere 0 0 -%(z)f 0.00001\n" %
                  arrowDict)
         ff.close()
 
 
-def printCmd(cmd):
-    """ Debug function. """
-    pass
-    # print cmd
-
-
 class ChimeraAngDist(pwviewer.CommandView):
 
     def __init__(self, volFile, tmpFilesPath, **kwargs):
         self.kwargs = kwargs
         self.volfile = os.path.abspath(os.path.join(volFile))
         self.cmdFile = os.path.join(tmpFilesPath,
                                     "chimera_angular_distribution.cxc")
@@ -204,14 +202,15 @@
             fhCmd.write("open %s format %s\n" % (self.volfile.replace(":mrc", ""),
                                                  format))
         else:
             fhCmd.write("open %s\n" % self.volfile.replace(":mrc", ""))
         fhCmd.write("volume #3 voxelSize %s\n" % self.voxelSize)
         x, y, z = self.volOrigin
         fhCmd.write("volume #3 origin %s,%s,%s\n" % (x, y, z))
+        fhCmd.write("view\n")
 
         fhCmd.close()
 
     def createAngularDistributionFile(self, bildFileName="/tmp/spheres.bild"):
         ff = open(bildFileName, "w")
 
         for angulardist in self.angularDistributionList:
@@ -280,99 +279,141 @@
                        (x, y, z, radius))
             self.angularDistributionList.append(command)
 
 
 class ChimeraView(pwviewer.CommandView):
     """ View for calling an external command. """
 
-    def __init__(self, inputFile, **kwargs):
-        program = Chimera.getProgram()
-        inputFile = inputFile.replace(":mrc", "")
-        pwviewer.CommandView.__init__(self, '%s "%s" &' % (program, inputFile),
-                                      env=Chimera.getEnviron(), **kwargs)
+    def getProgram(self):
+        return Chimera.getProgram()
 
+    def getEnviron(self):
+        return Chimera.getEnviron()
 
-class ChimeraClientView(ChimeraView):
-    """ View for calling an external command. """
-    pass
+    def __init__(self, inputFiles, **kwargs):
 
+        if isinstance(inputFiles,str):
+            inputFiles = [inputFiles]
 
-class ChimeraDataView(ChimeraView):
-
-    def __init__(self, dataview, vol, viewParams={}, **kwargs):
-        self.dataview = dataview
-        ChimeraClientView.__init__(self, vol.getFileName())
-
-    def show(self):
-        self.dataview.show()
-        ChimeraClientView.show(self)
+        program = self.getProgram()
 
+        # Join files
+        filesStr = '" "'.join(inputFiles)
+        filesStr = filesStr.replace(":mrc", "")
+        pwviewer.CommandView.__init__(self, '%s "%s" &' % (program, filesStr),
+                                      env=self.getEnviron(), **kwargs)
 
 class ChimeraViewer(pwviewer.Viewer):
     """ Wrapper to visualize PDB object with Chimera. """
     _environments = [pwviewer.DESKTOP_TKINTER]
-    _targets = [emobj.AtomStruct, emobj.PdbFile]
+    _targets = [emobj.AtomStruct, emobj.PdbFile, emobj.SetOfAtomStructs,
+                emobj.Volume, emobj.SetOfVolumes, emobj.SetOfClasses3D]
+
+    _name = "ChimeraX"
 
     def __init__(self, **kwargs):
         pwviewer.Viewer.__init__(self, **kwargs)
 
-    def visualize(self, obj, **kwargs):
+    def _visualize(self, obj, **kwargs):
         cls = type(obj)
         if issubclass(cls, emobj.AtomStruct):
-            # if attribute _chimeraScript exists then protocol
-            # has create a script file USE IT
+            objSet = SetOfAtomStructs.create(outputPath='/tmp', suffix=self.protocol.getObjId())
+            objSet.append(obj)
+            if hasattr(obj, '_chimeraScript'):
+                objSet.copyAttributes(obj, '_chimeraScript')
+
+            obj, cls = objSet, type(objSet)
+
+        if issubclass(cls, emobj.SetOfAtomStructs):
             if hasattr(obj, '_chimeraScript'):
                 fn = obj._chimeraScript.get()
-                ChimeraView(fn).show()
-                return
-            # if not create a script file with: coordinates axis, PDB and
-            # volume (if available)
+                view = ChimeraView(fn)
+                return [view]
             else:
-                fn = obj.getFileName()
-                extraPath = self.protocol._getExtraPath()
-                fnCmd = os.path.join(extraPath, "chimera.cxc")
+                fnCmd = self.protocol._getExtraPath("chimera_output.cxc")
+
                 f = open(fnCmd, 'w')
+                f.write('cd %s\n' % os.getcwd())
                 f.write("cofr 0,0,0\n")  # set center of coordinates
-                if obj.hasVolume():
+                f.write("style stick\n")
+
+                _inputVol = obj.getFirstItem().getVolume()
+                if _inputVol is not None:
                     volID = 1
-                    volumeObject = obj.getVolume()
-                    dim = volumeObject.getDim()[0]
-                    sampling = volumeObject.getSamplingRate()
-                    f.write("open %s\n" % os.path.abspath(
-                        emlib.image.ImageHandler.removeFileType(volumeObject.getFileName())))
-                    f.write("volume #%d style surface voxelSize %f\n"
-                            % (volID, sampling))
-                    x, y, z = volumeObject.getShiftsFromOrigin()
-                    f.write("volume #%d origin %0.2f,%0.2f,%0.2f\n"
-                            % (volID, x, y, z))
+                    dim, sampling = _inputVol.getDim()[0], _inputVol.getSamplingRate()
+
+                    f.write("open %s\n" % _inputVol.getFileName())
+                    x, y, z = _inputVol.getOrigin(force=True).getShifts()
+                    f.write("volume #%d style surface voxelSize %f\nvolume #%d origin "
+                            "%0.2f,%0.2f,%0.2f\n"
+                            % (volID, sampling, volID, x, y, z))
                 else:
-                    dim = 150  # eventually we will create a PDB library that
-                    # computes PDB dim
-                    sampling = 1.
-                # Construct the coordinate file
-                bildFileName = os.path.abspath(
-                    os.path.join(extraPath, "axis.bild"))
-                Chimera.createCoordinateAxisFile(dim,
-                                                 bildFileName=bildFileName,
-                                                 sampling=sampling)
+                    dim, sampling = 150., 1.
+
+                bildFileName = self.protocol._getExtraPath("axis_output.bild")
+                Chimera.createCoordinateAxisFile(dim, bildFileName=bildFileName, sampling=sampling)
                 f.write("open %s\n" % bildFileName)
-                f.write("open %s\n" % os.path.abspath(fn))
-                f.write("style stick")
+
+                for AS in obj:
+                    f.write("open %s\n" % AS.getFileName())
+                    #f.write("style stick\n")
+
                 f.close()
-                ChimeraView(fnCmd).show()
-            # FIXME: there is an asymmetry between ProtocolViewer and Viewer
-            # for the first, the visualize method return a list of View's
-            # (that are shown)
-            # for the second, the visualize directly shows the objects.
-            # the first approach is better
+                view = ChimeraView(fnCmd)
+                return [view]
+
+        elif issubclass(cls,emobj.Volume):
+            view = ChimeraView(obj.getFileName())
+            return [view]
+
+        elif issubclass(cls,emobj.EMSet):
+            files = obj.getFiles()
+            view = ChimeraView(files)
+            return [view]
+
         else:
             raise Exception('ChimeraViewer.visualize: '
                             'can not visualize class: %s' % obj.getClassName())
 
 
+class ChimeraOldView(ChimeraView):
+    """ View for calling an external command. """
+
+    def getProgram(self):
+        return emConfig.CHIMERA_OLD_BINARY_PATH
+
+    def getEnviron(self):
+        return None
+
+class ChimeraOldViewer(ChimeraViewer):
+    """ Wrapper to visualize Chimera OLD (1.10 , 1.13, ..) compatible objects . """
+    _name = "Chimera"
+
+    def __init__(self, **kwargs):
+        pwviewer.Viewer.__init__(self, **kwargs)
+
+    def _visualize(self, obj, **kwargs):
+        cls = type(obj)
+
+        if issubclass(cls, emobj.EMSet):
+
+            files = obj.getFiles()
+            view = ChimeraOldView(files)
+            return [view]
+
+        elif issubclass(cls, (emobj.Volume, emobj.AtomStruct)):
+            view = ChimeraOldView(obj.getFileName())
+            return [view]
+
+        else:
+            raise Exception('ChimeraOldViewer.visualize: '
+                            'can not visualize class: %s' % obj.getClassName())
+
+
+
 def mapVolsWithColorkey(displayVolFileName,
                         mapVolFileName,
                         stepColors,  # List with resolution values
                         colorList,  # List with colors
                         voldim,  # pixels
                         volOrigin=None,  # in A.
                         step=-1,  # chimera volume step (display resolution)
@@ -383,17 +424,14 @@
                         fontSize=12):  # default chimera font size
     """ colors surface of volume 'displayVolFileName' using values from
     'mapVolFikeName'. A colorkey is created using the values in stepColors
     and the color in colorList. """
     scriptFile = scriptFileName
     fhCmd = open(scriptFile, 'w')
     fhCmd.write("from chimerax.core.commands import run\n")
-    fhCmd.write("from chimerax.graphics.windowsize import window_size\n")
-    fhCmd.write("from PyQt5.QtGui import QFontMetrics\n")
-    fhCmd.write("from PyQt5.QtGui import QFont\n")
     fhCmd.write("run(session, 'set bgColor %s')\n" % bgColorImage)
 
     chimeraVolId = 1
 
     bildFileName = scriptFile.replace(".py", ".bild")
     Chimera.createCoordinateAxisFile(voldim[0],
                                      bildFileName=bildFileName,
@@ -442,39 +480,33 @@
     for step, color in zip(stepColors, colorList):
         scolorStr += '%s,%s:' % (step, color)
     scolorStr = scolorStr[:-1]
     fhCmd.write("run(session, 'color sample #%d map #%d "
                 "palette " % (chimeraVolId - 1, chimeraVolId) +
                 scolorStr + "')\n"
                 )
-    # get window size so we can place labels properly
+    fhCmd.write(generateColorLegend(stepColors, colorList, threeLabelsOnly=False))
+    fhCmd.write("run(session, 'view')\n")
+    fhCmd.close()
+
+
+def generateColorLegend(stepColors, colorList, threeLabelsOnly=True):
+    """Return a string to write in a chimera script file a color legend - key command
 
-    fhCmd.write("v = session.main_view\n")
-    fhCmd.write("vx,vy=v.window_size\n")
+    :param stepColors: list with the values for the colors
+    :param colorList: list with the colors
+    :param threeLabelsOnly: True, with ignore stepColors and show just 3 values: min, max and medium."""
+
+    colorStr = 'run(session, "key{} fontSize 15 size 0.025,0.4 pos 0.01,0.3")\n'
+    labelCount, keyStr = 0, ''
+    stepColors.reverse(), colorList.reverse()
+    if threeLabelsOnly:
+        labelsIndex = [0, len(colorList) - 1, (len(colorList) - 1) // 2]
 
-    # Calculate heights and Y positions: font, scale height and firstY
-    ptSize = fontSize  # default size chimera font
-    fhCmd.write('font = QFont("Ariel", %d)\n' % ptSize)
-    fhCmd.write('f = QFontMetrics(font)\n')
-    fhCmd.write('_height =  1 * f.height()/vy\n')  # Font height
-    fhCmd.write('_half_scale_height = _height * %f/2\n' % len(stepColors))  # Full height of the scale
-    fhCmd.write("_firstY= 0.5 + _half_scale_height\n")  # Y location for first label
-
-    fhCmd.write("step = ")
-    # place labels in right place
-    # unfortunately chimera has no colorbar
-    labelCount = 0
     for step, color in zip(stepColors, colorList):
-        if step > 99.9:
-            step = "%.2f" % step
-        else:
-            step = "{:05.2f}".format(step)
-        command = 'run(session, "2dlabel text ' + step + \
-                  ' bgColor ' + color + \
-                  ' xpos 0.01 ypos %f' + \
-                  ' size ' + str(ptSize) + \
-                  '" % ' + \
-                  '(_firstY - %f*_height))\n' % (labelCount)
+      if not threeLabelsOnly or labelCount in labelsIndex:
+          keyStr += ' {}:{}'.format(color, step)
+      else:
+          keyStr += ' {}:'.format(color)
 
-        fhCmd.write(command)
-        labelCount += 1
-    fhCmd.close()
+      labelCount += 1
+    return colorStr.format(keyStr)
```

### Comparing `scipion-em-3.0.9/pwem/viewers/viewer_fsc.py` & `scipion-em-3.1.0/pwem/viewers/viewer_fsc.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,16 +24,16 @@
 # *  e-mail address 'scipion@cnb.csic.es'
 # *
 # **************************************************************************
 
 from matplotlib.ticker import FuncFormatter
 from matplotlib.widgets import Button
 
+from pyworkflow import Config
 import pyworkflow.viewer as pwviewer
-import pyworkflow.utils as pwutils
 
 import pwem.objects as emobj
 import pwem.protocols as emprot
 
 from .plotter import EmPlotter, plt
 
 
@@ -67,15 +67,15 @@
             # Button does not allow to define text color so
             # I write it directly
             axcreateFSC.text(0.5, 0.5, 'create FSC',
                              verticalalignment='center',
                              horizontalalignment='center',
                              transform=axcreateFSC.transAxes, color='white')
             bcreateFSC = Button(axcreateFSC, '',  # leave label empty
-                                color=pwutils.Color.RED_COLOR,
+                                color=Config.SCIPION_MAIN_COLOR,
                                 hovercolor='maroon')
             bcreateFSC.on_clicked(self.createFSCObject)
             self._addButton = False
             return bcreateFSC
 
     def visualize(self, obj, **kwargs):
         # Keep input object in case we need to launch
@@ -83,15 +83,16 @@
         self.fscList = []
         if isinstance(obj, emobj.SetOfFSCs):
             for i, fsc in enumerate(obj):
                 self.fscList.append(fsc.clone())
                 fscLabel = fsc.getObjLabel() or 'FSC %d' % (i + 1)
                 self.plotFsc(fsc, label=fscLabel, **kwargs)
         else:  # single FSC
-            self.plotFsc(obj, **kwargs)
+            fscLabel = obj.getObjLabel() or 'FSC 1'
+            self.plotFsc(obj, label=fscLabel, **kwargs)
             self.fscList.append(obj.clone())
 
         bcreateFSC = self._plotButton()  # if you do not assign the result
         # to something it will be
         # delete
         self.show()
         # return [self.plotter]
@@ -113,12 +114,12 @@
             a.set_ylim([-0.1, 1.1])
             a.plot([0, x[-1]],
                    [self.threshold, self.threshold],
                    'k--')
             a.grid(True)
             a.xaxis.set_major_formatter(FuncFormatter(self._formatFreq))
             self._lastSubPlot = a
-
-        self.label = kwargs.get('label', self.protocol.getRunName())
+        resolution = obj.calculateResolution(self.threshold)
+        self.label = kwargs.get('label', self.protocol.getRunName()) + " (" + str(resolution) + "Å)"
         self.plotter.plotData(x, y, '-', label=self.label)
         self.plotter.legend()
         # if I run this
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `scipion-em-3.0.9/pwem/viewers/viewer_pdf.py` & `scipion-em-3.1.0/pwem/viewers/viewer_pdf.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.0.9/pwem/viewers/viewer_sequence.py` & `scipion-em-3.1.0/pwem/viewers/viewer_sequence.py`

 * *Files 5% similar despite different names*

```diff
@@ -51,22 +51,26 @@
         # SequenceHandler that requires a Biopython sequence (Bio.Seq.Seq
         # object);
 
         # Step 1: transformation of the sequence of our Scipion Sequence
         # object (obj.getSequence()) in a Biopython Sequence:
         # Let keep the SequenceHandler import here to avoid a default BioPython
         # import
-        seqHandler = emconv.SequenceHandler(obj.getSequence(),
-                                            isAminoacid=obj.getIsAminoacids())
+        seqHandler = emconv.SequenceHandler(obj.getSequence())
         seqBio = seqHandler._sequence  # Bio.Seq.Seq object
         # Step 2: retrieving of the other args needed in the saveFile method
-        seqID = obj.getId()
-        seqName = obj.getSeqName()
-        seqDescription = obj.getDescription()
-        seqFileName = os.path.abspath(
-            self.protocol._getExtraPath(seqName + ".fasta"))
+        seqID = obj.getId() if obj.getId() is not None else 'seqID'
+        seqName = obj.getSeqName() if obj.getSeqName() is not None else 'sequence'
+        seqDescription = obj.getDescription() if obj.getDescription() is not None else ''
+        # check if protocol has created directory extructura, if not use /tmp
+        extraDir = self.protocol._getExtraPath() 
+        if os.path.isdir(extraDir):
+            seqFileName = os.path.abspath(
+                self.protocol._getExtraPath(seqName + ".fasta"))
+        else:
+            seqFileName = os.path.abspath(os.path.join("/tmp", seqName + ".fasta"))
         # Step 3: Sequence saved in the extra file
         seqHandler.saveFile(seqFileName, seqID, sequence=seqBio,
                             name=seqName, seqDescription=seqDescription,
                             type="fasta")
         # Step 4: Visualization of extra file
         openTextFileEditor(seqFileName)
```

### Comparing `scipion-em-3.0.9/pwem/viewers/viewer_vmd.py` & `scipion-em-3.1.0/pwem/viewers/viewer_vmd.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.0.9/pwem/viewers/viewers_data.py` & `scipion-em-3.1.0/pwem/viewers/viewers_data.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,54 +34,96 @@
 import pwem.objects as emobj
 import pwem.protocols as emprot
 
 from .views import (ObjectView, MicrographsView, CoordinatesObjectView,
                     ClassesView, Classes3DView, CtfView, DataView)
 from .showj import (RENDER, SAMPLINGRATE, ORDER, VISIBLE, MODE, MODE_MD,
                     SORT_BY, getJvmMaxMemory, launchTiltPairPickerGUI)
+from ..convert.headers import Ccp4Header
 
 
 class DataViewer(pwviewer.Viewer):
     """ Wrapper to visualize different type of objects
     with the Xmipp program xmipp_showj
     """
+    _name = "Xmipp metadata viewer"
     _environments = [pwviewer.DESKTOP_TKINTER, pwviewer.WEB_DJANGO]
     _targets = [
         emobj.Image,
         emobj.SetOfClasses2D,
         emobj.SetOfClasses3D,
         emobj.SetOfCoordinates,
         emobj.SetOfCTF,
-        emobj.SetOfImages,
+        emobj.SetOfParticles,
         emobj.SetOfMovies,
         emobj.SetOfNormalModes,
+        emobj.SetOfPrincipalComponents,
         emobj.SetOfPDBs,
+        emobj.SetOfAtomStructs,
         emprot.ProtParticlePicking,
         emprot.ProtImportMovies,
         # TiltPairs related data
         emobj.CoordinatesTiltPair,
         emobj.MicrographsTiltPair,
-        emobj.ParticlesTiltPair
+        emobj.ParticlesTiltPair,
+        emobj.SetOfImages,
     ]
+    _configRegistry = dict() # Extra configuration for specific types not in this plugin (e.g.: Tomo objects)
+
+    @classmethod
+    def registerConfig(cls, type, config=None):
+        """
+        Allow registration of other objects
+        :param type: Class to register --> SetOfXXX
+        :param config: Optional, dictionary with the fields configuration, otherwise all fields will be shown.
+
+        :return: Nothing
+
+        """
+        cls._targets.append(type)
+
+        if config is None:
+            config = {MODE: MODE_MD}
+
+        cls._configRegistry[type]=config
 
     def __init__(self, **kwargs):
         pwviewer.Viewer.__init__(self, **kwargs)
         self._views = []
 
     def _addObjView(self, obj, fn, viewParams={}):
         objView = ObjectView(self._project, obj.strId(), fn,
                              viewParams=viewParams)
         self._views.append(objView)
         return objView
 
     def _visualize(self, obj, **kwargs):
         cls = type(obj)
 
+        # Try registry first
+        config = self._configRegistry.get(cls, None)
+
+        if config is not None:
+            fn = obj.getFileName()
+            self._addObjView(obj, fn, config)
+            return self._views
+
         if issubclass(cls, emobj.Volume):
             fn = emlib.image.ImageHandler.locationToXmipp(obj)
+
+            if fn.endswith(':mrc'):
+                # fn may came in the form of 000001@Runs/..../vol.mrc". We need to pass an actual file to Ccp4Header
+                actualFile = fn.split("@")[-1]
+                ccp4header = Ccp4Header(actualFile, readHeader=True)
+                if ccp4header.getISPG() == 1:
+                    fn = fn.replace(':mrc', '')
+                else:
+                    print('Developers warning: %s headers do not match the standard for volumes. '
+                          'You can use fixVolume(pwem.convert.headers.py) '
+                          'method to fix the headers' % fn)
             self._addObjView(obj, fn,
                              {RENDER: 'image',
                               SAMPLINGRATE: obj.getSamplingRate()})
 
         elif issubclass(cls, emobj.Image):
             fn = emlib.image.ImageHandler.locationToXmipp(obj)
             self._addObjView(obj, fn)
@@ -215,8 +257,14 @@
             movs = obj.outputMovies
             self._visualize(movs)
             gainFn = movs.getGain()
             if gainFn is not None:
                 if os.path.exists(gainFn):
                     self._views.append(DataView(gainFn))
 
+        elif issubclass(cls, emobj.SetOfNormalModes):
+            self._views.append(DataView(obj.getFileName()))
+
+        elif issubclass(cls, emobj.EMSet):
+            self._views.append(DataView(obj.getFileName()))
+
         return self._views
```

### Comparing `scipion-em-3.0.9/pwem/viewers/viewers_protocols.py` & `scipion-em-3.1.0/pwem/viewers/viewers_protocols.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.0.9/pwem/viewers/views.py` & `scipion-em-3.1.0/pwem/viewers/views.py`

 * *Files identical despite different names*

### Comparing `scipion-em-3.0.9/pwem/wizards/__init__.py` & `scipion-em-3.1.0/pwem/wizards/wizards_3d/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # **************************************************************************
 # *
-# * Authors: Yunior C. Fonseca Reyna    (cfonseca@cnb.csic.es)
+# * Authors: David Herreros Calero    (dherreros@cnb.csic.es)
 # *
 # *
 # * Unidad de  Bioinformatica of Centro Nacional de Biotecnologia , CSIC
 # *
 # * This program is free software; you can redistribute it and/or modify
 # * it under the terms of the GNU General Public License as published by
 # * the Free Software Foundation; either version 3 of the License, or
@@ -21,9 +21,10 @@
 # * 02111-1307  USA
 # *
 # *  All comments concerning this program package may be sent to the
 # *  e-mail address 'scipion@cnb.csic.es'
 # *
 # **************************************************************************
 
-from .wizard import *
-from .wizards import *
+from .mask_volume_wizard import *
+from .mask_structure_wizard import *
+from .callbacks import *
```

### Comparing `scipion-em-3.0.9/pwem/wizards/wizard.py` & `scipion-em-3.1.0/pwem/wizards/wizard.py`

 * *Files 13% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 import pyworkflow as pw
 import pyworkflow.object as pwobj
 import pyworkflow.wizard as pwizard
 import pyworkflow.gui.dialog as dialog
 from matplotlib import cm
 from pwem import convertPixToLength, splitRange
 from pyworkflow.gui.plotter import getHexColorList
-from pyworkflow.gui.tree import BoundTree, ListTreeProvider
+from pyworkflow.gui.tree import BoundTree, ListTreeProvider, ListTreeProviderString, AttributesTreeProvider
 from pyworkflow.gui.widgets import LabelSlider, ExplanationText
 
 import pwem.constants as emcts
 import pwem.objects as emobj
 from pwem import emlib
 from pyworkflow.protocol import IntParam, StringParam, FloatParam, LEVEL_ADVANCED
 
@@ -135,14 +135,63 @@
             return label[0], value[0]
 
 
 # ===============================================================================
 #    Wizards base classes
 # ===============================================================================
 
+class VariableWizard(pwizard.Wizard):
+    """Wizard base class object where input and output paramNames can be modified and added, so
+    one wizard can be used in several protocols with parameters of different names"""
+    #Variables _targets, _inputs and _outputs must be created in sons
+    # _targets, _inputs, _outputs = [], {}, {}
+
+    def addTarget(self, protocol, targets, inputs, outputs):
+        '''Add a target to a wizard and the input and output parameters are stored in a dictionary with
+        (protocol, targetParamName) as key.
+        Targets must be added one by one.'''
+        self._targets += [(protocol, targets)]
+        self._inputs.update({(protocol, targets[0]): inputs})
+        self._outputs.update({(protocol, targets[0]): outputs})
+
+    def getInputOutput(self, form):
+        '''Retrieving input and output paramNames corresponding to the protocol and target of the wizard clicked'''
+        outParam = ''
+        for target in self._targets:
+            if form.wizParamName == target[1][0] and form.protocol.__class__ == target[0]:
+                prot, target = (target[0], target[1][0])
+                inParams, outParam = self._inputs[(prot, target)], self._outputs[(prot, target)]
+                inParams = self.filterPresentInputs(inParams, form.protocol)
+        return inParams, outParam
+
+    def filterPresentInputs(self, inputParams, protocol):
+        '''Filter the inputs to allow flexibility:
+        1) InputParams can be lists: the first not None parameter of the list will be chosen.
+        2) InputParams can be dict: key -> EnumParam (or IntParam) which functions as index
+                                    value -> list containing paramNames. The hey index element will be chosen
+        '''
+        fInpParams = []
+        for inPar in inputParams:
+            if type(inPar) == list:
+                present = ''
+                for option in inPar:
+                    if getattr(protocol, option).get():
+                        present = option
+                        break
+                fInpParams.append(present)
+            elif type(inPar) == dict:
+                idxParam = list(inPar.keys())[0]
+                optionParams = inPar[idxParam]
+
+                idx = getattr(protocol, idxParam).get()
+                fInpParams.append(optionParams[idx])
+            else:
+                fInpParams.append(inPar)
+        return fInpParams
+
 class DownsampleWizard(EmWizard):
 
     def show(self, form, value, label, units=emcts.UNIT_PIXEL):
         protocol = form.protocol
         provider = self._getProvider(protocol)
 
         if provider is not None:
@@ -1306,7 +1355,127 @@
         """ Select all the text of the widget that triggered the event"""
         # select text
         event.widget.select_range(0, 'end')
         # move cursor to the end
         event.widget.icursor('end')
         # stop propagation
         # return 'break'
+
+
+class FormulaDialog(dialog.Dialog):
+    """ This will assist users to create a formula based on class attibutes.
+    """
+
+    def __init__(self, parentWindow, set, formula=""):
+        """
+            :param set: set with the items to use in the formulae
+            :param formula: initial formulate to load
+        """
+        self.set = set
+        self.item = set.getFirstItem()
+        self.formula = tk.StringVar(value=formula)
+        self.formula.trace("w", self.evaluateFormula)
+        self.formulaTxt = None # To be instantiated later.
+        self.info = tk.StringVar()
+        dialog.Dialog.__init__(self, parentWindow, "Formula wizard", default="None")
+
+
+    # Getters
+    def getFormula(self):
+        return self.formula.get()
+
+    def getItem(self):
+        return self.item
+
+    ### ----- GUI methods ------ ###
+    def _createTree(self, parent):
+        provider = AttributesTreeProvider(self.item)
+        self.tree = BoundTree(parent, provider)
+        self.tree.itemDoubleClick = self.addAttributeToFormula
+        self.tree.grid(row=1, column=0)
+
+    def addAttributeToFormula(self, event):
+        attr = self.tree.getSelectedObjects()[0]
+        self._insertText("item." + attr.attrName , self.formulaTxt)
+
+    def body(self, master):
+        """ Draws the main frame of the dialog"""
+        body = tk.Frame(self)
+        body.grid(row=0, column=0, sticky="news")
+        body.grid_columnconfigure(1, weight=10)
+
+        # GUI attributes
+        self.attributes = tk.Frame(body)
+        self.attributes.grid(row=0, column=0, sticky='nes',
+                          padx=5, pady=5)
+
+        # Formula
+        self.formulaFrame = tk.Frame(body)
+        self.formulaFrame.grid(row=0, column=1, sticky='news',
+                         padx=5, pady=5)
+        #self.params.bind("<Key>", self._keyPressedOnParams)
+
+        self._fillParams()
+
+
+    def _fillParams(self):
+
+        # Add the formula text
+        formulaLbl = tk.Label(self.formulaFrame, text="Formula:")
+        formulaLbl.grid(row=0, column=0, sticky="w")
+        self.formulaTxt = self._addEntry(1, 0, self.formula,  width=100)
+
+        self._createTree(self.attributes)
+
+        # Label to show formula result or error
+        infoLabel = tk.Label(self.formulaFrame, textvariable=self.info)
+        infoLabel.grid(row=2, column=0, columnspan=2, sticky="news")
+
+    def _addEntry(self, row, column, var, width=None):
+
+        newEntry = tk.Entry(self.formulaFrame, textvariable=var, width=width)
+        newEntry.grid(row=row, column=column, sticky="news")
+        newEntry.lift()
+        # Bind events
+        newEntry.bind("<Return>", self._paramChanged)
+        newEntry.bind("<FocusOut>", self._paramChanged)
+
+        return newEntry
+
+    def evaluateFormula(self, name='', index='', mode=''):
+        try:
+            item = self.item
+            result = eval(self.formula.get())
+            self.info.set(result)
+        except Exception as e:
+            self.info.set(str(e))
+
+    ### Events handling
+    def _paramChanged(self, event):
+        # Handles change in palette Option
+        self.evaluateFormula()
+
+    def _selectAllText(self, event):
+        """ Select all the text of the widget that triggered the event"""
+        # select text
+        event.widget.select_range(0, 'end')
+        # move cursor to the end
+        event.widget.icursor('end')
+        # stop propagation
+        # return 'break'
+
+    def _insertText(self, text, widget):
+        """ Insert the passed text in the entry at current cursor location"""
+        # Get inserting position
+        pos = widget.index(tk.INSERT)
+
+        # Insert he text
+        widget.insert(pos, text)
+
+def insertText (target, textToInsert, position):
+    """ Inserts a text into another at a position
+
+    :param target: text to do the insertion on
+    :param textToInsert: text to be inserted
+    :param position: position where to insert the new text"""
+
+    return target[:position] + textToInsert + target[position:]
```

### Comparing `scipion-em-3.0.9/scipion_em.egg-info/PKG-INFO` & `scipion-em-3.1.0/scipion_em.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,60 +1,62 @@
 Metadata-Version: 1.1
 Name: scipion-em
-Version: 3.0.9
+Version: 3.1.0
 Summary: This modules contains classes related with EM
 Home-page: https://github.com/scipion-em/scipion-em
 Author: J.M. De la Rosa Trevin, Roberto Marabini, Grigory Sharov, Josue Gomez Blanco, Pablo Conesa, Yunior Fonseca Reyna
 Author-email: delarosatrevin@scilifelab.se, roberto@cnb.csic.es, gsharov@mrc-lmb.cam.ac.uk, josue.gomez-blanco@mcgill.ca, pconesa@cnb.csic.es, fonsecareyna@cnb.csic.es
 License: UNKNOWN
-Description: ====
+Description: .. image:: https://img.shields.io/badge/Contributor%20Covenant-v2.0%20adopted-ff69b4.svg
+          :width: 200
+          :alt: Contributor Covenant
+          :target: https://www.contributor-covenant.org/version/2/0/code_of_conduct/
+        
+        
         pwem
         ====
         
         **pwem** is a Python module of Scipion framework for image processing in Electron Microscopy
         
-        
         The entire collection is licensed under the terms of the GNU Public License,
         version 3 (GPLv3).
         
-        -------------
         Development
-        -------------
+        -----------
         
         To install **pwem** for development purposes, one can do:
         
-        ::
+        .. code-block:: bash
         
             # Create a clean virtual environment
-            python -m venv ~/myenv
-            source ~/myenv/bin/activate
-            git clone git@github.com:scipion-em/scipion-em.git
+            conda create -n scipion python=3.8
+            conda activate
+            git clone https://github.com/scipion-em/scipion-em.git
             cd scipion-em
-            python -m pip install -e .  # Install in the environment as development
+            pip install -e .
         
-        -------------
         Running tests
         -------------
         
-        First make sure that **pwem** is available as a Python module in your
-        current Python environment. During development, I tend to set the PYTHONPATH:
-        
-        ::
+        .. code-block:: bash
         
+            conda activate scipion
             cd scipion-em
-            # Either you have installed as mentioned above, or modify the PYTHONPATH
-            export PYTHONPATH=$PYTHONPATH:$PWD
-            # After pyworkflow is accessible as a module, then:
-            cd pwem/tests
-        
+            export SCIPION_DOMAIN="pwem"
             python -m unittest discover
         
+        API documentation
+        -----------------
+        
+        https://scipion-em.github.io/docs/release-3.0.0/api/pwem/pwem.html
         
 Keywords: scipion cryoem imageprocessing scipion-3.0
 Platform: UNKNOWN
-Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering
```

### Comparing `scipion-em-3.0.9/scipion_em.egg-info/SOURCES.txt` & `scipion-em-3.1.0/scipion_em.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 MANIFEST.in
 README.rst
 requirements.txt
 setup.py
 pwem/__init__.py
 pwem/bibtex.py
 pwem/constants.py
+pwem/protocols.conf
+pwem/scipion_icon.png
 pwem/utils.py
 pwem/cmd/chimera_client.py
 pwem/cmd/convert.py
 pwem/cmd/program.py
 pwem/convert/__init__.py
 pwem/convert/atom_struct.py
 pwem/convert/headers.py
@@ -33,28 +35,35 @@
 pwem/protocols/protocol.py
 pwem/protocols/protocol_2d.py
 pwem/protocols/protocol_3d.py
 pwem/protocols/protocol_align_movies.py
 pwem/protocols/protocol_alignment_assign.py
 pwem/protocols/protocol_alignment_invertHand.py
 pwem/protocols/protocol_batch.py
-pwem/protocols/protocol_classes_consensus.py
+pwem/protocols/protocol_boxsize_checkpoint.py
+pwem/protocols/protocol_boxsize_parameters.py
+pwem/protocols/protocol_classes_selector.py
 pwem/protocols/protocol_create_stream_data.py
 pwem/protocols/protocol_ctf_assign.py
 pwem/protocols/protocol_extract_coordinates.py
-pwem/protocols/protocol_metadata_editor.py
+pwem/protocols/protocol_mathematical_operator.py
 pwem/protocols/protocol_micrographs.py
+pwem/protocols/protocol_movie_eraser.py
 pwem/protocols/protocol_movies.py
 pwem/protocols/protocol_origin_sampling_volume.py
 pwem/protocols/protocol_particles.py
 pwem/protocols/protocol_particles_picking.py
 pwem/protocols/protocol_pdf_report.py
+pwem/protocols/protocol_projection_edit.py
+pwem/protocols/protocol_set_editor.py
+pwem/protocols/protocol_set_filter.py
 pwem/protocols/protocol_sets.py
 pwem/protocols/protocol_tests.py
 pwem/protocols/protocol_tiltpairs.py
+pwem/protocols/protocol_tools.py
 pwem/protocols/protocol_export/__init__.py
 pwem/protocols/protocol_export/protocol_export_DB.py
 pwem/protocols/protocol_import/__init__.py
 pwem/protocols/protocol_import/base.py
 pwem/protocols/protocol_import/coordinates.py
 pwem/protocols/protocol_import/ctfs.py
 pwem/protocols/protocol_import/dataimport.py
@@ -64,35 +73,44 @@
 pwem/protocols/protocol_import/particles.py
 pwem/protocols/protocol_import/sequence.py
 pwem/protocols/protocol_import/volumes.py
 pwem/templates/demo.json.template
 pwem/tests/__init__.py
 pwem/tests/utils.py
 pwem/tests/data/__init__.py
+pwem/tests/data/hexonAtomStruct.py
 pwem/tests/data/test_convert_atom_struct.py
 pwem/tests/data/test_data.py
 pwem/tests/data/test_metadata.py
 pwem/tests/data/test_symmetry.py
 pwem/tests/protocols/__init__.py
 pwem/tests/protocols/test_extract_particles.py
 pwem/tests/protocols/test_notifier.py
+pwem/tests/protocols/test_plugin.py
+pwem/tests/protocols/test_projection_edit.py
 pwem/tests/protocols/test_protocol_alignment_assign.py
+pwem/tests/protocols/test_protocol_boxsize_checkpoint.py
+pwem/tests/protocols/test_protocol_boxsize_parameters.py
 pwem/tests/protocols/test_protocol_export2DB.py
 pwem/tests/protocols/test_protocol_extract_coorinates.py
 pwem/tests/protocols/test_protocol_invert_Hand.py
+pwem/tests/protocols/test_protocol_mathematical_operator.py
 pwem/tests/protocols/test_protocol_volume_homogenizer.py
 pwem/tests/protocols/test_protocols_assign_orig.py
+pwem/tests/protocols/test_protocols_import_atomstruct.py
 pwem/tests/protocols/test_protocols_import_coords.py
 pwem/tests/protocols/test_protocols_import_ctfs.py
 pwem/tests/protocols/test_protocols_import_masks.py
 pwem/tests/protocols/test_protocols_import_micrographs.py
 pwem/tests/protocols/test_protocols_import_movies.py
 pwem/tests/protocols/test_protocols_import_particles.py
 pwem/tests/protocols/test_protocols_import_sequence.py
 pwem/tests/protocols/test_protocols_import_volumes.py
+pwem/tests/protocols/test_protocols_set_editor.py
+pwem/tests/protocols/test_protocols_set_filter.py
 pwem/tests/protocols/test_protocols_sets.py
 pwem/tests/workflows/__init__.py
 pwem/tests/workflows/test_parallel_gpu_queue.py
 pwem/tests/workflows/test_workflow.py
 pwem/tests/workflows/test_workflow_initialvolume.py
 pwem/tests/workflows/test_workflow_mixed.py
 pwem/tests/workflows/test_workflow_mixed_large.py
@@ -101,27 +119,32 @@
 pwem/tests/workflows/test_workflow_xmipp_assignment_tiltpairs.py
 pwem/tests/workflows/test_workflow_xmipp_ctf_consensus.py
 pwem/tests/workflows/test_workflow_xmipp_rct.py
 pwem/viewers/__init__.py
 pwem/viewers/filehandlers.py
 pwem/viewers/plotter.py
 pwem/viewers/showj.py
+pwem/viewers/viewer_angular_dist.py
 pwem/viewers/viewer_base.py
 pwem/viewers/viewer_chimera.py
 pwem/viewers/viewer_fsc.py
 pwem/viewers/viewer_localres.py
 pwem/viewers/viewer_pdf.py
 pwem/viewers/viewer_sequence.py
 pwem/viewers/viewer_vmd.py
 pwem/viewers/viewer_volumes.py
 pwem/viewers/viewers_data.py
 pwem/viewers/viewers_protocols.py
 pwem/viewers/views.py
 pwem/wizards/__init__.py
 pwem/wizards/wizard.py
 pwem/wizards/wizards.py
+pwem/wizards/wizards_3d/__init__.py
+pwem/wizards/wizards_3d/callbacks.py
+pwem/wizards/wizards_3d/mask_structure_wizard.py
+pwem/wizards/wizards_3d/mask_volume_wizard.py
 scipion_em.egg-info/PKG-INFO
 scipion_em.egg-info/SOURCES.txt
 scipion_em.egg-info/dependency_links.txt
 scipion_em.egg-info/entry_points.txt
 scipion_em.egg-info/requires.txt
 scipion_em.egg-info/top_level.txt
```

### Comparing `scipion-em-3.0.9/setup.py` & `scipion-em-3.1.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -58,34 +58,36 @@
     # For a list of valid classifiers, see
     # https://pypi.python.org/pypi?%3Aaction=list_classifiers
     classifiers=[  # Optional
         # How mature is this project? Common values are
         #   3 - Alpha
         #   4 - Beta
         #   5 - Production/Stable
-        'Development Status :: 2 - Pre-Alpha',
+        'Development Status :: 5 - Production/Stable',
         # Indicate who your project is intended for
         'Intended Audience :: Science/Research',
         # Pick your license as you wish
         'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
         # Specify the Python versions you support here. In particular, ensure
         # that you indicate whether you support Python 2, Python 3 or both.
-        'Programming Language :: Python :: 3.5',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
         'Topic :: Scientific/Engineering'
     ],
     keywords='scipion cryoem imageprocessing scipion-3.0',  # Optional
     packages=find_packages(),
     install_requires=[requirements],
     entry_points={
         'console_scripts': [
             '%s = pwem.cmd.program:main' % EM_PROGRAM_ENTRY_POINT,
             '%s = pwem.cmd.chimera_client:main' % CHIMERA_ENTRY_POINT,
             '%s = pwem.cmd.convert:main' % CONVERT_ENTRY_POINT,
         ],
         'pyworkflow.plugin': 'pwem = pwem'
     },
     package_data={
-      'pwem': ['templates/*', 'cmd/*']
+      'pwem': ['scipion_icon.png', 'protocols.conf', 'templates/*', 'cmd/*']
     }
 )
```

