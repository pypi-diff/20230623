# Comparing `tmp/stor-4.0.2.tar.gz` & `tmp/stor-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stor-4.0.2.tar", last modified: Fri Feb 12 21:11:47 2021, max compression
+gzip compressed data, was "stor-4.1.0.tar", last modified: Fri Jun 23 02:15:49 2023, max compression
```

## Comparing `stor-4.0.2.tar` & `stor-4.1.0.tar`

### file list

```diff
@@ -1,208 +1,208 @@
--rw-r--r--   0        0        0     2330 2021-02-12 21:11:43.380000 stor-4.0.2/LICENSE
--rw-r--r--   0        0        0     5295 2021-02-12 21:11:43.380000 stor-4.0.2/README.rst
--rw-r--r--   0        0        0     1585 2021-02-12 21:11:43.380000 stor-4.0.2/pyproject.toml
--rw-r--r--   0        0        0     3465 2021-02-12 21:11:43.380000 stor-4.0.2/stor/__init__.py
--rw-r--r--   0        0        0    19880 2021-02-12 21:11:43.390000 stor-4.0.2/stor/base.py
--rw-r--r--   0        0        0    18210 2021-02-12 21:11:43.390000 stor-4.0.2/stor/cli.py
--rw-r--r--   0        0        0     5065 2021-02-12 21:11:43.390000 stor-4.0.2/stor/default.cfg
--rw-r--r--   0        0        0       44 2021-02-12 21:11:43.390000 stor-4.0.2/stor/default.env
--rw-r--r--   0        0        0    52552 2021-02-12 21:11:43.390000 stor-4.0.2/stor/dx.py
--rw-r--r--   0        0        0     3339 2021-02-12 21:11:43.390000 stor-4.0.2/stor/exceptions.py
--rw-r--r--   0        0        0        0 2021-02-12 21:11:43.390000 stor-4.0.2/stor/extensions/__init__.py
--rw-r--r--   0        0        0     1328 2021-02-12 21:11:43.390000 stor-4.0.2/stor/extensions/swiftstack.py
--rw-r--r--   0        0        0    17823 2021-02-12 21:11:43.390000 stor-4.0.2/stor/obs.py
--rw-r--r--   0        0        0     1459 2021-02-12 21:11:43.390000 stor-4.0.2/stor/posix.py
--rw-r--r--   0        0        0    30893 2021-02-12 21:11:43.390000 stor-4.0.2/stor/s3.py
--rw-r--r--   0        0        0     5433 2021-02-12 21:11:43.390000 stor-4.0.2/stor/settings.py
--rw-r--r--   0        0        0      558 2021-02-12 21:11:43.390000 stor-4.0.2/stor/stor-completion.bash
--rw-r--r--   0        0        0    62780 2021-02-12 21:11:43.390000 stor-4.0.2/stor/swift.py
--rw-r--r--   0        0        0    14275 2021-02-12 21:11:43.390000 stor-4.0.2/stor/test.py
--rw-r--r--   0        0        0        0 2021-02-12 21:11:43.390000 stor-4.0.2/stor/tests/__init__.py
--rw-r--r--   0        0        0    20324 2021-02-12 21:11:43.390000 stor-4.0.2/stor/tests/cassettes_py3/TestCanonicalProject/test_canonical_path.yaml
--rw-r--r--   0        0        0     8236 2021-02-12 21:11:43.390000 stor-4.0.2/stor/tests/cassettes_py3/TestCanonicalProject/test_canonical_path_on_dir.yaml
--rw-r--r--   0        0        0     8262 2021-02-12 21:11:43.390000 stor-4.0.2/stor/tests/cassettes_py3/TestCanonicalProject/test_duplicate_projects.yaml
--rw-r--r--   0        0        0     1248 2021-02-12 21:11:43.390000 stor-4.0.2/stor/tests/cassettes_py3/TestCanonicalProject/test_no_project.yaml
--rw-r--r--   0        0        0     5682 2021-02-12 21:11:43.390000 stor-4.0.2/stor/tests/cassettes_py3/TestCanonicalProject/test_unique_project.yaml
--rw-r--r--   0        0        0    27246 2021-02-12 21:11:43.390000 stor-4.0.2/stor/tests/cassettes_py3/TestCanonicalResource/test_duplicate_resource.yaml
--rw-r--r--   0        0        0     6960 2021-02-12 21:11:43.390000 stor-4.0.2/stor/tests/cassettes_py3/TestCanonicalResource/test_no_resource.yaml
--rw-r--r--   0        0        0     4284 2021-02-12 21:11:43.390000 stor-4.0.2/stor/tests/cassettes_py3/TestCanonicalResource/test_project.yaml
--rw-r--r--   0        0        0    17075 2021-02-12 21:11:43.390000 stor-4.0.2/stor/tests/cassettes_py3/TestCanonicalResource/test_unique_resource.yaml
--rw-r--r--   0        0        0    16155 2021-02-12 21:11:43.390000 stor-4.0.2/stor/tests/cassettes_py3/TestCanonicalResource/test_virtual_on_virtual.yaml
--rw-r--r--   0        0        0    19311 2021-02-12 21:11:43.390000 stor-4.0.2/stor/tests/cassettes_py3/TestCopy/test_clone_move_project_fail.yaml
--rw-r--r--   0        0        0    32263 2021-02-12 21:11:43.390000 stor-4.0.2/stor/tests/cassettes_py3/TestCopy/test_clone_within_project_fail.yaml
--rw-r--r--   0        0        0    36334 2021-02-12 21:11:43.390000 stor-4.0.2/stor/tests/cassettes_py3/TestCopy/test_dx_canonical_to_dx_file.yaml
--rw-r--r--   0        0        0    19572 2021-02-12 21:11:43.390000 stor-4.0.2/stor/tests/cassettes_py3/TestCopy/test_dx_dir_to_posix_error.yaml
--rw-r--r--   0        0        0    78875 2021-02-12 21:11:43.390000 stor-4.0.2/stor/tests/cassettes_py3/TestCopy/test_dx_to_dx_diff_project_exist_file.yaml
--rw-r--r--   0        0        0    36267 2021-02-12 21:11:43.390000 stor-4.0.2/stor/tests/cassettes_py3/TestCopy/test_dx_to_dx_file.yaml
--rw-r--r--   0        0        0    62844 2021-02-12 21:11:43.390000 stor-4.0.2/stor/tests/cassettes_py3/TestCopy/test_dx_to_dx_file_folder_no_ext.yaml
--rw-r--r--   0        0        0    39012 2021-02-12 21:11:43.390000 stor-4.0.2/stor/tests/cassettes_py3/TestCopy/test_dx_to_dx_folder.yaml
--rw-r--r--   0        0        0    84362 2021-02-12 21:11:43.390000 stor-4.0.2/stor/tests/cassettes_py3/TestCopy/test_dx_to_dx_same_project_exist_dest.yaml
--rw-r--r--   0        0        0    23018 2021-02-12 21:11:43.390000 stor-4.0.2/stor/tests/cassettes_py3/TestCopy/test_dx_to_dx_within_project_fail.yaml
--rw-r--r--   0        0        0    66832 2021-02-12 21:11:43.390000 stor-4.0.2/stor/tests/cassettes_py3/TestCopy/test_dx_to_dx_within_project_pass.yaml
--rw-r--r--   0        0        0    18184 2021-02-12 21:11:43.390000 stor-4.0.2/stor/tests/cassettes_py3/TestCopy/test_dx_to_other_obs.yaml
--rw-r--r--   0        0        0    24022 2021-02-12 21:11:43.390000 stor-4.0.2/stor/tests/cassettes_py3/TestCopy/test_dx_to_posix_file.yaml
--rw-r--r--   0        0        0    31201 2021-02-12 21:11:43.390000 stor-4.0.2/stor/tests/cassettes_py3/TestCopy/test_dx_to_posix_file_folder_no_ext.yaml
--rw-r--r--   0        0        0    24027 2021-02-12 21:11:43.390000 stor-4.0.2/stor/tests/cassettes_py3/TestCopy/test_dx_to_posix_folder.yaml
--rw-r--r--   0        0        0    24202 2021-02-12 21:11:43.390000 stor-4.0.2/stor/tests/cassettes_py3/TestCopy/test_dx_to_same_dx_pass.yaml
--rw-r--r--   0        0        0    22069 2021-02-12 21:11:43.390000 stor-4.0.2/stor/tests/cassettes_py3/TestCopy/test_move_diff_project_fail.yaml
--rw-r--r--   0        0        0    16892 2021-02-12 21:11:43.390000 stor-4.0.2/stor/tests/cassettes_py3/TestCopy/test_other_obs_to_dx.yaml
--rw-r--r--   0        0        0    11502 2021-02-12 21:11:43.390000 stor-4.0.2/stor/tests/cassettes_py3/TestCopy/test_posix_to_dx_fail.yaml
--rw-r--r--   0        0        0    21649 2021-02-12 21:11:43.390000 stor-4.0.2/stor/tests/cassettes_py3/TestCopy/test_posix_to_dx_file.yaml
--rw-r--r--   0        0        0    47262 2021-02-12 21:11:43.390000 stor-4.0.2/stor/tests/cassettes_py3/TestCopy/test_posix_to_dx_file_folder_no_ext.yaml
--rw-r--r--   0        0        0    21622 2021-02-12 21:11:43.390000 stor-4.0.2/stor/tests/cassettes_py3/TestCopy/test_posix_to_dx_folder.yaml
--rw-r--r--   0        0        0    48364 2021-02-12 21:11:43.390000 stor-4.0.2/stor/tests/cassettes_py3/TestCopy/test_posix_to_existing_dx.yaml
--rw-r--r--   0        0        0    32339 2021-02-12 21:11:43.390000 stor-4.0.2/stor/tests/cassettes_py3/TestCopyTree/test_clonetree_within_project_fail.yaml
--rw-r--r--   0        0        0    47177 2021-02-12 21:11:43.390000 stor-4.0.2/stor/tests/cassettes_py3/TestCopyTree/test_dx_dir_to_dx_dir.yaml
--rw-r--r--   0        0        0    32151 2021-02-12 21:11:43.390000 stor-4.0.2/stor/tests/cassettes_py3/TestCopyTree/test_dx_dir_to_dx_dir_same_project.yaml
--rw-r--r--   0        0        0    35304 2021-02-12 21:11:43.390000 stor-4.0.2/stor/tests/cassettes_py3/TestCopyTree/test_dx_dir_to_dx_dir_same_project_fail.yaml
--rw-r--r--   0        0        0    48797 2021-02-12 21:11:43.390000 stor-4.0.2/stor/tests/cassettes_py3/TestCopyTree/test_dx_dir_to_dx_dir_w_slash.yaml
--rw-r--r--   0        0        0    47283 2021-02-12 21:11:43.390000 stor-4.0.2/stor/tests/cassettes_py3/TestCopyTree/test_dx_dir_to_dx_existing_dir.yaml
--rw-r--r--   0        0        0    35180 2021-02-12 21:11:43.390000 stor-4.0.2/stor/tests/cassettes_py3/TestCopyTree/test_dx_dir_to_dx_root.yaml
--rw-r--r--   0        0        0    30228 2021-02-12 21:11:43.390000 stor-4.0.2/stor/tests/cassettes_py3/TestCopyTree/test_dx_dir_to_dx_root_same_project.yaml
--rw-r--r--   0        0        0    62333 2021-02-12 21:11:43.390000 stor-4.0.2/stor/tests/cassettes_py3/TestCopyTree/test_dx_dir_to_posix.yaml
--rw-r--r--   0        0        0    17613 2021-02-12 21:11:43.390000 stor-4.0.2/stor/tests/cassettes_py3/TestCopyTree/test_dx_file_to_posix.yaml
--rw-r--r--   0        0        0    44999 2021-02-12 21:11:43.390000 stor-4.0.2/stor/tests/cassettes_py3/TestCopyTree/test_dx_root_to_dx_dir.yaml
--rw-r--r--   0        0        0    19014 2021-02-12 21:11:43.390000 stor-4.0.2/stor/tests/cassettes_py3/TestCopyTree/test_dx_root_to_dx_dir_same_project.yaml
--rw-r--r--   0        0        0    48181 2021-02-12 21:11:43.390000 stor-4.0.2/stor/tests/cassettes_py3/TestCopyTree/test_dx_root_to_dx_dir_w_slash.yaml
--rw-r--r--   0        0        0    35766 2021-02-12 21:11:43.390000 stor-4.0.2/stor/tests/cassettes_py3/TestCopyTree/test_dx_root_to_dx_root.yaml
--rw-r--r--   0        0        0    49292 2021-02-12 21:11:43.390000 stor-4.0.2/stor/tests/cassettes_py3/TestCopyTree/test_dx_root_to_existing_dx_dir.yaml
--rw-r--r--   0        0        0    26139 2021-02-12 21:11:43.390000 stor-4.0.2/stor/tests/cassettes_py3/TestCopyTree/test_dx_to_existing_dx_dest_fail.yaml
--rw-r--r--   0        0        0    14320 2021-02-12 21:11:43.390000 stor-4.0.2/stor/tests/cassettes_py3/TestCopyTree/test_dx_to_other_obs.yaml
--rw-r--r--   0        0        0    23578 2021-02-12 21:11:43.390000 stor-4.0.2/stor/tests/cassettes_py3/TestCopyTree/test_dx_to_same_dx_pass.yaml
--rw-r--r--   0        0        0    22091 2021-02-12 21:11:43.390000 stor-4.0.2/stor/tests/cassettes_py3/TestCopyTree/test_move_diff_project_fail.yaml
--rw-r--r--   0        0        0    17134 2021-02-12 21:11:43.390000 stor-4.0.2/stor/tests/cassettes_py3/TestCopyTree/test_move_root_within_project_fail.yaml
--rw-r--r--   0        0        0    17176 2021-02-12 21:11:43.390000 stor-4.0.2/stor/tests/cassettes_py3/TestCopyTree/test_nonexistent_dir.yaml
--rw-r--r--   0        0        0    14323 2021-02-12 21:11:43.390000 stor-4.0.2/stor/tests/cassettes_py3/TestCopyTree/test_other_obs_to_dx.yaml
--rw-r--r--   0        0        0    34316 2021-02-12 21:11:43.390000 stor-4.0.2/stor/tests/cassettes_py3/TestCopyTree/test_posix_dir_to_dx.yaml
--rw-r--r--   0        0        0    47195 2021-02-12 21:11:43.390000 stor-4.0.2/stor/tests/cassettes_py3/TestCopyTree/test_posix_dir_to_dx_existing.yaml
--rw-r--r--   0        0        0    19753 2021-02-12 21:11:43.390000 stor-4.0.2/stor/tests/cassettes_py3/TestCopyTree/test_posix_dir_to_dx_fail.yaml
--rw-r--r--   0        0        0    37245 2021-02-12 21:11:43.390000 stor-4.0.2/stor/tests/cassettes_py3/TestCopyTree/test_posix_dir_to_dx_nested.yaml
--rw-r--r--   0        0        0     9972 2021-02-12 21:11:43.390000 stor-4.0.2/stor/tests/cassettes_py3/TestCopyTree/test_posix_file_to_dx.yaml
--rw-r--r--   0        0        0    63525 2021-02-12 21:11:43.400000 stor-4.0.2/stor/tests/cassettes_py3/TestDownloadObjects/test_absolute_paths.yaml
--rw-r--r--   0        0        0    63514 2021-02-12 21:11:43.400000 stor-4.0.2/stor/tests/cassettes_py3/TestDownloadObjects/test_local_paths.yaml
--rw-r--r--   0        0        0    17494 2021-02-12 21:11:43.400000 stor-4.0.2/stor/tests/cassettes_py3/TestExists/test_false_canonical_path.yaml
--rw-r--r--   0        0        0     1206 2021-02-12 21:11:43.400000 stor-4.0.2/stor/tests/cassettes_py3/TestExists/test_false_canonical_project.yaml
--rw-r--r--   0        0        0     8382 2021-02-12 21:11:43.400000 stor-4.0.2/stor/tests/cassettes_py3/TestExists/test_false_file.yaml
--rw-r--r--   0        0        0     8393 2021-02-12 21:11:43.400000 stor-4.0.2/stor/tests/cassettes_py3/TestExists/test_false_folder.yaml
--rw-r--r--   0        0        0    19698 2021-02-12 21:11:43.400000 stor-4.0.2/stor/tests/cassettes_py3/TestExists/test_false_mixed_path.yaml
--rw-r--r--   0        0        0     2471 2021-02-12 21:11:43.400000 stor-4.0.2/stor/tests/cassettes_py3/TestExists/test_project_does_not_exist.yaml
--rw-r--r--   0        0        0    17614 2021-02-12 21:11:43.400000 stor-4.0.2/stor/tests/cassettes_py3/TestExists/test_true_canonical_path.yaml
--rw-r--r--   0        0        0     5563 2021-02-12 21:11:43.400000 stor-4.0.2/stor/tests/cassettes_py3/TestExists/test_true_canonical_project.yaml
--rw-r--r--   0        0        0    18307 2021-02-12 21:11:43.400000 stor-4.0.2/stor/tests/cassettes_py3/TestExists/test_true_dir_with_object.yaml
--rw-r--r--   0        0        0    12186 2021-02-12 21:11:43.400000 stor-4.0.2/stor/tests/cassettes_py3/TestExists/test_true_empty_dir.yaml
--rw-r--r--   0        0        0    18643 2021-02-12 21:11:43.400000 stor-4.0.2/stor/tests/cassettes_py3/TestExists/test_true_file.yaml
--rw-r--r--   0        0        0    15725 2021-02-12 21:11:43.400000 stor-4.0.2/stor/tests/cassettes_py3/TestExists/test_true_mixed_path.yaml
--rw-r--r--   0        0        0    21193 2021-02-12 21:11:43.400000 stor-4.0.2/stor/tests/cassettes_py3/TestGetSize/test_file.yaml
--rw-r--r--   0        0        0    16952 2021-02-12 21:11:43.400000 stor-4.0.2/stor/tests/cassettes_py3/TestGetSize/test_folder.yaml
--rw-r--r--   0        0        0     7447 2021-02-12 21:11:43.400000 stor-4.0.2/stor/tests/cassettes_py3/TestGetSize/test_project.yaml
--rw-r--r--   0        0        0    27463 2021-02-12 21:11:43.400000 stor-4.0.2/stor/tests/cassettes_py3/TestGlob/test_cond_no_met.yaml
--rw-r--r--   0        0        0    17249 2021-02-12 21:11:43.400000 stor-4.0.2/stor/tests/cassettes_py3/TestGlob/test_glob_cond_met.yaml
--rw-r--r--   0        0        0    27097 2021-02-12 21:11:43.400000 stor-4.0.2/stor/tests/cassettes_py3/TestGlob/test_pattern_no_file_match.yaml
--rw-r--r--   0        0        0    27272 2021-02-12 21:11:43.400000 stor-4.0.2/stor/tests/cassettes_py3/TestGlob/test_prefix_pattern.yaml
--rw-r--r--   0        0        0    27288 2021-02-12 21:11:43.400000 stor-4.0.2/stor/tests/cassettes_py3/TestGlob/test_suffix_pattern.yaml
--rw-r--r--   0        0        0    27469 2021-02-12 21:11:43.400000 stor-4.0.2/stor/tests/cassettes_py3/TestGlob/test_valid_pattern.yaml
--rw-r--r--   0        0        0    27138 2021-02-12 21:11:43.400000 stor-4.0.2/stor/tests/cassettes_py3/TestGlob/test_valid_pattern_wo_wildcard.yaml
--rw-r--r--   0        0        0     7014 2021-02-12 21:11:43.400000 stor-4.0.2/stor/tests/cassettes_py3/TestList/test_list_absent_folder.yaml
--rw-r--r--   0        0        0    27398 2021-02-12 21:11:43.400000 stor-4.0.2/stor/tests/cassettes_py3/TestList/test_list_canonical.yaml
--rw-r--r--   0        0        0     8257 2021-02-12 21:11:43.400000 stor-4.0.2/stor/tests/cassettes_py3/TestList/test_list_empty_folder.yaml
--rw-r--r--   0        0        0    27419 2021-02-12 21:11:43.400000 stor-4.0.2/stor/tests/cassettes_py3/TestList/test_list_fail_w_condition.yaml
--rw-r--r--   0        0        0    17004 2021-02-12 21:11:43.400000 stor-4.0.2/stor/tests/cassettes_py3/TestList/test_list_file.yaml
--rw-r--r--   0        0        0    27270 2021-02-12 21:11:43.400000 stor-4.0.2/stor/tests/cassettes_py3/TestList/test_list_folder_share_filename.yaml
--rw-r--r--   0        0        0    27459 2021-02-12 21:11:43.400000 stor-4.0.2/stor/tests/cassettes_py3/TestList/test_list_folder_w_files.yaml
--rw-r--r--   0        0        0    27975 2021-02-12 21:11:43.400000 stor-4.0.2/stor/tests/cassettes_py3/TestList/test_list_iter_canon_on_canon.yaml
--rw-r--r--   0        0        0    27409 2021-02-12 21:11:43.400000 stor-4.0.2/stor/tests/cassettes_py3/TestList/test_list_iter_project.yaml
--rw-r--r--   0        0        0    28904 2021-02-12 21:11:43.400000 stor-4.0.2/stor/tests/cassettes_py3/TestList/test_list_limit.yaml
--rw-r--r--   0        0        0    27912 2021-02-12 21:11:43.400000 stor-4.0.2/stor/tests/cassettes_py3/TestList/test_list_on_canonical_project.yaml
--rw-r--r--   0        0        0    21879 2021-02-12 21:11:43.400000 stor-4.0.2/stor/tests/cassettes_py3/TestList/test_list_on_canonical_resource.yaml
--rw-r--r--   0        0        0    27394 2021-02-12 21:11:43.400000 stor-4.0.2/stor/tests/cassettes_py3/TestList/test_list_project.yaml
--rw-r--r--   0        0        0    27245 2021-02-12 21:11:43.400000 stor-4.0.2/stor/tests/cassettes_py3/TestList/test_list_starts_with.yaml
--rw-r--r--   0        0        0    28783 2021-02-12 21:11:43.400000 stor-4.0.2/stor/tests/cassettes_py3/TestList/test_list_w_category.yaml
--rw-r--r--   0        0        0    27245 2021-02-12 21:11:43.400000 stor-4.0.2/stor/tests/cassettes_py3/TestList/test_list_w_condition.yaml
--rw-r--r--   0        0        0     7132 2021-02-12 21:11:43.400000 stor-4.0.2/stor/tests/cassettes_py3/TestListDir/test_listdir_absent_folder.yaml
--rw-r--r--   0        0        0    27167 2021-02-12 21:11:43.400000 stor-4.0.2/stor/tests/cassettes_py3/TestListDir/test_listdir_canonical.yaml
--rw-r--r--   0        0        0     8243 2021-02-12 21:11:43.400000 stor-4.0.2/stor/tests/cassettes_py3/TestListDir/test_listdir_empty_folder.yaml
--rw-r--r--   0        0        0    17122 2021-02-12 21:11:43.400000 stor-4.0.2/stor/tests/cassettes_py3/TestListDir/test_listdir_file.yaml
--rw-r--r--   0        0        0    27213 2021-02-12 21:11:43.400000 stor-4.0.2/stor/tests/cassettes_py3/TestListDir/test_listdir_folder_share_filename.yaml
--rw-r--r--   0        0        0    27347 2021-02-12 21:11:43.400000 stor-4.0.2/stor/tests/cassettes_py3/TestListDir/test_listdir_folder_w_file.yaml
--rw-r--r--   0        0        0    29139 2021-02-12 21:11:43.400000 stor-4.0.2/stor/tests/cassettes_py3/TestListDir/test_listdir_iter_canon_on_canon.yaml
--rw-r--r--   0        0        0    28557 2021-02-12 21:11:43.400000 stor-4.0.2/stor/tests/cassettes_py3/TestListDir/test_listdir_iter_project.yaml
--rw-r--r--   0        0        0    27685 2021-02-12 21:11:43.400000 stor-4.0.2/stor/tests/cassettes_py3/TestListDir/test_listdir_on_canonical_project.yaml
--rw-r--r--   0        0        0    21944 2021-02-12 21:11:43.400000 stor-4.0.2/stor/tests/cassettes_py3/TestListDir/test_listdir_on_canonical_resource.yaml
--rw-r--r--   0        0        0    27164 2021-02-12 21:11:43.400000 stor-4.0.2/stor/tests/cassettes_py3/TestListDir/test_listdir_project.yaml
--rw-r--r--   0        0        0     9415 2021-02-12 21:11:43.400000 stor-4.0.2/stor/tests/cassettes_py3/TestLoginAuth/test_login_auth.yaml
--rw-r--r--   0        0        0     9624 2021-02-12 21:11:43.400000 stor-4.0.2/stor/tests/cassettes_py3/TestMakedirsP/test_makedirs_p_folder.yaml
--rw-r--r--   0        0        0    15040 2021-02-12 21:11:43.400000 stor-4.0.2/stor/tests/cassettes_py3/TestMakedirsP/test_makedirs_p_folder_exists.yaml
--rw-r--r--   0        0        0    12403 2021-02-12 21:11:43.400000 stor-4.0.2/stor/tests/cassettes_py3/TestMakedirsP/test_makedirs_p_nested_folder.yaml
--rw-r--r--   0        0        0     2457 2021-02-12 21:11:43.400000 stor-4.0.2/stor/tests/cassettes_py3/TestMakedirsP/test_makedirs_p_project.yaml
--rw-r--r--   0        0        0     9359 2021-02-12 21:11:43.400000 stor-4.0.2/stor/tests/cassettes_py3/TestMakedirsP/test_makedirs_p_project_exists.yaml
--rw-r--r--   0        0        0     4276 2021-02-12 21:11:43.400000 stor-4.0.2/stor/tests/cassettes_py3/TestOpen/test_append_mode_fail.yaml
--rw-r--r--   0        0        0    16958 2021-02-12 21:11:43.400000 stor-4.0.2/stor/tests/cassettes_py3/TestOpen/test_read_dir_fail.yaml
--rw-r--r--   0        0        0    16912 2021-02-12 21:11:43.400000 stor-4.0.2/stor/tests/cassettes_py3/TestOpen/test_read_fail_on_closed_buffer.yaml
--rw-r--r--   0        0        0    37454 2021-02-12 21:11:43.400000 stor-4.0.2/stor/tests/cassettes_py3/TestOpen/test_read_on_open_buffer.yaml
--rw-r--r--   0        0        0     9944 2021-02-12 21:11:43.400000 stor-4.0.2/stor/tests/cassettes_py3/TestOpen/test_read_on_open_dx_file.yaml
--rw-r--r--   0        0        0    14409 2021-02-12 21:11:43.400000 stor-4.0.2/stor/tests/cassettes_py3/TestOpen/test_valid_and_invalid_encoding_for_dnanexus.yaml
--rw-r--r--   0        0        0    54380 2021-02-12 21:11:43.400000 stor-4.0.2/stor/tests/cassettes_py3/TestOpen/test_write_multiple_flush_multiple_upload.yaml
--rw-r--r--   0        0        0    25654 2021-02-12 21:11:43.400000 stor-4.0.2/stor/tests/cassettes_py3/TestOpen/test_write_multiple_wo_context_manager.yaml
--rw-r--r--   0        0        0    56821 2021-02-12 21:11:43.400000 stor-4.0.2/stor/tests/cassettes_py3/TestOpen/test_write_read_over_files.yaml
--rw-r--r--   0        0        0     4286 2021-02-12 21:11:43.400000 stor-4.0.2/stor/tests/cassettes_py3/TestOpen/test_write_to_project_fail.yaml
--rw-r--r--   0        0        0    26927 2021-02-12 21:11:43.400000 stor-4.0.2/stor/tests/cassettes_py3/TestOpen/test_write_w_settings_big_timeout.yaml
--rw-r--r--   0        0        0    24601 2021-02-12 21:11:43.400000 stor-4.0.2/stor/tests/cassettes_py3/TestOpen/test_write_w_settings_no_timeout.yaml
--rw-r--r--   0        0        0     8200 2021-02-12 21:11:43.400000 stor-4.0.2/stor/tests/cassettes_py3/TestRemove/test_fail_remove_folder.yaml
--rw-r--r--   0        0        0     6980 2021-02-12 21:11:43.400000 stor-4.0.2/stor/tests/cassettes_py3/TestRemove/test_fail_remove_nonexistent_file.yaml
--rw-r--r--   0        0        0     5532 2021-02-12 21:11:43.400000 stor-4.0.2/stor/tests/cassettes_py3/TestRemove/test_fail_remove_nonexistent_project.yaml
--rw-r--r--   0        0        0     4286 2021-02-12 21:11:43.400000 stor-4.0.2/stor/tests/cassettes_py3/TestRemove/test_fail_remove_project.yaml
--rw-r--r--   0        0        0    17050 2021-02-12 21:11:43.400000 stor-4.0.2/stor/tests/cassettes_py3/TestRemove/test_fail_rmtree_file.yaml
--rw-r--r--   0        0        0    22218 2021-02-12 21:11:43.400000 stor-4.0.2/stor/tests/cassettes_py3/TestRemove/test_remove_file.yaml
--rw-r--r--   0        0        0    24863 2021-02-12 21:11:43.400000 stor-4.0.2/stor/tests/cassettes_py3/TestRemove/test_rmtree_folder.yaml
--rw-r--r--   0        0        0    42175 2021-02-12 21:11:43.400000 stor-4.0.2/stor/tests/cassettes_py3/TestRemove/test_rmtree_project.yaml
--rw-r--r--   0        0        0    22690 2021-02-12 21:11:43.400000 stor-4.0.2/stor/tests/cassettes_py3/TestRename/test_rename_file_pass.yaml
--rw-r--r--   0        0        0    16984 2021-02-12 21:11:43.400000 stor-4.0.2/stor/tests/cassettes_py3/TestRename/test_rename_folder_fail.yaml
--rw-r--r--   0        0        0    18646 2021-02-12 21:11:43.400000 stor-4.0.2/stor/tests/cassettes_py3/TestRename/test_rename_to_self.yaml
--rw-r--r--   0        0        0     6113 2021-02-12 21:11:43.400000 stor-4.0.2/stor/tests/cassettes_py3/TestStat/test_stat_canonical_project.yaml
--rw-r--r--   0        0        0    18612 2021-02-12 21:11:43.400000 stor-4.0.2/stor/tests/cassettes_py3/TestStat/test_stat_canonical_resource.yaml
--rw-r--r--   0        0        0    32942 2021-02-12 21:11:43.400000 stor-4.0.2/stor/tests/cassettes_py3/TestStat/test_stat_file.yaml
--rw-r--r--   0        0        0    16963 2021-02-12 21:11:43.400000 stor-4.0.2/stor/tests/cassettes_py3/TestStat/test_stat_folder.yaml
--rw-r--r--   0        0        0    10934 2021-02-12 21:11:43.400000 stor-4.0.2/stor/tests/cassettes_py3/TestStat/test_stat_project_error.yaml
--rw-r--r--   0        0        0    10689 2021-02-12 21:11:43.400000 stor-4.0.2/stor/tests/cassettes_py3/TestStat/test_stat_virtual_project.yaml
--rw-r--r--   0        0        0    18913 2021-02-12 21:11:43.400000 stor-4.0.2/stor/tests/cassettes_py3/TestTempUrl/test_fail_on_folder.yaml
--rw-r--r--   0        0        0     3828 2021-02-12 21:11:43.400000 stor-4.0.2/stor/tests/cassettes_py3/TestTempUrl/test_fail_on_project.yaml
--rw-r--r--   0        0        0    20224 2021-02-12 21:11:43.400000 stor-4.0.2/stor/tests/cassettes_py3/TestTempUrl/test_on_file.yaml
--rw-r--r--   0        0        0    24611 2021-02-12 21:11:43.400000 stor-4.0.2/stor/tests/cassettes_py3/TestTempUrl/test_on_file_canonical.yaml
--rw-r--r--   0        0        0    21814 2021-02-12 21:11:43.400000 stor-4.0.2/stor/tests/cassettes_py3/TestTempUrl/test_on_file_named_timed.yaml
--rw-r--r--   0        0        0    51935 2021-02-12 21:11:43.400000 stor-4.0.2/stor/tests/cassettes_py3/TestTempUrl/test_on_file_with_proxy_url.yaml
--rw-r--r--   0        0        0    43020 2021-02-12 21:11:43.400000 stor-4.0.2/stor/tests/cassettes_py3/TestUpload/test_upload_files_existing.yaml
--rw-r--r--   0        0        0    17078 2021-02-12 21:11:43.400000 stor-4.0.2/stor/tests/cassettes_py3/TestWalkFiles/test_pattern_no_match.yaml
--rw-r--r--   0        0        0    27305 2021-02-12 21:11:43.400000 stor-4.0.2/stor/tests/cassettes_py3/TestWalkFiles/test_pattern_share_folder_match.yaml
--rw-r--r--   0        0        0    27274 2021-02-12 21:11:43.400000 stor-4.0.2/stor/tests/cassettes_py3/TestWalkFiles/test_pattern_w_prefix.yaml
--rw-r--r--   0        0        0    27469 2021-02-12 21:11:43.400000 stor-4.0.2/stor/tests/cassettes_py3/TestWalkFiles/test_pattern_w_prefix_suffix.yaml
--rw-r--r--   0        0        0    27263 2021-02-12 21:11:43.400000 stor-4.0.2/stor/tests/cassettes_py3/TestWalkFiles/test_pattern_w_suffix.yaml
--rw-r--r--   0        0        0  1506424 2021-02-12 21:11:43.410000 stor-4.0.2/stor/tests/file_data/s_3_2126.bcl.gz
--rw-r--r--   0        0        0      107 2021-02-12 21:11:43.410000 stor-4.0.2/stor/tests/file_data/test.cfg
--rw-r--r--   0        0        0      259 2021-02-12 21:11:43.410000 stor-4.0.2/stor/tests/shared.py
--rw-r--r--   0        0        0     7817 2021-02-12 21:11:43.410000 stor-4.0.2/stor/tests/shared_obs.py
--rw-r--r--   0        0        0        0 2021-02-12 21:11:43.410000 stor-4.0.2/stor/tests/swift_upload/data_dir/file2
--rw-r--r--   0        0        0        0 2021-02-12 21:11:43.410000 stor-4.0.2/stor/tests/swift_upload/file1
--rw-r--r--   0        0        0    27556 2021-02-12 21:11:43.410000 stor-4.0.2/stor/tests/test_cli.py
--rw-r--r--   0        0        0    85377 2021-02-12 21:11:43.410000 stor-4.0.2/stor/tests/test_dx.py
--rw-r--r--   0        0        0    10215 2021-02-12 21:11:43.410000 stor-4.0.2/stor/tests/test_dx_path_compat.py
--rw-r--r--   0        0        0     1464 2021-02-12 21:11:43.410000 stor-4.0.2/stor/tests/test_extensions_swiftstack.py
--rw-r--r--   0        0        0    11174 2021-02-12 21:11:43.410000 stor-4.0.2/stor/tests/test_integration.py
--rw-r--r--   0        0        0    11813 2021-02-12 21:11:43.410000 stor-4.0.2/stor/tests/test_integration_dx.py
--rw-r--r--   0        0        0     1024 2021-02-12 21:11:43.410000 stor-4.0.2/stor/tests/test_integration_posix.py
--rw-r--r--   0        0        0    11946 2021-02-12 21:11:43.410000 stor-4.0.2/stor/tests/test_integration_s3.py
--rw-r--r--   0        0        0    19309 2021-02-12 21:11:43.410000 stor-4.0.2/stor/tests/test_integration_swift.py
--rw-r--r--   0        0        0    11484 2021-02-12 21:11:43.410000 stor-4.0.2/stor/tests/test_posix.py
--rw-r--r--   0        0        0     8568 2021-02-12 21:11:43.410000 stor-4.0.2/stor/tests/test_posix_path_compat.py
--rw-r--r--   0        0        0    64190 2021-02-12 21:11:43.410000 stor-4.0.2/stor/tests/test_s3.py
--rw-r--r--   0        0        0     1692 2021-02-12 21:11:43.410000 stor-4.0.2/stor/tests/test_s3_path_compat.py
--rw-r--r--   0        0        0    10064 2021-02-12 21:11:43.410000 stor-4.0.2/stor/tests/test_settings.py
--rw-r--r--   0        0        0   108660 2021-02-12 21:11:43.410000 stor-4.0.2/stor/tests/test_swift.py
--rw-r--r--   0        0        0     1812 2021-02-12 21:11:43.420000 stor-4.0.2/stor/tests/test_swift_path_compat.py
--rw-r--r--   0        0        0    17579 2021-02-12 21:11:43.420000 stor-4.0.2/stor/tests/test_utils.py
--rw-r--r--   0        0        0     1628 2021-02-12 21:11:43.420000 stor-4.0.2/stor/tests/test_windows.py
--rw-r--r--   0        0        0        0 2021-02-12 21:11:43.420000 stor-4.0.2/stor/third_party/__init__.py
--rw-r--r--   0        0        0     4934 2021-02-12 21:11:43.420000 stor-4.0.2/stor/third_party/backoff.py
--rw-r--r--   0        0        0    25379 2021-02-12 21:11:43.420000 stor-4.0.2/stor/utils.py
--rw-r--r--   0        0        0      498 2021-02-12 21:11:43.420000 stor-4.0.2/stor/windows.py
--rw-r--r--   0        0        0     7558 2021-02-12 21:11:47.990000 stor-4.0.2/setup.py
--rw-r--r--   0        0        0     6330 2021-02-12 21:11:47.990000 stor-4.0.2/PKG-INFO
+-rw-r--r--   0        0        0     2330 2023-06-23 02:15:24.130302 stor-4.1.0/LICENSE
+-rw-r--r--   0        0        0     5295 2023-06-23 02:15:24.130302 stor-4.1.0/README.rst
+-rw-r--r--   0        0        0     1585 2023-06-23 02:15:24.138302 stor-4.1.0/pyproject.toml
+-rw-r--r--   0        0        0     3465 2023-06-23 02:15:24.138302 stor-4.1.0/stor/__init__.py
+-rw-r--r--   0        0        0    19880 2023-06-23 02:15:24.138302 stor-4.1.0/stor/base.py
+-rw-r--r--   0        0        0    18210 2023-06-23 02:15:24.138302 stor-4.1.0/stor/cli.py
+-rw-r--r--   0        0        0     5065 2023-06-23 02:15:24.138302 stor-4.1.0/stor/default.cfg
+-rw-r--r--   0        0        0       44 2023-06-23 02:15:24.138302 stor-4.1.0/stor/default.env
+-rw-r--r--   0        0        0    52552 2023-06-23 02:15:24.138302 stor-4.1.0/stor/dx.py
+-rw-r--r--   0        0        0     3339 2023-06-23 02:15:24.138302 stor-4.1.0/stor/exceptions.py
+-rw-r--r--   0        0        0        0 2023-06-23 02:15:24.138302 stor-4.1.0/stor/extensions/__init__.py
+-rw-r--r--   0        0        0     1328 2023-06-23 02:15:24.138302 stor-4.1.0/stor/extensions/swiftstack.py
+-rw-r--r--   0        0        0    17823 2023-06-23 02:15:24.138302 stor-4.1.0/stor/obs.py
+-rw-r--r--   0        0        0     1459 2023-06-23 02:15:24.138302 stor-4.1.0/stor/posix.py
+-rw-r--r--   0        0        0    31296 2023-06-23 02:15:24.138302 stor-4.1.0/stor/s3.py
+-rw-r--r--   0        0        0     5433 2023-06-23 02:15:24.138302 stor-4.1.0/stor/settings.py
+-rw-r--r--   0        0        0      558 2023-06-23 02:15:24.138302 stor-4.1.0/stor/stor-completion.bash
+-rw-r--r--   0        0        0    62780 2023-06-23 02:15:24.138302 stor-4.1.0/stor/swift.py
+-rw-r--r--   0        0        0    16675 2023-06-23 02:15:24.138302 stor-4.1.0/stor/test.py
+-rw-r--r--   0        0        0        0 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/__init__.py
+-rw-r--r--   0        0        0    20324 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/cassettes_py3/TestCanonicalProject/test_canonical_path.yaml
+-rw-r--r--   0        0        0     8236 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/cassettes_py3/TestCanonicalProject/test_canonical_path_on_dir.yaml
+-rw-r--r--   0        0        0     8262 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/cassettes_py3/TestCanonicalProject/test_duplicate_projects.yaml
+-rw-r--r--   0        0        0     1248 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/cassettes_py3/TestCanonicalProject/test_no_project.yaml
+-rw-r--r--   0        0        0     5682 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/cassettes_py3/TestCanonicalProject/test_unique_project.yaml
+-rw-r--r--   0        0        0    27246 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/cassettes_py3/TestCanonicalResource/test_duplicate_resource.yaml
+-rw-r--r--   0        0        0     6960 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/cassettes_py3/TestCanonicalResource/test_no_resource.yaml
+-rw-r--r--   0        0        0     4284 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/cassettes_py3/TestCanonicalResource/test_project.yaml
+-rw-r--r--   0        0        0    17075 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/cassettes_py3/TestCanonicalResource/test_unique_resource.yaml
+-rw-r--r--   0        0        0    16155 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/cassettes_py3/TestCanonicalResource/test_virtual_on_virtual.yaml
+-rw-r--r--   0        0        0    19311 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/cassettes_py3/TestCopy/test_clone_move_project_fail.yaml
+-rw-r--r--   0        0        0    32263 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/cassettes_py3/TestCopy/test_clone_within_project_fail.yaml
+-rw-r--r--   0        0        0    36334 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/cassettes_py3/TestCopy/test_dx_canonical_to_dx_file.yaml
+-rw-r--r--   0        0        0    19572 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/cassettes_py3/TestCopy/test_dx_dir_to_posix_error.yaml
+-rw-r--r--   0        0        0    78875 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/cassettes_py3/TestCopy/test_dx_to_dx_diff_project_exist_file.yaml
+-rw-r--r--   0        0        0    36267 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/cassettes_py3/TestCopy/test_dx_to_dx_file.yaml
+-rw-r--r--   0        0        0    62844 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/cassettes_py3/TestCopy/test_dx_to_dx_file_folder_no_ext.yaml
+-rw-r--r--   0        0        0    39012 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/cassettes_py3/TestCopy/test_dx_to_dx_folder.yaml
+-rw-r--r--   0        0        0    84362 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/cassettes_py3/TestCopy/test_dx_to_dx_same_project_exist_dest.yaml
+-rw-r--r--   0        0        0    23018 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/cassettes_py3/TestCopy/test_dx_to_dx_within_project_fail.yaml
+-rw-r--r--   0        0        0    66832 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/cassettes_py3/TestCopy/test_dx_to_dx_within_project_pass.yaml
+-rw-r--r--   0        0        0    18184 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/cassettes_py3/TestCopy/test_dx_to_other_obs.yaml
+-rw-r--r--   0        0        0    24022 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/cassettes_py3/TestCopy/test_dx_to_posix_file.yaml
+-rw-r--r--   0        0        0    31201 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/cassettes_py3/TestCopy/test_dx_to_posix_file_folder_no_ext.yaml
+-rw-r--r--   0        0        0    24027 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/cassettes_py3/TestCopy/test_dx_to_posix_folder.yaml
+-rw-r--r--   0        0        0    24202 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/cassettes_py3/TestCopy/test_dx_to_same_dx_pass.yaml
+-rw-r--r--   0        0        0    22069 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/cassettes_py3/TestCopy/test_move_diff_project_fail.yaml
+-rw-r--r--   0        0        0    16892 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/cassettes_py3/TestCopy/test_other_obs_to_dx.yaml
+-rw-r--r--   0        0        0    11502 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/cassettes_py3/TestCopy/test_posix_to_dx_fail.yaml
+-rw-r--r--   0        0        0    21649 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/cassettes_py3/TestCopy/test_posix_to_dx_file.yaml
+-rw-r--r--   0        0        0    47262 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/cassettes_py3/TestCopy/test_posix_to_dx_file_folder_no_ext.yaml
+-rw-r--r--   0        0        0    21622 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/cassettes_py3/TestCopy/test_posix_to_dx_folder.yaml
+-rw-r--r--   0        0        0    48364 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/cassettes_py3/TestCopy/test_posix_to_existing_dx.yaml
+-rw-r--r--   0        0        0    32339 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/cassettes_py3/TestCopyTree/test_clonetree_within_project_fail.yaml
+-rw-r--r--   0        0        0    47177 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/cassettes_py3/TestCopyTree/test_dx_dir_to_dx_dir.yaml
+-rw-r--r--   0        0        0    32151 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/cassettes_py3/TestCopyTree/test_dx_dir_to_dx_dir_same_project.yaml
+-rw-r--r--   0        0        0    35304 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/cassettes_py3/TestCopyTree/test_dx_dir_to_dx_dir_same_project_fail.yaml
+-rw-r--r--   0        0        0    48797 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/cassettes_py3/TestCopyTree/test_dx_dir_to_dx_dir_w_slash.yaml
+-rw-r--r--   0        0        0    47283 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/cassettes_py3/TestCopyTree/test_dx_dir_to_dx_existing_dir.yaml
+-rw-r--r--   0        0        0    35180 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/cassettes_py3/TestCopyTree/test_dx_dir_to_dx_root.yaml
+-rw-r--r--   0        0        0    30228 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/cassettes_py3/TestCopyTree/test_dx_dir_to_dx_root_same_project.yaml
+-rw-r--r--   0        0        0    62333 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/cassettes_py3/TestCopyTree/test_dx_dir_to_posix.yaml
+-rw-r--r--   0        0        0    17613 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/cassettes_py3/TestCopyTree/test_dx_file_to_posix.yaml
+-rw-r--r--   0        0        0    44999 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/cassettes_py3/TestCopyTree/test_dx_root_to_dx_dir.yaml
+-rw-r--r--   0        0        0    19014 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/cassettes_py3/TestCopyTree/test_dx_root_to_dx_dir_same_project.yaml
+-rw-r--r--   0        0        0    48181 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/cassettes_py3/TestCopyTree/test_dx_root_to_dx_dir_w_slash.yaml
+-rw-r--r--   0        0        0    35766 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/cassettes_py3/TestCopyTree/test_dx_root_to_dx_root.yaml
+-rw-r--r--   0        0        0    49292 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/cassettes_py3/TestCopyTree/test_dx_root_to_existing_dx_dir.yaml
+-rw-r--r--   0        0        0    26139 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/cassettes_py3/TestCopyTree/test_dx_to_existing_dx_dest_fail.yaml
+-rw-r--r--   0        0        0    14320 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/cassettes_py3/TestCopyTree/test_dx_to_other_obs.yaml
+-rw-r--r--   0        0        0    23578 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/cassettes_py3/TestCopyTree/test_dx_to_same_dx_pass.yaml
+-rw-r--r--   0        0        0    22091 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/cassettes_py3/TestCopyTree/test_move_diff_project_fail.yaml
+-rw-r--r--   0        0        0    17134 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/cassettes_py3/TestCopyTree/test_move_root_within_project_fail.yaml
+-rw-r--r--   0        0        0    17176 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/cassettes_py3/TestCopyTree/test_nonexistent_dir.yaml
+-rw-r--r--   0        0        0    14323 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/cassettes_py3/TestCopyTree/test_other_obs_to_dx.yaml
+-rw-r--r--   0        0        0    34316 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/cassettes_py3/TestCopyTree/test_posix_dir_to_dx.yaml
+-rw-r--r--   0        0        0    47195 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/cassettes_py3/TestCopyTree/test_posix_dir_to_dx_existing.yaml
+-rw-r--r--   0        0        0    19753 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/cassettes_py3/TestCopyTree/test_posix_dir_to_dx_fail.yaml
+-rw-r--r--   0        0        0    37245 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/cassettes_py3/TestCopyTree/test_posix_dir_to_dx_nested.yaml
+-rw-r--r--   0        0        0     9972 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/cassettes_py3/TestCopyTree/test_posix_file_to_dx.yaml
+-rw-r--r--   0        0        0    63525 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/cassettes_py3/TestDownloadObjects/test_absolute_paths.yaml
+-rw-r--r--   0        0        0    63514 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/cassettes_py3/TestDownloadObjects/test_local_paths.yaml
+-rw-r--r--   0        0        0    17494 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/cassettes_py3/TestExists/test_false_canonical_path.yaml
+-rw-r--r--   0        0        0     1206 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/cassettes_py3/TestExists/test_false_canonical_project.yaml
+-rw-r--r--   0        0        0     8382 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/cassettes_py3/TestExists/test_false_file.yaml
+-rw-r--r--   0        0        0     8393 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/cassettes_py3/TestExists/test_false_folder.yaml
+-rw-r--r--   0        0        0    19698 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/cassettes_py3/TestExists/test_false_mixed_path.yaml
+-rw-r--r--   0        0        0     2471 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/cassettes_py3/TestExists/test_project_does_not_exist.yaml
+-rw-r--r--   0        0        0    17614 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/cassettes_py3/TestExists/test_true_canonical_path.yaml
+-rw-r--r--   0        0        0     5563 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/cassettes_py3/TestExists/test_true_canonical_project.yaml
+-rw-r--r--   0        0        0    18307 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/cassettes_py3/TestExists/test_true_dir_with_object.yaml
+-rw-r--r--   0        0        0    12186 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/cassettes_py3/TestExists/test_true_empty_dir.yaml
+-rw-r--r--   0        0        0    18643 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/cassettes_py3/TestExists/test_true_file.yaml
+-rw-r--r--   0        0        0    15725 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/cassettes_py3/TestExists/test_true_mixed_path.yaml
+-rw-r--r--   0        0        0    21193 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/cassettes_py3/TestGetSize/test_file.yaml
+-rw-r--r--   0        0        0    16952 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/cassettes_py3/TestGetSize/test_folder.yaml
+-rw-r--r--   0        0        0     7447 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/cassettes_py3/TestGetSize/test_project.yaml
+-rw-r--r--   0        0        0    27463 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/cassettes_py3/TestGlob/test_cond_no_met.yaml
+-rw-r--r--   0        0        0    17249 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/cassettes_py3/TestGlob/test_glob_cond_met.yaml
+-rw-r--r--   0        0        0    27097 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/cassettes_py3/TestGlob/test_pattern_no_file_match.yaml
+-rw-r--r--   0        0        0    27272 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/cassettes_py3/TestGlob/test_prefix_pattern.yaml
+-rw-r--r--   0        0        0    27288 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/cassettes_py3/TestGlob/test_suffix_pattern.yaml
+-rw-r--r--   0        0        0    27469 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/cassettes_py3/TestGlob/test_valid_pattern.yaml
+-rw-r--r--   0        0        0    27138 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/cassettes_py3/TestGlob/test_valid_pattern_wo_wildcard.yaml
+-rw-r--r--   0        0        0     7014 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/cassettes_py3/TestList/test_list_absent_folder.yaml
+-rw-r--r--   0        0        0    27398 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/cassettes_py3/TestList/test_list_canonical.yaml
+-rw-r--r--   0        0        0     8257 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/cassettes_py3/TestList/test_list_empty_folder.yaml
+-rw-r--r--   0        0        0    27419 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/cassettes_py3/TestList/test_list_fail_w_condition.yaml
+-rw-r--r--   0        0        0    17004 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/cassettes_py3/TestList/test_list_file.yaml
+-rw-r--r--   0        0        0    27270 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/cassettes_py3/TestList/test_list_folder_share_filename.yaml
+-rw-r--r--   0        0        0    27459 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/cassettes_py3/TestList/test_list_folder_w_files.yaml
+-rw-r--r--   0        0        0    27975 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/cassettes_py3/TestList/test_list_iter_canon_on_canon.yaml
+-rw-r--r--   0        0        0    27409 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/cassettes_py3/TestList/test_list_iter_project.yaml
+-rw-r--r--   0        0        0    28904 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/cassettes_py3/TestList/test_list_limit.yaml
+-rw-r--r--   0        0        0    27912 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/cassettes_py3/TestList/test_list_on_canonical_project.yaml
+-rw-r--r--   0        0        0    21879 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/cassettes_py3/TestList/test_list_on_canonical_resource.yaml
+-rw-r--r--   0        0        0    27394 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/cassettes_py3/TestList/test_list_project.yaml
+-rw-r--r--   0        0        0    27245 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/cassettes_py3/TestList/test_list_starts_with.yaml
+-rw-r--r--   0        0        0    28783 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/cassettes_py3/TestList/test_list_w_category.yaml
+-rw-r--r--   0        0        0    27245 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/cassettes_py3/TestList/test_list_w_condition.yaml
+-rw-r--r--   0        0        0     7132 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/cassettes_py3/TestListDir/test_listdir_absent_folder.yaml
+-rw-r--r--   0        0        0    27167 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/cassettes_py3/TestListDir/test_listdir_canonical.yaml
+-rw-r--r--   0        0        0     8243 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/cassettes_py3/TestListDir/test_listdir_empty_folder.yaml
+-rw-r--r--   0        0        0    17122 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/cassettes_py3/TestListDir/test_listdir_file.yaml
+-rw-r--r--   0        0        0    27213 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/cassettes_py3/TestListDir/test_listdir_folder_share_filename.yaml
+-rw-r--r--   0        0        0    27347 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/cassettes_py3/TestListDir/test_listdir_folder_w_file.yaml
+-rw-r--r--   0        0        0    29139 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/cassettes_py3/TestListDir/test_listdir_iter_canon_on_canon.yaml
+-rw-r--r--   0        0        0    28557 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/cassettes_py3/TestListDir/test_listdir_iter_project.yaml
+-rw-r--r--   0        0        0    27685 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/cassettes_py3/TestListDir/test_listdir_on_canonical_project.yaml
+-rw-r--r--   0        0        0    21944 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/cassettes_py3/TestListDir/test_listdir_on_canonical_resource.yaml
+-rw-r--r--   0        0        0    27164 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/cassettes_py3/TestListDir/test_listdir_project.yaml
+-rw-r--r--   0        0        0     9415 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/cassettes_py3/TestLoginAuth/test_login_auth.yaml
+-rw-r--r--   0        0        0     9624 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/cassettes_py3/TestMakedirsP/test_makedirs_p_folder.yaml
+-rw-r--r--   0        0        0    15040 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/cassettes_py3/TestMakedirsP/test_makedirs_p_folder_exists.yaml
+-rw-r--r--   0        0        0    12403 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/cassettes_py3/TestMakedirsP/test_makedirs_p_nested_folder.yaml
+-rw-r--r--   0        0        0     2457 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/cassettes_py3/TestMakedirsP/test_makedirs_p_project.yaml
+-rw-r--r--   0        0        0     9359 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/cassettes_py3/TestMakedirsP/test_makedirs_p_project_exists.yaml
+-rw-r--r--   0        0        0     4276 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/cassettes_py3/TestOpen/test_append_mode_fail.yaml
+-rw-r--r--   0        0        0    16958 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/cassettes_py3/TestOpen/test_read_dir_fail.yaml
+-rw-r--r--   0        0        0    16912 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/cassettes_py3/TestOpen/test_read_fail_on_closed_buffer.yaml
+-rw-r--r--   0        0        0    37454 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/cassettes_py3/TestOpen/test_read_on_open_buffer.yaml
+-rw-r--r--   0        0        0     9944 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/cassettes_py3/TestOpen/test_read_on_open_dx_file.yaml
+-rw-r--r--   0        0        0    14409 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/cassettes_py3/TestOpen/test_valid_and_invalid_encoding_for_dnanexus.yaml
+-rw-r--r--   0        0        0    54380 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/cassettes_py3/TestOpen/test_write_multiple_flush_multiple_upload.yaml
+-rw-r--r--   0        0        0    25654 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/cassettes_py3/TestOpen/test_write_multiple_wo_context_manager.yaml
+-rw-r--r--   0        0        0    56821 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/cassettes_py3/TestOpen/test_write_read_over_files.yaml
+-rw-r--r--   0        0        0     4286 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/cassettes_py3/TestOpen/test_write_to_project_fail.yaml
+-rw-r--r--   0        0        0    26927 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/cassettes_py3/TestOpen/test_write_w_settings_big_timeout.yaml
+-rw-r--r--   0        0        0    24601 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/cassettes_py3/TestOpen/test_write_w_settings_no_timeout.yaml
+-rw-r--r--   0        0        0     8200 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/cassettes_py3/TestRemove/test_fail_remove_folder.yaml
+-rw-r--r--   0        0        0     6980 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/cassettes_py3/TestRemove/test_fail_remove_nonexistent_file.yaml
+-rw-r--r--   0        0        0     5532 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/cassettes_py3/TestRemove/test_fail_remove_nonexistent_project.yaml
+-rw-r--r--   0        0        0     4286 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/cassettes_py3/TestRemove/test_fail_remove_project.yaml
+-rw-r--r--   0        0        0    17050 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/cassettes_py3/TestRemove/test_fail_rmtree_file.yaml
+-rw-r--r--   0        0        0    22218 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/cassettes_py3/TestRemove/test_remove_file.yaml
+-rw-r--r--   0        0        0    24863 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/cassettes_py3/TestRemove/test_rmtree_folder.yaml
+-rw-r--r--   0        0        0    42175 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/cassettes_py3/TestRemove/test_rmtree_project.yaml
+-rw-r--r--   0        0        0    22690 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/cassettes_py3/TestRename/test_rename_file_pass.yaml
+-rw-r--r--   0        0        0    16984 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/cassettes_py3/TestRename/test_rename_folder_fail.yaml
+-rw-r--r--   0        0        0    18646 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/cassettes_py3/TestRename/test_rename_to_self.yaml
+-rw-r--r--   0        0        0     6113 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/cassettes_py3/TestStat/test_stat_canonical_project.yaml
+-rw-r--r--   0        0        0    18612 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/cassettes_py3/TestStat/test_stat_canonical_resource.yaml
+-rw-r--r--   0        0        0    32942 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/cassettes_py3/TestStat/test_stat_file.yaml
+-rw-r--r--   0        0        0    16963 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/cassettes_py3/TestStat/test_stat_folder.yaml
+-rw-r--r--   0        0        0    10934 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/cassettes_py3/TestStat/test_stat_project_error.yaml
+-rw-r--r--   0        0        0    10689 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/cassettes_py3/TestStat/test_stat_virtual_project.yaml
+-rw-r--r--   0        0        0    18913 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/cassettes_py3/TestTempUrl/test_fail_on_folder.yaml
+-rw-r--r--   0        0        0     3828 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/cassettes_py3/TestTempUrl/test_fail_on_project.yaml
+-rw-r--r--   0        0        0    20224 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/cassettes_py3/TestTempUrl/test_on_file.yaml
+-rw-r--r--   0        0        0    24611 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/cassettes_py3/TestTempUrl/test_on_file_canonical.yaml
+-rw-r--r--   0        0        0    21814 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/cassettes_py3/TestTempUrl/test_on_file_named_timed.yaml
+-rw-r--r--   0        0        0    51935 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/cassettes_py3/TestTempUrl/test_on_file_with_proxy_url.yaml
+-rw-r--r--   0        0        0    43020 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/cassettes_py3/TestUpload/test_upload_files_existing.yaml
+-rw-r--r--   0        0        0    17078 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/cassettes_py3/TestWalkFiles/test_pattern_no_match.yaml
+-rw-r--r--   0        0        0    27305 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/cassettes_py3/TestWalkFiles/test_pattern_share_folder_match.yaml
+-rw-r--r--   0        0        0    27274 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/cassettes_py3/TestWalkFiles/test_pattern_w_prefix.yaml
+-rw-r--r--   0        0        0    27469 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/cassettes_py3/TestWalkFiles/test_pattern_w_prefix_suffix.yaml
+-rw-r--r--   0        0        0    27263 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/cassettes_py3/TestWalkFiles/test_pattern_w_suffix.yaml
+-rw-r--r--   0        0        0  1506424 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/file_data/s_3_2126.bcl.gz
+-rw-r--r--   0        0        0      107 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/file_data/test.cfg
+-rw-r--r--   0        0        0      259 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/shared.py
+-rw-r--r--   0        0        0     7817 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/shared_obs.py
+-rw-r--r--   0        0        0        0 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/swift_upload/data_dir/file2
+-rw-r--r--   0        0        0        0 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/swift_upload/file1
+-rw-r--r--   0        0        0    27556 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/test_cli.py
+-rw-r--r--   0        0        0    85377 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/test_dx.py
+-rw-r--r--   0        0        0    10215 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/test_dx_path_compat.py
+-rw-r--r--   0        0        0     1464 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/test_extensions_swiftstack.py
+-rw-r--r--   0        0        0    11174 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/test_integration.py
+-rw-r--r--   0        0        0    11813 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/test_integration_dx.py
+-rw-r--r--   0        0        0     1024 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/test_integration_posix.py
+-rw-r--r--   0        0        0    11946 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/test_integration_s3.py
+-rw-r--r--   0        0        0    19309 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/test_integration_swift.py
+-rw-r--r--   0        0        0    11484 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/test_posix.py
+-rw-r--r--   0        0        0     8568 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/test_posix_path_compat.py
+-rw-r--r--   0        0        0    65879 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/test_s3.py
+-rw-r--r--   0        0        0     1692 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/test_s3_path_compat.py
+-rw-r--r--   0        0        0    10064 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/test_settings.py
+-rw-r--r--   0        0        0   108660 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/test_swift.py
+-rw-r--r--   0        0        0     1812 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/test_swift_path_compat.py
+-rw-r--r--   0        0        0    17579 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/test_utils.py
+-rw-r--r--   0        0        0     1628 2023-06-23 02:15:24.138302 stor-4.1.0/stor/tests/test_windows.py
+-rw-r--r--   0        0        0        0 2023-06-23 02:15:24.138302 stor-4.1.0/stor/third_party/__init__.py
+-rw-r--r--   0        0        0     4934 2023-06-23 02:15:24.138302 stor-4.1.0/stor/third_party/backoff.py
+-rw-r--r--   0        0        0    25379 2023-06-23 02:15:24.138302 stor-4.1.0/stor/utils.py
+-rw-r--r--   0        0        0      498 2023-06-23 02:15:24.138302 stor-4.1.0/stor/windows.py
+-rw-r--r--   0        0        0     7468 2023-06-23 02:15:50.088987 stor-4.1.0/setup.py
+-rw-r--r--   0        0        0     6280 2023-06-23 02:15:50.090113 stor-4.1.0/PKG-INFO
```

### Comparing `stor-4.0.2/LICENSE` & `stor-4.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/README.rst` & `stor-4.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/pyproject.toml` & `stor-4.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "stor"
-version = "4.0.2"
+version = "4.1.0"
 description = "Cross-compatible API for accessing Posix and OBS storage systems"
 authors = ["Counsyl Inc. <opensource@counsyl.com>"]
 license = "MIT"
 homepage = "https://counsyl.github.io/stor"
 readme = "README.rst"
 repository = "https://github.com/counsyl/stor"
 classifiers = [
```

### Comparing `stor-4.0.2/stor/__init__.py` & `stor-4.1.0/stor/__init__.py`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/base.py` & `stor-4.1.0/stor/base.py`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/cli.py` & `stor-4.1.0/stor/cli.py`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/default.cfg` & `stor-4.1.0/stor/default.cfg`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/dx.py` & `stor-4.1.0/stor/dx.py`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/exceptions.py` & `stor-4.1.0/stor/exceptions.py`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/extensions/swiftstack.py` & `stor-4.1.0/stor/extensions/swiftstack.py`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/obs.py` & `stor-4.1.0/stor/obs.py`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/posix.py` & `stor-4.1.0/stor/posix.py`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/s3.py` & `stor-4.1.0/stor/s3.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 An experimental implementation of S3 in stor
 """
 from functools import partial
 import logging
-from multiprocessing.pool import ThreadPool
+from concurrent.futures import as_completed, ThreadPoolExecutor
 import os
 import tempfile
 import threading
 
 import boto3
 from boto3 import exceptions as boto3_exceptions
 from boto3.s3.transfer import S3Transfer
@@ -576,36 +576,38 @@
             'max_concurrency': options.get('segment_threads'),
             'multipart_chunksize': segment_size
         }
         download_w_config = partial(self._download_object_worker, config=transfer_config)
 
         downloaded = {'completed': [], 'failed': []}
         with S3DownloadLogger(len(files_to_download)) as dl:
-            pool = ThreadPool(options['object_threads'])
-            try:
-                result_iter = pool.imap_unordered(download_w_config, files_to_download)
-                while True:
+            with ThreadPoolExecutor(max_workers=options.get("object_threads")) as executor:
+                futures = {
+                    executor.submit(download_w_config, file_to_download): file_to_download
+                    for file_to_download in files_to_download
+                }
+                for fut in as_completed(futures.keys()):
                     try:
-                        result = result_iter.next(0xFFFF)
-                        if result['success']:
-                            dl.add_result(result)
-                            downloaded['completed'].append(result)
-                        else:
-                            downloaded['failed'].append(result)
-                    except StopIteration:
-                        break
-                pool.close()
-            except BaseException:
-                pool.terminate()
-                raise
-            finally:
-                pool.join()
-
-        if downloaded['failed']:
-            raise exceptions.FailedDownloadError('an error occurred while downloading', downloaded)
+                        result = fut.result()
+                    except Exception as e:
+                        raise exceptions.FailedDownloadError(
+                            "An exception occured while attempting to download file "
+                            f'{futures[fut]["source"]}: {e}'
+                        )
+
+                    if result["success"]:
+                        dl.add_result(result)
+                        downloaded["completed"].append(result)
+                    else:
+                        downloaded["failed"].append(result)
+
+        if downloaded["failed"]:
+            raise exceptions.FailedDownloadError(
+                f"An error occurred while downloading the following files: {downloaded}"
+            )
 
         utils.check_condition(condition, [r['source'] for r in downloaded['completed']])
         return downloaded
 
     def _upload_object(self, upload_obj, config=None):
         """Upload a single object given an OBSUploadObject."""
         if utils.has_trailing_slash(upload_obj.object_name):
@@ -719,37 +721,38 @@
             'max_concurrency': options.get('segment_threads'),
             'multipart_chunksize': segment_size
         }
         upload_w_config = partial(self._upload_object, config=transfer_config)
 
         uploaded = {'completed': [], 'failed': []}
         with S3UploadLogger(len(files_to_upload)) as ul:
-            pool = ThreadPool(options['object_threads'])
-            try:
-                result_iter = pool.imap_unordered(upload_w_config, files_to_upload)
-                while True:
+            with ThreadPoolExecutor(max_workers=options.get("object_threads")) as executor:
+                futures = {
+                    executor.submit(upload_w_config, file_to_upload): file_to_upload
+                    for file_to_upload in files_to_upload
+                }
+                for fut in as_completed(futures.keys()):
                     try:
-                        result = result_iter.next(0xFFFF)
-                        if result['success']:
-                            ul.add_result(result)
-                            uploaded['completed'].append(result)
-                        else:
-                            uploaded['failed'].append(result)
-                    except StopIteration:
-                        break
-                pool.close()
-            except BaseException:
-                pool.terminate()
-                raise
-            finally:
-                pool.join()
+                        result = fut.result()
+                    except Exception as e:
+                        raise exceptions.FailedUploadError(
+                            "An exception occured while attempting to upload file "
+                            f"{futures[fut].source}: {e}"
+                        )
+
+                    if result["success"]:
+                        ul.add_result(result)
+                        uploaded["completed"].append(result)
+                    else:
+                        uploaded["failed"].append(result)
 
         if uploaded['failed']:
             raise exceptions.FailedUploadError(
-                'an error occurred while uploading, info={info}'.format(info=uploaded))
+                f"An error occurred while uploading the following files: {uploaded}"
+            )
 
         utils.check_condition(condition, [r['dest'] for r in uploaded['completed']])
         return uploaded
 
     def to_url(self):
         """Returns HTTP url for object (virtual host-style)"""
         return u'https://{bucket}.s3.amazonaws.com/{key}'.format(bucket=self.bucket,
```

### Comparing `stor-4.0.2/stor/settings.py` & `stor-4.1.0/stor/settings.py`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/stor-completion.bash` & `stor-4.1.0/stor/stor-completion.bash`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/swift.py` & `stor-4.1.0/stor/swift.py`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/test.py` & `stor-4.1.0/stor/test.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,19 @@
+from concurrent.futures import Executor
 import inspect
-import unittest
 import os
 import sys
+from threading import Lock
+import unittest
+from unittest import mock
 import uuid
 
 import dxpy
 import vcr
 
-from unittest import mock
-
 from stor import Path
 from stor import s3
 from stor.s3 import S3Path
 from stor.swift import SwiftPath
 from stor import settings
 
 
@@ -260,14 +261,18 @@
         self.setup_s3_mocks()
         try:
             del s3._thread_local.s3_transfer
             del s3._thread_local.s3_transfer_config
         except AttributeError:
             pass
 
+    def tearDown(self):
+        super(S3TestCase, self).tearDown()
+        self.doCleanups()
+
 
 class DXTestCase(DXTestMixin, unittest.TestCase):
     """A TestCase class that sets up DNAnexus vars and provides additional assertions.
 
     Since DXTestCase inherits from DXTestMixin, all the tests under DXTestCase are
     auto-wrapped with VCRpy, and hence use cassettes for playback.
     Look into `DXTestMixin` to turn off VCRpy and additional details.
@@ -341,7 +346,66 @@
     def teardown_posix_files(self):
         posix_p = Path('./{test_folder}'.format(test_folder=self.project))
         posix_p.rmtree()
 
     def teardown_project(self):
         self.project_handler.destroy()
         self.project_handler = None
+
+
+class MockFuture():
+    """A class to minimally mock methods for Future objects in ThreadPoolExecutor.
+
+    This mock Future class returns a completed result immediately to prevent test hanging.
+    'dest' and 'source' keys are expected in the inputs provided to set the result value;
+    this follows the result construction of Futures in file download and upload."""
+    def __init__(self, **kwargs):
+        self.__result = {
+            "success": "complete",
+            "dest": kwargs.get("dest"),
+            "source": kwargs.get("source")
+        }
+
+    def result(self):
+        return self.__result
+
+
+class MockExecutor(Executor):
+    """An Executor class to minimally mock methods for ThreadPoolExecutor.
+
+    This mock executor returns mock Future objects to avoid additional complexity in creating a
+    queue and executing passed-in functions. This prevents unit tests from hanging."""
+    def __init__(self):
+        self._shutdown = False
+        self._shutdownLock = Lock()
+
+    def submit(self, fn, *args, **kwargs):
+        """Mock the executor.submit function to immediately return a done mocked Future.
+
+        Does not implement a work queue nor use the passed in function to calculate results.
+        Based on the object submitted for the job, the Future will have specific dict keys to
+        be used in testing to confirm used of the upload/download information passed in.
+        The object submitted for download is a dict with keys "source" and "dest".
+        The object submitted for upload is an OBSUploadObject.
+
+        Args:
+            fn: function used to get a result value
+            args: args to be passed into fn
+            kwargs: kwargs to be passed into fn
+
+        Returns:
+            MockFuture: a mock Future class with a completed result containing a success status,
+                a source value, and a dest value
+        """
+        obj = args[0]
+        if isinstance(obj, dict):
+            dest = obj.get("dest")
+            source = obj.get("source")
+        else:
+            dest = None
+            source = obj.source
+
+        return MockFuture(dest=dest, source=source)
+
+    def shutdown(self, wait=True):
+        with self._shutdownLock:
+            self._shutdown = True
```

### Comparing `stor-4.0.2/stor/tests/cassettes_py3/TestCanonicalProject/test_canonical_path.yaml` & `stor-4.1.0/stor/tests/cassettes_py3/TestCanonicalProject/test_canonical_path.yaml`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/tests/cassettes_py3/TestCanonicalProject/test_canonical_path_on_dir.yaml` & `stor-4.1.0/stor/tests/cassettes_py3/TestCanonicalProject/test_canonical_path_on_dir.yaml`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/tests/cassettes_py3/TestCanonicalProject/test_duplicate_projects.yaml` & `stor-4.1.0/stor/tests/cassettes_py3/TestCanonicalProject/test_duplicate_projects.yaml`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/tests/cassettes_py3/TestCanonicalProject/test_no_project.yaml` & `stor-4.1.0/stor/tests/cassettes_py3/TestCanonicalProject/test_no_project.yaml`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/tests/cassettes_py3/TestCanonicalProject/test_unique_project.yaml` & `stor-4.1.0/stor/tests/cassettes_py3/TestCanonicalProject/test_unique_project.yaml`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/tests/cassettes_py3/TestCanonicalResource/test_duplicate_resource.yaml` & `stor-4.1.0/stor/tests/cassettes_py3/TestCanonicalResource/test_duplicate_resource.yaml`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/tests/cassettes_py3/TestCanonicalResource/test_no_resource.yaml` & `stor-4.1.0/stor/tests/cassettes_py3/TestCanonicalResource/test_no_resource.yaml`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/tests/cassettes_py3/TestCanonicalResource/test_project.yaml` & `stor-4.1.0/stor/tests/cassettes_py3/TestCanonicalResource/test_project.yaml`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/tests/cassettes_py3/TestCanonicalResource/test_unique_resource.yaml` & `stor-4.1.0/stor/tests/cassettes_py3/TestCanonicalResource/test_unique_resource.yaml`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/tests/cassettes_py3/TestCanonicalResource/test_virtual_on_virtual.yaml` & `stor-4.1.0/stor/tests/cassettes_py3/TestCanonicalResource/test_virtual_on_virtual.yaml`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/tests/cassettes_py3/TestCopy/test_clone_move_project_fail.yaml` & `stor-4.1.0/stor/tests/cassettes_py3/TestCopy/test_clone_move_project_fail.yaml`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/tests/cassettes_py3/TestCopy/test_clone_within_project_fail.yaml` & `stor-4.1.0/stor/tests/cassettes_py3/TestCopy/test_clone_within_project_fail.yaml`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/tests/cassettes_py3/TestCopy/test_dx_canonical_to_dx_file.yaml` & `stor-4.1.0/stor/tests/cassettes_py3/TestCopy/test_dx_canonical_to_dx_file.yaml`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/tests/cassettes_py3/TestCopy/test_dx_dir_to_posix_error.yaml` & `stor-4.1.0/stor/tests/cassettes_py3/TestCopy/test_dx_dir_to_posix_error.yaml`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/tests/cassettes_py3/TestCopy/test_dx_to_dx_diff_project_exist_file.yaml` & `stor-4.1.0/stor/tests/cassettes_py3/TestCopy/test_dx_to_dx_diff_project_exist_file.yaml`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/tests/cassettes_py3/TestCopy/test_dx_to_dx_file.yaml` & `stor-4.1.0/stor/tests/cassettes_py3/TestCopy/test_dx_to_dx_file.yaml`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/tests/cassettes_py3/TestCopy/test_dx_to_dx_file_folder_no_ext.yaml` & `stor-4.1.0/stor/tests/cassettes_py3/TestCopy/test_dx_to_dx_file_folder_no_ext.yaml`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/tests/cassettes_py3/TestCopy/test_dx_to_dx_folder.yaml` & `stor-4.1.0/stor/tests/cassettes_py3/TestCopy/test_dx_to_dx_folder.yaml`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/tests/cassettes_py3/TestCopy/test_dx_to_dx_same_project_exist_dest.yaml` & `stor-4.1.0/stor/tests/cassettes_py3/TestCopy/test_dx_to_dx_same_project_exist_dest.yaml`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/tests/cassettes_py3/TestCopy/test_dx_to_dx_within_project_fail.yaml` & `stor-4.1.0/stor/tests/cassettes_py3/TestCopy/test_dx_to_dx_within_project_fail.yaml`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/tests/cassettes_py3/TestCopy/test_dx_to_dx_within_project_pass.yaml` & `stor-4.1.0/stor/tests/cassettes_py3/TestCopy/test_dx_to_dx_within_project_pass.yaml`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/tests/cassettes_py3/TestCopy/test_dx_to_other_obs.yaml` & `stor-4.1.0/stor/tests/cassettes_py3/TestCopy/test_dx_to_other_obs.yaml`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/tests/cassettes_py3/TestCopy/test_dx_to_posix_file.yaml` & `stor-4.1.0/stor/tests/cassettes_py3/TestCopy/test_dx_to_posix_file.yaml`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/tests/cassettes_py3/TestCopy/test_dx_to_posix_file_folder_no_ext.yaml` & `stor-4.1.0/stor/tests/cassettes_py3/TestCopy/test_dx_to_posix_file_folder_no_ext.yaml`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/tests/cassettes_py3/TestCopy/test_dx_to_posix_folder.yaml` & `stor-4.1.0/stor/tests/cassettes_py3/TestCopy/test_dx_to_posix_folder.yaml`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/tests/cassettes_py3/TestCopy/test_dx_to_same_dx_pass.yaml` & `stor-4.1.0/stor/tests/cassettes_py3/TestCopy/test_dx_to_same_dx_pass.yaml`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/tests/cassettes_py3/TestCopy/test_move_diff_project_fail.yaml` & `stor-4.1.0/stor/tests/cassettes_py3/TestCopy/test_move_diff_project_fail.yaml`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/tests/cassettes_py3/TestCopy/test_other_obs_to_dx.yaml` & `stor-4.1.0/stor/tests/cassettes_py3/TestCopy/test_other_obs_to_dx.yaml`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/tests/cassettes_py3/TestCopy/test_posix_to_dx_fail.yaml` & `stor-4.1.0/stor/tests/cassettes_py3/TestCopy/test_posix_to_dx_fail.yaml`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/tests/cassettes_py3/TestCopy/test_posix_to_dx_file.yaml` & `stor-4.1.0/stor/tests/cassettes_py3/TestCopy/test_posix_to_dx_file.yaml`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/tests/cassettes_py3/TestCopy/test_posix_to_dx_file_folder_no_ext.yaml` & `stor-4.1.0/stor/tests/cassettes_py3/TestCopy/test_posix_to_dx_file_folder_no_ext.yaml`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/tests/cassettes_py3/TestCopy/test_posix_to_dx_folder.yaml` & `stor-4.1.0/stor/tests/cassettes_py3/TestCopy/test_posix_to_dx_folder.yaml`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/tests/cassettes_py3/TestCopy/test_posix_to_existing_dx.yaml` & `stor-4.1.0/stor/tests/cassettes_py3/TestCopy/test_posix_to_existing_dx.yaml`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/tests/cassettes_py3/TestCopyTree/test_clonetree_within_project_fail.yaml` & `stor-4.1.0/stor/tests/cassettes_py3/TestCopyTree/test_clonetree_within_project_fail.yaml`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/tests/cassettes_py3/TestCopyTree/test_dx_dir_to_dx_dir.yaml` & `stor-4.1.0/stor/tests/cassettes_py3/TestCopyTree/test_dx_dir_to_dx_dir.yaml`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/tests/cassettes_py3/TestCopyTree/test_dx_dir_to_dx_dir_same_project.yaml` & `stor-4.1.0/stor/tests/cassettes_py3/TestCopyTree/test_dx_dir_to_dx_dir_same_project.yaml`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/tests/cassettes_py3/TestCopyTree/test_dx_dir_to_dx_dir_same_project_fail.yaml` & `stor-4.1.0/stor/tests/cassettes_py3/TestCopyTree/test_dx_dir_to_dx_dir_same_project_fail.yaml`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/tests/cassettes_py3/TestCopyTree/test_dx_dir_to_dx_dir_w_slash.yaml` & `stor-4.1.0/stor/tests/cassettes_py3/TestCopyTree/test_dx_dir_to_dx_dir_w_slash.yaml`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/tests/cassettes_py3/TestCopyTree/test_dx_dir_to_dx_existing_dir.yaml` & `stor-4.1.0/stor/tests/cassettes_py3/TestCopyTree/test_dx_dir_to_dx_existing_dir.yaml`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/tests/cassettes_py3/TestCopyTree/test_dx_dir_to_dx_root.yaml` & `stor-4.1.0/stor/tests/cassettes_py3/TestCopyTree/test_dx_dir_to_dx_root.yaml`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/tests/cassettes_py3/TestCopyTree/test_dx_dir_to_dx_root_same_project.yaml` & `stor-4.1.0/stor/tests/cassettes_py3/TestCopyTree/test_dx_dir_to_dx_root_same_project.yaml`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/tests/cassettes_py3/TestCopyTree/test_dx_dir_to_posix.yaml` & `stor-4.1.0/stor/tests/cassettes_py3/TestCopyTree/test_dx_dir_to_posix.yaml`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/tests/cassettes_py3/TestCopyTree/test_dx_file_to_posix.yaml` & `stor-4.1.0/stor/tests/cassettes_py3/TestCopyTree/test_dx_file_to_posix.yaml`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/tests/cassettes_py3/TestCopyTree/test_dx_root_to_dx_dir.yaml` & `stor-4.1.0/stor/tests/cassettes_py3/TestCopyTree/test_dx_root_to_dx_dir.yaml`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/tests/cassettes_py3/TestCopyTree/test_dx_root_to_dx_dir_same_project.yaml` & `stor-4.1.0/stor/tests/cassettes_py3/TestCopyTree/test_dx_root_to_dx_dir_same_project.yaml`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/tests/cassettes_py3/TestCopyTree/test_dx_root_to_dx_dir_w_slash.yaml` & `stor-4.1.0/stor/tests/cassettes_py3/TestCopyTree/test_dx_root_to_dx_dir_w_slash.yaml`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/tests/cassettes_py3/TestCopyTree/test_dx_root_to_dx_root.yaml` & `stor-4.1.0/stor/tests/cassettes_py3/TestCopyTree/test_dx_root_to_dx_root.yaml`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/tests/cassettes_py3/TestCopyTree/test_dx_root_to_existing_dx_dir.yaml` & `stor-4.1.0/stor/tests/cassettes_py3/TestCopyTree/test_dx_root_to_existing_dx_dir.yaml`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/tests/cassettes_py3/TestCopyTree/test_dx_to_existing_dx_dest_fail.yaml` & `stor-4.1.0/stor/tests/cassettes_py3/TestCopyTree/test_dx_to_existing_dx_dest_fail.yaml`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/tests/cassettes_py3/TestCopyTree/test_dx_to_other_obs.yaml` & `stor-4.1.0/stor/tests/cassettes_py3/TestCopyTree/test_dx_to_other_obs.yaml`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/tests/cassettes_py3/TestCopyTree/test_dx_to_same_dx_pass.yaml` & `stor-4.1.0/stor/tests/cassettes_py3/TestCopyTree/test_dx_to_same_dx_pass.yaml`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/tests/cassettes_py3/TestCopyTree/test_move_diff_project_fail.yaml` & `stor-4.1.0/stor/tests/cassettes_py3/TestCopyTree/test_move_diff_project_fail.yaml`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/tests/cassettes_py3/TestCopyTree/test_move_root_within_project_fail.yaml` & `stor-4.1.0/stor/tests/cassettes_py3/TestCopyTree/test_move_root_within_project_fail.yaml`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/tests/cassettes_py3/TestCopyTree/test_nonexistent_dir.yaml` & `stor-4.1.0/stor/tests/cassettes_py3/TestCopyTree/test_nonexistent_dir.yaml`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/tests/cassettes_py3/TestCopyTree/test_other_obs_to_dx.yaml` & `stor-4.1.0/stor/tests/cassettes_py3/TestCopyTree/test_other_obs_to_dx.yaml`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/tests/cassettes_py3/TestCopyTree/test_posix_dir_to_dx.yaml` & `stor-4.1.0/stor/tests/cassettes_py3/TestCopyTree/test_posix_dir_to_dx.yaml`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/tests/cassettes_py3/TestCopyTree/test_posix_dir_to_dx_existing.yaml` & `stor-4.1.0/stor/tests/cassettes_py3/TestCopyTree/test_posix_dir_to_dx_existing.yaml`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/tests/cassettes_py3/TestCopyTree/test_posix_dir_to_dx_fail.yaml` & `stor-4.1.0/stor/tests/cassettes_py3/TestCopyTree/test_posix_dir_to_dx_fail.yaml`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/tests/cassettes_py3/TestCopyTree/test_posix_dir_to_dx_nested.yaml` & `stor-4.1.0/stor/tests/cassettes_py3/TestCopyTree/test_posix_dir_to_dx_nested.yaml`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/tests/cassettes_py3/TestCopyTree/test_posix_file_to_dx.yaml` & `stor-4.1.0/stor/tests/cassettes_py3/TestCopyTree/test_posix_file_to_dx.yaml`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/tests/cassettes_py3/TestDownloadObjects/test_absolute_paths.yaml` & `stor-4.1.0/stor/tests/cassettes_py3/TestDownloadObjects/test_absolute_paths.yaml`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/tests/cassettes_py3/TestDownloadObjects/test_local_paths.yaml` & `stor-4.1.0/stor/tests/cassettes_py3/TestDownloadObjects/test_local_paths.yaml`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/tests/cassettes_py3/TestExists/test_false_canonical_path.yaml` & `stor-4.1.0/stor/tests/cassettes_py3/TestExists/test_false_canonical_path.yaml`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/tests/cassettes_py3/TestExists/test_false_canonical_project.yaml` & `stor-4.1.0/stor/tests/cassettes_py3/TestExists/test_false_canonical_project.yaml`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/tests/cassettes_py3/TestExists/test_false_file.yaml` & `stor-4.1.0/stor/tests/cassettes_py3/TestExists/test_false_file.yaml`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/tests/cassettes_py3/TestExists/test_false_folder.yaml` & `stor-4.1.0/stor/tests/cassettes_py3/TestExists/test_false_folder.yaml`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/tests/cassettes_py3/TestExists/test_false_mixed_path.yaml` & `stor-4.1.0/stor/tests/cassettes_py3/TestExists/test_false_mixed_path.yaml`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/tests/cassettes_py3/TestExists/test_project_does_not_exist.yaml` & `stor-4.1.0/stor/tests/cassettes_py3/TestExists/test_project_does_not_exist.yaml`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/tests/cassettes_py3/TestExists/test_true_canonical_path.yaml` & `stor-4.1.0/stor/tests/cassettes_py3/TestExists/test_true_canonical_path.yaml`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/tests/cassettes_py3/TestExists/test_true_canonical_project.yaml` & `stor-4.1.0/stor/tests/cassettes_py3/TestExists/test_true_canonical_project.yaml`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/tests/cassettes_py3/TestExists/test_true_dir_with_object.yaml` & `stor-4.1.0/stor/tests/cassettes_py3/TestExists/test_true_dir_with_object.yaml`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/tests/cassettes_py3/TestExists/test_true_empty_dir.yaml` & `stor-4.1.0/stor/tests/cassettes_py3/TestExists/test_true_empty_dir.yaml`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/tests/cassettes_py3/TestExists/test_true_file.yaml` & `stor-4.1.0/stor/tests/cassettes_py3/TestExists/test_true_file.yaml`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/tests/cassettes_py3/TestExists/test_true_mixed_path.yaml` & `stor-4.1.0/stor/tests/cassettes_py3/TestExists/test_true_mixed_path.yaml`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/tests/cassettes_py3/TestGetSize/test_file.yaml` & `stor-4.1.0/stor/tests/cassettes_py3/TestGetSize/test_file.yaml`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/tests/cassettes_py3/TestGetSize/test_folder.yaml` & `stor-4.1.0/stor/tests/cassettes_py3/TestGetSize/test_folder.yaml`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/tests/cassettes_py3/TestGetSize/test_project.yaml` & `stor-4.1.0/stor/tests/cassettes_py3/TestGetSize/test_project.yaml`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/tests/cassettes_py3/TestGlob/test_cond_no_met.yaml` & `stor-4.1.0/stor/tests/cassettes_py3/TestGlob/test_cond_no_met.yaml`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/tests/cassettes_py3/TestGlob/test_glob_cond_met.yaml` & `stor-4.1.0/stor/tests/cassettes_py3/TestGlob/test_glob_cond_met.yaml`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/tests/cassettes_py3/TestGlob/test_pattern_no_file_match.yaml` & `stor-4.1.0/stor/tests/cassettes_py3/TestGlob/test_pattern_no_file_match.yaml`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/tests/cassettes_py3/TestGlob/test_prefix_pattern.yaml` & `stor-4.1.0/stor/tests/cassettes_py3/TestGlob/test_prefix_pattern.yaml`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/tests/cassettes_py3/TestGlob/test_suffix_pattern.yaml` & `stor-4.1.0/stor/tests/cassettes_py3/TestGlob/test_suffix_pattern.yaml`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/tests/cassettes_py3/TestGlob/test_valid_pattern.yaml` & `stor-4.1.0/stor/tests/cassettes_py3/TestGlob/test_valid_pattern.yaml`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/tests/cassettes_py3/TestGlob/test_valid_pattern_wo_wildcard.yaml` & `stor-4.1.0/stor/tests/cassettes_py3/TestGlob/test_valid_pattern_wo_wildcard.yaml`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/tests/cassettes_py3/TestList/test_list_absent_folder.yaml` & `stor-4.1.0/stor/tests/cassettes_py3/TestList/test_list_absent_folder.yaml`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/tests/cassettes_py3/TestList/test_list_canonical.yaml` & `stor-4.1.0/stor/tests/cassettes_py3/TestList/test_list_canonical.yaml`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/tests/cassettes_py3/TestList/test_list_empty_folder.yaml` & `stor-4.1.0/stor/tests/cassettes_py3/TestList/test_list_empty_folder.yaml`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/tests/cassettes_py3/TestList/test_list_fail_w_condition.yaml` & `stor-4.1.0/stor/tests/cassettes_py3/TestList/test_list_fail_w_condition.yaml`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/tests/cassettes_py3/TestList/test_list_file.yaml` & `stor-4.1.0/stor/tests/cassettes_py3/TestList/test_list_file.yaml`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/tests/cassettes_py3/TestList/test_list_folder_share_filename.yaml` & `stor-4.1.0/stor/tests/cassettes_py3/TestList/test_list_folder_share_filename.yaml`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/tests/cassettes_py3/TestList/test_list_folder_w_files.yaml` & `stor-4.1.0/stor/tests/cassettes_py3/TestList/test_list_folder_w_files.yaml`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/tests/cassettes_py3/TestList/test_list_iter_canon_on_canon.yaml` & `stor-4.1.0/stor/tests/cassettes_py3/TestList/test_list_iter_canon_on_canon.yaml`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/tests/cassettes_py3/TestList/test_list_iter_project.yaml` & `stor-4.1.0/stor/tests/cassettes_py3/TestList/test_list_iter_project.yaml`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/tests/cassettes_py3/TestList/test_list_limit.yaml` & `stor-4.1.0/stor/tests/cassettes_py3/TestList/test_list_limit.yaml`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/tests/cassettes_py3/TestList/test_list_on_canonical_project.yaml` & `stor-4.1.0/stor/tests/cassettes_py3/TestList/test_list_on_canonical_project.yaml`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/tests/cassettes_py3/TestList/test_list_on_canonical_resource.yaml` & `stor-4.1.0/stor/tests/cassettes_py3/TestList/test_list_on_canonical_resource.yaml`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/tests/cassettes_py3/TestList/test_list_project.yaml` & `stor-4.1.0/stor/tests/cassettes_py3/TestList/test_list_project.yaml`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/tests/cassettes_py3/TestList/test_list_starts_with.yaml` & `stor-4.1.0/stor/tests/cassettes_py3/TestList/test_list_starts_with.yaml`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/tests/cassettes_py3/TestList/test_list_w_category.yaml` & `stor-4.1.0/stor/tests/cassettes_py3/TestList/test_list_w_category.yaml`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/tests/cassettes_py3/TestList/test_list_w_condition.yaml` & `stor-4.1.0/stor/tests/cassettes_py3/TestList/test_list_w_condition.yaml`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/tests/cassettes_py3/TestListDir/test_listdir_absent_folder.yaml` & `stor-4.1.0/stor/tests/cassettes_py3/TestListDir/test_listdir_absent_folder.yaml`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/tests/cassettes_py3/TestListDir/test_listdir_canonical.yaml` & `stor-4.1.0/stor/tests/cassettes_py3/TestListDir/test_listdir_canonical.yaml`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/tests/cassettes_py3/TestListDir/test_listdir_empty_folder.yaml` & `stor-4.1.0/stor/tests/cassettes_py3/TestListDir/test_listdir_empty_folder.yaml`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/tests/cassettes_py3/TestListDir/test_listdir_file.yaml` & `stor-4.1.0/stor/tests/cassettes_py3/TestListDir/test_listdir_file.yaml`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/tests/cassettes_py3/TestListDir/test_listdir_folder_share_filename.yaml` & `stor-4.1.0/stor/tests/cassettes_py3/TestListDir/test_listdir_folder_share_filename.yaml`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/tests/cassettes_py3/TestListDir/test_listdir_folder_w_file.yaml` & `stor-4.1.0/stor/tests/cassettes_py3/TestListDir/test_listdir_folder_w_file.yaml`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/tests/cassettes_py3/TestListDir/test_listdir_iter_canon_on_canon.yaml` & `stor-4.1.0/stor/tests/cassettes_py3/TestListDir/test_listdir_iter_canon_on_canon.yaml`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/tests/cassettes_py3/TestListDir/test_listdir_iter_project.yaml` & `stor-4.1.0/stor/tests/cassettes_py3/TestListDir/test_listdir_iter_project.yaml`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/tests/cassettes_py3/TestListDir/test_listdir_on_canonical_project.yaml` & `stor-4.1.0/stor/tests/cassettes_py3/TestListDir/test_listdir_on_canonical_project.yaml`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/tests/cassettes_py3/TestListDir/test_listdir_on_canonical_resource.yaml` & `stor-4.1.0/stor/tests/cassettes_py3/TestListDir/test_listdir_on_canonical_resource.yaml`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/tests/cassettes_py3/TestListDir/test_listdir_project.yaml` & `stor-4.1.0/stor/tests/cassettes_py3/TestListDir/test_listdir_project.yaml`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/tests/cassettes_py3/TestLoginAuth/test_login_auth.yaml` & `stor-4.1.0/stor/tests/cassettes_py3/TestLoginAuth/test_login_auth.yaml`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/tests/cassettes_py3/TestMakedirsP/test_makedirs_p_folder.yaml` & `stor-4.1.0/stor/tests/cassettes_py3/TestMakedirsP/test_makedirs_p_folder.yaml`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/tests/cassettes_py3/TestMakedirsP/test_makedirs_p_folder_exists.yaml` & `stor-4.1.0/stor/tests/cassettes_py3/TestMakedirsP/test_makedirs_p_folder_exists.yaml`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/tests/cassettes_py3/TestMakedirsP/test_makedirs_p_nested_folder.yaml` & `stor-4.1.0/stor/tests/cassettes_py3/TestMakedirsP/test_makedirs_p_nested_folder.yaml`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/tests/cassettes_py3/TestMakedirsP/test_makedirs_p_project.yaml` & `stor-4.1.0/stor/tests/cassettes_py3/TestMakedirsP/test_makedirs_p_project.yaml`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/tests/cassettes_py3/TestMakedirsP/test_makedirs_p_project_exists.yaml` & `stor-4.1.0/stor/tests/cassettes_py3/TestMakedirsP/test_makedirs_p_project_exists.yaml`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/tests/cassettes_py3/TestOpen/test_append_mode_fail.yaml` & `stor-4.1.0/stor/tests/cassettes_py3/TestOpen/test_append_mode_fail.yaml`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/tests/cassettes_py3/TestOpen/test_read_dir_fail.yaml` & `stor-4.1.0/stor/tests/cassettes_py3/TestOpen/test_read_dir_fail.yaml`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/tests/cassettes_py3/TestOpen/test_read_fail_on_closed_buffer.yaml` & `stor-4.1.0/stor/tests/cassettes_py3/TestOpen/test_read_fail_on_closed_buffer.yaml`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/tests/cassettes_py3/TestOpen/test_read_on_open_buffer.yaml` & `stor-4.1.0/stor/tests/cassettes_py3/TestOpen/test_read_on_open_buffer.yaml`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/tests/cassettes_py3/TestOpen/test_read_on_open_dx_file.yaml` & `stor-4.1.0/stor/tests/cassettes_py3/TestOpen/test_read_on_open_dx_file.yaml`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/tests/cassettes_py3/TestOpen/test_valid_and_invalid_encoding_for_dnanexus.yaml` & `stor-4.1.0/stor/tests/cassettes_py3/TestOpen/test_valid_and_invalid_encoding_for_dnanexus.yaml`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/tests/cassettes_py3/TestOpen/test_write_multiple_flush_multiple_upload.yaml` & `stor-4.1.0/stor/tests/cassettes_py3/TestOpen/test_write_multiple_flush_multiple_upload.yaml`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/tests/cassettes_py3/TestOpen/test_write_multiple_wo_context_manager.yaml` & `stor-4.1.0/stor/tests/cassettes_py3/TestOpen/test_write_multiple_wo_context_manager.yaml`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/tests/cassettes_py3/TestOpen/test_write_read_over_files.yaml` & `stor-4.1.0/stor/tests/cassettes_py3/TestOpen/test_write_read_over_files.yaml`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/tests/cassettes_py3/TestOpen/test_write_to_project_fail.yaml` & `stor-4.1.0/stor/tests/cassettes_py3/TestOpen/test_write_to_project_fail.yaml`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/tests/cassettes_py3/TestOpen/test_write_w_settings_big_timeout.yaml` & `stor-4.1.0/stor/tests/cassettes_py3/TestOpen/test_write_w_settings_big_timeout.yaml`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/tests/cassettes_py3/TestOpen/test_write_w_settings_no_timeout.yaml` & `stor-4.1.0/stor/tests/cassettes_py3/TestOpen/test_write_w_settings_no_timeout.yaml`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/tests/cassettes_py3/TestRemove/test_fail_remove_folder.yaml` & `stor-4.1.0/stor/tests/cassettes_py3/TestRemove/test_fail_remove_folder.yaml`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/tests/cassettes_py3/TestRemove/test_fail_remove_nonexistent_file.yaml` & `stor-4.1.0/stor/tests/cassettes_py3/TestRemove/test_fail_remove_nonexistent_file.yaml`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/tests/cassettes_py3/TestRemove/test_fail_remove_nonexistent_project.yaml` & `stor-4.1.0/stor/tests/cassettes_py3/TestRemove/test_fail_remove_nonexistent_project.yaml`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/tests/cassettes_py3/TestRemove/test_fail_remove_project.yaml` & `stor-4.1.0/stor/tests/cassettes_py3/TestRemove/test_fail_remove_project.yaml`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/tests/cassettes_py3/TestRemove/test_fail_rmtree_file.yaml` & `stor-4.1.0/stor/tests/cassettes_py3/TestRemove/test_fail_rmtree_file.yaml`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/tests/cassettes_py3/TestRemove/test_remove_file.yaml` & `stor-4.1.0/stor/tests/cassettes_py3/TestRemove/test_remove_file.yaml`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/tests/cassettes_py3/TestRemove/test_rmtree_folder.yaml` & `stor-4.1.0/stor/tests/cassettes_py3/TestRemove/test_rmtree_folder.yaml`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/tests/cassettes_py3/TestRemove/test_rmtree_project.yaml` & `stor-4.1.0/stor/tests/cassettes_py3/TestRemove/test_rmtree_project.yaml`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/tests/cassettes_py3/TestRename/test_rename_file_pass.yaml` & `stor-4.1.0/stor/tests/cassettes_py3/TestRename/test_rename_file_pass.yaml`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/tests/cassettes_py3/TestRename/test_rename_folder_fail.yaml` & `stor-4.1.0/stor/tests/cassettes_py3/TestRename/test_rename_folder_fail.yaml`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/tests/cassettes_py3/TestRename/test_rename_to_self.yaml` & `stor-4.1.0/stor/tests/cassettes_py3/TestRename/test_rename_to_self.yaml`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/tests/cassettes_py3/TestStat/test_stat_canonical_project.yaml` & `stor-4.1.0/stor/tests/cassettes_py3/TestStat/test_stat_canonical_project.yaml`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/tests/cassettes_py3/TestStat/test_stat_canonical_resource.yaml` & `stor-4.1.0/stor/tests/cassettes_py3/TestStat/test_stat_canonical_resource.yaml`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/tests/cassettes_py3/TestStat/test_stat_file.yaml` & `stor-4.1.0/stor/tests/cassettes_py3/TestStat/test_stat_file.yaml`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/tests/cassettes_py3/TestStat/test_stat_folder.yaml` & `stor-4.1.0/stor/tests/cassettes_py3/TestStat/test_stat_folder.yaml`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/tests/cassettes_py3/TestStat/test_stat_project_error.yaml` & `stor-4.1.0/stor/tests/cassettes_py3/TestStat/test_stat_project_error.yaml`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/tests/cassettes_py3/TestStat/test_stat_virtual_project.yaml` & `stor-4.1.0/stor/tests/cassettes_py3/TestStat/test_stat_virtual_project.yaml`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/tests/cassettes_py3/TestTempUrl/test_fail_on_folder.yaml` & `stor-4.1.0/stor/tests/cassettes_py3/TestTempUrl/test_fail_on_folder.yaml`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/tests/cassettes_py3/TestTempUrl/test_fail_on_project.yaml` & `stor-4.1.0/stor/tests/cassettes_py3/TestTempUrl/test_fail_on_project.yaml`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/tests/cassettes_py3/TestTempUrl/test_on_file.yaml` & `stor-4.1.0/stor/tests/cassettes_py3/TestTempUrl/test_on_file.yaml`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/tests/cassettes_py3/TestTempUrl/test_on_file_canonical.yaml` & `stor-4.1.0/stor/tests/cassettes_py3/TestTempUrl/test_on_file_canonical.yaml`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/tests/cassettes_py3/TestTempUrl/test_on_file_named_timed.yaml` & `stor-4.1.0/stor/tests/cassettes_py3/TestTempUrl/test_on_file_named_timed.yaml`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/tests/cassettes_py3/TestTempUrl/test_on_file_with_proxy_url.yaml` & `stor-4.1.0/stor/tests/cassettes_py3/TestTempUrl/test_on_file_with_proxy_url.yaml`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/tests/cassettes_py3/TestUpload/test_upload_files_existing.yaml` & `stor-4.1.0/stor/tests/cassettes_py3/TestUpload/test_upload_files_existing.yaml`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/tests/cassettes_py3/TestWalkFiles/test_pattern_no_match.yaml` & `stor-4.1.0/stor/tests/cassettes_py3/TestWalkFiles/test_pattern_no_match.yaml`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/tests/cassettes_py3/TestWalkFiles/test_pattern_share_folder_match.yaml` & `stor-4.1.0/stor/tests/cassettes_py3/TestWalkFiles/test_pattern_share_folder_match.yaml`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/tests/cassettes_py3/TestWalkFiles/test_pattern_w_prefix.yaml` & `stor-4.1.0/stor/tests/cassettes_py3/TestWalkFiles/test_pattern_w_prefix.yaml`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/tests/cassettes_py3/TestWalkFiles/test_pattern_w_prefix_suffix.yaml` & `stor-4.1.0/stor/tests/cassettes_py3/TestWalkFiles/test_pattern_w_prefix_suffix.yaml`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/tests/cassettes_py3/TestWalkFiles/test_pattern_w_suffix.yaml` & `stor-4.1.0/stor/tests/cassettes_py3/TestWalkFiles/test_pattern_w_suffix.yaml`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/tests/file_data/s_3_2126.bcl.gz` & `stor-4.1.0/stor/tests/file_data/s_3_2126.bcl.gz`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/tests/shared_obs.py` & `stor-4.1.0/stor/tests/shared_obs.py`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/tests/test_cli.py` & `stor-4.1.0/stor/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/tests/test_dx.py` & `stor-4.1.0/stor/tests/test_dx.py`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/tests/test_dx_path_compat.py` & `stor-4.1.0/stor/tests/test_dx_path_compat.py`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/tests/test_extensions_swiftstack.py` & `stor-4.1.0/stor/tests/test_extensions_swiftstack.py`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/tests/test_integration.py` & `stor-4.1.0/stor/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/tests/test_integration_dx.py` & `stor-4.1.0/stor/tests/test_integration_dx.py`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/tests/test_integration_posix.py` & `stor-4.1.0/stor/tests/test_integration_posix.py`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/tests/test_integration_s3.py` & `stor-4.1.0/stor/tests/test_integration_s3.py`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/tests/test_integration_swift.py` & `stor-4.1.0/stor/tests/test_integration_swift.py`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/tests/test_posix.py` & `stor-4.1.0/stor/tests/test_posix.py`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/tests/test_posix_path_compat.py` & `stor-4.1.0/stor/tests/test_posix_path_compat.py`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/tests/test_s3.py` & `stor-4.1.0/stor/tests/test_s3.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from stor import exceptions
 from stor import NamedTemporaryDirectory
 from stor.obs import OBSUploadObject
 from stor import Path
 from stor import settings
 from stor import s3
 from stor.s3 import S3Path
-from stor.test import S3TestCase
+from stor.test import MockExecutor, S3TestCase
 from stor.tests.shared_obs import SharedOBSFileCases
 from stor import utils
 
 
 class TestBasicPathMethods(unittest.TestCase):
     def test_name(self):
         p = Path('s3://bucket/path/to/resource')
@@ -1081,27 +1081,47 @@
                                               use_manifest=True)
 
     def test_upload_w_use_manifest_single_file(self, mock_getsize, mock_files):
         with self.assertRaisesRegexp(ValueError, 'can only upload one directory'):
             S3Path('s3://bucket/path').upload(['file'],
                                               use_manifest=True)
 
-    @mock.patch('stor.s3.ThreadPool', autospec=True)
-    def test_upload_object_threads(self, mock_pool, mock_getsize, mock_files):
+    @mock.patch(
+        "stor.s3.as_completed",
+        autospec=True,
+        side_effect=lambda futures: [fut for fut in futures]
+    )
+    @mock.patch("stor.s3.ThreadPoolExecutor", autospec=True, return_value=MockExecutor())
+    def test_upload_object_threads(
+        self, mock_pool, mock_completed, mock_getsize, mock_files
+    ):
         mock_files.return_value = {
-            'file%s' % i: 20
+            f"file{i}": 20
             for i in range(20)
         }
         mock_getsize.return_value = 20
-        mock_pool.return_value.imap_unordered.return_value.next.side_effect = StopIteration
 
-        s3_p = S3Path('s3://bucket')
-        with settings.use({'s3:upload': {'object_threads': 20}}):
-            s3_p.upload(['test'])
-        mock_pool.assert_called_once_with(20)
+        s3_p = S3Path("s3://bucket")
+        with settings.use({"s3:upload": {"object_threads": 20}}):
+            s3_p.upload(["test"])
+
+        # confirm ThreadPoolExecutor called with expected args
+        mock_pool.assert_called_once_with(max_workers=20)
+
+        # confirm as_completed called with expected args
+        mock_completed.assert_called_once()
+        # check length of MockFutures list passed in to as_completed
+        mock_completed_called_with_futures = mock_completed.call_args[0][0]
+        assert len(mock_completed_called_with_futures) == 20
+        assert all(
+            [
+                fut.result()["dest"] is None and fut.result()["source"] == f"file{idx}"
+                for idx, fut in enumerate(mock_completed_called_with_futures)
+            ]
+        )
 
     def test_upload_remote_error(self, mock_getsize, mock_files):
         mock_files.return_value = {
             'file1': 20,
             'file2': 10
         }
         self.mock_s3_transfer.upload_file.side_effect = [
@@ -1111,19 +1131,22 @@
 
         with self.assertRaises(exceptions.FailedUploadError):
             S3Path('s3://bucket/path').upload(['test'])
 
     def test_upload_other_error(self, mock_getsize, mock_files):
         mock_files.return_value = {
             'file1': 20,
-            'file2': 10
+            'file2': 10,
         }
-        self.mock_s3_transfer.upload_file.side_effect = [None, ValueError]
+        self.mock_s3_transfer.upload_file.side_effect = [None, ValueError("Error information")]
 
-        with self.assertRaises(ValueError):
+        with self.assertRaisesRegex(
+            exceptions.FailedUploadError,
+            f"{list(mock_files.return_value.keys())[1]}"
+        ):
             S3Path('s3://bucket/path').upload(['test'])
 
     def test_upload_multipart_settings(self, mock_getsize, mock_files):
         mock_files.return_value = {
             'file1': 20,
             'file2': 10
         }
@@ -1271,27 +1294,50 @@
 
         s3_p = S3Path('s3://bucket')
         s3_p.download('test',
                       use_manifest=True,
                       condition=lambda results: len(results) == 3)
         self.assertEquals(self.mock_s3_transfer.download_file.call_count, 3)
 
-    @mock.patch.object(S3Path, 'list', autospec=True)
-    @mock.patch('stor.s3.ThreadPool', autospec=True)
-    def test_download_object_threads(self, mock_pool, mock_list, mock_getsize,
-                                     mock_make_dest_dir):
+    @mock.patch.object(S3Path, "list", autospec=True)
+    @mock.patch(
+        "stor.s3.as_completed",
+        autospec=True,
+        side_effect=lambda futures: [fut for fut in futures]
+    )
+    @mock.patch("stor.s3.ThreadPoolExecutor", autospec=True, return_value=MockExecutor())
+    def test_download_object_threads(
+        self, mock_pool, mock_completed, mock_list, mock_getsize, mock_make_dest_dir
+    ):
         mock_list.return_value = [
-            S3Path('s3://bucket/file%s' % i)
+            S3Path(f"s3://bucket/file{i}")
             for i in range(20)
         ]
-        mock_pool.return_value.imap_unordered.return_value.next.side_effect = StopIteration
-        s3_p = S3Path('s3://bucket')
-        with settings.use({'s3:download': {'object_threads': 20}}):
-            s3_p.download(['test'])
-        mock_pool.assert_called_once_with(20)
+        s3_p = S3Path("s3://bucket")
+
+        with settings.use({"s3:download": {"object_threads": 20}}):
+            s3_p.download(["test"])
+
+        # confirm ThreadPoolExecutor called with expected args
+        mock_pool.assert_called_once_with(max_workers=20)
+
+        # confirm as_completed called with expected args
+        mock_completed.assert_called_once()
+        # check length of MockFutures list passed in to as_completed
+        mock_completed_called_with_futures = mock_completed.call_args[0][0]
+        assert len(mock_completed_called_with_futures) == 20
+        assert all(
+            [
+                (
+                    fut.result()["dest"] == ["test"] and
+                    fut.result()["source"] == f"s3://bucket/file{idx}"
+                )
+                for idx, fut in enumerate(mock_completed_called_with_futures)
+            ]
+        )
 
     @mock.patch.object(S3Path, 'list', autospec=True)
     def test_download_remote_error(self, mock_list, mock_getsize, mock_make_dest_dir):
         mock_list.return_value = [
             S3Path('s3://bucket/my/obj1'),
             S3Path('s3://bucket/my/obj2'),
             S3Path('s3://bucket/my/obj3')
@@ -1302,19 +1348,21 @@
             S3Path('s3://bucket/path').download('test')
 
     @mock.patch.object(S3Path, 'list', autospec=True)
     def test_download_other_error(self, mock_list, mock_getsize, mock_make_dest_dir):
         mock_list.return_value = [
             S3Path('s3://bucket/my/obj1'),
             S3Path('s3://bucket/my/obj2'),
-            S3Path('s3://bucket/my/obj3')
         ]
-        self.mock_s3_transfer.download_file.side_effect = [None, ValueError]
+        self.mock_s3_transfer.download_file.side_effect = [None, ValueError("Error information")]
 
-        with self.assertRaises(ValueError):
+        with self.assertRaisesRegex(
+            exceptions.FailedDownloadError,
+            f"{mock_list.return_value[1]}"
+        ):
             S3Path('s3://bucket/path').download('test')
 
     @mock.patch.object(S3Path, 'list', autospec=True)
     def test_download_multipart_settings(self, mock_list, mock_getsize, mock_make_dest_dir):
         mock_list.return_value = [
             S3Path('s3://bucket/my/obj1'),
             S3Path('s3://bucket/my/obj2'),
```

### Comparing `stor-4.0.2/stor/tests/test_s3_path_compat.py` & `stor-4.1.0/stor/tests/test_s3_path_compat.py`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/tests/test_settings.py` & `stor-4.1.0/stor/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/tests/test_swift.py` & `stor-4.1.0/stor/tests/test_swift.py`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/tests/test_swift_path_compat.py` & `stor-4.1.0/stor/tests/test_swift_path_compat.py`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/tests/test_utils.py` & `stor-4.1.0/stor/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/tests/test_windows.py` & `stor-4.1.0/stor/tests/test_windows.py`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/third_party/backoff.py` & `stor-4.1.0/stor/third_party/backoff.py`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/stor/utils.py` & `stor-4.1.0/stor/utils.py`

 * *Files identical despite different names*

### Comparing `stor-4.0.2/setup.py` & `stor-4.1.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -38,17 +38,17 @@
  'requests>=2.20.0']
 
 entry_points = \
 {'console_scripts': ['stor = stor.cli:main']}
 
 setup_kwargs = {
     'name': 'stor',
-    'version': '4.0.2',
+    'version': '4.1.0',
     'description': 'Cross-compatible API for accessing Posix and OBS storage systems',
-    'long_description': 'stor\n====\n\n|Build Status|\n\n``stor`` provides a cross-compatible CLI and Python API for accessing\nblock and object storage. ``stor`` was created so you could write one\npiece of code to work with local or remote files, without needing to\nwrite specialized code to handle failure modes, retrying or temporarily\nsystem unavailability. The functional API (i.e., ``stor.copytree``,\n``stor.rmtree``, ``stor.remove``, ``stor.listdir``) will work with the\nsame semantics across all storage backends. This makes it really easy to\ndevelop/test code locally with files and then take advantage of robust\nand cheaper object storage when you push to remote.\n\nView full docs for stor at https://counsyl.github.io/stor/ .\n\nQuickstart\n----------\n\n::\n\n    pip install stor\n\n``stor`` provides both a CLI and a Python library for manipulating Posix\nand OBS with a single, cross-compatible API.\n\nQuickstart - CLI\n----------------\n\n::\n\n    usage: stor [-h] [-c CONFIG_FILE] [--version]\n                {list,ls,cp,rm,walkfiles,cat,cd,pwd,clear,url,convert-swiftstack}\n                ...\n\n    A command line interface for stor.\n\n    positional arguments:\n      {list,ls,cp,rm,walkfiles,cat,cd,pwd,clear,url,convert-swiftstack}\n        list                List contents using the path as a prefix.\n        ls                  List path as a directory.\n        cp                  Copy a source to a destination path.\n        rm                  Remove file at a path.\n        walkfiles           List all files under a path that match an optional\n                            pattern.\n        cat                 Output file contents to stdout.\n        cd                  Change directory to a given OBS path.\n        pwd                 Get the present working directory of a service or all\n                            current directories.\n        clear               Clear current directories of a specified service.\n        url                 generate URI for path\n        convert-swiftstack  convert swiftstack paths\n\n    optional arguments:\n      -h, --help            show this help message and exit\n      -c CONFIG_FILE, --config CONFIG_FILE\n                            File containing configuration settings.\n      --version             Print version\n\nYou can ``ls`` local and remote directories\n\n::\n\n    \xe2\x80\xba\xe2\x80\xba stor ls s3://stor-test-bucket\n    s3://stor-test-bucket/b.txt\n    s3://stor-test-bucket/counsyl-storage-utils\n    s3://stor-test-bucket/file_test.txt\n    s3://stor-test-bucket/counsyl-storage-utils/\n    s3://stor-test-bucket/empty/\n    s3://stor-test-bucket/lots_of_files/\n    s3://stor-test-bucket/small_test/\n\nCopy files locally or remotely or upload from stdin\n\n::\n\n    \xe2\x80\xba\xe2\x80\xba echo "HELLO WORLD" | stor cp - swift://AUTH_stor_test/hello_world.txt\n    starting upload of 1 objects\n    upload complete - 1/1   0:00:00 0.00 MB 0.00 MB/s\n    \xe2\x80\xba\xe2\x80\xba stor cat swift://AUTH_stor_test/hello_world.txt\n    HELLO WORLD\n    \xe2\x80\xba\xe2\x80\xba stor cp swift://AUTH_stor_test/hello_world.txt hello_world.txt\n    \xe2\x80\xba\xe2\x80\xba stor cat hello_world.txt\n    HELLO WORLD\n\nQuickstart - Python\n-------------------\n\nList files in a directory, taking advantage of delimiters\n\n.. code:: python\n\n    >>> stor.listdir(\'s3://bestbucket\')\n    [S3Path(\'s3://bestbucket/a/\')\n     S3Path(\'s3://bestbucket/b/\')]\n\nList all objects in a bucket\n\n.. code:: python\n\n    >>> stor.list(\'s3://bestbucket\')\n    [S3Path(\'s3://bestbucket/a/1.txt\')\n     S3Path(\'s3://bestbucket/a/2.txt\')\n     S3Path(\'s3://bestbucket/a/3.txt\')\n     S3Path(\'s3://bestbucket/b/1.txt\')]\n\nOr in a local path\n\n.. code:: python\n\n    >>> stor.list(\'stor\')\n    [PosixPath(\'stor/__init__.py\'),\n     PosixPath(\'stor/exceptions.pyc\'),\n     PosixPath(\'stor/tests/test_s3.py\'),\n     PosixPath(\'stor/tests/test_swift.py\'),\n     PosixPath(\'stor/tests/test_integration_swift.py\'),\n     PosixPath(\'stor/tests/test_utils.py\'),\n     PosixPath(\'stor/posix.pyc\'),\n     PosixPath(\'stor/base.py\'),\n\nRead and write files from POSIX or OBS, using python file objects.\n\n.. code:: python\n\n    import stor\n    with stor.open(\'/my/exciting.json\') as fp:\n        data1 = json.load(fp)\n\n    data1[\'read\'] = True\n\n    with stor.open(\'s3://bestbucket/exciting.json\') as fp:\n        json.dump(data1, fp)\n\nTesting code that uses stor\n---------------------------\n\nThe key design consideration of ``stor`` is that your code should be\nable to transparently use POSIX or any object storage system to read and\nupdate files. So, rather than use mocks, we suggest that you structure\nyour test code to point to local filesystem paths and restrict yourself\nto the functional API. E.g., in your prod settings, you could set\n``DATADIR = \'s3://bestbucketever\'``\\ and when you test, you could use\n``DATADIR = \'/somewhat/cool/path/to/test/data\'``, while your actual code\njust says:\n\n.. code:: python\n\n    with stor.open(stor.join(DATADIR, experiment)) as fp:\n        data = json.load(fp)\n\nEasy! and no mocks required!\n\nRunning the Tests\n-----------------\n\n::\n\n    make test\n\nContributing and Semantic Versioning\n------------------------------------\n\nWe use semantic versioning to communicate when we make API changes to\nthe library. See CONTRIBUTING.md for more details on contributing to\nstor.\n\n.. |Build Status| image:: https://travis-ci.org/counsyl/stor.svg?branch=master\n   :target: https://travis-ci.org/counsyl/stor\n',
+    'long_description': 'stor\n====\n\n|Build Status|\n\n``stor`` provides a cross-compatible CLI and Python API for accessing\nblock and object storage. ``stor`` was created so you could write one\npiece of code to work with local or remote files, without needing to\nwrite specialized code to handle failure modes, retrying or temporarily\nsystem unavailability. The functional API (i.e., ``stor.copytree``,\n``stor.rmtree``, ``stor.remove``, ``stor.listdir``) will work with the\nsame semantics across all storage backends. This makes it really easy to\ndevelop/test code locally with files and then take advantage of robust\nand cheaper object storage when you push to remote.\n\nView full docs for stor at https://counsyl.github.io/stor/ .\n\nQuickstart\n----------\n\n::\n\n    pip install stor\n\n``stor`` provides both a CLI and a Python library for manipulating Posix\nand OBS with a single, cross-compatible API.\n\nQuickstart - CLI\n----------------\n\n::\n\n    usage: stor [-h] [-c CONFIG_FILE] [--version]\n                {list,ls,cp,rm,walkfiles,cat,cd,pwd,clear,url,convert-swiftstack}\n                ...\n\n    A command line interface for stor.\n\n    positional arguments:\n      {list,ls,cp,rm,walkfiles,cat,cd,pwd,clear,url,convert-swiftstack}\n        list                List contents using the path as a prefix.\n        ls                  List path as a directory.\n        cp                  Copy a source to a destination path.\n        rm                  Remove file at a path.\n        walkfiles           List all files under a path that match an optional\n                            pattern.\n        cat                 Output file contents to stdout.\n        cd                  Change directory to a given OBS path.\n        pwd                 Get the present working directory of a service or all\n                            current directories.\n        clear               Clear current directories of a specified service.\n        url                 generate URI for path\n        convert-swiftstack  convert swiftstack paths\n\n    optional arguments:\n      -h, --help            show this help message and exit\n      -c CONFIG_FILE, --config CONFIG_FILE\n                            File containing configuration settings.\n      --version             Print version\n\nYou can ``ls`` local and remote directories\n\n::\n\n    ›› stor ls s3://stor-test-bucket\n    s3://stor-test-bucket/b.txt\n    s3://stor-test-bucket/counsyl-storage-utils\n    s3://stor-test-bucket/file_test.txt\n    s3://stor-test-bucket/counsyl-storage-utils/\n    s3://stor-test-bucket/empty/\n    s3://stor-test-bucket/lots_of_files/\n    s3://stor-test-bucket/small_test/\n\nCopy files locally or remotely or upload from stdin\n\n::\n\n    ›› echo "HELLO WORLD" | stor cp - swift://AUTH_stor_test/hello_world.txt\n    starting upload of 1 objects\n    upload complete - 1/1   0:00:00 0.00 MB 0.00 MB/s\n    ›› stor cat swift://AUTH_stor_test/hello_world.txt\n    HELLO WORLD\n    ›› stor cp swift://AUTH_stor_test/hello_world.txt hello_world.txt\n    ›› stor cat hello_world.txt\n    HELLO WORLD\n\nQuickstart - Python\n-------------------\n\nList files in a directory, taking advantage of delimiters\n\n.. code:: python\n\n    >>> stor.listdir(\'s3://bestbucket\')\n    [S3Path(\'s3://bestbucket/a/\')\n     S3Path(\'s3://bestbucket/b/\')]\n\nList all objects in a bucket\n\n.. code:: python\n\n    >>> stor.list(\'s3://bestbucket\')\n    [S3Path(\'s3://bestbucket/a/1.txt\')\n     S3Path(\'s3://bestbucket/a/2.txt\')\n     S3Path(\'s3://bestbucket/a/3.txt\')\n     S3Path(\'s3://bestbucket/b/1.txt\')]\n\nOr in a local path\n\n.. code:: python\n\n    >>> stor.list(\'stor\')\n    [PosixPath(\'stor/__init__.py\'),\n     PosixPath(\'stor/exceptions.pyc\'),\n     PosixPath(\'stor/tests/test_s3.py\'),\n     PosixPath(\'stor/tests/test_swift.py\'),\n     PosixPath(\'stor/tests/test_integration_swift.py\'),\n     PosixPath(\'stor/tests/test_utils.py\'),\n     PosixPath(\'stor/posix.pyc\'),\n     PosixPath(\'stor/base.py\'),\n\nRead and write files from POSIX or OBS, using python file objects.\n\n.. code:: python\n\n    import stor\n    with stor.open(\'/my/exciting.json\') as fp:\n        data1 = json.load(fp)\n\n    data1[\'read\'] = True\n\n    with stor.open(\'s3://bestbucket/exciting.json\') as fp:\n        json.dump(data1, fp)\n\nTesting code that uses stor\n---------------------------\n\nThe key design consideration of ``stor`` is that your code should be\nable to transparently use POSIX or any object storage system to read and\nupdate files. So, rather than use mocks, we suggest that you structure\nyour test code to point to local filesystem paths and restrict yourself\nto the functional API. E.g., in your prod settings, you could set\n``DATADIR = \'s3://bestbucketever\'``\\ and when you test, you could use\n``DATADIR = \'/somewhat/cool/path/to/test/data\'``, while your actual code\njust says:\n\n.. code:: python\n\n    with stor.open(stor.join(DATADIR, experiment)) as fp:\n        data = json.load(fp)\n\nEasy! and no mocks required!\n\nRunning the Tests\n-----------------\n\n::\n\n    make test\n\nContributing and Semantic Versioning\n------------------------------------\n\nWe use semantic versioning to communicate when we make API changes to\nthe library. See CONTRIBUTING.md for more details on contributing to\nstor.\n\n.. |Build Status| image:: https://travis-ci.org/counsyl/stor.svg?branch=master\n   :target: https://travis-ci.org/counsyl/stor\n',
     'author': 'Counsyl Inc.',
     'author_email': 'opensource@counsyl.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://counsyl.github.io/stor',
     'packages': packages,
     'package_data': package_data,
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `stor-4.0.2/PKG-INFO` & `stor-4.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: stor
-Version: 4.0.2
+Version: 4.1.0
 Summary: Cross-compatible API for accessing Posix and OBS storage systems
 Home-page: https://counsyl.github.io/stor
 License: MIT
 Author: Counsyl Inc.
 Author-email: opensource@counsyl.com
 Requires-Python: >=3.6,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: boto3 (>=1.7.0)
 Requires-Dist: cached-property (>=1.5.1)
 Requires-Dist: dxpy (>=0.278.0)
 Requires-Dist: python-keystoneclient (>=1.8.1)
 Requires-Dist: python-swiftclient (>=3.6.0)
 Requires-Dist: requests (>=2.20.0)
 Project-URL: Repository, https://github.com/counsyl/stor
```

