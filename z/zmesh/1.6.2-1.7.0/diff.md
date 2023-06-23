# Comparing `tmp/zmesh-1.6.2.tar.gz` & `tmp/zmesh-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zmesh-1.6.2.tar", last modified: Tue Feb 14 22:40:45 2023, max compression
+gzip compressed data, was "zmesh-1.7.0.tar", last modified: Fri Jun 23 06:57:49 2023, max compression
```

## Comparing `zmesh-1.6.2.tar` & `zmesh-1.7.0.tar`

### file list

```diff
@@ -1,453 +1,452 @@
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-02-14 22:40:45.847563 zmesh-1.6.2/
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-02-14 22:40:45.746772 zmesh-1.6.2/.github/
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-02-14 22:40:45.760256 zmesh-1.6.2/.github/workflows/
--rw-r--r--   0 wms        (501) staff       (20)      696 2022-12-16 18:26:49.000000 zmesh-1.6.2/.github/workflows/build_wheels.yml
--rw-r--r--   0 wms        (501) staff       (20)      854 2022-09-24 16:18:58.000000 zmesh-1.6.2/.github/workflows/test.yml
--rw-r--r--   0 wms        (501) staff       (20)      176 2023-02-14 22:40:43.000000 zmesh-1.6.2/AUTHORS
--rw-r--r--   0 wms        (501) staff       (20)     5122 2023-02-14 22:40:43.000000 zmesh-1.6.2/ChangeLog
--rw-r--r--   0 wms        (501) staff       (20)     1567 2021-10-08 19:53:42.000000 zmesh-1.6.2/Dockerfile
--rw-r--r--   0 wms        (501) staff       (20)    35149 2021-01-20 02:40:15.000000 zmesh-1.6.2/LICENSE
--rw-r--r--   0 wms        (501) staff       (20)       74 2022-09-20 17:11:36.000000 zmesh-1.6.2/MANIFEST.in
--rw-r--r--   0 wms        (501) staff       (20)     5065 2023-02-14 22:40:45.847742 zmesh-1.6.2/PKG-INFO
--rw-r--r--   0 wms        (501) staff       (20)     3905 2022-12-16 18:26:49.000000 zmesh-1.6.2/README.md
--rw-r--r--   0 wms        (501) staff       (20)     6749 2023-02-14 22:22:20.000000 zmesh-1.6.2/automated_test.py
--rwxr-xr-x   0 wms        (501) staff       (20)     4404 2022-12-16 00:12:51.000000 zmesh-1.6.2/cMesher.hpp
--rw-r--r--   0 wms        (501) staff       (20)       24 2022-09-20 17:11:39.000000 zmesh-1.6.2/dev_requirements.txt
--rw-r--r--   0 wms        (501) staff       (20)    46865 2022-12-16 18:26:49.000000 zmesh-1.6.2/fanc_bug.npy.gz
--rw-r--r--   0 wms        (501) staff       (20)     3637 2022-09-20 17:12:08.000000 zmesh-1.6.2/perf.py
--rw-r--r--   0 wms        (501) staff       (20)        5 2022-05-04 06:53:15.000000 zmesh-1.6.2/requirements.txt
--rw-r--r--   0 wms        (501) staff       (20)      433 2022-09-20 17:12:08.000000 zmesh-1.6.2/sample.py
--rwxr-xr-x   0 wms        (501) staff       (20)     1097 2023-02-14 22:40:45.848419 zmesh-1.6.2/setup.cfg
--rwxr-xr-x   0 wms        (501) staff       (20)      930 2023-02-14 22:25:19.000000 zmesh-1.6.2/setup.py
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-02-14 22:40:45.760918 zmesh-1.6.2/templates/
--rw-r--r--   0 wms        (501) staff       (20)     1006 2022-09-20 17:11:39.000000 zmesh-1.6.2/templates/mesherclass.j2
--rw-r--r--   0 wms        (501) staff       (20)      276 2022-01-28 03:38:36.000000 zmesh-1.6.2/templates/rendertemplate.py
--rw-r--r--   0 wms        (501) staff       (20)      402 2022-09-02 02:50:28.000000 zmesh-1.6.2/test.py
--rw-r--r--   0 wms        (501) staff       (20)      241 2022-12-16 18:26:49.000000 zmesh-1.6.2/tox.ini
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-02-14 22:40:45.761249 zmesh-1.6.2/zi_lib/
--rwxr-xr-x   0 wms        (501) staff       (20)    35147 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/gpl-3.0.txt
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-02-14 22:40:45.771146 zmesh-1.6.2/zi_lib/zi/
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-02-14 22:40:45.771678 zmesh-1.6.2/zi_lib/zi/ai/
--rwxr-xr-x   0 wms        (501) staff       (20)     8796 2022-09-24 16:18:58.000000 zmesh-1.6.2/zi_lib/zi/ai/decision_tree.hpp
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-02-14 22:40:45.772723 zmesh-1.6.2/zi_lib/zi/ai/detail/
--rwxr-xr-x   0 wms        (501) staff       (20)     1775 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/ai/detail/entropy.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     7189 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/ai/detail/gini_maximizing_splitter.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     6975 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/ai/detail/information_gain_splitter.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     2809 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/ai/detail/mmdt_splitter.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     6374 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/ai/random_forest.hpp
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-02-14 22:40:45.773654 zmesh-1.6.2/zi_lib/zi/ansi_term/
--rwxr-xr-x   0 wms        (501) staff       (20)     2172 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/ansi_term/constants.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     6586 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/ansi_term/flags.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     1706 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/ansi_term/tags.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     4633 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/ansi_term/term_ostream.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)      883 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/ansi_term.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)      872 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/arguments.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)      863 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/array.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)      867 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/assert.hpp
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-02-14 22:40:45.774700 zmesh-1.6.2/zi_lib/zi/atomic/
--rwxr-xr-x   0 wms        (501) staff       (20)     1514 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/atomic/atomic.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     1577 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/atomic/config.hpp
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-02-14 22:40:45.777000 zmesh-1.6.2/zi_lib/zi/atomic/detail/
--rwxr-xr-x   0 wms        (501) staff       (20)     3024 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/atomic/detail/atomic_gcc_i386.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     2651 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/atomic/detail/atomic_gcc_ppc.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     2233 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/atomic/detail/atomic_gcc_sync.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     2983 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/atomic/detail/atomic_gcc_x64.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     2354 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/atomic/detail/atomic_win32.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     1242 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/atomic/detail/fenced_block_gcc_sync.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     1409 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/atomic/detail/fenced_block_gcc_x86.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     1170 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/atomic/detail/fenced_block_macos.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     1341 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/atomic/detail/fenced_block_win32.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     1831 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/atomic/fenced_block.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     1048 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/atomic/spinlock.hpp
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-02-14 22:40:45.777215 zmesh-1.6.2/zi_lib/zi/atomic/test/
--rwxr-xr-x   0 wms        (501) staff       (20)     2026 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/atomic/test/atomic_test.cpp
--rwxr-xr-x   0 wms        (501) staff       (20)      881 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/binary_heap.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)      860 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/bind.hpp
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-02-14 22:40:45.781059 zmesh-1.6.2/zi_lib/zi/bits/
--rwxr-xr-x   0 wms        (501) staff       (20)     1053 2022-09-24 16:18:58.000000 zmesh-1.6.2/zi_lib/zi/bits/array.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     1862 2022-09-24 16:18:58.000000 zmesh-1.6.2/zi_lib/zi/bits/bind.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     4686 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/bits/cerrno.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     2256 2022-09-24 16:18:58.000000 zmesh-1.6.2/zi_lib/zi/bits/cstdint.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     1130 2022-09-24 16:18:58.000000 zmesh-1.6.2/zi_lib/zi/bits/enable_shared_from_this.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     1127 2022-09-24 16:18:58.000000 zmesh-1.6.2/zi_lib/zi/bits/function.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     1114 2022-09-24 16:18:58.000000 zmesh-1.6.2/zi_lib/zi/bits/hash.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     1032 2022-09-24 16:18:58.000000 zmesh-1.6.2/zi_lib/zi/bits/mem_fn.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     1861 2022-09-24 16:18:58.000000 zmesh-1.6.2/zi_lib/zi/bits/random.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     1087 2022-09-24 16:18:58.000000 zmesh-1.6.2/zi_lib/zi/bits/ref.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     1050 2022-09-24 16:18:58.000000 zmesh-1.6.2/zi_lib/zi/bits/result_of.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     1097 2022-09-24 16:18:58.000000 zmesh-1.6.2/zi_lib/zi/bits/shared_ptr.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     1234 2022-09-24 16:18:58.000000 zmesh-1.6.2/zi_lib/zi/bits/tuple.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     4224 2022-09-24 16:18:58.000000 zmesh-1.6.2/zi_lib/zi/bits/type_traits.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)      956 2022-09-24 16:18:58.000000 zmesh-1.6.2/zi_lib/zi/bits/typeof.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     1199 2022-09-24 16:18:58.000000 zmesh-1.6.2/zi_lib/zi/bits/unordered_map.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     1171 2022-09-24 16:18:58.000000 zmesh-1.6.2/zi_lib/zi/bits/unordered_set.hpp
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-02-14 22:40:45.783475 zmesh-1.6.2/zi_lib/zi/cache/
--rwxr-xr-x   0 wms        (501) staff       (20)     3430 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/cache/cache_container.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     1212 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/cache/cache_fwd.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)      898 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/cache/config.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     4665 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/cache/container.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     3430 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/cache/container_fwd.hpp
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-02-14 22:40:45.786255 zmesh-1.6.2/zi_lib/zi/cache/detail/
--rwxr-xr-x   0 wms        (501) staff       (20)     3430 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/cache/detail/container_base.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     3664 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/cache/detail/container_entry.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     1691 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/cache/detail/default_constructor.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)      903 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/cache/detail/enable_if.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     1508 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/cache/detail/if.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     2337 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/cache/detail/key_extractors.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     1357 2022-09-24 16:18:58.000000 zmesh-1.6.2/zi_lib/zi/cache/detail/multi_index.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)      882 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/cache/detail/ref.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     6004 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/cache/detail/storage_base.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     2408 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/cache/detail/storage_entry.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)      906 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/cache/detail/type_traits.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     1027 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/cache/detail/yes_no_type.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     4764 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/cache/global_function.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     2789 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/cache/identity.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     2699 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/cache/member_function.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     3309 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/cache/member_variable.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)      975 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/cache/tags.hpp
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-02-14 22:40:45.787107 zmesh-1.6.2/zi_lib/zi/cache/test/
--rwxr-xr-x   0 wms        (501) staff       (20)    12562 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/cache/test/container_test._cc
--rwxr-xr-x   0 wms        (501) staff       (20)     5304 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/cache/test/key_extractors_test.cpp
--rwxr-xr-x   0 wms        (501) staff       (20)     1239 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/cache/test/key_extractors_test.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     3827 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/cache/test/member_function_test.cpp
--rwxr-xr-x   0 wms        (501) staff       (20)      865 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/cerrno.hpp
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-02-14 22:40:45.791376 zmesh-1.6.2/zi_lib/zi/concurrency/
--rwxr-xr-x   0 wms        (501) staff       (20)     1910 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/concurrency/barrier.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     1386 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/concurrency/concurrency.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     1238 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/concurrency/condition_variable.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     1524 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/concurrency/config.hpp
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-02-14 22:40:45.794249 zmesh-1.6.2/zi_lib/zi/concurrency/detail/
--rwxr-xr-x   0 wms        (501) staff       (20)     1480 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/concurrency/detail/all_threads.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     4136 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/concurrency/detail/all_threads_data.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     4368 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/concurrency/detail/is_mutex.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     2184 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/concurrency/detail/is_runnable.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     1458 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/concurrency/detail/mutex_guard.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     1987 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/concurrency/detail/mutex_pool.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     1088 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/concurrency/detail/mutex_tags.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     2810 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/concurrency/detail/priority_task_container.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     7862 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/concurrency/detail/rwmutex_impl.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     1192 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/concurrency/detail/simple_task_container.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     7614 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/concurrency/detail/task_manager_impl.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     2121 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/concurrency/detail/this_thread.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     6758 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/concurrency/detail/thread_info.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     1160 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/concurrency/event.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     3215 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/concurrency/guard.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     6537 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/concurrency/monitor.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     2827 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/concurrency/mutex.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)    25884 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/concurrency/periodic_function.hpp
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-02-14 22:40:45.796949 zmesh-1.6.2/zi_lib/zi/concurrency/pthread/
--rwxr-xr-x   0 wms        (501) staff       (20)     3536 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/concurrency/pthread/condition_variable.hpp
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-02-14 22:40:45.797207 zmesh-1.6.2/zi_lib/zi/concurrency/pthread/detail/
--rwxr-xr-x   0 wms        (501) staff       (20)     1312 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/concurrency/pthread/detail/this_thread.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     2070 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/concurrency/pthread/event.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     2859 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/concurrency/pthread/mutex_initializers.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)      929 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/concurrency/pthread/mutex_tags.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     2927 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/concurrency/pthread/mutex_tpl.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     1585 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/concurrency/pthread/mutex_types.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     1052 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/concurrency/pthread/rwmutex.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     2806 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/concurrency/pthread/rwmutex_using_pthread_rwlock_t.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     2073 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/concurrency/pthread/spinlock.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     3933 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/concurrency/pthread/thread.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     2130 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/concurrency/pthread/thread_attributes.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     1090 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/concurrency/pthread/types.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     2805 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/concurrency/runnable.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     2838 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/concurrency/rwmutex.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     3425 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/concurrency/semaphore.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     1167 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/concurrency/spinlock.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     2581 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/concurrency/state.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     7161 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/concurrency/task_manager.hpp
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-02-14 22:40:45.799027 zmesh-1.6.2/zi_lib/zi/concurrency/test/
--rwxr-xr-x   0 wms        (501) staff       (20)     1685 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/concurrency/test/barrier_test.cpp
--rwxr-xr-x   0 wms        (501) staff       (20)     6256 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/concurrency/test/condition_variable_test.cpp
--rwxr-xr-x   0 wms        (501) staff       (20)     2224 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/concurrency/test/event_test.cpp
--rwxr-xr-x   0 wms        (501) staff       (20)     5798 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/concurrency/test/mutex_test.cpp
--rwxr-xr-x   0 wms        (501) staff       (20)     3870 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/concurrency/test/periodic_function_test.cpp
--rwxr-xr-x   0 wms        (501) staff       (20)     2544 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/concurrency/test/rwmutex_test.cpp
--rwxr-xr-x   0 wms        (501) staff       (20)     2308 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/concurrency/test/semaphore_test.cpp
--rwxr-xr-x   0 wms        (501) staff       (20)     4489 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/concurrency/test/task_manager_test.cpp
--rwxr-xr-x   0 wms        (501) staff       (20)     1456 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/concurrency/thread.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     1726 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/concurrency/thread_types.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     3137 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/concurrency/trigger.hpp
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-02-14 22:40:45.802119 zmesh-1.6.2/zi_lib/zi/concurrency/win32/
--rwxr-xr-x   0 wms        (501) staff       (20)     4789 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/concurrency/win32/condition_variable.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     2119 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/concurrency/win32/default_mutex.hpp
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-02-14 22:40:45.802905 zmesh-1.6.2/zi_lib/zi/concurrency/win32/detail/
--rwxr-xr-x   0 wms        (501) staff       (20)     2631 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/concurrency/win32/detail/interlocked.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     1749 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/concurrency/win32/detail/primitives.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     1372 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/concurrency/win32/detail/this_thread.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     2048 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/concurrency/win32/event.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)      925 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/concurrency/win32/mutex_tags.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     1504 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/concurrency/win32/mutex_tpl.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     1187 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/concurrency/win32/mutex_types.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     3066 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/concurrency/win32/recursive_mutex.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)      923 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/concurrency/win32/rwmutex.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     2030 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/concurrency/win32/spinlock.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     2935 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/concurrency/win32/spinlock_fast.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     3942 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/concurrency/win32/thread.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     1148 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/concurrency/win32/types.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)      888 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/concurrency.hpp
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-02-14 22:40:45.803338 zmesh-1.6.2/zi_lib/zi/config/
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-02-14 22:40:45.803727 zmesh-1.6.2/zi_lib/zi/config/compiler/
--rwxr-xr-x   0 wms        (501) staff       (20)      853 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/config/compiler/gcc.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)      855 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/config/compiler/msvc.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     1776 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/config/config.hpp
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-02-14 22:40:45.804430 zmesh-1.6.2/zi_lib/zi/config/os/
--rwxr-xr-x   0 wms        (501) staff       (20)     1121 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/config/os/linux.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)      967 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/config/os/macos.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     1170 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/config/os/windows.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     1261 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/config/posix.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)      869 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/cstdint.hpp
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-02-14 22:40:45.805193 zmesh-1.6.2/zi_lib/zi/debug/
--rwxr-xr-x   0 wms        (501) staff       (20)      882 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/debug/assert.hpp
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-02-14 22:40:45.805426 zmesh-1.6.2/zi_lib/zi/debug/detail/
--rwxr-xr-x   0 wms        (501) staff       (20)     2057 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/debug/detail/demangle.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     1279 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/debug/printable_type.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     2048 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/debug/printable_value.hpp
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-02-14 22:40:45.806296 zmesh-1.6.2/zi_lib/zi/detail/
--rwxr-xr-x   0 wms        (501) staff       (20)     4593 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/detail/global_function.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     2735 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/detail/identity.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     2596 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/detail/member_function.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     2816 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/detail/member_variable.hpp
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-02-14 22:40:45.806512 zmesh-1.6.2/zi_lib/zi/disjoint_sets/
--rwxr-xr-x   0 wms        (501) staff       (20)     3637 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/disjoint_sets/disjoint_sets.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)      917 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/enable_shared_from_this.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)      929 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/enable_singleton_from_this.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)      874 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/for_each.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)      872 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/function.hpp
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-02-14 22:40:45.808778 zmesh-1.6.2/zi_lib/zi/gl/
--rwxr-xr-x   0 wms        (501) staff       (20)     9858 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/gl/camera.hpp
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-02-14 22:40:45.809883 zmesh-1.6.2/zi_lib/zi/gl/detail/
--rwxr-xr-x   0 wms        (501) staff       (20)     1321 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/gl/detail/config.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     1029 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/gl/detail/gl_prefix.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)      977 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/gl/detail/gl_suffix.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     1476 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/gl/detail/types.hpp
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-02-14 22:40:45.810119 zmesh-1.6.2/zi_lib/zi/gl/example/
--rwxr-xr-x   0 wms        (501) staff       (20)     4467 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/gl/example/example.cpp
--rwxr-xr-x   0 wms        (501) staff       (20)    56229 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/gl/gl.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     6982 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/gl/gl_1_1.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     4924 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/gl/gl_1_2.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)    13448 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/gl/gl_1_3.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)    10024 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/gl/gl_arb_imaging.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)    17823 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/gl/glu.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)    19644 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/gl/glut.hpp
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-02-14 22:40:45.810611 zmesh-1.6.2/zi_lib/zi/graph/
--rwxr-xr-x   0 wms        (501) staff       (20)     5607 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/graph/bipartite_matching.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     4694 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/graph/strongly_connected_components.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)      860 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/hash.hpp
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-02-14 22:40:45.811084 zmesh-1.6.2/zi_lib/zi/heap/
--rwxr-xr-x   0 wms        (501) staff       (20)     4047 2022-09-24 15:51:55.000000 zmesh-1.6.2/zi_lib/zi/heap/binary_heap.hpp
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-02-14 22:40:45.811538 zmesh-1.6.2/zi_lib/zi/heap/detail/
--rwxr-xr-x   0 wms        (501) staff       (20)    10983 2022-09-24 16:18:58.000000 zmesh-1.6.2/zi_lib/zi/heap/detail/binary_heap_impl.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     5950 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/heap/detail/binary_heap_impl2.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     5415 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/heap/simple_binary_heap.hpp
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-02-14 22:40:45.811991 zmesh-1.6.2/zi_lib/zi/heap/test/
--rwxr-xr-x   0 wms        (501) staff       (20)     4084 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/heap/test/binary_heap_test.cpp
--rwxr-xr-x   0 wms        (501) staff       (20)     3440 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/heap/test/simple_binary_heap_test.cpp
--rwxr-xr-x   0 wms        (501) staff       (20)      866 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/logging.hpp
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-02-14 22:40:45.812917 zmesh-1.6.2/zi_lib/zi/math/
--rwxr-xr-x   0 wms        (501) staff       (20)     7917 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/math/bit_reverse.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     9007 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/math/constants.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     2925 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/math/fast_log.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     2217 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/math/integral_log2.hpp
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-02-14 22:40:45.750866 zmesh-1.6.2/zi_lib/zi/math/transforms/
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-02-14 22:40:45.814307 zmesh-1.6.2/zi_lib/zi/math/transforms/detail/
--rwxr-xr-x   0 wms        (501) staff       (20)     5394 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/math/transforms/detail/fft8.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     6336 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/math/transforms/detail/fft_radix2.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     4271 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/math/transforms/detail/fft_splitradix.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     4722 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/math/transforms/detail/permuter.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     3536 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/math/transforms/detail/roots_table.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     1642 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/math/transforms/detail/size_log2.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)      866 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/mem_fn.hpp
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-02-14 22:40:45.816198 zmesh-1.6.2/zi_lib/zi/mesh/
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-02-14 22:40:45.818080 zmesh-1.6.2/zi_lib/zi/mesh/detail/
--rw-r--r--   0 wms        (501) staff       (20)     1844 2022-09-24 16:25:01.000000 zmesh-1.6.2/zi_lib/zi/mesh/detail/all_equal.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)    21023 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/mesh/detail/marching_cubes_tables.hpp
--rw-r--r--   0 wms        (501) staff       (20)    19148 2022-09-20 17:12:08.000000 zmesh-1.6.2/zi_lib/zi/mesh/detail/mc_tables.hpp
--rw-r--r--   0 wms        (501) staff       (20)     4607 2022-09-20 17:12:08.000000 zmesh-1.6.2/zi_lib/zi/mesh/detail/packed_coordinate.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     9633 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/mesh/detail/qmetric.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)    10719 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/mesh/detail/quadratic.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     7524 2022-09-20 17:12:08.000000 zmesh-1.6.2/zi_lib/zi/mesh/detail/tri_mesh_edge.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)    10044 2022-09-20 17:12:08.000000 zmesh-1.6.2/zi_lib/zi/mesh/detail/tri_mesh_face.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     1923 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/mesh/detail/tri_mesh_vertex.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     7118 2022-09-24 16:18:58.000000 zmesh-1.6.2/zi_lib/zi/mesh/face_mesh.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     4467 2022-09-24 16:18:58.000000 zmesh-1.6.2/zi_lib/zi/mesh/int_mesh.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)    13499 2022-12-16 18:26:49.000000 zmesh-1.6.2/zi_lib/zi/mesh/marching_cubes.hpp
--rw-r--r--   0 wms        (501) staff       (20)     3631 2022-09-20 17:12:08.000000 zmesh-1.6.2/zi_lib/zi/mesh/network_sort.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)    25282 2022-09-20 17:12:08.000000 zmesh-1.6.2/zi_lib/zi/mesh/quadratic_simplifier.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     5872 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/mesh/tri_list.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)    15072 2022-09-20 17:12:08.000000 zmesh-1.6.2/zi_lib/zi/mesh/tri_mesh.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)    11185 2022-09-19 22:57:33.000000 zmesh-1.6.2/zi_lib/zi/mesh/tri_stripper.hpp
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-02-14 22:40:45.819948 zmesh-1.6.2/zi_lib/zi/meta/
--rwxr-xr-x   0 wms        (501) staff       (20)     1423 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/meta/and.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     1141 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/meta/bool.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     1877 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/meta/enable_if.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     1018 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/meta/false_type.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     1429 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/meta/if.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     1049 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/meta/meta.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     1005 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/meta/null_type.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     1866 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/meta/or.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     1013 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/meta/true_type.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)      906 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/mutex.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)      887 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/non_copyable.hpp
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-02-14 22:40:45.820396 zmesh-1.6.2/zi_lib/zi/parallel/
--rwxr-xr-x   0 wms        (501) staff       (20)     2659 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/parallel/algorithm.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     1323 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/parallel/numeric.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)      866 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/random.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)      857 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/ref.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)      875 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/result_of.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)      878 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/shared_ptr.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)      878 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/singleton.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)      890 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/static_assert.hpp
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-02-14 22:40:45.821220 zmesh-1.6.2/zi_lib/zi/system/
--rwxr-xr-x   0 wms        (501) staff       (20)     1573 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/system/config.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     2219 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/system/daemon.hpp
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-02-14 22:40:45.822971 zmesh-1.6.2/zi_lib/zi/system/detail/
--rwxr-xr-x   0 wms        (501) staff       (20)     4536 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/system/detail/cerrno_code.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     1386 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/system/detail/cpu_count.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     1639 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/system/detail/get_hostname.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     1521 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/system/detail/get_username.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     3297 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/system/detail/linux_errno_code.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     2485 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/system/detail/memory_size.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     2606 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/system/detail/memory_usage.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     3193 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/system/detail/win32_errno_code.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     1294 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/system/error.hpp
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-02-14 22:40:45.823216 zmesh-1.6.2/zi_lib/zi/system/example/
--rwxr-xr-x   0 wms        (501) staff       (20)     5027 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/system/example/example.cpp
--rwxr-xr-x   0 wms        (501) staff       (20)     8169 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/system/system.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)      868 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/system.hpp
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-02-14 22:40:45.825230 zmesh-1.6.2/zi_lib/zi/test/
--rwxr-xr-x   0 wms        (501) staff       (20)      652 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/test/Makefile
--rwxr-xr-x   0 wms        (501) staff       (20)     2794 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/test/Makefile-include-mingw32
--rwxr-xr-x   0 wms        (501) staff       (20)     2889 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/test/Makefile-include-nix
--rwxr-xr-x   0 wms        (501) staff       (20)     2605 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/test/Makefile-include-wine
--rwxr-xr-x   0 wms        (501) staff       (20)      691 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/test/Makefile-mingw32
--rwxr-xr-x   0 wms        (501) staff       (20)      654 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/test/Makefile-nix-mingw32
--rwxr-xr-x   0 wms        (501) staff       (20)      672 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/test/Makefile-tmp
--rwxr-xr-x   0 wms        (501) staff       (20)     1400 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/test/Makefile-wine
--rwxr-xr-x   0 wms        (501) staff       (20)       29 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/test/main.cpp
--rwxr-xr-x   0 wms        (501) staff       (20)      862 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/test.hpp
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-02-14 22:40:45.827160 zmesh-1.6.2/zi_lib/zi/time/
--rwxr-xr-x   0 wms        (501) staff       (20)     1498 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/time/config.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     5963 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/time/interval.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     2894 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/time/now.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     3224 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/time/process_timer.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)      997 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/time/time.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     1764 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/time/time_units.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     3685 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/time/time_utils.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     2084 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/time/timer.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     3769 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/time/wall_timer.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)      860 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/time.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)      863 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/timer.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)      863 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/tuple.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)      881 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/type_traits.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)      866 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/typeof.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)      870 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/unittest.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)      887 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/unordered_map.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)      886 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/unordered_set.hpp
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-02-14 22:40:45.831678 zmesh-1.6.2/zi_lib/zi/utility/
--rwxr-xr-x   0 wms        (501) staff       (20)     1481 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/utility/address_of.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     1751 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/utility/assert.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     2510 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/utility/binary_printer.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     1056 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/utility/container_utilities.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     1665 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/utility/deferred_instantiation.hpp
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-02-14 22:40:45.833438 zmesh-1.6.2/zi_lib/zi/utility/detail/
--rwxr-xr-x   0 wms        (501) staff       (20)     1219 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/utility/detail/bare_type.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     1062 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/utility/detail/dummy.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)      973 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/utility/detail/empty_type.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     1402 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/utility/detail/get_instance.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     1783 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/utility/detail/nbyte_int.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     1054 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/utility/detail/not_this_type.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)      987 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/utility/detail/whatever.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     1009 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/utility/detail/yes_no_type.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     1973 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/utility/enable_if.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     1387 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/utility/enable_singleton_of_this.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     2330 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/utility/exception.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     2360 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/utility/for_each.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     1387 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/utility/is_complex.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     2417 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/utility/is_printable.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     4557 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/utility/natural_compare.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     1182 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/utility/non_copyable.hpp
--rw-r--r--   0 wms        (501) staff       (20)    94949 2022-09-20 17:12:08.000000 zmesh-1.6.2/zi_lib/zi/utility/robin_hood.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     1588 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/utility/singleton.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     1914 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/utility/static_and.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     1494 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/utility/static_assert.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     1371 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/utility/static_if.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     1940 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/utility/static_or.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     1748 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/utility/string_printf.hpp
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-02-14 22:40:45.834102 zmesh-1.6.2/zi_lib/zi/utility/test/
--rwxr-xr-x   0 wms        (501) staff       (20)     1517 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/utility/test/address_of_test.cpp
--rwxr-xr-x   0 wms        (501) staff       (20)     1788 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/utility/test/enable_if_test.cpp
--rwxr-xr-x   0 wms        (501) staff       (20)     4041 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/utility/test/is_printable_test.cpp
--rwxr-xr-x   0 wms        (501) staff       (20)     1349 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/utility/this_function.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     1830 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/utility/value_iterator.hpp
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-02-14 22:40:45.835519 zmesh-1.6.2/zi_lib/zi/vl/
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-02-14 22:40:45.836699 zmesh-1.6.2/zi_lib/zi/vl/detail/
--rwxr-xr-x   0 wms        (501) staff       (20)     2026 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/vl/detail/enable_if.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)    11929 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/vl/detail/householder.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     8484 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/vl/detail/invert.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     7182 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/vl/detail/jacobi.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     1726 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/vl/detail/mat_lookup_table.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     7894 2022-09-24 15:32:42.000000 zmesh-1.6.2/zi_lib/zi/vl/detail/promote.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)    37154 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/vl/mat.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)    14937 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/vl/mat_functions.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)    31314 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/vl/quat.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     9118 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/vl/quat_functions.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)    22196 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/vl/vec.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)    13509 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/vl/vec_functions.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)      910 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/vl/vl.hpp
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-02-14 22:40:45.837191 zmesh-1.6.2/zi_lib/zi/watershed/
--rwxr-xr-x   0 wms        (501) staff       (20)     3829 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/watershed/quickie.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)      942 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/watershed/watershed.hpp
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-02-14 22:40:45.837999 zmesh-1.6.2/zi_lib/zi/zargs/
--rwxr-xr-x   0 wms        (501) staff       (20)     4643 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/zargs/arguments.hpp
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-02-14 22:40:45.839038 zmesh-1.6.2/zi_lib/zi/zargs/detail/
--rwxr-xr-x   0 wms        (501) staff       (20)     1054 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/zargs/detail/boost_lexical_cast.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)      956 2022-09-24 16:18:58.000000 zmesh-1.6.2/zi_lib/zi/zargs/detail/lexical_cast.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     2847 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/zargs/detail/simple_lexical_cast.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     2521 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/zargs/detail/string_utils.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     2469 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/zargs/matcher.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     4025 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/zargs/parser.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)    11502 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/zargs/zargs.hpp
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-02-14 22:40:45.840442 zmesh-1.6.2/zi_lib/zi/zlog/
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-02-14 22:40:45.840880 zmesh-1.6.2/zi_lib/zi/zlog/example/
--rwxr-xr-x   0 wms        (501) staff       (20)     4845 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/zlog/example/example.cpp
--rwxr-xr-x   0 wms        (501) staff       (20)     1157 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/zlog/example/example_other.cpp
--rwxr-xr-x   0 wms        (501) staff       (20)     1835 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/zlog/log_printf.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     3775 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/zlog/logs.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     2276 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/zlog/registry.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     2015 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/zlog/sink.hpp
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-02-14 22:40:45.841081 zmesh-1.6.2/zi_lib/zi/zlog/test/
--rwxr-xr-x   0 wms        (501) staff       (20)     1557 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/zlog/test/token_sink_test.cpp
--rwxr-xr-x   0 wms        (501) staff       (20)     2190 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/zlog/token.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     7269 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/zlog/zlog.hpp
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-02-14 22:40:45.841656 zmesh-1.6.2/zi_lib/zi/zpp/
--rwxr-xr-x   0 wms        (501) staff       (20)     3756 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/zpp/count_args.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)      920 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/zpp/glue.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)      932 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/zpp/stringify.hpp
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-02-14 22:40:45.844381 zmesh-1.6.2/zi_lib/zi/zunit/
--rwxr-xr-x   0 wms        (501) staff       (20)     6176 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/zunit/checker.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)      879 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/zunit/config.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     4382 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/zunit/exception.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     7523 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/zunit/expect_xxx.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     5428 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/zunit/macros.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)      873 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/zunit/main.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     1022 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/zunit/main.ipp
--rwxr-xr-x   0 wms        (501) staff       (20)     1937 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/zunit/registry.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     1072 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/zunit/tags.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     1388 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/zunit/test_case.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     4382 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/zunit/test_suite.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)     1340 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/zunit/test_suite_tpl.hpp
--rwxr-xr-x   0 wms        (501) staff       (20)      979 2022-04-04 21:20:05.000000 zmesh-1.6.2/zi_lib/zi/zunit/zunit.hpp
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-02-14 22:40:45.846145 zmesh-1.6.2/zmesh/
--rw-r--r--   0 wms        (501) staff       (20)       78 2023-02-14 22:22:45.000000 zmesh-1.6.2/zmesh/__init__.py
--rw-r--r--   0 wms        (501) staff       (20)   962863 2022-12-16 18:26:49.000000 zmesh-1.6.2/zmesh/_zmesh.cpp
--rwxr-xr-x   0 wms        (501) staff       (20)    15441 2022-10-04 19:52:05.000000 zmesh-1.6.2/zmesh/_zmesh.pyx
--rw-r--r--   0 wms        (501) staff       (20)     6875 2023-02-14 19:41:50.000000 zmesh-1.6.2/zmesh/mesh.py
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-02-14 22:40:45.847390 zmesh-1.6.2/zmesh.egg-info/
--rw-r--r--   0 wms        (501) staff       (20)     5065 2023-02-14 22:40:43.000000 zmesh-1.6.2/zmesh.egg-info/PKG-INFO
--rw-r--r--   0 wms        (501) staff       (20)    12898 2023-02-14 22:40:45.000000 zmesh-1.6.2/zmesh.egg-info/SOURCES.txt
--rw-r--r--   0 wms        (501) staff       (20)        1 2023-02-14 22:40:43.000000 zmesh-1.6.2/zmesh.egg-info/dependency_links.txt
--rw-r--r--   0 wms        (501) staff       (20)        1 2021-01-20 02:44:29.000000 zmesh-1.6.2/zmesh.egg-info/not-zip-safe
--rw-r--r--   0 wms        (501) staff       (20)       46 2023-02-14 22:40:43.000000 zmesh-1.6.2/zmesh.egg-info/pbr.json
--rw-r--r--   0 wms        (501) staff       (20)        6 2023-02-14 22:40:43.000000 zmesh-1.6.2/zmesh.egg-info/requires.txt
--rw-r--r--   0 wms        (501) staff       (20)        6 2023-02-14 22:40:43.000000 zmesh-1.6.2/zmesh.egg-info/top_level.txt
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-06-23 06:57:49.374127 zmesh-1.7.0/
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-06-23 06:57:49.278706 zmesh-1.7.0/.github/
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-06-23 06:57:49.290108 zmesh-1.7.0/.github/workflows/
+-rw-r--r--   0 wms        (501) staff       (20)      696 2022-12-16 18:26:49.000000 zmesh-1.7.0/.github/workflows/build_wheels.yml
+-rw-r--r--   0 wms        (501) staff       (20)      854 2022-09-24 16:18:58.000000 zmesh-1.7.0/.github/workflows/test.yml
+-rw-r--r--   0 wms        (501) staff       (20)      176 2023-06-23 06:57:47.000000 zmesh-1.7.0/AUTHORS
+-rw-r--r--   0 wms        (501) staff       (20)     5228 2023-06-23 06:57:47.000000 zmesh-1.7.0/ChangeLog
+-rw-r--r--   0 wms        (501) staff       (20)     1567 2021-10-08 19:53:42.000000 zmesh-1.7.0/Dockerfile
+-rw-r--r--   0 wms        (501) staff       (20)    35149 2021-01-20 02:40:15.000000 zmesh-1.7.0/LICENSE
+-rw-r--r--   0 wms        (501) staff       (20)       74 2022-09-20 17:11:36.000000 zmesh-1.7.0/MANIFEST.in
+-rw-r--r--   0 wms        (501) staff       (20)     6180 2023-06-23 06:57:49.374310 zmesh-1.7.0/PKG-INFO
+-rw-r--r--   0 wms        (501) staff       (20)     4205 2023-06-23 06:46:57.000000 zmesh-1.7.0/README.md
+-rw-r--r--   0 wms        (501) staff       (20)     8803 2023-06-23 06:46:57.000000 zmesh-1.7.0/automated_test.py
+-rwxr-xr-x   0 wms        (501) staff       (20)     5441 2023-06-23 06:46:57.000000 zmesh-1.7.0/cMesher.hpp
+-rw-r--r--   0 wms        (501) staff       (20)       24 2022-09-20 17:11:39.000000 zmesh-1.7.0/dev_requirements.txt
+-rw-r--r--   0 wms        (501) staff       (20)    46865 2022-12-16 18:26:49.000000 zmesh-1.7.0/fanc_bug.npy.gz
+-rw-r--r--   0 wms        (501) staff       (20)     3637 2023-06-21 02:46:57.000000 zmesh-1.7.0/perf.py
+-rw-r--r--   0 wms        (501) staff       (20)        5 2022-05-04 06:53:15.000000 zmesh-1.7.0/requirements.txt
+-rw-r--r--   0 wms        (501) staff       (20)      433 2022-09-20 17:12:08.000000 zmesh-1.7.0/sample.py
+-rwxr-xr-x   0 wms        (501) staff       (20)     1097 2023-06-23 06:57:49.374791 zmesh-1.7.0/setup.cfg
+-rwxr-xr-x   0 wms        (501) staff       (20)      940 2023-06-23 06:46:57.000000 zmesh-1.7.0/setup.py
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-06-23 06:57:49.290632 zmesh-1.7.0/templates/
+-rw-r--r--   0 wms        (501) staff       (20)     1014 2023-06-23 06:46:57.000000 zmesh-1.7.0/templates/mesherclass.j2
+-rw-r--r--   0 wms        (501) staff       (20)      276 2023-06-20 22:12:55.000000 zmesh-1.7.0/templates/rendertemplate.py
+-rw-r--r--   0 wms        (501) staff       (20)      402 2022-09-02 02:50:28.000000 zmesh-1.7.0/test.py
+-rw-r--r--   0 wms        (501) staff       (20)      241 2022-12-16 18:26:49.000000 zmesh-1.7.0/tox.ini
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-06-23 06:57:49.290948 zmesh-1.7.0/zi_lib/
+-rwxr-xr-x   0 wms        (501) staff       (20)    35147 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/gpl-3.0.txt
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-06-23 06:57:49.299702 zmesh-1.7.0/zi_lib/zi/
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-06-23 06:57:49.300391 zmesh-1.7.0/zi_lib/zi/ai/
+-rwxr-xr-x   0 wms        (501) staff       (20)     8796 2022-09-24 16:18:58.000000 zmesh-1.7.0/zi_lib/zi/ai/decision_tree.hpp
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-06-23 06:57:49.301205 zmesh-1.7.0/zi_lib/zi/ai/detail/
+-rwxr-xr-x   0 wms        (501) staff       (20)     1775 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/ai/detail/entropy.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     7189 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/ai/detail/gini_maximizing_splitter.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     6975 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/ai/detail/information_gain_splitter.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     2809 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/ai/detail/mmdt_splitter.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     6374 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/ai/random_forest.hpp
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-06-23 06:57:49.302015 zmesh-1.7.0/zi_lib/zi/ansi_term/
+-rwxr-xr-x   0 wms        (501) staff       (20)     2172 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/ansi_term/constants.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     6586 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/ansi_term/flags.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     1706 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/ansi_term/tags.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     4633 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/ansi_term/term_ostream.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)      883 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/ansi_term.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)      872 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/arguments.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)      863 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/array.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)      867 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/assert.hpp
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-06-23 06:57:49.302792 zmesh-1.7.0/zi_lib/zi/atomic/
+-rwxr-xr-x   0 wms        (501) staff       (20)     1514 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/atomic/atomic.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     1577 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/atomic/config.hpp
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-06-23 06:57:49.304506 zmesh-1.7.0/zi_lib/zi/atomic/detail/
+-rwxr-xr-x   0 wms        (501) staff       (20)     3024 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/atomic/detail/atomic_gcc_i386.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     2651 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/atomic/detail/atomic_gcc_ppc.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     2233 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/atomic/detail/atomic_gcc_sync.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     2983 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/atomic/detail/atomic_gcc_x64.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     2354 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/atomic/detail/atomic_win32.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     1242 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/atomic/detail/fenced_block_gcc_sync.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     1409 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/atomic/detail/fenced_block_gcc_x86.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     1170 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/atomic/detail/fenced_block_macos.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     1341 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/atomic/detail/fenced_block_win32.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     1831 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/atomic/fenced_block.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     1048 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/atomic/spinlock.hpp
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-06-23 06:57:49.304710 zmesh-1.7.0/zi_lib/zi/atomic/test/
+-rwxr-xr-x   0 wms        (501) staff       (20)     2026 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/atomic/test/atomic_test.cpp
+-rwxr-xr-x   0 wms        (501) staff       (20)      881 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/binary_heap.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)      860 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/bind.hpp
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-06-23 06:57:49.308291 zmesh-1.7.0/zi_lib/zi/bits/
+-rwxr-xr-x   0 wms        (501) staff       (20)     1053 2022-09-24 16:18:58.000000 zmesh-1.7.0/zi_lib/zi/bits/array.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     1862 2022-09-24 16:18:58.000000 zmesh-1.7.0/zi_lib/zi/bits/bind.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     4686 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/bits/cerrno.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     2256 2022-09-24 16:18:58.000000 zmesh-1.7.0/zi_lib/zi/bits/cstdint.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     1130 2022-09-24 16:18:58.000000 zmesh-1.7.0/zi_lib/zi/bits/enable_shared_from_this.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     1127 2022-09-24 16:18:58.000000 zmesh-1.7.0/zi_lib/zi/bits/function.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     1114 2022-09-24 16:18:58.000000 zmesh-1.7.0/zi_lib/zi/bits/hash.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     1032 2022-09-24 16:18:58.000000 zmesh-1.7.0/zi_lib/zi/bits/mem_fn.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     1861 2022-09-24 16:18:58.000000 zmesh-1.7.0/zi_lib/zi/bits/random.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     1087 2022-09-24 16:18:58.000000 zmesh-1.7.0/zi_lib/zi/bits/ref.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     1050 2022-09-24 16:18:58.000000 zmesh-1.7.0/zi_lib/zi/bits/result_of.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     1097 2022-09-24 16:18:58.000000 zmesh-1.7.0/zi_lib/zi/bits/shared_ptr.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     1234 2022-09-24 16:18:58.000000 zmesh-1.7.0/zi_lib/zi/bits/tuple.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     4224 2022-09-24 16:18:58.000000 zmesh-1.7.0/zi_lib/zi/bits/type_traits.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)      956 2022-09-24 16:18:58.000000 zmesh-1.7.0/zi_lib/zi/bits/typeof.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     1199 2022-09-24 16:18:58.000000 zmesh-1.7.0/zi_lib/zi/bits/unordered_map.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     1171 2022-09-24 16:18:58.000000 zmesh-1.7.0/zi_lib/zi/bits/unordered_set.hpp
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-06-23 06:57:49.310416 zmesh-1.7.0/zi_lib/zi/cache/
+-rwxr-xr-x   0 wms        (501) staff       (20)     3430 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/cache/cache_container.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     1212 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/cache/cache_fwd.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)      898 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/cache/config.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     4665 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/cache/container.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     3430 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/cache/container_fwd.hpp
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-06-23 06:57:49.312731 zmesh-1.7.0/zi_lib/zi/cache/detail/
+-rwxr-xr-x   0 wms        (501) staff       (20)     3430 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/cache/detail/container_base.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     3664 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/cache/detail/container_entry.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     1691 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/cache/detail/default_constructor.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)      903 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/cache/detail/enable_if.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     1508 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/cache/detail/if.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     2337 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/cache/detail/key_extractors.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     1357 2022-09-24 16:18:58.000000 zmesh-1.7.0/zi_lib/zi/cache/detail/multi_index.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)      882 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/cache/detail/ref.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     6004 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/cache/detail/storage_base.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     2408 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/cache/detail/storage_entry.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)      906 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/cache/detail/type_traits.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     1027 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/cache/detail/yes_no_type.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     4764 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/cache/global_function.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     2789 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/cache/identity.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     2699 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/cache/member_function.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     3309 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/cache/member_variable.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)      975 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/cache/tags.hpp
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-06-23 06:57:49.313530 zmesh-1.7.0/zi_lib/zi/cache/test/
+-rwxr-xr-x   0 wms        (501) staff       (20)    12562 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/cache/test/container_test._cc
+-rwxr-xr-x   0 wms        (501) staff       (20)     5304 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/cache/test/key_extractors_test.cpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     1239 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/cache/test/key_extractors_test.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     3827 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/cache/test/member_function_test.cpp
+-rwxr-xr-x   0 wms        (501) staff       (20)      865 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/cerrno.hpp
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-06-23 06:57:49.317549 zmesh-1.7.0/zi_lib/zi/concurrency/
+-rwxr-xr-x   0 wms        (501) staff       (20)     1910 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/concurrency/barrier.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     1386 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/concurrency/concurrency.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     1238 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/concurrency/condition_variable.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     1524 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/concurrency/config.hpp
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-06-23 06:57:49.320244 zmesh-1.7.0/zi_lib/zi/concurrency/detail/
+-rwxr-xr-x   0 wms        (501) staff       (20)     1480 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/concurrency/detail/all_threads.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     4136 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/concurrency/detail/all_threads_data.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     4368 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/concurrency/detail/is_mutex.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     2184 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/concurrency/detail/is_runnable.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     1458 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/concurrency/detail/mutex_guard.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     1987 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/concurrency/detail/mutex_pool.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     1088 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/concurrency/detail/mutex_tags.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     2810 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/concurrency/detail/priority_task_container.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     7862 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/concurrency/detail/rwmutex_impl.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     1192 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/concurrency/detail/simple_task_container.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     7614 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/concurrency/detail/task_manager_impl.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     2121 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/concurrency/detail/this_thread.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     6758 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/concurrency/detail/thread_info.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     1160 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/concurrency/event.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     3215 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/concurrency/guard.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     6537 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/concurrency/monitor.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     2827 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/concurrency/mutex.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)    25884 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/concurrency/periodic_function.hpp
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-06-23 06:57:49.322560 zmesh-1.7.0/zi_lib/zi/concurrency/pthread/
+-rwxr-xr-x   0 wms        (501) staff       (20)     3536 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/concurrency/pthread/condition_variable.hpp
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-06-23 06:57:49.322745 zmesh-1.7.0/zi_lib/zi/concurrency/pthread/detail/
+-rwxr-xr-x   0 wms        (501) staff       (20)     1312 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/concurrency/pthread/detail/this_thread.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     2070 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/concurrency/pthread/event.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     2859 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/concurrency/pthread/mutex_initializers.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)      929 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/concurrency/pthread/mutex_tags.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     2927 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/concurrency/pthread/mutex_tpl.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     1585 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/concurrency/pthread/mutex_types.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     1052 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/concurrency/pthread/rwmutex.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     2806 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/concurrency/pthread/rwmutex_using_pthread_rwlock_t.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     2073 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/concurrency/pthread/spinlock.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     3933 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/concurrency/pthread/thread.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     2130 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/concurrency/pthread/thread_attributes.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     1090 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/concurrency/pthread/types.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     2805 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/concurrency/runnable.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     2838 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/concurrency/rwmutex.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     3425 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/concurrency/semaphore.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     1167 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/concurrency/spinlock.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     2581 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/concurrency/state.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     7161 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/concurrency/task_manager.hpp
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-06-23 06:57:49.324375 zmesh-1.7.0/zi_lib/zi/concurrency/test/
+-rwxr-xr-x   0 wms        (501) staff       (20)     1685 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/concurrency/test/barrier_test.cpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     6256 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/concurrency/test/condition_variable_test.cpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     2224 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/concurrency/test/event_test.cpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     5798 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/concurrency/test/mutex_test.cpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     3870 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/concurrency/test/periodic_function_test.cpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     2544 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/concurrency/test/rwmutex_test.cpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     2308 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/concurrency/test/semaphore_test.cpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     4489 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/concurrency/test/task_manager_test.cpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     1456 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/concurrency/thread.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     1726 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/concurrency/thread_types.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     3137 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/concurrency/trigger.hpp
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-06-23 06:57:49.327168 zmesh-1.7.0/zi_lib/zi/concurrency/win32/
+-rwxr-xr-x   0 wms        (501) staff       (20)     4789 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/concurrency/win32/condition_variable.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     2119 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/concurrency/win32/default_mutex.hpp
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-06-23 06:57:49.327833 zmesh-1.7.0/zi_lib/zi/concurrency/win32/detail/
+-rwxr-xr-x   0 wms        (501) staff       (20)     2631 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/concurrency/win32/detail/interlocked.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     1749 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/concurrency/win32/detail/primitives.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     1372 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/concurrency/win32/detail/this_thread.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     2048 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/concurrency/win32/event.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)      925 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/concurrency/win32/mutex_tags.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     1504 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/concurrency/win32/mutex_tpl.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     1187 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/concurrency/win32/mutex_types.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     3066 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/concurrency/win32/recursive_mutex.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)      923 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/concurrency/win32/rwmutex.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     2030 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/concurrency/win32/spinlock.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     2935 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/concurrency/win32/spinlock_fast.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     3942 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/concurrency/win32/thread.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     1148 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/concurrency/win32/types.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)      888 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/concurrency.hpp
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-06-23 06:57:49.328307 zmesh-1.7.0/zi_lib/zi/config/
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-06-23 06:57:49.328752 zmesh-1.7.0/zi_lib/zi/config/compiler/
+-rwxr-xr-x   0 wms        (501) staff       (20)      853 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/config/compiler/gcc.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)      855 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/config/compiler/msvc.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     1776 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/config/config.hpp
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-06-23 06:57:49.329411 zmesh-1.7.0/zi_lib/zi/config/os/
+-rwxr-xr-x   0 wms        (501) staff       (20)     1121 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/config/os/linux.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)      967 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/config/os/macos.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     1170 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/config/os/windows.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     1261 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/config/posix.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)      869 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/cstdint.hpp
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-06-23 06:57:49.330092 zmesh-1.7.0/zi_lib/zi/debug/
+-rwxr-xr-x   0 wms        (501) staff       (20)      882 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/debug/assert.hpp
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-06-23 06:57:49.330341 zmesh-1.7.0/zi_lib/zi/debug/detail/
+-rwxr-xr-x   0 wms        (501) staff       (20)     2057 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/debug/detail/demangle.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     1279 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/debug/printable_type.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     2048 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/debug/printable_value.hpp
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-06-23 06:57:49.331168 zmesh-1.7.0/zi_lib/zi/detail/
+-rwxr-xr-x   0 wms        (501) staff       (20)     4593 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/detail/global_function.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     2735 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/detail/identity.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     2596 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/detail/member_function.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     2816 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/detail/member_variable.hpp
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-06-23 06:57:49.331395 zmesh-1.7.0/zi_lib/zi/disjoint_sets/
+-rwxr-xr-x   0 wms        (501) staff       (20)     3637 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/disjoint_sets/disjoint_sets.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)      917 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/enable_shared_from_this.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)      929 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/enable_singleton_from_this.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)      874 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/for_each.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)      872 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/function.hpp
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-06-23 06:57:49.333567 zmesh-1.7.0/zi_lib/zi/gl/
+-rwxr-xr-x   0 wms        (501) staff       (20)     9858 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/gl/camera.hpp
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-06-23 06:57:49.334513 zmesh-1.7.0/zi_lib/zi/gl/detail/
+-rwxr-xr-x   0 wms        (501) staff       (20)     1321 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/gl/detail/config.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     1029 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/gl/detail/gl_prefix.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)      977 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/gl/detail/gl_suffix.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     1476 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/gl/detail/types.hpp
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-06-23 06:57:49.334710 zmesh-1.7.0/zi_lib/zi/gl/example/
+-rwxr-xr-x   0 wms        (501) staff       (20)     4467 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/gl/example/example.cpp
+-rwxr-xr-x   0 wms        (501) staff       (20)    56229 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/gl/gl.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     6982 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/gl/gl_1_1.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     4924 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/gl/gl_1_2.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)    13448 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/gl/gl_1_3.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)    10024 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/gl/gl_arb_imaging.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)    17823 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/gl/glu.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)    19644 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/gl/glut.hpp
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-06-23 06:57:49.335153 zmesh-1.7.0/zi_lib/zi/graph/
+-rwxr-xr-x   0 wms        (501) staff       (20)     5607 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/graph/bipartite_matching.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     4694 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/graph/strongly_connected_components.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)      860 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/hash.hpp
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-06-23 06:57:49.335635 zmesh-1.7.0/zi_lib/zi/heap/
+-rwxr-xr-x   0 wms        (501) staff       (20)     4047 2022-09-24 15:51:55.000000 zmesh-1.7.0/zi_lib/zi/heap/binary_heap.hpp
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-06-23 06:57:49.336140 zmesh-1.7.0/zi_lib/zi/heap/detail/
+-rwxr-xr-x   0 wms        (501) staff       (20)    10983 2022-09-24 16:18:58.000000 zmesh-1.7.0/zi_lib/zi/heap/detail/binary_heap_impl.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     5950 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/heap/detail/binary_heap_impl2.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     5415 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/heap/simple_binary_heap.hpp
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-06-23 06:57:49.336639 zmesh-1.7.0/zi_lib/zi/heap/test/
+-rwxr-xr-x   0 wms        (501) staff       (20)     4084 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/heap/test/binary_heap_test.cpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     3440 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/heap/test/simple_binary_heap_test.cpp
+-rwxr-xr-x   0 wms        (501) staff       (20)      866 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/logging.hpp
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-06-23 06:57:49.337658 zmesh-1.7.0/zi_lib/zi/math/
+-rwxr-xr-x   0 wms        (501) staff       (20)     7917 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/math/bit_reverse.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     9007 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/math/constants.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     2925 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/math/fast_log.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     2217 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/math/integral_log2.hpp
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-06-23 06:57:49.282139 zmesh-1.7.0/zi_lib/zi/math/transforms/
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-06-23 06:57:49.338995 zmesh-1.7.0/zi_lib/zi/math/transforms/detail/
+-rwxr-xr-x   0 wms        (501) staff       (20)     5394 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/math/transforms/detail/fft8.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     6336 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/math/transforms/detail/fft_radix2.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     4271 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/math/transforms/detail/fft_splitradix.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     4722 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/math/transforms/detail/permuter.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     3536 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/math/transforms/detail/roots_table.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     1642 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/math/transforms/detail/size_log2.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)      866 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/mem_fn.hpp
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-06-23 06:57:49.341548 zmesh-1.7.0/zi_lib/zi/mesh/
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-06-23 06:57:49.344671 zmesh-1.7.0/zi_lib/zi/mesh/detail/
+-rw-r--r--   0 wms        (501) staff       (20)     1844 2022-09-24 16:25:01.000000 zmesh-1.7.0/zi_lib/zi/mesh/detail/all_equal.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)    21023 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/mesh/detail/marching_cubes_tables.hpp
+-rw-r--r--   0 wms        (501) staff       (20)    19148 2022-09-20 17:12:08.000000 zmesh-1.7.0/zi_lib/zi/mesh/detail/mc_tables.hpp
+-rw-r--r--   0 wms        (501) staff       (20)     4607 2022-09-20 17:12:08.000000 zmesh-1.7.0/zi_lib/zi/mesh/detail/packed_coordinate.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     9633 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/mesh/detail/qmetric.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)    10719 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/mesh/detail/quadratic.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     7524 2022-09-20 17:12:08.000000 zmesh-1.7.0/zi_lib/zi/mesh/detail/tri_mesh_edge.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)    10044 2022-09-20 17:12:08.000000 zmesh-1.7.0/zi_lib/zi/mesh/detail/tri_mesh_face.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     1923 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/mesh/detail/tri_mesh_vertex.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     7118 2022-09-24 16:18:58.000000 zmesh-1.7.0/zi_lib/zi/mesh/face_mesh.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     4467 2022-09-24 16:18:58.000000 zmesh-1.7.0/zi_lib/zi/mesh/int_mesh.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)    13499 2022-12-16 18:26:49.000000 zmesh-1.7.0/zi_lib/zi/mesh/marching_cubes.hpp
+-rw-r--r--   0 wms        (501) staff       (20)     3631 2022-09-20 17:12:08.000000 zmesh-1.7.0/zi_lib/zi/mesh/network_sort.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)    25282 2023-06-23 01:01:23.000000 zmesh-1.7.0/zi_lib/zi/mesh/quadratic_simplifier.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     5872 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/mesh/tri_list.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)    15072 2023-06-23 01:01:23.000000 zmesh-1.7.0/zi_lib/zi/mesh/tri_mesh.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)    11185 2022-09-19 22:57:33.000000 zmesh-1.7.0/zi_lib/zi/mesh/tri_stripper.hpp
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-06-23 06:57:49.346439 zmesh-1.7.0/zi_lib/zi/meta/
+-rwxr-xr-x   0 wms        (501) staff       (20)     1423 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/meta/and.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     1141 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/meta/bool.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     1877 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/meta/enable_if.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     1018 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/meta/false_type.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     1429 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/meta/if.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     1049 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/meta/meta.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     1005 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/meta/null_type.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     1866 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/meta/or.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     1013 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/meta/true_type.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)      906 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/mutex.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)      887 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/non_copyable.hpp
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-06-23 06:57:49.346837 zmesh-1.7.0/zi_lib/zi/parallel/
+-rwxr-xr-x   0 wms        (501) staff       (20)     2659 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/parallel/algorithm.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     1323 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/parallel/numeric.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)      866 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/random.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)      857 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/ref.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)      875 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/result_of.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)      878 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/shared_ptr.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)      878 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/singleton.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)      890 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/static_assert.hpp
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-06-23 06:57:49.347640 zmesh-1.7.0/zi_lib/zi/system/
+-rwxr-xr-x   0 wms        (501) staff       (20)     1573 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/system/config.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     2219 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/system/daemon.hpp
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-06-23 06:57:49.349377 zmesh-1.7.0/zi_lib/zi/system/detail/
+-rwxr-xr-x   0 wms        (501) staff       (20)     4536 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/system/detail/cerrno_code.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     1386 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/system/detail/cpu_count.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     1639 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/system/detail/get_hostname.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     1521 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/system/detail/get_username.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     3297 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/system/detail/linux_errno_code.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     2485 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/system/detail/memory_size.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     2606 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/system/detail/memory_usage.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     3193 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/system/detail/win32_errno_code.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     1294 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/system/error.hpp
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-06-23 06:57:49.349592 zmesh-1.7.0/zi_lib/zi/system/example/
+-rwxr-xr-x   0 wms        (501) staff       (20)     5027 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/system/example/example.cpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     8169 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/system/system.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)      868 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/system.hpp
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-06-23 06:57:49.351462 zmesh-1.7.0/zi_lib/zi/test/
+-rwxr-xr-x   0 wms        (501) staff       (20)      652 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/test/Makefile
+-rwxr-xr-x   0 wms        (501) staff       (20)     2794 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/test/Makefile-include-mingw32
+-rwxr-xr-x   0 wms        (501) staff       (20)     2889 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/test/Makefile-include-nix
+-rwxr-xr-x   0 wms        (501) staff       (20)     2605 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/test/Makefile-include-wine
+-rwxr-xr-x   0 wms        (501) staff       (20)      691 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/test/Makefile-mingw32
+-rwxr-xr-x   0 wms        (501) staff       (20)      654 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/test/Makefile-nix-mingw32
+-rwxr-xr-x   0 wms        (501) staff       (20)      672 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/test/Makefile-tmp
+-rwxr-xr-x   0 wms        (501) staff       (20)     1400 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/test/Makefile-wine
+-rwxr-xr-x   0 wms        (501) staff       (20)       29 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/test/main.cpp
+-rwxr-xr-x   0 wms        (501) staff       (20)      862 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/test.hpp
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-06-23 06:57:49.353221 zmesh-1.7.0/zi_lib/zi/time/
+-rwxr-xr-x   0 wms        (501) staff       (20)     1498 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/time/config.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     5963 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/time/interval.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     2894 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/time/now.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     3224 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/time/process_timer.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)      997 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/time/time.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     1764 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/time/time_units.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     3685 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/time/time_utils.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     2084 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/time/timer.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     3769 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/time/wall_timer.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)      860 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/time.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)      863 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/timer.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)      863 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/tuple.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)      881 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/type_traits.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)      866 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/typeof.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)      870 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/unittest.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)      887 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/unordered_map.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)      886 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/unordered_set.hpp
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-06-23 06:57:49.358960 zmesh-1.7.0/zi_lib/zi/utility/
+-rwxr-xr-x   0 wms        (501) staff       (20)     1481 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/utility/address_of.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     1751 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/utility/assert.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     2510 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/utility/binary_printer.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     1056 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/utility/container_utilities.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     1665 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/utility/deferred_instantiation.hpp
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-06-23 06:57:49.360777 zmesh-1.7.0/zi_lib/zi/utility/detail/
+-rwxr-xr-x   0 wms        (501) staff       (20)     1219 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/utility/detail/bare_type.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     1062 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/utility/detail/dummy.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)      973 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/utility/detail/empty_type.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     1402 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/utility/detail/get_instance.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     1783 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/utility/detail/nbyte_int.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     1054 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/utility/detail/not_this_type.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)      987 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/utility/detail/whatever.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     1009 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/utility/detail/yes_no_type.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     1973 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/utility/enable_if.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     1387 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/utility/enable_singleton_of_this.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     2330 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/utility/exception.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     2360 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/utility/for_each.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     1387 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/utility/is_complex.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     2417 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/utility/is_printable.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     4557 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/utility/natural_compare.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     1182 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/utility/non_copyable.hpp
+-rw-r--r--   0 wms        (501) staff       (20)    94949 2022-09-20 17:12:08.000000 zmesh-1.7.0/zi_lib/zi/utility/robin_hood.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     1588 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/utility/singleton.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     1914 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/utility/static_and.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     1494 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/utility/static_assert.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     1371 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/utility/static_if.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     1940 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/utility/static_or.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     1748 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/utility/string_printf.hpp
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-06-23 06:57:49.361572 zmesh-1.7.0/zi_lib/zi/utility/test/
+-rwxr-xr-x   0 wms        (501) staff       (20)     1517 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/utility/test/address_of_test.cpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     1788 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/utility/test/enable_if_test.cpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     4041 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/utility/test/is_printable_test.cpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     1349 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/utility/this_function.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     1830 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/utility/value_iterator.hpp
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-06-23 06:57:49.363765 zmesh-1.7.0/zi_lib/zi/vl/
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-06-23 06:57:49.365061 zmesh-1.7.0/zi_lib/zi/vl/detail/
+-rwxr-xr-x   0 wms        (501) staff       (20)     2026 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/vl/detail/enable_if.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)    11929 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/vl/detail/householder.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     8484 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/vl/detail/invert.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     7182 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/vl/detail/jacobi.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     1726 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/vl/detail/mat_lookup_table.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     7894 2022-09-24 15:32:42.000000 zmesh-1.7.0/zi_lib/zi/vl/detail/promote.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)    37154 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/vl/mat.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)    14937 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/vl/mat_functions.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)    31314 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/vl/quat.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     9118 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/vl/quat_functions.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)    22196 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/vl/vec.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)    13509 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/vl/vec_functions.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)      910 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/vl/vl.hpp
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-06-23 06:57:49.365588 zmesh-1.7.0/zi_lib/zi/watershed/
+-rwxr-xr-x   0 wms        (501) staff       (20)     3829 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/watershed/quickie.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)      942 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/watershed/watershed.hpp
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-06-23 06:57:49.366435 zmesh-1.7.0/zi_lib/zi/zargs/
+-rwxr-xr-x   0 wms        (501) staff       (20)     4643 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/zargs/arguments.hpp
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-06-23 06:57:49.367479 zmesh-1.7.0/zi_lib/zi/zargs/detail/
+-rwxr-xr-x   0 wms        (501) staff       (20)     1054 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/zargs/detail/boost_lexical_cast.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)      956 2022-09-24 16:18:58.000000 zmesh-1.7.0/zi_lib/zi/zargs/detail/lexical_cast.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     2847 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/zargs/detail/simple_lexical_cast.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     2521 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/zargs/detail/string_utils.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     2469 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/zargs/matcher.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     4025 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/zargs/parser.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)    11502 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/zargs/zargs.hpp
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-06-23 06:57:49.368724 zmesh-1.7.0/zi_lib/zi/zlog/
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-06-23 06:57:49.369081 zmesh-1.7.0/zi_lib/zi/zlog/example/
+-rwxr-xr-x   0 wms        (501) staff       (20)     4845 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/zlog/example/example.cpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     1157 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/zlog/example/example_other.cpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     1835 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/zlog/log_printf.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     3775 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/zlog/logs.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     2276 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/zlog/registry.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     2015 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/zlog/sink.hpp
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-06-23 06:57:49.369265 zmesh-1.7.0/zi_lib/zi/zlog/test/
+-rwxr-xr-x   0 wms        (501) staff       (20)     1557 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/zlog/test/token_sink_test.cpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     2190 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/zlog/token.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     7269 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/zlog/zlog.hpp
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-06-23 06:57:49.369806 zmesh-1.7.0/zi_lib/zi/zpp/
+-rwxr-xr-x   0 wms        (501) staff       (20)     3756 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/zpp/count_args.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)      920 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/zpp/glue.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)      932 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/zpp/stringify.hpp
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-06-23 06:57:49.372239 zmesh-1.7.0/zi_lib/zi/zunit/
+-rwxr-xr-x   0 wms        (501) staff       (20)     6176 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/zunit/checker.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)      879 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/zunit/config.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     4382 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/zunit/exception.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     7523 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/zunit/expect_xxx.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     5428 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/zunit/macros.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)      873 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/zunit/main.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     1022 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/zunit/main.ipp
+-rwxr-xr-x   0 wms        (501) staff       (20)     1937 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/zunit/registry.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     1072 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/zunit/tags.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     1388 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/zunit/test_case.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     4382 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/zunit/test_suite.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)     1340 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/zunit/test_suite_tpl.hpp
+-rwxr-xr-x   0 wms        (501) staff       (20)      979 2022-04-04 21:20:05.000000 zmesh-1.7.0/zi_lib/zi/zunit/zunit.hpp
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-06-23 06:57:49.372897 zmesh-1.7.0/zmesh/
+-rw-r--r--   0 wms        (501) staff       (20)       78 2023-06-23 06:47:28.000000 zmesh-1.7.0/zmesh/__init__.py
+-rwxr-xr-x   0 wms        (501) staff       (20)    17122 2023-06-23 06:46:57.000000 zmesh-1.7.0/zmesh/_zmesh.pyx
+-rw-r--r--   0 wms        (501) staff       (20)     6875 2023-02-14 19:41:50.000000 zmesh-1.7.0/zmesh/mesh.py
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-06-23 06:57:49.373988 zmesh-1.7.0/zmesh.egg-info/
+-rw-r--r--   0 wms        (501) staff       (20)     6180 2023-06-23 06:57:47.000000 zmesh-1.7.0/zmesh.egg-info/PKG-INFO
+-rw-r--r--   0 wms        (501) staff       (20)    12881 2023-06-23 06:57:49.000000 zmesh-1.7.0/zmesh.egg-info/SOURCES.txt
+-rw-r--r--   0 wms        (501) staff       (20)        1 2023-06-23 06:57:47.000000 zmesh-1.7.0/zmesh.egg-info/dependency_links.txt
+-rw-r--r--   0 wms        (501) staff       (20)        1 2021-01-20 02:44:29.000000 zmesh-1.7.0/zmesh.egg-info/not-zip-safe
+-rw-r--r--   0 wms        (501) staff       (20)       46 2023-06-23 06:57:47.000000 zmesh-1.7.0/zmesh.egg-info/pbr.json
+-rw-r--r--   0 wms        (501) staff       (20)        6 2023-06-23 06:57:47.000000 zmesh-1.7.0/zmesh.egg-info/requires.txt
+-rw-r--r--   0 wms        (501) staff       (20)        6 2023-06-23 06:57:47.000000 zmesh-1.7.0/zmesh.egg-info/top_level.txt
```

### Comparing `zmesh-1.6.2/.github/workflows/build_wheels.yml` & `zmesh-1.7.0/.github/workflows/build_wheels.yml`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/.github/workflows/test.yml` & `zmesh-1.7.0/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/ChangeLog` & `zmesh-1.7.0/ChangeLog`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 CHANGES
 =======
 
+1.7.0
+-----
+
+* release(1.7.0): deprecates get\_mesh in favor of get
+* fix: transpose of mesh image (#38)
+
 1.6.2
 -----
 
 * release(1.6.2): obj import accepts scientific notation
 * feat: allow from\_obj to parse scientific notation (e.g. 1e-5)
 * test: check broken fanc example to prevent regressions
 * build: update cibuildwheel
```

### Comparing `zmesh-1.6.2/Dockerfile` & `zmesh-1.7.0/Dockerfile`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/LICENSE` & `zmesh-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/PKG-INFO` & `zmesh-1.7.0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,35 +1,7 @@
-Metadata-Version: 2.1
-Name: zmesh
-Version: 1.6.2
-Summary: Multilabel marching cubes and simplification of volumetric data.
-Home-page: https://github.com/seung-lab/zmesh/
-Author: William Silversmith (maintainer), Aleks Zlateski (original author)
-Author-email: ws9@princeton.edu
-License: GPLv3+
-Platform: UNKNOWN
-Classifier: Intended Audience :: Developers
-Classifier: Development Status :: 4 - Beta
-Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Utilities
-Classifier: Topic :: Scientific/Engineering
-Classifier: Topic :: Scientific/Engineering :: Visualization
-Classifier: Topic :: Multimedia :: Graphics :: 3D Modeling
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
-License-File: LICENSE
-License-File: AUTHORS
-
 ## zmesh: Multi-Label Marching Cubes &amp; Mesh Simplification
 [![Tests](https://github.com/seung-lab/zmesh/actions/workflows/test.yml/badge.svg?branch=master)](https://github.com/seung-lab/zmesh/actions/workflows/test.yml) [![PyPI version](https://badge.fury.io/py/zmesh.svg)](https://badge.fury.io/py/zmesh)  
 
 ```python
 from zmesh import Mesher
 
 labels = ... # some dense volumetric labeled image
@@ -39,39 +11,42 @@
 # close controls whether meshes touching
 # the image boundary are left open or closed
 mesher.mesh(labels, close=False) 
 
 meshes = []
 for obj_id in mesher.ids():
   meshes.append(
-    mesher.get_mesh(
+    mesher.get(
       obj_id, 
       normals=False, # whether to calculate normals or not
 
       # tries to reduce triangles by this factor
       # 0 disables simplification
-      simplification_factor=100, 
+      reduction_factor=100, 
 
       # Max tolerable error in physical distance
-      max_simplification_error=8,
+      # note: if max_error is not set, the max error
+      # will be set equivalent to one voxel along the 
+      # smallest dimension.
+      max_error=8,
       # whether meshes should be centered in the voxel
       # on (0,0,0) [False] or (0.5,0.5,0.5) [True]
       voxel_centered=False, 
     )
   )
   mesher.erase(obj_id) # delete high res mesh
 
 mesher.clear() # clear memory retained by mesher
 
 mesh = meshes[0]
 mesh = mesher.simplify(
   mesh, 
-  # same as simplification_factor in get_mesh
+  # same as reduction_factor in get
   reduction_factor=100, 
-  # same as max_simplification_error in get_mesh
+  # same as max_error in get
   max_error=40, 
   compute_normals=False, # whether to also compute face normals
 ) # apply simplifier to a pre-existing mesh
 
 # compute normals without simplifying
 mesh = mesher.compute_normals(mesh) 
 
@@ -89,14 +64,16 @@
   f.write(mesh.to_ply())
 
 # Neuroglancer Precomputed format
 with open('10001001:0', 'wb') as f:
   f.write(mesh.to_precomputed())
 ```
 
+Note: As of the latest version, `mesher.get_mesh` has been deprecated in favor of `mesher.get` which fixes a long standing bug where you needed to transpose your data in order to get a mesh in the correct orientation.
+
 ## Installation 
 
 If binaries are not available for your system, ensure you have a C++ compiler installed.
 
 ```bash
 pip install zmesh
 ```
@@ -121,11 +98,8 @@
 
 Later changes by Will Silversmith, Nico Kemnitz, and Jingpeng Wu. 
 
 ## References  
 
 1. W. Lorensen and H. Cline. "Marching Cubes: A High Resolution 3D Surface Construction Algorithm". pp 163-169. Computer Graphics, Volume 21, Number 4, July 1987. ([link](https://people.eecs.berkeley.edu/~jrs/meshpapers/LorensenCline.pdf))  
 2. M. Garland and P. Heckbert. "Surface simplification using quadric error metrics". SIGGRAPH '97: Proceedings of the 24th annual conference on Computer graphics and interactive techniques. Pages 209–216. August 1997. doi: 10.1145/258734.258849 ([link](https://mgarland.org/files/papers/quadrics.pdf))  
-3. H. Hoppe. "New Quadric Metric for Simplifying Meshes with Appearance Attributes". IEEE Visualization 1999 Conference. pp. 59-66. doi: 10.1109/VISUAL.1999.809869 ([link](http://hhoppe.com/newqem.pdf))
-
-
-
+3. H. Hoppe. "New Quadric Metric for Simplifying Meshes with Appearance Attributes". IEEE Visualization 1999 Conference. pp. 59-66. doi: 10.1109/VISUAL.1999.809869 ([link](http://hhoppe.com/newqem.pdf))
```

### Comparing `zmesh-1.6.2/automated_test.py` & `zmesh-1.7.0/automated_test.py`

 * *Files 26% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 def fanc_label():
   with gzip.open('./fanc_bug.npy.gz', 'rb') as f:
     return np.load(f)[...,0]
 
 @pytest.mark.parametrize("dtype", DTYPE)
 @pytest.mark.parametrize("close", [ False, True ])
 @pytest.mark.parametrize("order", [ 'C', 'F' ])
-def test_executes(dtype, close, order):
+def test_executes_legacy(dtype, close, order):
   labels = np.zeros( (11,17,19), dtype=dtype, order=order)
   labels[1:-1, 1:-1, 1:-1] = 1
 
   mesher = zmesh.Mesher( (4,4,40) )
   mesher.mesh(labels, close=close)
 
   mesh = mesher.get_mesh(1, normals=False)
@@ -33,14 +33,35 @@
   assert mesh.normals is None
 
   mesh = mesher.get_mesh(1, normals=True)
   assert len(mesh.vertices) > 0
   assert len(mesh.faces) > 0
   assert len(mesh.normals) > 0
 
+
+@pytest.mark.parametrize("dtype", DTYPE)
+@pytest.mark.parametrize("close", [ False, True ])
+@pytest.mark.parametrize("order", [ 'C', 'F' ])
+def test_executes(dtype, close, order):
+  labels = np.zeros( (11,17,19), dtype=dtype, order=order)
+  labels[1:-1, 1:-1, 1:-1] = 1
+
+  mesher = zmesh.Mesher( (4,4,40) )
+  mesher.mesh(labels, close=close)
+
+  mesh = mesher.get(1, normals=False)
+  assert len(mesh.vertices) > 0
+  assert len(mesh.faces) > 0
+  assert mesh.normals is None
+
+  mesh = mesher.get(1, normals=True)
+  assert len(mesh.vertices) > 0
+  assert len(mesh.faces) > 0
+  assert len(mesh.normals) > 0
+
 @pytest.mark.parametrize("dtype", DTYPE)
 @pytest.mark.parametrize("order", [ 'C', 'F' ])
 def test_simplify(dtype, order):
   labels = np.zeros( (11,17,19), dtype=dtype, order=order)
   labels[1:-1, 1:-1, 1:-1] = 1
 
   mesher = zmesh.Mesher( (4,4,40) )
@@ -79,15 +100,15 @@
     mesh.vertices[1:] = 2**20
     mesh = mesher.simplify(mesh, reduction_factor=2, max_error=40, compute_normals=True)
     assert False
   except ValueError:
     pass
 
 @pytest.mark.parametrize("dtype", DTYPE)
-def test_precomputed(dtype):
+def test_precomputed_legacy(dtype):
   labels = np.zeros( (11,17,19), dtype=dtype)
   labels[1:-1, 1:-1, 1:-1] = 1
 
   mesher = zmesh.Mesher( (4,4,40) )
   mesher.mesh(labels)
   mesh = mesher.get_mesh(1, normals=False)
 
@@ -97,41 +118,60 @@
 
   mesh = mesher.get_mesh(1, normals=True)
 
   precomputed_mesh = mesh.to_precomputed()
   reconstituted = zmesh.Mesh.from_precomputed(precomputed_mesh)
   assert reconstituted != mesh # Precomputed doesn't preserve normals
 
+@pytest.mark.parametrize("dtype", DTYPE)
+def test_precomputed(dtype):
+  labels = np.zeros( (11,17,19), dtype=dtype)
+  labels[1:-1, 1:-1, 1:-1] = 1
+
+  mesher = zmesh.Mesher( (4,4,40) )
+  mesher.mesh(labels)
+  mesh = mesher.get(1, normals=False)
+
+  precomputed_mesh = mesh.to_precomputed()
+  reconstituted = zmesh.Mesh.from_precomputed(precomputed_mesh)
+  assert reconstituted == mesh
+
+  mesh = mesher.get(1, normals=True)
+
+  precomputed_mesh = mesh.to_precomputed()
+  reconstituted = zmesh.Mesh.from_precomputed(precomputed_mesh)
+  assert reconstituted != mesh # Precomputed doesn't preserve normals
+
 def test_obj_import():
   labels = np.zeros( (11,17,19), dtype=np.uint32)
   labels[1:-1, 1:-1, 1:-1] = 1
 
   mesher = zmesh.Mesher( (4,4,40) )
   mesher.mesh(labels)
-  mesh = mesher.get_mesh(1, normals=False)
+  mesh = mesher.get(1, normals=False)
 
   obj_str = mesh.to_obj()
   mesh2 = zmesh.Mesh.from_obj(obj_str)
   
   assert mesh == mesh2
 
 def test_ply_import():
   labels = np.zeros( (11,17,19), dtype=np.uint32)
   labels[1:-1, 1:-1, 1:-1] = 1
 
   mesher = zmesh.Mesher( (4,4,40) )
   mesher.mesh(labels)
-  mesh = mesher.get_mesh(1, normals=False)
+  mesh = mesher.get(1, normals=False)
 
   plydata = mesh.to_ply()
   mesh2 = zmesh.Mesh.from_ply(plydata)
   
   assert mesh == mesh2
 
-def test_C_F_meshes_same(connectomics_labels):
+def test_C_F_meshes_same_legacy(connectomics_labels):
   connectomics_labels = connectomics_labels[102:,31:,17:]
 
   fdata = np.asfortranarray(connectomics_labels)
   cdata = np.ascontiguousarray(connectomics_labels)
 
   f_mesher = zmesh.Mesher((1,1,1))
   f_mesher.mesh(fdata)
@@ -162,16 +202,16 @@
 
   c_mesher = zmesh.Mesher((1,1,1))
   c_mesher.mesh(cdata)
 
   assert c_mesher.ids() == f_mesher.ids()
 
   for label in c_mesher.ids():
-    c_mesh = c_mesher.get_mesh(label, normals=False, simplification_factor=0)
-    f_mesh = f_mesher.get_mesh(label, normals=False, simplification_factor=0)
+    c_mesh = c_mesher.get(label, normals=False, reduction_factor=0)
+    f_mesh = f_mesher.get(label, normals=False, reduction_factor=0)
     assert np.isclose(c_mesh.vertices.mean(), f_mesh.vertices.mean())
 
 @pytest.mark.parametrize("order", [ 'C', 'F' ])
 def test_unsimplified_meshes_remain_the_same(connectomics_labels, order):
   if order == "C":
     connectomics_labels = np.ascontiguousarray(connectomics_labels)
   else:
@@ -184,14 +224,39 @@
     with gzip.open(f"./connectomics_npy_meshes/unsimplified/{lbl}.ply.gz", "rb") as f:
       old_mesh = zmesh.Mesh.from_ply(f.read())
     new_mesh = mesher.get_mesh(lbl, normals=False, simplification_factor=0, max_simplification_error=40)
     assert np.all(np.sort(old_mesh.vertices[old_mesh.faces], axis=0) == np.sort(new_mesh.vertices[new_mesh.faces], axis=0))
     print(lbl, "ok")
 
 
+  mesher = zmesh.Mesher( (1,1,1) )
+  mesher.mesh(connectomics_labels)
+
+  mesher2 = zmesh.Mesher( (1,1,1) )
+  mesher2.mesh(connectomics_labels)
+
+  for lbl in mesher.ids()[:50]:
+    old_mesh = mesher.get_mesh(lbl, normals=False, simplification_factor=0, max_simplification_error=40)
+    new_mesh = mesher2.get(lbl, normals=False, reduction_factor=0, max_error=40)
+
+    old_pts = old_mesh.vertices[old_mesh.faces]
+    old_pts = old_pts.reshape(old_pts.shape[0] * old_pts.shape[1], 3)
+    transposed_old = np.copy(old_pts)
+    transposed_old[:,0] = old_pts[:,2]
+    transposed_old[:,2] = old_pts[:,0]
+    del old_pts
+    transposed_old.sort(axis=0)
+
+    new_pts = new_mesh.vertices[new_mesh.faces]
+    new_pts = new_pts.reshape(new_pts.shape[0] * new_pts.shape[1], 3)
+    new_pts.sort(axis=0)
+
+    assert np.all(transposed_old == new_pts)
+    print(lbl, "ok")  
+
 # F order meshes are processed in a different order and so
 # the simplifier produces a different mesh. Will have to add F order examples
 # in order to test.
 @pytest.mark.parametrize("order", [ 'C' ])
 @pytest.mark.skipif(sys.platform != 'darwin', reason="Different implementations of unordered_map on different platforms have different iteration behavior. Only MacOS will match.")
 def test_simplified_meshes_remain_the_same(connectomics_labels, order):
   if order == "C":
```

### Comparing `zmesh-1.6.2/cMesher.hpp` & `zmesh-1.7.0/cMesher.hpp`

 * *Files 19% similar despite different names*

```diff
@@ -46,51 +46,68 @@
   }
 
   PositionType pack_coords(PositionType x, PositionType y, PositionType z) {
     return marchingcubes_.pack_coords(x,y,z);
   }
 
   MeshObject get_mesh(
-      LabelType segid, bool generate_normals,
-      int simplification_factor,
-      int max_simplification_error
-    ) {
+    LabelType segid, 
+    bool generate_normals,
+    int simplification_factor,
+    int max_simplification_error,
+    bool transpose = true
+  ) {
 
     // MC produces no triangles if either
     // none or all voxels were labeled.
     MeshObject empty_obj;
     if (marchingcubes_.count(segid) == 0) { 
       return empty_obj;
     }
 
     std::vector< zi::vl::vec< PositionType, 3> > triangles = marchingcubes_.get_triangles(segid);
 
     return simplify(
       triangles,
       generate_normals,
       simplification_factor,
-      max_simplification_error
+      max_simplification_error,
+      transpose
     );
   }
 
   MeshObject simplify(      
       const std::vector< zi::vl::vec< PositionType, 3> >& triangles,
       bool generate_normals,
       int simplification_factor,
-      int max_simplification_error
+      int max_simplification_error,
+
+      // This is to support the old broken version
+      // w/ backwards compatibility
+      bool transpose = true 
     ) {
 
     MeshObject obj;
 
     zi::mesh::int_mesh<PositionType, LabelType> im;
     im.add(triangles);
+
+    float wx = voxelresolution_[0];
+    float wy = voxelresolution_[1]; 
+    float wz = voxelresolution_[2];
+    if (transpose) {
+      wx = voxelresolution_[2];
+      wy = voxelresolution_[1];
+      wz = voxelresolution_[0];
+    }
+
     im.template fill_simplifier<SimplifierType>(
       simplifier_, 
       0, 0, 0, 
-      voxelresolution_[2], voxelresolution_[1], voxelresolution_[0]
+      wx, wy, wz
     );
 
     if (simplification_factor > 0) {
       simplifier_.prepare(generate_normals);
       // This is the most cpu intensive line
       simplifier_.optimize(
           simplifier_.face_count() / simplification_factor,
@@ -106,32 +123,55 @@
     obj.points.reserve(3 * points.size());
     obj.faces.reserve(3 * faces.size());
 
     if (generate_normals) {
       obj.normals.reserve(3 * points.size());
     }
 
-    for (auto v = points.begin(); v != points.end(); ++v) {
-      obj.points.push_back((*v)[2]);
-      obj.points.push_back((*v)[1]);
-      obj.points.push_back((*v)[0]);
-    }
+    if (transpose) {
+      for (auto v = points.begin(); v != points.end(); ++v) {
+        obj.points.push_back((*v)[2]);
+        obj.points.push_back((*v)[1]);
+        obj.points.push_back((*v)[0]);
+      }
 
-    if (generate_normals) {
-      for (auto vn = normals.begin(); vn != normals.end(); ++vn) {
-        obj.normals.push_back((*vn)[2]);
-        obj.normals.push_back((*vn)[1]);
-        obj.normals.push_back((*vn)[0]);
+      if (generate_normals) {
+        for (auto vn = normals.begin(); vn != normals.end(); ++vn) {
+          obj.normals.push_back((*vn)[2]);
+          obj.normals.push_back((*vn)[1]);
+          obj.normals.push_back((*vn)[0]);
+        }
+      }
+
+      for (auto f = faces.begin(); f != faces.end(); ++f) {
+        obj.faces.push_back((*f)[0]);
+        obj.faces.push_back((*f)[2]);
+        obj.faces.push_back((*f)[1]);
       }
     }
+    else {
+      for (auto v = points.begin(); v != points.end(); ++v) {
+        obj.points.push_back((*v)[0]);
+        obj.points.push_back((*v)[1]);
+        obj.points.push_back((*v)[2]);
+      }
 
-    for (auto f = faces.begin(); f != faces.end(); ++f) {
-      obj.faces.push_back((*f)[0]);
-      obj.faces.push_back((*f)[2]);
-      obj.faces.push_back((*f)[1]);
+      if (generate_normals) {
+        for (auto vn = normals.begin(); vn != normals.end(); ++vn) {
+          obj.normals.push_back((*vn)[0]);
+          obj.normals.push_back((*vn)[1]);
+          obj.normals.push_back((*vn)[2]);
+        }
+      }
+
+      for (auto f = faces.begin(); f != faces.end(); ++f) {
+        obj.faces.push_back((*f)[1]);
+        obj.faces.push_back((*f)[2]);
+        obj.faces.push_back((*f)[0]);
+      }
     }
 
     return obj;
   }
 
   MeshObject simplify_points(
     const uint64_t* points,
```

### Comparing `zmesh-1.6.2/fanc_bug.npy.gz` & `zmesh-1.7.0/fanc_bug.npy.gz`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/perf.py` & `zmesh-1.7.0/perf.py`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/setup.cfg` & `zmesh-1.7.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/setup.py` & `zmesh-1.7.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,22 +26,22 @@
     '-std=c++17', '-O3', '-Wno-unused-local-typedefs', 
     '-DNDEBUG',
   ]
 
 include_dirs = [ NumpyImport(), 'zi_lib/', './' ]
 
 setuptools.setup(
-  setup_requires=['pbr', 'numpy'],
+  setup_requires=['pbr', 'numpy', 'cython'],
   python_requires=">=3.7", # >= 3.6 < 4.0
   pbr=True,
   define_macros=[ ("NDEBUG", 1) ],
   ext_modules=[
     setuptools.Extension(
       'zmesh._zmesh',
-      sources=[ 'zmesh/_zmesh.cpp' ],
+      sources=[ 'zmesh/_zmesh.pyx' ],
       depends=[ 'cMesher.hpp' ],
       language='c++',
       include_dirs=include_dirs,
       extra_compile_args=extra_compile_args
     ),
   ],
 )
```

### Comparing `zmesh-1.6.2/templates/mesherclass.j2` & `zmesh-1.7.0/templates/mesherclass.j2`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 cdef class Mesher{{ position_type }}{{ '%02d' % label_type }}:
   cdef CMesher[uint{{ position_type }}_t, uint{{ label_type }}_t, float] *ptr      # hold a C++ instance which we're wrapping
 
   def __cinit__(self, voxel_res):
-    self.ptr = new CMesher[uint{{ position_type }}_t, uint{{ label_type }}_t, float](voxel_res.astype(np.float32))
+    self.ptr = new CMesher[uint{{ position_type }}_t, uint{{ label_type }}_t, float](voxel_res)
 
   def __dealloc__(self):
     del self.ptr
 
   def mesh(self, data):
     cdef cnp.ndarray[uint{{label_type}}_t, ndim=1] flat_data = reshape(data, (data.size,)).view(np.uint{{ label_type }})
     self.ptr.mesh(
@@ -14,16 +14,16 @@
       data.shape[0], data.shape[1], data.shape[2],
       data.flags.c_contiguous
     )
 
   def ids(self):
     return self.ptr.ids()
   
-  def get_mesh(self, mesh_id, normals=False, simplification_factor=0, max_simplification_error=40):
-    return self.ptr.get_mesh(mesh_id, normals, simplification_factor, max_simplification_error)
+  def get_mesh(self, mesh_id, normals=False, simplification_factor=0, max_simplification_error=40, transpose=True):
+    return self.ptr.get_mesh(mesh_id, normals, simplification_factor, max_simplification_error, transpose)
   
   def clear(self):
     self.ptr.clear()
 
   def erase(self, mesh_id):
     return self.ptr.erase(mesh_id)
```

### Comparing `zmesh-1.6.2/zi_lib/gpl-3.0.txt` & `zmesh-1.7.0/zi_lib/gpl-3.0.txt`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/ai/decision_tree.hpp` & `zmesh-1.7.0/zi_lib/zi/ai/decision_tree.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/ai/detail/entropy.hpp` & `zmesh-1.7.0/zi_lib/zi/ai/detail/entropy.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/ai/detail/gini_maximizing_splitter.hpp` & `zmesh-1.7.0/zi_lib/zi/ai/detail/gini_maximizing_splitter.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/ai/detail/information_gain_splitter.hpp` & `zmesh-1.7.0/zi_lib/zi/ai/detail/information_gain_splitter.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/ai/detail/mmdt_splitter.hpp` & `zmesh-1.7.0/zi_lib/zi/ai/detail/mmdt_splitter.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/ai/random_forest.hpp` & `zmesh-1.7.0/zi_lib/zi/ai/random_forest.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/ansi_term/constants.hpp` & `zmesh-1.7.0/zi_lib/zi/ansi_term/constants.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/ansi_term/flags.hpp` & `zmesh-1.7.0/zi_lib/zi/ansi_term/flags.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/ansi_term/tags.hpp` & `zmesh-1.7.0/zi_lib/zi/ansi_term/tags.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/ansi_term/term_ostream.hpp` & `zmesh-1.7.0/zi_lib/zi/ansi_term/term_ostream.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/ansi_term.hpp` & `zmesh-1.7.0/zi_lib/zi/ansi_term.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/arguments.hpp` & `zmesh-1.7.0/zi_lib/zi/arguments.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/array.hpp` & `zmesh-1.7.0/zi_lib/zi/array.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/assert.hpp` & `zmesh-1.7.0/zi_lib/zi/assert.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/atomic/atomic.hpp` & `zmesh-1.7.0/zi_lib/zi/atomic/atomic.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/atomic/config.hpp` & `zmesh-1.7.0/zi_lib/zi/atomic/config.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/atomic/detail/atomic_gcc_i386.hpp` & `zmesh-1.7.0/zi_lib/zi/atomic/detail/atomic_gcc_i386.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/atomic/detail/atomic_gcc_ppc.hpp` & `zmesh-1.7.0/zi_lib/zi/atomic/detail/atomic_gcc_ppc.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/atomic/detail/atomic_gcc_sync.hpp` & `zmesh-1.7.0/zi_lib/zi/atomic/detail/atomic_gcc_sync.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/atomic/detail/atomic_gcc_x64.hpp` & `zmesh-1.7.0/zi_lib/zi/atomic/detail/atomic_gcc_x64.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/atomic/detail/atomic_win32.hpp` & `zmesh-1.7.0/zi_lib/zi/atomic/detail/atomic_win32.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/atomic/detail/fenced_block_gcc_sync.hpp` & `zmesh-1.7.0/zi_lib/zi/atomic/detail/fenced_block_gcc_sync.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/atomic/detail/fenced_block_gcc_x86.hpp` & `zmesh-1.7.0/zi_lib/zi/atomic/detail/fenced_block_gcc_x86.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/atomic/detail/fenced_block_macos.hpp` & `zmesh-1.7.0/zi_lib/zi/atomic/detail/fenced_block_macos.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/atomic/detail/fenced_block_win32.hpp` & `zmesh-1.7.0/zi_lib/zi/atomic/detail/fenced_block_win32.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/atomic/fenced_block.hpp` & `zmesh-1.7.0/zi_lib/zi/atomic/fenced_block.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/atomic/spinlock.hpp` & `zmesh-1.7.0/zi_lib/zi/atomic/spinlock.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/atomic/test/atomic_test.cpp` & `zmesh-1.7.0/zi_lib/zi/atomic/test/atomic_test.cpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/binary_heap.hpp` & `zmesh-1.7.0/zi_lib/zi/binary_heap.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/bind.hpp` & `zmesh-1.7.0/zi_lib/zi/bind.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/bits/array.hpp` & `zmesh-1.7.0/zi_lib/zi/bits/array.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/bits/bind.hpp` & `zmesh-1.7.0/zi_lib/zi/bits/bind.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/bits/cerrno.hpp` & `zmesh-1.7.0/zi_lib/zi/bits/cerrno.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/bits/cstdint.hpp` & `zmesh-1.7.0/zi_lib/zi/bits/cstdint.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/bits/enable_shared_from_this.hpp` & `zmesh-1.7.0/zi_lib/zi/bits/enable_shared_from_this.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/bits/function.hpp` & `zmesh-1.7.0/zi_lib/zi/bits/function.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/bits/hash.hpp` & `zmesh-1.7.0/zi_lib/zi/bits/hash.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/bits/mem_fn.hpp` & `zmesh-1.7.0/zi_lib/zi/bits/mem_fn.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/bits/random.hpp` & `zmesh-1.7.0/zi_lib/zi/bits/random.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/bits/ref.hpp` & `zmesh-1.7.0/zi_lib/zi/bits/ref.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/bits/result_of.hpp` & `zmesh-1.7.0/zi_lib/zi/bits/result_of.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/bits/shared_ptr.hpp` & `zmesh-1.7.0/zi_lib/zi/bits/shared_ptr.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/bits/tuple.hpp` & `zmesh-1.7.0/zi_lib/zi/bits/tuple.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/bits/type_traits.hpp` & `zmesh-1.7.0/zi_lib/zi/bits/type_traits.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/bits/typeof.hpp` & `zmesh-1.7.0/zi_lib/zi/bits/typeof.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/bits/unordered_map.hpp` & `zmesh-1.7.0/zi_lib/zi/bits/unordered_map.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/bits/unordered_set.hpp` & `zmesh-1.7.0/zi_lib/zi/bits/unordered_set.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/cache/cache_container.hpp` & `zmesh-1.7.0/zi_lib/zi/cache/cache_container.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/cache/cache_fwd.hpp` & `zmesh-1.7.0/zi_lib/zi/cache/cache_fwd.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/cache/config.hpp` & `zmesh-1.7.0/zi_lib/zi/cache/config.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/cache/container.hpp` & `zmesh-1.7.0/zi_lib/zi/cache/container.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/cache/container_fwd.hpp` & `zmesh-1.7.0/zi_lib/zi/cache/container_fwd.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/cache/detail/container_base.hpp` & `zmesh-1.7.0/zi_lib/zi/cache/detail/container_base.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/cache/detail/container_entry.hpp` & `zmesh-1.7.0/zi_lib/zi/cache/detail/container_entry.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/cache/detail/default_constructor.hpp` & `zmesh-1.7.0/zi_lib/zi/cache/detail/default_constructor.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/cache/detail/enable_if.hpp` & `zmesh-1.7.0/zi_lib/zi/cache/detail/enable_if.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/cache/detail/if.hpp` & `zmesh-1.7.0/zi_lib/zi/cache/detail/if.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/cache/detail/key_extractors.hpp` & `zmesh-1.7.0/zi_lib/zi/cache/detail/key_extractors.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/cache/detail/multi_index.hpp` & `zmesh-1.7.0/zi_lib/zi/cache/detail/multi_index.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/cache/detail/ref.hpp` & `zmesh-1.7.0/zi_lib/zi/cache/detail/ref.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/cache/detail/storage_base.hpp` & `zmesh-1.7.0/zi_lib/zi/cache/detail/storage_base.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/cache/detail/storage_entry.hpp` & `zmesh-1.7.0/zi_lib/zi/cache/detail/storage_entry.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/cache/detail/type_traits.hpp` & `zmesh-1.7.0/zi_lib/zi/cache/detail/type_traits.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/cache/detail/yes_no_type.hpp` & `zmesh-1.7.0/zi_lib/zi/cache/detail/yes_no_type.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/cache/global_function.hpp` & `zmesh-1.7.0/zi_lib/zi/cache/global_function.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/cache/identity.hpp` & `zmesh-1.7.0/zi_lib/zi/cache/identity.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/cache/member_function.hpp` & `zmesh-1.7.0/zi_lib/zi/cache/member_function.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/cache/member_variable.hpp` & `zmesh-1.7.0/zi_lib/zi/cache/member_variable.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/cache/tags.hpp` & `zmesh-1.7.0/zi_lib/zi/cache/tags.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/cache/test/container_test._cc` & `zmesh-1.7.0/zi_lib/zi/cache/test/container_test._cc`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/cache/test/key_extractors_test.cpp` & `zmesh-1.7.0/zi_lib/zi/cache/test/key_extractors_test.cpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/cache/test/key_extractors_test.hpp` & `zmesh-1.7.0/zi_lib/zi/cache/test/key_extractors_test.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/cache/test/member_function_test.cpp` & `zmesh-1.7.0/zi_lib/zi/cache/test/member_function_test.cpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/cerrno.hpp` & `zmesh-1.7.0/zi_lib/zi/cerrno.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/concurrency/barrier.hpp` & `zmesh-1.7.0/zi_lib/zi/concurrency/barrier.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/concurrency/concurrency.hpp` & `zmesh-1.7.0/zi_lib/zi/concurrency/concurrency.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/concurrency/condition_variable.hpp` & `zmesh-1.7.0/zi_lib/zi/concurrency/condition_variable.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/concurrency/config.hpp` & `zmesh-1.7.0/zi_lib/zi/concurrency/config.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/concurrency/detail/all_threads.hpp` & `zmesh-1.7.0/zi_lib/zi/concurrency/detail/all_threads.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/concurrency/detail/all_threads_data.hpp` & `zmesh-1.7.0/zi_lib/zi/concurrency/detail/all_threads_data.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/concurrency/detail/is_mutex.hpp` & `zmesh-1.7.0/zi_lib/zi/concurrency/detail/is_mutex.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/concurrency/detail/is_runnable.hpp` & `zmesh-1.7.0/zi_lib/zi/concurrency/detail/is_runnable.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/concurrency/detail/mutex_guard.hpp` & `zmesh-1.7.0/zi_lib/zi/concurrency/detail/mutex_guard.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/concurrency/detail/mutex_pool.hpp` & `zmesh-1.7.0/zi_lib/zi/concurrency/detail/mutex_pool.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/concurrency/detail/mutex_tags.hpp` & `zmesh-1.7.0/zi_lib/zi/concurrency/detail/mutex_tags.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/concurrency/detail/priority_task_container.hpp` & `zmesh-1.7.0/zi_lib/zi/concurrency/detail/priority_task_container.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/concurrency/detail/rwmutex_impl.hpp` & `zmesh-1.7.0/zi_lib/zi/concurrency/detail/rwmutex_impl.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/concurrency/detail/simple_task_container.hpp` & `zmesh-1.7.0/zi_lib/zi/concurrency/detail/simple_task_container.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/concurrency/detail/task_manager_impl.hpp` & `zmesh-1.7.0/zi_lib/zi/concurrency/detail/task_manager_impl.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/concurrency/detail/this_thread.hpp` & `zmesh-1.7.0/zi_lib/zi/concurrency/detail/this_thread.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/concurrency/detail/thread_info.hpp` & `zmesh-1.7.0/zi_lib/zi/concurrency/detail/thread_info.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/concurrency/event.hpp` & `zmesh-1.7.0/zi_lib/zi/concurrency/event.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/concurrency/guard.hpp` & `zmesh-1.7.0/zi_lib/zi/concurrency/guard.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/concurrency/monitor.hpp` & `zmesh-1.7.0/zi_lib/zi/concurrency/monitor.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/concurrency/mutex.hpp` & `zmesh-1.7.0/zi_lib/zi/concurrency/mutex.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/concurrency/periodic_function.hpp` & `zmesh-1.7.0/zi_lib/zi/concurrency/periodic_function.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/concurrency/pthread/condition_variable.hpp` & `zmesh-1.7.0/zi_lib/zi/concurrency/pthread/condition_variable.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/concurrency/pthread/detail/this_thread.hpp` & `zmesh-1.7.0/zi_lib/zi/concurrency/pthread/detail/this_thread.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/concurrency/pthread/event.hpp` & `zmesh-1.7.0/zi_lib/zi/concurrency/pthread/event.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/concurrency/pthread/mutex_initializers.hpp` & `zmesh-1.7.0/zi_lib/zi/concurrency/pthread/mutex_initializers.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/concurrency/pthread/mutex_tags.hpp` & `zmesh-1.7.0/zi_lib/zi/concurrency/pthread/mutex_tags.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/concurrency/pthread/mutex_tpl.hpp` & `zmesh-1.7.0/zi_lib/zi/concurrency/pthread/mutex_tpl.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/concurrency/pthread/mutex_types.hpp` & `zmesh-1.7.0/zi_lib/zi/concurrency/pthread/mutex_types.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/concurrency/pthread/rwmutex.hpp` & `zmesh-1.7.0/zi_lib/zi/concurrency/pthread/rwmutex.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/concurrency/pthread/rwmutex_using_pthread_rwlock_t.hpp` & `zmesh-1.7.0/zi_lib/zi/concurrency/pthread/rwmutex_using_pthread_rwlock_t.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/concurrency/pthread/spinlock.hpp` & `zmesh-1.7.0/zi_lib/zi/concurrency/pthread/spinlock.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/concurrency/pthread/thread.hpp` & `zmesh-1.7.0/zi_lib/zi/concurrency/pthread/thread.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/concurrency/pthread/thread_attributes.hpp` & `zmesh-1.7.0/zi_lib/zi/concurrency/pthread/thread_attributes.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/concurrency/pthread/types.hpp` & `zmesh-1.7.0/zi_lib/zi/concurrency/pthread/types.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/concurrency/runnable.hpp` & `zmesh-1.7.0/zi_lib/zi/concurrency/runnable.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/concurrency/rwmutex.hpp` & `zmesh-1.7.0/zi_lib/zi/concurrency/rwmutex.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/concurrency/semaphore.hpp` & `zmesh-1.7.0/zi_lib/zi/concurrency/semaphore.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/concurrency/spinlock.hpp` & `zmesh-1.7.0/zi_lib/zi/concurrency/spinlock.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/concurrency/state.hpp` & `zmesh-1.7.0/zi_lib/zi/concurrency/state.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/concurrency/task_manager.hpp` & `zmesh-1.7.0/zi_lib/zi/concurrency/task_manager.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/concurrency/test/barrier_test.cpp` & `zmesh-1.7.0/zi_lib/zi/concurrency/test/barrier_test.cpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/concurrency/test/condition_variable_test.cpp` & `zmesh-1.7.0/zi_lib/zi/concurrency/test/condition_variable_test.cpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/concurrency/test/event_test.cpp` & `zmesh-1.7.0/zi_lib/zi/concurrency/test/event_test.cpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/concurrency/test/mutex_test.cpp` & `zmesh-1.7.0/zi_lib/zi/concurrency/test/mutex_test.cpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/concurrency/test/periodic_function_test.cpp` & `zmesh-1.7.0/zi_lib/zi/concurrency/test/periodic_function_test.cpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/concurrency/test/rwmutex_test.cpp` & `zmesh-1.7.0/zi_lib/zi/concurrency/test/rwmutex_test.cpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/concurrency/test/semaphore_test.cpp` & `zmesh-1.7.0/zi_lib/zi/concurrency/test/semaphore_test.cpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/concurrency/test/task_manager_test.cpp` & `zmesh-1.7.0/zi_lib/zi/concurrency/test/task_manager_test.cpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/concurrency/thread.hpp` & `zmesh-1.7.0/zi_lib/zi/concurrency/thread.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/concurrency/thread_types.hpp` & `zmesh-1.7.0/zi_lib/zi/concurrency/thread_types.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/concurrency/trigger.hpp` & `zmesh-1.7.0/zi_lib/zi/concurrency/trigger.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/concurrency/win32/condition_variable.hpp` & `zmesh-1.7.0/zi_lib/zi/concurrency/win32/condition_variable.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/concurrency/win32/default_mutex.hpp` & `zmesh-1.7.0/zi_lib/zi/concurrency/win32/default_mutex.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/concurrency/win32/detail/interlocked.hpp` & `zmesh-1.7.0/zi_lib/zi/concurrency/win32/detail/interlocked.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/concurrency/win32/detail/primitives.hpp` & `zmesh-1.7.0/zi_lib/zi/concurrency/win32/detail/primitives.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/concurrency/win32/detail/this_thread.hpp` & `zmesh-1.7.0/zi_lib/zi/concurrency/win32/detail/this_thread.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/concurrency/win32/event.hpp` & `zmesh-1.7.0/zi_lib/zi/concurrency/win32/event.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/concurrency/win32/mutex_tags.hpp` & `zmesh-1.7.0/zi_lib/zi/concurrency/win32/mutex_tags.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/concurrency/win32/mutex_tpl.hpp` & `zmesh-1.7.0/zi_lib/zi/concurrency/win32/mutex_tpl.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/concurrency/win32/mutex_types.hpp` & `zmesh-1.7.0/zi_lib/zi/concurrency/win32/mutex_types.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/concurrency/win32/recursive_mutex.hpp` & `zmesh-1.7.0/zi_lib/zi/concurrency/win32/recursive_mutex.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/concurrency/win32/rwmutex.hpp` & `zmesh-1.7.0/zi_lib/zi/concurrency/win32/rwmutex.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/concurrency/win32/spinlock.hpp` & `zmesh-1.7.0/zi_lib/zi/concurrency/win32/spinlock.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/concurrency/win32/spinlock_fast.hpp` & `zmesh-1.7.0/zi_lib/zi/concurrency/win32/spinlock_fast.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/concurrency/win32/thread.hpp` & `zmesh-1.7.0/zi_lib/zi/concurrency/win32/thread.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/concurrency/win32/types.hpp` & `zmesh-1.7.0/zi_lib/zi/concurrency/win32/types.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/concurrency.hpp` & `zmesh-1.7.0/zi_lib/zi/concurrency.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/config/compiler/gcc.hpp` & `zmesh-1.7.0/zi_lib/zi/config/compiler/gcc.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/config/compiler/msvc.hpp` & `zmesh-1.7.0/zi_lib/zi/config/compiler/msvc.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/config/config.hpp` & `zmesh-1.7.0/zi_lib/zi/config/config.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/config/os/linux.hpp` & `zmesh-1.7.0/zi_lib/zi/config/os/linux.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/config/os/macos.hpp` & `zmesh-1.7.0/zi_lib/zi/config/os/macos.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/config/os/windows.hpp` & `zmesh-1.7.0/zi_lib/zi/config/os/windows.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/config/posix.hpp` & `zmesh-1.7.0/zi_lib/zi/config/posix.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/cstdint.hpp` & `zmesh-1.7.0/zi_lib/zi/cstdint.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/debug/assert.hpp` & `zmesh-1.7.0/zi_lib/zi/debug/assert.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/debug/detail/demangle.hpp` & `zmesh-1.7.0/zi_lib/zi/debug/detail/demangle.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/debug/printable_type.hpp` & `zmesh-1.7.0/zi_lib/zi/debug/printable_type.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/debug/printable_value.hpp` & `zmesh-1.7.0/zi_lib/zi/debug/printable_value.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/detail/global_function.hpp` & `zmesh-1.7.0/zi_lib/zi/detail/global_function.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/detail/identity.hpp` & `zmesh-1.7.0/zi_lib/zi/detail/identity.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/detail/member_function.hpp` & `zmesh-1.7.0/zi_lib/zi/detail/member_function.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/detail/member_variable.hpp` & `zmesh-1.7.0/zi_lib/zi/detail/member_variable.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/disjoint_sets/disjoint_sets.hpp` & `zmesh-1.7.0/zi_lib/zi/disjoint_sets/disjoint_sets.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/enable_shared_from_this.hpp` & `zmesh-1.7.0/zi_lib/zi/enable_shared_from_this.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/enable_singleton_from_this.hpp` & `zmesh-1.7.0/zi_lib/zi/enable_singleton_from_this.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/for_each.hpp` & `zmesh-1.7.0/zi_lib/zi/for_each.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/function.hpp` & `zmesh-1.7.0/zi_lib/zi/function.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/gl/camera.hpp` & `zmesh-1.7.0/zi_lib/zi/gl/camera.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/gl/detail/config.hpp` & `zmesh-1.7.0/zi_lib/zi/gl/detail/config.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/gl/detail/gl_prefix.hpp` & `zmesh-1.7.0/zi_lib/zi/gl/detail/gl_prefix.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/gl/detail/gl_suffix.hpp` & `zmesh-1.7.0/zi_lib/zi/gl/detail/gl_suffix.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/gl/detail/types.hpp` & `zmesh-1.7.0/zi_lib/zi/gl/detail/types.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/gl/example/example.cpp` & `zmesh-1.7.0/zi_lib/zi/gl/example/example.cpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/gl/gl.hpp` & `zmesh-1.7.0/zi_lib/zi/gl/gl.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/gl/gl_1_1.hpp` & `zmesh-1.7.0/zi_lib/zi/gl/gl_1_1.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/gl/gl_1_2.hpp` & `zmesh-1.7.0/zi_lib/zi/gl/gl_1_2.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/gl/gl_1_3.hpp` & `zmesh-1.7.0/zi_lib/zi/gl/gl_1_3.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/gl/gl_arb_imaging.hpp` & `zmesh-1.7.0/zi_lib/zi/gl/gl_arb_imaging.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/gl/glu.hpp` & `zmesh-1.7.0/zi_lib/zi/gl/glu.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/gl/glut.hpp` & `zmesh-1.7.0/zi_lib/zi/gl/glut.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/graph/bipartite_matching.hpp` & `zmesh-1.7.0/zi_lib/zi/graph/bipartite_matching.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/graph/strongly_connected_components.hpp` & `zmesh-1.7.0/zi_lib/zi/graph/strongly_connected_components.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/hash.hpp` & `zmesh-1.7.0/zi_lib/zi/hash.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/heap/binary_heap.hpp` & `zmesh-1.7.0/zi_lib/zi/heap/binary_heap.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/heap/detail/binary_heap_impl.hpp` & `zmesh-1.7.0/zi_lib/zi/heap/detail/binary_heap_impl.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/heap/detail/binary_heap_impl2.hpp` & `zmesh-1.7.0/zi_lib/zi/heap/detail/binary_heap_impl2.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/heap/simple_binary_heap.hpp` & `zmesh-1.7.0/zi_lib/zi/heap/simple_binary_heap.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/heap/test/binary_heap_test.cpp` & `zmesh-1.7.0/zi_lib/zi/heap/test/binary_heap_test.cpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/heap/test/simple_binary_heap_test.cpp` & `zmesh-1.7.0/zi_lib/zi/heap/test/simple_binary_heap_test.cpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/logging.hpp` & `zmesh-1.7.0/zi_lib/zi/logging.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/math/bit_reverse.hpp` & `zmesh-1.7.0/zi_lib/zi/math/bit_reverse.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/math/constants.hpp` & `zmesh-1.7.0/zi_lib/zi/math/constants.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/math/fast_log.hpp` & `zmesh-1.7.0/zi_lib/zi/math/fast_log.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/math/integral_log2.hpp` & `zmesh-1.7.0/zi_lib/zi/math/integral_log2.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/math/transforms/detail/fft8.hpp` & `zmesh-1.7.0/zi_lib/zi/math/transforms/detail/fft8.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/math/transforms/detail/fft_radix2.hpp` & `zmesh-1.7.0/zi_lib/zi/math/transforms/detail/fft_radix2.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/math/transforms/detail/fft_splitradix.hpp` & `zmesh-1.7.0/zi_lib/zi/math/transforms/detail/fft_splitradix.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/math/transforms/detail/permuter.hpp` & `zmesh-1.7.0/zi_lib/zi/math/transforms/detail/permuter.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/math/transforms/detail/roots_table.hpp` & `zmesh-1.7.0/zi_lib/zi/math/transforms/detail/roots_table.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/math/transforms/detail/size_log2.hpp` & `zmesh-1.7.0/zi_lib/zi/math/transforms/detail/size_log2.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/mem_fn.hpp` & `zmesh-1.7.0/zi_lib/zi/mem_fn.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/mesh/detail/all_equal.hpp` & `zmesh-1.7.0/zi_lib/zi/mesh/detail/all_equal.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/mesh/detail/marching_cubes_tables.hpp` & `zmesh-1.7.0/zi_lib/zi/mesh/detail/marching_cubes_tables.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/mesh/detail/mc_tables.hpp` & `zmesh-1.7.0/zi_lib/zi/mesh/detail/mc_tables.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/mesh/detail/packed_coordinate.hpp` & `zmesh-1.7.0/zi_lib/zi/mesh/detail/packed_coordinate.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/mesh/detail/qmetric.hpp` & `zmesh-1.7.0/zi_lib/zi/mesh/detail/qmetric.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/mesh/detail/quadratic.hpp` & `zmesh-1.7.0/zi_lib/zi/mesh/detail/quadratic.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/mesh/detail/tri_mesh_edge.hpp` & `zmesh-1.7.0/zi_lib/zi/mesh/detail/tri_mesh_edge.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/mesh/detail/tri_mesh_face.hpp` & `zmesh-1.7.0/zi_lib/zi/mesh/detail/tri_mesh_face.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/mesh/detail/tri_mesh_vertex.hpp` & `zmesh-1.7.0/zi_lib/zi/mesh/detail/tri_mesh_vertex.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/mesh/face_mesh.hpp` & `zmesh-1.7.0/zi_lib/zi/mesh/face_mesh.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/mesh/int_mesh.hpp` & `zmesh-1.7.0/zi_lib/zi/mesh/int_mesh.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/mesh/marching_cubes.hpp` & `zmesh-1.7.0/zi_lib/zi/mesh/marching_cubes.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/mesh/network_sort.hpp` & `zmesh-1.7.0/zi_lib/zi/mesh/network_sort.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/mesh/quadratic_simplifier.hpp` & `zmesh-1.7.0/zi_lib/zi/mesh/quadratic_simplifier.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/mesh/tri_list.hpp` & `zmesh-1.7.0/zi_lib/zi/mesh/tri_list.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/mesh/tri_mesh.hpp` & `zmesh-1.7.0/zi_lib/zi/mesh/tri_mesh.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/mesh/tri_stripper.hpp` & `zmesh-1.7.0/zi_lib/zi/mesh/tri_stripper.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/meta/and.hpp` & `zmesh-1.7.0/zi_lib/zi/meta/and.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/meta/bool.hpp` & `zmesh-1.7.0/zi_lib/zi/meta/bool.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/meta/enable_if.hpp` & `zmesh-1.7.0/zi_lib/zi/meta/enable_if.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/meta/false_type.hpp` & `zmesh-1.7.0/zi_lib/zi/meta/false_type.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/meta/if.hpp` & `zmesh-1.7.0/zi_lib/zi/meta/if.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/meta/meta.hpp` & `zmesh-1.7.0/zi_lib/zi/meta/meta.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/meta/null_type.hpp` & `zmesh-1.7.0/zi_lib/zi/meta/null_type.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/meta/or.hpp` & `zmesh-1.7.0/zi_lib/zi/meta/or.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/meta/true_type.hpp` & `zmesh-1.7.0/zi_lib/zi/meta/true_type.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/mutex.hpp` & `zmesh-1.7.0/zi_lib/zi/mutex.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/non_copyable.hpp` & `zmesh-1.7.0/zi_lib/zi/non_copyable.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/parallel/algorithm.hpp` & `zmesh-1.7.0/zi_lib/zi/parallel/algorithm.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/parallel/numeric.hpp` & `zmesh-1.7.0/zi_lib/zi/parallel/numeric.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/random.hpp` & `zmesh-1.7.0/zi_lib/zi/random.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/ref.hpp` & `zmesh-1.7.0/zi_lib/zi/ref.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/result_of.hpp` & `zmesh-1.7.0/zi_lib/zi/result_of.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/shared_ptr.hpp` & `zmesh-1.7.0/zi_lib/zi/shared_ptr.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/singleton.hpp` & `zmesh-1.7.0/zi_lib/zi/singleton.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/static_assert.hpp` & `zmesh-1.7.0/zi_lib/zi/static_assert.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/system/config.hpp` & `zmesh-1.7.0/zi_lib/zi/system/config.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/system/daemon.hpp` & `zmesh-1.7.0/zi_lib/zi/system/daemon.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/system/detail/cerrno_code.hpp` & `zmesh-1.7.0/zi_lib/zi/system/detail/cerrno_code.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/system/detail/cpu_count.hpp` & `zmesh-1.7.0/zi_lib/zi/system/detail/cpu_count.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/system/detail/get_hostname.hpp` & `zmesh-1.7.0/zi_lib/zi/system/detail/get_hostname.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/system/detail/get_username.hpp` & `zmesh-1.7.0/zi_lib/zi/system/detail/get_username.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/system/detail/linux_errno_code.hpp` & `zmesh-1.7.0/zi_lib/zi/system/detail/linux_errno_code.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/system/detail/memory_size.hpp` & `zmesh-1.7.0/zi_lib/zi/system/detail/memory_size.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/system/detail/memory_usage.hpp` & `zmesh-1.7.0/zi_lib/zi/system/detail/memory_usage.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/system/detail/win32_errno_code.hpp` & `zmesh-1.7.0/zi_lib/zi/system/detail/win32_errno_code.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/system/error.hpp` & `zmesh-1.7.0/zi_lib/zi/system/error.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/system/example/example.cpp` & `zmesh-1.7.0/zi_lib/zi/system/example/example.cpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/system/system.hpp` & `zmesh-1.7.0/zi_lib/zi/system/system.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/system.hpp` & `zmesh-1.7.0/zi_lib/zi/system.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/test/Makefile` & `zmesh-1.7.0/zi_lib/zi/test/Makefile`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/test/Makefile-include-mingw32` & `zmesh-1.7.0/zi_lib/zi/test/Makefile-include-mingw32`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/test/Makefile-include-nix` & `zmesh-1.7.0/zi_lib/zi/test/Makefile-include-nix`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/test/Makefile-include-wine` & `zmesh-1.7.0/zi_lib/zi/test/Makefile-include-wine`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/test/Makefile-mingw32` & `zmesh-1.7.0/zi_lib/zi/test/Makefile-mingw32`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/test/Makefile-nix-mingw32` & `zmesh-1.7.0/zi_lib/zi/test/Makefile-nix-mingw32`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/test/Makefile-tmp` & `zmesh-1.7.0/zi_lib/zi/test/Makefile-tmp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/test/Makefile-wine` & `zmesh-1.7.0/zi_lib/zi/test/Makefile-wine`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/test.hpp` & `zmesh-1.7.0/zi_lib/zi/test.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/time/config.hpp` & `zmesh-1.7.0/zi_lib/zi/time/config.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/time/interval.hpp` & `zmesh-1.7.0/zi_lib/zi/time/interval.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/time/now.hpp` & `zmesh-1.7.0/zi_lib/zi/time/now.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/time/process_timer.hpp` & `zmesh-1.7.0/zi_lib/zi/time/process_timer.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/time/time.hpp` & `zmesh-1.7.0/zi_lib/zi/time/time.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/time/time_units.hpp` & `zmesh-1.7.0/zi_lib/zi/time/time_units.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/time/time_utils.hpp` & `zmesh-1.7.0/zi_lib/zi/time/time_utils.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/time/timer.hpp` & `zmesh-1.7.0/zi_lib/zi/time/timer.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/time/wall_timer.hpp` & `zmesh-1.7.0/zi_lib/zi/time/wall_timer.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/time.hpp` & `zmesh-1.7.0/zi_lib/zi/time.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/timer.hpp` & `zmesh-1.7.0/zi_lib/zi/timer.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/tuple.hpp` & `zmesh-1.7.0/zi_lib/zi/tuple.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/type_traits.hpp` & `zmesh-1.7.0/zi_lib/zi/type_traits.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/typeof.hpp` & `zmesh-1.7.0/zi_lib/zi/typeof.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/unittest.hpp` & `zmesh-1.7.0/zi_lib/zi/unittest.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/unordered_map.hpp` & `zmesh-1.7.0/zi_lib/zi/unordered_map.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/unordered_set.hpp` & `zmesh-1.7.0/zi_lib/zi/unordered_set.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/utility/address_of.hpp` & `zmesh-1.7.0/zi_lib/zi/utility/address_of.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/utility/assert.hpp` & `zmesh-1.7.0/zi_lib/zi/utility/assert.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/utility/binary_printer.hpp` & `zmesh-1.7.0/zi_lib/zi/utility/binary_printer.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/utility/container_utilities.hpp` & `zmesh-1.7.0/zi_lib/zi/utility/container_utilities.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/utility/deferred_instantiation.hpp` & `zmesh-1.7.0/zi_lib/zi/utility/deferred_instantiation.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/utility/detail/bare_type.hpp` & `zmesh-1.7.0/zi_lib/zi/utility/detail/bare_type.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/utility/detail/dummy.hpp` & `zmesh-1.7.0/zi_lib/zi/utility/detail/dummy.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/utility/detail/empty_type.hpp` & `zmesh-1.7.0/zi_lib/zi/utility/detail/empty_type.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/utility/detail/get_instance.hpp` & `zmesh-1.7.0/zi_lib/zi/utility/detail/get_instance.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/utility/detail/nbyte_int.hpp` & `zmesh-1.7.0/zi_lib/zi/utility/detail/nbyte_int.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/utility/detail/not_this_type.hpp` & `zmesh-1.7.0/zi_lib/zi/utility/detail/not_this_type.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/utility/detail/whatever.hpp` & `zmesh-1.7.0/zi_lib/zi/utility/detail/whatever.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/utility/detail/yes_no_type.hpp` & `zmesh-1.7.0/zi_lib/zi/utility/detail/yes_no_type.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/utility/enable_if.hpp` & `zmesh-1.7.0/zi_lib/zi/utility/enable_if.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/utility/enable_singleton_of_this.hpp` & `zmesh-1.7.0/zi_lib/zi/utility/enable_singleton_of_this.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/utility/exception.hpp` & `zmesh-1.7.0/zi_lib/zi/utility/exception.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/utility/for_each.hpp` & `zmesh-1.7.0/zi_lib/zi/utility/for_each.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/utility/is_complex.hpp` & `zmesh-1.7.0/zi_lib/zi/utility/is_complex.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/utility/is_printable.hpp` & `zmesh-1.7.0/zi_lib/zi/utility/is_printable.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/utility/natural_compare.hpp` & `zmesh-1.7.0/zi_lib/zi/utility/natural_compare.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/utility/non_copyable.hpp` & `zmesh-1.7.0/zi_lib/zi/utility/non_copyable.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/utility/robin_hood.hpp` & `zmesh-1.7.0/zi_lib/zi/utility/robin_hood.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/utility/singleton.hpp` & `zmesh-1.7.0/zi_lib/zi/utility/singleton.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/utility/static_and.hpp` & `zmesh-1.7.0/zi_lib/zi/utility/static_and.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/utility/static_assert.hpp` & `zmesh-1.7.0/zi_lib/zi/utility/static_assert.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/utility/static_if.hpp` & `zmesh-1.7.0/zi_lib/zi/utility/static_if.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/utility/static_or.hpp` & `zmesh-1.7.0/zi_lib/zi/utility/static_or.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/utility/string_printf.hpp` & `zmesh-1.7.0/zi_lib/zi/utility/string_printf.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/utility/test/address_of_test.cpp` & `zmesh-1.7.0/zi_lib/zi/utility/test/address_of_test.cpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/utility/test/enable_if_test.cpp` & `zmesh-1.7.0/zi_lib/zi/utility/test/enable_if_test.cpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/utility/test/is_printable_test.cpp` & `zmesh-1.7.0/zi_lib/zi/utility/test/is_printable_test.cpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/utility/this_function.hpp` & `zmesh-1.7.0/zi_lib/zi/utility/this_function.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/utility/value_iterator.hpp` & `zmesh-1.7.0/zi_lib/zi/utility/value_iterator.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/vl/detail/enable_if.hpp` & `zmesh-1.7.0/zi_lib/zi/vl/detail/enable_if.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/vl/detail/householder.hpp` & `zmesh-1.7.0/zi_lib/zi/vl/detail/householder.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/vl/detail/invert.hpp` & `zmesh-1.7.0/zi_lib/zi/vl/detail/invert.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/vl/detail/jacobi.hpp` & `zmesh-1.7.0/zi_lib/zi/vl/detail/jacobi.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/vl/detail/mat_lookup_table.hpp` & `zmesh-1.7.0/zi_lib/zi/vl/detail/mat_lookup_table.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/vl/detail/promote.hpp` & `zmesh-1.7.0/zi_lib/zi/vl/detail/promote.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/vl/mat.hpp` & `zmesh-1.7.0/zi_lib/zi/vl/mat.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/vl/mat_functions.hpp` & `zmesh-1.7.0/zi_lib/zi/vl/mat_functions.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/vl/quat.hpp` & `zmesh-1.7.0/zi_lib/zi/vl/quat.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/vl/quat_functions.hpp` & `zmesh-1.7.0/zi_lib/zi/vl/quat_functions.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/vl/vec.hpp` & `zmesh-1.7.0/zi_lib/zi/vl/vec.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/vl/vec_functions.hpp` & `zmesh-1.7.0/zi_lib/zi/vl/vec_functions.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/vl/vl.hpp` & `zmesh-1.7.0/zi_lib/zi/vl/vl.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/watershed/quickie.hpp` & `zmesh-1.7.0/zi_lib/zi/watershed/quickie.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/watershed/watershed.hpp` & `zmesh-1.7.0/zi_lib/zi/watershed/watershed.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/zargs/arguments.hpp` & `zmesh-1.7.0/zi_lib/zi/zargs/arguments.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/zargs/detail/boost_lexical_cast.hpp` & `zmesh-1.7.0/zi_lib/zi/zargs/detail/boost_lexical_cast.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/zargs/detail/lexical_cast.hpp` & `zmesh-1.7.0/zi_lib/zi/zargs/detail/lexical_cast.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/zargs/detail/simple_lexical_cast.hpp` & `zmesh-1.7.0/zi_lib/zi/zargs/detail/simple_lexical_cast.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/zargs/detail/string_utils.hpp` & `zmesh-1.7.0/zi_lib/zi/zargs/detail/string_utils.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/zargs/matcher.hpp` & `zmesh-1.7.0/zi_lib/zi/zargs/matcher.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/zargs/parser.hpp` & `zmesh-1.7.0/zi_lib/zi/zargs/parser.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/zargs/zargs.hpp` & `zmesh-1.7.0/zi_lib/zi/zargs/zargs.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/zlog/example/example.cpp` & `zmesh-1.7.0/zi_lib/zi/zlog/example/example.cpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/zlog/example/example_other.cpp` & `zmesh-1.7.0/zi_lib/zi/zlog/example/example_other.cpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/zlog/log_printf.hpp` & `zmesh-1.7.0/zi_lib/zi/zlog/log_printf.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/zlog/logs.hpp` & `zmesh-1.7.0/zi_lib/zi/zlog/logs.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/zlog/registry.hpp` & `zmesh-1.7.0/zi_lib/zi/zlog/registry.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/zlog/sink.hpp` & `zmesh-1.7.0/zi_lib/zi/zlog/sink.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/zlog/test/token_sink_test.cpp` & `zmesh-1.7.0/zi_lib/zi/zlog/test/token_sink_test.cpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/zlog/token.hpp` & `zmesh-1.7.0/zi_lib/zi/zlog/token.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/zlog/zlog.hpp` & `zmesh-1.7.0/zi_lib/zi/zlog/zlog.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/zpp/count_args.hpp` & `zmesh-1.7.0/zi_lib/zi/zpp/count_args.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/zpp/glue.hpp` & `zmesh-1.7.0/zi_lib/zi/zpp/glue.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/zpp/stringify.hpp` & `zmesh-1.7.0/zi_lib/zi/zpp/stringify.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/zunit/checker.hpp` & `zmesh-1.7.0/zi_lib/zi/zunit/checker.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/zunit/config.hpp` & `zmesh-1.7.0/zi_lib/zi/zunit/config.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/zunit/exception.hpp` & `zmesh-1.7.0/zi_lib/zi/zunit/exception.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/zunit/expect_xxx.hpp` & `zmesh-1.7.0/zi_lib/zi/zunit/expect_xxx.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/zunit/macros.hpp` & `zmesh-1.7.0/zi_lib/zi/zunit/macros.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/zunit/main.hpp` & `zmesh-1.7.0/zi_lib/zi/zunit/main.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/zunit/main.ipp` & `zmesh-1.7.0/zi_lib/zi/zunit/main.ipp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/zunit/registry.hpp` & `zmesh-1.7.0/zi_lib/zi/zunit/registry.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/zunit/tags.hpp` & `zmesh-1.7.0/zi_lib/zi/zunit/tags.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/zunit/test_case.hpp` & `zmesh-1.7.0/zi_lib/zi/zunit/test_case.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/zunit/test_suite.hpp` & `zmesh-1.7.0/zi_lib/zi/zunit/test_suite.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/zunit/test_suite_tpl.hpp` & `zmesh-1.7.0/zi_lib/zi/zunit/test_suite_tpl.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zi_lib/zi/zunit/zunit.hpp` & `zmesh-1.7.0/zi_lib/zi/zunit/zunit.hpp`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zmesh/_zmesh.pyx` & `zmesh-1.7.0/zmesh/_zmesh.pyx`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,10 @@
+# cython:language_level = 3
 # distutils: language = c++
+import cython
 
 from libc.stdint cimport uint64_t, uint32_t, uint16_t, uint8_t
 from libcpp.vector cimport vector
 from libcpp cimport bool
 
 import operator
 from functools import reduce
@@ -15,43 +17,65 @@
   cdef struct MeshObject:
     vector[float] points
     vector[float] normals
     vector[unsigned int] faces
 
   cdef cppclass CMesher[P,L,S]:
     CMesher(vector[float] voxel_res) except +
-    void mesh(L*, unsigned int, unsigned int, unsigned int, bool c_order)
+    void mesh(
+      L* data, 
+      unsigned int sx, 
+      unsigned int sy, 
+      unsigned int sz, 
+      bool c_order
+    )
     vector[L] ids()
-    MeshObject get_mesh(L segid, bool normals, int simplification_factor, int max_simplification_error)
+    MeshObject get_mesh(
+      L segid, 
+      bool normals,
+      int simplification_factor, 
+      int max_simplification_error, 
+      bool transpose
+    )
     # NOTE: need to define triangle_t
     MeshObject simplify_points(
-      uint64_t* points, size_t Nv, 
-      bool normals, int simplification_factor, int max_simplification_error
+      uint64_t* points, 
+      size_t Nv, 
+      bool normals, 
+      int simplification_factor, 
+      int max_simplification_error
     )
     bool erase(L segid)
     void clear()
     P pack_coords(P x, P y, P z)
 
 class Mesher:
+  """
+  Represents a meshed volume. 
+
+  Call mesher.mesh(labels) then you can 
+  extract meshes from it using mesher.get(label).
+  """
   def __init__(self, voxel_res):
     self.voxel_res = voxel_res
     self._mesher = Mesher6464(self.voxel_res)
 
   @property
   def voxel_res(self):
     return self._voxel_res
 
   @voxel_res.setter
   def voxel_res(self, res):
     self._voxel_res = np.array(res, dtype=np.float32)
 
+  @cython.binding(True)
   def mesh(self, data, close=False):
     """
     Triggers the multi-label meshing process.
-    After the mesher has run, you can call get_mesh.
+    After the mesher has run, you can call mesher.get.
 
     data: 3d numpy array
     close: By default, meshes flush against the edge of
       the image will be left open on the sides that touch
       the boundary. If True, this ensures that all meshes
       produced will be closed.
     """
@@ -89,41 +113,79 @@
       elif nbytes == 1:
         MesherClass = Mesher3208
 
     self._mesher = MesherClass(self.voxel_res)
 
     return self._mesher.mesh(data)
 
+  @cython.binding(True)
   def ids(self):
     return self._mesher.ids()
 
+  @cython.binding(True)
   def get_mesh(
     self, mesh_id, normals=False, 
     simplification_factor=0, max_simplification_error=40,
     voxel_centered=False
   ):
     """
-    get_mesh(self, mesh_id, normals=False, simplification_factor=0, max_simplification_error=40)
+    NOTE: This function is deprecated. Please use "get" as 
+    this function transposes the mesh.
 
     mesh_id: the integer id of the mesh
     normals: whether to calculate vertex normals for the mesh
     simplification_factor: Try to reduce the number of triangles by this factor.
     max_simplification_error: maximum distance vertices are allowed to deviate from
       their original position. Units are physical, not voxels.
     voxel_centered: By default, the meshes produced will be centered at 0,0,0.
       If enabled, the meshes will be centered in the voxel at 0.5,0.5,0.5.
 
     Returns: Mesh
     """
     mesh = self._mesher.get_mesh(
-      mesh_id, normals, simplification_factor, max_simplification_error
+      mesh_id, normals, 
+      simplification_factor, max_simplification_error, 
+      transpose=True
     )
 
     return self._normalize_simplified_mesh(mesh, voxel_centered, physical=True)
-  
+
+  @cython.binding(True)
+  def get(
+    self, label, 
+    normals = False, 
+    reduction_factor = 0, 
+    max_error = None,
+    voxel_centered = False
+  ):
+    """
+    label: the integer id of the mesh
+    normals: whether to calculate vertex normals for the mesh
+    reduction_factor: Try to reduce the number of triangles by this integer factor. 
+      0 disables simplification.
+    max_error: maximum distance vertices are allowed to deviate from
+      their original position. Units are physical, not voxels. If None, automatically
+      is set to at most one voxel distortion based on the provided resolution.
+    voxel_centered: By default, the meshes produced will be centered at 0,0,0.
+      If enabled, the meshes will be centered in the voxel at 0.5,0.5,0.5.
+
+    Returns: Mesh
+    """
+    # automatically select one voxel max distortion
+    if max_error is None:
+      max_error = self.voxel_res.max()
+
+    mesh = self._mesher.get_mesh(
+      label, normals, 
+      reduction_factor, max_error,
+      transpose=False
+    )
+
+    return self._normalize_simplified_mesh(mesh, voxel_centered, physical=True)
+
   def _normalize_simplified_mesh(self, mesh, voxel_centered, physical):
     points = np.array(mesh['points'], dtype=np.float32)
     Nv = points.size // 3
     Nf = len(mesh['faces']) // 3
 
     points = points.reshape(Nv, 3)
     if not physical:
@@ -136,29 +198,32 @@
     
     normals = None
     if mesh['normals']:
       normals = np.array(mesh['normals'], dtype=np.float32).reshape(Nv, 3)
 
     return Mesh(points, faces, normals)
 
+  @cython.binding(True)
   def compute_normals(self, mesh):
     """
-    Mesh compute_normals(mesh)
-
     Returns: Mesh with normals computed
     """
     return self.simplify(mesh, reduction_factor=0, max_error=0, compute_normals=True)
 
   def simplify(
     self, mesh, int reduction_factor=0, 
     int max_error=40, compute_normals=False,
     voxel_centered=False
   ):
     """
-    Mesh simplify(mesh, reduction_factor=0, max_error=40)
+    Mesh simplify(
+      mesh, reduction_factor=0, 
+      max_error=40, compute_normals=False, 
+      voxel_centered=False
+    )
 
     Given a mesh object (either zmesh.Mesh or another object that has
     mesh.vertices and mesh.faces implemented as numpy arrays), apply
     the quadratic edge collapse algorithm. 
 
     Note: the maximum range spread between vertex values (in x, y, or z)
     is 2^20. The simplifier cannot represent values outside that range.
@@ -217,18 +282,19 @@
 
     cdef int i = 0
     if min_vertex != 0:
       for i in range(len(result.points)):
         result.points[i] += min_vertex
 
     return self._normalize_simplified_mesh(result, voxel_centered, physical=False)
-
+  
   def clear(self):
     self._mesher.clear()
-   
+  
+  @cython.binding(True) 
   def erase(self, segid):
     return self._mesher.erase(segid)
 
 def reshape(arr, shape, order=None):
   """
   If the array is contiguous, attempt an in place reshape
   rather than potentially making a copy.
@@ -269,15 +335,15 @@
 # The pattern is: Mesher[PositionType bits][LabelType bits]
 # 64 bit position type can represent very large arrays
 # 32 bit can represent 1023 x 1023 x 511 arrays
 cdef class Mesher3208:
   cdef CMesher[uint32_t, uint8_t, float] *ptr      # hold a C++ instance which we're wrapping
 
   def __cinit__(self, voxel_res):
-    self.ptr = new CMesher[uint32_t, uint8_t, float](voxel_res.astype(np.float32))
+    self.ptr = new CMesher[uint32_t, uint8_t, float](voxel_res)
 
   def __dealloc__(self):
     del self.ptr
 
   def mesh(self, data):
     cdef cnp.ndarray[uint8_t, ndim=1] flat_data = reshape(data, (data.size,)).view(np.uint8)
     self.ptr.mesh(
@@ -285,28 +351,28 @@
       data.shape[0], data.shape[1], data.shape[2],
       data.flags.c_contiguous
     )
 
   def ids(self):
     return self.ptr.ids()
   
-  def get_mesh(self, mesh_id, normals=False, simplification_factor=0, max_simplification_error=40):
-    return self.ptr.get_mesh(mesh_id, normals, simplification_factor, max_simplification_error)
+  def get_mesh(self, mesh_id, normals=False, simplification_factor=0, max_simplification_error=40, transpose=True):
+    return self.ptr.get_mesh(mesh_id, normals, simplification_factor, max_simplification_error, transpose)
   
   def clear(self):
     self.ptr.clear()
 
   def erase(self, mesh_id):
     return self.ptr.erase(mesh_id)
 
 cdef class Mesher3216:
   cdef CMesher[uint32_t, uint16_t, float] *ptr      # hold a C++ instance which we're wrapping
 
   def __cinit__(self, voxel_res):
-    self.ptr = new CMesher[uint32_t, uint16_t, float](voxel_res.astype(np.float32))
+    self.ptr = new CMesher[uint32_t, uint16_t, float](voxel_res)
 
   def __dealloc__(self):
     del self.ptr
 
   def mesh(self, data):
     cdef cnp.ndarray[uint16_t, ndim=1] flat_data = reshape(data, (data.size,)).view(np.uint16)
     self.ptr.mesh(
@@ -314,28 +380,28 @@
       data.shape[0], data.shape[1], data.shape[2],
       data.flags.c_contiguous
     )
 
   def ids(self):
     return self.ptr.ids()
   
-  def get_mesh(self, mesh_id, normals=False, simplification_factor=0, max_simplification_error=40):
-    return self.ptr.get_mesh(mesh_id, normals, simplification_factor, max_simplification_error)
+  def get_mesh(self, mesh_id, normals=False, simplification_factor=0, max_simplification_error=40, transpose=True):
+    return self.ptr.get_mesh(mesh_id, normals, simplification_factor, max_simplification_error, transpose)
   
   def clear(self):
     self.ptr.clear()
 
   def erase(self, mesh_id):
     return self.ptr.erase(mesh_id)
 
 cdef class Mesher3232:
   cdef CMesher[uint32_t, uint32_t, float] *ptr      # hold a C++ instance which we're wrapping
 
   def __cinit__(self, voxel_res):
-    self.ptr = new CMesher[uint32_t, uint32_t, float](voxel_res.astype(np.float32))
+    self.ptr = new CMesher[uint32_t, uint32_t, float](voxel_res)
 
   def __dealloc__(self):
     del self.ptr
 
   def mesh(self, data):
     cdef cnp.ndarray[uint32_t, ndim=1] flat_data = reshape(data, (data.size,)).view(np.uint32)
     self.ptr.mesh(
@@ -343,28 +409,28 @@
       data.shape[0], data.shape[1], data.shape[2],
       data.flags.c_contiguous
     )
 
   def ids(self):
     return self.ptr.ids()
   
-  def get_mesh(self, mesh_id, normals=False, simplification_factor=0, max_simplification_error=40):
-    return self.ptr.get_mesh(mesh_id, normals, simplification_factor, max_simplification_error)
+  def get_mesh(self, mesh_id, normals=False, simplification_factor=0, max_simplification_error=40, transpose=True):
+    return self.ptr.get_mesh(mesh_id, normals, simplification_factor, max_simplification_error, transpose)
   
   def clear(self):
     self.ptr.clear()
 
   def erase(self, mesh_id):
     return self.ptr.erase(mesh_id)
 
 cdef class Mesher3264:
   cdef CMesher[uint32_t, uint64_t, float] *ptr      # hold a C++ instance which we're wrapping
 
   def __cinit__(self, voxel_res):
-    self.ptr = new CMesher[uint32_t, uint64_t, float](voxel_res.astype(np.float32))
+    self.ptr = new CMesher[uint32_t, uint64_t, float](voxel_res)
 
   def __dealloc__(self):
     del self.ptr
 
   def mesh(self, data):
     cdef cnp.ndarray[uint64_t, ndim=1] flat_data = reshape(data, (data.size,)).view(np.uint64)
     self.ptr.mesh(
@@ -372,28 +438,28 @@
       data.shape[0], data.shape[1], data.shape[2],
       data.flags.c_contiguous
     )
 
   def ids(self):
     return self.ptr.ids()
   
-  def get_mesh(self, mesh_id, normals=False, simplification_factor=0, max_simplification_error=40):
-    return self.ptr.get_mesh(mesh_id, normals, simplification_factor, max_simplification_error)
+  def get_mesh(self, mesh_id, normals=False, simplification_factor=0, max_simplification_error=40, transpose=True):
+    return self.ptr.get_mesh(mesh_id, normals, simplification_factor, max_simplification_error, transpose)
   
   def clear(self):
     self.ptr.clear()
 
   def erase(self, mesh_id):
     return self.ptr.erase(mesh_id)
 
 cdef class Mesher6408:
   cdef CMesher[uint64_t, uint8_t, float] *ptr      # hold a C++ instance which we're wrapping
 
   def __cinit__(self, voxel_res):
-    self.ptr = new CMesher[uint64_t, uint8_t, float](voxel_res.astype(np.float32))
+    self.ptr = new CMesher[uint64_t, uint8_t, float](voxel_res)
 
   def __dealloc__(self):
     del self.ptr
 
   def mesh(self, data):
     cdef cnp.ndarray[uint8_t, ndim=1] flat_data = reshape(data, (data.size,)).view(np.uint8)
     self.ptr.mesh(
@@ -401,28 +467,28 @@
       data.shape[0], data.shape[1], data.shape[2],
       data.flags.c_contiguous
     )
 
   def ids(self):
     return self.ptr.ids()
   
-  def get_mesh(self, mesh_id, normals=False, simplification_factor=0, max_simplification_error=40):
-    return self.ptr.get_mesh(mesh_id, normals, simplification_factor, max_simplification_error)
+  def get_mesh(self, mesh_id, normals=False, simplification_factor=0, max_simplification_error=40, transpose=True):
+    return self.ptr.get_mesh(mesh_id, normals, simplification_factor, max_simplification_error, transpose)
   
   def clear(self):
     self.ptr.clear()
 
   def erase(self, mesh_id):
     return self.ptr.erase(mesh_id)
 
 cdef class Mesher6416:
   cdef CMesher[uint64_t, uint16_t, float] *ptr      # hold a C++ instance which we're wrapping
 
   def __cinit__(self, voxel_res):
-    self.ptr = new CMesher[uint64_t, uint16_t, float](voxel_res.astype(np.float32))
+    self.ptr = new CMesher[uint64_t, uint16_t, float](voxel_res)
 
   def __dealloc__(self):
     del self.ptr
 
   def mesh(self, data):
     cdef cnp.ndarray[uint16_t, ndim=1] flat_data = reshape(data, (data.size,)).view(np.uint16)
     self.ptr.mesh(
@@ -430,28 +496,28 @@
       data.shape[0], data.shape[1], data.shape[2],
       data.flags.c_contiguous
     )
 
   def ids(self):
     return self.ptr.ids()
   
-  def get_mesh(self, mesh_id, normals=False, simplification_factor=0, max_simplification_error=40):
-    return self.ptr.get_mesh(mesh_id, normals, simplification_factor, max_simplification_error)
+  def get_mesh(self, mesh_id, normals=False, simplification_factor=0, max_simplification_error=40, transpose=True):
+    return self.ptr.get_mesh(mesh_id, normals, simplification_factor, max_simplification_error, transpose)
   
   def clear(self):
     self.ptr.clear()
 
   def erase(self, mesh_id):
     return self.ptr.erase(mesh_id)
 
 cdef class Mesher6432:
   cdef CMesher[uint64_t, uint32_t, float] *ptr      # hold a C++ instance which we're wrapping
 
   def __cinit__(self, voxel_res):
-    self.ptr = new CMesher[uint64_t, uint32_t, float](voxel_res.astype(np.float32))
+    self.ptr = new CMesher[uint64_t, uint32_t, float](voxel_res)
 
   def __dealloc__(self):
     del self.ptr
 
   def mesh(self, data):
     cdef cnp.ndarray[uint32_t, ndim=1] flat_data = reshape(data, (data.size,)).view(np.uint32)
     self.ptr.mesh(
@@ -459,28 +525,28 @@
       data.shape[0], data.shape[1], data.shape[2],
       data.flags.c_contiguous
     )
 
   def ids(self):
     return self.ptr.ids()
   
-  def get_mesh(self, mesh_id, normals=False, simplification_factor=0, max_simplification_error=40):
-    return self.ptr.get_mesh(mesh_id, normals, simplification_factor, max_simplification_error)
+  def get_mesh(self, mesh_id, normals=False, simplification_factor=0, max_simplification_error=40, transpose=True):
+    return self.ptr.get_mesh(mesh_id, normals, simplification_factor, max_simplification_error, transpose)
   
   def clear(self):
     self.ptr.clear()
 
   def erase(self, mesh_id):
     return self.ptr.erase(mesh_id)
 
 cdef class Mesher6464:
   cdef CMesher[uint64_t, uint64_t, float] *ptr      # hold a C++ instance which we're wrapping
 
   def __cinit__(self, voxel_res):
-    self.ptr = new CMesher[uint64_t, uint64_t, float](voxel_res.astype(np.float32))
+    self.ptr = new CMesher[uint64_t, uint64_t, float](voxel_res)
 
   def __dealloc__(self):
     del self.ptr
 
   def mesh(self, data):
     cdef cnp.ndarray[uint64_t, ndim=1] flat_data = reshape(data, (data.size,)).view(np.uint64)
     self.ptr.mesh(
@@ -488,16 +554,16 @@
       data.shape[0], data.shape[1], data.shape[2],
       data.flags.c_contiguous
     )
 
   def ids(self):
     return self.ptr.ids()
   
-  def get_mesh(self, mesh_id, normals=False, simplification_factor=0, max_simplification_error=40):
-    return self.ptr.get_mesh(mesh_id, normals, simplification_factor, max_simplification_error)
+  def get_mesh(self, mesh_id, normals=False, simplification_factor=0, max_simplification_error=40, transpose=True):
+    return self.ptr.get_mesh(mesh_id, normals, simplification_factor, max_simplification_error, transpose)
   
   def clear(self):
     self.ptr.clear()
 
   def erase(self, mesh_id):
     return self.ptr.erase(mesh_id)
```

### Comparing `zmesh-1.6.2/zmesh/mesh.py` & `zmesh-1.7.0/zmesh/mesh.py`

 * *Files identical despite different names*

### Comparing `zmesh-1.6.2/zmesh.egg-info/SOURCES.txt` & `zmesh-1.7.0/zmesh.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -372,15 +372,14 @@
 zi_lib/zi/zunit/registry.hpp
 zi_lib/zi/zunit/tags.hpp
 zi_lib/zi/zunit/test_case.hpp
 zi_lib/zi/zunit/test_suite.hpp
 zi_lib/zi/zunit/test_suite_tpl.hpp
 zi_lib/zi/zunit/zunit.hpp
 zmesh/__init__.py
-zmesh/_zmesh.cpp
 zmesh/_zmesh.pyx
 zmesh/mesh.py
 zmesh.egg-info/PKG-INFO
 zmesh.egg-info/SOURCES.txt
 zmesh.egg-info/dependency_links.txt
 zmesh.egg-info/not-zip-safe
 zmesh.egg-info/pbr.json
```

