# Comparing `tmp/dxpy-v0.82.1.tar.gz` & `tmp/dxpy-v0.83.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dxpy-v0.82.1.tar", last modified: Wed Jan 22 21:59:33 2014, max compression
+gzip compressed data, was "dist/dxpy-v0.83.0.tar", last modified: Wed Feb  5 22:02:35 2014, max compression
```

## Comparing `dxpy-v0.82.1.tar` & `dxpy-v0.83.0.tar`

### file list

```diff
@@ -1,187 +1,188 @@
-drwxrwsr-x   0 dnanexus  (1002) dnanexus  (1002)        0 2014-01-22 21:59:33.000000 dxpy-v0.82.1/
--rwxrwxr-x   0 dnanexus  (1002) dnanexus  (1002)     4098 2014-01-22 21:59:30.000000 dxpy-v0.82.1/setup.py
-drwxrwsr-x   0 dnanexus  (1002) dnanexus  (1002)        0 2014-01-22 21:59:33.000000 dxpy-v0.82.1/dxpy.egg-info/
--rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)        1 2013-03-06 00:16:52.000000 dxpy-v0.82.1/dxpy.egg-info/not-zip-safe
--rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)        1 2014-01-22 21:59:33.000000 dxpy-v0.82.1/dxpy.egg-info/dependency_links.txt
--rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)      170 2014-01-22 21:59:33.000000 dxpy-v0.82.1/dxpy.egg-info/requires.txt
--rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)       10 2014-01-22 21:59:33.000000 dxpy-v0.82.1/dxpy.egg-info/top_level.txt
--rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)     6116 2014-01-22 21:59:33.000000 dxpy-v0.82.1/dxpy.egg-info/SOURCES.txt
--rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)     1023 2014-01-22 21:59:33.000000 dxpy-v0.82.1/dxpy.egg-info/entry_points.txt
--rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)      767 2014-01-22 21:59:33.000000 dxpy-v0.82.1/dxpy.egg-info/PKG-INFO
-drwxrwsr-x   0 dnanexus  (1002) dnanexus  (1002)        0 2014-01-22 21:59:33.000000 dxpy-v0.82.1/test/
--rwxrwxr-x   0 dnanexus  (1002) dnanexus  (1002)     8131 2014-01-22 21:59:30.000000 dxpy-v0.82.1/test/test_dx_completion.py
--rwxrwxr-x   0 dnanexus  (1002) dnanexus  (1002)    75223 2014-01-22 21:59:30.000000 dxpy-v0.82.1/test/test_dxpy.py
--rwxrwxr-x   0 dnanexus  (1002) dnanexus  (1002)    22381 2014-01-22 21:59:30.000000 dxpy-v0.82.1/test/coveragereport.py
--rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)     2871 2014-01-22 21:59:30.000000 dxpy-v0.82.1/test/dxpy_testutil.py
--rwxrwxr-x   0 dnanexus  (1002) dnanexus  (1002)     5168 2014-01-22 21:59:30.000000 dxpy-v0.82.1/test/test_dxpy_utils.py
--rwxrwxr-x   0 dnanexus  (1002) dnanexus  (1002)   139269 2014-01-22 21:59:30.000000 dxpy-v0.82.1/test/test_dxclient.py
--rwxrwxr-x   0 dnanexus  (1002) dnanexus  (1002)     4610 2014-01-22 21:59:30.000000 dxpy-v0.82.1/test/test_dxfs.py
--rwxrwxr-x   0 dnanexus  (1002) dnanexus  (1002)    14890 2014-01-22 21:59:30.000000 dxpy-v0.82.1/test/test_dx_app_wizard_and_run_app_locally.py
--rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)        0 2014-01-22 21:59:30.000000 dxpy-v0.82.1/test/__init__.py
-drwxrwsr-x   0 dnanexus  (1002) dnanexus  (1002)        0 2014-01-22 21:59:33.000000 dxpy-v0.82.1/dxpy/
-drwxrwsr-x   0 dnanexus  (1002) dnanexus  (1002)        0 2014-01-22 21:59:33.000000 dxpy-v0.82.1/dxpy/bindings/
--rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)    14341 2014-01-22 21:59:30.000000 dxpy-v0.82.1/dxpy/bindings/dxapp.py
--rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)     5856 2014-01-22 21:59:30.000000 dxpy-v0.82.1/dxpy/bindings/dxanalysis.py
--rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)    14578 2014-01-22 21:59:30.000000 dxpy-v0.82.1/dxpy/bindings/dxapplet.py
--rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)    29727 2014-01-22 21:59:30.000000 dxpy-v0.82.1/dxpy/bindings/search.py
--rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)     4985 2014-01-22 21:59:30.000000 dxpy-v0.82.1/dxpy/bindings/dxapp_container_functions.py
--rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)    23641 2014-01-22 21:59:30.000000 dxpy-v0.82.1/dxpy/bindings/dxworkflow.py
--rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)    23188 2014-01-22 21:59:30.000000 dxpy-v0.82.1/dxpy/bindings/dxfile.py
--rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)     5088 2014-01-22 21:59:30.000000 dxpy-v0.82.1/dxpy/bindings/dxdataobject_functions.py
--rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)     3938 2014-01-22 21:59:30.000000 dxpy-v0.82.1/dxpy/bindings/dxgtable_functions.py
--rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)    29378 2014-01-22 21:59:30.000000 dxpy-v0.82.1/dxpy/bindings/dxgtable.py
--rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)    11202 2014-01-22 21:59:30.000000 dxpy-v0.82.1/dxpy/bindings/dxfile_functions.py
--rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)      356 2014-01-22 21:59:30.000000 dxpy-v0.82.1/dxpy/bindings/auth.py
--rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)     3332 2014-01-22 21:59:30.000000 dxpy-v0.82.1/dxpy/bindings/dxrecord.py
--rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)    13410 2014-01-22 21:59:30.000000 dxpy-v0.82.1/dxpy/bindings/dxjob.py
--rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)    14577 2014-01-22 21:59:30.000000 dxpy-v0.82.1/dxpy/bindings/dxproject.py
--rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)    20255 2014-01-22 21:59:30.000000 dxpy-v0.82.1/dxpy/bindings/__init__.py
--rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)    22910 2014-01-22 21:59:30.000000 dxpy-v0.82.1/dxpy/app_builder.py
--rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)   100688 2014-01-22 21:59:30.000000 dxpy-v0.82.1/dxpy/api.py
--rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)     3578 2014-01-22 21:59:30.000000 dxpy-v0.82.1/dxpy/dxlog.py
--rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)      285 2014-01-22 21:59:30.000000 dxpy-v0.82.1/dxpy/app_categories.py
-drwxrwsr-x   0 dnanexus  (1002) dnanexus  (1002)        0 2014-01-22 21:59:33.000000 dxpy-v0.82.1/dxpy/scripts/
--rwxrwxr-x   0 dnanexus  (1002) dnanexus  (1002)    24866 2014-01-22 21:59:30.000000 dxpy-v0.82.1/dxpy/scripts/dx_fastq_to_reads.py
--rwxrwxr-x   0 dnanexus  (1002) dnanexus  (1002)     7386 2014-01-22 21:59:30.000000 dxpy-v0.82.1/dxpy/scripts/dx_genes_to_gtf.py
--rwxrwxr-x   0 dnanexus  (1002) dnanexus  (1002)    20386 2014-01-22 21:59:30.000000 dxpy-v0.82.1/dxpy/scripts/dx_gff_to_genes.py
--rwxrwxr-x   0 dnanexus  (1002) dnanexus  (1002)    14324 2014-01-22 21:59:30.000000 dxpy-v0.82.1/dxpy/scripts/dx_mappings_to_sam.py
--rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)     2136 2014-01-22 21:59:30.000000 dxpy-v0.82.1/dxpy/scripts/dx_mappings_to_fastq.py
--rwxrwxr-x   0 dnanexus  (1002) dnanexus  (1002)    15055 2014-01-22 21:59:30.000000 dxpy-v0.82.1/dxpy/scripts/dx_variants_to_vcf.py
--rwxrwxr-x   0 dnanexus  (1002) dnanexus  (1002)      888 2014-01-22 21:59:30.000000 dxpy-v0.82.1/dxpy/scripts/dx_csv_to_gtable.py
--rwxrwxr-x   0 dnanexus  (1002) dnanexus  (1002)     5195 2014-01-22 21:59:30.000000 dxpy-v0.82.1/dxpy/scripts/dx_reads_to_fastq.py
--rwxrwxr-x   0 dnanexus  (1002) dnanexus  (1002)     4957 2014-01-22 21:59:30.000000 dxpy-v0.82.1/dxpy/scripts/dx_gtable_to_tsv.py
--rwxrwxr-x   0 dnanexus  (1002) dnanexus  (1002)      888 2014-01-22 21:59:30.000000 dxpy-v0.82.1/dxpy/scripts/dx_gtable_to_csv.py
--rwxrwxr-x   0 dnanexus  (1002) dnanexus  (1002)    24762 2014-01-22 21:59:30.000000 dxpy-v0.82.1/dxpy/scripts/dx_gtf_to_genes.py
--rwxrwxr-x   0 dnanexus  (1002) dnanexus  (1002)    45185 2014-01-22 21:59:30.000000 dxpy-v0.82.1/dxpy/scripts/dx_build_app.py
--rwxrwxr-x   0 dnanexus  (1002) dnanexus  (1002)     4525 2014-01-22 21:59:30.000000 dxpy-v0.82.1/dxpy/scripts/dx_genes_to_gff.py
--rwxrwxr-x   0 dnanexus  (1002) dnanexus  (1002)    30832 2014-01-22 21:59:30.000000 dxpy-v0.82.1/dxpy/scripts/dx_bed_to_spans.py
--rwxrwxr-x   0 dnanexus  (1002) dnanexus  (1002)   229964 2014-01-22 21:59:30.000000 dxpy-v0.82.1/dxpy/scripts/dx.py
--rwxrwxr-x   0 dnanexus  (1002) dnanexus  (1002)     9914 2014-01-22 21:59:30.000000 dxpy-v0.82.1/dxpy/scripts/dx_spans_to_bed.py
--rwxrwxr-x   0 dnanexus  (1002) dnanexus  (1002)      890 2014-01-22 21:59:30.000000 dxpy-v0.82.1/dxpy/scripts/dx_build_applet.py
--rwxrwxr-x   0 dnanexus  (1002) dnanexus  (1002)     6458 2014-01-22 21:59:30.000000 dxpy-v0.82.1/dxpy/scripts/dx_tsv_to_gtable.py
--rwxrwxr-x   0 dnanexus  (1002) dnanexus  (1002)     8712 2014-01-22 21:59:30.000000 dxpy-v0.82.1/dxpy/scripts/dx_build_report_html.py
--rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)      899 2014-01-22 21:59:30.000000 dxpy-v0.82.1/dxpy/scripts/__init__.py
-drwxrwsr-x   0 dnanexus  (1002) dnanexus  (1002)        0 2014-01-22 21:59:33.000000 dxpy-v0.82.1/dxpy/packages/
-drwxrwsr-x   0 dnanexus  (1002) dnanexus  (1002)        0 2014-01-22 21:59:33.000000 dxpy-v0.82.1/dxpy/packages/requests/
--rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)      544 2014-01-22 21:59:30.000000 dxpy-v0.82.1/dxpy/packages/requests/certs.py
--rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)      820 2014-01-22 21:59:30.000000 dxpy-v0.82.1/dxpy/packages/requests/hooks.py
--rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)     3104 2014-01-22 21:59:30.000000 dxpy-v0.82.1/dxpy/packages/requests/status_codes.py
--rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)     4333 2014-01-22 21:59:30.000000 dxpy-v0.82.1/dxpy/packages/requests/api.py
--rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)    17371 2014-01-22 21:59:30.000000 dxpy-v0.82.1/dxpy/packages/requests/sessions.py
-drwxrwsr-x   0 dnanexus  (1002) dnanexus  (1002)        0 2014-01-22 21:59:33.000000 dxpy-v0.82.1/dxpy/packages/requests/packages/
-drwxrwsr-x   0 dnanexus  (1002) dnanexus  (1002)        0 2014-01-22 21:59:33.000000 dxpy-v0.82.1/dxpy/packages/requests/packages/charade/
--rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)    20183 2014-01-22 21:59:30.000000 dxpy-v0.82.1/dxpy/packages/requests/packages/charade/mbcssm.py
--rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)    82594 2014-01-22 21:59:30.000000 dxpy-v0.82.1/dxpy/packages/requests/packages/charade/big5freq.py
--rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)     5380 2014-01-22 21:59:30.000000 dxpy-v0.82.1/dxpy/packages/requests/packages/charade/latin1prober.py
--rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)     4913 2014-01-22 21:59:30.000000 dxpy-v0.82.1/dxpy/packages/requests/packages/charade/sbcharsetprober.py
--rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)     1717 2014-01-22 21:59:30.000000 dxpy-v0.82.1/dxpy/packages/requests/packages/charade/euctwprober.py
--rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)     2379 2014-01-22 21:59:30.000000 dxpy-v0.82.1/dxpy/packages/requests/packages/charade/codingstatemachine.py
--rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)     2021 2014-01-22 21:59:30.000000 dxpy-v0.82.1/dxpy/packages/requests/packages/charade/mbcsgroupprober.py
--rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)    19323 2014-01-22 21:59:30.000000 dxpy-v0.82.1/dxpy/packages/requests/packages/charade/jpcntx.py
--rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)     3354 2014-01-22 21:59:30.000000 dxpy-v0.82.1/dxpy/packages/requests/packages/charade/mbcharsetprober.py
--rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)    12761 2014-01-22 21:59:30.000000 dxpy-v0.82.1/dxpy/packages/requests/packages/charade/langhungarianmodel.py
--rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)     8081 2014-01-22 21:59:30.000000 dxpy-v0.82.1/dxpy/packages/requests/packages/charade/escsm.py
--rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)     3273 2014-01-22 21:59:30.000000 dxpy-v0.82.1/dxpy/packages/requests/packages/charade/escprober.py
--rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)    13642 2014-01-22 21:59:30.000000 dxpy-v0.82.1/dxpy/packages/requests/packages/charade/hebrewprober.py
--rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)    47315 2014-01-22 21:59:30.000000 dxpy-v0.82.1/dxpy/packages/requests/packages/charade/jisfreq.py
--rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)     7030 2014-01-22 21:59:30.000000 dxpy-v0.82.1/dxpy/packages/requests/packages/charade/universaldetector.py
--rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)    12853 2014-01-22 21:59:30.000000 dxpy-v0.82.1/dxpy/packages/requests/packages/charade/langgreekmodel.py
--rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)     1717 2014-01-22 21:59:30.000000 dxpy-v0.82.1/dxpy/packages/requests/packages/charade/euckrprober.py
--rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)     3360 2014-01-22 21:59:30.000000 dxpy-v0.82.1/dxpy/packages/requests/packages/charade/sbcsgroupprober.py
--rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)     1722 2014-01-22 21:59:30.000000 dxpy-v0.82.1/dxpy/packages/requests/packages/charade/gb2312prober.py
--rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)    18054 2014-01-22 21:59:30.000000 dxpy-v0.82.1/dxpy/packages/requests/packages/charade/langcyrillicmodel.py
--rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)    45978 2014-01-22 21:59:30.000000 dxpy-v0.82.1/dxpy/packages/requests/packages/charade/euckrfreq.py
--rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)     3768 2014-01-22 21:59:30.000000 dxpy-v0.82.1/dxpy/packages/requests/packages/charade/eucjpprober.py
--rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)    11519 2014-01-22 21:59:30.000000 dxpy-v0.82.1/dxpy/packages/requests/packages/charade/langhebrewmodel.py
--rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)     1157 2014-01-22 21:59:30.000000 dxpy-v0.82.1/dxpy/packages/requests/packages/charade/compat.py
--rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)     3897 2014-01-22 21:59:30.000000 dxpy-v0.82.1/dxpy/packages/requests/packages/charade/charsetgroupprober.py
--rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)     1826 2014-01-22 21:59:30.000000 dxpy-v0.82.1/dxpy/packages/requests/packages/charade/cp949prober.py
--rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)     2728 2014-01-22 21:59:30.000000 dxpy-v0.82.1/dxpy/packages/requests/packages/charade/utf8prober.py
--rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)    13013 2014-01-22 21:59:30.000000 dxpy-v0.82.1/dxpy/packages/requests/packages/charade/langbulgarianmodel.py
--rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)     1374 2014-01-22 21:59:30.000000 dxpy-v0.82.1/dxpy/packages/requests/packages/charade/constants.py
--rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)     9457 2014-01-22 21:59:30.000000 dxpy-v0.82.1/dxpy/packages/requests/packages/charade/chardistribution.py
--rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)    34872 2014-01-22 21:59:30.000000 dxpy-v0.82.1/dxpy/packages/requests/packages/charade/euctwfreq.py
--rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)    36011 2014-01-22 21:59:30.000000 dxpy-v0.82.1/dxpy/packages/requests/packages/charade/gb2312freq.py
--rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)     1726 2014-01-22 21:59:30.000000 dxpy-v0.82.1/dxpy/packages/requests/packages/charade/big5prober.py
--rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)     3825 2014-01-22 21:59:30.000000 dxpy-v0.82.1/dxpy/packages/requests/packages/charade/sjisprober.py
--rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)    11475 2014-01-22 21:59:30.000000 dxpy-v0.82.1/dxpy/packages/requests/packages/charade/langthaimodel.py
--rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)     1902 2014-01-22 21:59:30.000000 dxpy-v0.82.1/dxpy/packages/requests/packages/charade/charsetprober.py
--rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)     1327 2014-01-22 21:59:30.000000 dxpy-v0.82.1/dxpy/packages/requests/packages/charade/__init__.py
-drwxrwsr-x   0 dnanexus  (1002) dnanexus  (1002)        0 2014-01-22 21:59:33.000000 dxpy-v0.82.1/dxpy/packages/requests/packages/urllib3/
--rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)     5873 2014-01-22 21:59:30.000000 dxpy-v0.82.1/dxpy/packages/requests/packages/urllib3/request.py
--rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)    22855 2014-01-22 21:59:30.000000 dxpy-v0.82.1/dxpy/packages/requests/packages/urllib3/connectionpool.py
--rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)     8897 2014-01-22 21:59:30.000000 dxpy-v0.82.1/dxpy/packages/requests/packages/urllib3/poolmanager.py
--rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)     2903 2014-01-22 21:59:30.000000 dxpy-v0.82.1/dxpy/packages/requests/packages/urllib3/_collections.py
-drwxrwsr-x   0 dnanexus  (1002) dnanexus  (1002)        0 2014-01-22 21:59:33.000000 dxpy-v0.82.1/dxpy/packages/requests/packages/urllib3/packages/
--rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)     8936 2014-01-22 21:59:30.000000 dxpy-v0.82.1/dxpy/packages/requests/packages/urllib3/packages/ordered_dict.py
-drwxrwsr-x   0 dnanexus  (1002) dnanexus  (1002)        0 2014-01-22 21:59:33.000000 dxpy-v0.82.1/dxpy/packages/requests/packages/urllib3/packages/ssl_match_hostname/
--rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)     2174 2014-01-22 21:59:30.000000 dxpy-v0.82.1/dxpy/packages/requests/packages/urllib3/packages/ssl_match_hostname/__init__.py
--rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)    11628 2014-01-22 21:59:30.000000 dxpy-v0.82.1/dxpy/packages/requests/packages/urllib3/packages/six.py
--rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)       74 2014-01-22 21:59:30.000000 dxpy-v0.82.1/dxpy/packages/requests/packages/urllib3/packages/__init__.py
--rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)    10972 2014-01-22 21:59:30.000000 dxpy-v0.82.1/dxpy/packages/requests/packages/urllib3/util.py
--rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)     3049 2014-01-22 21:59:30.000000 dxpy-v0.82.1/dxpy/packages/requests/packages/urllib3/filepost.py
-drwxrwsr-x   0 dnanexus  (1002) dnanexus  (1002)        0 2014-01-22 21:59:33.000000 dxpy-v0.82.1/dxpy/packages/requests/packages/urllib3/contrib/
--rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)     4740 2014-01-22 21:59:30.000000 dxpy-v0.82.1/dxpy/packages/requests/packages/urllib3/contrib/ntlmpool.py
--rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)     5235 2014-01-22 21:59:30.000000 dxpy-v0.82.1/dxpy/packages/requests/packages/urllib3/contrib/pyopenssl.py
--rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)        0 2014-01-22 21:59:30.000000 dxpy-v0.82.1/dxpy/packages/requests/packages/urllib3/contrib/__init__.py
--rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)     2258 2014-01-22 21:59:30.000000 dxpy-v0.82.1/dxpy/packages/requests/packages/urllib3/exceptions.py
--rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)     8245 2014-01-22 21:59:30.000000 dxpy-v0.82.1/dxpy/packages/requests/packages/urllib3/response.py
--rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)     1692 2014-01-22 21:59:30.000000 dxpy-v0.82.1/dxpy/packages/requests/packages/urllib3/__init__.py
--rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)       62 2014-01-22 21:59:30.000000 dxpy-v0.82.1/dxpy/packages/requests/packages/__init__.py
--rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)    14112 2014-01-22 21:59:30.000000 dxpy-v0.82.1/dxpy/packages/requests/cookies.py
--rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)     3576 2014-01-22 21:59:30.000000 dxpy-v0.82.1/dxpy/packages/requests/structures.py
--rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)    21905 2014-01-22 21:59:30.000000 dxpy-v0.82.1/dxpy/packages/requests/models.py
--rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)     2433 2014-01-22 21:59:30.000000 dxpy-v0.82.1/dxpy/packages/requests/compat.py
--rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)   211059 2014-01-22 21:59:30.000000 dxpy-v0.82.1/dxpy/packages/requests/cacert.pem
--rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)    12616 2014-01-22 21:59:30.000000 dxpy-v0.82.1/dxpy/packages/requests/adapters.py
--rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)     5531 2014-01-22 21:59:30.000000 dxpy-v0.82.1/dxpy/packages/requests/auth.py
--rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)     1246 2014-01-22 21:59:30.000000 dxpy-v0.82.1/dxpy/packages/requests/exceptions.py
--rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)    16299 2014-01-22 21:59:30.000000 dxpy-v0.82.1/dxpy/packages/requests/utils.py
--rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)     1863 2014-01-22 21:59:30.000000 dxpy-v0.82.1/dxpy/packages/requests/__init__.py
--rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)        0 2014-01-22 21:59:30.000000 dxpy-v0.82.1/dxpy/packages/__init__.py
--rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)       20 2014-01-22 21:59:30.000000 dxpy-v0.82.1/dxpy/toolkit_version.py
-drwxrwsr-x   0 dnanexus  (1002) dnanexus  (1002)        0 2014-01-22 21:59:33.000000 dxpy-v0.82.1/dxpy/utils/
--rwxrwxr-x   0 dnanexus  (1002) dnanexus  (1002)     7346 2014-01-22 21:59:30.000000 dxpy-v0.82.1/dxpy/utils/pretty_print.py
--rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)     4405 2014-01-22 21:59:30.000000 dxpy-v0.82.1/dxpy/utils/job_log_client.py
--rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)     2420 2014-01-22 21:59:30.000000 dxpy-v0.82.1/dxpy/utils/pathmatch.py
--rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)     7957 2014-01-22 21:59:30.000000 dxpy-v0.82.1/dxpy/utils/env.py
--rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)    38579 2014-01-22 21:59:30.000000 dxpy-v0.82.1/dxpy/utils/describe.py
--rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)     4331 2014-01-22 21:59:30.000000 dxpy-v0.82.1/dxpy/utils/printing.py
--rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)     7987 2014-01-22 21:59:30.000000 dxpy-v0.82.1/dxpy/utils/exec_utils.py
--rwxrwxr-x   0 dnanexus  (1002) dnanexus  (1002)    18464 2014-01-22 21:59:30.000000 dxpy-v0.82.1/dxpy/utils/local_exec_utils.py
--rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)    32891 2014-01-22 21:59:30.000000 dxpy-v0.82.1/dxpy/utils/resolver.py
--rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)      434 2014-01-22 21:59:30.000000 dxpy-v0.82.1/dxpy/utils/genomic_utils.py
--rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)    19222 2014-01-22 21:59:30.000000 dxpy-v0.82.1/dxpy/utils/completer.py
--rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)    11895 2014-01-22 21:59:30.000000 dxpy-v0.82.1/dxpy/utils/__init__.py
-drwxrwsr-x   0 dnanexus  (1002) dnanexus  (1002)        0 2014-01-22 21:59:33.000000 dxpy-v0.82.1/dxpy/templating/
--rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)     6277 2014-01-22 21:59:30.000000 dxpy-v0.82.1/dxpy/templating/python.py
--rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)     4683 2014-01-22 21:59:30.000000 dxpy-v0.82.1/dxpy/templating/bash.py
--rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)     6502 2014-01-22 21:59:30.000000 dxpy-v0.82.1/dxpy/templating/cpp.py
--rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)    18656 2014-01-22 21:59:30.000000 dxpy-v0.82.1/dxpy/templating/utils.py
--rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)      674 2014-01-22 21:59:30.000000 dxpy-v0.82.1/dxpy/templating/__init__.py
--rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)      387 2014-01-22 21:59:30.000000 dxpy-v0.82.1/dxpy/compat.py
--rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)     7752 2014-01-22 21:59:30.000000 dxpy-v0.82.1/dxpy/exceptions.py
-drwxrwsr-x   0 dnanexus  (1002) dnanexus  (1002)        0 2014-01-22 21:59:33.000000 dxpy-v0.82.1/dxpy/cli/
--rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)    18757 2014-01-22 21:59:30.000000 dxpy-v0.82.1/dxpy/cli/parsers.py
--rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)    30930 2014-01-22 21:59:30.000000 dxpy-v0.82.1/dxpy/cli/exec_io.py
--rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)    10516 2014-01-22 21:59:30.000000 dxpy-v0.82.1/dxpy/cli/workflow.py
--rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)     1049 2014-01-22 21:59:30.000000 dxpy-v0.82.1/dxpy/cli/__init__.py
--rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)    24371 2014-01-22 21:59:30.000000 dxpy-v0.82.1/dxpy/__init__.py
--rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)      224 2014-01-22 21:59:33.000000 dxpy-v0.82.1/setup.cfg
-drwxrwsr-x   0 dnanexus  (1002) dnanexus  (1002)        0 2014-01-22 21:59:33.000000 dxpy-v0.82.1/scripts/
--rwxrwxr-x   0 dnanexus  (1002) dnanexus  (1002)     7815 2014-01-22 21:59:30.000000 dxpy-v0.82.1/scripts/dx-jobutil-add-output
--rwxrwxr-x   0 dnanexus  (1002) dnanexus  (1002)     1693 2014-01-22 21:59:30.000000 dxpy-v0.82.1/scripts/dx-fetch-bundled-depends
--rwxrwxr-x   0 dnanexus  (1002) dnanexus  (1002)     1620 2014-01-22 21:59:30.000000 dxpy-v0.82.1/scripts/dx-jobutil-report-error
--rwxrwxr-x   0 dnanexus  (1002) dnanexus  (1002)    18367 2014-01-22 21:59:30.000000 dxpy-v0.82.1/scripts/dx-app-wizard
--rwxrwxr-x   0 dnanexus  (1002) dnanexus  (1002)     1349 2014-01-22 21:59:30.000000 dxpy-v0.82.1/scripts/dx-jobutil-dxlink
--rwxrwxr-x   0 dnanexus  (1002) dnanexus  (1002)     1381 2014-01-22 21:59:30.000000 dxpy-v0.82.1/scripts/dx-jobutil-parse-link
--rwxrwxr-x   0 dnanexus  (1002) dnanexus  (1002)     1766 2014-01-22 21:59:30.000000 dxpy-v0.82.1/scripts/dx-log-stream
--rwxrwxr-x   0 dnanexus  (1002) dnanexus  (1002)    18418 2014-01-22 21:59:30.000000 dxpy-v0.82.1/scripts/dx-mount
--rwxrwxr-x   0 dnanexus  (1002) dnanexus  (1002)     7001 2014-01-22 21:59:30.000000 dxpy-v0.82.1/scripts/dx-run-app-locally
--rwxrwxr-x   0 dnanexus  (1002) dnanexus  (1002)    12950 2014-01-22 21:59:30.000000 dxpy-v0.82.1/scripts/dx-workflow-to-applet
--rwxrwxr-x   0 dnanexus  (1002) dnanexus  (1002)     2335 2014-01-22 21:59:30.000000 dxpy-v0.82.1/scripts/dx-jobutil-new-job
--rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)      132 2014-01-22 21:59:30.000000 dxpy-v0.82.1/MANIFEST.in
--rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)       24 2014-01-22 21:59:30.000000 dxpy-v0.82.1/requirements_test.txt
--rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)      144 2014-01-22 21:59:30.000000 dxpy-v0.82.1/requirements.txt
--rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)       27 2014-01-22 21:59:30.000000 dxpy-v0.82.1/requirements_dxfs.txt
--rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)      767 2014-01-22 21:59:33.000000 dxpy-v0.82.1/PKG-INFO
+drwxrwsr-x   0 dnanexus  (1002) dnanexus  (1002)        0 2014-02-05 22:02:35.000000 dxpy-v0.83.0/
+-rwxrwxr-x   0 dnanexus  (1002) dnanexus  (1002)     4098 2014-02-05 22:02:34.000000 dxpy-v0.83.0/setup.py
+drwxrwsr-x   0 dnanexus  (1002) dnanexus  (1002)        0 2014-02-05 22:02:35.000000 dxpy-v0.83.0/dxpy.egg-info/
+-rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)        1 2013-03-06 00:16:52.000000 dxpy-v0.83.0/dxpy.egg-info/not-zip-safe
+-rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)        1 2014-02-05 22:02:35.000000 dxpy-v0.83.0/dxpy.egg-info/dependency_links.txt
+-rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)      170 2014-02-05 22:02:35.000000 dxpy-v0.83.0/dxpy.egg-info/requires.txt
+-rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)       10 2014-02-05 22:02:35.000000 dxpy-v0.83.0/dxpy.egg-info/top_level.txt
+-rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)     6144 2014-02-05 22:02:35.000000 dxpy-v0.83.0/dxpy.egg-info/SOURCES.txt
+-rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)     1023 2014-02-05 22:02:35.000000 dxpy-v0.83.0/dxpy.egg-info/entry_points.txt
+-rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)      767 2014-02-05 22:02:35.000000 dxpy-v0.83.0/dxpy.egg-info/PKG-INFO
+drwxrwsr-x   0 dnanexus  (1002) dnanexus  (1002)        0 2014-02-05 22:02:35.000000 dxpy-v0.83.0/test/
+-rwxrwxr-x   0 dnanexus  (1002) dnanexus  (1002)     8131 2014-02-05 22:02:34.000000 dxpy-v0.83.0/test/test_dx_completion.py
+-rwxrwxr-x   0 dnanexus  (1002) dnanexus  (1002)    75223 2014-02-05 22:02:34.000000 dxpy-v0.83.0/test/test_dxpy.py
+-rwxrwxr-x   0 dnanexus  (1002) dnanexus  (1002)    22381 2014-02-05 22:02:34.000000 dxpy-v0.83.0/test/coveragereport.py
+-rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)     2915 2014-02-05 22:02:34.000000 dxpy-v0.83.0/test/dxpy_testutil.py
+-rwxrwxr-x   0 dnanexus  (1002) dnanexus  (1002)     5519 2014-02-05 22:02:34.000000 dxpy-v0.83.0/test/test_dxpy_utils.py
+-rwxrwxr-x   0 dnanexus  (1002) dnanexus  (1002)   141800 2014-02-05 22:02:34.000000 dxpy-v0.83.0/test/test_dxclient.py
+-rwxrwxr-x   0 dnanexus  (1002) dnanexus  (1002)     4610 2014-02-05 22:02:34.000000 dxpy-v0.83.0/test/test_dxfs.py
+-rwxrwxr-x   0 dnanexus  (1002) dnanexus  (1002)    14890 2014-02-05 22:02:34.000000 dxpy-v0.83.0/test/test_dx_app_wizard_and_run_app_locally.py
+-rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)        0 2014-02-05 22:02:34.000000 dxpy-v0.83.0/test/__init__.py
+drwxrwsr-x   0 dnanexus  (1002) dnanexus  (1002)        0 2014-02-05 22:02:35.000000 dxpy-v0.83.0/dxpy/
+drwxrwsr-x   0 dnanexus  (1002) dnanexus  (1002)        0 2014-02-05 22:02:35.000000 dxpy-v0.83.0/dxpy/bindings/
+-rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)    14341 2014-02-05 22:02:34.000000 dxpy-v0.83.0/dxpy/bindings/dxapp.py
+-rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)     5856 2014-02-05 22:02:34.000000 dxpy-v0.83.0/dxpy/bindings/dxanalysis.py
+-rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)    14578 2014-02-05 22:02:34.000000 dxpy-v0.83.0/dxpy/bindings/dxapplet.py
+-rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)    29727 2014-02-05 22:02:34.000000 dxpy-v0.83.0/dxpy/bindings/search.py
+-rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)     4985 2014-02-05 22:02:34.000000 dxpy-v0.83.0/dxpy/bindings/dxapp_container_functions.py
+-rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)    23711 2014-02-05 22:02:34.000000 dxpy-v0.83.0/dxpy/bindings/dxworkflow.py
+-rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)    23106 2014-02-05 22:02:34.000000 dxpy-v0.83.0/dxpy/bindings/dxfile.py
+-rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)     5088 2014-02-05 22:02:34.000000 dxpy-v0.83.0/dxpy/bindings/dxdataobject_functions.py
+-rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)     3938 2014-02-05 22:02:34.000000 dxpy-v0.83.0/dxpy/bindings/dxgtable_functions.py
+-rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)    29378 2014-02-05 22:02:34.000000 dxpy-v0.83.0/dxpy/bindings/dxgtable.py
+-rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)    11202 2014-02-05 22:02:34.000000 dxpy-v0.83.0/dxpy/bindings/dxfile_functions.py
+-rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)      356 2014-02-05 22:02:34.000000 dxpy-v0.83.0/dxpy/bindings/auth.py
+-rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)     3332 2014-02-05 22:02:34.000000 dxpy-v0.83.0/dxpy/bindings/dxrecord.py
+-rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)    13410 2014-02-05 22:02:34.000000 dxpy-v0.83.0/dxpy/bindings/dxjob.py
+-rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)    14577 2014-02-05 22:02:34.000000 dxpy-v0.83.0/dxpy/bindings/dxproject.py
+-rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)    20255 2014-02-05 22:02:34.000000 dxpy-v0.83.0/dxpy/bindings/__init__.py
+-rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)    22910 2014-02-05 22:02:34.000000 dxpy-v0.83.0/dxpy/app_builder.py
+-rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)   100688 2014-02-05 22:02:34.000000 dxpy-v0.83.0/dxpy/api.py
+-rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)     3578 2014-02-05 22:02:34.000000 dxpy-v0.83.0/dxpy/dxlog.py
+-rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)      285 2014-02-05 22:02:34.000000 dxpy-v0.83.0/dxpy/app_categories.py
+drwxrwsr-x   0 dnanexus  (1002) dnanexus  (1002)        0 2014-02-05 22:02:35.000000 dxpy-v0.83.0/dxpy/scripts/
+-rwxrwxr-x   0 dnanexus  (1002) dnanexus  (1002)    24866 2014-02-05 22:02:34.000000 dxpy-v0.83.0/dxpy/scripts/dx_fastq_to_reads.py
+-rwxrwxr-x   0 dnanexus  (1002) dnanexus  (1002)     7386 2014-02-05 22:02:34.000000 dxpy-v0.83.0/dxpy/scripts/dx_genes_to_gtf.py
+-rwxrwxr-x   0 dnanexus  (1002) dnanexus  (1002)    20386 2014-02-05 22:02:34.000000 dxpy-v0.83.0/dxpy/scripts/dx_gff_to_genes.py
+-rwxrwxr-x   0 dnanexus  (1002) dnanexus  (1002)    14324 2014-02-05 22:02:34.000000 dxpy-v0.83.0/dxpy/scripts/dx_mappings_to_sam.py
+-rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)     2136 2014-02-05 22:02:34.000000 dxpy-v0.83.0/dxpy/scripts/dx_mappings_to_fastq.py
+-rwxrwxr-x   0 dnanexus  (1002) dnanexus  (1002)    15055 2014-02-05 22:02:34.000000 dxpy-v0.83.0/dxpy/scripts/dx_variants_to_vcf.py
+-rwxrwxr-x   0 dnanexus  (1002) dnanexus  (1002)      888 2014-02-05 22:02:34.000000 dxpy-v0.83.0/dxpy/scripts/dx_csv_to_gtable.py
+-rwxrwxr-x   0 dnanexus  (1002) dnanexus  (1002)     5195 2014-02-05 22:02:34.000000 dxpy-v0.83.0/dxpy/scripts/dx_reads_to_fastq.py
+-rwxrwxr-x   0 dnanexus  (1002) dnanexus  (1002)     4957 2014-02-05 22:02:34.000000 dxpy-v0.83.0/dxpy/scripts/dx_gtable_to_tsv.py
+-rwxrwxr-x   0 dnanexus  (1002) dnanexus  (1002)      888 2014-02-05 22:02:34.000000 dxpy-v0.83.0/dxpy/scripts/dx_gtable_to_csv.py
+-rwxrwxr-x   0 dnanexus  (1002) dnanexus  (1002)    24762 2014-02-05 22:02:34.000000 dxpy-v0.83.0/dxpy/scripts/dx_gtf_to_genes.py
+-rwxrwxr-x   0 dnanexus  (1002) dnanexus  (1002)    45185 2014-02-05 22:02:34.000000 dxpy-v0.83.0/dxpy/scripts/dx_build_app.py
+-rwxrwxr-x   0 dnanexus  (1002) dnanexus  (1002)     4525 2014-02-05 22:02:34.000000 dxpy-v0.83.0/dxpy/scripts/dx_genes_to_gff.py
+-rwxrwxr-x   0 dnanexus  (1002) dnanexus  (1002)    30832 2014-02-05 22:02:34.000000 dxpy-v0.83.0/dxpy/scripts/dx_bed_to_spans.py
+-rwxrwxr-x   0 dnanexus  (1002) dnanexus  (1002)   225360 2014-02-05 22:02:34.000000 dxpy-v0.83.0/dxpy/scripts/dx.py
+-rwxrwxr-x   0 dnanexus  (1002) dnanexus  (1002)     9914 2014-02-05 22:02:34.000000 dxpy-v0.83.0/dxpy/scripts/dx_spans_to_bed.py
+-rwxrwxr-x   0 dnanexus  (1002) dnanexus  (1002)      890 2014-02-05 22:02:34.000000 dxpy-v0.83.0/dxpy/scripts/dx_build_applet.py
+-rwxrwxr-x   0 dnanexus  (1002) dnanexus  (1002)     6458 2014-02-05 22:02:34.000000 dxpy-v0.83.0/dxpy/scripts/dx_tsv_to_gtable.py
+-rwxrwxr-x   0 dnanexus  (1002) dnanexus  (1002)     8712 2014-02-05 22:02:34.000000 dxpy-v0.83.0/dxpy/scripts/dx_build_report_html.py
+-rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)      899 2014-02-05 22:02:34.000000 dxpy-v0.83.0/dxpy/scripts/__init__.py
+drwxrwsr-x   0 dnanexus  (1002) dnanexus  (1002)        0 2014-02-05 22:02:35.000000 dxpy-v0.83.0/dxpy/packages/
+drwxrwsr-x   0 dnanexus  (1002) dnanexus  (1002)        0 2014-02-05 22:02:35.000000 dxpy-v0.83.0/dxpy/packages/requests/
+-rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)      544 2014-02-05 22:02:34.000000 dxpy-v0.83.0/dxpy/packages/requests/certs.py
+-rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)      820 2014-02-05 22:02:34.000000 dxpy-v0.83.0/dxpy/packages/requests/hooks.py
+-rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)     3104 2014-02-05 22:02:34.000000 dxpy-v0.83.0/dxpy/packages/requests/status_codes.py
+-rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)     4333 2014-02-05 22:02:34.000000 dxpy-v0.83.0/dxpy/packages/requests/api.py
+-rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)    17371 2014-02-05 22:02:34.000000 dxpy-v0.83.0/dxpy/packages/requests/sessions.py
+drwxrwsr-x   0 dnanexus  (1002) dnanexus  (1002)        0 2014-02-05 22:02:35.000000 dxpy-v0.83.0/dxpy/packages/requests/packages/
+drwxrwsr-x   0 dnanexus  (1002) dnanexus  (1002)        0 2014-02-05 22:02:35.000000 dxpy-v0.83.0/dxpy/packages/requests/packages/charade/
+-rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)    20183 2014-02-05 22:02:34.000000 dxpy-v0.83.0/dxpy/packages/requests/packages/charade/mbcssm.py
+-rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)    82594 2014-02-05 22:02:34.000000 dxpy-v0.83.0/dxpy/packages/requests/packages/charade/big5freq.py
+-rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)     5380 2014-02-05 22:02:34.000000 dxpy-v0.83.0/dxpy/packages/requests/packages/charade/latin1prober.py
+-rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)     4913 2014-02-05 22:02:34.000000 dxpy-v0.83.0/dxpy/packages/requests/packages/charade/sbcharsetprober.py
+-rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)     1717 2014-02-05 22:02:34.000000 dxpy-v0.83.0/dxpy/packages/requests/packages/charade/euctwprober.py
+-rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)     2379 2014-02-05 22:02:34.000000 dxpy-v0.83.0/dxpy/packages/requests/packages/charade/codingstatemachine.py
+-rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)     2021 2014-02-05 22:02:34.000000 dxpy-v0.83.0/dxpy/packages/requests/packages/charade/mbcsgroupprober.py
+-rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)    19323 2014-02-05 22:02:34.000000 dxpy-v0.83.0/dxpy/packages/requests/packages/charade/jpcntx.py
+-rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)     3354 2014-02-05 22:02:34.000000 dxpy-v0.83.0/dxpy/packages/requests/packages/charade/mbcharsetprober.py
+-rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)    12761 2014-02-05 22:02:34.000000 dxpy-v0.83.0/dxpy/packages/requests/packages/charade/langhungarianmodel.py
+-rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)     8081 2014-02-05 22:02:34.000000 dxpy-v0.83.0/dxpy/packages/requests/packages/charade/escsm.py
+-rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)     3273 2014-02-05 22:02:34.000000 dxpy-v0.83.0/dxpy/packages/requests/packages/charade/escprober.py
+-rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)    13642 2014-02-05 22:02:34.000000 dxpy-v0.83.0/dxpy/packages/requests/packages/charade/hebrewprober.py
+-rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)    47315 2014-02-05 22:02:34.000000 dxpy-v0.83.0/dxpy/packages/requests/packages/charade/jisfreq.py
+-rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)     7030 2014-02-05 22:02:34.000000 dxpy-v0.83.0/dxpy/packages/requests/packages/charade/universaldetector.py
+-rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)    12853 2014-02-05 22:02:34.000000 dxpy-v0.83.0/dxpy/packages/requests/packages/charade/langgreekmodel.py
+-rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)     1717 2014-02-05 22:02:34.000000 dxpy-v0.83.0/dxpy/packages/requests/packages/charade/euckrprober.py
+-rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)     3360 2014-02-05 22:02:34.000000 dxpy-v0.83.0/dxpy/packages/requests/packages/charade/sbcsgroupprober.py
+-rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)     1722 2014-02-05 22:02:34.000000 dxpy-v0.83.0/dxpy/packages/requests/packages/charade/gb2312prober.py
+-rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)    18054 2014-02-05 22:02:34.000000 dxpy-v0.83.0/dxpy/packages/requests/packages/charade/langcyrillicmodel.py
+-rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)    45978 2014-02-05 22:02:34.000000 dxpy-v0.83.0/dxpy/packages/requests/packages/charade/euckrfreq.py
+-rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)     3768 2014-02-05 22:02:34.000000 dxpy-v0.83.0/dxpy/packages/requests/packages/charade/eucjpprober.py
+-rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)    11519 2014-02-05 22:02:34.000000 dxpy-v0.83.0/dxpy/packages/requests/packages/charade/langhebrewmodel.py
+-rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)     1157 2014-02-05 22:02:34.000000 dxpy-v0.83.0/dxpy/packages/requests/packages/charade/compat.py
+-rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)     3897 2014-02-05 22:02:34.000000 dxpy-v0.83.0/dxpy/packages/requests/packages/charade/charsetgroupprober.py
+-rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)     1826 2014-02-05 22:02:34.000000 dxpy-v0.83.0/dxpy/packages/requests/packages/charade/cp949prober.py
+-rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)     2728 2014-02-05 22:02:34.000000 dxpy-v0.83.0/dxpy/packages/requests/packages/charade/utf8prober.py
+-rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)    13013 2014-02-05 22:02:34.000000 dxpy-v0.83.0/dxpy/packages/requests/packages/charade/langbulgarianmodel.py
+-rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)     1374 2014-02-05 22:02:34.000000 dxpy-v0.83.0/dxpy/packages/requests/packages/charade/constants.py
+-rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)     9457 2014-02-05 22:02:34.000000 dxpy-v0.83.0/dxpy/packages/requests/packages/charade/chardistribution.py
+-rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)    34872 2014-02-05 22:02:34.000000 dxpy-v0.83.0/dxpy/packages/requests/packages/charade/euctwfreq.py
+-rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)    36011 2014-02-05 22:02:34.000000 dxpy-v0.83.0/dxpy/packages/requests/packages/charade/gb2312freq.py
+-rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)     1726 2014-02-05 22:02:34.000000 dxpy-v0.83.0/dxpy/packages/requests/packages/charade/big5prober.py
+-rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)     3825 2014-02-05 22:02:34.000000 dxpy-v0.83.0/dxpy/packages/requests/packages/charade/sjisprober.py
+-rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)    11475 2014-02-05 22:02:34.000000 dxpy-v0.83.0/dxpy/packages/requests/packages/charade/langthaimodel.py
+-rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)     1902 2014-02-05 22:02:34.000000 dxpy-v0.83.0/dxpy/packages/requests/packages/charade/charsetprober.py
+-rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)     1327 2014-02-05 22:02:34.000000 dxpy-v0.83.0/dxpy/packages/requests/packages/charade/__init__.py
+drwxrwsr-x   0 dnanexus  (1002) dnanexus  (1002)        0 2014-02-05 22:02:35.000000 dxpy-v0.83.0/dxpy/packages/requests/packages/urllib3/
+-rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)     5873 2014-02-05 22:02:34.000000 dxpy-v0.83.0/dxpy/packages/requests/packages/urllib3/request.py
+-rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)    22855 2014-02-05 22:02:34.000000 dxpy-v0.83.0/dxpy/packages/requests/packages/urllib3/connectionpool.py
+-rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)     8897 2014-02-05 22:02:34.000000 dxpy-v0.83.0/dxpy/packages/requests/packages/urllib3/poolmanager.py
+-rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)     2903 2014-02-05 22:02:34.000000 dxpy-v0.83.0/dxpy/packages/requests/packages/urllib3/_collections.py
+drwxrwsr-x   0 dnanexus  (1002) dnanexus  (1002)        0 2014-02-05 22:02:35.000000 dxpy-v0.83.0/dxpy/packages/requests/packages/urllib3/packages/
+-rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)     8936 2014-02-05 22:02:34.000000 dxpy-v0.83.0/dxpy/packages/requests/packages/urllib3/packages/ordered_dict.py
+drwxrwsr-x   0 dnanexus  (1002) dnanexus  (1002)        0 2014-02-05 22:02:35.000000 dxpy-v0.83.0/dxpy/packages/requests/packages/urllib3/packages/ssl_match_hostname/
+-rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)     2174 2014-02-05 22:02:34.000000 dxpy-v0.83.0/dxpy/packages/requests/packages/urllib3/packages/ssl_match_hostname/__init__.py
+-rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)    11628 2014-02-05 22:02:34.000000 dxpy-v0.83.0/dxpy/packages/requests/packages/urllib3/packages/six.py
+-rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)       74 2014-02-05 22:02:34.000000 dxpy-v0.83.0/dxpy/packages/requests/packages/urllib3/packages/__init__.py
+-rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)    10972 2014-02-05 22:02:34.000000 dxpy-v0.83.0/dxpy/packages/requests/packages/urllib3/util.py
+-rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)     3049 2014-02-05 22:02:34.000000 dxpy-v0.83.0/dxpy/packages/requests/packages/urllib3/filepost.py
+drwxrwsr-x   0 dnanexus  (1002) dnanexus  (1002)        0 2014-02-05 22:02:35.000000 dxpy-v0.83.0/dxpy/packages/requests/packages/urllib3/contrib/
+-rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)     4740 2014-02-05 22:02:34.000000 dxpy-v0.83.0/dxpy/packages/requests/packages/urllib3/contrib/ntlmpool.py
+-rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)     5235 2014-02-05 22:02:34.000000 dxpy-v0.83.0/dxpy/packages/requests/packages/urllib3/contrib/pyopenssl.py
+-rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)        0 2014-02-05 22:02:34.000000 dxpy-v0.83.0/dxpy/packages/requests/packages/urllib3/contrib/__init__.py
+-rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)     2258 2014-02-05 22:02:34.000000 dxpy-v0.83.0/dxpy/packages/requests/packages/urllib3/exceptions.py
+-rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)     8245 2014-02-05 22:02:34.000000 dxpy-v0.83.0/dxpy/packages/requests/packages/urllib3/response.py
+-rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)     1692 2014-02-05 22:02:34.000000 dxpy-v0.83.0/dxpy/packages/requests/packages/urllib3/__init__.py
+-rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)       62 2014-02-05 22:02:34.000000 dxpy-v0.83.0/dxpy/packages/requests/packages/__init__.py
+-rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)    14112 2014-02-05 22:02:34.000000 dxpy-v0.83.0/dxpy/packages/requests/cookies.py
+-rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)     3576 2014-02-05 22:02:34.000000 dxpy-v0.83.0/dxpy/packages/requests/structures.py
+-rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)    21905 2014-02-05 22:02:34.000000 dxpy-v0.83.0/dxpy/packages/requests/models.py
+-rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)     2433 2014-02-05 22:02:34.000000 dxpy-v0.83.0/dxpy/packages/requests/compat.py
+-rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)   211059 2014-02-05 22:02:34.000000 dxpy-v0.83.0/dxpy/packages/requests/cacert.pem
+-rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)    12616 2014-02-05 22:02:34.000000 dxpy-v0.83.0/dxpy/packages/requests/adapters.py
+-rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)     5531 2014-02-05 22:02:34.000000 dxpy-v0.83.0/dxpy/packages/requests/auth.py
+-rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)     1246 2014-02-05 22:02:34.000000 dxpy-v0.83.0/dxpy/packages/requests/exceptions.py
+-rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)    16299 2014-02-05 22:02:34.000000 dxpy-v0.83.0/dxpy/packages/requests/utils.py
+-rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)     1863 2014-02-05 22:02:34.000000 dxpy-v0.83.0/dxpy/packages/requests/__init__.py
+-rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)        0 2014-02-05 22:02:34.000000 dxpy-v0.83.0/dxpy/packages/__init__.py
+-rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)       20 2014-02-05 22:02:34.000000 dxpy-v0.83.0/dxpy/toolkit_version.py
+drwxrwsr-x   0 dnanexus  (1002) dnanexus  (1002)        0 2014-02-05 22:02:35.000000 dxpy-v0.83.0/dxpy/utils/
+-rwxrwxr-x   0 dnanexus  (1002) dnanexus  (1002)     7346 2014-02-05 22:02:34.000000 dxpy-v0.83.0/dxpy/utils/pretty_print.py
+-rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)     5741 2014-02-05 22:02:34.000000 dxpy-v0.83.0/dxpy/utils/app_unbuilder.py
+-rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)     4414 2014-02-05 22:02:34.000000 dxpy-v0.83.0/dxpy/utils/job_log_client.py
+-rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)     2420 2014-02-05 22:02:34.000000 dxpy-v0.83.0/dxpy/utils/pathmatch.py
+-rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)     7957 2014-02-05 22:02:34.000000 dxpy-v0.83.0/dxpy/utils/env.py
+-rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)    38702 2014-02-05 22:02:34.000000 dxpy-v0.83.0/dxpy/utils/describe.py
+-rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)     4331 2014-02-05 22:02:34.000000 dxpy-v0.83.0/dxpy/utils/printing.py
+-rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)     8197 2014-02-05 22:02:34.000000 dxpy-v0.83.0/dxpy/utils/exec_utils.py
+-rwxrwxr-x   0 dnanexus  (1002) dnanexus  (1002)    18464 2014-02-05 22:02:34.000000 dxpy-v0.83.0/dxpy/utils/local_exec_utils.py
+-rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)    32891 2014-02-05 22:02:34.000000 dxpy-v0.83.0/dxpy/utils/resolver.py
+-rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)      546 2014-02-05 22:02:34.000000 dxpy-v0.83.0/dxpy/utils/genomic_utils.py
+-rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)    19222 2014-02-05 22:02:34.000000 dxpy-v0.83.0/dxpy/utils/completer.py
+-rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)    11895 2014-02-05 22:02:34.000000 dxpy-v0.83.0/dxpy/utils/__init__.py
+drwxrwsr-x   0 dnanexus  (1002) dnanexus  (1002)        0 2014-02-05 22:02:35.000000 dxpy-v0.83.0/dxpy/templating/
+-rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)     6277 2014-02-05 22:02:34.000000 dxpy-v0.83.0/dxpy/templating/python.py
+-rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)     4683 2014-02-05 22:02:34.000000 dxpy-v0.83.0/dxpy/templating/bash.py
+-rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)     6502 2014-02-05 22:02:34.000000 dxpy-v0.83.0/dxpy/templating/cpp.py
+-rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)    18656 2014-02-05 22:02:34.000000 dxpy-v0.83.0/dxpy/templating/utils.py
+-rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)      674 2014-02-05 22:02:34.000000 dxpy-v0.83.0/dxpy/templating/__init__.py
+-rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)      387 2014-02-05 22:02:34.000000 dxpy-v0.83.0/dxpy/compat.py
+-rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)     7752 2014-02-05 22:02:34.000000 dxpy-v0.83.0/dxpy/exceptions.py
+drwxrwsr-x   0 dnanexus  (1002) dnanexus  (1002)        0 2014-02-05 22:02:35.000000 dxpy-v0.83.0/dxpy/cli/
+-rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)    18757 2014-02-05 22:02:34.000000 dxpy-v0.83.0/dxpy/cli/parsers.py
+-rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)    30930 2014-02-05 22:02:34.000000 dxpy-v0.83.0/dxpy/cli/exec_io.py
+-rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)    10561 2014-02-05 22:02:34.000000 dxpy-v0.83.0/dxpy/cli/workflow.py
+-rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)     1049 2014-02-05 22:02:34.000000 dxpy-v0.83.0/dxpy/cli/__init__.py
+-rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)    24367 2014-02-05 22:02:34.000000 dxpy-v0.83.0/dxpy/__init__.py
+-rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)      224 2014-02-05 22:02:35.000000 dxpy-v0.83.0/setup.cfg
+drwxrwsr-x   0 dnanexus  (1002) dnanexus  (1002)        0 2014-02-05 22:02:35.000000 dxpy-v0.83.0/scripts/
+-rwxrwxr-x   0 dnanexus  (1002) dnanexus  (1002)     7815 2014-02-05 22:02:34.000000 dxpy-v0.83.0/scripts/dx-jobutil-add-output
+-rwxrwxr-x   0 dnanexus  (1002) dnanexus  (1002)     1693 2014-02-05 22:02:34.000000 dxpy-v0.83.0/scripts/dx-fetch-bundled-depends
+-rwxrwxr-x   0 dnanexus  (1002) dnanexus  (1002)     1620 2014-02-05 22:02:34.000000 dxpy-v0.83.0/scripts/dx-jobutil-report-error
+-rwxrwxr-x   0 dnanexus  (1002) dnanexus  (1002)    18367 2014-02-05 22:02:34.000000 dxpy-v0.83.0/scripts/dx-app-wizard
+-rwxrwxr-x   0 dnanexus  (1002) dnanexus  (1002)     1349 2014-02-05 22:02:34.000000 dxpy-v0.83.0/scripts/dx-jobutil-dxlink
+-rwxrwxr-x   0 dnanexus  (1002) dnanexus  (1002)     1381 2014-02-05 22:02:34.000000 dxpy-v0.83.0/scripts/dx-jobutil-parse-link
+-rwxrwxr-x   0 dnanexus  (1002) dnanexus  (1002)     1762 2014-02-05 22:02:34.000000 dxpy-v0.83.0/scripts/dx-log-stream
+-rwxrwxr-x   0 dnanexus  (1002) dnanexus  (1002)    18418 2014-02-05 22:02:34.000000 dxpy-v0.83.0/scripts/dx-mount
+-rwxrwxr-x   0 dnanexus  (1002) dnanexus  (1002)     7001 2014-02-05 22:02:34.000000 dxpy-v0.83.0/scripts/dx-run-app-locally
+-rwxrwxr-x   0 dnanexus  (1002) dnanexus  (1002)    12950 2014-02-05 22:02:34.000000 dxpy-v0.83.0/scripts/dx-workflow-to-applet
+-rwxrwxr-x   0 dnanexus  (1002) dnanexus  (1002)     2335 2014-02-05 22:02:34.000000 dxpy-v0.83.0/scripts/dx-jobutil-new-job
+-rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)      132 2014-02-05 22:02:34.000000 dxpy-v0.83.0/MANIFEST.in
+-rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)       24 2014-02-05 22:02:34.000000 dxpy-v0.83.0/requirements_test.txt
+-rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)      144 2014-02-05 22:02:34.000000 dxpy-v0.83.0/requirements.txt
+-rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)       27 2014-02-05 22:02:34.000000 dxpy-v0.83.0/requirements_dxfs.txt
+-rw-rw-r--   0 dnanexus  (1002) dnanexus  (1002)      767 2014-02-05 22:02:35.000000 dxpy-v0.83.0/PKG-INFO
```

### Comparing `dxpy-v0.82.1/setup.py` & `dxpy-v0.83.0/setup.py`

 * *Files identical despite different names*

### Comparing `dxpy-v0.82.1/dxpy.egg-info/SOURCES.txt` & `dxpy-v0.83.0/dxpy.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -131,14 +131,15 @@
 dxpy/scripts/dx_variants_to_vcf.py
 dxpy/templating/__init__.py
 dxpy/templating/bash.py
 dxpy/templating/cpp.py
 dxpy/templating/python.py
 dxpy/templating/utils.py
 dxpy/utils/__init__.py
+dxpy/utils/app_unbuilder.py
 dxpy/utils/completer.py
 dxpy/utils/describe.py
 dxpy/utils/env.py
 dxpy/utils/exec_utils.py
 dxpy/utils/genomic_utils.py
 dxpy/utils/job_log_client.py
 dxpy/utils/local_exec_utils.py
```

### Comparing `dxpy-v0.82.1/dxpy.egg-info/entry_points.txt` & `dxpy-v0.83.0/dxpy.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `dxpy-v0.82.1/dxpy.egg-info/PKG-INFO` & `dxpy-v0.83.0/dxpy.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: dxpy
-Version: v0.82.1
+Version: v0.83.0
 Summary: DNAnexus Platform API bindings for Python
 Home-page: https://github.com/dnanexus/dx-toolkit
 Author: Katherine Lai, Phil Sung, Andrey Kislyuk, Anurag Biyani
 Author-email: expert-dev@dnanexus.com
 License: Apache Software License
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `dxpy-v0.82.1/test/test_dx_completion.py` & `dxpy-v0.83.0/test/test_dx_completion.py`

 * *Files identical despite different names*

### Comparing `dxpy-v0.82.1/test/test_dxpy.py` & `dxpy-v0.83.0/test/test_dxpy.py`

 * *Files identical despite different names*

### Comparing `dxpy-v0.82.1/test/coveragereport.py` & `dxpy-v0.83.0/test/coveragereport.py`

 * *Files identical despite different names*

### Comparing `dxpy-v0.82.1/test/dxpy_testutil.py` & `dxpy-v0.83.0/test/dxpy_testutil.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # -*- coding: utf-8 -*-
 
+from __future__ import print_function
+
 import platform, locale, sys
 sys_encoding = locale.getdefaultlocale()[1] or 'UTF-8'
 if platform.python_implementation() != "PyPy":
     try:
         reload(sys).setdefaultencoding(sys_encoding)
     except:
         pass
@@ -31,15 +33,15 @@
         if 'DX_CLI_WD' in os.environ:
             del os.environ['DX_CLI_WD']
 
     def tearDown(self):
         try:
             subprocess.check_call(u"dx rmproject --yes --quiet {p}".format(p=self.project), shell=True)
         except Exception as e:
-            print "Failed to remove test project:", str(e)
+            print("Failed to remove test project:", str(e))
         if 'DX_PROJECT_CONTEXT_ID' in os.environ:
             del os.environ['DX_PROJECT_CONTEXT_ID']
         if 'DX_CLI_WD' in os.environ:
             del os.environ['DX_CLI_WD']
 
     # Be sure to use the check_output defined in this module if you wish
     # to use stderr_regexp. Python's usual subprocess.check_output
@@ -47,18 +49,18 @@
     @contextmanager
     def assertSubprocessFailure(self, output_regexp=None, stderr_regexp=None, exit_code=3):
         try:
             yield
         except subprocess.CalledProcessError as e:
             self.assertEqual(exit_code, e.returncode, "Expected command to return code %d but it returned code %d" % (exit_code, e.returncode))
             if output_regexp:
-                print "stdout:"
-                print e.output
+                print("stdout:")
+                print(e.output)
                 self.assertTrue(re.search(output_regexp, e.output), "Expected stdout to match '%s' but it didn't" % (output_regexp,))
             if stderr_regexp:
                 if not hasattr(e, 'stderr'):
                     raise Exception('A stderr_regexp was supplied but the CalledProcessError did not return the contents of stderr')
-                print "stderr:"
-                print e.stderr
+                print("stderr:")
+                print(e.stderr)
                 self.assertTrue(re.search(stderr_regexp, e.stderr), "Expected stderr to match '%s' but it didn't" % (stderr_regexp,))
             return
         self.assertFalse(True, "Expected command to fail with CalledProcessError but it succeeded")
```

### Comparing `dxpy-v0.82.1/test/test_dxpy_utils.py` & `dxpy-v0.83.0/test/test_dxpy_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,17 +13,20 @@
 #
 #   Unless required by applicable law or agreed to in writing, software
 #   distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 #   WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 #   License for the specific language governing permissions and limitations
 #   under the License.
 
+from __future__ import print_function
+
 import os, unittest, json, tempfile, subprocess, csv, shutil, re, time
 from dxpy import AppError
 from dxpy.utils import (describe, exec_utils, genomic_utils, response_iterator, get_futures_threadpool)
+from dxpy.compat import is_py2
 
 class TestDescribe(unittest.TestCase):
     def test_is_job_ref(self):
         # Positive results
         jobref = {"job": "job-B55ZF5kZKQGz1Xxyb5FQ0003", "field": "number"}
         self.assertTrue(describe.is_job_ref(jobref))
         jobref = {"$dnanexus_link": jobref}
@@ -53,39 +56,44 @@
         self.assertIn("job-B55ZF5kZKQGz1Xxyb5FQ0003:number", resolved_jbors)
 
 class TestErrorSanitizing(unittest.TestCase):
     def test_error_sanitizing(self):
         # ASCII str
         self.assertEqual(exec_utils._safe_unicode(ValueError("foo")), "foo")
         # UTF-8 encoded str
-        self.assertEqual(exec_utils._safe_unicode(ValueError(u"crème".encode("utf-8"))), u"cr\xe8me")
+        self.assertEqual(exec_utils._safe_unicode(ValueError(u"crème".encode("utf-8"))),
+                         u"cr\xe8me" if is_py2 else u"b'cr\\xc3\\xa8me'")
         # Unicode obj
         self.assertEqual(exec_utils._safe_unicode(ValueError(u"brûlée")), u"br\xfbl\xe9e")
         # Not UTF-8
-        self.assertEqual(exec_utils._safe_unicode(ValueError(u"Invalid read name: DÑÁnèxûs".encode("ISO-8859-1"))),
-                         "Invalid read name: D??n?x?s [Raw error message: 496e76616c69642072656164206e616d653a2044d1c16ee878fb73]")
+        if is_py2:
+            expected = "Invalid read name: D??n?x?s [Raw error message: 496e76616c69642072656164206e616d653a2044d1c16ee878fb73]"
+        else:
+            expected = "b'Invalid read name: D\\xd1\\xc1n\\xe8x\\xfbs'"
+        self.assertEqual(exec_utils._safe_unicode(ValueError(u"Invalid read name: DÑÁnèxûs".encode("ISO-8859-1"))), expected)
 
     def test_formatting_exceptions(self):
         self.assertEqual(exec_utils._format_exception_message(ValueError("foo")), "ValueError: foo")
         self.assertEqual(exec_utils._format_exception_message(AppError("foo")), "foo")
 
 class TestGenomicUtils(unittest.TestCase):
     def test_reverse_complement(self):
-        self.assertEqual("TTTTAAACCG", genomic_utils.reverse_complement("CGGTTTAAAA"))
-        self.assertEqual("TTTTAAACCG", genomic_utils.reverse_complement(u"CGGTTTAAAA"))
-        self.assertEqual("TTTTAAACCG", genomic_utils.reverse_complement("cggtttaaaa"))
-        self.assertEqual("TTTTAAACCG", genomic_utils.reverse_complement(u"cggtttaaaa"))
-        self.assertEqual("NNNNNTTTTAAACCG", genomic_utils.reverse_complement("CGGTTTAAAANNNNN"))
+        self.assertEqual(b"TTTTAAACCG", genomic_utils.reverse_complement(b"CGGTTTAAAA"))
+        self.assertEqual(b"TTTTAAACCG", genomic_utils.reverse_complement(u"CGGTTTAAAA"))
+        self.assertEqual(b"TTTTAAACCG", genomic_utils.reverse_complement(b"cggtttaaaa"))
+        self.assertEqual(b"TTTTAAACCG", genomic_utils.reverse_complement(u"cggtttaaaa"))
+        self.assertEqual(b"NNNNNTTTTAAACCG", genomic_utils.reverse_complement(b"CGGTTTAAAANNNNN"))
+        self.assertEqual(b"NNNNNTTTTAAACCG", genomic_utils.reverse_complement(u"CGGTTTAAAANNNNN"))
         with self.assertRaises(ValueError):
             genomic_utils.reverse_complement("oops")
 
 class TestResponseIterator(unittest.TestCase):
     def test_basic_iteration(self):
         def task(i, sleep_for=1):
-            print "Task", i, "sleeping for", sleep_for
+            print("Task", i, "sleeping for", sleep_for)
             time.sleep(sleep_for)
             return i
 
         def tasks():
             for i in range(8):
                 yield task, [i], {"sleep_for": i/8.0}
```

### Comparing `dxpy-v0.82.1/test/test_dxclient.py` & `dxpy-v0.83.0/test/test_dxclient.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,16 @@
 #
 #   Unless required by applicable law or agreed to in writing, software
 #   distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 #   WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 #   License for the specific language governing permissions and limitations
 #   under the License.
 
+from __future__ import print_function
+
 import os, sys, unittest, json, tempfile, subprocess, csv, shutil, re, base64, random, time
 from contextlib import contextmanager
 import pexpect
 
 import dxpy
 from dxpy.scripts import dx_build_app
 from dxpy_testutil import DXTestCase
@@ -58,26 +60,26 @@
         raise ValueError('stdout argument not allowed, it will be overridden.')
     if 'stderr' in kwargs:
         raise ValueError('stderr argument not allowed, it will be overridden.')
     process = subprocess.Popen(stdout=subprocess.PIPE, stderr=subprocess.PIPE, *popenargs, **kwargs)
     output, err = process.communicate()
     retcode = process.poll()
     if retcode:
-        print err
+        print(err)
         cmd = kwargs.get("args")
         if cmd is None:
             cmd = popenargs[0]
         exc = DXCalledProcessError(retcode, cmd, output=output, stderr=err)
         raise exc
     return output
 
 def run(command, **kwargs):
-    print "$ %s" % (command,)
+    print("$ %s" % (command,))
     output = check_output(command, shell=True, **kwargs)
-    print output
+    print(output)
     return output
 
 def overrideEnvironment(**kwargs):
     env = os.environ.copy()
     for key in kwargs:
         if kwargs[key] is None:
             if key in env:
@@ -477,20 +479,20 @@
         shell1.sendline("dx env")
         expect_dx_env_cwd(shell1, "sessiontest1")
         # Grandchild subprocess inherits session
         try:
             shell1.sendline("bash -c 'dx env'")
             expect_dx_env_cwd(shell1, "sessiontest1")
         except:
-            print "*** TODO: FIXME: Unable to verify that grandchild subprocess inherited session"
-            print "*** Begin test_dxpy_session_isolation debug data"
-            print str(shell1)
-            print "*** test_dxpy_session_isolation debug data, begin buffer:"
-            print str(shell1.buffer)
-            print "*** End test_dxpy_session_isolation debug data"
+            print("*** TODO: FIXME: Unable to verify that grandchild subprocess inherited session")
+            print("*** Begin test_dxpy_session_isolation debug data")
+            print(str(shell1))
+            print("*** test_dxpy_session_isolation debug data, begin buffer:")
+            print(str(shell1.buffer))
+            print("*** End test_dxpy_session_isolation debug data")
 
 class TestDXClientUploadDownload(DXTestCase):
     def test_dx_upload_download(self):
         with self.assertSubprocessFailure(stderr_regexp='expected the path to be a non-empty string', exit_code=3):
             run('dx download ""')
         wd = tempfile.mkdtemp()
         os.mkdir(os.path.join(wd, "a"))
@@ -843,15 +845,15 @@
         applet_id = dxpy.api.applet_new({"project": self.project,
                                          "dxapi": "1.0.0",
                                          "inputSpec": [{"name": "number", "class": "int"}],
                                          "outputSpec": [{"name": "number", "class": "int"}],
                                          "runSpec": {"interpreter": "bash",
                                                      "code": "exit 1"}
                                          })['id']
-        workflow_id = dxpy.api.workflow_new({"project": self.project})['id']
+        workflow_id = run("dx new workflow myworkflow --brief").strip()
         stage_id = dxpy.api.workflow_add_stage(workflow_id,
                                                {"editVersion": 0, "executable": applet_id})['stage']
         analysis_id = run("dx run " + workflow_id + " -i0.number=32 -y --brief").strip()
         self.assertTrue(analysis_id.startswith('analysis-'))
         analysis_desc = run("dx describe " + analysis_id)
         self.assertIn(stage_id + '.number = 32', analysis_desc)
         analysis_desc = json.loads(run("dx describe " + analysis_id + " --json"))
@@ -886,14 +888,20 @@
         with self.assertSubprocessFailure(stderr_regexp='Some inputs.+are missing', exit_code=3):
             run("dx run " + workflow_id + " -y")
 
         # Setting the input in the workflow allows it to be run
         run("dx update stage " + workflow_id + " 0 -inumber=42")
         run("dx run " + workflow_id + " -y")
 
+        # initialize a new workflow from an analysis
+        new_workflow_desc = run("dx new workflow --init " + analysis_id)
+        self.assertNotIn(workflow_id, new_workflow_desc)
+        self.assertIn(analysis_id, new_workflow_desc)
+        self.assertIn(stage_id, new_workflow_desc)
+
     @unittest.skipUnless(testutil.TEST_RUN_JOBS, 'skipping test that runs jobs')
     def test_dx_run_workflow_prints_cached_executions(self):
         applet_id = dxpy.api.applet_new({"project": self.project,
                                          "name": "myapplet",
                                          "dxapi": "1.0.0",
                                          "inputSpec": [{"name": "number", "class": "int"}],
                                          "outputSpec": [{"name": "number", "class": "int"}],
@@ -1008,14 +1016,49 @@
         self.assertEqual(desc["name"], u"wØrkflØwname")
         self.assertEqual(desc["title"], u"тitle")
         self.assertEqual(desc["summary"], u"SΨmmary")
         self.assertEqual(desc["description"], u"DΣsc")
         self.assertEqual(desc["outputFolder"], u"/wØrkflØwØutput")
         self.assertEqual(desc["project"], self.project)
 
+        # add some stages and then create a new one initializing from
+        # the first
+        applet_id = dxpy.api.applet_new({"name": "myapplet",
+                                         "project": self.project,
+                                         "dxapi": "1.0.0",
+                                         "inputSpec": [],
+                                         "outputSpec": [],
+                                         "runSpec": {"interpreter": "bash", "code": ""}
+                                         })['id']
+        run(u"dx add stage wØrkflØwname " + applet_id)
+
+        new_workflow_id = run(u"dx new workflow --init wØrkflØwname --title newtitle " +
+                              u"--summary newsummary --output-folder /output --brief").strip()
+        desc = dxpy.describe(new_workflow_id)
+        self.assertNotEqual(new_workflow_id, workflow_id)
+        self.assertEqual(desc["id"], new_workflow_id)
+        self.assertEqual(desc["editVersion"], 0)
+        self.assertEqual(desc["name"], u"wØrkflØwname")
+        self.assertEqual(desc["title"], "newtitle")
+        self.assertEqual(desc["summary"], "newsummary")
+        self.assertEqual(desc["description"], u"DΣsc")
+        self.assertEqual(desc["outputFolder"], "/output")
+        self.assertEqual(desc["project"], self.project)
+        self.assertEqual(len(desc["stages"]), 1)
+        self.assertEqual(desc["stages"][0]["executable"], applet_id)
+
+        # run without --brief; should see initializedFrom information
+        new_workflow_desc = run(u"dx new workflow --init " + workflow_id)
+        self.assertIn(workflow_id, new_workflow_desc)
+
+        # error when initializing from a nonexistent workflow
+        run("dx rm " + workflow_id)
+        with self.assertSubprocessFailure(stderr_regexp='ResourceNotFound', exit_code=3):
+            run("dx new workflow --init " + workflow_id)
+
     def test_dx_workflow_resolution(self):
         with self.assertSubprocessFailure(stderr_regexp='Could not resolve', exit_code=3):
             run("dx update workflow foo")
 
         record_id = run("dx new record --type pipeline --brief").strip()
         run("dx describe " + record_id)
         with self.assertSubprocessFailure(stderr_regexp='Could not resolve', exit_code=3):
@@ -1047,14 +1090,19 @@
                                          "dxapi": "1.0.0",
                                          "inputSpec": [{"name": "number", "class": "int"}],
                                          "outputSpec": [{"name": "number", "class": "int"}],
                                          "runSpec": {"interpreter": "bash",
                                                      "code": "exit 0"}
                                          })['id']
         stage_ids = []
+
+        # list stages when there are no stages yet
+        list_output = run("dx list stages myworkflow")
+        self.assertIn("No stages", list_output)
+
         stage_ids.append(run("dx add stage " + workflow_id + " --name first " + applet_id + " --brief").strip())
         # not-yet-existing folder path should work
         # also, set input and instance type
         stage_ids.append(run("dx add stage myworkflow --relative-output-folder output myapplet --brief -inumber=32 --instance-type dx_m1.large").strip())
         # test relative folder path
         run("dx mkdir -p a/b/c")
         run("dx cd a/b/c")
@@ -1100,24 +1148,26 @@
             self.assertIn("Stage " + str(i), list_output)
         self.assertIn("<workflow output folder>/output", list_output)
         self.assertIn("number=32", list_output)
         self.assertIn("/a/b/c", list_output)
 
         run("dx describe " + workflow_id)
         # remove a stage by index
-        run("dx remove stage /myworkflow 1")
+        remove_output = run("dx remove stage /myworkflow 1")
+        self.assertIn(stage_ids[1], remove_output)
         desc = dxpy.api.workflow_describe(workflow_id)
         self.assertEqual(len(desc['stages']), 2)
         self.assertEqual(desc['stages'][0]['id'], stage_ids[0])
         self.assertEqual(desc['stages'][0]['folder'], None)
         self.assertEqual(desc['stages'][1]['id'], stage_ids[2])
         self.assertEqual(desc['stages'][1]['folder'], '/a/b/c')
 
         # remove a stage by ID
-        run("dx remove stage " + workflow_id + " " + stage_ids[0])
+        remove_output = run("dx remove stage " + workflow_id + " " + stage_ids[0] + ' --brief').strip()
+        self.assertEqual(remove_output, stage_ids[0])
         desc = dxpy.api.workflow_describe(workflow_id)
         self.assertEqual(len(desc['stages']), 1)
         self.assertEqual(desc['stages'][0]['id'], stage_ids[2])
         self.assertEqual(desc['stages'][0]['name'], 'second')
         self.assertEqual(desc['stages'][0]['folder'], '/a/b/c')
 
         # remove a stage by name
@@ -1565,23 +1615,23 @@
                      'skipping HTTP Proxy support test that needs squid3')
 class TestHTTPProxySupport(DXTestCase):
     def setUp(self):
         squid_wd = os.path.join(os.path.dirname(__file__), 'http_proxy')
         self.proxy_process = subprocess.Popen(['squid3', '-N', '-f', 'squid.conf'], cwd=squid_wd)
         time.sleep(1)
 
-        print "Waiting for squid to come up..."
+        print("Waiting for squid to come up...")
         t = 0
         while True:
             try:
                 if requests.get("http://localhost:3129").status_code == requests.codes.bad_request:
                     if self.proxy_process.poll() is not None:
                         # Got a response on port 3129, but our proxy quit with an error, so it must be another process.
                         raise Exception("Tried launching squid, but port 3129 is already bound")
-                    print "squid is up"
+                    print("squid is up")
                     break
             except requests.exceptions.RequestException:
                 pass
             time.sleep(0.5)
             t += 1
             if t > 16:
                 raise Exception("Failed to launch Squid")
@@ -2177,15 +2227,15 @@
             "inputSpec": [],
             "outputSpec": [],
             "version": "1.0.0"
             }
         app_dir = self.write_app_directory("build_app_autonumbering", json.dumps(app_spec), "code.py")
         run("dx build --create-app --json --publish " + app_dir)
         with self.assertSubprocessFailure(stderr_regexp="Could not create"):
-            print run("dx build --create-app --json --no-version-autonumbering " + app_dir)
+            print(run("dx build --create-app --json --no-version-autonumbering " + app_dir))
         run("dx build --create-app --json " + app_dir) # Creates autonumbered version
 
     def test_build_failure(self):
         app_spec = {
             "name": "build_failure",
             "dxapi": "1.0.0",
             "runSpec": {"file": "code.py", "interpreter": "python2.7"},
```

### Comparing `dxpy-v0.82.1/test/test_dxfs.py` & `dxpy-v0.83.0/test/test_dxfs.py`

 * *Files identical despite different names*

### Comparing `dxpy-v0.82.1/test/test_dx_app_wizard_and_run_app_locally.py` & `dxpy-v0.83.0/test/test_dx_app_wizard_and_run_app_locally.py`

 * *Files identical despite different names*

### Comparing `dxpy-v0.82.1/dxpy/bindings/dxapp.py` & `dxpy-v0.83.0/dxpy/bindings/dxapp.py`

 * *Files identical despite different names*

### Comparing `dxpy-v0.82.1/dxpy/bindings/dxanalysis.py` & `dxpy-v0.83.0/dxpy/bindings/dxanalysis.py`

 * *Files identical despite different names*

### Comparing `dxpy-v0.82.1/dxpy/bindings/dxapplet.py` & `dxpy-v0.83.0/dxpy/bindings/dxapplet.py`

 * *Files identical despite different names*

### Comparing `dxpy-v0.82.1/dxpy/bindings/search.py` & `dxpy-v0.83.0/dxpy/bindings/search.py`

 * *Files identical despite different names*

### Comparing `dxpy-v0.82.1/dxpy/bindings/dxapp_container_functions.py` & `dxpy-v0.83.0/dxpy/bindings/dxapp_container_functions.py`

 * *Files identical despite different names*

### Comparing `dxpy-v0.82.1/dxpy/bindings/dxworkflow.py` & `dxpy-v0.83.0/dxpy/bindings/dxworkflow.py`

 * *Files 0% similar despite different names*

```diff
@@ -110,16 +110,17 @@
                 if not (isinstance(kwargs["init_from"], (DXWorkflow, DXAnalysis)) or \
                         (isinstance(kwargs["init_from"], basestring) and \
                          re.compile('^analysis-[0-9A-Za-z]{24}$').match(kwargs["init_from"]))):
                     raise DXError("Expected init_from to be an instance of DXWorkflow or DXAnalysis, or to be a string analysis ID.")
                 if isinstance(kwargs["init_from"], basestring):
                     dx_hash["initializeFrom"] = {"id": kwargs["init_from"]}
                 else:
-                    dx_hash["initializeFrom"] = {"id": kwargs["init_from"].get_id(),
-                                                 "project": kwargs["init_from"].get_proj_id()}
+                    dx_hash["initializeFrom"] = {"id": kwargs["init_from"].get_id()}
+                    if isinstance(kwargs["init_from"], DXWorkflow):
+                        dx_hash["initializeFrom"]["project"] = kwargs["init_from"].get_proj_id()
             del kwargs["init_from"]
 
         if "title" in kwargs:
             if kwargs["title"] is not None:
                 dx_hash["title"] = kwargs["title"]
             del kwargs["title"]
```

### Comparing `dxpy-v0.82.1/dxpy/bindings/dxfile.py` & `dxpy-v0.83.0/dxpy/bindings/dxfile.py`

 * *Files 0% similar despite different names*

```diff
@@ -506,16 +506,15 @@
 
     def _next_response_content(self):
         if self._http_threadpool is None:
             DXFile._http_threadpool = dxpy.utils.get_futures_threadpool(max_workers=self._http_threadpool_size)
 
         if self._response_iterator is None:
             self._response_iterator = dxpy.utils.response_iterator(self._request_iterator, self._http_threadpool,
-                                                                   max_active_tasks=self._http_threadpool_size,
-                                                                   num_retries=1)
+                                                                   max_active_tasks=self._http_threadpool_size)
         return next(self._response_iterator)
 
     def read(self, length=None, use_compression=None, **kwargs):
         '''
         :param size: Maximum number of bytes to be read
         :type size: integer
         :rtype: string
```

### Comparing `dxpy-v0.82.1/dxpy/bindings/dxdataobject_functions.py` & `dxpy-v0.83.0/dxpy/bindings/dxdataobject_functions.py`

 * *Files identical despite different names*

### Comparing `dxpy-v0.82.1/dxpy/bindings/dxgtable_functions.py` & `dxpy-v0.83.0/dxpy/bindings/dxgtable_functions.py`

 * *Files identical despite different names*

### Comparing `dxpy-v0.82.1/dxpy/bindings/dxgtable.py` & `dxpy-v0.83.0/dxpy/bindings/dxgtable.py`

 * *Files identical despite different names*

### Comparing `dxpy-v0.82.1/dxpy/bindings/dxfile_functions.py` & `dxpy-v0.83.0/dxpy/bindings/dxfile_functions.py`

 * *Files identical despite different names*

### Comparing `dxpy-v0.82.1/dxpy/bindings/dxrecord.py` & `dxpy-v0.83.0/dxpy/bindings/dxrecord.py`

 * *Files identical despite different names*

### Comparing `dxpy-v0.82.1/dxpy/bindings/dxjob.py` & `dxpy-v0.83.0/dxpy/bindings/dxjob.py`

 * *Files identical despite different names*

### Comparing `dxpy-v0.82.1/dxpy/bindings/dxproject.py` & `dxpy-v0.83.0/dxpy/bindings/dxproject.py`

 * *Files identical despite different names*

### Comparing `dxpy-v0.82.1/dxpy/bindings/__init__.py` & `dxpy-v0.83.0/dxpy/bindings/__init__.py`

 * *Files identical despite different names*

### Comparing `dxpy-v0.82.1/dxpy/app_builder.py` & `dxpy-v0.83.0/dxpy/app_builder.py`

 * *Files identical despite different names*

### Comparing `dxpy-v0.82.1/dxpy/api.py` & `dxpy-v0.83.0/dxpy/api.py`

 * *Files identical despite different names*

### Comparing `dxpy-v0.82.1/dxpy/dxlog.py` & `dxpy-v0.83.0/dxpy/dxlog.py`

 * *Files identical despite different names*

### Comparing `dxpy-v0.82.1/dxpy/scripts/dx_fastq_to_reads.py` & `dxpy-v0.83.0/dxpy/scripts/dx_fastq_to_reads.py`

 * *Files identical despite different names*

### Comparing `dxpy-v0.82.1/dxpy/scripts/dx_genes_to_gtf.py` & `dxpy-v0.83.0/dxpy/scripts/dx_genes_to_gtf.py`

 * *Files identical despite different names*

### Comparing `dxpy-v0.82.1/dxpy/scripts/dx_gff_to_genes.py` & `dxpy-v0.83.0/dxpy/scripts/dx_gff_to_genes.py`

 * *Files identical despite different names*

### Comparing `dxpy-v0.82.1/dxpy/scripts/dx_mappings_to_sam.py` & `dxpy-v0.83.0/dxpy/scripts/dx_mappings_to_sam.py`

 * *Files identical despite different names*

### Comparing `dxpy-v0.82.1/dxpy/scripts/dx_mappings_to_fastq.py` & `dxpy-v0.83.0/dxpy/scripts/dx_mappings_to_fastq.py`

 * *Files identical despite different names*

### Comparing `dxpy-v0.82.1/dxpy/scripts/dx_variants_to_vcf.py` & `dxpy-v0.83.0/dxpy/scripts/dx_variants_to_vcf.py`

 * *Files identical despite different names*

### Comparing `dxpy-v0.82.1/dxpy/scripts/dx_csv_to_gtable.py` & `dxpy-v0.83.0/dxpy/scripts/dx_csv_to_gtable.py`

 * *Files identical despite different names*

### Comparing `dxpy-v0.82.1/dxpy/scripts/dx_reads_to_fastq.py` & `dxpy-v0.83.0/dxpy/scripts/dx_reads_to_fastq.py`

 * *Files identical despite different names*

### Comparing `dxpy-v0.82.1/dxpy/scripts/dx_gtable_to_tsv.py` & `dxpy-v0.83.0/dxpy/scripts/dx_gtable_to_tsv.py`

 * *Files identical despite different names*

### Comparing `dxpy-v0.82.1/dxpy/scripts/dx_gtable_to_csv.py` & `dxpy-v0.83.0/dxpy/scripts/dx_gtable_to_csv.py`

 * *Files identical despite different names*

### Comparing `dxpy-v0.82.1/dxpy/scripts/dx_gtf_to_genes.py` & `dxpy-v0.83.0/dxpy/scripts/dx_gtf_to_genes.py`

 * *Files identical despite different names*

### Comparing `dxpy-v0.82.1/dxpy/scripts/dx_build_app.py` & `dxpy-v0.83.0/dxpy/scripts/dx_build_app.py`

 * *Files identical despite different names*

### Comparing `dxpy-v0.82.1/dxpy/scripts/dx_genes_to_gff.py` & `dxpy-v0.83.0/dxpy/scripts/dx_genes_to_gff.py`

 * *Files identical despite different names*

### Comparing `dxpy-v0.82.1/dxpy/scripts/dx_bed_to_spans.py` & `dxpy-v0.83.0/dxpy/scripts/dx_bed_to_spans.py`

 * *Files identical despite different names*

### Comparing `dxpy-v0.82.1/dxpy/scripts/dx.py` & `dxpy-v0.83.0/dxpy/scripts/dx.py`

 * *Files 2% similar despite different names*

```diff
@@ -1863,126 +1863,14 @@
         err_exit(fill("Error: {path} could not be found".format(path=args.output)))
     else:
         destdir, dest_filename = os.getcwd(), args.output
 
     download_folders(folders_to_get, destdir)
     download_files(files_to_get, destdir, dest_filename=dest_filename)
 
-def dump_applet(applet, destination_directory):
-    """
-    Reconstitutes applet into a directory that would create a
-    functionally identical app if "dx build" were run on it.
-    destination_directory will be the root source directory for the
-    applet.
-
-    applet: DXApplet object to be dumped
-    destination_directory: an existing, empty, and writable directory
-    """
-    def recursive_cleanup(foo):
-        """
-        Aggressively cleans up things that look empty.
-        """
-        if isinstance(foo, dict):
-            for (key, val) in foo.items():
-                if isinstance(val, dict):
-                    recursive_cleanup(val)
-                if val == "" or val == [] or val == {}:
-                    del foo[key]
-
-    old_cwd = os.getcwd()
-    os.chdir(destination_directory)
-    try:
-        info = applet.get()
-
-        # Used only to obtain properties and details for the applet--
-        # everything else comes from the result of the get() method
-        # above.
-        describe_output = applet.describe(incl_properties=True, incl_details=True)
-
-        if info["runSpec"]["interpreter"] == "bash":
-            suffix = "sh"
-        elif info["runSpec"]["interpreter"] == "python2.7":
-            suffix = "py"
-        else:
-            parser.exit(1, fill('Sorry, I don\'t know how to get applets with interpreter ' + info["runSpec"]["interpreter"]) + '\n')
-
-        # Entry point script
-        script = "src/code.%s" % (suffix,)
-        os.mkdir("src")
-        with open(script, "w") as f:
-            f.write(info["runSpec"]["code"])
-
-        # resources/ directory
-        deps_to_remove = []
-        created_resources_directory = False
-        for dep in info["runSpec"]["bundledDepends"]:
-            handler = dxpy.get_handler(dep["id"])
-            if handler.__class__.__name__ == "DXFile":
-                if not created_resources_directory:
-                    os.mkdir("resources")
-                    created_resources_directory = True
-                fname = "resources/%s.tar.gz" % (handler.get_id())
-                dxpy.download_dxfile(handler.get_id(), fname)
-                subprocess.check_call(["tar", "-C", "resources", "-zxvf", fname], shell=False)
-                os.unlink(fname)
-                deps_to_remove.append(dep)
-
-        # TODO: if output directory is not the same as applet name we
-        # should print a warning and/or offer to rewrite the "name"
-        # field in the dxapp.json.
-        dxapp_json = collections.OrderedDict()
-        for key in ["name", "title", "summary", "types", "tags", "properties", "dxapi", "inputSpec", "outputSpec", "runSpec", "access", "details"]:
-            if key in ['properties', 'details']:
-                dxapp_json[key] = describe_output[key]
-            if key in info:
-                dxapp_json[key] = info[key]
-        if info.get("hidden", False):
-            dxapp_json["hidden"] = True
-        # TODO: inputSpec and outputSpec elements should have their keys
-        # printed in a sensible (or at least consistent) order too
-
-        # Un-inline code
-        del dxapp_json["runSpec"]["code"]
-        dxapp_json["runSpec"]["file"] = script
-
-        # Remove resources from bundledDepends
-        for dep in deps_to_remove:
-            dxapp_json["runSpec"]["bundledDepends"].remove(dep)
-
-        # Remove dx-toolkit from execDepends
-        dx_toolkit = {"name": "dx-toolkit", "package_manager": "apt"}
-        if dx_toolkit in dxapp_json["runSpec"]["execDepends"]:
-            dxapp_json["runSpec"]["execDepends"].remove(dx_toolkit)
-
-        # Cleanup of empty elements. Be careful not to let this step
-        # introduce any semantic changes to the app specification. For
-        # example, an empty input (output) spec is not equivalent to a
-        # missing input (output) spec.
-        recursive_cleanup(dxapp_json['runSpec'])
-        recursive_cleanup(dxapp_json['access'])
-        for key in ['name', 'title', 'summary', 'types', 'tags', 'properties', 'runSpec', 'access', 'details']:
-            if not dxapp_json[key]:
-                del dxapp_json[key]
-
-        readme = info.get("description", "")
-        devnotes = info.get("developerNotes", "")
-
-        # Write dxapp.json, Readme.md, and Readme.developer.md
-        with open("dxapp.json", "w") as f:
-            f.write(json.dumps(dxapp_json, sort_keys=False, indent=2, separators=(',', ': ')))
-            f.write('\n')
-        if readme:
-            with open("Readme.md", "w") as f:
-                f.write(readme)
-        if devnotes:
-            with open("Readme.developer.md", "w") as f:
-                f.write(devnotes)
-    finally:
-        os.chdir(old_cwd)
-
 def get(args):
     # Attempt to resolve name
     project, _folderpath, entity_result = try_call(resolve_existing_path,
                                                    args.path, expected='entity')
 
     if entity_result is None:
         parser.exit(3, fill('Could not resolve ' + args.path + ' to a data object') + '\n')
@@ -2039,14 +1927,15 @@
         try:
             details = dxpy.DXHTTPRequest('/' + entity_result['id'] + '/getDetails',
                                          {})
         except:
             err_exit()
         fd.write(json.dumps(details, indent=4))
     elif entity_result['describe']['class'] == 'applet':
+        from dxpy.utils.app_unbuilder import dump_applet
         dump_applet(dxpy.DXApplet(entity_result['id'], project=project), output_path)
     if fd is not None and args.output != '-':
         fd.close()
 
 def cat(args):
     for path in args.path:
         project, folderpath, entity_result = try_call(resolve_existing_path, path)
```

### Comparing `dxpy-v0.82.1/dxpy/scripts/dx_spans_to_bed.py` & `dxpy-v0.83.0/dxpy/scripts/dx_spans_to_bed.py`

 * *Files identical despite different names*

### Comparing `dxpy-v0.82.1/dxpy/scripts/dx_build_applet.py` & `dxpy-v0.83.0/dxpy/scripts/dx_build_applet.py`

 * *Files identical despite different names*

### Comparing `dxpy-v0.82.1/dxpy/scripts/dx_tsv_to_gtable.py` & `dxpy-v0.83.0/dxpy/scripts/dx_tsv_to_gtable.py`

 * *Files identical despite different names*

### Comparing `dxpy-v0.82.1/dxpy/scripts/dx_build_report_html.py` & `dxpy-v0.83.0/dxpy/scripts/dx_build_report_html.py`

 * *Files identical despite different names*

### Comparing `dxpy-v0.82.1/dxpy/scripts/__init__.py` & `dxpy-v0.83.0/dxpy/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `dxpy-v0.82.1/dxpy/packages/requests/certs.py` & `dxpy-v0.83.0/dxpy/packages/requests/certs.py`

 * *Files identical despite different names*

### Comparing `dxpy-v0.82.1/dxpy/packages/requests/hooks.py` & `dxpy-v0.83.0/dxpy/packages/requests/hooks.py`

 * *Files identical despite different names*

### Comparing `dxpy-v0.82.1/dxpy/packages/requests/status_codes.py` & `dxpy-v0.83.0/dxpy/packages/requests/status_codes.py`

 * *Files identical despite different names*

### Comparing `dxpy-v0.82.1/dxpy/packages/requests/api.py` & `dxpy-v0.83.0/dxpy/packages/requests/api.py`

 * *Files identical despite different names*

### Comparing `dxpy-v0.82.1/dxpy/packages/requests/sessions.py` & `dxpy-v0.83.0/dxpy/packages/requests/sessions.py`

 * *Files identical despite different names*

### Comparing `dxpy-v0.82.1/dxpy/packages/requests/packages/charade/mbcssm.py` & `dxpy-v0.83.0/dxpy/packages/requests/packages/charade/mbcssm.py`

 * *Files identical despite different names*

### Comparing `dxpy-v0.82.1/dxpy/packages/requests/packages/charade/big5freq.py` & `dxpy-v0.83.0/dxpy/packages/requests/packages/charade/big5freq.py`

 * *Files identical despite different names*

### Comparing `dxpy-v0.82.1/dxpy/packages/requests/packages/charade/latin1prober.py` & `dxpy-v0.83.0/dxpy/packages/requests/packages/charade/latin1prober.py`

 * *Files identical despite different names*

### Comparing `dxpy-v0.82.1/dxpy/packages/requests/packages/charade/sbcharsetprober.py` & `dxpy-v0.83.0/dxpy/packages/requests/packages/charade/sbcharsetprober.py`

 * *Files identical despite different names*

### Comparing `dxpy-v0.82.1/dxpy/packages/requests/packages/charade/euctwprober.py` & `dxpy-v0.83.0/dxpy/packages/requests/packages/charade/euctwprober.py`

 * *Files identical despite different names*

### Comparing `dxpy-v0.82.1/dxpy/packages/requests/packages/charade/codingstatemachine.py` & `dxpy-v0.83.0/dxpy/packages/requests/packages/charade/codingstatemachine.py`

 * *Files identical despite different names*

### Comparing `dxpy-v0.82.1/dxpy/packages/requests/packages/charade/mbcsgroupprober.py` & `dxpy-v0.83.0/dxpy/packages/requests/packages/charade/mbcsgroupprober.py`

 * *Files identical despite different names*

### Comparing `dxpy-v0.82.1/dxpy/packages/requests/packages/charade/jpcntx.py` & `dxpy-v0.83.0/dxpy/packages/requests/packages/charade/jpcntx.py`

 * *Files identical despite different names*

### Comparing `dxpy-v0.82.1/dxpy/packages/requests/packages/charade/mbcharsetprober.py` & `dxpy-v0.83.0/dxpy/packages/requests/packages/charade/mbcharsetprober.py`

 * *Files identical despite different names*

### Comparing `dxpy-v0.82.1/dxpy/packages/requests/packages/charade/langhungarianmodel.py` & `dxpy-v0.83.0/dxpy/packages/requests/packages/charade/langhungarianmodel.py`

 * *Files identical despite different names*

### Comparing `dxpy-v0.82.1/dxpy/packages/requests/packages/charade/escsm.py` & `dxpy-v0.83.0/dxpy/packages/requests/packages/charade/escsm.py`

 * *Files identical despite different names*

### Comparing `dxpy-v0.82.1/dxpy/packages/requests/packages/charade/escprober.py` & `dxpy-v0.83.0/dxpy/packages/requests/packages/charade/escprober.py`

 * *Files identical despite different names*

### Comparing `dxpy-v0.82.1/dxpy/packages/requests/packages/charade/hebrewprober.py` & `dxpy-v0.83.0/dxpy/packages/requests/packages/charade/hebrewprober.py`

 * *Files identical despite different names*

### Comparing `dxpy-v0.82.1/dxpy/packages/requests/packages/charade/jisfreq.py` & `dxpy-v0.83.0/dxpy/packages/requests/packages/charade/jisfreq.py`

 * *Files identical despite different names*

### Comparing `dxpy-v0.82.1/dxpy/packages/requests/packages/charade/universaldetector.py` & `dxpy-v0.83.0/dxpy/packages/requests/packages/charade/universaldetector.py`

 * *Files identical despite different names*

### Comparing `dxpy-v0.82.1/dxpy/packages/requests/packages/charade/langgreekmodel.py` & `dxpy-v0.83.0/dxpy/packages/requests/packages/charade/langgreekmodel.py`

 * *Files identical despite different names*

### Comparing `dxpy-v0.82.1/dxpy/packages/requests/packages/charade/euckrprober.py` & `dxpy-v0.83.0/dxpy/packages/requests/packages/charade/euckrprober.py`

 * *Files identical despite different names*

### Comparing `dxpy-v0.82.1/dxpy/packages/requests/packages/charade/sbcsgroupprober.py` & `dxpy-v0.83.0/dxpy/packages/requests/packages/charade/sbcsgroupprober.py`

 * *Files identical despite different names*

### Comparing `dxpy-v0.82.1/dxpy/packages/requests/packages/charade/gb2312prober.py` & `dxpy-v0.83.0/dxpy/packages/requests/packages/charade/gb2312prober.py`

 * *Files identical despite different names*

### Comparing `dxpy-v0.82.1/dxpy/packages/requests/packages/charade/langcyrillicmodel.py` & `dxpy-v0.83.0/dxpy/packages/requests/packages/charade/langcyrillicmodel.py`

 * *Files identical despite different names*

### Comparing `dxpy-v0.82.1/dxpy/packages/requests/packages/charade/euckrfreq.py` & `dxpy-v0.83.0/dxpy/packages/requests/packages/charade/euckrfreq.py`

 * *Files identical despite different names*

### Comparing `dxpy-v0.82.1/dxpy/packages/requests/packages/charade/eucjpprober.py` & `dxpy-v0.83.0/dxpy/packages/requests/packages/charade/eucjpprober.py`

 * *Files identical despite different names*

### Comparing `dxpy-v0.82.1/dxpy/packages/requests/packages/charade/langhebrewmodel.py` & `dxpy-v0.83.0/dxpy/packages/requests/packages/charade/langhebrewmodel.py`

 * *Files identical despite different names*

### Comparing `dxpy-v0.82.1/dxpy/packages/requests/packages/charade/compat.py` & `dxpy-v0.83.0/dxpy/packages/requests/packages/charade/compat.py`

 * *Files identical despite different names*

### Comparing `dxpy-v0.82.1/dxpy/packages/requests/packages/charade/charsetgroupprober.py` & `dxpy-v0.83.0/dxpy/packages/requests/packages/charade/charsetgroupprober.py`

 * *Files identical despite different names*

### Comparing `dxpy-v0.82.1/dxpy/packages/requests/packages/charade/cp949prober.py` & `dxpy-v0.83.0/dxpy/packages/requests/packages/charade/cp949prober.py`

 * *Files identical despite different names*

### Comparing `dxpy-v0.82.1/dxpy/packages/requests/packages/charade/utf8prober.py` & `dxpy-v0.83.0/dxpy/packages/requests/packages/charade/utf8prober.py`

 * *Files identical despite different names*

### Comparing `dxpy-v0.82.1/dxpy/packages/requests/packages/charade/langbulgarianmodel.py` & `dxpy-v0.83.0/dxpy/packages/requests/packages/charade/langbulgarianmodel.py`

 * *Files identical despite different names*

### Comparing `dxpy-v0.82.1/dxpy/packages/requests/packages/charade/constants.py` & `dxpy-v0.83.0/dxpy/packages/requests/packages/charade/constants.py`

 * *Files identical despite different names*

### Comparing `dxpy-v0.82.1/dxpy/packages/requests/packages/charade/chardistribution.py` & `dxpy-v0.83.0/dxpy/packages/requests/packages/charade/chardistribution.py`

 * *Files identical despite different names*

### Comparing `dxpy-v0.82.1/dxpy/packages/requests/packages/charade/euctwfreq.py` & `dxpy-v0.83.0/dxpy/packages/requests/packages/charade/euctwfreq.py`

 * *Files identical despite different names*

### Comparing `dxpy-v0.82.1/dxpy/packages/requests/packages/charade/gb2312freq.py` & `dxpy-v0.83.0/dxpy/packages/requests/packages/charade/gb2312freq.py`

 * *Files identical despite different names*

### Comparing `dxpy-v0.82.1/dxpy/packages/requests/packages/charade/big5prober.py` & `dxpy-v0.83.0/dxpy/packages/requests/packages/charade/big5prober.py`

 * *Files identical despite different names*

### Comparing `dxpy-v0.82.1/dxpy/packages/requests/packages/charade/sjisprober.py` & `dxpy-v0.83.0/dxpy/packages/requests/packages/charade/sjisprober.py`

 * *Files identical despite different names*

### Comparing `dxpy-v0.82.1/dxpy/packages/requests/packages/charade/langthaimodel.py` & `dxpy-v0.83.0/dxpy/packages/requests/packages/charade/langthaimodel.py`

 * *Files identical despite different names*

### Comparing `dxpy-v0.82.1/dxpy/packages/requests/packages/charade/charsetprober.py` & `dxpy-v0.83.0/dxpy/packages/requests/packages/charade/charsetprober.py`

 * *Files identical despite different names*

### Comparing `dxpy-v0.82.1/dxpy/packages/requests/packages/charade/__init__.py` & `dxpy-v0.83.0/dxpy/packages/requests/packages/charade/__init__.py`

 * *Files identical despite different names*

### Comparing `dxpy-v0.82.1/dxpy/packages/requests/packages/urllib3/request.py` & `dxpy-v0.83.0/dxpy/packages/requests/packages/urllib3/request.py`

 * *Files identical despite different names*

### Comparing `dxpy-v0.82.1/dxpy/packages/requests/packages/urllib3/connectionpool.py` & `dxpy-v0.83.0/dxpy/packages/requests/packages/urllib3/connectionpool.py`

 * *Files identical despite different names*

### Comparing `dxpy-v0.82.1/dxpy/packages/requests/packages/urllib3/poolmanager.py` & `dxpy-v0.83.0/dxpy/packages/requests/packages/urllib3/poolmanager.py`

 * *Files identical despite different names*

### Comparing `dxpy-v0.82.1/dxpy/packages/requests/packages/urllib3/_collections.py` & `dxpy-v0.83.0/dxpy/packages/requests/packages/urllib3/_collections.py`

 * *Files identical despite different names*

### Comparing `dxpy-v0.82.1/dxpy/packages/requests/packages/urllib3/packages/ordered_dict.py` & `dxpy-v0.83.0/dxpy/packages/requests/packages/urllib3/packages/ordered_dict.py`

 * *Files identical despite different names*

### Comparing `dxpy-v0.82.1/dxpy/packages/requests/packages/urllib3/packages/ssl_match_hostname/__init__.py` & `dxpy-v0.83.0/dxpy/packages/requests/packages/urllib3/packages/ssl_match_hostname/__init__.py`

 * *Files identical despite different names*

### Comparing `dxpy-v0.82.1/dxpy/packages/requests/packages/urllib3/packages/six.py` & `dxpy-v0.83.0/dxpy/packages/requests/packages/urllib3/packages/six.py`

 * *Files identical despite different names*

### Comparing `dxpy-v0.82.1/dxpy/packages/requests/packages/urllib3/util.py` & `dxpy-v0.83.0/dxpy/packages/requests/packages/urllib3/util.py`

 * *Files identical despite different names*

### Comparing `dxpy-v0.82.1/dxpy/packages/requests/packages/urllib3/filepost.py` & `dxpy-v0.83.0/dxpy/packages/requests/packages/urllib3/filepost.py`

 * *Files identical despite different names*

### Comparing `dxpy-v0.82.1/dxpy/packages/requests/packages/urllib3/contrib/ntlmpool.py` & `dxpy-v0.83.0/dxpy/packages/requests/packages/urllib3/contrib/ntlmpool.py`

 * *Files identical despite different names*

### Comparing `dxpy-v0.82.1/dxpy/packages/requests/packages/urllib3/contrib/pyopenssl.py` & `dxpy-v0.83.0/dxpy/packages/requests/packages/urllib3/contrib/pyopenssl.py`

 * *Files identical despite different names*

### Comparing `dxpy-v0.82.1/dxpy/packages/requests/packages/urllib3/exceptions.py` & `dxpy-v0.83.0/dxpy/packages/requests/packages/urllib3/exceptions.py`

 * *Files identical despite different names*

### Comparing `dxpy-v0.82.1/dxpy/packages/requests/packages/urllib3/response.py` & `dxpy-v0.83.0/dxpy/packages/requests/packages/urllib3/response.py`

 * *Files identical despite different names*

### Comparing `dxpy-v0.82.1/dxpy/packages/requests/packages/urllib3/__init__.py` & `dxpy-v0.83.0/dxpy/packages/requests/packages/urllib3/__init__.py`

 * *Files identical despite different names*

### Comparing `dxpy-v0.82.1/dxpy/packages/requests/cookies.py` & `dxpy-v0.83.0/dxpy/packages/requests/cookies.py`

 * *Files identical despite different names*

### Comparing `dxpy-v0.82.1/dxpy/packages/requests/structures.py` & `dxpy-v0.83.0/dxpy/packages/requests/structures.py`

 * *Files identical despite different names*

### Comparing `dxpy-v0.82.1/dxpy/packages/requests/models.py` & `dxpy-v0.83.0/dxpy/packages/requests/models.py`

 * *Files identical despite different names*

### Comparing `dxpy-v0.82.1/dxpy/packages/requests/compat.py` & `dxpy-v0.83.0/dxpy/packages/requests/compat.py`

 * *Files identical despite different names*

### Comparing `dxpy-v0.82.1/dxpy/packages/requests/cacert.pem` & `dxpy-v0.83.0/dxpy/packages/requests/cacert.pem`

 * *Files identical despite different names*

### Comparing `dxpy-v0.82.1/dxpy/packages/requests/adapters.py` & `dxpy-v0.83.0/dxpy/packages/requests/adapters.py`

 * *Files identical despite different names*

### Comparing `dxpy-v0.82.1/dxpy/packages/requests/auth.py` & `dxpy-v0.83.0/dxpy/packages/requests/auth.py`

 * *Files identical despite different names*

### Comparing `dxpy-v0.82.1/dxpy/packages/requests/exceptions.py` & `dxpy-v0.83.0/dxpy/packages/requests/exceptions.py`

 * *Files identical despite different names*

### Comparing `dxpy-v0.82.1/dxpy/packages/requests/utils.py` & `dxpy-v0.83.0/dxpy/packages/requests/utils.py`

 * *Files identical despite different names*

### Comparing `dxpy-v0.82.1/dxpy/packages/requests/__init__.py` & `dxpy-v0.83.0/dxpy/packages/requests/__init__.py`

 * *Files identical despite different names*

### Comparing `dxpy-v0.82.1/dxpy/utils/pretty_print.py` & `dxpy-v0.83.0/dxpy/utils/pretty_print.py`

 * *Files identical despite different names*

### Comparing `dxpy-v0.82.1/dxpy/utils/job_log_client.py` & `dxpy-v0.83.0/dxpy/utils/job_log_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,15 +81,15 @@
         else:
             self.seen_jobs[self.job_id] = dxpy.describe(self.job_id)
 
         if self.seen_jobs[self.job_id].get('state') in ['failed', 'terminated']:
             err_exit(code=3)
 
     def received_message(self, message):
-        message = json.loads(str(message))
+        message = json.loads(message.__unicode__())
 
         if self.print_job_info and 'job' in message and message['job'] not in self.seen_jobs:
             self.seen_jobs[message['job']] = dxpy.describe(message['job'])
             print(get_find_executions_string(self.seen_jobs[message['job']], has_children=False, show_outputs=False))
 
         if message.get('source') == 'SYSTEM' and message.get('msg') == 'END_LOG':
             self.close()
```

### Comparing `dxpy-v0.82.1/dxpy/utils/pathmatch.py` & `dxpy-v0.83.0/dxpy/utils/pathmatch.py`

 * *Files identical despite different names*

### Comparing `dxpy-v0.82.1/dxpy/utils/env.py` & `dxpy-v0.83.0/dxpy/utils/env.py`

 * *Files identical despite different names*

### Comparing `dxpy-v0.82.1/dxpy/utils/describe.py` & `dxpy-v0.83.0/dxpy/utils/describe.py`

 * *Files 0% similar despite different names*

```diff
@@ -440,15 +440,15 @@
             print_json_field(field, desc[field])
 
 def get_col_str(col_desc):
     return col_desc['name'] + DELIMITER(" (") + col_desc['type'] + DELIMITER(")")
 
 def print_data_obj_desc(desc, verbose=False):
     recognized_fields = ['id', 'class', 'project', 'folder', 'name', 'properties', 'tags', 'types', 'hidden', 'details', 'links', 'created', 'modified', 'state', 'title', 'subtitle', 'description', 'inputSpec', 'outputSpec', 'runSpec', 'summary', 'dxapi', 'access', 'createdBy', 'summary', 'sponsored', 'developerNotes',
-                         'stages', 'latestAnalysis', 'editVersion', 'outputFolder']
+                         'stages', 'latestAnalysis', 'editVersion', 'outputFolder', 'initializedFrom']
 
     def get_advanced_inputs():
         details = desc.get("details")
         if not verbose and isinstance(details, dict):
             return details.get("advancedInputs", [])
         return []
 
@@ -510,14 +510,16 @@
         if "execDepends" in desc["runSpec"]:
             print_list_field("execDepends", render_execdepends(desc["runSpec"]["execDepends"]))
         if "systemRequirements" in desc['runSpec']:
             print_json_field('Sys Requirements', desc['runSpec']['systemRequirements'])
     if 'stages' in desc:
         for i, stage in enumerate(desc["stages"]):
             render_stage("Stage " + str(i), stage)
+    if 'initializedFrom' in desc:
+        print_field("initializedFrom", desc["initializedFrom"]["id"])
     if 'latestAnalysis' in desc and desc['latestAnalysis'] is not None:
         print_field("Last execution", desc["latestAnalysis"]["id"])
         print_field("  run at", render_timestamp(desc["latestAnalysis"]["created"]))
         print_field("  state", JOB_STATES(desc["latestAnalysis"]["state"]))
 
     for field in desc:
         if field in recognized_fields:
```

### Comparing `dxpy-v0.82.1/dxpy/utils/printing.py` & `dxpy-v0.83.0/dxpy/utils/printing.py`

 * *Files identical despite different names*

### Comparing `dxpy-v0.82.1/dxpy/utils/exec_utils.py` & `dxpy-v0.83.0/dxpy/utils/exec_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,49 +19,56 @@
 '''
 
 from __future__ import print_function
 
 import os, sys, json, collections, logging, argparse, string
 from functools import wraps
 import dxpy
+from ..compat import is_py2
 
 ENTRY_POINT_TABLE = {}
 
 RUN_COUNT = 0
 
 # Locale-independent version of string.printable
 ASCII_PRINTABLE = string.ascii_letters + string.digits + string.punctuation + string.whitespace
 def _safe_unicode(o):
     """
     Returns an equivalent unicode object, trying harder to avoid
     dependencies on the Python default encoding.
     """
     def clean(s):
         return u''.join([c if c in ASCII_PRINTABLE else '?' for c in s])
-    try:
-        return unicode(o)
-    except:
+    if is_py2:
         try:
-            s = str(o)
+            return unicode(o)
+        except:
             try:
-                return s.decode("utf-8")
+                s = str(o)
+                try:
+                    return s.decode("utf-8")
+                except:
+                    return clean(s[:2048]) + u" [Raw error message: " + unicode(s.encode("hex"), 'utf-8') + u"]"
             except:
-                return clean(s[:2048]) + u" [Raw error message: " + unicode(s.encode("hex"), 'utf-8') + u"]"
-        except:
-            return u"(Unable to decode Python exception message)"
+                return u"(Unable to decode Python exception message)"
+    else:
+        return str(o)
 
 def _format_exception_message(e):
     """
     Formats the specified exception.
     """
     # Prevent duplication of "AppError" in places that print "AppError"
     # and then this formatted string
     if isinstance(e, dxpy.AppError):
         return _safe_unicode(e)
-    return unicode(e.__class__.__name__, 'utf-8') + ": " + _safe_unicode(e)
+    if is_py2:
+        return unicode(e.__class__.__name__, 'utf-8') + ": " + _safe_unicode(e)
+    else:
+        return e.__class__.__name__ + ": " + _safe_unicode(e)
 
 def run(function_name=None, function_input=None):
     '''
     Triggers the execution environment entry point processor.
 
     Use this function in the program entry point code:
```

### Comparing `dxpy-v0.82.1/dxpy/utils/local_exec_utils.py` & `dxpy-v0.83.0/dxpy/utils/local_exec_utils.py`

 * *Files identical despite different names*

### Comparing `dxpy-v0.82.1/dxpy/utils/resolver.py` & `dxpy-v0.83.0/dxpy/utils/resolver.py`

 * *Files identical despite different names*

### Comparing `dxpy-v0.82.1/dxpy/utils/completer.py` & `dxpy-v0.83.0/dxpy/utils/completer.py`

 * *Files identical despite different names*

### Comparing `dxpy-v0.82.1/dxpy/utils/__init__.py` & `dxpy-v0.83.0/dxpy/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `dxpy-v0.82.1/dxpy/templating/python.py` & `dxpy-v0.83.0/dxpy/templating/python.py`

 * *Files identical despite different names*

### Comparing `dxpy-v0.82.1/dxpy/templating/bash.py` & `dxpy-v0.83.0/dxpy/templating/bash.py`

 * *Files identical despite different names*

### Comparing `dxpy-v0.82.1/dxpy/templating/cpp.py` & `dxpy-v0.83.0/dxpy/templating/cpp.py`

 * *Files identical despite different names*

### Comparing `dxpy-v0.82.1/dxpy/templating/utils.py` & `dxpy-v0.83.0/dxpy/templating/utils.py`

 * *Files identical despite different names*

### Comparing `dxpy-v0.82.1/dxpy/templating/__init__.py` & `dxpy-v0.83.0/dxpy/templating/__init__.py`

 * *Files identical despite different names*

### Comparing `dxpy-v0.82.1/dxpy/exceptions.py` & `dxpy-v0.83.0/dxpy/exceptions.py`

 * *Files identical despite different names*

### Comparing `dxpy-v0.82.1/dxpy/cli/parsers.py` & `dxpy-v0.83.0/dxpy/cli/parsers.py`

 * *Files identical despite different names*

### Comparing `dxpy-v0.82.1/dxpy/cli/exec_io.py` & `dxpy-v0.83.0/dxpy/cli/exec_io.py`

 * *Files identical despite different names*

### Comparing `dxpy-v0.82.1/dxpy/cli/workflow.py` & `dxpy-v0.83.0/dxpy/cli/workflow.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,30 +24,30 @@
 import os, sys
 
 import dxpy
 import dxpy.utils.printing as printing
 from .parsers import (process_dataobject_args, process_single_dataobject_output_args,
                       process_instance_type_arg)
 from ..utils.describe import io_val_to_str
-from ..utils.resolver import (resolve_existing_path, resolve_path)
+from ..utils.resolver import (resolve_existing_path, resolve_path, is_analysis_id)
 from ..exceptions import (err_exit, DXCLIError)
 from . import try_call
 
 def new_workflow(args):
     try_call(process_dataobject_args, args)
     try_call(process_single_dataobject_output_args, args)
     init_from = None
     if args.init is not None:
-        try:
+        if is_analysis_id(args.init):
+            init_from = args.init
+        else:
             init_project, init_folder, init_result = try_call(resolve_existing_path,
                                                               args.init,
                                                               expected='entity')
             init_from = dxpy.get_handler(init_result['id'], project=init_project)
-        except:
-            init_from = args.init
     if args.output is None:
         project = dxpy.WORKSPACE_ID
         folder = os.environ.get('DX_CLI_WD', '/')
         name = None
     else:
         project, folder, name = dxpy.utils.resolver.resolve_path(args.output)
     if args.output_folder is not None:
@@ -131,23 +131,23 @@
 def list_stages(args):
     # get workflow
     workflow_id, project = get_workflow_id_and_project(args.workflow)
 
     dxworkflow = dxpy.DXWorkflow(workflow_id, project=project)
     desc = dxworkflow.describe()
     print((printing.BOLD() + printing.GREEN() + '{name}' + printing.ENDC() + ' ({id})').format(**desc))
-    print
+    print()
     print('Title: ' + desc['title'])
     print('Output Folder: ' + (desc.get('outputFolder') if desc.get('outputFolder') is not None else '-'))
     if len(desc['stages']) == 0:
-        print
+        print()
         print(' No stages; add stages with the command "dx add stage"')
     for i, stage in enumerate(desc['stages']):
         stage['i'] = i
-        print
+        print()
         if stage['name'] is None:
             stage['name'] = '<no name>'
         print((printing.UNDERLINE() + 'Stage {i}' + printing.ENDC() + ': {name} ({id})').format(**stage))
         print('Executable      {executable}'.format(**stage) + \
             (" (" + printing.RED() + "inaccessible" + printing.ENDC() + ")" \
              if stage.get('accessible') is False else ""))
         if stage['folder'] is not None and stage['folder'].startswith('/'):
```

### Comparing `dxpy-v0.82.1/dxpy/cli/__init__.py` & `dxpy-v0.83.0/dxpy/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `dxpy-v0.82.1/dxpy/__init__.py` & `dxpy-v0.83.0/dxpy/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -167,15 +167,15 @@
 
 APISERVER_PROTOCOL = DEFAULT_APISERVER_PROTOCOL
 APISERVER_HOST = DEFAULT_APISERVER_HOST
 APISERVER_PORT = DEFAULT_APISERVER_PORT
 
 SESSION_HANDLERS = collections.defaultdict(requests.session)
 
-DEFAULT_RETRIES = 5
+DEFAULT_RETRIES = 6
 _DEBUG, _UPGRADE_NOTIFY = False, True
 
 USER_AGENT = "{name}/{version} ({platform})".format(name=__name__,
                                                     version=TOOLKIT_VERSION,
                                                     platform=platform.platform())
 
 http_server_errors = set([requests.codes.server_error,
@@ -369,15 +369,15 @@
                     ok_to_retry = always_retry or (method == 'GET')
                 else:
                     ok_to_retry = (response.status_code >= 500 and response.status_code < 600) or streaming_response_truncated
 
                 if ok_to_retry:
                     if rewind_input_buffer_offset is not None:
                         data.seek(rewind_input_buffer_offset)
-                    delay = 2 ** (retry+1)
+                    delay = 2 ** retry
                     logger.warn("%s %s: %s. Waiting %d seconds before retry %d of %d..." % (method, url, str(e), delay,
                                                                                             retry+1, max_retries))
                     time.sleep(delay)
                     continue
             break
         if last_error is None:
             last_error = exceptions.DXError("Internal error in DXHTTPRequest")
```

### Comparing `dxpy-v0.82.1/scripts/dx-jobutil-add-output` & `dxpy-v0.83.0/scripts/dx-jobutil-add-output`

 * *Files identical despite different names*

### Comparing `dxpy-v0.82.1/scripts/dx-fetch-bundled-depends` & `dxpy-v0.83.0/scripts/dx-fetch-bundled-depends`

 * *Files identical despite different names*

### Comparing `dxpy-v0.82.1/scripts/dx-jobutil-report-error` & `dxpy-v0.83.0/scripts/dx-jobutil-report-error`

 * *Files identical despite different names*

### Comparing `dxpy-v0.82.1/scripts/dx-app-wizard` & `dxpy-v0.83.0/scripts/dx-app-wizard`

 * *Files identical despite different names*

### Comparing `dxpy-v0.82.1/scripts/dx-jobutil-dxlink` & `dxpy-v0.83.0/scripts/dx-jobutil-dxlink`

 * *Files identical despite different names*

### Comparing `dxpy-v0.82.1/scripts/dx-jobutil-parse-link` & `dxpy-v0.83.0/scripts/dx-jobutil-parse-link`

 * *Files identical despite different names*

### Comparing `dxpy-v0.82.1/scripts/dx-log-stream` & `dxpy-v0.83.0/scripts/dx-log-stream`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 #   License for the specific language governing permissions and limitations
 #   under the License.
 
 '''
 Redirects stdin to a DNAnexus log socket in the execution environment.
 '''
 
-import os, sys, logging, argparse
+import sys, logging, argparse
 import dxpy
 
 logging.basicConfig(level=logging.DEBUG, format="%(message)s")
 
 parser = argparse.ArgumentParser(description=__doc__)
 parser.add_argument("-l", "--level", help="Logging level to use", default='info')
 parser.add_argument("-s", "--source", help="Source ID to use", default='DX_APP_STREAM',
```

### Comparing `dxpy-v0.82.1/scripts/dx-mount` & `dxpy-v0.83.0/scripts/dx-mount`

 * *Files identical despite different names*

### Comparing `dxpy-v0.82.1/scripts/dx-run-app-locally` & `dxpy-v0.83.0/scripts/dx-run-app-locally`

 * *Files identical despite different names*

### Comparing `dxpy-v0.82.1/scripts/dx-workflow-to-applet` & `dxpy-v0.83.0/scripts/dx-workflow-to-applet`

 * *Files identical despite different names*

### Comparing `dxpy-v0.82.1/scripts/dx-jobutil-new-job` & `dxpy-v0.83.0/scripts/dx-jobutil-new-job`

 * *Files identical despite different names*

### Comparing `dxpy-v0.82.1/PKG-INFO` & `dxpy-v0.83.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: dxpy
-Version: v0.82.1
+Version: v0.83.0
 Summary: DNAnexus Platform API bindings for Python
 Home-page: https://github.com/dnanexus/dx-toolkit
 Author: Katherine Lai, Phil Sung, Andrey Kislyuk, Anurag Biyani
 Author-email: expert-dev@dnanexus.com
 License: Apache Software License
 Description: UNKNOWN
 Platform: UNKNOWN
```

