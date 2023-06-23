# Comparing `tmp/jcvi-1.3.5.tar.gz` & `tmp/jcvi-1.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jcvi-1.3.5.tar", last modified: Sat May 20 02:09:56 2023, max compression
+gzip compressed data, was "jcvi-1.3.6.tar", last modified: Fri Jun 23 16:27:06 2023, max compression
```

## Comparing `jcvi-1.3.5.tar` & `jcvi-1.3.6.tar`

### file list

```diff
@@ -1,215 +1,215 @@
-drwxr-xr-x   0 bao        (501) staff       (20)        0 2023-05-20 02:09:56.444485 jcvi-1.3.5/
--rw-r--r--   0 bao        (501) staff       (20)     1292 2020-03-03 07:11:04.000000 jcvi-1.3.5/LICENSE
--rw-r--r--   0 bao        (501) staff       (20)       91 2022-11-27 15:24:30.000000 jcvi-1.3.5/MANIFEST.in
--rw-r--r--   0 bao        (501) staff       (20)     8759 2023-05-20 02:09:56.444574 jcvi-1.3.5/PKG-INFO
--rw-r--r--   0 bao        (501) staff       (20)     8094 2021-04-18 23:59:49.000000 jcvi-1.3.5/README.md
-drwxr-xr-x   0 bao        (501) staff       (20)        0 2023-05-20 02:09:56.406541 jcvi-1.3.5/jcvi/
--rw-r--r--   0 bao        (501) staff       (20)      770 2022-11-26 21:23:29.000000 jcvi-1.3.5/jcvi/__init__.py
-drwxr-xr-x   0 bao        (501) staff       (20)        0 2023-05-20 02:09:56.411054 jcvi-1.3.5/jcvi/algorithms/
--rw-r--r--   0 bao        (501) staff       (20)        0 2020-01-29 05:28:41.000000 jcvi-1.3.5/jcvi/algorithms/__init__.py
--rw-r--r--   0 bao        (501) staff       (20)      263 2021-06-19 08:23:09.000000 jcvi-1.3.5/jcvi/algorithms/__main__.py
--rw-r--r--   0 bao        (501) staff       (20)     6422 2021-06-19 08:23:09.000000 jcvi-1.3.5/jcvi/algorithms/ec.py
--rw-r--r--   0 bao        (501) staff       (20)     5678 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/algorithms/formula.py
--rw-r--r--   0 bao        (501) staff       (20)    14132 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/algorithms/graph.py
--rwxr-xr-x   0 bao        (501) staff       (20)     6275 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/algorithms/lis.py
--rwxr-xr-x   0 bao        (501) staff       (20)    24228 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/algorithms/lpsolve.py
--rw-r--r--   0 bao        (501) staff       (20)     6104 2021-06-19 08:23:09.000000 jcvi-1.3.5/jcvi/algorithms/matrix.py
--rw-r--r--   0 bao        (501) staff       (20)     1296 2021-06-19 19:45:56.000000 jcvi-1.3.5/jcvi/algorithms/maxsum.py
--rw-r--r--   0 bao        (501) staff       (20)     1203 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/algorithms/ml.py
--rwxr-xr-x   0 bao        (501) staff       (20)     4999 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/algorithms/supermap.py
--rw-r--r--   0 bao        (501) staff       (20)    12559 2022-11-26 15:55:17.000000 jcvi-1.3.5/jcvi/algorithms/tsp.py
-drwxr-xr-x   0 bao        (501) staff       (20)        0 2023-05-20 02:09:56.415895 jcvi-1.3.5/jcvi/annotation/
--rw-r--r--   0 bao        (501) staff       (20)        0 2020-01-29 05:28:41.000000 jcvi-1.3.5/jcvi/annotation/__init__.py
--rw-r--r--   0 bao        (501) staff       (20)      261 2021-06-19 08:23:09.000000 jcvi-1.3.5/jcvi/annotation/__main__.py
--rw-r--r--   0 bao        (501) staff       (20)    21414 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/annotation/ahrd.py
--rw-r--r--   0 bao        (501) staff       (20)     7899 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/annotation/automaton.py
--rwxr-xr-x   0 bao        (501) staff       (20)     6417 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/annotation/depth.py
--rw-r--r--   0 bao        (501) staff       (20)     7042 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/annotation/evm.py
--rw-r--r--   0 bao        (501) staff       (20)    14687 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/annotation/maker.py
--rw-r--r--   0 bao        (501) staff       (20)    19485 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/annotation/pasa.py
--rw-r--r--   0 bao        (501) staff       (20)    12822 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/annotation/qc.py
--rw-r--r--   0 bao        (501) staff       (20)    42839 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/annotation/reformat.py
--rw-r--r--   0 bao        (501) staff       (20)    12645 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/annotation/stats.py
--rw-r--r--   0 bao        (501) staff       (20)     6793 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/annotation/train.py
-drwxr-xr-x   0 bao        (501) staff       (20)        0 2023-05-20 02:09:56.420105 jcvi-1.3.5/jcvi/apps/
--rw-r--r--   0 bao        (501) staff       (20)        0 2020-01-29 05:28:41.000000 jcvi-1.3.5/jcvi/apps/__init__.py
--rw-r--r--   0 bao        (501) staff       (20)      258 2021-06-19 08:23:09.000000 jcvi-1.3.5/jcvi/apps/__main__.py
--rw-r--r--   0 bao        (501) staff       (20)    16889 2023-02-19 15:03:46.000000 jcvi-1.3.5/jcvi/apps/align.py
--rw-r--r--   0 bao        (501) staff       (20)    67790 2023-05-20 01:38:16.000000 jcvi-1.3.5/jcvi/apps/base.py
--rw-r--r--   0 bao        (501) staff       (20)    12271 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/apps/biomart.py
--rwxr-xr-x   0 bao        (501) staff       (20)     3554 2021-06-19 19:45:56.000000 jcvi-1.3.5/jcvi/apps/blastplus.py
--rw-r--r--   0 bao        (501) staff       (20)     5219 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/apps/bowtie.py
--rw-r--r--   0 bao        (501) staff       (20)     7695 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/apps/bwa.py
--rw-r--r--   0 bao        (501) staff       (20)     7279 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/apps/cdhit.py
--rw-r--r--   0 bao        (501) staff       (20)     2623 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/apps/emboss.py
--rw-r--r--   0 bao        (501) staff       (20)    21332 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/apps/fetch.py
--rw-r--r--   0 bao        (501) staff       (20)    19459 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/apps/gbsubmit.py
--rw-r--r--   0 bao        (501) staff       (20)     6892 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/apps/gmap.py
--rw-r--r--   0 bao        (501) staff       (20)    18476 2023-04-29 14:56:25.000000 jcvi-1.3.5/jcvi/apps/grid.py
--rw-r--r--   0 bao        (501) staff       (20)    33945 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/apps/ks.py
--rwxr-xr-x   0 bao        (501) staff       (20)     7238 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/apps/lastz.py
--rwxr-xr-x   0 bao        (501) staff       (20)     3004 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/apps/mask.py
--rw-r--r--   0 bao        (501) staff       (20)    35471 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/apps/phylo.py
--rw-r--r--   0 bao        (501) staff       (20)     1896 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/apps/r.py
--rw-r--r--   0 bao        (501) staff       (20)     4901 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/apps/restriction.py
--rw-r--r--   0 bao        (501) staff       (20)     2116 2021-06-19 08:23:09.000000 jcvi-1.3.5/jcvi/apps/script.py
--rw-r--r--   0 bao        (501) staff       (20)     3784 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/apps/softlink.py
--rw-r--r--   0 bao        (501) staff       (20)    33065 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/apps/uclust.py
--rw-r--r--   0 bao        (501) staff       (20)     5208 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/apps/uniprot.py
--rw-r--r--   0 bao        (501) staff       (20)     3661 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/apps/vecscreen.py
-drwxr-xr-x   0 bao        (501) staff       (20)        0 2023-05-20 02:09:56.423678 jcvi-1.3.5/jcvi/assembly/
--rw-r--r--   0 bao        (501) staff       (20)        0 2020-01-29 05:28:41.000000 jcvi-1.3.5/jcvi/assembly/__init__.py
--rw-r--r--   0 bao        (501) staff       (20)      257 2021-06-19 08:23:09.000000 jcvi-1.3.5/jcvi/assembly/__main__.py
--rw-r--r--   0 bao        (501) staff       (20)    66136 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/assembly/allmaps.py
--rw-r--r--   0 bao        (501) staff       (20)    15451 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/assembly/allpaths.py
--rw-r--r--   0 bao        (501) staff       (20)    13265 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/assembly/automaton.py
--rw-r--r--   0 bao        (501) staff       (20)     5544 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/assembly/base.py
--rw-r--r--   0 bao        (501) staff       (20)    34986 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/assembly/ca.py
--rw-r--r--   0 bao        (501) staff       (20)     3457 2022-09-27 05:18:33.000000 jcvi-1.3.5/jcvi/assembly/chic.pyx
--rw-r--r--   0 bao        (501) staff       (20)     4581 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/assembly/coverage.py
--rw-r--r--   0 bao        (501) staff       (20)     8676 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/assembly/gaps.py
--rw-r--r--   0 bao        (501) staff       (20)    20212 2023-02-19 15:03:46.000000 jcvi-1.3.5/jcvi/assembly/geneticmap.py
--rw-r--r--   0 bao        (501) staff       (20)    34693 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/assembly/goldenpath.py
--rw-r--r--   0 bao        (501) staff       (20)    57613 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/assembly/hic.py
--rw-r--r--   0 bao        (501) staff       (20)    43632 2023-05-05 09:23:28.000000 jcvi-1.3.5/jcvi/assembly/kmer.py
--rw-r--r--   0 bao        (501) staff       (20)    12519 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/assembly/opticalmap.py
--rw-r--r--   0 bao        (501) staff       (20)    27279 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/assembly/patch.py
--rw-r--r--   0 bao        (501) staff       (20)    15741 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/assembly/postprocess.py
--rw-r--r--   0 bao        (501) staff       (20)    23470 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/assembly/preprocess.py
--rw-r--r--   0 bao        (501) staff       (20)     6287 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/assembly/sim.py
--rw-r--r--   0 bao        (501) staff       (20)     8830 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/assembly/soap.py
--rw-r--r--   0 bao        (501) staff       (20)    16183 2023-04-26 05:51:28.000000 jcvi-1.3.5/jcvi/assembly/syntenypath.py
--rw-r--r--   0 bao        (501) staff       (20)     5042 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/assembly/trinity.py
-drwxr-xr-x   0 bao        (501) staff       (20)        0 2023-05-20 02:09:56.425737 jcvi-1.3.5/jcvi/compara/
--rw-r--r--   0 bao        (501) staff       (20)        0 2020-01-29 05:28:41.000000 jcvi-1.3.5/jcvi/compara/__init__.py
--rw-r--r--   0 bao        (501) staff       (20)      251 2021-06-19 08:23:09.000000 jcvi-1.3.5/jcvi/compara/__main__.py
--rw-r--r--   0 bao        (501) staff       (20)     4210 2023-04-26 05:51:28.000000 jcvi-1.3.5/jcvi/compara/base.py
--rwxr-xr-x   0 bao        (501) staff       (20)     9796 2023-04-26 05:51:28.000000 jcvi-1.3.5/jcvi/compara/blastfilter.py
--rw-r--r--   0 bao        (501) staff       (20)    27460 2023-05-20 02:09:12.000000 jcvi-1.3.5/jcvi/compara/catalog.py
--rw-r--r--   0 bao        (501) staff       (20)    26355 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/compara/fractionation.py
--rw-r--r--   0 bao        (501) staff       (20)     9216 2023-04-26 05:51:28.000000 jcvi-1.3.5/jcvi/compara/pad.py
--rw-r--r--   0 bao        (501) staff       (20)     3051 2021-06-19 08:23:09.000000 jcvi-1.3.5/jcvi/compara/phylogeny.py
--rwxr-xr-x   0 bao        (501) staff       (20)     7948 2023-04-26 05:51:28.000000 jcvi-1.3.5/jcvi/compara/quota.py
--rw-r--r--   0 bao        (501) staff       (20)    10341 2023-04-26 05:51:28.000000 jcvi-1.3.5/jcvi/compara/reconstruct.py
--rwxr-xr-x   0 bao        (501) staff       (20)     9233 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/compara/synfind.py
--rwxr-xr-x   0 bao        (501) staff       (20)    57574 2023-04-26 05:51:28.000000 jcvi-1.3.5/jcvi/compara/synteny.py
-drwxr-xr-x   0 bao        (501) staff       (20)        0 2023-05-20 02:09:56.430616 jcvi-1.3.5/jcvi/formats/
--rw-r--r--   0 bao        (501) staff       (20)        0 2020-01-29 05:28:41.000000 jcvi-1.3.5/jcvi/formats/__init__.py
--rw-r--r--   0 bao        (501) staff       (20)      262 2021-06-19 08:23:09.000000 jcvi-1.3.5/jcvi/formats/__main__.py
--rw-r--r--   0 bao        (501) staff       (20)    63612 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/formats/agp.py
--rw-r--r--   0 bao        (501) staff       (20)    33966 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/formats/base.py
--rwxr-xr-x   0 bao        (501) staff       (20)    72552 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/formats/bed.py
--rw-r--r--   0 bao        (501) staff       (20)    42967 2023-05-20 02:09:12.000000 jcvi-1.3.5/jcvi/formats/blast.py
--rw-r--r--   0 bao        (501) staff       (20)     7010 2022-09-27 05:18:33.000000 jcvi-1.3.5/jcvi/formats/cblast.pyx
--rw-r--r--   0 bao        (501) staff       (20)     3193 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/formats/cdt.py
--rw-r--r--   0 bao        (501) staff       (20)     8612 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/formats/chain.py
--rw-r--r--   0 bao        (501) staff       (20)     4644 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/formats/contig.py
--rw-r--r--   0 bao        (501) staff       (20)    15170 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/formats/coords.py
--rw-r--r--   0 bao        (501) staff       (20)     6529 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/formats/excel.py
--rw-r--r--   0 bao        (501) staff       (20)    75590 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/formats/fasta.py
--rw-r--r--   0 bao        (501) staff       (20)    29575 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/formats/fastq.py
--rw-r--r--   0 bao        (501) staff       (20)    15549 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/formats/genbank.py
--rw-r--r--   0 bao        (501) staff       (20)   118976 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/formats/gff.py
--rw-r--r--   0 bao        (501) staff       (20)     3979 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/formats/html.py
--rw-r--r--   0 bao        (501) staff       (20)     4612 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/formats/maf.py
--rwxr-xr-x   0 bao        (501) staff       (20)     2842 2021-07-05 22:45:00.000000 jcvi-1.3.5/jcvi/formats/obo.py
--rw-r--r--   0 bao        (501) staff       (20)     2900 2021-01-11 06:59:36.000000 jcvi-1.3.5/jcvi/formats/paf.py
--rw-r--r--   0 bao        (501) staff       (20)     2785 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/formats/pdf.py
--rwxr-xr-x   0 bao        (501) staff       (20)    10355 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/formats/psl.py
--rw-r--r--   0 bao        (501) staff       (20)     2746 2021-06-19 08:23:09.000000 jcvi-1.3.5/jcvi/formats/pyblast.py
--rw-r--r--   0 bao        (501) staff       (20)    28231 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/formats/sam.py
--rw-r--r--   0 bao        (501) staff       (20)     8041 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/formats/sizes.py
--rw-r--r--   0 bao        (501) staff       (20)    25480 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/formats/vcf.py
-drwxr-xr-x   0 bao        (501) staff       (20)        0 2023-05-20 02:09:56.435114 jcvi-1.3.5/jcvi/graphics/
--rw-r--r--   0 bao        (501) staff       (20)        0 2020-01-29 05:28:41.000000 jcvi-1.3.5/jcvi/graphics/__init__.py
--rw-r--r--   0 bao        (501) staff       (20)      271 2021-06-19 08:23:09.000000 jcvi-1.3.5/jcvi/graphics/__main__.py
--rw-r--r--   0 bao        (501) staff       (20)    16271 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/graphics/align.py
--rw-r--r--   0 bao        (501) staff       (20)    15265 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/graphics/assembly.py
--rw-r--r--   0 bao        (501) staff       (20)    22166 2023-02-23 05:35:25.000000 jcvi-1.3.5/jcvi/graphics/base.py
--rwxr-xr-x   0 bao        (501) staff       (20)    10006 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/graphics/blastplot.py
--rw-r--r--   0 bao        (501) staff       (20)    22427 2023-02-06 05:16:46.000000 jcvi-1.3.5/jcvi/graphics/chromosome.py
--rw-r--r--   0 bao        (501) staff       (20)     7145 2021-06-19 08:23:09.000000 jcvi-1.3.5/jcvi/graphics/coverage.py
--rwxr-xr-x   0 bao        (501) staff       (20)    14873 2023-04-26 05:51:28.000000 jcvi-1.3.5/jcvi/graphics/dotplot.py
--rw-r--r--   0 bao        (501) staff       (20)    21810 2023-02-06 05:16:46.000000 jcvi-1.3.5/jcvi/graphics/glyph.py
--rw-r--r--   0 bao        (501) staff       (20)    23626 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/graphics/grabseeds.py
--rwxr-xr-x   0 bao        (501) staff       (20)     2379 2021-06-19 08:23:09.000000 jcvi-1.3.5/jcvi/graphics/graph.py
--rw-r--r--   0 bao        (501) staff       (20)     5025 2021-03-26 15:38:36.000000 jcvi-1.3.5/jcvi/graphics/heatmap.py
--rw-r--r--   0 bao        (501) staff       (20)     9612 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/graphics/histogram.py
--rw-r--r--   0 bao        (501) staff       (20)    13375 2023-02-08 03:44:09.000000 jcvi-1.3.5/jcvi/graphics/karyotype.py
--rw-r--r--   0 bao        (501) staff       (20)    31416 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/graphics/landscape.py
--rw-r--r--   0 bao        (501) staff       (20)     1276 2021-06-19 08:23:09.000000 jcvi-1.3.5/jcvi/graphics/logo.py
--rw-r--r--   0 bao        (501) staff       (20)     3893 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/graphics/mummerplot.py
--rw-r--r--   0 bao        (501) staff       (20)    20888 2023-02-08 03:44:09.000000 jcvi-1.3.5/jcvi/graphics/synteny.py
--rw-r--r--   0 bao        (501) staff       (20)     5488 2021-06-19 19:45:56.000000 jcvi-1.3.5/jcvi/graphics/table.py
--rw-r--r--   0 bao        (501) staff       (20)    20377 2022-11-26 16:06:34.000000 jcvi-1.3.5/jcvi/graphics/tree.py
--rw-r--r--   0 bao        (501) staff       (20)     6194 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/graphics/wheel.py
--rw-r--r--   0 bao        (501) staff       (20)     1675 2021-03-26 15:38:36.000000 jcvi-1.3.5/jcvi/graphics/whisker.py
-drwxr-xr-x   0 bao        (501) staff       (20)        0 2023-05-20 02:09:56.437840 jcvi-1.3.5/jcvi/projects/
--rw-r--r--   0 bao        (501) staff       (20)        0 2020-01-29 05:28:41.000000 jcvi-1.3.5/jcvi/projects/__init__.py
--rw-r--r--   0 bao        (501) staff       (20)      260 2021-06-19 08:23:09.000000 jcvi-1.3.5/jcvi/projects/__main__.py
--rw-r--r--   0 bao        (501) staff       (20)    22445 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/projects/age.py
--rw-r--r--   0 bao        (501) staff       (20)     1571 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/projects/alfalfa.py
--rw-r--r--   0 bao        (501) staff       (20)    15907 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/projects/allmaps.py
--rw-r--r--   0 bao        (501) staff       (20)     6750 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/projects/bites.py
--rw-r--r--   0 bao        (501) staff       (20)     5679 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/projects/heterosis.py
--rw-r--r--   0 bao        (501) staff       (20)    14136 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/projects/ies.py
--rw-r--r--   0 bao        (501) staff       (20)    22201 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/projects/misc.py
--rw-r--r--   0 bao        (501) staff       (20)    25024 2023-02-06 05:16:46.000000 jcvi-1.3.5/jcvi/projects/napus.py
--rw-r--r--   0 bao        (501) staff       (20)    12754 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/projects/pineapple.py
--rw-r--r--   0 bao        (501) staff       (20)     2367 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/projects/pistachio.py
--rw-r--r--   0 bao        (501) staff       (20)    67857 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/projects/str.py
--rw-r--r--   0 bao        (501) staff       (20)    25768 2023-04-29 14:56:25.000000 jcvi-1.3.5/jcvi/projects/sugarcane.py
--rw-r--r--   0 bao        (501) staff       (20)    23950 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/projects/synfind.py
--rw-r--r--   0 bao        (501) staff       (20)    21554 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/projects/tgbs.py
--rw-r--r--   0 bao        (501) staff       (20)    11941 2023-04-26 05:51:28.000000 jcvi-1.3.5/jcvi/projects/vanilla.py
-drwxr-xr-x   0 bao        (501) staff       (20)        0 2023-05-20 02:09:56.440327 jcvi-1.3.5/jcvi/utils/
--rw-r--r--   0 bao        (501) staff       (20)        0 2020-01-29 05:28:41.000000 jcvi-1.3.5/jcvi/utils/__init__.py
--rw-r--r--   0 bao        (501) staff       (20)      260 2021-06-19 08:23:09.000000 jcvi-1.3.5/jcvi/utils/__main__.py
--rw-r--r--   0 bao        (501) staff       (20)    24200 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/utils/aws.py
--rw-r--r--   0 bao        (501) staff       (20)    12512 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/utils/cbook.py
--rw-r--r--   0 bao        (501) staff       (20)      355 2021-01-11 02:34:49.000000 jcvi-1.3.5/jcvi/utils/console.py
-drwxr-xr-x   0 bao        (501) staff       (20)        0 2023-05-20 02:09:56.442696 jcvi-1.3.5/jcvi/utils/data/
--rwxr-xr-x   0 bao        (501) staff       (20)    16912 2020-01-29 05:28:41.000000 jcvi-1.3.5/jcvi/utils/data/Airswing.ttf
--rwxr-xr-x   0 bao        (501) staff       (20)   103940 2020-01-29 05:28:41.000000 jcvi-1.3.5/jcvi/utils/data/Collegia.ttf
--rwxr-xr-x   0 bao        (501) staff       (20)    20468 2020-01-29 05:28:41.000000 jcvi-1.3.5/jcvi/utils/data/HookedUp.ttf
--rw-r--r--   0 bao        (501) staff       (20)    25832 2020-01-29 05:28:41.000000 jcvi-1.3.5/jcvi/utils/data/Humor-Sans.ttf
--rw-r--r--   0 bao        (501) staff       (20)    28065 2020-01-29 05:28:41.000000 jcvi-1.3.5/jcvi/utils/data/TREDs.meta.csv
--rw-r--r--   0 bao        (501) staff       (20)        0 2020-01-29 05:28:41.000000 jcvi-1.3.5/jcvi/utils/data/__init__.py
--rw-r--r--   0 bao        (501) staff       (20)      911 2020-01-29 05:28:41.000000 jcvi-1.3.5/jcvi/utils/data/adapters.fasta
--rw-r--r--   0 bao        (501) staff       (20)     3321 2020-01-29 05:28:41.000000 jcvi-1.3.5/jcvi/utils/data/blosum80.mat
--rw-r--r--   0 bao        (501) staff       (20)     7686 2020-01-29 05:28:41.000000 jcvi-1.3.5/jcvi/utils/data/chrY.hg38.unique_ccn.gc
--rw-r--r--   0 bao        (501) staff       (20)      282 2020-01-29 05:28:41.000000 jcvi-1.3.5/jcvi/utils/data/colorchecker.txt
--rw-r--r--   0 bao        (501) staff       (20)    45544 2020-01-29 05:28:41.000000 jcvi-1.3.5/jcvi/utils/data/hg38.band.txt
--rw-r--r--   0 bao        (501) staff       (20)    11672 2020-01-29 05:28:41.000000 jcvi-1.3.5/jcvi/utils/data/hg38.chrom.sizes
--rw-r--r--   0 bao        (501) staff       (20)     1000 2020-01-29 05:28:41.000000 jcvi-1.3.5/jcvi/utils/data/instance.json
--rw-r--r--   0 bao        (501) staff       (20)     9795 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/utils/db.py
--rw-r--r--   0 bao        (501) staff       (20)     4145 2021-01-09 20:22:53.000000 jcvi-1.3.5/jcvi/utils/ez_setup.py
--rwxr-xr-x   0 bao        (501) staff       (20)     2884 2021-06-19 08:23:09.000000 jcvi-1.3.5/jcvi/utils/grouper.py
--rw-r--r--   0 bao        (501) staff       (20)    10437 2021-06-19 08:23:09.000000 jcvi-1.3.5/jcvi/utils/orderedcollections.py
--rw-r--r--   0 bao        (501) staff       (20)    14595 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/utils/range.py
--rw-r--r--   0 bao        (501) staff       (20)     3946 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/utils/table.py
--rw-r--r--   0 bao        (501) staff       (20)     4687 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/utils/taxonomy.py
--rw-r--r--   0 bao        (501) staff       (20)     1522 2021-07-13 05:06:52.000000 jcvi-1.3.5/jcvi/utils/validator.py
--rwxr-xr-x   0 bao        (501) staff       (20)     1377 2021-01-15 14:44:37.000000 jcvi-1.3.5/jcvi/utils/webcolors.py
-drwxr-xr-x   0 bao        (501) staff       (20)        0 2023-05-20 02:09:56.444323 jcvi-1.3.5/jcvi/variation/
--rw-r--r--   0 bao        (501) staff       (20)        0 2020-01-29 05:28:41.000000 jcvi-1.3.5/jcvi/variation/__init__.py
--rw-r--r--   0 bao        (501) staff       (20)      259 2021-06-19 08:23:09.000000 jcvi-1.3.5/jcvi/variation/__main__.py
--rw-r--r--   0 bao        (501) staff       (20)    45321 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/variation/cnv.py
--rw-r--r--   0 bao        (501) staff       (20)     7036 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/variation/deconvolute.py
--rw-r--r--   0 bao        (501) staff       (20)     9385 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/variation/delly.py
--rw-r--r--   0 bao        (501) staff       (20)    11777 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/variation/impute.py
--rw-r--r--   0 bao        (501) staff       (20)     3478 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/variation/phase.py
--rw-r--r--   0 bao        (501) staff       (20)    10831 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/variation/snp.py
--rw-r--r--   0 bao        (501) staff       (20)    48818 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/variation/str.py
--rw-r--r--   0 bao        (501) staff       (20)     3672 2023-02-06 03:44:04.000000 jcvi-1.3.5/jcvi/variation/tassel.py
--rw-r--r--   0 bao        (501) staff       (20)      176 2023-05-20 02:09:56.000000 jcvi-1.3.5/jcvi/version.py
-drwxr-xr-x   0 bao        (501) staff       (20)        0 2023-05-20 02:09:56.408609 jcvi-1.3.5/jcvi.egg-info/
--rw-r--r--   0 bao        (501) staff       (20)     8759 2023-05-20 02:09:56.000000 jcvi-1.3.5/jcvi.egg-info/PKG-INFO
--rw-r--r--   0 bao        (501) staff       (20)     4727 2023-05-20 02:09:56.000000 jcvi-1.3.5/jcvi.egg-info/SOURCES.txt
--rw-r--r--   0 bao        (501) staff       (20)        1 2023-05-20 02:09:56.000000 jcvi-1.3.5/jcvi.egg-info/dependency_links.txt
--rw-r--r--   0 bao        (501) staff       (20)        1 2022-11-26 21:54:22.000000 jcvi-1.3.5/jcvi.egg-info/not-zip-safe
--rw-r--r--   0 bao        (501) staff       (20)      206 2023-05-20 02:09:56.000000 jcvi-1.3.5/jcvi.egg-info/requires.txt
--rw-r--r--   0 bao        (501) staff       (20)        5 2023-05-20 02:09:56.000000 jcvi-1.3.5/jcvi.egg-info/top_level.txt
--rw-r--r--   0 bao        (501) staff       (20)      359 2022-11-26 21:23:29.000000 jcvi-1.3.5/pyproject.toml
--rw-r--r--   0 bao        (501) staff       (20)     1219 2023-05-20 02:09:56.444952 jcvi-1.3.5/setup.cfg
--rw-r--r--   0 bao        (501) staff       (20)      553 2022-11-26 21:23:29.000000 jcvi-1.3.5/setup.py
+drwxr-xr-x   0 bao        (501) staff       (20)        0 2023-06-23 16:27:06.307044 jcvi-1.3.6/
+-rw-r--r--   0 bao        (501) staff       (20)     1292 2020-03-03 07:11:04.000000 jcvi-1.3.6/LICENSE
+-rw-r--r--   0 bao        (501) staff       (20)       91 2022-11-27 15:24:30.000000 jcvi-1.3.6/MANIFEST.in
+-rw-r--r--   0 bao        (501) staff       (20)     8759 2023-06-23 16:27:06.307129 jcvi-1.3.6/PKG-INFO
+-rw-r--r--   0 bao        (501) staff       (20)     8094 2021-04-18 23:59:49.000000 jcvi-1.3.6/README.md
+drwxr-xr-x   0 bao        (501) staff       (20)        0 2023-06-23 16:27:06.274035 jcvi-1.3.6/jcvi/
+-rw-r--r--   0 bao        (501) staff       (20)      770 2022-11-26 21:23:29.000000 jcvi-1.3.6/jcvi/__init__.py
+drwxr-xr-x   0 bao        (501) staff       (20)        0 2023-06-23 16:27:06.276680 jcvi-1.3.6/jcvi/algorithms/
+-rw-r--r--   0 bao        (501) staff       (20)        0 2020-01-29 05:28:41.000000 jcvi-1.3.6/jcvi/algorithms/__init__.py
+-rw-r--r--   0 bao        (501) staff       (20)      263 2021-06-19 08:23:09.000000 jcvi-1.3.6/jcvi/algorithms/__main__.py
+-rw-r--r--   0 bao        (501) staff       (20)     6422 2021-06-19 08:23:09.000000 jcvi-1.3.6/jcvi/algorithms/ec.py
+-rw-r--r--   0 bao        (501) staff       (20)     5678 2023-02-06 03:44:04.000000 jcvi-1.3.6/jcvi/algorithms/formula.py
+-rw-r--r--   0 bao        (501) staff       (20)    14132 2023-02-06 03:44:04.000000 jcvi-1.3.6/jcvi/algorithms/graph.py
+-rwxr-xr-x   0 bao        (501) staff       (20)     6275 2023-02-06 03:44:04.000000 jcvi-1.3.6/jcvi/algorithms/lis.py
+-rwxr-xr-x   0 bao        (501) staff       (20)    24228 2023-02-06 03:44:04.000000 jcvi-1.3.6/jcvi/algorithms/lpsolve.py
+-rw-r--r--   0 bao        (501) staff       (20)     6104 2021-06-19 08:23:09.000000 jcvi-1.3.6/jcvi/algorithms/matrix.py
+-rw-r--r--   0 bao        (501) staff       (20)     1296 2021-06-19 19:45:56.000000 jcvi-1.3.6/jcvi/algorithms/maxsum.py
+-rw-r--r--   0 bao        (501) staff       (20)     1203 2023-02-06 03:44:04.000000 jcvi-1.3.6/jcvi/algorithms/ml.py
+-rwxr-xr-x   0 bao        (501) staff       (20)     4999 2023-02-06 03:44:04.000000 jcvi-1.3.6/jcvi/algorithms/supermap.py
+-rw-r--r--   0 bao        (501) staff       (20)    12559 2022-11-26 15:55:17.000000 jcvi-1.3.6/jcvi/algorithms/tsp.py
+drwxr-xr-x   0 bao        (501) staff       (20)        0 2023-06-23 16:27:06.278418 jcvi-1.3.6/jcvi/annotation/
+-rw-r--r--   0 bao        (501) staff       (20)        0 2020-01-29 05:28:41.000000 jcvi-1.3.6/jcvi/annotation/__init__.py
+-rw-r--r--   0 bao        (501) staff       (20)      261 2021-06-19 08:23:09.000000 jcvi-1.3.6/jcvi/annotation/__main__.py
+-rw-r--r--   0 bao        (501) staff       (20)    21414 2023-02-06 03:44:04.000000 jcvi-1.3.6/jcvi/annotation/ahrd.py
+-rw-r--r--   0 bao        (501) staff       (20)     7899 2023-02-06 03:44:04.000000 jcvi-1.3.6/jcvi/annotation/automaton.py
+-rwxr-xr-x   0 bao        (501) staff       (20)     6417 2023-02-06 03:44:04.000000 jcvi-1.3.6/jcvi/annotation/depth.py
+-rw-r--r--   0 bao        (501) staff       (20)     7042 2023-02-06 03:44:04.000000 jcvi-1.3.6/jcvi/annotation/evm.py
+-rw-r--r--   0 bao        (501) staff       (20)    14687 2023-02-06 03:44:04.000000 jcvi-1.3.6/jcvi/annotation/maker.py
+-rw-r--r--   0 bao        (501) staff       (20)    19485 2023-02-06 03:44:04.000000 jcvi-1.3.6/jcvi/annotation/pasa.py
+-rw-r--r--   0 bao        (501) staff       (20)    12822 2023-02-06 03:44:04.000000 jcvi-1.3.6/jcvi/annotation/qc.py
+-rw-r--r--   0 bao        (501) staff       (20)    42839 2023-02-06 03:44:04.000000 jcvi-1.3.6/jcvi/annotation/reformat.py
+-rw-r--r--   0 bao        (501) staff       (20)    12645 2023-02-06 03:44:04.000000 jcvi-1.3.6/jcvi/annotation/stats.py
+-rw-r--r--   0 bao        (501) staff       (20)     6793 2023-02-06 03:44:04.000000 jcvi-1.3.6/jcvi/annotation/train.py
+drwxr-xr-x   0 bao        (501) staff       (20)        0 2023-06-23 16:27:06.282909 jcvi-1.3.6/jcvi/apps/
+-rw-r--r--   0 bao        (501) staff       (20)        0 2020-01-29 05:28:41.000000 jcvi-1.3.6/jcvi/apps/__init__.py
+-rw-r--r--   0 bao        (501) staff       (20)      258 2021-06-19 08:23:09.000000 jcvi-1.3.6/jcvi/apps/__main__.py
+-rw-r--r--   0 bao        (501) staff       (20)    16889 2023-02-19 15:03:46.000000 jcvi-1.3.6/jcvi/apps/align.py
+-rw-r--r--   0 bao        (501) staff       (20)    68559 2023-06-23 01:57:24.000000 jcvi-1.3.6/jcvi/apps/base.py
+-rw-r--r--   0 bao        (501) staff       (20)    12271 2023-02-06 03:44:04.000000 jcvi-1.3.6/jcvi/apps/biomart.py
+-rwxr-xr-x   0 bao        (501) staff       (20)     3554 2021-06-19 19:45:56.000000 jcvi-1.3.6/jcvi/apps/blastplus.py
+-rw-r--r--   0 bao        (501) staff       (20)     5219 2023-02-06 03:44:04.000000 jcvi-1.3.6/jcvi/apps/bowtie.py
+-rw-r--r--   0 bao        (501) staff       (20)     7695 2023-02-06 03:44:04.000000 jcvi-1.3.6/jcvi/apps/bwa.py
+-rw-r--r--   0 bao        (501) staff       (20)     7279 2023-02-06 03:44:04.000000 jcvi-1.3.6/jcvi/apps/cdhit.py
+-rw-r--r--   0 bao        (501) staff       (20)     2623 2023-02-06 03:44:04.000000 jcvi-1.3.6/jcvi/apps/emboss.py
+-rw-r--r--   0 bao        (501) staff       (20)    21332 2023-02-06 03:44:04.000000 jcvi-1.3.6/jcvi/apps/fetch.py
+-rw-r--r--   0 bao        (501) staff       (20)    19459 2023-02-06 03:44:04.000000 jcvi-1.3.6/jcvi/apps/gbsubmit.py
+-rw-r--r--   0 bao        (501) staff       (20)     6892 2023-02-06 03:44:04.000000 jcvi-1.3.6/jcvi/apps/gmap.py
+-rw-r--r--   0 bao        (501) staff       (20)    18476 2023-04-29 14:56:25.000000 jcvi-1.3.6/jcvi/apps/grid.py
+-rw-r--r--   0 bao        (501) staff       (20)    33945 2023-02-06 03:44:04.000000 jcvi-1.3.6/jcvi/apps/ks.py
+-rwxr-xr-x   0 bao        (501) staff       (20)     7238 2023-02-06 03:44:04.000000 jcvi-1.3.6/jcvi/apps/lastz.py
+-rwxr-xr-x   0 bao        (501) staff       (20)     3004 2023-02-06 03:44:04.000000 jcvi-1.3.6/jcvi/apps/mask.py
+-rw-r--r--   0 bao        (501) staff       (20)    35471 2023-02-06 03:44:04.000000 jcvi-1.3.6/jcvi/apps/phylo.py
+-rw-r--r--   0 bao        (501) staff       (20)     1896 2023-02-06 03:44:04.000000 jcvi-1.3.6/jcvi/apps/r.py
+-rw-r--r--   0 bao        (501) staff       (20)     4901 2023-02-06 03:44:04.000000 jcvi-1.3.6/jcvi/apps/restriction.py
+-rw-r--r--   0 bao        (501) staff       (20)     2116 2021-06-19 08:23:09.000000 jcvi-1.3.6/jcvi/apps/script.py
+-rw-r--r--   0 bao        (501) staff       (20)     3784 2023-02-06 03:44:04.000000 jcvi-1.3.6/jcvi/apps/softlink.py
+-rw-r--r--   0 bao        (501) staff       (20)    33065 2023-02-06 03:44:04.000000 jcvi-1.3.6/jcvi/apps/uclust.py
+-rw-r--r--   0 bao        (501) staff       (20)     5208 2023-02-06 03:44:04.000000 jcvi-1.3.6/jcvi/apps/uniprot.py
+-rw-r--r--   0 bao        (501) staff       (20)     3661 2023-02-06 03:44:04.000000 jcvi-1.3.6/jcvi/apps/vecscreen.py
+drwxr-xr-x   0 bao        (501) staff       (20)        0 2023-06-23 16:27:06.286836 jcvi-1.3.6/jcvi/assembly/
+-rw-r--r--   0 bao        (501) staff       (20)        0 2020-01-29 05:28:41.000000 jcvi-1.3.6/jcvi/assembly/__init__.py
+-rw-r--r--   0 bao        (501) staff       (20)      257 2021-06-19 08:23:09.000000 jcvi-1.3.6/jcvi/assembly/__main__.py
+-rw-r--r--   0 bao        (501) staff       (20)    66136 2023-02-06 03:44:04.000000 jcvi-1.3.6/jcvi/assembly/allmaps.py
+-rw-r--r--   0 bao        (501) staff       (20)    15451 2023-02-06 03:44:04.000000 jcvi-1.3.6/jcvi/assembly/allpaths.py
+-rw-r--r--   0 bao        (501) staff       (20)    13265 2023-02-06 03:44:04.000000 jcvi-1.3.6/jcvi/assembly/automaton.py
+-rw-r--r--   0 bao        (501) staff       (20)     5544 2023-02-06 03:44:04.000000 jcvi-1.3.6/jcvi/assembly/base.py
+-rw-r--r--   0 bao        (501) staff       (20)    34986 2023-02-06 03:44:04.000000 jcvi-1.3.6/jcvi/assembly/ca.py
+-rw-r--r--   0 bao        (501) staff       (20)     3457 2022-09-27 05:18:33.000000 jcvi-1.3.6/jcvi/assembly/chic.pyx
+-rw-r--r--   0 bao        (501) staff       (20)     4581 2023-02-06 03:44:04.000000 jcvi-1.3.6/jcvi/assembly/coverage.py
+-rw-r--r--   0 bao        (501) staff       (20)     8676 2023-02-06 03:44:04.000000 jcvi-1.3.6/jcvi/assembly/gaps.py
+-rw-r--r--   0 bao        (501) staff       (20)    20212 2023-02-19 15:03:46.000000 jcvi-1.3.6/jcvi/assembly/geneticmap.py
+-rw-r--r--   0 bao        (501) staff       (20)    34693 2023-02-06 03:44:04.000000 jcvi-1.3.6/jcvi/assembly/goldenpath.py
+-rw-r--r--   0 bao        (501) staff       (20)    57613 2023-02-06 03:44:04.000000 jcvi-1.3.6/jcvi/assembly/hic.py
+-rw-r--r--   0 bao        (501) staff       (20)    43632 2023-05-05 09:23:28.000000 jcvi-1.3.6/jcvi/assembly/kmer.py
+-rw-r--r--   0 bao        (501) staff       (20)    12519 2023-02-06 03:44:04.000000 jcvi-1.3.6/jcvi/assembly/opticalmap.py
+-rw-r--r--   0 bao        (501) staff       (20)    27279 2023-02-06 03:44:04.000000 jcvi-1.3.6/jcvi/assembly/patch.py
+-rw-r--r--   0 bao        (501) staff       (20)    15741 2023-02-06 03:44:04.000000 jcvi-1.3.6/jcvi/assembly/postprocess.py
+-rw-r--r--   0 bao        (501) staff       (20)    23470 2023-02-06 03:44:04.000000 jcvi-1.3.6/jcvi/assembly/preprocess.py
+-rw-r--r--   0 bao        (501) staff       (20)     6287 2023-02-06 03:44:04.000000 jcvi-1.3.6/jcvi/assembly/sim.py
+-rw-r--r--   0 bao        (501) staff       (20)     8830 2023-02-06 03:44:04.000000 jcvi-1.3.6/jcvi/assembly/soap.py
+-rw-r--r--   0 bao        (501) staff       (20)    16183 2023-04-26 05:51:28.000000 jcvi-1.3.6/jcvi/assembly/syntenypath.py
+-rw-r--r--   0 bao        (501) staff       (20)     5042 2023-02-06 03:44:04.000000 jcvi-1.3.6/jcvi/assembly/trinity.py
+drwxr-xr-x   0 bao        (501) staff       (20)        0 2023-06-23 16:27:06.289168 jcvi-1.3.6/jcvi/compara/
+-rw-r--r--   0 bao        (501) staff       (20)        0 2020-01-29 05:28:41.000000 jcvi-1.3.6/jcvi/compara/__init__.py
+-rw-r--r--   0 bao        (501) staff       (20)      251 2021-06-19 08:23:09.000000 jcvi-1.3.6/jcvi/compara/__main__.py
+-rw-r--r--   0 bao        (501) staff       (20)     4210 2023-04-26 05:51:28.000000 jcvi-1.3.6/jcvi/compara/base.py
+-rwxr-xr-x   0 bao        (501) staff       (20)     9796 2023-04-26 05:51:28.000000 jcvi-1.3.6/jcvi/compara/blastfilter.py
+-rw-r--r--   0 bao        (501) staff       (20)    27460 2023-05-20 02:09:12.000000 jcvi-1.3.6/jcvi/compara/catalog.py
+-rw-r--r--   0 bao        (501) staff       (20)    26355 2023-02-06 03:44:04.000000 jcvi-1.3.6/jcvi/compara/fractionation.py
+-rw-r--r--   0 bao        (501) staff       (20)     9216 2023-04-26 05:51:28.000000 jcvi-1.3.6/jcvi/compara/pad.py
+-rw-r--r--   0 bao        (501) staff       (20)     3051 2021-06-19 08:23:09.000000 jcvi-1.3.6/jcvi/compara/phylogeny.py
+-rwxr-xr-x   0 bao        (501) staff       (20)     7948 2023-04-26 05:51:28.000000 jcvi-1.3.6/jcvi/compara/quota.py
+-rw-r--r--   0 bao        (501) staff       (20)    10341 2023-04-26 05:51:28.000000 jcvi-1.3.6/jcvi/compara/reconstruct.py
+-rwxr-xr-x   0 bao        (501) staff       (20)     9233 2023-02-06 03:44:04.000000 jcvi-1.3.6/jcvi/compara/synfind.py
+-rwxr-xr-x   0 bao        (501) staff       (20)    57574 2023-04-26 05:51:28.000000 jcvi-1.3.6/jcvi/compara/synteny.py
+drwxr-xr-x   0 bao        (501) staff       (20)        0 2023-06-23 16:27:06.294557 jcvi-1.3.6/jcvi/formats/
+-rw-r--r--   0 bao        (501) staff       (20)        0 2020-01-29 05:28:41.000000 jcvi-1.3.6/jcvi/formats/__init__.py
+-rw-r--r--   0 bao        (501) staff       (20)      262 2021-06-19 08:23:09.000000 jcvi-1.3.6/jcvi/formats/__main__.py
+-rw-r--r--   0 bao        (501) staff       (20)    63612 2023-02-06 03:44:04.000000 jcvi-1.3.6/jcvi/formats/agp.py
+-rw-r--r--   0 bao        (501) staff       (20)    33966 2023-02-06 03:44:04.000000 jcvi-1.3.6/jcvi/formats/base.py
+-rwxr-xr-x   0 bao        (501) staff       (20)    75038 2023-06-23 01:57:20.000000 jcvi-1.3.6/jcvi/formats/bed.py
+-rw-r--r--   0 bao        (501) staff       (20)    43184 2023-06-19 14:46:14.000000 jcvi-1.3.6/jcvi/formats/blast.py
+-rw-r--r--   0 bao        (501) staff       (20)     7010 2022-09-27 05:18:33.000000 jcvi-1.3.6/jcvi/formats/cblast.pyx
+-rw-r--r--   0 bao        (501) staff       (20)     3193 2023-02-06 03:44:04.000000 jcvi-1.3.6/jcvi/formats/cdt.py
+-rw-r--r--   0 bao        (501) staff       (20)     8612 2023-02-06 03:44:04.000000 jcvi-1.3.6/jcvi/formats/chain.py
+-rw-r--r--   0 bao        (501) staff       (20)     4644 2023-02-06 03:44:04.000000 jcvi-1.3.6/jcvi/formats/contig.py
+-rw-r--r--   0 bao        (501) staff       (20)    15170 2023-02-06 03:44:04.000000 jcvi-1.3.6/jcvi/formats/coords.py
+-rw-r--r--   0 bao        (501) staff       (20)     6529 2023-02-06 03:44:04.000000 jcvi-1.3.6/jcvi/formats/excel.py
+-rw-r--r--   0 bao        (501) staff       (20)    75590 2023-02-06 03:44:04.000000 jcvi-1.3.6/jcvi/formats/fasta.py
+-rw-r--r--   0 bao        (501) staff       (20)    29575 2023-02-06 03:44:04.000000 jcvi-1.3.6/jcvi/formats/fastq.py
+-rw-r--r--   0 bao        (501) staff       (20)    15549 2023-02-06 03:44:04.000000 jcvi-1.3.6/jcvi/formats/genbank.py
+-rw-r--r--   0 bao        (501) staff       (20)   118976 2023-02-06 03:44:04.000000 jcvi-1.3.6/jcvi/formats/gff.py
+-rw-r--r--   0 bao        (501) staff       (20)     3979 2023-02-06 03:44:04.000000 jcvi-1.3.6/jcvi/formats/html.py
+-rw-r--r--   0 bao        (501) staff       (20)     4612 2023-02-06 03:44:04.000000 jcvi-1.3.6/jcvi/formats/maf.py
+-rwxr-xr-x   0 bao        (501) staff       (20)     2842 2021-07-05 22:45:00.000000 jcvi-1.3.6/jcvi/formats/obo.py
+-rw-r--r--   0 bao        (501) staff       (20)     2900 2021-01-11 06:59:36.000000 jcvi-1.3.6/jcvi/formats/paf.py
+-rw-r--r--   0 bao        (501) staff       (20)     2785 2023-02-06 03:44:04.000000 jcvi-1.3.6/jcvi/formats/pdf.py
+-rwxr-xr-x   0 bao        (501) staff       (20)    10355 2023-02-06 03:44:04.000000 jcvi-1.3.6/jcvi/formats/psl.py
+-rw-r--r--   0 bao        (501) staff       (20)     2746 2021-06-19 08:23:09.000000 jcvi-1.3.6/jcvi/formats/pyblast.py
+-rw-r--r--   0 bao        (501) staff       (20)    28231 2023-02-06 03:44:04.000000 jcvi-1.3.6/jcvi/formats/sam.py
+-rw-r--r--   0 bao        (501) staff       (20)     8041 2023-02-06 03:44:04.000000 jcvi-1.3.6/jcvi/formats/sizes.py
+-rw-r--r--   0 bao        (501) staff       (20)    25480 2023-02-06 03:44:04.000000 jcvi-1.3.6/jcvi/formats/vcf.py
+drwxr-xr-x   0 bao        (501) staff       (20)        0 2023-06-23 16:27:06.298621 jcvi-1.3.6/jcvi/graphics/
+-rw-r--r--   0 bao        (501) staff       (20)        0 2020-01-29 05:28:41.000000 jcvi-1.3.6/jcvi/graphics/__init__.py
+-rw-r--r--   0 bao        (501) staff       (20)      271 2021-06-19 08:23:09.000000 jcvi-1.3.6/jcvi/graphics/__main__.py
+-rw-r--r--   0 bao        (501) staff       (20)    16271 2023-02-06 03:44:04.000000 jcvi-1.3.6/jcvi/graphics/align.py
+-rw-r--r--   0 bao        (501) staff       (20)    15265 2023-02-06 03:44:04.000000 jcvi-1.3.6/jcvi/graphics/assembly.py
+-rw-r--r--   0 bao        (501) staff       (20)    22168 2023-06-23 01:57:24.000000 jcvi-1.3.6/jcvi/graphics/base.py
+-rwxr-xr-x   0 bao        (501) staff       (20)    10006 2023-02-06 03:44:04.000000 jcvi-1.3.6/jcvi/graphics/blastplot.py
+-rw-r--r--   0 bao        (501) staff       (20)    22427 2023-02-06 05:16:46.000000 jcvi-1.3.6/jcvi/graphics/chromosome.py
+-rw-r--r--   0 bao        (501) staff       (20)     7145 2021-06-19 08:23:09.000000 jcvi-1.3.6/jcvi/graphics/coverage.py
+-rwxr-xr-x   0 bao        (501) staff       (20)    14873 2023-04-26 05:51:28.000000 jcvi-1.3.6/jcvi/graphics/dotplot.py
+-rw-r--r--   0 bao        (501) staff       (20)    21810 2023-02-06 05:16:46.000000 jcvi-1.3.6/jcvi/graphics/glyph.py
+-rw-r--r--   0 bao        (501) staff       (20)    23626 2023-02-06 03:44:04.000000 jcvi-1.3.6/jcvi/graphics/grabseeds.py
+-rwxr-xr-x   0 bao        (501) staff       (20)     2379 2021-06-19 08:23:09.000000 jcvi-1.3.6/jcvi/graphics/graph.py
+-rw-r--r--   0 bao        (501) staff       (20)     5025 2021-03-26 15:38:36.000000 jcvi-1.3.6/jcvi/graphics/heatmap.py
+-rw-r--r--   0 bao        (501) staff       (20)     9612 2023-02-06 03:44:04.000000 jcvi-1.3.6/jcvi/graphics/histogram.py
+-rw-r--r--   0 bao        (501) staff       (20)    13375 2023-02-08 03:44:09.000000 jcvi-1.3.6/jcvi/graphics/karyotype.py
+-rw-r--r--   0 bao        (501) staff       (20)    31416 2023-02-06 03:44:04.000000 jcvi-1.3.6/jcvi/graphics/landscape.py
+-rw-r--r--   0 bao        (501) staff       (20)     1276 2021-06-19 08:23:09.000000 jcvi-1.3.6/jcvi/graphics/logo.py
+-rw-r--r--   0 bao        (501) staff       (20)     3893 2023-02-06 03:44:04.000000 jcvi-1.3.6/jcvi/graphics/mummerplot.py
+-rw-r--r--   0 bao        (501) staff       (20)    20888 2023-02-08 03:44:09.000000 jcvi-1.3.6/jcvi/graphics/synteny.py
+-rw-r--r--   0 bao        (501) staff       (20)     5488 2021-06-19 19:45:56.000000 jcvi-1.3.6/jcvi/graphics/table.py
+-rw-r--r--   0 bao        (501) staff       (20)    20377 2022-11-26 16:06:34.000000 jcvi-1.3.6/jcvi/graphics/tree.py
+-rw-r--r--   0 bao        (501) staff       (20)     6194 2023-02-06 03:44:04.000000 jcvi-1.3.6/jcvi/graphics/wheel.py
+-rw-r--r--   0 bao        (501) staff       (20)     1675 2021-03-26 15:38:36.000000 jcvi-1.3.6/jcvi/graphics/whisker.py
+drwxr-xr-x   0 bao        (501) staff       (20)        0 2023-06-23 16:27:06.301437 jcvi-1.3.6/jcvi/projects/
+-rw-r--r--   0 bao        (501) staff       (20)        0 2020-01-29 05:28:41.000000 jcvi-1.3.6/jcvi/projects/__init__.py
+-rw-r--r--   0 bao        (501) staff       (20)      260 2021-06-19 08:23:09.000000 jcvi-1.3.6/jcvi/projects/__main__.py
+-rw-r--r--   0 bao        (501) staff       (20)    22445 2023-02-06 03:44:04.000000 jcvi-1.3.6/jcvi/projects/age.py
+-rw-r--r--   0 bao        (501) staff       (20)     1571 2023-02-06 03:44:04.000000 jcvi-1.3.6/jcvi/projects/alfalfa.py
+-rw-r--r--   0 bao        (501) staff       (20)    15907 2023-02-06 03:44:04.000000 jcvi-1.3.6/jcvi/projects/allmaps.py
+-rw-r--r--   0 bao        (501) staff       (20)     6750 2023-02-06 03:44:04.000000 jcvi-1.3.6/jcvi/projects/bites.py
+-rw-r--r--   0 bao        (501) staff       (20)     5679 2023-02-06 03:44:04.000000 jcvi-1.3.6/jcvi/projects/heterosis.py
+-rw-r--r--   0 bao        (501) staff       (20)    14136 2023-02-06 03:44:04.000000 jcvi-1.3.6/jcvi/projects/ies.py
+-rw-r--r--   0 bao        (501) staff       (20)    22201 2023-02-06 03:44:04.000000 jcvi-1.3.6/jcvi/projects/misc.py
+-rw-r--r--   0 bao        (501) staff       (20)    25024 2023-02-06 05:16:46.000000 jcvi-1.3.6/jcvi/projects/napus.py
+-rw-r--r--   0 bao        (501) staff       (20)    12754 2023-02-06 03:44:04.000000 jcvi-1.3.6/jcvi/projects/pineapple.py
+-rw-r--r--   0 bao        (501) staff       (20)     2367 2023-02-06 03:44:04.000000 jcvi-1.3.6/jcvi/projects/pistachio.py
+-rw-r--r--   0 bao        (501) staff       (20)    67857 2023-02-06 03:44:04.000000 jcvi-1.3.6/jcvi/projects/str.py
+-rw-r--r--   0 bao        (501) staff       (20)    25768 2023-04-29 14:56:25.000000 jcvi-1.3.6/jcvi/projects/sugarcane.py
+-rw-r--r--   0 bao        (501) staff       (20)    23950 2023-02-06 03:44:04.000000 jcvi-1.3.6/jcvi/projects/synfind.py
+-rw-r--r--   0 bao        (501) staff       (20)    21554 2023-02-06 03:44:04.000000 jcvi-1.3.6/jcvi/projects/tgbs.py
+-rw-r--r--   0 bao        (501) staff       (20)    11941 2023-04-26 05:51:28.000000 jcvi-1.3.6/jcvi/projects/vanilla.py
+drwxr-xr-x   0 bao        (501) staff       (20)        0 2023-06-23 16:27:06.303911 jcvi-1.3.6/jcvi/utils/
+-rw-r--r--   0 bao        (501) staff       (20)        0 2020-01-29 05:28:41.000000 jcvi-1.3.6/jcvi/utils/__init__.py
+-rw-r--r--   0 bao        (501) staff       (20)      260 2021-06-19 08:23:09.000000 jcvi-1.3.6/jcvi/utils/__main__.py
+-rw-r--r--   0 bao        (501) staff       (20)    24200 2023-02-06 03:44:04.000000 jcvi-1.3.6/jcvi/utils/aws.py
+-rw-r--r--   0 bao        (501) staff       (20)    12512 2023-02-06 03:44:04.000000 jcvi-1.3.6/jcvi/utils/cbook.py
+-rw-r--r--   0 bao        (501) staff       (20)      355 2021-01-11 02:34:49.000000 jcvi-1.3.6/jcvi/utils/console.py
+drwxr-xr-x   0 bao        (501) staff       (20)        0 2023-06-23 16:27:06.305721 jcvi-1.3.6/jcvi/utils/data/
+-rwxr-xr-x   0 bao        (501) staff       (20)    16912 2020-01-29 05:28:41.000000 jcvi-1.3.6/jcvi/utils/data/Airswing.ttf
+-rwxr-xr-x   0 bao        (501) staff       (20)   103940 2020-01-29 05:28:41.000000 jcvi-1.3.6/jcvi/utils/data/Collegia.ttf
+-rwxr-xr-x   0 bao        (501) staff       (20)    20468 2020-01-29 05:28:41.000000 jcvi-1.3.6/jcvi/utils/data/HookedUp.ttf
+-rw-r--r--   0 bao        (501) staff       (20)    25832 2020-01-29 05:28:41.000000 jcvi-1.3.6/jcvi/utils/data/Humor-Sans.ttf
+-rw-r--r--   0 bao        (501) staff       (20)    28065 2020-01-29 05:28:41.000000 jcvi-1.3.6/jcvi/utils/data/TREDs.meta.csv
+-rw-r--r--   0 bao        (501) staff       (20)        0 2020-01-29 05:28:41.000000 jcvi-1.3.6/jcvi/utils/data/__init__.py
+-rw-r--r--   0 bao        (501) staff       (20)      911 2020-01-29 05:28:41.000000 jcvi-1.3.6/jcvi/utils/data/adapters.fasta
+-rw-r--r--   0 bao        (501) staff       (20)     3321 2020-01-29 05:28:41.000000 jcvi-1.3.6/jcvi/utils/data/blosum80.mat
+-rw-r--r--   0 bao        (501) staff       (20)     7686 2020-01-29 05:28:41.000000 jcvi-1.3.6/jcvi/utils/data/chrY.hg38.unique_ccn.gc
+-rw-r--r--   0 bao        (501) staff       (20)      282 2020-01-29 05:28:41.000000 jcvi-1.3.6/jcvi/utils/data/colorchecker.txt
+-rw-r--r--   0 bao        (501) staff       (20)    45544 2020-01-29 05:28:41.000000 jcvi-1.3.6/jcvi/utils/data/hg38.band.txt
+-rw-r--r--   0 bao        (501) staff       (20)    11672 2020-01-29 05:28:41.000000 jcvi-1.3.6/jcvi/utils/data/hg38.chrom.sizes
+-rw-r--r--   0 bao        (501) staff       (20)     1000 2020-01-29 05:28:41.000000 jcvi-1.3.6/jcvi/utils/data/instance.json
+-rw-r--r--   0 bao        (501) staff       (20)     9795 2023-02-06 03:44:04.000000 jcvi-1.3.6/jcvi/utils/db.py
+-rw-r--r--   0 bao        (501) staff       (20)     4145 2021-01-09 20:22:53.000000 jcvi-1.3.6/jcvi/utils/ez_setup.py
+-rwxr-xr-x   0 bao        (501) staff       (20)     2884 2021-06-19 08:23:09.000000 jcvi-1.3.6/jcvi/utils/grouper.py
+-rw-r--r--   0 bao        (501) staff       (20)    10437 2021-06-19 08:23:09.000000 jcvi-1.3.6/jcvi/utils/orderedcollections.py
+-rw-r--r--   0 bao        (501) staff       (20)    14595 2023-02-06 03:44:04.000000 jcvi-1.3.6/jcvi/utils/range.py
+-rw-r--r--   0 bao        (501) staff       (20)     3946 2023-02-06 03:44:04.000000 jcvi-1.3.6/jcvi/utils/table.py
+-rw-r--r--   0 bao        (501) staff       (20)     4687 2023-02-06 03:44:04.000000 jcvi-1.3.6/jcvi/utils/taxonomy.py
+-rw-r--r--   0 bao        (501) staff       (20)     1522 2021-07-13 05:06:52.000000 jcvi-1.3.6/jcvi/utils/validator.py
+-rwxr-xr-x   0 bao        (501) staff       (20)     1377 2021-01-15 14:44:37.000000 jcvi-1.3.6/jcvi/utils/webcolors.py
+drwxr-xr-x   0 bao        (501) staff       (20)        0 2023-06-23 16:27:06.306920 jcvi-1.3.6/jcvi/variation/
+-rw-r--r--   0 bao        (501) staff       (20)        0 2020-01-29 05:28:41.000000 jcvi-1.3.6/jcvi/variation/__init__.py
+-rw-r--r--   0 bao        (501) staff       (20)      259 2021-06-19 08:23:09.000000 jcvi-1.3.6/jcvi/variation/__main__.py
+-rw-r--r--   0 bao        (501) staff       (20)    45321 2023-02-06 03:44:04.000000 jcvi-1.3.6/jcvi/variation/cnv.py
+-rw-r--r--   0 bao        (501) staff       (20)     7036 2023-02-06 03:44:04.000000 jcvi-1.3.6/jcvi/variation/deconvolute.py
+-rw-r--r--   0 bao        (501) staff       (20)     9385 2023-02-06 03:44:04.000000 jcvi-1.3.6/jcvi/variation/delly.py
+-rw-r--r--   0 bao        (501) staff       (20)    11777 2023-02-06 03:44:04.000000 jcvi-1.3.6/jcvi/variation/impute.py
+-rw-r--r--   0 bao        (501) staff       (20)     3478 2023-02-06 03:44:04.000000 jcvi-1.3.6/jcvi/variation/phase.py
+-rw-r--r--   0 bao        (501) staff       (20)    10831 2023-02-06 03:44:04.000000 jcvi-1.3.6/jcvi/variation/snp.py
+-rw-r--r--   0 bao        (501) staff       (20)    48818 2023-02-06 03:44:04.000000 jcvi-1.3.6/jcvi/variation/str.py
+-rw-r--r--   0 bao        (501) staff       (20)     3672 2023-02-06 03:44:04.000000 jcvi-1.3.6/jcvi/variation/tassel.py
+-rw-r--r--   0 bao        (501) staff       (20)      176 2023-06-23 16:27:06.000000 jcvi-1.3.6/jcvi/version.py
+drwxr-xr-x   0 bao        (501) staff       (20)        0 2023-06-23 16:27:06.274742 jcvi-1.3.6/jcvi.egg-info/
+-rw-r--r--   0 bao        (501) staff       (20)     8759 2023-06-23 16:27:06.000000 jcvi-1.3.6/jcvi.egg-info/PKG-INFO
+-rw-r--r--   0 bao        (501) staff       (20)     4727 2023-06-23 16:27:06.000000 jcvi-1.3.6/jcvi.egg-info/SOURCES.txt
+-rw-r--r--   0 bao        (501) staff       (20)        1 2023-06-23 16:27:06.000000 jcvi-1.3.6/jcvi.egg-info/dependency_links.txt
+-rw-r--r--   0 bao        (501) staff       (20)        1 2022-11-26 21:54:22.000000 jcvi-1.3.6/jcvi.egg-info/not-zip-safe
+-rw-r--r--   0 bao        (501) staff       (20)      206 2023-06-23 16:27:06.000000 jcvi-1.3.6/jcvi.egg-info/requires.txt
+-rw-r--r--   0 bao        (501) staff       (20)        5 2023-06-23 16:27:06.000000 jcvi-1.3.6/jcvi.egg-info/top_level.txt
+-rw-r--r--   0 bao        (501) staff       (20)      359 2022-11-26 21:23:29.000000 jcvi-1.3.6/pyproject.toml
+-rw-r--r--   0 bao        (501) staff       (20)     1225 2023-06-23 16:27:06.307472 jcvi-1.3.6/setup.cfg
+-rw-r--r--   0 bao        (501) staff       (20)      553 2022-11-26 21:23:29.000000 jcvi-1.3.6/setup.py
```

### Comparing `jcvi-1.3.5/LICENSE` & `jcvi-1.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.5/PKG-INFO` & `jcvi-1.3.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jcvi
-Version: 1.3.5
+Version: 1.3.6
 Summary: Python utility libraries on genome assembly, annotation and comparative genomics
 Home-page: http://github.com/tanghaibao/jcvi
 Author: Haibao Tang, Vivek Krishnakumar, Jingping Li
 Author-email: tanghaibao@gmail.com
 License: BSD
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `jcvi-1.3.5/README.md` & `jcvi-1.3.6/README.md`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.5/jcvi/__init__.py` & `jcvi-1.3.6/jcvi/__init__.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.5/jcvi/algorithms/ec.py` & `jcvi-1.3.6/jcvi/algorithms/ec.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.5/jcvi/algorithms/formula.py` & `jcvi-1.3.6/jcvi/algorithms/formula.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.5/jcvi/algorithms/graph.py` & `jcvi-1.3.6/jcvi/algorithms/graph.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.5/jcvi/algorithms/lis.py` & `jcvi-1.3.6/jcvi/algorithms/lis.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.5/jcvi/algorithms/lpsolve.py` & `jcvi-1.3.6/jcvi/algorithms/lpsolve.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.5/jcvi/algorithms/matrix.py` & `jcvi-1.3.6/jcvi/algorithms/matrix.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.5/jcvi/algorithms/maxsum.py` & `jcvi-1.3.6/jcvi/algorithms/maxsum.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.5/jcvi/algorithms/ml.py` & `jcvi-1.3.6/jcvi/algorithms/ml.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.5/jcvi/algorithms/supermap.py` & `jcvi-1.3.6/jcvi/algorithms/supermap.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.5/jcvi/algorithms/tsp.py` & `jcvi-1.3.6/jcvi/algorithms/tsp.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.5/jcvi/annotation/ahrd.py` & `jcvi-1.3.6/jcvi/annotation/ahrd.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.5/jcvi/annotation/automaton.py` & `jcvi-1.3.6/jcvi/annotation/automaton.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.5/jcvi/annotation/depth.py` & `jcvi-1.3.6/jcvi/annotation/depth.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.5/jcvi/annotation/evm.py` & `jcvi-1.3.6/jcvi/annotation/evm.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.5/jcvi/annotation/maker.py` & `jcvi-1.3.6/jcvi/annotation/maker.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.5/jcvi/annotation/pasa.py` & `jcvi-1.3.6/jcvi/annotation/pasa.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.5/jcvi/annotation/qc.py` & `jcvi-1.3.6/jcvi/annotation/qc.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.5/jcvi/annotation/reformat.py` & `jcvi-1.3.6/jcvi/annotation/reformat.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.5/jcvi/annotation/stats.py` & `jcvi-1.3.6/jcvi/annotation/stats.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.5/jcvi/annotation/train.py` & `jcvi-1.3.6/jcvi/annotation/train.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.5/jcvi/apps/align.py` & `jcvi-1.3.6/jcvi/apps/align.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.5/jcvi/apps/base.py` & `jcvi-1.3.6/jcvi/apps/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 import time
 import os.path as op
 import shutil
 import signal
 import sys
 import logging
 import fnmatch
+import functools
+
 
 from collections.abc import Iterable
 from http.client import HTTPSConnection
 from urllib.parse import urlencode
 from configparser import (
     ConfigParser,
     RawConfigParser,
@@ -34,14 +36,38 @@
 # http://newbebweb.blogspot.com/2012/02/python-head-ioerror-errno-32-broken.html
 nobreakbuffer = lambda: signal.signal(signal.SIGPIPE, signal.SIG_DFL)
 nobreakbuffer()
 os.environ["LC_ALL"] = "C"
 JCVIHELP = "JCVI utility libraries {} [{}]\n".format(__version__, __copyright__)
 
 
+def patch_debug(func):
+    @functools.wraps(func)
+    def wraps(*args, **kwargs):
+        import inspect
+
+        callerframerecord = inspect.stack()[1]
+        frame = callerframerecord[0]
+        info = inspect.getframeinfo(frame)
+        # get caller function name
+        caller = frame.f_code.co_name
+        patch_message = f"{info.filename}:{info.lineno}:{caller}"
+        old_debug = logging.debug
+
+        def my_debug(message: str, *args, **kwargs):
+            old_debug(f"{patch_message} {message}", *args, **kwargs)
+
+        logging.debug = my_debug
+        ret = func(*args, **kwargs)
+        logging.debug = old_debug
+        return ret
+
+    return wraps
+
+
 class ActionDispatcher(object):
     """
     This class will be invoked
     a) when the base package is run via __main__, listing all MODULESs
     a) when a directory is run via __main__, listing all SCRIPTs
     b) when a script is run directly, listing all ACTIONs
 
@@ -1219,15 +1245,15 @@
     """
     Emulates the unix which command.
 
     >>> which("cat")
     "/bin/cat"
     >>> which("nosuchprogram")
     """
-    fpath, fname = op.split(program)
+    fpath, _ = op.split(program)
     if fpath:
         if is_exe(program):
             return program
     else:
         for path in os.environ["PATH"].split(os.pathsep):
             exe_file = op.join(path, program)
             if is_exe(exe_file):
@@ -2165,15 +2191,21 @@
         logging.error(
             "There was a problem reading or parsing "
             "your credentials file: %s" % (e.args[0],),
         )
     return config
 
 
-def getpath(cmd, name=None, url=None, cfg="~/.jcvirc", warn="exit"):
+def getpath(
+    cmd: str,
+    name: Optional[str] = None,
+    url: Optional[str] = None,
+    cfg: str = "~/.jcvirc",
+    warn: str = "exit",
+) -> Optional[str]:
     """
     Get install locations of common binaries
     First, check ~/.jcvirc file to get the full path
     If not present, ask on the console and store
     """
     p = which(cmd)  # if in PATH, just returns it
     if p:
@@ -2188,37 +2220,40 @@
 
     assert name is not None, "Need a program name"
 
     try:
         fullpath = config.get(PATH, name)
     except NoSectionError:
         config.add_section(PATH)
-        changed = True
 
     try:
         fullpath = config.get(PATH, name)
     except NoOptionError:
-        msg = "=== Configure path for {0} ===\n".format(name, cfg)
+        msg = f"=== Configure path for {name} ===\n"
         if url:
-            msg += "URL: {0}\n".format(url)
-        msg += "[Directory that contains `{0}`]: ".format(cmd)
+            msg += f"URL: {url}\n"
+        msg += f"[Directory that contains `{cmd}`]: "
         fullpath = input(msg).strip()
-        config.set(PATH, name, fullpath)
-        changed = True
 
     path = op.join(op.expanduser(fullpath), cmd)
-    if warn == "exit":
-        try:
-            assert is_exe(path), "***ERROR: Cannot execute binary `{0}`. ".format(path)
-        except AssertionError as e:
-            sys.exit("{0!s}Please verify and rerun.".format(e))
+    if is_exe(path):
+        config.set(PATH, name, fullpath)
+        changed = True
+    else:
+        err_msg = f"Cannot execute binary `{path}`. Please verify and rerun."
+        if warn == "exit":
+            logging.fatal(err_msg)
+        else:
+            logging.warning(err_msg)
+        return None
 
     if changed:
         configfile = open(cfg, "w")
         config.write(configfile)
+        configfile.close()
         logging.debug("Configuration written to `{0}`.".format(cfg))
 
     return path
 
 
 def inspect(object):
     """A better dir() showing attributes and values"""
```

### Comparing `jcvi-1.3.5/jcvi/apps/biomart.py` & `jcvi-1.3.6/jcvi/apps/biomart.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.5/jcvi/apps/blastplus.py` & `jcvi-1.3.6/jcvi/apps/blastplus.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.5/jcvi/apps/bowtie.py` & `jcvi-1.3.6/jcvi/apps/bowtie.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.5/jcvi/apps/bwa.py` & `jcvi-1.3.6/jcvi/apps/bwa.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.5/jcvi/apps/cdhit.py` & `jcvi-1.3.6/jcvi/apps/cdhit.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.5/jcvi/apps/emboss.py` & `jcvi-1.3.6/jcvi/apps/emboss.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.5/jcvi/apps/fetch.py` & `jcvi-1.3.6/jcvi/apps/fetch.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.5/jcvi/apps/gbsubmit.py` & `jcvi-1.3.6/jcvi/apps/gbsubmit.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.5/jcvi/apps/gmap.py` & `jcvi-1.3.6/jcvi/apps/gmap.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.5/jcvi/apps/grid.py` & `jcvi-1.3.6/jcvi/apps/grid.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.5/jcvi/apps/ks.py` & `jcvi-1.3.6/jcvi/apps/ks.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.5/jcvi/apps/lastz.py` & `jcvi-1.3.6/jcvi/apps/lastz.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.5/jcvi/apps/mask.py` & `jcvi-1.3.6/jcvi/apps/mask.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.5/jcvi/apps/phylo.py` & `jcvi-1.3.6/jcvi/apps/phylo.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.5/jcvi/apps/r.py` & `jcvi-1.3.6/jcvi/apps/r.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.5/jcvi/apps/restriction.py` & `jcvi-1.3.6/jcvi/apps/restriction.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.5/jcvi/apps/script.py` & `jcvi-1.3.6/jcvi/apps/script.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.5/jcvi/apps/softlink.py` & `jcvi-1.3.6/jcvi/apps/softlink.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.5/jcvi/apps/uclust.py` & `jcvi-1.3.6/jcvi/apps/uclust.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.5/jcvi/apps/uniprot.py` & `jcvi-1.3.6/jcvi/apps/uniprot.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.5/jcvi/apps/vecscreen.py` & `jcvi-1.3.6/jcvi/apps/vecscreen.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.5/jcvi/assembly/allmaps.py` & `jcvi-1.3.6/jcvi/assembly/allmaps.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.5/jcvi/assembly/allpaths.py` & `jcvi-1.3.6/jcvi/assembly/allpaths.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.5/jcvi/assembly/automaton.py` & `jcvi-1.3.6/jcvi/assembly/automaton.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.5/jcvi/assembly/base.py` & `jcvi-1.3.6/jcvi/assembly/base.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.5/jcvi/assembly/ca.py` & `jcvi-1.3.6/jcvi/assembly/ca.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.5/jcvi/assembly/chic.pyx` & `jcvi-1.3.6/jcvi/assembly/chic.pyx`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.5/jcvi/assembly/coverage.py` & `jcvi-1.3.6/jcvi/assembly/coverage.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.5/jcvi/assembly/gaps.py` & `jcvi-1.3.6/jcvi/assembly/gaps.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.5/jcvi/assembly/geneticmap.py` & `jcvi-1.3.6/jcvi/assembly/geneticmap.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.5/jcvi/assembly/goldenpath.py` & `jcvi-1.3.6/jcvi/assembly/goldenpath.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.5/jcvi/assembly/hic.py` & `jcvi-1.3.6/jcvi/assembly/hic.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.5/jcvi/assembly/kmer.py` & `jcvi-1.3.6/jcvi/assembly/kmer.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.5/jcvi/assembly/opticalmap.py` & `jcvi-1.3.6/jcvi/assembly/opticalmap.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.5/jcvi/assembly/patch.py` & `jcvi-1.3.6/jcvi/assembly/patch.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.5/jcvi/assembly/postprocess.py` & `jcvi-1.3.6/jcvi/assembly/postprocess.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.5/jcvi/assembly/preprocess.py` & `jcvi-1.3.6/jcvi/assembly/preprocess.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.5/jcvi/assembly/sim.py` & `jcvi-1.3.6/jcvi/assembly/sim.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.5/jcvi/assembly/soap.py` & `jcvi-1.3.6/jcvi/assembly/soap.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.5/jcvi/assembly/syntenypath.py` & `jcvi-1.3.6/jcvi/assembly/syntenypath.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.5/jcvi/assembly/trinity.py` & `jcvi-1.3.6/jcvi/assembly/trinity.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.5/jcvi/compara/base.py` & `jcvi-1.3.6/jcvi/compara/base.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.5/jcvi/compara/blastfilter.py` & `jcvi-1.3.6/jcvi/compara/blastfilter.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.5/jcvi/compara/catalog.py` & `jcvi-1.3.6/jcvi/compara/catalog.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.5/jcvi/compara/fractionation.py` & `jcvi-1.3.6/jcvi/compara/fractionation.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.5/jcvi/compara/pad.py` & `jcvi-1.3.6/jcvi/compara/pad.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.5/jcvi/compara/phylogeny.py` & `jcvi-1.3.6/jcvi/compara/phylogeny.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.5/jcvi/compara/quota.py` & `jcvi-1.3.6/jcvi/compara/quota.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.5/jcvi/compara/reconstruct.py` & `jcvi-1.3.6/jcvi/compara/reconstruct.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.5/jcvi/compara/synfind.py` & `jcvi-1.3.6/jcvi/compara/synfind.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.5/jcvi/compara/synteny.py` & `jcvi-1.3.6/jcvi/compara/synteny.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.5/jcvi/formats/agp.py` & `jcvi-1.3.6/jcvi/formats/agp.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.5/jcvi/formats/base.py` & `jcvi-1.3.6/jcvi/formats/base.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.5/jcvi/formats/bed.py` & `jcvi-1.3.6/jcvi/formats/bed.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 """
 Classes to handle the .bed files
 """
+import logging
+import math
+import numpy as np
 import os
 import os.path as op
+import shutil
 import sys
-import math
-import logging
-import numpy as np
 
 from collections import defaultdict, OrderedDict
 from itertools import groupby
+from typing import Optional
 
 from more_itertools import pairwise
 from natsort import natsorted, natsort_key
 
 from jcvi.formats.base import DictFile, LineFile, must_open, is_number, get_number
 from jcvi.formats.sizes import Sizes
 from jcvi.utils.cbook import SummaryStats, thousands, percentage
@@ -243,15 +245,14 @@
     def sub_bed(self, seqid):
         # get all the beds on one chromosome
         for b in self:
             if b.seqid == seqid:
                 yield b
 
     def sub_beds(self):
-
         self.sort(key=self.nullkey)
         # get all the beds on all chromosomes, emitting one at a time
         for bs, sb in groupby(self, key=lambda x: x.seqid):
             yield bs, list(sb)
 
     def get_breaks(self):
         # get chromosome break positions
@@ -339,15 +340,14 @@
         assert self.start1 <= self.end2
         args = (self.seqid1, self.start1 - 1, self.end2, self.accn)
         return "\t".join(str(x) for x in args)
 
 
 class BedEvaluate(object):
     def __init__(self, TPbed, FPbed, FNbed, TNbed):
-
         self.TP = Bed(TPbed).sum(unique=True)
         self.FP = Bed(FPbed).sum(unique=True)
         self.FN = Bed(FNbed).sum(unique=True)
         self.TN = Bed(TNbed).sum(unique=True)
 
     def __str__(self):
         from jcvi.utils.table import tabulate
@@ -440,15 +440,14 @@
 
     unique_sum = range_union(ranges)
     raw_sum = sum(x.span for x in beds)
     return unique_sum if unique else raw_sum
 
 
 def main():
-
     actions = (
         ("depth", "calculate average depth per feature using coverageBed"),
         ("mergebydepth", "returns union of features beyond certain depth"),
         ("sort", "sort bed file"),
         ("merge", "merge bed files"),
         ("index", "index bed file using tabix"),
         ("bins", "bin bed lengths into each window"),
@@ -475,19 +474,81 @@
         ("alignextend", "alignextend based on BEDPE and FASTA ref"),
         ("clr", "extract clear range based on BEDPE"),
         ("chain", "chain bed segments together"),
         ("density", "calculates density of features per seqid"),
         ("tiling", "compute the minimum tiling path"),
         ("format", "reformat BED file"),
         ("closest", "find closest BED feature"),
+        ("gaps", "define gaps in BED file using complementBed"),
     )
     p = ActionDispatcher(actions)
     p.dispatch(globals())
 
 
+def gaps(args):
+    """
+    %prog gaps bedfile reference.fasta
+
+    This is used to define gaps in BED file using complementBed. One use case is
+    to define gaps in a BED file that was derived from a pairwise BLAST, for
+    example between two genomes. The reference.fasta is the reference genome.
+    The bedfile contains 'covered' features by BLAST hits, while the output
+    bedfile will contain 'uncovered' (i.e. gap) features, in that case use
+    --missing to note if gap is missing in one or more seqids.
+    """
+    from pybedtools import BedTool
+
+    p = OptionParser(gaps.__doc__)
+    p.add_option(
+        "--na_in",
+        help="Add '_na_in_xxx' to gap name, use comma to separate, "
+        + "e.g. --na_in=chr1,chr2 to note if gap is missing in chr1 or "
+        + "chr2, default is to not add anything. Note that if one of the "
+        + "missing seqids happens to be the seqid of the current feature, "
+        + "it will not be reported.",
+    )
+    p.add_option("--minsize", default=1000, type="int", help="Minimum gap size")
+    p.set_outfile()
+    opts, args = p.parse_args(args)
+
+    if len(args) != 2:
+        sys.exit(not p.print_help())
+
+    inputbed, ref_fasta = args
+    ref_sizes = Sizes(ref_fasta).mapping
+    minsize = opts.minsize
+    fw = must_open(opts.outfile, "w")
+    na_in = set(opts.na_in.split(",")) if opts.na_in else set()
+    comp = BedTool(inputbed).complement(genome=ref_fasta, L=True, stream=True)
+    n_gaps = 0
+    all_gaps = defaultdict(list)
+    for f in comp:
+        seqid = f[0]
+        start = f[1]
+        end = f[2]
+        size = int(end) - int(start)
+        if size < minsize:
+            continue
+        all_gaps[seqid].append(size)
+        gap_name = f"{seqid}_{start}_L{size}"
+        miss = "_".join(na_in - set([seqid]))
+        if miss:
+            gap_name += f"_na_in_{miss}"
+        print("\t".join((seqid, start, end, gap_name)), file=fw)
+        n_gaps += 1
+    for seqid, gap_sizes in all_gaps.items():
+        total_gap_size = sum(gap_sizes)
+        logging.debug(
+            "Total gaps in %s: %d, %s",
+            seqid,
+            len(gap_sizes),
+            percentage(total_gap_size, ref_sizes[seqid]),
+        )
+
+
 def closest(args):
     """
     %prog closest input.bed features.bed
 
     Find the closest feature in `features.bed` to `input.bed`.
     `features.bed` must be sorted using `jcvi.formats.bed sort`.
     """
@@ -1504,15 +1565,14 @@
         a = np.zeros(nbins)  # values
         b = np.zeros(nbins, dtype="int")  # bases
         c = np.zeros(nbins, dtype="int")  # count
         b[:-1] = binsize
         b[-1] = last_bin
 
         for bb in subbeds:
-
             start, end = bb.start, bb.end
             startbin = start / binsize
             endbin = end / binsize
 
             assert startbin <= endbin
             c[startbin : endbin + 1] += 1
 
@@ -1631,15 +1691,24 @@
 
     if need_update([bedfile, fastafile], outfile):
         sh(cmd, outfile=outfile)
 
     return outfile
 
 
-def mergeBed(bedfile, d=0, sorted=False, nms=False, s=False, scores=None, delim=";"):
+def mergeBed(
+    bedfile: str,
+    d: int = 0,
+    sorted: bool = False,
+    nms: bool = False,
+    s: bool = False,
+    scores: Optional[str] = None,
+    delim: str = ";",
+    inplace: bool = False,
+):
     if not sorted:
         bedfile = sort([bedfile, "-i"])
     cmd = "mergeBed -i {0}".format(bedfile)
     if d:
         cmd += " -d {0}".format(d)
     if nms:
         nargs = len(open(bedfile).readline().split())
@@ -1660,22 +1729,25 @@
             "antimode",
             "collapse",
         )
         if scores not in valid_opts:
             scores = "mean"
         cmd += " -scores {0}".format(scores)
 
-    if delim:
+    if nms and delim:
         cmd += ' -delim "{0}"'.format(delim)
 
     pf = bedfile.rsplit(".", 1)[0] if bedfile.endswith(".bed") else bedfile
     mergebedfile = op.basename(pf) + ".merge.bed"
 
     if need_update(bedfile, mergebedfile):
         sh(cmd, outfile=mergebedfile)
+
+    if inplace:
+        shutil.move(mergebedfile, bedfile)
     return mergebedfile
 
 
 def complementBed(bedfile, sizesfile):
     cmd = "complementBed"
     cmd += " -i {0} -g {1}".format(bedfile, sizesfile)
     complementbedfile = "complement_" + op.basename(bedfile)
```

### Comparing `jcvi-1.3.5/jcvi/formats/blast.py` & `jcvi-1.3.6/jcvi/formats/blast.py`

 * *Files 1% similar despite different names*

```diff
@@ -1257,29 +1257,35 @@
 def bed(args):
     """
     %prog bed blastfile
 
     Print out bed file based on coordinates in BLAST report. By default, write
     out subject positions. Use --swap to write query positions.
     """
-    from jcvi.formats.bed import sort as bed_sort
+    from .bed import sort as bed_sort, mergeBed
 
     p = OptionParser(bed.__doc__)
     p.add_option(
         "--swap",
         default=False,
         action="store_true",
         help="Write query positions",
     )
     p.add_option(
         "--both",
         default=False,
         action="store_true",
         help="Generate one line for each of query and subject",
     )
+    p.add_option(
+        "--merge",
+        default=None,
+        type="int",
+        help="Merge hits within this distance",
+    )
 
     opts, args = p.parse_args(args)
 
     if len(args) != 1:
         sys.exit(p.print_help())
 
     (blastfile,) = args
@@ -1299,14 +1305,16 @@
             print(b.bedline, file=fw)
         if negative:
             print(b.swapped.bedline, file=fw)
 
     logging.debug("File written to `%s`.", bedfile)
     fw.close()
     bed_sort([bedfile, "-i"])
+    if opts.merge:
+        mergeBed(bedfile, sorted=True, d=opts.merge, inplace=True)
 
     return bedfile
 
 
 def pairs(args):
     """
     See __doc__ for OptionParser.set_pairs().
```

### Comparing `jcvi-1.3.5/jcvi/formats/cblast.pyx` & `jcvi-1.3.6/jcvi/formats/cblast.pyx`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.5/jcvi/formats/cdt.py` & `jcvi-1.3.6/jcvi/formats/cdt.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.5/jcvi/formats/chain.py` & `jcvi-1.3.6/jcvi/formats/chain.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.5/jcvi/formats/contig.py` & `jcvi-1.3.6/jcvi/formats/contig.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.5/jcvi/formats/coords.py` & `jcvi-1.3.6/jcvi/formats/coords.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.5/jcvi/formats/excel.py` & `jcvi-1.3.6/jcvi/formats/excel.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.5/jcvi/formats/fasta.py` & `jcvi-1.3.6/jcvi/formats/fasta.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.5/jcvi/formats/fastq.py` & `jcvi-1.3.6/jcvi/formats/fastq.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.5/jcvi/formats/genbank.py` & `jcvi-1.3.6/jcvi/formats/genbank.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.5/jcvi/formats/gff.py` & `jcvi-1.3.6/jcvi/formats/gff.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.5/jcvi/formats/html.py` & `jcvi-1.3.6/jcvi/formats/html.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.5/jcvi/formats/maf.py` & `jcvi-1.3.6/jcvi/formats/maf.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.5/jcvi/formats/obo.py` & `jcvi-1.3.6/jcvi/formats/obo.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.5/jcvi/formats/paf.py` & `jcvi-1.3.6/jcvi/formats/paf.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.5/jcvi/formats/pdf.py` & `jcvi-1.3.6/jcvi/formats/pdf.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.5/jcvi/formats/psl.py` & `jcvi-1.3.6/jcvi/formats/psl.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.5/jcvi/formats/pyblast.py` & `jcvi-1.3.6/jcvi/formats/pyblast.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.5/jcvi/formats/sam.py` & `jcvi-1.3.6/jcvi/formats/sam.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.5/jcvi/formats/sizes.py` & `jcvi-1.3.6/jcvi/formats/sizes.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.5/jcvi/formats/vcf.py` & `jcvi-1.3.6/jcvi/formats/vcf.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.5/jcvi/graphics/align.py` & `jcvi-1.3.6/jcvi/graphics/align.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.5/jcvi/graphics/assembly.py` & `jcvi-1.3.6/jcvi/graphics/assembly.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.5/jcvi/graphics/base.py` & `jcvi-1.3.6/jcvi/graphics/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,15 +71,15 @@
 
 
 class ImageOptions(object):
     def __init__(self, opts):
         self.w, self.h = [int(x) for x in opts.figsize.split("x")]
         self.dpi = opts.dpi
         self.format = opts.format
-        self.cmap = cm.get_cmap(opts.cmap)
+        self.cmap = mpl.colormaps[opts.cmap]
         self.seed = opts.seed
         self.usetex = is_tex_available() and not opts.notex
         self.opts = opts
 
     def __str__(self):
         return "({0}px x {1}px)".format(self.dpi * self.w, self.dpi * self.h)
```

### Comparing `jcvi-1.3.5/jcvi/graphics/blastplot.py` & `jcvi-1.3.6/jcvi/graphics/blastplot.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.5/jcvi/graphics/chromosome.py` & `jcvi-1.3.6/jcvi/graphics/chromosome.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.5/jcvi/graphics/coverage.py` & `jcvi-1.3.6/jcvi/graphics/coverage.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.5/jcvi/graphics/dotplot.py` & `jcvi-1.3.6/jcvi/graphics/dotplot.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.5/jcvi/graphics/glyph.py` & `jcvi-1.3.6/jcvi/graphics/glyph.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.5/jcvi/graphics/grabseeds.py` & `jcvi-1.3.6/jcvi/graphics/grabseeds.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.5/jcvi/graphics/graph.py` & `jcvi-1.3.6/jcvi/graphics/graph.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.5/jcvi/graphics/heatmap.py` & `jcvi-1.3.6/jcvi/graphics/heatmap.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.5/jcvi/graphics/histogram.py` & `jcvi-1.3.6/jcvi/graphics/histogram.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.5/jcvi/graphics/karyotype.py` & `jcvi-1.3.6/jcvi/graphics/karyotype.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.5/jcvi/graphics/landscape.py` & `jcvi-1.3.6/jcvi/graphics/landscape.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.5/jcvi/graphics/logo.py` & `jcvi-1.3.6/jcvi/graphics/logo.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.5/jcvi/graphics/mummerplot.py` & `jcvi-1.3.6/jcvi/graphics/mummerplot.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.5/jcvi/graphics/synteny.py` & `jcvi-1.3.6/jcvi/graphics/synteny.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.5/jcvi/graphics/table.py` & `jcvi-1.3.6/jcvi/graphics/table.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.5/jcvi/graphics/tree.py` & `jcvi-1.3.6/jcvi/graphics/tree.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.5/jcvi/graphics/wheel.py` & `jcvi-1.3.6/jcvi/graphics/wheel.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.5/jcvi/graphics/whisker.py` & `jcvi-1.3.6/jcvi/graphics/whisker.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.5/jcvi/projects/age.py` & `jcvi-1.3.6/jcvi/projects/age.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.5/jcvi/projects/alfalfa.py` & `jcvi-1.3.6/jcvi/projects/alfalfa.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.5/jcvi/projects/allmaps.py` & `jcvi-1.3.6/jcvi/projects/allmaps.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.5/jcvi/projects/bites.py` & `jcvi-1.3.6/jcvi/projects/bites.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.5/jcvi/projects/heterosis.py` & `jcvi-1.3.6/jcvi/projects/heterosis.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.5/jcvi/projects/ies.py` & `jcvi-1.3.6/jcvi/projects/ies.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.5/jcvi/projects/misc.py` & `jcvi-1.3.6/jcvi/projects/misc.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.5/jcvi/projects/napus.py` & `jcvi-1.3.6/jcvi/projects/napus.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.5/jcvi/projects/pineapple.py` & `jcvi-1.3.6/jcvi/projects/pineapple.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.5/jcvi/projects/pistachio.py` & `jcvi-1.3.6/jcvi/projects/pistachio.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.5/jcvi/projects/str.py` & `jcvi-1.3.6/jcvi/projects/str.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.5/jcvi/projects/sugarcane.py` & `jcvi-1.3.6/jcvi/projects/sugarcane.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.5/jcvi/projects/synfind.py` & `jcvi-1.3.6/jcvi/projects/synfind.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.5/jcvi/projects/tgbs.py` & `jcvi-1.3.6/jcvi/projects/tgbs.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.5/jcvi/projects/vanilla.py` & `jcvi-1.3.6/jcvi/projects/vanilla.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.5/jcvi/utils/aws.py` & `jcvi-1.3.6/jcvi/utils/aws.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.5/jcvi/utils/cbook.py` & `jcvi-1.3.6/jcvi/utils/cbook.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.5/jcvi/utils/data/Airswing.ttf` & `jcvi-1.3.6/jcvi/utils/data/Airswing.ttf`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.5/jcvi/utils/data/Collegia.ttf` & `jcvi-1.3.6/jcvi/utils/data/Collegia.ttf`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.5/jcvi/utils/data/HookedUp.ttf` & `jcvi-1.3.6/jcvi/utils/data/HookedUp.ttf`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.5/jcvi/utils/data/Humor-Sans.ttf` & `jcvi-1.3.6/jcvi/utils/data/Humor-Sans.ttf`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.5/jcvi/utils/data/TREDs.meta.csv` & `jcvi-1.3.6/jcvi/utils/data/TREDs.meta.csv`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.5/jcvi/utils/data/adapters.fasta` & `jcvi-1.3.6/jcvi/utils/data/adapters.fasta`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.5/jcvi/utils/data/blosum80.mat` & `jcvi-1.3.6/jcvi/utils/data/blosum80.mat`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.5/jcvi/utils/data/chrY.hg38.unique_ccn.gc` & `jcvi-1.3.6/jcvi/utils/data/chrY.hg38.unique_ccn.gc`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.5/jcvi/utils/data/hg38.band.txt` & `jcvi-1.3.6/jcvi/utils/data/hg38.band.txt`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.5/jcvi/utils/data/hg38.chrom.sizes` & `jcvi-1.3.6/jcvi/utils/data/hg38.chrom.sizes`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.5/jcvi/utils/data/instance.json` & `jcvi-1.3.6/jcvi/utils/data/instance.json`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.5/jcvi/utils/db.py` & `jcvi-1.3.6/jcvi/utils/db.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.5/jcvi/utils/ez_setup.py` & `jcvi-1.3.6/jcvi/utils/ez_setup.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.5/jcvi/utils/grouper.py` & `jcvi-1.3.6/jcvi/utils/grouper.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.5/jcvi/utils/orderedcollections.py` & `jcvi-1.3.6/jcvi/utils/orderedcollections.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.5/jcvi/utils/range.py` & `jcvi-1.3.6/jcvi/utils/range.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.5/jcvi/utils/table.py` & `jcvi-1.3.6/jcvi/utils/table.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.5/jcvi/utils/taxonomy.py` & `jcvi-1.3.6/jcvi/utils/taxonomy.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.5/jcvi/utils/validator.py` & `jcvi-1.3.6/jcvi/utils/validator.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.5/jcvi/utils/webcolors.py` & `jcvi-1.3.6/jcvi/utils/webcolors.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.5/jcvi/variation/cnv.py` & `jcvi-1.3.6/jcvi/variation/cnv.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.5/jcvi/variation/deconvolute.py` & `jcvi-1.3.6/jcvi/variation/deconvolute.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.5/jcvi/variation/delly.py` & `jcvi-1.3.6/jcvi/variation/delly.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.5/jcvi/variation/impute.py` & `jcvi-1.3.6/jcvi/variation/impute.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.5/jcvi/variation/phase.py` & `jcvi-1.3.6/jcvi/variation/phase.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.5/jcvi/variation/snp.py` & `jcvi-1.3.6/jcvi/variation/snp.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.5/jcvi/variation/str.py` & `jcvi-1.3.6/jcvi/variation/str.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.5/jcvi/variation/tassel.py` & `jcvi-1.3.6/jcvi/variation/tassel.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.5/jcvi.egg-info/PKG-INFO` & `jcvi-1.3.6/jcvi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jcvi
-Version: 1.3.5
+Version: 1.3.6
 Summary: Python utility libraries on genome assembly, annotation and comparative genomics
 Home-page: http://github.com/tanghaibao/jcvi
 Author: Haibao Tang, Vivek Krishnakumar, Jingping Li
 Author-email: tanghaibao@gmail.com
 License: BSD
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `jcvi-1.3.5/jcvi.egg-info/SOURCES.txt` & `jcvi-1.3.6/jcvi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jcvi-1.3.5/setup.cfg` & `jcvi-1.3.6/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -53,13 +53,13 @@
 	pybedtools
 	rich
 	scikit-image
 	scipy
 	seaborn
 	webcolors
 include_package_data = True
-tests_require = PyYAML; pytest; pytest-cov; pytest-benchmark
+tests_require = PyYAML; pytest; pytest-cov; pytest-benchmark; mock
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `jcvi-1.3.5/setup.py` & `jcvi-1.3.6/setup.py`

 * *Files identical despite different names*

