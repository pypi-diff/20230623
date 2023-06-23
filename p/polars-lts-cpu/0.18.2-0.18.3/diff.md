# Comparing `tmp/polars_lts_cpu-0.18.2.tar.gz` & `tmp/polars_lts_cpu-0.18.3.tar.gz`

## Comparing `polars_lts_cpu-0.18.2.tar` & `polars_lts_cpu-0.18.3.tar`

### file list

```diff
@@ -1,1240 +1,1241 @@
--rw-r--r--   0        0        0     1998 1970-01-01 00:00:00.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/Cargo.toml
--rw-r--r--   0     1001      123     1055 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/LICENSE
--rw-r--r--   0     1001      123      165 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/README.md
--rw-r--r--   0     1001      123       98 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/mod.rs
--rw-r--r--   0     1001      123     1219 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/operators/filter.rs
--rw-r--r--   0     1001      123     4103 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/operators/function.rs
--rw-r--r--   0     1001      123      266 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/operators/mod.rs
--rw-r--r--   0     1001      123      682 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/operators/pass.rs
--rw-r--r--   0     1001      123      548 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/operators/placeholder.rs
--rw-r--r--   0     1001      123     3553 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/operators/projection.rs
--rw-r--r--   0     1001      123     3559 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/operators/reproject.rs
--rw-r--r--   0     1001      123     6479 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sinks/file_sink.rs
--rw-r--r--   0     1001      123    11288 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/convert.rs
--rw-r--r--   0     1001      123     1207 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/count.rs
--rw-r--r--   0     1001      123     1888 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/first.rs
--rw-r--r--   0     1001      123     4554 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/interface.rs
--rw-r--r--   0     1001      123     1746 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/last.rs
--rw-r--r--   0     1001      123     5413 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/mean.rs
--rw-r--r--   0     1001      123     4951 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/min_max.rs
--rw-r--r--   0     1001      123      211 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/mod.rs
--rw-r--r--   0     1001      123      856 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/null.rs
--rw-r--r--   0     1001      123     4294 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/sum.rs
--rw-r--r--   0     1001      123     3030 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/eval.rs
--rw-r--r--   0     1001      123     7500 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/global.rs
--rw-r--r--   0     1001      123    13819 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/hash_table.rs
--rw-r--r--   0     1001      123     3243 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/mod.rs
--rw-r--r--   0     1001      123     2767 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/ooc_state.rs
--rw-r--r--   0     1001      123     6311 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/sink.rs
--rw-r--r--   0     1001      123     3116 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/source.rs
--rw-r--r--   0     1001      123    11264 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/thread_local.rs
--rw-r--r--   0     1001      123     2119 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sinks/groupby/mod.rs
--rw-r--r--   0     1001      123     4695 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sinks/groupby/ooc.rs
--rw-r--r--   0     1001      123     1887 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sinks/groupby/ooc_state.rs
--rw-r--r--   0     1001      123    20783 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sinks/groupby/primitive/mod.rs
--rw-r--r--   0     1001      123    23420 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sinks/groupby/string.rs
--rw-r--r--   0     1001      123     2457 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sinks/groupby/utils.rs
--rw-r--r--   0     1001      123     9239 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sinks/io.rs
--rw-r--r--   0     1001      123     5451 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sinks/joins/cross.rs
--rw-r--r--   0     1001      123    14279 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sinks/joins/generic_build.rs
--rw-r--r--   0     1001      123    11824 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sinks/joins/inner_left.rs
--rw-r--r--   0     1001      123      178 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sinks/joins/mod.rs
--rw-r--r--   0     1001      123     2241 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sinks/memory.rs
--rw-r--r--   0     1001      123      589 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sinks/mod.rs
--rw-r--r--   0     1001      123     1492 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sinks/ordered.rs
--rw-r--r--   0     1001      123     1824 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sinks/reproject.rs
--rw-r--r--   0     1001      123     3108 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sinks/slice.rs
--rw-r--r--   0     1001      123      130 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sinks/sort/mod.rs
--rw-r--r--   0     1001      123     6787 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sinks/sort/ooc.rs
--rw-r--r--   0     1001      123     7279 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sinks/sort/sink.rs
--rw-r--r--   0     1001      123     5953 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sinks/sort/sink_multiple.rs
--rw-r--r--   0     1001      123     3908 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sinks/sort/source.rs
--rw-r--r--   0     1001      123      635 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sinks/utils.rs
--rw-r--r--   0     1001      123     5984 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sources/csv.rs
--rw-r--r--   0     1001      123     1231 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sources/frame.rs
--rw-r--r--   0     1001      123      987 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sources/ipc_one_shot.rs
--rw-r--r--   0     1001      123      366 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sources/mod.rs
--rw-r--r--   0     1001      123     4335 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sources/parquet.rs
--rw-r--r--   0     1001      123     1146 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sources/reproject.rs
--rw-r--r--   0     1001      123     1022 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sources/union.rs
--rw-r--r--   0     1001      123      448 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/expressions.rs
--rw-r--r--   0     1001      123      272 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/lib.rs
--rw-r--r--   0     1001      123      719 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/operators/chunks.rs
--rw-r--r--   0     1001      123      474 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/operators/context.rs
--rw-r--r--   0     1001      123      223 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/operators/mod.rs
--rw-r--r--   0     1001      123      514 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/operators/operator.rs
--rw-r--r--   0     1001      123      626 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/operators/sink.rs
--rw-r--r--   0     1001      123      241 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/operators/source.rs
--rw-r--r--   0     1001      123        1 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/pipeline/config.rs
--rw-r--r--   0     1001      123    21304 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/pipeline/convert.rs
--rw-r--r--   0     1001      123    18204 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/pipeline/dispatcher.rs
--rw-r--r--   0     1001      123     1155 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/pipeline/mod.rs
--rw-r--r--   0        0        0     5971 1970-01-01 00:00:00.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/Cargo.toml
--rw-r--r--   0     1001      123     1055 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/LICENSE
--rw-r--r--   0     1001      123      358 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/README.md
--rw-r--r--   0     1001      123     1796 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/dot.rs
--rw-r--r--   0     1001      123     4479 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/dsl/eval.rs
--rw-r--r--   0     1001      123     5127 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/dsl/functions.rs
--rw-r--r--   0     1001      123      164 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/dsl/into.rs
--rw-r--r--   0     1001      123     6754 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/dsl/list.rs
--rw-r--r--   0     1001      123     2899 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/dsl/mod.rs
--rw-r--r--   0     1001      123     1182 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/frame/anonymous_scan.rs
--rw-r--r--   0     1001      123     9278 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/frame/csv.rs
--rw-r--r--   0     1001      123     4309 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/frame/file_list_reader.rs
--rw-r--r--   0     1001      123     2261 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/frame/ipc.rs
--rw-r--r--   0     1001      123    48867 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/frame/mod.rs
--rw-r--r--   0     1001      123     3414 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/frame/ndjson.rs
--rw-r--r--   0     1001      123     2734 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/frame/parquet.rs
--rw-r--r--   0     1001      123     2892 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/frame/pivot.rs
--rw-r--r--   0     1001      123      416 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/frame/python.rs
--rw-r--r--   0     1001      123     6376 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/lib.rs
--rw-r--r--   0     1001      123     1049 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/executors/cache.rs
--rw-r--r--   0     1001      123      776 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/executors/executor.rs
--rw-r--r--   0     1001      123      670 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/executors/ext_context.rs
--rw-r--r--   0     1001      123     1555 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/executors/filter.rs
--rw-r--r--   0     1001      123     3986 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/executors/groupby.rs
--rw-r--r--   0     1001      123     4125 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/executors/groupby_dynamic.rs
--rw-r--r--   0     1001      123    13580 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/executors/groupby_partitioned.rs
--rw-r--r--   0     1001      123     4883 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/executors/groupby_rolling.rs
--rw-r--r--   0     1001      123     5859 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/executors/join.rs
--rw-r--r--   0     1001      123     6753 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/executors/mod.rs
--rw-r--r--   0     1001      123     2045 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/executors/projection.rs
--rw-r--r--   0     1001      123     1677 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/executors/python_scan.rs
--rw-r--r--   0     1001      123     2854 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/executors/scan/csv.rs
--rw-r--r--   0     1001      123     1963 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/executors/scan/ipc.rs
--rw-r--r--   0     1001      123     4303 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/executors/scan/mod.rs
--rw-r--r--   0     1001      123     1209 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/executors/scan/ndjson.rs
--rw-r--r--   0     1001      123     2421 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/executors/scan/parquet.rs
--rw-r--r--   0     1001      123      548 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/executors/slice.rs
--rw-r--r--   0     1001      123     2197 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/executors/sort.rs
--rw-r--r--   0     1001      123     2015 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/executors/stack.rs
--rw-r--r--   0     1001      123      663 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/executors/udf.rs
--rw-r--r--   0     1001      123     4041 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/executors/union.rs
--rw-r--r--   0     1001      123      838 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/executors/unique.rs
--rw-r--r--   0     1001      123     1335 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/exotic.rs
--rw-r--r--   0     1001      123    21959 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/expressions/aggregation.rs
--rw-r--r--   0     1001      123     2689 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/expressions/alias.rs
--rw-r--r--   0     1001      123    18331 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/expressions/apply.rs
--rw-r--r--   0     1001      123    17197 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/expressions/binary.rs
--rw-r--r--   0     1001      123     2583 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/expressions/cache.rs
--rw-r--r--   0     1001      123     3153 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/expressions/cast.rs
--rw-r--r--   0     1001      123     6326 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/expressions/column.rs
--rw-r--r--   0     1001      123     1996 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/expressions/count.rs
--rw-r--r--   0     1001      123     5809 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/expressions/filter.rs
--rw-r--r--   0     1001      123     4131 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/expressions/group_iter.rs
--rw-r--r--   0     1001      123     5304 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/expressions/literal.rs
--rw-r--r--   0     1001      123    23566 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/expressions/mod.rs
--rw-r--r--   0     1001      123    10091 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/expressions/slice.rs
--rw-r--r--   0     1001      123     4332 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/expressions/sort.rs
--rw-r--r--   0     1001      123    13549 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/expressions/sortby.rs
--rw-r--r--   0     1001      123     8331 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/expressions/take.rs
--rw-r--r--   0     1001      123    14360 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/expressions/ternary.rs
--rw-r--r--   0     1001      123    31558 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/expressions/window.rs
--rw-r--r--   0     1001      123     2039 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/file_cache.rs
--rw-r--r--   0     1001      123      414 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/mod.rs
--rw-r--r--   0     1001      123     2005 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/node_timer.rs
--rw-r--r--   0     1001      123    24050 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/planner/expr.rs
--rw-r--r--   0     1001      123    20552 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/planner/lp.rs
--rw-r--r--   0     1001      123       87 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/planner/mod.rs
--rw-r--r--   0     1001      123     9647 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/state.rs
--rw-r--r--   0     1001      123     2535 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/streaming/checks.rs
--rw-r--r--   0     1001      123     9227 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/streaming/construct_pipeline.rs
--rw-r--r--   0     1001      123    15835 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/streaming/convert_alp.rs
--rw-r--r--   0     1001      123      116 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/streaming/mod.rs
--rw-r--r--   0     1001      123     5827 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/streaming/tree.rs
--rw-r--r--   0     1001      123      722 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/prelude.rs
--rw-r--r--   0     1001      123    14990 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/tests/aggregations.rs
--rw-r--r--   0     1001      123     2339 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/tests/arity.rs
--rw-r--r--   0     1001      123     7066 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/tests/cse.rs
--rw-r--r--   0     1001      123    12759 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/tests/io.rs
--rw-r--r--   0     1001      123     4166 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/tests/logical.rs
--rw-r--r--   0     1001      123     4273 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/tests/mod.rs
--rw-r--r--   0     1001      123    15680 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/tests/optimization_checks.rs
--rw-r--r--   0     1001      123     6772 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/tests/predicate_queries.rs
--rw-r--r--   0     1001      123     3165 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/tests/projection_queries.rs
--rw-r--r--   0     1001      123    47687 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/tests/queries.rs
--rw-r--r--   0     1001      123     9513 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/tests/streaming.rs
--rw-r--r--   0     1001      123     2893 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/tests/tpch.rs
--rw-r--r--   0     1001      123     1028 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/utils.rs
--rw-r--r--   0        0        0    10560 1970-01-01 00:00:00.000000 polars_lts_cpu-0.18.2/local_dependencies/polars/Cargo.toml
--rw-r--r--   0     1001      123     1055 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars/LICENSE
--rw-r--r--   0     1001      123     3472 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars/Makefile
--rw-r--r--   0     1001      123      215 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars/build.rs
--rw-r--r--   0     1001      123       78 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars/clippy.toml
--rw-r--r--   0     1001      123    17602 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars/src/docs/eager.rs
--rw-r--r--   0     1001      123     8794 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars/src/docs/lazy.rs
--rw-r--r--   0     1001      123       50 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars/src/docs/mod.rs
--rw-r--r--   0     1001      123     3797 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars/src/docs/performance.rs
--rw-r--r--   0     1001      123       59 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars/src/export.rs
--rw-r--r--   0     1001      123    20214 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars/src/lib.rs
--rw-r--r--   0     1001      123      387 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars/src/prelude.rs
--rw-r--r--   0     1001      123       54 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars/src/sql.rs
--rw-r--r--   0     1001      123     4272 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars/tests/it/core/date_like.rs
--rw-r--r--   0     1001      123     2401 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars/tests/it/core/groupby.rs
--rw-r--r--   0     1001      123    17836 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars/tests/it/core/joins.rs
--rw-r--r--   0     1001      123      545 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars/tests/it/core/list.rs
--rw-r--r--   0     1001      123      198 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars/tests/it/core/mod.rs
--rw-r--r--   0     1001      123       24 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars/tests/it/core/ops/mod.rs
--rw-r--r--   0     1001      123      457 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars/tests/it/core/ops/take.rs
--rw-r--r--   0     1001      123     6259 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars/tests/it/core/pivot.rs
--rw-r--r--   0     1001      123     1102 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars/tests/it/core/random.rs
--rw-r--r--   0     1001      123    11096 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars/tests/it/core/rolling_window.rs
--rw-r--r--   0     1001      123     1093 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars/tests/it/core/series.rs
--rw-r--r--   0     1001      123      370 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars/tests/it/core/utils.rs
--rw-r--r--   0     1001      123    30423 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars/tests/it/io/csv.rs
--rw-r--r--   0     1001      123     4490 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars/tests/it/io/ipc_stream.rs
--rw-r--r--   0     1001      123     7043 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars/tests/it/io/json.rs
--rw-r--r--   0     1001      123      378 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars/tests/it/io/mod.rs
--rw-r--r--   0     1001      123      531 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars/tests/it/io/parquet.rs
--rw-r--r--   0     1001      123     1530 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars/tests/it/joins.rs
--rw-r--r--   0     1001      123     2452 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars/tests/it/lazy/aggregation.rs
--rw-r--r--   0     1001      123      709 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars/tests/it/lazy/cse.rs
--rw-r--r--   0     1001      123      500 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars/tests/it/lazy/explodes.rs
--rw-r--r--   0     1001      123     2279 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars/tests/it/lazy/expressions/apply.rs
--rw-r--r--   0     1001      123    10285 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars/tests/it/lazy/expressions/arity.rs
--rw-r--r--   0     1001      123     1065 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars/tests/it/lazy/expressions/expand.rs
--rw-r--r--   0     1001      123     1008 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars/tests/it/lazy/expressions/filter.rs
--rw-r--r--   0     1001      123      428 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars/tests/it/lazy/expressions/is_in.rs
--rw-r--r--   0     1001      123      121 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars/tests/it/lazy/expressions/mod.rs
--rw-r--r--   0     1001      123      659 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars/tests/it/lazy/expressions/slice.rs
--rw-r--r--   0     1001      123    10657 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars/tests/it/lazy/expressions/window.rs
--rw-r--r--   0     1001      123      579 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars/tests/it/lazy/folds.rs
--rw-r--r--   0     1001      123      557 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars/tests/it/lazy/functions.rs
--rw-r--r--   0     1001      123     4482 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars/tests/it/lazy/groupby.rs
--rw-r--r--   0     1001      123     1635 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars/tests/it/lazy/groupby_dynamic.rs
--rw-r--r--   0     1001      123      691 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars/tests/it/lazy/mod.rs
--rw-r--r--   0     1001      123     5614 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars/tests/it/lazy/predicate_queries.rs
--rw-r--r--   0     1001      123     4483 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars/tests/it/lazy/projection_queries.rs
--rw-r--r--   0     1001      123     6584 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars/tests/it/lazy/queries.rs
--rw-r--r--   0     1001      123      141 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars/tests/it/main.rs
--rw-r--r--   0     1001      123    12591 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars/tests/it/schema.rs
--rw-r--r--   0        0        0     2037 1970-01-01 00:00:00.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-time/Cargo.toml
--rw-r--r--   0     1001      123     1055 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-time/LICENSE
--rw-r--r--   0     1001      123      143 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-time/README.md
--rw-r--r--   0     1001      123     3565 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-time/src/chunkedarray/date.rs
--rw-r--r--   0     1001      123     6465 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-time/src/chunkedarray/datetime.rs
--rw-r--r--   0     1001      123     3305 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-time/src/chunkedarray/duration.rs
--rw-r--r--   0     1001      123     5607 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-time/src/chunkedarray/kernels.rs
--rw-r--r--   0     1001      123     1062 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-time/src/chunkedarray/mod.rs
--rw-r--r--   0     1001      123     7302 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-time/src/chunkedarray/rolling_window/floats.rs
--rw-r--r--   0     1001      123     2582 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-time/src/chunkedarray/rolling_window/ints.rs
--rw-r--r--   0     1001      123    11101 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-time/src/chunkedarray/rolling_window/mod.rs
--rw-r--r--   0     1001      123      428 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-time/src/chunkedarray/rolling_window/rolling_kernels/mod.rs
--rw-r--r--   0     1001      123     6408 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-time/src/chunkedarray/rolling_window/rolling_kernels/no_nulls.rs
--rw-r--r--   0     1001      123     2372 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-time/src/chunkedarray/time.rs
--rw-r--r--   0     1001      123    18180 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-time/src/chunkedarray/utf8/infer.rs
--rw-r--r--   0     1001      123    18997 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-time/src/chunkedarray/utf8/mod.rs
--rw-r--r--   0     1001      123     3975 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-time/src/chunkedarray/utf8/patterns.rs
--rw-r--r--   0     1001      123    10548 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-time/src/chunkedarray/utf8/strptime.rs
--rw-r--r--   0     1001      123     3442 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-time/src/date_range.rs
--rw-r--r--   0     1001      123    34469 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-time/src/groupby/dynamic.rs
--rw-r--r--   0     1001      123       88 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-time/src/groupby/mod.rs
--rw-r--r--   0     1001      123      621 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-time/src/lib.rs
--rw-r--r--   0     1001      123     2976 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-time/src/month_end.rs
--rw-r--r--   0     1001      123     3365 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-time/src/month_start.rs
--rw-r--r--   0     1001      123      274 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-time/src/prelude.rs
--rw-r--r--   0     1001      123     1381 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-time/src/round.rs
--rw-r--r--   0     1001      123     3992 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-time/src/series/_trait.rs
--rw-r--r--   0     1001      123      136 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-time/src/series/implementations/boolean.rs
--rw-r--r--   0     1001      123      140 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-time/src/series/implementations/categoricals.rs
--rw-r--r--   0     1001      123      133 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-time/src/series/implementations/date.rs
--rw-r--r--   0     1001      123      137 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-time/src/series/implementations/datetime.rs
--rw-r--r--   0     1001      123      137 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-time/src/series/implementations/duration.rs
--rw-r--r--   0     1001      123     1863 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-time/src/series/implementations/floats.rs
--rw-r--r--   0     1001      123     1792 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-time/src/series/implementations/integers.rs
--rw-r--r--   0     1001      123      133 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-time/src/series/implementations/list.rs
--rw-r--r--   0     1001      123      486 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-time/src/series/implementations/mod.rs
--rw-r--r--   0     1001      123      155 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-time/src/series/implementations/object.rs
--rw-r--r--   0     1001      123      135 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-time/src/series/implementations/struct_.rs
--rw-r--r--   0     1001      123      133 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-time/src/series/implementations/time.rs
--rw-r--r--   0     1001      123      133 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-time/src/series/implementations/utf8.rs
--rw-r--r--   0     1001      123    12787 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-time/src/series/mod.rs
--rw-r--r--   0     1001      123     1443 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-time/src/truncate.rs
--rw-r--r--   0     1001      123     6845 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-time/src/upsample.rs
--rw-r--r--   0     1001      123     2511 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-time/src/utils.rs
--rw-r--r--   0     1001      123     1524 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-time/src/windows/bounds.rs
--rw-r--r--   0     1001      123     2672 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-time/src/windows/calendar.rs
--rw-r--r--   0     1001      123    25015 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-time/src/windows/duration.rs
--rw-r--r--   0     1001      123    21244 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-time/src/windows/groupby.rs
--rw-r--r--   0     1001      123      503 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-time/src/windows/mod.rs
--rw-r--r--   0     1001      123    23652 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-time/src/windows/test.rs
--rw-r--r--   0     1001      123    11666 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-time/src/windows/window.rs
--rw-r--r--   0        0        0     3439 1970-01-01 00:00:00.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-ops/Cargo.toml
--rw-r--r--   0     1001      123     1055 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-ops/LICENSE
--rw-r--r--   0     1001      123      132 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-ops/README.md
--rw-r--r--   0     1001      123     2382 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-ops/src/chunked_array/array/min_max.rs
--rw-r--r--   0     1001      123      267 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-ops/src/chunked_array/array/mod.rs
--rw-r--r--   0     1001      123     1512 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-ops/src/chunked_array/array/namespace.rs
--rw-r--r--   0     1001      123     4108 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-ops/src/chunked_array/array/sum_mean.rs
--rw-r--r--   0     1001      123      234 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-ops/src/chunked_array/binary/mod.rs
--rw-r--r--   0     1001      123     3549 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-ops/src/chunked_array/binary/namespace.rs
--rw-r--r--   0     1001      123    11023 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-ops/src/chunked_array/interpolate.rs
--rw-r--r--   0     1001      123     1687 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-ops/src/chunked_array/list/count.rs
--rw-r--r--   0     1001      123     2419 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-ops/src/chunked_array/list/hash.rs
--rw-r--r--   0     1001      123     7861 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-ops/src/chunked_array/list/min_max.rs
--rw-r--r--   0     1001      123      511 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-ops/src/chunked_array/list/mod.rs
--rw-r--r--   0     1001      123    19010 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-ops/src/chunked_array/list/namespace.rs
--rw-r--r--   0     1001      123     7633 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-ops/src/chunked_array/list/sum_mean.rs
--rw-r--r--   0     1001      123     2435 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-ops/src/chunked_array/list/to_struct.rs
--rw-r--r--   0     1001      123      545 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-ops/src/chunked_array/mod.rs
--rw-r--r--   0     1001      123     9452 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-ops/src/chunked_array/nan_propagating_aggregate.rs
--rw-r--r--   0     1001      123     6795 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-ops/src/chunked_array/set.rs
--rw-r--r--   0     1001      123     7490 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-ops/src/chunked_array/strings/case.rs
--rw-r--r--   0     1001      123     8409 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-ops/src/chunked_array/strings/json_path.rs
--rw-r--r--   0     1001      123     2345 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-ops/src/chunked_array/strings/justify.rs
--rw-r--r--   0     1001      123      514 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-ops/src/chunked_array/strings/mod.rs
--rw-r--r--   0     1001      123    14731 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-ops/src/chunked_array/strings/namespace.rs
--rw-r--r--   0     1001      123     4053 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-ops/src/chunked_array/strings/replace.rs
--rw-r--r--   0     1001      123      439 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-ops/src/chunked_array/sum.rs
--rw-r--r--   0     1001      123     2486 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-ops/src/chunked_array/top_k.rs
--rw-r--r--   0     1001      123     7727 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-ops/src/frame/join/merge_sorted.rs
--rw-r--r--   0     1001      123    18232 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-ops/src/frame/join/mod.rs
--rw-r--r--   0     1001      123     4174 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-ops/src/frame/mod.rs
--rw-r--r--   0     1001      123    10257 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-ops/src/frame/pivot/mod.rs
--rw-r--r--   0     1001      123    13486 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-ops/src/frame/pivot/positioning.rs
--rw-r--r--   0     1001      123      237 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-ops/src/lib.rs
--rw-r--r--   0     1001      123      290 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-ops/src/prelude.rs
--rw-r--r--   0     1001      123       25 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-ops/src/series/mod.rs
--rw-r--r--   0     1001      123     9623 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-ops/src/series/ops/approx_algo/hyperloglogplus.rs
--rw-r--r--   0     1001      123      118 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-ops/src/series/ops/approx_algo/mod.rs
--rw-r--r--   0     1001      123     2016 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-ops/src/series/ops/approx_unique.rs
--rw-r--r--   0     1001      123    11866 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-ops/src/series/ops/arg_min_max.rs
--rw-r--r--   0     1001      123     3688 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-ops/src/series/ops/floor_divide.rs
--rw-r--r--   0     1001      123     5245 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-ops/src/series/ops/fused.rs
--rw-r--r--   0     1001      123     3423 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-ops/src/series/ops/is_first.rs
--rw-r--r--   0     1001      123     2975 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-ops/src/series/ops/is_unique.rs
--rw-r--r--   0     1001      123     3626 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-ops/src/series/ops/log.rs
--rw-r--r--   0     1001      123     1187 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-ops/src/series/ops/mod.rs
--rw-r--r--   0     1001      123     1769 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-ops/src/series/ops/rolling.rs
--rw-r--r--   0     1001      123     7642 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-ops/src/series/ops/search_sorted.rs
--rw-r--r--   0     1001      123     2500 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-ops/src/series/ops/to_dummies.rs
--rw-r--r--   0     1001      123     2067 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-ops/src/series/ops/various.rs
--rw-r--r--   0        0        0     4397 1970-01-01 00:00:00.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-io/Cargo.toml
--rw-r--r--   0     1001      123     1055 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-io/LICENSE
--rw-r--r--   0     1001      123      138 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-io/README.md
--rw-r--r--   0     1001      123     2383 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-io/src/avro/mod.rs
--rw-r--r--   0     1001      123     3608 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-io/src/avro/read.rs
--rw-r--r--   0     1001      123     2622 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-io/src/avro/write.rs
--rw-r--r--   0     1001      123     4505 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-io/src/cloud/adaptors.rs
--rw-r--r--   0     1001      123     9506 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-io/src/cloud/glob.rs
--rw-r--r--   0     1001      123     3089 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-io/src/cloud/mod.rs
--rw-r--r--   0     1001      123    28133 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-io/src/csv/buffer.rs
--rw-r--r--   0     1001      123     1815 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-io/src/csv/mod.rs
--rw-r--r--   0     1001      123    19446 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-io/src/csv/parser.rs
--rw-r--r--   0     1001      123    22226 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-io/src/csv/read.rs
--rw-r--r--   0     1001      123    10846 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-io/src/csv/read_impl/batched_mmap.rs
--rw-r--r--   0     1001      123    13938 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-io/src/csv/read_impl/batched_read.rs
--rw-r--r--   0     1001      123    30724 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-io/src/csv/read_impl/mod.rs
--rw-r--r--   0     1001      123    11466 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-io/src/csv/splitfields.rs
--rw-r--r--   0     1001      123    24531 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-io/src/csv/utils.rs
--rw-r--r--   0     1001      123     2796 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-io/src/csv/write.rs
--rw-r--r--   0     1001      123    14759 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-io/src/csv/write_impl.rs
--rw-r--r--   0     1001      123      184 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-io/src/export.rs
--rw-r--r--   0     1001      123     7586 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-io/src/ipc/ipc_file.rs
--rw-r--r--   0     1001      123     9227 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-io/src/ipc/ipc_stream.rs
--rw-r--r--   0     1001      123     3253 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-io/src/ipc/mmap.rs
--rw-r--r--   0     1001      123      401 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-io/src/ipc/mod.rs
--rw-r--r--   0     1001      123     8287 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-io/src/ipc/write.rs
--rw-r--r--   0     1001      123     1471 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-io/src/ipc/write_async.rs
--rw-r--r--   0     1001      123    11044 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-io/src/json/mod.rs
--rw-r--r--   0     1001      123     4771 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-io/src/lib.rs
--rw-r--r--   0     1001      123     1969 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-io/src/mmap.rs
--rw-r--r--   0     1001      123     7155 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-io/src/ndjson/buffer.rs
--rw-r--r--   0     1001      123    11979 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-io/src/ndjson/core.rs
--rw-r--r--   0     1001      123       37 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-io/src/ndjson/mod.rs
--rw-r--r--   0     1001      123      273 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-io/src/options.rs
--rw-r--r--   0     1001      123     7360 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-io/src/parquet/async_impl.rs
--rw-r--r--   0     1001      123     3093 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-io/src/parquet/mmap.rs
--rw-r--r--   0     1001      123     3132 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-io/src/parquet/mod.rs
--rw-r--r--   0     1001      123     4784 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-io/src/parquet/predicates.rs
--rw-r--r--   0     1001      123     9623 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-io/src/parquet/read.rs
--rw-r--r--   0     1001      123    16886 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-io/src/parquet/read_impl.rs
--rw-r--r--   0     1001      123    10052 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-io/src/parquet/write.rs
--rw-r--r--   0     1001      123     5334 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-io/src/partition.rs
--rw-r--r--   0     1001      123     1455 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-io/src/predicates.rs
--rw-r--r--   0     1001      123      621 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-io/src/prelude.rs
--rw-r--r--   0     1001      123      417 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-io/src/tests.rs
--rw-r--r--   0     1001      123     4374 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-io/src/utils.rs
--rw-r--r--   0        0        0      569 1970-01-01 00:00:00.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-utils/Cargo.toml
--rw-r--r--   0     1001      123     1055 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-utils/LICENSE
--rw-r--r--   0     1001      123      141 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-utils/README.md
--rw-r--r--   0     1001      123      151 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-utils/src/aliases.rs
--rw-r--r--   0     1001      123     2862 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-utils/src/arena.rs
--rw-r--r--   0     1001      123     1373 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-utils/src/atomic.rs
--rw-r--r--   0     1001      123     2659 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-utils/src/cell.rs
--rw-r--r--   0     1001      123     1015 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-utils/src/contention_pool.rs
--rw-r--r--   0     1001      123      509 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-utils/src/error.rs
--rw-r--r--   0     1001      123      271 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-utils/src/fmt.rs
--rw-r--r--   0     1001      123      763 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-utils/src/functions.rs
--rw-r--r--   0     1001      123     2709 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-utils/src/iter/enumerate_idx.rs
--rw-r--r--   0     1001      123       61 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-utils/src/iter/mod.rs
--rw-r--r--   0     1001      123      490 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-utils/src/lib.rs
--rw-r--r--   0     1001      123      573 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-utils/src/macros.rs
--rw-r--r--   0     1001      123      282 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-utils/src/mem.rs
--rw-r--r--   0     1001      123     2336 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-utils/src/slice.rs
--rw-r--r--   0     1001      123     2467 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-utils/src/sort.rs
--rw-r--r--   0     1001      123     1115 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-utils/src/sync.rs
--rw-r--r--   0     1001      123      504 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-utils/src/sys.rs
--rw-r--r--   0     1001      123      697 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-utils/src/unwrap.rs
--rw-r--r--   0     1001      123      616 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-utils/src/wasm.rs
--rw-r--r--   0        0        0     1106 1970-01-01 00:00:00.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-sql/Cargo.toml
--rw-r--r--   0     1001      123     1055 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-sql/LICENSE
--rw-r--r--   0     1001      123      466 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-sql/README.md
--rw-r--r--   0     1001      123    22794 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-sql/src/context.rs
--rw-r--r--   0     1001      123    20710 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-sql/src/functions.rs
--rw-r--r--   0     1001      123     2098 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-sql/src/keywords.rs
--rw-r--r--   0     1001      123      239 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-sql/src/lib.rs
--rw-r--r--   0     1001      123    19192 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-sql/src/sql_expr.rs
--rw-r--r--   0     1001      123     4572 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-sql/src/table_functions.rs
--rw-r--r--   0     1001      123     1682 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-sql/tests/functions_cumulative.rs
--rw-r--r--   0     1001      123     3063 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-sql/tests/functions_io.rs
--rw-r--r--   0     1001      123     1539 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-sql/tests/functions_math.rs
--rw-r--r--   0     1001      123      860 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-sql/tests/functions_meta.rs
--rw-r--r--   0     1001      123     2982 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-sql/tests/functions_string.rs
--rw-r--r--   0     1001      123     1056 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-sql/tests/iss_7436.rs
--rw-r--r--   0     1001      123      888 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-sql/tests/iss_7437.rs
--rw-r--r--   0     1001      123      652 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-sql/tests/iss_7440.rs
--rw-r--r--   0     1001      123      700 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-sql/tests/iss_8395.rs
--rw-r--r--   0     1001      123     1062 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-sql/tests/iss_8419.rs
--rw-r--r--   0     1001      123      982 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-sql/tests/ops_distinct_on.rs
--rw-r--r--   0     1001      123    15418 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-sql/tests/simple_exprs.rs
--rw-r--r--   0     1001      123     2985 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-sql/tests/statements.rs
--rw-r--r--   0        0        0      954 1970-01-01 00:00:00.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-row/Cargo.toml
--rw-r--r--   0     1001      123     1055 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-row/LICENSE
--rw-r--r--   0     1001      123      137 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-row/README.md
--rw-r--r--   0     1001      123     8985 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-row/src/encode.rs
--rw-r--r--   0     1001      123     4591 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-row/src/encodings/fixed.rs
--rw-r--r--   0     1001      123       47 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-row/src/encodings/mod.rs
--rw-r--r--   0     1001      123     4508 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-row/src/encodings/variable.rs
--rw-r--r--   0     1001      123    13676 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-row/src/lib.rs
--rw-r--r--   0     1001      123     2079 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-row/src/row.rs
--rw-r--r--   0     1001      123      682 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-row/src/utils.rs
--rw-r--r--   0        0        0     1353 1970-01-01 00:00:00.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-json/Cargo.toml
--rw-r--r--   0     1001      123     1055 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-json/LICENSE
--rw-r--r--   0     1001      123    16770 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-json/src/json/deserialize.rs
--rw-r--r--   0     1001      123     6564 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-json/src/json/infer_schema.rs
--rw-r--r--   0     1001      123      189 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-json/src/json/mod.rs
--rw-r--r--   0     1001      123       30 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-json/src/lib.rs
--rw-r--r--   0     1001      123     1198 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-json/src/ndjson/deserialize.rs
--rw-r--r--   0     1001      123     4808 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-json/src/ndjson/file.rs
--rw-r--r--   0     1001      123      143 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-json/src/ndjson/mod.rs
--rw-r--r--   0        0        0     1592 1970-01-01 00:00:00.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/Cargo.toml
--rw-r--r--   0     1001      123     1055 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/LICENSE
--rw-r--r--   0     1001      123      144 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/README.md
--rw-r--r--   0     1001      123     1975 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/array/default_arrays.rs
--rw-r--r--   0     1001      123     1791 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/array/fixed_size_list.rs
--rw-r--r--   0     1001      123     3773 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/array/get.rs
--rw-r--r--   0     1001      123     6664 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/array/list.rs
--rw-r--r--   0     1001      123     8165 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/array/mod.rs
--rw-r--r--   0     1001      123      878 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/array/null.rs
--rw-r--r--   0     1001      123     1125 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/array/slice.rs
--rw-r--r--   0     1001      123     2252 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/array/utf8.rs
--rw-r--r--   0     1001      123     2294 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/bit_util.rs
--rw-r--r--   0     1001      123       17 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/bitmap/mod.rs
--rw-r--r--   0     1001      123      819 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/bitmap/mutable.rs
--rw-r--r--   0     1001      123      370 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/compute/arithmetics/decimal/add.rs
--rw-r--r--   0     1001      123     2181 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/compute/arithmetics/decimal/commutative.rs
--rw-r--r--   0     1001      123     1482 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/compute/arithmetics/decimal/div.rs
--rw-r--r--   0     1001      123     1028 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/compute/arithmetics/decimal/mod.rs
--rw-r--r--   0     1001      123     1177 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/compute/arithmetics/decimal/mul.rs
--rw-r--r--   0     1001      123      508 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/compute/arithmetics/decimal/sub.rs
--rw-r--r--   0     1001      123       51 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/compute/arithmetics/mod.rs
--rw-r--r--   0     1001      123        1 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/compute/arity.rs
--rw-r--r--   0     1001      123      727 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/compute/bitwise.rs
--rw-r--r--   0     1001      123     1206 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/compute/cast.rs
--rw-r--r--   0     1001      123     3964 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/compute/decimal.rs
--rw-r--r--   0     1001      123     1250 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/compute/mod.rs
--rw-r--r--   0     1001      123      391 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/compute/take/bitmap.rs
--rw-r--r--   0     1001      123     2767 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/compute/take/boolean.rs
--rw-r--r--   0     1001      123     3487 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/compute/take/fixed_size_list.rs
--rw-r--r--   0     1001      123    25289 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/compute/take/mod.rs
--rw-r--r--   0     1001      123      797 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/compute/tile.rs
--rw-r--r--   0     1001      123     1102 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/conversion.rs
--rw-r--r--   0     1001      123     1609 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/data_types.rs
--rw-r--r--   0     1001      123       25 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/error.rs
--rw-r--r--   0     1001      123       28 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/export.rs
--rw-r--r--   0     1001      123       26 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/floats/mod.rs
--rw-r--r--   0     1001      123     2066 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/floats/ord.rs
--rw-r--r--   0     1001      123     1273 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/index.rs
--rw-r--r--   0     1001      123      984 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/is_valid.rs
--rw-r--r--   0     1001      123     4783 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/kernels/agg_mean.rs
--rw-r--r--   0     1001      123     1074 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/kernels/comparison.rs
--rw-r--r--   0     1001      123     1068 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/kernels/concatenate.rs
--rw-r--r--   0     1001      123     5161 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/kernels/ewm/average.rs
--rw-r--r--   0     1001      123     1808 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/kernels/ewm/mod.rs
--rw-r--r--   0     1001      123    25065 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/kernels/ewm/variance.rs
--rw-r--r--   0     1001      123     1406 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/kernels/float.rs
--rw-r--r--   0     1001      123     4907 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/kernels/list.rs
--rw-r--r--   0     1001      123     1885 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/kernels/list_bytes_iter.rs
--rw-r--r--   0     1001      123     9783 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/kernels/mod.rs
--rw-r--r--   0     1001      123     3923 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/kernels/rolling/mod.rs
--rw-r--r--   0     1001      123     2019 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/mean.rs
--rw-r--r--   0     1001      123    16191 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/min_max.rs
--rw-r--r--   0     1001      123     3839 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/mod.rs
--rw-r--r--   0     1001      123    11729 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/quantile.rs
--rw-r--r--   0     1001      123     5684 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/sum.rs
--rw-r--r--   0     1001      123     9609 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/variance.rs
--rw-r--r--   0     1001      123     1879 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/kernels/rolling/nulls/mean.rs
--rw-r--r--   0     1001      123    14722 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/kernels/rolling/nulls/min_max.rs
--rw-r--r--   0     1001      123    10055 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/kernels/rolling/nulls/mod.rs
--rw-r--r--   0     1001      123    11643 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/kernels/rolling/nulls/quantile.rs
--rw-r--r--   0     1001      123     4821 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/kernels/rolling/nulls/sum.rs
--rw-r--r--   0     1001      123     8687 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/kernels/rolling/nulls/variance.rs
--rw-r--r--   0     1001      123     8109 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/kernels/rolling/window.rs
--rw-r--r--   0     1001      123     4752 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/kernels/set.rs
--rw-r--r--   0     1001      123     4529 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/kernels/sort_partition.rs
--rw-r--r--   0     1001      123     2948 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/kernels/sorted_join/inner.rs
--rw-r--r--   0     1001      123     5974 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/kernels/sorted_join/left.rs
--rw-r--r--   0     1001      123      231 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/kernels/sorted_join/mod.rs
--rw-r--r--   0     1001      123      841 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/kernels/string.rs
--rw-r--r--   0     1001      123     2310 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/kernels/take_agg/boolean.rs
--rw-r--r--   0     1001      123     4344 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/kernels/take_agg/mod.rs
--rw-r--r--   0     1001      123     2606 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/kernels/take_agg/var.rs
--rw-r--r--   0     1001      123     3672 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/kernels/time.rs
--rw-r--r--   0     1001      123      341 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/lib.rs
--rw-r--r--   0     1001      123      496 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/prelude.rs
--rw-r--r--   0     1001      123      534 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/slice.rs
--rw-r--r--   0     1001      123      183 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/time_zone.rs
--rw-r--r--   0     1001      123      998 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/trusted_len/boolean.rs
--rw-r--r--   0     1001      123     2821 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/trusted_len/mod.rs
--rw-r--r--   0     1001      123     2052 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/trusted_len/push_unchecked.rs
--rw-r--r--   0     1001      123      158 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/trusted_len/rev.rs
--rw-r--r--   0     1001      123     5232 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/utils.rs
--rw-r--r--   0        0        0      894 1970-01-01 00:00:00.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-error/Cargo.toml
--rw-r--r--   0     1001      123     1055 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-error/LICENSE
--rw-r--r--   0     1001      123      145 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-error/README.md
--rw-r--r--   0     1001      123     6584 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-error/src/lib.rs
--rw-r--r--   0        0        0      827 1970-01-01 00:00:00.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-algo/Cargo.toml
--rw-r--r--   0     1001      123     1055 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-algo/LICENSE
--rw-r--r--   0     1001      123      142 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-algo/README.md
--rw-r--r--   0     1001      123     7548 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-algo/src/algo.rs
--rw-r--r--   0     1001      123       88 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-algo/src/lib.rs
--rw-r--r--   0     1001      123       28 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-algo/src/prelude.rs
--rw-r--r--   0        0        0     5484 1970-01-01 00:00:00.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/Cargo.toml
--rw-r--r--   0     1001      123     1055 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/LICENSE
--rw-r--r--   0     1001      123      144 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/README.md
--rw-r--r--   0     1001      123     5125 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/arithmetic/decimal.rs
--rw-r--r--   0     1001      123     8275 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/arithmetic/mod.rs
--rw-r--r--   0     1001      123     9406 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/arithmetic/numeric.rs
--rw-r--r--   0     1001      123     3588 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/array/iterator.rs
--rw-r--r--   0     1001      123     2551 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/array/mod.rs
--rw-r--r--   0     1001      123     6448 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/bitwise.rs
--rw-r--r--   0     1001      123     2298 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/builder/binary.rs
--rw-r--r--   0     1001      123     1207 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/builder/boolean.rs
--rw-r--r--   0     1001      123     4311 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/builder/fixed_size_list.rs
--rw-r--r--   0     1001      123     1556 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/builder/from.rs
--rw-r--r--   0     1001      123    20366 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/builder/list.rs
--rw-r--r--   0     1001      123     8969 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/builder/mod.rs
--rw-r--r--   0     1001      123     1410 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/builder/primitive.rs
--rw-r--r--   0     1001      123     2291 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/builder/utf8.rs
--rw-r--r--   0     1001      123    16475 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/cast.rs
--rw-r--r--   0     1001      123    49461 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/comparison/mod.rs
--rw-r--r--   0     1001      123    10060 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/comparison/scalar.rs
--rw-r--r--   0     1001      123      551 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/drop.rs
--rw-r--r--   0     1001      123      963 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/float.rs
--rw-r--r--   0     1001      123     7175 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/from.rs
--rw-r--r--   0     1001      123    42339 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/iterator/mod.rs
--rw-r--r--   0     1001      123     1453 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/iterator/par/list.rs
--rw-r--r--   0     1001      123       28 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/iterator/par/mod.rs
--rw-r--r--   0     1001      123     1129 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/iterator/par/utf8.rs
--rw-r--r--   0     1001      123       21 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/kernels/mod.rs
--rw-r--r--   0     1001      123     2347 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/kernels/take.rs
--rw-r--r--   0     1001      123     7963 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/list/iterator.rs
--rw-r--r--   0     1001      123     3242 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/list/mod.rs
--rw-r--r--   0     1001      123    19830 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/logical/categorical/builder.rs
--rw-r--r--   0     1001      123     3688 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/logical/categorical/from.rs
--rw-r--r--   0     1001      123     4270 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/logical/categorical/merge.rs
--rw-r--r--   0     1001      123    10219 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/logical/categorical/mod.rs
--rw-r--r--   0     1001      123     1400 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/append.rs
--rw-r--r--   0     1001      123      358 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/full.rs
--rw-r--r--   0     1001      123      192 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/mod.rs
--rw-r--r--   0     1001      123     2731 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/take_random.rs
--rw-r--r--   0     1001      123     2172 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/unique.rs
--rw-r--r--   0     1001      123      925 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/zip.rs
--rw-r--r--   0     1001      123     6417 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/logical/categorical/stringcache.rs
--rw-r--r--   0     1001      123     1604 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/logical/date.rs
--rw-r--r--   0     1001      123     4105 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/logical/datetime.rs
--rw-r--r--   0     1001      123     4443 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/logical/decimal.rs
--rw-r--r--   0     1001      123     2434 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/logical/duration.rs
--rw-r--r--   0     1001      123     2556 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/logical/mod.rs
--rw-r--r--   0     1001      123      476 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/logical/struct_/from.rs
--rw-r--r--   0     1001      123    15982 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/logical/struct_/mod.rs
--rw-r--r--   0     1001      123     1182 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/logical/time.rs
--rw-r--r--   0     1001      123    23389 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/mod.rs
--rw-r--r--   0     1001      123     7200 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/ndarray.rs
--rw-r--r--   0     1001      123     4484 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/object/builder.rs
--rw-r--r--   0     1001      123     1547 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/object/extension/drop.rs
--rw-r--r--   0     1001      123     3124 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/object/extension/list.rs
--rw-r--r--   0     1001      123     7054 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/object/extension/mod.rs
--rw-r--r--   0     1001      123     3410 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/object/extension/polars_extension.rs
--rw-r--r--   0     1001      123      137 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/object/is_valid.rs
--rw-r--r--   0     1001      123     4419 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/object/iterator.rs
--rw-r--r--   0     1001      123     4806 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/object/mod.rs
--rw-r--r--   0     1001      123     2956 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/object/registry.rs
--rw-r--r--   0     1001      123      272 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/ops/abs.rs
--rw-r--r--   0     1001      123    32691 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/ops/aggregate/mod.rs
--rw-r--r--   0     1001      123    10025 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/ops/aggregate/quantile.rs
--rw-r--r--   0     1001      123     2880 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/ops/aggregate/var.rs
--rw-r--r--   0     1001      123    10551 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/ops/any_value.rs
--rw-r--r--   0     1001      123     2820 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/ops/append.rs
--rw-r--r--   0     1001      123    28256 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/ops/apply.rs
--rw-r--r--   0     1001      123    12799 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/ops/bit_repr.rs
--rw-r--r--   0     1001      123     6214 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/ops/chunkops.rs
--rw-r--r--   0     1001      123    11537 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/ops/compare_inner.rs
--rw-r--r--   0     1001      123     1737 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/ops/concat_str.rs
--rw-r--r--   0     1001      123     4801 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/ops/cum_agg.rs
--rw-r--r--   0     1001      123      908 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/ops/decimal.rs
--rw-r--r--   0     1001      123     7056 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/ops/downcast.rs
--rw-r--r--   0     1001      123    19463 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/ops/explode.rs
--rw-r--r--   0     1001      123     8691 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/ops/explode_and_offsets.rs
--rw-r--r--   0     1001      123     8866 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/ops/extend.rs
--rw-r--r--   0     1001      123    13777 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/ops/fill_null.rs
--rw-r--r--   0     1001      123     6323 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/ops/filter.rs
--rw-r--r--   0     1001      123     5876 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/ops/full.rs
--rw-r--r--   0     1001      123        1 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/ops/interpolate.rs
--rw-r--r--   0     1001      123    16797 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/ops/is_in.rs
--rw-r--r--   0     1001      123        1 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/ops/len.rs
--rw-r--r--   0     1001      123     2658 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/ops/min_max_binary.rs
--rw-r--r--   0     1001      123    23276 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/ops/mod.rs
--rw-r--r--   0     1001      123     2403 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/ops/nulls.rs
--rw-r--r--   0     1001      123      593 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/ops/peaks.rs
--rw-r--r--   0     1001      123     4375 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/ops/repeat_by.rs
--rw-r--r--   0     1001      123     2771 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/ops/reverse.rs
--rw-r--r--   0     1001      123    10266 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/ops/rolling_window.rs
--rw-r--r--   0     1001      123    12518 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/ops/set.rs
--rw-r--r--   0     1001      123     7391 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/ops/shift.rs
--rw-r--r--   0     1001      123     2299 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/ops/sort/arg_sort.rs
--rw-r--r--   0     1001      123     5528 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/ops/sort/arg_sort_multiple.rs
--rw-r--r--   0     1001      123     7543 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/ops/sort/categorical.rs
--rw-r--r--   0     1001      123    31164 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/ops/sort/mod.rs
--rw-r--r--   0     1001      123      380 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/ops/sort/slice.rs
--rw-r--r--   0     1001      123    22078 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/ops/take/mod.rs
--rw-r--r--   0     1001      123     7848 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/ops/take/take_chunked.rs
--rw-r--r--   0     1001      123      301 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/ops/take/take_every.rs
--rw-r--r--   0     1001      123    16256 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/ops/take/take_random.rs
--rw-r--r--   0     1001      123     5810 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/ops/take/take_single.rs
--rw-r--r--   0     1001      123     6072 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/ops/take/traits.rs
--rw-r--r--   0     1001      123      459 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/ops/tile.rs
--rw-r--r--   0     1001      123    11626 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/ops/unique/mod.rs
--rw-r--r--   0     1001      123    14620 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/ops/unique/rank.rs
--rw-r--r--   0     1001      123     8427 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/ops/zip.rs
--rw-r--r--   0     1001      123     9093 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/random.rs
--rw-r--r--   0     1001      123     1875 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/temporal/conversion.rs
--rw-r--r--   0     1001      123     2826 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/temporal/date.rs
--rw-r--r--   0     1001      123    10497 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/temporal/datetime.rs
--rw-r--r--   0     1001      123     3201 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/temporal/duration.rs
--rw-r--r--   0     1001      123      595 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/temporal/mod.rs
--rw-r--r--   0     1001      123     3042 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/temporal/time.rs
--rw-r--r--   0     1001      123      872 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/to_vec.rs
--rw-r--r--   0     1001      123     8113 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/trusted_len.rs
--rw-r--r--   0     1001      123    25939 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/upstream_traits.rs
--rw-r--r--   0     1001      123     7944 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/cloud.rs
--rw-r--r--   0     1001      123     1549 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/config.rs
--rw-r--r--   0     1001      123     3946 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/datatypes/_serde.rs
--rw-r--r--   0     1001      123     2509 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/datatypes/aliases.rs
--rw-r--r--   0     1001      123    42658 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/datatypes/any_value.rs
--rw-r--r--   0     1001      123    13349 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/datatypes/dtype.rs
--rw-r--r--   0     1001      123     5609 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/datatypes/field.rs
--rw-r--r--   0     1001      123     8059 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/datatypes/mod.rs
--rw-r--r--   0     1001      123     2016 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/datatypes/time_unit.rs
--rw-r--r--   0     1001      123      118 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/doc/changelog/mod.rs
--rw-r--r--   0     1001      123      898 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/doc/changelog/v0_10_0_11.rs
--rw-r--r--   0     1001      123      481 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/doc/changelog/v0_3.rs
--rw-r--r--   0     1001      123      293 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/doc/changelog/v0_4.rs
--rw-r--r--   0     1001      123      499 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/doc/changelog/v0_5.rs
--rw-r--r--   0     1001      123      288 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/doc/changelog/v0_6.rs
--rw-r--r--   0     1001      123     1071 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/doc/changelog/v0_7.rs
--rw-r--r--   0     1001      123      819 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/doc/changelog/v0_8.rs
--rw-r--r--   0     1001      123      596 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/doc/changelog/v0_9.rs
--rw-r--r--   0     1001      123       43 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/doc/mod.rs
--rw-r--r--   0     1001      123       25 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/error.rs
--rw-r--r--   0     1001      123      263 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/export.rs
--rw-r--r--   0     1001      123    36432 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/fmt.rs
--rw-r--r--   0     1001      123     5177 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/frame/arithmetic.rs
--rw-r--r--   0     1001      123     9916 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/frame/asof_join/asof.rs
--rw-r--r--   0     1001      123    35761 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/frame/asof_join/groups.rs
--rw-r--r--   0     1001      123     6973 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/frame/asof_join/mod.rs
--rw-r--r--   0     1001      123      559 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/frame/chunks.rs
--rw-r--r--   0     1001      123     5181 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/frame/cross_join.rs
--rw-r--r--   0     1001      123    16760 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/frame/explode.rs
--rw-r--r--   0     1001      123     1019 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/frame/from.rs
--rw-r--r--   0     1001      123    19219 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/frame/groupby/aggregations/agg_list.rs
--rw-r--r--   0     1001      123     4113 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/frame/groupby/aggregations/boolean.rs
--rw-r--r--   0     1001      123     7749 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/frame/groupby/aggregations/dispatch.rs
--rw-r--r--   0     1001      123    40369 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/frame/groupby/aggregations/mod.rs
--rw-r--r--   0     1001      123     5634 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/frame/groupby/aggregations/utf8.rs
--rw-r--r--   0     1001      123      218 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/frame/groupby/expr.rs
--rw-r--r--   0     1001      123    22901 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/frame/groupby/hashing.rs
--rw-r--r--   0     1001      123    14380 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/frame/groupby/into_groups.rs
--rw-r--r--   0     1001      123    39516 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/frame/groupby/mod.rs
--rw-r--r--   0     1001      123    10637 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/frame/groupby/perfect.rs
--rw-r--r--   0     1001      123    19780 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/frame/groupby/proxy.rs
--rw-r--r--   0     1001      123     5406 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/frame/hash_join/args.rs
--rw-r--r--   0     1001      123    13329 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/frame/hash_join/mod.rs
--rw-r--r--   0     1001      123    22364 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/frame/hash_join/multiple_keys.rs
--rw-r--r--   0     1001      123     2413 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/frame/hash_join/single_keys.rs
--rw-r--r--   0     1001      123    17372 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/frame/hash_join/single_keys_dispatch.rs
--rw-r--r--   0     1001      123     4608 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/frame/hash_join/single_keys_inner.rs
--rw-r--r--   0     1001      123     6434 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/frame/hash_join/single_keys_left.rs
--rw-r--r--   0     1001      123     4564 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/frame/hash_join/single_keys_outer.rs
--rw-r--r--   0     1001      123     3913 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/frame/hash_join/single_keys_semi_anti.rs
--rw-r--r--   0     1001      123    12313 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/frame/hash_join/sort_merge.rs
--rw-r--r--   0     1001      123     3865 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/frame/hash_join/zip_outer.rs
--rw-r--r--   0     1001      123   126128 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/frame/mod.rs
--rw-r--r--   0     1001      123    27652 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/frame/row/av_buffer.rs
--rw-r--r--   0     1001      123     5183 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/frame/row/dataframe.rs
--rw-r--r--   0     1001      123     5976 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/frame/row/mod.rs
--rw-r--r--   0     1001      123     9875 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/frame/row/transpose.rs
--rw-r--r--   0     1001      123     2811 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/frame/top_k.rs
--rw-r--r--   0     1001      123     1388 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/frame/upstream_traits.rs
--rw-r--r--   0     1001      123    10198 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/functions.rs
--rw-r--r--   0     1001      123     2149 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/hashing/fx.rs
--rw-r--r--   0     1001      123     1503 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/hashing/identity.rs
--rw-r--r--   0     1001      123      457 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/hashing/mod.rs
--rw-r--r--   0     1001      123     2684 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/hashing/partition.rs
--rw-r--r--   0     1001      123    17611 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/hashing/vector_hasher.rs
--rw-r--r--   0     1001      123     1896 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/lib.rs
--rw-r--r--   0     1001      123    15733 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/named_from.rs
--rw-r--r--   0     1001      123     2423 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/prelude.rs
--rw-r--r--   0     1001      123    17006 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/schema.rs
--rw-r--r--   0     1001      123     4218 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/serde/chunked_array.rs
--rw-r--r--   0     1001      123     1094 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/serde/df.rs
--rw-r--r--   0     1001      123     6559 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/serde/mod.rs
--rw-r--r--   0     1001      123     9929 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/serde/series.rs
--rw-r--r--   0     1001      123    18543 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/series/any_value.rs
--rw-r--r--   0     1001      123    28755 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/series/arithmetic/borrowed.rs
--rw-r--r--   0     1001      123      222 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/series/arithmetic/mod.rs
--rw-r--r--   0     1001      123     3546 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/series/arithmetic/owned.rs
--rw-r--r--   0     1001      123    19293 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/series/comparison.rs
--rw-r--r--   0     1001      123    29575 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/series/from.rs
--rw-r--r--   0     1001      123     6080 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/series/implementations/array.rs
--rw-r--r--   0     1001      123     9089 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/series/implementations/binary.rs
--rw-r--r--   0     1001      123    10835 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/series/implementations/boolean.rs
--rw-r--r--   0     1001      123    12800 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/series/implementations/categorical.rs
--rw-r--r--   0     1001      123    18214 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/series/implementations/dates_time.rs
--rw-r--r--   0     1001      123    15034 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/series/implementations/datetime.rs
--rw-r--r--   0     1001      123     7981 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/series/implementations/decimal.rs
--rw-r--r--   0     1001      123    14734 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/series/implementations/duration.rs
--rw-r--r--   0     1001      123    14063 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/series/implementations/floats.rs
--rw-r--r--   0     1001      123     6078 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/series/implementations/list.rs
--rw-r--r--   0     1001      123    18396 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/series/implementations/mod.rs
--rw-r--r--   0     1001      123     5522 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/series/implementations/null.rs
--rw-r--r--   0     1001      123     7939 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/series/implementations/object.rs
--rw-r--r--   0     1001      123    11788 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/series/implementations/struct_.rs
--rw-r--r--   0     1001      123     9607 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/series/implementations/utf8.rs
--rw-r--r--   0     1001      123     4471 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/series/into.rs
--rw-r--r--   0     1001      123     6241 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/series/iterator.rs
--rw-r--r--   0     1001      123    38559 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/series/mod.rs
--rw-r--r--   0     1001      123      853 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/series/ops/diff.rs
--rw-r--r--   0     1001      123     5814 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/series/ops/downcast.rs
--rw-r--r--   0     1001      123     3601 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/series/ops/ewm.rs
--rw-r--r--   0     1001      123      413 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/series/ops/extend.rs
--rw-r--r--   0     1001      123      562 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/series/ops/mod.rs
--rw-r--r--   0     1001      123     5974 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/series/ops/moment.rs
--rw-r--r--   0     1001      123     2908 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/series/ops/null.rs
--rw-r--r--   0     1001      123     1347 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/series/ops/pct_change.rs
--rw-r--r--   0     1001      123     4620 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/series/ops/round.rs
--rw-r--r--   0     1001      123     5073 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/series/ops/to_list.rs
--rw-r--r--   0     1001      123     1476 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/series/ops/unique.rs
--rw-r--r--   0     1001      123    18408 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/series/series_trait.rs
--rw-r--r--   0     1001      123     2912 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/series/unstable.rs
--rw-r--r--   0     1001      123     7077 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/testing.rs
--rw-r--r--   0     1001      123      508 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/tests.rs
--rw-r--r--   0     1001      123     2492 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/utils/flatten.rs
--rw-r--r--   0     1001      123    30596 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/utils/mod.rs
--rw-r--r--   0     1001      123     1600 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/utils/series.rs
--rw-r--r--   0     1001      123    13201 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/utils/supertype.rs
--rw-r--r--   0        0        0     5152 1970-01-01 00:00:00.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/Cargo.toml
--rw-r--r--   0     1001      123     1055 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/LICENSE
--rw-r--r--   0     1001      123       45 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/constants.rs
--rw-r--r--   0     1001      123    17253 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dot.rs
--rw-r--r--   0     1001      123     4171 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/arithmetic.rs
--rw-r--r--   0     1001      123     3992 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/arity.rs
--rw-r--r--   0     1001      123     1278 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/array.rs
--rw-r--r--   0     1001      123      935 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/binary.rs
--rw-r--r--   0     1001      123      650 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/cat.rs
--rw-r--r--   0     1001      123    10228 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/dt.rs
--rw-r--r--   0     1001      123     9538 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/expr.rs
--rw-r--r--   0     1001      123     6441 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/expr_dyn_fn.rs
--rw-r--r--   0     1001      123      753 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/from.rs
--rw-r--r--   0     1001      123       85 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/function_expr/abs.rs
--rw-r--r--   0     1001      123     1431 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/function_expr/arg_where.rs
--rw-r--r--   0     1001      123     1074 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/function_expr/array.rs
--rw-r--r--   0     1001      123     1327 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/function_expr/binary.rs
--rw-r--r--   0     1001      123     4221 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/function_expr/boolean.rs
--rw-r--r--   0     1001      123     1910 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/function_expr/bounds.rs
--rw-r--r--   0     1001      123     1216 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/function_expr/cat.rs
--rw-r--r--   0     1001      123      344 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/function_expr/clip.rs
--rw-r--r--   0     1001      123      257 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/function_expr/concat.rs
--rw-r--r--   0     1001      123     6261 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/function_expr/correlation.rs
--rw-r--r--   0     1001      123     1593 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/function_expr/cum.rs
--rw-r--r--   0     1001      123     9597 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/function_expr/datetime.rs
--rw-r--r--   0     1001      123      782 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/function_expr/dispatch.rs
--rw-r--r--   0     1001      123     2567 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/function_expr/fill_null.rs
--rw-r--r--   0     1001      123      992 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/function_expr/fused.rs
--rw-r--r--   0     1001      123     8119 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/function_expr/list.rs
--rw-r--r--   0     1001      123      581 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/function_expr/log.rs
--rw-r--r--   0     1001      123    21146 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/function_expr/mod.rs
--rw-r--r--   0     1001      123      462 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/function_expr/nan.rs
--rw-r--r--   0     1001      123     3132 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/function_expr/pow.rs
--rw-r--r--   0     1001      123      152 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/function_expr/rolling.rs
--rw-r--r--   0     1001      123      260 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/function_expr/round.rs
--rw-r--r--   0     1001      123      200 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/function_expr/row_hash.rs
--rw-r--r--   0     1001      123    14453 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/function_expr/schema.rs
--rw-r--r--   0     1001      123      306 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/function_expr/search_sorted.rs
--rw-r--r--   0     1001      123     3812 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/function_expr/shift_and_fill.rs
--rw-r--r--   0     1001      123     1238 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/function_expr/shrink_type.rs
--rw-r--r--   0     1001      123      972 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/function_expr/sign.rs
--rw-r--r--   0     1001      123    21047 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/function_expr/strings.rs
--rw-r--r--   0     1001      123     1017 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/function_expr/struct_.rs
--rw-r--r--   0     1001      123     5509 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/function_expr/temporal.rs
--rw-r--r--   0     1001      123     5122 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/function_expr/trigonometry.rs
--rw-r--r--   0     1001      123      170 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/function_expr/unique.rs
--rw-r--r--   0     1001      123     1155 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/functions/arity.rs
--rw-r--r--   0     1001      123      611 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/functions/coerce.rs
--rw-r--r--   0     1001      123     2717 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/functions/concat.rs
--rw-r--r--   0     1001      123     4525 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/functions/correlation.rs
--rw-r--r--   0     1001      123     8736 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/functions/horizontal.rs
--rw-r--r--   0     1001      123     1044 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/functions/index.rs
--rw-r--r--   0     1001      123      968 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/functions/mod.rs
--rw-r--r--   0     1001      123     9827 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/functions/range.rs
--rw-r--r--   0     1001      123     1308 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/functions/selectors.rs
--rw-r--r--   0     1001      123     1973 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/functions/syntactic_sugar.rs
--rw-r--r--   0     1001      123    11328 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/functions/temporal.rs
--rw-r--r--   0     1001      123    10213 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/list.rs
--rw-r--r--   0     1001      123     3772 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/meta.rs
--rw-r--r--   0     1001      123    61431 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/mod.rs
--rw-r--r--   0     1001      123       40 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/names.rs
--rw-r--r--   0     1001      123     2658 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/options.rs
--rw-r--r--   0     1001      123     1068 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/selector.rs
--rw-r--r--   0     1001      123    17095 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/string.rs
--rw-r--r--   0     1001      123     2715 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/struct_.rs
--rw-r--r--   0     1001      123       38 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/frame/mod.rs
--rw-r--r--   0     1001      123      933 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/frame/opt_state.rs
--rw-r--r--   0     1001      123      466 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/global.rs
--rw-r--r--   0     1001      123      175 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/lib.rs
--rw-r--r--   0     1001      123     8318 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/aexpr/mod.rs
--rw-r--r--   0     1001      123    11742 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/aexpr/schema.rs
--rw-r--r--   0     1001      123    25683 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/alp.rs
--rw-r--r--   0     1001      123     1622 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/anonymous_scan.rs
--rw-r--r--   0     1001      123     1428 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/apply.rs
--rw-r--r--   0     1001      123    24898 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/builder.rs
--rw-r--r--   0     1001      123    29993 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/conversion.rs
--rw-r--r--   0     1001      123      301 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/debug.rs
--rw-r--r--   0     1001      123    15470 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/format.rs
--rw-r--r--   0     1001      123      895 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/functions/drop.rs
--rw-r--r--   0     1001      123      137 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/functions/explode.rs
--rw-r--r--   0     1001      123     1169 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/functions/merge_sorted.rs
--rw-r--r--   0     1001      123    11905 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/functions/mod.rs
--rw-r--r--   0     1001      123     1330 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/functions/rename.rs
--rw-r--r--   0     1001      123    10140 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/iterator.rs
--rw-r--r--   0     1001      123    10559 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/lit.rs
--rw-r--r--   0     1001      123     8072 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/mod.rs
--rw-r--r--   0     1001      123     7416 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/optimizer/cache_states.rs
--rw-r--r--   0     1001      123    15277 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/optimizer/cse.rs
--rw-r--r--   0     1001      123     2889 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/optimizer/delay_rechunk.rs
--rw-r--r--   0     1001      123     3236 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/optimizer/drop_nulls.rs
--rw-r--r--   0     1001      123     3994 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/optimizer/fast_projection.rs
--rw-r--r--   0     1001      123    14479 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/optimizer/file_caching.rs
--rw-r--r--   0     1001      123     1556 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/optimizer/flatten_union.rs
--rw-r--r--   0     1001      123     6017 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/optimizer/fused.rs
--rw-r--r--   0     1001      123     6774 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/optimizer/mod.rs
--rw-r--r--   0     1001      123     1222 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/optimizer/predicate_pushdown/keys.rs
--rw-r--r--   0     1001      123    28901 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/optimizer/predicate_pushdown/mod.rs
--rw-r--r--   0     1001      123     2571 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/optimizer/predicate_pushdown/rename.rs
--rw-r--r--   0     1001      123    15756 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/optimizer/predicate_pushdown/utils.rs
--rw-r--r--   0     1001      123     1755 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/functions/melt.rs
--rw-r--r--   0     1001      123     3930 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/functions/mod.rs
--rw-r--r--   0     1001      123     1799 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/generic.rs
--rw-r--r--   0     1001      123     3269 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/groupby.rs
--rw-r--r--   0     1001      123     2638 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/hstack.rs
--rw-r--r--   0     1001      123    15752 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/joins.rs
--rw-r--r--   0     1001      123    26507 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/mod.rs
--rw-r--r--   0     1001      123     3707 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/projection.rs
--rw-r--r--   0     1001      123     2639 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/rename.rs
--rw-r--r--   0     1001      123     3501 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/semi_anti_join.rs
--rw-r--r--   0     1001      123    27269 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/optimizer/simplify_expr.rs
--rw-r--r--   0     1001      123     3492 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/optimizer/slice_pushdown_expr.rs
--rw-r--r--   0     1001      123    13786 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/optimizer/slice_pushdown_lp.rs
--rw-r--r--   0     1001      123     4181 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/optimizer/stack_opt.rs
--rw-r--r--   0     1001      123     9725 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/optimizer/type_coercion/binary.rs
--rw-r--r--   0     1001      123    20215 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/optimizer/type_coercion/mod.rs
--rw-r--r--   0     1001      123    10545 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/options.rs
--rw-r--r--   0     1001      123    18601 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/projection.rs
--rw-r--r--   0     1001      123     6144 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/pyarrow.rs
--rw-r--r--   0     1001      123    13026 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/schema.rs
--rw-r--r--   0     1001      123      832 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/prelude.rs
--rw-r--r--   0     1001      123    11871 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/utils.rs
--rw-r--r--   0        0        0     4393 1970-01-01 00:00:00.000000 polars_lts_cpu-0.18.2/Cargo.toml
--rw-r--r--   0     1001      123       76 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/.gitignore
--rw-r--r--   0     1001      123     1055 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/LICENSE
--rw-r--r--   0     1001      123     2414 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/Makefile
--rw-r--r--   0     1001      123    11998 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/README.md
--rw-r--r--   0     1001      123      651 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/build.rs
--rw-r--r--   0     1001      123       32 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/docs/.gitignore
--rw-r--r--   0     1001      123      679 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/docs/Makefile
--rw-r--r--   0     1001      123      318 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/docs/_templates/api_redirect.html
--rw-r--r--   0     1001      123      151 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/docs/_templates/autosummary/accessor.rst
--rw-r--r--   0     1001      123      160 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/docs/_templates/autosummary/accessor_attribute.rst
--rw-r--r--   0     1001      123      168 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/docs/_templates/autosummary/accessor_callable.rst
--rw-r--r--   0     1001      123      157 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/docs/_templates/autosummary/accessor_method.rst
--rw-r--r--   0     1001      123      836 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/docs/_templates/autosummary/class.rst
--rw-r--r--   0     1001      123       94 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/docs/_templates/autosummary/class_without_autosummary.rst
--rw-r--r--   0     1001      123      406 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/docs/_templates/sidebar-nav-bs.html
--rw-r--r--   0     1001      123      491 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/docs/requirements-docs.txt
--rw-r--r--   0     1001      123     1164 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/docs/run_live_docs_server.py
--rw-r--r--   0     1001      123     1567 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/docs/source/_static/css/custom.css
--rw-r--r--   0     1001      123     7297 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/docs/source/conf.py
--rw-r--r--   0     1001      123       51 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/docs/source/index.rst
--rw-r--r--   0     1001      123     6767 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/docs/source/reference/api.rst
--rw-r--r--   0     1001      123     2069 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/docs/source/reference/config.rst
--rw-r--r--   0     1001      123      274 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/docs/source/reference/dataframe/aggregation.rst
--rw-r--r--   0     1001      123      221 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/docs/source/reference/dataframe/attributes.rst
--rw-r--r--   0     1001      123      142 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/docs/source/reference/dataframe/computation.rst
--rw-r--r--   0     1001      123      319 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/docs/source/reference/dataframe/descriptive.rst
--rw-r--r--   0     1001      123      319 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/docs/source/reference/dataframe/export.rst
--rw-r--r--   0     1001      123      464 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/docs/source/reference/dataframe/groupby.rst
--rw-r--r--   0     1001      123      379 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/docs/source/reference/dataframe/index.rst
--rw-r--r--   0     1001      123      189 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/docs/source/reference/dataframe/miscellaneous.rst
--rw-r--r--   0     1001      123     1538 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/docs/source/reference/dataframe/modify_select.rst
--rw-r--r--   0     1001      123      673 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/docs/source/reference/datatypes.rst
--rw-r--r--   0     1001      123      421 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/docs/source/reference/exceptions.rst
--rw-r--r--   0     1001      123      391 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/docs/source/reference/expressions/aggregation.rst
--rw-r--r--   0     1001      123      267 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/docs/source/reference/expressions/array.rst
--rw-r--r--   0     1001      123      309 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/docs/source/reference/expressions/binary.rst
--rw-r--r--   0     1001      123      338 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/docs/source/reference/expressions/boolean.rst
--rw-r--r--   0     1001      123      237 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/docs/source/reference/expressions/categories.rst
--rw-r--r--   0     1001      123      221 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/docs/source/reference/expressions/columns.rst
--rw-r--r--   0     1001      123     1061 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/docs/source/reference/expressions/computation.rst
--rw-r--r--   0     1001      123     1130 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/docs/source/reference/expressions/functions.rst
--rw-r--r--   0     1001      123      470 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/docs/source/reference/expressions/index.rst
--rw-r--r--   0     1001      123      722 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/docs/source/reference/expressions/list.rst
--rw-r--r--   0     1001      123      432 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/docs/source/reference/expressions/meta.rst
--rw-r--r--   0     1001      123      159 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/docs/source/reference/expressions/miscellaneous.rst
--rw-r--r--   0     1001      123      977 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/docs/source/reference/expressions/modify_select.rst
--rw-r--r--   0     1001      123      639 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/docs/source/reference/expressions/operators.rst
--rw-r--r--   0     1001      123      951 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/docs/source/reference/expressions/string.rst
--rw-r--r--   0     1001      123      254 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/docs/source/reference/expressions/struct.rst
--rw-r--r--   0     1001      123     1036 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/docs/source/reference/expressions/temporal.rst
--rw-r--r--   0     1001      123       98 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/docs/source/reference/expressions/window.rst
--rw-r--r--   0     1001      123      836 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/docs/source/reference/functions.rst
--rw-r--r--   0     1001      123      405 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/docs/source/reference/index.rst
--rw-r--r--   0     1001      123     1294 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/docs/source/reference/io.rst
--rw-r--r--   0     1001      123      277 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/docs/source/reference/lazyframe/aggregation.rst
--rw-r--r--   0     1001      123      179 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/docs/source/reference/lazyframe/attributes.rst
--rw-r--r--   0     1001      123      146 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/docs/source/reference/lazyframe/descriptive.rst
--rw-r--r--   0     1001      123      497 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/docs/source/reference/lazyframe/groupby.rst
--rw-r--r--   0     1001      123      354 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/docs/source/reference/lazyframe/index.rst
--rw-r--r--   0     1001      123      455 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/docs/source/reference/lazyframe/miscellaneous.rst
--rw-r--r--   0     1001      123     1013 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/docs/source/reference/lazyframe/modify_select.rst
--rw-r--r--   0     1001      123     3279 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/docs/source/reference/selectors.rst
--rw-r--r--   0     1001      123      358 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/docs/source/reference/series/aggregation.rst
--rw-r--r--   0     1001      123      277 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/docs/source/reference/series/array.rst
--rw-r--r--   0     1001      123      257 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/docs/source/reference/series/attributes.rst
--rw-r--r--   0     1001      123      321 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/docs/source/reference/series/binary.rst
--rw-r--r--   0     1001      123      117 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/docs/source/reference/series/boolean.rst
--rw-r--r--   0     1001      123      241 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/docs/source/reference/series/categories.rst
--rw-r--r--   0     1001      123     1103 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/docs/source/reference/series/computation.rst
--rw-r--r--   0     1001      123      744 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/docs/source/reference/series/descriptive.rst
--rw-r--r--   0     1001      123      240 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/docs/source/reference/series/export.rst
--rw-r--r--   0     1001      123      437 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/docs/source/reference/series/index.rst
--rw-r--r--   0     1001      123      776 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/docs/source/reference/series/list.rst
--rw-r--r--   0     1001      123      236 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/docs/source/reference/series/miscellaneous.rst
--rw-r--r--   0     1001      123     1077 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/docs/source/reference/series/modify_select.rst
--rw-r--r--   0     1001      123     1021 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/docs/source/reference/series/string.rst
--rw-r--r--   0     1001      123      421 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/docs/source/reference/series/struct.rst
--rw-r--r--   0     1001      123     1192 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/docs/source/reference/series/temporal.rst
--rw-r--r--   0     1001      123      503 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/docs/source/reference/sql.rst
--rw-r--r--   0     1001      123     8067 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/docs/source/reference/testing.rst
--rw-r--r--   0     1001      123      168 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/docs/source/reference/utils.rst
--rw-r--r--   0     1001      123     6161 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/__init__.py
--rw-r--r--   0     1001      123      280 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/_reexport.py
--rw-r--r--   0     1001      123    13229 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/api.py
--rw-r--r--   0     1001      123    29008 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/config.py
--rw-r--r--   0     1001      123    28105 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/convert.py
--rw-r--r--   0     1001      123       77 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/dataframe/__init__.py
--rw-r--r--   0     1001      123     5227 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/dataframe/_html.py
--rw-r--r--   0     1001      123   315508 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/dataframe/frame.py
--rw-r--r--   0     1001      123    40637 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/dataframe/groupby.py
--rw-r--r--   0     1001      123     2692 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/datatypes/__init__.py
--rw-r--r--   0     1001      123    16199 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/datatypes/classes.py
--rw-r--r--   0     1001      123     1603 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/datatypes/constants.py
--rw-r--r--   0     1001      123     4701 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/datatypes/constructor.py
--rw-r--r--   0     1001      123    15739 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/datatypes/convert.py
--rw-r--r--   0     1001      123     7338 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/dependencies.py
--rw-r--r--   0     1001      123     3573 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/exceptions.py
--rw-r--r--   0     1001      123       61 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/expr/__init__.py
--rw-r--r--   0     1001      123     3020 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/expr/array.py
--rw-r--r--   0     1001      123     2704 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/expr/binary.py
--rw-r--r--   0     1001      123     1698 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/expr/categorical.py
--rw-r--r--   0     1001      123    77598 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/expr/datetime.py
--rw-r--r--   0     1001      123   261537 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/expr/expr.py
--rw-r--r--   0     1001      123    23905 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/expr/list.py
--rw-r--r--   0     1001      123     4050 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/expr/meta.py
--rw-r--r--   0     1001      123    59014 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/expr/string.py
--rw-r--r--   0     1001      123     5426 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/expr/struct.py
--rw-r--r--   0     1001      123     2068 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/functions/__init__.py
--rw-r--r--   0     1001      123    16541 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/functions/as_datatype.py
--rw-r--r--   0     1001      123    18358 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/functions/eager.py
--rw-r--r--   0     1001      123    72401 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/functions/lazy.py
--rw-r--r--   0     1001      123    16227 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/functions/range.py
--rw-r--r--   0     1001      123     6027 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/functions/repeat.py
--rw-r--r--   0     1001      123     6139 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/functions/whenthen.py
--rw-r--r--   0     1001      123      952 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/io/__init__.py
--rw-r--r--   0     1001      123     6264 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/io/_utils.py
--rw-r--r--   0     1001      123      861 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/io/avro.py
--rw-r--r--   0     1001      123      144 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/io/csv/__init__.py
--rw-r--r--   0     1001      123     1072 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/io/csv/_utils.py
--rw-r--r--   0     1001      123     4681 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/io/csv/batched_reader.py
--rw-r--r--   0     1001      123    35482 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/io/csv/functions.py
--rw-r--r--   0     1001      123     5627 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/io/database.py
--rw-r--r--   0     1001      123    11047 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/io/delta.py
--rw-r--r--   0     1001      123       75 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/io/excel/__init__.py
--rw-r--r--   0     1001      123    18449 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/io/excel/_write_utils.py
--rw-r--r--   0     1001      123     6466 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/io/excel/functions.py
--rw-r--r--   0     1001      123      142 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/io/ipc/__init__.py
--rw-r--r--   0     1001      123     1227 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/io/ipc/anonymous_scan.py
--rw-r--r--   0     1001      123     5804 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/io/ipc/functions.py
--rw-r--r--   0     1001      123      502 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/io/json.py
--rw-r--r--   0     1001      123     2207 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/io/ndjson.py
--rw-r--r--   0     1001      123      170 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/io/parquet/__init__.py
--rw-r--r--   0     1001      123     1259 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/io/parquet/anonymous_scan.py
--rw-r--r--   0     1001      123     7177 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/io/parquet/functions.py
--rw-r--r--   0     1001      123      136 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/io/pyarrow_dataset/__init__.py
--rw-r--r--   0     1001      123     2291 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/io/pyarrow_dataset/anonymous_scan.py
--rw-r--r--   0     1001      123     3601 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/io/pyarrow_dataset/functions.py
--rw-r--r--   0     1001      123       77 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/lazyframe/__init__.py
--rw-r--r--   0     1001      123   168214 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/lazyframe/frame.py
--rw-r--r--   0     1001      123    24078 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/lazyframe/groupby.py
--rw-r--r--   0     1001      123        0 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/py.typed
--rw-r--r--   0     1001      123    32502 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/selectors.py
--rw-r--r--   0     1001      123       69 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/series/__init__.py
--rw-r--r--   0     1001      123     1572 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/series/_numpy.py
--rw-r--r--   0     1001      123     2515 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/series/array.py
--rw-r--r--   0     1001      123     1913 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/series/binary.py
--rw-r--r--   0     1001      123     1692 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/series/categorical.py
--rw-r--r--   0     1001      123    51711 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/series/datetime.py
--rw-r--r--   0     1001      123    13196 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/series/list.py
--rw-r--r--   0     1001      123   170010 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/series/series.py
--rw-r--r--   0     1001      123    37808 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/series/string.py
--rw-r--r--   0     1001      123     2542 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/series/struct.py
--rw-r--r--   0     1001      123     5361 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/series/utils.py
--rw-r--r--   0     1001      123     7559 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/slice.py
--rw-r--r--   0     1001      123       75 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/sql/__init__.py
--rw-r--r--   0     1001      123    17409 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/sql/context.py
--rw-r--r--   0     1001      123     4793 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/string_cache.py
--rw-r--r--   0     1001      123      362 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/testing/__init__.py
--rw-r--r--   0     1001      123     1060 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/testing/_private.py
--rw-r--r--   0     1001      123    16425 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/testing/asserts.py
--rw-r--r--   0     1001      123      898 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/testing/parametric/__init__.py
--rw-r--r--   0     1001      123    26833 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/testing/parametric/primitives.py
--rw-r--r--   0     1001      123     3409 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/testing/parametric/profiles.py
--rw-r--r--   0     1001      123    12132 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/testing/parametric/strategies.py
--rw-r--r--   0     1001      123     6214 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/type_aliases.py
--rw-r--r--   0     1001      123     1169 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/utils/__init__.py
--rw-r--r--   0     1001      123    54302 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/utils/_construction.py
--rw-r--r--   0     1001      123     3902 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/utils/_parse_expr_input.py
--rw-r--r--   0     1001      123      711 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/utils/_scan.py
--rw-r--r--   0     1001      123      579 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/utils/_wrap.py
--rw-r--r--   0     1001      123      683 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/utils/build_info.py
--rw-r--r--   0     1001      123     8609 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/utils/convert.py
--rw-r--r--   0     1001      123     6132 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/utils/decorators.py
--rw-r--r--   0     1001      123     1660 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/utils/meta.py
--rw-r--r--   0     1001      123      514 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/utils/polars_version.py
--rw-r--r--   0     1001      123     2673 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/utils/show_versions.py
--rw-r--r--   0     1001      123    12905 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/utils/various.py
--rw-r--r--   0     1001      123     5375 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/pyproject.toml
--rw-r--r--   0     1001      123      697 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/requirements-dev.txt
--rw-r--r--   0     1001      123       68 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/requirements-lint.txt
--rw-r--r--   0     1001      123     1640 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/scripts/check_stacklevels.py
--rw-r--r--   0     1001      123    10980 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/src/apply/dataframe.rs
--rw-r--r--   0     1001      123     7448 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/src/apply/lazy.rs
--rw-r--r--   0     1001      123     8402 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/src/apply/mod.rs
--rw-r--r--   0     1001      123    90009 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/src/apply/series.rs
--rw-r--r--   0     1001      123       32 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/src/arrow_interop/mod.rs
--rw-r--r--   0     1001      123     1306 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/src/arrow_interop/to_py.rs
--rw-r--r--   0     1001      123     3902 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/src/arrow_interop/to_rust.rs
--rw-r--r--   0     1001      123     5250 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/src/batched_csv.rs
--rw-r--r--   0     1001      123    48675 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/src/conversion.rs
--rw-r--r--   0     1001      123    45928 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/src/dataframe.rs
--rw-r--r--   0     1001      123     3950 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/src/datatypes.rs
--rw-r--r--   0     1001      123     3288 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/src/error.rs
--rw-r--r--   0     1001      123      570 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/src/expr/array.rs
--rw-r--r--   0     1001      123     2080 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/src/expr/binary.rs
--rw-r--r--   0     1001      123      274 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/src/expr/categorical.rs
--rw-r--r--   0     1001      123     5935 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/src/expr/datetime.rs
--rw-r--r--   0     1001      123    34040 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/src/expr/general.rs
--rw-r--r--   0     1001      123     3937 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/src/expr/list.rs
--rw-r--r--   0     1001      123     2907 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/src/expr/meta.rs
--rw-r--r--   0     1001      123      870 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/src/expr/mod.rs
--rw-r--r--   0     1001      123     8677 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/src/expr/string.rs
--rw-r--r--   0     1001      123      467 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/src/expr/struct.rs
--rw-r--r--   0     1001      123     9482 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/src/file.rs
--rw-r--r--   0     1001      123     3307 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/src/functions/eager.rs
--rw-r--r--   0     1001      123     1657 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/src/functions/io.rs
--rw-r--r--   0     1001      123    11835 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/src/functions/lazy.rs
--rw-r--r--   0     1001      123     1312 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/src/functions/meta.rs
--rw-r--r--   0     1001      123      217 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/src/functions/misc.rs
--rw-r--r--   0     1001      123       87 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/src/functions/mod.rs
--rw-r--r--   0     1001      123     1474 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/src/functions/whenthen.rs
--rw-r--r--   0     1001      123    30767 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/src/lazyframe.rs
--rw-r--r--   0     1001      123     2670 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/src/lazygroupby.rs
--rw-r--r--   0     1001      123     8268 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/src/lib.rs
--rw-r--r--   0     1001      123     1029 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/src/object.rs
--rw-r--r--   0     1001      123      122 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/src/prelude.rs
--rw-r--r--   0     1001      123      435 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/src/py_modules.rs
--rw-r--r--   0     1001      123     1964 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/src/series/aggregation.rs
--rw-r--r--   0     1001      123     5406 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/src/series/arithmetic.rs
--rw-r--r--   0     1001      123     5138 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/src/series/comparison.rs
--rw-r--r--   0     1001      123     9077 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/src/series/construction.rs
--rw-r--r--   0     1001      123     8971 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/src/series/export.rs
--rw-r--r--   0     1001      123    26521 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/src/series/mod.rs
--rw-r--r--   0     1001      123     4569 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/src/series/numpy_ufunc.rs
--rw-r--r--   0     1001      123     4046 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/src/series/set_at_idx.rs
--rw-r--r--   0     1001      123     1036 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/src/sql.rs
--rw-r--r--   0     1001      123     2335 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/src/utils.rs
--rw-r--r--   0     1001      123     6165 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/README.md
--rw-r--r--   0     1001      123     2189 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/benchmark/groupby-datagen.R
--rw-r--r--   0     1001      123     7963 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/benchmark/run_h2oai_benchmark.py
--rw-r--r--   0     1001      123     6530 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/benchmark/test_release.py
--rw-r--r--   0     1001      123     4589 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/docs/run_doctest.py
--rw-r--r--   0     1001      123      179 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/parametric/conftest.py
--rw-r--r--   0     1001      123     3856 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/parametric/test_dataframe.py
--rw-r--r--   0     1001      123     1692 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/parametric/test_lazyframe.py
--rw-r--r--   0     1001      123     6897 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/parametric/test_series.py
--rw-r--r--   0     1001      123     8299 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/parametric/test_testing.py
--rw-r--r--   0     1001      123        0 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/__init__.py
--rw-r--r--   0     1001      123     3382 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/conftest.py
--rw-r--r--   0     1001      123       86 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/datatypes/__init__.py
--rw-r--r--   0     1001      123      973 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/datatypes/test_array.py
--rw-r--r--   0     1001      123      847 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/datatypes/test_binary.py
--rw-r--r--   0     1001      123     1420 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/datatypes/test_bool.py
--rw-r--r--   0     1001      123    13228 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/datatypes/test_categorical.py
--rw-r--r--   0     1001      123     5222 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/datatypes/test_decimal.py
--rw-r--r--   0     1001      123      549 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/datatypes/test_duration.py
--rw-r--r--   0     1001      123      423 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/datatypes/test_integer.py
--rw-r--r--   0     1001      123    13216 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/datatypes/test_list.py
--rw-r--r--   0     1001      123      284 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/datatypes/test_null.py
--rw-r--r--   0     1001      123     2801 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/datatypes/test_object.py
--rw-r--r--   0     1001      123    27749 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/datatypes/test_struct.py
--rw-r--r--   0     1001      123    87542 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/datatypes/test_temporal.py
--rw-r--r--   0     1001      123      418 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/datatypes/test_time.py
--rw-r--r--   0     1001      123        0 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/functions/__init__.py
--rw-r--r--   0     1001      123    13970 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/functions/test_as_datatype.py
--rw-r--r--   0     1001      123      480 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/functions/test_concat.py
--rw-r--r--   0     1001      123    15610 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/functions/test_functions.py
--rw-r--r--   0     1001      123    18470 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/functions/test_range.py
--rw-r--r--   0     1001      123     3724 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/functions/test_repeat.py
--rw-r--r--   0     1001      123      218 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/io/conftest.py
--rw-r--r--   0     1001      123       16 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/io/files/delta-table/.part-00000-e42312d7-60e5-454d-acbc-db192d220e73-c000.snappy.parquet.crc
--rw-r--r--   0     1001      123       16 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/io/files/delta-table/.part-00000-e4a999da-df45-4fb0-bdc4-d999fc0f58aa-c000.snappy.parquet.crc
--rw-r--r--   0     1001      123       16 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/io/files/delta-table/_delta_log/.00000000000000000000.json.crc
--rw-r--r--   0     1001      123       16 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/io/files/delta-table/_delta_log/.00000000000000000001.json.crc
--rw-r--r--   0     1001      123      905 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/io/files/delta-table/_delta_log/00000000000000000000.json
--rw-r--r--   0     1001      123      936 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/io/files/delta-table/_delta_log/00000000000000000001.json
--rw-r--r--   0     1001      123      972 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/io/files/delta-table/part-00000-e42312d7-60e5-454d-acbc-db192d220e73-c000.snappy.parquet
--rw-r--r--   0     1001      123      690 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/io/files/delta-table/part-00000-e4a999da-df45-4fb0-bdc4-d999fc0f58aa-c000.snappy.parquet
--rw-r--r--   0     1001      123        0 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/io/files/empty.csv
--rw-r--r--   0     1001      123     5959 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/io/files/example.xlsx
--rw-r--r--   0     1001      123      457 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/io/files/foods1.csv
--rw-r--r--   0     1001      123     2351 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/io/files/foods1.ipc
--rw-r--r--   0     1001      123     1713 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/io/files/foods1.ndjson
--rw-r--r--   0     1001      123     1427 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/io/files/foods1.parquet
--rw-r--r--   0     1001      123      455 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/io/files/foods2.csv
--rw-r--r--   0     1001      123     2351 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/io/files/foods2.ipc
--rw-r--r--   0     1001      123     1711 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/io/files/foods2.ndjson
--rw-r--r--   0     1001      123     1916 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/io/files/foods2.parquet
--rw-r--r--   0     1001      123      455 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/io/files/foods3.csv
--rw-r--r--   0     1001      123      457 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/io/files/foods4.csv
--rw-r--r--   0     1001      123      452 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/io/files/foods5.csv
--rw-r--r--   0     1001      123       49 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/io/files/gzipped.csv
--rw-r--r--   0     1001      123       57 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/io/files/small.csv
--rw-r--r--   0     1001      123      756 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/io/files/small.parquet
--rw-r--r--   0     1001      123     1884 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/io/test_avro.py
--rw-r--r--   0     1001      123    39230 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/io/test_csv.py
--rw-r--r--   0     1001      123     6336 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/io/test_database.py
--rw-r--r--   0     1001      123     6172 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/io/test_delta.py
--rw-r--r--   0     1001      123    11169 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/io/test_excel.py
--rw-r--r--   0     1001      123     5483 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/io/test_ipc.py
--rw-r--r--   0     1001      123     3986 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/io/test_json.py
--rw-r--r--   0     1001      123     7379 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/io/test_lazy_csv.py
--rw-r--r--   0     1001      123     2060 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/io/test_lazy_ipc.py
--rw-r--r--   0     1001      123     2867 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/io/test_lazy_json.py
--rw-r--r--   0     1001      123    11145 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/io/test_lazy_parquet.py
--rw-r--r--   0     1001      123     2012 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/io/test_other.py
--rw-r--r--   0     1001      123    13738 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/io/test_parquet.py
--rw-r--r--   0     1001      123      612 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/io/test_pickle.py
--rw-r--r--   0     1001      123     3686 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/io/test_pyarrow_dataset.py
--rw-r--r--   0     1001      123      509 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/namespaces/__init__.py
--rw-r--r--   0     1001      123      589 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/namespaces/test_array.py
--rw-r--r--   0     1001      123     3218 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/namespaces/test_binary.py
--rw-r--r--   0     1001      123     2489 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/namespaces/test_categorical.py
--rw-r--r--   0     1001      123    19585 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/namespaces/test_datetime.py
--rw-r--r--   0     1001      123    14067 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/namespaces/test_list.py
--rw-r--r--   0     1001      123     1829 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/namespaces/test_meta.py
--rw-r--r--   0     1001      123    23544 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/namespaces/test_string.py
--rw-r--r--   0     1001      123    17964 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/namespaces/test_strptime.py
--rw-r--r--   0     1001      123      982 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/namespaces/test_struct.py
--rw-r--r--   0     1001      123       85 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/operations/__init__.py
--rw-r--r--   0     1001      123     7755 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/operations/test_aggregations.py
--rw-r--r--   0     1001      123    10643 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/operations/test_apply.py
--rw-r--r--   0     1001      123     6932 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/operations/test_arithmetic.py
--rw-r--r--   0     1001      123     4631 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/operations/test_comparison.py
--rw-r--r--   0     1001      123     3275 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/operations/test_drop.py
--rw-r--r--   0     1001      123     8813 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/operations/test_explode.py
--rw-r--r--   0     1001      123     3664 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/operations/test_filter.py
--rw-r--r--   0     1001      123     1801 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/operations/test_folds.py
--rw-r--r--   0     1001      123    24998 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/operations/test_groupby.py
--rw-r--r--   0     1001      123     7649 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/operations/test_groupby_rolling.py
--rw-r--r--   0     1001      123     2983 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/operations/test_is_in.py
--rw-r--r--   0     1001      123    18169 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/operations/test_join.py
--rw-r--r--   0     1001      123    14612 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/operations/test_join_asof.py
--rw-r--r--   0     1001      123      643 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/operations/test_melt.py
--rw-r--r--   0     1001      123    10253 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/operations/test_pivot.py
--rw-r--r--   0     1001      123    19818 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/operations/test_rolling.py
--rw-r--r--   0     1001      123     1917 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/operations/test_select.py
--rw-r--r--   0     1001      123    20578 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/operations/test_sort.py
--rw-r--r--   0     1001      123     4273 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/operations/test_statistics.py
--rw-r--r--   0     1001      123     4130 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/operations/test_transpose.py
--rw-r--r--   0     1001      123      771 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/operations/test_unique.py
--rw-r--r--   0     1001      123    11694 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/operations/test_window.py
--rw-r--r--   0     1001      123     5401 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/operations/test_with_columns.py
--rw-r--r--   0     1001      123        0 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/streaming/__init__.py
--rw-r--r--   0     1001      123      196 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/streaming/conftest.py
--rw-r--r--   0     1001      123      908 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/streaming/test_ooc.py
--rw-r--r--   0     1001      123    16053 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/streaming/test_streaming.py
--rw-r--r--   0     1001      123     4775 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/test_api.py
--rw-r--r--   0     1001      123     1077 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/test_arity.py
--rw-r--r--   0     1001      123    20002 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/test_cfg.py
--rw-r--r--   0     1001      123    42513 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/test_constructors.py
--rw-r--r--   0     1001      123      454 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/test_context.py
--rw-r--r--   0     1001      123     1628 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/test_cse.py
--rw-r--r--   0     1001      123     5198 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/test_datatypes.py
--rw-r--r--   0     1001      123   119414 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/test_df.py
--rw-r--r--   0     1001      123     2151 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/test_empty.py
--rw-r--r--   0     1001      123    18790 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/test_errors.py
--rw-r--r--   0     1001      123     2741 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/test_expr_multi_cols.py
--rw-r--r--   0     1001      123    34736 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/test_exprs.py
--rw-r--r--   0     1001      123     3516 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/test_fmt.py
--rw-r--r--   0     1001      123     3763 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/test_interchange.py
--rw-r--r--   0     1001      123    38286 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/test_interop.py
--rw-r--r--   0     1001      123    47730 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/test_lazy.py
--rw-r--r--   0     1001      123     2463 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/test_polars_import.py
--rw-r--r--   0     1001      123     4610 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/test_predicates.py
--rw-r--r--   0     1001      123     7073 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/test_projections.py
--rw-r--r--   0     1001      123    11551 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/test_queries.py
--rw-r--r--   0     1001      123     4743 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/test_rows.py
--rw-r--r--   0     1001      123    13394 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/test_schema.py
--rw-r--r--   0     1001      123     7419 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/test_selectors.py
--rw-r--r--   0     1001      123     2823 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/test_serde.py
--rw-r--r--   0     1001      123    83729 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/test_series.py
--rw-r--r--   0     1001      123      657 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/test_single.py
--rw-r--r--   0     1001      123     6747 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/test_sql.py
--rw-r--r--   0     1001      123    12957 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/test_testing.py
--rw-r--r--   0     1001      123       41 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/utils/__init__.py
--rw-r--r--   0     1001      123      306 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/utils/test_build_info.py
--rw-r--r--   0     1001      123     2784 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/utils/test_parse_expr_input.py
--rw-r--r--   0     1001      123      247 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/utils/test_show_versions.py
--rw-r--r--   0     1001      123     5026 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/utils/test_utils.py
--rw-r--r--   0     1001      123    63894 2023-06-09 08:26:02.000000 polars_lts_cpu-0.18.2/Cargo.lock
--rw-r--r--   0        0        0    14545 1970-01-01 00:00:00.000000 polars_lts_cpu-0.18.2/PKG-INFO
+-rw-r--r--   0        0        0      954 1970-01-01 00:00:00.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-row/Cargo.toml
+-rw-r--r--   0     1001      123     1055 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-row/LICENSE
+-rw-r--r--   0     1001      123      137 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-row/README.md
+-rw-r--r--   0     1001      123     1916 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-row/src/decode.rs
+-rw-r--r--   0     1001      123    11571 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-row/src/encode.rs
+-rw-r--r--   0     1001      123     7436 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-row/src/fixed.rs
+-rw-r--r--   0     1001      123    13846 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-row/src/lib.rs
+-rw-r--r--   0     1001      123     3019 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-row/src/row.rs
+-rw-r--r--   0     1001      123      682 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-row/src/utils.rs
+-rw-r--r--   0     1001      123     7559 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-row/src/variable.rs
+-rw-r--r--   0        0        0     3439 1970-01-01 00:00:00.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-ops/Cargo.toml
+-rw-r--r--   0     1001      123     1055 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-ops/LICENSE
+-rw-r--r--   0     1001      123      132 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-ops/README.md
+-rw-r--r--   0     1001      123     2382 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-ops/src/chunked_array/array/min_max.rs
+-rw-r--r--   0     1001      123      267 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-ops/src/chunked_array/array/mod.rs
+-rw-r--r--   0     1001      123     1512 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-ops/src/chunked_array/array/namespace.rs
+-rw-r--r--   0     1001      123     4108 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-ops/src/chunked_array/array/sum_mean.rs
+-rw-r--r--   0     1001      123      234 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-ops/src/chunked_array/binary/mod.rs
+-rw-r--r--   0     1001      123     3549 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-ops/src/chunked_array/binary/namespace.rs
+-rw-r--r--   0     1001      123    11023 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-ops/src/chunked_array/interpolate.rs
+-rw-r--r--   0     1001      123     1687 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-ops/src/chunked_array/list/count.rs
+-rw-r--r--   0     1001      123     2419 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-ops/src/chunked_array/list/hash.rs
+-rw-r--r--   0     1001      123     7861 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-ops/src/chunked_array/list/min_max.rs
+-rw-r--r--   0     1001      123      511 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-ops/src/chunked_array/list/mod.rs
+-rw-r--r--   0     1001      123    19010 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-ops/src/chunked_array/list/namespace.rs
+-rw-r--r--   0     1001      123     7633 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-ops/src/chunked_array/list/sum_mean.rs
+-rw-r--r--   0     1001      123     2435 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-ops/src/chunked_array/list/to_struct.rs
+-rw-r--r--   0     1001      123      545 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-ops/src/chunked_array/mod.rs
+-rw-r--r--   0     1001      123     9452 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-ops/src/chunked_array/nan_propagating_aggregate.rs
+-rw-r--r--   0     1001      123     6795 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-ops/src/chunked_array/set.rs
+-rw-r--r--   0     1001      123     7490 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-ops/src/chunked_array/strings/case.rs
+-rw-r--r--   0     1001      123     8409 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-ops/src/chunked_array/strings/json_path.rs
+-rw-r--r--   0     1001      123     2345 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-ops/src/chunked_array/strings/justify.rs
+-rw-r--r--   0     1001      123      514 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-ops/src/chunked_array/strings/mod.rs
+-rw-r--r--   0     1001      123    14731 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-ops/src/chunked_array/strings/namespace.rs
+-rw-r--r--   0     1001      123     4053 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-ops/src/chunked_array/strings/replace.rs
+-rw-r--r--   0     1001      123      439 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-ops/src/chunked_array/sum.rs
+-rw-r--r--   0     1001      123     2486 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-ops/src/chunked_array/top_k.rs
+-rw-r--r--   0     1001      123     7727 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-ops/src/frame/join/merge_sorted.rs
+-rw-r--r--   0     1001      123    18232 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-ops/src/frame/join/mod.rs
+-rw-r--r--   0     1001      123     4174 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-ops/src/frame/mod.rs
+-rw-r--r--   0     1001      123    10257 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-ops/src/frame/pivot/mod.rs
+-rw-r--r--   0     1001      123    13486 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-ops/src/frame/pivot/positioning.rs
+-rw-r--r--   0     1001      123      237 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-ops/src/lib.rs
+-rw-r--r--   0     1001      123      290 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-ops/src/prelude.rs
+-rw-r--r--   0     1001      123       25 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-ops/src/series/mod.rs
+-rw-r--r--   0     1001      123     9623 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-ops/src/series/ops/approx_algo/hyperloglogplus.rs
+-rw-r--r--   0     1001      123      118 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-ops/src/series/ops/approx_algo/mod.rs
+-rw-r--r--   0     1001      123     2016 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-ops/src/series/ops/approx_unique.rs
+-rw-r--r--   0     1001      123    11866 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-ops/src/series/ops/arg_min_max.rs
+-rw-r--r--   0     1001      123     3688 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-ops/src/series/ops/floor_divide.rs
+-rw-r--r--   0     1001      123     5245 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-ops/src/series/ops/fused.rs
+-rw-r--r--   0     1001      123     3423 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-ops/src/series/ops/is_first.rs
+-rw-r--r--   0     1001      123     2975 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-ops/src/series/ops/is_unique.rs
+-rw-r--r--   0     1001      123     3626 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-ops/src/series/ops/log.rs
+-rw-r--r--   0     1001      123     1187 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-ops/src/series/ops/mod.rs
+-rw-r--r--   0     1001      123     1769 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-ops/src/series/ops/rolling.rs
+-rw-r--r--   0     1001      123     7642 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-ops/src/series/ops/search_sorted.rs
+-rw-r--r--   0     1001      123     2500 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-ops/src/series/ops/to_dummies.rs
+-rw-r--r--   0     1001      123     2067 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-ops/src/series/ops/various.rs
+-rw-r--r--   0        0        0     5971 1970-01-01 00:00:00.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-lazy/Cargo.toml
+-rw-r--r--   0     1001      123     1055 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-lazy/LICENSE
+-rw-r--r--   0     1001      123      358 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-lazy/README.md
+-rw-r--r--   0     1001      123     1796 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-lazy/src/dot.rs
+-rw-r--r--   0     1001      123     4479 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-lazy/src/dsl/eval.rs
+-rw-r--r--   0     1001      123     7115 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-lazy/src/dsl/functions.rs
+-rw-r--r--   0     1001      123      164 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-lazy/src/dsl/into.rs
+-rw-r--r--   0     1001      123     6754 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-lazy/src/dsl/list.rs
+-rw-r--r--   0     1001      123     2899 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-lazy/src/dsl/mod.rs
+-rw-r--r--   0     1001      123     1182 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-lazy/src/frame/anonymous_scan.rs
+-rw-r--r--   0     1001      123     9285 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-lazy/src/frame/csv.rs
+-rw-r--r--   0     1001      123     4316 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-lazy/src/frame/file_list_reader.rs
+-rw-r--r--   0     1001      123     2261 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-lazy/src/frame/ipc.rs
+-rw-r--r--   0     1001      123    49023 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-lazy/src/frame/mod.rs
+-rw-r--r--   0     1001      123     3414 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-lazy/src/frame/ndjson.rs
+-rw-r--r--   0     1001      123     2734 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-lazy/src/frame/parquet.rs
+-rw-r--r--   0     1001      123     2892 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-lazy/src/frame/pivot.rs
+-rw-r--r--   0     1001      123      416 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-lazy/src/frame/python.rs
+-rw-r--r--   0     1001      123     6374 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-lazy/src/lib.rs
+-rw-r--r--   0     1001      123     1049 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-lazy/src/physical_plan/executors/cache.rs
+-rw-r--r--   0     1001      123      776 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-lazy/src/physical_plan/executors/executor.rs
+-rw-r--r--   0     1001      123      670 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-lazy/src/physical_plan/executors/ext_context.rs
+-rw-r--r--   0     1001      123     1555 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-lazy/src/physical_plan/executors/filter.rs
+-rw-r--r--   0     1001      123     3986 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-lazy/src/physical_plan/executors/groupby.rs
+-rw-r--r--   0     1001      123     4125 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-lazy/src/physical_plan/executors/groupby_dynamic.rs
+-rw-r--r--   0     1001      123    13599 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-lazy/src/physical_plan/executors/groupby_partitioned.rs
+-rw-r--r--   0     1001      123     4883 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-lazy/src/physical_plan/executors/groupby_rolling.rs
+-rw-r--r--   0     1001      123     5859 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-lazy/src/physical_plan/executors/join.rs
+-rw-r--r--   0     1001      123     6753 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-lazy/src/physical_plan/executors/mod.rs
+-rw-r--r--   0     1001      123     2045 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-lazy/src/physical_plan/executors/projection.rs
+-rw-r--r--   0     1001      123     1677 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-lazy/src/physical_plan/executors/python_scan.rs
+-rw-r--r--   0     1001      123     2854 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-lazy/src/physical_plan/executors/scan/csv.rs
+-rw-r--r--   0     1001      123     1963 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-lazy/src/physical_plan/executors/scan/ipc.rs
+-rw-r--r--   0     1001      123     4303 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-lazy/src/physical_plan/executors/scan/mod.rs
+-rw-r--r--   0     1001      123     1209 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-lazy/src/physical_plan/executors/scan/ndjson.rs
+-rw-r--r--   0     1001      123     2421 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-lazy/src/physical_plan/executors/scan/parquet.rs
+-rw-r--r--   0     1001      123      548 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-lazy/src/physical_plan/executors/slice.rs
+-rw-r--r--   0     1001      123     2197 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-lazy/src/physical_plan/executors/sort.rs
+-rw-r--r--   0     1001      123     2015 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-lazy/src/physical_plan/executors/stack.rs
+-rw-r--r--   0     1001      123      663 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-lazy/src/physical_plan/executors/udf.rs
+-rw-r--r--   0     1001      123     4041 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-lazy/src/physical_plan/executors/union.rs
+-rw-r--r--   0     1001      123      838 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-lazy/src/physical_plan/executors/unique.rs
+-rw-r--r--   0     1001      123     1335 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-lazy/src/physical_plan/exotic.rs
+-rw-r--r--   0     1001      123    21959 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-lazy/src/physical_plan/expressions/aggregation.rs
+-rw-r--r--   0     1001      123     2689 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-lazy/src/physical_plan/expressions/alias.rs
+-rw-r--r--   0     1001      123    18331 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-lazy/src/physical_plan/expressions/apply.rs
+-rw-r--r--   0     1001      123    17197 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-lazy/src/physical_plan/expressions/binary.rs
+-rw-r--r--   0     1001      123     2583 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-lazy/src/physical_plan/expressions/cache.rs
+-rw-r--r--   0     1001      123     3153 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-lazy/src/physical_plan/expressions/cast.rs
+-rw-r--r--   0     1001      123     6326 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-lazy/src/physical_plan/expressions/column.rs
+-rw-r--r--   0     1001      123     1996 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-lazy/src/physical_plan/expressions/count.rs
+-rw-r--r--   0     1001      123     5809 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-lazy/src/physical_plan/expressions/filter.rs
+-rw-r--r--   0     1001      123     4131 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-lazy/src/physical_plan/expressions/group_iter.rs
+-rw-r--r--   0     1001      123     5304 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-lazy/src/physical_plan/expressions/literal.rs
+-rw-r--r--   0     1001      123    23566 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-lazy/src/physical_plan/expressions/mod.rs
+-rw-r--r--   0     1001      123    10091 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-lazy/src/physical_plan/expressions/slice.rs
+-rw-r--r--   0     1001      123     4332 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-lazy/src/physical_plan/expressions/sort.rs
+-rw-r--r--   0     1001      123    13549 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-lazy/src/physical_plan/expressions/sortby.rs
+-rw-r--r--   0     1001      123     8331 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-lazy/src/physical_plan/expressions/take.rs
+-rw-r--r--   0     1001      123    14360 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-lazy/src/physical_plan/expressions/ternary.rs
+-rw-r--r--   0     1001      123    31558 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-lazy/src/physical_plan/expressions/window.rs
+-rw-r--r--   0     1001      123     2039 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-lazy/src/physical_plan/file_cache.rs
+-rw-r--r--   0     1001      123      414 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-lazy/src/physical_plan/mod.rs
+-rw-r--r--   0     1001      123     2005 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-lazy/src/physical_plan/node_timer.rs
+-rw-r--r--   0     1001      123    24050 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-lazy/src/physical_plan/planner/expr.rs
+-rw-r--r--   0     1001      123    20552 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-lazy/src/physical_plan/planner/lp.rs
+-rw-r--r--   0     1001      123       87 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-lazy/src/physical_plan/planner/mod.rs
+-rw-r--r--   0     1001      123     9647 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-lazy/src/physical_plan/state.rs
+-rw-r--r--   0     1001      123     2583 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-lazy/src/physical_plan/streaming/checks.rs
+-rw-r--r--   0     1001      123     9227 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-lazy/src/physical_plan/streaming/construct_pipeline.rs
+-rw-r--r--   0     1001      123    16847 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-lazy/src/physical_plan/streaming/convert_alp.rs
+-rw-r--r--   0     1001      123      116 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-lazy/src/physical_plan/streaming/mod.rs
+-rw-r--r--   0     1001      123     5827 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-lazy/src/physical_plan/streaming/tree.rs
+-rw-r--r--   0     1001      123      722 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-lazy/src/prelude.rs
+-rw-r--r--   0     1001      123    14990 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-lazy/src/tests/aggregations.rs
+-rw-r--r--   0     1001      123     2339 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-lazy/src/tests/arity.rs
+-rw-r--r--   0     1001      123     7276 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-lazy/src/tests/cse.rs
+-rw-r--r--   0     1001      123    12759 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-lazy/src/tests/io.rs
+-rw-r--r--   0     1001      123     4166 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-lazy/src/tests/logical.rs
+-rw-r--r--   0     1001      123     4273 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-lazy/src/tests/mod.rs
+-rw-r--r--   0     1001      123    15770 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-lazy/src/tests/optimization_checks.rs
+-rw-r--r--   0     1001      123     6772 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-lazy/src/tests/predicate_queries.rs
+-rw-r--r--   0     1001      123     3165 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-lazy/src/tests/projection_queries.rs
+-rw-r--r--   0     1001      123    47687 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-lazy/src/tests/queries.rs
+-rw-r--r--   0     1001      123     9519 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-lazy/src/tests/streaming.rs
+-rw-r--r--   0     1001      123     2893 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-lazy/src/tests/tpch.rs
+-rw-r--r--   0     1001      123     1028 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-lazy/src/utils.rs
+-rw-r--r--   0        0        0      569 1970-01-01 00:00:00.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-utils/Cargo.toml
+-rw-r--r--   0     1001      123     1055 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-utils/LICENSE
+-rw-r--r--   0     1001      123      141 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-utils/README.md
+-rw-r--r--   0     1001      123      151 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-utils/src/aliases.rs
+-rw-r--r--   0     1001      123     2862 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-utils/src/arena.rs
+-rw-r--r--   0     1001      123     1373 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-utils/src/atomic.rs
+-rw-r--r--   0     1001      123     2659 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-utils/src/cell.rs
+-rw-r--r--   0     1001      123     1015 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-utils/src/contention_pool.rs
+-rw-r--r--   0     1001      123      509 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-utils/src/error.rs
+-rw-r--r--   0     1001      123      271 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-utils/src/fmt.rs
+-rw-r--r--   0     1001      123      763 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-utils/src/functions.rs
+-rw-r--r--   0     1001      123     2709 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-utils/src/iter/enumerate_idx.rs
+-rw-r--r--   0     1001      123       61 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-utils/src/iter/mod.rs
+-rw-r--r--   0     1001      123      503 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-utils/src/lib.rs
+-rw-r--r--   0     1001      123      573 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-utils/src/macros.rs
+-rw-r--r--   0     1001      123      282 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-utils/src/mem.rs
+-rw-r--r--   0     1001      123     2336 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-utils/src/slice.rs
+-rw-r--r--   0     1001      123     2467 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-utils/src/sort.rs
+-rw-r--r--   0     1001      123     1115 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-utils/src/sync.rs
+-rw-r--r--   0     1001      123      504 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-utils/src/sys.rs
+-rw-r--r--   0     1001      123      697 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-utils/src/unwrap.rs
+-rw-r--r--   0     1001      123      498 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-utils/src/vec.rs
+-rw-r--r--   0     1001      123      616 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-utils/src/wasm.rs
+-rw-r--r--   0        0        0     4397 1970-01-01 00:00:00.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-io/Cargo.toml
+-rw-r--r--   0     1001      123     1055 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-io/LICENSE
+-rw-r--r--   0     1001      123      138 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-io/README.md
+-rw-r--r--   0     1001      123     2383 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-io/src/avro/mod.rs
+-rw-r--r--   0     1001      123     3608 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-io/src/avro/read.rs
+-rw-r--r--   0     1001      123     2622 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-io/src/avro/write.rs
+-rw-r--r--   0     1001      123     4505 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-io/src/cloud/adaptors.rs
+-rw-r--r--   0     1001      123     9506 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-io/src/cloud/glob.rs
+-rw-r--r--   0     1001      123     3089 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-io/src/cloud/mod.rs
+-rw-r--r--   0     1001      123    28133 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-io/src/csv/buffer.rs
+-rw-r--r--   0     1001      123     1815 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-io/src/csv/mod.rs
+-rw-r--r--   0     1001      123    19446 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-io/src/csv/parser.rs
+-rw-r--r--   0     1001      123    22226 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-io/src/csv/read.rs
+-rw-r--r--   0     1001      123    10846 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-io/src/csv/read_impl/batched_mmap.rs
+-rw-r--r--   0     1001      123    13938 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-io/src/csv/read_impl/batched_read.rs
+-rw-r--r--   0     1001      123    30724 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-io/src/csv/read_impl/mod.rs
+-rw-r--r--   0     1001      123    11466 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-io/src/csv/splitfields.rs
+-rw-r--r--   0     1001      123    24531 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-io/src/csv/utils.rs
+-rw-r--r--   0     1001      123     2796 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-io/src/csv/write.rs
+-rw-r--r--   0     1001      123    14759 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-io/src/csv/write_impl.rs
+-rw-r--r--   0     1001      123      184 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-io/src/export.rs
+-rw-r--r--   0     1001      123     7586 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-io/src/ipc/ipc_file.rs
+-rw-r--r--   0     1001      123     9227 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-io/src/ipc/ipc_stream.rs
+-rw-r--r--   0     1001      123     3253 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-io/src/ipc/mmap.rs
+-rw-r--r--   0     1001      123      401 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-io/src/ipc/mod.rs
+-rw-r--r--   0     1001      123     8287 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-io/src/ipc/write.rs
+-rw-r--r--   0     1001      123     1471 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-io/src/ipc/write_async.rs
+-rw-r--r--   0     1001      123    11044 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-io/src/json/mod.rs
+-rw-r--r--   0     1001      123     4771 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-io/src/lib.rs
+-rw-r--r--   0     1001      123     1969 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-io/src/mmap.rs
+-rw-r--r--   0     1001      123     7155 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-io/src/ndjson/buffer.rs
+-rw-r--r--   0     1001      123    11979 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-io/src/ndjson/core.rs
+-rw-r--r--   0     1001      123       37 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-io/src/ndjson/mod.rs
+-rw-r--r--   0     1001      123      273 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-io/src/options.rs
+-rw-r--r--   0     1001      123     7360 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-io/src/parquet/async_impl.rs
+-rw-r--r--   0     1001      123     3093 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-io/src/parquet/mmap.rs
+-rw-r--r--   0     1001      123     3132 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-io/src/parquet/mod.rs
+-rw-r--r--   0     1001      123     4784 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-io/src/parquet/predicates.rs
+-rw-r--r--   0     1001      123     9623 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-io/src/parquet/read.rs
+-rw-r--r--   0     1001      123    17320 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-io/src/parquet/read_impl.rs
+-rw-r--r--   0     1001      123    10052 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-io/src/parquet/write.rs
+-rw-r--r--   0     1001      123     5334 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-io/src/partition.rs
+-rw-r--r--   0     1001      123     1455 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-io/src/predicates.rs
+-rw-r--r--   0     1001      123      621 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-io/src/prelude.rs
+-rw-r--r--   0     1001      123      417 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-io/src/tests.rs
+-rw-r--r--   0     1001      123     4374 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-io/src/utils.rs
+-rw-r--r--   0        0        0     1592 1970-01-01 00:00:00.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-arrow/Cargo.toml
+-rw-r--r--   0     1001      123     1055 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-arrow/LICENSE
+-rw-r--r--   0     1001      123      144 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-arrow/README.md
+-rw-r--r--   0     1001      123     1975 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-arrow/src/array/default_arrays.rs
+-rw-r--r--   0     1001      123     1791 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-arrow/src/array/fixed_size_list.rs
+-rw-r--r--   0     1001      123     3773 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-arrow/src/array/get.rs
+-rw-r--r--   0     1001      123     6664 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-arrow/src/array/list.rs
+-rw-r--r--   0     1001      123     8165 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-arrow/src/array/mod.rs
+-rw-r--r--   0     1001      123      878 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-arrow/src/array/null.rs
+-rw-r--r--   0     1001      123     1125 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-arrow/src/array/slice.rs
+-rw-r--r--   0     1001      123     2252 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-arrow/src/array/utf8.rs
+-rw-r--r--   0     1001      123     2294 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-arrow/src/bit_util.rs
+-rw-r--r--   0     1001      123       17 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-arrow/src/bitmap/mod.rs
+-rw-r--r--   0     1001      123      819 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-arrow/src/bitmap/mutable.rs
+-rw-r--r--   0     1001      123      370 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-arrow/src/compute/arithmetics/decimal/add.rs
+-rw-r--r--   0     1001      123     2181 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-arrow/src/compute/arithmetics/decimal/commutative.rs
+-rw-r--r--   0     1001      123     1482 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-arrow/src/compute/arithmetics/decimal/div.rs
+-rw-r--r--   0     1001      123     1028 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-arrow/src/compute/arithmetics/decimal/mod.rs
+-rw-r--r--   0     1001      123     1177 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-arrow/src/compute/arithmetics/decimal/mul.rs
+-rw-r--r--   0     1001      123      508 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-arrow/src/compute/arithmetics/decimal/sub.rs
+-rw-r--r--   0     1001      123       51 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-arrow/src/compute/arithmetics/mod.rs
+-rw-r--r--   0     1001      123        1 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-arrow/src/compute/arity.rs
+-rw-r--r--   0     1001      123      727 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-arrow/src/compute/bitwise.rs
+-rw-r--r--   0     1001      123     1206 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-arrow/src/compute/cast.rs
+-rw-r--r--   0     1001      123     3964 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-arrow/src/compute/decimal.rs
+-rw-r--r--   0     1001      123     1250 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-arrow/src/compute/mod.rs
+-rw-r--r--   0     1001      123      391 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-arrow/src/compute/take/bitmap.rs
+-rw-r--r--   0     1001      123     2767 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-arrow/src/compute/take/boolean.rs
+-rw-r--r--   0     1001      123     3487 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-arrow/src/compute/take/fixed_size_list.rs
+-rw-r--r--   0     1001      123    25289 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-arrow/src/compute/take/mod.rs
+-rw-r--r--   0     1001      123      797 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-arrow/src/compute/tile.rs
+-rw-r--r--   0     1001      123     1102 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-arrow/src/conversion.rs
+-rw-r--r--   0     1001      123     1609 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-arrow/src/data_types.rs
+-rw-r--r--   0     1001      123       25 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-arrow/src/error.rs
+-rw-r--r--   0     1001      123       28 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-arrow/src/export.rs
+-rw-r--r--   0     1001      123       26 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-arrow/src/floats/mod.rs
+-rw-r--r--   0     1001      123     2066 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-arrow/src/floats/ord.rs
+-rw-r--r--   0     1001      123     1273 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-arrow/src/index.rs
+-rw-r--r--   0     1001      123      984 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-arrow/src/is_valid.rs
+-rw-r--r--   0     1001      123     4783 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-arrow/src/kernels/agg_mean.rs
+-rw-r--r--   0     1001      123     1074 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-arrow/src/kernels/comparison.rs
+-rw-r--r--   0     1001      123     1068 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-arrow/src/kernels/concatenate.rs
+-rw-r--r--   0     1001      123     5161 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-arrow/src/kernels/ewm/average.rs
+-rw-r--r--   0     1001      123     1808 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-arrow/src/kernels/ewm/mod.rs
+-rw-r--r--   0     1001      123    25065 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-arrow/src/kernels/ewm/variance.rs
+-rw-r--r--   0     1001      123     1406 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-arrow/src/kernels/float.rs
+-rw-r--r--   0     1001      123     4907 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-arrow/src/kernels/list.rs
+-rw-r--r--   0     1001      123     1885 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-arrow/src/kernels/list_bytes_iter.rs
+-rw-r--r--   0     1001      123     9783 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-arrow/src/kernels/mod.rs
+-rw-r--r--   0     1001      123     3923 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-arrow/src/kernels/rolling/mod.rs
+-rw-r--r--   0     1001      123     2019 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/mean.rs
+-rw-r--r--   0     1001      123    16191 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/min_max.rs
+-rw-r--r--   0     1001      123     3839 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/mod.rs
+-rw-r--r--   0     1001      123    11729 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/quantile.rs
+-rw-r--r--   0     1001      123     5684 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/sum.rs
+-rw-r--r--   0     1001      123     9609 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/variance.rs
+-rw-r--r--   0     1001      123     1879 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-arrow/src/kernels/rolling/nulls/mean.rs
+-rw-r--r--   0     1001      123    14722 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-arrow/src/kernels/rolling/nulls/min_max.rs
+-rw-r--r--   0     1001      123    10055 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-arrow/src/kernels/rolling/nulls/mod.rs
+-rw-r--r--   0     1001      123    11643 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-arrow/src/kernels/rolling/nulls/quantile.rs
+-rw-r--r--   0     1001      123     4821 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-arrow/src/kernels/rolling/nulls/sum.rs
+-rw-r--r--   0     1001      123     8687 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-arrow/src/kernels/rolling/nulls/variance.rs
+-rw-r--r--   0     1001      123     8109 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-arrow/src/kernels/rolling/window.rs
+-rw-r--r--   0     1001      123     4752 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-arrow/src/kernels/set.rs
+-rw-r--r--   0     1001      123     4529 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-arrow/src/kernels/sort_partition.rs
+-rw-r--r--   0     1001      123     2948 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-arrow/src/kernels/sorted_join/inner.rs
+-rw-r--r--   0     1001      123     5974 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-arrow/src/kernels/sorted_join/left.rs
+-rw-r--r--   0     1001      123      231 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-arrow/src/kernels/sorted_join/mod.rs
+-rw-r--r--   0     1001      123      841 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-arrow/src/kernels/string.rs
+-rw-r--r--   0     1001      123     2310 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-arrow/src/kernels/take_agg/boolean.rs
+-rw-r--r--   0     1001      123     4315 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-arrow/src/kernels/take_agg/mod.rs
+-rw-r--r--   0     1001      123     2606 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-arrow/src/kernels/take_agg/var.rs
+-rw-r--r--   0     1001      123     3672 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-arrow/src/kernels/time.rs
+-rw-r--r--   0     1001      123      341 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-arrow/src/lib.rs
+-rw-r--r--   0     1001      123      496 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-arrow/src/prelude.rs
+-rw-r--r--   0     1001      123      534 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-arrow/src/slice.rs
+-rw-r--r--   0     1001      123      183 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-arrow/src/time_zone.rs
+-rw-r--r--   0     1001      123      998 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-arrow/src/trusted_len/boolean.rs
+-rw-r--r--   0     1001      123     2821 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-arrow/src/trusted_len/mod.rs
+-rw-r--r--   0     1001      123     2052 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-arrow/src/trusted_len/push_unchecked.rs
+-rw-r--r--   0     1001      123      158 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-arrow/src/trusted_len/rev.rs
+-rw-r--r--   0     1001      123     5232 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-arrow/src/utils.rs
+-rw-r--r--   0        0        0     1998 1970-01-01 00:00:00.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-pipe/Cargo.toml
+-rw-r--r--   0     1001      123     1055 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-pipe/LICENSE
+-rw-r--r--   0     1001      123      165 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-pipe/README.md
+-rw-r--r--   0     1001      123       98 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-pipe/src/executors/mod.rs
+-rw-r--r--   0     1001      123     1219 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-pipe/src/executors/operators/filter.rs
+-rw-r--r--   0     1001      123     4103 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-pipe/src/executors/operators/function.rs
+-rw-r--r--   0     1001      123      266 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-pipe/src/executors/operators/mod.rs
+-rw-r--r--   0     1001      123      682 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-pipe/src/executors/operators/pass.rs
+-rw-r--r--   0     1001      123      548 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-pipe/src/executors/operators/placeholder.rs
+-rw-r--r--   0     1001      123     3553 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-pipe/src/executors/operators/projection.rs
+-rw-r--r--   0     1001      123     3559 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-pipe/src/executors/operators/reproject.rs
+-rw-r--r--   0     1001      123     6479 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-pipe/src/executors/sinks/file_sink.rs
+-rw-r--r--   0     1001      123    11288 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/convert.rs
+-rw-r--r--   0     1001      123     1207 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/count.rs
+-rw-r--r--   0     1001      123     1888 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/first.rs
+-rw-r--r--   0     1001      123     4554 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/interface.rs
+-rw-r--r--   0     1001      123     1746 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/last.rs
+-rw-r--r--   0     1001      123     5413 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/mean.rs
+-rw-r--r--   0     1001      123     4951 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/min_max.rs
+-rw-r--r--   0     1001      123      211 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/mod.rs
+-rw-r--r--   0     1001      123      856 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/null.rs
+-rw-r--r--   0     1001      123     4294 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/sum.rs
+-rw-r--r--   0     1001      123     4102 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/eval.rs
+-rw-r--r--   0     1001      123     7404 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/global.rs
+-rw-r--r--   0     1001      123    10553 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/hash_table.rs
+-rw-r--r--   0     1001      123     3589 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/mod.rs
+-rw-r--r--   0     1001      123     2767 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/ooc_state.rs
+-rw-r--r--   0     1001      123     6326 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/sink.rs
+-rw-r--r--   0     1001      123     3116 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/source.rs
+-rw-r--r--   0     1001      123    10194 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/thread_local.rs
+-rw-r--r--   0     1001      123     2119 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-pipe/src/executors/sinks/groupby/mod.rs
+-rw-r--r--   0     1001      123     4695 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-pipe/src/executors/sinks/groupby/ooc.rs
+-rw-r--r--   0     1001      123     1887 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-pipe/src/executors/sinks/groupby/ooc_state.rs
+-rw-r--r--   0     1001      123    20783 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-pipe/src/executors/sinks/groupby/primitive/mod.rs
+-rw-r--r--   0     1001      123    23825 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-pipe/src/executors/sinks/groupby/string.rs
+-rw-r--r--   0     1001      123     2457 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-pipe/src/executors/sinks/groupby/utils.rs
+-rw-r--r--   0     1001      123     9239 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-pipe/src/executors/sinks/io.rs
+-rw-r--r--   0     1001      123     5451 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-pipe/src/executors/sinks/joins/cross.rs
+-rw-r--r--   0     1001      123    11949 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-pipe/src/executors/sinks/joins/generic_build.rs
+-rw-r--r--   0     1001      123    11756 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-pipe/src/executors/sinks/joins/inner_left.rs
+-rw-r--r--   0     1001      123      178 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-pipe/src/executors/sinks/joins/mod.rs
+-rw-r--r--   0     1001      123     2241 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-pipe/src/executors/sinks/memory.rs
+-rw-r--r--   0     1001      123      589 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-pipe/src/executors/sinks/mod.rs
+-rw-r--r--   0     1001      123     1492 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-pipe/src/executors/sinks/ordered.rs
+-rw-r--r--   0     1001      123     1824 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-pipe/src/executors/sinks/reproject.rs
+-rw-r--r--   0     1001      123     3108 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-pipe/src/executors/sinks/slice.rs
+-rw-r--r--   0     1001      123      130 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-pipe/src/executors/sinks/sort/mod.rs
+-rw-r--r--   0     1001      123     6787 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-pipe/src/executors/sinks/sort/ooc.rs
+-rw-r--r--   0     1001      123     7279 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-pipe/src/executors/sinks/sort/sink.rs
+-rw-r--r--   0     1001      123     5953 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-pipe/src/executors/sinks/sort/sink_multiple.rs
+-rw-r--r--   0     1001      123     3908 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-pipe/src/executors/sinks/sort/source.rs
+-rw-r--r--   0     1001      123      526 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-pipe/src/executors/sinks/utils.rs
+-rw-r--r--   0     1001      123     5984 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-pipe/src/executors/sources/csv.rs
+-rw-r--r--   0     1001      123     1231 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-pipe/src/executors/sources/frame.rs
+-rw-r--r--   0     1001      123      987 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-pipe/src/executors/sources/ipc_one_shot.rs
+-rw-r--r--   0     1001      123      366 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-pipe/src/executors/sources/mod.rs
+-rw-r--r--   0     1001      123     4335 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-pipe/src/executors/sources/parquet.rs
+-rw-r--r--   0     1001      123     1146 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-pipe/src/executors/sources/reproject.rs
+-rw-r--r--   0     1001      123     1022 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-pipe/src/executors/sources/union.rs
+-rw-r--r--   0     1001      123      448 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-pipe/src/expressions.rs
+-rw-r--r--   0     1001      123      272 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-pipe/src/lib.rs
+-rw-r--r--   0     1001      123      719 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-pipe/src/operators/chunks.rs
+-rw-r--r--   0     1001      123      474 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-pipe/src/operators/context.rs
+-rw-r--r--   0     1001      123      223 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-pipe/src/operators/mod.rs
+-rw-r--r--   0     1001      123      514 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-pipe/src/operators/operator.rs
+-rw-r--r--   0     1001      123      626 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-pipe/src/operators/sink.rs
+-rw-r--r--   0     1001      123      241 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-pipe/src/operators/source.rs
+-rw-r--r--   0     1001      123        1 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-pipe/src/pipeline/config.rs
+-rw-r--r--   0     1001      123    21321 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-pipe/src/pipeline/convert.rs
+-rw-r--r--   0     1001      123    18204 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-pipe/src/pipeline/dispatcher.rs
+-rw-r--r--   0     1001      123     1155 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-pipe/src/pipeline/mod.rs
+-rw-r--r--   0        0        0     1106 1970-01-01 00:00:00.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-sql/Cargo.toml
+-rw-r--r--   0     1001      123     1055 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-sql/LICENSE
+-rw-r--r--   0     1001      123      466 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-sql/README.md
+-rw-r--r--   0     1001      123    23236 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-sql/src/context.rs
+-rw-r--r--   0     1001      123    20711 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-sql/src/functions.rs
+-rw-r--r--   0     1001      123     2122 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-sql/src/keywords.rs
+-rw-r--r--   0     1001      123      239 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-sql/src/lib.rs
+-rw-r--r--   0     1001      123    20991 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-sql/src/sql_expr.rs
+-rw-r--r--   0     1001      123     4572 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-sql/src/table_functions.rs
+-rw-r--r--   0     1001      123     1682 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-sql/tests/functions_cumulative.rs
+-rw-r--r--   0     1001      123     3063 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-sql/tests/functions_io.rs
+-rw-r--r--   0     1001      123     1539 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-sql/tests/functions_math.rs
+-rw-r--r--   0     1001      123      860 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-sql/tests/functions_meta.rs
+-rw-r--r--   0     1001      123     2982 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-sql/tests/functions_string.rs
+-rw-r--r--   0     1001      123     1056 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-sql/tests/iss_7436.rs
+-rw-r--r--   0     1001      123      888 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-sql/tests/iss_7437.rs
+-rw-r--r--   0     1001      123      652 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-sql/tests/iss_7440.rs
+-rw-r--r--   0     1001      123      700 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-sql/tests/iss_8395.rs
+-rw-r--r--   0     1001      123     1062 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-sql/tests/iss_8419.rs
+-rw-r--r--   0     1001      123      982 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-sql/tests/ops_distinct_on.rs
+-rw-r--r--   0     1001      123    15418 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-sql/tests/simple_exprs.rs
+-rw-r--r--   0     1001      123     3343 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-sql/tests/statements.rs
+-rw-r--r--   0        0        0    10560 1970-01-01 00:00:00.000000 polars_lts_cpu-0.18.3/local_dependencies/polars/Cargo.toml
+-rw-r--r--   0     1001      123     1055 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars/LICENSE
+-rw-r--r--   0     1001      123     3472 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars/Makefile
+-rw-r--r--   0     1001      123      215 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars/build.rs
+-rw-r--r--   0     1001      123       78 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars/clippy.toml
+-rw-r--r--   0     1001      123    17602 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars/src/docs/eager.rs
+-rw-r--r--   0     1001      123     8794 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars/src/docs/lazy.rs
+-rw-r--r--   0     1001      123       50 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars/src/docs/mod.rs
+-rw-r--r--   0     1001      123     3797 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars/src/docs/performance.rs
+-rw-r--r--   0     1001      123       59 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars/src/export.rs
+-rw-r--r--   0     1001      123    20214 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars/src/lib.rs
+-rw-r--r--   0     1001      123      387 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars/src/prelude.rs
+-rw-r--r--   0     1001      123       54 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars/src/sql.rs
+-rw-r--r--   0     1001      123     4272 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars/tests/it/core/date_like.rs
+-rw-r--r--   0     1001      123     2401 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars/tests/it/core/groupby.rs
+-rw-r--r--   0     1001      123    17836 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars/tests/it/core/joins.rs
+-rw-r--r--   0     1001      123      545 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars/tests/it/core/list.rs
+-rw-r--r--   0     1001      123      198 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars/tests/it/core/mod.rs
+-rw-r--r--   0     1001      123       24 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars/tests/it/core/ops/mod.rs
+-rw-r--r--   0     1001      123      457 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars/tests/it/core/ops/take.rs
+-rw-r--r--   0     1001      123     6259 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars/tests/it/core/pivot.rs
+-rw-r--r--   0     1001      123     1102 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars/tests/it/core/random.rs
+-rw-r--r--   0     1001      123    11096 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars/tests/it/core/rolling_window.rs
+-rw-r--r--   0     1001      123     1093 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars/tests/it/core/series.rs
+-rw-r--r--   0     1001      123      370 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars/tests/it/core/utils.rs
+-rw-r--r--   0     1001      123    30423 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars/tests/it/io/csv.rs
+-rw-r--r--   0     1001      123     4490 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars/tests/it/io/ipc_stream.rs
+-rw-r--r--   0     1001      123     7043 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars/tests/it/io/json.rs
+-rw-r--r--   0     1001      123      378 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars/tests/it/io/mod.rs
+-rw-r--r--   0     1001      123      531 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars/tests/it/io/parquet.rs
+-rw-r--r--   0     1001      123     1530 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars/tests/it/joins.rs
+-rw-r--r--   0     1001      123     2452 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars/tests/it/lazy/aggregation.rs
+-rw-r--r--   0     1001      123      821 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars/tests/it/lazy/cse.rs
+-rw-r--r--   0     1001      123      500 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars/tests/it/lazy/explodes.rs
+-rw-r--r--   0     1001      123     2279 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars/tests/it/lazy/expressions/apply.rs
+-rw-r--r--   0     1001      123    10285 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars/tests/it/lazy/expressions/arity.rs
+-rw-r--r--   0     1001      123     1065 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars/tests/it/lazy/expressions/expand.rs
+-rw-r--r--   0     1001      123     1008 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars/tests/it/lazy/expressions/filter.rs
+-rw-r--r--   0     1001      123      428 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars/tests/it/lazy/expressions/is_in.rs
+-rw-r--r--   0     1001      123      121 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars/tests/it/lazy/expressions/mod.rs
+-rw-r--r--   0     1001      123      659 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars/tests/it/lazy/expressions/slice.rs
+-rw-r--r--   0     1001      123    10657 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars/tests/it/lazy/expressions/window.rs
+-rw-r--r--   0     1001      123      579 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars/tests/it/lazy/folds.rs
+-rw-r--r--   0     1001      123      557 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars/tests/it/lazy/functions.rs
+-rw-r--r--   0     1001      123     4482 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars/tests/it/lazy/groupby.rs
+-rw-r--r--   0     1001      123     1681 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars/tests/it/lazy/groupby_dynamic.rs
+-rw-r--r--   0     1001      123      691 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars/tests/it/lazy/mod.rs
+-rw-r--r--   0     1001      123     5747 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars/tests/it/lazy/predicate_queries.rs
+-rw-r--r--   0     1001      123     4483 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars/tests/it/lazy/projection_queries.rs
+-rw-r--r--   0     1001      123     6584 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars/tests/it/lazy/queries.rs
+-rw-r--r--   0     1001      123      141 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars/tests/it/main.rs
+-rw-r--r--   0     1001      123    12591 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars/tests/it/schema.rs
+-rw-r--r--   0        0        0      827 1970-01-01 00:00:00.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-algo/Cargo.toml
+-rw-r--r--   0     1001      123     1055 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-algo/LICENSE
+-rw-r--r--   0     1001      123      142 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-algo/README.md
+-rw-r--r--   0     1001      123     7548 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-algo/src/algo.rs
+-rw-r--r--   0     1001      123       88 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-algo/src/lib.rs
+-rw-r--r--   0     1001      123       28 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-algo/src/prelude.rs
+-rw-r--r--   0        0        0     5484 1970-01-01 00:00:00.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/Cargo.toml
+-rw-r--r--   0     1001      123     1055 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/LICENSE
+-rw-r--r--   0     1001      123      144 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/README.md
+-rw-r--r--   0     1001      123     5158 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/arithmetic/decimal.rs
+-rw-r--r--   0     1001      123     8275 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/arithmetic/mod.rs
+-rw-r--r--   0     1001      123     9417 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/arithmetic/numeric.rs
+-rw-r--r--   0     1001      123     3588 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/array/iterator.rs
+-rw-r--r--   0     1001      123     2551 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/array/mod.rs
+-rw-r--r--   0     1001      123     6448 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/bitwise.rs
+-rw-r--r--   0     1001      123     2298 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/builder/binary.rs
+-rw-r--r--   0     1001      123     1207 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/builder/boolean.rs
+-rw-r--r--   0     1001      123     4311 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/builder/fixed_size_list.rs
+-rw-r--r--   0     1001      123     1556 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/builder/from.rs
+-rw-r--r--   0     1001      123    20366 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/builder/list.rs
+-rw-r--r--   0     1001      123     8969 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/builder/mod.rs
+-rw-r--r--   0     1001      123     1410 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/builder/primitive.rs
+-rw-r--r--   0     1001      123     2291 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/builder/utf8.rs
+-rw-r--r--   0     1001      123    16475 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/cast.rs
+-rw-r--r--   0     1001      123    49461 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/comparison/mod.rs
+-rw-r--r--   0     1001      123    10060 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/comparison/scalar.rs
+-rw-r--r--   0     1001      123      551 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/drop.rs
+-rw-r--r--   0     1001      123      963 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/float.rs
+-rw-r--r--   0     1001      123     7175 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/from.rs
+-rw-r--r--   0     1001      123    42339 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/iterator/mod.rs
+-rw-r--r--   0     1001      123     1453 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/iterator/par/list.rs
+-rw-r--r--   0     1001      123       28 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/iterator/par/mod.rs
+-rw-r--r--   0     1001      123     1129 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/iterator/par/utf8.rs
+-rw-r--r--   0     1001      123       21 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/kernels/mod.rs
+-rw-r--r--   0     1001      123     2347 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/kernels/take.rs
+-rw-r--r--   0     1001      123     7963 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/list/iterator.rs
+-rw-r--r--   0     1001      123     3242 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/list/mod.rs
+-rw-r--r--   0     1001      123    19830 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/logical/categorical/builder.rs
+-rw-r--r--   0     1001      123     3688 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/logical/categorical/from.rs
+-rw-r--r--   0     1001      123     4270 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/logical/categorical/merge.rs
+-rw-r--r--   0     1001      123    10219 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/logical/categorical/mod.rs
+-rw-r--r--   0     1001      123     1400 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/append.rs
+-rw-r--r--   0     1001      123      358 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/full.rs
+-rw-r--r--   0     1001      123      192 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/mod.rs
+-rw-r--r--   0     1001      123     2731 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/take_random.rs
+-rw-r--r--   0     1001      123     2172 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/unique.rs
+-rw-r--r--   0     1001      123      925 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/zip.rs
+-rw-r--r--   0     1001      123     6417 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/logical/categorical/stringcache.rs
+-rw-r--r--   0     1001      123     1604 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/logical/date.rs
+-rw-r--r--   0     1001      123     4105 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/logical/datetime.rs
+-rw-r--r--   0     1001      123     4443 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/logical/decimal.rs
+-rw-r--r--   0     1001      123     2434 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/logical/duration.rs
+-rw-r--r--   0     1001      123     2556 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/logical/mod.rs
+-rw-r--r--   0     1001      123      476 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/logical/struct_/from.rs
+-rw-r--r--   0     1001      123    15982 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/logical/struct_/mod.rs
+-rw-r--r--   0     1001      123     1182 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/logical/time.rs
+-rw-r--r--   0     1001      123    23489 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/mod.rs
+-rw-r--r--   0     1001      123     7200 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/ndarray.rs
+-rw-r--r--   0     1001      123     4484 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/object/builder.rs
+-rw-r--r--   0     1001      123     1547 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/object/extension/drop.rs
+-rw-r--r--   0     1001      123     3124 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/object/extension/list.rs
+-rw-r--r--   0     1001      123     7054 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/object/extension/mod.rs
+-rw-r--r--   0     1001      123     3410 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/object/extension/polars_extension.rs
+-rw-r--r--   0     1001      123      137 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/object/is_valid.rs
+-rw-r--r--   0     1001      123     4419 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/object/iterator.rs
+-rw-r--r--   0     1001      123     4806 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/object/mod.rs
+-rw-r--r--   0     1001      123     2956 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/object/registry.rs
+-rw-r--r--   0     1001      123      272 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/ops/abs.rs
+-rw-r--r--   0     1001      123    32691 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/ops/aggregate/mod.rs
+-rw-r--r--   0     1001      123    10025 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/ops/aggregate/quantile.rs
+-rw-r--r--   0     1001      123     2880 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/ops/aggregate/var.rs
+-rw-r--r--   0     1001      123    10551 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/ops/any_value.rs
+-rw-r--r--   0     1001      123     2820 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/ops/append.rs
+-rw-r--r--   0     1001      123    28256 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/ops/apply.rs
+-rw-r--r--   0     1001      123    12799 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/ops/bit_repr.rs
+-rw-r--r--   0     1001      123     6236 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/ops/chunkops.rs
+-rw-r--r--   0     1001      123    11537 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/ops/compare_inner.rs
+-rw-r--r--   0     1001      123     1737 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/ops/concat_str.rs
+-rw-r--r--   0     1001      123     4801 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/ops/cum_agg.rs
+-rw-r--r--   0     1001      123      908 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/ops/decimal.rs
+-rw-r--r--   0     1001      123     7056 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/ops/downcast.rs
+-rw-r--r--   0     1001      123    19461 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/ops/explode.rs
+-rw-r--r--   0     1001      123     8691 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/ops/explode_and_offsets.rs
+-rw-r--r--   0     1001      123     8866 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/ops/extend.rs
+-rw-r--r--   0     1001      123    13777 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/ops/fill_null.rs
+-rw-r--r--   0     1001      123     6356 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/ops/filter.rs
+-rw-r--r--   0     1001      123     5876 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/ops/full.rs
+-rw-r--r--   0     1001      123        1 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/ops/interpolate.rs
+-rw-r--r--   0     1001      123    16797 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/ops/is_in.rs
+-rw-r--r--   0     1001      123        1 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/ops/len.rs
+-rw-r--r--   0     1001      123     2658 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/ops/min_max_binary.rs
+-rw-r--r--   0     1001      123    23276 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/ops/mod.rs
+-rw-r--r--   0     1001      123     2414 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/ops/nulls.rs
+-rw-r--r--   0     1001      123      593 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/ops/peaks.rs
+-rw-r--r--   0     1001      123     4375 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/ops/repeat_by.rs
+-rw-r--r--   0     1001      123     2771 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/ops/reverse.rs
+-rw-r--r--   0     1001      123    10266 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/ops/rolling_window.rs
+-rw-r--r--   0     1001      123    12518 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/ops/set.rs
+-rw-r--r--   0     1001      123     7391 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/ops/shift.rs
+-rw-r--r--   0     1001      123     2299 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/ops/sort/arg_sort.rs
+-rw-r--r--   0     1001      123     5528 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/ops/sort/arg_sort_multiple.rs
+-rw-r--r--   0     1001      123     7543 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/ops/sort/categorical.rs
+-rw-r--r--   0     1001      123    31164 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/ops/sort/mod.rs
+-rw-r--r--   0     1001      123      380 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/ops/sort/slice.rs
+-rw-r--r--   0     1001      123    22089 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/ops/take/mod.rs
+-rw-r--r--   0     1001      123     7848 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/ops/take/take_chunked.rs
+-rw-r--r--   0     1001      123      301 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/ops/take/take_every.rs
+-rw-r--r--   0     1001      123    16256 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/ops/take/take_random.rs
+-rw-r--r--   0     1001      123     5810 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/ops/take/take_single.rs
+-rw-r--r--   0     1001      123     6072 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/ops/take/traits.rs
+-rw-r--r--   0     1001      123      459 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/ops/tile.rs
+-rw-r--r--   0     1001      123    11626 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/ops/unique/mod.rs
+-rw-r--r--   0     1001      123    14620 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/ops/unique/rank.rs
+-rw-r--r--   0     1001      123     5846 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/ops/zip.rs
+-rw-r--r--   0     1001      123     9093 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/random.rs
+-rw-r--r--   0     1001      123     1875 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/temporal/conversion.rs
+-rw-r--r--   0     1001      123     2826 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/temporal/date.rs
+-rw-r--r--   0     1001      123    10497 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/temporal/datetime.rs
+-rw-r--r--   0     1001      123     3201 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/temporal/duration.rs
+-rw-r--r--   0     1001      123      595 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/temporal/mod.rs
+-rw-r--r--   0     1001      123     3042 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/temporal/time.rs
+-rw-r--r--   0     1001      123      872 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/to_vec.rs
+-rw-r--r--   0     1001      123     8113 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/trusted_len.rs
+-rw-r--r--   0     1001      123    25939 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/upstream_traits.rs
+-rw-r--r--   0     1001      123     7944 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/cloud.rs
+-rw-r--r--   0     1001      123     1549 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/config.rs
+-rw-r--r--   0     1001      123     3946 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/datatypes/_serde.rs
+-rw-r--r--   0     1001      123     2509 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/datatypes/aliases.rs
+-rw-r--r--   0     1001      123    42658 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/datatypes/any_value.rs
+-rw-r--r--   0     1001      123    13349 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/datatypes/dtype.rs
+-rw-r--r--   0     1001      123     5609 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/datatypes/field.rs
+-rw-r--r--   0     1001      123     8059 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/datatypes/mod.rs
+-rw-r--r--   0     1001      123     2016 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/datatypes/time_unit.rs
+-rw-r--r--   0     1001      123      118 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/doc/changelog/mod.rs
+-rw-r--r--   0     1001      123      898 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/doc/changelog/v0_10_0_11.rs
+-rw-r--r--   0     1001      123      481 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/doc/changelog/v0_3.rs
+-rw-r--r--   0     1001      123      293 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/doc/changelog/v0_4.rs
+-rw-r--r--   0     1001      123      499 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/doc/changelog/v0_5.rs
+-rw-r--r--   0     1001      123      288 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/doc/changelog/v0_6.rs
+-rw-r--r--   0     1001      123     1071 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/doc/changelog/v0_7.rs
+-rw-r--r--   0     1001      123      819 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/doc/changelog/v0_8.rs
+-rw-r--r--   0     1001      123      596 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/doc/changelog/v0_9.rs
+-rw-r--r--   0     1001      123       43 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/doc/mod.rs
+-rw-r--r--   0     1001      123       25 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/error.rs
+-rw-r--r--   0     1001      123      263 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/export.rs
+-rw-r--r--   0     1001      123    36432 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/fmt.rs
+-rw-r--r--   0     1001      123     5177 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/frame/arithmetic.rs
+-rw-r--r--   0     1001      123     9916 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/frame/asof_join/asof.rs
+-rw-r--r--   0     1001      123    35761 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/frame/asof_join/groups.rs
+-rw-r--r--   0     1001      123     7168 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/frame/asof_join/mod.rs
+-rw-r--r--   0     1001      123      559 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/frame/chunks.rs
+-rw-r--r--   0     1001      123     5181 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/frame/cross_join.rs
+-rw-r--r--   0     1001      123    16760 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/frame/explode.rs
+-rw-r--r--   0     1001      123     1019 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/frame/from.rs
+-rw-r--r--   0     1001      123    19219 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/frame/groupby/aggregations/agg_list.rs
+-rw-r--r--   0     1001      123     4113 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/frame/groupby/aggregations/boolean.rs
+-rw-r--r--   0     1001      123     7749 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/frame/groupby/aggregations/dispatch.rs
+-rw-r--r--   0     1001      123    40369 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/frame/groupby/aggregations/mod.rs
+-rw-r--r--   0     1001      123     5634 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/frame/groupby/aggregations/utf8.rs
+-rw-r--r--   0     1001      123      218 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/frame/groupby/expr.rs
+-rw-r--r--   0     1001      123    22901 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/frame/groupby/hashing.rs
+-rw-r--r--   0     1001      123    14380 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/frame/groupby/into_groups.rs
+-rw-r--r--   0     1001      123    39623 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/frame/groupby/mod.rs
+-rw-r--r--   0     1001      123    10637 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/frame/groupby/perfect.rs
+-rw-r--r--   0     1001      123    19780 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/frame/groupby/proxy.rs
+-rw-r--r--   0     1001      123     5406 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/frame/hash_join/args.rs
+-rw-r--r--   0     1001      123    13329 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/frame/hash_join/mod.rs
+-rw-r--r--   0     1001      123    22364 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/frame/hash_join/multiple_keys.rs
+-rw-r--r--   0     1001      123     2413 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/frame/hash_join/single_keys.rs
+-rw-r--r--   0     1001      123    17372 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/frame/hash_join/single_keys_dispatch.rs
+-rw-r--r--   0     1001      123     4608 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/frame/hash_join/single_keys_inner.rs
+-rw-r--r--   0     1001      123     6434 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/frame/hash_join/single_keys_left.rs
+-rw-r--r--   0     1001      123     4564 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/frame/hash_join/single_keys_outer.rs
+-rw-r--r--   0     1001      123     3913 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/frame/hash_join/single_keys_semi_anti.rs
+-rw-r--r--   0     1001      123    12313 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/frame/hash_join/sort_merge.rs
+-rw-r--r--   0     1001      123     3865 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/frame/hash_join/zip_outer.rs
+-rw-r--r--   0     1001      123   126103 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/frame/mod.rs
+-rw-r--r--   0     1001      123    27652 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/frame/row/av_buffer.rs
+-rw-r--r--   0     1001      123     5183 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/frame/row/dataframe.rs
+-rw-r--r--   0     1001      123     5976 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/frame/row/mod.rs
+-rw-r--r--   0     1001      123     9875 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/frame/row/transpose.rs
+-rw-r--r--   0     1001      123     2811 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/frame/top_k.rs
+-rw-r--r--   0     1001      123     1388 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/frame/upstream_traits.rs
+-rw-r--r--   0     1001      123    10198 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/functions.rs
+-rw-r--r--   0     1001      123     2149 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/hashing/fx.rs
+-rw-r--r--   0     1001      123     1503 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/hashing/identity.rs
+-rw-r--r--   0     1001      123      457 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/hashing/mod.rs
+-rw-r--r--   0     1001      123     2684 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/hashing/partition.rs
+-rw-r--r--   0     1001      123    17704 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/hashing/vector_hasher.rs
+-rw-r--r--   0     1001      123     1896 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/lib.rs
+-rw-r--r--   0     1001      123    15733 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/named_from.rs
+-rw-r--r--   0     1001      123     2423 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/prelude.rs
+-rw-r--r--   0     1001      123    17667 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/schema.rs
+-rw-r--r--   0     1001      123     4218 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/serde/chunked_array.rs
+-rw-r--r--   0     1001      123     1094 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/serde/df.rs
+-rw-r--r--   0     1001      123     6559 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/serde/mod.rs
+-rw-r--r--   0     1001      123     9510 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/serde/series.rs
+-rw-r--r--   0     1001      123    18543 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/series/any_value.rs
+-rw-r--r--   0     1001      123    28755 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/series/arithmetic/borrowed.rs
+-rw-r--r--   0     1001      123      222 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/series/arithmetic/mod.rs
+-rw-r--r--   0     1001      123     3546 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/series/arithmetic/owned.rs
+-rw-r--r--   0     1001      123    19293 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/series/comparison.rs
+-rw-r--r--   0     1001      123    29575 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/series/from.rs
+-rw-r--r--   0     1001      123     6080 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/series/implementations/array.rs
+-rw-r--r--   0     1001      123     9089 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/series/implementations/binary.rs
+-rw-r--r--   0     1001      123    10835 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/series/implementations/boolean.rs
+-rw-r--r--   0     1001      123    12800 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/series/implementations/categorical.rs
+-rw-r--r--   0     1001      123    18214 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/series/implementations/dates_time.rs
+-rw-r--r--   0     1001      123    15034 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/series/implementations/datetime.rs
+-rw-r--r--   0     1001      123     7981 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/series/implementations/decimal.rs
+-rw-r--r--   0     1001      123    14734 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/series/implementations/duration.rs
+-rw-r--r--   0     1001      123    14063 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/series/implementations/floats.rs
+-rw-r--r--   0     1001      123     6078 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/series/implementations/list.rs
+-rw-r--r--   0     1001      123    18396 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/series/implementations/mod.rs
+-rw-r--r--   0     1001      123     5522 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/series/implementations/null.rs
+-rw-r--r--   0     1001      123     7939 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/series/implementations/object.rs
+-rw-r--r--   0     1001      123    11788 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/series/implementations/struct_.rs
+-rw-r--r--   0     1001      123     9607 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/series/implementations/utf8.rs
+-rw-r--r--   0     1001      123     4471 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/series/into.rs
+-rw-r--r--   0     1001      123     6241 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/series/iterator.rs
+-rw-r--r--   0     1001      123    39074 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/series/mod.rs
+-rw-r--r--   0     1001      123      853 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/series/ops/diff.rs
+-rw-r--r--   0     1001      123     5814 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/series/ops/downcast.rs
+-rw-r--r--   0     1001      123     3601 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/series/ops/ewm.rs
+-rw-r--r--   0     1001      123      413 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/series/ops/extend.rs
+-rw-r--r--   0     1001      123      562 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/series/ops/mod.rs
+-rw-r--r--   0     1001      123     5974 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/series/ops/moment.rs
+-rw-r--r--   0     1001      123     2908 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/series/ops/null.rs
+-rw-r--r--   0     1001      123     1347 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/series/ops/pct_change.rs
+-rw-r--r--   0     1001      123     4620 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/series/ops/round.rs
+-rw-r--r--   0     1001      123     5073 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/series/ops/to_list.rs
+-rw-r--r--   0     1001      123     1476 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/series/ops/unique.rs
+-rw-r--r--   0     1001      123    18408 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/series/series_trait.rs
+-rw-r--r--   0     1001      123     2912 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/series/unstable.rs
+-rw-r--r--   0     1001      123     7077 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/testing.rs
+-rw-r--r--   0     1001      123      508 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/tests.rs
+-rw-r--r--   0     1001      123     2492 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/utils/flatten.rs
+-rw-r--r--   0     1001      123    30596 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/utils/mod.rs
+-rw-r--r--   0     1001      123     1600 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/utils/series.rs
+-rw-r--r--   0     1001      123    13201 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/utils/supertype.rs
+-rw-r--r--   0        0        0     1353 1970-01-01 00:00:00.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-json/Cargo.toml
+-rw-r--r--   0     1001      123     1055 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-json/LICENSE
+-rw-r--r--   0     1001      123    16770 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-json/src/json/deserialize.rs
+-rw-r--r--   0     1001      123     6564 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-json/src/json/infer_schema.rs
+-rw-r--r--   0     1001      123      189 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-json/src/json/mod.rs
+-rw-r--r--   0     1001      123       30 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-json/src/lib.rs
+-rw-r--r--   0     1001      123     1198 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-json/src/ndjson/deserialize.rs
+-rw-r--r--   0     1001      123     4808 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-json/src/ndjson/file.rs
+-rw-r--r--   0     1001      123      143 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-json/src/ndjson/mod.rs
+-rw-r--r--   0        0        0     5152 1970-01-01 00:00:00.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-plan/Cargo.toml
+-rw-r--r--   0     1001      123     1055 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-plan/LICENSE
+-rw-r--r--   0     1001      123       45 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/constants.rs
+-rw-r--r--   0     1001      123    17253 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/dot.rs
+-rw-r--r--   0     1001      123     4171 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/dsl/arithmetic.rs
+-rw-r--r--   0     1001      123     3992 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/dsl/arity.rs
+-rw-r--r--   0     1001      123     1278 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/dsl/array.rs
+-rw-r--r--   0     1001      123      935 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/dsl/binary.rs
+-rw-r--r--   0     1001      123      650 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/dsl/cat.rs
+-rw-r--r--   0     1001      123    10228 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/dsl/dt.rs
+-rw-r--r--   0     1001      123     9538 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/dsl/expr.rs
+-rw-r--r--   0     1001      123     6441 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/dsl/expr_dyn_fn.rs
+-rw-r--r--   0     1001      123      753 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/dsl/from.rs
+-rw-r--r--   0     1001      123       85 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/dsl/function_expr/abs.rs
+-rw-r--r--   0     1001      123     1431 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/dsl/function_expr/arg_where.rs
+-rw-r--r--   0     1001      123     1074 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/dsl/function_expr/array.rs
+-rw-r--r--   0     1001      123     1327 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/dsl/function_expr/binary.rs
+-rw-r--r--   0     1001      123     4221 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/dsl/function_expr/boolean.rs
+-rw-r--r--   0     1001      123     1910 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/dsl/function_expr/bounds.rs
+-rw-r--r--   0     1001      123     1216 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/dsl/function_expr/cat.rs
+-rw-r--r--   0     1001      123      344 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/dsl/function_expr/clip.rs
+-rw-r--r--   0     1001      123      257 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/dsl/function_expr/concat.rs
+-rw-r--r--   0     1001      123     6261 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/dsl/function_expr/correlation.rs
+-rw-r--r--   0     1001      123     1593 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/dsl/function_expr/cum.rs
+-rw-r--r--   0     1001      123     9597 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/dsl/function_expr/datetime.rs
+-rw-r--r--   0     1001      123      782 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/dsl/function_expr/dispatch.rs
+-rw-r--r--   0     1001      123     2567 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/dsl/function_expr/fill_null.rs
+-rw-r--r--   0     1001      123      992 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/dsl/function_expr/fused.rs
+-rw-r--r--   0     1001      123     8119 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/dsl/function_expr/list.rs
+-rw-r--r--   0     1001      123      581 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/dsl/function_expr/log.rs
+-rw-r--r--   0     1001      123    21146 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/dsl/function_expr/mod.rs
+-rw-r--r--   0     1001      123      462 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/dsl/function_expr/nan.rs
+-rw-r--r--   0     1001      123     3132 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/dsl/function_expr/pow.rs
+-rw-r--r--   0     1001      123      152 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/dsl/function_expr/rolling.rs
+-rw-r--r--   0     1001      123      260 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/dsl/function_expr/round.rs
+-rw-r--r--   0     1001      123      200 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/dsl/function_expr/row_hash.rs
+-rw-r--r--   0     1001      123    14453 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/dsl/function_expr/schema.rs
+-rw-r--r--   0     1001      123      306 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/dsl/function_expr/search_sorted.rs
+-rw-r--r--   0     1001      123     3812 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/dsl/function_expr/shift_and_fill.rs
+-rw-r--r--   0     1001      123     1238 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/dsl/function_expr/shrink_type.rs
+-rw-r--r--   0     1001      123      972 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/dsl/function_expr/sign.rs
+-rw-r--r--   0     1001      123    21047 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/dsl/function_expr/strings.rs
+-rw-r--r--   0     1001      123     1017 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/dsl/function_expr/struct_.rs
+-rw-r--r--   0     1001      123     5509 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/dsl/function_expr/temporal.rs
+-rw-r--r--   0     1001      123     5122 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/dsl/function_expr/trigonometry.rs
+-rw-r--r--   0     1001      123      170 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/dsl/function_expr/unique.rs
+-rw-r--r--   0     1001      123     1155 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/dsl/functions/arity.rs
+-rw-r--r--   0     1001      123      611 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/dsl/functions/coerce.rs
+-rw-r--r--   0     1001      123     2717 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/dsl/functions/concat.rs
+-rw-r--r--   0     1001      123     4525 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/dsl/functions/correlation.rs
+-rw-r--r--   0     1001      123     8736 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/dsl/functions/horizontal.rs
+-rw-r--r--   0     1001      123     1044 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/dsl/functions/index.rs
+-rw-r--r--   0     1001      123      968 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/dsl/functions/mod.rs
+-rw-r--r--   0     1001      123     9827 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/dsl/functions/range.rs
+-rw-r--r--   0     1001      123     1308 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/dsl/functions/selectors.rs
+-rw-r--r--   0     1001      123     1973 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/dsl/functions/syntactic_sugar.rs
+-rw-r--r--   0     1001      123    11328 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/dsl/functions/temporal.rs
+-rw-r--r--   0     1001      123    10213 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/dsl/list.rs
+-rw-r--r--   0     1001      123     3772 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/dsl/meta.rs
+-rw-r--r--   0     1001      123    61431 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/dsl/mod.rs
+-rw-r--r--   0     1001      123       40 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/dsl/names.rs
+-rw-r--r--   0     1001      123     2658 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/dsl/options.rs
+-rw-r--r--   0     1001      123     1068 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/dsl/selector.rs
+-rw-r--r--   0     1001      123    17095 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/dsl/string.rs
+-rw-r--r--   0     1001      123     2715 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/dsl/struct_.rs
+-rw-r--r--   0     1001      123       38 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/frame/mod.rs
+-rw-r--r--   0     1001      123      933 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/frame/opt_state.rs
+-rw-r--r--   0     1001      123      466 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/global.rs
+-rw-r--r--   0     1001      123      175 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/lib.rs
+-rw-r--r--   0     1001      123     8318 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/logical_plan/aexpr/mod.rs
+-rw-r--r--   0     1001      123    11742 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/logical_plan/aexpr/schema.rs
+-rw-r--r--   0     1001      123    25683 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/logical_plan/alp.rs
+-rw-r--r--   0     1001      123     1622 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/logical_plan/anonymous_scan.rs
+-rw-r--r--   0     1001      123     1428 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/logical_plan/apply.rs
+-rw-r--r--   0     1001      123    24898 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/logical_plan/builder.rs
+-rw-r--r--   0     1001      123    29993 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/logical_plan/conversion.rs
+-rw-r--r--   0     1001      123      301 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/logical_plan/debug.rs
+-rw-r--r--   0     1001      123    15470 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/logical_plan/format.rs
+-rw-r--r--   0     1001      123      895 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/logical_plan/functions/drop.rs
+-rw-r--r--   0     1001      123      137 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/logical_plan/functions/explode.rs
+-rw-r--r--   0     1001      123     1169 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/logical_plan/functions/merge_sorted.rs
+-rw-r--r--   0     1001      123    11905 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/logical_plan/functions/mod.rs
+-rw-r--r--   0     1001      123     1330 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/logical_plan/functions/rename.rs
+-rw-r--r--   0     1001      123    10140 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/logical_plan/iterator.rs
+-rw-r--r--   0     1001      123    10559 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/logical_plan/lit.rs
+-rw-r--r--   0     1001      123     8072 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/logical_plan/mod.rs
+-rw-r--r--   0     1001      123     7416 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/logical_plan/optimizer/cache_states.rs
+-rw-r--r--   0     1001      123    15277 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/logical_plan/optimizer/cse.rs
+-rw-r--r--   0     1001      123     2889 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/logical_plan/optimizer/delay_rechunk.rs
+-rw-r--r--   0     1001      123     3236 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/logical_plan/optimizer/drop_nulls.rs
+-rw-r--r--   0     1001      123     3994 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/logical_plan/optimizer/fast_projection.rs
+-rw-r--r--   0     1001      123    14479 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/logical_plan/optimizer/file_caching.rs
+-rw-r--r--   0     1001      123     1556 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/logical_plan/optimizer/flatten_union.rs
+-rw-r--r--   0     1001      123     6017 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/logical_plan/optimizer/fused.rs
+-rw-r--r--   0     1001      123     6774 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/logical_plan/optimizer/mod.rs
+-rw-r--r--   0     1001      123     1222 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/logical_plan/optimizer/predicate_pushdown/keys.rs
+-rw-r--r--   0     1001      123    28901 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/logical_plan/optimizer/predicate_pushdown/mod.rs
+-rw-r--r--   0     1001      123     2571 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/logical_plan/optimizer/predicate_pushdown/rename.rs
+-rw-r--r--   0     1001      123    15756 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/logical_plan/optimizer/predicate_pushdown/utils.rs
+-rw-r--r--   0     1001      123     1755 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/functions/melt.rs
+-rw-r--r--   0     1001      123     3930 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/functions/mod.rs
+-rw-r--r--   0     1001      123     1799 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/generic.rs
+-rw-r--r--   0     1001      123     3269 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/groupby.rs
+-rw-r--r--   0     1001      123     2638 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/hstack.rs
+-rw-r--r--   0     1001      123    15752 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/joins.rs
+-rw-r--r--   0     1001      123    26507 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/mod.rs
+-rw-r--r--   0     1001      123     3707 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/projection.rs
+-rw-r--r--   0     1001      123     2639 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/rename.rs
+-rw-r--r--   0     1001      123     3501 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/semi_anti_join.rs
+-rw-r--r--   0     1001      123    27269 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/logical_plan/optimizer/simplify_expr.rs
+-rw-r--r--   0     1001      123     3492 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/logical_plan/optimizer/slice_pushdown_expr.rs
+-rw-r--r--   0     1001      123    13232 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/logical_plan/optimizer/slice_pushdown_lp.rs
+-rw-r--r--   0     1001      123     4181 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/logical_plan/optimizer/stack_opt.rs
+-rw-r--r--   0     1001      123     9725 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/logical_plan/optimizer/type_coercion/binary.rs
+-rw-r--r--   0     1001      123    20215 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/logical_plan/optimizer/type_coercion/mod.rs
+-rw-r--r--   0     1001      123    10545 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/logical_plan/options.rs
+-rw-r--r--   0     1001      123    18601 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/logical_plan/projection.rs
+-rw-r--r--   0     1001      123     6144 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/logical_plan/pyarrow.rs
+-rw-r--r--   0     1001      123    13026 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/logical_plan/schema.rs
+-rw-r--r--   0     1001      123      832 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/prelude.rs
+-rw-r--r--   0     1001      123    12428 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/utils.rs
+-rw-r--r--   0        0        0     2037 1970-01-01 00:00:00.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-time/Cargo.toml
+-rw-r--r--   0     1001      123     1055 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-time/LICENSE
+-rw-r--r--   0     1001      123      143 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-time/README.md
+-rw-r--r--   0     1001      123     3565 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-time/src/chunkedarray/date.rs
+-rw-r--r--   0     1001      123     6465 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-time/src/chunkedarray/datetime.rs
+-rw-r--r--   0     1001      123     3305 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-time/src/chunkedarray/duration.rs
+-rw-r--r--   0     1001      123     5607 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-time/src/chunkedarray/kernels.rs
+-rw-r--r--   0     1001      123     1062 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-time/src/chunkedarray/mod.rs
+-rw-r--r--   0     1001      123     7302 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-time/src/chunkedarray/rolling_window/floats.rs
+-rw-r--r--   0     1001      123     2582 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-time/src/chunkedarray/rolling_window/ints.rs
+-rw-r--r--   0     1001      123    11101 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-time/src/chunkedarray/rolling_window/mod.rs
+-rw-r--r--   0     1001      123      428 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-time/src/chunkedarray/rolling_window/rolling_kernels/mod.rs
+-rw-r--r--   0     1001      123     6408 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-time/src/chunkedarray/rolling_window/rolling_kernels/no_nulls.rs
+-rw-r--r--   0     1001      123     2372 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-time/src/chunkedarray/time.rs
+-rw-r--r--   0     1001      123    18180 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-time/src/chunkedarray/utf8/infer.rs
+-rw-r--r--   0     1001      123    18997 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-time/src/chunkedarray/utf8/mod.rs
+-rw-r--r--   0     1001      123     3975 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-time/src/chunkedarray/utf8/patterns.rs
+-rw-r--r--   0     1001      123    10548 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-time/src/chunkedarray/utf8/strptime.rs
+-rw-r--r--   0     1001      123     3442 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-time/src/date_range.rs
+-rw-r--r--   0     1001      123    34469 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-time/src/groupby/dynamic.rs
+-rw-r--r--   0     1001      123       88 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-time/src/groupby/mod.rs
+-rw-r--r--   0     1001      123      621 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-time/src/lib.rs
+-rw-r--r--   0     1001      123     2976 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-time/src/month_end.rs
+-rw-r--r--   0     1001      123     3365 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-time/src/month_start.rs
+-rw-r--r--   0     1001      123      274 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-time/src/prelude.rs
+-rw-r--r--   0     1001      123     1381 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-time/src/round.rs
+-rw-r--r--   0     1001      123     3992 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-time/src/series/_trait.rs
+-rw-r--r--   0     1001      123      136 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-time/src/series/implementations/boolean.rs
+-rw-r--r--   0     1001      123      140 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-time/src/series/implementations/categoricals.rs
+-rw-r--r--   0     1001      123      133 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-time/src/series/implementations/date.rs
+-rw-r--r--   0     1001      123      137 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-time/src/series/implementations/datetime.rs
+-rw-r--r--   0     1001      123      137 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-time/src/series/implementations/duration.rs
+-rw-r--r--   0     1001      123     1863 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-time/src/series/implementations/floats.rs
+-rw-r--r--   0     1001      123     1792 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-time/src/series/implementations/integers.rs
+-rw-r--r--   0     1001      123      133 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-time/src/series/implementations/list.rs
+-rw-r--r--   0     1001      123      486 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-time/src/series/implementations/mod.rs
+-rw-r--r--   0     1001      123      155 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-time/src/series/implementations/object.rs
+-rw-r--r--   0     1001      123      135 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-time/src/series/implementations/struct_.rs
+-rw-r--r--   0     1001      123      133 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-time/src/series/implementations/time.rs
+-rw-r--r--   0     1001      123      133 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-time/src/series/implementations/utf8.rs
+-rw-r--r--   0     1001      123    12787 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-time/src/series/mod.rs
+-rw-r--r--   0     1001      123     1443 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-time/src/truncate.rs
+-rw-r--r--   0     1001      123     6845 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-time/src/upsample.rs
+-rw-r--r--   0     1001      123     2511 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-time/src/utils.rs
+-rw-r--r--   0     1001      123     1524 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-time/src/windows/bounds.rs
+-rw-r--r--   0     1001      123     2672 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-time/src/windows/calendar.rs
+-rw-r--r--   0     1001      123    25015 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-time/src/windows/duration.rs
+-rw-r--r--   0     1001      123    21244 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-time/src/windows/groupby.rs
+-rw-r--r--   0     1001      123      503 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-time/src/windows/mod.rs
+-rw-r--r--   0     1001      123    23652 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-time/src/windows/test.rs
+-rw-r--r--   0     1001      123    10657 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-time/src/windows/window.rs
+-rw-r--r--   0        0        0      894 1970-01-01 00:00:00.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-error/Cargo.toml
+-rw-r--r--   0     1001      123     1055 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-error/LICENSE
+-rw-r--r--   0     1001      123      145 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-error/README.md
+-rw-r--r--   0     1001      123     6584 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/local_dependencies/polars-error/src/lib.rs
+-rw-r--r--   0        0        0     4393 1970-01-01 00:00:00.000000 polars_lts_cpu-0.18.3/Cargo.toml
+-rw-r--r--   0     1001      123       76 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/.gitignore
+-rw-r--r--   0     1001      123     1055 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/LICENSE
+-rw-r--r--   0     1001      123     2414 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/Makefile
+-rw-r--r--   0     1001      123    11998 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/README.md
+-rw-r--r--   0     1001      123      651 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/build.rs
+-rw-r--r--   0     1001      123       32 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/docs/.gitignore
+-rw-r--r--   0     1001      123      679 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/docs/Makefile
+-rw-r--r--   0     1001      123      318 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/docs/_templates/api_redirect.html
+-rw-r--r--   0     1001      123      151 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/docs/_templates/autosummary/accessor.rst
+-rw-r--r--   0     1001      123      160 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/docs/_templates/autosummary/accessor_attribute.rst
+-rw-r--r--   0     1001      123      168 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/docs/_templates/autosummary/accessor_callable.rst
+-rw-r--r--   0     1001      123      157 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/docs/_templates/autosummary/accessor_method.rst
+-rw-r--r--   0     1001      123      836 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/docs/_templates/autosummary/class.rst
+-rw-r--r--   0     1001      123       94 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/docs/_templates/autosummary/class_without_autosummary.rst
+-rw-r--r--   0     1001      123      406 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/docs/_templates/sidebar-nav-bs.html
+-rw-r--r--   0     1001      123      491 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/docs/requirements-docs.txt
+-rw-r--r--   0     1001      123     1164 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/docs/run_live_docs_server.py
+-rw-r--r--   0     1001      123     1567 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/docs/source/_static/css/custom.css
+-rw-r--r--   0     1001      123     7297 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/docs/source/conf.py
+-rw-r--r--   0     1001      123       51 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/docs/source/index.rst
+-rw-r--r--   0     1001      123     6767 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/docs/source/reference/api.rst
+-rw-r--r--   0     1001      123     2069 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/docs/source/reference/config.rst
+-rw-r--r--   0     1001      123      274 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/docs/source/reference/dataframe/aggregation.rst
+-rw-r--r--   0     1001      123      221 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/docs/source/reference/dataframe/attributes.rst
+-rw-r--r--   0     1001      123      142 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/docs/source/reference/dataframe/computation.rst
+-rw-r--r--   0     1001      123      319 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/docs/source/reference/dataframe/descriptive.rst
+-rw-r--r--   0     1001      123      319 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/docs/source/reference/dataframe/export.rst
+-rw-r--r--   0     1001      123      464 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/docs/source/reference/dataframe/groupby.rst
+-rw-r--r--   0     1001      123      379 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/docs/source/reference/dataframe/index.rst
+-rw-r--r--   0     1001      123      189 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/docs/source/reference/dataframe/miscellaneous.rst
+-rw-r--r--   0     1001      123     1538 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/docs/source/reference/dataframe/modify_select.rst
+-rw-r--r--   0     1001      123      673 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/docs/source/reference/datatypes.rst
+-rw-r--r--   0     1001      123      421 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/docs/source/reference/exceptions.rst
+-rw-r--r--   0     1001      123      391 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/docs/source/reference/expressions/aggregation.rst
+-rw-r--r--   0     1001      123      267 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/docs/source/reference/expressions/array.rst
+-rw-r--r--   0     1001      123      309 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/docs/source/reference/expressions/binary.rst
+-rw-r--r--   0     1001      123      338 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/docs/source/reference/expressions/boolean.rst
+-rw-r--r--   0     1001      123      237 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/docs/source/reference/expressions/categories.rst
+-rw-r--r--   0     1001      123      221 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/docs/source/reference/expressions/columns.rst
+-rw-r--r--   0     1001      123     1061 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/docs/source/reference/expressions/computation.rst
+-rw-r--r--   0     1001      123     1130 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/docs/source/reference/expressions/functions.rst
+-rw-r--r--   0     1001      123      470 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/docs/source/reference/expressions/index.rst
+-rw-r--r--   0     1001      123      722 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/docs/source/reference/expressions/list.rst
+-rw-r--r--   0     1001      123      432 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/docs/source/reference/expressions/meta.rst
+-rw-r--r--   0     1001      123      159 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/docs/source/reference/expressions/miscellaneous.rst
+-rw-r--r--   0     1001      123      977 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/docs/source/reference/expressions/modify_select.rst
+-rw-r--r--   0     1001      123      679 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/docs/source/reference/expressions/operators.rst
+-rw-r--r--   0     1001      123      951 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/docs/source/reference/expressions/string.rst
+-rw-r--r--   0     1001      123      254 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/docs/source/reference/expressions/struct.rst
+-rw-r--r--   0     1001      123     1036 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/docs/source/reference/expressions/temporal.rst
+-rw-r--r--   0     1001      123       98 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/docs/source/reference/expressions/window.rst
+-rw-r--r--   0     1001      123      836 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/docs/source/reference/functions.rst
+-rw-r--r--   0     1001      123      405 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/docs/source/reference/index.rst
+-rw-r--r--   0     1001      123     1294 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/docs/source/reference/io.rst
+-rw-r--r--   0     1001      123      277 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/docs/source/reference/lazyframe/aggregation.rst
+-rw-r--r--   0     1001      123      179 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/docs/source/reference/lazyframe/attributes.rst
+-rw-r--r--   0     1001      123      146 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/docs/source/reference/lazyframe/descriptive.rst
+-rw-r--r--   0     1001      123      497 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/docs/source/reference/lazyframe/groupby.rst
+-rw-r--r--   0     1001      123      354 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/docs/source/reference/lazyframe/index.rst
+-rw-r--r--   0     1001      123      455 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/docs/source/reference/lazyframe/miscellaneous.rst
+-rw-r--r--   0     1001      123     1013 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/docs/source/reference/lazyframe/modify_select.rst
+-rw-r--r--   0     1001      123     3279 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/docs/source/reference/selectors.rst
+-rw-r--r--   0     1001      123      358 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/docs/source/reference/series/aggregation.rst
+-rw-r--r--   0     1001      123      277 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/docs/source/reference/series/array.rst
+-rw-r--r--   0     1001      123      257 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/docs/source/reference/series/attributes.rst
+-rw-r--r--   0     1001      123      321 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/docs/source/reference/series/binary.rst
+-rw-r--r--   0     1001      123      117 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/docs/source/reference/series/boolean.rst
+-rw-r--r--   0     1001      123      241 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/docs/source/reference/series/categories.rst
+-rw-r--r--   0     1001      123     1103 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/docs/source/reference/series/computation.rst
+-rw-r--r--   0     1001      123      744 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/docs/source/reference/series/descriptive.rst
+-rw-r--r--   0     1001      123      240 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/docs/source/reference/series/export.rst
+-rw-r--r--   0     1001      123      437 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/docs/source/reference/series/index.rst
+-rw-r--r--   0     1001      123      776 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/docs/source/reference/series/list.rst
+-rw-r--r--   0     1001      123      236 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/docs/source/reference/series/miscellaneous.rst
+-rw-r--r--   0     1001      123     1077 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/docs/source/reference/series/modify_select.rst
+-rw-r--r--   0     1001      123     1021 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/docs/source/reference/series/string.rst
+-rw-r--r--   0     1001      123      421 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/docs/source/reference/series/struct.rst
+-rw-r--r--   0     1001      123     1192 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/docs/source/reference/series/temporal.rst
+-rw-r--r--   0     1001      123      503 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/docs/source/reference/sql.rst
+-rw-r--r--   0     1001      123     8067 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/docs/source/reference/testing.rst
+-rw-r--r--   0     1001      123      168 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/docs/source/reference/utils.rst
+-rw-r--r--   0     1001      123     6161 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/polars/__init__.py
+-rw-r--r--   0     1001      123      280 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/polars/_reexport.py
+-rw-r--r--   0     1001      123    13229 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/polars/api.py
+-rw-r--r--   0     1001      123    29763 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/polars/config.py
+-rw-r--r--   0     1001      123    28105 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/polars/convert.py
+-rw-r--r--   0     1001      123       77 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/polars/dataframe/__init__.py
+-rw-r--r--   0     1001      123     5227 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/polars/dataframe/_html.py
+-rw-r--r--   0     1001      123   316258 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/polars/dataframe/frame.py
+-rw-r--r--   0     1001      123    40637 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/polars/dataframe/groupby.py
+-rw-r--r--   0     1001      123     2692 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/polars/datatypes/__init__.py
+-rw-r--r--   0     1001      123    16199 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/polars/datatypes/classes.py
+-rw-r--r--   0     1001      123     1603 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/polars/datatypes/constants.py
+-rw-r--r--   0     1001      123     4701 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/polars/datatypes/constructor.py
+-rw-r--r--   0     1001      123    15739 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/polars/datatypes/convert.py
+-rw-r--r--   0     1001      123     7338 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/polars/dependencies.py
+-rw-r--r--   0     1001      123     3573 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/polars/exceptions.py
+-rw-r--r--   0     1001      123       61 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/polars/expr/__init__.py
+-rw-r--r--   0     1001      123     3020 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/polars/expr/array.py
+-rw-r--r--   0     1001      123     2704 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/polars/expr/binary.py
+-rw-r--r--   0     1001      123     1698 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/polars/expr/categorical.py
+-rw-r--r--   0     1001      123    77648 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/polars/expr/datetime.py
+-rw-r--r--   0     1001      123   261911 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/polars/expr/expr.py
+-rw-r--r--   0     1001      123    23905 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/polars/expr/list.py
+-rw-r--r--   0     1001      123     4050 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/polars/expr/meta.py
+-rw-r--r--   0     1001      123    59014 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/polars/expr/string.py
+-rw-r--r--   0     1001      123     5426 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/polars/expr/struct.py
+-rw-r--r--   0     1001      123     2068 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/polars/functions/__init__.py
+-rw-r--r--   0     1001      123    16541 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/polars/functions/as_datatype.py
+-rw-r--r--   0     1001      123    18853 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/polars/functions/eager.py
+-rw-r--r--   0     1001      123    72401 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/polars/functions/lazy.py
+-rw-r--r--   0     1001      123    16227 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/polars/functions/range.py
+-rw-r--r--   0     1001      123     6027 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/polars/functions/repeat.py
+-rw-r--r--   0     1001      123     6139 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/polars/functions/whenthen.py
+-rw-r--r--   0     1001      123      952 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/polars/io/__init__.py
+-rw-r--r--   0     1001      123     6264 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/polars/io/_utils.py
+-rw-r--r--   0     1001      123      861 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/polars/io/avro.py
+-rw-r--r--   0     1001      123      144 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/polars/io/csv/__init__.py
+-rw-r--r--   0     1001      123     1072 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/polars/io/csv/_utils.py
+-rw-r--r--   0     1001      123     4681 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/polars/io/csv/batched_reader.py
+-rw-r--r--   0     1001      123    35482 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/polars/io/csv/functions.py
+-rw-r--r--   0     1001      123     5627 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/polars/io/database.py
+-rw-r--r--   0     1001      123    11047 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/polars/io/delta.py
+-rw-r--r--   0     1001      123       75 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/polars/io/excel/__init__.py
+-rw-r--r--   0     1001      123    18449 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/polars/io/excel/_write_utils.py
+-rw-r--r--   0     1001      123     6466 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/polars/io/excel/functions.py
+-rw-r--r--   0     1001      123      142 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/polars/io/ipc/__init__.py
+-rw-r--r--   0     1001      123     1227 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/polars/io/ipc/anonymous_scan.py
+-rw-r--r--   0     1001      123     5804 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/polars/io/ipc/functions.py
+-rw-r--r--   0     1001      123      502 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/polars/io/json.py
+-rw-r--r--   0     1001      123     2207 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/polars/io/ndjson.py
+-rw-r--r--   0     1001      123      170 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/polars/io/parquet/__init__.py
+-rw-r--r--   0     1001      123     1259 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/polars/io/parquet/anonymous_scan.py
+-rw-r--r--   0     1001      123     7177 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/polars/io/parquet/functions.py
+-rw-r--r--   0     1001      123      136 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/polars/io/pyarrow_dataset/__init__.py
+-rw-r--r--   0     1001      123     2291 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/polars/io/pyarrow_dataset/anonymous_scan.py
+-rw-r--r--   0     1001      123     3601 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/polars/io/pyarrow_dataset/functions.py
+-rw-r--r--   0     1001      123       77 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/polars/lazyframe/__init__.py
+-rw-r--r--   0     1001      123   168959 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/polars/lazyframe/frame.py
+-rw-r--r--   0     1001      123    24078 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/polars/lazyframe/groupby.py
+-rw-r--r--   0     1001      123        0 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/polars/py.typed
+-rw-r--r--   0     1001      123    32502 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/polars/selectors.py
+-rw-r--r--   0     1001      123       69 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/polars/series/__init__.py
+-rw-r--r--   0     1001      123     1572 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/polars/series/_numpy.py
+-rw-r--r--   0     1001      123     2515 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/polars/series/array.py
+-rw-r--r--   0     1001      123     1913 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/polars/series/binary.py
+-rw-r--r--   0     1001      123     1692 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/polars/series/categorical.py
+-rw-r--r--   0     1001      123    51825 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/polars/series/datetime.py
+-rw-r--r--   0     1001      123    13196 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/polars/series/list.py
+-rw-r--r--   0     1001      123   170198 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/polars/series/series.py
+-rw-r--r--   0     1001      123    37808 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/polars/series/string.py
+-rw-r--r--   0     1001      123     2542 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/polars/series/struct.py
+-rw-r--r--   0     1001      123     5361 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/polars/series/utils.py
+-rw-r--r--   0     1001      123     7559 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/polars/slice.py
+-rw-r--r--   0     1001      123       75 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/polars/sql/__init__.py
+-rw-r--r--   0     1001      123    17409 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/polars/sql/context.py
+-rw-r--r--   0     1001      123     4793 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/polars/string_cache.py
+-rw-r--r--   0     1001      123      362 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/polars/testing/__init__.py
+-rw-r--r--   0     1001      123     1060 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/polars/testing/_private.py
+-rw-r--r--   0     1001      123    16964 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/polars/testing/asserts.py
+-rw-r--r--   0     1001      123      898 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/polars/testing/parametric/__init__.py
+-rw-r--r--   0     1001      123    26833 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/polars/testing/parametric/primitives.py
+-rw-r--r--   0     1001      123     3409 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/polars/testing/parametric/profiles.py
+-rw-r--r--   0     1001      123    12132 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/polars/testing/parametric/strategies.py
+-rw-r--r--   0     1001      123     6304 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/polars/type_aliases.py
+-rw-r--r--   0     1001      123     1169 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/polars/utils/__init__.py
+-rw-r--r--   0     1001      123    54302 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/polars/utils/_construction.py
+-rw-r--r--   0     1001      123     3902 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/polars/utils/_parse_expr_input.py
+-rw-r--r--   0     1001      123      711 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/polars/utils/_scan.py
+-rw-r--r--   0     1001      123      579 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/polars/utils/_wrap.py
+-rw-r--r--   0     1001      123      683 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/polars/utils/build_info.py
+-rw-r--r--   0     1001      123     8609 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/polars/utils/convert.py
+-rw-r--r--   0     1001      123     6132 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/polars/utils/decorators.py
+-rw-r--r--   0     1001      123     1660 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/polars/utils/meta.py
+-rw-r--r--   0     1001      123      514 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/polars/utils/polars_version.py
+-rw-r--r--   0     1001      123     2673 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/polars/utils/show_versions.py
+-rw-r--r--   0     1001      123    12905 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/polars/utils/various.py
+-rw-r--r--   0     1001      123     5377 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/pyproject.toml
+-rw-r--r--   0     1001      123      698 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/requirements-dev.txt
+-rw-r--r--   0     1001      123       68 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/requirements-lint.txt
+-rw-r--r--   0     1001      123     1640 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/scripts/check_stacklevels.py
+-rw-r--r--   0     1001      123    10980 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/src/apply/dataframe.rs
+-rw-r--r--   0     1001      123     7448 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/src/apply/lazy.rs
+-rw-r--r--   0     1001      123     8402 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/src/apply/mod.rs
+-rw-r--r--   0     1001      123    90009 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/src/apply/series.rs
+-rw-r--r--   0     1001      123       32 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/src/arrow_interop/mod.rs
+-rw-r--r--   0     1001      123     1306 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/src/arrow_interop/to_py.rs
+-rw-r--r--   0     1001      123     3902 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/src/arrow_interop/to_rust.rs
+-rw-r--r--   0     1001      123     5250 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/src/batched_csv.rs
+-rw-r--r--   0     1001      123    48675 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/src/conversion.rs
+-rw-r--r--   0     1001      123    45928 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/src/dataframe.rs
+-rw-r--r--   0     1001      123     3950 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/src/datatypes.rs
+-rw-r--r--   0     1001      123     3288 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/src/error.rs
+-rw-r--r--   0     1001      123      570 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/src/expr/array.rs
+-rw-r--r--   0     1001      123     2080 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/src/expr/binary.rs
+-rw-r--r--   0     1001      123      274 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/src/expr/categorical.rs
+-rw-r--r--   0     1001      123     5935 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/src/expr/datetime.rs
+-rw-r--r--   0     1001      123    34040 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/src/expr/general.rs
+-rw-r--r--   0     1001      123     3937 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/src/expr/list.rs
+-rw-r--r--   0     1001      123     2907 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/src/expr/meta.rs
+-rw-r--r--   0     1001      123      870 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/src/expr/mod.rs
+-rw-r--r--   0     1001      123     8677 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/src/expr/string.rs
+-rw-r--r--   0     1001      123      467 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/src/expr/struct.rs
+-rw-r--r--   0     1001      123     9482 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/src/file.rs
+-rw-r--r--   0     1001      123     3307 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/src/functions/eager.rs
+-rw-r--r--   0     1001      123     1657 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/src/functions/io.rs
+-rw-r--r--   0     1001      123    11977 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/src/functions/lazy.rs
+-rw-r--r--   0     1001      123     1312 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/src/functions/meta.rs
+-rw-r--r--   0     1001      123      217 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/src/functions/misc.rs
+-rw-r--r--   0     1001      123       87 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/src/functions/mod.rs
+-rw-r--r--   0     1001      123     1474 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/src/functions/whenthen.rs
+-rw-r--r--   0     1001      123    30767 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/src/lazyframe.rs
+-rw-r--r--   0     1001      123     2670 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/src/lazygroupby.rs
+-rw-r--r--   0     1001      123     8268 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/src/lib.rs
+-rw-r--r--   0     1001      123     1029 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/src/object.rs
+-rw-r--r--   0     1001      123      122 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/src/prelude.rs
+-rw-r--r--   0     1001      123      435 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/src/py_modules.rs
+-rw-r--r--   0     1001      123     1964 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/src/series/aggregation.rs
+-rw-r--r--   0     1001      123     5406 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/src/series/arithmetic.rs
+-rw-r--r--   0     1001      123     5138 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/src/series/comparison.rs
+-rw-r--r--   0     1001      123     9077 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/src/series/construction.rs
+-rw-r--r--   0     1001      123     8971 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/src/series/export.rs
+-rw-r--r--   0     1001      123    26521 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/src/series/mod.rs
+-rw-r--r--   0     1001      123     4569 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/src/series/numpy_ufunc.rs
+-rw-r--r--   0     1001      123     4046 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/src/series/set_at_idx.rs
+-rw-r--r--   0     1001      123     1036 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/src/sql.rs
+-rw-r--r--   0     1001      123     2335 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/src/utils.rs
+-rw-r--r--   0     1001      123     6165 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/tests/README.md
+-rw-r--r--   0     1001      123     2189 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/tests/benchmark/groupby-datagen.R
+-rw-r--r--   0     1001      123     7963 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/tests/benchmark/run_h2oai_benchmark.py
+-rw-r--r--   0     1001      123     6530 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/tests/benchmark/test_release.py
+-rw-r--r--   0     1001      123     4589 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/tests/docs/run_doctest.py
+-rw-r--r--   0     1001      123      179 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/tests/parametric/conftest.py
+-rw-r--r--   0     1001      123     3856 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/tests/parametric/test_dataframe.py
+-rw-r--r--   0     1001      123     1692 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/tests/parametric/test_lazyframe.py
+-rw-r--r--   0     1001      123     6897 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/tests/parametric/test_series.py
+-rw-r--r--   0     1001      123     8299 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/tests/parametric/test_testing.py
+-rw-r--r--   0     1001      123        0 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/tests/unit/__init__.py
+-rw-r--r--   0     1001      123     3382 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/tests/unit/conftest.py
+-rw-r--r--   0     1001      123       86 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/tests/unit/datatypes/__init__.py
+-rw-r--r--   0     1001      123      973 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/tests/unit/datatypes/test_array.py
+-rw-r--r--   0     1001      123      847 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/tests/unit/datatypes/test_binary.py
+-rw-r--r--   0     1001      123     1420 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/tests/unit/datatypes/test_bool.py
+-rw-r--r--   0     1001      123    13228 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/tests/unit/datatypes/test_categorical.py
+-rw-r--r--   0     1001      123     5222 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/tests/unit/datatypes/test_decimal.py
+-rw-r--r--   0     1001      123      549 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/tests/unit/datatypes/test_duration.py
+-rw-r--r--   0     1001      123      423 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/tests/unit/datatypes/test_integer.py
+-rw-r--r--   0     1001      123    13216 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/tests/unit/datatypes/test_list.py
+-rw-r--r--   0     1001      123      284 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/tests/unit/datatypes/test_null.py
+-rw-r--r--   0     1001      123     2801 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/tests/unit/datatypes/test_object.py
+-rw-r--r--   0     1001      123    27749 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/tests/unit/datatypes/test_struct.py
+-rw-r--r--   0     1001      123    87949 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/tests/unit/datatypes/test_temporal.py
+-rw-r--r--   0     1001      123      418 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/tests/unit/datatypes/test_time.py
+-rw-r--r--   0     1001      123        0 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/tests/unit/functions/__init__.py
+-rw-r--r--   0     1001      123    13970 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/tests/unit/functions/test_as_datatype.py
+-rw-r--r--   0     1001      123      480 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/tests/unit/functions/test_concat.py
+-rw-r--r--   0     1001      123    15610 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/tests/unit/functions/test_functions.py
+-rw-r--r--   0     1001      123    18470 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/tests/unit/functions/test_range.py
+-rw-r--r--   0     1001      123     3724 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/tests/unit/functions/test_repeat.py
+-rw-r--r--   0     1001      123      218 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/tests/unit/io/conftest.py
+-rw-r--r--   0     1001      123       16 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/tests/unit/io/files/delta-table/.part-00000-e42312d7-60e5-454d-acbc-db192d220e73-c000.snappy.parquet.crc
+-rw-r--r--   0     1001      123       16 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/tests/unit/io/files/delta-table/.part-00000-e4a999da-df45-4fb0-bdc4-d999fc0f58aa-c000.snappy.parquet.crc
+-rw-r--r--   0     1001      123       16 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/tests/unit/io/files/delta-table/_delta_log/.00000000000000000000.json.crc
+-rw-r--r--   0     1001      123       16 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/tests/unit/io/files/delta-table/_delta_log/.00000000000000000001.json.crc
+-rw-r--r--   0     1001      123      905 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/tests/unit/io/files/delta-table/_delta_log/00000000000000000000.json
+-rw-r--r--   0     1001      123      936 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/tests/unit/io/files/delta-table/_delta_log/00000000000000000001.json
+-rw-r--r--   0     1001      123      972 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/tests/unit/io/files/delta-table/part-00000-e42312d7-60e5-454d-acbc-db192d220e73-c000.snappy.parquet
+-rw-r--r--   0     1001      123      690 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/tests/unit/io/files/delta-table/part-00000-e4a999da-df45-4fb0-bdc4-d999fc0f58aa-c000.snappy.parquet
+-rw-r--r--   0     1001      123        0 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/tests/unit/io/files/empty.csv
+-rw-r--r--   0     1001      123     5959 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/tests/unit/io/files/example.xlsx
+-rw-r--r--   0     1001      123      457 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/tests/unit/io/files/foods1.csv
+-rw-r--r--   0     1001      123     2351 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/tests/unit/io/files/foods1.ipc
+-rw-r--r--   0     1001      123     1713 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/tests/unit/io/files/foods1.ndjson
+-rw-r--r--   0     1001      123     1427 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/tests/unit/io/files/foods1.parquet
+-rw-r--r--   0     1001      123      455 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/tests/unit/io/files/foods2.csv
+-rw-r--r--   0     1001      123     2351 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/tests/unit/io/files/foods2.ipc
+-rw-r--r--   0     1001      123     1711 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/tests/unit/io/files/foods2.ndjson
+-rw-r--r--   0     1001      123     1916 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/tests/unit/io/files/foods2.parquet
+-rw-r--r--   0     1001      123      455 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/tests/unit/io/files/foods3.csv
+-rw-r--r--   0     1001      123      457 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/tests/unit/io/files/foods4.csv
+-rw-r--r--   0     1001      123      452 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/tests/unit/io/files/foods5.csv
+-rw-r--r--   0     1001      123       49 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/tests/unit/io/files/gzipped.csv
+-rw-r--r--   0     1001      123       57 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/tests/unit/io/files/small.csv
+-rw-r--r--   0     1001      123      756 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/tests/unit/io/files/small.parquet
+-rw-r--r--   0     1001      123     1884 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/tests/unit/io/test_avro.py
+-rw-r--r--   0     1001      123    39230 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/tests/unit/io/test_csv.py
+-rw-r--r--   0     1001      123     6336 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/tests/unit/io/test_database.py
+-rw-r--r--   0     1001      123     6172 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/tests/unit/io/test_delta.py
+-rw-r--r--   0     1001      123    11169 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/tests/unit/io/test_excel.py
+-rw-r--r--   0     1001      123     5483 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/tests/unit/io/test_ipc.py
+-rw-r--r--   0     1001      123     3986 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/tests/unit/io/test_json.py
+-rw-r--r--   0     1001      123     7379 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/tests/unit/io/test_lazy_csv.py
+-rw-r--r--   0     1001      123     2060 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/tests/unit/io/test_lazy_ipc.py
+-rw-r--r--   0     1001      123     2867 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/tests/unit/io/test_lazy_json.py
+-rw-r--r--   0     1001      123    11145 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/tests/unit/io/test_lazy_parquet.py
+-rw-r--r--   0     1001      123     2012 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/tests/unit/io/test_other.py
+-rw-r--r--   0     1001      123    14201 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/tests/unit/io/test_parquet.py
+-rw-r--r--   0     1001      123      612 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/tests/unit/io/test_pickle.py
+-rw-r--r--   0     1001      123     3686 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/tests/unit/io/test_pyarrow_dataset.py
+-rw-r--r--   0     1001      123      509 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/tests/unit/namespaces/__init__.py
+-rw-r--r--   0     1001      123      589 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/tests/unit/namespaces/test_array.py
+-rw-r--r--   0     1001      123     3218 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/tests/unit/namespaces/test_binary.py
+-rw-r--r--   0     1001      123     2489 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/tests/unit/namespaces/test_categorical.py
+-rw-r--r--   0     1001      123    19585 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/tests/unit/namespaces/test_datetime.py
+-rw-r--r--   0     1001      123    14067 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/tests/unit/namespaces/test_list.py
+-rw-r--r--   0     1001      123     1829 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/tests/unit/namespaces/test_meta.py
+-rw-r--r--   0     1001      123    23544 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/tests/unit/namespaces/test_string.py
+-rw-r--r--   0     1001      123    17964 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/tests/unit/namespaces/test_strptime.py
+-rw-r--r--   0     1001      123      982 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/tests/unit/namespaces/test_struct.py
+-rw-r--r--   0     1001      123       85 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/tests/unit/operations/__init__.py
+-rw-r--r--   0     1001      123     7755 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/tests/unit/operations/test_aggregations.py
+-rw-r--r--   0     1001      123    10643 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/tests/unit/operations/test_apply.py
+-rw-r--r--   0     1001      123     6932 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/tests/unit/operations/test_arithmetic.py
+-rw-r--r--   0     1001      123     4631 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/tests/unit/operations/test_comparison.py
+-rw-r--r--   0     1001      123     3275 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/tests/unit/operations/test_drop.py
+-rw-r--r--   0     1001      123     8813 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/tests/unit/operations/test_explode.py
+-rw-r--r--   0     1001      123     3664 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/tests/unit/operations/test_filter.py
+-rw-r--r--   0     1001      123     1801 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/tests/unit/operations/test_folds.py
+-rw-r--r--   0     1001      123    24998 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/tests/unit/operations/test_groupby.py
+-rw-r--r--   0     1001      123     7649 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/tests/unit/operations/test_groupby_rolling.py
+-rw-r--r--   0     1001      123     2983 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/tests/unit/operations/test_is_in.py
+-rw-r--r--   0     1001      123    18169 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/tests/unit/operations/test_join.py
+-rw-r--r--   0     1001      123    14952 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/tests/unit/operations/test_join_asof.py
+-rw-r--r--   0     1001      123      643 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/tests/unit/operations/test_melt.py
+-rw-r--r--   0     1001      123    10253 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/tests/unit/operations/test_pivot.py
+-rw-r--r--   0     1001      123    19818 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/tests/unit/operations/test_rolling.py
+-rw-r--r--   0     1001      123     1917 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/tests/unit/operations/test_select.py
+-rw-r--r--   0     1001      123    20731 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/tests/unit/operations/test_sort.py
+-rw-r--r--   0     1001      123     4273 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/tests/unit/operations/test_statistics.py
+-rw-r--r--   0     1001      123     4130 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/tests/unit/operations/test_transpose.py
+-rw-r--r--   0     1001      123      771 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/tests/unit/operations/test_unique.py
+-rw-r--r--   0     1001      123    11694 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/tests/unit/operations/test_window.py
+-rw-r--r--   0     1001      123     5401 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/tests/unit/operations/test_with_columns.py
+-rw-r--r--   0     1001      123        0 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/tests/unit/streaming/__init__.py
+-rw-r--r--   0     1001      123      196 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/tests/unit/streaming/conftest.py
+-rw-r--r--   0     1001      123      908 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/tests/unit/streaming/test_ooc.py
+-rw-r--r--   0     1001      123    16944 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/tests/unit/streaming/test_streaming.py
+-rw-r--r--   0     1001      123     4775 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/tests/unit/test_api.py
+-rw-r--r--   0     1001      123     1969 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/tests/unit/test_arity.py
+-rw-r--r--   0     1001      123    20333 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/tests/unit/test_cfg.py
+-rw-r--r--   0     1001      123    42513 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/tests/unit/test_constructors.py
+-rw-r--r--   0     1001      123      454 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/tests/unit/test_context.py
+-rw-r--r--   0     1001      123     1628 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/tests/unit/test_cse.py
+-rw-r--r--   0     1001      123     5198 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/tests/unit/test_datatypes.py
+-rw-r--r--   0     1001      123   119414 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/tests/unit/test_df.py
+-rw-r--r--   0     1001      123     2396 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/tests/unit/test_empty.py
+-rw-r--r--   0     1001      123    18809 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/tests/unit/test_errors.py
+-rw-r--r--   0     1001      123     2741 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/tests/unit/test_expr_multi_cols.py
+-rw-r--r--   0     1001      123    34736 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/tests/unit/test_exprs.py
+-rw-r--r--   0     1001      123     3516 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/tests/unit/test_fmt.py
+-rw-r--r--   0     1001      123     3763 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/tests/unit/test_interchange.py
+-rw-r--r--   0     1001      123    38286 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/tests/unit/test_interop.py
+-rw-r--r--   0     1001      123    47730 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/tests/unit/test_lazy.py
+-rw-r--r--   0     1001      123     2463 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/tests/unit/test_polars_import.py
+-rw-r--r--   0     1001      123     4610 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/tests/unit/test_predicates.py
+-rw-r--r--   0     1001      123     7073 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/tests/unit/test_projections.py
+-rw-r--r--   0     1001      123    11551 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/tests/unit/test_queries.py
+-rw-r--r--   0     1001      123     4743 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/tests/unit/test_rows.py
+-rw-r--r--   0     1001      123    13987 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/tests/unit/test_schema.py
+-rw-r--r--   0     1001      123     7419 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/tests/unit/test_selectors.py
+-rw-r--r--   0     1001      123     2823 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/tests/unit/test_serde.py
+-rw-r--r--   0     1001      123    83729 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/tests/unit/test_series.py
+-rw-r--r--   0     1001      123      657 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/tests/unit/test_single.py
+-rw-r--r--   0     1001      123    10068 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/tests/unit/test_sql.py
+-rw-r--r--   0     1001      123    35314 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/tests/unit/test_testing.py
+-rw-r--r--   0     1001      123       41 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/tests/unit/utils/__init__.py
+-rw-r--r--   0     1001      123      306 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/tests/unit/utils/test_build_info.py
+-rw-r--r--   0     1001      123     2784 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/tests/unit/utils/test_parse_expr_input.py
+-rw-r--r--   0     1001      123      247 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/tests/unit/utils/test_show_versions.py
+-rw-r--r--   0     1001      123     5026 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/tests/unit/utils/test_utils.py
+-rw-r--r--   0     1001      123    63894 2023-06-16 12:30:56.000000 polars_lts_cpu-0.18.3/Cargo.lock
+-rw-r--r--   0        0        0    14545 1970-01-01 00:00:00.000000 polars_lts_cpu-0.18.3/PKG-INFO
```

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/Cargo.toml` & `polars_lts_cpu-0.18.3/local_dependencies/polars-pipe/Cargo.toml`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/LICENSE` & `polars_lts_cpu-0.18.3/local_dependencies/polars-row/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/operators/filter.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-pipe/src/executors/operators/filter.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/operators/function.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-pipe/src/executors/operators/function.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/operators/pass.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-pipe/src/executors/operators/pass.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/operators/placeholder.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-pipe/src/executors/operators/placeholder.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/operators/projection.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-pipe/src/executors/operators/projection.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/operators/reproject.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-pipe/src/executors/operators/reproject.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sinks/file_sink.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-pipe/src/executors/sinks/file_sink.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/convert.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/convert.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/count.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/count.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/first.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/first.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/interface.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/interface.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/last.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/last.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/mean.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/mean.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/min_max.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/min_max.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/null.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/null.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/sum.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/sum.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/global.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/global.rs`

 * *Files 2% similar despite different names*

```diff
@@ -127,42 +127,40 @@
     }
 
     fn process_partition_impl(
         &self,
         hash_map: &mut AggHashTable<false>,
         hashes: &[u64],
         chunk_indexes: &[IdxSize],
-        keys: &[Series],
+        keys: &BinaryArray<i64>,
         agg_cols: &[Series],
     ) {
         debug_assert_eq!(hashes.len(), chunk_indexes.len());
-        debug_assert_eq!(hashes.len(), keys[0].len());
+        debug_assert_eq!(hashes.len(), keys.len());
 
-        let mut keys_iters = keys.iter().map(|s| s.phys_iter()).collect::<Vec<_>>();
+        // let mut keys_iters = keys.iter().map(|s| s.phys_iter()).collect::<Vec<_>>();
         let mut agg_cols_iters = agg_cols.iter().map(|s| s.phys_iter()).collect::<Vec<_>>();
 
         // amortize loop counter
-        for i in 0..hashes.len() {
+        for (i, row) in keys.values_iter().enumerate() {
             unsafe {
                 let hash = *hashes.get_unchecked(i);
                 let chunk_index = *chunk_indexes.get_unchecked(i);
 
                 // safety: keys_iters and cols_iters are not depleted
-                let out = hash_map.insert(hash, &mut keys_iters, &mut agg_cols_iters, chunk_index);
+                let overflow = hash_map.insert(hash, row, &mut agg_cols_iters, chunk_index);
                 // should never overflow
-                debug_assert!(out.is_none());
+                debug_assert!(!overflow);
             }
         }
     }
 
     pub(super) fn process_partition_from_dumped(&self, partition: usize, spilled: &DataFrame) {
         let mut hash_map = self.inner_maps[partition].lock().unwrap();
-        let (hashes, chunk_indexes, keys_and_aggs) = SpillPayload::spilled_to_columns(spilled);
-        let keys = &keys_and_aggs[..hash_map.num_keys];
-        let aggs = &keys_and_aggs[hash_map.num_keys..];
+        let (hashes, chunk_indexes, keys, aggs) = SpillPayload::spilled_to_columns(spilled);
         self.process_partition_impl(&mut hash_map, hashes, chunk_indexes, keys, aggs);
     }
 
     fn process_partition(&self, partition: usize) {
         if let Some(bucket) = self.spill_partitions.drain_partition(partition, 0) {
             let mut hash_map = self.inner_maps[partition].lock().unwrap();
```

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/hash_table.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/hash_table.rs`

 * *Files 20% similar despite different names*

```diff
@@ -1,28 +1,23 @@
-use std::cell::UnsafeCell;
-
 use polars_arrow::trusted_len::PushUnchecked;
 use polars_core::hashing::partition::this_partition;
 
 use super::*;
 use crate::pipeline::PARTITION_SIZE;
 
 pub(super) struct AggHashTable<const FIXED: bool> {
-    inner_map: PlIdHashMap<Key, IdxSize>,
-    keys: Vec<AnyValue<'static>>,
+    inner_map: PlIdHashMap<Key, u32>,
+    // row data of the keys
+    keys: Vec<u8>,
     // the aggregation that are in process
     // the index the hashtable points to the start of the aggregations of that key/group
     running_aggregations: Vec<AggregateFunction>,
     // n aggregation function constructors
     // The are used to create new running aggregators
     agg_constructors: Arc<[AggregateFunction]>,
-    // amortize alloc
-    // lifetime is tied to self, so we use static
-    // to ensure bck to leave us be
-    keys_scratch: UnsafeCell<Vec<AnyValue<'static>>>,
     output_schema: SchemaRef,
     pub num_keys: usize,
     spill_size: usize,
 }
 
 impl<const FIXED: bool> AggHashTable<FIXED> {
     pub(super) fn new(
@@ -33,101 +28,63 @@
     ) -> Self {
         assert_eq!(FIXED, spill_size.is_some());
         Self {
             inner_map: Default::default(),
             keys: Default::default(),
             running_aggregations: Default::default(),
             agg_constructors,
-            keys_scratch: UnsafeCell::new(Vec::with_capacity(key_dtypes.len())),
             num_keys: key_dtypes.len(),
             spill_size: spill_size.unwrap_or(usize::MAX),
             output_schema,
         }
     }
 
     pub(super) fn split(&self) -> Self {
         Self {
             inner_map: Default::default(),
             keys: Default::default(),
             running_aggregations: Default::default(),
             agg_constructors: self.agg_constructors.iter().map(|c| c.split()).collect(),
-            keys_scratch: UnsafeCell::new(Vec::with_capacity(self.num_keys)),
             num_keys: self.num_keys,
             spill_size: self.spill_size,
             output_schema: self.output_schema.clone(),
         }
     }
 
-    unsafe fn get_keys(&self, idx: IdxSize) -> &[AnyValue] {
-        let start = idx as usize;
-        let end = start + self.num_keys;
+    unsafe fn get_keys_row(&self, key: &Key) -> &[u8] {
+        let start = key.offset as usize;
+        let end = start + key.len as usize;
         self.keys.get_unchecked(start..end)
     }
 
     pub(super) fn is_empty(&self) -> bool {
         self.inner_map.is_empty()
     }
 
-    fn get_entry(
-        &mut self,
-        hash: u64,
-        tuples: &[AnyValue],
-    ) -> RawEntryMut<Key, IdxSize, IdBuildHasher> {
+    fn get_entry(&mut self, hash: u64, row: &[u8]) -> RawEntryMut<Key, u32, IdBuildHasher> {
+        let keys = self.keys.as_ptr();
+
         self.inner_map
             .raw_entry_mut()
             .from_hash(hash, |hash_map_key| {
+                // first check the hash as that has no indirection
                 hash_map_key.hash == hash && {
-                    let idx = hash_map_key.idx as usize;
-                    if tuples.len() > 1 {
-                        tuples.iter().enumerate().all(|(i, key)| unsafe {
-                            self.keys.get_unchecked_release(i + idx) == key
-                        })
-                    } else {
-                        unsafe {
-                            self.keys.get_unchecked_release(idx) == tuples.get_unchecked_release(0)
-                        }
-                    }
+                    let offset = hash_map_key.offset as usize;
+                    let len = hash_map_key.len as usize;
+
+                    unsafe { std::slice::from_raw_parts(keys.add(offset), len) == row }
                 }
             })
     }
 
-    /// # Safety
-    /// Caller must ensure that `keys` and `agg_iters` are not depleted.
-    /// # Returns &keys
-    pub(super) unsafe fn insert<'a>(
-        &'a mut self,
-        hash: u64,
-        keys: &mut [SeriesPhysIter],
-        agg_iters: &mut [SeriesPhysIter],
-        chunk_index: IdxSize,
-    ) -> Option<&[AnyValue]> {
-        // safety: no references
-        let keys_scratch = unsafe { &mut *self.keys_scratch.get() };
-
-        unsafe {
-            // safety:
-            // this scratch is set with borrowed anyvalues, so we don't have to drop
-            // them as they only borrow data
-            keys_scratch.set_len(0);
-        }
-        for key in keys {
-            unsafe {
-                // safety: this function should never be called if iterator is depleted
-                let key = key.next().unwrap_unchecked_release();
-                // safety: the static is temporary, we will never access them outside of this function
-                let key = std::mem::transmute::<AnyValue<'_>, AnyValue<'static>>(key);
-                // safety: we amortized n_keys
-                keys_scratch.push_unchecked(key)
-            }
-        }
+    fn insert_key<'a>(&'a mut self, hash: u64, row: &[u8]) -> Option<u32> {
+        let entry = self.get_entry(hash, row);
 
-        let entry = self.get_entry(hash, keys_scratch);
-
-        let agg_idx = match entry {
-            RawEntryMut::Occupied(entry) => *entry.get(),
+        match entry {
+            RawEntryMut::Occupied(entry) => Some(*entry.get()),
             RawEntryMut::Vacant(entry) => {
                 // bchk shenanigans:
                 // it does not allow us to hold a `raw entry` and in the meantime
                 // have &self access to get the length of keys
                 // so we work with pointers instead
                 let borrow = &entry;
                 let borrow = borrow as *const RawVacantEntryMut<_, _, _> as usize;
@@ -136,55 +93,67 @@
                 std::mem::forget(entry);
 
                 // OVERFLOW logic
                 if FIXED && self.inner_map.len() > self.spill_size {
                     unsafe {
                         // take a hold of the entry again and ensure it gets dropped
                         let borrow =
-                            borrow as *const RawVacantEntryMut<'a, Key, IdxSize, IdBuildHasher>;
+                            borrow as *const RawVacantEntryMut<'a, Key, u32, IdBuildHasher>;
                         let _entry = std::ptr::read(borrow);
                     }
-                    return Some(keys_scratch);
+                    return None;
                 }
 
-                let aggregation_idx = self.running_aggregations.len() as IdxSize;
-                let key_idx = self.keys.len() as IdxSize;
+                let aggregation_idx = self.running_aggregations.len() as u32;
+                let key_offset = self.keys.len() as u32;
+                let key_len = row.len() as u32;
+                let key = Key::new(hash, key_offset, key_len);
 
-                let key = Key::new(hash, key_idx);
                 unsafe {
                     // take a hold of the entry again and ensure it gets dropped
-                    let borrow =
-                        borrow as *const RawVacantEntryMut<'a, Key, IdxSize, IdBuildHasher>;
+                    let borrow = borrow as *const RawVacantEntryMut<'a, Key, u32, IdBuildHasher>;
                     let entry = std::ptr::read(borrow);
                     entry.insert(key, aggregation_idx);
                 }
 
                 for agg in self.agg_constructors.as_ref() {
                     self.running_aggregations.push(agg.split())
                 }
 
-                unsafe {
-                    self.keys.extend(
-                        keys_scratch
-                            .iter()
-                            .map(|av| av.clone().into_static().unwrap_unchecked_release()),
-                    );
-                }
-                aggregation_idx
+                self.keys.extend_from_slice(row);
+                Some(aggregation_idx)
             }
+        }
+    }
+
+    /// # Safety
+    /// Caller must ensure that `keys` and `agg_iters` are not depleted.
+    /// # Returns &keys
+    pub(super) unsafe fn insert(
+        &mut self,
+        hash: u64,
+        row: &[u8],
+        agg_iters: &mut [SeriesPhysIter],
+        chunk_index: IdxSize,
+    ) -> bool {
+        let agg_idx = match self.insert_key(hash, row) {
+            // overflow
+            None => return true,
+            Some(agg_idx) => agg_idx,
         };
 
         // apply the aggregation
         for (i, agg_iter) in agg_iters.iter_mut().enumerate() {
             let i = agg_idx as usize + i;
             let agg_fn = unsafe { self.running_aggregations.get_unchecked_release_mut(i) };
 
             agg_fn.pre_agg(chunk_index, agg_iter.as_mut())
         }
-        None
+        // no overflow
+        false
     }
 
     pub(super) fn combine(&mut self, other: &mut Self) {
         self.combine_impl(other, |_hash| true)
     }
 
     pub(super) fn combine_on_partition<const FIXED_OTHER: bool>(
@@ -203,59 +172,25 @@
         other: &mut AggHashTable<FIXED_OTHER>,
         on_condition: C,
     )
     // takes a hash and if true, this keys will be combined
     where
         C: Fn(u64) -> bool,
     {
+        let spill_size = self.spill_size;
+        self.spill_size = usize::MAX;
         for (key_other, agg_idx_other) in other.inner_map.iter() {
             // safety: idx is from the hashmap, so is in bounds
-            let keys = unsafe { other.get_keys(key_other.idx) };
+            let row = unsafe { other.get_keys_row(key_other) };
 
             if on_condition(key_other.hash) {
-                let entry = self.get_entry(key_other.hash, keys);
-                let agg_idx_self = match entry {
-                    RawEntryMut::Occupied(entry) => *entry.get(),
-                    RawEntryMut::Vacant(entry) => {
-                        let borrow = &entry;
-                        let borrow = borrow as *const RawVacantEntryMut<_, _, _> as usize;
-                        // ensure the bck forgets this guy
-                        #[allow(clippy::forget_non_drop)]
-                        std::mem::forget(entry);
-
-                        let key_idx = self.keys.len() as IdxSize;
-                        let aggregation_idx = self.running_aggregations.len() as IdxSize;
-
-                        let key = Key::new(key_other.hash, key_idx);
-                        for agg in self.agg_constructors.as_ref() {
-                            self.running_aggregations.push(agg.split())
-                        }
-
-                        // take a hold of the entry again and ensure it gets dropped
-                        unsafe {
-                            let borrow =
-                                borrow as *const RawVacantEntryMut<'_, Key, IdxSize, IdBuildHasher>;
-                            let entry = std::ptr::read(borrow);
-                            entry.insert(key, aggregation_idx);
-                        }
-                        // update the keys
-                        unsafe {
-                            let start = key_other.idx as usize;
-                            let end = start + self.num_keys;
-                            let keys = other.keys.get_unchecked_release_mut(start..end);
-
-                            for key in keys {
-                                let mut owned_key = AnyValue::Null;
-                                // this prevents cloning a string
-                                std::mem::swap(&mut owned_key, key);
-                                self.keys.push(owned_key)
-                            }
-                        }
-                        aggregation_idx
-                    }
+                // safety: will not overflow as we set it to usize::MAX;
+                let agg_idx_self = unsafe {
+                    self.insert_key(key_other.hash, row)
+                        .unwrap_unchecked_release()
                 };
                 let start = *agg_idx_other as usize;
                 let end = start + self.agg_constructors.len();
                 let aggs_other =
                     unsafe { other.running_aggregations.get_unchecked_release(start..end) };
                 let start = agg_idx_self as usize;
                 let end = start + self.agg_constructors.len();
@@ -269,14 +204,15 @@
                         let other = aggs_other.get_unchecked_release(i);
                         // TODO!: try transmutes
                         agg_self.combine(other.as_any())
                     }
                 }
             }
         }
+        self.spill_size = spill_size;
     }
 
     pub(super) fn finalize(&mut self, slice: &mut Option<(i64, usize)>) -> DataFrame {
         let local_len = self.inner_map.len();
         let (skip_len, take_len) = if let Some((offset, slice_len)) = slice {
             if *offset as usize >= local_len {
                 *offset -= local_len as i64;
@@ -287,64 +223,61 @@
                 *slice_len = slice_len.saturating_sub(local_len);
                 out
             }
         } else {
             (0, local_len)
         };
         let inner_map = std::mem::take(&mut self.inner_map);
-
-        let mut key_builders = self
-            .output_schema
-            .iter_dtypes()
-            .take(self.num_keys)
-            .map(|dtype| AnyValueBufferTrusted::new(&dtype.to_physical(), take_len))
-            .collect::<Vec<_>>();
+        let mut running_aggregations = std::mem::take(&mut self.running_aggregations);
 
         let mut agg_builders = self
             .agg_constructors
             .iter()
             .map(|ac| AnyValueBufferTrusted::new(&ac.dtype(), take_len))
             .collect::<Vec<_>>();
         let num_aggs = self.agg_constructors.len();
+        let mut key_rows = Vec::with_capacity(take_len);
 
         inner_map
             .into_iter()
             .skip(skip_len)
             .take(take_len)
             .for_each(|(k, agg_offset)| {
-                let keys_offset = k.idx as usize;
-                let keys = unsafe {
-                    self.keys
-                        .get_unchecked_release(keys_offset..keys_offset + self.num_keys)
-                };
-
-                // amortize loop counter
-                for i in 0..self.num_keys {
-                    unsafe {
-                        let key = keys.get_unchecked_release(i);
-                        let key_builder = key_builders.get_unchecked_release_mut(i);
-                        // safety: we own the keys
-                        key_builder.add_unchecked_owned_physical(key);
-                    }
+                unsafe {
+                    key_rows.push_unchecked(self.get_keys_row(&k));
                 }
 
                 let start = agg_offset as usize;
                 let end = start + num_aggs;
                 for (i, buffer) in (start..end).zip(agg_builders.iter_mut()) {
                     unsafe {
-                        let running_agg = self.running_aggregations.get_unchecked_release_mut(i);
+                        let running_agg = running_aggregations.get_unchecked_release_mut(i);
                         let av = running_agg.finalize();
                         // safety: finalize creates owned anyvalues
                         buffer.add_unchecked_owned_physical(&av);
                     }
                 }
             });
 
+        let key_dtypes = self
+            .output_schema
+            .iter_dtypes()
+            .take(self.num_keys)
+            .map(|dtype| dtype.to_physical().to_arrow())
+            .collect::<Vec<_>>();
+        let fields = vec![Default::default(); self.num_keys];
+        let key_columns =
+            unsafe { polars_row::decode::decode_rows(&mut key_rows, &fields, &key_dtypes) };
+
         let mut cols = Vec::with_capacity(self.num_keys + self.agg_constructors.len());
-        cols.extend(key_builders.into_iter().map(|buf| buf.into_series()));
+        cols.extend(
+            key_columns
+                .into_iter()
+                .map(|arr| Series::try_from(("", arr)).unwrap()),
+        );
         cols.extend(agg_builders.into_iter().map(|buf| buf.into_series()));
         physical_agg_to_logical(&mut cols, &self.output_schema);
         DataFrame::new_no_checks(cols)
     }
 }
 
 unsafe impl<const FIXED: bool> Send for AggHashTable<FIXED> {}
```

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/mod.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/mod.rs`

 * *Files 18% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 use std::any::Any;
 use std::hash::{Hash, Hasher};
 use std::sync::Mutex;
 
 use eval::Eval;
 use hash_table::AggHashTable;
 use hashbrown::hash_map::{RawEntryMut, RawVacantEntryMut};
+use polars_arrow::export::arrow::array::BinaryArray;
 use polars_core::frame::row::AnyValueBufferTrusted;
 use polars_core::series::SeriesPhysIter;
 use polars_core::IdBuildHasher;
 use polars_utils::hash_to_partition;
 use polars_utils::slice::GetSaferUnchecked;
 use polars_utils::unwrap::UnwrapUncheckedRelease;
 pub(crate) use sink::GenericGroupby2;
@@ -30,83 +31,93 @@
 type PartitionVec<T> = Vec<T>;
 type IOThreadRef = Arc<Mutex<Option<IOThread>>>;
 
 #[derive(Clone)]
 struct SpillPayload {
     hashes: Vec<u64>,
     chunk_idx: Vec<IdxSize>,
-    keys_and_aggs: Vec<Series>,
-    num_keys: usize,
+    keys: BinaryArray<i64>,
+    aggs: Vec<Series>,
 }
 
 static HASH_COL: &str = "__POLARS_h";
 static INDEX_COL: &str = "__POLARS_idx";
+static KEYS_COL: &str = "__POLARS_keys";
 
 impl SpillPayload {
     fn hashes(&self) -> &[u64] {
         &self.hashes
     }
 
-    fn keys(&self) -> &[Series] {
-        &self.keys_and_aggs[..self.num_keys]
+    fn keys(&self) -> &BinaryArray<i64> {
+        &self.keys
     }
 
     fn cols(&self) -> &[Series] {
-        &self.keys_and_aggs[self.num_keys..]
+        &self.aggs
     }
 
     fn chunk_index(&self) -> &[IdxSize] {
         &self.chunk_idx
     }
 
     fn get_schema(&self) -> Schema {
-        let mut schema = Schema::with_capacity(self.keys_and_aggs.len() + 2);
+        let mut schema = Schema::with_capacity(self.aggs.len() + 2);
         schema.with_column(HASH_COL.into(), DataType::UInt64);
         schema.with_column(INDEX_COL.into(), IDX_DTYPE);
-        for s in &self.keys_and_aggs {
+        schema.with_column(KEYS_COL.into(), DataType::Binary);
+        for s in &self.aggs {
             schema.with_column(s.name().into(), s.dtype().clone());
         }
         schema
     }
 
     fn into_df(self) -> DataFrame {
         debug_assert_eq!(self.hashes.len(), self.chunk_idx.len());
-        debug_assert_eq!(self.hashes.len(), self.keys_and_aggs[0].len());
+        debug_assert_eq!(self.hashes.len(), self.keys.len());
 
         let hashes = UInt64Chunked::from_vec(HASH_COL, self.hashes).into_series();
         let chunk_idx = IdxCa::from_vec(INDEX_COL, self.chunk_idx).into_series();
-        let mut cols = Vec::with_capacity(self.keys_and_aggs.len() + 2);
+        let keys = Series::try_from((KEYS_COL, Box::new(self.keys) as ArrayRef)).unwrap();
+
+        let mut cols = Vec::with_capacity(self.aggs.len() + 3);
         cols.push(hashes);
         cols.push(chunk_idx);
-        cols.extend(self.keys_and_aggs);
+        cols.push(keys);
+        cols.extend(self.aggs);
         DataFrame::new_no_checks(cols)
     }
 
-    fn spilled_to_columns(spilled: &DataFrame) -> (&[u64], &[IdxSize], &[Series]) {
+    fn spilled_to_columns(
+        spilled: &DataFrame,
+    ) -> (&[u64], &[IdxSize], &BinaryArray<i64>, &[Series]) {
         let cols = spilled.get_columns();
         let hashes = cols[0].u64().unwrap();
         let hashes = hashes.cont_slice().unwrap();
         let chunk_indexes = cols[1].idx().unwrap();
         let chunk_indexes = chunk_indexes.cont_slice().unwrap();
-        let keys_and_aggs = &cols[2..];
-        (hashes, chunk_indexes, keys_and_aggs)
+        let keys = cols[2].binary().unwrap();
+        let keys = keys.downcast_iter().next().unwrap();
+        let aggs = &cols[3..];
+        (hashes, chunk_indexes, keys, aggs)
     }
 }
 
 // This is the hash and the Index offset in the linear buffer
 #[derive(Copy, Clone)]
 pub(super) struct Key {
     pub(super) hash: u64,
-    pub(super) idx: IdxSize,
+    pub(super) offset: u32,
+    pub(super) len: u32,
 }
 
 impl Key {
     #[inline]
-    pub(super) fn new(hash: u64, idx: IdxSize) -> Self {
-        Self { hash, idx }
+    pub(super) fn new(hash: u64, offset: u32, len: u32) -> Self {
+        Self { hash, offset, len }
     }
 }
 
 impl Hash for Key {
     #[inline]
     fn hash<H: Hasher>(&self, state: &mut H) {
         state.write_u64(self.hash)
```

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/ooc_state.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/ooc_state.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/sink.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/sink.rs`

 * *Files 2% similar despite different names*

```diff
@@ -60,36 +60,35 @@
 impl Sink for GenericGroupby2 {
     fn sink(&mut self, context: &PExecutionContext, chunk: DataChunk) -> PolarsResult<SinkResult> {
         // load data and hashes
         unsafe {
             // safety: we don't hold mutable refs
             self.eval.evaluate_keys_aggs_and_hashes(context, &chunk)?;
         }
-        // safety: we don't hold mutable refs
-        let mut keys = unsafe { self.eval.get_keys_iters() };
+        // safety: eval is alive for the duration of keys
+        let keys = unsafe { self.eval.get_keys_iter() };
         // safety: we don't hold mutable refs
         let mut aggs = unsafe { self.eval.get_aggs_iters() };
 
         let chunk_idx = chunk.chunk_index;
         unsafe {
             // safety: the mutable borrows are not aliasing
             let table = &mut *self.thread_local_table.get();
 
-            for hash in self.eval.hashes() {
+            for (hash, row) in self.eval.hashes().iter().zip(keys.values_iter()) {
                 if let Some((partition, spill_payload)) =
-                    table.insert(*hash, &mut keys, &mut aggs, chunk_idx)
+                    table.insert(*hash, row, &mut aggs, chunk_idx)
                 {
                     self.global_table.spill(partition, spill_payload)
                 }
             }
         }
 
         // clear memory
         unsafe {
-            drop(keys);
             drop(aggs);
             // safety: we don't hold mutable refs, we just dropped them
             self.eval.clear()
         };
 
         // indicates if we should early merge a partition
         // other scenario could be that we must spill to disk
```

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/source.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/source.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/thread_local.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/thread_local.rs`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 use once_cell::sync::Lazy;
+use polars_arrow::export::arrow::array::MutableBinaryArray;
 use polars_core::export::once_cell;
 
 use super::*;
 use crate::pipeline::PARTITION_SIZE;
 
 const OB_SIZE: usize = 2048;
 
@@ -12,18 +13,18 @@
         .unwrap_or(10_000)
 });
 
 #[derive(Clone)]
 struct SpillPartitions {
     // outer vec: partitions (factor of 2)
     // inner vec: number of keys + number of aggregated columns
-    keys_aggs_partitioned: PartitionVec<Vec<AnyValueBufferTrusted<'static>>>,
+    keys_partitioned: PartitionVec<MutableBinaryArray<i64>>,
+    aggs_partitioned: PartitionVec<Vec<AnyValueBufferTrusted<'static>>>,
     hash_partitioned: PartitionVec<Vec<u64>>,
     chunk_index_partitioned: PartitionVec<Vec<IdxSize>>,
-    num_keys: usize,
     spilled: bool,
     // this only fills during the reduce phase IFF
     // there are spilled tuples
     finished_payloads: PartitionVec<Vec<SpillPayload>>,
     keys_dtypes: Arc<[DataType]>,
     agg_dtypes: Arc<[DataType]>,
     output_schema: SchemaRef,
@@ -32,145 +33,115 @@
 impl SpillPartitions {
     fn new(keys: Arc<[DataType]>, aggs: Arc<[DataType]>, output_schema: SchemaRef) -> Self {
         let hash_partitioned = vec![];
         let chunk_index_partitioned = vec![];
 
         // construct via split so that pre-allocation succeeds
         Self {
-            keys_aggs_partitioned: vec![],
+            keys_partitioned: vec![],
+            aggs_partitioned: vec![],
             hash_partitioned,
             chunk_index_partitioned,
-            num_keys: keys.as_ref().len(),
             spilled: false,
             finished_payloads: vec![],
             keys_dtypes: keys,
             agg_dtypes: aggs,
             output_schema,
         }
         .split()
     }
 
     fn split(&self) -> Self {
-        let n_columns = self.keys_dtypes.as_ref().len() + self.agg_dtypes.as_ref().len();
+        let n_columns = self.agg_dtypes.as_ref().len();
 
-        let keys_aggs_partitioned = (0..PARTITION_SIZE)
+        let aggs_partitioned = (0..PARTITION_SIZE)
             .map(|_| {
                 let mut buf = Vec::with_capacity(n_columns);
-                for dtype in self.keys_dtypes.as_ref() {
-                    let builder = AnyValueBufferTrusted::new(&dtype.to_physical(), OB_SIZE);
-                    buf.push(builder);
-                }
                 for dtype in self.agg_dtypes.as_ref() {
                     let builder = AnyValueBufferTrusted::new(&dtype.to_physical(), OB_SIZE);
                     buf.push(builder);
                 }
                 buf
             })
             .collect();
 
+        let keys_partitioned = (0..PARTITION_SIZE)
+            .map(|_| MutableBinaryArray::with_capacity(OB_SIZE))
+            .collect();
+
         let hash_partitioned = vec![Vec::with_capacity(OB_SIZE); PARTITION_SIZE];
         let chunk_index_partitioned = vec![Vec::with_capacity(OB_SIZE); PARTITION_SIZE];
 
         Self {
-            keys_aggs_partitioned,
+            keys_partitioned,
+            aggs_partitioned,
             hash_partitioned,
             chunk_index_partitioned,
-            num_keys: self.num_keys,
             spilled: false,
             finished_payloads: vec![],
             keys_dtypes: self.keys_dtypes.clone(),
             agg_dtypes: self.agg_dtypes.clone(),
             output_schema: self.output_schema.clone(),
         }
     }
 }
 
 impl SpillPartitions {
-    fn pre_alloc(&mut self) {
-        if !self.spilled {
-            let n_columns = self.keys_dtypes.as_ref().len() + self.agg_dtypes.as_ref().len();
-
-            self.keys_aggs_partitioned = (0..PARTITION_SIZE)
-                .map(|_| {
-                    let mut buf = Vec::with_capacity(n_columns);
-                    for dtype in self.keys_dtypes.as_ref() {
-                        let builder = AnyValueBufferTrusted::new(&dtype.to_physical(), OB_SIZE);
-                        buf.push(builder);
-                    }
-                    for dtype in self.agg_dtypes.as_ref() {
-                        let builder = AnyValueBufferTrusted::new(&dtype.to_physical(), OB_SIZE);
-                        buf.push(builder);
-                    }
-                    buf
-                })
-                .collect();
-
-            self.hash_partitioned = vec![Vec::with_capacity(OB_SIZE); PARTITION_SIZE];
-            self.chunk_index_partitioned = vec![Vec::with_capacity(OB_SIZE); PARTITION_SIZE];
-        }
-    }
     /// Returns (partition, overflowing hashes, chunk_indexes, keys and aggs)
     fn insert(
         &mut self,
         hash: u64,
         chunk_idx: IdxSize,
-        keys: &[AnyValue<'_>],
-        aggs: &mut [SeriesPhysIter],
+        row: &[u8],
+        agg_iters: &mut [SeriesPhysIter],
     ) -> Option<(usize, SpillPayload)> {
-        self.pre_alloc();
-        let partition = hash_to_partition(hash, self.keys_aggs_partitioned.len());
+        let partition = hash_to_partition(hash, self.aggs_partitioned.len());
         self.spilled = true;
         unsafe {
-            let keys_aggs = self
-                .keys_aggs_partitioned
-                .get_unchecked_release_mut(partition);
+            let agg_values = self.aggs_partitioned.get_unchecked_release_mut(partition);
             let hashes = self.hash_partitioned.get_unchecked_release_mut(partition);
             let chunk_indexes = self
                 .chunk_index_partitioned
                 .get_unchecked_release_mut(partition);
+            let key_builder = self.keys_partitioned.get_unchecked_mut(partition);
 
             hashes.push(hash);
             chunk_indexes.push(chunk_idx);
 
             // amortize the loop counter
-            for i in 0..keys.len() {
-                let av = keys.get_unchecked(i);
-                let buf = keys_aggs.get_unchecked_mut(i);
-                // safety: we can trust the input types to be of consistent dtype
-                buf.add_unchecked_borrowed_physical(av);
-            }
-            let mut i = keys.len();
-            for agg in aggs {
+            key_builder.push(Some(row));
+            for (i, agg) in agg_iters.iter_mut().enumerate() {
                 let av = agg.next().unwrap_unchecked_release();
-                let buf = keys_aggs.get_unchecked_mut(i);
+                let buf = agg_values.get_unchecked_mut(i);
                 buf.add_unchecked_borrowed_physical(&av);
-                i += 1;
             }
 
             if hashes.len() >= OB_SIZE {
                 let mut new_hashes = Vec::with_capacity(OB_SIZE);
                 let mut new_chunk_indexes = Vec::with_capacity(OB_SIZE);
+                let mut new_keys_builder = MutableBinaryArray::with_capacity(OB_SIZE);
                 std::mem::swap(&mut new_hashes, hashes);
                 std::mem::swap(&mut new_chunk_indexes, chunk_indexes);
+                std::mem::swap(&mut new_keys_builder, key_builder);
 
                 Some((
                     partition,
                     SpillPayload {
                         hashes: new_hashes,
                         chunk_idx: new_chunk_indexes,
-                        keys_and_aggs: keys_aggs
+                        keys: new_keys_builder.into(),
+                        aggs: agg_values
                             .iter_mut()
                             .zip(self.output_schema.iter_names())
                             .map(|(b, name)| {
                                 let mut s = b.reset(OB_SIZE);
                                 s.rename(name);
                                 s
                             })
                             .collect(),
-                        num_keys: self.num_keys,
                     },
                 ))
             } else {
                 None
             }
         }
     }
@@ -219,31 +190,31 @@
             for payload in payloads {
                 flattened.push((part, payload))
             }
         }
 
         (0..PARTITION_SIZE)
             .map(|partition| unsafe {
-                let keys_aggs = self
-                    .keys_aggs_partitioned
-                    .get_unchecked_release_mut(partition);
+                let spilled_aggs = self.aggs_partitioned.get_unchecked_release_mut(partition);
                 let hashes = self.hash_partitioned.get_unchecked_release_mut(partition);
                 let chunk_indexes = self
                     .chunk_index_partitioned
                     .get_unchecked_release_mut(partition);
+                let keys_builder =
+                    std::mem::take(self.keys_partitioned.get_unchecked_mut(partition));
                 let hashes = std::mem::take(hashes);
                 let chunk_idx = std::mem::take(chunk_indexes);
 
                 (
                     partition,
                     SpillPayload {
                         hashes,
                         chunk_idx,
-                        keys_and_aggs: keys_aggs.iter_mut().map(|b| b.reset(0)).collect(),
-                        num_keys: self.num_keys,
+                        keys: keys_builder.into(),
+                        aggs: spilled_aggs.iter_mut().map(|b| b.reset(0)).collect(),
                     },
                 )
             })
             .chain(flattened.into_iter())
     }
 }
 
@@ -285,24 +256,28 @@
 
     pub(super) fn get_inner_map_mut(&mut self) -> &mut AggHashTable<true> {
         &mut self.inner_map
     }
 
     /// # Safety
     /// Caller must ensure that `keys` and `agg_iters` are not depleted.
+    #[inline]
     pub(super) unsafe fn insert(
         &mut self,
         hash: u64,
-        keys: &mut [SeriesPhysIter],
+        keys_row: &[u8],
         agg_iters: &mut [SeriesPhysIter],
         chunk_index: IdxSize,
     ) -> Option<(usize, SpillPayload)> {
-        if let Some(keys) = self.inner_map.insert(hash, keys, agg_iters, chunk_index) {
+        if self
+            .inner_map
+            .insert(hash, keys_row, agg_iters, chunk_index)
+        {
             self.spill_partitions
-                .insert(hash, chunk_index, keys, agg_iters)
+                .insert(hash, chunk_index, keys_row, agg_iters)
         } else {
             None
         }
     }
 
     pub(super) fn combine(&mut self, other: &mut Self) {
         self.inner_map.combine(&mut other.inner_map);
```

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sinks/groupby/mod.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-pipe/src/executors/sinks/groupby/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sinks/groupby/ooc.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-pipe/src/executors/sinks/groupby/ooc.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sinks/groupby/ooc_state.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-pipe/src/executors/sinks/groupby/ooc_state.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sinks/groupby/primitive/mod.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-pipe/src/executors/sinks/groupby/primitive/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sinks/groupby/string.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-pipe/src/executors/sinks/groupby/string.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 use std::any::Any;
+use std::hash::{Hash, Hasher};
 use std::sync::Mutex;
 
 use hashbrown::hash_map::RawEntryMut;
 use num_traits::NumCast;
 use polars_core::export::ahash::RandomState;
 use polars_core::frame::row::AnyValueBuffer;
 use polars_core::prelude::*;
@@ -10,26 +11,46 @@
 use polars_core::{IdBuildHasher, POOL};
 use polars_utils::hash_to_partition;
 use polars_utils::slice::GetSaferUnchecked;
 use polars_utils::unwrap::UnwrapUncheckedRelease;
 use rayon::prelude::*;
 
 use super::aggregates::AggregateFn;
-use super::generic::Key;
 use crate::executors::sinks::groupby::aggregates::AggregateFunction;
 use crate::executors::sinks::groupby::ooc_state::OocState;
 use crate::executors::sinks::groupby::physical_agg_to_logical;
 use crate::executors::sinks::groupby::primitive::apply_aggregation;
 use crate::executors::sinks::groupby::utils::{compute_slices, finalize_groupby};
 use crate::executors::sinks::io::IOThread;
 use crate::executors::sinks::utils::load_vec;
 use crate::executors::sinks::HASHMAP_INIT_SIZE;
 use crate::expressions::PhysicalPipedExpr;
 use crate::operators::{DataChunk, FinalizedSink, PExecutionContext, Sink, SinkResult};
 
+// This is the hash and the Index offset in the linear buffer
+#[derive(Copy, Clone)]
+struct Key {
+    pub(super) hash: u64,
+    pub(super) idx: IdxSize,
+}
+
+impl Key {
+    #[inline]
+    pub(super) fn new(hash: u64, idx: IdxSize) -> Self {
+        Self { hash, idx }
+    }
+}
+
+impl Hash for Key {
+    #[inline]
+    fn hash<H: Hasher>(&self, state: &mut H) {
+        state.write_u64(self.hash)
+    }
+}
+
 // we store a hashmap per partition (partitioned by hash)
 // the hashmap contains indexes as keys and as values
 // those indexes point into the keys buffer and the values buffer
 // the keys buffer are buffers of AnyValue per partition
 // and the values are buffer of Aggregation functions per partition
 pub struct Utf8GroupbySink {
     thread_no: usize,
```

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sinks/groupby/utils.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-pipe/src/executors/sinks/groupby/utils.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sinks/io.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-pipe/src/executors/sinks/io.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sinks/joins/cross.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-pipe/src/executors/sinks/joins/cross.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sinks/joins/generic_build.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-pipe/src/executors/sinks/joins/generic_build.rs`

 * *Files 16% similar despite different names*

```diff
@@ -1,42 +1,41 @@
 use std::any::Any;
 use std::hash::{Hash, Hasher};
 use std::sync::Arc;
 
 use hashbrown::hash_map::RawEntryMut;
-use polars_arrow::trusted_len::PushUnchecked;
+use polars_arrow::export::arrow::array::BinaryArray;
 use polars_core::error::PolarsResult;
 use polars_core::export::ahash::RandomState;
 use polars_core::frame::hash_join::ChunkId;
 use polars_core::prelude::*;
 use polars_core::utils::{_set_partition_size, accumulate_dataframes_vertical_unchecked};
 use polars_utils::hash_to_partition;
 use polars_utils::slice::GetSaferUnchecked;
-use polars_utils::unwrap::UnwrapUncheckedRelease;
 
 use crate::executors::sinks::joins::inner_left::GenericJoinProbe;
-use crate::executors::sinks::utils::{hash_series, load_vec};
+use crate::executors::sinks::utils::{hash_rows, load_vec};
 use crate::executors::sinks::HASHMAP_INIT_SIZE;
 use crate::expressions::PhysicalPipedExpr;
 use crate::operators::{DataChunk, FinalizedSink, PExecutionContext, Sink, SinkResult};
 
 pub(super) type ChunkIdx = IdxSize;
 pub(super) type DfIdx = IdxSize;
 
 // This is the hash and the Index offset in the chunks and the index offset in the dataframe
 #[derive(Copy, Clone, Debug)]
 pub(super) struct Key {
     pub(super) hash: u64,
-    chunk_idx: ChunkIdx,
-    df_idx: DfIdx,
+    chunk_idx: IdxSize,
+    df_idx: IdxSize,
 }
 
 impl Key {
     #[inline]
-    fn new(hash: u64, chunk_idx: ChunkIdx, df_idx: DfIdx) -> Self {
+    fn new(hash: u64, chunk_idx: IdxSize, df_idx: IdxSize) -> Self {
         Key {
             hash,
             chunk_idx,
             df_idx,
         }
     }
 }
@@ -53,27 +52,27 @@
     // the join columns are all tightly packed
     // the values of a join column(s) can be found
     // by:
     // first get the offset of the chunks and multiply that with the number of join
     // columns
     //      * chunk_offset = (idx * n_join_keys)
     //      * end = (offset + n_join_keys)
-    materialized_join_cols: Vec<ArrayRef>,
+    materialized_join_cols: Vec<BinaryArray<i64>>,
     suffix: Arc<str>,
     hb: RandomState,
     // partitioned tables that will be used for probing
     // stores the key and the chunk_idx, df_idx of the left table
     hash_tables: Vec<PlIdHashMap<Key, Vec<ChunkId>>>,
 
     // the columns that will be joined on
     join_columns_left: Arc<Vec<Arc<dyn PhysicalPipedExpr>>>,
     join_columns_right: Arc<Vec<Arc<dyn PhysicalPipedExpr>>>,
 
     // amortize allocations
-    join_series: Vec<Series>,
+    join_columns: Vec<ArrayRef>,
     hashes: Vec<u64>,
     join_type: JoinType,
     // the join order is swapped to ensure we hash the smaller table
     swapped: bool,
 }
 
 impl GenericBuild {
@@ -91,99 +90,77 @@
             chunks: vec![],
             join_type,
             suffix,
             hb,
             swapped,
             join_columns_left,
             join_columns_right,
-            join_series: vec![],
+            join_columns: vec![],
             materialized_join_cols: vec![],
             hash_tables,
             hashes: vec![],
         }
     }
 }
 
+#[inline]
 pub(super) fn compare_fn(
     key: &Key,
     h: u64,
-    join_columns_all_chunks: &[ArrayRef],
-    current_row: &[AnyValue],
-    n_join_cols: usize,
+    join_columns_all_chunks: &[BinaryArray<i64>],
+    current_row: &[u8],
 ) -> bool {
     let key_hash = key.hash;
 
     // we check the hash first
     // as that has no indirection
     key_hash == h && {
         // we get the appropriate values from the join columns and compare it with the current row
-        let chunk_idx = key.chunk_idx as usize * n_join_cols;
+        let chunk_idx = key.chunk_idx as usize;
         let df_idx = key.df_idx as usize;
 
         // get the right columns from the linearly packed buffer
-        let join_cols = unsafe {
-            join_columns_all_chunks.get_unchecked_release(chunk_idx..chunk_idx + n_join_cols)
+        let other_row = unsafe {
+            join_columns_all_chunks
+                .get_unchecked_release(chunk_idx)
+                .value_unchecked(df_idx)
         };
-
-        join_cols
-            .iter()
-            .zip(current_row)
-            .all(|(column, value)| unsafe { &column.get_unchecked(df_idx) == value })
+        current_row == other_row
     }
 }
 
 impl GenericBuild {
     fn is_empty(&self) -> bool {
         match self.chunks.len() {
             0 => true,
             1 => self.chunks[0].is_empty(),
             _ => false,
         }
     }
 
-    #[inline]
-    fn number_of_keys(&self) -> usize {
-        self.join_columns_left.len()
-    }
-
     fn set_join_series(
         &mut self,
         context: &PExecutionContext,
         chunk: &DataChunk,
-    ) -> PolarsResult<&[Series]> {
-        self.join_series.clear();
+    ) -> PolarsResult<&BinaryArray<i64>> {
+        self.join_columns.clear();
 
         for phys_e in self.join_columns_left.iter() {
             let s = phys_e.evaluate(chunk, context.execution_state.as_any())?;
-            let s = s.to_physical_repr();
-            let s = s.rechunk();
-            self.materialized_join_cols.push(s.array_ref(0).clone());
-            self.join_series.push(s);
+            let arr = s.to_physical_repr().rechunk().array_ref(0).clone();
+            self.join_columns.push(arr);
         }
-        Ok(&self.join_series)
+        let rows_encoded = polars_row::convert_columns_no_order(&self.join_columns).into_array();
+        self.materialized_join_cols.push(rows_encoded);
+        Ok(self.materialized_join_cols.last().unwrap())
     }
-    unsafe fn get_tuple<'a>(
-        &'a self,
-        chunk_idx: ChunkIdx,
-        df_idx: DfIdx,
-        buf: &mut Vec<AnyValue<'a>>,
-    ) {
-        buf.clear();
-        // get the right columns from the linearly packed buffer
-        let n_keys = self.number_of_keys();
-        let chunk_offset = chunk_idx as usize * n_keys;
-        let chunk_end = chunk_offset + n_keys;
-        let join_cols = self
-            .materialized_join_cols
-            .get_unchecked_release(chunk_offset..chunk_end);
-        buf.extend(
-            join_cols
-                .iter()
-                .map(|arr| arr.get_unchecked(df_idx as usize)),
-        )
+    unsafe fn get_row(&self, chunk_idx: ChunkIdx, df_idx: DfIdx) -> &[u8] {
+        self.materialized_join_cols
+            .get_unchecked_release(chunk_idx as usize)
+            .value_unchecked(df_idx as usize)
     }
 }
 
 impl Sink for GenericBuild {
     fn sink(&mut self, context: &PExecutionContext, chunk: DataChunk) -> PolarsResult<SinkResult> {
         // we do some juggling here so that we don't
         // end up with empty chunks
@@ -195,40 +172,29 @@
         if chunk.is_empty() {
             if self.chunks.is_empty() {
                 self.chunks.push(chunk)
             }
             return Ok(SinkResult::CanHaveMoreInput);
         }
         let mut hashes = std::mem::take(&mut self.hashes);
-        self.set_join_series(context, &chunk)?;
-        hash_series(&self.join_series, &mut hashes, &self.hb);
+        let rows = self.set_join_series(context, &chunk)?.clone();
+        hash_rows(&rows, &mut hashes, &self.hb);
         self.hashes = hashes;
 
         let current_chunk_offset = self.chunks.len() as ChunkIdx;
 
-        let mut keys_iter = KeysIter::new(&self.join_series);
-        let n_join_cols = self.number_of_keys();
-
         // row offset in the chunk belonging to the hash
         let mut current_df_idx = 0 as IdxSize;
-        for h in &self.hashes {
-            let current_tuple = unsafe { keys_iter.lend_next() };
-
-            // get the hashtable belonging by this hash partition
+        for (row, h) in rows.values_iter().zip(&self.hashes) {
+            // get the hashtable belonging to this hash partition
             let partition = hash_to_partition(*h, self.hash_tables.len());
             let current_table = unsafe { self.hash_tables.get_unchecked_release_mut(partition) };
 
             let entry = current_table.raw_entry_mut().from_hash(*h, |key| {
-                compare_fn(
-                    key,
-                    *h,
-                    &self.materialized_join_cols,
-                    current_tuple,
-                    n_join_cols,
-                )
+                compare_fn(key, *h, &self.materialized_join_cols, row)
             });
 
             let payload = [current_chunk_offset, current_df_idx];
             match entry {
                 RawEntryMut::Vacant(entry) => {
                     let key = Key::new(*h, current_chunk_offset, current_df_idx);
                     entry.insert(key, vec![payload]);
@@ -252,42 +218,33 @@
             }
             return;
         }
         let other = other.as_any().downcast_ref::<Self>().unwrap();
         if other.is_empty() {
             return;
         }
-        let mut tuple_buf = Vec::with_capacity(self.number_of_keys());
 
         let chunks_offset = self.chunks.len() as IdxSize;
         self.chunks.extend_from_slice(&other.chunks);
         self.materialized_join_cols
             .extend_from_slice(&other.materialized_join_cols);
 
         // we combine the other hashtable with ours, but we must offset the chunk_idx
         // values by the number of chunks we already got.
         self.hash_tables
             .iter_mut()
             .zip(&other.hash_tables)
             .for_each(|(ht, other_ht)| {
                 for (k, val) in other_ht.iter() {
                     // use the indexes to materialize the row
-                    for [chunk_idx, df_idx] in val {
-                        unsafe { other.get_tuple(*chunk_idx, *df_idx, &mut tuple_buf) };
-                    }
+                    let other_row = unsafe { other.get_row(k.chunk_idx, k.df_idx) };
 
                     let h = k.hash;
                     let entry = ht.raw_entry_mut().from_hash(h, |key| {
-                        compare_fn(
-                            key,
-                            h,
-                            &self.materialized_join_cols,
-                            &tuple_buf,
-                            tuple_buf.len(),
-                        )
+                        compare_fn(key, h, &self.materialized_join_cols, other_row)
                     });
 
                     match entry {
                         RawEntryMut::Vacant(entry) => {
                             let [chunk_idx, df_idx] = unsafe { val.get_unchecked_release(0) };
                             let new_chunk_idx = chunk_idx + chunks_offset;
                             let key = Key::new(h, new_chunk_idx, *df_idx);
@@ -340,15 +297,15 @@
                 let suffix = self.suffix.clone();
                 let hb = self.hb.clone();
                 let hash_tables = Arc::new(std::mem::take(&mut self.hash_tables));
                 let join_columns_left = self.join_columns_left.clone();
                 let join_columns_right = self.join_columns_right.clone();
 
                 // take the buffers, this saves one allocation
-                let mut join_series = std::mem::take(&mut self.join_series);
+                let mut join_series = std::mem::take(&mut self.join_columns);
                 join_series.clear();
                 let mut hashes = std::mem::take(&mut self.hashes);
                 hashes.clear();
 
                 let probe_operator = GenericJoinProbe::new(
                     left_df,
                     materialized_join_cols,
@@ -372,41 +329,7 @@
     fn as_any(&mut self) -> &mut dyn Any {
         self
     }
     fn fmt(&self) -> &str {
         "generic_join_build"
     }
 }
-
-pub(super) struct KeysIter<'a> {
-    key_iters: Vec<Box<dyn ExactSizeIterator<Item = AnyValue<'a>> + 'a>>,
-    // a small buffer that holds the current key values
-    // if we join by 2 keys, this holds 2 anyvalues.
-    buf: Vec<AnyValue<'a>>,
-}
-
-impl<'a> KeysIter<'a> {
-    pub(super) fn new(join_series: &'a [Series]) -> Self {
-        // iterators over anyvalues
-        let key_iters = join_series
-            .iter()
-            .map(|s| s.phys_iter())
-            .collect::<Vec<_>>();
-
-        // ensure that they have the appriate size as we will not bound check on push
-        let buf = Vec::with_capacity(key_iters.len());
-        Self { key_iters, buf }
-    }
-
-    /// # Safety
-    /// will not check any bounds on iterators. `lend_next` should not be called more often
-    /// than items in the given iterators.
-    pub(super) unsafe fn lend_next<'b>(&'b mut self) -> &'b [AnyValue<'a>] {
-        self.buf.clear();
-        for key_iter in self.key_iters.iter_mut() {
-            // safety: we allocated up front
-            self.buf
-                .push_unchecked(key_iter.next().unwrap_unchecked_release())
-        }
-        &self.buf
-    }
-}
```

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sinks/joins/inner_left.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-pipe/src/executors/sinks/joins/inner_left.rs`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 use std::borrow::Cow;
 use std::sync::Arc;
 
+use polars_arrow::export::arrow::array::BinaryArray;
 use polars_core::error::PolarsResult;
 use polars_core::export::ahash::RandomState;
 use polars_core::frame::hash_join::{ChunkId, _finish_join};
 use polars_core::prelude::*;
 use polars_core::series::IsSorted;
+use polars_row::RowsEncoded;
 use polars_utils::hash_to_partition;
 use polars_utils::slice::GetSaferUnchecked;
 use smartstring::alias::String as SmartString;
 
 use crate::executors::sinks::joins::generic_build::*;
-use crate::executors::sinks::utils::hash_series;
+use crate::executors::sinks::utils::hash_rows;
 use crate::expressions::PhysicalPipedExpr;
 use crate::operators::{DataChunk, Operator, OperatorResult, PExecutionContext};
 
 #[derive(Clone)]
 pub struct GenericJoinProbe {
     // all chunks are stacked into a single dataframe
     // the dataframe is not rechunked.
@@ -23,26 +25,27 @@
     // the join columns are all tightly packed
     // the values of a join column(s) can be found
     // by:
     // first get the offset of the chunks and multiply that with the number of join
     // columns
     //      * chunk_offset = (idx * n_join_keys)
     //      * end = (offset + n_join_keys)
-    materialized_join_cols: Arc<Vec<ArrayRef>>,
+    materialized_join_cols: Arc<Vec<BinaryArray<i64>>>,
     suffix: Arc<str>,
     hb: RandomState,
     // partitioned tables that will be used for probing
     // stores the key and the chunk_idx, df_idx of the left table
     hash_tables: Arc<Vec<PlIdHashMap<Key, Vec<ChunkId>>>>,
 
     // the columns that will be joined on
     join_columns_right: Arc<Vec<Arc<dyn PhysicalPipedExpr>>>,
 
     // amortize allocations
-    join_series: Vec<Series>,
+    current_rows: RowsEncoded,
+    join_columns: Vec<ArrayRef>,
     // in inner join these are the left table
     // in left join there are the right table
     join_tuples_a: Vec<ChunkId>,
     join_tuples_a_left_join: Vec<Option<ChunkId>>,
     // in inner join these are the right table
     // in left join there are the left table
     join_tuples_b: Vec<DfIdx>,
@@ -57,22 +60,22 @@
     how: JoinType,
 }
 
 impl GenericJoinProbe {
     #[allow(clippy::too_many_arguments)]
     pub(super) fn new(
         mut df_a: DataFrame,
-        materialized_join_cols: Arc<Vec<ArrayRef>>,
+        materialized_join_cols: Arc<Vec<BinaryArray<i64>>>,
         suffix: Arc<str>,
         hb: RandomState,
         hash_tables: Arc<Vec<PlIdHashMap<Key, Vec<ChunkId>>>>,
         join_columns_left: Arc<Vec<Arc<dyn PhysicalPipedExpr>>>,
         join_columns_right: Arc<Vec<Arc<dyn PhysicalPipedExpr>>>,
         swapped_or_left: bool,
-        join_series: Vec<Series>,
+        join_columns: Vec<ArrayRef>,
         hashes: Vec<u64>,
         context: &PExecutionContext,
         how: JoinType,
     ) -> Self {
         if swapped_or_left {
             let tmp = DataChunk {
                 data: df_a.slice(0, 1),
@@ -95,89 +98,90 @@
         GenericJoinProbe {
             df_a: Arc::new(df_a),
             materialized_join_cols,
             suffix,
             hb,
             hash_tables,
             join_columns_right,
-            join_series,
+            join_columns,
             join_tuples_a: vec![],
             join_tuples_a_left_join: vec![],
             join_tuples_b: vec![],
             hashes,
             swapped_or_left,
+            current_rows: Default::default(),
             join_column_idx: None,
             output_names: None,
             how,
         }
     }
     fn set_join_series(
         &mut self,
         context: &PExecutionContext,
         chunk: &DataChunk,
-    ) -> PolarsResult<&[Series]> {
-        self.join_series.clear();
+    ) -> PolarsResult<BinaryArray<i64>> {
+        self.join_columns.clear();
+
+        let determine_idx = !self.swapped_or_left && self.join_column_idx.is_none();
+        let mut names = vec![];
+
         for phys_e in self.join_columns_right.iter() {
             let s = phys_e.evaluate(chunk, context.execution_state.as_any())?;
-            let s = s.to_physical_repr();
-            self.join_series.push(s.rechunk());
+            let s = s.to_physical_repr().rechunk();
+            if determine_idx {
+                names.push(s.name().to_string());
+            }
+            self.join_columns.push(s.array_ref(0).clone());
         }
 
         // we determine the indices of the columns that have to be removed
         // if swapped the join column is already removed from the `build_df` as that will
         // be the rhs one.
         if !self.swapped_or_left && self.join_column_idx.is_none() {
-            let mut idx = self
-                .join_series
+            let mut idx = names
                 .iter()
-                .filter_map(|s| chunk.data.find_idx_by_name(s.name()))
+                .filter_map(|name| chunk.data.find_idx_by_name(name))
                 .collect::<Vec<_>>();
             // ensure that it is sorted so that we can later remove columns in
             // a predictable order
             idx.sort_unstable();
             self.join_column_idx = Some(idx);
         }
+        polars_row::convert_columns_amortized_no_order(&self.join_columns, &mut self.current_rows);
 
-        Ok(&self.join_series)
+        // safety: we keep rows-encode alive
+        unsafe { Ok(self.current_rows.borrow_array()) }
     }
 
     fn execute_left(
         &mut self,
         context: &PExecutionContext,
         chunk: &DataChunk,
     ) -> PolarsResult<OperatorResult> {
         // A left join holds the right table as build table
         // and streams the left table through. This allows us to maintain
         // the left table order
 
         self.join_tuples_a_left_join.clear();
         self.join_tuples_b.clear();
         let mut hashes = std::mem::take(&mut self.hashes);
-        self.set_join_series(context, chunk)?;
-        hash_series(&self.join_series, &mut hashes, &self.hb);
+        let rows = self.set_join_series(context, chunk)?;
+        hash_rows(&rows, &mut hashes, &self.hb);
         self.hashes = hashes;
-        let mut keys_iter = KeysIter::new(&self.join_series);
 
-        for (i, h) in self.hashes.iter().enumerate() {
+        for (i, (h, row)) in self.hashes.iter().zip(rows.values_iter()).enumerate() {
             let df_idx_left = i as IdxSize;
-            let current_tuple = unsafe { keys_iter.lend_next() };
             // get the hashtable belonging by this hash partition
             let partition = hash_to_partition(*h, self.hash_tables.len());
             let current_table = unsafe { self.hash_tables.get_unchecked_release(partition) };
 
             let entry = current_table
                 .raw_entry()
                 .from_hash(*h, |key| {
-                    compare_fn(
-                        key,
-                        *h,
-                        &self.materialized_join_cols,
-                        current_tuple,
-                        current_tuple.len(),
-                    )
+                    compare_fn(key, *h, &self.materialized_join_cols, row)
                 })
                 .map(|key_val| key_val.1);
 
             match entry {
                 Some(indexes_right) => {
                     self.join_tuples_a_left_join
                         .extend(indexes_right.iter().copied().map(Some));
@@ -186,18 +190,14 @@
                 }
                 None => {
                     self.join_tuples_b.push(df_idx_left);
                     self.join_tuples_a_left_join.push(None);
                 }
             }
         }
-        // tuples_b = left
-        // tuples_a = right
-        // left_df = right_df
-
         let right_df = self.df_a.as_ref();
 
         let mut left_df = unsafe { chunk.data._take_unchecked_slice(&self.join_tuples_b, false) };
         let right_df =
             unsafe { right_df._take_opt_chunked_unchecked_seq(&self.join_tuples_a_left_join) };
 
         let out = match &self.output_names {
@@ -228,36 +228,28 @@
         &mut self,
         context: &PExecutionContext,
         chunk: &DataChunk,
     ) -> PolarsResult<OperatorResult> {
         self.join_tuples_a.clear();
         self.join_tuples_b.clear();
         let mut hashes = std::mem::take(&mut self.hashes);
-        self.set_join_series(context, chunk)?;
-        hash_series(&self.join_series, &mut hashes, &self.hb);
+        let rows = self.set_join_series(context, chunk)?;
+        hash_rows(&rows, &mut hashes, &self.hb);
         self.hashes = hashes;
-        let mut keys_iter = KeysIter::new(&self.join_series);
 
-        for (i, h) in self.hashes.iter().enumerate() {
+        for (i, (h, row)) in self.hashes.iter().zip(rows.values_iter()).enumerate() {
             let df_idx_right = i as IdxSize;
-            let current_tuple = unsafe { keys_iter.lend_next() };
             // get the hashtable belonging by this hash partition
             let partition = hash_to_partition(*h, self.hash_tables.len());
             let current_table = unsafe { self.hash_tables.get_unchecked_release(partition) };
 
             let entry = current_table
                 .raw_entry()
                 .from_hash(*h, |key| {
-                    compare_fn(
-                        key,
-                        *h,
-                        &self.materialized_join_cols,
-                        current_tuple,
-                        current_tuple.len(),
-                    )
+                    compare_fn(key, *h, &self.materialized_join_cols, row)
                 })
                 .map(|key_val| key_val.1);
 
             if let Some(indexes_left) = entry {
                 self.join_tuples_a.extend_from_slice(indexes_left);
                 self.join_tuples_b
                     .extend(std::iter::repeat(df_idx_right).take(indexes_left.len()));
```

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sinks/memory.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-pipe/src/executors/sinks/memory.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sinks/mod.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-pipe/src/executors/sinks/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sinks/ordered.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-pipe/src/executors/sinks/ordered.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sinks/reproject.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-pipe/src/executors/sinks/reproject.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sinks/slice.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-pipe/src/executors/sinks/slice.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sinks/sort/ooc.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-pipe/src/executors/sinks/sort/ooc.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sinks/sort/sink.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-pipe/src/executors/sinks/sort/sink.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sinks/sort/sink_multiple.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-pipe/src/executors/sinks/sort/sink_multiple.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sinks/sort/source.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-pipe/src/executors/sinks/sort/source.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sources/csv.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-pipe/src/executors/sources/csv.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sources/frame.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-pipe/src/executors/sources/frame.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sources/ipc_one_shot.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-pipe/src/executors/sources/ipc_one_shot.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sources/parquet.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-pipe/src/executors/sources/parquet.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sources/reproject.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-pipe/src/executors/sources/reproject.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sources/union.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-pipe/src/executors/sources/union.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/operators/chunks.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-pipe/src/operators/chunks.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/operators/operator.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-pipe/src/operators/operator.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/operators/sink.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-pipe/src/operators/sink.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/pipeline/convert.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-pipe/src/pipeline/convert.rs`

 * *Files 0% similar despite different names*

```diff
@@ -134,15 +134,15 @@
                     Box::new(ParquetSink::new(path, *options, input_schema.as_ref())?)
                         as Box<dyn Sink>
                 }
                 #[cfg(feature = "ipc")]
                 FileType::Ipc(options) => {
                     Box::new(IpcSink::new(path, *options, input_schema.as_ref())?) as Box<dyn Sink>
                 }
-                FileType::Memory => Box::new(OrderedSink::new()),
+                FileType::Memory => Box::new(OrderedSink::new()) as Box<dyn Sink>,
             }
         }
         Join {
             input_left,
             input_right,
             options,
             left_on,
```

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/pipeline/dispatcher.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-pipe/src/pipeline/dispatcher.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/pipeline/mod.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-pipe/src/pipeline/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/Cargo.toml` & `polars_lts_cpu-0.18.3/local_dependencies/polars-lazy/Cargo.toml`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/LICENSE` & `polars_lts_cpu-0.18.3/local_dependencies/polars-ops/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/dot.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-lazy/src/dot.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/dsl/eval.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-lazy/src/dsl/eval.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/dsl/functions.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-lazy/src/dsl/functions.rs`

 * *Files 21% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 use crate::prelude::*;
 
 pub(crate) fn concat_impl<L: AsRef<[LazyFrame]>>(
     inputs: L,
     rechunk: bool,
     parallel: bool,
     from_partitioned_ds: bool,
+    convert_supertypes: bool,
 ) -> PolarsResult<LazyFrame> {
     let mut inputs = inputs.as_ref().to_vec();
 
     let mut lf = std::mem::take(
         inputs
             .get_mut(0)
             .ok_or_else(|| polars_err!(NoData: "empty container given"))?,
@@ -26,27 +27,27 @@
     let options = UnionOptions {
         parallel,
         from_partitioned_ds,
         rechunk,
         ..Default::default()
     };
 
-    match &mut lf.logical_plan {
+    let lf = match &mut lf.logical_plan {
         // re-use the same union
         LogicalPlan::Union {
             inputs: existing_inputs,
             options: opts,
         } if opts == &options => {
             for lf in &mut inputs[1..] {
                 // ensure we enable file caching if any lf has it enabled
                 opt_state.file_caching |= lf.opt_state.file_caching;
                 let lp = std::mem::take(&mut lf.logical_plan);
                 existing_inputs.push(lp)
             }
-            Ok(lf)
+            lf
         }
         _ => {
             let mut lps = Vec::with_capacity(inputs.len());
             lps.push(lf.logical_plan);
 
             for lf in &mut inputs[1..] {
                 // ensure we enable file caching if any lf has it enabled
@@ -58,16 +59,57 @@
             let lp = LogicalPlan::Union {
                 inputs: lps,
                 options,
             };
             let mut lf = LazyFrame::from(lp);
             lf.opt_state = opt_state;
 
-            Ok(lf)
+            lf
         }
+    };
+
+    if convert_supertypes {
+        let LogicalPlan::Union {mut inputs, options} = lf.logical_plan else { unreachable!()} ;
+        let mut schema = inputs[0].schema()?.as_ref().as_ref().clone();
+
+        let mut changed = false;
+        for input in inputs[1..].iter() {
+            changed |= schema.to_supertype(input.schema()?.as_ref().as_ref())?;
+        }
+
+        let mut placeholder = LogicalPlan::default();
+        if changed {
+            let mut exprs = vec![];
+            for input in &mut inputs {
+                std::mem::swap(input, &mut placeholder);
+                let input_schema = placeholder.schema()?;
+
+                exprs.clear();
+                let to_cast = input_schema.iter().zip(schema.iter_dtypes()).flat_map(
+                    |((left_name, left_type), st)| {
+                        if left_type != st {
+                            Some(col(left_name.as_ref()).cast(st.clone()))
+                        } else {
+                            None
+                        }
+                    },
+                );
+                exprs.extend(to_cast);
+                let mut lf = LazyFrame::from(placeholder);
+                if !exprs.is_empty() {
+                    lf = lf.with_columns(exprs.as_slice());
+                }
+
+                placeholder = lf.logical_plan;
+                std::mem::swap(&mut placeholder, input);
+            }
+        }
+        Ok(LazyFrame::from(LogicalPlan::Union { inputs, options }))
+    } else {
+        Ok(lf)
     }
 }
 
 #[cfg(feature = "diagonal_concat")]
 /// Concat [LazyFrame]s diagonally.
 /// Calls [`concat`][concat()] internally.
 pub fn diag_concat_lf<L: AsRef<[LazyFrame]>>(
@@ -116,24 +158,50 @@
                     .collect::<Vec<Expr>>(),
             );
 
             Ok(reordered_lf)
         })
         .collect::<PolarsResult<Vec<_>>>()?;
 
-    concat(lfs_with_all_columns, rechunk, parallel)
+    concat(
+        lfs_with_all_columns,
+        UnionArgs {
+            rechunk,
+            parallel,
+            to_supertypes: false,
+        },
+    )
+}
+
+#[derive(Clone, Copy)]
+pub struct UnionArgs {
+    pub parallel: bool,
+    pub rechunk: bool,
+    pub to_supertypes: bool,
+}
+
+impl Default for UnionArgs {
+    fn default() -> Self {
+        Self {
+            parallel: true,
+            rechunk: true,
+            to_supertypes: false,
+        }
+    }
 }
 
 /// Concat multiple
-pub fn concat<L: AsRef<[LazyFrame]>>(
-    inputs: L,
-    rechunk: bool,
-    parallel: bool,
-) -> PolarsResult<LazyFrame> {
-    concat_impl(inputs, rechunk, parallel, false)
+pub fn concat<L: AsRef<[LazyFrame]>>(inputs: L, args: UnionArgs) -> PolarsResult<LazyFrame> {
+    concat_impl(
+        inputs,
+        args.rechunk,
+        args.parallel,
+        false,
+        args.to_supertypes,
+    )
 }
 
 /// Collect all `LazyFrame` computations.
 pub fn collect_all<I>(lfs: I) -> PolarsResult<Vec<DataFrame>>
 where
     I: IntoParallelIterator<Item = LazyFrame>,
 {
```

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/dsl/list.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-lazy/src/dsl/list.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/dsl/mod.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-lazy/src/dsl/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/frame/anonymous_scan.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-lazy/src/frame/anonymous_scan.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/frame/csv.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-lazy/src/frame/csv.rs`

 * *Files 0% similar despite different names*

```diff
@@ -304,10 +304,10 @@
     /// Add a `row_count` column.
     fn row_count(&self) -> Option<&RowCount> {
         self.row_count.as_ref()
     }
 
     fn concat_impl(&self, lfs: Vec<LazyFrame>) -> PolarsResult<LazyFrame> {
         // set to false, as the csv parser has full thread utilization
-        concat_impl(&lfs, self.rechunk(), false, true)
+        concat_impl(&lfs, self.rechunk(), false, true, false)
     }
 }
```

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/frame/file_list_reader.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-lazy/src/frame/file_list_reader.rs`

 * *Files 2% similar despite different names*

```diff
@@ -71,15 +71,15 @@
     }
 
     /// Recommended concatenation of [LazyFrame]s from many input files.
     ///
     /// This method should not take into consideration [LazyFileListReader::n_rows]
     /// nor [LazyFileListReader::row_count].
     fn concat_impl(&self, lfs: Vec<LazyFrame>) -> PolarsResult<LazyFrame> {
-        concat_impl(&lfs, self.rechunk(), true, true)
+        concat_impl(&lfs, self.rechunk(), true, true, false)
     }
 
     /// Get the final [LazyFrame].
     /// This method assumes, that path is *not* a glob.
     ///
     /// It is recommended to always use [LazyFileListReader::finish] method.
     fn finish_no_glob(self) -> PolarsResult<LazyFrame>;
```

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/frame/ipc.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-lazy/src/frame/ipc.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/frame/mod.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-lazy/src/frame/mod.rs`

 * *Files 0% similar despite different names*

```diff
@@ -475,15 +475,15 @@
             opt_state.common_subplan_elimination = false;
         }
         let lp_top = optimize(self.logical_plan, opt_state, lp_arena, expr_arena, scratch)?;
 
         if streaming {
             #[cfg(feature = "streaming")]
             {
-                insert_streaming_nodes(lp_top, lp_arena, expr_arena, scratch, _fmt)?;
+                insert_streaming_nodes(lp_top, lp_arena, expr_arena, scratch, _fmt, true)?;
             }
             #[cfg(not(feature = "streaming"))]
             {
                 panic!("activate feature 'streaming'")
             }
         }
         Ok(lp_top)
@@ -1261,15 +1261,22 @@
     #[cfg(feature = "merge_sorted")]
     pub fn merge_sorted(self, other: LazyFrame, key: &str) -> PolarsResult<LazyFrame> {
         // The two DataFrames are temporary concatenated
         // this indicates until which chunk the data is from the left df
         // this trick allows us to reuse the `Union` architecture to get map over
         // two DataFrames
         let left = self.map_private(FunctionNode::Rechunk);
-        let q = concat(&[left, other], false, true)?;
+        let q = concat(
+            &[left, other],
+            UnionArgs {
+                rechunk: false,
+                parallel: true,
+                ..Default::default()
+            },
+        )?;
         Ok(q.map_private(FunctionNode::MergeSorted {
             column: Arc::from(key),
         }))
     }
 }
 
 /// Utility struct for lazy groupby operation.
```

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/frame/ndjson.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-lazy/src/frame/ndjson.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/frame/parquet.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-lazy/src/frame/parquet.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/frame/pivot.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-lazy/src/frame/pivot.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/lib.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-lazy/src/lib.rs`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 //! it is very similar to [Apache Spark](https://spark.apache.org/). You write queries in a
 //! domain specific language. These queries translate to a logical plan, which represent your query steps.
 //! Before execution this logical plan is optimized and may change the order of operations if this will increase performance.
 //! Or implicit type casts may be added such that execution of the query won't lead to a type error (if it can be resolved).
 //!
 //! # Lazy DSL
 //!
-//! The lazy API of polars can be used as long we operation on one or multiple DataFrame(s) and
+//! The lazy API of polars can be used as long we operate on one or multiple DataFrame(s) and
 //! Series of the same length as the DataFrame. To get started we call the [lazy](crate::frame::IntoLazy::lazy)
 //! method. This returns a [LazyFrame](crate::frame::LazyFrame) exposing the lazy API.
 //!
 //! Lazy operations don't execute until we call [collect](crate::frame::LazyFrame::collect).
 //! This allows polars to optimize/reorder the query which may lead to faster queries or less type errors.
 //!
 //! The DSL is mostly defined by [LazyFrame](crate::frame::LazyFrame) for operations on DataFrames and
```

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/executors/cache.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-lazy/src/physical_plan/executors/cache.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/executors/executor.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-lazy/src/physical_plan/executors/executor.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/executors/ext_context.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-lazy/src/physical_plan/executors/ext_context.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/executors/filter.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-lazy/src/physical_plan/executors/filter.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/executors/groupby.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-lazy/src/physical_plan/executors/groupby.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/executors/groupby_dynamic.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-lazy/src/physical_plan/executors/groupby_dynamic.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/executors/groupby_partitioned.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-lazy/src/physical_plan/executors/groupby_partitioned.rs`

 * *Files 0% similar despite different names*

```diff
@@ -249,14 +249,15 @@
 
         let inserted = streaming::insert_streaming_nodes(
             node,
             &mut lp_arena,
             &mut expr_arena,
             &mut vec![],
             false,
+            false,
         )
         .unwrap();
 
         if inserted {
             let mut phys_plan = create_physical_plan(node, &mut lp_arena, &mut expr_arena).unwrap();
 
             if state.verbose() {
```

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/executors/groupby_rolling.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-lazy/src/physical_plan/executors/groupby_rolling.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/executors/join.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-lazy/src/physical_plan/executors/join.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/executors/mod.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-lazy/src/physical_plan/executors/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/executors/projection.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-lazy/src/physical_plan/executors/projection.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/executors/python_scan.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-lazy/src/physical_plan/executors/python_scan.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/executors/scan/csv.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-lazy/src/physical_plan/executors/scan/csv.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/executors/scan/ipc.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-lazy/src/physical_plan/executors/scan/ipc.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/executors/scan/mod.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-lazy/src/physical_plan/executors/scan/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/executors/scan/ndjson.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-lazy/src/physical_plan/executors/scan/ndjson.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/executors/scan/parquet.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-lazy/src/physical_plan/executors/scan/parquet.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/executors/slice.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-lazy/src/physical_plan/executors/slice.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/executors/sort.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-lazy/src/physical_plan/executors/sort.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/executors/stack.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-lazy/src/physical_plan/executors/stack.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/executors/udf.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-lazy/src/physical_plan/executors/udf.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/executors/union.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-lazy/src/physical_plan/executors/union.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/executors/unique.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-lazy/src/physical_plan/executors/unique.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/exotic.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-lazy/src/physical_plan/exotic.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/expressions/aggregation.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-lazy/src/physical_plan/expressions/aggregation.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/expressions/alias.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-lazy/src/physical_plan/expressions/alias.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/expressions/apply.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-lazy/src/physical_plan/expressions/apply.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/expressions/binary.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-lazy/src/physical_plan/expressions/binary.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/expressions/cache.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-lazy/src/physical_plan/expressions/cache.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/expressions/cast.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-lazy/src/physical_plan/expressions/cast.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/expressions/column.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-lazy/src/physical_plan/expressions/column.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/expressions/count.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-lazy/src/physical_plan/expressions/count.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/expressions/filter.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-lazy/src/physical_plan/expressions/filter.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/expressions/group_iter.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-lazy/src/physical_plan/expressions/group_iter.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/expressions/literal.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-lazy/src/physical_plan/expressions/literal.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/expressions/mod.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-lazy/src/physical_plan/expressions/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/expressions/slice.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-lazy/src/physical_plan/expressions/slice.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/expressions/sort.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-lazy/src/physical_plan/expressions/sort.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/expressions/sortby.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-lazy/src/physical_plan/expressions/sortby.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/expressions/take.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-lazy/src/physical_plan/expressions/take.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/expressions/ternary.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-lazy/src/physical_plan/expressions/ternary.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/expressions/window.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-lazy/src/physical_plan/expressions/window.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/file_cache.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-lazy/src/physical_plan/file_cache.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/node_timer.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-lazy/src/physical_plan/node_timer.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/planner/expr.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-lazy/src/physical_plan/planner/expr.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/planner/lp.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-lazy/src/physical_plan/planner/lp.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/state.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-lazy/src/physical_plan/state.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/streaming/checks.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-lazy/src/physical_plan/streaming/checks.rs`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,18 @@
             ),
             Context::Aggregation => matches!(options.collect_groups, ApplyOptions::ApplyFlat),
         },
         AExpr::Column(_) => {
             seen_column = true;
             true
         }
-        AExpr::BinaryExpr { .. } | AExpr::Alias(_, _) | AExpr::Cast { .. } => true,
+        AExpr::Ternary { .. }
+        | AExpr::BinaryExpr { .. }
+        | AExpr::Alias(_, _)
+        | AExpr::Cast { .. } => true,
         AExpr::Literal(lv) => match lv {
             LiteralValue::Series(_) | LiteralValue::Range { .. } => {
                 seen_lit_range = true;
                 true
             }
             _ => true,
         },
```

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/streaming/construct_pipeline.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-lazy/src/physical_plan/streaming/construct_pipeline.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/streaming/convert_alp.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-lazy/src/physical_plan/streaming/convert_alp.rs`

 * *Files 4% similar despite different names*

```diff
@@ -66,25 +66,40 @@
 
 pub(crate) fn insert_streaming_nodes(
     root: Node,
     lp_arena: &mut Arena<ALogicalPlan>,
     expr_arena: &mut Arena<AExpr>,
     scratch: &mut Vec<Node>,
     fmt: bool,
+    // whether the full plan needs to be translated
+    // to streaming
+    allow_partial: bool,
 ) -> PolarsResult<bool> {
     // this is needed to determine which side of the joins should be
     // traversed first
     set_estimated_row_counts(root, lp_arena, expr_arena, 0);
 
     scratch.clear();
 
-    // The pipelines need a final sink, we insert that here.
+    // The pipelines always need to end in a SINK, we insert that here.
     // this allows us to split at joins/unions and share a sink
     let root = insert_file_sink(root, lp_arena);
 
+    // We use mutation to communicate when we need to insert a file sink.
+    // This happens for instance when we
+    //
+    //     ________*non-streamable part of query
+    //   /\
+    //     ________*streamable below this line so we must insert
+    //    /\        a file sink here so the pipeline can be built
+    //     /\
+    //
+    // when this is positive we should insert a file sink
+    let mut insert_file_sink_ptr: u32 = 0;
+
     let mut stack = Vec::with_capacity(16);
 
     stack.push((root, Branch::default(), 0 as CurrentIdx));
 
     // A state holds a full pipeline until the breaker
     //  1/\
     //   2/\
@@ -109,17 +124,14 @@
     // an `execution_id` which will be incremented on every stack operation.
     // This way we know in which order the stack/tree was traversed and can
     // use that info to determine the execution order of the single branch/pipelines
     let mut pipeline_trees: Vec<Tree> = vec![vec![]];
     // keep the counter global so that the order will match traversal order
     let mut execution_id = 0;
 
-    // when this is positive we should insert a file sink
-    let mut insert_file_sink_ptr: u32 = 0;
-
     use ALogicalPlan::*;
     while let Some((mut root, mut state, mut current_idx)) = stack.pop() {
         if insert_file_sink_ptr > 0 {
             root = insert_file_sink(root, lp_arena);
         }
         insert_file_sink_ptr = insert_file_sink_ptr.saturating_sub(1);
         state.execution_id = execution_id;
@@ -328,15 +340,15 @@
                     && !matches!(options.keep_strategy, UniqueKeepStrategy::None) =>
             {
                 state.streamable = true;
                 state.operators_sinks.push(PipelineNode::Sink(root));
                 stack.push((*input, state, current_idx))
             }
             #[allow(unused_variables)]
-            Aggregate {
+            lp @ Aggregate {
                 input,
                 aggs,
                 maintain_order: false,
                 apply: None,
                 schema,
                 options,
                 ..
@@ -378,27 +390,43 @@
                     && schema
                         .iter_dtypes()
                         .all(|dt| allowed_dtype(dt, string_cache))
                 {
                     state.streamable = true;
                     state.operators_sinks.push(PipelineNode::Sink(root));
                     stack.push((*input, state, current_idx))
+                } else if allow_partial {
+                    process_non_streamable_node(
+                        &mut current_idx,
+                        &mut state,
+                        &mut stack,
+                        scratch,
+                        &mut pipeline_trees,
+                        lp,
+                        &mut insert_file_sink_ptr,
+                    )
+                } else {
+                    return Ok(false);
+                }
+            }
+            lp => {
+                if allow_partial {
+                    process_non_streamable_node(
+                        &mut current_idx,
+                        &mut state,
+                        &mut stack,
+                        scratch,
+                        &mut pipeline_trees,
+                        lp,
+                        &mut insert_file_sink_ptr,
+                    )
                 } else {
-                    stack.push((*input, Branch::default(), current_idx))
+                    return Ok(false);
                 }
             }
-            lp => process_non_streamable_node(
-                &mut current_idx,
-                &mut state,
-                &mut stack,
-                scratch,
-                &mut pipeline_trees,
-                lp,
-                &mut insert_file_sink_ptr,
-            ),
         }
     }
     let mut inserted = false;
     for tree in pipeline_trees {
         if is_valid_tree(&tree)
             && super::construct_pipeline::construct(tree, lp_arena, expr_arena, fmt)?.is_some()
         {
```

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/streaming/tree.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-lazy/src/physical_plan/streaming/tree.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/prelude.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-lazy/src/prelude.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/tests/aggregations.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-lazy/src/tests/aggregations.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/tests/arity.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-lazy/src/tests/arity.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/tests/cse.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-lazy/src/tests/cse.rs`

 * *Files 1% similar despite different names*

```diff
@@ -28,17 +28,24 @@
 
 #[test]
 fn test_cse_unions() -> PolarsResult<()> {
     let lf = scan_foods_ipc();
 
     let lf1 = lf.clone().with_column(col("category").str().to_uppercase());
 
-    let lf = concat(&[lf1.clone(), lf, lf1], false, false)?
-        .select([col("category"), col("fats_g")])
-        .with_common_subplan_elimination(true);
+    let lf = concat(
+        &[lf1.clone(), lf, lf1],
+        UnionArgs {
+            rechunk: false,
+            parallel: false,
+            ..Default::default()
+        },
+    )?
+    .select([col("category"), col("fats_g")])
+    .with_common_subplan_elimination(true);
 
     let (mut expr_arena, mut lp_arena) = get_arenas();
     let lp = lf.clone().optimize(&mut lp_arena, &mut expr_arena).unwrap();
     assert!((&lp_arena).iter(lp).all(|(_, lp)| {
         use ALogicalPlan::*;
         match lp {
             IpcScan { options, .. } => {
@@ -104,16 +111,21 @@
 
     let lf2 = df![
         "ts" => [1],
         "d" => [3],
     ]?
     .lazy();
 
-    let lf1 = concat(&[lf1.clone(), lf1], false, false)?;
-    let lf2 = concat(&[lf2.clone(), lf2], false, false)?;
+    let args = UnionArgs {
+        parallel: false,
+        rechunk: false,
+        ..Default::default()
+    };
+    let lf1 = concat(&[lf1.clone(), lf1], args)?;
+    let lf2 = concat(&[lf2.clone(), lf2], args)?;
 
     let q = lf1.inner_join(lf2, col("ts"), col("ts")).select([
         col("ts"),
         col("sym"),
         col("d") / col("c"),
     ]);
```

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/tests/io.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-lazy/src/tests/io.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/tests/logical.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-lazy/src/tests/logical.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/tests/mod.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-lazy/src/tests/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/tests/optimization_checks.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-lazy/src/tests/optimization_checks.rs`

 * *Files 2% similar despite different names*

```diff
@@ -569,17 +569,22 @@
 
     let lf = df! {
         "a" => [1,2,3,4,5],
     }
     .unwrap()
     .lazy();
 
-    let lf2 = concat(&[lf.clone(), lf.clone()], false, true).unwrap();
-    let lf3 = concat(&[lf.clone(), lf.clone(), lf.clone()], false, true).unwrap();
-    let lf4 = concat(&[lf2.clone(), lf3], false, true).unwrap();
+    let args = UnionArgs {
+        rechunk: false,
+        parallel: true,
+        ..Default::default()
+    };
+    let lf2 = concat(&[lf.clone(), lf.clone()], args).unwrap();
+    let lf3 = concat(&[lf.clone(), lf.clone(), lf.clone()], args).unwrap();
+    let lf4 = concat(&[lf2.clone(), lf3], args).unwrap();
     let root = lf4.optimize(&mut lp_arena, &mut expr_arena).unwrap();
     let lp = lp_arena.get(root);
     match lp {
         ALogicalPlan::Union { inputs, .. } => {
             // we make sure that the nested unions are flattened into a single union
             assert_eq!(inputs.len(), 5);
         }
```

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/tests/predicate_queries.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-lazy/src/tests/predicate_queries.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/tests/projection_queries.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-lazy/src/tests/projection_queries.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/tests/queries.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-lazy/src/tests/queries.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/tests/streaming.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-lazy/src/tests/streaming.rs`

 * *Files 4% similar despite different names*

```diff
@@ -67,15 +67,15 @@
     assert_streaming_with_default(q, true, false);
     Ok(())
 }
 
 #[test]
 fn test_streaming_union_order() -> PolarsResult<()> {
     let q = get_csv_glob();
-    let q = concat([q.clone(), q], false, false)?;
+    let q = concat([q.clone(), q], Default::default())?;
     let q = q.select([col("sugars_g"), col("calories")]);
 
     assert_streaming_with_default(q, true, false);
     Ok(())
 }
 
 #[test]
```

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/tests/tpch.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-lazy/src/tests/tpch.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/utils.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-lazy/src/utils.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars/Cargo.toml` & `polars_lts_cpu-0.18.3/local_dependencies/polars/Cargo.toml`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars/LICENSE` & `polars_lts_cpu-0.18.3/local_dependencies/polars-lazy/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars/Makefile` & `polars_lts_cpu-0.18.3/local_dependencies/polars/Makefile`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars/src/docs/eager.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars/src/docs/eager.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars/src/docs/lazy.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars/src/docs/lazy.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars/src/docs/performance.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars/src/docs/performance.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars/src/lib.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars/src/lib.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars/tests/it/core/date_like.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars/tests/it/core/date_like.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars/tests/it/core/groupby.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars/tests/it/core/groupby.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars/tests/it/core/joins.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars/tests/it/core/joins.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars/tests/it/core/list.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars/tests/it/core/list.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars/tests/it/core/pivot.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars/tests/it/core/pivot.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars/tests/it/core/random.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars/tests/it/core/random.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars/tests/it/core/rolling_window.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars/tests/it/core/rolling_window.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars/tests/it/core/series.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars/tests/it/core/series.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars/tests/it/io/csv.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars/tests/it/io/csv.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars/tests/it/io/ipc_stream.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars/tests/it/io/ipc_stream.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars/tests/it/io/json.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars/tests/it/io/json.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars/tests/it/io/parquet.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars/tests/it/io/parquet.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars/tests/it/joins.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars/tests/it/joins.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars/tests/it/lazy/aggregation.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars/tests/it/lazy/aggregation.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars/tests/it/lazy/cse.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars/tests/it/lazy/cse.rs`

 * *Files 18% similar despite different names*

```diff
@@ -15,18 +15,25 @@
 
     let q3 = q2
         .clone()
         .join(q1.clone(), [col("b")], [col("b")], JoinType::Anti.into())
         .with_column(lit(0).alias("a"))
         .select([col("a"), col("b")]);
 
-    let out = concat([q1, q3], true, true)
-        .unwrap()
-        .with_common_subplan_elimination(true)
-        .collect()?;
+    let out = concat(
+        [q1, q3],
+        UnionArgs {
+            rechunk: false,
+            parallel: false,
+            ..Default::default()
+        },
+    )
+    .unwrap()
+    .with_common_subplan_elimination(true)
+    .collect()?;
     let expected = df![
         "a" => [1, 0],
         "b" => [2, 1],
     ]?;
     assert!(out.frame_equal(&expected));
 
     Ok(())
```

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars/tests/it/lazy/expressions/apply.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars/tests/it/lazy/expressions/apply.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars/tests/it/lazy/expressions/arity.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars/tests/it/lazy/expressions/arity.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars/tests/it/lazy/expressions/expand.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars/tests/it/lazy/expressions/expand.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars/tests/it/lazy/expressions/filter.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars/tests/it/lazy/expressions/filter.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars/tests/it/lazy/expressions/slice.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars/tests/it/lazy/expressions/slice.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars/tests/it/lazy/expressions/window.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars/tests/it/lazy/expressions/window.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars/tests/it/lazy/folds.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars/tests/it/lazy/folds.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars/tests/it/lazy/functions.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars/tests/it/lazy/functions.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars/tests/it/lazy/groupby.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars/tests/it/lazy/groupby.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars/tests/it/lazy/groupby_dynamic.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars/tests/it/lazy/groupby_dynamic.rs`

 * *Files 15% similar despite different names*

```diff
@@ -46,14 +46,15 @@
             DynamicGroupOptions {
                 every: Duration::parse("1w"),
                 period: Duration::parse("1w"),
                 offset: Duration::parse("0w"),
                 closed_window: ClosedWindow::Left,
                 truncate: false,
                 include_boundaries: true,
+                start_by: StartBy::DataPoint,
                 ..Default::default()
             },
         )
         .agg([col("a").sum()])
         .collect()?;
     let a = out.column("a")?;
     assert_eq!(a.get(0)?, AnyValue::Int32(7));
```

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars/tests/it/lazy/mod.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars/tests/it/lazy/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars/tests/it/lazy/predicate_queries.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars/tests/it/lazy/predicate_queries.rs`

 * *Files 2% similar despite different names*

```diff
@@ -192,17 +192,24 @@
 
     let expected = df![
         "k" => ["x", "x", "a", "a"],
         "v" => [3, 2, 1, 8]
     ]?;
 
     for rechunk in [true, false] {
-        let out = concat([lf1.clone(), lf2.clone()], rechunk, true)?
-            .filter(count().over([col("k")]).gt(lit(1)))
-            .collect()?;
+        let out = concat(
+            [lf1.clone(), lf2.clone()],
+            UnionArgs {
+                rechunk,
+                parallel: true,
+                ..Default::default()
+            },
+        )?
+        .filter(count().over([col("k")]).gt(lit(1)))
+        .collect()?;
 
         assert!(out.frame_equal(&expected));
     }
 
     Ok(())
 }
```

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars/tests/it/lazy/projection_queries.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars/tests/it/lazy/projection_queries.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars/tests/it/lazy/queries.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars/tests/it/lazy/queries.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars/tests/it/schema.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars/tests/it/schema.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-time/Cargo.toml` & `polars_lts_cpu-0.18.3/local_dependencies/polars-time/Cargo.toml`

 * *Files 8% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 
 default = []
 
 [dependencies.arrow]
 package = "arrow2"
 git = "https://github.com/jorgecarleitao/arrow2"
 # git = "https://github.com/ritchie46/arrow2"
-rev = "fb5e4d591c7149df590a330365fae55d2370962f"
+rev = "2d2e7053f9a50810bfe9cecff25ab39089aef98e"
 # path = "../arrow2"
 # branch = "polars_2023-05-25"
 version = "0.17"
 default-features = false
 features = [
   "compute_aggregate",
   "compute_arithmetics",
```

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-time/LICENSE` & `polars_lts_cpu-0.18.3/local_dependencies/polars-utils/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-time/src/chunkedarray/date.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-time/src/chunkedarray/date.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-time/src/chunkedarray/datetime.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-time/src/chunkedarray/datetime.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-time/src/chunkedarray/duration.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-time/src/chunkedarray/duration.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-time/src/chunkedarray/kernels.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-time/src/chunkedarray/kernels.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-time/src/chunkedarray/mod.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-time/src/chunkedarray/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-time/src/chunkedarray/rolling_window/floats.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-time/src/chunkedarray/rolling_window/floats.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-time/src/chunkedarray/rolling_window/ints.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-time/src/chunkedarray/rolling_window/ints.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-time/src/chunkedarray/rolling_window/mod.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-time/src/chunkedarray/rolling_window/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-time/src/chunkedarray/rolling_window/rolling_kernels/no_nulls.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-time/src/chunkedarray/rolling_window/rolling_kernels/no_nulls.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-time/src/chunkedarray/time.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-time/src/chunkedarray/time.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-time/src/chunkedarray/utf8/infer.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-time/src/chunkedarray/utf8/infer.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-time/src/chunkedarray/utf8/mod.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-time/src/chunkedarray/utf8/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-time/src/chunkedarray/utf8/patterns.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-time/src/chunkedarray/utf8/patterns.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-time/src/chunkedarray/utf8/strptime.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-time/src/chunkedarray/utf8/strptime.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-time/src/date_range.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-time/src/date_range.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-time/src/groupby/dynamic.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-time/src/groupby/dynamic.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-time/src/lib.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-time/src/lib.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-time/src/month_end.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-time/src/month_end.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-time/src/month_start.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-time/src/month_start.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-time/src/round.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-time/src/round.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-time/src/series/_trait.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-time/src/series/_trait.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-time/src/series/implementations/floats.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-time/src/series/implementations/floats.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-time/src/series/implementations/integers.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-time/src/series/implementations/integers.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-time/src/series/mod.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-time/src/series/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-time/src/truncate.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-time/src/truncate.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-time/src/upsample.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-time/src/upsample.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-time/src/utils.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-time/src/utils.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-time/src/windows/bounds.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-time/src/windows/bounds.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-time/src/windows/calendar.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-time/src/windows/calendar.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-time/src/windows/duration.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-time/src/windows/duration.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-time/src/windows/groupby.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-time/src/windows/groupby.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-time/src/windows/test.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-time/src/windows/test.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-time/src/windows/window.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-time/src/windows/window.rs`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 use chrono::NaiveDateTime;
 #[cfg(feature = "timezones")]
 use chrono::TimeZone;
 use now::DateTimeNow;
 use polars_arrow::export::arrow::temporal_conversions::*;
 use polars_arrow::time_zone::Tz;
 use polars_core::prelude::*;
-use polars_core::utils::arrow::temporal_conversions::{timeunit_scale, SECONDS_IN_DAY};
+use polars_core::utils::arrow::temporal_conversions::timeunit_scale;
 
 use crate::prelude::*;
 
 /// Represents a window in time
 #[derive(Copy, Clone)]
 pub struct Window {
     // The ith window start is expressed via this equation:
@@ -79,60 +79,29 @@
             / (2 * timeunit_scale(ArrowTimeUnit::Nanosecond, ArrowTimeUnit::Millisecond) as i64);
         self.truncate_ms(t, tz)
     }
 
     /// returns the bounds for the earliest window bounds
     /// that contains the given time t.  For underlapping windows that
     /// do not contain time t, the window directly after time t will be returned.
-    ///
-    /// For `every` larger than `1day` we just take the given timestamp `t` as start as truncation
-    /// does not seems intuitive.
-    /// Below 1 day, it make sense to truncate to:
-    /// - days
-    /// - hours
-    /// - 15 minutes
-    /// - etc.
-    ///
-    /// But for 2w3d, it does not make sense to start it on a different lower bound, so we start at `t`
     pub fn get_earliest_bounds_ns(&self, t: i64, tz: Option<&Tz>) -> PolarsResult<Bounds> {
-        let start = if !self.every.months_only()
-            && self.every.duration_ns() > NANOSECONDS * SECONDS_IN_DAY
-        {
-            self.offset.add_ns(t, tz)?
-        } else {
-            // offset is translated in the truncate
-            self.truncate_ns(t, tz)?
-        };
-
+        let start = self.truncate_ns(t, tz)?;
         let stop = self.period.add_ns(start, tz)?;
 
         Ok(Bounds::new_checked(start, stop))
     }
 
     pub fn get_earliest_bounds_us(&self, t: i64, tz: Option<&Tz>) -> PolarsResult<Bounds> {
-        let start = if !self.every.months_only()
-            && self.every.duration_us() > MICROSECONDS * SECONDS_IN_DAY
-        {
-            self.offset.add_us(t, tz)?
-        } else {
-            self.truncate_us(t, tz)?
-        };
+        let start = self.truncate_us(t, tz)?;
         let stop = self.period.add_us(start, tz)?;
         Ok(Bounds::new_checked(start, stop))
     }
 
     pub fn get_earliest_bounds_ms(&self, t: i64, tz: Option<&Tz>) -> PolarsResult<Bounds> {
-        let start = if !self.every.months_only()
-            && self.every.duration_ms() > MILLISECONDS * SECONDS_IN_DAY
-        {
-            self.offset.add_ms(t, tz)?
-        } else {
-            self.truncate_ms(t, tz)?
-        };
-
+        let start = self.truncate_ms(t, tz)?;
         let stop = self.period.add_ms(start, tz)?;
 
         Ok(Bounds::new_checked(start, stop))
     }
 
     pub(crate) fn estimate_overlapping_bounds_ns(&self, boundary: Bounds) -> usize {
         (boundary.duration() / self.every.duration_ns()
```

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-ops/Cargo.toml` & `polars_lts_cpu-0.18.3/local_dependencies/polars-ops/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -78,15 +78,15 @@
 semi_anti_join = ["polars-core/semi_anti_join"]
 list_take = []
 
 [dependencies.arrow]
 package = "arrow2"
 git = "https://github.com/jorgecarleitao/arrow2"
 # git = "https://github.com/ritchie46/arrow2"
-rev = "fb5e4d591c7149df590a330365fae55d2370962f"
+rev = "2d2e7053f9a50810bfe9cecff25ab39089aef98e"
 # path = "../arrow2"
 # branch = "polars_2023-05-25"
 version = "0.17"
 default-features = false
 features = [
   "compute_aggregate",
   "compute_arithmetics",
```

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-ops/LICENSE` & `polars_lts_cpu-0.18.3/local_dependencies/polars-io/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-ops/src/chunked_array/array/min_max.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-ops/src/chunked_array/array/min_max.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-ops/src/chunked_array/array/namespace.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-ops/src/chunked_array/array/namespace.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-ops/src/chunked_array/array/sum_mean.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-ops/src/chunked_array/array/sum_mean.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-ops/src/chunked_array/binary/namespace.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-ops/src/chunked_array/binary/namespace.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-ops/src/chunked_array/interpolate.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-ops/src/chunked_array/interpolate.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-ops/src/chunked_array/list/count.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-ops/src/chunked_array/list/count.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-ops/src/chunked_array/list/hash.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-ops/src/chunked_array/list/hash.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-ops/src/chunked_array/list/min_max.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-ops/src/chunked_array/list/min_max.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-ops/src/chunked_array/list/namespace.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-ops/src/chunked_array/list/namespace.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-ops/src/chunked_array/list/sum_mean.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-ops/src/chunked_array/list/sum_mean.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-ops/src/chunked_array/list/to_struct.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-ops/src/chunked_array/list/to_struct.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-ops/src/chunked_array/mod.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-ops/src/chunked_array/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-ops/src/chunked_array/nan_propagating_aggregate.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-ops/src/chunked_array/nan_propagating_aggregate.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-ops/src/chunked_array/set.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-ops/src/chunked_array/set.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-ops/src/chunked_array/strings/case.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-ops/src/chunked_array/strings/case.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-ops/src/chunked_array/strings/json_path.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-ops/src/chunked_array/strings/json_path.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-ops/src/chunked_array/strings/justify.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-ops/src/chunked_array/strings/justify.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-ops/src/chunked_array/strings/mod.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-ops/src/chunked_array/strings/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-ops/src/chunked_array/strings/namespace.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-ops/src/chunked_array/strings/namespace.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-ops/src/chunked_array/strings/replace.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-ops/src/chunked_array/strings/replace.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-ops/src/chunked_array/top_k.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-ops/src/chunked_array/top_k.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-ops/src/frame/join/merge_sorted.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-ops/src/frame/join/merge_sorted.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-ops/src/frame/join/mod.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-ops/src/frame/join/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-ops/src/frame/mod.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-ops/src/frame/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-ops/src/frame/pivot/mod.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-ops/src/frame/pivot/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-ops/src/frame/pivot/positioning.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-ops/src/frame/pivot/positioning.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-ops/src/series/ops/approx_algo/hyperloglogplus.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-ops/src/series/ops/approx_algo/hyperloglogplus.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-ops/src/series/ops/approx_unique.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-ops/src/series/ops/approx_unique.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-ops/src/series/ops/arg_min_max.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-ops/src/series/ops/arg_min_max.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-ops/src/series/ops/floor_divide.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-ops/src/series/ops/floor_divide.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-ops/src/series/ops/fused.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-ops/src/series/ops/fused.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-ops/src/series/ops/is_first.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-ops/src/series/ops/is_first.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-ops/src/series/ops/is_unique.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-ops/src/series/ops/is_unique.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-ops/src/series/ops/log.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-ops/src/series/ops/log.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-ops/src/series/ops/mod.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-ops/src/series/ops/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-ops/src/series/ops/rolling.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-ops/src/series/ops/rolling.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-ops/src/series/ops/search_sorted.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-ops/src/series/ops/search_sorted.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-ops/src/series/ops/to_dummies.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-ops/src/series/ops/to_dummies.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-ops/src/series/ops/various.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-ops/src/series/ops/various.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-io/Cargo.toml` & `polars_lts_cpu-0.18.3/local_dependencies/polars-io/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -82,15 +82,15 @@
 tokio = { version = "1.26.0", features = ["net"], optional = true }
 url = { version = "2.3.1", optional = true }
 
 [dependencies.arrow]
 package = "arrow2"
 git = "https://github.com/jorgecarleitao/arrow2"
 # git = "https://github.com/ritchie46/arrow2"
-rev = "fb5e4d591c7149df590a330365fae55d2370962f"
+rev = "2d2e7053f9a50810bfe9cecff25ab39089aef98e"
 # path = "../arrow2"
 # branch = "polars_2023-05-25"
 version = "0.17"
 default-features = false
 features = [
   "compute_aggregate",
   "compute_arithmetics",
```

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-io/LICENSE` & `polars_lts_cpu-0.18.3/local_dependencies/polars-arrow/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-io/src/avro/mod.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-io/src/avro/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-io/src/avro/read.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-io/src/avro/read.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-io/src/avro/write.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-io/src/avro/write.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-io/src/cloud/adaptors.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-io/src/cloud/adaptors.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-io/src/cloud/glob.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-io/src/cloud/glob.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-io/src/cloud/mod.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-io/src/cloud/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-io/src/csv/buffer.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-io/src/csv/buffer.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-io/src/csv/mod.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-io/src/csv/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-io/src/csv/parser.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-io/src/csv/parser.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-io/src/csv/read.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-io/src/csv/read.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-io/src/csv/read_impl/batched_mmap.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-io/src/csv/read_impl/batched_mmap.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-io/src/csv/read_impl/batched_read.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-io/src/csv/read_impl/batched_read.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-io/src/csv/read_impl/mod.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-io/src/csv/read_impl/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-io/src/csv/splitfields.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-io/src/csv/splitfields.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-io/src/csv/utils.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-io/src/csv/utils.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-io/src/csv/write.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-io/src/csv/write.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-io/src/csv/write_impl.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-io/src/csv/write_impl.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-io/src/ipc/ipc_file.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-io/src/ipc/ipc_file.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-io/src/ipc/ipc_stream.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-io/src/ipc/ipc_stream.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-io/src/ipc/mmap.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-io/src/ipc/mmap.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-io/src/ipc/write.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-io/src/ipc/write.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-io/src/ipc/write_async.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-io/src/ipc/write_async.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-io/src/json/mod.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-io/src/json/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-io/src/lib.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-io/src/lib.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-io/src/mmap.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-io/src/mmap.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-io/src/ndjson/buffer.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-io/src/ndjson/buffer.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-io/src/ndjson/core.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-io/src/ndjson/core.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-io/src/parquet/async_impl.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-io/src/parquet/async_impl.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-io/src/parquet/mmap.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-io/src/parquet/mmap.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-io/src/parquet/mod.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-io/src/parquet/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-io/src/parquet/predicates.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-io/src/parquet/predicates.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-io/src/parquet/read.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-io/src/parquet/read.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-io/src/parquet/read_impl.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-io/src/parquet/read_impl.rs`

 * *Files 3% similar despite different names*

```diff
@@ -243,22 +243,38 @@
     mut parallel: ParallelStrategy,
     row_count: Option<RowCount>,
     use_statistics: bool,
 ) -> PolarsResult<DataFrame> {
     let file_metadata = metadata
         .map(Ok)
         .unwrap_or_else(|| read::read_metadata(&mut reader))?;
-    let row_group_len = file_metadata.row_groups.len();
+    let n_row_groups = file_metadata.row_groups.len();
+
+    // if there are multiple row groups and categorical data
+    // we need a string cache
+    // we keep it alive until the end of the function
+    let _string_cache = if n_row_groups > 1 {
+        #[cfg(feature = "dtype-categorical")]
+        {
+            Some(polars_core::IUseStringCache::new())
+        }
+        #[cfg(not(feature = "dtype-categorical"))]
+        {
+            Some(0u8)
+        }
+    } else {
+        None
+    };
 
     let projection = projection
         .map(Cow::Borrowed)
         .unwrap_or_else(|| Cow::Owned((0usize..schema.fields.len()).collect::<Vec<_>>()));
 
     if let ParallelStrategy::Auto = parallel {
-        if row_group_len > projection.len() || row_group_len > POOL.current_num_threads() {
+        if n_row_groups > projection.len() || n_row_groups > POOL.current_num_threads() {
             parallel = ParallelStrategy::RowGroups;
         } else {
             parallel = ParallelStrategy::Columns;
         }
     }
 
     if let (ParallelStrategy::Columns, true) = (parallel, projection.len() == 1) {
@@ -269,15 +285,15 @@
     let bytes = reader.deref();
     let store = mmap::ColumnStore::Local(bytes);
     let dfs = match parallel {
         ParallelStrategy::Columns | ParallelStrategy::None => rg_to_dfs(
             &store,
             &mut 0,
             0,
-            row_group_len,
+            n_row_groups,
             &mut limit,
             &file_metadata,
             schema,
             predicate,
             row_count,
             parallel,
             &projection,
```

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-io/src/parquet/write.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-io/src/parquet/write.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-io/src/partition.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-io/src/partition.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-io/src/predicates.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-io/src/predicates.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-io/src/prelude.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-io/src/prelude.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-io/src/utils.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-io/src/utils.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-utils/Cargo.toml` & `polars_lts_cpu-0.18.3/local_dependencies/polars-utils/Cargo.toml`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-utils/LICENSE` & `polars_lts_cpu-0.18.3/local_dependencies/polars-pipe/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-utils/src/arena.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-utils/src/arena.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-utils/src/atomic.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-utils/src/atomic.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-utils/src/cell.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-utils/src/cell.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-utils/src/contention_pool.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-utils/src/contention_pool.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-utils/src/functions.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-utils/src/functions.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-utils/src/iter/enumerate_idx.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-utils/src/iter/enumerate_idx.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-utils/src/macros.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-utils/src/macros.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-utils/src/slice.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-utils/src/slice.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-utils/src/sort.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-utils/src/sort.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-utils/src/sync.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-utils/src/sync.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-utils/src/unwrap.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-utils/src/unwrap.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-utils/src/wasm.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-utils/src/wasm.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-sql/Cargo.toml` & `polars_lts_cpu-0.18.3/local_dependencies/polars-sql/Cargo.toml`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-sql/LICENSE` & `polars_lts_cpu-0.18.3/local_dependencies/polars-sql/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-sql/src/context.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-sql/src/context.rs`

 * *Files 2% similar despite different names*

```diff
@@ -3,17 +3,18 @@
 
 use polars_arrow::error::to_compute_err;
 use polars_core::prelude::*;
 use polars_lazy::prelude::*;
 use polars_plan::prelude::*;
 use polars_plan::utils::expressions_to_schema;
 use sqlparser::ast::{
-    Distinct, ExcludeSelectItem, Expr as SqlExpr, FunctionArg, JoinOperator, ObjectName, Offset,
-    OrderByExpr, Query, Select, SelectItem, SetExpr, SetOperator, SetQuantifier, Statement,
-    TableAlias, TableFactor, TableWithJoins, Value as SQLValue, WildcardAdditionalOptions,
+    Distinct, ExcludeSelectItem, Expr as SqlExpr, FunctionArg, JoinOperator, ObjectName,
+    ObjectType, Offset, OrderByExpr, Query, Select, SelectItem, SetExpr, SetOperator,
+    SetQuantifier, Statement, TableAlias, TableFactor, TableWithJoins, Value as SQLValue,
+    WildcardAdditionalOptions,
 };
 use sqlparser::dialect::GenericDialect;
 use sqlparser::parser::{Parser, ParserOptions};
 
 use crate::sql_expr::{parse_sql_expr, process_join_constraint};
 use crate::table_functions::PolarsTableFunctions;
 
@@ -122,14 +123,18 @@
 
     pub(crate) fn execute_statement(&mut self, stmt: &Statement) -> PolarsResult<LazyFrame> {
         let ast = stmt;
         Ok(match ast {
             Statement::Query(query) => self.execute_query(query)?,
             stmt @ Statement::ShowTables { .. } => self.execute_show_tables(stmt)?,
             stmt @ Statement::CreateTable { .. } => self.execute_create_table(stmt)?,
+            stmt @ Statement::Drop {
+                object_type: ObjectType::Table,
+                ..
+            } => self.execute_drop_table(stmt)?,
             stmt @ Statement::Explain { .. } => self.execute_explain(stmt)?,
             _ => polars_bail!(
                 ComputeError: "SQL statement type {:?} is not supported", ast,
             ),
         })
     }
 
@@ -161,28 +166,28 @@
     fn process_union(
         &mut self,
         left: &SetExpr,
         right: &SetExpr,
         quantifier: &SetQuantifier,
         query: &Query,
     ) -> PolarsResult<LazyFrame> {
+        let left = self.process_set_expr(left, query)?;
+        let right = self.process_set_expr(right, query)?;
+        let concatenated = polars_lazy::dsl::concat(
+            vec![left, right],
+            UnionArgs {
+                parallel: true,
+                ..Default::default()
+            },
+        );
         match quantifier {
             // UNION ALL
-            SetQuantifier::All => {
-                let left = self.process_set_expr(left, query)?;
-                let right = self.process_set_expr(right, query)?;
-                polars_lazy::dsl::concat(vec![left, right], false, true)
-            }
+            SetQuantifier::All => concatenated,
             // UNION DISTINCT | UNION
-            _ => {
-                let left = self.process_set_expr(left, query)?;
-                let right = self.process_set_expr(right, query)?;
-                Ok(polars_lazy::dsl::concat(vec![left, right], true, true)?
-                    .unique(None, UniqueKeepStrategy::Any))
-            }
+            _ => concatenated.map(|lf| lf.unique(None, UniqueKeepStrategy::Any)),
         }
     }
     // EXPLAIN SELECT * FROM DF
     fn execute_explain(&mut self, stmt: &Statement) -> PolarsResult<LazyFrame> {
         match stmt {
             Statement::Explain { statement, .. } => {
                 let lf = self.execute_statement(statement)?;
@@ -200,14 +205,26 @@
     /// SHOW TABLES
     fn execute_show_tables(&mut self, _: &Statement) -> PolarsResult<LazyFrame> {
         let tables = Series::new("name", self.get_tables());
         let df = DataFrame::new(vec![tables])?;
         Ok(df.lazy())
     }
 
+    fn execute_drop_table(&mut self, stmt: &Statement) -> PolarsResult<LazyFrame> {
+        match stmt {
+            Statement::Drop { names, .. } => {
+                for name in names {
+                    self.table_map.remove(&name.to_string());
+                }
+                Ok(DataFrame::empty().lazy())
+            }
+            _ => unreachable!(),
+        }
+    }
+
     fn register_ctes(&mut self, query: &Query) -> PolarsResult<()> {
         if let Some(with) = &query.with {
             if with.recursive {
                 polars_bail!(ComputeError: "Recursive CTEs are not supported")
             }
             for cte in &with.cte_tables {
                 let cte_name = cte.alias.name.to_string();
```

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-sql/src/functions.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-sql/src/functions.rs`

 * *Files 0% similar despite different names*

```diff
@@ -229,14 +229,15 @@
     /// SQL 'array_contains' function
     /// Returns true if the array contains the value
     /// ```sql
     /// SELECT ARRAY_CONTAINS(column_1, 'foo') from df;
     /// ```
     ArrayContains,
 }
+
 impl PolarsSqlFunctions {
     pub(crate) fn keywords() -> &'static [&'static str] {
         &[
             "abs",
             "acos",
             "array_contains",
             "array_get",
```

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-sql/src/keywords.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-sql/src/keywords.rs`

 * *Files 2% similar despite different names*

```diff
@@ -18,20 +18,23 @@
         keywords::AND,
         keywords::ARRAY,
         keywords::AS,
         keywords::AS,
         keywords::ASC,
         keywords::BOOLEAN,
         keywords::BY,
+        keywords::CASE,
         keywords::CREATE,
         keywords::DATE,
         keywords::DATETIME,
         keywords::DESC,
         keywords::DISTINCT,
         keywords::DOUBLE,
+        keywords::DROP,
+        keywords::EXCLUDE,
         keywords::FLOAT,
         keywords::FROM,
         keywords::FULL,
         keywords::GROUP,
         keywords::HAVING,
         keywords::IN,
         keywords::INNER,
@@ -47,23 +50,21 @@
         keywords::ORDER,
         keywords::OUTER,
         keywords::RIGHT,
         keywords::SELECT,
         keywords::SHOW,
         keywords::TABLE,
         keywords::TABLES,
+        keywords::THEN,
         keywords::TIME,
         keywords::USING,
         keywords::VARCHAR,
+        keywords::WHEN,
         keywords::WHERE,
         keywords::WITH,
-        keywords::CASE,
-        keywords::WHEN,
-        keywords::THEN,
-        keywords::EXCLUDE,
     ];
     keywords.extend_from_slice(sql_keywords);
     keywords
 }
 
 /// Get a list of all function names that are supported by Polars SQL
 pub fn all_functions() -> Vec<&'static str> {
```

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-sql/src/sql_expr.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-sql/src/sql_expr.rs`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 use polars_arrow::error::to_compute_err;
 use polars_core::prelude::*;
 use polars_lazy::dsl::Expr;
 use polars_lazy::prelude::*;
-use polars_plan::prelude::{col, when};
+use polars_plan::prelude::{col, lit, when};
 use sqlparser::ast::{
     ArrayAgg, BinaryOperator as SQLBinaryOperator, BinaryOperator, DataType as SQLDataType,
     Expr as SqlExpr, Function as SQLFunction, JoinConstraint, OrderByExpr, TrimWhereField,
     UnaryOperator, Value as SqlValue,
 };
 use sqlparser::dialect::GenericDialect;
 use sqlparser::parser::{Parser, ParserOptions};
@@ -71,14 +71,20 @@
             SqlExpr::Function(function) => self.visit_function(function),
             SqlExpr::Identifier(ident) => self.visit_identifier(ident),
             SqlExpr::InList {
                 expr,
                 list,
                 negated,
             } => self.visit_is_in(expr, list, *negated),
+            SqlExpr::IsDistinctFrom(e1, e2) => {
+                Ok(self.visit_expr(e1)?.neq_missing(self.visit_expr(e2)?))
+            }
+            SqlExpr::IsNotDistinctFrom(e1, e2) => {
+                Ok(self.visit_expr(e1)?.eq_missing(self.visit_expr(e2)?))
+            }
             SqlExpr::IsFalse(expr) => Ok(self.visit_expr(expr)?.eq(lit(false))),
             SqlExpr::IsNotFalse(expr) => Ok(self.visit_expr(expr)?.eq(lit(false)).not()),
             SqlExpr::IsNotNull(expr) => Ok(self.visit_expr(expr)?.is_not_null()),
             SqlExpr::IsNotTrue(expr) => Ok(self.visit_expr(expr)?.eq(lit(true)).not()),
             SqlExpr::IsNull(expr) => Ok(self.visit_expr(expr)?.is_null()),
             SqlExpr::IsTrue(expr) => Ok(self.visit_expr(expr)?.eq(lit(true))),
             SqlExpr::Nested(expr) => self.visit_expr(expr),
@@ -129,14 +135,15 @@
 
     fn visit_unary_op(&self, op: &UnaryOperator, expr: &SqlExpr) -> PolarsResult<Expr> {
         let expr = self.visit_expr(expr)?;
         Ok(match op {
             UnaryOperator::Plus => lit(0) + expr,
             UnaryOperator::Minus => lit(0) - expr,
             UnaryOperator::Not => expr.not(),
+            UnaryOperator::PGSquareRoot => expr.pow(0.5),
             other => polars_bail!(InvalidOperation: "Unary operator {:?} is not supported", other),
         })
     }
 
     /// Visit a single identifier
     ///
     /// e.g. column
@@ -154,29 +161,54 @@
         right: &SqlExpr,
     ) -> PolarsResult<Expr> {
         let left = self.visit_expr(left)?;
         let right = self.visit_expr(right)?;
         Ok(match op {
             SQLBinaryOperator::And => left.and(right),
             SQLBinaryOperator::Divide => left / right,
+            SQLBinaryOperator::DuckIntegerDivide => left.floor_div(right).cast(DataType::Int64),
             SQLBinaryOperator::Eq => left.eq(right),
             SQLBinaryOperator::Gt => left.gt(right),
             SQLBinaryOperator::GtEq => left.gt_eq(right),
             SQLBinaryOperator::Lt => left.lt(right),
             SQLBinaryOperator::LtEq => left.lt_eq(right),
             SQLBinaryOperator::Minus => left - right,
             SQLBinaryOperator::Modulo => left % right,
             SQLBinaryOperator::Multiply => left * right,
             SQLBinaryOperator::NotEq => left.eq(right).not(),
             SQLBinaryOperator::Or => left.or(right),
             SQLBinaryOperator::Plus => left + right,
+            SQLBinaryOperator::Spaceship => left.eq_missing(right),
             SQLBinaryOperator::StringConcat => {
                 left.cast(DataType::Utf8) + right.cast(DataType::Utf8)
             }
             SQLBinaryOperator::Xor => left.xor(right),
+            // ----
+            // Regular expression operators
+            // ----
+            SQLBinaryOperator::PGRegexMatch => match right {
+                Expr::Literal(LiteralValue::Utf8(_)) => left.str().contains(right, true),
+                _ => polars_bail!(ComputeError: "Invalid pattern for '~' operator: {:?}", right),
+            },
+            SQLBinaryOperator::PGRegexNotMatch => match right {
+                Expr::Literal(LiteralValue::Utf8(_)) => left.str().contains(right, true).not(),
+                _ => polars_bail!(ComputeError: "Invalid pattern for '!~' operator: {:?}", right),
+            },
+            SQLBinaryOperator::PGRegexIMatch => match right {
+                Expr::Literal(LiteralValue::Utf8(pat)) => {
+                    left.str().contains(lit(format!("(?i){}", pat)), true)
+                }
+                _ => polars_bail!(ComputeError: "Invalid pattern for '~*' operator: {:?}", right),
+            },
+            SQLBinaryOperator::PGRegexNotIMatch => match right {
+                Expr::Literal(LiteralValue::Utf8(pat)) => {
+                    left.str().contains(lit(format!("(?i){}", pat)), true).not()
+                }
+                _ => polars_bail!(ComputeError: "Invalid pattern for '!~*' operator: {:?}", right),
+            },
             other => polars_bail!(ComputeError: "SQL operator {:?} is not yet supported", other),
         })
     }
 
     /// Visit a SQL function
     ///
     /// e.g. SUM(column) or COUNT(*)
@@ -215,15 +247,15 @@
             SqlValue::Number(s, _) => {
                 // Check for existence of decimal separator dot
                 if s.contains('.') {
                     s.parse::<f64>().map(lit).map_err(|_| ())
                 } else {
                     s.parse::<i64>().map(lit).map_err(|_| ())
                 }
-                .map_err(|_| polars_err!(ComputeError: "cannot parse literal: {:?}"))?
+                .map_err(|_| polars_err!(ComputeError: "cannot parse literal: {:?}", s))?
             }
             SqlValue::SingleQuotedString(s) => lit(s.clone()),
             other => polars_bail!(ComputeError: "SQL value {:?} is not yet supported", other),
         })
     }
 
     // similar to visit_literal, but returns an AnyValue instead of Expr
```

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-sql/src/table_functions.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-sql/src/table_functions.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-sql/tests/functions_cumulative.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-sql/tests/functions_cumulative.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-sql/tests/functions_io.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-sql/tests/functions_io.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-sql/tests/functions_math.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-sql/tests/functions_math.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-sql/tests/functions_meta.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-sql/tests/functions_meta.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-sql/tests/functions_string.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-sql/tests/functions_string.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-sql/tests/iss_7436.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-sql/tests/iss_7436.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-sql/tests/iss_7437.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-sql/tests/iss_7437.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-sql/tests/iss_7440.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-sql/tests/iss_7440.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-sql/tests/iss_8395.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-sql/tests/iss_8395.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-sql/tests/iss_8419.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-sql/tests/iss_8419.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-sql/tests/ops_distinct_on.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-sql/tests/ops_distinct_on.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-sql/tests/simple_exprs.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-sql/tests/simple_exprs.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-sql/tests/statements.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-sql/tests/statements.rs`

 * *Files 10% similar despite different names*

```diff
@@ -128,15 +128,34 @@
 
     let sql = r#"
     SELECT * FROM test
     UNION ALL (
         SELECT * FROM test2
     )
     "#;
-    let expected = polars_lazy::dsl::concat(vec![df1.lazy(), df2.lazy()], false, true)
-        .unwrap()
-        .collect()
-        .unwrap();
+    let expected = polars_lazy::dsl::concat(
+        vec![df1.lazy(), df2.lazy()],
+        UnionArgs {
+            rechunk: false,
+            parallel: true,
+            ..Default::default()
+        },
+    )
+    .unwrap()
+    .collect()
+    .unwrap();
 
     let actual = ctx.execute(sql).unwrap().collect().unwrap();
     assert!(actual.frame_equal(&expected));
 }
+
+#[test]
+fn test_drop_table() {
+    let mut ctx = create_ctx();
+    let sql = r#"
+    DROP TABLE df
+    "#;
+    let actual = ctx.execute(sql);
+    assert!(actual.is_ok());
+    let res = ctx.execute("SELECT * FROM df");
+    assert!(res.is_err());
+}
```

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-row/Cargo.toml` & `polars_lts_cpu-0.18.3/local_dependencies/polars-row/Cargo.toml`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 polars-error = { version = "0.30.0", path = "../polars-error" }
 polars-utils = { version = "0.30.0", path = "../polars-utils" }
 
 [dependencies.arrow]
 package = "arrow2"
 git = "https://github.com/jorgecarleitao/arrow2"
 # git = "https://github.com/ritchie46/arrow2"
-rev = "fb5e4d591c7149df590a330365fae55d2370962f"
+rev = "2d2e7053f9a50810bfe9cecff25ab39089aef98e"
 # path = "../arrow2"
 # branch = "polars_2023-05-25"
 version = "0.17"
 default-features = false
 features = [
   "compute_aggregate",
   "compute_arithmetics",
```

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-row/LICENSE` & `polars_lts_cpu-0.18.3/local_dependencies/polars/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-row/src/encode.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-row/src/encode.rs`

 * *Files 21% similar despite different names*

```diff
@@ -1,66 +1,128 @@
-use arrow::array::{Array, BinaryArray, BooleanArray, DictionaryArray, PrimitiveArray, Utf8Array};
+use arrow::array::{
+    Array, BinaryArray, BooleanArray, DictionaryArray, PrimitiveArray, StructArray, Utf8Array,
+};
+use arrow::compute::cast::cast;
 use arrow::datatypes::{DataType as ArrowDataType, DataType};
 use arrow::types::NativeType;
 
-use crate::encodings::fixed::FixedLengthEncoding;
+use crate::fixed::FixedLengthEncoding;
 use crate::row::{RowsEncoded, SortField};
 use crate::{with_match_arrow_primitive_type, ArrayRef};
 
 pub fn convert_columns(columns: &[ArrayRef], fields: &[SortField]) -> RowsEncoded {
-    assert_eq!(fields.len(), columns.len());
+    let mut rows = RowsEncoded::new(vec![], vec![]);
+    convert_columns_amortized(columns, fields, &mut rows);
+    rows
+}
 
-    let mut rows = allocate_rows_buf(columns);
-    for (arr, field) in columns.iter().zip(fields.iter()) {
-        // Safety:
-        // we allocated rows with enough bytes.
-        unsafe { encode_array(&**arr, field, &mut rows) }
-    }
+pub fn convert_columns_no_order(columns: &[ArrayRef]) -> RowsEncoded {
+    let mut rows = RowsEncoded::new(vec![], vec![]);
+    convert_columns_amortized_no_order(columns, &mut rows);
     rows
 }
 
+pub fn convert_columns_amortized_no_order(columns: &[ArrayRef], rows: &mut RowsEncoded) {
+    convert_columns_amortized(
+        columns,
+        std::iter::repeat(&SortField::default()).take(columns.len()),
+        rows,
+    );
+}
+
+pub fn convert_columns_amortized<'a, I: IntoIterator<Item = &'a SortField>>(
+    columns: &'a [ArrayRef],
+    fields: I,
+    rows: &mut RowsEncoded,
+) {
+    let fields = fields.into_iter();
+    assert_eq!(fields.size_hint().0, columns.len());
+    if columns
+        .iter()
+        .any(|arr| matches!(arr.data_type(), DataType::Struct(_) | DataType::LargeUtf8))
+    {
+        let mut flattened_columns = Vec::with_capacity(columns.len() * 5);
+        let mut flattened_fields = Vec::with_capacity(columns.len() * 5);
+
+        for (arr, field) in columns.iter().zip(fields) {
+            match arr.data_type() {
+                DataType::Struct(_) => {
+                    let arr = arr.as_any().downcast_ref::<StructArray>().unwrap();
+                    for arr in arr.values() {
+                        flattened_columns.push(arr.clone() as ArrayRef);
+                        flattened_fields.push(field.clone())
+                    }
+                }
+                DataType::LargeUtf8 => {
+                    flattened_columns.push(
+                        cast(arr.as_ref(), &DataType::LargeBinary, Default::default()).unwrap(),
+                    );
+                    flattened_fields.push(field.clone());
+                }
+                _ => {
+                    flattened_columns.push(arr.clone());
+                    flattened_fields.push(field.clone());
+                }
+            }
+        }
+        allocate_rows_buf(&flattened_columns, &mut rows.values, &mut rows.offsets);
+        for (arr, field) in flattened_columns.iter().zip(flattened_fields.iter()) {
+            // Safety:
+            // we allocated rows with enough bytes.
+            unsafe { encode_array(&**arr, field, rows) }
+        }
+    } else {
+        allocate_rows_buf(columns, &mut rows.values, &mut rows.offsets);
+        for (arr, field) in columns.iter().zip(fields) {
+            // Safety:
+            // we allocated rows with enough bytes.
+            unsafe { encode_array(&**arr, field, rows) }
+        }
+    }
+}
+
 fn encode_primitive<T: NativeType + FixedLengthEncoding>(
     arr: &PrimitiveArray<T>,
     field: &SortField,
     out: &mut RowsEncoded,
 ) {
     if arr.null_count() == 0 {
-        crate::encodings::fixed::encode_slice(arr.values().as_slice(), out, field);
+        crate::fixed::encode_slice(arr.values().as_slice(), out, field);
     } else {
-        crate::encodings::fixed::encode_iter(arr.into_iter().map(|v| v.copied()), out, field);
+        crate::fixed::encode_iter(arr.into_iter().map(|v| v.copied()), out, field);
     }
 }
 
 /// Ecnodes an array into `out`
 ///
 /// # Safety
 /// `out` must have enough bytes allocated otherwise it will be out of bounds.
 unsafe fn encode_array(array: &dyn Array, field: &SortField, out: &mut RowsEncoded) {
     match array.data_type() {
         DataType::Boolean => {
             let array = array.as_any().downcast_ref::<BooleanArray>().unwrap();
-            crate::encodings::fixed::encode_iter(array.into_iter(), out, field);
+            crate::fixed::encode_iter(array.into_iter(), out, field);
         }
         DataType::LargeBinary => {
             let array = array.as_any().downcast_ref::<BinaryArray<i64>>().unwrap();
-            crate::encodings::variable::encode_iter(array.into_iter(), out, field)
+            crate::variable::encode_iter(array.into_iter(), out, field)
         }
         DataType::LargeUtf8 => {
             panic!("should be cast to binary")
         }
         DataType::Dictionary(_, _, _) => {
             let array = array
                 .as_any()
                 .downcast_ref::<DictionaryArray<u32>>()
                 .unwrap();
             let iter = array
                 .iter_typed::<Utf8Array<i64>>()
                 .unwrap()
                 .map(|opt_s| opt_s.map(|s| s.as_bytes()));
-            crate::encodings::variable::encode_iter(iter, out, field)
+            crate::variable::encode_iter(iter, out, field)
         }
         dt => {
             with_match_arrow_primitive_type!(dt, |$T| {
                 let array = array.as_any().downcast_ref::<PrimitiveArray<$T>>().unwrap();
                 encode_primitive(array, field, out);
             })
         }
@@ -76,19 +138,20 @@
         UInt64 => u64::ENCODED_LEN,
         Int8 => i8::ENCODED_LEN,
         Int16 => i16::ENCODED_LEN,
         Int32 => i32::ENCODED_LEN,
         Int64 => i64::ENCODED_LEN,
         Float32 => f32::ENCODED_LEN,
         Float64 => f64::ENCODED_LEN,
-        _ => unimplemented!(),
+        Boolean => bool::ENCODED_LEN,
+        dt => unimplemented!("{dt:?}"),
     }
 }
 
-pub fn allocate_rows_buf(columns: &[ArrayRef]) -> RowsEncoded {
+pub fn allocate_rows_buf(columns: &[ArrayRef], values: &mut Vec<u8>, offsets: &mut Vec<usize>) {
     let has_variable = columns.iter().any(|arr| {
         matches!(
             arr.data_type(),
             ArrowDataType::LargeBinary | ArrowDataType::Dictionary(_, _, _)
         )
     });
 
@@ -106,101 +169,111 @@
                     0
                 } else {
                     encoded_size(arr.data_type())
                 }
             })
             .sum();
 
-        let mut lengths = vec![row_size_fixed; num_rows];
+        offsets.clear();
+        offsets.reserve(num_rows + 1);
+        offsets.resize(num_rows, row_size_fixed);
+
+        // first write lengths to this buffer
+        let lengths = offsets;
 
         // for the variable length columns we must iterate to determine the length per row location
         for array in columns.iter() {
             match array.data_type() {
                 ArrowDataType::LargeBinary => {
                     let array = array.as_any().downcast_ref::<BinaryArray<i64>>().unwrap();
                     for (opt_val, row_length) in array.into_iter().zip(lengths.iter_mut()) {
-                        *row_length += crate::encodings::variable::encoded_len(opt_val)
+                        *row_length += crate::variable::encoded_len(opt_val)
                     }
                 }
                 ArrowDataType::Dictionary(_, _, _) => {
                     let array = array
                         .as_any()
                         .downcast_ref::<DictionaryArray<u32>>()
                         .unwrap();
                     let iter = array
                         .iter_typed::<Utf8Array<i64>>()
                         .unwrap()
                         .map(|opt_s| opt_s.map(|s| s.as_bytes()));
                     for (opt_val, row_length) in iter.zip(lengths.iter_mut()) {
-                        *row_length += crate::encodings::variable::encoded_len(opt_val)
+                        *row_length += crate::variable::encoded_len(opt_val)
                     }
                 }
                 _ => {
                     // the rest is fixed
                 }
             }
         }
-        let mut offsets = Vec::with_capacity(num_rows + 1);
+        // now we use the lengths and the same buffer to determine the offsets
+        let offsets = lengths;
+        // we write lagged because the offsets will be written by the encoding column
         let mut current_offset = 0_usize;
-        offsets.push(current_offset);
+        let mut lagged_offset = 0_usize;
 
-        for length in lengths {
-            offsets.push(current_offset);
-            #[cfg(target_pointer_width = "64")]
-            {
-                // don't do overflow check, counting exabytes here.
-                current_offset += length;
-            }
-            #[cfg(not(target_pointer_width = "64"))]
-            {
-                current_offset = current_offset.checked_add(length).expect("overflow");
-            }
+        for length in offsets.iter_mut() {
+            let to_write = lagged_offset;
+            lagged_offset = current_offset;
+            current_offset += *length;
+
+            *length = to_write;
         }
+        // ensure we have len + 1 offsets
+        offsets.push(lagged_offset);
 
+        values.clear();
         // todo! allocate uninit
-        let buf = vec![0u8; current_offset];
-        RowsEncoded::new(buf, offsets)
+        values.resize(current_offset, 0u8);
     } else {
         let row_size: usize = columns
             .iter()
             .map(|arr| encoded_size(arr.data_type()))
             .sum();
         let n_bytes = num_rows * row_size;
         // todo! allocate uninit
-        let buf = vec![0u8; n_bytes];
+        if values.capacity() == 0 {
+            // it is faster to allocate zeroed
+            // so if the capacity is 0, we alloc
+            *values = vec![0u8; n_bytes]
+        } else {
+            values.resize(n_bytes, 0u8);
+        }
 
         // note that offsets are shifted to the left
         // assume 2 fields with a len of 1
         // e.g. in arrow we would have 0, 2, 4, 6
 
         // now we write 0, 0, 2, 4
 
         // and when we encode field 1, we update the offset
         // so that becomes: 0, 1, 3, 5
 
         // and when the final field, field 2 is written
         // the offsets are correct:
         // 0, 2, 4, 6
-        let mut offsets = Vec::with_capacity(num_rows + 1);
+        offsets.clear();
+        offsets.reserve(num_rows + 1);
         let mut current_offset = 0;
         offsets.push(current_offset);
         for _ in 0..num_rows {
             offsets.push(current_offset);
             current_offset += row_size;
         }
-        RowsEncoded::new(buf, offsets)
     }
 }
 
 #[cfg(test)]
 mod test {
     use arrow::array::Utf8Array;
 
     use super::*;
-    use crate::encodings::variable::{BLOCK_SIZE, EMPTY_SENTINEL, NON_EMPTY_SENTINEL};
+    use crate::variable::{BLOCK_SIZE, EMPTY_SENTINEL, NON_EMPTY_SENTINEL};
 
     #[test]
     fn test_str_encode() {
         let sentence = "The black cat walked under a ladder but forget it's milk so it ...";
         let arr =
             Utf8Array::<i64>::from_iter([Some("a"), Some(""), Some("meep"), Some(sentence), None]);
```

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-row/src/encodings/variable.rs` & `polars_lts_cpu-0.18.3/src/arrow_interop/to_rust.rs`

 * *Files 27% similar despite different names*

```diff
@@ -1,137 +1,106 @@
-//! Variable length values are encoded as
-//!
-//! - single `0_u8` if null
-//! - single `1_u8` if empty array
-//! - `2_u8` if not empty, followed by one or more blocks
-//!
-//! where a block is encoded as
-//!
-//! - [`BLOCK_SIZE`] bytes of string data, padded with 0s
-//! - `0xFF_u8` if this is not the last block for this string
-//! - otherwise the length of the block as a `u8`
-
-use polars_utils::slice::GetSaferUnchecked;
-
-use crate::encodings::fixed::null_sentinel;
-use crate::row::RowsEncoded;
-use crate::SortField;
-
-/// The block size of the variable length encoding
-pub(crate) const BLOCK_SIZE: usize = 32;
-
-/// The continuation token.
-pub(crate) const BLOCK_CONTINUATION_TOKEN: u8 = 0xFF;
-
-/// Indicates an empty string
-pub(crate) const EMPTY_SENTINEL: u8 = 1;
-
-/// Indicates a non-empty string
-pub(crate) const NON_EMPTY_SENTINEL: u8 = 2;
-
-/// Returns the ceil of `value`/`divisor`
-#[inline]
-pub fn ceil(value: usize, divisor: usize) -> usize {
-    // Rewrite as `value.div_ceil(&divisor)` after
-    // https://github.com/rust-lang/rust/issues/88581 is merged.
-    value / divisor + (0 != value % divisor) as usize
-}
-
-#[inline]
-fn padded_length(a: usize) -> usize {
-    1 + ceil(a, BLOCK_SIZE) * (BLOCK_SIZE + 1)
-}
-
-#[inline]
-fn padded_length_opt(a: Option<usize>) -> usize {
-    if let Some(a) = a {
-        padded_length(a)
-    } else {
-        1
+use polars_core::export::rayon::prelude::*;
+use polars_core::prelude::*;
+use polars_core::utils::accumulate_dataframes_vertical_unchecked;
+use polars_core::utils::arrow::ffi;
+use polars_core::POOL;
+use pyo3::ffi::Py_uintptr_t;
+use pyo3::prelude::*;
+use pyo3::types::PyList;
+
+use crate::error::PyPolarsErr;
+
+pub fn field_to_rust(obj: &PyAny) -> PyResult<Field> {
+    let schema = Box::new(ffi::ArrowSchema::empty());
+    let schema_ptr = &*schema as *const ffi::ArrowSchema;
+
+    // make the conversion through PyArrow's private API
+    obj.call_method1("_export_to_c", (schema_ptr as Py_uintptr_t,))?;
+    let field = unsafe { ffi::import_field_from_c(schema.as_ref()).map_err(PyPolarsErr::from)? };
+    Ok((&field).into())
+}
+
+// PyList<Field> which you get by calling `list(schema)`
+pub fn pyarrow_schema_to_rust(obj: &PyList) -> PyResult<Schema> {
+    obj.into_iter().map(field_to_rust).collect()
+}
+
+pub fn array_to_rust(obj: &PyAny) -> PyResult<ArrayRef> {
+    // prepare a pointer to receive the Array struct
+    let array = Box::new(ffi::ArrowArray::empty());
+    let schema = Box::new(ffi::ArrowSchema::empty());
+
+    let array_ptr = &*array as *const ffi::ArrowArray;
+    let schema_ptr = &*schema as *const ffi::ArrowSchema;
+
+    // make the conversion through PyArrow's private API
+    // this changes the pointer's memory and is thus unsafe. In particular, `_export_to_c` can go out of bounds
+    obj.call_method1(
+        "_export_to_c",
+        (array_ptr as Py_uintptr_t, schema_ptr as Py_uintptr_t),
+    )?;
+
+    unsafe {
+        let field = ffi::import_field_from_c(schema.as_ref()).map_err(PyPolarsErr::from)?;
+        let array = ffi::import_array_from_c(*array, field.data_type).map_err(PyPolarsErr::from)?;
+        Ok(array)
     }
 }
 
-#[inline]
-pub fn encoded_len(a: Option<&[u8]>) -> usize {
-    padded_length_opt(a.map(|v| v.len()))
-}
-
-/// Encode one strings/bytes object and return the written length.
-///
-/// # Safety
-/// `out` must have allocated enough room
-unsafe fn encode_one(out: &mut [u8], val: Option<&[u8]>, field: &SortField) -> usize {
-    match val {
-        Some(val) if val.is_empty() => {
-            let byte = if field.descending {
-                !EMPTY_SENTINEL
+pub fn to_rust_df(rb: &[&PyAny]) -> PyResult<DataFrame> {
+    let schema = rb
+        .get(0)
+        .ok_or_else(|| PyPolarsErr::Other("empty table".into()))?
+        .getattr("schema")?;
+    let names = schema.getattr("names")?.extract::<Vec<String>>()?;
+
+    let dfs = rb
+        .iter()
+        .map(|rb| {
+            let mut run_parallel = false;
+
+            let columns = (0..names.len())
+                .map(|i| {
+                    let array = rb.call_method1("column", (i,))?;
+                    let arr = array_to_rust(array)?;
+                    run_parallel |= matches!(
+                        arr.data_type(),
+                        ArrowDataType::Utf8 | ArrowDataType::Dictionary(_, _, _)
+                    );
+                    Ok(arr)
+                })
+                .collect::<PyResult<Vec<_>>>()?;
+
+            // we parallelize this part because we can have dtypes that are not zero copy
+            // for instance utf8 -> large-utf8
+            // dict encoded to categorical
+            let columns = if run_parallel {
+                POOL.install(|| {
+                    columns
+                        .into_par_iter()
+                        .enumerate()
+                        .map(|(i, arr)| {
+                            let s = Series::try_from((names[i].as_str(), arr))
+                                .map_err(PyPolarsErr::from)?;
+                            Ok(s)
+                        })
+                        .collect::<PyResult<Vec<_>>>()
+                })
             } else {
-                EMPTY_SENTINEL
-            };
-            *out.get_unchecked_release_mut(0) = byte;
-            1
-        }
-        Some(val) => {
-            let block_count = ceil(val.len(), BLOCK_SIZE);
-            let end_offset = 1 + block_count * (BLOCK_SIZE + 1);
-
-            let dst = out.get_unchecked_release_mut(..end_offset);
-
-            // Write `2_u8` to demarcate as non-empty, non-null string
-            *dst.get_unchecked_release_mut(0) = NON_EMPTY_SENTINEL;
-
-            let src_chunks = val.chunks_exact(BLOCK_SIZE);
-            let src_remainder = src_chunks.remainder();
-
-            // + 1 is for the BLOCK CONTINUATION TOKEN
-            let dst_chunks = dst
-                .get_unchecked_release_mut(1..)
-                .chunks_exact_mut(BLOCK_SIZE + 1);
-
-            for (src, dst) in src_chunks.zip(dst_chunks) {
-                // we copy src.len() that leaves 1 bytes for the continuation tkn.
-                std::ptr::copy_nonoverlapping(src.as_ptr(), dst.as_mut_ptr(), src.len());
-                // Indicate that there are further blocks to follow
-                *dst.get_unchecked_release_mut(BLOCK_SIZE) = BLOCK_CONTINUATION_TOKEN;
-            }
-
-            if src_remainder.is_empty() {
-                // overwrite the latest continuation marker.
-                // replace the "there is another block" with
-                // "we are finished this, this is the length of this block"
-                *dst.last_mut().unwrap_unchecked() = BLOCK_SIZE as u8;
-            } else {
-                // get the last block
-                let start_offset = 1 + (block_count - 1) * (BLOCK_SIZE + 1);
-                let last_dst = dst.get_unchecked_release_mut(start_offset..);
-                std::ptr::copy_nonoverlapping(
-                    src_remainder.as_ptr(),
-                    last_dst.as_mut_ptr(),
-                    src_remainder.len(),
-                );
-                *dst.last_mut().unwrap_unchecked() = src_remainder.len() as u8;
-            }
-
-            if field.descending {
-                for byte in dst {
-                    *byte = !*byte;
-                }
-            }
-            end_offset
-        }
-        None => {
-            *out.get_unchecked_release_mut(0) = null_sentinel(field);
-            1
-        }
-    }
-}
-pub(crate) unsafe fn encode_iter<'a, I: Iterator<Item = Option<&'a [u8]>>>(
-    input: I,
-    out: &mut RowsEncoded,
-    field: &SortField,
-) {
-    for (offset, opt_value) in out.offsets.iter_mut().skip(1).zip(input) {
-        let dst = out.buf.get_unchecked_release_mut(*offset..);
-        let written_len = encode_one(dst, opt_value, field);
-        *offset += written_len;
-    }
+                columns
+                    .into_iter()
+                    .enumerate()
+                    .map(|(i, arr)| {
+                        let s = Series::try_from((names[i].as_str(), arr))
+                            .map_err(PyPolarsErr::from)?;
+                        Ok(s)
+                    })
+                    .collect::<PyResult<Vec<_>>>()
+            }?;
+
+            // no need to check as a record batch has the same guarantees
+            Ok(DataFrame::new_no_checks(columns))
+        })
+        .collect::<PyResult<Vec<_>>>()?;
+
+    Ok(accumulate_dataframes_vertical_unchecked(dfs))
 }
```

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-row/src/lib.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-row/src/lib.rs`

 * *Files 2% similar despite different names*

```diff
@@ -262,17 +262,24 @@
 //! ## Reverse Column Ordering
 //!
 //! The order of a given column can be reversed by negating the encoded bytes of non-null values
 //!
 //! [COBS]: https://en.wikipedia.org/wiki/Consistent_Overhead_Byte_Stuffing
 //! [byte stuffing]: https://en.wikipedia.org/wiki/High-Level_Data_Link_Control#Asynchronous_framing
 
+extern crate core;
+
+pub mod decode;
 pub mod encode;
-mod encodings;
+pub(crate) mod fixed;
 mod row;
 mod utils;
+pub(crate) mod variable;
 
 use arrow::array::*;
 pub type ArrayRef = Box<dyn Array>;
 
-pub use encode::convert_columns;
+pub use encode::{
+    convert_columns, convert_columns_amortized, convert_columns_amortized_no_order,
+    convert_columns_no_order,
+};
 pub use row::{RowsEncoded, SortField};
```

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-row/src/row.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-row/src/row.rs`

 * *Files 18% similar despite different names*

```diff
@@ -1,79 +1,107 @@
 use arrow::array::BinaryArray;
 use arrow::datatypes::DataType;
-use arrow::offset::Offsets;
+use arrow::ffi::mmap;
+use arrow::offset::{Offsets, OffsetsBuffer};
 
-#[derive(Clone)]
+#[derive(Clone, Default)]
 pub struct SortField {
     /// Whether to sort in descending order
     pub descending: bool,
     /// Whether to sort nulls first
     pub nulls_last: bool,
 }
 
+#[derive(Default, Clone)]
 pub struct RowsEncoded {
-    pub(crate) buf: Vec<u8>,
+    pub(crate) values: Vec<u8>,
     pub(crate) offsets: Vec<usize>,
 }
 
+fn checks(offsets: &[usize]) {
+    assert_eq!(
+        std::mem::size_of::<usize>(),
+        std::mem::size_of::<i64>(),
+        "only supported on 64bit arch"
+    );
+    assert!(
+        (*offsets.last().unwrap() as u64) < i64::MAX as u64,
+        "overflow"
+    );
+}
+
+unsafe fn rows_to_array(buf: Vec<u8>, offsets: Vec<usize>) -> BinaryArray<i64> {
+    checks(&offsets);
+
+    // Safety: we checked overflow
+    let offsets = std::mem::transmute::<Vec<usize>, Vec<i64>>(offsets);
+
+    // Safety: monotonically increasing
+    let offsets = Offsets::new_unchecked(offsets);
+
+    BinaryArray::new(DataType::LargeBinary, offsets.into(), buf.into(), None)
+}
+
 impl RowsEncoded {
-    pub(crate) fn new(buf: Vec<u8>, offsets: Vec<usize>) -> Self {
-        RowsEncoded { buf, offsets }
+    pub(crate) fn new(values: Vec<u8>, offsets: Vec<usize>) -> Self {
+        RowsEncoded { values, offsets }
     }
 
     pub fn iter(&self) -> RowsEncodedIter {
         let iter = self.offsets[1..].iter();
         let offset = self.offsets[0];
         RowsEncodedIter {
             offset,
             end: iter,
-            buf: &self.buf,
+            values: &self.values,
         }
     }
 
-    pub fn into_array(self) -> BinaryArray<i64> {
-        assert_eq!(
-            std::mem::size_of::<usize>(),
-            std::mem::size_of::<i64>(),
-            "only supported on 64bit arch"
-        );
-        assert!(
-            (*self.offsets.last().unwrap() as u64) < i64::MAX as u64,
-            "overflow"
-        );
-
-        // Safety: we checked overflow
-        let offsets = unsafe { std::mem::transmute::<Vec<usize>, Vec<i64>>(self.offsets) };
+    /// Borrows the buffers and returns a [`BinaryArray`].
+    ///
+    /// # Safety
+    /// The lifetime of that `BinaryArray` is tight to the lifetime of
+    /// `Self`. The caller must ensure that both stay alive for the same time.
+    pub unsafe fn borrow_array(&self) -> BinaryArray<i64> {
+        checks(&self.offsets);
+
+        unsafe {
+            let (_, values, _) = mmap::slice(&self.values).into_inner();
+            let offsets = std::mem::transmute::<&[usize], &[i64]>(self.offsets.as_slice());
+            let (_, offsets, _) = mmap::slice(offsets).into_inner();
+            let offsets = OffsetsBuffer::new_unchecked(offsets);
 
-        // Safety: monotonically increasing
-        let offsets = unsafe { Offsets::new_unchecked(offsets) };
+            BinaryArray::new(DataType::LargeBinary, offsets, values, None)
+        }
+    }
 
-        BinaryArray::new(DataType::LargeBinary, offsets.into(), self.buf.into(), None)
+    pub fn into_array(self) -> BinaryArray<i64> {
+        unsafe { rows_to_array(self.values, self.offsets) }
     }
 
     #[cfg(test)]
     pub fn get(&self, i: usize) -> &[u8] {
         let start = self.offsets[i];
         let end = self.offsets[i + 1];
-        &self.buf[start..end]
+        &self.values[start..end]
     }
 }
 
 pub struct RowsEncodedIter<'a> {
     offset: usize,
     end: std::slice::Iter<'a, usize>,
-    buf: &'a [u8],
+    values: &'a [u8],
 }
 
 impl<'a> Iterator for RowsEncodedIter<'a> {
     type Item = &'a [u8];
 
     fn next(&mut self) -> Option<Self::Item> {
         let new_offset = *self.end.next()?;
-        let payload = unsafe { self.buf.get_unchecked(self.offset..new_offset) };
+        let payload = unsafe { self.values.get_unchecked(self.offset..new_offset) };
         self.offset = new_offset;
         Some(payload)
     }
 
     fn size_hint(&self) -> (usize, Option<usize>) {
         self.end.size_hint()
     }
```

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-row/src/utils.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-row/src/utils.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-json/Cargo.toml` & `polars_lts_cpu-0.18.3/local_dependencies/polars-json/Cargo.toml`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 polars-utils = { version = "0.30.0", path = "../polars-utils" }
 simd-json = { version = "0.10", features = ["allow-non-simd", "known-key"] }
 
 [dependencies.arrow]
 package = "arrow2"
 git = "https://github.com/jorgecarleitao/arrow2"
 # git = "https://github.com/ritchie46/arrow2"
-rev = "fb5e4d591c7149df590a330365fae55d2370962f"
+rev = "2d2e7053f9a50810bfe9cecff25ab39089aef98e"
 # path = "../arrow2"
 # branch = "polars_2023-05-25"
 version = "0.17"
 default-features = false
 features = [
   "compute_aggregate",
   "compute_arithmetics",
```

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-json/LICENSE` & `polars_lts_cpu-0.18.3/local_dependencies/polars-algo/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-json/src/json/deserialize.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-json/src/json/deserialize.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-json/src/json/infer_schema.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-json/src/json/infer_schema.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-json/src/ndjson/deserialize.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-json/src/ndjson/deserialize.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-json/src/ndjson/file.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-json/src/ndjson/file.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/Cargo.toml` & `polars_lts_cpu-0.18.3/local_dependencies/polars-arrow/Cargo.toml`

 * *Files 3% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 timezones = ["chrono-tz", "chrono"]
 simd = []
 
 [dependencies.arrow]
 package = "arrow2"
 git = "https://github.com/jorgecarleitao/arrow2"
 # git = "https://github.com/ritchie46/arrow2"
-rev = "fb5e4d591c7149df590a330365fae55d2370962f"
+rev = "2d2e7053f9a50810bfe9cecff25ab39089aef98e"
 # path = "../arrow2"
 # branch = "polars_2023-05-25"
 version = "0.17"
 default-features = false
 features = [
   "compute_aggregate",
   "compute_arithmetics",
```

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/LICENSE` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/array/default_arrays.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-arrow/src/array/default_arrays.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/array/fixed_size_list.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-arrow/src/array/fixed_size_list.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/array/get.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-arrow/src/array/get.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/array/list.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-arrow/src/array/list.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/array/mod.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-arrow/src/array/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/array/null.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-arrow/src/array/null.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/array/slice.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-arrow/src/array/slice.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/array/utf8.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-arrow/src/array/utf8.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/bit_util.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-arrow/src/bit_util.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/bitmap/mutable.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-arrow/src/bitmap/mutable.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/compute/arithmetics/decimal/commutative.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-arrow/src/compute/arithmetics/decimal/commutative.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/compute/arithmetics/decimal/div.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-arrow/src/compute/arithmetics/decimal/div.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/compute/arithmetics/decimal/mod.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-arrow/src/compute/arithmetics/decimal/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/compute/arithmetics/decimal/mul.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-arrow/src/compute/arithmetics/decimal/mul.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/compute/bitwise.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-arrow/src/compute/bitwise.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/compute/cast.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-arrow/src/compute/cast.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/compute/decimal.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-arrow/src/compute/decimal.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/compute/mod.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-arrow/src/compute/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/compute/take/boolean.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-arrow/src/compute/take/boolean.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/compute/take/fixed_size_list.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-arrow/src/compute/take/fixed_size_list.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/compute/take/mod.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-arrow/src/compute/take/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/compute/tile.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-arrow/src/compute/tile.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/conversion.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-arrow/src/conversion.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/data_types.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-arrow/src/data_types.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/floats/ord.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-arrow/src/floats/ord.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/index.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-arrow/src/index.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/is_valid.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-arrow/src/is_valid.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/kernels/agg_mean.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-arrow/src/kernels/agg_mean.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/kernels/comparison.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-arrow/src/kernels/comparison.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/kernels/concatenate.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-arrow/src/kernels/concatenate.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/kernels/ewm/average.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-arrow/src/kernels/ewm/average.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/kernels/ewm/mod.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-arrow/src/kernels/ewm/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/kernels/ewm/variance.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-arrow/src/kernels/ewm/variance.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/kernels/float.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-arrow/src/kernels/float.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/kernels/list.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-arrow/src/kernels/list.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/kernels/list_bytes_iter.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-arrow/src/kernels/list_bytes_iter.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/kernels/mod.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-arrow/src/kernels/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/kernels/rolling/mod.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-arrow/src/kernels/rolling/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/mean.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/mean.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/min_max.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/min_max.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/mod.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/quantile.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/quantile.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/sum.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/sum.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/variance.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/variance.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/kernels/rolling/nulls/mean.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-arrow/src/kernels/rolling/nulls/mean.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/kernels/rolling/nulls/min_max.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-arrow/src/kernels/rolling/nulls/min_max.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/kernels/rolling/nulls/mod.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-arrow/src/kernels/rolling/nulls/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/kernels/rolling/nulls/quantile.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-arrow/src/kernels/rolling/nulls/quantile.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/kernels/rolling/nulls/sum.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-arrow/src/kernels/rolling/nulls/sum.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/kernels/rolling/nulls/variance.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-arrow/src/kernels/rolling/nulls/variance.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/kernels/rolling/window.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-arrow/src/kernels/rolling/window.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/kernels/set.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-arrow/src/kernels/set.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/kernels/sort_partition.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-arrow/src/kernels/sort_partition.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/kernels/sorted_join/inner.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-arrow/src/kernels/sorted_join/inner.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/kernels/sorted_join/left.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-arrow/src/kernels/sorted_join/left.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/kernels/string.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-arrow/src/kernels/string.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/kernels/take_agg/boolean.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-arrow/src/kernels/take_agg/boolean.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/kernels/take_agg/mod.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-arrow/src/kernels/take_agg/mod.rs`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 
 use arrow::array::{Array, BooleanArray, PrimitiveArray, Utf8Array};
 use arrow::types::NativeType;
 pub use boolean::*;
 use num_traits::{NumCast, ToPrimitive};
 pub use var::*;
 
-use crate::array::PolarsArray;
 use crate::index::IdxSize;
 
 /// Take kernel for single chunk without nulls and an iterator as index.
 /// # Safety
 /// caller must ensure iterators indexes are in bounds
 #[inline]
 pub unsafe fn take_agg_no_null_primitive_iter_unchecked<
@@ -22,15 +21,15 @@
     F: Fn(TOut, TOut) -> TOut,
 >(
     arr: &PrimitiveArray<T>,
     indices: I,
     f: F,
     init: TOut,
 ) -> TOut {
-    debug_assert!(!arr.has_validity());
+    debug_assert!(arr.null_count() == 0);
     let array_values = arr.values().as_slice();
 
     indices.into_iter().fold(init, |acc, idx| {
         f(
             acc,
             NumCast::from(*array_values.get_unchecked(idx)).unwrap_unchecked(),
         )
```

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/kernels/take_agg/var.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-arrow/src/kernels/take_agg/var.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/kernels/time.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-arrow/src/kernels/time.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/slice.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-arrow/src/slice.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/trusted_len/boolean.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-arrow/src/trusted_len/boolean.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/trusted_len/mod.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-arrow/src/trusted_len/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/trusted_len/push_unchecked.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-arrow/src/trusted_len/push_unchecked.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/utils.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-arrow/src/utils.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-error/Cargo.toml` & `polars_lts_cpu-0.18.3/local_dependencies/polars-error/Cargo.toml`

 * *Files 16% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 regex = { version = "1.6", optional = true }
 thiserror= "^1"
 
 [dependencies.arrow]
 package = "arrow2"
 git = "https://github.com/jorgecarleitao/arrow2"
 # git = "https://github.com/ritchie46/arrow2"
-rev = "fb5e4d591c7149df590a330365fae55d2370962f"
+rev = "2d2e7053f9a50810bfe9cecff25ab39089aef98e"
 # path = "../arrow2"
 # branch = "polars_2023-05-25"
 version = "0.17"
 default-features = false
 features = [
   "compute_aggregate",
   "compute_arithmetics",
```

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-error/LICENSE` & `polars_lts_cpu-0.18.3/local_dependencies/polars-json/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-error/src/lib.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-error/src/lib.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-algo/Cargo.toml` & `polars_lts_cpu-0.18.3/local_dependencies/polars-algo/Cargo.toml`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-algo/LICENSE` & `polars_lts_cpu-0.18.3/local_dependencies/polars-plan/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-algo/src/algo.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-algo/src/algo.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/Cargo.toml` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -178,15 +178,15 @@
 url = { version = "2.3.1", optional = true }
 xxhash-rust= { version = "0.8.6", features = ["xxh3"] }
 
 [dependencies.arrow]
 package = "arrow2"
 git = "https://github.com/jorgecarleitao/arrow2"
 # git = "https://github.com/ritchie46/arrow2"
-rev = "fb5e4d591c7149df590a330365fae55d2370962f"
+rev = "2d2e7053f9a50810bfe9cecff25ab39089aef98e"
 # path = "../arrow2"
 # branch = "polars_2023-05-25"
 version = "0.17"
 default-features = false
 features = [
   "compute_aggregate",
   "compute_arithmetics",
```

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/LICENSE` & `polars_lts_cpu-0.18.3/local_dependencies/polars-time/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/arithmetic/decimal.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/arithmetic/decimal.rs`

 * *Files 8% similar despite different names*

```diff
@@ -54,40 +54,40 @@
             (a, b) if a == b => {
                 let (lhs, rhs) = align_chunks_binary(lhs, rhs);
                 let chunks = lhs
                     .downcast_iter()
                     .zip(rhs.downcast_iter())
                     .map(|(lhs, rhs)| kernel(lhs, rhs).map(|a| Box::new(a) as ArrayRef))
                     .collect::<PolarsResult<_>>()?;
-                lhs.copy_with_chunks(chunks, false, false)
+                unsafe { lhs.copy_with_chunks(chunks, false, false) }
             }
             // broadcast right path
             (_, 1) => {
                 let opt_rhs = rhs.get(0);
                 match opt_rhs {
                     None => ChunkedArray::full_null(lhs.name(), lhs.len()),
                     Some(rhs_val) => {
                         let chunks = lhs
                             .downcast_iter()
                             .map(|lhs| operation_lhs(lhs, rhs_val).map(|a| Box::new(a) as ArrayRef))
                             .collect::<PolarsResult<_>>()?;
-                        lhs.copy_with_chunks(chunks, false, false)
+                        unsafe { lhs.copy_with_chunks(chunks, false, false) }
                     }
                 }
             }
             (1, _) => {
                 let opt_lhs = lhs.get(0);
                 match opt_lhs {
                     None => ChunkedArray::full_null(lhs.name(), rhs.len()),
                     Some(lhs_val) => {
                         let chunks = rhs
                             .downcast_iter()
                             .map(|rhs| operation_rhs(lhs_val, rhs).map(|a| Box::new(a) as ArrayRef))
                             .collect::<PolarsResult<_>>()?;
-                        lhs.copy_with_chunks(chunks, false, false)
+                        unsafe { lhs.copy_with_chunks(chunks, false, false) }
                     }
                 }
             }
             _ => {
                 polars_bail!(ComputeError: "Cannot apply operation on arrays of different lengths")
             }
         };
```

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/arithmetic/mod.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/arithmetic/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/arithmetic/numeric.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/arithmetic/numeric.rs`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
         (a, b) if a == b => {
             let (lhs, rhs) = align_chunks_binary(lhs, rhs);
             let chunks = lhs
                 .downcast_iter()
                 .zip(rhs.downcast_iter())
                 .map(|(lhs, rhs)| Box::new(kernel(lhs, rhs)) as ArrayRef)
                 .collect();
-            lhs.copy_with_chunks(chunks, false, false)
+            unsafe { lhs.copy_with_chunks(chunks, false, false) }
         }
         // broadcast right path
         (_, 1) => {
             let opt_rhs = rhs.get(0);
             match opt_rhs {
                 None => ChunkedArray::full_null(lhs.name(), lhs.len()),
                 Some(rhs) => lhs.apply(|lhs| operation(lhs, rhs)),
```

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/array/iterator.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/array/iterator.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/array/mod.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/array/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/bitwise.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/bitwise.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/builder/binary.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/builder/binary.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/builder/boolean.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/builder/boolean.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/builder/fixed_size_list.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/builder/fixed_size_list.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/builder/from.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/builder/from.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/builder/list.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/builder/list.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/builder/mod.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/builder/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/builder/primitive.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/builder/primitive.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/builder/utf8.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/builder/utf8.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/cast.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/cast.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/comparison/mod.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/comparison/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/comparison/scalar.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/comparison/scalar.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/drop.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/drop.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/float.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/float.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/from.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/from.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/iterator/mod.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/iterator/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/iterator/par/list.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/iterator/par/list.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/iterator/par/utf8.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/iterator/par/utf8.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/kernels/take.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/kernels/take.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/list/iterator.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/list/iterator.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/list/mod.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/list/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/logical/categorical/builder.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/logical/categorical/builder.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/logical/categorical/from.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/logical/categorical/from.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/logical/categorical/merge.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/logical/categorical/merge.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/logical/categorical/mod.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/logical/categorical/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/append.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/append.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/take_random.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/take_random.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/unique.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/unique.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/zip.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/zip.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/logical/categorical/stringcache.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/logical/categorical/stringcache.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/logical/date.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/logical/date.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/logical/datetime.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/logical/datetime.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/logical/decimal.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/logical/decimal.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/logical/duration.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/logical/duration.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/logical/mod.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/logical/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/logical/struct_/mod.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/logical/struct_/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/logical/time.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/logical/time.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/mod.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/mod.rs`

 * *Files 1% similar despite different names*

```diff
@@ -311,15 +311,18 @@
     /// Count the null values.
     #[inline]
     pub fn null_count(&self) -> usize {
         self.chunks.iter().map(|arr| arr.null_count()).sum()
     }
 
     /// Create a new ChunkedArray from self, where the chunks are replaced.
-    fn copy_with_chunks(
+    ///
+    /// # Safety
+    /// The caller must ensure the dtypes of the chunks are correct
+    unsafe fn copy_with_chunks(
         &self,
         chunks: Vec<ArrayRef>,
         keep_sorted: bool,
         keep_fast_explode: bool,
     ) -> Self {
         let mut out = ChunkedArray {
             field: self.field.clone(),
```

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/ndarray.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/ndarray.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/object/builder.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/object/builder.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/object/extension/drop.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/object/extension/drop.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/object/extension/list.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/object/extension/list.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/object/extension/mod.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/object/extension/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/object/extension/polars_extension.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/object/extension/polars_extension.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/object/iterator.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/object/iterator.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/object/mod.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/object/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/object/registry.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/object/registry.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/ops/aggregate/mod.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/ops/aggregate/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/ops/aggregate/quantile.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/ops/aggregate/quantile.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/ops/aggregate/var.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/ops/aggregate/var.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/ops/any_value.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/ops/any_value.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/ops/append.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/ops/append.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/ops/apply.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/ops/apply.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/ops/bit_repr.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/ops/bit_repr.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/ops/chunkops.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/ops/chunkops.rs`

 * *Files 2% similar despite different names*

```diff
@@ -96,29 +96,29 @@
                     vec![concatenate_owned_unchecked(chunks).unwrap()]
                 }
 
                 if self.chunks.len() == 1 {
                     self.clone()
                 } else {
                     let chunks = inner_rechunk(&self.chunks);
-                    self.copy_with_chunks(chunks, true, true)
+                    unsafe { self.copy_with_chunks(chunks, true, true) }
                 }
             }
         }
     }
 
     /// Slice the array. The chunks are reallocated the underlying data slices are zero copy.
     ///
     /// When offset is negative it will be counted from the end of the array.
     /// This method will never error,
     /// and will slice the best match when offset, or length is out of bounds
     #[inline]
     pub fn slice(&self, offset: i64, length: usize) -> Self {
         let (chunks, len) = slice(&self.chunks, offset, length, self.len());
-        let mut out = self.copy_with_chunks(chunks, true, true);
+        let mut out = unsafe { self.copy_with_chunks(chunks, true, true) };
         out.length = len as IdxSize;
         out
     }
 
     /// Take a view of top n elements
     #[must_use]
     pub fn limit(&self, num_elements: usize) -> Self
```

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/ops/compare_inner.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/ops/compare_inner.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/ops/concat_str.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/ops/concat_str.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/ops/cum_agg.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/ops/cum_agg.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/ops/decimal.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/ops/decimal.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/ops/downcast.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/ops/downcast.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/ops/explode.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/ops/explode.rs`

 * *Files 1% similar despite different names*

```diff
@@ -262,16 +262,15 @@
                 builder.push_null();
                 start = o;
             }
             last = o;
         }
         process_range(start, last, &mut builder);
         let arr = builder.finish(Some(&inner_type.to_arrow())).unwrap();
-        self.copy_with_chunks(vec![Box::new(arr)], true, true)
-            .into_series()
+        unsafe { self.copy_with_chunks(vec![Box::new(arr)], true, true) }.into_series()
     }
 }
 
 #[cfg(feature = "dtype-array")]
 impl ExplodeByOffsets for ArrayChunked {
     fn explode_by_offsets(&self, offsets: &[i64]) -> Series {
         debug_assert_eq!(self.chunks.len(), 1);
```

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/ops/explode_and_offsets.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/ops/explode_and_offsets.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/ops/extend.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/ops/extend.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/ops/fill_null.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/ops/fill_null.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/ops/filter.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/ops/filter.rs`

 * *Files 8% similar despite different names*

```diff
@@ -33,15 +33,15 @@
         let (left, filter) = align_chunks_binary(self, filter);
 
         let chunks = left
             .downcast_iter()
             .zip(filter.downcast_iter())
             .map(|(left, mask)| filter_fn(left, mask).unwrap())
             .collect::<Vec<_>>();
-        Ok(self.copy_with_chunks(chunks, true, true))
+        unsafe { Ok(self.copy_with_chunks(chunks, true, true)) }
     }
 }
 
 impl ChunkFilter<BooleanType> for BooleanChunked {
     fn filter(&self, filter: &BooleanChunked) -> PolarsResult<ChunkedArray<BooleanType>> {
         // broadcast
         if filter.len() == 1 {
@@ -54,15 +54,15 @@
         let (left, filter) = align_chunks_binary(self, filter);
 
         let chunks = left
             .downcast_iter()
             .zip(filter.downcast_iter())
             .map(|(left, mask)| filter_fn(left, mask).unwrap())
             .collect::<Vec<_>>();
-        Ok(self.copy_with_chunks(chunks, true, true))
+        unsafe { Ok(self.copy_with_chunks(chunks, true, true)) }
     }
 }
 
 impl ChunkFilter<Utf8Type> for Utf8Chunked {
     fn filter(&self, filter: &BooleanChunked) -> PolarsResult<ChunkedArray<Utf8Type>> {
         let out = self.as_binary().filter(filter)?;
         unsafe { Ok(out.to_utf8()) }
@@ -83,15 +83,15 @@
 
         let chunks = left
             .downcast_iter()
             .zip(filter.downcast_iter())
             .map(|(left, mask)| filter_fn(left, mask).unwrap())
             .collect::<Vec<_>>();
 
-        Ok(self.copy_with_chunks(chunks, true, true))
+        unsafe { Ok(self.copy_with_chunks(chunks, true, true)) }
     }
 }
 
 impl ChunkFilter<ListType> for ListChunked {
     fn filter(&self, filter: &BooleanChunked) -> PolarsResult<ListChunked> {
         // broadcast
         if filter.len() == 1 {
```

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/ops/full.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/ops/full.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/ops/is_in.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/ops/is_in.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/ops/min_max_binary.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/ops/min_max_binary.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/ops/mod.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/ops/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/ops/nulls.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/ops/nulls.rs`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,15 @@
         }
         // dispatch to non-generic function
         is_not_null(self.name(), &self.chunks)
     }
 
     pub(crate) fn coalesce_nulls(&self, other: &[ArrayRef]) -> Self {
         let chunks = coalesce_nulls(&self.chunks, other);
-        self.copy_with_chunks(chunks, true, false)
+        unsafe { self.copy_with_chunks(chunks, true, false) }
     }
 }
 pub fn is_not_null(name: &str, chunks: &[ArrayRef]) -> BooleanChunked {
     let chunks = chunks
         .iter()
         .map(|arr| {
             let bitmap = arr
```

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/ops/peaks.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/ops/peaks.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/ops/repeat_by.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/ops/repeat_by.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/ops/reverse.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/ops/reverse.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/ops/rolling_window.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/ops/rolling_window.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/ops/set.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/ops/set.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/ops/shift.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/ops/shift.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/ops/sort/arg_sort.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/ops/sort/arg_sort.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/ops/sort/arg_sort_multiple.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/ops/sort/arg_sort_multiple.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/ops/sort/categorical.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/ops/sort/categorical.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/ops/sort/mod.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/ops/sort/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/ops/take/mod.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/ops/take/mod.rs`

 * *Files 0% similar despite different names*

```diff
@@ -60,15 +60,15 @@
 
 impl<T> ChunkedArray<T>
 where
     T: PolarsDataType,
 {
     fn finish_from_array(&self, array: Box<dyn Array>) -> Self {
         let keep_fast_explode = array.null_count() == 0;
-        self.copy_with_chunks(vec![array], false, keep_fast_explode)
+        unsafe { self.copy_with_chunks(vec![array], false, keep_fast_explode) }
     }
 }
 
 impl<T> ChunkTake for ChunkedArray<T>
 where
     T: PolarsNumericType,
 {
```

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/ops/take/take_chunked.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/ops/take/take_chunked.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/ops/take/take_random.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/ops/take/take_random.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/ops/take/take_single.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/ops/take/take_single.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/ops/take/traits.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/ops/take/traits.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/ops/unique/mod.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/ops/unique/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/ops/unique/rank.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/ops/unique/rank.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/random.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/random.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/temporal/conversion.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/temporal/conversion.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/temporal/date.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/temporal/date.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/temporal/datetime.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/temporal/datetime.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/temporal/duration.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/temporal/duration.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/temporal/mod.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/temporal/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/temporal/time.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/temporal/time.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/to_vec.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/to_vec.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/trusted_len.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/trusted_len.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/upstream_traits.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/chunked_array/upstream_traits.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/cloud.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/cloud.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/config.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/config.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/datatypes/_serde.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/datatypes/_serde.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/datatypes/aliases.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/datatypes/aliases.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/datatypes/any_value.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/datatypes/any_value.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/datatypes/dtype.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/datatypes/dtype.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/datatypes/field.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/datatypes/field.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/datatypes/mod.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/datatypes/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/datatypes/time_unit.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/datatypes/time_unit.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/doc/changelog/v0_10_0_11.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/doc/changelog/v0_10_0_11.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/doc/changelog/v0_7.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/doc/changelog/v0_7.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/doc/changelog/v0_8.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/doc/changelog/v0_8.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/doc/changelog/v0_9.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/doc/changelog/v0_9.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/fmt.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/fmt.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/frame/arithmetic.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/frame/arithmetic.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/frame/asof_join/asof.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/frame/asof_join/asof.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/frame/asof_join/groups.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/frame/asof_join/groups.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/frame/asof_join/mod.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/frame/asof_join/mod.rs`

 * *Files 2% similar despite different names*

```diff
@@ -27,14 +27,19 @@
     pub right_by: Option<Vec<SmartString>>,
 }
 
 fn check_asof_columns(a: &Series, b: &Series, check_sorted: bool) -> PolarsResult<()> {
     let dtype_a = a.dtype();
     let dtype_b = b.dtype();
     polars_ensure!(
+        dtype_a.to_physical().is_numeric() && dtype_b.to_physical().is_numeric(),
+        InvalidOperation:
+        "asof join only supported on numeric/temporal keys"
+    );
+    polars_ensure!(
         dtype_a == dtype_b,
         ComputeError: "mismatching key dtypes in asof-join: `{}` and `{}`",
         a.dtype(), b.dtype()
     );
     polars_ensure!(
         a.null_count() == 0 && b.null_count() == 0,
         ComputeError: "asof join must not have null values in 'on' arguments"
```

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/frame/chunks.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/frame/chunks.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/frame/cross_join.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/frame/cross_join.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/frame/explode.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/frame/explode.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/frame/from.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/frame/from.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/frame/groupby/aggregations/agg_list.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/frame/groupby/aggregations/agg_list.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/frame/groupby/aggregations/boolean.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/frame/groupby/aggregations/boolean.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/frame/groupby/aggregations/dispatch.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/frame/groupby/aggregations/dispatch.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/frame/groupby/aggregations/mod.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/frame/groupby/aggregations/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/frame/groupby/aggregations/utf8.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/frame/groupby/aggregations/utf8.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/frame/groupby/hashing.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/frame/groupby/hashing.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/frame/groupby/into_groups.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/frame/groupby/into_groups.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/frame/groupby/mod.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/frame/groupby/mod.rs`

 * *Files 0% similar despite different names*

```diff
@@ -770,14 +770,15 @@
             agg.rename(&new_name);
             cols.push(agg);
         }
         DataFrame::new(cols)
     }
 
     fn prepare_apply(&self) -> PolarsResult<DataFrame> {
+        polars_ensure!(self.df.height() > 0, ComputeError: "cannot groupby + apply on empty 'DataFrame'");
         if let Some(agg) = &self.selected_agg {
             if agg.is_empty() {
                 Ok(self.df.clone())
             } else {
                 let mut new_cols = Vec::with_capacity(self.selected_keys.len() + agg.len());
                 new_cols.extend_from_slice(&self.selected_keys);
                 let cols = self.df.select_series(agg)?;
```

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/frame/groupby/perfect.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/frame/groupby/perfect.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/frame/groupby/proxy.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/frame/groupby/proxy.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/frame/hash_join/args.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/frame/hash_join/args.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/frame/hash_join/mod.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/frame/hash_join/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/frame/hash_join/multiple_keys.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/frame/hash_join/multiple_keys.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/frame/hash_join/single_keys.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/frame/hash_join/single_keys.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/frame/hash_join/single_keys_dispatch.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/frame/hash_join/single_keys_dispatch.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/frame/hash_join/single_keys_inner.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/frame/hash_join/single_keys_inner.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/frame/hash_join/single_keys_left.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/frame/hash_join/single_keys_left.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/frame/hash_join/single_keys_outer.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/frame/hash_join/single_keys_outer.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/frame/hash_join/single_keys_semi_anti.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/frame/hash_join/single_keys_semi_anti.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/frame/hash_join/sort_merge.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/frame/hash_join/sort_merge.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/frame/hash_join/zip_outer.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/frame/hash_join/zip_outer.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/frame/mod.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/frame/mod.rs`

 * *Files 0% similar despite different names*

```diff
@@ -915,15 +915,15 @@
         }
 
         self.columns
             .iter_mut()
             .zip(other.columns.iter())
             .try_for_each::<_, PolarsResult<_>>(|(left, right)| {
                 ensure_can_extend(left, right)?;
-                left.append(right).expect("should not fail");
+                left.append(right)?;
                 Ok(())
             })?;
         Ok(self)
     }
 
     /// Does not check if schema is correct
     pub(crate) fn vstack_mut_unchecked(&mut self, other: &DataFrame) {
```

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/frame/row/av_buffer.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/frame/row/av_buffer.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/frame/row/dataframe.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/frame/row/dataframe.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/frame/row/mod.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/frame/row/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/frame/row/transpose.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/frame/row/transpose.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/frame/top_k.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/frame/top_k.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/frame/upstream_traits.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/frame/upstream_traits.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/functions.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/functions.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/hashing/fx.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/hashing/fx.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/hashing/identity.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/hashing/identity.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/hashing/partition.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/hashing/partition.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/hashing/vector_hasher.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/hashing/vector_hasher.rs`

 * *Files 1% similar despite different names*

```diff
@@ -159,31 +159,34 @@
     }
 
     fn vec_hash_combine(&self, random_state: RandomState, hashes: &mut [u64]) {
         self.as_binary().vec_hash_combine(random_state, hashes)
     }
 }
 
+// used in polars-pipe
+pub fn _hash_binary_array(arr: &BinaryArray<i64>, random_state: RandomState, buf: &mut Vec<u64>) {
+    let null_h = get_null_hash_value(random_state);
+    if arr.null_count() == 0 {
+        // use the null_hash as seed to get a hash determined by `random_state` that is passed
+        buf.extend(arr.values_iter().map(|v| xxh3_64_with_seed(v, null_h)))
+    } else {
+        buf.extend(arr.into_iter().map(|opt_v| match opt_v {
+            Some(v) => xxh3_64_with_seed(v, null_h),
+            None => null_h,
+        }))
+    }
+}
+
 impl VecHash for BinaryChunked {
     fn vec_hash(&self, random_state: RandomState, buf: &mut Vec<u64>) {
         buf.clear();
         buf.reserve(self.len());
-        let null_h = get_null_hash_value(random_state);
-
-        self.downcast_iter().for_each(|arr| {
-            if arr.null_count() == 0 {
-                // simply use the null_hash as seed to get a hash determined by `random_state` that is passed
-                buf.extend(arr.values_iter().map(|v| xxh3_64_with_seed(v, null_h)))
-            } else {
-                buf.extend(arr.into_iter().map(|opt_v| match opt_v {
-                    Some(v) => xxh3_64_with_seed(v, null_h),
-                    None => null_h,
-                }))
-            }
-        });
+        self.downcast_iter()
+            .for_each(|arr| _hash_binary_array(arr, random_state.clone(), buf));
     }
 
     fn vec_hash_combine(&self, random_state: RandomState, hashes: &mut [u64]) {
         let null_h = get_null_hash_value(random_state);
 
         let mut offset = 0;
         self.downcast_iter().for_each(|arr| {
```

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/lib.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/lib.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/named_from.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/named_from.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/prelude.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/prelude.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/schema.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/schema.rs`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 use indexmap::IndexMap;
 #[cfg(feature = "serde-lazy")]
 use serde::{Deserialize, Serialize};
 use smartstring::alias::String as SmartString;
 
 use crate::prelude::*;
+use crate::utils::try_get_supertype;
 
 /// A map from field/column name (`String`) to the type of that field/column (`DataType`)
 #[derive(Eq, Clone, Default)]
 #[cfg_attr(feature = "serde-lazy", derive(Serialize, Deserialize))]
 pub struct Schema {
     inner: PlIndexMap<SmartString, DataType>,
 }
@@ -363,14 +364,29 @@
 
     /// Iterates over the `(&name, &dtype)` pairs in this schema
     ///
     /// For an owned version, use [`iter_fields`][Self::iter_fields], which clones the data to iterate owned `Field`s
     pub fn iter(&self) -> impl Iterator<Item = (&SmartString, &DataType)> + '_ {
         self.inner.iter()
     }
+
+    /// Take another [`Schema`] and try to find the supertypes between them.
+    pub fn to_supertype(&mut self, other: &Schema) -> PolarsResult<bool> {
+        polars_ensure!(self.len() == other.len(), ComputeError: "schema lengths differ");
+
+        let mut changed = false;
+        for ((k, dt), (other_k, other_dt)) in self.inner.iter_mut().zip(other.iter()) {
+            polars_ensure!(k == other_k, ComputeError: "schema names differ: got {}, expected {}", k, other_k);
+
+            let st = try_get_supertype(dt, other_dt)?;
+            changed |= &st != dt;
+            *dt = st
+        }
+        Ok(changed)
+    }
 }
 
 pub type SchemaRef = Arc<Schema>;
 
 impl IntoIterator for Schema {
     type Item = (SmartString, DataType);
     type IntoIter = <PlIndexMap<SmartString, DataType> as IntoIterator>::IntoIter;
```

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/serde/chunked_array.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/serde/chunked_array.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/serde/df.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/serde/df.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/serde/mod.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/serde/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/serde/series.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/serde/series.rs`

 * *Files 8% similar despite different names*

```diff
@@ -11,72 +11,66 @@
     fn serialize<S>(
         &self,
         serializer: S,
     ) -> std::result::Result<<S as Serializer>::Ok, <S as Serializer>::Error>
     where
         S: Serializer,
     {
-        if let Ok(ca) = self.i32() {
-            ca.serialize(serializer)
-        } else if let Ok(ca) = self.u32() {
-            ca.serialize(serializer)
-        } else if let Ok(ca) = self.i64() {
-            ca.serialize(serializer)
-        } else if let Ok(ca) = self.u64() {
-            ca.serialize(serializer)
-        } else if let Ok(ca) = self.f32() {
-            ca.serialize(serializer)
-        } else if let Ok(ca) = self.f64() {
-            ca.serialize(serializer)
-        } else if let Ok(ca) = self.utf8() {
-            ca.serialize(serializer)
-        } else if let Ok(ca) = self.bool() {
-            ca.serialize(serializer)
-        } else if let Ok(ca) = self.list() {
-            ca.serialize(serializer)
-        } else {
-            match self.dtype() {
-                DataType::Binary => {
-                    let ca = self.binary().unwrap();
-                    ca.serialize(serializer)
-                }
-                #[cfg(feature = "dtype-struct")]
-                DataType::Struct(_) => {
-                    let ca = self.struct_().unwrap();
-                    ca.serialize(serializer)
-                }
-                #[cfg(feature = "dtype-date")]
-                DataType::Date => {
-                    let ca = self.date().unwrap();
-                    ca.serialize(serializer)
-                }
-                #[cfg(feature = "dtype-datetime")]
-                DataType::Datetime(_, _) => {
-                    let ca = self.datetime().unwrap();
-                    ca.serialize(serializer)
-                }
-                #[cfg(feature = "dtype-categorical")]
-                DataType::Categorical(_) => {
-                    let ca = self.categorical().unwrap();
-                    ca.serialize(serializer)
-                }
-                #[cfg(feature = "dtype-duration")]
-                DataType::Duration(_) => {
-                    let ca = self.duration().unwrap();
-                    ca.serialize(serializer)
-                }
-                #[cfg(feature = "dtype-time")]
-                DataType::Time => {
-                    let ca = self.time().unwrap();
-                    ca.serialize(serializer)
-                }
-                _ => {
-                    // cast small integers to i32
-                    self.cast(&DataType::Int32).unwrap().serialize(serializer)
-                }
+        match self.dtype() {
+            DataType::Binary => {
+                let ca = self.binary().unwrap();
+                ca.serialize(serializer)
+            }
+            DataType::List(_) => {
+                let ca = self.list().unwrap();
+                ca.serialize(serializer)
+            }
+            DataType::Boolean => {
+                let ca = self.bool().unwrap();
+                ca.serialize(serializer)
+            }
+            DataType::Utf8 => {
+                let ca = self.utf8().unwrap();
+                ca.serialize(serializer)
+            }
+            #[cfg(feature = "dtype-struct")]
+            DataType::Struct(_) => {
+                let ca = self.struct_().unwrap();
+                ca.serialize(serializer)
+            }
+            #[cfg(feature = "dtype-date")]
+            DataType::Date => {
+                let ca = self.date().unwrap();
+                ca.serialize(serializer)
+            }
+            #[cfg(feature = "dtype-datetime")]
+            DataType::Datetime(_, _) => {
+                let ca = self.datetime().unwrap();
+                ca.serialize(serializer)
+            }
+            #[cfg(feature = "dtype-categorical")]
+            DataType::Categorical(_) => {
+                let ca = self.categorical().unwrap();
+                ca.serialize(serializer)
+            }
+            #[cfg(feature = "dtype-duration")]
+            DataType::Duration(_) => {
+                let ca = self.duration().unwrap();
+                ca.serialize(serializer)
+            }
+            #[cfg(feature = "dtype-time")]
+            DataType::Time => {
+                let ca = self.time().unwrap();
+                ca.serialize(serializer)
+            }
+            dt => {
+                with_match_physical_numeric_polars_type!(dt, |$T| {
+                let ca: &ChunkedArray<$T> = self.as_ref().as_ref().as_ref();
+                ca.serialize(serializer)
+                })
             }
         }
     }
 }
 
 impl<'de> Deserialize<'de> for Series {
     fn deserialize<D>(deserializer: D) -> std::result::Result<Self, <D as Deserializer<'de>>::Error>
```

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/series/any_value.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/series/any_value.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/series/arithmetic/borrowed.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/series/arithmetic/borrowed.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/series/arithmetic/owned.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/series/arithmetic/owned.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/series/comparison.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/series/comparison.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/series/from.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/series/from.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/series/implementations/array.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/series/implementations/array.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/series/implementations/binary.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/series/implementations/binary.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/series/implementations/boolean.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/series/implementations/boolean.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/series/implementations/categorical.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/series/implementations/categorical.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/series/implementations/dates_time.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/series/implementations/dates_time.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/series/implementations/datetime.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/series/implementations/datetime.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/series/implementations/decimal.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/series/implementations/decimal.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/series/implementations/duration.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/series/implementations/duration.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/series/implementations/floats.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/series/implementations/floats.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/series/implementations/list.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/series/implementations/list.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/series/implementations/mod.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/series/implementations/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/series/implementations/null.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/series/implementations/null.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/series/implementations/object.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/series/implementations/object.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/series/implementations/struct_.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/series/implementations/struct_.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/series/implementations/utf8.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/series/implementations/utf8.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/series/into.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/series/into.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/series/iterator.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/series/iterator.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/series/mod.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/series/mod.rs`

 * *Files 0% similar despite different names*

```diff
@@ -415,14 +415,28 @@
         use DataType::*;
         match self.dtype() {
             Date => Cow::Owned(self.cast(&Int32).unwrap()),
             Datetime(_, _) | Duration(_) | Time => Cow::Owned(self.cast(&Int64).unwrap()),
             #[cfg(feature = "dtype-categorical")]
             Categorical(_) => Cow::Owned(self.cast(&UInt32).unwrap()),
             List(inner) => Cow::Owned(self.cast(&List(Box::new(inner.to_physical()))).unwrap()),
+            #[cfg(feature = "dtype-struct")]
+            Struct(_) => {
+                let arr = self.struct_().unwrap();
+                let fields = arr
+                    .fields()
+                    .iter()
+                    .map(|s| s.to_physical_repr().into_owned())
+                    .collect::<Vec<_>>();
+                Cow::Owned(
+                    StructChunked::new(self.name(), &fields)
+                        .unwrap()
+                        .into_series(),
+                )
+            }
             _ => Cow::Borrowed(self),
         }
     }
 
     fn finish_take_threaded(&self, s: Vec<Series>, rechunk: bool) -> Series {
         let s = s
             .into_iter()
```

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/series/ops/diff.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/series/ops/diff.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/series/ops/downcast.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/series/ops/downcast.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/series/ops/ewm.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/series/ops/ewm.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/series/ops/mod.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/series/ops/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/series/ops/moment.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/series/ops/moment.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/series/ops/null.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/series/ops/null.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/series/ops/pct_change.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/series/ops/pct_change.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/series/ops/round.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/series/ops/round.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/series/ops/to_list.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/series/ops/to_list.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/series/ops/unique.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/series/ops/unique.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/series/series_trait.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/series/series_trait.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/series/unstable.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/series/unstable.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/testing.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/testing.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/utils/flatten.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/utils/flatten.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/utils/mod.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/utils/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/utils/series.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/utils/series.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/utils/supertype.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-core/src/utils/supertype.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/Cargo.toml` & `polars_lts_cpu-0.18.3/local_dependencies/polars-plan/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -125,15 +125,15 @@
 # defines the configuration attribute `docsrs`
 rustdoc-args = ["--cfg", "docsrs"]
 
 [dependencies.arrow]
 package = "arrow2"
 git = "https://github.com/jorgecarleitao/arrow2"
 # git = "https://github.com/ritchie46/arrow2"
-rev = "fb5e4d591c7149df590a330365fae55d2370962f"
+rev = "2d2e7053f9a50810bfe9cecff25ab39089aef98e"
 # path = "../arrow2"
 # branch = "polars_2023-05-25"
 version = "0.17"
 default-features = false
 features = [
   "compute_aggregate",
   "compute_arithmetics",
```

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/LICENSE` & `polars_lts_cpu-0.18.3/local_dependencies/polars-error/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dot.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/dot.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/arithmetic.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/dsl/arithmetic.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/arity.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/dsl/arity.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/array.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/dsl/array.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/binary.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/dsl/binary.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/cat.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/dsl/cat.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/dt.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/dsl/dt.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/expr.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/dsl/expr.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/expr_dyn_fn.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/dsl/expr_dyn_fn.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/from.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/dsl/from.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/function_expr/arg_where.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/dsl/function_expr/arg_where.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/function_expr/array.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/dsl/function_expr/array.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/function_expr/binary.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/dsl/function_expr/binary.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/function_expr/boolean.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/dsl/function_expr/boolean.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/function_expr/bounds.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/dsl/function_expr/bounds.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/function_expr/cat.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/dsl/function_expr/cat.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/function_expr/correlation.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/dsl/function_expr/correlation.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/function_expr/cum.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/dsl/function_expr/cum.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/function_expr/datetime.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/dsl/function_expr/datetime.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/function_expr/dispatch.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/dsl/function_expr/dispatch.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/function_expr/fill_null.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/dsl/function_expr/fill_null.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/function_expr/fused.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/dsl/function_expr/fused.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/function_expr/list.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/dsl/function_expr/list.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/function_expr/log.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/dsl/function_expr/log.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/function_expr/mod.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/dsl/function_expr/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/function_expr/pow.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/dsl/function_expr/pow.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/function_expr/schema.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/dsl/function_expr/schema.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/function_expr/shift_and_fill.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/dsl/function_expr/shift_and_fill.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/function_expr/shrink_type.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/dsl/function_expr/shrink_type.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/function_expr/sign.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/dsl/function_expr/sign.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/function_expr/strings.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/dsl/function_expr/strings.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/function_expr/struct_.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/dsl/function_expr/struct_.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/function_expr/temporal.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/dsl/function_expr/temporal.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/function_expr/trigonometry.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/dsl/function_expr/trigonometry.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/functions/arity.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/dsl/functions/arity.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/functions/coerce.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/dsl/functions/coerce.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/functions/concat.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/dsl/functions/concat.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/functions/correlation.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/dsl/functions/correlation.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/functions/horizontal.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/dsl/functions/horizontal.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/functions/index.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/dsl/functions/index.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/functions/mod.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/dsl/functions/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/functions/range.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/dsl/functions/range.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/functions/selectors.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/dsl/functions/selectors.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/functions/syntactic_sugar.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/dsl/functions/syntactic_sugar.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/functions/temporal.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/dsl/functions/temporal.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/list.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/dsl/list.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/meta.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/dsl/meta.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/mod.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/dsl/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/options.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/dsl/options.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/selector.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/dsl/selector.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/string.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/dsl/string.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/struct_.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/dsl/struct_.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/frame/opt_state.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/frame/opt_state.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/aexpr/mod.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/logical_plan/aexpr/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/aexpr/schema.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/logical_plan/aexpr/schema.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/alp.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/logical_plan/alp.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/anonymous_scan.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/logical_plan/anonymous_scan.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/apply.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/logical_plan/apply.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/builder.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/logical_plan/builder.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/conversion.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/logical_plan/conversion.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/format.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/logical_plan/format.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/functions/drop.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/logical_plan/functions/drop.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/functions/merge_sorted.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/logical_plan/functions/merge_sorted.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/functions/mod.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/logical_plan/functions/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/functions/rename.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/logical_plan/functions/rename.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/iterator.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/logical_plan/iterator.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/lit.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/logical_plan/lit.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/mod.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/logical_plan/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/optimizer/cache_states.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/logical_plan/optimizer/cache_states.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/optimizer/cse.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/logical_plan/optimizer/cse.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/optimizer/delay_rechunk.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/logical_plan/optimizer/delay_rechunk.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/optimizer/drop_nulls.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/logical_plan/optimizer/drop_nulls.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/optimizer/fast_projection.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/logical_plan/optimizer/fast_projection.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/optimizer/file_caching.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/logical_plan/optimizer/file_caching.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/optimizer/flatten_union.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/logical_plan/optimizer/flatten_union.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/optimizer/fused.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/logical_plan/optimizer/fused.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/optimizer/mod.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/logical_plan/optimizer/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/optimizer/predicate_pushdown/keys.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/logical_plan/optimizer/predicate_pushdown/keys.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/optimizer/predicate_pushdown/mod.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/logical_plan/optimizer/predicate_pushdown/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/optimizer/predicate_pushdown/rename.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/logical_plan/optimizer/predicate_pushdown/rename.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/optimizer/predicate_pushdown/utils.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/logical_plan/optimizer/predicate_pushdown/utils.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/functions/melt.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/functions/melt.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/functions/mod.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/functions/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/generic.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/generic.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/groupby.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/groupby.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/hstack.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/hstack.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/joins.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/joins.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/mod.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/projection.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/projection.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/rename.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/rename.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/semi_anti_join.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/semi_anti_join.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/optimizer/simplify_expr.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/logical_plan/optimizer/simplify_expr.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/optimizer/slice_pushdown_expr.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/logical_plan/optimizer/slice_pushdown_expr.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/optimizer/slice_pushdown_lp.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/logical_plan/optimizer/slice_pushdown_lp.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 use polars_core::prelude::*;
 
 use crate::prelude::*;
-use crate::utils::aexpr_is_simple_projection;
 
 pub(super) struct SlicePushDown {
     streaming: bool,
 }
 
 #[derive(Copy, Clone)]
 struct State {
@@ -347,37 +346,26 @@
              // State is None, we can continue
              m @(Projection{..}, None)
             => {
                 let (lp, state) = m;
                 self.pushdown_and_continue(lp, state, lp_arena, expr_arena)
             }
             // there is state, inspect the projection to determine how to deal with it
-            (Projection {input, mut expr, schema}, Some(State{offset, len})) => {
+            (Projection {input, expr, schema}, Some(_)) => {
                 // The slice operation may only pass on simple projections. col("foo").alias("bar")
                 if expr.iter().all(|root|  {
-                    aexpr_is_simple_projection(*root, expr_arena)
+                    aexpr_is_elementwise(*root, expr_arena)
                 }) {
                     let lp = Projection {input, expr, schema};
                     self.pushdown_and_continue(lp, state, lp_arena, expr_arena)
                 }
-                // we add a slice node to the projections
+                // don't push down slice, but restart optimization
                 else {
-                    let offset_node = to_aexpr(lit(offset), expr_arena);
-                    let length_node = to_aexpr(lit(len), expr_arena);
-                    expr.iter_mut().for_each(|node| {
-                        let aexpr = AExpr::Slice {
-                            input: *node,
-                            offset: offset_node,
-                            length: length_node
-                        };
-                        *node = expr_arena.add(aexpr)
-                    });
                     let lp = Projection {input, expr, schema};
-
-                    self.pushdown_and_continue(lp, None, lp_arena, expr_arena)
+                    self.no_pushdown_restart_opt(lp, state, lp_arena, expr_arena)
                 }
             }
             (catch_all, state) => {
                 self.no_pushdown_finish_opt(catch_all, state, lp_arena)
             }
 
         }
```

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/optimizer/stack_opt.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/logical_plan/optimizer/stack_opt.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/optimizer/type_coercion/binary.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/logical_plan/optimizer/type_coercion/binary.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/optimizer/type_coercion/mod.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/logical_plan/optimizer/type_coercion/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/options.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/logical_plan/options.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/projection.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/logical_plan/projection.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/pyarrow.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/logical_plan/pyarrow.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/schema.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/logical_plan/schema.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/prelude.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/prelude.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/utils.rs` & `polars_lts_cpu-0.18.3/local_dependencies/polars-plan/src/utils.rs`

 * *Files 2% similar despite different names*

```diff
@@ -93,14 +93,32 @@
 /// A projection that only takes a column or a column + alias.
 pub(crate) fn aexpr_is_simple_projection(current_node: Node, arena: &Arena<AExpr>) -> bool {
     arena
         .iter(current_node)
         .all(|(_node, e)| matches!(e, AExpr::Column(_) | AExpr::Alias(_, _)))
 }
 
+pub(crate) fn aexpr_is_elementwise(current_node: Node, arena: &Arena<AExpr>) -> bool {
+    arena.iter(current_node).all(|(_node, e)| {
+        use AExpr::*;
+        match e {
+            AnonymousFunction { options, .. } | Function { options, .. } => {
+                !matches!(options.collect_groups, ApplyOptions::ApplyGroups)
+            }
+            Column(_)
+            | Alias(_, _)
+            | Literal(_)
+            | BinaryExpr { .. }
+            | Ternary { .. }
+            | Cast { .. } => true,
+            _ => false,
+        }
+    })
+}
+
 pub fn has_aexpr<F>(current_node: Node, arena: &Arena<AExpr>, matches: F) -> bool
 where
     F: Fn(&AExpr) -> bool,
 {
     arena.iter(current_node).any(|(_node, e)| matches(e))
 }
```

### Comparing `polars_lts_cpu-0.18.2/Cargo.toml` & `polars_lts_cpu-0.18.3/Cargo.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "py-polars"
-version = "0.18.2"
+version = "0.18.3"
 edition = "2021"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 
 [workspace]
 # prevents package from thinking it's in the workspace
 [target.'cfg(any(not(target_os = "linux"), use_mimalloc))'.dependencies]
```

### Comparing `polars_lts_cpu-0.18.2/LICENSE` & `polars_lts_cpu-0.18.3/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/Makefile` & `polars_lts_cpu-0.18.3/Makefile`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/README.md` & `polars_lts_cpu-0.18.3/README.md`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/build.rs` & `polars_lts_cpu-0.18.3/build.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/docs/Makefile` & `polars_lts_cpu-0.18.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/docs/_templates/autosummary/class.rst` & `polars_lts_cpu-0.18.3/docs/_templates/autosummary/class.rst`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/docs/run_live_docs_server.py` & `polars_lts_cpu-0.18.3/docs/run_live_docs_server.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/docs/source/_static/css/custom.css` & `polars_lts_cpu-0.18.3/docs/source/_static/css/custom.css`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/docs/source/conf.py` & `polars_lts_cpu-0.18.3/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/docs/source/reference/api.rst` & `polars_lts_cpu-0.18.3/docs/source/reference/api.rst`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/docs/source/reference/config.rst` & `polars_lts_cpu-0.18.3/docs/source/reference/config.rst`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/docs/source/reference/dataframe/modify_select.rst` & `polars_lts_cpu-0.18.3/docs/source/reference/dataframe/modify_select.rst`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/docs/source/reference/datatypes.rst` & `polars_lts_cpu-0.18.3/docs/source/reference/datatypes.rst`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/docs/source/reference/expressions/computation.rst` & `polars_lts_cpu-0.18.3/docs/source/reference/expressions/computation.rst`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/docs/source/reference/expressions/functions.rst` & `polars_lts_cpu-0.18.3/docs/source/reference/expressions/functions.rst`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/docs/source/reference/expressions/list.rst` & `polars_lts_cpu-0.18.3/docs/source/reference/expressions/list.rst`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/docs/source/reference/expressions/modify_select.rst` & `polars_lts_cpu-0.18.3/docs/source/reference/expressions/modify_select.rst`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/docs/source/reference/expressions/operators.rst` & `polars_lts_cpu-0.18.3/docs/source/reference/expressions/operators.rst`

 * *Files 14% similar despite different names*

```diff
@@ -19,19 +19,21 @@
 Comparison
 ~~~~~~~~~~
 
 .. autosummary::
    :toctree: api/
 
     Expr.eq
+    Expr.eq_missing
     Expr.ge
     Expr.gt
     Expr.le
     Expr.lt
     Expr.ne
+    Expr.ne_missing
 
 Numeric
 ~~~~~~~
 
 .. autosummary::
    :toctree: api/
```

### Comparing `polars_lts_cpu-0.18.2/docs/source/reference/expressions/string.rst` & `polars_lts_cpu-0.18.3/docs/source/reference/expressions/string.rst`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/docs/source/reference/expressions/temporal.rst` & `polars_lts_cpu-0.18.3/docs/source/reference/expressions/temporal.rst`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/docs/source/reference/functions.rst` & `polars_lts_cpu-0.18.3/docs/source/reference/functions.rst`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/docs/source/reference/io.rst` & `polars_lts_cpu-0.18.3/docs/source/reference/io.rst`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/docs/source/reference/lazyframe/modify_select.rst` & `polars_lts_cpu-0.18.3/docs/source/reference/lazyframe/modify_select.rst`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/docs/source/reference/selectors.rst` & `polars_lts_cpu-0.18.3/docs/source/reference/selectors.rst`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/docs/source/reference/series/computation.rst` & `polars_lts_cpu-0.18.3/docs/source/reference/series/computation.rst`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/docs/source/reference/series/descriptive.rst` & `polars_lts_cpu-0.18.3/docs/source/reference/series/descriptive.rst`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/docs/source/reference/series/list.rst` & `polars_lts_cpu-0.18.3/docs/source/reference/series/list.rst`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/docs/source/reference/series/modify_select.rst` & `polars_lts_cpu-0.18.3/docs/source/reference/series/modify_select.rst`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/docs/source/reference/series/string.rst` & `polars_lts_cpu-0.18.3/docs/source/reference/series/string.rst`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/docs/source/reference/series/temporal.rst` & `polars_lts_cpu-0.18.3/docs/source/reference/series/temporal.rst`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/docs/source/reference/testing.rst` & `polars_lts_cpu-0.18.3/docs/source/reference/testing.rst`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/polars/__init__.py` & `polars_lts_cpu-0.18.3/polars/__init__.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/polars/api.py` & `polars_lts_cpu-0.18.3/polars/api.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/polars/config.py` & `polars_lts_cpu-0.18.3/polars/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from __future__ import annotations
 
 import contextlib
 import os
+from pathlib import Path
 from typing import TYPE_CHECKING, Any
 
 from polars.dependencies import json
+from polars.utils.various import normalise_filepath
 
 
 # dummy func required (so docs build)
 def _get_float_fmt() -> str:
     return "n/a"
 
 
@@ -143,25 +145,29 @@
         exc_tb: TracebackType | None,
     ) -> None:
         """Reset any Config options that were set within the scope."""
         self.restore_defaults().load(self._original_state)
         self._original_state = ""
 
     @classmethod
-    def load(cls, cfg: str) -> type[Config]:
+    def load(cls, cfg: Path | str) -> type[Config]:
         """
-        Load and set previously saved (or shared) Config options.
+        Load and set previously saved (or shared) Config options from json/file.
 
         Parameters
         ----------
         cfg : str
-            json string produced by ``Config.save()``.
+            json string produced by ``Config.save()``, or a filepath to the same.
 
         """
-        options = json.loads(cfg)
+        options = json.loads(
+            Path(normalise_filepath(cfg)).read_text()
+            if isinstance(cfg, Path) or os.path.exists(cfg)
+            else cfg
+        )
         os.environ.update(options.get("environment", {}))
         for cfg_methodname, value in options.get("direct", {}).items():
             if hasattr(cls, cfg_methodname):
                 getattr(cls, cfg_methodname)(value)
         return cls
 
     @classmethod
@@ -184,36 +190,51 @@
             os.environ.pop(var, None)
 
         # apply any 'direct' setting values
         cls.set_fmt_float()
         return cls
 
     @classmethod
-    def save(cls) -> str:
+    def save(cls, file: Path | str | None = None) -> str:
         """
-        Save the current set of Config options as a json string.
+        Save the current set of Config options as a json string or file.
+
+        Parameters
+        ----------
+        file
+            optional path to a file into which the json string will be written.
 
         Examples
         --------
         >>> cfg = pl.Config.save()
 
+        Returns
+        -------
+        str : json string containing current Config options, or filepath where saved.
+
         """
         environment_vars = {
             key: os.environ[key]
             for key in sorted(_POLARS_CFG_ENV_VARS)
             if (key in os.environ)
         }
         direct_vars = {
             cfg_methodname: get_value()
             for cfg_methodname, get_value in _POLARS_CFG_DIRECT_VARS.items()
         }
-        return json.dumps(
+        options = json.dumps(
             {"environment": environment_vars, "direct": direct_vars},
             separators=(",", ":"),
         )
+        if isinstance(file, (str, Path)):
+            file = os.path.abspath(normalise_filepath(file))
+            Path(file).write_text(options)
+            return file
+
+        return options
 
     @classmethod
     def state(
         cls, if_set: bool = False, env_only: bool = False
     ) -> dict[str, str | None]:
         """
         Show the current state of all Config variables as a dict.
```

### Comparing `polars_lts_cpu-0.18.2/polars/convert.py` & `polars_lts_cpu-0.18.3/polars/convert.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/polars/dataframe/_html.py` & `polars_lts_cpu-0.18.3/polars/dataframe/_html.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/polars/dataframe/frame.py` & `polars_lts_cpu-0.18.3/polars/dataframe/frame.py`

 * *Files 0% similar despite different names*

```diff
@@ -134,14 +134,15 @@
         DbWriteEngine,
         DbWriteMode,
         FillNullStrategy,
         FrameInitTypes,
         IntoExpr,
         IpcCompression,
         JoinStrategy,
+        JoinValidation,
         NullStrategy,
         OneOrMoreDataTypes,
         Orientation,
         ParallelStrategy,
         ParquetCompression,
         PivotAgg,
         PolarsDataType,
@@ -3322,15 +3323,15 @@
         ... )  # doctest: +SKIP
 
         """
         from polars.io.delta import check_if_delta_available, resolve_delta_lake_uri
 
         check_if_delta_available()
 
-        from deltalake.writer import (  # type: ignore[import]
+        from deltalake.writer import (
             try_get_deltatable,
             write_deltalake,
         )
 
         if delta_write_options is None:
             delta_write_options = {}
 
@@ -3357,15 +3358,15 @@
                 f"Column(s) in {unsupported_cols} have unsupported data types."
             )
 
         data = self.to_arrow()
         data_schema = data.schema
 
         # Workaround to prevent manual casting of large types
-        table = try_get_deltatable(target, storage_options)
+        table = try_get_deltatable(target, storage_options)  # type: ignore[arg-type]
 
         if table is not None:
             table_schema = table.schema()
 
             if data_schema == table_schema.to_pyarrow(as_large_types=True):
                 data_schema = table_schema.to_pyarrow()
 
@@ -4983,34 +4984,57 @@
         closed : {'left', 'right', 'both', 'none'}
             Define which sides of the temporal interval are closed (inclusive).
         by
             Also group by this column/these columns
         start_by : {'window', 'datapoint', 'monday', 'tuesday', 'wednesday', 'thursday', 'friday', 'saturday', 'sunday'}
             The strategy to determine the start of the first window by.
 
-            - 'window': Truncate the start of the window with the 'every' argument.
-            - 'datapoint': Start from the first encountered data point.
-            - 'monday': Start the window on the monday before the first data point.
-            - 'tuesday': Start the window on the tuesday before the first data point.
-            - ...
-            - 'sunday': Start the window on the sunday before the first data point.
+            * 'window': Truncate the start of the window with the 'every' argument.
+              Note that weekly windows start on Monday.
+            * 'datapoint': Start from the first encountered data point.
+            * a day of the week (only takes effect if `every` contains ``'w'``):
+
+              * 'monday': Start the window on the Monday before the first data point.
+              * 'tuesday': Start the window on the Tuesday before the first data point.
+              * ...
+              * 'sunday': Start the window on the Sunday before the first data point.
         check_sorted
             When the ``by`` argument is given, polars can not check sortedness
             by the metadata and has to do a full scan on the index column to
             verify data is sorted. This is expensive. If you are sure the
             data within the by groups is sorted, you can set this to ``False``.
             Doing so incorrectly will lead to incorrect output
 
         Returns
         -------
         DynamicGroupBy
             Object you can call ``.agg`` on to aggregate by groups, the result
             of which will be sorted by `index_column` (but note that if `by` columns are
             passed, it will only be sorted within each `by` group).
 
+        Notes
+        -----
+        If you're coming from pandas, then
+
+        .. code-block:: python
+
+            # polars
+            df.groupby_dynamic("ts", every="1d").agg(pl.col("value").sum())
+
+        is equivalent to
+
+        .. code-block:: python
+
+            # pandas
+            df.set_index("ts").resample("D")["value"].sum().reset_index()
+
+        though note that, unlike pandas, polars doesn't add extra rows for empty
+        windows. If you need `index_column` to be evenly spaced, then please combine
+        with :func:`DataFrame.upsample`.
+
         Examples
         --------
         >>> from datetime import datetime
         >>> # create an example dataframe
         >>> df = pl.DataFrame(
         ...     {
         ...         "time": pl.date_range(
@@ -5215,28 +5239,14 @@
         offset: str | timedelta | None = None,
         by: str | Sequence[str] | None = None,
         maintain_order: bool = False,
     ) -> Self:
         """
         Upsample a DataFrame at a regular frequency.
 
-        Parameters
-        ----------
-        time_column
-            time column will be used to determine a date_range.
-            Note that this column has to be sorted for the output to make sense.
-        every
-            interval will start 'every' duration
-        offset
-            change the start of the date_range by this offset.
-        by
-            First group by these columns and then upsample for every group
-        maintain_order
-            Keep the ordering predictable. This is slower.
-
         The `every` and `offset` arguments are created with
         the following string language:
 
         - 1ns   (1 nanosecond)
         - 1us   (1 microsecond)
         - 1ms   (1 millisecond)
         - 1s    (1 second)
@@ -5246,20 +5256,35 @@
         - 1w    (1 week)
         - 1mo   (1 calendar month)
         - 1q    (1 calendar quarter)
         - 1y    (1 calendar year)
         - 1i    (1 index count)
 
         Or combine them:
-        "3d12h4m25s" # 3 days, 12 hours, 4 minutes, and 25 seconds
+
+        - "3d12h4m25s" # 3 days, 12 hours, 4 minutes, and 25 seconds
 
         Suffix with `"_saturating"` to indicate that dates too large for
         their month should saturate at the largest date (e.g. 2022-02-29 -> 2022-02-28)
         instead of erroring.
 
+        Parameters
+        ----------
+        time_column
+            time column will be used to determine a date_range.
+            Note that this column has to be sorted for the output to make sense.
+        every
+            interval will start 'every' duration
+        offset
+            change the start of the date_range by this offset.
+        by
+            First group by these columns and then upsample for every group
+        maintain_order
+            Keep the ordering predictable. This is slower.
+
         Returns
         -------
         DataFrame
             Result will be sorted by `time_column` (but note that if `by` columns are
             passed, it will only be sorted within each `by` group).
 
         Examples
@@ -5471,15 +5496,15 @@
         other: DataFrame,
         on: str | Expr | Sequence[str | Expr] | None = None,
         how: JoinStrategy = "inner",
         *,
         left_on: str | Expr | Sequence[str | Expr] | None = None,
         right_on: str | Expr | Sequence[str | Expr] | None = None,
         suffix: str = "_right",
-        validate: str = "m:m",
+        validate: JoinValidation = "m:m",
     ) -> DataFrame:
         """
         Join in SQL-like fashion.
 
         Parameters
         ----------
         other
@@ -5490,15 +5515,15 @@
             Join strategy.
         left_on
             Name(s) of the left join column(s).
         right_on
             Name(s) of the right join column(s).
         suffix
             Suffix to append to columns with a duplicate name.
-        validate: {'m:m', 'm:1', '1:m', 'm:m'}
+        validate: {'m:m', 'm:1', '1:m', '1:1'}
             Checks if join is of specified type.
 
                 * *many_to_many*
                     “m:m”: default, does not result in checks
                 * *one_to_one*
                     “1:1”: check if join keys are unique in both left and right datasets
                 * *one_to_many*
```

### Comparing `polars_lts_cpu-0.18.2/polars/dataframe/groupby.py` & `polars_lts_cpu-0.18.3/polars/dataframe/groupby.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/polars/datatypes/__init__.py` & `polars_lts_cpu-0.18.3/polars/datatypes/__init__.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/polars/datatypes/classes.py` & `polars_lts_cpu-0.18.3/polars/datatypes/classes.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/polars/datatypes/constants.py` & `polars_lts_cpu-0.18.3/polars/datatypes/constants.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/polars/datatypes/constructor.py` & `polars_lts_cpu-0.18.3/polars/datatypes/constructor.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/polars/datatypes/convert.py` & `polars_lts_cpu-0.18.3/polars/datatypes/convert.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/polars/dependencies.py` & `polars_lts_cpu-0.18.3/polars/dependencies.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/polars/exceptions.py` & `polars_lts_cpu-0.18.3/polars/exceptions.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/polars/expr/array.py` & `polars_lts_cpu-0.18.3/polars/expr/array.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/polars/expr/binary.py` & `polars_lts_cpu-0.18.3/polars/expr/binary.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/polars/expr/categorical.py` & `polars_lts_cpu-0.18.3/polars/expr/categorical.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/polars/expr/datetime.py` & `polars_lts_cpu-0.18.3/polars/expr/datetime.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,16 @@
         self,
         every: str | timedelta,
         offset: str | timedelta | None = None,
     ) -> Expr:
         """
         Divide the date/datetime range into buckets.
 
-        Each date/datetime is mapped to the start of its bucket.
+        Each date/datetime is mapped to the start of its bucket. Note that weekly
+        buckets start on Monday.
 
         Parameters
         ----------
         every
             Every interval start and period length
         offset
             Offset the window
```

### Comparing `polars_lts_cpu-0.18.2/polars/expr/expr.py` & `polars_lts_cpu-0.18.3/polars/expr/expr.py`

 * *Files 0% similar despite different names*

```diff
@@ -3289,14 +3289,19 @@
         function
             Lambda/ function to apply.
         return_dtype
             Dtype of the output Series.
         agg_list
             Aggregate list
 
+        Warnings
+        --------
+        If ``return_dtype`` is not provided, this may lead to unexpected results.
+        We allow this, but it is considered a bug in the user's query.
+
         See Also
         --------
         map_dict
 
         Examples
         --------
         >>> df = pl.DataFrame(
@@ -3337,24 +3342,14 @@
         * Selection
             Expects `f` to be of type Callable[[Any], Any].
             Applies a python function over each individual value in the column.
         * GroupBy
             Expects `f` to be of type Callable[[Series], Series].
             Applies a python function over each group.
 
-        Notes
-        -----
-        * Using ``apply`` is strongly discouraged as you will be effectively running
-          python "for" loops. This will be very slow. Wherever possible you should
-          strongly prefer the native expression API to achieve the best performance.
-
-        * If your function is expensive and you don't want it to be called more than
-          once for a given input, consider applying an ``@lru_cache`` decorator to it.
-          With suitable data you may achieve order-of-magnitude speedups (or more).
-
         Parameters
         ----------
         function
             Lambda/ function to apply.
         return_dtype
             Dtype of the output Series.
             If not set, the dtype will be
@@ -3372,14 +3367,29 @@
             - 'thread_local': run the python function on a single thread.
             - 'threading': run the python function on separate threads. Use with
                         care as this can slow performance. This might only speed up
                         your code if the amount of work per element is significant
                         and the python function releases the GIL (e.g. via calling
                         a c function)
 
+        Notes
+        -----
+        * Using ``apply`` is strongly discouraged as you will be effectively running
+          python "for" loops. This will be very slow. Wherever possible you should
+          strongly prefer the native expression API to achieve the best performance.
+
+        * If your function is expensive and you don't want it to be called more than
+          once for a given input, consider applying an ``@lru_cache`` decorator to it.
+          With suitable data you may achieve order-of-magnitude speedups (or more).
+
+        Warnings
+        --------
+        If ``return_dtype`` is not provided, this may lead to unexpected results.
+        We allow this, but it is considered a bug in the user's query.
+
         Examples
         --------
         >>> df = pl.DataFrame(
         ...     {
         ...         "a": [1, 2, 3, 1],
         ...         "b": ["a", "b", "c", "c"],
         ...     }
@@ -4324,15 +4334,15 @@
         │ true     │
         │ false    │
         └──────────┘
 
         """
         if isinstance(other, Collection) and not isinstance(other, str):
             if isinstance(other, (Set, FrozenSet)):
-                other = sorted(other)
+                other = list(other)
             other = F.lit(None) if len(other) == 0 else F.lit(pl.Series(other))
             other = other._pyexpr
         else:
             other = parse_as_expression(other)
         return self._from_pyexpr(self._pyexpr.is_in(other))
 
     def repeat_by(self, by: pl.Series | Expr | str | int) -> Self:
```

### Comparing `polars_lts_cpu-0.18.2/polars/expr/list.py` & `polars_lts_cpu-0.18.3/polars/expr/list.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/polars/expr/meta.py` & `polars_lts_cpu-0.18.3/polars/expr/meta.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/polars/expr/string.py` & `polars_lts_cpu-0.18.3/polars/expr/string.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/polars/expr/struct.py` & `polars_lts_cpu-0.18.3/polars/expr/struct.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/polars/functions/__init__.py` & `polars_lts_cpu-0.18.3/polars/functions/__init__.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/polars/functions/as_datatype.py` & `polars_lts_cpu-0.18.3/polars/functions/as_datatype.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/polars/functions/eager.py` & `polars_lts_cpu-0.18.3/polars/functions/eager.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,14 +45,16 @@
     items
         DataFrames, LazyFrames, or Series to concatenate.
     how : {'vertical', 'diagonal', 'horizontal', 'align'}
         Series only support the `vertical` strategy.
         LazyFrames do not support the `horizontal` strategy.
 
         * vertical: Applies multiple `vstack` operations.
+        * vertical_relaxed: Applies multiple `vstack` operations and coerces column
+          dtypes that are not equal to their supertypes.
         * diagonal: Finds a union between the column schemas and fills missing column
           values with ``null``.
         * horizontal: Stacks Series from DataFrames horizontally and fills with ``null``
           if the lengths don't match.
         * align: Combines frames horizontally, auto-determining the common key columns
           and aligning rows using the same logic as ``align_frames``; this behaviour is
           patterned after a full outer join, but does not handle column-name collision.
@@ -158,31 +160,37 @@
 
     out: Series | DataFrame | LazyFrame | Expr
     first = elems[0]
 
     if isinstance(first, pl.DataFrame):
         if how == "vertical":
             out = wrap_df(plr.concat_df(elems))
+        elif how == "vertical_relaxed":
+            out = wrap_ldf(
+                plr.concat_lf([df.lazy() for df in elems], rechunk, parallel, True)
+            ).collect(no_optimization=True)
         elif how == "diagonal":
             out = wrap_df(plr.diag_concat_df(elems))
         elif how == "horizontal":
             out = wrap_df(plr.hor_concat_df(elems))
         else:
             raise ValueError(
-                f"`how` must be one of {{'vertical','diagonal','horizontal','align'}}, "
+                f"`how` must be one of {{'vertical','vertical_relaxed','diagonal','horizontal','align'}}, "
                 f"got {how!r}"
             )
     elif isinstance(first, pl.LazyFrame):
         if how == "vertical":
-            return wrap_ldf(plr.concat_lf(elems, rechunk, parallel))
+            return wrap_ldf(plr.concat_lf(elems, rechunk, parallel, False))
+        if how == "vertical_relaxed":
+            return wrap_ldf(plr.concat_lf(elems, rechunk, parallel, True))
         if how == "diagonal":
             return wrap_ldf(plr.diag_concat_lf(elems, rechunk, parallel))
         else:
             raise ValueError(
-                "'LazyFrame' only allows {'vertical','diagonal','align'} concat strategies."
+                "'LazyFrame' only allows {'vertical','vertical_relaxed','diagonal','align'} concat strategies."
             )
     elif isinstance(first, pl.Series):
         if how == "vertical":
             out = wrap_s(plr.concat_series(elems))
         else:
             raise ValueError("'Series' only allows {'vertical'} concat strategy.")
```

### Comparing `polars_lts_cpu-0.18.2/polars/functions/lazy.py` & `polars_lts_cpu-0.18.3/polars/functions/lazy.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/polars/functions/range.py` & `polars_lts_cpu-0.18.3/polars/functions/range.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/polars/functions/repeat.py` & `polars_lts_cpu-0.18.3/polars/functions/repeat.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/polars/functions/whenthen.py` & `polars_lts_cpu-0.18.3/polars/functions/whenthen.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/polars/io/__init__.py` & `polars_lts_cpu-0.18.3/polars/io/__init__.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/polars/io/_utils.py` & `polars_lts_cpu-0.18.3/polars/io/_utils.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/polars/io/avro.py` & `polars_lts_cpu-0.18.3/polars/io/avro.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/polars/io/csv/_utils.py` & `polars_lts_cpu-0.18.3/polars/io/csv/_utils.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/polars/io/csv/batched_reader.py` & `polars_lts_cpu-0.18.3/polars/io/csv/batched_reader.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/polars/io/csv/functions.py` & `polars_lts_cpu-0.18.3/polars/io/csv/functions.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/polars/io/database.py` & `polars_lts_cpu-0.18.3/polars/io/database.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/polars/io/delta.py` & `polars_lts_cpu-0.18.3/polars/io/delta.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/polars/io/excel/_write_utils.py` & `polars_lts_cpu-0.18.3/polars/io/excel/_write_utils.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/polars/io/excel/functions.py` & `polars_lts_cpu-0.18.3/polars/io/excel/functions.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/polars/io/ipc/anonymous_scan.py` & `polars_lts_cpu-0.18.3/polars/io/ipc/anonymous_scan.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/polars/io/ipc/functions.py` & `polars_lts_cpu-0.18.3/polars/io/ipc/functions.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/polars/io/ndjson.py` & `polars_lts_cpu-0.18.3/polars/io/ndjson.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/polars/io/parquet/anonymous_scan.py` & `polars_lts_cpu-0.18.3/polars/io/parquet/anonymous_scan.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/polars/io/parquet/functions.py` & `polars_lts_cpu-0.18.3/polars/io/parquet/functions.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/polars/io/pyarrow_dataset/anonymous_scan.py` & `polars_lts_cpu-0.18.3/polars/io/pyarrow_dataset/anonymous_scan.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/polars/io/pyarrow_dataset/functions.py` & `polars_lts_cpu-0.18.3/polars/io/pyarrow_dataset/functions.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/polars/lazyframe/frame.py` & `polars_lts_cpu-0.18.3/polars/lazyframe/frame.py`

 * *Files 0% similar despite different names*

```diff
@@ -78,14 +78,15 @@
         AsofJoinStrategy,
         ClosedInterval,
         CsvEncoding,
         FillNullStrategy,
         FrameInitTypes,
         IntoExpr,
         JoinStrategy,
+        JoinValidation,
         Orientation,
         ParallelStrategy,
         PolarsDataType,
         RollingInterpolationMethod,
         SchemaDefinition,
         SchemaDict,
         StartBy,
@@ -2380,19 +2381,22 @@
             Define which sides of the temporal interval are closed (inclusive).
         by
             Also group by this column/these columns
         start_by : {'window', 'datapoint', 'monday', 'tuesday', 'wednesday', 'thursday', 'friday', 'saturday', 'sunday'}
             The strategy to determine the start of the first window by.
 
             * 'window': Truncate the start of the window with the 'every' argument.
+              Note that weekly windows start on Monday.
             * 'datapoint': Start from the first encountered data point.
-            * 'monday': Start the window on the monday before the first data point.
-            * 'tuesday': Start the window on the tuesday before the first data point.
-            * ...
-            * 'sunday': Start the window on the sunday before the first data point.
+            * a day of the week (only takes effect if `every` contains ``'w'``):
+
+              * 'monday': Start the window on the Monday before the first data point.
+              * 'tuesday': Start the window on the Tuesday before the first data point.
+              * ...
+              * 'sunday': Start the window on the Sunday before the first data point.
         check_sorted
             When the ``by`` argument is given, polars can not check sortedness
             by the metadata and has to do a full scan on the index column to
             verify data is sorted. This is expensive. If you are sure the
             data within the by groups is sorted, you can set this to ``False``.
             Doing so incorrectly will lead to incorrect output
 
@@ -2403,14 +2407,34 @@
             of which will be sorted by `index_column` (but note that if `by` columns are
             passed, it will only be sorted within each `by` group).
 
         See Also
         --------
         groupby_rolling
 
+        Notes
+        -----
+        If you're coming from pandas, then
+
+        .. code-block:: python
+
+            # polars
+            df.groupby_dynamic("ts", every="1d").agg(pl.col("value").sum())
+
+        is equivalent to
+
+        .. code-block:: python
+
+            # pandas
+            df.set_index("ts").resample("D")["value"].sum().reset_index()
+
+        though note that, unlike pandas, polars doesn't add extra rows for empty
+        windows. If you need `index_column` to be evenly spaced, then please combine
+        with :func:`DataFrame.upsample`.
+
         Examples
         --------
         >>> from datetime import datetime
         >>> # create an example dataframe
         >>> lf = pl.LazyFrame(
         ...     {
         ...         "time": pl.date_range(
@@ -2807,15 +2831,15 @@
         other: LazyFrame,
         on: str | Expr | Sequence[str | Expr] | None = None,
         how: JoinStrategy = "inner",
         *,
         left_on: str | Expr | Sequence[str | Expr] | None = None,
         right_on: str | Expr | Sequence[str | Expr] | None = None,
         suffix: str = "_right",
-        validate: str = "m:m",
+        validate: JoinValidation = "m:m",
         allow_parallel: bool = True,
         force_parallel: bool = False,
     ) -> Self:
         """
         Add a join operation to the Logical Plan.
 
         Parameters
@@ -2829,15 +2853,15 @@
             Join strategy.
         left_on
             Join column of the left DataFrame.
         right_on
             Join column of the right DataFrame.
         suffix
             Suffix to append to columns with a duplicate name.
-        validate: {'m:m', 'm:1', '1:m', 'm:m'}
+        validate: {'m:m', 'm:1', '1:m', '1:1'}
             Checks if join is of specified type.
 
                 * *many_to_many*
                     “m:m”: default, does not result in checks
                 * *one_to_one*
                     “1:1”: check if join keys are unique in both left and right datasets
                 * *one_to_many*
```

### Comparing `polars_lts_cpu-0.18.2/polars/lazyframe/groupby.py` & `polars_lts_cpu-0.18.3/polars/lazyframe/groupby.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/polars/selectors.py` & `polars_lts_cpu-0.18.3/polars/selectors.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/polars/series/_numpy.py` & `polars_lts_cpu-0.18.3/polars/series/_numpy.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/polars/series/array.py` & `polars_lts_cpu-0.18.3/polars/series/array.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/polars/series/binary.py` & `polars_lts_cpu-0.18.3/polars/series/binary.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/polars/series/categorical.py` & `polars_lts_cpu-0.18.3/polars/series/categorical.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/polars/series/datetime.py` & `polars_lts_cpu-0.18.3/polars/series/datetime.py`

 * *Files 0% similar despite different names*

```diff
@@ -1562,15 +1562,16 @@
         self,
         every: str | dt.timedelta,
         offset: str | dt.timedelta | None = None,
     ) -> Series:
         """
         Divide the date/ datetime range into buckets.
 
-        Each date/datetime is mapped to the start of its bucket.
+        Each date/datetime is mapped to the start of its bucket. Note that weekly
+        buckets start on Monday.
 
         Parameters
         ----------
         every
             Every interval start and period length
         offset
             Offset the window
@@ -1683,27 +1684,29 @@
         is mapped to the start of its bucket.
         Each date/datetime in the second half of the interval
         is mapped to the end of its bucket.
 
         The `every` and `offset` argument are created with the
         the following string language:
 
-        1ns # 1 nanosecond
-        1us # 1 microsecond
-        1ms # 1 millisecond
-        1s  # 1 second
-        1m  # 1 minute
-        1h  # 1 hour
-        1d  # 1 day
-        1w  # 1 calendar week
-        1mo # 1 calendar month
-        1q  # 1 calendar quarter
-        1y  # 1 calendar year
+        - 1ns # 1 nanosecond
+        - 1us # 1 microsecond
+        - 1ms # 1 millisecond
+        - 1s  # 1 second
+        - 1m  # 1 minute
+        - 1h  # 1 hour
+        - 1d  # 1 day
+        - 1w  # 1 calendar week
+        - 1mo # 1 calendar month
+        - 1q  # 1 calendar quarter
+        - 1y  # 1 calendar year
 
-        3d12h4m25s # 3 days, 12 hours, 4 minutes, and 25 seconds
+        These strings can be combined:
+
+        - 3d12h4m25s # 3 days, 12 hours, 4 minutes, and 25 seconds
 
         Suffix with `"_saturating"` to indicate that dates too large for
         their month should saturate at the largest date (e.g. 2022-02-29 -> 2022-02-28)
         instead of erroring.
 
         Parameters
         ----------
```

### Comparing `polars_lts_cpu-0.18.2/polars/series/list.py` & `polars_lts_cpu-0.18.3/polars/series/list.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/polars/series/series.py` & `polars_lts_cpu-0.18.3/polars/series/series.py`

 * *Files 1% similar despite different names*

```diff
@@ -4249,14 +4249,19 @@
             Output datatype. If none is given, the same datatype as this Series will be
             used.
         skip_nulls
             Nulls will be skipped and not passed to the python function.
             This is faster because python can be skipped and because we call
             more specialized functions.
 
+        Warnings
+        --------
+        If ``return_dtype`` is not provided, this may lead to unexpected results.
+        We allow this, but it is considered a bug in the user's query.
+
         Notes
         -----
         If your function is expensive and you don't want it to be called more than
         once for a given input, consider applying an ``@lru_cache`` decorator to it.
         With suitable data you may achieve order-of-magnitude speedups (or more).
 
         Examples
```

### Comparing `polars_lts_cpu-0.18.2/polars/series/string.py` & `polars_lts_cpu-0.18.3/polars/series/string.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/polars/series/struct.py` & `polars_lts_cpu-0.18.3/polars/series/struct.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/polars/series/utils.py` & `polars_lts_cpu-0.18.3/polars/series/utils.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/polars/slice.py` & `polars_lts_cpu-0.18.3/polars/slice.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/polars/sql/context.py` & `polars_lts_cpu-0.18.3/polars/sql/context.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/polars/string_cache.py` & `polars_lts_cpu-0.18.3/polars/string_cache.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/polars/testing/_private.py` & `polars_lts_cpu-0.18.3/polars/testing/_private.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/polars/testing/asserts.py` & `polars_lts_cpu-0.18.3/polars/testing/asserts.py`

 * *Files 5% similar despite different names*

```diff
@@ -311,22 +311,14 @@
     check_dtype: bool,
     check_exact: bool,
     nans_compare_equal: bool,
     atol: float,
     rtol: float,
 ) -> None:
     """Compare Series dtype + values."""
-    try:
-        can_be_subtracted = hasattr(dtype_to_py_type(left.dtype), "__sub__")
-    except NotImplementedError:
-        can_be_subtracted = False
-
-    check_exact = (
-        check_exact or not can_be_subtracted or left.is_boolean() or left.is_temporal()
-    )
     if check_dtype and left.dtype != right.dtype:
         raise_assert_detail("Series", "Dtype mismatch", left.dtype, right.dtype)
 
     if left.null_count() != right.null_count():
         raise_assert_detail(
             "Series", "null_count is not equal", left.null_count(), right.null_count()
         )
@@ -339,25 +331,35 @@
     if unequal.any() and nans_compare_equal:
         # when both dtypes are scalar floats
         if comparing_float_dtypes:
             unequal = unequal & ~(
                 (left.is_nan() & right.is_nan()).fill_null(F.lit(False))
             )
 
-        # account for float values in nested dtypes
-        elif left.dtype.is_nested or right.dtype.is_nested:
-            if _assert_series_nested_nans_equal(
-                left=left.filter(unequal),
-                right=right.filter(unequal),
-                check_dtype=check_dtype,
-                check_exact=check_exact,
-                atol=atol,
-                rtol=rtol,
-            ):
-                return
+    # check nested dtypes in separate function
+    if left.dtype.is_nested or right.dtype.is_nested:
+        if _assert_series_nested(
+            left=left.filter(unequal),
+            right=right.filter(unequal),
+            check_dtype=check_dtype,
+            check_exact=check_exact,
+            nans_compare_equal=nans_compare_equal,
+            atol=atol,
+            rtol=rtol,
+        ):
+            return
+
+    try:
+        can_be_subtracted = hasattr(dtype_to_py_type(left.dtype), "__sub__")
+    except NotImplementedError:
+        can_be_subtracted = False
+
+    check_exact = (
+        check_exact or not can_be_subtracted or left.is_boolean() or left.is_temporal()
+    )
 
     # assert exact, or with tolerance
     if unequal.any():
         if check_exact:
             raise_assert_detail(
                 "Series",
                 "Exact value mismatch",
@@ -377,15 +379,18 @@
             mismatch, nan_info = False, ""
             if ((s_diff > (atol + rtol * right.abs())).sum() != 0) or (
                 left.is_null() != right.is_null()
             ).any():
                 mismatch = True
             elif comparing_float_dtypes:
                 # note: take special care with NaN values.
-                if not nans_compare_equal and (left.is_nan() == right.is_nan()).any():
+                # if NaNs don't compare as equal, any NaN in the left Series is
+                # sufficient for a mismatch because the if condition above already
+                # compares the null values.
+                if not nans_compare_equal and left.is_nan().any():
                     nan_info = " (nans_compare_equal=False)"
                     mismatch = True
                 elif (left.is_nan() != right.is_nan()).any():
                     nan_info = f" (nans_compare_equal={nans_compare_equal})"
                     mismatch = True
 
             if mismatch:
@@ -393,43 +398,53 @@
                     "Series",
                     f"Value mismatch{nan_info}",
                     left=list(left),
                     right=list(right),
                 )
 
 
-def _assert_series_nested_nans_equal(
+def _assert_series_nested(
     left: Series,
     right: Series,
     check_dtype: bool,
     check_exact: bool,
+    nans_compare_equal: bool,
     atol: float,
     rtol: float,
 ) -> bool:
     # check that float values exist at _some_ level of nesting
     if not any(tp in FLOAT_DTYPES for tp in unpack_dtypes(left.dtype, right.dtype)):
         return False
 
     # compare nested lists element-wise
     elif left.dtype == List == right.dtype:
         for s1, s2 in zip(left, right):
             if s1 is None and s2 is None:
-                continue
+                if nans_compare_equal:
+                    continue
+                else:
+                    raise_assert_detail(
+                        "Series",
+                        f"Nested value mismatch (nans_compare_equal={nans_compare_equal})",
+                        s1,
+                        s2,
+                    )
             elif (s1 is None and s2 is not None) or (s2 is None and s1 is not None):
                 raise_assert_detail("Series", "Nested value mismatch", s1, s2)
             elif len(s1) != len(s2):
                 raise_assert_detail(
                     "Series", "Nested list length mismatch", len(s1), len(s2)
                 )
+
             _assert_series_inner(
                 s1,
                 s2,
                 check_dtype=check_dtype,
                 check_exact=check_exact,
-                nans_compare_equal=True,
+                nans_compare_equal=nans_compare_equal,
                 atol=atol,
                 rtol=rtol,
             )
         return True
 
     # unnest structs as series and compare
     elif left.dtype == Struct == right.dtype:
@@ -447,15 +462,15 @@
             )
         for s1, s2 in zip(ls, rs):
             _assert_series_inner(
                 s1,
                 s2,
                 check_dtype=check_dtype,
                 check_exact=check_exact,
-                nans_compare_equal=True,
+                nans_compare_equal=nans_compare_equal,
                 atol=atol,
                 rtol=rtol,
             )
         return True
     else:
         # fall-back to outer codepath (if mismatched dtypes we would expect
         # the equality check to fail - unless ALL series values are null)
```

### Comparing `polars_lts_cpu-0.18.2/polars/testing/parametric/__init__.py` & `polars_lts_cpu-0.18.3/polars/testing/parametric/__init__.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/polars/testing/parametric/primitives.py` & `polars_lts_cpu-0.18.3/polars/testing/parametric/primitives.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/polars/testing/parametric/profiles.py` & `polars_lts_cpu-0.18.3/polars/testing/parametric/profiles.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/polars/testing/parametric/strategies.py` & `polars_lts_cpu-0.18.3/polars/testing/parametric/strategies.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/polars/type_aliases.py` & `polars_lts_cpu-0.18.3/polars/type_aliases.py`

 * *Files 4% similar despite different names*

```diff
@@ -79,14 +79,15 @@
 CategoricalOrdering: TypeAlias = Literal["physical", "lexical"]
 CsvEncoding: TypeAlias = Literal["utf8", "utf8-lossy"]
 FillNullStrategy: TypeAlias = Literal[
     "forward", "backward", "min", "max", "mean", "zero", "one"
 ]
 FloatFmt: TypeAlias = Literal["full", "mixed"]
 IpcCompression: TypeAlias = Literal["uncompressed", "lz4", "zstd"]
+JoinValidation: TypeAlias = Literal["m:m", "m:1", "1:m", "1:1"]
 NullBehavior: TypeAlias = Literal["ignore", "drop"]
 NullStrategy: TypeAlias = Literal["ignore", "propagate"]
 ParallelStrategy: TypeAlias = Literal["auto", "columns", "row_groups", "none"]
 ParquetCompression: TypeAlias = Literal[
     "lz4", "uncompressed", "snappy", "gzip", "lzo", "brotli", "zstd"
 ]
 PivotAgg: TypeAlias = Literal[
@@ -132,15 +133,17 @@
     "nearest", "higher", "lower", "midpoint", "linear"
 ]  # QuantileInterpolOptions
 ToStructStrategy: TypeAlias = Literal[
     "first_non_null", "max_width"
 ]  # ListToStructWidthStrategy
 
 # The following have no equivalent on the Rust side
-ConcatMethod = Literal["vertical", "diagonal", "horizontal", "align"]
+ConcatMethod = Literal[
+    "vertical", "vertical_relaxed", "diagonal", "horizontal", "align"
+]
 EpochTimeUnit = Literal["ns", "us", "ms", "s", "d"]
 Orientation: TypeAlias = Literal["col", "row"]
 SearchSortedSide: TypeAlias = Literal["any", "left", "right"]
 TransferEncoding: TypeAlias = Literal["hex", "base64"]
 CorrelationMethod: TypeAlias = Literal["pearson", "spearman"]
 DbReadEngine: TypeAlias = Literal["adbc", "connectorx"]
 DbWriteEngine: TypeAlias = Literal["sqlalchemy", "adbc"]
```

### Comparing `polars_lts_cpu-0.18.2/polars/utils/__init__.py` & `polars_lts_cpu-0.18.3/polars/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/polars/utils/_construction.py` & `polars_lts_cpu-0.18.3/polars/utils/_construction.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/polars/utils/_parse_expr_input.py` & `polars_lts_cpu-0.18.3/polars/utils/_parse_expr_input.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/polars/utils/_scan.py` & `polars_lts_cpu-0.18.3/polars/utils/_scan.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/polars/utils/_wrap.py` & `polars_lts_cpu-0.18.3/polars/utils/_wrap.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/polars/utils/build_info.py` & `polars_lts_cpu-0.18.3/polars/utils/build_info.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/polars/utils/convert.py` & `polars_lts_cpu-0.18.3/polars/utils/convert.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/polars/utils/decorators.py` & `polars_lts_cpu-0.18.3/polars/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/polars/utils/meta.py` & `polars_lts_cpu-0.18.3/polars/utils/meta.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/polars/utils/polars_version.py` & `polars_lts_cpu-0.18.3/polars/utils/polars_version.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/polars/utils/show_versions.py` & `polars_lts_cpu-0.18.3/polars/utils/show_versions.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/polars/utils/various.py` & `polars_lts_cpu-0.18.3/polars/utils/various.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/pyproject.toml` & `polars_lts_cpu-0.18.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -69,15 +69,15 @@
 ]
 
 [[tool.mypy.overrides]]
 module = [
   "IPython.*",
   "backports",
   "connectorx",
-  "deltalake",
+  "deltalake.*",
   "fsspec.*",
   "matplotlib.*",
   "polars.polars",
   "pyarrow.*",
   "pydantic",
   "sqlalchemy",
   "xlsx2csv",
```

### Comparing `polars_lts_cpu-0.18.2/requirements-dev.txt` & `polars_lts_cpu-0.18.3/requirements-dev.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # We're pinning our tooling, because it's an environment we can strictly control.
 # We're not pinning package dependencies, because our tests need to pass with the
 # latest version of the packages.
 
 --prefer-binary
 
 # Dependencies
-deltalake >= 0.8.0
+deltalake >= 0.10.0
 numpy
 pandas
 pyarrow
 pydantic
 backports.zoneinfo; python_version < '3.9'
 tzdata; platform_system == 'Windows'
 xlsx2csv
```

### Comparing `polars_lts_cpu-0.18.2/scripts/check_stacklevels.py` & `polars_lts_cpu-0.18.3/scripts/check_stacklevels.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/src/apply/dataframe.rs` & `polars_lts_cpu-0.18.3/src/apply/dataframe.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/src/apply/lazy.rs` & `polars_lts_cpu-0.18.3/src/apply/lazy.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/src/apply/mod.rs` & `polars_lts_cpu-0.18.3/src/apply/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/src/apply/series.rs` & `polars_lts_cpu-0.18.3/src/apply/series.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/src/arrow_interop/to_py.rs` & `polars_lts_cpu-0.18.3/src/arrow_interop/to_py.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/src/batched_csv.rs` & `polars_lts_cpu-0.18.3/src/batched_csv.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/src/conversion.rs` & `polars_lts_cpu-0.18.3/src/conversion.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/src/dataframe.rs` & `polars_lts_cpu-0.18.3/src/dataframe.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/src/datatypes.rs` & `polars_lts_cpu-0.18.3/src/datatypes.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/src/error.rs` & `polars_lts_cpu-0.18.3/src/error.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/src/expr/array.rs` & `polars_lts_cpu-0.18.3/src/expr/array.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/src/expr/binary.rs` & `polars_lts_cpu-0.18.3/src/expr/binary.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/src/expr/datetime.rs` & `polars_lts_cpu-0.18.3/src/expr/datetime.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/src/expr/general.rs` & `polars_lts_cpu-0.18.3/src/expr/general.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/src/expr/list.rs` & `polars_lts_cpu-0.18.3/src/expr/list.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/src/expr/meta.rs` & `polars_lts_cpu-0.18.3/src/expr/meta.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/src/expr/mod.rs` & `polars_lts_cpu-0.18.3/src/expr/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/src/expr/string.rs` & `polars_lts_cpu-0.18.3/src/expr/string.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/src/file.rs` & `polars_lts_cpu-0.18.3/src/file.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/src/functions/eager.rs` & `polars_lts_cpu-0.18.3/src/functions/eager.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/src/functions/io.rs` & `polars_lts_cpu-0.18.3/src/functions/io.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/src/functions/lazy.rs` & `polars_lts_cpu-0.18.3/src/functions/lazy.rs`

 * *Files 2% similar despite different names*

```diff
@@ -114,25 +114,38 @@
 
 #[pyfunction]
 pub fn cols(names: Vec<String>) -> PyExpr {
     dsl::cols(names).into()
 }
 
 #[pyfunction]
-pub fn concat_lf(seq: &PyAny, rechunk: bool, parallel: bool) -> PyResult<PyLazyFrame> {
+pub fn concat_lf(
+    seq: &PyAny,
+    rechunk: bool,
+    parallel: bool,
+    to_supertypes: bool,
+) -> PyResult<PyLazyFrame> {
     let len = seq.len()?;
     let mut lfs = Vec::with_capacity(len);
 
     for res in seq.iter()? {
         let item = res?;
         let lf = get_lf(item)?;
         lfs.push(lf);
     }
 
-    let lf = dsl::concat(lfs, rechunk, parallel).map_err(PyPolarsErr::from)?;
+    let lf = dsl::concat(
+        lfs,
+        UnionArgs {
+            rechunk,
+            parallel,
+            to_supertypes,
+        },
+    )
+    .map_err(PyPolarsErr::from)?;
     Ok(lf.into())
 }
 
 #[pyfunction]
 pub fn concat_list(s: Vec<PyExpr>) -> PyResult<PyExpr> {
     let s = s.into_iter().map(|e| e.inner).collect::<Vec<_>>();
     let expr = dsl::concat_list(s).map_err(PyPolarsErr::from)?;
```

### Comparing `polars_lts_cpu-0.18.2/src/functions/meta.rs` & `polars_lts_cpu-0.18.3/src/functions/meta.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/src/functions/whenthen.rs` & `polars_lts_cpu-0.18.3/src/functions/whenthen.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/src/lazyframe.rs` & `polars_lts_cpu-0.18.3/src/lazyframe.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/src/lazygroupby.rs` & `polars_lts_cpu-0.18.3/src/lazygroupby.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/src/lib.rs` & `polars_lts_cpu-0.18.3/src/lib.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/src/object.rs` & `polars_lts_cpu-0.18.3/src/object.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/src/series/aggregation.rs` & `polars_lts_cpu-0.18.3/src/series/aggregation.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/src/series/arithmetic.rs` & `polars_lts_cpu-0.18.3/src/series/arithmetic.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/src/series/comparison.rs` & `polars_lts_cpu-0.18.3/src/series/comparison.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/src/series/construction.rs` & `polars_lts_cpu-0.18.3/src/series/construction.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/src/series/export.rs` & `polars_lts_cpu-0.18.3/src/series/export.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/src/series/mod.rs` & `polars_lts_cpu-0.18.3/src/series/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/src/series/numpy_ufunc.rs` & `polars_lts_cpu-0.18.3/src/series/numpy_ufunc.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/src/series/set_at_idx.rs` & `polars_lts_cpu-0.18.3/src/series/set_at_idx.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/src/sql.rs` & `polars_lts_cpu-0.18.3/src/sql.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/src/utils.rs` & `polars_lts_cpu-0.18.3/src/utils.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/tests/README.md` & `polars_lts_cpu-0.18.3/tests/README.md`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/tests/benchmark/groupby-datagen.R` & `polars_lts_cpu-0.18.3/tests/benchmark/groupby-datagen.R`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/tests/benchmark/run_h2oai_benchmark.py` & `polars_lts_cpu-0.18.3/tests/benchmark/run_h2oai_benchmark.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/tests/benchmark/test_release.py` & `polars_lts_cpu-0.18.3/tests/benchmark/test_release.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/tests/docs/run_doctest.py` & `polars_lts_cpu-0.18.3/tests/docs/run_doctest.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/tests/parametric/test_dataframe.py` & `polars_lts_cpu-0.18.3/tests/parametric/test_dataframe.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/tests/parametric/test_lazyframe.py` & `polars_lts_cpu-0.18.3/tests/parametric/test_lazyframe.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/tests/parametric/test_series.py` & `polars_lts_cpu-0.18.3/tests/parametric/test_series.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/tests/parametric/test_testing.py` & `polars_lts_cpu-0.18.3/tests/parametric/test_testing.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/tests/unit/conftest.py` & `polars_lts_cpu-0.18.3/tests/unit/conftest.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/tests/unit/datatypes/test_array.py` & `polars_lts_cpu-0.18.3/tests/unit/datatypes/test_array.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/tests/unit/datatypes/test_binary.py` & `polars_lts_cpu-0.18.3/tests/unit/datatypes/test_binary.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/tests/unit/datatypes/test_bool.py` & `polars_lts_cpu-0.18.3/tests/unit/datatypes/test_bool.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/tests/unit/datatypes/test_categorical.py` & `polars_lts_cpu-0.18.3/tests/unit/datatypes/test_categorical.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/tests/unit/datatypes/test_decimal.py` & `polars_lts_cpu-0.18.3/tests/unit/datatypes/test_decimal.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/tests/unit/datatypes/test_duration.py` & `polars_lts_cpu-0.18.3/tests/unit/datatypes/test_duration.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/tests/unit/datatypes/test_list.py` & `polars_lts_cpu-0.18.3/tests/unit/datatypes/test_list.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/tests/unit/datatypes/test_object.py` & `polars_lts_cpu-0.18.3/tests/unit/datatypes/test_object.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/tests/unit/datatypes/test_struct.py` & `polars_lts_cpu-0.18.3/tests/unit/datatypes/test_struct.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/tests/unit/datatypes/test_temporal.py` & `polars_lts_cpu-0.18.3/tests/unit/datatypes/test_temporal.py`

 * *Files 0% similar despite different names*

```diff
@@ -897,15 +897,17 @@
 def test_groupby_dynamic_crossing_dst(rule: str, offset: timedelta) -> None:
     start_dt = datetime(2021, 11, 7)
     end_dt = start_dt + offset
     date_range = pl.date_range(
         start_dt, end_dt, rule, time_zone="US/Central", eager=True
     )
     df = pl.DataFrame({"time": date_range, "value": range(len(date_range))})
-    result = df.groupby_dynamic("time", every=rule).agg(pl.col("value").mean())
+    result = df.groupby_dynamic("time", every=rule, start_by="datapoint").agg(
+        pl.col("value").mean()
+    )
     expected = pl.DataFrame(
         {"time": date_range, "value": range(len(date_range))},
         schema_overrides={"value": pl.Float64},
     )
     assert_frame_equal(result, expected)
 
 
@@ -1022,14 +1024,22 @@
     expected = pl.DataFrame(
         {"time": date_range, "value": range(len(date_range))},
         schema_overrides={"value": pl.Float64},
     )
     assert_frame_equal(result, expected)
 
 
+def test_groupby_dynamic_2d_9333() -> None:
+    df = pl.DataFrame({"ts": [datetime(2000, 1, 1, 3)], "values": [10.0]})
+    df = df.with_columns(pl.col("ts").set_sorted())
+    result = df.groupby_dynamic("ts", every="2d").agg(pl.col("values"))
+    expected = pl.DataFrame({"ts": [datetime(1999, 12, 31, 0)], "values": [[10.0]]})
+    assert_frame_equal(result, expected)
+
+
 def test_asof_join_tolerance_grouper() -> None:
     from datetime import date
 
     df1 = pl.DataFrame({"date": [date(2020, 1, 5), date(2020, 1, 10)], "by": [1, 1]})
     df2 = pl.DataFrame(
         {
             "date": [date(2020, 1, 5), date(2020, 1, 6)],
```

### Comparing `polars_lts_cpu-0.18.2/tests/unit/functions/test_as_datatype.py` & `polars_lts_cpu-0.18.3/tests/unit/functions/test_as_datatype.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/tests/unit/functions/test_functions.py` & `polars_lts_cpu-0.18.3/tests/unit/functions/test_functions.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/tests/unit/functions/test_range.py` & `polars_lts_cpu-0.18.3/tests/unit/functions/test_range.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/tests/unit/functions/test_repeat.py` & `polars_lts_cpu-0.18.3/tests/unit/functions/test_repeat.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/tests/unit/io/files/delta-table/_delta_log/00000000000000000000.json` & `polars_lts_cpu-0.18.3/tests/unit/io/files/delta-table/_delta_log/00000000000000000000.json`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/tests/unit/io/files/delta-table/_delta_log/00000000000000000001.json` & `polars_lts_cpu-0.18.3/tests/unit/io/files/delta-table/_delta_log/00000000000000000001.json`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/tests/unit/io/files/delta-table/part-00000-e42312d7-60e5-454d-acbc-db192d220e73-c000.snappy.parquet` & `polars_lts_cpu-0.18.3/tests/unit/io/files/delta-table/part-00000-e42312d7-60e5-454d-acbc-db192d220e73-c000.snappy.parquet`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/tests/unit/io/files/delta-table/part-00000-e4a999da-df45-4fb0-bdc4-d999fc0f58aa-c000.snappy.parquet` & `polars_lts_cpu-0.18.3/tests/unit/io/files/delta-table/part-00000-e4a999da-df45-4fb0-bdc4-d999fc0f58aa-c000.snappy.parquet`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/tests/unit/io/files/example.xlsx` & `polars_lts_cpu-0.18.3/tests/unit/io/files/example.xlsx`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/tests/unit/io/files/foods1.ipc` & `polars_lts_cpu-0.18.3/tests/unit/io/files/foods1.ipc`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/tests/unit/io/files/foods1.ndjson` & `polars_lts_cpu-0.18.3/tests/unit/io/files/foods1.ndjson`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/tests/unit/io/files/foods1.parquet` & `polars_lts_cpu-0.18.3/tests/unit/io/files/foods1.parquet`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/tests/unit/io/files/foods2.ipc` & `polars_lts_cpu-0.18.3/tests/unit/io/files/foods2.ipc`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/tests/unit/io/files/foods2.ndjson` & `polars_lts_cpu-0.18.3/tests/unit/io/files/foods2.ndjson`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/tests/unit/io/files/foods2.parquet` & `polars_lts_cpu-0.18.3/tests/unit/io/files/foods2.parquet`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/tests/unit/io/files/small.parquet` & `polars_lts_cpu-0.18.3/tests/unit/io/files/small.parquet`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/tests/unit/io/test_avro.py` & `polars_lts_cpu-0.18.3/tests/unit/io/test_avro.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/tests/unit/io/test_csv.py` & `polars_lts_cpu-0.18.3/tests/unit/io/test_csv.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/tests/unit/io/test_database.py` & `polars_lts_cpu-0.18.3/tests/unit/io/test_database.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/tests/unit/io/test_delta.py` & `polars_lts_cpu-0.18.3/tests/unit/io/test_delta.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/tests/unit/io/test_excel.py` & `polars_lts_cpu-0.18.3/tests/unit/io/test_excel.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/tests/unit/io/test_ipc.py` & `polars_lts_cpu-0.18.3/tests/unit/io/test_ipc.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/tests/unit/io/test_json.py` & `polars_lts_cpu-0.18.3/tests/unit/io/test_json.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/tests/unit/io/test_lazy_csv.py` & `polars_lts_cpu-0.18.3/tests/unit/io/test_lazy_csv.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/tests/unit/io/test_lazy_ipc.py` & `polars_lts_cpu-0.18.3/tests/unit/io/test_lazy_ipc.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/tests/unit/io/test_lazy_json.py` & `polars_lts_cpu-0.18.3/tests/unit/io/test_lazy_json.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/tests/unit/io/test_lazy_parquet.py` & `polars_lts_cpu-0.18.3/tests/unit/io/test_lazy_parquet.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/tests/unit/io/test_other.py` & `polars_lts_cpu-0.18.3/tests/unit/io/test_other.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/tests/unit/io/test_parquet.py` & `polars_lts_cpu-0.18.3/tests/unit/io/test_parquet.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,19 @@
 import pandas as pd
 import pyarrow as pa
 import pyarrow.dataset as ds
 import pyarrow.parquet as pq
 import pytest
 
 import polars as pl
-from polars.testing import assert_frame_equal, assert_frame_equal_local_categoricals
+from polars.testing import (
+    assert_frame_equal,
+    assert_frame_equal_local_categoricals,
+    assert_series_equal,
+)
 
 if TYPE_CHECKING:
     from pathlib import Path
 
     from polars.type_aliases import ParquetCompression
 
 
@@ -477,7 +481,22 @@
     df = pd.DataFrame({"listcol": [[] * 10]})
     f = io.BytesIO()
     df.to_parquet(f)
     f.seek(0)
     df = pl.read_parquet(f)
     assert df.dtypes == [pl.List(pl.Null)]
     assert df.to_dict(False) == {"listcol": [[]]}
+
+
+def test_parquet_string_cache() -> None:
+    f = io.BytesIO()
+
+    df = pl.DataFrame({"a": ["a", "b", "c", "d"]}).with_columns(
+        pl.col("a").cast(pl.Categorical)
+    )
+
+    df.write_parquet(f, row_group_size=2)
+
+    # this file has 2 row groups and a categorical column
+    # so polars should automatically set string cache
+    f.seek(0)
+    assert_series_equal(pl.read_parquet(f)["a"].cast(str), df["a"].cast(str))
```

### Comparing `polars_lts_cpu-0.18.2/tests/unit/io/test_pickle.py` & `polars_lts_cpu-0.18.3/tests/unit/io/test_pickle.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/tests/unit/io/test_pyarrow_dataset.py` & `polars_lts_cpu-0.18.3/tests/unit/io/test_pyarrow_dataset.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/tests/unit/namespaces/test_array.py` & `polars_lts_cpu-0.18.3/tests/unit/namespaces/test_array.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/tests/unit/namespaces/test_binary.py` & `polars_lts_cpu-0.18.3/tests/unit/namespaces/test_binary.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/tests/unit/namespaces/test_categorical.py` & `polars_lts_cpu-0.18.3/tests/unit/namespaces/test_categorical.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/tests/unit/namespaces/test_datetime.py` & `polars_lts_cpu-0.18.3/tests/unit/namespaces/test_datetime.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/tests/unit/namespaces/test_list.py` & `polars_lts_cpu-0.18.3/tests/unit/namespaces/test_list.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/tests/unit/namespaces/test_meta.py` & `polars_lts_cpu-0.18.3/tests/unit/namespaces/test_meta.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/tests/unit/namespaces/test_string.py` & `polars_lts_cpu-0.18.3/tests/unit/namespaces/test_string.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/tests/unit/namespaces/test_strptime.py` & `polars_lts_cpu-0.18.3/tests/unit/namespaces/test_strptime.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/tests/unit/namespaces/test_struct.py` & `polars_lts_cpu-0.18.3/tests/unit/namespaces/test_struct.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/tests/unit/operations/test_aggregations.py` & `polars_lts_cpu-0.18.3/tests/unit/operations/test_aggregations.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/tests/unit/operations/test_apply.py` & `polars_lts_cpu-0.18.3/tests/unit/operations/test_apply.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/tests/unit/operations/test_arithmetic.py` & `polars_lts_cpu-0.18.3/tests/unit/operations/test_arithmetic.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/tests/unit/operations/test_comparison.py` & `polars_lts_cpu-0.18.3/tests/unit/operations/test_comparison.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/tests/unit/operations/test_drop.py` & `polars_lts_cpu-0.18.3/tests/unit/operations/test_drop.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/tests/unit/operations/test_explode.py` & `polars_lts_cpu-0.18.3/tests/unit/operations/test_explode.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/tests/unit/operations/test_filter.py` & `polars_lts_cpu-0.18.3/tests/unit/operations/test_filter.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/tests/unit/operations/test_folds.py` & `polars_lts_cpu-0.18.3/tests/unit/operations/test_folds.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/tests/unit/operations/test_groupby.py` & `polars_lts_cpu-0.18.3/tests/unit/operations/test_groupby.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/tests/unit/operations/test_groupby_rolling.py` & `polars_lts_cpu-0.18.3/tests/unit/operations/test_groupby_rolling.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/tests/unit/operations/test_is_in.py` & `polars_lts_cpu-0.18.3/tests/unit/operations/test_is_in.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     s1 = df1.select(pl.struct(["x", "y"])).to_series()
     s2 = df2.select(pl.struct(["x", "y"])).to_series()
 
     assert s1.is_in(s2).to_list() == [False, False, True, True, True, True, True]
 
 
 def test_is_in_bool() -> None:
-    bool_value_to_filter_on = [True, None]
+    bool_value_to_filter_on = {True, None}
     df = pl.DataFrame({"A": [True, False, None]})
     assert df.filter(pl.col("A").is_in(bool_value_to_filter_on)).to_dict(False) == {
         "A": [True, False]
     }
 
 
 def test_is_in_empty_list_4559() -> None:
```

### Comparing `polars_lts_cpu-0.18.2/tests/unit/operations/test_join.py` & `polars_lts_cpu-0.18.3/tests/unit/operations/test_join.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/tests/unit/operations/test_join_asof.py` & `polars_lts_cpu-0.18.3/tests/unit/operations/test_join_asof.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from datetime import date, datetime
 from typing import Any
 
 import numpy as np
+import pytest
 
 import polars as pl
 from polars.testing import assert_frame_equal
 
 
 def test_asof_join_inline_cast_6438() -> None:
     df_trades = pl.DataFrame(
@@ -482,7 +483,16 @@
             "a": [1, 2, 3, 2, 5],
             "b": [1, 1, 2, 3, 4],
         }
     ).sort(by=["group", "asof_key"])
 
     out = df1.join_asof(df2, on="asof_key", by="group", strategy="nearest")
     assert_frame_equal(out, expected)
+
+
+def test_asof_join_string_err() -> None:
+    left = pl.DataFrame({"date_str": ["2023/02/15"]}).sort("date_str")
+    right = pl.DataFrame(
+        {"date_str": ["2023/01/31", "2023/02/28"], "value": [0, 1]}
+    ).sort("date_str")
+    with pytest.raises(pl.InvalidOperationError):
+        left.join_asof(right, on="date_str")
```

### Comparing `polars_lts_cpu-0.18.2/tests/unit/operations/test_melt.py` & `polars_lts_cpu-0.18.3/tests/unit/operations/test_melt.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/tests/unit/operations/test_pivot.py` & `polars_lts_cpu-0.18.3/tests/unit/operations/test_pivot.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/tests/unit/operations/test_rolling.py` & `polars_lts_cpu-0.18.3/tests/unit/operations/test_rolling.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/tests/unit/operations/test_select.py` & `polars_lts_cpu-0.18.3/tests/unit/operations/test_select.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/tests/unit/operations/test_sort.py` & `polars_lts_cpu-0.18.3/tests/unit/operations/test_sort.py`

 * *Files 4% similar despite different names*

```diff
@@ -694,7 +694,13 @@
             df.groupby_dynamic(pl.col("ts").set_sorted(), every="1d").agg(
                 pl.col("val").sum()
             )
         )
         .to_series()
         .flags["SORTED_ASC"]
     )
+
+
+def test_top_k_9385() -> None:
+    assert pl.LazyFrame({"b": [True, False]}).sort(["b"]).slice(0, 1).collect()[
+        "b"
+    ].to_list() == [False]
```

### Comparing `polars_lts_cpu-0.18.2/tests/unit/operations/test_statistics.py` & `polars_lts_cpu-0.18.3/tests/unit/operations/test_statistics.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/tests/unit/operations/test_transpose.py` & `polars_lts_cpu-0.18.3/tests/unit/operations/test_transpose.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/tests/unit/operations/test_unique.py` & `polars_lts_cpu-0.18.3/tests/unit/operations/test_unique.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/tests/unit/operations/test_window.py` & `polars_lts_cpu-0.18.3/tests/unit/operations/test_window.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/tests/unit/operations/test_with_columns.py` & `polars_lts_cpu-0.18.3/tests/unit/operations/test_with_columns.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/tests/unit/streaming/test_ooc.py` & `polars_lts_cpu-0.18.3/tests/unit/streaming/test_ooc.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/tests/unit/streaming/test_streaming.py` & `polars_lts_cpu-0.18.3/tests/unit/streaming/test_streaming.py`

 * *Files 5% similar despite different names*

```diff
@@ -327,14 +327,26 @@
             streaming=True
         )
     )
     (_, err) = capfd.readouterr()
     assert "df -> projection -> ordered_sink" in err
 
 
+def test_streaming_ternary() -> None:
+    q = pl.LazyFrame({"a": [1, 2, 3]})
+
+    assert (
+        q.with_columns(
+            pl.when(pl.col("a") >= 2).then(pl.col("a")).otherwise(None).alias("b"),
+        )
+        .explain(streaming=True)
+        .startswith("--- PIPELINE")
+    )
+
+
 def test_streaming_unique(monkeypatch: Any, capfd: Any) -> None:
     monkeypatch.setenv("POLARS_VERBOSE", "1")
     df = pl.DataFrame({"a": [1, 2, 2, 2], "b": [3, 4, 4, 4], "c": [5, 6, 7, 7]})
     q = df.lazy().unique(subset=["a", "c"], maintain_order=False).sort(["a", "b", "c"])
     assert_frame_equal(q.collect(streaming=True), q.collect(streaming=False))
 
     q = df.lazy().unique(subset=["b", "c"], maintain_order=False).sort(["a", "b", "c"])
@@ -496,7 +508,25 @@
             date(2023, 5, 2),
             date(2023, 5, 3),
             date(2023, 5, 4),
             date(2023, 5, 5),
         ],
         "sum": ["a", "a", "b", "b", "c", "c", None, None],
     }
+
+
+def test_streaming_restart_non_streamable_groupby() -> None:
+    df = pl.DataFrame({"id": [1], "id2": [1], "id3": [1], "value": [1]})
+    res = (
+        df.lazy()
+        .join(df.lazy(), on=["id", "id2"], how="left")
+        .filter(
+            (pl.col("id3") > pl.col("id3_right"))
+            & (pl.col("id3") - pl.col("id3_right") < 30)
+        )
+        .groupby(["id2", "id3", "id3_right"])
+        .agg(
+            pl.col("value").apply(lambda x: x).sum() * pl.col("value").sum()
+        )  # non-streamable UDF + nested_agg
+    )
+
+    assert """--- PIPELINE""" in res.explain(streaming=True)
```

### Comparing `polars_lts_cpu-0.18.2/tests/unit/test_api.py` & `polars_lts_cpu-0.18.3/tests/unit/test_api.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/tests/unit/test_cfg.py` & `polars_lts_cpu-0.18.3/tests/unit/test_cfg.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 from __future__ import annotations
 
 import os
-from typing import Iterator
+from typing import TYPE_CHECKING, Iterator
 
 import pytest
 
 import polars as pl
 from polars.config import _get_float_fmt
 from polars.testing import assert_frame_equal
 
+if TYPE_CHECKING:
+    from pathlib import Path
+
 
 @pytest.fixture(autouse=True)
 def _environ() -> Iterator[None]:
     """Fixture to restore the environment after/during tests."""
     with pl.StringCache(), pl.Config(restore_defaults=True):
         yield
 
@@ -491,47 +494,51 @@
 
     expected = pl.DataFrame(
         {"a": ["foo"], "b": [1], "c": [3]}, schema_overrides={"a": pl.Categorical}
     )
     assert_frame_equal(out, expected)
 
 
-def test_config_load_save() -> None:
-    # set some config options...
-    pl.Config.set_tbl_cols(12)
-    pl.Config.set_verbose(True)
-    pl.Config.set_fmt_float("full")
-    assert os.environ.get("POLARS_VERBOSE") == "1"
-
-    cfg = pl.Config.save()
-    assert isinstance(cfg, str)
-    assert "POLARS_VERBOSE" in pl.Config.state(if_set=True)
-
-    # ...modify the same options...
-    pl.Config.set_tbl_cols(10)
-    pl.Config.set_verbose(False)
-    assert os.environ.get("POLARS_VERBOSE") == "0"
-
-    # ...load back from config...
-    pl.Config.load(cfg)
-
-    # ...and confirm the saved options were set.
-    assert os.environ.get("POLARS_FMT_MAX_COLS") == "12"
-    assert os.environ.get("POLARS_VERBOSE") == "1"
-    assert _get_float_fmt() == "full"
-
-    # restore all default options (unsets from env)
-    pl.Config.restore_defaults()
-    for e in ("POLARS_FMT_MAX_COLS", "POLARS_VERBOSE"):
-        assert e not in pl.Config.state(if_set=True)
-        assert e in pl.Config.state()
-
-    assert os.environ.get("POLARS_FMT_MAX_COLS") is None
-    assert os.environ.get("POLARS_VERBOSE") is None
-    assert _get_float_fmt() == "mixed"
+@pytest.mark.write_disk()
+def test_config_load_save(tmp_path: Path) -> None:
+    for file in (None, tmp_path / "polars.config"):
+        # set some config options...
+        pl.Config.set_tbl_cols(12)
+        pl.Config.set_verbose(True)
+        pl.Config.set_fmt_float("full")
+        assert os.environ.get("POLARS_VERBOSE") == "1"
+
+        cfg = pl.Config.save(file)
+        assert isinstance(cfg, str)
+        assert "POLARS_VERBOSE" in pl.Config.state(if_set=True)
+
+        # ...modify the same options...
+        pl.Config.set_tbl_cols(10)
+        pl.Config.set_verbose(False)
+        assert os.environ.get("POLARS_VERBOSE") == "0"
+
+        # ...load back from config...
+        if file is not None:
+            assert os.path.isfile(cfg)
+        pl.Config.load(cfg)
+
+        # ...and confirm the saved options were set.
+        assert os.environ.get("POLARS_FMT_MAX_COLS") == "12"
+        assert os.environ.get("POLARS_VERBOSE") == "1"
+        assert _get_float_fmt() == "full"
+
+        # restore all default options (unsets from env)
+        pl.Config.restore_defaults()
+        for e in ("POLARS_FMT_MAX_COLS", "POLARS_VERBOSE"):
+            assert e not in pl.Config.state(if_set=True)
+            assert e in pl.Config.state()
+
+        assert os.environ.get("POLARS_FMT_MAX_COLS") is None
+        assert os.environ.get("POLARS_VERBOSE") is None
+        assert _get_float_fmt() == "mixed"
 
 
 def test_config_scope() -> None:
     pl.Config.set_verbose(False)
     pl.Config.set_tbl_cols(8)
 
     initial_state = pl.Config.state()
```

### Comparing `polars_lts_cpu-0.18.2/tests/unit/test_constructors.py` & `polars_lts_cpu-0.18.3/tests/unit/test_constructors.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/tests/unit/test_cse.py` & `polars_lts_cpu-0.18.3/tests/unit/test_cse.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/tests/unit/test_datatypes.py` & `polars_lts_cpu-0.18.3/tests/unit/test_datatypes.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/tests/unit/test_df.py` & `polars_lts_cpu-0.18.3/tests/unit/test_df.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/tests/unit/test_empty.py` & `polars_lts_cpu-0.18.3/tests/unit/test_empty.py`

 * *Files 4% similar despite different names*

```diff
@@ -66,7 +66,15 @@
     out = (
         pl.DataFrame({"id": [], "value": []})
         .groupby("id")
         .agg(pl.col("value").pow(2).mean())
     )
     assert out.shape == (0, 2)
     assert out.dtypes == [pl.Float32, pl.Float32]
+
+
+def test_empty_groupby_apply_err() -> None:
+    df = pl.DataFrame(schema={"x": pl.Int64})
+    with pytest.raises(
+        pl.ComputeError, match=r"cannot groupby \+ apply on empty 'DataFrame'"
+    ):
+        df.groupby("x").apply(lambda x: x)
```

### Comparing `polars_lts_cpu-0.18.2/tests/unit/test_errors.py` & `polars_lts_cpu-0.18.3/tests/unit/test_errors.py`

 * *Files 0% similar despite different names*

```diff
@@ -294,15 +294,15 @@
             "foo": [3, 4],
             "ham": ["c", "d"],
             "bar": [8, 9],
         }
     )
     with pytest.raises(
         ValueError,
-        match="'LazyFrame' only allows {'vertical','diagonal','align'} concat strategies.",
+        match="'LazyFrame' only allows {'vertical','vertical_relaxed','diagonal','align'} concat strategies.",
     ):
         pl.concat([df1.lazy(), df2.lazy()], how="horizontal").collect()
 
 
 @typing.no_type_check
 def test_series_concat_err() -> None:
     s = pl.Series([1, 2, 3])
```

### Comparing `polars_lts_cpu-0.18.2/tests/unit/test_expr_multi_cols.py` & `polars_lts_cpu-0.18.3/tests/unit/test_expr_multi_cols.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/tests/unit/test_exprs.py` & `polars_lts_cpu-0.18.3/tests/unit/test_exprs.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/tests/unit/test_fmt.py` & `polars_lts_cpu-0.18.3/tests/unit/test_fmt.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/tests/unit/test_interchange.py` & `polars_lts_cpu-0.18.3/tests/unit/test_interchange.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/tests/unit/test_interop.py` & `polars_lts_cpu-0.18.3/tests/unit/test_interop.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/tests/unit/test_lazy.py` & `polars_lts_cpu-0.18.3/tests/unit/test_lazy.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/tests/unit/test_polars_import.py` & `polars_lts_cpu-0.18.3/tests/unit/test_polars_import.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/tests/unit/test_predicates.py` & `polars_lts_cpu-0.18.3/tests/unit/test_predicates.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/tests/unit/test_projections.py` & `polars_lts_cpu-0.18.3/tests/unit/test_projections.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/tests/unit/test_queries.py` & `polars_lts_cpu-0.18.3/tests/unit/test_queries.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/tests/unit/test_rows.py` & `polars_lts_cpu-0.18.3/tests/unit/test_rows.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/tests/unit/test_schema.py` & `polars_lts_cpu-0.18.3/tests/unit/test_schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -455,7 +455,32 @@
     assert pl.DataFrame(schema={"a": pl.List}).dtypes[0] == expected
 
 
 def test_schema_ne_missing_9256() -> None:
     df = pl.DataFrame({"a": [0, 1, None], "b": [True, False, True]})
 
     assert df.select(pl.col("a").ne_missing(0).or_(pl.col("b")))["a"].all()
+
+
+def test_concat_vertically_relaxed() -> None:
+    a = pl.DataFrame(
+        {
+            "a": [1, 2, 3],
+            "b": [True, False, None],
+        },
+        schema={"a": pl.Int8, "b": pl.Boolean},
+    )
+
+    b = pl.DataFrame(
+        {
+            "a": [43, 2, 3],
+            "b": [32, 1, None],
+        },
+        schema={"a": pl.Int16, "b": pl.Int64},
+    )
+
+    out = pl.concat([a, b], how="vertical_relaxed")
+    assert out.schema == {"a": pl.Int16, "b": pl.Int64}
+    assert out.to_dict(False) == {
+        "a": [1, 2, 3, 43, 2, 3],
+        "b": [1, 0, None, 32, 1, None],
+    }
```

### Comparing `polars_lts_cpu-0.18.2/tests/unit/test_selectors.py` & `polars_lts_cpu-0.18.3/tests/unit/test_selectors.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/tests/unit/test_serde.py` & `polars_lts_cpu-0.18.3/tests/unit/test_serde.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/tests/unit/test_series.py` & `polars_lts_cpu-0.18.3/tests/unit/test_series.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/tests/unit/test_single.py` & `polars_lts_cpu-0.18.3/tests/unit/test_single.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/tests/unit/utils/test_parse_expr_input.py` & `polars_lts_cpu-0.18.3/tests/unit/utils/test_parse_expr_input.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/tests/unit/utils/test_utils.py` & `polars_lts_cpu-0.18.3/tests/unit/utils/test_utils.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.2/Cargo.lock` & `polars_lts_cpu-0.18.3/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -89,15 +89,15 @@
  "planus",
  "serde",
 ]
 
 [[package]]
 name = "arrow2"
 version = "0.17.1"
-source = "git+https://github.com/jorgecarleitao/arrow2?rev=fb5e4d591c7149df590a330365fae55d2370962f#fb5e4d591c7149df590a330365fae55d2370962f"
+source = "git+https://github.com/jorgecarleitao/arrow2?rev=2d2e7053f9a50810bfe9cecff25ab39089aef98e#2d2e7053f9a50810bfe9cecff25ab39089aef98e"
 dependencies = [
  "ahash",
  "arrow-format",
  "avro-schema",
  "base64",
  "bytemuck",
  "chrono",
@@ -1678,15 +1678,15 @@
 checksum = "6aeca18b86b413c660b781aa319e4e2648a3e6f9eadc9b47e9038e6fe9f3451b"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "py-polars"
-version = "0.18.2"
+version = "0.18.3"
 dependencies = [
  "ahash",
  "built",
  "ciborium",
  "jemallocator",
  "lexical-core",
  "libc",
```

### Comparing `polars_lts_cpu-0.18.2/PKG-INFO` & `polars_lts_cpu-0.18.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polars-lts-cpu
-Version: 0.18.2
+Version: 0.18.3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: polars-lts-cpu Version: 0.18.2 Classifier:
+Metadata-Version: 2.1 Name: polars-lts-cpu Version: 0.18.3 Classifier:
 Development Status :: 5 - Production/Stable Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3 :: Only Classifier:
 Programming Language :: Python :: 3.7 Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
```

