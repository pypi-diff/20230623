# Comparing `tmp/econpizza-0.5.6.tar.gz` & `tmp/econpizza-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "econpizza-0.5.6.tar", last modified: Sat May 27 12:37:03 2023, max compression
+gzip compressed data, was "econpizza-0.6.0.tar", last modified: Fri Jun 23 09:41:45 2023, max compression
```

## Comparing `econpizza-0.5.6.tar` & `econpizza-0.6.0.tar`

### file list

```diff
@@ -1,90 +1,90 @@
-drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-05-27 12:37:03.754157 econpizza-0.5.6/
-drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-05-27 12:37:03.744156 econpizza-0.5.6/.github/
-drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-05-27 12:37:03.744156 econpizza-0.5.6/.github/workflows/
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1527 2023-04-15 12:29:25.000000 econpizza-0.5.6/.github/workflows/continuous-integration.yml
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)      173 2023-03-17 19:22:56.000000 econpizza-0.5.6/.gitignore
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)      287 2023-03-19 10:47:42.000000 econpizza-0.5.6/.pre-commit-config.yaml
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)      599 2023-03-22 13:14:47.000000 econpizza-0.5.6/.readthedocs.yaml
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1079 2023-03-02 09:28:46.000000 econpizza-0.5.6/LICENSE
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     3887 2023-05-27 12:37:03.754157 econpizza-0.5.6/PKG-INFO
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     3409 2023-05-27 12:18:41.000000 econpizza-0.5.6/README.rst
-drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-05-27 12:37:03.747490 econpizza-0.5.6/docs/
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)      634 2023-03-02 09:28:46.000000 econpizza-0.5.6/docs/Makefile
-drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-05-27 12:37:03.744156 econpizza-0.5.6/docs/_static/
-drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-05-27 12:37:03.747490 econpizza-0.5.6/docs/_static/css/
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)       55 2023-03-02 09:28:46.000000 econpizza-0.5.6/docs/_static/css/custom.css
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1551 2023-05-02 19:15:35.000000 econpizza-0.5.6/docs/conf.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)      331 2023-03-22 14:25:19.000000 econpizza-0.5.6/docs/content.rst
-drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-05-27 12:37:03.747490 econpizza-0.5.6/docs/guide/
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1759 2023-05-10 07:25:07.000000 econpizza-0.5.6/docs/guide/installation.rst
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     8245 2023-03-22 11:47:43.000000 econpizza-0.5.6/docs/guide/method.ipynb
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     2606 2023-05-07 18:36:01.000000 econpizza-0.5.6/docs/guide/solution.rst
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     2161 2023-05-07 18:29:06.000000 econpizza-0.5.6/docs/guide/steady_state.rst
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)    14328 2023-05-02 15:47:57.000000 econpizza-0.5.6/docs/guide/the_yaml.rst
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     2420 2023-05-27 12:18:06.000000 econpizza-0.5.6/docs/index.rst
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)    58150 2023-03-02 09:28:46.000000 econpizza-0.5.6/docs/lin_and_nlin.png
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)      800 2023-03-02 09:28:46.000000 econpizza-0.5.6/docs/make.bat
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)    22585 2023-03-02 09:28:46.000000 econpizza-0.5.6/docs/p_and_n.png
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)       80 2023-03-30 19:10:44.000000 econpizza-0.5.6/docs/requirements.txt
-drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-05-27 12:37:03.747490 econpizza-0.5.6/docs/tutorial/
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     2954 2023-03-10 20:34:11.000000 econpizza-0.5.6/docs/tutorial/boehl_hommes.rst
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)   389792 2023-03-23 23:03:36.000000 econpizza-0.5.6/docs/tutorial/hank1.ipynb
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)   234012 2023-03-22 12:13:19.000000 econpizza-0.5.6/docs/tutorial/hank2.ipynb
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)    63713 2023-03-22 11:52:34.000000 econpizza-0.5.6/docs/tutorial/quickstart.ipynb
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)   407267 2023-03-22 12:01:00.000000 econpizza-0.5.6/docs/tutorial/rank.ipynb
-drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-05-27 12:37:03.750823 econpizza-0.5.6/econpizza/
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     3547 2023-03-28 11:53:45.000000 econpizza-0.5.6/econpizza/__init__.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)       47 2023-05-27 12:36:57.000000 econpizza-0.5.6/econpizza/__version__.py
-drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-05-27 12:37:03.750823 econpizza-0.5.6/econpizza/examples/
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)      446 2023-03-25 22:11:17.000000 econpizza-0.5.6/econpizza/examples/__init__.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)      770 2023-03-02 09:28:46.000000 econpizza-0.5.6/econpizza/examples/bh.yml
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     7086 2023-05-27 12:24:35.000000 econpizza-0.5.6/econpizza/examples/dsge.yml
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     4857 2023-03-25 10:04:56.000000 econpizza-0.5.6/econpizza/examples/ghls.yml
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     8709 2023-03-24 20:08:58.000000 econpizza-0.5.6/econpizza/examples/hank2.yml
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     5559 2023-03-14 23:49:18.000000 econpizza-0.5.6/econpizza/examples/hank2_functions.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     6656 2023-03-26 20:12:16.000000 econpizza-0.5.6/econpizza/examples/hank2_no_capital.yml
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1652 2023-05-13 03:15:20.000000 econpizza-0.5.6/econpizza/examples/hank_functions.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     3716 2023-03-24 20:09:04.000000 econpizza-0.5.6/econpizza/examples/hank_labor.yml
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     3373 2023-03-15 14:58:36.000000 econpizza-0.5.6/econpizza/examples/hank_labor_functions.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     6137 2023-03-24 20:09:14.000000 econpizza-0.5.6/econpizza/examples/hank_with_comments.yml
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1550 2023-04-11 07:59:18.000000 econpizza-0.5.6/econpizza/examples/nk.yml
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     5512 2023-03-02 09:28:46.000000 econpizza-0.5.6/econpizza/examples/tank.yml
-drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-05-27 12:37:03.754157 econpizza-0.5.6/econpizza/parser/
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)    12187 2023-05-13 03:38:34.000000 econpizza-0.5.6/econpizza/parser/__init__.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     8145 2023-03-20 23:57:24.000000 econpizza-0.5.6/econpizza/parser/build_functions.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     4728 2023-04-21 09:07:56.000000 econpizza-0.5.6/econpizza/parser/checks.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     3237 2023-03-18 14:35:53.000000 econpizza-0.5.6/econpizza/parser/het_agent_base_funcs.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     4337 2023-05-12 08:16:06.000000 econpizza-0.5.6/econpizza/parser/write_dynamic_functions.py
-drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-05-27 12:37:03.754157 econpizza-0.5.6/econpizza/solvers/
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     6472 2023-03-10 20:34:11.000000 econpizza-0.5.6/econpizza/solvers/shooting.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     2789 2023-03-18 09:32:31.000000 econpizza-0.5.6/econpizza/solvers/solve_linear.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     4889 2023-03-10 20:34:11.000000 econpizza-0.5.6/econpizza/solvers/solve_linear_state_space.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     6278 2023-05-16 14:17:55.000000 econpizza-0.5.6/econpizza/solvers/stacking.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     8561 2023-05-05 14:50:38.000000 econpizza-0.5.6/econpizza/solvers/steady_state.py
-drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-05-27 12:37:03.754157 econpizza-0.5.6/econpizza/testing/
-drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-05-27 12:37:03.754157 econpizza-0.5.6/econpizza/testing/cache/
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1760 2023-03-14 23:53:28.000000 econpizza-0.5.6/econpizza/testing/cache/bh.npy
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     7064 2023-03-14 23:54:36.000000 econpizza-0.5.6/econpizza/testing/cache/hank_labor.npy
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     2984 2023-03-14 23:55:47.000000 econpizza-0.5.6/econpizza/testing/cache/hank_solid.npy
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)      429 2023-04-20 15:35:27.000000 econpizza-0.5.6/econpizza/testing/test_nb_hank1.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)      429 2023-04-20 15:44:49.000000 econpizza-0.5.6/econpizza/testing/test_nb_hank2.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)      421 2023-03-18 09:32:45.000000 econpizza-0.5.6/econpizza/testing/test_nb_quickstart.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)      415 2023-03-18 09:32:45.000000 econpizza-0.5.6/econpizza/testing/test_nb_rank.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)      414 2023-03-18 09:32:45.000000 econpizza-0.5.6/econpizza/testing/test_nb_under_the_hood.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1883 2023-05-10 08:08:46.000000 econpizza-0.5.6/econpizza/testing/test_rest.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)      940 2023-03-10 20:34:11.000000 econpizza-0.5.6/econpizza/tools.py
-drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-05-27 12:37:03.754157 econpizza-0.5.6/econpizza/utilities/
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     3391 2023-03-18 14:36:19.000000 econpizza-0.5.6/econpizza/utilities/dists.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     4185 2023-04-27 11:18:13.000000 econpizza-0.5.6/econpizza/utilities/grids.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     4769 2023-05-04 15:35:28.000000 econpizza-0.5.6/econpizza/utilities/interp.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     4173 2023-03-30 22:34:43.000000 econpizza-0.5.6/econpizza/utilities/jacobian.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     6395 2023-05-09 11:21:21.000000 econpizza-0.5.6/econpizza/utilities/newton.py
-drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-05-27 12:37:03.750823 econpizza-0.5.6/econpizza.egg-info/
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     3887 2023-05-27 12:37:03.000000 econpizza-0.5.6/econpizza.egg-info/PKG-INFO
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     2060 2023-05-27 12:37:03.000000 econpizza-0.5.6/econpizza.egg-info/SOURCES.txt
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)        1 2023-05-27 12:37:03.000000 econpizza-0.5.6/econpizza.egg-info/dependency_links.txt
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)       77 2023-05-27 12:37:03.000000 econpizza-0.5.6/econpizza.egg-info/requires.txt
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)       10 2023-05-27 12:37:03.000000 econpizza-0.5.6/econpizza.egg-info/top_level.txt
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)      147 2023-05-10 08:01:31.000000 econpizza-0.5.6/requirements.txt
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)       38 2023-05-27 12:37:03.754157 econpizza-0.5.6/setup.cfg
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1330 2023-04-15 12:24:22.000000 econpizza-0.5.6/setup.py
+drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-06-23 09:41:45.324484 econpizza-0.6.0/
+drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-06-23 09:41:45.301151 econpizza-0.6.0/.github/
+drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-06-23 09:41:45.304484 econpizza-0.6.0/.github/workflows/
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1316 2023-06-23 09:24:38.000000 econpizza-0.6.0/.github/workflows/continuous-integration.yml
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)      173 2023-03-17 19:22:56.000000 econpizza-0.6.0/.gitignore
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)      287 2023-03-19 10:47:42.000000 econpizza-0.6.0/.pre-commit-config.yaml
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)      599 2023-03-22 13:14:47.000000 econpizza-0.6.0/.readthedocs.yaml
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1079 2023-03-02 09:28:46.000000 econpizza-0.6.0/LICENSE
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     3994 2023-06-23 09:41:45.324484 econpizza-0.6.0/PKG-INFO
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     3516 2023-06-23 09:29:36.000000 econpizza-0.6.0/README.rst
+drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-06-23 09:41:45.307818 econpizza-0.6.0/docs/
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)      634 2023-03-02 09:28:46.000000 econpizza-0.6.0/docs/Makefile
+drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-06-23 09:41:45.301151 econpizza-0.6.0/docs/_static/
+drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-06-23 09:41:45.307818 econpizza-0.6.0/docs/_static/css/
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)       55 2023-03-02 09:28:46.000000 econpizza-0.6.0/docs/_static/css/custom.css
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1551 2023-05-02 19:15:35.000000 econpizza-0.6.0/docs/conf.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)      331 2023-03-22 14:25:19.000000 econpizza-0.6.0/docs/content.rst
+drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-06-23 09:41:45.307818 econpizza-0.6.0/docs/guide/
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)      564 2023-06-23 09:37:08.000000 econpizza-0.6.0/docs/guide/installation.rst
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     8245 2023-03-22 11:47:43.000000 econpizza-0.6.0/docs/guide/method.ipynb
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     2606 2023-05-07 18:36:01.000000 econpizza-0.6.0/docs/guide/solution.rst
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     2161 2023-05-07 18:29:06.000000 econpizza-0.6.0/docs/guide/steady_state.rst
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)    14328 2023-05-02 15:47:57.000000 econpizza-0.6.0/docs/guide/the_yaml.rst
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     2420 2023-05-27 12:18:06.000000 econpizza-0.6.0/docs/index.rst
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)    58150 2023-03-02 09:28:46.000000 econpizza-0.6.0/docs/lin_and_nlin.png
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)      800 2023-03-02 09:28:46.000000 econpizza-0.6.0/docs/make.bat
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)    22585 2023-03-02 09:28:46.000000 econpizza-0.6.0/docs/p_and_n.png
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)       80 2023-03-30 19:10:44.000000 econpizza-0.6.0/docs/requirements.txt
+drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-06-23 09:41:45.311151 econpizza-0.6.0/docs/tutorial/
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     2954 2023-03-10 20:34:11.000000 econpizza-0.6.0/docs/tutorial/boehl_hommes.rst
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)   389791 2023-06-06 14:13:17.000000 econpizza-0.6.0/docs/tutorial/hank1.ipynb
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)   234012 2023-03-22 12:13:19.000000 econpizza-0.6.0/docs/tutorial/hank2.ipynb
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)    63713 2023-03-22 11:52:34.000000 econpizza-0.6.0/docs/tutorial/quickstart.ipynb
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)   407267 2023-03-22 12:01:00.000000 econpizza-0.6.0/docs/tutorial/rank.ipynb
+drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-06-23 09:41:45.311151 econpizza-0.6.0/econpizza/
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     3547 2023-03-28 11:53:45.000000 econpizza-0.6.0/econpizza/__init__.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)       47 2023-06-23 09:40:38.000000 econpizza-0.6.0/econpizza/__version__.py
+drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-06-23 09:41:45.314484 econpizza-0.6.0/econpizza/examples/
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)      446 2023-03-25 22:11:17.000000 econpizza-0.6.0/econpizza/examples/__init__.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)      770 2023-03-02 09:28:46.000000 econpizza-0.6.0/econpizza/examples/bh.yml
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     7086 2023-05-27 12:24:35.000000 econpizza-0.6.0/econpizza/examples/dsge.yml
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     4857 2023-03-25 10:04:56.000000 econpizza-0.6.0/econpizza/examples/ghls.yml
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     8709 2023-03-24 20:08:58.000000 econpizza-0.6.0/econpizza/examples/hank2.yml
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     5559 2023-03-14 23:49:18.000000 econpizza-0.6.0/econpizza/examples/hank2_functions.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     6656 2023-03-26 20:12:16.000000 econpizza-0.6.0/econpizza/examples/hank2_no_capital.yml
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1652 2023-05-13 03:15:20.000000 econpizza-0.6.0/econpizza/examples/hank_functions.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     3716 2023-03-24 20:09:04.000000 econpizza-0.6.0/econpizza/examples/hank_labor.yml
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     3373 2023-03-15 14:58:36.000000 econpizza-0.6.0/econpizza/examples/hank_labor_functions.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     6137 2023-03-24 20:09:14.000000 econpizza-0.6.0/econpizza/examples/hank_with_comments.yml
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1550 2023-04-11 07:59:18.000000 econpizza-0.6.0/econpizza/examples/nk.yml
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     5512 2023-03-02 09:28:46.000000 econpizza-0.6.0/econpizza/examples/tank.yml
+drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-06-23 09:41:45.317818 econpizza-0.6.0/econpizza/parser/
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)    12187 2023-05-13 03:38:34.000000 econpizza-0.6.0/econpizza/parser/__init__.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     8145 2023-03-20 23:57:24.000000 econpizza-0.6.0/econpizza/parser/build_functions.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     4728 2023-04-21 09:07:56.000000 econpizza-0.6.0/econpizza/parser/checks.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     3237 2023-03-18 14:35:53.000000 econpizza-0.6.0/econpizza/parser/het_agent_base_funcs.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     4337 2023-05-12 08:16:06.000000 econpizza-0.6.0/econpizza/parser/write_dynamic_functions.py
+drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-06-23 09:41:45.317818 econpizza-0.6.0/econpizza/solvers/
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     6472 2023-03-10 20:34:11.000000 econpizza-0.6.0/econpizza/solvers/shooting.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     2789 2023-03-18 09:32:31.000000 econpizza-0.6.0/econpizza/solvers/solve_linear.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     4889 2023-03-10 20:34:11.000000 econpizza-0.6.0/econpizza/solvers/solve_linear_state_space.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     6278 2023-05-16 14:17:55.000000 econpizza-0.6.0/econpizza/solvers/stacking.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     8561 2023-05-05 14:50:38.000000 econpizza-0.6.0/econpizza/solvers/steady_state.py
+drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-06-23 09:41:45.321151 econpizza-0.6.0/econpizza/testing/
+drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-06-23 09:41:45.321151 econpizza-0.6.0/econpizza/testing/cache/
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1760 2023-03-14 23:53:28.000000 econpizza-0.6.0/econpizza/testing/cache/bh.npy
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     7064 2023-03-14 23:54:36.000000 econpizza-0.6.0/econpizza/testing/cache/hank_labor.npy
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     2984 2023-03-14 23:55:47.000000 econpizza-0.6.0/econpizza/testing/cache/hank_solid.npy
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)      429 2023-04-20 15:35:27.000000 econpizza-0.6.0/econpizza/testing/test_nb_hank1.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)      429 2023-04-20 15:44:49.000000 econpizza-0.6.0/econpizza/testing/test_nb_hank2.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)      421 2023-03-18 09:32:45.000000 econpizza-0.6.0/econpizza/testing/test_nb_quickstart.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)      415 2023-03-18 09:32:45.000000 econpizza-0.6.0/econpizza/testing/test_nb_rank.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)      414 2023-03-18 09:32:45.000000 econpizza-0.6.0/econpizza/testing/test_nb_under_the_hood.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1883 2023-05-10 08:08:46.000000 econpizza-0.6.0/econpizza/testing/test_rest.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)      940 2023-03-10 20:34:11.000000 econpizza-0.6.0/econpizza/tools.py
+drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-06-23 09:41:45.324484 econpizza-0.6.0/econpizza/utilities/
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     3391 2023-03-18 14:36:19.000000 econpizza-0.6.0/econpizza/utilities/dists.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     4185 2023-04-27 11:18:13.000000 econpizza-0.6.0/econpizza/utilities/grids.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     4769 2023-05-04 15:35:28.000000 econpizza-0.6.0/econpizza/utilities/interp.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     4173 2023-03-30 22:34:43.000000 econpizza-0.6.0/econpizza/utilities/jacobian.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     6395 2023-05-09 11:21:21.000000 econpizza-0.6.0/econpizza/utilities/newton.py
+drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-06-23 09:41:45.311151 econpizza-0.6.0/econpizza.egg-info/
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     3994 2023-06-23 09:41:45.000000 econpizza-0.6.0/econpizza.egg-info/PKG-INFO
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     2060 2023-06-23 09:41:45.000000 econpizza-0.6.0/econpizza.egg-info/SOURCES.txt
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)        1 2023-06-23 09:41:45.000000 econpizza-0.6.0/econpizza.egg-info/dependency_links.txt
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)       81 2023-06-23 09:41:45.000000 econpizza-0.6.0/econpizza.egg-info/requires.txt
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)       10 2023-06-23 09:41:45.000000 econpizza-0.6.0/econpizza.egg-info/top_level.txt
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)      163 2023-06-23 09:12:01.000000 econpizza-0.6.0/requirements.txt
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)       38 2023-06-23 09:41:45.324484 econpizza-0.6.0/setup.cfg
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1334 2023-06-23 09:12:23.000000 econpizza-0.6.0/setup.py
```

### Comparing `econpizza-0.5.6/.github/workflows/continuous-integration.yml` & `econpizza-0.6.0/.github/workflows/continuous-integration.yml`

 * *Files 6% similar despite different names*

```diff
@@ -15,27 +15,22 @@
     name: Run tests for ${{ matrix.os }} on ${{ matrix.python-version }}
     runs-on: ${{ matrix.os }}
 
     strategy:
       fail-fast: False
       matrix:
         os: [ubuntu-latest, macos-latest, windows-latest]
-        python-version: ['3.8', '3.10']
+        python-version: ['3.9', '3.10', '3.11']
 
     steps:
     - uses: actions/checkout@v3
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v3
       with:
         python-version: ${{ matrix.python-version }}
-    - if: matrix.os == 'windows-latest'
-      name: Install jax
-      run: |
-        python -m pip install "jax[cpu]===0.3.25" -f https://whls.blob.core.windows.net/unstable/index.html --use-deprecated legacy-resolver
-
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         python -m pip install .
         # testing deps
         python -m pip install pytest
         python -m pip install testbook
```

### Comparing `econpizza-0.5.6/.readthedocs.yaml` & `econpizza-0.6.0/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.6/LICENSE` & `econpizza-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.6/PKG-INFO` & `econpizza-0.6.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: econpizza
-Version: 0.5.6
+Version: 0.6.0
 Summary: Solve nonlinear perfect foresight models with heterogeneous agents
 Home-page: https://github.com/gboehl/econpizza
 Author: Gregor Boehl
 Author-email: admin@gregorboehl.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -39,17 +39,24 @@
 
 The package builds heavily on `automatic differentiation <https://en.wikipedia.org/wiki/Automatic_differentiation>`_ via `JAX <https://jax.readthedocs.io/en/latest/notebooks/quickstart.html>`_.
 
 
 Documentation
 -------------
 
+Installing the `repository version <https://pypi.org/project/econpizza/>`_ from PyPi is as simple as typing
+
+.. code-block:: bash
+
+   pip install econpizza
+
+in your terminal or Anaconda Prompt.
+
 Guides and tutorials are provided on ReadTheDocs:
 
- * `Installation <https://econpizza.readthedocs.io/en/stable/guide/installation.html>`_
  * `User guide <https://econpizza.readthedocs.io/en/stable/index.html>`_
  * `Quickstart tutorial <https://econpizza.readthedocs.io/en/stable/tutorial/quickstart.html>`_
 
 Citation
 --------
 .. code-block:: bibtex
```

### Comparing `econpizza-0.5.6/README.rst` & `econpizza-0.6.0/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -24,17 +24,24 @@
 
 The package builds heavily on `automatic differentiation <https://en.wikipedia.org/wiki/Automatic_differentiation>`_ via `JAX <https://jax.readthedocs.io/en/latest/notebooks/quickstart.html>`_.
 
 
 Documentation
 -------------
 
+Installing the `repository version <https://pypi.org/project/econpizza/>`_ from PyPi is as simple as typing
+
+.. code-block:: bash
+
+   pip install econpizza
+
+in your terminal or Anaconda Prompt.
+
 Guides and tutorials are provided on ReadTheDocs:
 
- * `Installation <https://econpizza.readthedocs.io/en/stable/guide/installation.html>`_
  * `User guide <https://econpizza.readthedocs.io/en/stable/index.html>`_
  * `Quickstart tutorial <https://econpizza.readthedocs.io/en/stable/tutorial/quickstart.html>`_
 
 Citation
 --------
 .. code-block:: bibtex
```

### Comparing `econpizza-0.5.6/docs/Makefile` & `econpizza-0.6.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.6/docs/conf.py` & `econpizza-0.6.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.6/docs/guide/method.ipynb` & `econpizza-0.6.0/docs/guide/method.ipynb`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.6/docs/guide/solution.rst` & `econpizza-0.6.0/docs/guide/solution.rst`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.6/docs/guide/steady_state.rst` & `econpizza-0.6.0/docs/guide/steady_state.rst`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.6/docs/guide/the_yaml.rst` & `econpizza-0.6.0/docs/guide/the_yaml.rst`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.6/docs/index.rst` & `econpizza-0.6.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.6/docs/lin_and_nlin.png` & `econpizza-0.6.0/docs/lin_and_nlin.png`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.6/docs/make.bat` & `econpizza-0.6.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.6/docs/p_and_n.png` & `econpizza-0.6.0/docs/p_and_n.png`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.6/docs/tutorial/boehl_hommes.rst` & `econpizza-0.6.0/docs/tutorial/boehl_hommes.rst`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.6/docs/tutorial/hank1.ipynb` & `econpizza-0.6.0/docs/tutorial/hank1.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9996438746438746%*

 * *Differences: {"'cells'": "{38: {'source': {insert: [(1, 'Again, since these are shares of nodes on a log-grid "*

 * *            '(rather than true densities), the shares for larger values on the grid are '*

 * *            "overrepresented.')], delete: [1]}}}"}*

```diff
@@ -537,15 +537,15 @@
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "The graph shows that the discount factor shock (and the ZLB) mainly affects the wealth of the housholds which hold no or very few assets, giving incentive to hold more assets for a short period of time.\n",
-                "NAgain, since these are shares of nodes on a log-grid (rather than true densities), the shares for larger values on the grid are overrepresented."
+                "Again, since these are shares of nodes on a log-grid (rather than true densities), the shares for larger values on the grid are overrepresented."
             ]
         }
     ],
     "metadata": {
         "@webio": {
             "lastCommId": null,
             "lastKernelId": null
```

### Comparing `econpizza-0.5.6/docs/tutorial/hank2.ipynb` & `econpizza-0.6.0/docs/tutorial/hank2.ipynb`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.6/docs/tutorial/quickstart.ipynb` & `econpizza-0.6.0/docs/tutorial/quickstart.ipynb`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.6/docs/tutorial/rank.ipynb` & `econpizza-0.6.0/docs/tutorial/rank.ipynb`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.6/econpizza/__init__.py` & `econpizza-0.6.0/econpizza/__init__.py`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.6/econpizza/examples/bh.yml` & `econpizza-0.6.0/econpizza/examples/bh.yml`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.6/econpizza/examples/dsge.yml` & `econpizza-0.6.0/econpizza/examples/dsge.yml`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.6/econpizza/examples/ghls.yml` & `econpizza-0.6.0/econpizza/examples/ghls.yml`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.6/econpizza/examples/hank2.yml` & `econpizza-0.6.0/econpizza/examples/hank2.yml`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.6/econpizza/examples/hank2_functions.py` & `econpizza-0.6.0/econpizza/examples/hank2_functions.py`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.6/econpizza/examples/hank2_no_capital.yml` & `econpizza-0.6.0/econpizza/examples/hank2_no_capital.yml`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.6/econpizza/examples/hank_functions.py` & `econpizza-0.6.0/econpizza/examples/hank_functions.py`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.6/econpizza/examples/hank_labor.yml` & `econpizza-0.6.0/econpizza/examples/hank_labor.yml`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.6/econpizza/examples/hank_labor_functions.py` & `econpizza-0.6.0/econpizza/examples/hank_labor_functions.py`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.6/econpizza/examples/hank_with_comments.yml` & `econpizza-0.6.0/econpizza/examples/hank_with_comments.yml`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.6/econpizza/examples/nk.yml` & `econpizza-0.6.0/econpizza/examples/nk.yml`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.6/econpizza/examples/tank.yml` & `econpizza-0.6.0/econpizza/examples/tank.yml`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.6/econpizza/parser/__init__.py` & `econpizza-0.6.0/econpizza/parser/__init__.py`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.6/econpizza/parser/build_functions.py` & `econpizza-0.6.0/econpizza/parser/build_functions.py`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.6/econpizza/parser/checks.py` & `econpizza-0.6.0/econpizza/parser/checks.py`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.6/econpizza/parser/het_agent_base_funcs.py` & `econpizza-0.6.0/econpizza/parser/het_agent_base_funcs.py`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.6/econpizza/parser/write_dynamic_functions.py` & `econpizza-0.6.0/econpizza/parser/write_dynamic_functions.py`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.6/econpizza/solvers/shooting.py` & `econpizza-0.6.0/econpizza/solvers/shooting.py`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.6/econpizza/solvers/solve_linear.py` & `econpizza-0.6.0/econpizza/solvers/solve_linear.py`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.6/econpizza/solvers/solve_linear_state_space.py` & `econpizza-0.6.0/econpizza/solvers/solve_linear_state_space.py`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.6/econpizza/solvers/stacking.py` & `econpizza-0.6.0/econpizza/solvers/stacking.py`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.6/econpizza/solvers/steady_state.py` & `econpizza-0.6.0/econpizza/solvers/steady_state.py`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.6/econpizza/testing/cache/bh.npy` & `econpizza-0.6.0/econpizza/testing/cache/bh.npy`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.6/econpizza/testing/cache/hank_labor.npy` & `econpizza-0.6.0/econpizza/testing/cache/hank_labor.npy`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.6/econpizza/testing/cache/hank_solid.npy` & `econpizza-0.6.0/econpizza/testing/cache/hank_solid.npy`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.6/econpizza/testing/test_rest.py` & `econpizza-0.6.0/econpizza/testing/test_rest.py`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.6/econpizza/tools.py` & `econpizza-0.6.0/econpizza/tools.py`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.6/econpizza/utilities/dists.py` & `econpizza-0.6.0/econpizza/utilities/dists.py`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.6/econpizza/utilities/grids.py` & `econpizza-0.6.0/econpizza/utilities/grids.py`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.6/econpizza/utilities/interp.py` & `econpizza-0.6.0/econpizza/utilities/interp.py`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.6/econpizza/utilities/jacobian.py` & `econpizza-0.6.0/econpizza/utilities/jacobian.py`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.6/econpizza/utilities/newton.py` & `econpizza-0.6.0/econpizza/utilities/newton.py`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.6/econpizza.egg-info/PKG-INFO` & `econpizza-0.6.0/econpizza.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: econpizza
-Version: 0.5.6
+Version: 0.6.0
 Summary: Solve nonlinear perfect foresight models with heterogeneous agents
 Home-page: https://github.com/gboehl/econpizza
 Author: Gregor Boehl
 Author-email: admin@gregorboehl.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -39,17 +39,24 @@
 
 The package builds heavily on `automatic differentiation <https://en.wikipedia.org/wiki/Automatic_differentiation>`_ via `JAX <https://jax.readthedocs.io/en/latest/notebooks/quickstart.html>`_.
 
 
 Documentation
 -------------
 
+Installing the `repository version <https://pypi.org/project/econpizza/>`_ from PyPi is as simple as typing
+
+.. code-block:: bash
+
+   pip install econpizza
+
+in your terminal or Anaconda Prompt.
+
 Guides and tutorials are provided on ReadTheDocs:
 
- * `Installation <https://econpizza.readthedocs.io/en/stable/guide/installation.html>`_
  * `User guide <https://econpizza.readthedocs.io/en/stable/index.html>`_
  * `Quickstart tutorial <https://econpizza.readthedocs.io/en/stable/tutorial/quickstart.html>`_
 
 Citation
 --------
 .. code-block:: bibtex
```

### Comparing `econpizza-0.5.6/econpizza.egg-info/SOURCES.txt` & `econpizza-0.6.0/econpizza.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.6/setup.py` & `econpizza-0.6.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,14 +30,14 @@
     packages=['econpizza', 'econpizza.parser',
               'econpizza.utilities', 'econpizza.solvers'],
     package_data={"econpizza": ["examples/*"]},
     extras_require={
         'linear': ['grgrlib>=0.1.22'],
     },
     install_requires=[
-        "jax<0.4.6",
-        "jaxlib<0.4.6",
+        "jax>=0.4.13",
+        "jaxlib>=0.4.13",
         "grgrjax>=0.4.3",
         "pyyaml",
         "scipy",
     ],
 )
```

