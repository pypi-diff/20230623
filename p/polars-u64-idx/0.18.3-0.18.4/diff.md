# Comparing `tmp/polars_u64_idx-0.18.3.tar.gz` & `tmp/polars_u64_idx-0.18.4.tar.gz`

## Comparing `polars_u64_idx-0.18.3.tar` & `polars_u64_idx-0.18.4.tar`

### file list

```diff
@@ -1,1241 +1,1246 @@
--rw-r--r--   0        0        0     4397 1970-01-01 00:00:00.000000 polars_u64_idx-0.18.3/local_dependencies/polars-io/Cargo.toml
--rw-r--r--   0     1001      123     1055 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-io/LICENSE
--rw-r--r--   0     1001      123      138 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-io/README.md
--rw-r--r--   0     1001      123     2383 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-io/src/avro/mod.rs
--rw-r--r--   0     1001      123     3608 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-io/src/avro/read.rs
--rw-r--r--   0     1001      123     2622 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-io/src/avro/write.rs
--rw-r--r--   0     1001      123     4505 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-io/src/cloud/adaptors.rs
--rw-r--r--   0     1001      123     9506 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-io/src/cloud/glob.rs
--rw-r--r--   0     1001      123     3089 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-io/src/cloud/mod.rs
--rw-r--r--   0     1001      123    28133 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-io/src/csv/buffer.rs
--rw-r--r--   0     1001      123     1815 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-io/src/csv/mod.rs
--rw-r--r--   0     1001      123    19446 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-io/src/csv/parser.rs
--rw-r--r--   0     1001      123    22226 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-io/src/csv/read.rs
--rw-r--r--   0     1001      123    10846 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-io/src/csv/read_impl/batched_mmap.rs
--rw-r--r--   0     1001      123    13938 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-io/src/csv/read_impl/batched_read.rs
--rw-r--r--   0     1001      123    30724 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-io/src/csv/read_impl/mod.rs
--rw-r--r--   0     1001      123    11466 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-io/src/csv/splitfields.rs
--rw-r--r--   0     1001      123    24531 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-io/src/csv/utils.rs
--rw-r--r--   0     1001      123     2796 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-io/src/csv/write.rs
--rw-r--r--   0     1001      123    14759 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-io/src/csv/write_impl.rs
--rw-r--r--   0     1001      123      184 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-io/src/export.rs
--rw-r--r--   0     1001      123     7586 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-io/src/ipc/ipc_file.rs
--rw-r--r--   0     1001      123     9227 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-io/src/ipc/ipc_stream.rs
--rw-r--r--   0     1001      123     3253 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-io/src/ipc/mmap.rs
--rw-r--r--   0     1001      123      401 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-io/src/ipc/mod.rs
--rw-r--r--   0     1001      123     8287 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-io/src/ipc/write.rs
--rw-r--r--   0     1001      123     1471 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-io/src/ipc/write_async.rs
--rw-r--r--   0     1001      123    11044 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-io/src/json/mod.rs
--rw-r--r--   0     1001      123     4771 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-io/src/lib.rs
--rw-r--r--   0     1001      123     1969 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-io/src/mmap.rs
--rw-r--r--   0     1001      123     7155 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-io/src/ndjson/buffer.rs
--rw-r--r--   0     1001      123    11979 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-io/src/ndjson/core.rs
--rw-r--r--   0     1001      123       37 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-io/src/ndjson/mod.rs
--rw-r--r--   0     1001      123      273 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-io/src/options.rs
--rw-r--r--   0     1001      123     7360 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-io/src/parquet/async_impl.rs
--rw-r--r--   0     1001      123     3093 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-io/src/parquet/mmap.rs
--rw-r--r--   0     1001      123     3132 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-io/src/parquet/mod.rs
--rw-r--r--   0     1001      123     4784 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-io/src/parquet/predicates.rs
--rw-r--r--   0     1001      123     9623 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-io/src/parquet/read.rs
--rw-r--r--   0     1001      123    17320 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-io/src/parquet/read_impl.rs
--rw-r--r--   0     1001      123    10052 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-io/src/parquet/write.rs
--rw-r--r--   0     1001      123     5334 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-io/src/partition.rs
--rw-r--r--   0     1001      123     1455 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-io/src/predicates.rs
--rw-r--r--   0     1001      123      621 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-io/src/prelude.rs
--rw-r--r--   0     1001      123      417 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-io/src/tests.rs
--rw-r--r--   0     1001      123     4374 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-io/src/utils.rs
--rw-r--r--   0        0        0      894 1970-01-01 00:00:00.000000 polars_u64_idx-0.18.3/local_dependencies/polars-error/Cargo.toml
--rw-r--r--   0     1001      123     1055 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-error/LICENSE
--rw-r--r--   0     1001      123      145 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-error/README.md
--rw-r--r--   0     1001      123     6584 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-error/src/lib.rs
--rw-r--r--   0        0        0     5152 1970-01-01 00:00:00.000000 polars_u64_idx-0.18.3/local_dependencies/polars-plan/Cargo.toml
--rw-r--r--   0     1001      123     1055 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-plan/LICENSE
--rw-r--r--   0     1001      123       45 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/constants.rs
--rw-r--r--   0     1001      123    17253 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/dot.rs
--rw-r--r--   0     1001      123     4171 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/dsl/arithmetic.rs
--rw-r--r--   0     1001      123     3992 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/dsl/arity.rs
--rw-r--r--   0     1001      123     1278 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/dsl/array.rs
--rw-r--r--   0     1001      123      935 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/dsl/binary.rs
--rw-r--r--   0     1001      123      650 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/dsl/cat.rs
--rw-r--r--   0     1001      123    10228 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/dsl/dt.rs
--rw-r--r--   0     1001      123     9538 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/dsl/expr.rs
--rw-r--r--   0     1001      123     6441 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/dsl/expr_dyn_fn.rs
--rw-r--r--   0     1001      123      753 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/dsl/from.rs
--rw-r--r--   0     1001      123       85 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/dsl/function_expr/abs.rs
--rw-r--r--   0     1001      123     1431 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/dsl/function_expr/arg_where.rs
--rw-r--r--   0     1001      123     1074 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/dsl/function_expr/array.rs
--rw-r--r--   0     1001      123     1327 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/dsl/function_expr/binary.rs
--rw-r--r--   0     1001      123     4221 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/dsl/function_expr/boolean.rs
--rw-r--r--   0     1001      123     1910 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/dsl/function_expr/bounds.rs
--rw-r--r--   0     1001      123     1216 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/dsl/function_expr/cat.rs
--rw-r--r--   0     1001      123      344 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/dsl/function_expr/clip.rs
--rw-r--r--   0     1001      123      257 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/dsl/function_expr/concat.rs
--rw-r--r--   0     1001      123     6261 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/dsl/function_expr/correlation.rs
--rw-r--r--   0     1001      123     1593 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/dsl/function_expr/cum.rs
--rw-r--r--   0     1001      123     9597 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/dsl/function_expr/datetime.rs
--rw-r--r--   0     1001      123      782 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/dsl/function_expr/dispatch.rs
--rw-r--r--   0     1001      123     2567 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/dsl/function_expr/fill_null.rs
--rw-r--r--   0     1001      123      992 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/dsl/function_expr/fused.rs
--rw-r--r--   0     1001      123     8119 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/dsl/function_expr/list.rs
--rw-r--r--   0     1001      123      581 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/dsl/function_expr/log.rs
--rw-r--r--   0     1001      123    21146 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/dsl/function_expr/mod.rs
--rw-r--r--   0     1001      123      462 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/dsl/function_expr/nan.rs
--rw-r--r--   0     1001      123     3132 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/dsl/function_expr/pow.rs
--rw-r--r--   0     1001      123      152 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/dsl/function_expr/rolling.rs
--rw-r--r--   0     1001      123      260 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/dsl/function_expr/round.rs
--rw-r--r--   0     1001      123      200 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/dsl/function_expr/row_hash.rs
--rw-r--r--   0     1001      123    14453 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/dsl/function_expr/schema.rs
--rw-r--r--   0     1001      123      306 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/dsl/function_expr/search_sorted.rs
--rw-r--r--   0     1001      123     3812 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/dsl/function_expr/shift_and_fill.rs
--rw-r--r--   0     1001      123     1238 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/dsl/function_expr/shrink_type.rs
--rw-r--r--   0     1001      123      972 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/dsl/function_expr/sign.rs
--rw-r--r--   0     1001      123    21047 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/dsl/function_expr/strings.rs
--rw-r--r--   0     1001      123     1017 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/dsl/function_expr/struct_.rs
--rw-r--r--   0     1001      123     5509 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/dsl/function_expr/temporal.rs
--rw-r--r--   0     1001      123     5122 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/dsl/function_expr/trigonometry.rs
--rw-r--r--   0     1001      123      170 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/dsl/function_expr/unique.rs
--rw-r--r--   0     1001      123     1155 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/dsl/functions/arity.rs
--rw-r--r--   0     1001      123      611 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/dsl/functions/coerce.rs
--rw-r--r--   0     1001      123     2717 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/dsl/functions/concat.rs
--rw-r--r--   0     1001      123     4525 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/dsl/functions/correlation.rs
--rw-r--r--   0     1001      123     8736 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/dsl/functions/horizontal.rs
--rw-r--r--   0     1001      123     1044 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/dsl/functions/index.rs
--rw-r--r--   0     1001      123      968 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/dsl/functions/mod.rs
--rw-r--r--   0     1001      123     9827 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/dsl/functions/range.rs
--rw-r--r--   0     1001      123     1308 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/dsl/functions/selectors.rs
--rw-r--r--   0     1001      123     1973 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/dsl/functions/syntactic_sugar.rs
--rw-r--r--   0     1001      123    11328 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/dsl/functions/temporal.rs
--rw-r--r--   0     1001      123    10213 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/dsl/list.rs
--rw-r--r--   0     1001      123     3772 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/dsl/meta.rs
--rw-r--r--   0     1001      123    61431 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/dsl/mod.rs
--rw-r--r--   0     1001      123       40 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/dsl/names.rs
--rw-r--r--   0     1001      123     2658 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/dsl/options.rs
--rw-r--r--   0     1001      123     1068 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/dsl/selector.rs
--rw-r--r--   0     1001      123    17095 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/dsl/string.rs
--rw-r--r--   0     1001      123     2715 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/dsl/struct_.rs
--rw-r--r--   0     1001      123       38 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/frame/mod.rs
--rw-r--r--   0     1001      123      933 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/frame/opt_state.rs
--rw-r--r--   0     1001      123      466 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/global.rs
--rw-r--r--   0     1001      123      175 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/lib.rs
--rw-r--r--   0     1001      123     8318 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/logical_plan/aexpr/mod.rs
--rw-r--r--   0     1001      123    11742 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/logical_plan/aexpr/schema.rs
--rw-r--r--   0     1001      123    25683 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/logical_plan/alp.rs
--rw-r--r--   0     1001      123     1622 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/logical_plan/anonymous_scan.rs
--rw-r--r--   0     1001      123     1428 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/logical_plan/apply.rs
--rw-r--r--   0     1001      123    24898 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/logical_plan/builder.rs
--rw-r--r--   0     1001      123    29993 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/logical_plan/conversion.rs
--rw-r--r--   0     1001      123      301 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/logical_plan/debug.rs
--rw-r--r--   0     1001      123    15470 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/logical_plan/format.rs
--rw-r--r--   0     1001      123      895 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/logical_plan/functions/drop.rs
--rw-r--r--   0     1001      123      137 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/logical_plan/functions/explode.rs
--rw-r--r--   0     1001      123     1169 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/logical_plan/functions/merge_sorted.rs
--rw-r--r--   0     1001      123    11905 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/logical_plan/functions/mod.rs
--rw-r--r--   0     1001      123     1330 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/logical_plan/functions/rename.rs
--rw-r--r--   0     1001      123    10140 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/logical_plan/iterator.rs
--rw-r--r--   0     1001      123    10559 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/logical_plan/lit.rs
--rw-r--r--   0     1001      123     8072 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/logical_plan/mod.rs
--rw-r--r--   0     1001      123     7416 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/logical_plan/optimizer/cache_states.rs
--rw-r--r--   0     1001      123    15277 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/logical_plan/optimizer/cse.rs
--rw-r--r--   0     1001      123     2889 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/logical_plan/optimizer/delay_rechunk.rs
--rw-r--r--   0     1001      123     3236 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/logical_plan/optimizer/drop_nulls.rs
--rw-r--r--   0     1001      123     3994 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/logical_plan/optimizer/fast_projection.rs
--rw-r--r--   0     1001      123    14479 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/logical_plan/optimizer/file_caching.rs
--rw-r--r--   0     1001      123     1556 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/logical_plan/optimizer/flatten_union.rs
--rw-r--r--   0     1001      123     6017 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/logical_plan/optimizer/fused.rs
--rw-r--r--   0     1001      123     6774 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/logical_plan/optimizer/mod.rs
--rw-r--r--   0     1001      123     1222 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/logical_plan/optimizer/predicate_pushdown/keys.rs
--rw-r--r--   0     1001      123    28901 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/logical_plan/optimizer/predicate_pushdown/mod.rs
--rw-r--r--   0     1001      123     2571 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/logical_plan/optimizer/predicate_pushdown/rename.rs
--rw-r--r--   0     1001      123    15756 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/logical_plan/optimizer/predicate_pushdown/utils.rs
--rw-r--r--   0     1001      123     1755 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/functions/melt.rs
--rw-r--r--   0     1001      123     3930 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/functions/mod.rs
--rw-r--r--   0     1001      123     1799 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/generic.rs
--rw-r--r--   0     1001      123     3269 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/groupby.rs
--rw-r--r--   0     1001      123     2638 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/hstack.rs
--rw-r--r--   0     1001      123    15752 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/joins.rs
--rw-r--r--   0     1001      123    26507 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/mod.rs
--rw-r--r--   0     1001      123     3707 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/projection.rs
--rw-r--r--   0     1001      123     2639 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/rename.rs
--rw-r--r--   0     1001      123     3501 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/semi_anti_join.rs
--rw-r--r--   0     1001      123    27269 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/logical_plan/optimizer/simplify_expr.rs
--rw-r--r--   0     1001      123     3492 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/logical_plan/optimizer/slice_pushdown_expr.rs
--rw-r--r--   0     1001      123    13232 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/logical_plan/optimizer/slice_pushdown_lp.rs
--rw-r--r--   0     1001      123     4181 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/logical_plan/optimizer/stack_opt.rs
--rw-r--r--   0     1001      123     9725 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/logical_plan/optimizer/type_coercion/binary.rs
--rw-r--r--   0     1001      123    20215 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/logical_plan/optimizer/type_coercion/mod.rs
--rw-r--r--   0     1001      123    10545 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/logical_plan/options.rs
--rw-r--r--   0     1001      123    18601 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/logical_plan/projection.rs
--rw-r--r--   0     1001      123     6144 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/logical_plan/pyarrow.rs
--rw-r--r--   0     1001      123    13026 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/logical_plan/schema.rs
--rw-r--r--   0     1001      123      832 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/prelude.rs
--rw-r--r--   0     1001      123    12428 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/utils.rs
--rw-r--r--   0        0        0     1998 1970-01-01 00:00:00.000000 polars_u64_idx-0.18.3/local_dependencies/polars-pipe/Cargo.toml
--rw-r--r--   0     1001      123     1055 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-pipe/LICENSE
--rw-r--r--   0     1001      123      165 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-pipe/README.md
--rw-r--r--   0     1001      123       98 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-pipe/src/executors/mod.rs
--rw-r--r--   0     1001      123     1219 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-pipe/src/executors/operators/filter.rs
--rw-r--r--   0     1001      123     4103 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-pipe/src/executors/operators/function.rs
--rw-r--r--   0     1001      123      266 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-pipe/src/executors/operators/mod.rs
--rw-r--r--   0     1001      123      682 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-pipe/src/executors/operators/pass.rs
--rw-r--r--   0     1001      123      548 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-pipe/src/executors/operators/placeholder.rs
--rw-r--r--   0     1001      123     3553 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-pipe/src/executors/operators/projection.rs
--rw-r--r--   0     1001      123     3559 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-pipe/src/executors/operators/reproject.rs
--rw-r--r--   0     1001      123     6479 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-pipe/src/executors/sinks/file_sink.rs
--rw-r--r--   0     1001      123    11288 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/convert.rs
--rw-r--r--   0     1001      123     1207 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/count.rs
--rw-r--r--   0     1001      123     1888 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/first.rs
--rw-r--r--   0     1001      123     4554 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/interface.rs
--rw-r--r--   0     1001      123     1746 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/last.rs
--rw-r--r--   0     1001      123     5413 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/mean.rs
--rw-r--r--   0     1001      123     4951 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/min_max.rs
--rw-r--r--   0     1001      123      211 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/mod.rs
--rw-r--r--   0     1001      123      856 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/null.rs
--rw-r--r--   0     1001      123     4294 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/sum.rs
--rw-r--r--   0     1001      123     4102 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/eval.rs
--rw-r--r--   0     1001      123     7404 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/global.rs
--rw-r--r--   0     1001      123    10553 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/hash_table.rs
--rw-r--r--   0     1001      123     3589 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/mod.rs
--rw-r--r--   0     1001      123     2767 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/ooc_state.rs
--rw-r--r--   0     1001      123     6326 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/sink.rs
--rw-r--r--   0     1001      123     3116 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/source.rs
--rw-r--r--   0     1001      123    10194 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/thread_local.rs
--rw-r--r--   0     1001      123     2119 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-pipe/src/executors/sinks/groupby/mod.rs
--rw-r--r--   0     1001      123     4695 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-pipe/src/executors/sinks/groupby/ooc.rs
--rw-r--r--   0     1001      123     1887 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-pipe/src/executors/sinks/groupby/ooc_state.rs
--rw-r--r--   0     1001      123    20783 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-pipe/src/executors/sinks/groupby/primitive/mod.rs
--rw-r--r--   0     1001      123    23825 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-pipe/src/executors/sinks/groupby/string.rs
--rw-r--r--   0     1001      123     2457 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-pipe/src/executors/sinks/groupby/utils.rs
--rw-r--r--   0     1001      123     9239 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-pipe/src/executors/sinks/io.rs
--rw-r--r--   0     1001      123     5451 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-pipe/src/executors/sinks/joins/cross.rs
--rw-r--r--   0     1001      123    11949 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-pipe/src/executors/sinks/joins/generic_build.rs
--rw-r--r--   0     1001      123    11756 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-pipe/src/executors/sinks/joins/inner_left.rs
--rw-r--r--   0     1001      123      178 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-pipe/src/executors/sinks/joins/mod.rs
--rw-r--r--   0     1001      123     2241 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-pipe/src/executors/sinks/memory.rs
--rw-r--r--   0     1001      123      589 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-pipe/src/executors/sinks/mod.rs
--rw-r--r--   0     1001      123     1492 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-pipe/src/executors/sinks/ordered.rs
--rw-r--r--   0     1001      123     1824 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-pipe/src/executors/sinks/reproject.rs
--rw-r--r--   0     1001      123     3108 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-pipe/src/executors/sinks/slice.rs
--rw-r--r--   0     1001      123      130 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-pipe/src/executors/sinks/sort/mod.rs
--rw-r--r--   0     1001      123     6787 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-pipe/src/executors/sinks/sort/ooc.rs
--rw-r--r--   0     1001      123     7279 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-pipe/src/executors/sinks/sort/sink.rs
--rw-r--r--   0     1001      123     5953 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-pipe/src/executors/sinks/sort/sink_multiple.rs
--rw-r--r--   0     1001      123     3908 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-pipe/src/executors/sinks/sort/source.rs
--rw-r--r--   0     1001      123      526 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-pipe/src/executors/sinks/utils.rs
--rw-r--r--   0     1001      123     5984 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-pipe/src/executors/sources/csv.rs
--rw-r--r--   0     1001      123     1231 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-pipe/src/executors/sources/frame.rs
--rw-r--r--   0     1001      123      987 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-pipe/src/executors/sources/ipc_one_shot.rs
--rw-r--r--   0     1001      123      366 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-pipe/src/executors/sources/mod.rs
--rw-r--r--   0     1001      123     4335 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-pipe/src/executors/sources/parquet.rs
--rw-r--r--   0     1001      123     1146 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-pipe/src/executors/sources/reproject.rs
--rw-r--r--   0     1001      123     1022 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-pipe/src/executors/sources/union.rs
--rw-r--r--   0     1001      123      448 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-pipe/src/expressions.rs
--rw-r--r--   0     1001      123      272 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-pipe/src/lib.rs
--rw-r--r--   0     1001      123      719 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-pipe/src/operators/chunks.rs
--rw-r--r--   0     1001      123      474 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-pipe/src/operators/context.rs
--rw-r--r--   0     1001      123      223 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-pipe/src/operators/mod.rs
--rw-r--r--   0     1001      123      514 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-pipe/src/operators/operator.rs
--rw-r--r--   0     1001      123      626 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-pipe/src/operators/sink.rs
--rw-r--r--   0     1001      123      241 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-pipe/src/operators/source.rs
--rw-r--r--   0     1001      123        1 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-pipe/src/pipeline/config.rs
--rw-r--r--   0     1001      123    21321 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-pipe/src/pipeline/convert.rs
--rw-r--r--   0     1001      123    18204 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-pipe/src/pipeline/dispatcher.rs
--rw-r--r--   0     1001      123     1155 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-pipe/src/pipeline/mod.rs
--rw-r--r--   0        0        0     2037 1970-01-01 00:00:00.000000 polars_u64_idx-0.18.3/local_dependencies/polars-time/Cargo.toml
--rw-r--r--   0     1001      123     1055 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-time/LICENSE
--rw-r--r--   0     1001      123      143 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-time/README.md
--rw-r--r--   0     1001      123     3565 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-time/src/chunkedarray/date.rs
--rw-r--r--   0     1001      123     6465 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-time/src/chunkedarray/datetime.rs
--rw-r--r--   0     1001      123     3305 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-time/src/chunkedarray/duration.rs
--rw-r--r--   0     1001      123     5607 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-time/src/chunkedarray/kernels.rs
--rw-r--r--   0     1001      123     1062 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-time/src/chunkedarray/mod.rs
--rw-r--r--   0     1001      123     7302 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-time/src/chunkedarray/rolling_window/floats.rs
--rw-r--r--   0     1001      123     2582 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-time/src/chunkedarray/rolling_window/ints.rs
--rw-r--r--   0     1001      123    11101 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-time/src/chunkedarray/rolling_window/mod.rs
--rw-r--r--   0     1001      123      428 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-time/src/chunkedarray/rolling_window/rolling_kernels/mod.rs
--rw-r--r--   0     1001      123     6408 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-time/src/chunkedarray/rolling_window/rolling_kernels/no_nulls.rs
--rw-r--r--   0     1001      123     2372 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-time/src/chunkedarray/time.rs
--rw-r--r--   0     1001      123    18180 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-time/src/chunkedarray/utf8/infer.rs
--rw-r--r--   0     1001      123    18997 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-time/src/chunkedarray/utf8/mod.rs
--rw-r--r--   0     1001      123     3975 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-time/src/chunkedarray/utf8/patterns.rs
--rw-r--r--   0     1001      123    10548 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-time/src/chunkedarray/utf8/strptime.rs
--rw-r--r--   0     1001      123     3442 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-time/src/date_range.rs
--rw-r--r--   0     1001      123    34469 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-time/src/groupby/dynamic.rs
--rw-r--r--   0     1001      123       88 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-time/src/groupby/mod.rs
--rw-r--r--   0     1001      123      621 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-time/src/lib.rs
--rw-r--r--   0     1001      123     2976 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-time/src/month_end.rs
--rw-r--r--   0     1001      123     3365 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-time/src/month_start.rs
--rw-r--r--   0     1001      123      274 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-time/src/prelude.rs
--rw-r--r--   0     1001      123     1381 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-time/src/round.rs
--rw-r--r--   0     1001      123     3992 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-time/src/series/_trait.rs
--rw-r--r--   0     1001      123      136 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-time/src/series/implementations/boolean.rs
--rw-r--r--   0     1001      123      140 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-time/src/series/implementations/categoricals.rs
--rw-r--r--   0     1001      123      133 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-time/src/series/implementations/date.rs
--rw-r--r--   0     1001      123      137 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-time/src/series/implementations/datetime.rs
--rw-r--r--   0     1001      123      137 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-time/src/series/implementations/duration.rs
--rw-r--r--   0     1001      123     1863 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-time/src/series/implementations/floats.rs
--rw-r--r--   0     1001      123     1792 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-time/src/series/implementations/integers.rs
--rw-r--r--   0     1001      123      133 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-time/src/series/implementations/list.rs
--rw-r--r--   0     1001      123      486 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-time/src/series/implementations/mod.rs
--rw-r--r--   0     1001      123      155 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-time/src/series/implementations/object.rs
--rw-r--r--   0     1001      123      135 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-time/src/series/implementations/struct_.rs
--rw-r--r--   0     1001      123      133 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-time/src/series/implementations/time.rs
--rw-r--r--   0     1001      123      133 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-time/src/series/implementations/utf8.rs
--rw-r--r--   0     1001      123    12787 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-time/src/series/mod.rs
--rw-r--r--   0     1001      123     1443 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-time/src/truncate.rs
--rw-r--r--   0     1001      123     6845 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-time/src/upsample.rs
--rw-r--r--   0     1001      123     2511 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-time/src/utils.rs
--rw-r--r--   0     1001      123     1524 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-time/src/windows/bounds.rs
--rw-r--r--   0     1001      123     2672 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-time/src/windows/calendar.rs
--rw-r--r--   0     1001      123    25015 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-time/src/windows/duration.rs
--rw-r--r--   0     1001      123    21244 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-time/src/windows/groupby.rs
--rw-r--r--   0     1001      123      503 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-time/src/windows/mod.rs
--rw-r--r--   0     1001      123    23652 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-time/src/windows/test.rs
--rw-r--r--   0     1001      123    10657 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-time/src/windows/window.rs
--rw-r--r--   0        0        0      569 1970-01-01 00:00:00.000000 polars_u64_idx-0.18.3/local_dependencies/polars-utils/Cargo.toml
--rw-r--r--   0     1001      123     1055 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-utils/LICENSE
--rw-r--r--   0     1001      123      141 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-utils/README.md
--rw-r--r--   0     1001      123      151 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-utils/src/aliases.rs
--rw-r--r--   0     1001      123     2862 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-utils/src/arena.rs
--rw-r--r--   0     1001      123     1373 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-utils/src/atomic.rs
--rw-r--r--   0     1001      123     2659 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-utils/src/cell.rs
--rw-r--r--   0     1001      123     1015 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-utils/src/contention_pool.rs
--rw-r--r--   0     1001      123      509 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-utils/src/error.rs
--rw-r--r--   0     1001      123      271 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-utils/src/fmt.rs
--rw-r--r--   0     1001      123      763 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-utils/src/functions.rs
--rw-r--r--   0     1001      123     2709 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-utils/src/iter/enumerate_idx.rs
--rw-r--r--   0     1001      123       61 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-utils/src/iter/mod.rs
--rw-r--r--   0     1001      123      503 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-utils/src/lib.rs
--rw-r--r--   0     1001      123      573 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-utils/src/macros.rs
--rw-r--r--   0     1001      123      282 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-utils/src/mem.rs
--rw-r--r--   0     1001      123     2336 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-utils/src/slice.rs
--rw-r--r--   0     1001      123     2467 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-utils/src/sort.rs
--rw-r--r--   0     1001      123     1115 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-utils/src/sync.rs
--rw-r--r--   0     1001      123      504 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-utils/src/sys.rs
--rw-r--r--   0     1001      123      697 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-utils/src/unwrap.rs
--rw-r--r--   0     1001      123      498 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-utils/src/vec.rs
--rw-r--r--   0     1001      123      616 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-utils/src/wasm.rs
--rw-r--r--   0        0        0      954 1970-01-01 00:00:00.000000 polars_u64_idx-0.18.3/local_dependencies/polars-row/Cargo.toml
--rw-r--r--   0     1001      123     1055 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-row/LICENSE
--rw-r--r--   0     1001      123      137 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-row/README.md
--rw-r--r--   0     1001      123     1916 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-row/src/decode.rs
--rw-r--r--   0     1001      123    11571 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-row/src/encode.rs
--rw-r--r--   0     1001      123     7436 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-row/src/fixed.rs
--rw-r--r--   0     1001      123    13846 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-row/src/lib.rs
--rw-r--r--   0     1001      123     3019 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-row/src/row.rs
--rw-r--r--   0     1001      123      682 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-row/src/utils.rs
--rw-r--r--   0     1001      123     7559 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-row/src/variable.rs
--rw-r--r--   0        0        0     1106 1970-01-01 00:00:00.000000 polars_u64_idx-0.18.3/local_dependencies/polars-sql/Cargo.toml
--rw-r--r--   0     1001      123     1055 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-sql/LICENSE
--rw-r--r--   0     1001      123      466 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-sql/README.md
--rw-r--r--   0     1001      123    23236 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-sql/src/context.rs
--rw-r--r--   0     1001      123    20711 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-sql/src/functions.rs
--rw-r--r--   0     1001      123     2122 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-sql/src/keywords.rs
--rw-r--r--   0     1001      123      239 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-sql/src/lib.rs
--rw-r--r--   0     1001      123    20991 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-sql/src/sql_expr.rs
--rw-r--r--   0     1001      123     4572 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-sql/src/table_functions.rs
--rw-r--r--   0     1001      123     1682 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-sql/tests/functions_cumulative.rs
--rw-r--r--   0     1001      123     3063 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-sql/tests/functions_io.rs
--rw-r--r--   0     1001      123     1539 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-sql/tests/functions_math.rs
--rw-r--r--   0     1001      123      860 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-sql/tests/functions_meta.rs
--rw-r--r--   0     1001      123     2982 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-sql/tests/functions_string.rs
--rw-r--r--   0     1001      123     1056 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-sql/tests/iss_7436.rs
--rw-r--r--   0     1001      123      888 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-sql/tests/iss_7437.rs
--rw-r--r--   0     1001      123      652 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-sql/tests/iss_7440.rs
--rw-r--r--   0     1001      123      700 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-sql/tests/iss_8395.rs
--rw-r--r--   0     1001      123     1062 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-sql/tests/iss_8419.rs
--rw-r--r--   0     1001      123      982 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-sql/tests/ops_distinct_on.rs
--rw-r--r--   0     1001      123    15418 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-sql/tests/simple_exprs.rs
--rw-r--r--   0     1001      123     3343 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-sql/tests/statements.rs
--rw-r--r--   0        0        0     5484 1970-01-01 00:00:00.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/Cargo.toml
--rw-r--r--   0     1001      123     1055 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/LICENSE
--rw-r--r--   0     1001      123      144 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/README.md
--rw-r--r--   0     1001      123     5158 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/arithmetic/decimal.rs
--rw-r--r--   0     1001      123     8275 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/arithmetic/mod.rs
--rw-r--r--   0     1001      123     9417 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/arithmetic/numeric.rs
--rw-r--r--   0     1001      123     3588 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/array/iterator.rs
--rw-r--r--   0     1001      123     2551 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/array/mod.rs
--rw-r--r--   0     1001      123     6448 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/bitwise.rs
--rw-r--r--   0     1001      123     2298 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/builder/binary.rs
--rw-r--r--   0     1001      123     1207 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/builder/boolean.rs
--rw-r--r--   0     1001      123     4311 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/builder/fixed_size_list.rs
--rw-r--r--   0     1001      123     1556 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/builder/from.rs
--rw-r--r--   0     1001      123    20366 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/builder/list.rs
--rw-r--r--   0     1001      123     8969 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/builder/mod.rs
--rw-r--r--   0     1001      123     1410 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/builder/primitive.rs
--rw-r--r--   0     1001      123     2291 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/builder/utf8.rs
--rw-r--r--   0     1001      123    16475 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/cast.rs
--rw-r--r--   0     1001      123    49461 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/comparison/mod.rs
--rw-r--r--   0     1001      123    10060 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/comparison/scalar.rs
--rw-r--r--   0     1001      123      551 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/drop.rs
--rw-r--r--   0     1001      123      963 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/float.rs
--rw-r--r--   0     1001      123     7175 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/from.rs
--rw-r--r--   0     1001      123    42339 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/iterator/mod.rs
--rw-r--r--   0     1001      123     1453 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/iterator/par/list.rs
--rw-r--r--   0     1001      123       28 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/iterator/par/mod.rs
--rw-r--r--   0     1001      123     1129 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/iterator/par/utf8.rs
--rw-r--r--   0     1001      123       21 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/kernels/mod.rs
--rw-r--r--   0     1001      123     2347 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/kernels/take.rs
--rw-r--r--   0     1001      123     7963 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/list/iterator.rs
--rw-r--r--   0     1001      123     3242 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/list/mod.rs
--rw-r--r--   0     1001      123    19830 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/logical/categorical/builder.rs
--rw-r--r--   0     1001      123     3688 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/logical/categorical/from.rs
--rw-r--r--   0     1001      123     4270 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/logical/categorical/merge.rs
--rw-r--r--   0     1001      123    10219 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/logical/categorical/mod.rs
--rw-r--r--   0     1001      123     1400 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/append.rs
--rw-r--r--   0     1001      123      358 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/full.rs
--rw-r--r--   0     1001      123      192 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/mod.rs
--rw-r--r--   0     1001      123     2731 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/take_random.rs
--rw-r--r--   0     1001      123     2172 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/unique.rs
--rw-r--r--   0     1001      123      925 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/zip.rs
--rw-r--r--   0     1001      123     6417 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/logical/categorical/stringcache.rs
--rw-r--r--   0     1001      123     1604 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/logical/date.rs
--rw-r--r--   0     1001      123     4105 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/logical/datetime.rs
--rw-r--r--   0     1001      123     4443 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/logical/decimal.rs
--rw-r--r--   0     1001      123     2434 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/logical/duration.rs
--rw-r--r--   0     1001      123     2556 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/logical/mod.rs
--rw-r--r--   0     1001      123      476 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/logical/struct_/from.rs
--rw-r--r--   0     1001      123    15982 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/logical/struct_/mod.rs
--rw-r--r--   0     1001      123     1182 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/logical/time.rs
--rw-r--r--   0     1001      123    23489 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/mod.rs
--rw-r--r--   0     1001      123     7200 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/ndarray.rs
--rw-r--r--   0     1001      123     4484 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/object/builder.rs
--rw-r--r--   0     1001      123     1547 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/object/extension/drop.rs
--rw-r--r--   0     1001      123     3124 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/object/extension/list.rs
--rw-r--r--   0     1001      123     7054 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/object/extension/mod.rs
--rw-r--r--   0     1001      123     3410 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/object/extension/polars_extension.rs
--rw-r--r--   0     1001      123      137 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/object/is_valid.rs
--rw-r--r--   0     1001      123     4419 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/object/iterator.rs
--rw-r--r--   0     1001      123     4806 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/object/mod.rs
--rw-r--r--   0     1001      123     2956 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/object/registry.rs
--rw-r--r--   0     1001      123      272 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/ops/abs.rs
--rw-r--r--   0     1001      123    32691 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/ops/aggregate/mod.rs
--rw-r--r--   0     1001      123    10025 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/ops/aggregate/quantile.rs
--rw-r--r--   0     1001      123     2880 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/ops/aggregate/var.rs
--rw-r--r--   0     1001      123    10551 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/ops/any_value.rs
--rw-r--r--   0     1001      123     2820 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/ops/append.rs
--rw-r--r--   0     1001      123    28256 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/ops/apply.rs
--rw-r--r--   0     1001      123    12799 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/ops/bit_repr.rs
--rw-r--r--   0     1001      123     6236 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/ops/chunkops.rs
--rw-r--r--   0     1001      123    11537 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/ops/compare_inner.rs
--rw-r--r--   0     1001      123     1737 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/ops/concat_str.rs
--rw-r--r--   0     1001      123     4801 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/ops/cum_agg.rs
--rw-r--r--   0     1001      123      908 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/ops/decimal.rs
--rw-r--r--   0     1001      123     7056 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/ops/downcast.rs
--rw-r--r--   0     1001      123    19461 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/ops/explode.rs
--rw-r--r--   0     1001      123     8691 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/ops/explode_and_offsets.rs
--rw-r--r--   0     1001      123     8866 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/ops/extend.rs
--rw-r--r--   0     1001      123    13777 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/ops/fill_null.rs
--rw-r--r--   0     1001      123     6356 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/ops/filter.rs
--rw-r--r--   0     1001      123     5876 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/ops/full.rs
--rw-r--r--   0     1001      123        1 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/ops/interpolate.rs
--rw-r--r--   0     1001      123    16797 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/ops/is_in.rs
--rw-r--r--   0     1001      123        1 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/ops/len.rs
--rw-r--r--   0     1001      123     2658 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/ops/min_max_binary.rs
--rw-r--r--   0     1001      123    23276 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/ops/mod.rs
--rw-r--r--   0     1001      123     2414 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/ops/nulls.rs
--rw-r--r--   0     1001      123      593 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/ops/peaks.rs
--rw-r--r--   0     1001      123     4375 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/ops/repeat_by.rs
--rw-r--r--   0     1001      123     2771 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/ops/reverse.rs
--rw-r--r--   0     1001      123    10266 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/ops/rolling_window.rs
--rw-r--r--   0     1001      123    12518 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/ops/set.rs
--rw-r--r--   0     1001      123     7391 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/ops/shift.rs
--rw-r--r--   0     1001      123     2299 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/ops/sort/arg_sort.rs
--rw-r--r--   0     1001      123     5528 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/ops/sort/arg_sort_multiple.rs
--rw-r--r--   0     1001      123     7543 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/ops/sort/categorical.rs
--rw-r--r--   0     1001      123    31164 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/ops/sort/mod.rs
--rw-r--r--   0     1001      123      380 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/ops/sort/slice.rs
--rw-r--r--   0     1001      123    22089 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/ops/take/mod.rs
--rw-r--r--   0     1001      123     7848 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/ops/take/take_chunked.rs
--rw-r--r--   0     1001      123      301 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/ops/take/take_every.rs
--rw-r--r--   0     1001      123    16256 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/ops/take/take_random.rs
--rw-r--r--   0     1001      123     5810 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/ops/take/take_single.rs
--rw-r--r--   0     1001      123     6072 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/ops/take/traits.rs
--rw-r--r--   0     1001      123      459 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/ops/tile.rs
--rw-r--r--   0     1001      123    11626 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/ops/unique/mod.rs
--rw-r--r--   0     1001      123    14620 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/ops/unique/rank.rs
--rw-r--r--   0     1001      123     5846 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/ops/zip.rs
--rw-r--r--   0     1001      123     9093 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/random.rs
--rw-r--r--   0     1001      123     1875 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/temporal/conversion.rs
--rw-r--r--   0     1001      123     2826 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/temporal/date.rs
--rw-r--r--   0     1001      123    10497 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/temporal/datetime.rs
--rw-r--r--   0     1001      123     3201 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/temporal/duration.rs
--rw-r--r--   0     1001      123      595 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/temporal/mod.rs
--rw-r--r--   0     1001      123     3042 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/temporal/time.rs
--rw-r--r--   0     1001      123      872 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/to_vec.rs
--rw-r--r--   0     1001      123     8113 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/trusted_len.rs
--rw-r--r--   0     1001      123    25939 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/upstream_traits.rs
--rw-r--r--   0     1001      123     7944 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/cloud.rs
--rw-r--r--   0     1001      123     1549 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/config.rs
--rw-r--r--   0     1001      123     3946 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/datatypes/_serde.rs
--rw-r--r--   0     1001      123     2509 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/datatypes/aliases.rs
--rw-r--r--   0     1001      123    42658 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/datatypes/any_value.rs
--rw-r--r--   0     1001      123    13349 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/datatypes/dtype.rs
--rw-r--r--   0     1001      123     5609 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/datatypes/field.rs
--rw-r--r--   0     1001      123     8059 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/datatypes/mod.rs
--rw-r--r--   0     1001      123     2016 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/datatypes/time_unit.rs
--rw-r--r--   0     1001      123      118 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/doc/changelog/mod.rs
--rw-r--r--   0     1001      123      898 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/doc/changelog/v0_10_0_11.rs
--rw-r--r--   0     1001      123      481 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/doc/changelog/v0_3.rs
--rw-r--r--   0     1001      123      293 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/doc/changelog/v0_4.rs
--rw-r--r--   0     1001      123      499 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/doc/changelog/v0_5.rs
--rw-r--r--   0     1001      123      288 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/doc/changelog/v0_6.rs
--rw-r--r--   0     1001      123     1071 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/doc/changelog/v0_7.rs
--rw-r--r--   0     1001      123      819 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/doc/changelog/v0_8.rs
--rw-r--r--   0     1001      123      596 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/doc/changelog/v0_9.rs
--rw-r--r--   0     1001      123       43 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/doc/mod.rs
--rw-r--r--   0     1001      123       25 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/error.rs
--rw-r--r--   0     1001      123      263 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/export.rs
--rw-r--r--   0     1001      123    36432 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/fmt.rs
--rw-r--r--   0     1001      123     5177 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/frame/arithmetic.rs
--rw-r--r--   0     1001      123     9916 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/frame/asof_join/asof.rs
--rw-r--r--   0     1001      123    35761 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/frame/asof_join/groups.rs
--rw-r--r--   0     1001      123     7168 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/frame/asof_join/mod.rs
--rw-r--r--   0     1001      123      559 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/frame/chunks.rs
--rw-r--r--   0     1001      123     5181 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/frame/cross_join.rs
--rw-r--r--   0     1001      123    16760 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/frame/explode.rs
--rw-r--r--   0     1001      123     1019 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/frame/from.rs
--rw-r--r--   0     1001      123    19219 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/frame/groupby/aggregations/agg_list.rs
--rw-r--r--   0     1001      123     4113 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/frame/groupby/aggregations/boolean.rs
--rw-r--r--   0     1001      123     7749 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/frame/groupby/aggregations/dispatch.rs
--rw-r--r--   0     1001      123    40369 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/frame/groupby/aggregations/mod.rs
--rw-r--r--   0     1001      123     5634 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/frame/groupby/aggregations/utf8.rs
--rw-r--r--   0     1001      123      218 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/frame/groupby/expr.rs
--rw-r--r--   0     1001      123    22901 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/frame/groupby/hashing.rs
--rw-r--r--   0     1001      123    14380 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/frame/groupby/into_groups.rs
--rw-r--r--   0     1001      123    39623 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/frame/groupby/mod.rs
--rw-r--r--   0     1001      123    10637 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/frame/groupby/perfect.rs
--rw-r--r--   0     1001      123    19780 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/frame/groupby/proxy.rs
--rw-r--r--   0     1001      123     5406 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/frame/hash_join/args.rs
--rw-r--r--   0     1001      123    13329 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/frame/hash_join/mod.rs
--rw-r--r--   0     1001      123    22364 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/frame/hash_join/multiple_keys.rs
--rw-r--r--   0     1001      123     2413 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/frame/hash_join/single_keys.rs
--rw-r--r--   0     1001      123    17372 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/frame/hash_join/single_keys_dispatch.rs
--rw-r--r--   0     1001      123     4608 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/frame/hash_join/single_keys_inner.rs
--rw-r--r--   0     1001      123     6434 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/frame/hash_join/single_keys_left.rs
--rw-r--r--   0     1001      123     4564 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/frame/hash_join/single_keys_outer.rs
--rw-r--r--   0     1001      123     3913 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/frame/hash_join/single_keys_semi_anti.rs
--rw-r--r--   0     1001      123    12313 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/frame/hash_join/sort_merge.rs
--rw-r--r--   0     1001      123     3865 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/frame/hash_join/zip_outer.rs
--rw-r--r--   0     1001      123   126103 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/frame/mod.rs
--rw-r--r--   0     1001      123    27652 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/frame/row/av_buffer.rs
--rw-r--r--   0     1001      123     5183 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/frame/row/dataframe.rs
--rw-r--r--   0     1001      123     5976 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/frame/row/mod.rs
--rw-r--r--   0     1001      123     9875 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/frame/row/transpose.rs
--rw-r--r--   0     1001      123     2811 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/frame/top_k.rs
--rw-r--r--   0     1001      123     1388 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/frame/upstream_traits.rs
--rw-r--r--   0     1001      123    10198 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/functions.rs
--rw-r--r--   0     1001      123     2149 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/hashing/fx.rs
--rw-r--r--   0     1001      123     1503 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/hashing/identity.rs
--rw-r--r--   0     1001      123      457 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/hashing/mod.rs
--rw-r--r--   0     1001      123     2684 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/hashing/partition.rs
--rw-r--r--   0     1001      123    17704 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/hashing/vector_hasher.rs
--rw-r--r--   0     1001      123     1896 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/lib.rs
--rw-r--r--   0     1001      123    15733 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/named_from.rs
--rw-r--r--   0     1001      123     2423 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/prelude.rs
--rw-r--r--   0     1001      123    17667 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/schema.rs
--rw-r--r--   0     1001      123     4218 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/serde/chunked_array.rs
--rw-r--r--   0     1001      123     1094 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/serde/df.rs
--rw-r--r--   0     1001      123     6559 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/serde/mod.rs
--rw-r--r--   0     1001      123     9510 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/serde/series.rs
--rw-r--r--   0     1001      123    18543 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/series/any_value.rs
--rw-r--r--   0     1001      123    28755 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/series/arithmetic/borrowed.rs
--rw-r--r--   0     1001      123      222 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/series/arithmetic/mod.rs
--rw-r--r--   0     1001      123     3546 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/series/arithmetic/owned.rs
--rw-r--r--   0     1001      123    19293 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/series/comparison.rs
--rw-r--r--   0     1001      123    29575 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/series/from.rs
--rw-r--r--   0     1001      123     6080 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/series/implementations/array.rs
--rw-r--r--   0     1001      123     9089 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/series/implementations/binary.rs
--rw-r--r--   0     1001      123    10835 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/series/implementations/boolean.rs
--rw-r--r--   0     1001      123    12800 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/series/implementations/categorical.rs
--rw-r--r--   0     1001      123    18214 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/series/implementations/dates_time.rs
--rw-r--r--   0     1001      123    15034 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/series/implementations/datetime.rs
--rw-r--r--   0     1001      123     7981 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/series/implementations/decimal.rs
--rw-r--r--   0     1001      123    14734 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/series/implementations/duration.rs
--rw-r--r--   0     1001      123    14063 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/series/implementations/floats.rs
--rw-r--r--   0     1001      123     6078 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/series/implementations/list.rs
--rw-r--r--   0     1001      123    18396 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/series/implementations/mod.rs
--rw-r--r--   0     1001      123     5522 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/series/implementations/null.rs
--rw-r--r--   0     1001      123     7939 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/series/implementations/object.rs
--rw-r--r--   0     1001      123    11788 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/series/implementations/struct_.rs
--rw-r--r--   0     1001      123     9607 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/series/implementations/utf8.rs
--rw-r--r--   0     1001      123     4471 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/series/into.rs
--rw-r--r--   0     1001      123     6241 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/series/iterator.rs
--rw-r--r--   0     1001      123    39074 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/series/mod.rs
--rw-r--r--   0     1001      123      853 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/series/ops/diff.rs
--rw-r--r--   0     1001      123     5814 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/series/ops/downcast.rs
--rw-r--r--   0     1001      123     3601 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/series/ops/ewm.rs
--rw-r--r--   0     1001      123      413 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/series/ops/extend.rs
--rw-r--r--   0     1001      123      562 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/series/ops/mod.rs
--rw-r--r--   0     1001      123     5974 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/series/ops/moment.rs
--rw-r--r--   0     1001      123     2908 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/series/ops/null.rs
--rw-r--r--   0     1001      123     1347 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/series/ops/pct_change.rs
--rw-r--r--   0     1001      123     4620 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/series/ops/round.rs
--rw-r--r--   0     1001      123     5073 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/series/ops/to_list.rs
--rw-r--r--   0     1001      123     1476 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/series/ops/unique.rs
--rw-r--r--   0     1001      123    18408 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/series/series_trait.rs
--rw-r--r--   0     1001      123     2912 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/series/unstable.rs
--rw-r--r--   0     1001      123     7077 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/testing.rs
--rw-r--r--   0     1001      123      508 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/tests.rs
--rw-r--r--   0     1001      123     2492 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/utils/flatten.rs
--rw-r--r--   0     1001      123    30596 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/utils/mod.rs
--rw-r--r--   0     1001      123     1600 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/utils/series.rs
--rw-r--r--   0     1001      123    13201 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-core/src/utils/supertype.rs
--rw-r--r--   0        0        0      827 1970-01-01 00:00:00.000000 polars_u64_idx-0.18.3/local_dependencies/polars-algo/Cargo.toml
--rw-r--r--   0     1001      123     1055 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-algo/LICENSE
--rw-r--r--   0     1001      123      142 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-algo/README.md
--rw-r--r--   0     1001      123     7548 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-algo/src/algo.rs
--rw-r--r--   0     1001      123       88 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-algo/src/lib.rs
--rw-r--r--   0     1001      123       28 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-algo/src/prelude.rs
--rw-r--r--   0        0        0     1353 1970-01-01 00:00:00.000000 polars_u64_idx-0.18.3/local_dependencies/polars-json/Cargo.toml
--rw-r--r--   0     1001      123     1055 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-json/LICENSE
--rw-r--r--   0     1001      123    16770 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-json/src/json/deserialize.rs
--rw-r--r--   0     1001      123     6564 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-json/src/json/infer_schema.rs
--rw-r--r--   0     1001      123      189 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-json/src/json/mod.rs
--rw-r--r--   0     1001      123       30 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-json/src/lib.rs
--rw-r--r--   0     1001      123     1198 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-json/src/ndjson/deserialize.rs
--rw-r--r--   0     1001      123     4808 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-json/src/ndjson/file.rs
--rw-r--r--   0     1001      123      143 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-json/src/ndjson/mod.rs
--rw-r--r--   0        0        0    10560 1970-01-01 00:00:00.000000 polars_u64_idx-0.18.3/local_dependencies/polars/Cargo.toml
--rw-r--r--   0     1001      123     1055 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars/LICENSE
--rw-r--r--   0     1001      123     3472 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars/Makefile
--rw-r--r--   0     1001      123      215 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars/build.rs
--rw-r--r--   0     1001      123       78 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars/clippy.toml
--rw-r--r--   0     1001      123    17602 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars/src/docs/eager.rs
--rw-r--r--   0     1001      123     8794 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars/src/docs/lazy.rs
--rw-r--r--   0     1001      123       50 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars/src/docs/mod.rs
--rw-r--r--   0     1001      123     3797 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars/src/docs/performance.rs
--rw-r--r--   0     1001      123       59 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars/src/export.rs
--rw-r--r--   0     1001      123    20214 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars/src/lib.rs
--rw-r--r--   0     1001      123      387 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars/src/prelude.rs
--rw-r--r--   0     1001      123       54 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars/src/sql.rs
--rw-r--r--   0     1001      123     4272 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars/tests/it/core/date_like.rs
--rw-r--r--   0     1001      123     2401 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars/tests/it/core/groupby.rs
--rw-r--r--   0     1001      123    17836 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars/tests/it/core/joins.rs
--rw-r--r--   0     1001      123      545 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars/tests/it/core/list.rs
--rw-r--r--   0     1001      123      198 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars/tests/it/core/mod.rs
--rw-r--r--   0     1001      123       24 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars/tests/it/core/ops/mod.rs
--rw-r--r--   0     1001      123      457 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars/tests/it/core/ops/take.rs
--rw-r--r--   0     1001      123     6259 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars/tests/it/core/pivot.rs
--rw-r--r--   0     1001      123     1102 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars/tests/it/core/random.rs
--rw-r--r--   0     1001      123    11096 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars/tests/it/core/rolling_window.rs
--rw-r--r--   0     1001      123     1093 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars/tests/it/core/series.rs
--rw-r--r--   0     1001      123      370 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars/tests/it/core/utils.rs
--rw-r--r--   0     1001      123    30423 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars/tests/it/io/csv.rs
--rw-r--r--   0     1001      123     4490 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars/tests/it/io/ipc_stream.rs
--rw-r--r--   0     1001      123     7043 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars/tests/it/io/json.rs
--rw-r--r--   0     1001      123      378 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars/tests/it/io/mod.rs
--rw-r--r--   0     1001      123      531 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars/tests/it/io/parquet.rs
--rw-r--r--   0     1001      123     1530 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars/tests/it/joins.rs
--rw-r--r--   0     1001      123     2452 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars/tests/it/lazy/aggregation.rs
--rw-r--r--   0     1001      123      821 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars/tests/it/lazy/cse.rs
--rw-r--r--   0     1001      123      500 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars/tests/it/lazy/explodes.rs
--rw-r--r--   0     1001      123     2279 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars/tests/it/lazy/expressions/apply.rs
--rw-r--r--   0     1001      123    10285 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars/tests/it/lazy/expressions/arity.rs
--rw-r--r--   0     1001      123     1065 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars/tests/it/lazy/expressions/expand.rs
--rw-r--r--   0     1001      123     1008 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars/tests/it/lazy/expressions/filter.rs
--rw-r--r--   0     1001      123      428 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars/tests/it/lazy/expressions/is_in.rs
--rw-r--r--   0     1001      123      121 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars/tests/it/lazy/expressions/mod.rs
--rw-r--r--   0     1001      123      659 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars/tests/it/lazy/expressions/slice.rs
--rw-r--r--   0     1001      123    10657 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars/tests/it/lazy/expressions/window.rs
--rw-r--r--   0     1001      123      579 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars/tests/it/lazy/folds.rs
--rw-r--r--   0     1001      123      557 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars/tests/it/lazy/functions.rs
--rw-r--r--   0     1001      123     4482 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars/tests/it/lazy/groupby.rs
--rw-r--r--   0     1001      123     1681 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars/tests/it/lazy/groupby_dynamic.rs
--rw-r--r--   0     1001      123      691 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars/tests/it/lazy/mod.rs
--rw-r--r--   0     1001      123     5747 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars/tests/it/lazy/predicate_queries.rs
--rw-r--r--   0     1001      123     4483 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars/tests/it/lazy/projection_queries.rs
--rw-r--r--   0     1001      123     6584 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars/tests/it/lazy/queries.rs
--rw-r--r--   0     1001      123      141 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars/tests/it/main.rs
--rw-r--r--   0     1001      123    12591 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars/tests/it/schema.rs
--rw-r--r--   0        0        0     3439 1970-01-01 00:00:00.000000 polars_u64_idx-0.18.3/local_dependencies/polars-ops/Cargo.toml
--rw-r--r--   0     1001      123     1055 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-ops/LICENSE
--rw-r--r--   0     1001      123      132 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-ops/README.md
--rw-r--r--   0     1001      123     2382 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-ops/src/chunked_array/array/min_max.rs
--rw-r--r--   0     1001      123      267 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-ops/src/chunked_array/array/mod.rs
--rw-r--r--   0     1001      123     1512 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-ops/src/chunked_array/array/namespace.rs
--rw-r--r--   0     1001      123     4108 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-ops/src/chunked_array/array/sum_mean.rs
--rw-r--r--   0     1001      123      234 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-ops/src/chunked_array/binary/mod.rs
--rw-r--r--   0     1001      123     3549 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-ops/src/chunked_array/binary/namespace.rs
--rw-r--r--   0     1001      123    11023 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-ops/src/chunked_array/interpolate.rs
--rw-r--r--   0     1001      123     1687 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-ops/src/chunked_array/list/count.rs
--rw-r--r--   0     1001      123     2419 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-ops/src/chunked_array/list/hash.rs
--rw-r--r--   0     1001      123     7861 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-ops/src/chunked_array/list/min_max.rs
--rw-r--r--   0     1001      123      511 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-ops/src/chunked_array/list/mod.rs
--rw-r--r--   0     1001      123    19010 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-ops/src/chunked_array/list/namespace.rs
--rw-r--r--   0     1001      123     7633 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-ops/src/chunked_array/list/sum_mean.rs
--rw-r--r--   0     1001      123     2435 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-ops/src/chunked_array/list/to_struct.rs
--rw-r--r--   0     1001      123      545 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-ops/src/chunked_array/mod.rs
--rw-r--r--   0     1001      123     9452 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-ops/src/chunked_array/nan_propagating_aggregate.rs
--rw-r--r--   0     1001      123     6795 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-ops/src/chunked_array/set.rs
--rw-r--r--   0     1001      123     7490 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-ops/src/chunked_array/strings/case.rs
--rw-r--r--   0     1001      123     8409 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-ops/src/chunked_array/strings/json_path.rs
--rw-r--r--   0     1001      123     2345 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-ops/src/chunked_array/strings/justify.rs
--rw-r--r--   0     1001      123      514 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-ops/src/chunked_array/strings/mod.rs
--rw-r--r--   0     1001      123    14731 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-ops/src/chunked_array/strings/namespace.rs
--rw-r--r--   0     1001      123     4053 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-ops/src/chunked_array/strings/replace.rs
--rw-r--r--   0     1001      123      439 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-ops/src/chunked_array/sum.rs
--rw-r--r--   0     1001      123     2486 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-ops/src/chunked_array/top_k.rs
--rw-r--r--   0     1001      123     7727 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-ops/src/frame/join/merge_sorted.rs
--rw-r--r--   0     1001      123    18232 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-ops/src/frame/join/mod.rs
--rw-r--r--   0     1001      123     4174 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-ops/src/frame/mod.rs
--rw-r--r--   0     1001      123    10257 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-ops/src/frame/pivot/mod.rs
--rw-r--r--   0     1001      123    13486 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-ops/src/frame/pivot/positioning.rs
--rw-r--r--   0     1001      123      237 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-ops/src/lib.rs
--rw-r--r--   0     1001      123      290 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-ops/src/prelude.rs
--rw-r--r--   0     1001      123       25 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-ops/src/series/mod.rs
--rw-r--r--   0     1001      123     9623 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-ops/src/series/ops/approx_algo/hyperloglogplus.rs
--rw-r--r--   0     1001      123      118 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-ops/src/series/ops/approx_algo/mod.rs
--rw-r--r--   0     1001      123     2016 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-ops/src/series/ops/approx_unique.rs
--rw-r--r--   0     1001      123    11866 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-ops/src/series/ops/arg_min_max.rs
--rw-r--r--   0     1001      123     3688 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-ops/src/series/ops/floor_divide.rs
--rw-r--r--   0     1001      123     5245 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-ops/src/series/ops/fused.rs
--rw-r--r--   0     1001      123     3423 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-ops/src/series/ops/is_first.rs
--rw-r--r--   0     1001      123     2975 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-ops/src/series/ops/is_unique.rs
--rw-r--r--   0     1001      123     3626 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-ops/src/series/ops/log.rs
--rw-r--r--   0     1001      123     1187 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-ops/src/series/ops/mod.rs
--rw-r--r--   0     1001      123     1769 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-ops/src/series/ops/rolling.rs
--rw-r--r--   0     1001      123     7642 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-ops/src/series/ops/search_sorted.rs
--rw-r--r--   0     1001      123     2500 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-ops/src/series/ops/to_dummies.rs
--rw-r--r--   0     1001      123     2067 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-ops/src/series/ops/various.rs
--rw-r--r--   0        0        0     5971 1970-01-01 00:00:00.000000 polars_u64_idx-0.18.3/local_dependencies/polars-lazy/Cargo.toml
--rw-r--r--   0     1001      123     1055 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-lazy/LICENSE
--rw-r--r--   0     1001      123      358 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-lazy/README.md
--rw-r--r--   0     1001      123     1796 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-lazy/src/dot.rs
--rw-r--r--   0     1001      123     4479 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-lazy/src/dsl/eval.rs
--rw-r--r--   0     1001      123     7115 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-lazy/src/dsl/functions.rs
--rw-r--r--   0     1001      123      164 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-lazy/src/dsl/into.rs
--rw-r--r--   0     1001      123     6754 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-lazy/src/dsl/list.rs
--rw-r--r--   0     1001      123     2899 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-lazy/src/dsl/mod.rs
--rw-r--r--   0     1001      123     1182 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-lazy/src/frame/anonymous_scan.rs
--rw-r--r--   0     1001      123     9285 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-lazy/src/frame/csv.rs
--rw-r--r--   0     1001      123     4316 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-lazy/src/frame/file_list_reader.rs
--rw-r--r--   0     1001      123     2261 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-lazy/src/frame/ipc.rs
--rw-r--r--   0     1001      123    49023 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-lazy/src/frame/mod.rs
--rw-r--r--   0     1001      123     3414 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-lazy/src/frame/ndjson.rs
--rw-r--r--   0     1001      123     2734 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-lazy/src/frame/parquet.rs
--rw-r--r--   0     1001      123     2892 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-lazy/src/frame/pivot.rs
--rw-r--r--   0     1001      123      416 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-lazy/src/frame/python.rs
--rw-r--r--   0     1001      123     6374 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-lazy/src/lib.rs
--rw-r--r--   0     1001      123     1049 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-lazy/src/physical_plan/executors/cache.rs
--rw-r--r--   0     1001      123      776 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-lazy/src/physical_plan/executors/executor.rs
--rw-r--r--   0     1001      123      670 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-lazy/src/physical_plan/executors/ext_context.rs
--rw-r--r--   0     1001      123     1555 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-lazy/src/physical_plan/executors/filter.rs
--rw-r--r--   0     1001      123     3986 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-lazy/src/physical_plan/executors/groupby.rs
--rw-r--r--   0     1001      123     4125 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-lazy/src/physical_plan/executors/groupby_dynamic.rs
--rw-r--r--   0     1001      123    13599 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-lazy/src/physical_plan/executors/groupby_partitioned.rs
--rw-r--r--   0     1001      123     4883 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-lazy/src/physical_plan/executors/groupby_rolling.rs
--rw-r--r--   0     1001      123     5859 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-lazy/src/physical_plan/executors/join.rs
--rw-r--r--   0     1001      123     6753 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-lazy/src/physical_plan/executors/mod.rs
--rw-r--r--   0     1001      123     2045 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-lazy/src/physical_plan/executors/projection.rs
--rw-r--r--   0     1001      123     1677 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-lazy/src/physical_plan/executors/python_scan.rs
--rw-r--r--   0     1001      123     2854 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-lazy/src/physical_plan/executors/scan/csv.rs
--rw-r--r--   0     1001      123     1963 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-lazy/src/physical_plan/executors/scan/ipc.rs
--rw-r--r--   0     1001      123     4303 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-lazy/src/physical_plan/executors/scan/mod.rs
--rw-r--r--   0     1001      123     1209 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-lazy/src/physical_plan/executors/scan/ndjson.rs
--rw-r--r--   0     1001      123     2421 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-lazy/src/physical_plan/executors/scan/parquet.rs
--rw-r--r--   0     1001      123      548 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-lazy/src/physical_plan/executors/slice.rs
--rw-r--r--   0     1001      123     2197 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-lazy/src/physical_plan/executors/sort.rs
--rw-r--r--   0     1001      123     2015 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-lazy/src/physical_plan/executors/stack.rs
--rw-r--r--   0     1001      123      663 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-lazy/src/physical_plan/executors/udf.rs
--rw-r--r--   0     1001      123     4041 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-lazy/src/physical_plan/executors/union.rs
--rw-r--r--   0     1001      123      838 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-lazy/src/physical_plan/executors/unique.rs
--rw-r--r--   0     1001      123     1335 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-lazy/src/physical_plan/exotic.rs
--rw-r--r--   0     1001      123    21959 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-lazy/src/physical_plan/expressions/aggregation.rs
--rw-r--r--   0     1001      123     2689 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-lazy/src/physical_plan/expressions/alias.rs
--rw-r--r--   0     1001      123    18331 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-lazy/src/physical_plan/expressions/apply.rs
--rw-r--r--   0     1001      123    17197 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-lazy/src/physical_plan/expressions/binary.rs
--rw-r--r--   0     1001      123     2583 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-lazy/src/physical_plan/expressions/cache.rs
--rw-r--r--   0     1001      123     3153 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-lazy/src/physical_plan/expressions/cast.rs
--rw-r--r--   0     1001      123     6326 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-lazy/src/physical_plan/expressions/column.rs
--rw-r--r--   0     1001      123     1996 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-lazy/src/physical_plan/expressions/count.rs
--rw-r--r--   0     1001      123     5809 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-lazy/src/physical_plan/expressions/filter.rs
--rw-r--r--   0     1001      123     4131 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-lazy/src/physical_plan/expressions/group_iter.rs
--rw-r--r--   0     1001      123     5304 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-lazy/src/physical_plan/expressions/literal.rs
--rw-r--r--   0     1001      123    23566 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-lazy/src/physical_plan/expressions/mod.rs
--rw-r--r--   0     1001      123    10091 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-lazy/src/physical_plan/expressions/slice.rs
--rw-r--r--   0     1001      123     4332 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-lazy/src/physical_plan/expressions/sort.rs
--rw-r--r--   0     1001      123    13549 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-lazy/src/physical_plan/expressions/sortby.rs
--rw-r--r--   0     1001      123     8331 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-lazy/src/physical_plan/expressions/take.rs
--rw-r--r--   0     1001      123    14360 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-lazy/src/physical_plan/expressions/ternary.rs
--rw-r--r--   0     1001      123    31558 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-lazy/src/physical_plan/expressions/window.rs
--rw-r--r--   0     1001      123     2039 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-lazy/src/physical_plan/file_cache.rs
--rw-r--r--   0     1001      123      414 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-lazy/src/physical_plan/mod.rs
--rw-r--r--   0     1001      123     2005 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-lazy/src/physical_plan/node_timer.rs
--rw-r--r--   0     1001      123    24050 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-lazy/src/physical_plan/planner/expr.rs
--rw-r--r--   0     1001      123    20552 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-lazy/src/physical_plan/planner/lp.rs
--rw-r--r--   0     1001      123       87 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-lazy/src/physical_plan/planner/mod.rs
--rw-r--r--   0     1001      123     9647 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-lazy/src/physical_plan/state.rs
--rw-r--r--   0     1001      123     2583 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-lazy/src/physical_plan/streaming/checks.rs
--rw-r--r--   0     1001      123     9227 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-lazy/src/physical_plan/streaming/construct_pipeline.rs
--rw-r--r--   0     1001      123    16847 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-lazy/src/physical_plan/streaming/convert_alp.rs
--rw-r--r--   0     1001      123      116 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-lazy/src/physical_plan/streaming/mod.rs
--rw-r--r--   0     1001      123     5827 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-lazy/src/physical_plan/streaming/tree.rs
--rw-r--r--   0     1001      123      722 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-lazy/src/prelude.rs
--rw-r--r--   0     1001      123    14990 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-lazy/src/tests/aggregations.rs
--rw-r--r--   0     1001      123     2339 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-lazy/src/tests/arity.rs
--rw-r--r--   0     1001      123     7276 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-lazy/src/tests/cse.rs
--rw-r--r--   0     1001      123    12759 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-lazy/src/tests/io.rs
--rw-r--r--   0     1001      123     4166 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-lazy/src/tests/logical.rs
--rw-r--r--   0     1001      123     4273 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-lazy/src/tests/mod.rs
--rw-r--r--   0     1001      123    15770 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-lazy/src/tests/optimization_checks.rs
--rw-r--r--   0     1001      123     6772 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-lazy/src/tests/predicate_queries.rs
--rw-r--r--   0     1001      123     3165 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-lazy/src/tests/projection_queries.rs
--rw-r--r--   0     1001      123    47687 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-lazy/src/tests/queries.rs
--rw-r--r--   0     1001      123     9519 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-lazy/src/tests/streaming.rs
--rw-r--r--   0     1001      123     2893 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-lazy/src/tests/tpch.rs
--rw-r--r--   0     1001      123     1028 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-lazy/src/utils.rs
--rw-r--r--   0        0        0     1592 1970-01-01 00:00:00.000000 polars_u64_idx-0.18.3/local_dependencies/polars-arrow/Cargo.toml
--rw-r--r--   0     1001      123     1055 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-arrow/LICENSE
--rw-r--r--   0     1001      123      144 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-arrow/README.md
--rw-r--r--   0     1001      123     1975 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-arrow/src/array/default_arrays.rs
--rw-r--r--   0     1001      123     1791 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-arrow/src/array/fixed_size_list.rs
--rw-r--r--   0     1001      123     3773 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-arrow/src/array/get.rs
--rw-r--r--   0     1001      123     6664 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-arrow/src/array/list.rs
--rw-r--r--   0     1001      123     8165 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-arrow/src/array/mod.rs
--rw-r--r--   0     1001      123      878 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-arrow/src/array/null.rs
--rw-r--r--   0     1001      123     1125 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-arrow/src/array/slice.rs
--rw-r--r--   0     1001      123     2252 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-arrow/src/array/utf8.rs
--rw-r--r--   0     1001      123     2294 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-arrow/src/bit_util.rs
--rw-r--r--   0     1001      123       17 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-arrow/src/bitmap/mod.rs
--rw-r--r--   0     1001      123      819 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-arrow/src/bitmap/mutable.rs
--rw-r--r--   0     1001      123      370 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-arrow/src/compute/arithmetics/decimal/add.rs
--rw-r--r--   0     1001      123     2181 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-arrow/src/compute/arithmetics/decimal/commutative.rs
--rw-r--r--   0     1001      123     1482 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-arrow/src/compute/arithmetics/decimal/div.rs
--rw-r--r--   0     1001      123     1028 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-arrow/src/compute/arithmetics/decimal/mod.rs
--rw-r--r--   0     1001      123     1177 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-arrow/src/compute/arithmetics/decimal/mul.rs
--rw-r--r--   0     1001      123      508 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-arrow/src/compute/arithmetics/decimal/sub.rs
--rw-r--r--   0     1001      123       51 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-arrow/src/compute/arithmetics/mod.rs
--rw-r--r--   0     1001      123        1 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-arrow/src/compute/arity.rs
--rw-r--r--   0     1001      123      727 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-arrow/src/compute/bitwise.rs
--rw-r--r--   0     1001      123     1206 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-arrow/src/compute/cast.rs
--rw-r--r--   0     1001      123     3964 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-arrow/src/compute/decimal.rs
--rw-r--r--   0     1001      123     1250 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-arrow/src/compute/mod.rs
--rw-r--r--   0     1001      123      391 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-arrow/src/compute/take/bitmap.rs
--rw-r--r--   0     1001      123     2767 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-arrow/src/compute/take/boolean.rs
--rw-r--r--   0     1001      123     3487 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-arrow/src/compute/take/fixed_size_list.rs
--rw-r--r--   0     1001      123    25289 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-arrow/src/compute/take/mod.rs
--rw-r--r--   0     1001      123      797 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-arrow/src/compute/tile.rs
--rw-r--r--   0     1001      123     1102 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-arrow/src/conversion.rs
--rw-r--r--   0     1001      123     1609 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-arrow/src/data_types.rs
--rw-r--r--   0     1001      123       25 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-arrow/src/error.rs
--rw-r--r--   0     1001      123       28 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-arrow/src/export.rs
--rw-r--r--   0     1001      123       26 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-arrow/src/floats/mod.rs
--rw-r--r--   0     1001      123     2066 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-arrow/src/floats/ord.rs
--rw-r--r--   0     1001      123     1273 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-arrow/src/index.rs
--rw-r--r--   0     1001      123      984 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-arrow/src/is_valid.rs
--rw-r--r--   0     1001      123     4783 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-arrow/src/kernels/agg_mean.rs
--rw-r--r--   0     1001      123     1074 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-arrow/src/kernels/comparison.rs
--rw-r--r--   0     1001      123     1068 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-arrow/src/kernels/concatenate.rs
--rw-r--r--   0     1001      123     5161 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-arrow/src/kernels/ewm/average.rs
--rw-r--r--   0     1001      123     1808 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-arrow/src/kernels/ewm/mod.rs
--rw-r--r--   0     1001      123    25065 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-arrow/src/kernels/ewm/variance.rs
--rw-r--r--   0     1001      123     1406 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-arrow/src/kernels/float.rs
--rw-r--r--   0     1001      123     4907 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-arrow/src/kernels/list.rs
--rw-r--r--   0     1001      123     1885 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-arrow/src/kernels/list_bytes_iter.rs
--rw-r--r--   0     1001      123     9783 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-arrow/src/kernels/mod.rs
--rw-r--r--   0     1001      123     3923 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-arrow/src/kernels/rolling/mod.rs
--rw-r--r--   0     1001      123     2019 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/mean.rs
--rw-r--r--   0     1001      123    16191 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/min_max.rs
--rw-r--r--   0     1001      123     3839 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/mod.rs
--rw-r--r--   0     1001      123    11729 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/quantile.rs
--rw-r--r--   0     1001      123     5684 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/sum.rs
--rw-r--r--   0     1001      123     9609 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/variance.rs
--rw-r--r--   0     1001      123     1879 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-arrow/src/kernels/rolling/nulls/mean.rs
--rw-r--r--   0     1001      123    14722 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-arrow/src/kernels/rolling/nulls/min_max.rs
--rw-r--r--   0     1001      123    10055 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-arrow/src/kernels/rolling/nulls/mod.rs
--rw-r--r--   0     1001      123    11643 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-arrow/src/kernels/rolling/nulls/quantile.rs
--rw-r--r--   0     1001      123     4821 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-arrow/src/kernels/rolling/nulls/sum.rs
--rw-r--r--   0     1001      123     8687 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-arrow/src/kernels/rolling/nulls/variance.rs
--rw-r--r--   0     1001      123     8109 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-arrow/src/kernels/rolling/window.rs
--rw-r--r--   0     1001      123     4752 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-arrow/src/kernels/set.rs
--rw-r--r--   0     1001      123     4529 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-arrow/src/kernels/sort_partition.rs
--rw-r--r--   0     1001      123     2948 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-arrow/src/kernels/sorted_join/inner.rs
--rw-r--r--   0     1001      123     5974 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-arrow/src/kernels/sorted_join/left.rs
--rw-r--r--   0     1001      123      231 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-arrow/src/kernels/sorted_join/mod.rs
--rw-r--r--   0     1001      123      841 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-arrow/src/kernels/string.rs
--rw-r--r--   0     1001      123     2310 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-arrow/src/kernels/take_agg/boolean.rs
--rw-r--r--   0     1001      123     4315 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-arrow/src/kernels/take_agg/mod.rs
--rw-r--r--   0     1001      123     2606 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-arrow/src/kernels/take_agg/var.rs
--rw-r--r--   0     1001      123     3672 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-arrow/src/kernels/time.rs
--rw-r--r--   0     1001      123      341 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-arrow/src/lib.rs
--rw-r--r--   0     1001      123      496 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-arrow/src/prelude.rs
--rw-r--r--   0     1001      123      534 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-arrow/src/slice.rs
--rw-r--r--   0     1001      123      183 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-arrow/src/time_zone.rs
--rw-r--r--   0     1001      123      998 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-arrow/src/trusted_len/boolean.rs
--rw-r--r--   0     1001      123     2821 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-arrow/src/trusted_len/mod.rs
--rw-r--r--   0     1001      123     2052 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-arrow/src/trusted_len/push_unchecked.rs
--rw-r--r--   0     1001      123      158 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-arrow/src/trusted_len/rev.rs
--rw-r--r--   0     1001      123     5232 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/local_dependencies/polars-arrow/src/utils.rs
--rw-r--r--   0        0        0     4403 1970-01-01 00:00:00.000000 polars_u64_idx-0.18.3/Cargo.toml
--rw-r--r--   0     1001      123       76 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/.gitignore
--rw-r--r--   0     1001      123     1055 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/LICENSE
--rw-r--r--   0     1001      123     2414 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/Makefile
--rw-r--r--   0     1001      123    11998 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/README.md
--rw-r--r--   0     1001      123      651 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/build.rs
--rw-r--r--   0     1001      123       32 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/docs/.gitignore
--rw-r--r--   0     1001      123      679 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/docs/Makefile
--rw-r--r--   0     1001      123      318 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/docs/_templates/api_redirect.html
--rw-r--r--   0     1001      123      151 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/docs/_templates/autosummary/accessor.rst
--rw-r--r--   0     1001      123      160 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/docs/_templates/autosummary/accessor_attribute.rst
--rw-r--r--   0     1001      123      168 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/docs/_templates/autosummary/accessor_callable.rst
--rw-r--r--   0     1001      123      157 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/docs/_templates/autosummary/accessor_method.rst
--rw-r--r--   0     1001      123      836 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/docs/_templates/autosummary/class.rst
--rw-r--r--   0     1001      123       94 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/docs/_templates/autosummary/class_without_autosummary.rst
--rw-r--r--   0     1001      123      406 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/docs/_templates/sidebar-nav-bs.html
--rw-r--r--   0     1001      123      491 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/docs/requirements-docs.txt
--rw-r--r--   0     1001      123     1164 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/docs/run_live_docs_server.py
--rw-r--r--   0     1001      123     1567 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/docs/source/_static/css/custom.css
--rw-r--r--   0     1001      123     7297 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/docs/source/conf.py
--rw-r--r--   0     1001      123       51 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/docs/source/index.rst
--rw-r--r--   0     1001      123     6767 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/docs/source/reference/api.rst
--rw-r--r--   0     1001      123     2069 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/docs/source/reference/config.rst
--rw-r--r--   0     1001      123      274 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/docs/source/reference/dataframe/aggregation.rst
--rw-r--r--   0     1001      123      221 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/docs/source/reference/dataframe/attributes.rst
--rw-r--r--   0     1001      123      142 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/docs/source/reference/dataframe/computation.rst
--rw-r--r--   0     1001      123      319 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/docs/source/reference/dataframe/descriptive.rst
--rw-r--r--   0     1001      123      319 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/docs/source/reference/dataframe/export.rst
--rw-r--r--   0     1001      123      464 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/docs/source/reference/dataframe/groupby.rst
--rw-r--r--   0     1001      123      379 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/docs/source/reference/dataframe/index.rst
--rw-r--r--   0     1001      123      189 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/docs/source/reference/dataframe/miscellaneous.rst
--rw-r--r--   0     1001      123     1538 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/docs/source/reference/dataframe/modify_select.rst
--rw-r--r--   0     1001      123      673 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/docs/source/reference/datatypes.rst
--rw-r--r--   0     1001      123      421 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/docs/source/reference/exceptions.rst
--rw-r--r--   0     1001      123      391 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/docs/source/reference/expressions/aggregation.rst
--rw-r--r--   0     1001      123      267 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/docs/source/reference/expressions/array.rst
--rw-r--r--   0     1001      123      309 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/docs/source/reference/expressions/binary.rst
--rw-r--r--   0     1001      123      338 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/docs/source/reference/expressions/boolean.rst
--rw-r--r--   0     1001      123      237 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/docs/source/reference/expressions/categories.rst
--rw-r--r--   0     1001      123      221 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/docs/source/reference/expressions/columns.rst
--rw-r--r--   0     1001      123     1061 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/docs/source/reference/expressions/computation.rst
--rw-r--r--   0     1001      123     1130 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/docs/source/reference/expressions/functions.rst
--rw-r--r--   0     1001      123      470 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/docs/source/reference/expressions/index.rst
--rw-r--r--   0     1001      123      722 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/docs/source/reference/expressions/list.rst
--rw-r--r--   0     1001      123      432 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/docs/source/reference/expressions/meta.rst
--rw-r--r--   0     1001      123      159 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/docs/source/reference/expressions/miscellaneous.rst
--rw-r--r--   0     1001      123      977 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/docs/source/reference/expressions/modify_select.rst
--rw-r--r--   0     1001      123      679 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/docs/source/reference/expressions/operators.rst
--rw-r--r--   0     1001      123      951 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/docs/source/reference/expressions/string.rst
--rw-r--r--   0     1001      123      254 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/docs/source/reference/expressions/struct.rst
--rw-r--r--   0     1001      123     1036 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/docs/source/reference/expressions/temporal.rst
--rw-r--r--   0     1001      123       98 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/docs/source/reference/expressions/window.rst
--rw-r--r--   0     1001      123      836 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/docs/source/reference/functions.rst
--rw-r--r--   0     1001      123      405 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/docs/source/reference/index.rst
--rw-r--r--   0     1001      123     1294 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/docs/source/reference/io.rst
--rw-r--r--   0     1001      123      277 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/docs/source/reference/lazyframe/aggregation.rst
--rw-r--r--   0     1001      123      179 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/docs/source/reference/lazyframe/attributes.rst
--rw-r--r--   0     1001      123      146 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/docs/source/reference/lazyframe/descriptive.rst
--rw-r--r--   0     1001      123      497 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/docs/source/reference/lazyframe/groupby.rst
--rw-r--r--   0     1001      123      354 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/docs/source/reference/lazyframe/index.rst
--rw-r--r--   0     1001      123      455 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/docs/source/reference/lazyframe/miscellaneous.rst
--rw-r--r--   0     1001      123     1013 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/docs/source/reference/lazyframe/modify_select.rst
--rw-r--r--   0     1001      123     3279 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/docs/source/reference/selectors.rst
--rw-r--r--   0     1001      123      358 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/docs/source/reference/series/aggregation.rst
--rw-r--r--   0     1001      123      277 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/docs/source/reference/series/array.rst
--rw-r--r--   0     1001      123      257 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/docs/source/reference/series/attributes.rst
--rw-r--r--   0     1001      123      321 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/docs/source/reference/series/binary.rst
--rw-r--r--   0     1001      123      117 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/docs/source/reference/series/boolean.rst
--rw-r--r--   0     1001      123      241 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/docs/source/reference/series/categories.rst
--rw-r--r--   0     1001      123     1103 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/docs/source/reference/series/computation.rst
--rw-r--r--   0     1001      123      744 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/docs/source/reference/series/descriptive.rst
--rw-r--r--   0     1001      123      240 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/docs/source/reference/series/export.rst
--rw-r--r--   0     1001      123      437 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/docs/source/reference/series/index.rst
--rw-r--r--   0     1001      123      776 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/docs/source/reference/series/list.rst
--rw-r--r--   0     1001      123      236 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/docs/source/reference/series/miscellaneous.rst
--rw-r--r--   0     1001      123     1077 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/docs/source/reference/series/modify_select.rst
--rw-r--r--   0     1001      123     1021 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/docs/source/reference/series/string.rst
--rw-r--r--   0     1001      123      421 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/docs/source/reference/series/struct.rst
--rw-r--r--   0     1001      123     1192 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/docs/source/reference/series/temporal.rst
--rw-r--r--   0     1001      123      503 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/docs/source/reference/sql.rst
--rw-r--r--   0     1001      123     8067 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/docs/source/reference/testing.rst
--rw-r--r--   0     1001      123      168 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/docs/source/reference/utils.rst
--rw-r--r--   0     1001      123     6161 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/polars/__init__.py
--rw-r--r--   0     1001      123      280 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/polars/_reexport.py
--rw-r--r--   0     1001      123    13229 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/polars/api.py
--rw-r--r--   0     1001      123    29763 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/polars/config.py
--rw-r--r--   0     1001      123    28105 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/polars/convert.py
--rw-r--r--   0     1001      123       77 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/polars/dataframe/__init__.py
--rw-r--r--   0     1001      123     5227 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/polars/dataframe/_html.py
--rw-r--r--   0     1001      123   316258 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/polars/dataframe/frame.py
--rw-r--r--   0     1001      123    40637 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/polars/dataframe/groupby.py
--rw-r--r--   0     1001      123     2692 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/polars/datatypes/__init__.py
--rw-r--r--   0     1001      123    16199 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/polars/datatypes/classes.py
--rw-r--r--   0     1001      123     1603 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/polars/datatypes/constants.py
--rw-r--r--   0     1001      123     4701 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/polars/datatypes/constructor.py
--rw-r--r--   0     1001      123    15739 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/polars/datatypes/convert.py
--rw-r--r--   0     1001      123     7338 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/polars/dependencies.py
--rw-r--r--   0     1001      123     3573 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/polars/exceptions.py
--rw-r--r--   0     1001      123       61 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/polars/expr/__init__.py
--rw-r--r--   0     1001      123     3020 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/polars/expr/array.py
--rw-r--r--   0     1001      123     2704 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/polars/expr/binary.py
--rw-r--r--   0     1001      123     1698 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/polars/expr/categorical.py
--rw-r--r--   0     1001      123    77648 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/polars/expr/datetime.py
--rw-r--r--   0     1001      123   261911 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/polars/expr/expr.py
--rw-r--r--   0     1001      123    23905 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/polars/expr/list.py
--rw-r--r--   0     1001      123     4050 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/polars/expr/meta.py
--rw-r--r--   0     1001      123    59014 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/polars/expr/string.py
--rw-r--r--   0     1001      123     5426 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/polars/expr/struct.py
--rw-r--r--   0     1001      123     2068 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/polars/functions/__init__.py
--rw-r--r--   0     1001      123    16541 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/polars/functions/as_datatype.py
--rw-r--r--   0     1001      123    18853 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/polars/functions/eager.py
--rw-r--r--   0     1001      123    72401 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/polars/functions/lazy.py
--rw-r--r--   0     1001      123    16227 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/polars/functions/range.py
--rw-r--r--   0     1001      123     6027 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/polars/functions/repeat.py
--rw-r--r--   0     1001      123     6139 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/polars/functions/whenthen.py
--rw-r--r--   0     1001      123      952 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/polars/io/__init__.py
--rw-r--r--   0     1001      123     6264 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/polars/io/_utils.py
--rw-r--r--   0     1001      123      861 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/polars/io/avro.py
--rw-r--r--   0     1001      123      144 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/polars/io/csv/__init__.py
--rw-r--r--   0     1001      123     1072 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/polars/io/csv/_utils.py
--rw-r--r--   0     1001      123     4681 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/polars/io/csv/batched_reader.py
--rw-r--r--   0     1001      123    35482 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/polars/io/csv/functions.py
--rw-r--r--   0     1001      123     5627 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/polars/io/database.py
--rw-r--r--   0     1001      123    11047 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/polars/io/delta.py
--rw-r--r--   0     1001      123       75 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/polars/io/excel/__init__.py
--rw-r--r--   0     1001      123    18449 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/polars/io/excel/_write_utils.py
--rw-r--r--   0     1001      123     6466 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/polars/io/excel/functions.py
--rw-r--r--   0     1001      123      142 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/polars/io/ipc/__init__.py
--rw-r--r--   0     1001      123     1227 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/polars/io/ipc/anonymous_scan.py
--rw-r--r--   0     1001      123     5804 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/polars/io/ipc/functions.py
--rw-r--r--   0     1001      123      502 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/polars/io/json.py
--rw-r--r--   0     1001      123     2207 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/polars/io/ndjson.py
--rw-r--r--   0     1001      123      170 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/polars/io/parquet/__init__.py
--rw-r--r--   0     1001      123     1259 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/polars/io/parquet/anonymous_scan.py
--rw-r--r--   0     1001      123     7177 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/polars/io/parquet/functions.py
--rw-r--r--   0     1001      123      136 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/polars/io/pyarrow_dataset/__init__.py
--rw-r--r--   0     1001      123     2291 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/polars/io/pyarrow_dataset/anonymous_scan.py
--rw-r--r--   0     1001      123     3601 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/polars/io/pyarrow_dataset/functions.py
--rw-r--r--   0     1001      123       77 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/polars/lazyframe/__init__.py
--rw-r--r--   0     1001      123   168959 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/polars/lazyframe/frame.py
--rw-r--r--   0     1001      123    24078 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/polars/lazyframe/groupby.py
--rw-r--r--   0     1001      123        0 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/polars/py.typed
--rw-r--r--   0     1001      123    32502 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/polars/selectors.py
--rw-r--r--   0     1001      123       69 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/polars/series/__init__.py
--rw-r--r--   0     1001      123     1572 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/polars/series/_numpy.py
--rw-r--r--   0     1001      123     2515 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/polars/series/array.py
--rw-r--r--   0     1001      123     1913 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/polars/series/binary.py
--rw-r--r--   0     1001      123     1692 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/polars/series/categorical.py
--rw-r--r--   0     1001      123    51825 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/polars/series/datetime.py
--rw-r--r--   0     1001      123    13196 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/polars/series/list.py
--rw-r--r--   0     1001      123   170198 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/polars/series/series.py
--rw-r--r--   0     1001      123    37808 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/polars/series/string.py
--rw-r--r--   0     1001      123     2542 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/polars/series/struct.py
--rw-r--r--   0     1001      123     5361 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/polars/series/utils.py
--rw-r--r--   0     1001      123     7559 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/polars/slice.py
--rw-r--r--   0     1001      123       75 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/polars/sql/__init__.py
--rw-r--r--   0     1001      123    17409 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/polars/sql/context.py
--rw-r--r--   0     1001      123     4793 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/polars/string_cache.py
--rw-r--r--   0     1001      123      362 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/polars/testing/__init__.py
--rw-r--r--   0     1001      123     1060 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/polars/testing/_private.py
--rw-r--r--   0     1001      123    16964 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/polars/testing/asserts.py
--rw-r--r--   0     1001      123      898 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/polars/testing/parametric/__init__.py
--rw-r--r--   0     1001      123    26833 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/polars/testing/parametric/primitives.py
--rw-r--r--   0     1001      123     3409 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/polars/testing/parametric/profiles.py
--rw-r--r--   0     1001      123    12132 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/polars/testing/parametric/strategies.py
--rw-r--r--   0     1001      123     6304 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/polars/type_aliases.py
--rw-r--r--   0     1001      123     1169 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/polars/utils/__init__.py
--rw-r--r--   0     1001      123    54302 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/polars/utils/_construction.py
--rw-r--r--   0     1001      123     3902 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/polars/utils/_parse_expr_input.py
--rw-r--r--   0     1001      123      711 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/polars/utils/_scan.py
--rw-r--r--   0     1001      123      579 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/polars/utils/_wrap.py
--rw-r--r--   0     1001      123      683 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/polars/utils/build_info.py
--rw-r--r--   0     1001      123     8609 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/polars/utils/convert.py
--rw-r--r--   0     1001      123     6132 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/polars/utils/decorators.py
--rw-r--r--   0     1001      123     1660 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/polars/utils/meta.py
--rw-r--r--   0     1001      123      514 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/polars/utils/polars_version.py
--rw-r--r--   0     1001      123     2673 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/polars/utils/show_versions.py
--rw-r--r--   0     1001      123    12905 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/polars/utils/various.py
--rw-r--r--   0     1001      123     5377 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/pyproject.toml
--rw-r--r--   0     1001      123      698 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/requirements-dev.txt
--rw-r--r--   0     1001      123       68 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/requirements-lint.txt
--rw-r--r--   0     1001      123     1640 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/scripts/check_stacklevels.py
--rw-r--r--   0     1001      123    10980 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/src/apply/dataframe.rs
--rw-r--r--   0     1001      123     7448 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/src/apply/lazy.rs
--rw-r--r--   0     1001      123     8402 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/src/apply/mod.rs
--rw-r--r--   0     1001      123    90009 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/src/apply/series.rs
--rw-r--r--   0     1001      123       32 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/src/arrow_interop/mod.rs
--rw-r--r--   0     1001      123     1306 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/src/arrow_interop/to_py.rs
--rw-r--r--   0     1001      123     3902 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/src/arrow_interop/to_rust.rs
--rw-r--r--   0     1001      123     5250 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/src/batched_csv.rs
--rw-r--r--   0     1001      123    48675 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/src/conversion.rs
--rw-r--r--   0     1001      123    45928 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/src/dataframe.rs
--rw-r--r--   0     1001      123     3950 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/src/datatypes.rs
--rw-r--r--   0     1001      123     3288 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/src/error.rs
--rw-r--r--   0     1001      123      570 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/src/expr/array.rs
--rw-r--r--   0     1001      123     2080 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/src/expr/binary.rs
--rw-r--r--   0     1001      123      274 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/src/expr/categorical.rs
--rw-r--r--   0     1001      123     5935 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/src/expr/datetime.rs
--rw-r--r--   0     1001      123    34040 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/src/expr/general.rs
--rw-r--r--   0     1001      123     3937 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/src/expr/list.rs
--rw-r--r--   0     1001      123     2907 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/src/expr/meta.rs
--rw-r--r--   0     1001      123      870 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/src/expr/mod.rs
--rw-r--r--   0     1001      123     8677 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/src/expr/string.rs
--rw-r--r--   0     1001      123      467 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/src/expr/struct.rs
--rw-r--r--   0     1001      123     9482 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/src/file.rs
--rw-r--r--   0     1001      123     3307 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/src/functions/eager.rs
--rw-r--r--   0     1001      123     1657 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/src/functions/io.rs
--rw-r--r--   0     1001      123    11977 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/src/functions/lazy.rs
--rw-r--r--   0     1001      123     1312 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/src/functions/meta.rs
--rw-r--r--   0     1001      123      217 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/src/functions/misc.rs
--rw-r--r--   0     1001      123       87 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/src/functions/mod.rs
--rw-r--r--   0     1001      123     1474 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/src/functions/whenthen.rs
--rw-r--r--   0     1001      123    30767 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/src/lazyframe.rs
--rw-r--r--   0     1001      123     2670 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/src/lazygroupby.rs
--rw-r--r--   0     1001      123     8268 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/src/lib.rs
--rw-r--r--   0     1001      123     1029 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/src/object.rs
--rw-r--r--   0     1001      123      122 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/src/prelude.rs
--rw-r--r--   0     1001      123      435 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/src/py_modules.rs
--rw-r--r--   0     1001      123     1964 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/src/series/aggregation.rs
--rw-r--r--   0     1001      123     5406 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/src/series/arithmetic.rs
--rw-r--r--   0     1001      123     5138 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/src/series/comparison.rs
--rw-r--r--   0     1001      123     9077 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/src/series/construction.rs
--rw-r--r--   0     1001      123     8971 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/src/series/export.rs
--rw-r--r--   0     1001      123    26521 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/src/series/mod.rs
--rw-r--r--   0     1001      123     4569 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/src/series/numpy_ufunc.rs
--rw-r--r--   0     1001      123     4046 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/src/series/set_at_idx.rs
--rw-r--r--   0     1001      123     1036 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/src/sql.rs
--rw-r--r--   0     1001      123     2335 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/src/utils.rs
--rw-r--r--   0     1001      123     6165 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/tests/README.md
--rw-r--r--   0     1001      123     2189 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/tests/benchmark/groupby-datagen.R
--rw-r--r--   0     1001      123     7963 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/tests/benchmark/run_h2oai_benchmark.py
--rw-r--r--   0     1001      123     6530 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/tests/benchmark/test_release.py
--rw-r--r--   0     1001      123     4589 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/tests/docs/run_doctest.py
--rw-r--r--   0     1001      123      179 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/tests/parametric/conftest.py
--rw-r--r--   0     1001      123     3856 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/tests/parametric/test_dataframe.py
--rw-r--r--   0     1001      123     1692 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/tests/parametric/test_lazyframe.py
--rw-r--r--   0     1001      123     6897 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/tests/parametric/test_series.py
--rw-r--r--   0     1001      123     8299 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/tests/parametric/test_testing.py
--rw-r--r--   0     1001      123        0 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/tests/unit/__init__.py
--rw-r--r--   0     1001      123     3382 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/tests/unit/conftest.py
--rw-r--r--   0     1001      123       86 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/tests/unit/datatypes/__init__.py
--rw-r--r--   0     1001      123      973 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/tests/unit/datatypes/test_array.py
--rw-r--r--   0     1001      123      847 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/tests/unit/datatypes/test_binary.py
--rw-r--r--   0     1001      123     1420 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/tests/unit/datatypes/test_bool.py
--rw-r--r--   0     1001      123    13228 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/tests/unit/datatypes/test_categorical.py
--rw-r--r--   0     1001      123     5222 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/tests/unit/datatypes/test_decimal.py
--rw-r--r--   0     1001      123      549 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/tests/unit/datatypes/test_duration.py
--rw-r--r--   0     1001      123      423 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/tests/unit/datatypes/test_integer.py
--rw-r--r--   0     1001      123    13216 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/tests/unit/datatypes/test_list.py
--rw-r--r--   0     1001      123      284 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/tests/unit/datatypes/test_null.py
--rw-r--r--   0     1001      123     2801 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/tests/unit/datatypes/test_object.py
--rw-r--r--   0     1001      123    27749 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/tests/unit/datatypes/test_struct.py
--rw-r--r--   0     1001      123    87949 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/tests/unit/datatypes/test_temporal.py
--rw-r--r--   0     1001      123      418 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/tests/unit/datatypes/test_time.py
--rw-r--r--   0     1001      123        0 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/tests/unit/functions/__init__.py
--rw-r--r--   0     1001      123    13970 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/tests/unit/functions/test_as_datatype.py
--rw-r--r--   0     1001      123      480 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/tests/unit/functions/test_concat.py
--rw-r--r--   0     1001      123    15610 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/tests/unit/functions/test_functions.py
--rw-r--r--   0     1001      123    18470 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/tests/unit/functions/test_range.py
--rw-r--r--   0     1001      123     3724 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/tests/unit/functions/test_repeat.py
--rw-r--r--   0     1001      123      218 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/tests/unit/io/conftest.py
--rw-r--r--   0     1001      123       16 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/tests/unit/io/files/delta-table/.part-00000-e42312d7-60e5-454d-acbc-db192d220e73-c000.snappy.parquet.crc
--rw-r--r--   0     1001      123       16 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/tests/unit/io/files/delta-table/.part-00000-e4a999da-df45-4fb0-bdc4-d999fc0f58aa-c000.snappy.parquet.crc
--rw-r--r--   0     1001      123       16 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/tests/unit/io/files/delta-table/_delta_log/.00000000000000000000.json.crc
--rw-r--r--   0     1001      123       16 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/tests/unit/io/files/delta-table/_delta_log/.00000000000000000001.json.crc
--rw-r--r--   0     1001      123      905 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/tests/unit/io/files/delta-table/_delta_log/00000000000000000000.json
--rw-r--r--   0     1001      123      936 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/tests/unit/io/files/delta-table/_delta_log/00000000000000000001.json
--rw-r--r--   0     1001      123      972 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/tests/unit/io/files/delta-table/part-00000-e42312d7-60e5-454d-acbc-db192d220e73-c000.snappy.parquet
--rw-r--r--   0     1001      123      690 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/tests/unit/io/files/delta-table/part-00000-e4a999da-df45-4fb0-bdc4-d999fc0f58aa-c000.snappy.parquet
--rw-r--r--   0     1001      123        0 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/tests/unit/io/files/empty.csv
--rw-r--r--   0     1001      123     5959 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/tests/unit/io/files/example.xlsx
--rw-r--r--   0     1001      123      457 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/tests/unit/io/files/foods1.csv
--rw-r--r--   0     1001      123     2351 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/tests/unit/io/files/foods1.ipc
--rw-r--r--   0     1001      123     1713 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/tests/unit/io/files/foods1.ndjson
--rw-r--r--   0     1001      123     1427 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/tests/unit/io/files/foods1.parquet
--rw-r--r--   0     1001      123      455 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/tests/unit/io/files/foods2.csv
--rw-r--r--   0     1001      123     2351 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/tests/unit/io/files/foods2.ipc
--rw-r--r--   0     1001      123     1711 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/tests/unit/io/files/foods2.ndjson
--rw-r--r--   0     1001      123     1916 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/tests/unit/io/files/foods2.parquet
--rw-r--r--   0     1001      123      455 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/tests/unit/io/files/foods3.csv
--rw-r--r--   0     1001      123      457 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/tests/unit/io/files/foods4.csv
--rw-r--r--   0     1001      123      452 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/tests/unit/io/files/foods5.csv
--rw-r--r--   0     1001      123       49 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/tests/unit/io/files/gzipped.csv
--rw-r--r--   0     1001      123       57 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/tests/unit/io/files/small.csv
--rw-r--r--   0     1001      123      756 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/tests/unit/io/files/small.parquet
--rw-r--r--   0     1001      123     1884 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/tests/unit/io/test_avro.py
--rw-r--r--   0     1001      123    39230 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/tests/unit/io/test_csv.py
--rw-r--r--   0     1001      123     6336 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/tests/unit/io/test_database.py
--rw-r--r--   0     1001      123     6172 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/tests/unit/io/test_delta.py
--rw-r--r--   0     1001      123    11169 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/tests/unit/io/test_excel.py
--rw-r--r--   0     1001      123     5483 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/tests/unit/io/test_ipc.py
--rw-r--r--   0     1001      123     3986 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/tests/unit/io/test_json.py
--rw-r--r--   0     1001      123     7379 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/tests/unit/io/test_lazy_csv.py
--rw-r--r--   0     1001      123     2060 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/tests/unit/io/test_lazy_ipc.py
--rw-r--r--   0     1001      123     2867 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/tests/unit/io/test_lazy_json.py
--rw-r--r--   0     1001      123    11145 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/tests/unit/io/test_lazy_parquet.py
--rw-r--r--   0     1001      123     2012 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/tests/unit/io/test_other.py
--rw-r--r--   0     1001      123    14201 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/tests/unit/io/test_parquet.py
--rw-r--r--   0     1001      123      612 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/tests/unit/io/test_pickle.py
--rw-r--r--   0     1001      123     3686 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/tests/unit/io/test_pyarrow_dataset.py
--rw-r--r--   0     1001      123      509 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/tests/unit/namespaces/__init__.py
--rw-r--r--   0     1001      123      589 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/tests/unit/namespaces/test_array.py
--rw-r--r--   0     1001      123     3218 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/tests/unit/namespaces/test_binary.py
--rw-r--r--   0     1001      123     2489 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/tests/unit/namespaces/test_categorical.py
--rw-r--r--   0     1001      123    19585 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/tests/unit/namespaces/test_datetime.py
--rw-r--r--   0     1001      123    14067 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/tests/unit/namespaces/test_list.py
--rw-r--r--   0     1001      123     1829 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/tests/unit/namespaces/test_meta.py
--rw-r--r--   0     1001      123    23544 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/tests/unit/namespaces/test_string.py
--rw-r--r--   0     1001      123    17964 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/tests/unit/namespaces/test_strptime.py
--rw-r--r--   0     1001      123      982 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/tests/unit/namespaces/test_struct.py
--rw-r--r--   0     1001      123       85 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/tests/unit/operations/__init__.py
--rw-r--r--   0     1001      123     7755 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/tests/unit/operations/test_aggregations.py
--rw-r--r--   0     1001      123    10643 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/tests/unit/operations/test_apply.py
--rw-r--r--   0     1001      123     6932 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/tests/unit/operations/test_arithmetic.py
--rw-r--r--   0     1001      123     4631 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/tests/unit/operations/test_comparison.py
--rw-r--r--   0     1001      123     3275 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/tests/unit/operations/test_drop.py
--rw-r--r--   0     1001      123     8813 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/tests/unit/operations/test_explode.py
--rw-r--r--   0     1001      123     3664 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/tests/unit/operations/test_filter.py
--rw-r--r--   0     1001      123     1801 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/tests/unit/operations/test_folds.py
--rw-r--r--   0     1001      123    24998 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/tests/unit/operations/test_groupby.py
--rw-r--r--   0     1001      123     7649 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/tests/unit/operations/test_groupby_rolling.py
--rw-r--r--   0     1001      123     2983 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/tests/unit/operations/test_is_in.py
--rw-r--r--   0     1001      123    18169 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/tests/unit/operations/test_join.py
--rw-r--r--   0     1001      123    14952 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/tests/unit/operations/test_join_asof.py
--rw-r--r--   0     1001      123      643 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/tests/unit/operations/test_melt.py
--rw-r--r--   0     1001      123    10253 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/tests/unit/operations/test_pivot.py
--rw-r--r--   0     1001      123    19818 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/tests/unit/operations/test_rolling.py
--rw-r--r--   0     1001      123     1917 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/tests/unit/operations/test_select.py
--rw-r--r--   0     1001      123    20731 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/tests/unit/operations/test_sort.py
--rw-r--r--   0     1001      123     4273 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/tests/unit/operations/test_statistics.py
--rw-r--r--   0     1001      123     4130 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/tests/unit/operations/test_transpose.py
--rw-r--r--   0     1001      123      771 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/tests/unit/operations/test_unique.py
--rw-r--r--   0     1001      123    11694 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/tests/unit/operations/test_window.py
--rw-r--r--   0     1001      123     5401 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/tests/unit/operations/test_with_columns.py
--rw-r--r--   0     1001      123        0 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/tests/unit/streaming/__init__.py
--rw-r--r--   0     1001      123      196 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/tests/unit/streaming/conftest.py
--rw-r--r--   0     1001      123      908 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/tests/unit/streaming/test_ooc.py
--rw-r--r--   0     1001      123    16944 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/tests/unit/streaming/test_streaming.py
--rw-r--r--   0     1001      123     4775 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/tests/unit/test_api.py
--rw-r--r--   0     1001      123     1969 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/tests/unit/test_arity.py
--rw-r--r--   0     1001      123    20333 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/tests/unit/test_cfg.py
--rw-r--r--   0     1001      123    42513 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/tests/unit/test_constructors.py
--rw-r--r--   0     1001      123      454 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/tests/unit/test_context.py
--rw-r--r--   0     1001      123     1628 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/tests/unit/test_cse.py
--rw-r--r--   0     1001      123     5198 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/tests/unit/test_datatypes.py
--rw-r--r--   0     1001      123   119414 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/tests/unit/test_df.py
--rw-r--r--   0     1001      123     2396 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/tests/unit/test_empty.py
--rw-r--r--   0     1001      123    18809 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/tests/unit/test_errors.py
--rw-r--r--   0     1001      123     2741 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/tests/unit/test_expr_multi_cols.py
--rw-r--r--   0     1001      123    34736 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/tests/unit/test_exprs.py
--rw-r--r--   0     1001      123     3516 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/tests/unit/test_fmt.py
--rw-r--r--   0     1001      123     3763 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/tests/unit/test_interchange.py
--rw-r--r--   0     1001      123    38286 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/tests/unit/test_interop.py
--rw-r--r--   0     1001      123    47730 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/tests/unit/test_lazy.py
--rw-r--r--   0     1001      123     2463 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/tests/unit/test_polars_import.py
--rw-r--r--   0     1001      123     4610 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/tests/unit/test_predicates.py
--rw-r--r--   0     1001      123     7073 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/tests/unit/test_projections.py
--rw-r--r--   0     1001      123    11551 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/tests/unit/test_queries.py
--rw-r--r--   0     1001      123     4743 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/tests/unit/test_rows.py
--rw-r--r--   0     1001      123    13987 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/tests/unit/test_schema.py
--rw-r--r--   0     1001      123     7419 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/tests/unit/test_selectors.py
--rw-r--r--   0     1001      123     2823 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/tests/unit/test_serde.py
--rw-r--r--   0     1001      123    83729 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/tests/unit/test_series.py
--rw-r--r--   0     1001      123      657 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/tests/unit/test_single.py
--rw-r--r--   0     1001      123    10068 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/tests/unit/test_sql.py
--rw-r--r--   0     1001      123    35314 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/tests/unit/test_testing.py
--rw-r--r--   0     1001      123       41 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/tests/unit/utils/__init__.py
--rw-r--r--   0     1001      123      306 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/tests/unit/utils/test_build_info.py
--rw-r--r--   0     1001      123     2784 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/tests/unit/utils/test_parse_expr_input.py
--rw-r--r--   0     1001      123      247 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/tests/unit/utils/test_show_versions.py
--rw-r--r--   0     1001      123     5026 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/tests/unit/utils/test_utils.py
--rw-r--r--   0     1001      123    63894 2023-06-16 12:30:57.000000 polars_u64_idx-0.18.3/Cargo.lock
--rw-r--r--   0        0        0    14545 1970-01-01 00:00:00.000000 polars_u64_idx-0.18.3/PKG-INFO
+-rw-r--r--   0        0        0     1353 1970-01-01 00:00:00.000000 polars_u64_idx-0.18.4/local_dependencies/polars-json/Cargo.toml
+-rw-r--r--   0     1001      123     1055 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-json/LICENSE
+-rw-r--r--   0     1001      123    16770 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-json/src/json/deserialize.rs
+-rw-r--r--   0     1001      123     6564 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-json/src/json/infer_schema.rs
+-rw-r--r--   0     1001      123      189 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-json/src/json/mod.rs
+-rw-r--r--   0     1001      123       30 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-json/src/lib.rs
+-rw-r--r--   0     1001      123     1198 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-json/src/ndjson/deserialize.rs
+-rw-r--r--   0     1001      123     4828 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-json/src/ndjson/file.rs
+-rw-r--r--   0     1001      123      143 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-json/src/ndjson/mod.rs
+-rw-r--r--   0        0        0      894 1970-01-01 00:00:00.000000 polars_u64_idx-0.18.4/local_dependencies/polars-error/Cargo.toml
+-rw-r--r--   0     1001      123     1055 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-error/LICENSE
+-rw-r--r--   0     1001      123      145 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-error/README.md
+-rw-r--r--   0     1001      123     6719 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-error/src/lib.rs
+-rw-r--r--   0        0        0     5291 1970-01-01 00:00:00.000000 polars_u64_idx-0.18.4/local_dependencies/polars-plan/Cargo.toml
+-rw-r--r--   0     1001      123     1055 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-plan/LICENSE
+-rw-r--r--   0     1001      123       45 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/constants.rs
+-rw-r--r--   0     1001      123    17253 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/dot.rs
+-rw-r--r--   0     1001      123     4789 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/dsl/arithmetic.rs
+-rw-r--r--   0     1001      123     3992 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/dsl/arity.rs
+-rw-r--r--   0     1001      123     1278 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/dsl/array.rs
+-rw-r--r--   0     1001      123      935 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/dsl/binary.rs
+-rw-r--r--   0     1001      123      650 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/dsl/cat.rs
+-rw-r--r--   0     1001      123    10232 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/dsl/dt.rs
+-rw-r--r--   0     1001      123     9542 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/dsl/expr.rs
+-rw-r--r--   0     1001      123     8359 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/dsl/expr_dyn_fn.rs
+-rw-r--r--   0     1001      123      753 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/dsl/from.rs
+-rw-r--r--   0     1001      123       85 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/dsl/function_expr/abs.rs
+-rw-r--r--   0     1001      123     1431 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/dsl/function_expr/arg_where.rs
+-rw-r--r--   0     1001      123     1074 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/dsl/function_expr/array.rs
+-rw-r--r--   0     1001      123     1327 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/dsl/function_expr/binary.rs
+-rw-r--r--   0     1001      123     4221 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/dsl/function_expr/boolean.rs
+-rw-r--r--   0     1001      123     1910 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/dsl/function_expr/bounds.rs
+-rw-r--r--   0     1001      123     1216 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/dsl/function_expr/cat.rs
+-rw-r--r--   0     1001      123      344 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/dsl/function_expr/clip.rs
+-rw-r--r--   0     1001      123      257 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/dsl/function_expr/concat.rs
+-rw-r--r--   0     1001      123     6125 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/dsl/function_expr/correlation.rs
+-rw-r--r--   0     1001      123     1593 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/dsl/function_expr/cum.rs
+-rw-r--r--   0     1001      123    10067 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/dsl/function_expr/datetime.rs
+-rw-r--r--   0     1001      123      782 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/dsl/function_expr/dispatch.rs
+-rw-r--r--   0     1001      123     2567 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/dsl/function_expr/fill_null.rs
+-rw-r--r--   0     1001      123      992 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/dsl/function_expr/fused.rs
+-rw-r--r--   0     1001      123     8119 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/dsl/function_expr/list.rs
+-rw-r--r--   0     1001      123      581 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/dsl/function_expr/log.rs
+-rw-r--r--   0     1001      123    21448 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/dsl/function_expr/mod.rs
+-rw-r--r--   0     1001      123      462 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/dsl/function_expr/nan.rs
+-rw-r--r--   0     1001      123     3132 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/dsl/function_expr/pow.rs
+-rw-r--r--   0     1001      123      152 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/dsl/function_expr/rolling.rs
+-rw-r--r--   0     1001      123      260 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/dsl/function_expr/round.rs
+-rw-r--r--   0     1001      123      200 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/dsl/function_expr/row_hash.rs
+-rw-r--r--   0     1001      123    14678 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/dsl/function_expr/schema.rs
+-rw-r--r--   0     1001      123      306 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/dsl/function_expr/search_sorted.rs
+-rw-r--r--   0     1001      123     3812 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/dsl/function_expr/shift_and_fill.rs
+-rw-r--r--   0     1001      123     1238 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/dsl/function_expr/shrink_type.rs
+-rw-r--r--   0     1001      123      972 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/dsl/function_expr/sign.rs
+-rw-r--r--   0     1001      123    22249 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/dsl/function_expr/strings.rs
+-rw-r--r--   0     1001      123     1017 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/dsl/function_expr/struct_.rs
+-rw-r--r--   0     1001      123     5509 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/dsl/function_expr/temporal.rs
+-rw-r--r--   0     1001      123     6112 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/dsl/function_expr/trigonometry.rs
+-rw-r--r--   0     1001      123      170 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/dsl/function_expr/unique.rs
+-rw-r--r--   0     1001      123     1155 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/dsl/functions/arity.rs
+-rw-r--r--   0     1001      123      611 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/dsl/functions/coerce.rs
+-rw-r--r--   0     1001      123     2717 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/dsl/functions/concat.rs
+-rw-r--r--   0     1001      123     4525 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/dsl/functions/correlation.rs
+-rw-r--r--   0     1001      123     8736 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/dsl/functions/horizontal.rs
+-rw-r--r--   0     1001      123     1044 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/dsl/functions/index.rs
+-rw-r--r--   0     1001      123      968 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/dsl/functions/mod.rs
+-rw-r--r--   0     1001      123     9827 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/dsl/functions/range.rs
+-rw-r--r--   0     1001      123     1308 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/dsl/functions/selectors.rs
+-rw-r--r--   0     1001      123     1973 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/dsl/functions/syntactic_sugar.rs
+-rw-r--r--   0     1001      123    11328 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/dsl/functions/temporal.rs
+-rw-r--r--   0     1001      123    10213 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/dsl/list.rs
+-rw-r--r--   0     1001      123     3772 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/dsl/meta.rs
+-rw-r--r--   0     1001      123    61502 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/dsl/mod.rs
+-rw-r--r--   0     1001      123       40 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/dsl/names.rs
+-rw-r--r--   0     1001      123     2658 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/dsl/options.rs
+-rw-r--r--   0     1001      123     6632 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/dsl/python_udf.rs
+-rw-r--r--   0     1001      123     1068 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/dsl/selector.rs
+-rw-r--r--   0     1001      123    17626 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/dsl/string.rs
+-rw-r--r--   0     1001      123     2715 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/dsl/struct_.rs
+-rw-r--r--   0     1001      123       38 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/frame/mod.rs
+-rw-r--r--   0     1001      123      933 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/frame/opt_state.rs
+-rw-r--r--   0     1001      123      466 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/global.rs
+-rw-r--r--   0     1001      123      175 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/lib.rs
+-rw-r--r--   0     1001      123     8318 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/logical_plan/aexpr/mod.rs
+-rw-r--r--   0     1001      123    11920 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/logical_plan/aexpr/schema.rs
+-rw-r--r--   0     1001      123    25683 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/logical_plan/alp.rs
+-rw-r--r--   0     1001      123     1622 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/logical_plan/anonymous_scan.rs
+-rw-r--r--   0     1001      123     1428 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/logical_plan/apply.rs
+-rw-r--r--   0     1001      123    24898 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/logical_plan/builder.rs
+-rw-r--r--   0     1001      123    29993 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/logical_plan/conversion.rs
+-rw-r--r--   0     1001      123      301 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/logical_plan/debug.rs
+-rw-r--r--   0     1001      123    15470 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/logical_plan/format.rs
+-rw-r--r--   0     1001      123      895 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/logical_plan/functions/drop.rs
+-rw-r--r--   0     1001      123      137 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/logical_plan/functions/explode.rs
+-rw-r--r--   0     1001      123     1169 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/logical_plan/functions/merge_sorted.rs
+-rw-r--r--   0     1001      123    11905 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/logical_plan/functions/mod.rs
+-rw-r--r--   0     1001      123     1330 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/logical_plan/functions/rename.rs
+-rw-r--r--   0     1001      123    10140 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/logical_plan/iterator.rs
+-rw-r--r--   0     1001      123    10559 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/logical_plan/lit.rs
+-rw-r--r--   0     1001      123     8072 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/logical_plan/mod.rs
+-rw-r--r--   0     1001      123     7416 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/logical_plan/optimizer/cache_states.rs
+-rw-r--r--   0     1001      123    15277 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/logical_plan/optimizer/cse.rs
+-rw-r--r--   0     1001      123     2889 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/logical_plan/optimizer/delay_rechunk.rs
+-rw-r--r--   0     1001      123     3236 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/logical_plan/optimizer/drop_nulls.rs
+-rw-r--r--   0     1001      123     3994 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/logical_plan/optimizer/fast_projection.rs
+-rw-r--r--   0     1001      123    14479 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/logical_plan/optimizer/file_caching.rs
+-rw-r--r--   0     1001      123     1556 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/logical_plan/optimizer/flatten_union.rs
+-rw-r--r--   0     1001      123     6017 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/logical_plan/optimizer/fused.rs
+-rw-r--r--   0     1001      123     6774 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/logical_plan/optimizer/mod.rs
+-rw-r--r--   0     1001      123     1222 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/logical_plan/optimizer/predicate_pushdown/keys.rs
+-rw-r--r--   0     1001      123    28901 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/logical_plan/optimizer/predicate_pushdown/mod.rs
+-rw-r--r--   0     1001      123     2571 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/logical_plan/optimizer/predicate_pushdown/rename.rs
+-rw-r--r--   0     1001      123    15756 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/logical_plan/optimizer/predicate_pushdown/utils.rs
+-rw-r--r--   0     1001      123     1755 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/functions/melt.rs
+-rw-r--r--   0     1001      123     3930 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/functions/mod.rs
+-rw-r--r--   0     1001      123     1799 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/generic.rs
+-rw-r--r--   0     1001      123     3269 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/groupby.rs
+-rw-r--r--   0     1001      123     2638 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/hstack.rs
+-rw-r--r--   0     1001      123    15752 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/joins.rs
+-rw-r--r--   0     1001      123    26507 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/mod.rs
+-rw-r--r--   0     1001      123     3707 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/projection.rs
+-rw-r--r--   0     1001      123     2639 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/rename.rs
+-rw-r--r--   0     1001      123     3501 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/semi_anti_join.rs
+-rw-r--r--   0     1001      123    27269 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/logical_plan/optimizer/simplify_expr.rs
+-rw-r--r--   0     1001      123     3492 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/logical_plan/optimizer/slice_pushdown_expr.rs
+-rw-r--r--   0     1001      123    13232 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/logical_plan/optimizer/slice_pushdown_lp.rs
+-rw-r--r--   0     1001      123     4181 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/logical_plan/optimizer/stack_opt.rs
+-rw-r--r--   0     1001      123     9725 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/logical_plan/optimizer/type_coercion/binary.rs
+-rw-r--r--   0     1001      123    20215 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/logical_plan/optimizer/type_coercion/mod.rs
+-rw-r--r--   0     1001      123    10585 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/logical_plan/options.rs
+-rw-r--r--   0     1001      123    18601 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/logical_plan/projection.rs
+-rw-r--r--   0     1001      123     6144 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/logical_plan/pyarrow.rs
+-rw-r--r--   0     1001      123    13026 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/logical_plan/schema.rs
+-rw-r--r--   0     1001      123      832 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/prelude.rs
+-rw-r--r--   0     1001      123    12428 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/utils.rs
+-rw-r--r--   0        0        0     5484 1970-01-01 00:00:00.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/Cargo.toml
+-rw-r--r--   0     1001      123     1055 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/LICENSE
+-rw-r--r--   0     1001      123      144 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/README.md
+-rw-r--r--   0     1001      123     5158 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/arithmetic/decimal.rs
+-rw-r--r--   0     1001      123     8275 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/arithmetic/mod.rs
+-rw-r--r--   0     1001      123     9417 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/arithmetic/numeric.rs
+-rw-r--r--   0     1001      123     3588 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/array/iterator.rs
+-rw-r--r--   0     1001      123     2551 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/array/mod.rs
+-rw-r--r--   0     1001      123     6448 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/bitwise.rs
+-rw-r--r--   0     1001      123     2298 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/builder/binary.rs
+-rw-r--r--   0     1001      123     1207 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/builder/boolean.rs
+-rw-r--r--   0     1001      123     4311 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/builder/fixed_size_list.rs
+-rw-r--r--   0     1001      123     1556 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/builder/from.rs
+-rw-r--r--   0     1001      123    20366 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/builder/list.rs
+-rw-r--r--   0     1001      123     8969 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/builder/mod.rs
+-rw-r--r--   0     1001      123     1410 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/builder/primitive.rs
+-rw-r--r--   0     1001      123     2291 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/builder/utf8.rs
+-rw-r--r--   0     1001      123    16475 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/cast.rs
+-rw-r--r--   0     1001      123    49461 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/comparison/mod.rs
+-rw-r--r--   0     1001      123    10060 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/comparison/scalar.rs
+-rw-r--r--   0     1001      123      551 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/drop.rs
+-rw-r--r--   0     1001      123      963 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/float.rs
+-rw-r--r--   0     1001      123     7175 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/from.rs
+-rw-r--r--   0     1001      123    42339 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/iterator/mod.rs
+-rw-r--r--   0     1001      123     1453 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/iterator/par/list.rs
+-rw-r--r--   0     1001      123       28 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/iterator/par/mod.rs
+-rw-r--r--   0     1001      123     1129 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/iterator/par/utf8.rs
+-rw-r--r--   0     1001      123       21 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/kernels/mod.rs
+-rw-r--r--   0     1001      123     2347 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/kernels/take.rs
+-rw-r--r--   0     1001      123     7963 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/list/iterator.rs
+-rw-r--r--   0     1001      123     3242 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/list/mod.rs
+-rw-r--r--   0     1001      123    19831 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/logical/categorical/builder.rs
+-rw-r--r--   0     1001      123     3688 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/logical/categorical/from.rs
+-rw-r--r--   0     1001      123     4270 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/logical/categorical/merge.rs
+-rw-r--r--   0     1001      123    10219 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/logical/categorical/mod.rs
+-rw-r--r--   0     1001      123     1400 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/append.rs
+-rw-r--r--   0     1001      123      358 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/full.rs
+-rw-r--r--   0     1001      123      192 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/mod.rs
+-rw-r--r--   0     1001      123     2731 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/take_random.rs
+-rw-r--r--   0     1001      123     2172 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/unique.rs
+-rw-r--r--   0     1001      123      925 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/zip.rs
+-rw-r--r--   0     1001      123     6417 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/logical/categorical/stringcache.rs
+-rw-r--r--   0     1001      123     1604 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/logical/date.rs
+-rw-r--r--   0     1001      123     4105 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/logical/datetime.rs
+-rw-r--r--   0     1001      123     4443 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/logical/decimal.rs
+-rw-r--r--   0     1001      123     2434 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/logical/duration.rs
+-rw-r--r--   0     1001      123     2556 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/logical/mod.rs
+-rw-r--r--   0     1001      123      476 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/logical/struct_/from.rs
+-rw-r--r--   0     1001      123    15983 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/logical/struct_/mod.rs
+-rw-r--r--   0     1001      123     1182 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/logical/time.rs
+-rw-r--r--   0     1001      123    23489 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/mod.rs
+-rw-r--r--   0     1001      123     7200 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/ndarray.rs
+-rw-r--r--   0     1001      123     4484 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/object/builder.rs
+-rw-r--r--   0     1001      123     1547 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/object/extension/drop.rs
+-rw-r--r--   0     1001      123     3124 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/object/extension/list.rs
+-rw-r--r--   0     1001      123     7054 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/object/extension/mod.rs
+-rw-r--r--   0     1001      123     3410 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/object/extension/polars_extension.rs
+-rw-r--r--   0     1001      123      137 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/object/is_valid.rs
+-rw-r--r--   0     1001      123     4419 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/object/iterator.rs
+-rw-r--r--   0     1001      123     4806 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/object/mod.rs
+-rw-r--r--   0     1001      123     2956 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/object/registry.rs
+-rw-r--r--   0     1001      123      272 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/ops/abs.rs
+-rw-r--r--   0     1001      123    32691 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/ops/aggregate/mod.rs
+-rw-r--r--   0     1001      123    10025 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/ops/aggregate/quantile.rs
+-rw-r--r--   0     1001      123     2880 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/ops/aggregate/var.rs
+-rw-r--r--   0     1001      123    10551 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/ops/any_value.rs
+-rw-r--r--   0     1001      123     4526 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/ops/append.rs
+-rw-r--r--   0     1001      123    28257 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/ops/apply.rs
+-rw-r--r--   0     1001      123    12799 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/ops/bit_repr.rs
+-rw-r--r--   0     1001      123     6236 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/ops/chunkops.rs
+-rw-r--r--   0     1001      123    11537 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/ops/compare_inner.rs
+-rw-r--r--   0     1001      123     1737 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/ops/concat_str.rs
+-rw-r--r--   0     1001      123     4801 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/ops/cum_agg.rs
+-rw-r--r--   0     1001      123      908 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/ops/decimal.rs
+-rw-r--r--   0     1001      123     7056 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/ops/downcast.rs
+-rw-r--r--   0     1001      123    19462 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/ops/explode.rs
+-rw-r--r--   0     1001      123     8691 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/ops/explode_and_offsets.rs
+-rw-r--r--   0     1001      123     9103 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/ops/extend.rs
+-rw-r--r--   0     1001      123    13777 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/ops/fill_null.rs
+-rw-r--r--   0     1001      123     6356 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/ops/filter.rs
+-rw-r--r--   0     1001      123     5876 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/ops/full.rs
+-rw-r--r--   0     1001      123        1 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/ops/interpolate.rs
+-rw-r--r--   0     1001      123    16797 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/ops/is_in.rs
+-rw-r--r--   0     1001      123        1 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/ops/len.rs
+-rw-r--r--   0     1001      123     2658 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/ops/min_max_binary.rs
+-rw-r--r--   0     1001      123    23276 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/ops/mod.rs
+-rw-r--r--   0     1001      123     2414 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/ops/nulls.rs
+-rw-r--r--   0     1001      123      593 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/ops/peaks.rs
+-rw-r--r--   0     1001      123     4375 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/ops/repeat_by.rs
+-rw-r--r--   0     1001      123     2771 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/ops/reverse.rs
+-rw-r--r--   0     1001      123    10267 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/ops/rolling_window.rs
+-rw-r--r--   0     1001      123    12518 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/ops/set.rs
+-rw-r--r--   0     1001      123     7391 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/ops/shift.rs
+-rw-r--r--   0     1001      123     2299 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/ops/sort/arg_sort.rs
+-rw-r--r--   0     1001      123     5528 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/ops/sort/arg_sort_multiple.rs
+-rw-r--r--   0     1001      123     7543 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/ops/sort/categorical.rs
+-rw-r--r--   0     1001      123    31165 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/ops/sort/mod.rs
+-rw-r--r--   0     1001      123      380 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/ops/sort/slice.rs
+-rw-r--r--   0     1001      123    22089 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/ops/take/mod.rs
+-rw-r--r--   0     1001      123     7848 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/ops/take/take_chunked.rs
+-rw-r--r--   0     1001      123      301 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/ops/take/take_every.rs
+-rw-r--r--   0     1001      123    16256 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/ops/take/take_random.rs
+-rw-r--r--   0     1001      123     6275 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/ops/take/take_single.rs
+-rw-r--r--   0     1001      123     6072 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/ops/take/traits.rs
+-rw-r--r--   0     1001      123      459 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/ops/tile.rs
+-rw-r--r--   0     1001      123    11626 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/ops/unique/mod.rs
+-rw-r--r--   0     1001      123    14620 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/ops/unique/rank.rs
+-rw-r--r--   0     1001      123     5846 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/ops/zip.rs
+-rw-r--r--   0     1001      123     9093 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/random.rs
+-rw-r--r--   0     1001      123     1875 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/temporal/conversion.rs
+-rw-r--r--   0     1001      123     2826 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/temporal/date.rs
+-rw-r--r--   0     1001      123    10497 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/temporal/datetime.rs
+-rw-r--r--   0     1001      123     3201 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/temporal/duration.rs
+-rw-r--r--   0     1001      123      595 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/temporal/mod.rs
+-rw-r--r--   0     1001      123     3042 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/temporal/time.rs
+-rw-r--r--   0     1001      123      872 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/to_vec.rs
+-rw-r--r--   0     1001      123     8114 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/trusted_len.rs
+-rw-r--r--   0     1001      123    25939 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/upstream_traits.rs
+-rw-r--r--   0     1001      123     7944 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/cloud.rs
+-rw-r--r--   0     1001      123     1549 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/config.rs
+-rw-r--r--   0     1001      123     4469 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/datatypes/_serde.rs
+-rw-r--r--   0     1001      123     2509 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/datatypes/aliases.rs
+-rw-r--r--   0     1001      123    42659 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/datatypes/any_value.rs
+-rw-r--r--   0     1001      123    13349 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/datatypes/dtype.rs
+-rw-r--r--   0     1001      123     5609 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/datatypes/field.rs
+-rw-r--r--   0     1001      123     8059 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/datatypes/mod.rs
+-rw-r--r--   0     1001      123     2016 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/datatypes/time_unit.rs
+-rw-r--r--   0     1001      123      118 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/doc/changelog/mod.rs
+-rw-r--r--   0     1001      123      898 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/doc/changelog/v0_10_0_11.rs
+-rw-r--r--   0     1001      123      481 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/doc/changelog/v0_3.rs
+-rw-r--r--   0     1001      123      293 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/doc/changelog/v0_4.rs
+-rw-r--r--   0     1001      123      499 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/doc/changelog/v0_5.rs
+-rw-r--r--   0     1001      123      288 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/doc/changelog/v0_6.rs
+-rw-r--r--   0     1001      123     1071 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/doc/changelog/v0_7.rs
+-rw-r--r--   0     1001      123      819 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/doc/changelog/v0_8.rs
+-rw-r--r--   0     1001      123      596 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/doc/changelog/v0_9.rs
+-rw-r--r--   0     1001      123       43 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/doc/mod.rs
+-rw-r--r--   0     1001      123       25 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/error.rs
+-rw-r--r--   0     1001      123      263 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/export.rs
+-rw-r--r--   0     1001      123    36432 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/fmt.rs
+-rw-r--r--   0     1001      123     5177 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/frame/arithmetic.rs
+-rw-r--r--   0     1001      123     9916 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/frame/asof_join/asof.rs
+-rw-r--r--   0     1001      123    35761 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/frame/asof_join/groups.rs
+-rw-r--r--   0     1001      123     7168 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/frame/asof_join/mod.rs
+-rw-r--r--   0     1001      123      559 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/frame/chunks.rs
+-rw-r--r--   0     1001      123     5181 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/frame/cross_join.rs
+-rw-r--r--   0     1001      123    16760 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/frame/explode.rs
+-rw-r--r--   0     1001      123     1019 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/frame/from.rs
+-rw-r--r--   0     1001      123    19219 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/frame/groupby/aggregations/agg_list.rs
+-rw-r--r--   0     1001      123     4113 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/frame/groupby/aggregations/boolean.rs
+-rw-r--r--   0     1001      123     7749 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/frame/groupby/aggregations/dispatch.rs
+-rw-r--r--   0     1001      123    40479 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/frame/groupby/aggregations/mod.rs
+-rw-r--r--   0     1001      123     5634 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/frame/groupby/aggregations/utf8.rs
+-rw-r--r--   0     1001      123      218 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/frame/groupby/expr.rs
+-rw-r--r--   0     1001      123    22901 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/frame/groupby/hashing.rs
+-rw-r--r--   0     1001      123    14380 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/frame/groupby/into_groups.rs
+-rw-r--r--   0     1001      123    39623 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/frame/groupby/mod.rs
+-rw-r--r--   0     1001      123    10637 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/frame/groupby/perfect.rs
+-rw-r--r--   0     1001      123    19780 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/frame/groupby/proxy.rs
+-rw-r--r--   0     1001      123     5406 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/frame/hash_join/args.rs
+-rw-r--r--   0     1001      123    13329 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/frame/hash_join/mod.rs
+-rw-r--r--   0     1001      123    22364 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/frame/hash_join/multiple_keys.rs
+-rw-r--r--   0     1001      123     2413 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/frame/hash_join/single_keys.rs
+-rw-r--r--   0     1001      123    17372 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/frame/hash_join/single_keys_dispatch.rs
+-rw-r--r--   0     1001      123     4608 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/frame/hash_join/single_keys_inner.rs
+-rw-r--r--   0     1001      123     6434 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/frame/hash_join/single_keys_left.rs
+-rw-r--r--   0     1001      123     4564 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/frame/hash_join/single_keys_outer.rs
+-rw-r--r--   0     1001      123     3913 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/frame/hash_join/single_keys_semi_anti.rs
+-rw-r--r--   0     1001      123    12313 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/frame/hash_join/sort_merge.rs
+-rw-r--r--   0     1001      123     3865 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/frame/hash_join/zip_outer.rs
+-rw-r--r--   0     1001      123   126103 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/frame/mod.rs
+-rw-r--r--   0     1001      123    27652 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/frame/row/av_buffer.rs
+-rw-r--r--   0     1001      123     5183 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/frame/row/dataframe.rs
+-rw-r--r--   0     1001      123     5976 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/frame/row/mod.rs
+-rw-r--r--   0     1001      123     9875 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/frame/row/transpose.rs
+-rw-r--r--   0     1001      123     2811 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/frame/top_k.rs
+-rw-r--r--   0     1001      123     1388 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/frame/upstream_traits.rs
+-rw-r--r--   0     1001      123    10198 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/functions.rs
+-rw-r--r--   0     1001      123     2149 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/hashing/fx.rs
+-rw-r--r--   0     1001      123     1503 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/hashing/identity.rs
+-rw-r--r--   0     1001      123      457 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/hashing/mod.rs
+-rw-r--r--   0     1001      123     2684 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/hashing/partition.rs
+-rw-r--r--   0     1001      123    17704 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/hashing/vector_hasher.rs
+-rw-r--r--   0     1001      123     1896 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/lib.rs
+-rw-r--r--   0     1001      123    15733 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/named_from.rs
+-rw-r--r--   0     1001      123     2423 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/prelude.rs
+-rw-r--r--   0     1001      123    17667 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/schema.rs
+-rw-r--r--   0     1001      123     3995 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/serde/chunked_array.rs
+-rw-r--r--   0     1001      123     1094 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/serde/df.rs
+-rw-r--r--   0     1001      123     4752 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/serde/mod.rs
+-rw-r--r--   0     1001      123     9938 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/serde/series.rs
+-rw-r--r--   0     1001      123    18543 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/series/any_value.rs
+-rw-r--r--   0     1001      123    28755 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/series/arithmetic/borrowed.rs
+-rw-r--r--   0     1001      123      222 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/series/arithmetic/mod.rs
+-rw-r--r--   0     1001      123     3546 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/series/arithmetic/owned.rs
+-rw-r--r--   0     1001      123    19293 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/series/comparison.rs
+-rw-r--r--   0     1001      123    29575 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/series/from.rs
+-rw-r--r--   0     1001      123     6080 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/series/implementations/array.rs
+-rw-r--r--   0     1001      123     9089 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/series/implementations/binary.rs
+-rw-r--r--   0     1001      123    10835 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/series/implementations/boolean.rs
+-rw-r--r--   0     1001      123    12800 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/series/implementations/categorical.rs
+-rw-r--r--   0     1001      123    18214 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/series/implementations/dates_time.rs
+-rw-r--r--   0     1001      123    15034 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/series/implementations/datetime.rs
+-rw-r--r--   0     1001      123     7981 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/series/implementations/decimal.rs
+-rw-r--r--   0     1001      123    14734 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/series/implementations/duration.rs
+-rw-r--r--   0     1001      123    14063 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/series/implementations/floats.rs
+-rw-r--r--   0     1001      123     6078 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/series/implementations/list.rs
+-rw-r--r--   0     1001      123    18396 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/series/implementations/mod.rs
+-rw-r--r--   0     1001      123     5522 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/series/implementations/null.rs
+-rw-r--r--   0     1001      123     7939 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/series/implementations/object.rs
+-rw-r--r--   0     1001      123    11788 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/series/implementations/struct_.rs
+-rw-r--r--   0     1001      123     9607 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/series/implementations/utf8.rs
+-rw-r--r--   0     1001      123     4471 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/series/into.rs
+-rw-r--r--   0     1001      123     6241 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/series/iterator.rs
+-rw-r--r--   0     1001      123    39074 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/series/mod.rs
+-rw-r--r--   0     1001      123      853 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/series/ops/diff.rs
+-rw-r--r--   0     1001      123     5814 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/series/ops/downcast.rs
+-rw-r--r--   0     1001      123     3601 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/series/ops/ewm.rs
+-rw-r--r--   0     1001      123      413 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/series/ops/extend.rs
+-rw-r--r--   0     1001      123      562 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/series/ops/mod.rs
+-rw-r--r--   0     1001      123     5974 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/series/ops/moment.rs
+-rw-r--r--   0     1001      123     2908 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/series/ops/null.rs
+-rw-r--r--   0     1001      123     1347 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/series/ops/pct_change.rs
+-rw-r--r--   0     1001      123     4620 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/series/ops/round.rs
+-rw-r--r--   0     1001      123     5073 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/series/ops/to_list.rs
+-rw-r--r--   0     1001      123     1476 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/series/ops/unique.rs
+-rw-r--r--   0     1001      123    18408 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/series/series_trait.rs
+-rw-r--r--   0     1001      123     2912 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/series/unstable.rs
+-rw-r--r--   0     1001      123     7077 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/testing.rs
+-rw-r--r--   0     1001      123      508 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/tests.rs
+-rw-r--r--   0     1001      123     2492 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/utils/flatten.rs
+-rw-r--r--   0     1001      123    30596 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/utils/mod.rs
+-rw-r--r--   0     1001      123     1600 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/utils/series.rs
+-rw-r--r--   0     1001      123    13201 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-core/src/utils/supertype.rs
+-rw-r--r--   0        0        0     1998 1970-01-01 00:00:00.000000 polars_u64_idx-0.18.4/local_dependencies/polars-pipe/Cargo.toml
+-rw-r--r--   0     1001      123     1055 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-pipe/LICENSE
+-rw-r--r--   0     1001      123      165 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-pipe/README.md
+-rw-r--r--   0     1001      123       98 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-pipe/src/executors/mod.rs
+-rw-r--r--   0     1001      123     1219 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-pipe/src/executors/operators/filter.rs
+-rw-r--r--   0     1001      123     4103 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-pipe/src/executors/operators/function.rs
+-rw-r--r--   0     1001      123      266 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-pipe/src/executors/operators/mod.rs
+-rw-r--r--   0     1001      123      682 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-pipe/src/executors/operators/pass.rs
+-rw-r--r--   0     1001      123      548 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-pipe/src/executors/operators/placeholder.rs
+-rw-r--r--   0     1001      123     3553 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-pipe/src/executors/operators/projection.rs
+-rw-r--r--   0     1001      123     3559 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-pipe/src/executors/operators/reproject.rs
+-rw-r--r--   0     1001      123     6479 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-pipe/src/executors/sinks/file_sink.rs
+-rw-r--r--   0     1001      123    11288 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/convert.rs
+-rw-r--r--   0     1001      123     1207 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/count.rs
+-rw-r--r--   0     1001      123     1888 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/first.rs
+-rw-r--r--   0     1001      123     4554 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/interface.rs
+-rw-r--r--   0     1001      123     1746 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/last.rs
+-rw-r--r--   0     1001      123     5413 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/mean.rs
+-rw-r--r--   0     1001      123     4951 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/min_max.rs
+-rw-r--r--   0     1001      123      211 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/mod.rs
+-rw-r--r--   0     1001      123      856 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/null.rs
+-rw-r--r--   0     1001      123     4294 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/sum.rs
+-rw-r--r--   0     1001      123     4109 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/eval.rs
+-rw-r--r--   0     1001      123     7404 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/global.rs
+-rw-r--r--   0     1001      123    10554 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/hash_table.rs
+-rw-r--r--   0     1001      123     3589 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/mod.rs
+-rw-r--r--   0     1001      123     2767 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/ooc_state.rs
+-rw-r--r--   0     1001      123     6326 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/sink.rs
+-rw-r--r--   0     1001      123     3116 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/source.rs
+-rw-r--r--   0     1001      123    10194 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/thread_local.rs
+-rw-r--r--   0     1001      123     2119 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-pipe/src/executors/sinks/groupby/mod.rs
+-rw-r--r--   0     1001      123     4695 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-pipe/src/executors/sinks/groupby/ooc.rs
+-rw-r--r--   0     1001      123     1887 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-pipe/src/executors/sinks/groupby/ooc_state.rs
+-rw-r--r--   0     1001      123    20783 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-pipe/src/executors/sinks/groupby/primitive/mod.rs
+-rw-r--r--   0     1001      123    23825 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-pipe/src/executors/sinks/groupby/string.rs
+-rw-r--r--   0     1001      123     2457 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-pipe/src/executors/sinks/groupby/utils.rs
+-rw-r--r--   0     1001      123     9239 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-pipe/src/executors/sinks/io.rs
+-rw-r--r--   0     1001      123     5451 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-pipe/src/executors/sinks/joins/cross.rs
+-rw-r--r--   0     1001      123    11949 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-pipe/src/executors/sinks/joins/generic_build.rs
+-rw-r--r--   0     1001      123    11756 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-pipe/src/executors/sinks/joins/inner_left.rs
+-rw-r--r--   0     1001      123      178 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-pipe/src/executors/sinks/joins/mod.rs
+-rw-r--r--   0     1001      123     2241 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-pipe/src/executors/sinks/memory.rs
+-rw-r--r--   0     1001      123      589 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-pipe/src/executors/sinks/mod.rs
+-rw-r--r--   0     1001      123     1492 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-pipe/src/executors/sinks/ordered.rs
+-rw-r--r--   0     1001      123     1824 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-pipe/src/executors/sinks/reproject.rs
+-rw-r--r--   0     1001      123     3108 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-pipe/src/executors/sinks/slice.rs
+-rw-r--r--   0     1001      123      130 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-pipe/src/executors/sinks/sort/mod.rs
+-rw-r--r--   0     1001      123     6774 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-pipe/src/executors/sinks/sort/ooc.rs
+-rw-r--r--   0     1001      123     7279 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-pipe/src/executors/sinks/sort/sink.rs
+-rw-r--r--   0     1001      123     5953 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-pipe/src/executors/sinks/sort/sink_multiple.rs
+-rw-r--r--   0     1001      123     3908 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-pipe/src/executors/sinks/sort/source.rs
+-rw-r--r--   0     1001      123      526 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-pipe/src/executors/sinks/utils.rs
+-rw-r--r--   0     1001      123     5984 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-pipe/src/executors/sources/csv.rs
+-rw-r--r--   0     1001      123     1231 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-pipe/src/executors/sources/frame.rs
+-rw-r--r--   0     1001      123      987 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-pipe/src/executors/sources/ipc_one_shot.rs
+-rw-r--r--   0     1001      123      366 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-pipe/src/executors/sources/mod.rs
+-rw-r--r--   0     1001      123     4335 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-pipe/src/executors/sources/parquet.rs
+-rw-r--r--   0     1001      123     1146 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-pipe/src/executors/sources/reproject.rs
+-rw-r--r--   0     1001      123     1022 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-pipe/src/executors/sources/union.rs
+-rw-r--r--   0     1001      123      448 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-pipe/src/expressions.rs
+-rw-r--r--   0     1001      123      272 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-pipe/src/lib.rs
+-rw-r--r--   0     1001      123      719 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-pipe/src/operators/chunks.rs
+-rw-r--r--   0     1001      123      474 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-pipe/src/operators/context.rs
+-rw-r--r--   0     1001      123      223 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-pipe/src/operators/mod.rs
+-rw-r--r--   0     1001      123      514 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-pipe/src/operators/operator.rs
+-rw-r--r--   0     1001      123      626 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-pipe/src/operators/sink.rs
+-rw-r--r--   0     1001      123      241 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-pipe/src/operators/source.rs
+-rw-r--r--   0     1001      123        1 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-pipe/src/pipeline/config.rs
+-rw-r--r--   0     1001      123    21321 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-pipe/src/pipeline/convert.rs
+-rw-r--r--   0     1001      123    20362 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-pipe/src/pipeline/dispatcher.rs
+-rw-r--r--   0     1001      123     1155 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-pipe/src/pipeline/mod.rs
+-rw-r--r--   0        0        0     4397 1970-01-01 00:00:00.000000 polars_u64_idx-0.18.4/local_dependencies/polars-io/Cargo.toml
+-rw-r--r--   0     1001      123     1055 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-io/LICENSE
+-rw-r--r--   0     1001      123      138 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-io/README.md
+-rw-r--r--   0     1001      123     2383 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-io/src/avro/mod.rs
+-rw-r--r--   0     1001      123     3608 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-io/src/avro/read.rs
+-rw-r--r--   0     1001      123     2622 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-io/src/avro/write.rs
+-rw-r--r--   0     1001      123     4505 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-io/src/cloud/adaptors.rs
+-rw-r--r--   0     1001      123     9506 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-io/src/cloud/glob.rs
+-rw-r--r--   0     1001      123     3089 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-io/src/cloud/mod.rs
+-rw-r--r--   0     1001      123    28829 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-io/src/csv/buffer.rs
+-rw-r--r--   0     1001      123     1815 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-io/src/csv/mod.rs
+-rw-r--r--   0     1001      123    19446 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-io/src/csv/parser.rs
+-rw-r--r--   0     1001      123    22226 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-io/src/csv/read.rs
+-rw-r--r--   0     1001      123    10846 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-io/src/csv/read_impl/batched_mmap.rs
+-rw-r--r--   0     1001      123    13938 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-io/src/csv/read_impl/batched_read.rs
+-rw-r--r--   0     1001      123    30724 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-io/src/csv/read_impl/mod.rs
+-rw-r--r--   0     1001      123    11466 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-io/src/csv/splitfields.rs
+-rw-r--r--   0     1001      123    24531 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-io/src/csv/utils.rs
+-rw-r--r--   0     1001      123     2796 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-io/src/csv/write.rs
+-rw-r--r--   0     1001      123    14759 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-io/src/csv/write_impl.rs
+-rw-r--r--   0     1001      123      184 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-io/src/export.rs
+-rw-r--r--   0     1001      123     7586 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-io/src/ipc/ipc_file.rs
+-rw-r--r--   0     1001      123     9227 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-io/src/ipc/ipc_stream.rs
+-rw-r--r--   0     1001      123     3253 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-io/src/ipc/mmap.rs
+-rw-r--r--   0     1001      123      401 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-io/src/ipc/mod.rs
+-rw-r--r--   0     1001      123     8287 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-io/src/ipc/write.rs
+-rw-r--r--   0     1001      123     1471 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-io/src/ipc/write_async.rs
+-rw-r--r--   0     1001      123    11044 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-io/src/json/mod.rs
+-rw-r--r--   0     1001      123     4771 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-io/src/lib.rs
+-rw-r--r--   0     1001      123     1969 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-io/src/mmap.rs
+-rw-r--r--   0     1001      123     7228 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-io/src/ndjson/buffer.rs
+-rw-r--r--   0     1001      123    11979 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-io/src/ndjson/core.rs
+-rw-r--r--   0     1001      123       37 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-io/src/ndjson/mod.rs
+-rw-r--r--   0     1001      123      273 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-io/src/options.rs
+-rw-r--r--   0     1001      123     7360 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-io/src/parquet/async_impl.rs
+-rw-r--r--   0     1001      123     3093 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-io/src/parquet/mmap.rs
+-rw-r--r--   0     1001      123     3132 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-io/src/parquet/mod.rs
+-rw-r--r--   0     1001      123     4784 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-io/src/parquet/predicates.rs
+-rw-r--r--   0     1001      123     9623 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-io/src/parquet/read.rs
+-rw-r--r--   0     1001      123    17320 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-io/src/parquet/read_impl.rs
+-rw-r--r--   0     1001      123    10052 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-io/src/parquet/write.rs
+-rw-r--r--   0     1001      123     5334 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-io/src/partition.rs
+-rw-r--r--   0     1001      123     1455 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-io/src/predicates.rs
+-rw-r--r--   0     1001      123      621 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-io/src/prelude.rs
+-rw-r--r--   0     1001      123      417 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-io/src/tests.rs
+-rw-r--r--   0     1001      123     4374 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-io/src/utils.rs
+-rw-r--r--   0        0        0     6077 1970-01-01 00:00:00.000000 polars_u64_idx-0.18.4/local_dependencies/polars-lazy/Cargo.toml
+-rw-r--r--   0     1001      123     1055 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-lazy/LICENSE
+-rw-r--r--   0     1001      123      358 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-lazy/README.md
+-rw-r--r--   0     1001      123     1796 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-lazy/src/dot.rs
+-rw-r--r--   0     1001      123     4479 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-lazy/src/dsl/eval.rs
+-rw-r--r--   0     1001      123     7115 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-lazy/src/dsl/functions.rs
+-rw-r--r--   0     1001      123      164 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-lazy/src/dsl/into.rs
+-rw-r--r--   0     1001      123     6754 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-lazy/src/dsl/list.rs
+-rw-r--r--   0     1001      123     2899 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-lazy/src/dsl/mod.rs
+-rw-r--r--   0     1001      123     1182 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-lazy/src/frame/anonymous_scan.rs
+-rw-r--r--   0     1001      123     9285 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-lazy/src/frame/csv.rs
+-rw-r--r--   0     1001      123     4316 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-lazy/src/frame/file_list_reader.rs
+-rw-r--r--   0     1001      123     2261 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-lazy/src/frame/ipc.rs
+-rw-r--r--   0     1001      123    49023 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-lazy/src/frame/mod.rs
+-rw-r--r--   0     1001      123     3414 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-lazy/src/frame/ndjson.rs
+-rw-r--r--   0     1001      123     2734 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-lazy/src/frame/parquet.rs
+-rw-r--r--   0     1001      123     2892 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-lazy/src/frame/pivot.rs
+-rw-r--r--   0     1001      123      459 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-lazy/src/frame/python.rs
+-rw-r--r--   0     1001      123     6374 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-lazy/src/lib.rs
+-rw-r--r--   0     1001      123     1049 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-lazy/src/physical_plan/executors/cache.rs
+-rw-r--r--   0     1001      123      776 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-lazy/src/physical_plan/executors/executor.rs
+-rw-r--r--   0     1001      123      670 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-lazy/src/physical_plan/executors/ext_context.rs
+-rw-r--r--   0     1001      123     1555 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-lazy/src/physical_plan/executors/filter.rs
+-rw-r--r--   0     1001      123     3986 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-lazy/src/physical_plan/executors/groupby.rs
+-rw-r--r--   0     1001      123     4125 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-lazy/src/physical_plan/executors/groupby_dynamic.rs
+-rw-r--r--   0     1001      123    13599 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-lazy/src/physical_plan/executors/groupby_partitioned.rs
+-rw-r--r--   0     1001      123     4883 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-lazy/src/physical_plan/executors/groupby_rolling.rs
+-rw-r--r--   0     1001      123     5859 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-lazy/src/physical_plan/executors/join.rs
+-rw-r--r--   0     1001      123     6753 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-lazy/src/physical_plan/executors/mod.rs
+-rw-r--r--   0     1001      123     2045 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-lazy/src/physical_plan/executors/projection.rs
+-rw-r--r--   0     1001      123     1761 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-lazy/src/physical_plan/executors/python_scan.rs
+-rw-r--r--   0     1001      123     2854 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-lazy/src/physical_plan/executors/scan/csv.rs
+-rw-r--r--   0     1001      123     1963 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-lazy/src/physical_plan/executors/scan/ipc.rs
+-rw-r--r--   0     1001      123     4303 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-lazy/src/physical_plan/executors/scan/mod.rs
+-rw-r--r--   0     1001      123     1209 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-lazy/src/physical_plan/executors/scan/ndjson.rs
+-rw-r--r--   0     1001      123     2421 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-lazy/src/physical_plan/executors/scan/parquet.rs
+-rw-r--r--   0     1001      123      548 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-lazy/src/physical_plan/executors/slice.rs
+-rw-r--r--   0     1001      123     2197 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-lazy/src/physical_plan/executors/sort.rs
+-rw-r--r--   0     1001      123     2015 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-lazy/src/physical_plan/executors/stack.rs
+-rw-r--r--   0     1001      123      663 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-lazy/src/physical_plan/executors/udf.rs
+-rw-r--r--   0     1001      123     4041 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-lazy/src/physical_plan/executors/union.rs
+-rw-r--r--   0     1001      123      838 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-lazy/src/physical_plan/executors/unique.rs
+-rw-r--r--   0     1001      123     1335 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-lazy/src/physical_plan/exotic.rs
+-rw-r--r--   0     1001      123    21959 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-lazy/src/physical_plan/expressions/aggregation.rs
+-rw-r--r--   0     1001      123     2689 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-lazy/src/physical_plan/expressions/alias.rs
+-rw-r--r--   0     1001      123    18331 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-lazy/src/physical_plan/expressions/apply.rs
+-rw-r--r--   0     1001      123    17674 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-lazy/src/physical_plan/expressions/binary.rs
+-rw-r--r--   0     1001      123     2583 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-lazy/src/physical_plan/expressions/cache.rs
+-rw-r--r--   0     1001      123     3153 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-lazy/src/physical_plan/expressions/cast.rs
+-rw-r--r--   0     1001      123     6326 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-lazy/src/physical_plan/expressions/column.rs
+-rw-r--r--   0     1001      123     1996 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-lazy/src/physical_plan/expressions/count.rs
+-rw-r--r--   0     1001      123     5809 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-lazy/src/physical_plan/expressions/filter.rs
+-rw-r--r--   0     1001      123     4131 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-lazy/src/physical_plan/expressions/group_iter.rs
+-rw-r--r--   0     1001      123     5304 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-lazy/src/physical_plan/expressions/literal.rs
+-rw-r--r--   0     1001      123    23566 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-lazy/src/physical_plan/expressions/mod.rs
+-rw-r--r--   0     1001      123    10091 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-lazy/src/physical_plan/expressions/slice.rs
+-rw-r--r--   0     1001      123     4332 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-lazy/src/physical_plan/expressions/sort.rs
+-rw-r--r--   0     1001      123    13549 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-lazy/src/physical_plan/expressions/sortby.rs
+-rw-r--r--   0     1001      123     8331 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-lazy/src/physical_plan/expressions/take.rs
+-rw-r--r--   0     1001      123    14360 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-lazy/src/physical_plan/expressions/ternary.rs
+-rw-r--r--   0     1001      123    31558 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-lazy/src/physical_plan/expressions/window.rs
+-rw-r--r--   0     1001      123     2039 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-lazy/src/physical_plan/file_cache.rs
+-rw-r--r--   0     1001      123      414 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-lazy/src/physical_plan/mod.rs
+-rw-r--r--   0     1001      123     2005 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-lazy/src/physical_plan/node_timer.rs
+-rw-r--r--   0     1001      123    24050 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-lazy/src/physical_plan/planner/expr.rs
+-rw-r--r--   0     1001      123    20552 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-lazy/src/physical_plan/planner/lp.rs
+-rw-r--r--   0     1001      123       87 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-lazy/src/physical_plan/planner/mod.rs
+-rw-r--r--   0     1001      123    10203 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-lazy/src/physical_plan/state.rs
+-rw-r--r--   0     1001      123     2583 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-lazy/src/physical_plan/streaming/checks.rs
+-rw-r--r--   0     1001      123     9280 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-lazy/src/physical_plan/streaming/construct_pipeline.rs
+-rw-r--r--   0     1001      123    16847 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-lazy/src/physical_plan/streaming/convert_alp.rs
+-rw-r--r--   0     1001      123      116 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-lazy/src/physical_plan/streaming/mod.rs
+-rw-r--r--   0     1001      123     5827 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-lazy/src/physical_plan/streaming/tree.rs
+-rw-r--r--   0     1001      123      722 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-lazy/src/prelude.rs
+-rw-r--r--   0     1001      123    14990 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-lazy/src/tests/aggregations.rs
+-rw-r--r--   0     1001      123     2339 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-lazy/src/tests/arity.rs
+-rw-r--r--   0     1001      123     7276 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-lazy/src/tests/cse.rs
+-rw-r--r--   0     1001      123    12759 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-lazy/src/tests/io.rs
+-rw-r--r--   0     1001      123     4166 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-lazy/src/tests/logical.rs
+-rw-r--r--   0     1001      123     4273 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-lazy/src/tests/mod.rs
+-rw-r--r--   0     1001      123    15770 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-lazy/src/tests/optimization_checks.rs
+-rw-r--r--   0     1001      123     6772 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-lazy/src/tests/predicate_queries.rs
+-rw-r--r--   0     1001      123     3165 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-lazy/src/tests/projection_queries.rs
+-rw-r--r--   0     1001      123    47687 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-lazy/src/tests/queries.rs
+-rw-r--r--   0     1001      123     9519 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-lazy/src/tests/streaming.rs
+-rw-r--r--   0     1001      123     2893 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-lazy/src/tests/tpch.rs
+-rw-r--r--   0     1001      123     1028 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-lazy/src/utils.rs
+-rw-r--r--   0        0        0     3439 1970-01-01 00:00:00.000000 polars_u64_idx-0.18.4/local_dependencies/polars-ops/Cargo.toml
+-rw-r--r--   0     1001      123     1055 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-ops/LICENSE
+-rw-r--r--   0     1001      123      132 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-ops/README.md
+-rw-r--r--   0     1001      123     2382 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-ops/src/chunked_array/array/min_max.rs
+-rw-r--r--   0     1001      123      267 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-ops/src/chunked_array/array/mod.rs
+-rw-r--r--   0     1001      123     1512 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-ops/src/chunked_array/array/namespace.rs
+-rw-r--r--   0     1001      123     4108 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-ops/src/chunked_array/array/sum_mean.rs
+-rw-r--r--   0     1001      123      234 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-ops/src/chunked_array/binary/mod.rs
+-rw-r--r--   0     1001      123     3549 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-ops/src/chunked_array/binary/namespace.rs
+-rw-r--r--   0     1001      123    11023 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-ops/src/chunked_array/interpolate.rs
+-rw-r--r--   0     1001      123     1687 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-ops/src/chunked_array/list/count.rs
+-rw-r--r--   0     1001      123     2419 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-ops/src/chunked_array/list/hash.rs
+-rw-r--r--   0     1001      123     7861 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-ops/src/chunked_array/list/min_max.rs
+-rw-r--r--   0     1001      123      511 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-ops/src/chunked_array/list/mod.rs
+-rw-r--r--   0     1001      123    19010 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-ops/src/chunked_array/list/namespace.rs
+-rw-r--r--   0     1001      123     7633 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-ops/src/chunked_array/list/sum_mean.rs
+-rw-r--r--   0     1001      123     2435 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-ops/src/chunked_array/list/to_struct.rs
+-rw-r--r--   0     1001      123      545 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-ops/src/chunked_array/mod.rs
+-rw-r--r--   0     1001      123     9452 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-ops/src/chunked_array/nan_propagating_aggregate.rs
+-rw-r--r--   0     1001      123     6795 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-ops/src/chunked_array/set.rs
+-rw-r--r--   0     1001      123     8781 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-ops/src/chunked_array/strings/case.rs
+-rw-r--r--   0     1001      123     8593 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-ops/src/chunked_array/strings/json_path.rs
+-rw-r--r--   0     1001      123     2345 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-ops/src/chunked_array/strings/justify.rs
+-rw-r--r--   0     1001      123      514 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-ops/src/chunked_array/strings/mod.rs
+-rw-r--r--   0     1001      123    14951 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-ops/src/chunked_array/strings/namespace.rs
+-rw-r--r--   0     1001      123     4053 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-ops/src/chunked_array/strings/replace.rs
+-rw-r--r--   0     1001      123      439 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-ops/src/chunked_array/sum.rs
+-rw-r--r--   0     1001      123     2486 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-ops/src/chunked_array/top_k.rs
+-rw-r--r--   0     1001      123     7727 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-ops/src/frame/join/merge_sorted.rs
+-rw-r--r--   0     1001      123    18232 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-ops/src/frame/join/mod.rs
+-rw-r--r--   0     1001      123     4291 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-ops/src/frame/mod.rs
+-rw-r--r--   0     1001      123    10257 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-ops/src/frame/pivot/mod.rs
+-rw-r--r--   0     1001      123    13486 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-ops/src/frame/pivot/positioning.rs
+-rw-r--r--   0     1001      123      237 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-ops/src/lib.rs
+-rw-r--r--   0     1001      123      290 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-ops/src/prelude.rs
+-rw-r--r--   0     1001      123       25 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-ops/src/series/mod.rs
+-rw-r--r--   0     1001      123     9623 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-ops/src/series/ops/approx_algo/hyperloglogplus.rs
+-rw-r--r--   0     1001      123      118 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-ops/src/series/ops/approx_algo/mod.rs
+-rw-r--r--   0     1001      123     2016 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-ops/src/series/ops/approx_unique.rs
+-rw-r--r--   0     1001      123    11866 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-ops/src/series/ops/arg_min_max.rs
+-rw-r--r--   0     1001      123     3688 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-ops/src/series/ops/floor_divide.rs
+-rw-r--r--   0     1001      123     5245 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-ops/src/series/ops/fused.rs
+-rw-r--r--   0     1001      123     3423 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-ops/src/series/ops/is_first.rs
+-rw-r--r--   0     1001      123     2975 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-ops/src/series/ops/is_unique.rs
+-rw-r--r--   0     1001      123     3626 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-ops/src/series/ops/log.rs
+-rw-r--r--   0     1001      123     1187 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-ops/src/series/ops/mod.rs
+-rw-r--r--   0     1001      123     1769 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-ops/src/series/ops/rolling.rs
+-rw-r--r--   0     1001      123     7642 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-ops/src/series/ops/search_sorted.rs
+-rw-r--r--   0     1001      123     2603 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-ops/src/series/ops/to_dummies.rs
+-rw-r--r--   0     1001      123     2067 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-ops/src/series/ops/various.rs
+-rw-r--r--   0        0        0     1106 1970-01-01 00:00:00.000000 polars_u64_idx-0.18.4/local_dependencies/polars-sql/Cargo.toml
+-rw-r--r--   0     1001      123     1055 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-sql/LICENSE
+-rw-r--r--   0     1001      123      466 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-sql/README.md
+-rw-r--r--   0     1001      123    23236 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-sql/src/context.rs
+-rw-r--r--   0     1001      123    23921 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-sql/src/functions.rs
+-rw-r--r--   0     1001      123     2122 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-sql/src/keywords.rs
+-rw-r--r--   0     1001      123      239 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-sql/src/lib.rs
+-rw-r--r--   0     1001      123    20933 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-sql/src/sql_expr.rs
+-rw-r--r--   0     1001      123     4572 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-sql/src/table_functions.rs
+-rw-r--r--   0     1001      123     1682 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-sql/tests/functions_cumulative.rs
+-rw-r--r--   0     1001      123     3063 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-sql/tests/functions_io.rs
+-rw-r--r--   0     1001      123     1539 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-sql/tests/functions_math.rs
+-rw-r--r--   0     1001      123      860 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-sql/tests/functions_meta.rs
+-rw-r--r--   0     1001      123     2982 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-sql/tests/functions_string.rs
+-rw-r--r--   0     1001      123     1056 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-sql/tests/iss_7436.rs
+-rw-r--r--   0     1001      123      888 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-sql/tests/iss_7437.rs
+-rw-r--r--   0     1001      123      652 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-sql/tests/iss_7440.rs
+-rw-r--r--   0     1001      123      700 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-sql/tests/iss_8395.rs
+-rw-r--r--   0     1001      123     1062 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-sql/tests/iss_8419.rs
+-rw-r--r--   0     1001      123      982 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-sql/tests/ops_distinct_on.rs
+-rw-r--r--   0     1001      123    15811 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-sql/tests/simple_exprs.rs
+-rw-r--r--   0     1001      123     3343 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-sql/tests/statements.rs
+-rw-r--r--   0        0        0      954 1970-01-01 00:00:00.000000 polars_u64_idx-0.18.4/local_dependencies/polars-row/Cargo.toml
+-rw-r--r--   0     1001      123     1055 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-row/LICENSE
+-rw-r--r--   0     1001      123      137 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-row/README.md
+-rw-r--r--   0     1001      123     1916 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-row/src/decode.rs
+-rw-r--r--   0     1001      123    13364 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-row/src/encode.rs
+-rw-r--r--   0     1001      123     7719 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-row/src/fixed.rs
+-rw-r--r--   0     1001      123    13846 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-row/src/lib.rs
+-rw-r--r--   0     1001      123     3019 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-row/src/row.rs
+-rw-r--r--   0     1001      123      682 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-row/src/utils.rs
+-rw-r--r--   0     1001      123     8679 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-row/src/variable.rs
+-rw-r--r--   0        0        0      827 1970-01-01 00:00:00.000000 polars_u64_idx-0.18.4/local_dependencies/polars-algo/Cargo.toml
+-rw-r--r--   0     1001      123     1055 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-algo/LICENSE
+-rw-r--r--   0     1001      123      142 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-algo/README.md
+-rw-r--r--   0     1001      123     7548 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-algo/src/algo.rs
+-rw-r--r--   0     1001      123       88 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-algo/src/lib.rs
+-rw-r--r--   0     1001      123       28 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-algo/src/prelude.rs
+-rw-r--r--   0        0        0    10626 1970-01-01 00:00:00.000000 polars_u64_idx-0.18.4/local_dependencies/polars/Cargo.toml
+-rw-r--r--   0     1001      123     1055 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars/LICENSE
+-rw-r--r--   0     1001      123     3472 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars/Makefile
+-rw-r--r--   0     1001      123      215 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars/build.rs
+-rw-r--r--   0     1001      123       78 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars/clippy.toml
+-rw-r--r--   0     1001      123    17602 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars/src/docs/eager.rs
+-rw-r--r--   0     1001      123     8794 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars/src/docs/lazy.rs
+-rw-r--r--   0     1001      123       50 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars/src/docs/mod.rs
+-rw-r--r--   0     1001      123     3797 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars/src/docs/performance.rs
+-rw-r--r--   0     1001      123       59 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars/src/export.rs
+-rw-r--r--   0     1001      123    20214 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars/src/lib.rs
+-rw-r--r--   0     1001      123      387 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars/src/prelude.rs
+-rw-r--r--   0     1001      123       54 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars/src/sql.rs
+-rw-r--r--   0     1001      123     4272 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars/tests/it/core/date_like.rs
+-rw-r--r--   0     1001      123     2401 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars/tests/it/core/groupby.rs
+-rw-r--r--   0     1001      123    17836 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars/tests/it/core/joins.rs
+-rw-r--r--   0     1001      123      545 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars/tests/it/core/list.rs
+-rw-r--r--   0     1001      123      198 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars/tests/it/core/mod.rs
+-rw-r--r--   0     1001      123       24 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars/tests/it/core/ops/mod.rs
+-rw-r--r--   0     1001      123      457 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars/tests/it/core/ops/take.rs
+-rw-r--r--   0     1001      123     6259 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars/tests/it/core/pivot.rs
+-rw-r--r--   0     1001      123     1102 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars/tests/it/core/random.rs
+-rw-r--r--   0     1001      123    11096 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars/tests/it/core/rolling_window.rs
+-rw-r--r--   0     1001      123     1093 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars/tests/it/core/series.rs
+-rw-r--r--   0     1001      123      370 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars/tests/it/core/utils.rs
+-rw-r--r--   0     1001      123    30423 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars/tests/it/io/csv.rs
+-rw-r--r--   0     1001      123     4490 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars/tests/it/io/ipc_stream.rs
+-rw-r--r--   0     1001      123     7043 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars/tests/it/io/json.rs
+-rw-r--r--   0     1001      123      378 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars/tests/it/io/mod.rs
+-rw-r--r--   0     1001      123      531 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars/tests/it/io/parquet.rs
+-rw-r--r--   0     1001      123     1530 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars/tests/it/joins.rs
+-rw-r--r--   0     1001      123     2452 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars/tests/it/lazy/aggregation.rs
+-rw-r--r--   0     1001      123      821 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars/tests/it/lazy/cse.rs
+-rw-r--r--   0     1001      123      500 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars/tests/it/lazy/explodes.rs
+-rw-r--r--   0     1001      123     2279 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars/tests/it/lazy/expressions/apply.rs
+-rw-r--r--   0     1001      123    10285 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars/tests/it/lazy/expressions/arity.rs
+-rw-r--r--   0     1001      123     1065 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars/tests/it/lazy/expressions/expand.rs
+-rw-r--r--   0     1001      123     1008 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars/tests/it/lazy/expressions/filter.rs
+-rw-r--r--   0     1001      123      428 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars/tests/it/lazy/expressions/is_in.rs
+-rw-r--r--   0     1001      123      121 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars/tests/it/lazy/expressions/mod.rs
+-rw-r--r--   0     1001      123      659 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars/tests/it/lazy/expressions/slice.rs
+-rw-r--r--   0     1001      123    10657 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars/tests/it/lazy/expressions/window.rs
+-rw-r--r--   0     1001      123      579 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars/tests/it/lazy/folds.rs
+-rw-r--r--   0     1001      123      557 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars/tests/it/lazy/functions.rs
+-rw-r--r--   0     1001      123     4482 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars/tests/it/lazy/groupby.rs
+-rw-r--r--   0     1001      123     1681 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars/tests/it/lazy/groupby_dynamic.rs
+-rw-r--r--   0     1001      123      691 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars/tests/it/lazy/mod.rs
+-rw-r--r--   0     1001      123     5747 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars/tests/it/lazy/predicate_queries.rs
+-rw-r--r--   0     1001      123     4483 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars/tests/it/lazy/projection_queries.rs
+-rw-r--r--   0     1001      123     6584 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars/tests/it/lazy/queries.rs
+-rw-r--r--   0     1001      123      141 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars/tests/it/main.rs
+-rw-r--r--   0     1001      123    12591 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars/tests/it/schema.rs
+-rw-r--r--   0     1001      123     2061 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars/tests/it/time/date_range.rs
+-rw-r--r--   0        0        0     1592 1970-01-01 00:00:00.000000 polars_u64_idx-0.18.4/local_dependencies/polars-arrow/Cargo.toml
+-rw-r--r--   0     1001      123     1055 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-arrow/LICENSE
+-rw-r--r--   0     1001      123      144 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-arrow/README.md
+-rw-r--r--   0     1001      123     1975 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-arrow/src/array/default_arrays.rs
+-rw-r--r--   0     1001      123     1791 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-arrow/src/array/fixed_size_list.rs
+-rw-r--r--   0     1001      123     3773 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-arrow/src/array/get.rs
+-rw-r--r--   0     1001      123     6664 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-arrow/src/array/list.rs
+-rw-r--r--   0     1001      123     8165 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-arrow/src/array/mod.rs
+-rw-r--r--   0     1001      123      878 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-arrow/src/array/null.rs
+-rw-r--r--   0     1001      123     1125 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-arrow/src/array/slice.rs
+-rw-r--r--   0     1001      123     2253 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-arrow/src/array/utf8.rs
+-rw-r--r--   0     1001      123     2294 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-arrow/src/bit_util.rs
+-rw-r--r--   0     1001      123       17 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-arrow/src/bitmap/mod.rs
+-rw-r--r--   0     1001      123      819 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-arrow/src/bitmap/mutable.rs
+-rw-r--r--   0     1001      123      370 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-arrow/src/compute/arithmetics/decimal/add.rs
+-rw-r--r--   0     1001      123     2181 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-arrow/src/compute/arithmetics/decimal/commutative.rs
+-rw-r--r--   0     1001      123     1482 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-arrow/src/compute/arithmetics/decimal/div.rs
+-rw-r--r--   0     1001      123     1028 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-arrow/src/compute/arithmetics/decimal/mod.rs
+-rw-r--r--   0     1001      123     1177 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-arrow/src/compute/arithmetics/decimal/mul.rs
+-rw-r--r--   0     1001      123      508 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-arrow/src/compute/arithmetics/decimal/sub.rs
+-rw-r--r--   0     1001      123       51 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-arrow/src/compute/arithmetics/mod.rs
+-rw-r--r--   0     1001      123        1 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-arrow/src/compute/arity.rs
+-rw-r--r--   0     1001      123      727 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-arrow/src/compute/bitwise.rs
+-rw-r--r--   0     1001      123     1206 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-arrow/src/compute/cast.rs
+-rw-r--r--   0     1001      123     3964 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-arrow/src/compute/decimal.rs
+-rw-r--r--   0     1001      123     1250 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-arrow/src/compute/mod.rs
+-rw-r--r--   0     1001      123      391 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-arrow/src/compute/take/bitmap.rs
+-rw-r--r--   0     1001      123     2767 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-arrow/src/compute/take/boolean.rs
+-rw-r--r--   0     1001      123     3487 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-arrow/src/compute/take/fixed_size_list.rs
+-rw-r--r--   0     1001      123    25290 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-arrow/src/compute/take/mod.rs
+-rw-r--r--   0     1001      123      797 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-arrow/src/compute/tile.rs
+-rw-r--r--   0     1001      123     1102 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-arrow/src/conversion.rs
+-rw-r--r--   0     1001      123     1609 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-arrow/src/data_types.rs
+-rw-r--r--   0     1001      123       25 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-arrow/src/error.rs
+-rw-r--r--   0     1001      123       28 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-arrow/src/export.rs
+-rw-r--r--   0     1001      123       26 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-arrow/src/floats/mod.rs
+-rw-r--r--   0     1001      123     2066 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-arrow/src/floats/ord.rs
+-rw-r--r--   0     1001      123     1273 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-arrow/src/index.rs
+-rw-r--r--   0     1001      123      984 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-arrow/src/is_valid.rs
+-rw-r--r--   0     1001      123     4783 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-arrow/src/kernels/agg_mean.rs
+-rw-r--r--   0     1001      123     1074 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-arrow/src/kernels/comparison.rs
+-rw-r--r--   0     1001      123     1068 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-arrow/src/kernels/concatenate.rs
+-rw-r--r--   0     1001      123     5161 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-arrow/src/kernels/ewm/average.rs
+-rw-r--r--   0     1001      123     1808 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-arrow/src/kernels/ewm/mod.rs
+-rw-r--r--   0     1001      123    25065 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-arrow/src/kernels/ewm/variance.rs
+-rw-r--r--   0     1001      123     1406 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-arrow/src/kernels/float.rs
+-rw-r--r--   0     1001      123     4908 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-arrow/src/kernels/list.rs
+-rw-r--r--   0     1001      123     1885 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-arrow/src/kernels/list_bytes_iter.rs
+-rw-r--r--   0     1001      123     9783 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-arrow/src/kernels/mod.rs
+-rw-r--r--   0     1001      123     3923 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-arrow/src/kernels/rolling/mod.rs
+-rw-r--r--   0     1001      123     2019 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/mean.rs
+-rw-r--r--   0     1001      123    16187 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/min_max.rs
+-rw-r--r--   0     1001      123     3839 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/mod.rs
+-rw-r--r--   0     1001      123    11729 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/quantile.rs
+-rw-r--r--   0     1001      123     5684 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/sum.rs
+-rw-r--r--   0     1001      123     7745 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/variance.rs
+-rw-r--r--   0     1001      123     1879 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-arrow/src/kernels/rolling/nulls/mean.rs
+-rw-r--r--   0     1001      123    14722 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-arrow/src/kernels/rolling/nulls/min_max.rs
+-rw-r--r--   0     1001      123    10055 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-arrow/src/kernels/rolling/nulls/mod.rs
+-rw-r--r--   0     1001      123    11643 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-arrow/src/kernels/rolling/nulls/quantile.rs
+-rw-r--r--   0     1001      123     4821 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-arrow/src/kernels/rolling/nulls/sum.rs
+-rw-r--r--   0     1001      123     6856 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-arrow/src/kernels/rolling/nulls/variance.rs
+-rw-r--r--   0     1001      123     8109 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-arrow/src/kernels/rolling/window.rs
+-rw-r--r--   0     1001      123     4753 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-arrow/src/kernels/set.rs
+-rw-r--r--   0     1001      123     4529 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-arrow/src/kernels/sort_partition.rs
+-rw-r--r--   0     1001      123     2948 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-arrow/src/kernels/sorted_join/inner.rs
+-rw-r--r--   0     1001      123     5974 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-arrow/src/kernels/sorted_join/left.rs
+-rw-r--r--   0     1001      123      231 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-arrow/src/kernels/sorted_join/mod.rs
+-rw-r--r--   0     1001      123      842 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-arrow/src/kernels/string.rs
+-rw-r--r--   0     1001      123     2310 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-arrow/src/kernels/take_agg/boolean.rs
+-rw-r--r--   0     1001      123     4315 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-arrow/src/kernels/take_agg/mod.rs
+-rw-r--r--   0     1001      123     2606 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-arrow/src/kernels/take_agg/var.rs
+-rw-r--r--   0     1001      123     3672 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-arrow/src/kernels/time.rs
+-rw-r--r--   0     1001      123      341 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-arrow/src/lib.rs
+-rw-r--r--   0     1001      123      496 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-arrow/src/prelude.rs
+-rw-r--r--   0     1001      123      534 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-arrow/src/slice.rs
+-rw-r--r--   0     1001      123      183 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-arrow/src/time_zone.rs
+-rw-r--r--   0     1001      123      998 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-arrow/src/trusted_len/boolean.rs
+-rw-r--r--   0     1001      123     2821 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-arrow/src/trusted_len/mod.rs
+-rw-r--r--   0     1001      123     2054 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-arrow/src/trusted_len/push_unchecked.rs
+-rw-r--r--   0     1001      123      158 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-arrow/src/trusted_len/rev.rs
+-rw-r--r--   0     1001      123     5233 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-arrow/src/utils.rs
+-rw-r--r--   0        0        0      587 1970-01-01 00:00:00.000000 polars_u64_idx-0.18.4/local_dependencies/polars-utils/Cargo.toml
+-rw-r--r--   0     1001      123     1055 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-utils/LICENSE
+-rw-r--r--   0     1001      123      141 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-utils/README.md
+-rw-r--r--   0     1001      123      151 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-utils/src/aliases.rs
+-rw-r--r--   0     1001      123     2862 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-utils/src/arena.rs
+-rw-r--r--   0     1001      123     1379 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-utils/src/atomic.rs
+-rw-r--r--   0     1001      123     2659 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-utils/src/cell.rs
+-rw-r--r--   0     1001      123     1015 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-utils/src/contention_pool.rs
+-rw-r--r--   0     1001      123      509 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-utils/src/error.rs
+-rw-r--r--   0     1001      123      271 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-utils/src/fmt.rs
+-rw-r--r--   0     1001      123      763 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-utils/src/functions.rs
+-rw-r--r--   0     1001      123     2709 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-utils/src/iter/enumerate_idx.rs
+-rw-r--r--   0     1001      123       61 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-utils/src/iter/mod.rs
+-rw-r--r--   0     1001      123      503 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-utils/src/lib.rs
+-rw-r--r--   0     1001      123      573 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-utils/src/macros.rs
+-rw-r--r--   0     1001      123      282 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-utils/src/mem.rs
+-rw-r--r--   0     1001      123     2642 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-utils/src/slice.rs
+-rw-r--r--   0     1001      123     2467 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-utils/src/sort.rs
+-rw-r--r--   0     1001      123     1115 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-utils/src/sync.rs
+-rw-r--r--   0     1001      123      504 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-utils/src/sys.rs
+-rw-r--r--   0     1001      123      697 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-utils/src/unwrap.rs
+-rw-r--r--   0     1001      123     2024 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-utils/src/vec.rs
+-rw-r--r--   0     1001      123      616 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-utils/src/wasm.rs
+-rw-r--r--   0        0        0     2037 1970-01-01 00:00:00.000000 polars_u64_idx-0.18.4/local_dependencies/polars-time/Cargo.toml
+-rw-r--r--   0     1001      123     1055 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-time/LICENSE
+-rw-r--r--   0     1001      123      143 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-time/README.md
+-rw-r--r--   0     1001      123     3569 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-time/src/chunkedarray/date.rs
+-rw-r--r--   0     1001      123     6465 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-time/src/chunkedarray/datetime.rs
+-rw-r--r--   0     1001      123     3305 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-time/src/chunkedarray/duration.rs
+-rw-r--r--   0     1001      123     5607 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-time/src/chunkedarray/kernels.rs
+-rw-r--r--   0     1001      123     1062 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-time/src/chunkedarray/mod.rs
+-rw-r--r--   0     1001      123     6737 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-time/src/chunkedarray/rolling_window/floats.rs
+-rw-r--r--   0     1001      123     2582 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-time/src/chunkedarray/rolling_window/ints.rs
+-rw-r--r--   0     1001      123    11122 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-time/src/chunkedarray/rolling_window/mod.rs
+-rw-r--r--   0     1001      123      413 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-time/src/chunkedarray/rolling_window/rolling_kernels/mod.rs
+-rw-r--r--   0     1001      123     4810 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-time/src/chunkedarray/rolling_window/rolling_kernels/no_nulls.rs
+-rw-r--r--   0     1001      123     2372 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-time/src/chunkedarray/time.rs
+-rw-r--r--   0     1001      123    21334 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-time/src/chunkedarray/utf8/infer.rs
+-rw-r--r--   0     1001      123    18997 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-time/src/chunkedarray/utf8/mod.rs
+-rw-r--r--   0     1001      123     3975 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-time/src/chunkedarray/utf8/patterns.rs
+-rw-r--r--   0     1001      123    10548 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-time/src/chunkedarray/utf8/strptime.rs
+-rw-r--r--   0     1001      123     3340 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-time/src/date_range.rs
+-rw-r--r--   0     1001      123    34703 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-time/src/groupby/dynamic.rs
+-rw-r--r--   0     1001      123       88 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-time/src/groupby/mod.rs
+-rw-r--r--   0     1001      123      621 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-time/src/lib.rs
+-rw-r--r--   0     1001      123     2976 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-time/src/month_end.rs
+-rw-r--r--   0     1001      123     3365 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-time/src/month_start.rs
+-rw-r--r--   0     1001      123      274 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-time/src/prelude.rs
+-rw-r--r--   0     1001      123     1381 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-time/src/round.rs
+-rw-r--r--   0     1001      123     3992 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-time/src/series/_trait.rs
+-rw-r--r--   0     1001      123      136 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-time/src/series/implementations/boolean.rs
+-rw-r--r--   0     1001      123      140 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-time/src/series/implementations/categoricals.rs
+-rw-r--r--   0     1001      123      133 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-time/src/series/implementations/date.rs
+-rw-r--r--   0     1001      123      137 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-time/src/series/implementations/datetime.rs
+-rw-r--r--   0     1001      123      137 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-time/src/series/implementations/duration.rs
+-rw-r--r--   0     1001      123     1863 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-time/src/series/implementations/floats.rs
+-rw-r--r--   0     1001      123     1792 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-time/src/series/implementations/integers.rs
+-rw-r--r--   0     1001      123      133 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-time/src/series/implementations/list.rs
+-rw-r--r--   0     1001      123      486 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-time/src/series/implementations/mod.rs
+-rw-r--r--   0     1001      123      155 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-time/src/series/implementations/object.rs
+-rw-r--r--   0     1001      123      135 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-time/src/series/implementations/struct_.rs
+-rw-r--r--   0     1001      123      133 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-time/src/series/implementations/time.rs
+-rw-r--r--   0     1001      123      133 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-time/src/series/implementations/utf8.rs
+-rw-r--r--   0     1001      123    12791 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-time/src/series/mod.rs
+-rw-r--r--   0     1001      123     1443 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-time/src/truncate.rs
+-rw-r--r--   0     1001      123     6845 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-time/src/upsample.rs
+-rw-r--r--   0     1001      123     2511 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-time/src/utils.rs
+-rw-r--r--   0     1001      123     1524 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-time/src/windows/bounds.rs
+-rw-r--r--   0     1001      123     2672 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-time/src/windows/calendar.rs
+-rw-r--r--   0     1001      123    25015 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-time/src/windows/duration.rs
+-rw-r--r--   0     1001      123    20201 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-time/src/windows/groupby.rs
+-rw-r--r--   0     1001      123      503 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-time/src/windows/mod.rs
+-rw-r--r--   0     1001      123    23627 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-time/src/windows/test.rs
+-rw-r--r--   0     1001      123    10657 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/local_dependencies/polars-time/src/windows/window.rs
+-rw-r--r--   0        0        0     4403 1970-01-01 00:00:00.000000 polars_u64_idx-0.18.4/Cargo.toml
+-rw-r--r--   0     1001      123       76 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/.gitignore
+-rw-r--r--   0     1001      123     1055 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/LICENSE
+-rw-r--r--   0     1001      123     2414 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/Makefile
+-rw-r--r--   0     1001      123    12006 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/README.md
+-rw-r--r--   0     1001      123      651 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/build.rs
+-rw-r--r--   0     1001      123       32 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/docs/.gitignore
+-rw-r--r--   0     1001      123      679 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/docs/Makefile
+-rw-r--r--   0     1001      123      318 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/docs/_templates/api_redirect.html
+-rw-r--r--   0     1001      123      151 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/docs/_templates/autosummary/accessor.rst
+-rw-r--r--   0     1001      123      160 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/docs/_templates/autosummary/accessor_attribute.rst
+-rw-r--r--   0     1001      123      168 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/docs/_templates/autosummary/accessor_callable.rst
+-rw-r--r--   0     1001      123      157 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/docs/_templates/autosummary/accessor_method.rst
+-rw-r--r--   0     1001      123      836 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/docs/_templates/autosummary/class.rst
+-rw-r--r--   0     1001      123       94 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/docs/_templates/autosummary/class_without_autosummary.rst
+-rw-r--r--   0     1001      123      406 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/docs/_templates/sidebar-nav-bs.html
+-rw-r--r--   0     1001      123      491 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/docs/requirements-docs.txt
+-rw-r--r--   0     1001      123     1164 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/docs/run_live_docs_server.py
+-rw-r--r--   0     1001      123     1567 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/docs/source/_static/css/custom.css
+-rw-r--r--   0     1001      123     7297 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/docs/source/conf.py
+-rw-r--r--   0     1001      123       51 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/docs/source/index.rst
+-rw-r--r--   0     1001      123     6767 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/docs/source/reference/api.rst
+-rw-r--r--   0     1001      123     2069 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/docs/source/reference/config.rst
+-rw-r--r--   0     1001      123      274 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/docs/source/reference/dataframe/aggregation.rst
+-rw-r--r--   0     1001      123      221 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/docs/source/reference/dataframe/attributes.rst
+-rw-r--r--   0     1001      123      142 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/docs/source/reference/dataframe/computation.rst
+-rw-r--r--   0     1001      123      319 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/docs/source/reference/dataframe/descriptive.rst
+-rw-r--r--   0     1001      123      319 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/docs/source/reference/dataframe/export.rst
+-rw-r--r--   0     1001      123      464 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/docs/source/reference/dataframe/groupby.rst
+-rw-r--r--   0     1001      123      379 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/docs/source/reference/dataframe/index.rst
+-rw-r--r--   0     1001      123      189 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/docs/source/reference/dataframe/miscellaneous.rst
+-rw-r--r--   0     1001      123     1538 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/docs/source/reference/dataframe/modify_select.rst
+-rw-r--r--   0     1001      123      673 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/docs/source/reference/datatypes.rst
+-rw-r--r--   0     1001      123      421 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/docs/source/reference/exceptions.rst
+-rw-r--r--   0     1001      123      391 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/docs/source/reference/expressions/aggregation.rst
+-rw-r--r--   0     1001      123      267 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/docs/source/reference/expressions/array.rst
+-rw-r--r--   0     1001      123      309 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/docs/source/reference/expressions/binary.rst
+-rw-r--r--   0     1001      123      338 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/docs/source/reference/expressions/boolean.rst
+-rw-r--r--   0     1001      123      237 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/docs/source/reference/expressions/categories.rst
+-rw-r--r--   0     1001      123      221 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/docs/source/reference/expressions/columns.rst
+-rw-r--r--   0     1001      123     1095 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/docs/source/reference/expressions/computation.rst
+-rw-r--r--   0     1001      123     1130 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/docs/source/reference/expressions/functions.rst
+-rw-r--r--   0     1001      123      470 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/docs/source/reference/expressions/index.rst
+-rw-r--r--   0     1001      123      722 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/docs/source/reference/expressions/list.rst
+-rw-r--r--   0     1001      123      432 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/docs/source/reference/expressions/meta.rst
+-rw-r--r--   0     1001      123      159 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/docs/source/reference/expressions/miscellaneous.rst
+-rw-r--r--   0     1001      123      977 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/docs/source/reference/expressions/modify_select.rst
+-rw-r--r--   0     1001      123      679 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/docs/source/reference/expressions/operators.rst
+-rw-r--r--   0     1001      123      977 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/docs/source/reference/expressions/string.rst
+-rw-r--r--   0     1001      123      254 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/docs/source/reference/expressions/struct.rst
+-rw-r--r--   0     1001      123     1036 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/docs/source/reference/expressions/temporal.rst
+-rw-r--r--   0     1001      123       98 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/docs/source/reference/expressions/window.rst
+-rw-r--r--   0     1001      123      836 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/docs/source/reference/functions.rst
+-rw-r--r--   0     1001      123      405 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/docs/source/reference/index.rst
+-rw-r--r--   0     1001      123     1294 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/docs/source/reference/io.rst
+-rw-r--r--   0     1001      123      277 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/docs/source/reference/lazyframe/aggregation.rst
+-rw-r--r--   0     1001      123      179 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/docs/source/reference/lazyframe/attributes.rst
+-rw-r--r--   0     1001      123      146 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/docs/source/reference/lazyframe/descriptive.rst
+-rw-r--r--   0     1001      123      497 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/docs/source/reference/lazyframe/groupby.rst
+-rw-r--r--   0     1001      123      354 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/docs/source/reference/lazyframe/index.rst
+-rw-r--r--   0     1001      123      455 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/docs/source/reference/lazyframe/miscellaneous.rst
+-rw-r--r--   0     1001      123     1013 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/docs/source/reference/lazyframe/modify_select.rst
+-rw-r--r--   0     1001      123     3279 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/docs/source/reference/selectors.rst
+-rw-r--r--   0     1001      123      358 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/docs/source/reference/series/aggregation.rst
+-rw-r--r--   0     1001      123      277 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/docs/source/reference/series/array.rst
+-rw-r--r--   0     1001      123      257 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/docs/source/reference/series/attributes.rst
+-rw-r--r--   0     1001      123      321 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/docs/source/reference/series/binary.rst
+-rw-r--r--   0     1001      123      117 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/docs/source/reference/series/boolean.rst
+-rw-r--r--   0     1001      123      241 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/docs/source/reference/series/categories.rst
+-rw-r--r--   0     1001      123     1103 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/docs/source/reference/series/computation.rst
+-rw-r--r--   0     1001      123      744 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/docs/source/reference/series/descriptive.rst
+-rw-r--r--   0     1001      123      240 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/docs/source/reference/series/export.rst
+-rw-r--r--   0     1001      123      437 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/docs/source/reference/series/index.rst
+-rw-r--r--   0     1001      123      776 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/docs/source/reference/series/list.rst
+-rw-r--r--   0     1001      123      236 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/docs/source/reference/series/miscellaneous.rst
+-rw-r--r--   0     1001      123     1077 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/docs/source/reference/series/modify_select.rst
+-rw-r--r--   0     1001      123     1049 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/docs/source/reference/series/string.rst
+-rw-r--r--   0     1001      123      421 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/docs/source/reference/series/struct.rst
+-rw-r--r--   0     1001      123     1192 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/docs/source/reference/series/temporal.rst
+-rw-r--r--   0     1001      123      503 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/docs/source/reference/sql.rst
+-rw-r--r--   0     1001      123     8067 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/docs/source/reference/testing.rst
+-rw-r--r--   0     1001      123      168 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/docs/source/reference/utils.rst
+-rw-r--r--   0     1001      123     6304 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/polars/__init__.py
+-rw-r--r--   0     1001      123      280 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/polars/_reexport.py
+-rw-r--r--   0     1001      123    13229 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/polars/api.py
+-rw-r--r--   0     1001      123    29763 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/polars/config.py
+-rw-r--r--   0     1001      123    28105 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/polars/convert.py
+-rw-r--r--   0     1001      123       77 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/polars/dataframe/__init__.py
+-rw-r--r--   0     1001      123     5227 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/polars/dataframe/_html.py
+-rw-r--r--   0     1001      123   313419 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/polars/dataframe/frame.py
+-rw-r--r--   0     1001      123    40637 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/polars/dataframe/groupby.py
+-rw-r--r--   0     1001      123     2692 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/polars/datatypes/__init__.py
+-rw-r--r--   0     1001      123    17722 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/polars/datatypes/classes.py
+-rw-r--r--   0     1001      123     1603 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/polars/datatypes/constants.py
+-rw-r--r--   0     1001      123     4701 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/polars/datatypes/constructor.py
+-rw-r--r--   0     1001      123    15786 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/polars/datatypes/convert.py
+-rw-r--r--   0     1001      123     7338 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/polars/dependencies.py
+-rw-r--r--   0     1001      123     3573 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/polars/exceptions.py
+-rw-r--r--   0     1001      123       61 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/polars/expr/__init__.py
+-rw-r--r--   0     1001      123     3020 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/polars/expr/array.py
+-rw-r--r--   0     1001      123     2704 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/polars/expr/binary.py
+-rw-r--r--   0     1001      123     1698 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/polars/expr/categorical.py
+-rw-r--r--   0     1001      123    77648 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/polars/expr/datetime.py
+-rw-r--r--   0     1001      123   309474 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/polars/expr/expr.py
+-rw-r--r--   0     1001      123    23905 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/polars/expr/list.py
+-rw-r--r--   0     1001      123     4050 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/polars/expr/meta.py
+-rw-r--r--   0     1001      123    60085 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/polars/expr/string.py
+-rw-r--r--   0     1001      123     5426 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/polars/expr/struct.py
+-rw-r--r--   0     1001      123     2068 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/polars/functions/__init__.py
+-rw-r--r--   0     1001      123    16541 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/polars/functions/as_datatype.py
+-rw-r--r--   0     1001      123    18853 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/polars/functions/eager.py
+-rw-r--r--   0     1001      123    72529 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/polars/functions/lazy.py
+-rw-r--r--   0     1001      123    18145 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/polars/functions/range.py
+-rw-r--r--   0     1001      123     6027 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/polars/functions/repeat.py
+-rw-r--r--   0     1001      123     6139 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/polars/functions/whenthen.py
+-rw-r--r--   0     1001      123      952 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/polars/io/__init__.py
+-rw-r--r--   0     1001      123     6264 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/polars/io/_utils.py
+-rw-r--r--   0     1001      123      861 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/polars/io/avro.py
+-rw-r--r--   0     1001      123      144 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/polars/io/csv/__init__.py
+-rw-r--r--   0     1001      123     1072 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/polars/io/csv/_utils.py
+-rw-r--r--   0     1001      123     4681 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/polars/io/csv/batched_reader.py
+-rw-r--r--   0     1001      123    35482 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/polars/io/csv/functions.py
+-rw-r--r--   0     1001      123     5627 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/polars/io/database.py
+-rw-r--r--   0     1001      123    11047 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/polars/io/delta.py
+-rw-r--r--   0     1001      123       75 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/polars/io/excel/__init__.py
+-rw-r--r--   0     1001      123    18449 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/polars/io/excel/_write_utils.py
+-rw-r--r--   0     1001      123     6466 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/polars/io/excel/functions.py
+-rw-r--r--   0     1001      123      142 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/polars/io/ipc/__init__.py
+-rw-r--r--   0     1001      123     1227 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/polars/io/ipc/anonymous_scan.py
+-rw-r--r--   0     1001      123     5804 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/polars/io/ipc/functions.py
+-rw-r--r--   0     1001      123      502 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/polars/io/json.py
+-rw-r--r--   0     1001      123     2207 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/polars/io/ndjson.py
+-rw-r--r--   0     1001      123      170 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/polars/io/parquet/__init__.py
+-rw-r--r--   0     1001      123     1259 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/polars/io/parquet/anonymous_scan.py
+-rw-r--r--   0     1001      123     7177 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/polars/io/parquet/functions.py
+-rw-r--r--   0     1001      123      136 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/polars/io/pyarrow_dataset/__init__.py
+-rw-r--r--   0     1001      123     2186 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/polars/io/pyarrow_dataset/anonymous_scan.py
+-rw-r--r--   0     1001      123     3601 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/polars/io/pyarrow_dataset/functions.py
+-rw-r--r--   0     1001      123       77 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/polars/lazyframe/__init__.py
+-rw-r--r--   0     1001      123   169447 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/polars/lazyframe/frame.py
+-rw-r--r--   0     1001      123    24078 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/polars/lazyframe/groupby.py
+-rw-r--r--   0     1001      123        0 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/polars/py.typed
+-rw-r--r--   0     1001      123    33639 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/polars/selectors.py
+-rw-r--r--   0     1001      123       69 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/polars/series/__init__.py
+-rw-r--r--   0     1001      123     1572 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/polars/series/_numpy.py
+-rw-r--r--   0     1001      123     2515 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/polars/series/array.py
+-rw-r--r--   0     1001      123     1913 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/polars/series/binary.py
+-rw-r--r--   0     1001      123     1692 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/polars/series/categorical.py
+-rw-r--r--   0     1001      123    51825 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/polars/series/datetime.py
+-rw-r--r--   0     1001      123    13196 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/polars/series/list.py
+-rw-r--r--   0     1001      123   167432 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/polars/series/series.py
+-rw-r--r--   0     1001      123    38879 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/polars/series/string.py
+-rw-r--r--   0     1001      123     2542 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/polars/series/struct.py
+-rw-r--r--   0     1001      123     5361 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/polars/series/utils.py
+-rw-r--r--   0     1001      123     7559 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/polars/slice.py
+-rw-r--r--   0     1001      123       75 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/polars/sql/__init__.py
+-rw-r--r--   0     1001      123    17409 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/polars/sql/context.py
+-rw-r--r--   0     1001      123     4793 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/polars/string_cache.py
+-rw-r--r--   0     1001      123      362 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/polars/testing/__init__.py
+-rw-r--r--   0     1001      123     1060 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/polars/testing/_private.py
+-rw-r--r--   0     1001      123    16964 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/polars/testing/asserts.py
+-rw-r--r--   0     1001      123      898 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/polars/testing/parametric/__init__.py
+-rw-r--r--   0     1001      123    28323 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/polars/testing/parametric/primitives.py
+-rw-r--r--   0     1001      123     3409 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/polars/testing/parametric/profiles.py
+-rw-r--r--   0     1001      123    12252 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/polars/testing/parametric/strategies.py
+-rw-r--r--   0     1001      123     6304 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/polars/type_aliases.py
+-rw-r--r--   0     1001      123     1157 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/polars/utils/__init__.py
+-rw-r--r--   0     1001      123    56119 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/polars/utils/_construction.py
+-rw-r--r--   0     1001      123     4937 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/polars/utils/_parse_expr_input.py
+-rw-r--r--   0     1001      123      647 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/polars/utils/_scan.py
+-rw-r--r--   0     1001      123      579 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/polars/utils/_wrap.py
+-rw-r--r--   0     1001      123      683 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/polars/utils/build_info.py
+-rw-r--r--   0     1001      123     8716 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/polars/utils/convert.py
+-rw-r--r--   0     1001      123     7199 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/polars/utils/decorators.py
+-rw-r--r--   0     1001      123     1660 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/polars/utils/meta.py
+-rw-r--r--   0     1001      123      514 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/polars/utils/polars_version.py
+-rw-r--r--   0     1001      123     2679 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/polars/utils/show_versions.py
+-rw-r--r--   0     1001      123    12905 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/polars/utils/various.py
+-rw-r--r--   0     1001      123     5337 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/pyproject.toml
+-rw-r--r--   0     1001      123      698 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/requirements-dev.txt
+-rw-r--r--   0     1001      123       68 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/requirements-lint.txt
+-rw-r--r--   0     1001      123     1610 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/scripts/check_stacklevels.py
+-rw-r--r--   0     1001      123    10980 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/src/apply/dataframe.rs
+-rw-r--r--   0     1001      123     6428 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/src/apply/lazy.rs
+-rw-r--r--   0     1001      123     8402 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/src/apply/mod.rs
+-rw-r--r--   0     1001      123    90009 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/src/apply/series.rs
+-rw-r--r--   0     1001      123       32 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/src/arrow_interop/mod.rs
+-rw-r--r--   0     1001      123     1306 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/src/arrow_interop/to_py.rs
+-rw-r--r--   0     1001      123     3902 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/src/arrow_interop/to_rust.rs
+-rw-r--r--   0     1001      123     5250 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/src/batched_csv.rs
+-rw-r--r--   0     1001      123    48666 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/src/conversion.rs
+-rw-r--r--   0     1001      123    46071 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/src/dataframe.rs
+-rw-r--r--   0     1001      123     3950 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/src/datatypes.rs
+-rw-r--r--   0     1001      123     3288 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/src/error.rs
+-rw-r--r--   0     1001      123      570 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/src/expr/array.rs
+-rw-r--r--   0     1001      123     2080 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/src/expr/binary.rs
+-rw-r--r--   0     1001      123      274 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/src/expr/categorical.rs
+-rw-r--r--   0     1001      123     5935 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/src/expr/datetime.rs
+-rw-r--r--   0     1001      123    34093 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/src/expr/general.rs
+-rw-r--r--   0     1001      123     3937 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/src/expr/list.rs
+-rw-r--r--   0     1001      123     2907 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/src/expr/meta.rs
+-rw-r--r--   0     1001      123      870 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/src/expr/mod.rs
+-rw-r--r--   0     1001      123     8366 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/src/expr/string.rs
+-rw-r--r--   0     1001      123      467 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/src/expr/struct.rs
+-rw-r--r--   0     1001      123     9482 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/src/file.rs
+-rw-r--r--   0     1001      123     3307 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/src/functions/eager.rs
+-rw-r--r--   0     1001      123     1657 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/src/functions/io.rs
+-rw-r--r--   0     1001      123    11977 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/src/functions/lazy.rs
+-rw-r--r--   0     1001      123     1312 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/src/functions/meta.rs
+-rw-r--r--   0     1001      123      217 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/src/functions/misc.rs
+-rw-r--r--   0     1001      123       87 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/src/functions/mod.rs
+-rw-r--r--   0     1001      123     1474 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/src/functions/whenthen.rs
+-rw-r--r--   0     1001      123    30769 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/src/lazyframe.rs
+-rw-r--r--   0     1001      123     2670 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/src/lazygroupby.rs
+-rw-r--r--   0     1001      123     8268 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/src/lib.rs
+-rw-r--r--   0     1001      123     1611 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/src/object.rs
+-rw-r--r--   0     1001      123      122 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/src/prelude.rs
+-rw-r--r--   0     1001      123      435 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/src/py_modules.rs
+-rw-r--r--   0     1001      123     1964 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/src/series/aggregation.rs
+-rw-r--r--   0     1001      123     5406 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/src/series/arithmetic.rs
+-rw-r--r--   0     1001      123     5138 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/src/series/comparison.rs
+-rw-r--r--   0     1001      123     9077 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/src/series/construction.rs
+-rw-r--r--   0     1001      123     8971 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/src/series/export.rs
+-rw-r--r--   0     1001      123    26606 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/src/series/mod.rs
+-rw-r--r--   0     1001      123     4569 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/src/series/numpy_ufunc.rs
+-rw-r--r--   0     1001      123     4046 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/src/series/set_at_idx.rs
+-rw-r--r--   0     1001      123     1036 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/src/sql.rs
+-rw-r--r--   0     1001      123     2335 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/src/utils.rs
+-rw-r--r--   0     1001      123     6165 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/tests/README.md
+-rw-r--r--   0     1001      123     2189 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/tests/benchmark/groupby-datagen.R
+-rw-r--r--   0     1001      123     7963 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/tests/benchmark/run_h2oai_benchmark.py
+-rw-r--r--   0     1001      123     6530 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/tests/benchmark/test_release.py
+-rw-r--r--   0     1001      123     4589 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/tests/docs/run_doctest.py
+-rw-r--r--   0     1001      123        0 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/tests/parametric/__init__.py
+-rw-r--r--   0     1001      123      179 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/tests/parametric/conftest.py
+-rw-r--r--   0     1001      123     3856 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/tests/parametric/test_dataframe.py
+-rw-r--r--   0     1001      123     2398 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/tests/parametric/test_groupby_rolling.py
+-rw-r--r--   0     1001      123     1692 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/tests/parametric/test_lazyframe.py
+-rw-r--r--   0     1001      123      976 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/tests/parametric/test_lit.py
+-rw-r--r--   0     1001      123     6897 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/tests/parametric/test_series.py
+-rw-r--r--   0     1001      123     8299 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/tests/parametric/test_testing.py
+-rw-r--r--   0     1001      123        0 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/tests/unit/__init__.py
+-rw-r--r--   0     1001      123     3382 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/tests/unit/conftest.py
+-rw-r--r--   0     1001      123       86 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/tests/unit/datatypes/__init__.py
+-rw-r--r--   0     1001      123      973 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/tests/unit/datatypes/test_array.py
+-rw-r--r--   0     1001      123      847 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/tests/unit/datatypes/test_binary.py
+-rw-r--r--   0     1001      123     1420 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/tests/unit/datatypes/test_bool.py
+-rw-r--r--   0     1001      123    13228 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/tests/unit/datatypes/test_categorical.py
+-rw-r--r--   0     1001      123     5222 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/tests/unit/datatypes/test_decimal.py
+-rw-r--r--   0     1001      123      549 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/tests/unit/datatypes/test_duration.py
+-rw-r--r--   0     1001      123      423 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/tests/unit/datatypes/test_integer.py
+-rw-r--r--   0     1001      123    13216 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/tests/unit/datatypes/test_list.py
+-rw-r--r--   0     1001      123      284 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/tests/unit/datatypes/test_null.py
+-rw-r--r--   0     1001      123     2801 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/tests/unit/datatypes/test_object.py
+-rw-r--r--   0     1001      123    27749 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/tests/unit/datatypes/test_struct.py
+-rw-r--r--   0     1001      123    87954 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/tests/unit/datatypes/test_temporal.py
+-rw-r--r--   0     1001      123      418 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/tests/unit/datatypes/test_time.py
+-rw-r--r--   0     1001      123        0 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/tests/unit/functions/__init__.py
+-rw-r--r--   0     1001      123    13970 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/tests/unit/functions/test_as_datatype.py
+-rw-r--r--   0     1001      123      480 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/tests/unit/functions/test_concat.py
+-rw-r--r--   0     1001      123    15610 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/tests/unit/functions/test_functions.py
+-rw-r--r--   0     1001      123    18470 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/tests/unit/functions/test_range.py
+-rw-r--r--   0     1001      123     3724 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/tests/unit/functions/test_repeat.py
+-rw-r--r--   0     1001      123      218 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/tests/unit/io/conftest.py
+-rw-r--r--   0     1001      123       16 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/tests/unit/io/files/delta-table/.part-00000-e42312d7-60e5-454d-acbc-db192d220e73-c000.snappy.parquet.crc
+-rw-r--r--   0     1001      123       16 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/tests/unit/io/files/delta-table/.part-00000-e4a999da-df45-4fb0-bdc4-d999fc0f58aa-c000.snappy.parquet.crc
+-rw-r--r--   0     1001      123       16 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/tests/unit/io/files/delta-table/_delta_log/.00000000000000000000.json.crc
+-rw-r--r--   0     1001      123       16 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/tests/unit/io/files/delta-table/_delta_log/.00000000000000000001.json.crc
+-rw-r--r--   0     1001      123      905 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/tests/unit/io/files/delta-table/_delta_log/00000000000000000000.json
+-rw-r--r--   0     1001      123      936 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/tests/unit/io/files/delta-table/_delta_log/00000000000000000001.json
+-rw-r--r--   0     1001      123      972 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/tests/unit/io/files/delta-table/part-00000-e42312d7-60e5-454d-acbc-db192d220e73-c000.snappy.parquet
+-rw-r--r--   0     1001      123      690 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/tests/unit/io/files/delta-table/part-00000-e4a999da-df45-4fb0-bdc4-d999fc0f58aa-c000.snappy.parquet
+-rw-r--r--   0     1001      123        0 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/tests/unit/io/files/empty.csv
+-rw-r--r--   0     1001      123     5959 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/tests/unit/io/files/example.xlsx
+-rw-r--r--   0     1001      123      457 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/tests/unit/io/files/foods1.csv
+-rw-r--r--   0     1001      123     2351 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/tests/unit/io/files/foods1.ipc
+-rw-r--r--   0     1001      123     1713 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/tests/unit/io/files/foods1.ndjson
+-rw-r--r--   0     1001      123     1427 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/tests/unit/io/files/foods1.parquet
+-rw-r--r--   0     1001      123      455 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/tests/unit/io/files/foods2.csv
+-rw-r--r--   0     1001      123     2351 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/tests/unit/io/files/foods2.ipc
+-rw-r--r--   0     1001      123     1711 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/tests/unit/io/files/foods2.ndjson
+-rw-r--r--   0     1001      123     1916 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/tests/unit/io/files/foods2.parquet
+-rw-r--r--   0     1001      123      455 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/tests/unit/io/files/foods3.csv
+-rw-r--r--   0     1001      123      457 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/tests/unit/io/files/foods4.csv
+-rw-r--r--   0     1001      123      452 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/tests/unit/io/files/foods5.csv
+-rw-r--r--   0     1001      123       49 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/tests/unit/io/files/gzipped.csv
+-rw-r--r--   0     1001      123       57 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/tests/unit/io/files/small.csv
+-rw-r--r--   0     1001      123      756 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/tests/unit/io/files/small.parquet
+-rw-r--r--   0     1001      123     1884 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/tests/unit/io/test_avro.py
+-rw-r--r--   0     1001      123    40088 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/tests/unit/io/test_csv.py
+-rw-r--r--   0     1001      123     6336 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/tests/unit/io/test_database.py
+-rw-r--r--   0     1001      123     6172 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/tests/unit/io/test_delta.py
+-rw-r--r--   0     1001      123    11169 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/tests/unit/io/test_excel.py
+-rw-r--r--   0     1001      123     5483 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/tests/unit/io/test_ipc.py
+-rw-r--r--   0     1001      123     3986 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/tests/unit/io/test_json.py
+-rw-r--r--   0     1001      123     7379 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/tests/unit/io/test_lazy_csv.py
+-rw-r--r--   0     1001      123     2060 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/tests/unit/io/test_lazy_ipc.py
+-rw-r--r--   0     1001      123     2867 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/tests/unit/io/test_lazy_json.py
+-rw-r--r--   0     1001      123    11145 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/tests/unit/io/test_lazy_parquet.py
+-rw-r--r--   0     1001      123     2012 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/tests/unit/io/test_other.py
+-rw-r--r--   0     1001      123    14201 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/tests/unit/io/test_parquet.py
+-rw-r--r--   0     1001      123      612 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/tests/unit/io/test_pickle.py
+-rw-r--r--   0     1001      123     3686 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/tests/unit/io/test_pyarrow_dataset.py
+-rw-r--r--   0     1001      123      509 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/tests/unit/namespaces/__init__.py
+-rw-r--r--   0     1001      123      589 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/tests/unit/namespaces/test_array.py
+-rw-r--r--   0     1001      123     3218 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/tests/unit/namespaces/test_binary.py
+-rw-r--r--   0     1001      123     2489 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/tests/unit/namespaces/test_categorical.py
+-rw-r--r--   0     1001      123    20480 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/tests/unit/namespaces/test_datetime.py
+-rw-r--r--   0     1001      123    14067 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/tests/unit/namespaces/test_list.py
+-rw-r--r--   0     1001      123     1829 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/tests/unit/namespaces/test_meta.py
+-rw-r--r--   0     1001      123    24050 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/tests/unit/namespaces/test_string.py
+-rw-r--r--   0     1001      123    19038 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/tests/unit/namespaces/test_strptime.py
+-rw-r--r--   0     1001      123      982 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/tests/unit/namespaces/test_struct.py
+-rw-r--r--   0     1001      123       85 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/tests/unit/operations/__init__.py
+-rw-r--r--   0     1001      123     7755 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/tests/unit/operations/test_aggregations.py
+-rw-r--r--   0     1001      123    10643 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/tests/unit/operations/test_apply.py
+-rw-r--r--   0     1001      123     6932 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/tests/unit/operations/test_arithmetic.py
+-rw-r--r--   0     1001      123     4631 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/tests/unit/operations/test_comparison.py
+-rw-r--r--   0     1001      123     3275 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/tests/unit/operations/test_drop.py
+-rw-r--r--   0     1001      123     8813 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/tests/unit/operations/test_explode.py
+-rw-r--r--   0     1001      123     3664 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/tests/unit/operations/test_filter.py
+-rw-r--r--   0     1001      123     1801 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/tests/unit/operations/test_folds.py
+-rw-r--r--   0     1001      123    25037 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/tests/unit/operations/test_groupby.py
+-rw-r--r--   0     1001      123     7649 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/tests/unit/operations/test_groupby_rolling.py
+-rw-r--r--   0     1001      123     2983 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/tests/unit/operations/test_is_in.py
+-rw-r--r--   0     1001      123    18169 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/tests/unit/operations/test_join.py
+-rw-r--r--   0     1001      123    14952 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/tests/unit/operations/test_join_asof.py
+-rw-r--r--   0     1001      123      643 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/tests/unit/operations/test_melt.py
+-rw-r--r--   0     1001      123    10253 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/tests/unit/operations/test_pivot.py
+-rw-r--r--   0     1001      123    24216 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/tests/unit/operations/test_rolling.py
+-rw-r--r--   0     1001      123     2389 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/tests/unit/operations/test_select.py
+-rw-r--r--   0     1001      123    20770 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/tests/unit/operations/test_sort.py
+-rw-r--r--   0     1001      123     4273 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/tests/unit/operations/test_statistics.py
+-rw-r--r--   0     1001      123     4130 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/tests/unit/operations/test_transpose.py
+-rw-r--r--   0     1001      123      771 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/tests/unit/operations/test_unique.py
+-rw-r--r--   0     1001      123    11694 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/tests/unit/operations/test_window.py
+-rw-r--r--   0     1001      123     5480 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/tests/unit/operations/test_with_columns.py
+-rw-r--r--   0     1001      123        0 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/tests/unit/streaming/__init__.py
+-rw-r--r--   0     1001      123      196 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/tests/unit/streaming/conftest.py
+-rw-r--r--   0     1001      123      908 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/tests/unit/streaming/test_ooc.py
+-rw-r--r--   0     1001      123    18757 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/tests/unit/streaming/test_streaming.py
+-rw-r--r--   0     1001      123     4775 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/tests/unit/test_api.py
+-rw-r--r--   0     1001      123     1969 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/tests/unit/test_arity.py
+-rw-r--r--   0     1001      123    20333 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/tests/unit/test_cfg.py
+-rw-r--r--   0     1001      123    42903 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/tests/unit/test_constructors.py
+-rw-r--r--   0     1001      123      454 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/tests/unit/test_context.py
+-rw-r--r--   0     1001      123     1628 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/tests/unit/test_cse.py
+-rw-r--r--   0     1001      123     5198 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/tests/unit/test_datatypes.py
+-rw-r--r--   0     1001      123   120498 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/tests/unit/test_df.py
+-rw-r--r--   0     1001      123     2396 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/tests/unit/test_empty.py
+-rw-r--r--   0     1001      123    18809 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/tests/unit/test_errors.py
+-rw-r--r--   0     1001      123     2741 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/tests/unit/test_expr_multi_cols.py
+-rw-r--r--   0     1001      123    35226 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/tests/unit/test_exprs.py
+-rw-r--r--   0     1001      123     3516 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/tests/unit/test_fmt.py
+-rw-r--r--   0     1001      123     3763 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/tests/unit/test_interchange.py
+-rw-r--r--   0     1001      123    38286 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/tests/unit/test_interop.py
+-rw-r--r--   0     1001      123    49654 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/tests/unit/test_lazy.py
+-rw-r--r--   0     1001      123     2463 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/tests/unit/test_polars_import.py
+-rw-r--r--   0     1001      123     4610 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/tests/unit/test_predicates.py
+-rw-r--r--   0     1001      123     7073 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/tests/unit/test_projections.py
+-rw-r--r--   0     1001      123    11551 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/tests/unit/test_queries.py
+-rw-r--r--   0     1001      123     4743 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/tests/unit/test_rows.py
+-rw-r--r--   0     1001      123    13987 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/tests/unit/test_schema.py
+-rw-r--r--   0     1001      123     9431 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/tests/unit/test_selectors.py
+-rw-r--r--   0     1001      123     3816 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/tests/unit/test_serde.py
+-rw-r--r--   0     1001      123    84086 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/tests/unit/test_series.py
+-rw-r--r--   0     1001      123      657 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/tests/unit/test_single.py
+-rw-r--r--   0     1001      123    16616 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/tests/unit/test_sql.py
+-rw-r--r--   0     1001      123    35314 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/tests/unit/test_testing.py
+-rw-r--r--   0     1001      123       41 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/tests/unit/utils/__init__.py
+-rw-r--r--   0     1001      123      306 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/tests/unit/utils/test_build_info.py
+-rw-r--r--   0     1001      123     2855 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/tests/unit/utils/test_parse_expr_input.py
+-rw-r--r--   0     1001      123      247 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/tests/unit/utils/test_show_versions.py
+-rw-r--r--   0     1001      123     5026 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/tests/unit/utils/test_utils.py
+-rw-r--r--   0     1001      123    63897 2023-06-23 15:05:52.000000 polars_u64_idx-0.18.4/Cargo.lock
+-rw-r--r--   0        0        0    14553 1970-01-01 00:00:00.000000 polars_u64_idx-0.18.4/PKG-INFO
```

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-io/Cargo.toml` & `polars_u64_idx-0.18.4/local_dependencies/polars-io/Cargo.toml`

 * *Files 0% similar despite different names*

```diff
@@ -80,19 +80,19 @@
 simd-json = { version = "0.10", optional = true, features = ["allow-non-simd", "known-key"] }
 simdutf8 = { version = "0.1", optional = true }
 tokio = { version = "1.26.0", features = ["net"], optional = true }
 url = { version = "2.3.1", optional = true }
 
 [dependencies.arrow]
 package = "arrow2"
-git = "https://github.com/jorgecarleitao/arrow2"
-# git = "https://github.com/ritchie46/arrow2"
-rev = "2d2e7053f9a50810bfe9cecff25ab39089aef98e"
+# git = "https://github.com/jorgecarleitao/arrow2"
+git = "https://github.com/ritchie46/arrow2"
+# rev = "2d2e7053f9a50810bfe9cecff25ab39089aef98e"
 # path = "../arrow2"
-# branch = "polars_2023-05-25"
+branch = "polars_2023-06-23"
 version = "0.17"
 default-features = false
 features = [
   "compute_aggregate",
   "compute_arithmetics",
   "compute_boolean",
   "compute_boolean_kleene",
```

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-io/LICENSE` & `polars_u64_idx-0.18.4/local_dependencies/polars-json/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-io/src/avro/mod.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-io/src/avro/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-io/src/avro/read.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-io/src/avro/read.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-io/src/avro/write.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-io/src/avro/write.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-io/src/cloud/adaptors.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-io/src/cloud/adaptors.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-io/src/cloud/glob.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-io/src/cloud/glob.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-io/src/cloud/mod.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-io/src/cloud/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-io/src/csv/buffer.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-io/src/csv/buffer.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 use arrow::array::Utf8Array;
 use arrow::bitmap::MutableBitmap;
 use polars_arrow::prelude::FromDataUtf8;
 use polars_core::prelude::*;
 #[cfg(any(feature = "dtype-datetime", feature = "dtype-date"))]
 use polars_time::chunkedarray::utf8::Pattern;
 #[cfg(any(feature = "dtype-datetime", feature = "dtype-date"))]
-use polars_time::prelude::utf8::infer::{infer_pattern_single, DatetimeInfer, StrpTimeParser};
+use polars_time::prelude::utf8::infer::{
+    infer_pattern_single, DatetimeInfer, StrpTimeParser, TryFromWithUnit,
+};
 
 use crate::csv::parser::{is_whitespace, skip_whitespace};
 use crate::csv::read_impl::RunningSize;
 use crate::csv::utils::escape_field;
 use crate::csv::CsvEncoding;
 
 pub(crate) trait PrimitiveParser: PolarsNumericType {
@@ -57,28 +59,30 @@
 trait ParsedBuffer {
     fn parse_bytes(
         &mut self,
         bytes: &[u8],
         ignore_errors: bool,
         _needs_escaping: bool,
         _missing_is_null: bool,
+        _time_unit: Option<TimeUnit>,
     ) -> PolarsResult<()>;
 }
 
 impl<T> ParsedBuffer for PrimitiveChunkedBuilder<T>
 where
     T: PolarsNumericType + PrimitiveParser,
 {
     #[inline]
     fn parse_bytes(
         &mut self,
         bytes: &[u8],
         ignore_errors: bool,
         needs_escaping: bool,
         _missing_is_null: bool,
+        _time_unit: Option<TimeUnit>,
     ) -> PolarsResult<()> {
         if bytes.is_empty() {
             self.append_null()
         } else {
             let bytes = if needs_escaping {
                 &bytes[1..bytes.len() - 1]
             } else {
@@ -96,14 +100,15 @@
                     if !bytes.is_empty() && is_whitespace(bytes[0]) {
                         let bytes = skip_whitespace(bytes);
                         return self.parse_bytes(
                             bytes,
                             ignore_errors,
                             false, // escaping was already done
                             _missing_is_null,
+                            None,
                         );
                     }
                     polars_ensure!(
                         bytes.is_empty() || ignore_errors,
                         ComputeError: "remaining bytes non-empty",
                     );
                     self.append_null()
@@ -165,14 +170,15 @@
     #[inline]
     fn parse_bytes(
         &mut self,
         bytes: &[u8],
         ignore_errors: bool,
         needs_escaping: bool,
         missing_is_null: bool,
+        _time_unit: Option<TimeUnit>,
     ) -> PolarsResult<()> {
         if bytes.is_empty() {
             // append null
             self.offsets.push(self.data.len() as i64);
             self.validity.push(!missing_is_null);
             return Ok(());
         }
@@ -273,14 +279,15 @@
     #[inline]
     fn parse_bytes(
         &mut self,
         bytes: &'a [u8],
         ignore_errors: bool,
         needs_escaping: bool,
         _missing_is_null: bool,
+        _time_unit: Option<TimeUnit>,
     ) -> PolarsResult<()> {
         if bytes.is_empty() {
             self.builder.append_null();
             return Ok(());
         }
 
         if validate_utf8(bytes) {
@@ -356,14 +363,15 @@
     #[inline]
     fn parse_bytes(
         &mut self,
         bytes: &[u8],
         ignore_errors: bool,
         needs_escaping: bool,
         _missing_is_null: bool,
+        _time_unit: Option<TimeUnit>,
     ) -> PolarsResult<()> {
         let bytes = if needs_escaping {
             &bytes[1..bytes.len() - 1]
         } else {
             bytes
         };
         if bytes.eq_ignore_ascii_case(b"false") {
@@ -399,19 +407,20 @@
     }
 }
 
 #[cfg(any(feature = "dtype-datetime", feature = "dtype-date"))]
 fn slow_datetime_parser<T>(
     buf: &mut DatetimeField<T>,
     bytes: &[u8],
+    time_unit: Option<TimeUnit>,
     ignore_errors: bool,
 ) -> PolarsResult<()>
 where
     T: PolarsNumericType,
-    DatetimeInfer<T::Native>: TryFrom<Pattern>,
+    DatetimeInfer<T::Native>: TryFromWithUnit<Pattern>,
 {
     let val = if bytes.is_ascii() {
         // Safety:
         // we just checked it is ascii
         unsafe { std::str::from_utf8_unchecked(bytes) }
     } else if ignore_errors {
         buf.builder.append_null();
@@ -429,15 +438,15 @@
             Some(pattern) => pattern,
             None => {
                 buf.builder.append_null();
                 return Ok(());
             }
         },
     };
-    match DatetimeInfer::<T::Native>::try_from(pattern) {
+    match DatetimeInfer::<T::Native>::try_from_with_unit(pattern, time_unit) {
         Ok(mut infer) => {
             let parsed = infer.parse(val);
             buf.compiled = Some(infer);
             buf.builder.append_option(parsed);
             Ok(())
         }
         Err(_) => {
@@ -447,40 +456,41 @@
     }
 }
 
 #[cfg(any(feature = "dtype-datetime", feature = "dtype-date"))]
 impl<T> ParsedBuffer for DatetimeField<T>
 where
     T: PolarsNumericType,
-    DatetimeInfer<T::Native>: TryFrom<Pattern> + StrpTimeParser<T::Native>,
+    DatetimeInfer<T::Native>: TryFromWithUnit<Pattern> + StrpTimeParser<T::Native>,
 {
     #[inline]
     fn parse_bytes(
         &mut self,
         mut bytes: &[u8],
         ignore_errors: bool,
         needs_escaping: bool,
         _missing_is_null: bool,
+        time_unit: Option<TimeUnit>,
     ) -> PolarsResult<()> {
         if needs_escaping && bytes.len() > 2 {
             bytes = &bytes[1..bytes.len() - 1]
         }
 
         match &mut self.compiled {
-            None => slow_datetime_parser(self, bytes, ignore_errors),
+            None => slow_datetime_parser(self, bytes, time_unit, ignore_errors),
             Some(compiled) => {
-                match compiled.parse_bytes(bytes) {
+                match compiled.parse_bytes(bytes, time_unit) {
                     Some(parsed) => {
                         self.builder.append_value(parsed);
                         Ok(())
                     }
                     // fall back on chrono parser
                     // this is a lot slower, we need to do utf8 checking and use
                     // the slower parser
-                    None => slow_datetime_parser(self, bytes, ignore_errors),
+                    None => slow_datetime_parser(self, bytes, time_unit, ignore_errors),
                 }
             }
         }
     }
 }
 
 pub(crate) fn init_buffers<'a>(
@@ -723,85 +733,97 @@
         match self {
             Boolean(buf) => <BooleanChunkedBuilder as ParsedBuffer>::parse_bytes(
                 buf,
                 bytes,
                 ignore_errors,
                 needs_escaping,
                 missing_is_null,
+                None,
             ),
             Int32(buf) => <PrimitiveChunkedBuilder<Int32Type> as ParsedBuffer>::parse_bytes(
                 buf,
                 bytes,
                 ignore_errors,
                 needs_escaping,
                 missing_is_null,
+                None,
             ),
             Int64(buf) => <PrimitiveChunkedBuilder<Int64Type> as ParsedBuffer>::parse_bytes(
                 buf,
                 bytes,
                 ignore_errors,
                 needs_escaping,
                 missing_is_null,
+                None,
             ),
             UInt64(buf) => <PrimitiveChunkedBuilder<UInt64Type> as ParsedBuffer>::parse_bytes(
                 buf,
                 bytes,
                 ignore_errors,
                 needs_escaping,
                 missing_is_null,
+                None,
             ),
             UInt32(buf) => <PrimitiveChunkedBuilder<UInt32Type> as ParsedBuffer>::parse_bytes(
                 buf,
                 bytes,
                 ignore_errors,
                 needs_escaping,
                 missing_is_null,
+                None,
             ),
             Float32(buf) => <PrimitiveChunkedBuilder<Float32Type> as ParsedBuffer>::parse_bytes(
                 buf,
                 bytes,
                 ignore_errors,
                 needs_escaping,
                 missing_is_null,
+                None,
             ),
             Float64(buf) => <PrimitiveChunkedBuilder<Float64Type> as ParsedBuffer>::parse_bytes(
                 buf,
                 bytes,
                 ignore_errors,
                 needs_escaping,
                 missing_is_null,
+                None,
             ),
             Utf8(buf) => <Utf8Field as ParsedBuffer>::parse_bytes(
                 buf,
                 bytes,
                 ignore_errors,
                 needs_escaping,
                 missing_is_null,
+                None,
             ),
             #[cfg(feature = "dtype-datetime")]
-            Datetime { buf, .. } => <DatetimeField<Int64Type> as ParsedBuffer>::parse_bytes(
-                buf,
-                bytes,
-                ignore_errors,
-                needs_escaping,
-                missing_is_null,
-            ),
+            Datetime { buf, time_unit, .. } => {
+                <DatetimeField<Int64Type> as ParsedBuffer>::parse_bytes(
+                    buf,
+                    bytes,
+                    ignore_errors,
+                    needs_escaping,
+                    missing_is_null,
+                    Some(*time_unit),
+                )
+            }
             #[cfg(feature = "dtype-date")]
             Date(buf) => <DatetimeField<Int32Type> as ParsedBuffer>::parse_bytes(
                 buf,
                 bytes,
                 ignore_errors,
                 needs_escaping,
                 missing_is_null,
+                None,
             ),
             #[allow(unused_variables)]
             Categorical(buf) => {
                 #[cfg(feature = "dtype-categorical")]
                 {
-                    buf.parse_bytes(bytes, ignore_errors, needs_escaping, missing_is_null)
+                    buf.parse_bytes(bytes, ignore_errors, needs_escaping, missing_is_null, None)
                 }
 
                 #[cfg(not(feature = "dtype-categorical"))]
                 {
                     panic!("activate 'dtype-categorical' feature")
                 }
             }
```

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-io/src/csv/mod.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-io/src/csv/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-io/src/csv/parser.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-io/src/csv/parser.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-io/src/csv/read.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-io/src/csv/read.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-io/src/csv/read_impl/batched_mmap.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-io/src/csv/read_impl/batched_mmap.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-io/src/csv/read_impl/batched_read.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-io/src/csv/read_impl/batched_read.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-io/src/csv/read_impl/mod.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-io/src/csv/read_impl/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-io/src/csv/splitfields.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-io/src/csv/splitfields.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-io/src/csv/utils.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-io/src/csv/utils.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-io/src/csv/write.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-io/src/csv/write.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-io/src/csv/write_impl.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-io/src/csv/write_impl.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-io/src/ipc/ipc_file.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-io/src/ipc/ipc_file.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-io/src/ipc/ipc_stream.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-io/src/ipc/ipc_stream.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-io/src/ipc/mmap.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-io/src/ipc/mmap.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-io/src/ipc/write.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-io/src/ipc/write.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-io/src/ipc/write_async.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-io/src/ipc/write_async.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-io/src/json/mod.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-io/src/json/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-io/src/lib.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-io/src/lib.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-io/src/mmap.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-io/src/mmap.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-io/src/ndjson/buffer.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-io/src/ndjson/buffer.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 use std::hash::{Hash, Hasher};
 
 use arrow::types::NativeType;
 use num_traits::NumCast;
 use polars_core::frame::row::AnyValueBuffer;
 use polars_core::prelude::*;
 #[cfg(any(feature = "dtype-datetime", feature = "dtype-date"))]
-use polars_time::prelude::utf8::infer::{infer_pattern_single, DatetimeInfer};
+use polars_time::prelude::utf8::infer::{infer_pattern_single, DatetimeInfer, TryFromWithUnit};
 #[cfg(any(feature = "dtype-datetime", feature = "dtype-date"))]
 use polars_time::prelude::utf8::Pattern;
 use simd_json::{BorrowedValue as Value, KnownKey, StaticNode};
 
 #[derive(Debug, Clone, PartialEq)]
 pub(crate) struct BufferKey<'a>(pub(crate) KnownKey<'a>);
 impl<'a> Eq for BufferKey<'a> {}
@@ -144,22 +144,23 @@
     }
 }
 
 #[cfg(feature = "dtype-datetime")]
 fn deserialize_datetime<T>(value: &Value) -> Option<T::Native>
 where
     T: PolarsNumericType,
-    DatetimeInfer<T::Native>: TryFrom<Pattern>,
+    DatetimeInfer<T::Native>: TryFromWithUnit<Pattern>,
 {
     let val = match value {
         Value::String(s) => s,
         _ => return None,
     };
     infer_pattern_single(val).and_then(|pattern| {
-        match DatetimeInfer::<T::Native>::try_from(pattern) {
+        match DatetimeInfer::<T::Native>::try_from_with_unit(pattern, Some(TimeUnit::Microseconds))
+        {
             Ok(mut infer) => infer.parse(val),
             Err(_) => None,
         }
     })
 }
 
 fn deserialize_all<'a>(json: &Value, dtype: &DataType) -> PolarsResult<AnyValue<'a>> {
```

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-io/src/ndjson/core.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-io/src/ndjson/core.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-io/src/parquet/async_impl.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-io/src/parquet/async_impl.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-io/src/parquet/mmap.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-io/src/parquet/mmap.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-io/src/parquet/mod.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-io/src/parquet/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-io/src/parquet/predicates.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-io/src/parquet/predicates.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-io/src/parquet/read.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-io/src/parquet/read.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-io/src/parquet/read_impl.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-io/src/parquet/read_impl.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-io/src/parquet/write.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-io/src/parquet/write.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-io/src/partition.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-io/src/partition.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-io/src/predicates.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-io/src/predicates.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-io/src/prelude.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-io/src/prelude.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-io/src/utils.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-io/src/utils.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-error/Cargo.toml` & `polars_u64_idx-0.18.4/local_dependencies/polars-row/Cargo.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 [package]
-name = "polars-error"
-version = "0.30.0"
+name = "polars-row"
+version= "0.30.0"
 edition = "2021"
 license = "MIT"
 repository = "https://github.com/pola-rs/polars"
-description = "Error definitions for the Polars DataFrame library"
+description = "Row encodings for the Polars DataFrame library"
 resolver = "2"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 
 [dependencies]
-regex = { version = "1.6", optional = true }
-thiserror= "^1"
+polars-error = { version = "0.30.0", path = "../polars-error" }
+polars-utils = { version = "0.30.0", path = "../polars-utils" }
 
 [dependencies.arrow]
 package = "arrow2"
-git = "https://github.com/jorgecarleitao/arrow2"
-# git = "https://github.com/ritchie46/arrow2"
-rev = "2d2e7053f9a50810bfe9cecff25ab39089aef98e"
+# git = "https://github.com/jorgecarleitao/arrow2"
+git = "https://github.com/ritchie46/arrow2"
+# rev = "2d2e7053f9a50810bfe9cecff25ab39089aef98e"
 # path = "../arrow2"
-# branch = "polars_2023-05-25"
+branch = "polars_2023-06-23"
 version = "0.17"
 default-features = false
 features = [
   "compute_aggregate",
   "compute_arithmetics",
   "compute_boolean",
   "compute_boolean_kleene",
```

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-error/LICENSE` & `polars_u64_idx-0.18.4/local_dependencies/polars-error/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-error/src/lib.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-error/src/lib.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 use std::borrow::Cow;
+use std::error::Error;
 use std::fmt::{self, Display, Formatter};
 use std::ops::Deref;
 use std::{env, io};
 
 #[derive(Debug)]
 pub struct ErrString(Cow<'static, str>);
 
@@ -91,14 +92,18 @@
             SchemaMismatch(msg) => SchemaMismatch(func(msg).into()),
             ShapeMismatch(msg) => ShapeMismatch(func(msg).into()),
             StructFieldNotFound(msg) => StructFieldNotFound(func(msg).into()),
         }
     }
 }
 
+pub fn map_err<E: Error>(error: E) -> PolarsError {
+    PolarsError::ComputeError(format!("{error}").into())
+}
+
 #[macro_export]
 macro_rules! polars_err {
     ($variant:ident: $err:expr $(,)?) => {
         $crate::__private::must_use(
             $crate::PolarsError::$variant($err.into())
         )
     };
```

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-plan/Cargo.toml` & `polars_u64_idx-0.18.4/local_dependencies/polars-plan/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 
 [dependencies]
 ahash= "0.8"
 chrono = { version = "0.4", optional = true }
 chrono-tz = { version = "0.8", optional = true }
+ciborium = { version = "0.2", optional = true }
 futures = { version = "0.3.25", optional = true }
 once_cell= "1"
 polars-arrow = { version = "0.30.0", path = "../polars-arrow" }
 polars-core = { version = "0.30.0", path = "../polars-core", features = ["lazy", "zip_with", "random"], default-features = false }
 polars-io = { version = "0.30.0", path = "../polars-io", features = ["lazy", "csv"], default-features = false }
 polars-ops = { version = "0.30.0", path = "../polars-ops", default-features = false }
 polars-time = { version = "0.30.0", path = "../polars-time", optional = true }
@@ -26,15 +27,15 @@
 regex = { version = "1.6", optional = true }
 serde = { version = "1", features = ["derive", "rc"], optional = true }
 smartstring= { version = "1" }
 
 [features]
 # debugging utility
 debugging = []
-python = ["pyo3"]
+python = ["pyo3", "ciborium"]
 # make sure we don't compile unneeded things even though
 # this dependency gets activated
 compile = []
 default = ["compile"]
 streaming = []
 parquet = ["polars-core/parquet", "polars-io/parquet"]
 async = []
@@ -63,14 +64,16 @@
 list_take = ["polars-ops/list_take"]
 list_count = ["polars-ops/list_count"]
 trigonometry = []
 sign = []
 timezones = ["chrono-tz", "polars-time/timezones", "polars-core/timezones", "regex"]
 binary_encoding = ["polars-ops/binary_encoding"]
 true_div = []
+nightly = ["polars-utils/nightly", "polars-ops/nightly"]
+extract_jsonpath = []
 
 # operations
 approx_unique = ["polars-ops/approx_unique"]
 is_in = ["polars-core/is_in"]
 repeat_by = ["polars-core/repeat_by"]
 round_series = ["polars-core/round_series"]
 is_first = ["polars-core/is_first", "polars-ops/is_first"]
@@ -123,19 +126,19 @@
 [package.metadata.docs.rs]
 all-features = true
 # defines the configuration attribute `docsrs`
 rustdoc-args = ["--cfg", "docsrs"]
 
 [dependencies.arrow]
 package = "arrow2"
-git = "https://github.com/jorgecarleitao/arrow2"
-# git = "https://github.com/ritchie46/arrow2"
-rev = "2d2e7053f9a50810bfe9cecff25ab39089aef98e"
+# git = "https://github.com/jorgecarleitao/arrow2"
+git = "https://github.com/ritchie46/arrow2"
+# rev = "2d2e7053f9a50810bfe9cecff25ab39089aef98e"
 # path = "../arrow2"
-# branch = "polars_2023-05-25"
+branch = "polars_2023-06-23"
 version = "0.17"
 default-features = false
 features = [
   "compute_aggregate",
   "compute_arithmetics",
   "compute_boolean",
   "compute_boolean_kleene",
```

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-plan/LICENSE` & `polars_u64_idx-0.18.4/local_dependencies/polars-plan/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/dot.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/dot.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/dsl/arithmetic.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/dsl/arithmetic.rs`

 * *Files 9% similar despite different names*

```diff
@@ -57,85 +57,103 @@
             options: FunctionOptions {
                 collect_groups: ApplyOptions::ApplyFlat,
                 ..Default::default()
             },
         }
     }
 
-    /// Compute the sine of the given expression
-    #[cfg(feature = "trigonometry")]
-    pub fn sin(self) -> Self {
-        self.map_private(FunctionExpr::Trigonometry(TrigonometricFunction::Sin))
-    }
-
     /// Compute the cosine of the given expression
     #[cfg(feature = "trigonometry")]
     pub fn cos(self) -> Self {
         self.map_private(FunctionExpr::Trigonometry(TrigonometricFunction::Cos))
     }
 
-    /// Compute the tangent of the given expression
+    /// Compute the cotangent of the given expression
     #[cfg(feature = "trigonometry")]
-    pub fn tan(self) -> Self {
-        self.map_private(FunctionExpr::Trigonometry(TrigonometricFunction::Tan))
+    pub fn cot(self) -> Self {
+        self.map_private(FunctionExpr::Trigonometry(TrigonometricFunction::Cot))
     }
 
-    /// Compute the inverse sine of the given expression
+    /// Compute the sine of the given expression
     #[cfg(feature = "trigonometry")]
-    pub fn arcsin(self) -> Self {
-        self.map_private(FunctionExpr::Trigonometry(TrigonometricFunction::ArcSin))
+    pub fn sin(self) -> Self {
+        self.map_private(FunctionExpr::Trigonometry(TrigonometricFunction::Sin))
+    }
+
+    /// Compute the tangent of the given expression
+    #[cfg(feature = "trigonometry")]
+    pub fn tan(self) -> Self {
+        self.map_private(FunctionExpr::Trigonometry(TrigonometricFunction::Tan))
     }
 
     /// Compute the inverse cosine of the given expression
     #[cfg(feature = "trigonometry")]
     pub fn arccos(self) -> Self {
         self.map_private(FunctionExpr::Trigonometry(TrigonometricFunction::ArcCos))
     }
 
-    /// Compute the inverse tangent of the given expression
+    /// Compute the inverse sine of the given expression
     #[cfg(feature = "trigonometry")]
-    pub fn arctan(self) -> Self {
-        self.map_private(FunctionExpr::Trigonometry(TrigonometricFunction::ArcTan))
+    pub fn arcsin(self) -> Self {
+        self.map_private(FunctionExpr::Trigonometry(TrigonometricFunction::ArcSin))
     }
 
-    /// Compute the hyperbolic sine of the given expression
+    /// Compute the inverse tangent of the given expression
     #[cfg(feature = "trigonometry")]
-    pub fn sinh(self) -> Self {
-        self.map_private(FunctionExpr::Trigonometry(TrigonometricFunction::Sinh))
+    pub fn arctan(self) -> Self {
+        self.map_private(FunctionExpr::Trigonometry(TrigonometricFunction::ArcTan))
     }
 
     /// Compute the hyperbolic cosine of the given expression
     #[cfg(feature = "trigonometry")]
     pub fn cosh(self) -> Self {
         self.map_private(FunctionExpr::Trigonometry(TrigonometricFunction::Cosh))
     }
 
-    /// Compute the hyperbolic tangent of the given expression
+    /// Compute the hyperbolic sine of the given expression
     #[cfg(feature = "trigonometry")]
-    pub fn tanh(self) -> Self {
-        self.map_private(FunctionExpr::Trigonometry(TrigonometricFunction::Tanh))
+    pub fn sinh(self) -> Self {
+        self.map_private(FunctionExpr::Trigonometry(TrigonometricFunction::Sinh))
     }
 
-    /// Compute the inverse hyperbolic sine of the given expression
+    /// Compute the hyperbolic tangent of the given expression
     #[cfg(feature = "trigonometry")]
-    pub fn arcsinh(self) -> Self {
-        self.map_private(FunctionExpr::Trigonometry(TrigonometricFunction::ArcSinh))
+    pub fn tanh(self) -> Self {
+        self.map_private(FunctionExpr::Trigonometry(TrigonometricFunction::Tanh))
     }
 
     /// Compute the inverse hyperbolic cosine of the given expression
     #[cfg(feature = "trigonometry")]
     pub fn arccosh(self) -> Self {
         self.map_private(FunctionExpr::Trigonometry(TrigonometricFunction::ArcCosh))
     }
 
+    /// Compute the inverse hyperbolic sine of the given expression
+    #[cfg(feature = "trigonometry")]
+    pub fn arcsinh(self) -> Self {
+        self.map_private(FunctionExpr::Trigonometry(TrigonometricFunction::ArcSinh))
+    }
+
     /// Compute the inverse hyperbolic tangent of the given expression
     #[cfg(feature = "trigonometry")]
     pub fn arctanh(self) -> Self {
         self.map_private(FunctionExpr::Trigonometry(TrigonometricFunction::ArcTanh))
     }
 
+    /// Convert from radians to degrees
+    #[cfg(feature = "trigonometry")]
+    pub fn degrees(self) -> Self {
+        self.map_private(FunctionExpr::Trigonometry(TrigonometricFunction::Degrees))
+    }
+
+    /// Convert from degrees to radians
+    #[cfg(feature = "trigonometry")]
+    pub fn radians(self) -> Self {
+        self.map_private(FunctionExpr::Trigonometry(TrigonometricFunction::Radians))
+    }
+
     /// Compute the sign of the given expression
     #[cfg(feature = "sign")]
     pub fn sign(self) -> Self {
         self.map_private(FunctionExpr::Sign)
     }
 }
```

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/dsl/arity.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/dsl/arity.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/dsl/array.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/dsl/array.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/dsl/binary.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/dsl/binary.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/dsl/cat.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/dsl/cat.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/dsl/dt.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/dsl/dt.rs`

 * *Files 1% similar despite different names*

```diff
@@ -142,18 +142,18 @@
     /// Returns the ISO week number starting from 1.
     /// The return value ranges from 1 to 53. (The last week of year differs by years.)
     pub fn week(self) -> Expr {
         self.0
             .map_private(FunctionExpr::TemporalExpr(TemporalFunction::Week))
     }
 
-    /// Extract the week day from the underlying Date representation.
+    /// Extract the ISO week day from the underlying Date representation.
     /// Can be performed on Date and Datetime.
 
-    /// Returns the weekday number where monday = 0 and sunday = 6
+    /// Returns the weekday number where monday = 1 and sunday = 7
     pub fn weekday(self) -> Expr {
         self.0
             .map_private(FunctionExpr::TemporalExpr(TemporalFunction::WeekDay))
     }
 
     /// Get the month of a Date/Datetime
     pub fn day(self) -> Expr {
```

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/dsl/expr.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/dsl/expr.rs`

 * *Files 0% similar despite different names*

```diff
@@ -140,21 +140,21 @@
     Nth(i64),
     // skipped fields must be last otherwise serde fails in pickle
     #[cfg_attr(feature = "serde", serde(skip))]
     RenameAlias {
         function: SpecialEq<Arc<dyn RenameAliasFn>>,
         expr: Box<Expr>,
     },
-    #[cfg_attr(feature = "serde", serde(skip))]
     AnonymousFunction {
         /// function arguments
         input: Vec<Expr>,
         /// function to apply
         function: SpecialEq<Arc<dyn SeriesUdf>>,
         /// output dtype of the function
+        #[cfg_attr(feature = "serde", serde(skip))]
         output_type: GetOutput,
         options: FunctionOptions,
     },
     Cache {
         input: Box<Expr>,
         id: usize,
     },
```

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/dsl/expr_dyn_fn.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/dsl/expr_dyn_fn.rs`

 * *Files 13% similar despite different names*

```diff
@@ -8,14 +8,72 @@
 use serde::{Deserializer, Serializer};
 
 use super::*;
 
 /// A wrapper trait for any closure `Fn(Vec<Series>) -> PolarsResult<Series>`
 pub trait SeriesUdf: Send + Sync {
     fn call_udf(&self, s: &mut [Series]) -> PolarsResult<Option<Series>>;
+
+    fn try_serialize(&self, _buf: &mut Vec<u8>) -> PolarsResult<()> {
+        polars_bail!(ComputeError: "serialize not supported for this 'opaque' function")
+    }
+
+    // Needed for python functions. After they are deserialized we first check if they
+    // have a function that generates an output
+    // This will be slower during optimization, so it is up to us to move
+    // all expression to the known function architecture.
+    fn get_output(&self) -> Option<GetOutput> {
+        None
+    }
+}
+
+#[cfg(feature = "serde")]
+impl Serialize for SpecialEq<Arc<dyn SeriesUdf>> {
+    fn serialize<S>(&self, serializer: S) -> std::result::Result<S::Ok, S::Error>
+    where
+        S: Serializer,
+    {
+        use serde::ser::Error;
+        let mut buf = vec![];
+        self.0
+            .try_serialize(&mut buf)
+            .map_err(|e| S::Error::custom(format!("{e}")))?;
+        serializer.serialize_bytes(&buf)
+    }
+}
+
+#[cfg(feature = "serde")]
+impl<'a> Deserialize<'a> for SpecialEq<Arc<dyn SeriesUdf>> {
+    fn deserialize<D>(_deserializer: D) -> std::result::Result<Self, D::Error>
+    where
+        D: Deserializer<'a>,
+    {
+        use serde::de::Error;
+        #[cfg(feature = "python")]
+        {
+            use crate::dsl::python_udf::MAGIC_BYTE_MARK;
+            let buf = Vec::<u8>::deserialize(_deserializer)?;
+
+            if buf.starts_with(MAGIC_BYTE_MARK) {
+                let udf = python_udf::PythonUdfExpression::try_deserialize(&buf)
+                    .map_err(|e| D::Error::custom(format!("{e}")))?;
+                Ok(SpecialEq::new(udf))
+            } else {
+                Err(D::Error::custom(
+                    "deserialize not supported for this 'opaque' function",
+                ))
+            }
+        }
+        #[cfg(not(feature = "python"))]
+        {
+            Err(D::Error::custom(
+                "deserialize not supported for this 'opaque' function",
+            ))
+        }
+    }
 }
 
 impl<F> SeriesUdf for F
 where
     F: Fn(&mut [Series]) -> PolarsResult<Option<Series>> + Send + Sync,
 {
     fn call_udf(&self, s: &mut [Series]) -> PolarsResult<Option<Series>> {
@@ -80,30 +138,30 @@
 
 #[derive(Clone)]
 /// Wrapper type that has special equality properties
 /// depending on the inner type specialization
 pub struct SpecialEq<T>(T);
 
 #[cfg(feature = "serde")]
-impl<T: Serialize> Serialize for SpecialEq<T> {
+impl Serialize for SpecialEq<Series> {
     fn serialize<S>(&self, serializer: S) -> std::result::Result<S::Ok, S::Error>
     where
         S: Serializer,
     {
         self.0.serialize(serializer)
     }
 }
 
 #[cfg(feature = "serde")]
-impl<'a, T: Deserialize<'a>> Deserialize<'a> for SpecialEq<T> {
+impl<'a> Deserialize<'a> for SpecialEq<Series> {
     fn deserialize<D>(deserializer: D) -> std::result::Result<Self, D::Error>
     where
         D: Deserializer<'a>,
     {
-        let t = T::deserialize(deserializer)?;
+        let t = Series::deserialize(deserializer)?;
         Ok(SpecialEq(t))
     }
 }
 
 impl<T> SpecialEq<T> {
     pub fn new(val: T) -> Self {
         SpecialEq(val)
```

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/dsl/from.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/dsl/from.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/dsl/function_expr/arg_where.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/dsl/function_expr/arg_where.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/dsl/function_expr/array.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/dsl/function_expr/array.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/dsl/function_expr/binary.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/dsl/function_expr/binary.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/dsl/function_expr/boolean.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/dsl/function_expr/boolean.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/dsl/function_expr/bounds.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/dsl/function_expr/bounds.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/dsl/function_expr/cat.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/dsl/function_expr/cat.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/dsl/function_expr/correlation.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/dsl/function_expr/correlation.rs`

 * *Files 13% similar despite different names*

```diff
@@ -175,29 +175,24 @@
         }
     }
 
     // drop nulls so that they are excluded
     let a = a.drop_nulls();
     let b = b.drop_nulls();
 
-    let a_idx = a.rank(
+    let a_rank = a.rank(
         RankOptions {
-            method: RankMethod::Min,
+            method: RankMethod::Average,
             ..Default::default()
         },
         None,
     );
-    let b_idx = b.rank(
+    let b_rank = b.rank(
         RankOptions {
-            method: RankMethod::Min,
+            method: RankMethod::Average,
             ..Default::default()
         },
         None,
     );
-    let a_idx = a_idx.idx().unwrap();
-    let b_idx = b_idx.idx().unwrap();
 
-    Ok(Series::new(
-        name,
-        &[polars_core::functions::pearson_corr_i(a_idx, b_idx, ddof)],
-    ))
+    pearson_corr(&[a_rank, b_rank], ddof)
 }
```

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/dsl/function_expr/cum.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/dsl/function_expr/cum.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/dsl/function_expr/datetime.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/dsl/function_expr/datetime.rs`

 * *Files 2% similar despite different names*

```diff
@@ -130,32 +130,46 @@
         DataType::Time => Ok(s.clone()),
         dtype => polars_bail!(ComputeError: "expected Datetime, Date, or Time, got {}", dtype),
     }
 }
 pub(super) fn date(s: &Series) -> PolarsResult<Series> {
     match s.dtype() {
         #[cfg(feature = "timezones")]
-        DataType::Datetime(_, Some(_)) => s
-            .datetime()
-            .unwrap()
-            .replace_time_zone(None, None)?
-            .cast(&DataType::Date),
+        DataType::Datetime(_, Some(tz)) => {
+            let mut out = s
+                .datetime()
+                .unwrap()
+                .replace_time_zone(None, None)?
+                .cast(&DataType::Date)?;
+            if tz != "UTC" {
+                // DST transitions may not preserve sortedness.
+                out.set_sorted_flag(IsSorted::Not);
+            }
+            Ok(out)
+        }
         DataType::Datetime(_, _) => s.datetime().unwrap().cast(&DataType::Date),
         DataType::Date => Ok(s.clone()),
         dtype => polars_bail!(ComputeError: "expected Datetime or Date, got {}", dtype),
     }
 }
 pub(super) fn datetime(s: &Series) -> PolarsResult<Series> {
     match s.dtype() {
         #[cfg(feature = "timezones")]
-        DataType::Datetime(tu, Some(_)) => s
-            .datetime()
-            .unwrap()
-            .replace_time_zone(None, None)?
-            .cast(&DataType::Datetime(*tu, None)),
+        DataType::Datetime(tu, Some(tz)) => {
+            let mut out = s
+                .datetime()
+                .unwrap()
+                .replace_time_zone(None, None)?
+                .cast(&DataType::Datetime(*tu, None))?;
+            if tz != "UTC" {
+                // DST transitions may not preserve sortedness.
+                out.set_sorted_flag(IsSorted::Not);
+            }
+            Ok(out)
+        }
         DataType::Datetime(tu, _) => s.datetime().unwrap().cast(&DataType::Datetime(*tu, None)),
         dtype => polars_bail!(ComputeError: "expected Datetime, got {}", dtype),
     }
 }
 pub(super) fn hour(s: &Series) -> PolarsResult<Series> {
     s.hour().map(|ca| ca.into_series())
 }
```

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/dsl/function_expr/dispatch.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/dsl/function_expr/dispatch.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/dsl/function_expr/fill_null.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/dsl/function_expr/fill_null.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/dsl/function_expr/fused.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/dsl/function_expr/fused.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/dsl/function_expr/list.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/dsl/function_expr/list.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/dsl/function_expr/log.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/dsl/function_expr/log.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/dsl/function_expr/mod.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/dsl/function_expr/mod.rs`

 * *Files 2% similar despite different names*

```diff
@@ -541,23 +541,30 @@
             ConcatVertical(delimiter) => map!(strings::concat, &delimiter),
             #[cfg(feature = "concat_str")]
             ConcatHorizontal(delimiter) => map_as_slice!(strings::concat_hor, &delimiter),
             #[cfg(feature = "regex")]
             Replace { n, literal } => map_as_slice!(strings::replace, literal, n),
             Uppercase => map!(strings::uppercase),
             Lowercase => map!(strings::lowercase),
+            #[cfg(feature = "nightly")]
+            Titlecase => map!(strings::titlecase),
             Strip(matches) => map!(strings::strip, matches.as_deref()),
             LStrip(matches) => map!(strings::lstrip, matches.as_deref()),
             RStrip(matches) => map!(strings::rstrip, matches.as_deref()),
             #[cfg(feature = "string_from_radix")]
             FromRadix(radix, strict) => map!(strings::from_radix, radix, strict),
             Slice(start, length) => map!(strings::str_slice, start, length),
             Explode => map!(strings::explode),
             #[cfg(feature = "dtype-decimal")]
             ToDecimal(infer_len) => map!(strings::to_decimal, infer_len),
+            #[cfg(feature = "extract_jsonpath")]
+            JsonExtract {
+                dtype,
+                infer_schema_len,
+            } => map!(strings::json_extract, dtype.clone(), infer_schema_len),
         }
     }
 }
 
 impl From<BinaryFunction> for SpecialEq<Arc<dyn SeriesUdf>> {
     fn from(func: BinaryFunction) -> Self {
         use BinaryFunction::*;
```

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/dsl/function_expr/pow.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/dsl/function_expr/pow.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/dsl/function_expr/schema.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/dsl/function_expr/schema.rs`

 * *Files 2% similar despite different names*

```diff
@@ -335,8 +335,14 @@
         if matches!(dt, UInt8 | Int8 | Int16 | UInt16) {
             first.coerce(Int64);
         } else {
             first.coerce(dt);
         }
         Ok(first)
     }
+
+    #[cfg(feature = "extract_jsonpath")]
+    pub(super) fn with_opt_dtype(&self, dtype: Option<DataType>) -> PolarsResult<Field> {
+        let dtype = dtype.unwrap_or(DataType::Unknown);
+        self.with_dtype(dtype)
+    }
 }
```

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/dsl/function_expr/shift_and_fill.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/dsl/function_expr/shift_and_fill.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/dsl/function_expr/shrink_type.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/dsl/function_expr/shrink_type.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/dsl/function_expr/sign.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/dsl/function_expr/sign.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/dsl/function_expr/strings.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/dsl/function_expr/strings.rs`

 * *Files 5% similar despite different names*

```diff
@@ -53,23 +53,30 @@
         // negative is replace all
         // how many matches to replace
         n: i64,
         literal: bool,
     },
     Uppercase,
     Lowercase,
+    #[cfg(feature = "nightly")]
+    Titlecase,
     Strip(Option<String>),
     RStrip(Option<String>),
     LStrip(Option<String>),
     #[cfg(feature = "string_from_radix")]
     FromRadix(u32, bool),
     Slice(i64, Option<u64>),
     Explode,
     #[cfg(feature = "dtype-decimal")]
     ToDecimal(usize),
+    #[cfg(feature = "extract_jsonpath")]
+    JsonExtract {
+        dtype: Option<DataType>,
+        infer_schema_len: Option<usize>,
+    },
 }
 
 impl StringFunction {
     pub(super) fn get_field(&self, mapper: FieldsMapper) -> PolarsResult<Field> {
         use StringFunction::*;
         match self {
             #[cfg(feature = "regex")]
@@ -79,25 +86,29 @@
             ExtractAll => mapper.with_dtype(DataType::List(Box::new(DataType::Utf8))),
             CountMatch(_) => mapper.with_dtype(DataType::UInt32),
             #[cfg(feature = "string_justify")]
             Zfill { .. } | LJust { .. } | RJust { .. } => mapper.with_same_dtype(),
             #[cfg(feature = "temporal")]
             Strptime(dtype, _) => mapper.with_dtype(dtype.clone()),
             #[cfg(feature = "concat_str")]
-            ConcatVertical(_) | ConcatHorizontal(_) => mapper.with_dtype(DataType::Utf8),
+            ConcatVertical(_) | ConcatHorizontal(_) => mapper.with_same_dtype(),
             #[cfg(feature = "regex")]
-            Replace { .. } => mapper.with_dtype(DataType::Utf8),
+            Replace { .. } => mapper.with_same_dtype(),
             Uppercase | Lowercase | Strip(_) | LStrip(_) | RStrip(_) | Slice(_, _) => {
-                mapper.with_dtype(DataType::Utf8)
+                mapper.with_same_dtype()
             }
+            #[cfg(feature = "nightly")]
+            Titlecase => mapper.with_same_dtype(),
             #[cfg(feature = "string_from_radix")]
             FromRadix { .. } => mapper.with_dtype(DataType::Int32),
             Explode => mapper.with_same_dtype(),
             #[cfg(feature = "dtype-decimal")]
             ToDecimal(_) => mapper.with_dtype(DataType::Decimal(None, None)),
+            #[cfg(feature = "extract_jsonpath")]
+            JsonExtract { dtype, .. } => mapper.with_opt_dtype(dtype.clone()),
         }
     }
 }
 
 impl Display for StringFunction {
     fn fmt(&self, f: &mut Formatter<'_>) -> std::fmt::Result {
         let s = match self {
@@ -120,23 +131,27 @@
             StringFunction::ConcatVertical(_) => "concat_vertical",
             #[cfg(feature = "concat_str")]
             StringFunction::ConcatHorizontal(_) => "concat_horizontal",
             #[cfg(feature = "regex")]
             StringFunction::Replace { .. } => "replace",
             StringFunction::Uppercase => "uppercase",
             StringFunction::Lowercase => "lowercase",
+            #[cfg(feature = "nightly")]
+            StringFunction::Titlecase => "titlecase",
             StringFunction::Strip(_) => "strip",
             StringFunction::LStrip(_) => "lstrip",
             StringFunction::RStrip(_) => "rstrip",
             #[cfg(feature = "string_from_radix")]
             StringFunction::FromRadix { .. } => "from_radix",
             StringFunction::Slice(_, _) => "str_slice",
             StringFunction::Explode => "explode",
             #[cfg(feature = "dtype-decimal")]
             StringFunction::ToDecimal(_) => "to_decimal",
+            #[cfg(feature = "extract_jsonpath")]
+            StringFunction::JsonExtract { .. } => "json_extract",
         };
 
         write!(f, "str.{s}")
     }
 }
 
 pub(super) fn uppercase(s: &Series) -> PolarsResult<Series> {
@@ -145,14 +160,20 @@
 }
 
 pub(super) fn lowercase(s: &Series) -> PolarsResult<Series> {
     let ca = s.utf8()?;
     Ok(ca.to_lowercase().into_series())
 }
 
+#[cfg(feature = "nightly")]
+pub(super) fn titlecase(s: &Series) -> PolarsResult<Series> {
+    let ca = s.utf8()?;
+    Ok(ca.to_titlecase().into_series())
+}
+
 #[cfg(feature = "regex")]
 pub(super) fn contains(s: &[Series], literal: bool, strict: bool) -> PolarsResult<Series> {
     let ca = &s[0].utf8()?;
     let pat = &s[1].utf8()?;
 
     let mut out: BooleanChunked = match pat.len() {
         1 => match pat.get(0) {
@@ -402,20 +423,22 @@
     options: &StrptimeOptions,
 ) -> PolarsResult<Series> {
     let tz_aware = match &options.format {
         #[cfg(feature = "timezones")]
         Some(format) => TZ_AWARE_RE.is_match(format),
         _ => false,
     };
-    if let (Some(_), true) = (time_zone, tz_aware) {
-        polars_bail!(
-            ComputeError:
-            "cannot use strptime with both a tz-aware format and a tz-aware dtype, \
-            please drop time zone from the dtype"
-        )
+    if let (Some(tz), true) = (time_zone, tz_aware) {
+        if tz != "UTC" {
+            polars_bail!(
+                ComputeError:
+                "if using strftime/to_datetime with a time-zone-aware format, the output will be in UTC. Please either drop the time zone from the function call, or set it to UTC. \
+                If you are trying to convert the output to a different time zone, please use `convert_time_zone`."
+            )
+        }
     };
 
     let ca = s.utf8()?;
     let out = if options.exact {
         ca.as_datetime(
             options.format.as_deref(),
             *time_unit,
@@ -657,7 +680,17 @@
 }
 
 #[cfg(feature = "dtype-decimal")]
 pub(super) fn to_decimal(s: &Series, infer_len: usize) -> PolarsResult<Series> {
     let ca = s.utf8()?;
     ca.to_decimal(infer_len)
 }
+
+#[cfg(feature = "extract_jsonpath")]
+pub(super) fn json_extract(
+    s: &Series,
+    dtype: Option<DataType>,
+    infer_schema_len: Option<usize>,
+) -> PolarsResult<Series> {
+    let ca = s.utf8()?;
+    ca.json_extract(dtype, infer_schema_len)
+}
```

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/dsl/function_expr/struct_.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/dsl/function_expr/struct_.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/dsl/function_expr/temporal.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/dsl/function_expr/temporal.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/dsl/function_expr/trigonometry.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/dsl/function_expr/trigonometry.rs`

 * *Files 4% similar despite different names*

```diff
@@ -2,44 +2,50 @@
 use polars_core::export::num;
 
 use super::*;
 
 #[cfg_attr(feature = "serde", derive(Serialize, Deserialize))]
 #[derive(Clone, Copy, PartialEq, Debug, Eq, Hash)]
 pub enum TrigonometricFunction {
-    Sin,
     Cos,
+    Cot,
+    Sin,
     Tan,
-    ArcSin,
     ArcCos,
+    ArcSin,
     ArcTan,
-    Sinh,
     Cosh,
+    Sinh,
     Tanh,
-    ArcSinh,
     ArcCosh,
+    ArcSinh,
     ArcTanh,
+    Degrees,
+    Radians,
 }
 
 impl Display for TrigonometricFunction {
     fn fmt(&self, f: &mut Formatter<'_>) -> std::fmt::Result {
         use self::*;
         match self {
-            TrigonometricFunction::Sin => write!(f, "sin"),
             TrigonometricFunction::Cos => write!(f, "cos"),
+            TrigonometricFunction::Cot => write!(f, "cot"),
+            TrigonometricFunction::Sin => write!(f, "sin"),
             TrigonometricFunction::Tan => write!(f, "tan"),
-            TrigonometricFunction::ArcSin => write!(f, "arcsin"),
             TrigonometricFunction::ArcCos => write!(f, "arccos"),
+            TrigonometricFunction::ArcSin => write!(f, "arcsin"),
             TrigonometricFunction::ArcTan => write!(f, "arctan"),
-            TrigonometricFunction::Sinh => write!(f, "sinh"),
             TrigonometricFunction::Cosh => write!(f, "cosh"),
+            TrigonometricFunction::Sinh => write!(f, "sinh"),
             TrigonometricFunction::Tanh => write!(f, "tanh"),
-            TrigonometricFunction::ArcSinh => write!(f, "arcsinh"),
             TrigonometricFunction::ArcCosh => write!(f, "arccosh"),
+            TrigonometricFunction::ArcSinh => write!(f, "arcsinh"),
             TrigonometricFunction::ArcTanh => write!(f, "arctanh"),
+            TrigonometricFunction::Degrees => write!(f, "degrees"),
+            TrigonometricFunction::Radians => write!(f, "radians"),
         }
     }
 }
 
 pub(super) fn apply_trigonometric_function(
     s: &Series,
     trig_function: TrigonometricFunction,
@@ -68,129 +74,159 @@
 ) -> PolarsResult<Series>
 where
     T: PolarsFloatType,
     T::Native: Float,
     ChunkedArray<T>: IntoSeries,
 {
     match trig_function {
-        TrigonometricFunction::Sin => sin(ca),
         TrigonometricFunction::Cos => cos(ca),
+        TrigonometricFunction::Cot => cot(ca),
+        TrigonometricFunction::Sin => sin(ca),
         TrigonometricFunction::Tan => tan(ca),
-        TrigonometricFunction::ArcSin => arcsin(ca),
         TrigonometricFunction::ArcCos => arccos(ca),
+        TrigonometricFunction::ArcSin => arcsin(ca),
         TrigonometricFunction::ArcTan => arctan(ca),
-        TrigonometricFunction::Sinh => sinh(ca),
         TrigonometricFunction::Cosh => cosh(ca),
+        TrigonometricFunction::Sinh => sinh(ca),
         TrigonometricFunction::Tanh => tanh(ca),
-        TrigonometricFunction::ArcSinh => arcsinh(ca),
         TrigonometricFunction::ArcCosh => arccosh(ca),
+        TrigonometricFunction::ArcSinh => arcsinh(ca),
         TrigonometricFunction::ArcTanh => arctanh(ca),
+        TrigonometricFunction::Degrees => degrees(ca),
+        TrigonometricFunction::Radians => radians(ca),
     }
 }
 
-fn sin<T>(ca: &ChunkedArray<T>) -> PolarsResult<Series>
+fn cos<T>(ca: &ChunkedArray<T>) -> PolarsResult<Series>
 where
     T: PolarsFloatType,
     T::Native: Float,
     ChunkedArray<T>: IntoSeries,
 {
-    Ok(ca.apply(|v| v.sin()).into_series())
+    Ok(ca.apply(|v| v.cos()).into_series())
 }
 
-fn cos<T>(ca: &ChunkedArray<T>) -> PolarsResult<Series>
+fn cot<T>(ca: &ChunkedArray<T>) -> PolarsResult<Series>
 where
     T: PolarsFloatType,
     T::Native: Float,
     ChunkedArray<T>: IntoSeries,
 {
-    Ok(ca.apply(|v| v.cos()).into_series())
+    Ok(ca.apply(|v| v.cos() / v.sin()).into_series())
 }
 
-fn tan<T>(ca: &ChunkedArray<T>) -> PolarsResult<Series>
+fn sin<T>(ca: &ChunkedArray<T>) -> PolarsResult<Series>
 where
     T: PolarsFloatType,
     T::Native: Float,
     ChunkedArray<T>: IntoSeries,
 {
-    Ok(ca.apply(|v| v.tan()).into_series())
+    Ok(ca.apply(|v| v.sin()).into_series())
 }
 
-fn arcsin<T>(ca: &ChunkedArray<T>) -> PolarsResult<Series>
+fn tan<T>(ca: &ChunkedArray<T>) -> PolarsResult<Series>
 where
     T: PolarsFloatType,
     T::Native: Float,
     ChunkedArray<T>: IntoSeries,
 {
-    Ok(ca.apply(|v| v.asin()).into_series())
+    Ok(ca.apply(|v| v.tan()).into_series())
 }
 
 fn arccos<T>(ca: &ChunkedArray<T>) -> PolarsResult<Series>
 where
     T: PolarsFloatType,
     T::Native: Float,
     ChunkedArray<T>: IntoSeries,
 {
     Ok(ca.apply(|v| v.acos()).into_series())
 }
 
-fn arctan<T>(ca: &ChunkedArray<T>) -> PolarsResult<Series>
+fn arcsin<T>(ca: &ChunkedArray<T>) -> PolarsResult<Series>
 where
     T: PolarsFloatType,
     T::Native: Float,
     ChunkedArray<T>: IntoSeries,
 {
-    Ok(ca.apply(|v| v.atan()).into_series())
+    Ok(ca.apply(|v| v.asin()).into_series())
 }
 
-fn sinh<T>(ca: &ChunkedArray<T>) -> PolarsResult<Series>
+fn arctan<T>(ca: &ChunkedArray<T>) -> PolarsResult<Series>
 where
     T: PolarsFloatType,
     T::Native: Float,
     ChunkedArray<T>: IntoSeries,
 {
-    Ok(ca.apply(|v| v.sinh()).into_series())
+    Ok(ca.apply(|v| v.atan()).into_series())
 }
 
 fn cosh<T>(ca: &ChunkedArray<T>) -> PolarsResult<Series>
 where
     T: PolarsFloatType,
     T::Native: Float,
     ChunkedArray<T>: IntoSeries,
 {
     Ok(ca.apply(|v| v.cosh()).into_series())
 }
 
-fn tanh<T>(ca: &ChunkedArray<T>) -> PolarsResult<Series>
+fn sinh<T>(ca: &ChunkedArray<T>) -> PolarsResult<Series>
 where
     T: PolarsFloatType,
     T::Native: Float,
     ChunkedArray<T>: IntoSeries,
 {
-    Ok(ca.apply(|v| v.tanh()).into_series())
+    Ok(ca.apply(|v| v.sinh()).into_series())
 }
 
-fn arcsinh<T>(ca: &ChunkedArray<T>) -> PolarsResult<Series>
+fn tanh<T>(ca: &ChunkedArray<T>) -> PolarsResult<Series>
 where
     T: PolarsFloatType,
     T::Native: Float,
     ChunkedArray<T>: IntoSeries,
 {
-    Ok(ca.apply(|v| v.asinh()).into_series())
+    Ok(ca.apply(|v| v.tanh()).into_series())
 }
 
 fn arccosh<T>(ca: &ChunkedArray<T>) -> PolarsResult<Series>
 where
     T: PolarsFloatType,
     T::Native: Float,
     ChunkedArray<T>: IntoSeries,
 {
     Ok(ca.apply(|v| v.acosh()).into_series())
 }
 
+fn arcsinh<T>(ca: &ChunkedArray<T>) -> PolarsResult<Series>
+where
+    T: PolarsFloatType,
+    T::Native: Float,
+    ChunkedArray<T>: IntoSeries,
+{
+    Ok(ca.apply(|v| v.asinh()).into_series())
+}
+
 fn arctanh<T>(ca: &ChunkedArray<T>) -> PolarsResult<Series>
 where
     T: PolarsFloatType,
     T::Native: Float,
     ChunkedArray<T>: IntoSeries,
 {
     Ok(ca.apply(|v| v.atanh()).into_series())
 }
+
+fn degrees<T>(ca: &ChunkedArray<T>) -> PolarsResult<Series>
+where
+    T: PolarsFloatType,
+    T::Native: Float,
+    ChunkedArray<T>: IntoSeries,
+{
+    Ok(ca.apply(|v| v.to_degrees()).into_series())
+}
+
+fn radians<T>(ca: &ChunkedArray<T>) -> PolarsResult<Series>
+where
+    T: PolarsFloatType,
+    T::Native: Float,
+    ChunkedArray<T>: IntoSeries,
+{
+    Ok(ca.apply(|v| v.to_radians()).into_series())
+}
```

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/dsl/functions/arity.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/dsl/functions/arity.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/dsl/functions/coerce.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/dsl/functions/coerce.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/dsl/functions/concat.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/dsl/functions/concat.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/dsl/functions/correlation.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/dsl/functions/correlation.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/dsl/functions/horizontal.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/dsl/functions/horizontal.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/dsl/functions/index.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/dsl/functions/index.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/dsl/functions/mod.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/dsl/functions/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/dsl/functions/range.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/dsl/functions/range.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/dsl/functions/selectors.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/dsl/functions/selectors.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/dsl/functions/syntactic_sugar.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/dsl/functions/syntactic_sugar.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/dsl/functions/temporal.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/dsl/functions/temporal.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/dsl/list.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/dsl/list.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/dsl/meta.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/dsl/meta.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/dsl/mod.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/dsl/mod.rs`

 * *Files 1% similar despite different names*

```diff
@@ -18,14 +18,16 @@
 #[cfg(feature = "compile")]
 pub mod functions;
 mod list;
 #[cfg(feature = "meta")]
 mod meta;
 pub(crate) mod names;
 mod options;
+#[cfg(all(feature = "python", feature = "serde"))]
+pub mod python_udf;
 mod selector;
 #[cfg(feature = "strings")]
 pub mod string;
 #[cfg(feature = "dtype-struct")]
 mod struct_;
 
 use std::fmt::Debug;
```

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/dsl/options.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/dsl/options.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/dsl/selector.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/dsl/selector.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/dsl/string.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/dsl/string.rs`

 * *Files 2% similar despite different names*

```diff
@@ -444,14 +444,21 @@
 
     /// Convert all characters to uppercase.
     pub fn to_uppercase(self) -> Expr {
         self.0
             .map_private(FunctionExpr::StringExpr(StringFunction::Uppercase))
     }
 
+    /// Convert all characters to titlecase.
+    #[cfg(feature = "nightly")]
+    pub fn to_titlecase(self) -> Expr {
+        self.0
+            .map_private(FunctionExpr::StringExpr(StringFunction::Titlecase))
+    }
+
     #[cfg(feature = "string_from_radix")]
     /// Parse string in base radix into decimal
     pub fn from_radix(self, radix: u32, strict: bool) -> Expr {
         self.0
             .map_private(FunctionExpr::StringExpr(StringFunction::FromRadix(
                 radix, strict,
             )))
@@ -465,8 +472,17 @@
             )))
     }
 
     pub fn explode(self) -> Expr {
         self.0
             .apply_private(FunctionExpr::StringExpr(StringFunction::Explode))
     }
+
+    #[cfg(feature = "extract_jsonpath")]
+    pub fn json_extract(self, dtype: Option<DataType>, infer_schema_len: Option<usize>) -> Expr {
+        self.0
+            .map_private(FunctionExpr::StringExpr(StringFunction::JsonExtract {
+                dtype,
+                infer_schema_len,
+            }))
+    }
 }
```

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/dsl/struct_.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/dsl/struct_.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/frame/opt_state.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/frame/opt_state.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/logical_plan/aexpr/mod.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/logical_plan/aexpr/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/logical_plan/aexpr/schema.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/logical_plan/aexpr/schema.rs`

 * *Files 2% similar despite different names*

```diff
@@ -178,16 +178,21 @@
                 } else {
                     let st = try_get_supertype(truthy.data_type(), falsy.data_type())?;
                     truthy.coerce(st);
                     Ok(truthy)
                 }
             }
             AnonymousFunction {
-                output_type, input, ..
+                output_type,
+                input,
+                function,
+                ..
             } => {
+                let tmp = function.get_output();
+                let output_type = tmp.as_ref().unwrap_or(output_type);
                 let fields = input
                     .iter()
                     // default context because `col()` would return a list in aggregation context
                     .map(|node| arena.get(*node).to_field(schema, Context::Default, arena))
                     .collect::<PolarsResult<Vec<_>>>()?;
                 Ok(output_type.get_field(schema, ctxt, &fields))
             }
```

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/logical_plan/alp.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/logical_plan/alp.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/logical_plan/anonymous_scan.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/logical_plan/anonymous_scan.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/logical_plan/apply.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/logical_plan/apply.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/logical_plan/builder.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/logical_plan/builder.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/logical_plan/conversion.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/logical_plan/conversion.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/logical_plan/format.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/logical_plan/format.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/logical_plan/functions/drop.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/logical_plan/functions/drop.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/logical_plan/functions/merge_sorted.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/logical_plan/functions/merge_sorted.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/logical_plan/functions/mod.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/logical_plan/functions/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/logical_plan/functions/rename.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/logical_plan/functions/rename.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/logical_plan/iterator.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/logical_plan/iterator.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/logical_plan/lit.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/logical_plan/lit.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/logical_plan/mod.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/logical_plan/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/logical_plan/optimizer/cache_states.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/logical_plan/optimizer/cache_states.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/logical_plan/optimizer/cse.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/logical_plan/optimizer/cse.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/logical_plan/optimizer/delay_rechunk.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/logical_plan/optimizer/delay_rechunk.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/logical_plan/optimizer/drop_nulls.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/logical_plan/optimizer/drop_nulls.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/logical_plan/optimizer/fast_projection.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/logical_plan/optimizer/fast_projection.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/logical_plan/optimizer/file_caching.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/logical_plan/optimizer/file_caching.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/logical_plan/optimizer/flatten_union.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/logical_plan/optimizer/flatten_union.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/logical_plan/optimizer/fused.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/logical_plan/optimizer/fused.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/logical_plan/optimizer/mod.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/logical_plan/optimizer/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/logical_plan/optimizer/predicate_pushdown/keys.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/logical_plan/optimizer/predicate_pushdown/keys.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/logical_plan/optimizer/predicate_pushdown/mod.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/logical_plan/optimizer/predicate_pushdown/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/logical_plan/optimizer/predicate_pushdown/rename.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/logical_plan/optimizer/predicate_pushdown/rename.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/logical_plan/optimizer/predicate_pushdown/utils.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/logical_plan/optimizer/predicate_pushdown/utils.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/functions/melt.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/functions/melt.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/functions/mod.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/functions/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/generic.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/generic.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/groupby.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/groupby.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/hstack.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/hstack.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/joins.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/joins.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/mod.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/projection.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/projection.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/rename.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/rename.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/semi_anti_join.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/semi_anti_join.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/logical_plan/optimizer/simplify_expr.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/logical_plan/optimizer/simplify_expr.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/logical_plan/optimizer/slice_pushdown_expr.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/logical_plan/optimizer/slice_pushdown_expr.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/logical_plan/optimizer/slice_pushdown_lp.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/logical_plan/optimizer/slice_pushdown_lp.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/logical_plan/optimizer/stack_opt.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/logical_plan/optimizer/stack_opt.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/logical_plan/optimizer/type_coercion/binary.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/logical_plan/optimizer/type_coercion/binary.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/logical_plan/optimizer/type_coercion/mod.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/logical_plan/optimizer/type_coercion/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/logical_plan/options.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/logical_plan/options.rs`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 use polars_io::parquet::ParquetCompression;
 use polars_io::RowCount;
 #[cfg(feature = "dynamic_groupby")]
 use polars_time::{DynamicGroupOptions, RollingGroupOptions};
 #[cfg(feature = "serde")]
 use serde::{Deserialize, Serialize};
 
+#[cfg(feature = "python")]
+use crate::prelude::python_udf::PythonFunction;
 use crate::prelude::Expr;
 
 pub type FileCount = u32;
 
 #[cfg(feature = "csv")]
 #[derive(Clone, Debug, PartialEq, Eq)]
 #[cfg_attr(feature = "serde", derive(Serialize, Deserialize))]
@@ -285,16 +287,15 @@
     pub slice: Option<(i64, usize)>,
 }
 
 #[derive(Clone, PartialEq, Eq, Debug, Default)]
 #[cfg_attr(feature = "serde", derive(Serialize, Deserialize))]
 #[cfg(feature = "python")]
 pub struct PythonOptions {
-    // Serialized Fn() -> PolarsResult<DataFrame>
-    pub scan_fn: Vec<u8>,
+    pub scan_fn: Option<PythonFunction>,
     pub schema: SchemaRef,
     pub output_schema: Option<SchemaRef>,
     pub with_columns: Option<Arc<Vec<String>>>,
     pub pyarrow: bool,
     // a pyarrow predicate python expression
     // can be evaluated with python.eval
     pub predicate: Option<String>,
```

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/logical_plan/projection.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/logical_plan/projection.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/logical_plan/pyarrow.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/logical_plan/pyarrow.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/logical_plan/schema.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/logical_plan/schema.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/prelude.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/prelude.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-plan/src/utils.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-plan/src/utils.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-pipe/Cargo.toml` & `polars_u64_idx-0.18.4/local_dependencies/polars-pipe/Cargo.toml`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-pipe/LICENSE` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-pipe/src/executors/operators/filter.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-pipe/src/executors/operators/filter.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-pipe/src/executors/operators/function.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-pipe/src/executors/operators/function.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-pipe/src/executors/operators/pass.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-pipe/src/executors/operators/pass.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-pipe/src/executors/operators/placeholder.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-pipe/src/executors/operators/placeholder.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-pipe/src/executors/operators/projection.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-pipe/src/executors/operators/projection.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-pipe/src/executors/operators/reproject.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-pipe/src/executors/operators/reproject.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-pipe/src/executors/sinks/file_sink.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-pipe/src/executors/sinks/file_sink.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/convert.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/convert.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/count.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/count.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/first.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/first.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/interface.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/interface.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/last.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/last.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/mean.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/mean.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/min_max.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/min_max.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/null.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/null.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/sum.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/sum.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/eval.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/eval.rs`

 * *Files 5% similar despite different names*

```diff
@@ -68,22 +68,22 @@
     ) -> PolarsResult<()> {
         let keys_columns = &mut *self.keys_columns.get();
         let aggregation_series = &mut *self.aggregation_series.get();
 
         for phys_e in self.aggregation_columns_expr.iter() {
             let s = phys_e.evaluate(chunk, context.execution_state.as_any())?;
             let s = s.to_physical_repr();
-            aggregation_series.push(s.rechunk());
+            aggregation_series.push(s.into_owned());
         }
         for phys_e in self.key_columns_expr.iter() {
             let s = phys_e.evaluate(chunk, context.execution_state.as_any())?;
             let s = match s.dtype() {
-                // todo! add binary to phyical repr?
+                // todo! add binary to physical repr?
                 DataType::Utf8 => unsafe { s.cast_unchecked(&DataType::Binary).unwrap() },
-                _ => s.to_physical_repr().rechunk(),
+                _ => s.to_physical_repr().into_owned(),
             };
             keys_columns.push(s.to_arrow(0));
         }
 
         polars_row::convert_columns_amortized(
             keys_columns,
             &self.key_fields,
```

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/global.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/global.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/hash_table.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/hash_table.rs`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-use polars_arrow::trusted_len::PushUnchecked;
+use polars_arrow::trusted_len::TrustedLenPush;
 use polars_core::hashing::partition::this_partition;
 
 use super::*;
 use crate::pipeline::PARTITION_SIZE;
 
 pub(super) struct AggHashTable<const FIXED: bool> {
     inner_map: PlIdHashMap<Key, u32>,
```

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/mod.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/ooc_state.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/ooc_state.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/sink.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/sink.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/source.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/source.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/thread_local.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/thread_local.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-pipe/src/executors/sinks/groupby/mod.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-pipe/src/executors/sinks/groupby/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-pipe/src/executors/sinks/groupby/ooc.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-pipe/src/executors/sinks/groupby/ooc.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-pipe/src/executors/sinks/groupby/ooc_state.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-pipe/src/executors/sinks/groupby/ooc_state.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-pipe/src/executors/sinks/groupby/primitive/mod.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-pipe/src/executors/sinks/groupby/primitive/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-pipe/src/executors/sinks/groupby/string.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-pipe/src/executors/sinks/groupby/string.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-pipe/src/executors/sinks/groupby/utils.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-pipe/src/executors/sinks/groupby/utils.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-pipe/src/executors/sinks/io.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-pipe/src/executors/sinks/io.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-pipe/src/executors/sinks/joins/cross.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-pipe/src/executors/sinks/joins/cross.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-pipe/src/executors/sinks/joins/generic_build.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-pipe/src/executors/sinks/joins/generic_build.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-pipe/src/executors/sinks/joins/inner_left.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-pipe/src/executors/sinks/joins/inner_left.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-pipe/src/executors/sinks/memory.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-pipe/src/executors/sinks/memory.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-pipe/src/executors/sinks/mod.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-pipe/src/executors/sinks/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-pipe/src/executors/sinks/ordered.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-pipe/src/executors/sinks/ordered.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-pipe/src/executors/sinks/reproject.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-pipe/src/executors/sinks/reproject.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-pipe/src/executors/sinks/slice.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-pipe/src/executors/sinks/slice.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-pipe/src/executors/sinks/sort/ooc.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-pipe/src/executors/sinks/sort/ooc.rs`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,15 @@
             Some(accumulate_dataframes_vertical_unchecked(iter))
         } else {
             None
         }
     }
 
     fn finish(self) -> Option<DataFrame> {
-        if self.len.load(Ordering::Relaxed) > 0 {
+        if !self.chunks.is_empty() {
             let iter = self.chunks.into_iter();
             Some(accumulate_dataframes_vertical_unchecked(iter))
         } else {
             None
         }
     }
 }
```

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-pipe/src/executors/sinks/sort/sink.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-pipe/src/executors/sinks/sort/sink.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-pipe/src/executors/sinks/sort/sink_multiple.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-pipe/src/executors/sinks/sort/sink_multiple.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-pipe/src/executors/sinks/sort/source.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-pipe/src/executors/sinks/sort/source.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-pipe/src/executors/sinks/utils.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-pipe/src/executors/sinks/utils.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-pipe/src/executors/sources/csv.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-pipe/src/executors/sources/csv.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-pipe/src/executors/sources/frame.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-pipe/src/executors/sources/frame.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-pipe/src/executors/sources/ipc_one_shot.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-pipe/src/executors/sources/ipc_one_shot.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-pipe/src/executors/sources/parquet.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-pipe/src/executors/sources/parquet.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-pipe/src/executors/sources/reproject.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-pipe/src/executors/sources/reproject.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-pipe/src/executors/sources/union.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-pipe/src/executors/sources/union.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-pipe/src/operators/chunks.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-pipe/src/operators/chunks.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-pipe/src/operators/operator.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-pipe/src/operators/operator.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-pipe/src/operators/sink.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-pipe/src/operators/sink.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-pipe/src/pipeline/convert.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-pipe/src/pipeline/convert.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-pipe/src/pipeline/dispatcher.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-pipe/src/pipeline/dispatcher.rs`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 use std::cell::RefCell;
 use std::collections::VecDeque;
 use std::fmt::{Debug, Formatter};
 use std::rc::Rc;
+use std::sync::{Arc, Mutex};
 
 use polars_core::error::PolarsResult;
 use polars_core::frame::DataFrame;
 use polars_core::utils::accumulate_dataframes_vertical_unchecked;
 use polars_core::POOL;
 use polars_utils::arena::Node;
+use polars_utils::sync::SyncPtr;
 use rayon::prelude::*;
 
 use crate::executors::sources::DataFrameSource;
 use crate::operators::{
     DataChunk, FinalizedSink, Operator, OperatorResult, PExecutionContext, SExecutionContext, Sink,
     SinkResult, Source, SourceResult,
 };
@@ -178,43 +180,99 @@
     fn par_process_chunks(
         &mut self,
         chunks: Vec<DataChunk>,
         sink: &mut [Box<dyn Sink>],
         ec: &PExecutionContext,
         operator_start: usize,
         operator_end: usize,
-    ) -> PolarsResult<Vec<SinkResult>> {
+        src: &mut Box<dyn Source>,
+    ) -> PolarsResult<(Option<SinkResult>, SourceResult)> {
         debug_assert!(chunks.len() <= sink.len());
+
+        fn run_operator_pipe(
+            pipe: &PipeLine,
+            operator_start: usize,
+            operator_end: usize,
+            chunk: DataChunk,
+            sink: &mut Box<dyn Sink>,
+            operator_pipe: &mut [Box<dyn Operator>],
+            ec: &PExecutionContext,
+        ) -> PolarsResult<SinkResult> {
+            // truncate the operators that should run into the current sink.
+            let operator_pipe = &mut operator_pipe[operator_start..operator_end];
+
+            if operator_pipe.is_empty() {
+                sink.sink(ec, chunk)
+            } else {
+                pipe.push_operators(chunk, ec, operator_pipe, sink)
+            }
+        }
+        let sink_results = Arc::new(Mutex::new(None));
+        let mut next_batches: Option<PolarsResult<SourceResult>> = None;
+        let next_batches_ptr = &mut next_batches as *mut Option<PolarsResult<SourceResult>>;
+        let next_batches_ptr = unsafe { SyncPtr::new(next_batches_ptr) };
+
+        // 1. We will iterate the chunks/sinks/operators
+        // where every iteration belongs to a single thread
+        // 2. Then we will truncate the pipeline by `start`/`end`
+        // so that the pipeline represents pipeline that belongs to this sink
+        // 3. Then we push the data
+        // # Threading
+        // Within a rayon scope
+        // we spawn the jobs. They don't have to finish in any specific order,
+        // this makes it more lightweight than `par_iter`
+
+        // temporarily take to please the borrow checker
         let mut operators = std::mem::take(&mut self.operators);
-        let out = POOL.install(|| {
-            chunks
-                .into_par_iter()
-                .zip(sink.par_iter_mut())
-                .zip(operators.par_iter_mut())
-                .map(|((chunk, sink), operator_pipe)| {
-                    // truncate the operators that should run into the current sink.
-                    let operator_pipe = &mut operator_pipe[operator_start..operator_end];
-
-                    if operator_pipe.is_empty() {
-                        sink.sink(ec, chunk)
-                    } else {
-                        self.push_operators(chunk, ec, operator_pipe, sink)
+
+        // borrow as ref and move into the closure
+        let pipeline = &*self;
+        POOL.scope(|s| {
+            for ((chunk, sink), operator_pipe) in chunks
+                .into_iter()
+                .zip(sink.iter_mut())
+                .zip(operators.iter_mut())
+            {
+                let sink_results = sink_results.clone();
+                s.spawn(move |_| {
+                    let out = run_operator_pipe(
+                        pipeline,
+                        operator_start,
+                        operator_end,
+                        chunk,
+                        sink,
+                        operator_pipe,
+                        ec,
+                    );
+                    match out {
+                        Ok(SinkResult::Finished) | Err(_) => {
+                            let mut lock = sink_results.lock().unwrap();
+                            *lock = Some(out)
+                        }
+                        _ => {}
                     }
                 })
-                // only collect failed and finished messages as there should be acted upon those
-                // the other ones (e.g. success and can have more input) can be ignored
-                // this saves a lot of allocations.
-                .filter(|result| match result {
-                    Ok(sink_result) => matches!(sink_result, SinkResult::Finished),
-                    Err(_) => true,
-                })
-                .collect()
+            }
+            // already get batches on the thread pool
+            // if one job is finished earlier we can already start that work
+            s.spawn(|_| {
+                let out = src.get_batches(ec);
+                unsafe {
+                    let ptr = next_batches_ptr.get();
+                    *ptr = Some(out);
+                }
+            })
         });
         self.operators = operators;
-        out
+
+        let next_batches = next_batches.unwrap()?;
+        let mut lock = sink_results.lock().unwrap();
+        lock.take()
+            .transpose()
+            .map(|sink_result| (sink_result, next_batches))
     }
 
     /// This thread local logic that pushed a data chunk into the operators + sink
     /// It can be that a single operator needs to be called multiple times, this is for instance the
     /// case with joins that produce many tuples, that's why we keep a stack of `in_process`
     /// operators.
     fn push_operators(
@@ -287,27 +345,28 @@
         // we don't want to run the rest of the pipelines and we finalize early
         let mut sink_finished = false;
 
         for (i, (operator_end, shared_count, mut sink)) in
             std::mem::take(&mut self.sinks).into_iter().enumerate()
         {
             for src in &mut std::mem::take(&mut self.sources) {
-                while let SourceResult::GotMoreData(chunks) = src.get_batches(ec)? {
-                    let results = self.par_process_chunks(
+                let mut next_batches = src.get_batches(ec)?;
+
+                while let SourceResult::GotMoreData(chunks) = next_batches {
+                    let (sink_result, next_batches2) = self.par_process_chunks(
                         chunks,
                         &mut sink,
                         ec,
                         operator_start,
                         operator_end,
+                        src,
                     )?;
+                    next_batches = next_batches2;
 
-                    if results
-                        .iter()
-                        .any(|sink_result| matches!(sink_result, SinkResult::Finished))
-                    {
+                    if let Some(SinkResult::Finished) = sink_result {
                         sink_finished = true;
                         break;
                     }
                 }
             }
 
             // The sinks have taken all chunks thread locally, now we reduce them into a single
```

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-pipe/src/pipeline/mod.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-pipe/src/pipeline/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-time/Cargo.toml` & `polars_u64_idx-0.18.4/local_dependencies/polars-time/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -34,19 +34,19 @@
 
 test = ["dtype-date", "dtype-datetime", "polars-core/fmt"]
 
 default = []
 
 [dependencies.arrow]
 package = "arrow2"
-git = "https://github.com/jorgecarleitao/arrow2"
-# git = "https://github.com/ritchie46/arrow2"
-rev = "2d2e7053f9a50810bfe9cecff25ab39089aef98e"
+# git = "https://github.com/jorgecarleitao/arrow2"
+git = "https://github.com/ritchie46/arrow2"
+# rev = "2d2e7053f9a50810bfe9cecff25ab39089aef98e"
 # path = "../arrow2"
-# branch = "polars_2023-05-25"
+branch = "polars_2023-06-23"
 version = "0.17"
 default-features = false
 features = [
   "compute_aggregate",
   "compute_arithmetics",
   "compute_boolean",
   "compute_boolean_kleene",
```

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-time/LICENSE` & `polars_u64_idx-0.18.4/local_dependencies/polars-pipe/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-time/src/chunkedarray/date.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-time/src/chunkedarray/date.rs`

 * *Files 1% similar despite different names*

```diff
@@ -45,16 +45,16 @@
     ///
     /// The return value ranges from 1 to 12.
     fn month(&self) -> UInt32Chunked {
         let ca = self.as_date();
         ca.apply_kernel_cast::<UInt32Type>(&date_to_month)
     }
 
-    /// Extract weekday from underlying NaiveDate representation.
-    /// Returns the weekday number where monday = 0 and sunday = 6
+    /// Extract ISO weekday from underlying NaiveDate representation.
+    /// Returns the weekday number where monday = 1 and sunday = 7
     fn weekday(&self) -> UInt32Chunked {
         let ca = self.as_date();
         ca.apply_kernel_cast::<UInt32Type>(&date_to_iso_weekday)
     }
 
     /// Returns the ISO week number starting from 1.
     /// The return value ranges from 1 to 53. (The last week of year differs by years.)
```

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-time/src/chunkedarray/datetime.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-time/src/chunkedarray/datetime.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-time/src/chunkedarray/duration.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-time/src/chunkedarray/duration.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-time/src/chunkedarray/kernels.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-time/src/chunkedarray/kernels.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-time/src/chunkedarray/mod.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-time/src/chunkedarray/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-time/src/chunkedarray/rolling_window/floats.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-time/src/chunkedarray/rolling_window/floats.rs`

 * *Files 2% similar despite different names*

```diff
@@ -144,44 +144,30 @@
     }
 
     /// Apply a rolling std (moving std) over the values in this array.
     /// A window of length `window_size` will traverse the array. The values that fill this window
     /// will (optionally) be multiplied with the weights given by the `weights` vector. The resulting
     /// values will be aggregated to their std.
     fn rolling_std(&self, options: RollingOptionsImpl) -> PolarsResult<Series> {
-        if options.window_size.parsed_int {
-            let options_fixed: RollingOptionsFixedWindow = options.clone().into();
-            check_input(options_fixed.window_size, options.min_periods)?;
-        }
-
-        // weights is only implemented by var kernel
-        if options.weights.is_some() {
-            return self
-                .0
-                .clone()
-                .into_series()
-                .rolling_var(options)
-                .map(|mut s| {
-                    match s.dtype().clone() {
-                        DataType::Float32 => {
-                            let ca: &mut ChunkedArray<Float32Type> = s._get_inner_mut().as_mut();
-                            ca.apply_mut(|v| v.powf(0.5))
-                        }
-                        DataType::Float64 => {
-                            let ca: &mut ChunkedArray<Float64Type> = s._get_inner_mut().as_mut();
-                            ca.apply_mut(|v| v.powf(0.5))
-                        }
-                        _ => unreachable!(),
-                    }
-                    s
-                });
-        }
-
         rolling_agg(
             &self.0,
             options,
-            &rolling::no_nulls::rolling_std,
-            &rolling::nulls::rolling_std,
-            Some(&super::rolling_kernels::no_nulls::rolling_std),
+            &rolling::no_nulls::rolling_var,
+            &rolling::nulls::rolling_var,
+            Some(&super::rolling_kernels::no_nulls::rolling_var),
         )
+        .map(|mut s| {
+            match s.dtype().clone() {
+                DataType::Float32 => {
+                    let ca: &mut ChunkedArray<Float32Type> = s._get_inner_mut().as_mut();
+                    ca.apply_mut(|v| v.powf(0.5))
+                }
+                DataType::Float64 => {
+                    let ca: &mut ChunkedArray<Float64Type> = s._get_inner_mut().as_mut();
+                    ca.apply_mut(|v| v.powf(0.5))
+                }
+                _ => unreachable!(),
+            }
+            s
+        })
     }
 }
```

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-time/src/chunkedarray/rolling_window/ints.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-time/src/chunkedarray/rolling_window/ints.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-time/src/chunkedarray/rolling_window/mod.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-time/src/chunkedarray/rolling_window/mod.rs`

 * *Files 1% similar despite different names*

```diff
@@ -243,15 +243,14 @@
         Option<&[f64]>,
         DynArgs,
     ) -> ArrayRef,
     rolling_agg_fn_dynamic: Option<
         &dyn Fn(
             &[T::Native],
             Duration,
-            Duration,
             &[i64],
             ClosedWindow,
             TimeUnit,
             Option<&TimeZone>,
             DynArgs,
         ) -> PolarsResult<ArrayRef>,
     >,
@@ -290,27 +289,25 @@
         })
     } else {
         if arr.null_count() > 0 {
             panic!("'rolling by' not yet supported for series with null values, consider using 'groupby_rolling'")
         }
         let values = arr.values().as_slice();
         let duration = options.window_size;
+        polars_ensure!(duration.duration_ns() > 0 && !duration.negative, ComputeError:"window size should be strictly positive");
         let tu = options.tu.unwrap();
         let by = options.by.unwrap();
         let closed_window = options.closed_window.expect("closed window  must be set");
-        let mut offset = duration;
-        offset.negative = true;
         let func = rolling_agg_fn_dynamic.expect(
             "'rolling by' not yet supported for this expression, consider using 'groupby_rolling'",
         );
 
         func(
             values,
             duration,
-            offset,
             by,
             closed_window,
             tu,
             options.tz,
             options.fn_params,
         )
     }?;
```

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-time/src/chunkedarray/rolling_window/rolling_kernels/no_nulls.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-time/src/chunkedarray/rolling_window/rolling_kernels/no_nulls.rs`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 #[cfg(feature = "timezones")]
 use chrono_tz::Tz;
 use polars_arrow::kernels::rolling::no_nulls::{self, RollingAggWindowNoNulls};
-use polars_core::export::num;
 
 use super::*;
 
 // Use an aggregation window that maintains the state
 pub(crate) fn rolling_apply_agg_window<'a, Agg, T, O>(
     values: &'a [T],
     offsets: O,
@@ -47,186 +46,107 @@
     Ok(Box::new(out))
 }
 
 #[allow(clippy::too_many_arguments)]
 pub(crate) fn rolling_min<T>(
     values: &[T],
     period: Duration,
-    offset: Duration,
     time: &[i64],
     closed_window: ClosedWindow,
     tu: TimeUnit,
     tz: Option<&TimeZone>,
     _params: DynArgs,
 ) -> PolarsResult<ArrayRef>
 where
     T: NativeType + PartialOrd + IsFloat + Bounded + NumCast + Mul<Output = T>,
 {
     let offset_iter = match tz {
         #[cfg(feature = "timezones")]
-        Some(tz) => groupby_values_iter(
-            period,
-            offset,
-            time,
-            closed_window,
-            tu,
-            tz.parse::<Tz>().ok(),
-        ),
-        _ => groupby_values_iter(period, offset, time, closed_window, tu, None),
+        Some(tz) => groupby_values_iter(period, time, closed_window, tu, tz.parse::<Tz>().ok()),
+        _ => groupby_values_iter(period, time, closed_window, tu, None),
     };
     rolling_apply_agg_window::<no_nulls::MinWindow<_>, _, _>(values, offset_iter, None)
 }
 
 #[allow(clippy::too_many_arguments)]
 pub(crate) fn rolling_max<T>(
     values: &[T],
     period: Duration,
-    offset: Duration,
     time: &[i64],
     closed_window: ClosedWindow,
     tu: TimeUnit,
     tz: Option<&TimeZone>,
     _params: DynArgs,
 ) -> PolarsResult<ArrayRef>
 where
     T: NativeType + PartialOrd + IsFloat + Bounded + NumCast + Mul<Output = T>,
 {
     let offset_iter = match tz {
         #[cfg(feature = "timezones")]
-        Some(tz) => groupby_values_iter(
-            period,
-            offset,
-            time,
-            closed_window,
-            tu,
-            tz.parse::<Tz>().ok(),
-        ),
-        _ => groupby_values_iter(period, offset, time, closed_window, tu, None),
+        Some(tz) => groupby_values_iter(period, time, closed_window, tu, tz.parse::<Tz>().ok()),
+        _ => groupby_values_iter(period, time, closed_window, tu, None),
     };
     rolling_apply_agg_window::<no_nulls::MaxWindow<_>, _, _>(values, offset_iter, None)
 }
 
 #[allow(clippy::too_many_arguments)]
 pub(crate) fn rolling_sum<T>(
     values: &[T],
     period: Duration,
-    offset: Duration,
     time: &[i64],
     closed_window: ClosedWindow,
     tu: TimeUnit,
     tz: Option<&TimeZone>,
     _params: DynArgs,
 ) -> PolarsResult<ArrayRef>
 where
     T: NativeType + std::iter::Sum + NumCast + Mul<Output = T> + AddAssign + SubAssign + IsFloat,
 {
     let offset_iter = match tz {
         #[cfg(feature = "timezones")]
-        Some(tz) => groupby_values_iter(
-            period,
-            offset,
-            time,
-            closed_window,
-            tu,
-            tz.parse::<Tz>().ok(),
-        ),
-        _ => groupby_values_iter(period, offset, time, closed_window, tu, None),
+        Some(tz) => groupby_values_iter(period, time, closed_window, tu, tz.parse::<Tz>().ok()),
+        _ => groupby_values_iter(period, time, closed_window, tu, None),
     };
     rolling_apply_agg_window::<no_nulls::SumWindow<_>, _, _>(values, offset_iter, None)
 }
 
 #[allow(clippy::too_many_arguments)]
 pub(crate) fn rolling_mean<T>(
     values: &[T],
     period: Duration,
-    offset: Duration,
     time: &[i64],
     closed_window: ClosedWindow,
     tu: TimeUnit,
     tz: Option<&TimeZone>,
     _params: DynArgs,
 ) -> PolarsResult<ArrayRef>
 where
     T: NativeType + Float + std::iter::Sum<T> + SubAssign + AddAssign + IsFloat,
 {
     let offset_iter = match tz {
         #[cfg(feature = "timezones")]
-        Some(tz) => groupby_values_iter(
-            period,
-            offset,
-            time,
-            closed_window,
-            tu,
-            tz.parse::<Tz>().ok(),
-        ),
-        _ => groupby_values_iter(period, offset, time, closed_window, tu, None),
+        Some(tz) => groupby_values_iter(period, time, closed_window, tu, tz.parse::<Tz>().ok()),
+        _ => groupby_values_iter(period, time, closed_window, tu, None),
     };
     rolling_apply_agg_window::<no_nulls::MeanWindow<_>, _, _>(values, offset_iter, None)
 }
 
 #[allow(clippy::too_many_arguments)]
 pub(crate) fn rolling_var<T>(
     values: &[T],
     period: Duration,
-    offset: Duration,
     time: &[i64],
     closed_window: ClosedWindow,
     tu: TimeUnit,
     tz: Option<&TimeZone>,
     params: DynArgs,
 ) -> PolarsResult<ArrayRef>
 where
     T: NativeType + Float + std::iter::Sum<T> + SubAssign + AddAssign + IsFloat,
 {
     let offset_iter = match tz {
         #[cfg(feature = "timezones")]
-        Some(tz) => groupby_values_iter(
-            period,
-            offset,
-            time,
-            closed_window,
-            tu,
-            tz.parse::<Tz>().ok(),
-        ),
-        _ => groupby_values_iter(period, offset, time, closed_window, tu, None),
+        Some(tz) => groupby_values_iter(period, time, closed_window, tu, tz.parse::<Tz>().ok()),
+        _ => groupby_values_iter(period, time, closed_window, tu, None),
     };
     rolling_apply_agg_window::<no_nulls::VarWindow<_>, _, _>(values, offset_iter, params)
 }
-
-#[allow(clippy::too_many_arguments)]
-pub(crate) fn rolling_std<T>(
-    values: &[T],
-    period: Duration,
-    offset: Duration,
-    time: &[i64],
-    closed_window: ClosedWindow,
-    tu: TimeUnit,
-    tz: Option<&TimeZone>,
-    params: DynArgs,
-) -> PolarsResult<ArrayRef>
-where
-    T: NativeType
-        + Float
-        + IsFloat
-        + std::iter::Sum
-        + AddAssign
-        + SubAssign
-        + Div<Output = T>
-        + NumCast
-        + One
-        + Sub<Output = T>
-        + num::pow::Pow<T, Output = T>,
-{
-    let offset_iter = match tz {
-        #[cfg(feature = "timezones")]
-        Some(tz) => groupby_values_iter(
-            period,
-            offset,
-            time,
-            closed_window,
-            tu,
-            tz.parse::<Tz>().ok(),
-        ),
-        _ => groupby_values_iter(period, offset, time, closed_window, tu, None),
-    };
-    rolling_apply_agg_window::<no_nulls::StdWindow<_>, _, _>(values, offset_iter, params)
-}
```

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-time/src/chunkedarray/time.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-time/src/chunkedarray/time.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-time/src/chunkedarray/utf8/infer.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-time/src/chunkedarray/utf8/infer.rs`

 * *Files 25% similar despite different names*

```diff
@@ -133,27 +133,33 @@
                 None => false,
             },
         }
     }
 }
 
 pub trait StrpTimeParser<T> {
-    fn parse_bytes(&mut self, val: &[u8]) -> Option<T>;
+    fn parse_bytes(&mut self, val: &[u8], time_unit: Option<TimeUnit>) -> Option<T>;
 }
 
 #[cfg(feature = "dtype-datetime")]
 impl StrpTimeParser<i64> for DatetimeInfer<i64> {
-    fn parse_bytes(&mut self, val: &[u8]) -> Option<i64> {
+    fn parse_bytes(&mut self, val: &[u8], time_unit: Option<TimeUnit>) -> Option<i64> {
         if self.fmt_len == 0 {
             self.fmt_len = strptime::fmt_len(self.latest_fmt.as_bytes())?;
         }
+        let transform = match time_unit {
+            Some(TimeUnit::Nanoseconds) => datetime_to_timestamp_ns,
+            Some(TimeUnit::Microseconds) => datetime_to_timestamp_us,
+            Some(TimeUnit::Milliseconds) => datetime_to_timestamp_ms,
+            _ => unreachable!(), // time_unit has to be provided for datetime
+        };
         unsafe {
             self.transform_bytes
                 .parse(val, self.latest_fmt.as_bytes(), self.fmt_len)
-                .map(datetime_to_timestamp_us)
+                .map(transform)
                 .or_else(|| {
                     // TODO! this will try all patterns.
                     // somehow we must early escape if value is invalid
                     for fmt in self.patterns {
                         if self.fmt_len == 0 {
                             self.fmt_len = strptime::fmt_len(fmt.as_bytes())?;
                         }
@@ -170,15 +176,15 @@
                 })
         }
     }
 }
 
 #[cfg(feature = "dtype-date")]
 impl StrpTimeParser<i32> for DatetimeInfer<i32> {
-    fn parse_bytes(&mut self, val: &[u8]) -> Option<i32> {
+    fn parse_bytes(&mut self, val: &[u8], _time_unit: Option<TimeUnit>) -> Option<i32> {
         if self.fmt_len == 0 {
             self.fmt_len = strptime::fmt_len(self.latest_fmt.as_bytes())?;
         }
         unsafe {
             self.transform_bytes
                 .parse(val, self.latest_fmt.as_bytes(), self.fmt_len)
                 .map(|ndt| naive_date_to_date(ndt.date()))
@@ -211,57 +217,117 @@
     latest_fmt: &'static str,
     transform: fn(&str, &str) -> Option<T>,
     transform_bytes: StrpTimeState,
     fmt_len: u16,
     pub logical_type: DataType,
 }
 
+pub trait TryFromWithUnit<T>: Sized {
+    type Error;
+    fn try_from_with_unit(pattern: T, unit: Option<TimeUnit>) -> PolarsResult<Self>;
+}
+
 #[cfg(feature = "dtype-datetime")]
-impl TryFrom<Pattern> for DatetimeInfer<i64> {
+impl TryFromWithUnit<Pattern> for DatetimeInfer<i64> {
     type Error = PolarsError;
 
-    fn try_from(value: Pattern) -> PolarsResult<Self> {
-        match value {
-            Pattern::DatetimeDMY => Ok(DatetimeInfer {
+    fn try_from_with_unit(value: Pattern, time_unit: Option<TimeUnit>) -> PolarsResult<Self> {
+        let time_unit = time_unit.expect("time_unit must be provided for datetime");
+        match (value, time_unit) {
+            (Pattern::DatetimeDMY, TimeUnit::Milliseconds) => Ok(DatetimeInfer {
+                pattern: Pattern::DatetimeDMY,
+                patterns: patterns::DATETIME_D_M_Y,
+                latest_fmt: patterns::DATETIME_D_M_Y[0],
+                transform: transform_datetime_ms,
+                transform_bytes: StrpTimeState::default(),
+                fmt_len: 0,
+                logical_type: DataType::Datetime(TimeUnit::Milliseconds, None),
+            }),
+            (Pattern::DatetimeDMY, TimeUnit::Microseconds) => Ok(DatetimeInfer {
                 pattern: Pattern::DatetimeDMY,
                 patterns: patterns::DATETIME_D_M_Y,
                 latest_fmt: patterns::DATETIME_D_M_Y[0],
                 transform: transform_datetime_us,
                 transform_bytes: StrpTimeState::default(),
                 fmt_len: 0,
                 logical_type: DataType::Datetime(TimeUnit::Microseconds, None),
             }),
-            Pattern::DatetimeYMD => Ok(DatetimeInfer {
+            (Pattern::DatetimeDMY, TimeUnit::Nanoseconds) => Ok(DatetimeInfer {
+                pattern: Pattern::DatetimeDMY,
+                patterns: patterns::DATETIME_D_M_Y,
+                latest_fmt: patterns::DATETIME_D_M_Y[0],
+                transform: transform_datetime_ns,
+                transform_bytes: StrpTimeState::default(),
+                fmt_len: 0,
+                logical_type: DataType::Datetime(TimeUnit::Nanoseconds, None),
+            }),
+            (Pattern::DatetimeYMD, TimeUnit::Milliseconds) => Ok(DatetimeInfer {
+                pattern: Pattern::DatetimeYMD,
+                patterns: patterns::DATETIME_Y_M_D,
+                latest_fmt: patterns::DATETIME_Y_M_D[0],
+                transform: transform_datetime_ms,
+                transform_bytes: StrpTimeState::default(),
+                fmt_len: 0,
+                logical_type: DataType::Datetime(TimeUnit::Milliseconds, None),
+            }),
+            (Pattern::DatetimeYMD, TimeUnit::Microseconds) => Ok(DatetimeInfer {
                 pattern: Pattern::DatetimeYMD,
                 patterns: patterns::DATETIME_Y_M_D,
                 latest_fmt: patterns::DATETIME_Y_M_D[0],
                 transform: transform_datetime_us,
                 transform_bytes: StrpTimeState::default(),
                 fmt_len: 0,
                 logical_type: DataType::Datetime(TimeUnit::Microseconds, None),
             }),
-            Pattern::DatetimeYMDZ => Ok(DatetimeInfer {
+            (Pattern::DatetimeYMD, TimeUnit::Nanoseconds) => Ok(DatetimeInfer {
+                pattern: Pattern::DatetimeYMD,
+                patterns: patterns::DATETIME_Y_M_D,
+                latest_fmt: patterns::DATETIME_Y_M_D[0],
+                transform: transform_datetime_ns,
+                transform_bytes: StrpTimeState::default(),
+                fmt_len: 0,
+                logical_type: DataType::Datetime(TimeUnit::Nanoseconds, None),
+            }),
+            (Pattern::DatetimeYMDZ, TimeUnit::Milliseconds) => Ok(DatetimeInfer {
+                pattern: Pattern::DatetimeYMDZ,
+                patterns: patterns::DATETIME_Y_M_D_Z,
+                latest_fmt: patterns::DATETIME_Y_M_D_Z[0],
+                transform: transform_tzaware_datetime_ms,
+                transform_bytes: StrpTimeState::default(),
+                fmt_len: 0,
+                logical_type: DataType::Datetime(TimeUnit::Milliseconds, None),
+            }),
+            (Pattern::DatetimeYMDZ, TimeUnit::Microseconds) => Ok(DatetimeInfer {
                 pattern: Pattern::DatetimeYMDZ,
                 patterns: patterns::DATETIME_Y_M_D_Z,
                 latest_fmt: patterns::DATETIME_Y_M_D_Z[0],
                 transform: transform_tzaware_datetime_us,
                 transform_bytes: StrpTimeState::default(),
                 fmt_len: 0,
                 logical_type: DataType::Datetime(TimeUnit::Microseconds, None),
             }),
+            (Pattern::DatetimeYMDZ, TimeUnit::Nanoseconds) => Ok(DatetimeInfer {
+                pattern: Pattern::DatetimeYMDZ,
+                patterns: patterns::DATETIME_Y_M_D_Z,
+                latest_fmt: patterns::DATETIME_Y_M_D_Z[0],
+                transform: transform_tzaware_datetime_ns,
+                transform_bytes: StrpTimeState::default(),
+                fmt_len: 0,
+                logical_type: DataType::Datetime(TimeUnit::Nanoseconds, None),
+            }),
             _ => polars_bail!(ComputeError: "could not convert pattern"),
         }
     }
 }
 
 #[cfg(feature = "dtype-date")]
-impl TryFrom<Pattern> for DatetimeInfer<i32> {
+impl TryFromWithUnit<Pattern> for DatetimeInfer<i32> {
     type Error = PolarsError;
 
-    fn try_from(value: Pattern) -> PolarsResult<Self> {
+    fn try_from_with_unit(value: Pattern, _time_unit: Option<TimeUnit>) -> PolarsResult<Self> {
         match value {
             Pattern::DateDMY => Ok(DatetimeInfer {
                 pattern: Pattern::DateDMY,
                 patterns: patterns::DATE_D_M_Y,
                 latest_fmt: patterns::DATE_D_M_Y[0],
                 transform: transform_date,
                 transform_bytes: StrpTimeState::default(),
@@ -439,31 +505,22 @@
         None => Ok(Int64Chunked::full_null(ca.name(), ca.len()).into_datetime(tu, tz.cloned())),
         Some(idx) => {
             let subset = ca.slice(idx as i64, ca.len());
             let pattern = subset
                 .into_iter()
                 .find_map(|opt_val| opt_val.and_then(infer_pattern_datetime_single))
                 .ok_or_else(|| polars_err!(parse_fmt_idk = "date"))?;
-            let mut infer = DatetimeInfer::<i64>::try_from(pattern)?;
-            match (tu, pattern) {
-                (TimeUnit::Nanoseconds, Pattern::DatetimeYMDZ) => {
-                    infer.transform = transform_tzaware_datetime_ns
-                }
-                (TimeUnit::Microseconds, Pattern::DatetimeYMDZ) => {
-                    infer.transform = transform_tzaware_datetime_us
-                }
-                (TimeUnit::Milliseconds, Pattern::DatetimeYMDZ) => {
-                    infer.transform = transform_tzaware_datetime_ms
-                }
-                (TimeUnit::Nanoseconds, _) => infer.transform = transform_datetime_ns,
-                (TimeUnit::Microseconds, _) => infer.transform = transform_datetime_us,
-                (TimeUnit::Milliseconds, _) => infer.transform = transform_datetime_ms,
-            }
-            if tz.is_some() && pattern == Pattern::DatetimeYMDZ {
-                polars_bail!(ComputeError: "cannot parse tz-aware values with tz-aware dtype - please drop the time zone from the dtype.")
+            let mut infer = DatetimeInfer::<i64>::try_from_with_unit(pattern, Some(tu))?;
+            if pattern == Pattern::DatetimeYMDZ
+                && tz.is_some()
+                && tz.map(|x| x.as_str()) != Some("UTC")
+            {
+                polars_bail!(ComputeError: "offset-aware datetimes are converted to UTC. \
+                    Please either drop the time zone from the function call, or set it to UTC. \
+                    To convert to a different time zone, please use `convert_time_zone`.")
             }
             match pattern {
                 #[cfg(feature = "timezones")]
                 Pattern::DatetimeYMDZ => infer.coerce_utf8(ca).datetime().map(|ca| {
                     let mut ca = ca.clone();
                     ca.set_time_unit(tu);
                     ca.replace_time_zone(Some("UTC"), None)
@@ -487,12 +544,12 @@
         None => Ok(Int32Chunked::full_null(ca.name(), ca.len()).into_date()),
         Some(idx) => {
             let subset = ca.slice(idx as i64, ca.len());
             let pattern = subset
                 .into_iter()
                 .find_map(|opt_val| opt_val.and_then(infer_pattern_date_single))
                 .ok_or_else(|| polars_err!(parse_fmt_idk = "date"))?;
-            let mut infer = DatetimeInfer::<i32>::try_from(pattern).unwrap();
+            let mut infer = DatetimeInfer::<i32>::try_from_with_unit(pattern, None).unwrap();
             infer.coerce_utf8(ca).date().cloned()
         }
     }
 }
```

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-time/src/chunkedarray/utf8/mod.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-time/src/chunkedarray/utf8/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-time/src/chunkedarray/utf8/patterns.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-time/src/chunkedarray/utf8/patterns.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-time/src/chunkedarray/utf8/strptime.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-time/src/chunkedarray/utf8/strptime.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-time/src/date_range.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-time/src/date_range.rs`

 * *Files 9% similar despite different names*

```diff
@@ -61,18 +61,15 @@
     every: Duration,
     closed: ClosedWindow,
     tu: TimeUnit,
     tz: Option<TimeZone>,
 ) -> PolarsResult<DatetimeChunked> {
     let (start, stop) = match tu {
         TimeUnit::Nanoseconds => (start.timestamp_nanos(), stop.timestamp_nanos()),
-        TimeUnit::Microseconds => (
-            start.timestamp() + start.timestamp_subsec_micros() as i64,
-            stop.timestamp() + stop.timestamp_subsec_millis() as i64,
-        ),
+        TimeUnit::Microseconds => (start.timestamp_micros(), stop.timestamp_micros()),
         TimeUnit::Milliseconds => (start.timestamp_millis(), stop.timestamp_millis()),
     };
     date_range_impl(name, start, stop, every, closed, tu, tz.as_ref())
 }
 
 #[doc(hidden)]
 pub fn time_range_impl(
```

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-time/src/groupby/dynamic.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-time/src/groupby/dynamic.rs`

 * *Files 1% similar despite different names*

```diff
@@ -125,14 +125,19 @@
 
 impl Wrap<&DataFrame> {
     fn groupby_rolling(
         &self,
         by: Vec<Series>,
         options: &RollingGroupOptions,
     ) -> PolarsResult<(Series, Vec<Series>, GroupsProxy)> {
+        polars_ensure!(
+                        options.period.duration_ns()>0 && !options.period.negative,
+                        ComputeError:
+                        "rolling window period should be strictly positive",
+        );
         let time = self.0.column(&options.index_column)?.clone();
         if by.is_empty() {
             // if by is given, the column must be sorted in the 'by' arg, which we can not check now
             // this will be checked when the groups are materialized
             ensure_sorted_arg(&time, "groupby_rolling")?;
         }
         let time_type = time.dtype();
```

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-time/src/lib.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-time/src/lib.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-time/src/month_end.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-time/src/month_end.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-time/src/month_start.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-time/src/month_start.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-time/src/round.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-time/src/round.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-time/src/series/_trait.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-time/src/series/_trait.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-time/src/series/implementations/floats.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-time/src/series/implementations/floats.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-time/src/series/implementations/integers.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-time/src/series/implementations/integers.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-time/src/series/mod.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-time/src/series/mod.rs`

 * *Files 1% similar despite different names*

```diff
@@ -183,15 +183,15 @@
             #[cfg(feature = "dtype-date")]
             DataType::Date => s.date().map(|ca| ca.day()),
             #[cfg(feature = "dtype-datetime")]
             DataType::Datetime(_, _) => s.datetime().map(|ca| ca.day()),
             dt => polars_bail!(opq = day, dt),
         }
     }
-    /// Returns the weekday number where monday = 0 and sunday = 6
+    /// Returns the ISO weekday number where monday = 1 and sunday = 7
     fn weekday(&self) -> PolarsResult<UInt32Chunked> {
         let s = self.as_series();
         match s.dtype() {
             #[cfg(feature = "dtype-date")]
             DataType::Date => s.date().map(|ca| ca.weekday()),
             #[cfg(feature = "dtype-datetime")]
             DataType::Datetime(_, _) => s.datetime().map(|ca| ca.weekday()),
```

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-time/src/truncate.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-time/src/truncate.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-time/src/upsample.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-time/src/upsample.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-time/src/utils.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-time/src/utils.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-time/src/windows/bounds.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-time/src/windows/bounds.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-time/src/windows/calendar.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-time/src/windows/calendar.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-time/src/windows/duration.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-time/src/windows/duration.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-time/src/windows/groupby.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-time/src/windows/groupby.rs`

 * *Files 4% similar despite different names*

```diff
@@ -219,25 +219,25 @@
             );
         }
     };
 
     (groups, lower_bound, upper_bound)
 }
 
-// this assumes that the starting point is alwa
-pub(crate) fn groupby_values_iter_full_lookbehind(
+// this assumes that the given time point is the right endpoint of the window
+pub(crate) fn groupby_values_iter_lookbehind(
     period: Duration,
     offset: Duration,
     time: &[i64],
     closed_window: ClosedWindow,
     tu: TimeUnit,
     tz: Option<Tz>,
     start_offset: usize,
 ) -> impl Iterator<Item = PolarsResult<(IdxSize, IdxSize)>> + TrustedLen + '_ {
-    debug_assert!(offset.duration_ns() >= period.duration_ns());
+    debug_assert!(offset.duration_ns() == period.duration_ns());
     debug_assert!(offset.negative);
     let add = match tu {
         TimeUnit::Nanoseconds => Duration::add_ns,
         TimeUnit::Microseconds => Duration::add_us,
         TimeUnit::Milliseconds => Duration::add_ms,
     };
 
@@ -452,64 +452,24 @@
             Ok((i as IdxSize, len as IdxSize))
         })
 }
 
 #[cfg(feature = "rolling_window")]
 pub(crate) fn groupby_values_iter<'a>(
     period: Duration,
-    offset: Duration,
     time: &'a [i64],
     closed_window: ClosedWindow,
     tu: TimeUnit,
     tz: Option<Tz>,
 ) -> Box<dyn TrustedLen<Item = PolarsResult<(IdxSize, IdxSize)>> + 'a> {
-    // we have a (partial) lookbehind window
-    if offset.negative {
-        // only lookbehind
-        if offset.nanoseconds() == period.nanoseconds() {
-            let iter =
-                groupby_values_iter_full_lookbehind(period, offset, time, closed_window, tu, tz, 0);
-            Box::new(iter)
-        }
-        // partial lookbehind
-        else {
-            let iter =
-                groupby_values_iter_partial_lookbehind(period, offset, time, closed_window, tu, tz);
-            Box::new(iter)
-        }
-    } else if offset != Duration::parse("0ns")
-        || closed_window == ClosedWindow::Right
-        || closed_window == ClosedWindow::None
-    {
-        // only lookahead
-        let iter = groupby_values_iter_full_lookahead(
-            period,
-            offset,
-            time,
-            closed_window,
-            tu,
-            tz,
-            0,
-            None,
-        );
-        Box::new(iter)
-    } else {
-        // partial lookahead
-        let iter = groupby_values_iter_partial_lookahead(
-            period,
-            offset,
-            time,
-            closed_window,
-            tu,
-            tz,
-            0,
-            None,
-        );
-        Box::new(iter)
-    }
+    let mut offset = period;
+    offset.negative = true;
+    // t is at the right endpoint of the window
+    let iter = groupby_values_iter_lookbehind(period, offset, time, closed_window, tu, tz, 0);
+    Box::new(iter)
 }
 
 /// Different from `groupby_windows`, where define window buckets and search which values fit that
 /// pre-defined bucket, this function defines every window based on the:
 ///     - timestamp (lower bound)
 ///     - timestamp + period (upper bound)
 /// where timestamps are the individual values in the array `time`
@@ -521,57 +481,52 @@
     tu: TimeUnit,
     tz: Option<Tz>,
 ) -> PolarsResult<GroupsSlice> {
     let thread_offsets = _split_offsets(time.len(), POOL.current_num_threads());
 
     // we have a (partial) lookbehind window
     if offset.negative {
-        if offset.duration_ns() >= period.duration_ns() {
-            // lookbehind
-            // window is within 2 periods length of t
+        // lookbehind
+        if offset.duration_ns() == period.duration_ns() {
+            // t is right at the end of the window
             // ------t---
             // [------]
-            if offset.duration_ns() < period.duration_ns() * 2 {
-                POOL.install(|| {
-                    let vals = thread_offsets
-                        .par_iter()
-                        .copied()
-                        .map(|(base_offset, len)| {
-                            let upper_bound = base_offset + len;
-                            let iter = groupby_values_iter_full_lookbehind(
-                                period,
-                                offset,
-                                &time[..upper_bound],
-                                closed_window,
-                                tu,
-                                tz,
-                                base_offset,
-                            );
-                            iter.map(|result| result.map(|(offset, len)| [offset, len]))
-                                .collect::<PolarsResult<Vec<_>>>()
-                        })
-                        .collect::<PolarsResult<Vec<_>>>()?;
-                    Ok(flatten_par(&vals))
-                })
-            }
+            POOL.install(|| {
+                let vals = thread_offsets
+                    .par_iter()
+                    .copied()
+                    .map(|(base_offset, len)| {
+                        let upper_bound = base_offset + len;
+                        let iter = groupby_values_iter_lookbehind(
+                            period,
+                            offset,
+                            &time[..upper_bound],
+                            closed_window,
+                            tu,
+                            tz,
+                            base_offset,
+                        );
+                        iter.map(|result| result.map(|(offset, len)| [offset, len]))
+                            .collect::<PolarsResult<Vec<_>>>()
+                    })
+                    .collect::<PolarsResult<Vec<_>>>()?;
+                Ok(flatten_par(&vals))
+            })
+        } else if ((offset.duration_ns() >= period.duration_ns())
+            && matches!(closed_window, ClosedWindow::Left | ClosedWindow::None))
+            || ((offset.duration_ns() > period.duration_ns())
+                && matches!(closed_window, ClosedWindow::Right | ClosedWindow::Both))
+        {
             // window is completely behind t and t itself is not a member
             // ---------------t---
             //  [---]
-            else {
-                let iter = groupby_values_iter_window_behind_t(
-                    period,
-                    offset,
-                    time,
-                    closed_window,
-                    tu,
-                    tz,
-                );
-                iter.map(|result| result.map(|(offset, len)| [offset, len]))
-                    .collect::<PolarsResult<_>>()
-            }
+            let iter =
+                groupby_values_iter_window_behind_t(period, offset, time, closed_window, tu, tz);
+            iter.map(|result| result.map(|(offset, len)| [offset, len]))
+                .collect::<PolarsResult<_>>()
         }
         // partial lookbehind
         // this one is still single threaded
         // can make it parallel later, its a bit more complicated because the boundaries are unknown
         // window is with -1 periods of t
         // ----t---
         //  [---]
@@ -608,15 +563,15 @@
                     iter.map(|result| result.map(|(offset, len)| [offset as IdxSize, len]))
                         .collect::<PolarsResult<Vec<_>>>()
                 })
                 .collect::<PolarsResult<Vec<_>>>()?;
             Ok(flatten_par(&vals))
         })
     } else {
-        // Duration is 0 and window is closed on the left:
+        // Offset is 0 and window is closed on the left:
         // it must be that the window starts at t and t is a member
         // --t-----------
         //  [---]
         POOL.install(|| {
             let vals = thread_offsets
                 .par_iter()
                 .copied()
```

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-time/src/windows/test.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-time/src/windows/test.rs`

 * *Files 0% similar despite different names*

```diff
@@ -705,18 +705,17 @@
     for closed_window in [
         ClosedWindow::Left,
         ClosedWindow::Right,
         ClosedWindow::Both,
         ClosedWindow::None,
     ] {
         let offset = Duration::parse("-2h");
-        let g0 =
-            groupby_values_iter_full_lookbehind(period, offset, &dates, closed_window, tu, None, 0)
-                .collect::<PolarsResult<Vec<_>>>()
-                .unwrap();
+        let g0 = groupby_values_iter_lookbehind(period, offset, &dates, closed_window, tu, None, 0)
+            .collect::<PolarsResult<Vec<_>>>()
+            .unwrap();
         let g1 =
             groupby_values_iter_partial_lookbehind(period, offset, &dates, closed_window, tu, None)
                 .collect::<PolarsResult<Vec<_>>>()
                 .unwrap();
         assert_eq!(g0, g1);
     }
 }
```

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-time/src/windows/window.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-time/src/windows/window.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-utils/Cargo.toml` & `polars_u64_idx-0.18.4/local_dependencies/polars-utils/Cargo.toml`

 * *Files 20% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 resolver = "2"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 
 [dependencies]
 ahash= "0.8"
 hashbrown= { version = "0.13.1", features = ["rayon", "ahash"] }
+num-traits= "0.2"
 once_cell= "1"
 rayon= "1.6"
 smartstring= { version = "1" }
 sysinfo = { version = "0.29", default-features = false, optional = true }
 
 [features]
 bigidx = []
```

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-utils/LICENSE` & `polars_u64_idx-0.18.4/local_dependencies/polars-io/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-utils/src/arena.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-utils/src/arena.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-utils/src/atomic.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-utils/src/atomic.rs`

 * *Files 5% similar despite different names*

```diff
@@ -27,15 +27,15 @@
         SyncCounter { count }
     }
 
     /// # Safety
     /// This will deref the pointer and after this all autoderef will be invalid.
     pub unsafe fn manual_drop(&mut self) {
         // recreate the box and drop it
-        unsafe { Box::from_raw(self.count.as_ptr()) };
+        unsafe { drop(Box::from_raw(self.count.as_ptr())) };
     }
 }
 
 impl Deref for SyncCounter {
     type Target = AtomicUsize;
 
     fn deref(&self) -> &Self::Target {
```

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-utils/src/cell.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-utils/src/cell.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-utils/src/contention_pool.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-utils/src/contention_pool.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-utils/src/functions.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-utils/src/functions.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-utils/src/iter/enumerate_idx.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-utils/src/iter/enumerate_idx.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-utils/src/macros.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-utils/src/macros.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-utils/src/slice.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-utils/src/slice.rs`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 use core::slice::SliceIndex;
 use std::cmp::Ordering;
+use std::mem::MaybeUninit;
 
 pub trait Extrema<T> {
     fn min_value(&self) -> Option<&T>;
     fn max_value(&self) -> Option<&T>;
 }
 
 impl<T: PartialOrd> Extrema<T> for [T] {
@@ -86,7 +87,18 @@
         if cfg!(debug_assertions) {
             &mut self[index]
         } else {
             self.get_unchecked_mut(index)
         }
     }
 }
+
+pub trait Slice2Uninit<T> {
+    fn as_uninit(&self) -> &[MaybeUninit<T>];
+}
+
+impl<T> Slice2Uninit<T> for [T] {
+    #[inline]
+    fn as_uninit(&self) -> &[MaybeUninit<T>] {
+        unsafe { std::slice::from_raw_parts(self.as_ptr() as *const MaybeUninit<T>, self.len()) }
+    }
+}
```

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-utils/src/sort.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-utils/src/sort.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-utils/src/sync.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-utils/src/sync.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-utils/src/unwrap.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-utils/src/unwrap.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-utils/src/wasm.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-utils/src/wasm.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-row/Cargo.toml` & `polars_u64_idx-0.18.4/local_dependencies/polars-error/Cargo.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 [package]
-name = "polars-row"
-version= "0.30.0"
+name = "polars-error"
+version = "0.30.0"
 edition = "2021"
 license = "MIT"
 repository = "https://github.com/pola-rs/polars"
-description = "Row encodings for the Polars DataFrame library"
+description = "Error definitions for the Polars DataFrame library"
 resolver = "2"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 
 [dependencies]
-polars-error = { version = "0.30.0", path = "../polars-error" }
-polars-utils = { version = "0.30.0", path = "../polars-utils" }
+regex = { version = "1.6", optional = true }
+thiserror= "^1"
 
 [dependencies.arrow]
 package = "arrow2"
-git = "https://github.com/jorgecarleitao/arrow2"
-# git = "https://github.com/ritchie46/arrow2"
-rev = "2d2e7053f9a50810bfe9cecff25ab39089aef98e"
+# git = "https://github.com/jorgecarleitao/arrow2"
+git = "https://github.com/ritchie46/arrow2"
+# rev = "2d2e7053f9a50810bfe9cecff25ab39089aef98e"
 # path = "../arrow2"
-# branch = "polars_2023-05-25"
+branch = "polars_2023-06-23"
 version = "0.17"
 default-features = false
 features = [
   "compute_aggregate",
   "compute_arithmetics",
   "compute_boolean",
   "compute_boolean_kleene",
```

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-row/LICENSE` & `polars_u64_idx-0.18.4/local_dependencies/polars-lazy/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-row/src/decode.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-row/src/decode.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-row/src/encode.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-row/src/encode.rs`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 use arrow::array::{
     Array, BinaryArray, BooleanArray, DictionaryArray, PrimitiveArray, StructArray, Utf8Array,
 };
 use arrow::compute::cast::cast;
 use arrow::datatypes::{DataType as ArrowDataType, DataType};
 use arrow::types::NativeType;
+use polars_utils::vec::PushUnchecked;
 
 use crate::fixed::FixedLengthEncoding;
 use crate::row::{RowsEncoded, SortField};
 use crate::{with_match_arrow_primitive_type, ArrayRef};
 
 pub fn convert_columns(columns: &[ArrayRef], fields: &[SortField]) -> RowsEncoded {
     let mut rows = RowsEncoded::new(vec![], vec![]);
@@ -60,39 +61,46 @@
                 }
                 _ => {
                     flattened_columns.push(arr.clone());
                     flattened_fields.push(field.clone());
                 }
             }
         }
-        allocate_rows_buf(&flattened_columns, &mut rows.values, &mut rows.offsets);
+        let values_size =
+            allocate_rows_buf(&flattened_columns, &mut rows.values, &mut rows.offsets);
         for (arr, field) in flattened_columns.iter().zip(flattened_fields.iter()) {
             // Safety:
             // we allocated rows with enough bytes.
             unsafe { encode_array(&**arr, field, rows) }
         }
+        // safety: values are initialized
+        unsafe { rows.values.set_len(values_size) }
     } else {
-        allocate_rows_buf(columns, &mut rows.values, &mut rows.offsets);
+        let values_size = allocate_rows_buf(columns, &mut rows.values, &mut rows.offsets);
         for (arr, field) in columns.iter().zip(fields) {
             // Safety:
             // we allocated rows with enough bytes.
             unsafe { encode_array(&**arr, field, rows) }
         }
+        // safety: values are initialized
+        unsafe { rows.values.set_len(values_size) }
     }
 }
 
 fn encode_primitive<T: NativeType + FixedLengthEncoding>(
     arr: &PrimitiveArray<T>,
     field: &SortField,
     out: &mut RowsEncoded,
 ) {
     if arr.null_count() == 0 {
-        crate::fixed::encode_slice(arr.values().as_slice(), out, field);
+        unsafe { crate::fixed::encode_slice(arr.values().as_slice(), out, field) };
     } else {
-        crate::fixed::encode_iter(arr.into_iter().map(|v| v.copied()), out, field);
+        unsafe {
+            crate::fixed::encode_iter(arr.into_iter().map(|v| v.copied()), out, field);
+        }
     }
 }
 
 /// Ecnodes an array into `out`
 ///
 /// # Safety
 /// `out` must have enough bytes allocated otherwise it will be out of bounds.
@@ -143,15 +151,21 @@
         Float32 => f32::ENCODED_LEN,
         Float64 => f64::ENCODED_LEN,
         Boolean => bool::ENCODED_LEN,
         dt => unimplemented!("{dt:?}"),
     }
 }
 
-pub fn allocate_rows_buf(columns: &[ArrayRef], values: &mut Vec<u8>, offsets: &mut Vec<usize>) {
+// Returns the length that the caller must set on the `values` buf  once the bytes
+// are initialized.
+pub fn allocate_rows_buf(
+    columns: &[ArrayRef],
+    values: &mut Vec<u8>,
+    offsets: &mut Vec<usize>,
+) -> usize {
     let has_variable = columns.iter().any(|arr| {
         matches!(
             arr.data_type(),
             ArrowDataType::LargeBinary | ArrowDataType::Dictionary(_, _, _)
         )
     });
 
@@ -171,40 +185,62 @@
                     encoded_size(arr.data_type())
                 }
             })
             .sum();
 
         offsets.clear();
         offsets.reserve(num_rows + 1);
-        offsets.resize(num_rows, row_size_fixed);
 
         // first write lengths to this buffer
         let lengths = offsets;
 
         // for the variable length columns we must iterate to determine the length per row location
+        let mut processed_count = 0;
         for array in columns.iter() {
             match array.data_type() {
                 ArrowDataType::LargeBinary => {
                     let array = array.as_any().downcast_ref::<BinaryArray<i64>>().unwrap();
-                    for (opt_val, row_length) in array.into_iter().zip(lengths.iter_mut()) {
-                        *row_length += crate::variable::encoded_len(opt_val)
+                    if processed_count == 0 {
+                        for opt_val in array.into_iter() {
+                            unsafe {
+                                lengths.push_unchecked(
+                                    row_size_fixed + crate::variable::encoded_len(opt_val),
+                                );
+                            }
+                        }
+                    } else {
+                        for (opt_val, row_length) in array.into_iter().zip(lengths.iter_mut()) {
+                            *row_length += crate::variable::encoded_len(opt_val)
+                        }
                     }
+                    processed_count += 1;
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
-                    for (opt_val, row_length) in iter.zip(lengths.iter_mut()) {
-                        *row_length += crate::variable::encoded_len(opt_val)
+                    if processed_count == 0 {
+                        for opt_val in iter {
+                            unsafe {
+                                lengths.push_unchecked(
+                                    row_size_fixed + crate::variable::encoded_len(opt_val),
+                                )
+                            }
+                        }
+                    } else {
+                        for (opt_val, row_length) in iter.zip(lengths.iter_mut()) {
+                            *row_length += crate::variable::encoded_len(opt_val)
+                        }
                     }
+                    processed_count += 1;
                 }
                 _ => {
                     // the rest is fixed
                 }
             }
         }
         // now we use the lengths and the same buffer to determine the offsets
@@ -219,31 +255,25 @@
             current_offset += *length;
 
             *length = to_write;
         }
         // ensure we have len + 1 offsets
         offsets.push(lagged_offset);
 
-        values.clear();
-        // todo! allocate uninit
-        values.resize(current_offset, 0u8);
+        // Only reserve. The init will be done later
+        values.reserve(current_offset);
+        current_offset
     } else {
         let row_size: usize = columns
             .iter()
             .map(|arr| encoded_size(arr.data_type()))
             .sum();
         let n_bytes = num_rows * row_size;
-        // todo! allocate uninit
-        if values.capacity() == 0 {
-            // it is faster to allocate zeroed
-            // so if the capacity is 0, we alloc
-            *values = vec![0u8; n_bytes]
-        } else {
-            values.resize(n_bytes, 0u8);
-        }
+        values.clear();
+        values.reserve(n_bytes);
 
         // note that offsets are shifted to the left
         // assume 2 fields with a len of 1
         // e.g. in arrow we would have 0, 2, 4, 6
 
         // now we write 0, 0, 2, 4
 
@@ -257,25 +287,39 @@
         offsets.reserve(num_rows + 1);
         let mut current_offset = 0;
         offsets.push(current_offset);
         for _ in 0..num_rows {
             offsets.push(current_offset);
             current_offset += row_size;
         }
+        n_bytes
     }
 }
 
 #[cfg(test)]
 mod test {
-    use arrow::array::Utf8Array;
+    use arrow::array::{Int32Array, Utf8Array};
 
     use super::*;
     use crate::variable::{BLOCK_SIZE, EMPTY_SENTINEL, NON_EMPTY_SENTINEL};
 
     #[test]
+    fn test_fixed_and_variable_encode() {
+        let a = Int32Array::from_vec(vec![1, 2, 3]);
+        let b = Int32Array::from_vec(vec![213, 12, 12]);
+        let c = Utf8Array::<i64>::from_iter([Some("a"), Some(""), Some("meep")]);
+
+        let encoded = convert_columns_no_order(&[Box::new(a), Box::new(b), Box::new(c)]);
+        assert_eq!(encoded.offsets, &[0, 44, 55, 99,]);
+        assert_eq!(encoded.values.len(), 99);
+        assert!(encoded.values.ends_with(&[0, 0, 0, 4]));
+        assert!(encoded.values.starts_with(&[1, 128, 0, 0, 1, 1, 128]));
+    }
+
+    #[test]
     fn test_str_encode() {
         let sentence = "The black cat walked under a ladder but forget it's milk so it ...";
         let arr =
             Utf8Array::<i64>::from_iter([Some("a"), Some(""), Some("meep"), Some(sentence), None]);
 
         let field = SortField {
             descending: false,
```

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-row/src/fixed.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-row/src/fixed.rs`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+use std::mem::MaybeUninit;
+
 use arrow::array::{BooleanArray, PrimitiveArray};
 use arrow::bitmap::Bitmap;
 use arrow::datatypes::DataType;
 use arrow::types::NativeType;
 use polars_utils::slice::*;
 
 use crate::row::{RowsEncoded, SortField};
@@ -135,62 +137,69 @@
 }
 
 #[inline]
 fn encode_value<T: FixedLengthEncoding>(
     value: &T,
     offset: &mut usize,
     descending: bool,
-    buf: &mut [u8],
+    buf: &mut [MaybeUninit<u8>],
 ) {
     let end_offset = *offset + T::ENCODED_LEN;
     let dst = unsafe { buf.get_unchecked_release_mut(*offset..end_offset) };
     // set valid
-    dst[0] = 1;
+    dst[0] = MaybeUninit::new(1);
     let mut encoded = value.encode();
 
     // invert bits to reverse order
     if descending {
         for v in encoded.as_mut() {
             *v = !*v
         }
     }
 
-    dst[1..].copy_from_slice(encoded.as_ref());
+    dst[1..].copy_from_slice(encoded.as_ref().as_uninit());
     *offset = end_offset;
 }
 
-pub(crate) fn encode_slice<T: FixedLengthEncoding>(
+pub(crate) unsafe fn encode_slice<T: FixedLengthEncoding>(
     input: &[T],
     out: &mut RowsEncoded,
     field: &SortField,
 ) {
+    out.values.set_len(0);
+    let values = out.values.spare_capacity_mut();
     for (offset, value) in out.offsets.iter_mut().skip(1).zip(input) {
-        encode_value(value, offset, field.descending, &mut out.values);
+        encode_value(value, offset, field.descending, values);
     }
 }
 
 #[inline]
 pub(crate) fn get_null_sentinel(field: &SortField) -> u8 {
     if field.nulls_last {
         0xFF
     } else {
         0
     }
 }
 
-pub(crate) fn encode_iter<I: Iterator<Item = Option<T>>, T: FixedLengthEncoding>(
+pub(crate) unsafe fn encode_iter<I: Iterator<Item = Option<T>>, T: FixedLengthEncoding>(
     input: I,
     out: &mut RowsEncoded,
     field: &SortField,
 ) {
+    out.values.set_len(0);
+    let values = out.values.spare_capacity_mut();
     for (offset, opt_value) in out.offsets.iter_mut().skip(1).zip(input) {
         if let Some(value) = opt_value {
-            encode_value(&value, offset, field.descending, &mut out.values);
+            encode_value(&value, offset, field.descending, values);
         } else {
-            unsafe { *out.values.get_unchecked_release_mut(*offset) = get_null_sentinel(field) };
+            unsafe {
+                *values.get_unchecked_release_mut(*offset) =
+                    MaybeUninit::new(get_null_sentinel(field))
+            };
             let end_offset = *offset + T::ENCODED_LEN;
             *offset = end_offset;
         }
     }
 }
 
 pub(super) unsafe fn decode_primitive<T: NativeType + FixedLengthEncoding>(
```

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-row/src/lib.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-row/src/lib.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-row/src/row.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-row/src/row.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-row/src/utils.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-row/src/utils.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-row/src/variable.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-row/src/variable.rs`

 * *Files 7% similar despite different names*

```diff
@@ -6,18 +6,20 @@
 //!
 //! where a block is encoded as
 //!
 //! - [`BLOCK_SIZE`] bytes of string data, padded with 0s
 //! - `0xFF_u8` if this is not the last block for this string
 //! - otherwise the length of the block as a `u8`
 
+use std::mem::MaybeUninit;
+
 use arrow::array::BinaryArray;
 use arrow::datatypes::DataType;
 use arrow::offset::Offsets;
-use polars_utils::slice::GetSaferUnchecked;
+use polars_utils::slice::{GetSaferUnchecked, Slice2Uninit};
 
 use crate::fixed::{decode_nulls, get_null_sentinel};
 use crate::row::RowsEncoded;
 use crate::SortField;
 
 /// The block size of the variable length encoding
 pub(crate) const BLOCK_SIZE: usize = 32;
@@ -58,89 +60,112 @@
     padded_length_opt(a.map(|v| v.len()))
 }
 
 /// Encode one strings/bytes object and return the written length.
 ///
 /// # Safety
 /// `out` must have allocated enough room
-unsafe fn encode_one(out: &mut [u8], val: Option<&[u8]>, field: &SortField) -> usize {
+unsafe fn encode_one(
+    out: &mut [MaybeUninit<u8>],
+    val: Option<&[MaybeUninit<u8>]>,
+    field: &SortField,
+) -> usize {
     match val {
         Some(val) if val.is_empty() => {
             let byte = if field.descending {
                 !EMPTY_SENTINEL
             } else {
                 EMPTY_SENTINEL
             };
-            *out.get_unchecked_release_mut(0) = byte;
+            *out.get_unchecked_release_mut(0) = MaybeUninit::new(byte);
+            // write remainder as zeros
+            out.get_unchecked_release_mut(1..).fill(MaybeUninit::new(0));
             1
         }
         Some(val) => {
             let block_count = ceil(val.len(), BLOCK_SIZE);
             let end_offset = 1 + block_count * (BLOCK_SIZE + 1);
 
             let dst = out.get_unchecked_release_mut(..end_offset);
 
             // Write `2_u8` to demarcate as non-empty, non-null string
-            *dst.get_unchecked_release_mut(0) = NON_EMPTY_SENTINEL;
+            *dst.get_unchecked_release_mut(0) = MaybeUninit::new(NON_EMPTY_SENTINEL);
 
             let src_chunks = val.chunks_exact(BLOCK_SIZE);
             let src_remainder = src_chunks.remainder();
 
             // + 1 is for the BLOCK CONTINUATION TOKEN
             let dst_chunks = dst
                 .get_unchecked_release_mut(1..)
                 .chunks_exact_mut(BLOCK_SIZE + 1);
 
             for (src, dst) in src_chunks.zip(dst_chunks) {
                 // we copy src.len() that leaves 1 bytes for the continuation tkn.
                 std::ptr::copy_nonoverlapping(src.as_ptr(), dst.as_mut_ptr(), src.len());
                 // Indicate that there are further blocks to follow
-                *dst.get_unchecked_release_mut(BLOCK_SIZE) = BLOCK_CONTINUATION_TOKEN;
+                *dst.get_unchecked_release_mut(BLOCK_SIZE) =
+                    MaybeUninit::new(BLOCK_CONTINUATION_TOKEN);
             }
 
             if src_remainder.is_empty() {
+                // get the last block
+                let start_offset = 1 + (block_count - 1) * (BLOCK_SIZE + 1);
+                let last_dst = dst.get_unchecked_release_mut(start_offset..);
+                last_dst.fill(MaybeUninit::new(0));
+
                 // overwrite the latest continuation marker.
                 // replace the "there is another block" with
                 // "we are finished this, this is the length of this block"
-                *dst.last_mut().unwrap_unchecked() = BLOCK_SIZE as u8;
+                *dst.last_mut().unwrap_unchecked() = MaybeUninit::new(BLOCK_SIZE as u8);
             } else {
                 // get the last block
                 let start_offset = 1 + (block_count - 1) * (BLOCK_SIZE + 1);
                 let last_dst = dst.get_unchecked_release_mut(start_offset..);
+                let n_bytes_to_write = src_remainder.len();
+
                 std::ptr::copy_nonoverlapping(
                     src_remainder.as_ptr(),
                     last_dst.as_mut_ptr(),
-                    src_remainder.len(),
+                    n_bytes_to_write,
                 );
-                *dst.last_mut().unwrap_unchecked() = src_remainder.len() as u8;
+                // write remainder as zeros
+                last_dst
+                    .get_unchecked_release_mut(n_bytes_to_write..last_dst.len() - 1)
+                    .fill(MaybeUninit::new(0));
+                *dst.last_mut().unwrap_unchecked() = MaybeUninit::new(src_remainder.len() as u8);
             }
 
             if field.descending {
                 for byte in dst {
-                    *byte = !*byte;
+                    *byte = MaybeUninit::new(!byte.assume_init());
                 }
             }
             end_offset
         }
         None => {
-            *out.get_unchecked_release_mut(0) = get_null_sentinel(field);
+            *out.get_unchecked_release_mut(0) = MaybeUninit::new(get_null_sentinel(field));
+            // write remainder as zeros
+            out.get_unchecked_release_mut(1..).fill(MaybeUninit::new(0));
             1
         }
     }
 }
 pub(crate) unsafe fn encode_iter<'a, I: Iterator<Item = Option<&'a [u8]>>>(
     input: I,
     out: &mut RowsEncoded,
     field: &SortField,
 ) {
+    out.values.set_len(0);
+    let values = out.values.spare_capacity_mut();
     for (offset, opt_value) in out.offsets.iter_mut().skip(1).zip(input) {
-        let dst = out.values.get_unchecked_release_mut(*offset..);
-        let written_len = encode_one(dst, opt_value, field);
+        let dst = values.get_unchecked_release_mut(*offset..);
+        let written_len = encode_one(dst, opt_value.map(|v| v.as_uninit()), field);
         *offset += written_len;
     }
+    out.values.set_len(out.values.capacity())
 }
 
 unsafe fn has_nulls(rows: &[&[u8]], null_sentinel: u8) -> bool {
     rows.iter()
         .any(|row| *row.get_unchecked(0) == null_sentinel)
 }
```

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-sql/Cargo.toml` & `polars_u64_idx-0.18.4/local_dependencies/polars-sql/Cargo.toml`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-sql/LICENSE` & `polars_u64_idx-0.18.4/local_dependencies/polars-ops/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-sql/src/context.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-sql/src/context.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-sql/src/functions.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-sql/src/functions.rs`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 use polars_core::prelude::{polars_bail, polars_err, PolarsError, PolarsResult};
 use polars_lazy::dsl::Expr;
 use polars_plan::dsl::count;
+use polars_plan::logical_plan::LiteralValue;
 use sqlparser::ast::{
     Expr as SqlExpr, Function as SQLFunction, FunctionArg, FunctionArgExpr, Value as SqlValue,
     WindowSpec, WindowType,
 };
 
 use crate::sql_expr::parse_sql_expr;
 use crate::SQLContext;
@@ -20,14 +21,54 @@
     // Math functions
     // ----
     /// SQL 'abs' function
     /// ```sql
     /// SELECT ABS(column_1) from df;
     /// ```
     Abs,
+    /// SQL 'cos' function
+    /// ```sql
+    /// SELECT COS(column_1) from df;
+    /// ```
+    Cos,
+    /// SQL 'cot' function
+    /// ```sql
+    /// SELECT COT(column_1) from df;
+    /// ```
+    Cot,
+    /// SQL 'sin' function
+    /// ```sql
+    /// SELECT SIN(column_1) from df;
+    /// ```
+    Sin,
+    /// SQL 'tan' function
+    /// ```sql
+    /// SELECT TAN(column_1) from df;
+    /// ```
+    Tan,
+    /// SQL 'cosd' function
+    /// ```sql
+    /// SELECT COSD(column_1) from df;
+    /// ```
+    CosD,
+    /// SQL 'cotd' function
+    /// ```sql
+    /// SELECT COTD(column_1) from df;
+    /// ```
+    CotD,
+    /// SQL 'sind' function
+    /// ```sql
+    /// SELECT SIND(column_1) from df;
+    /// ```
+    SinD,
+    /// SQL 'tand' function
+    /// ```sql
+    /// SELECT TAND(column_1) from df;
+    /// ```
+    TanD,
     /// SQL 'acos' function
     /// ```sql
     /// SELECT ACOS(column_1) from df;
     /// ```
     Acos,
     /// SQL 'asin' function
     /// ```sql
@@ -35,14 +76,29 @@
     /// ```
     Asin,
     /// SQL 'atan' function
     /// ```sql
     /// SELECT ATAN(column_1) from df;
     /// ```
     Atan,
+    /// SQL 'acosd' function
+    /// ```sql
+    /// SELECT ACOSD(column_1) from df;
+    /// ```
+    AcosD,
+    /// SQL 'asind' function
+    /// ```sql
+    /// SELECT ASIND(column_1) from df;
+    /// ```
+    AsinD,
+    /// SQL 'atand' function
+    /// ```sql
+    /// SELECT ATAND(column_1) from df;
+    /// ```
+    AtanD,
     /// SQL 'ceil' function
     /// ```sql
     /// SELECT CEIL(column_1) from df;
     /// ```
     Ceil,
     /// SQL 'exp' function
     /// ```sql
@@ -80,14 +136,19 @@
     /// ```
     Log1p,
     /// SQL 'pow' function
     /// ```sql
     /// SELECT POW(column_1, 2) from df;
     /// ```
     Pow,
+    /// SQL 'round' function
+    /// ```sql
+    /// SELECT ROUND(column_1, 3) from df;
+    /// ```
+    Round,
     // ----
     // String functions
     // ----
     /// SQL 'lower' function
     /// ```sql
     /// SELECT LOWER(column_1) from df;
     /// ```
@@ -174,14 +235,24 @@
     // Array functions
     // ----
     /// SQL 'array_length' function
     /// ```sql
     /// SELECT ARRAY_LENGTH(column_1) from df;
     /// ```
     ArrayLength,
+    /// SQL 'degrees' function
+    /// ```sql
+    /// SELECT DEGREES(column_1) from df;
+    /// ```
+    Degrees,
+    /// SQL 'RADIANS' function
+    /// ```sql
+    /// SELECT radians(column_1) from df;
+    /// ```
+    Radians,
     /// SQL 'array_lower' function
     /// Returns the minimum value in an array; equivalent to `array_min`
     /// ```sql
     /// SELECT ARRAY_LOWER(column_1) from df;
     /// ```
     ArrayMin,
     /// SQL 'array_upper' function
@@ -235,29 +306,37 @@
 }
 
 impl PolarsSqlFunctions {
     pub(crate) fn keywords() -> &'static [&'static str] {
         &[
             "abs",
             "acos",
+            "acosd",
             "array_contains",
             "array_get",
             "array_length",
             "array_lower",
             "array_mean",
             "array_reverse",
             "array_sum",
             "array_unique",
             "array_upper",
             "asin",
+            "asind",
             "atan",
+            "atand",
             "avg",
             "ceil",
             "ceiling",
+            "cos",
+            "cosd",
+            "cot",
+            "cotd",
             "count",
+            "degrees",
             "ends_with",
             "exp",
             "first",
             "floor",
             "last",
             "len",
             "length",
@@ -267,18 +346,26 @@
             "log1p",
             "log2",
             "lower",
             "ltrim",
             "max",
             "min",
             "pow",
+            "radians",
+            "round",
             "rtrim",
+            "sin",
+            "sind",
             "starts_with",
             "stddev",
             "sum",
+            "tan",
+            "tan",
+            "tand",
+            "tand",
             "unnest",
             "upper",
             "variance",
         ]
     }
 }
 
@@ -287,26 +374,40 @@
     fn try_from(function: &'_ SQLFunction) -> Result<Self, Self::Error> {
         let function_name = function.name.0[0].value.to_lowercase();
         Ok(match function_name.as_str() {
             // ----
             // Math functions
             // ----
             "abs" => Self::Abs,
+            "cos" => Self::Cos,
+            "cot" => Self::Cot,
+            "sin" => Self::Sin,
+            "tan" => Self::Tan,
+            "cosd" => Self::CosD,
+            "cotd" => Self::CotD,
+            "sind" => Self::SinD,
+            "tand" => Self::TanD,
             "acos" => Self::Acos,
             "asin" => Self::Asin,
             "atan" => Self::Atan,
+            "acosd" => Self::AcosD,
+            "asind" => Self::AsinD,
+            "atand" => Self::AtanD,
+            "degrees" => Self::Degrees,
+            "radians" => Self::Radians,
             "ceil" | "ceiling" => Self::Ceil,
             "exp" => Self::Exp,
             "floor" => Self::Floor,
             "ln" => Self::Ln,
             "log" => Self::Log,
             "log10" => Self::Log10,
             "log1p" => Self::Log1p,
             "log2" => Self::Log2,
             "pow" => Self::Pow,
+            "round" => Self::Round,
             // ----
             // String functions
             // ----
             "ends_with" => Self::EndsWith,
             "lower" => Self::Lower,
             "ltrim" => Self::LTrim,
             "rtrim" => Self::RTrim,
@@ -350,43 +451,70 @@
         use PolarsSqlFunctions::*;
 
         match function_name {
             // ----
             // Math functions
             // ----
             Abs => self.visit_unary(Expr::abs),
+            Cos => self.visit_unary(Expr::cos),
+            Cot => self.visit_unary(Expr::cot),
+            Sin => self.visit_unary(Expr::sin),
+            Tan => self.visit_unary(Expr::tan),
+            CosD => self.visit_unary(|e| e.radians().cos()),
+            CotD => self.visit_unary(|e| e.radians().cot()),
+            SinD => self.visit_unary(|e| e.radians().sin()),
+            TanD => self.visit_unary(|e| e.radians().tan()),
             Acos => self.visit_unary(Expr::arccos),
             Asin => self.visit_unary(Expr::arcsin),
             Atan => self.visit_unary(Expr::arctan),
+            AcosD => self.visit_unary(|e| e.arccos().degrees()),
+            AsinD => self.visit_unary(|e| e.arcsin().degrees()),
+            AtanD => self.visit_unary(|e| e.arctan().degrees()),
+            Degrees => self.visit_unary(Expr::degrees),
+            Radians => self.visit_unary(Expr::radians),
             Ceil => self.visit_unary(Expr::ceil),
             Exp => self.visit_unary(Expr::exp),
             Floor => self.visit_unary(Expr::floor),
             Ln => self.visit_unary(|e| e.log(std::f64::consts::E)),
             Log => self.visit_binary(Expr::log),
             Log10 => self.visit_unary(|e| e.log(10.0)),
             Log1p => self.visit_unary(Expr::log1p),
             Log2 => self.visit_unary(|e| e.log(2.0)),
             Pow => self.visit_binary::<Expr>(Expr::pow),
+            Round => match function.args.len() {
+                1 => self.visit_unary(|e| e.round(0)),
+                2 => self.try_visit_binary(|e, decimals| {
+                    Ok(e.round(match decimals {
+                        Expr::Literal(LiteralValue::Int64(n)) => n as u32,
+                        _ => {
+                            polars_bail!(InvalidOperation: "Invalid 'decimals' for Round: {}", function.args[1]);
+                        }
+                    }))
+                }),
+                _ => {
+                    polars_bail!(InvalidOperation:"Invalid number of arguments for Round: {}",function.args.len());
+                },
+            },
             // ----
             // String functions
             // ----
             EndsWith => self.visit_binary(|e, s| e.str().ends_with(s)),
             Lower => self.visit_unary(|e| e.str().to_lowercase()),
             LTrim => match function.args.len() {
                 1 => self.visit_unary(|e| e.str().lstrip(None)),
                 2 => self.visit_binary(|e, s| e.str().lstrip(Some(s))),
-                _ => panic!(
+                _ => polars_bail!(InvalidOperation:
                     "Invalid number of arguments for LTrim: {}",
                     function.args.len()
                 ),
             },
             RTrim => match function.args.len() {
                 1 => self.visit_unary(|e| e.str().rstrip(None)),
                 2 => self.visit_binary(|e, s| e.str().rstrip(Some(s))),
-                _ => panic!(
+                _ => polars_bail!(InvalidOperation:
                     "Invalid number of arguments for RTrim: {}",
                     function.args.len()
                 ),
             },
             StartsWith => self.visit_binary(|e, s| e.str().starts_with(s)),
             Upper => self.visit_unary(|e| e.str().to_uppercase()),
             // ----
@@ -472,74 +600,67 @@
         } else {
             self.visit_unary(f)
         }
     }
 
     fn visit_unary_no_window(&self, f: impl Fn(Expr) -> Expr) -> PolarsResult<Expr> {
         let function = self.func;
+
         let args = extract_args(function);
-        if let FunctionArgExpr::Expr(sql_expr) = args[0] {
-            // parse the inner sql expr -- e.g. SUM(a) -> a
-            let expr = parse_sql_expr(sql_expr, self.ctx)?;
-            // apply the function on the inner expr -- e.g. SUM(a) -> SUM
-            Ok(f(expr))
-        } else {
-            not_supported_error(function.name.0[0].value.as_str(), &args)
+        match args.as_slice() {
+            [FunctionArgExpr::Expr(sql_expr)] => {
+                let expr = parse_sql_expr(sql_expr, self.ctx)?;
+                // apply the function on the inner expr -- e.g. SUM(a) -> SUM
+                Ok(f(expr))
+            }
+            _ => self.not_supported_error(),
         }
     }
 
     fn visit_binary<Arg: FromSqlExpr>(&self, f: impl Fn(Expr, Arg) -> Expr) -> PolarsResult<Expr> {
+        self.try_visit_binary(|e, a| Ok(f(e, a)))
+    }
+
+    fn try_visit_binary<Arg: FromSqlExpr>(
+        &self,
+        f: impl Fn(Expr, Arg) -> PolarsResult<Expr>,
+    ) -> PolarsResult<Expr> {
         let function = self.func;
         let args = extract_args(function);
-        if let FunctionArgExpr::Expr(sql_expr) = args[0] {
-            let expr =
-                self.apply_window_spec(parse_sql_expr(sql_expr, self.ctx)?, &function.over)?;
-            if let FunctionArgExpr::Expr(sql_expr) = args[1] {
-                let expr2 = Arg::from_sql_expr(sql_expr, self.ctx)?;
-                Ok(f(expr, expr2))
-            } else {
-                not_supported_error(function.name.0[0].value.as_str(), &args)
+        match args.as_slice() {
+            [FunctionArgExpr::Expr(sql_expr), FunctionArgExpr::Expr(sql_expr2)] => {
+                let expr = parse_sql_expr(sql_expr, self.ctx)?;
+                let expr2 = Arg::from_sql_expr(sql_expr2, self.ctx)?;
+                f(expr, expr2)
             }
-        } else {
-            not_supported_error(function.name.0[0].value.as_str(), &args)
+            _ => self.not_supported_error(),
         }
     }
 
     fn visit_count(&self) -> PolarsResult<Expr> {
         let args = extract_args(self.func);
-        Ok(match (args.len(), self.func.distinct) {
+        match (self.func.distinct, args.as_slice()) {
             // count()
-            (0, false) => count(),
-            // count(distinct)
-            (0, true) => return not_supported_error("count", &args),
-            (1, false) => match args[0] {
-                // count(col)
-                FunctionArgExpr::Expr(sql_expr) => {
-                    let expr = self
-                        .apply_window_spec(parse_sql_expr(sql_expr, self.ctx)?, &self.func.over)?;
-                    expr.count()
-                }
-                // count(*)
-                FunctionArgExpr::Wildcard => count(),
-                // count(tbl.*) is not supported
-                _ => return not_supported_error("count", &args),
-            },
-            (1, true) => {
-                // count(distinct col)
-                if let FunctionArgExpr::Expr(sql_expr) = args[0] {
-                    let expr = self
-                        .apply_window_spec(parse_sql_expr(sql_expr, self.ctx)?, &self.func.over)?;
-                    expr.n_unique()
-                } else {
-                    // count(distinct *) or count(distinct tbl.*) is not supported
-                    return not_supported_error("count", &args);
-                }
+            (false, []) => Ok(count()),
+            // count(column_name)
+            (false, [FunctionArgExpr::Expr(sql_expr)]) => {
+                let expr =
+                    self.apply_window_spec(parse_sql_expr(sql_expr, self.ctx)?, &self.func.over)?;
+                Ok(expr.count())
             }
-            _ => return not_supported_error("count", &args),
-        })
+            // count(*)
+            (false, [FunctionArgExpr::Wildcard]) => Ok(count()),
+            // count(distinct column_name)
+            (true, [FunctionArgExpr::Expr(sql_expr)]) => {
+                let expr =
+                    self.apply_window_spec(parse_sql_expr(sql_expr, self.ctx)?, &self.func.over)?;
+                Ok(expr.n_unique())
+            }
+            _ => self.not_supported_error(),
+        }
     }
 
     fn apply_window_spec(
         &self,
         expr: Expr,
         window_type: &Option<WindowType>,
     ) -> PolarsResult<Expr> {
@@ -571,22 +692,22 @@
             Some(WindowType::NamedWindow(named_window)) => polars_bail!(
                 InvalidOperation: "Named windows are not supported yet. Got: {:?}",
                 named_window
             ),
             None => expr,
         })
     }
-}
 
-fn not_supported_error(function_name: &str, args: &Vec<&FunctionArgExpr>) -> PolarsResult<Expr> {
-    polars_bail!(
-        InvalidOperation:
-        "function `{}` with args {:?} is not supported in polars-sql",
-        function_name, args
-    );
+    fn not_supported_error(&self) -> PolarsResult<Expr> {
+        polars_bail!(
+            InvalidOperation:
+            "No function matches the given name and arguments: `{}`",
+            self.func.to_string()
+        );
+    }
 }
 
 fn extract_args(sql_function: &SQLFunction) -> Vec<&FunctionArgExpr> {
     sql_function
         .args
         .iter()
         .map(|arg| match arg {
```

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-sql/src/keywords.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-sql/src/keywords.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-sql/src/sql_expr.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-sql/src/sql_expr.rs`

 * *Files 0% similar despite different names*

```diff
@@ -135,15 +135,14 @@
 
     fn visit_unary_op(&self, op: &UnaryOperator, expr: &SqlExpr) -> PolarsResult<Expr> {
         let expr = self.visit_expr(expr)?;
         Ok(match op {
             UnaryOperator::Plus => lit(0) + expr,
             UnaryOperator::Minus => lit(0) - expr,
             UnaryOperator::Not => expr.not(),
-            UnaryOperator::PGSquareRoot => expr.pow(0.5),
             other => polars_bail!(InvalidOperation: "Unary operator {:?} is not supported", other),
         })
     }
 
     /// Visit a single identifier
     ///
     /// e.g. column
```

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-sql/src/table_functions.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-sql/src/table_functions.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-sql/tests/functions_cumulative.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-sql/tests/functions_cumulative.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-sql/tests/functions_io.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-sql/tests/functions_io.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-sql/tests/functions_math.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-sql/tests/functions_math.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-sql/tests/functions_meta.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-sql/tests/functions_meta.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-sql/tests/functions_string.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-sql/tests/functions_string.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-sql/tests/iss_7436.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-sql/tests/iss_7436.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-sql/tests/iss_7437.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-sql/tests/iss_7437.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-sql/tests/iss_7440.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-sql/tests/iss_7440.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-sql/tests/iss_8395.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-sql/tests/iss_8395.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-sql/tests/iss_8419.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-sql/tests/iss_8419.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-sql/tests/ops_distinct_on.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-sql/tests/ops_distinct_on.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-sql/tests/simple_exprs.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-sql/tests/simple_exprs.rs`

 * *Files 1% similar despite different names*

```diff
@@ -529,7 +529,24 @@
 fn test_sql_expr() {
     let df = create_sample_df().unwrap();
     let expr = sql_expr("MIN(a)").unwrap();
     let actual = df.clone().lazy().select(&[expr]).collect().unwrap();
     let expected = df.lazy().select(&[col("a").min()]).collect().unwrap();
     assert!(actual.frame_equal(&expected));
 }
+
+#[test]
+fn test_iss_9471() {
+    let sql = r#"
+    SELECT 
+        ABS(a,a,a,a,1,2,3,XYZRandomLetters,"XYZRandomLetters") as "abs",
+    FROM df"#;
+    let df = df! {
+        "a" => [-4, -3, -2, -1, 0, 1, 2, 3, 4],
+    }
+    .unwrap()
+    .lazy();
+    let mut context = SQLContext::new();
+    context.register("df", df.clone());
+    let res = context.execute(sql);
+    assert!(res.is_err())
+}
```

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-sql/tests/statements.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-sql/tests/statements.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/Cargo.toml` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/Cargo.toml`

 * *Files 0% similar despite different names*

```diff
@@ -176,19 +176,19 @@
 smartstring= { version = "1" }
 thiserror= "^1"
 url = { version = "2.3.1", optional = true }
 xxhash-rust= { version = "0.8.6", features = ["xxh3"] }
 
 [dependencies.arrow]
 package = "arrow2"
-git = "https://github.com/jorgecarleitao/arrow2"
-# git = "https://github.com/ritchie46/arrow2"
-rev = "2d2e7053f9a50810bfe9cecff25ab39089aef98e"
+# git = "https://github.com/jorgecarleitao/arrow2"
+git = "https://github.com/ritchie46/arrow2"
+# rev = "2d2e7053f9a50810bfe9cecff25ab39089aef98e"
 # path = "../arrow2"
-# branch = "polars_2023-05-25"
+branch = "polars_2023-06-23"
 version = "0.17"
 default-features = false
 features = [
   "compute_aggregate",
   "compute_arithmetics",
   "compute_boolean",
   "compute_boolean_kleene",
```

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/LICENSE` & `polars_u64_idx-0.18.4/local_dependencies/polars-sql/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/arithmetic/decimal.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/arithmetic/decimal.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/arithmetic/mod.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/arithmetic/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/arithmetic/numeric.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/arithmetic/numeric.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/array/iterator.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/array/iterator.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/array/mod.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/array/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/bitwise.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/bitwise.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/builder/binary.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/builder/binary.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/builder/boolean.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/builder/boolean.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/builder/fixed_size_list.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/builder/fixed_size_list.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/builder/from.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/builder/from.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/builder/list.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/builder/list.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/builder/mod.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/builder/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/builder/primitive.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/builder/primitive.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/builder/utf8.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/builder/utf8.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/cast.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/cast.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/comparison/mod.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/comparison/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/comparison/scalar.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/comparison/scalar.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/drop.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/drop.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/float.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/float.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/from.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/from.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/iterator/mod.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/iterator/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/iterator/par/list.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/iterator/par/list.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/iterator/par/utf8.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/iterator/par/utf8.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/kernels/take.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/kernels/take.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/list/iterator.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/list/iterator.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/list/mod.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/list/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/logical/categorical/builder.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/logical/categorical/builder.rs`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 use std::fmt::{Debug, Formatter};
 use std::hash::{Hash, Hasher};
 
 use arrow::array::*;
 use hashbrown::hash_map::{Entry, RawEntryMut};
-use polars_arrow::trusted_len::PushUnchecked;
+use polars_arrow::trusted_len::TrustedLenPush;
 
 use crate::datatypes::PlHashMap;
 use crate::frame::groupby::hashing::HASHMAP_INIT_SIZE;
 use crate::prelude::*;
 use crate::{using_string_cache, StringCache, POOL};
 
 pub enum RevMappingBuilder {
```

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/logical/categorical/from.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/logical/categorical/from.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/logical/categorical/merge.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/logical/categorical/merge.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/logical/categorical/mod.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/logical/categorical/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/append.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/append.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/take_random.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/take_random.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/unique.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/unique.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/zip.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/zip.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/logical/categorical/stringcache.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/logical/categorical/stringcache.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/logical/date.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/logical/date.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/logical/datetime.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/logical/datetime.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/logical/decimal.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/logical/decimal.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/logical/duration.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/logical/duration.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/logical/mod.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/logical/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/logical/struct_/mod.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/logical/struct_/mod.rs`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 use std::collections::BTreeMap;
 use std::io::Write;
 use std::ops::BitAnd;
 
 use arrow::bitmap::MutableBitmap;
 use arrow::offset::OffsetsBuffer;
-use polars_arrow::trusted_len::PushUnchecked;
+use polars_arrow::trusted_len::TrustedLenPush;
 use smartstring::alias::String as SmartString;
 
 use super::*;
 use crate::datatypes::*;
 use crate::utils::index_to_chunked_index2;
 
 /// This is logical type [`StructChunked`] that
```

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/logical/time.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/logical/time.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/mod.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/ndarray.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/ndarray.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/object/builder.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/object/builder.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/object/extension/drop.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/object/extension/drop.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/object/extension/list.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/object/extension/list.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/object/extension/mod.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/object/extension/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/object/extension/polars_extension.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/object/extension/polars_extension.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/object/iterator.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/object/iterator.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/object/mod.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/object/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/object/registry.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/object/registry.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/ops/aggregate/mod.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/ops/aggregate/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/ops/aggregate/quantile.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/ops/aggregate/quantile.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/ops/aggregate/var.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/ops/aggregate/var.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/ops/any_value.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/ops/any_value.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/ops/apply.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/ops/apply.rs`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 //! Implementations of the ChunkApply Trait.
 use std::borrow::Cow;
 use std::convert::TryFrom;
 
 use arrow::array::{BooleanArray, PrimitiveArray};
 use polars_arrow::array::PolarsArray;
-use polars_arrow::trusted_len::PushUnchecked;
+use polars_arrow::trusted_len::TrustedLenPush;
 
 use crate::prelude::*;
 use crate::series::IsSorted;
 use crate::utils::{CustomIterTools, NoNull};
 
 macro_rules! try_apply {
     ($self:expr, $f:expr) => {{
```

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/ops/bit_repr.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/ops/bit_repr.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/ops/chunkops.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/ops/chunkops.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/ops/compare_inner.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/ops/compare_inner.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/ops/concat_str.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/ops/concat_str.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/ops/cum_agg.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/ops/cum_agg.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/ops/decimal.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/ops/decimal.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/ops/downcast.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/ops/downcast.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/ops/explode.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/ops/explode.rs`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 use arrow::bitmap::{Bitmap, MutableBitmap};
 use polars_arrow::array::list::AnonymousBuilder;
 use polars_arrow::array::PolarsArray;
 use polars_arrow::bit_util::unset_bit_raw;
 #[cfg(feature = "dtype-array")]
 use polars_arrow::is_valid::IsValid;
 use polars_arrow::prelude::*;
-use polars_arrow::trusted_len::PushUnchecked;
+use polars_arrow::trusted_len::TrustedLenPush;
 
 #[cfg(feature = "dtype-array")]
 use crate::chunked_array::builder::get_fixed_size_list_builder;
 use crate::prelude::*;
 use crate::series::implementations::null::NullChunked;
 
 pub(crate) trait ExplodeByOffsets {
```

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/ops/explode_and_offsets.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/ops/explode_and_offsets.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/ops/extend.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/ops/extend.rs`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 use arrow::compute::concatenate::concatenate;
 use arrow::Either;
 
+use crate::prelude::append::update_sorted_flag_before_append;
 use crate::prelude::*;
 use crate::series::IsSorted;
 
 fn extend_immutable(immutable: &dyn Array, chunks: &mut Vec<ArrayRef>, other_chunks: &[ArrayRef]) {
     let out = if chunks.len() == 1 {
         concatenate(&[immutable, &*other_chunks[0]]).unwrap()
     } else {
@@ -32,14 +33,15 @@
     /// Prefer `extend` over `append` when you want to do a query after a single append. For instance during
     /// online operations where you add `n` rows and rerun a query.
     ///
     /// Prefer `append` over `extend` when you want to append many times before doing a query. For instance
     /// when you read in multiple files and when to store them in a single `DataFrame`.
     /// In the latter case finish the sequence of `append` operations with a [`rechunk`](Self::rechunk).
     pub fn extend(&mut self, other: &Self) {
+        update_sorted_flag_before_append(self, other);
         // all to a single chunk
         if self.chunks.len() > 1 {
             self.append(other);
             *self = self.rechunk();
             return;
         }
         // Depending on the state of the underlying arrow array we
@@ -78,21 +80,21 @@
                     }
                     let arr: PrimitiveArray<T::Native> = mutable.into();
                     self.chunks.push(Box::new(arr) as ArrayRef)
                 }
             }
         }
         self.compute_len();
-        self.set_sorted_flag(IsSorted::Not);
     }
 }
 
 #[doc(hidden)]
 impl Utf8Chunked {
     pub fn extend(&mut self, other: &Self) {
+        update_sorted_flag_before_append(self, other);
         if self.chunks.len() > 1 {
             self.append(other);
             *self = self.rechunk();
             return;
         }
         let arr = self.downcast_iter().next().unwrap();
 
@@ -123,14 +125,15 @@
         self.set_sorted_flag(IsSorted::Not);
     }
 }
 
 #[doc(hidden)]
 impl BinaryChunked {
     pub fn extend(&mut self, other: &Self) {
+        update_sorted_flag_before_append(self, other);
         if self.chunks.len() > 1 {
             self.append(other);
             *self = self.rechunk();
             return;
         }
         let arr = self.downcast_iter().next().unwrap();
 
@@ -160,14 +163,15 @@
         self.compute_len();
     }
 }
 
 #[doc(hidden)]
 impl BooleanChunked {
     pub fn extend(&mut self, other: &Self) {
+        update_sorted_flag_before_append(self, other);
         // make sure that we are a single chunk already
         if self.chunks.len() > 1 {
             self.append(other);
             *self = self.rechunk();
             return;
         }
         let arr = self.downcast_iter().next().unwrap();
```

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/ops/fill_null.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/ops/fill_null.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/ops/filter.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/ops/filter.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/ops/full.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/ops/full.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/ops/is_in.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/ops/is_in.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/ops/min_max_binary.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/ops/min_max_binary.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/ops/mod.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/ops/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/ops/nulls.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/ops/nulls.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/ops/peaks.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/ops/peaks.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/ops/repeat_by.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/ops/repeat_by.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/ops/reverse.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/ops/reverse.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/ops/rolling_window.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/ops/rolling_window.rs`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 
     use arrow::array::{Array, PrimitiveArray};
     use arrow::bitmap::MutableBitmap;
     use num_traits::pow::Pow;
     use num_traits::{Float, Zero};
     use polars_arrow::bit_util::unset_bit_raw;
     use polars_arrow::data_types::IsFloat;
-    use polars_arrow::trusted_len::PushUnchecked;
+    use polars_arrow::trusted_len::TrustedLenPush;
 
     use crate::prelude::*;
 
     /// utility
     fn check_input(window_size: usize, min_periods: usize) -> PolarsResult<()> {
         polars_ensure!(
             min_periods <= window_size,
```

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/ops/set.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/ops/set.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/ops/shift.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/ops/shift.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/ops/sort/arg_sort.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/ops/sort/arg_sort.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/ops/sort/arg_sort_multiple.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/ops/sort/arg_sort_multiple.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/ops/sort/categorical.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/ops/sort/categorical.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/ops/sort/mod.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/ops/sort/mod.rs`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 pub(crate) use arg_sort_multiple::argsort_multiple_row_fmt;
 use arrow::bitmap::MutableBitmap;
 use arrow::buffer::Buffer;
 use num_traits::Float;
 use polars_arrow::array::default_arrays::FromDataUtf8;
 use polars_arrow::kernels::rolling::compare_fn_nan_max;
 use polars_arrow::prelude::{FromData, ValueSize};
-use polars_arrow::trusted_len::PushUnchecked;
+use polars_arrow::trusted_len::TrustedLenPush;
 use rayon::prelude::*;
 pub use slice::*;
 
 use crate::prelude::compare_inner::PartialOrdInner;
 #[cfg(feature = "dtype-struct")]
 use crate::prelude::sort::arg_sort_multiple::_get_rows_encoded_ca;
 use crate::prelude::sort::arg_sort_multiple::{arg_sort_multiple_impl, args_validate};
```

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/ops/take/mod.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/ops/take/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/ops/take/take_chunked.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/ops/take/take_chunked.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/ops/take/take_random.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/ops/take/take_random.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/ops/take/take_single.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/ops/take/take_single.rs`

 * *Files 13% similar despite different names*

```diff
@@ -91,14 +91,32 @@
 
     #[inline]
     fn get(&self, index: usize) -> Option<Self::Item> {
         // Safety:
         // Out of bounds is checked and downcast is of correct type
         unsafe { impl_take_random_get!(self, index, BooleanArray) }
     }
+    #[inline]
+    unsafe fn get_unchecked(&self, index: usize) -> Option<Self::Item> {
+        impl_take_random_get_unchecked!(self, index, BooleanArray)
+    }
+}
+
+impl<'a> TakeRandom for &'a BooleanChunked {
+    type Item = bool;
+
+    #[inline]
+    fn get(&self, index: usize) -> Option<Self::Item> {
+        (*self).get(index)
+    }
+
+    #[inline]
+    unsafe fn get_unchecked(&self, index: usize) -> Option<Self::Item> {
+        (*self).get_unchecked(index)
+    }
 }
 
 impl<'a> TakeRandom for &'a Utf8Chunked {
     type Item = &'a str;
 
     #[inline]
     fn get(&self, index: usize) -> Option<Self::Item> {
```

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/ops/take/traits.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/ops/take/traits.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/ops/unique/mod.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/ops/unique/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/ops/unique/rank.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/ops/unique/rank.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/ops/zip.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/ops/zip.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/random.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/random.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/temporal/conversion.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/temporal/conversion.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/temporal/date.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/temporal/date.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/temporal/datetime.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/temporal/datetime.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/temporal/duration.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/temporal/duration.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/temporal/mod.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/temporal/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/temporal/time.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/temporal/time.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/to_vec.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/to_vec.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/trusted_len.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/trusted_len.rs`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 use std::borrow::Borrow;
 
 use arrow::bitmap::MutableBitmap;
 use polars_arrow::bit_util::{set_bit_raw, unset_bit_raw};
-use polars_arrow::trusted_len::{FromIteratorReversed, PushUnchecked};
+use polars_arrow::trusted_len::{FromIteratorReversed, TrustedLenPush};
 
 use crate::chunked_array::upstream_traits::PolarsAsRef;
 use crate::prelude::*;
 use crate::utils::{CustomIterTools, FromTrustedLenIterator, NoNull};
 
 impl<T> FromTrustedLenIterator<Option<T::Native>> for ChunkedArray<T>
 where
```

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/chunked_array/upstream_traits.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/chunked_array/upstream_traits.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/cloud.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/cloud.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/config.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/config.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/datatypes/_serde.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/datatypes/_serde.rs`

 * *Files 21% similar despite different names*

```diff
@@ -55,14 +55,18 @@
     Time,
     List(Box<SerializableDataType>),
     Null,
     #[cfg(feature = "dtype-struct")]
     Struct(Vec<Field>),
     // some logical types we cannot know statically, e.g. Datetime
     Unknown,
+    #[cfg(feature = "dtype-categorical")]
+    Categorical,
+    #[cfg(feature = "object")]
+    Object(String),
 }
 
 impl From<&DataType> for SerializableDataType {
     fn from(dt: &DataType) -> Self {
         use DataType::*;
         match dt {
             Boolean => Self::Boolean,
@@ -83,15 +87,19 @@
             Duration(tu) => Self::Duration(*tu),
             Time => Self::Time,
             List(dt) => Self::List(Box::new(dt.as_ref().into())),
             Null => Self::Null,
             Unknown => Self::Unknown,
             #[cfg(feature = "dtype-struct")]
             Struct(flds) => Self::Struct(flds.clone()),
-            _ => todo!(),
+            #[cfg(feature = "dtype-categorical")]
+            Categorical(_) => Self::Categorical,
+            #[cfg(feature = "object")]
+            Object(name) => Self::Object(name.to_string()),
+            dt => panic!("{dt:?} not supported"),
         }
     }
 }
 impl From<SerializableDataType> for DataType {
     fn from(dt: SerializableDataType) -> Self {
         use SerializableDataType::*;
         match dt {
@@ -113,10 +121,14 @@
             Duration(tu) => Self::Duration(tu),
             Time => Self::Time,
             List(dt) => Self::List(Box::new((*dt).into())),
             Null => Self::Null,
             Unknown => Self::Unknown,
             #[cfg(feature = "dtype-struct")]
             Struct(flds) => Self::Struct(flds),
+            #[cfg(feature = "dtype-categorical")]
+            Categorical => Self::Categorical(None),
+            #[cfg(feature = "object")]
+            Object(_) => Self::Object("unknown"),
         }
     }
 }
```

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/datatypes/aliases.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/datatypes/aliases.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/datatypes/any_value.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/datatypes/any_value.rs`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 use arrow::temporal_conversions::{
     timestamp_ms_to_datetime, timestamp_ns_to_datetime, timestamp_us_to_datetime,
 };
 use arrow::types::PrimitiveType;
 #[cfg(feature = "dtype-struct")]
-use polars_arrow::trusted_len::PushUnchecked;
+use polars_arrow::trusted_len::TrustedLenPush;
 #[cfg(feature = "dtype-struct")]
 use polars_utils::slice::GetSaferUnchecked;
 #[cfg(feature = "dtype-categorical")]
 use polars_utils::sync::SyncPtr;
 use polars_utils::unwrap::UnwrapUncheckedRelease;
 
 use super::*;
```

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/datatypes/dtype.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/datatypes/dtype.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/datatypes/field.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/datatypes/field.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/datatypes/mod.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/datatypes/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/datatypes/time_unit.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/datatypes/time_unit.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/doc/changelog/v0_10_0_11.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/doc/changelog/v0_10_0_11.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/doc/changelog/v0_7.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/doc/changelog/v0_7.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/doc/changelog/v0_8.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/doc/changelog/v0_8.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/doc/changelog/v0_9.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/doc/changelog/v0_9.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/fmt.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/fmt.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/frame/arithmetic.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/frame/arithmetic.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/frame/asof_join/asof.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/frame/asof_join/asof.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/frame/asof_join/groups.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/frame/asof_join/groups.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/frame/asof_join/mod.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/frame/asof_join/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/frame/chunks.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/frame/chunks.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/frame/cross_join.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/frame/cross_join.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/frame/explode.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/frame/explode.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/frame/from.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/frame/from.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/frame/groupby/aggregations/agg_list.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/frame/groupby/aggregations/agg_list.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/frame/groupby/aggregations/boolean.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/frame/groupby/aggregations/boolean.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/frame/groupby/aggregations/dispatch.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/frame/groupby/aggregations/dispatch.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/frame/groupby/aggregations/mod.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/frame/groupby/aggregations/mod.rs`

 * *Files 1% similar despite different names*

```diff
@@ -4,25 +4,25 @@
 mod utf8;
 
 pub use agg_list::*;
 use arrow::bitmap::{Bitmap, MutableBitmap};
 use arrow::types::simd::Simd;
 use arrow::types::NativeType;
 use num_traits::pow::Pow;
-use num_traits::{Bounded, Num, NumCast, ToPrimitive, Zero};
+use num_traits::{Bounded, Float, Num, NumCast, ToPrimitive, Zero};
 use polars_arrow::data_types::IsFloat;
 use polars_arrow::kernels::rolling;
 use polars_arrow::kernels::rolling::no_nulls::{
-    MaxWindow, MeanWindow, MinWindow, RollingAggWindowNoNulls, StdWindow, SumWindow, VarWindow,
+    MaxWindow, MeanWindow, MinWindow, RollingAggWindowNoNulls, SumWindow, VarWindow,
 };
 use polars_arrow::kernels::rolling::nulls::RollingAggWindowNulls;
 use polars_arrow::kernels::rolling::{DynArgs, RollingVarParams};
 use polars_arrow::kernels::take_agg::*;
 use polars_arrow::prelude::QuantileInterpolOptions;
-use polars_arrow::trusted_len::PushUnchecked;
+use polars_arrow::trusted_len::TrustedLenPush;
 use rayon::prelude::*;
 
 #[cfg(feature = "object")]
 use crate::chunked_array::object::extension::create_extension;
 use crate::frame::groupby::GroupsIdx;
 #[cfg(feature = "object")]
 use crate::frame::groupby::GroupsIndicator;
@@ -779,29 +779,32 @@
             }
             GroupsProxy::Slice { groups, .. } => {
                 if _use_rolling_kernels(groups, self.chunks()) {
                     let arr = self.downcast_iter().next().unwrap();
                     let values = arr.values().as_slice();
                     let offset_iter = groups.iter().map(|[first, len]| (*first, *len));
                     let arr = match arr.validity() {
-                        None => _rolling_apply_agg_window_no_nulls::<StdWindow<_>, _, _>(
+                        None => _rolling_apply_agg_window_no_nulls::<VarWindow<_>, _, _>(
                             values,
                             offset_iter,
                             Some(Arc::new(RollingVarParams { ddof })),
                         ),
                         Some(validity) => {
-                            _rolling_apply_agg_window_nulls::<rolling::nulls::StdWindow<_>, _, _>(
+                            _rolling_apply_agg_window_nulls::<rolling::nulls::VarWindow<_>, _, _>(
                                 values,
                                 validity,
                                 offset_iter,
                                 Some(Arc::new(RollingVarParams { ddof })),
                             )
                         }
                     };
-                    ChunkedArray::<T>::from_chunks("", vec![arr]).into_series()
+
+                    let mut ca = ChunkedArray::<T>::from_chunks("", vec![arr]);
+                    ca.apply_mut(|v| v.powf(NumCast::from(0.5).unwrap()));
+                    ca.into_series()
                 } else {
                     _agg_helper_slice::<T, _>(groups, |[first, len]| {
                         debug_assert!(len <= self.len() as IdxSize);
                         match len {
                             0 => None,
                             1 => NumCast::from(0),
                             _ => {
```

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/frame/groupby/aggregations/utf8.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/frame/groupby/aggregations/utf8.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/frame/groupby/hashing.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/frame/groupby/hashing.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/frame/groupby/into_groups.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/frame/groupby/into_groups.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/frame/groupby/mod.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/frame/groupby/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/frame/groupby/perfect.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/frame/groupby/perfect.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/frame/groupby/proxy.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/frame/groupby/proxy.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/frame/hash_join/args.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/frame/hash_join/args.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/frame/hash_join/mod.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/frame/hash_join/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/frame/hash_join/multiple_keys.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/frame/hash_join/multiple_keys.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/frame/hash_join/single_keys.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/frame/hash_join/single_keys.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/frame/hash_join/single_keys_dispatch.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/frame/hash_join/single_keys_dispatch.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/frame/hash_join/single_keys_inner.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/frame/hash_join/single_keys_inner.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/frame/hash_join/single_keys_left.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/frame/hash_join/single_keys_left.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/frame/hash_join/single_keys_outer.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/frame/hash_join/single_keys_outer.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/frame/hash_join/single_keys_semi_anti.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/frame/hash_join/single_keys_semi_anti.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/frame/hash_join/sort_merge.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/frame/hash_join/sort_merge.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/frame/hash_join/zip_outer.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/frame/hash_join/zip_outer.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/frame/mod.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/frame/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/frame/row/av_buffer.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/frame/row/av_buffer.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/frame/row/dataframe.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/frame/row/dataframe.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/frame/row/mod.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/frame/row/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/frame/row/transpose.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/frame/row/transpose.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/frame/top_k.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/frame/top_k.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/frame/upstream_traits.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/frame/upstream_traits.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/functions.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/functions.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/hashing/fx.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/hashing/fx.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/hashing/identity.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/hashing/identity.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/hashing/partition.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/hashing/partition.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/hashing/vector_hasher.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/hashing/vector_hasher.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/lib.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/lib.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/named_from.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/named_from.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/prelude.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/prelude.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/schema.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/schema.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/serde/chunked_array.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/serde/chunked_array.rs`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 use std::cell::RefCell;
 
 use serde::ser::SerializeMap;
 use serde::{Serialize, Serializer};
 
-use super::DeDataType;
 use crate::prelude::*;
 
 pub struct IterSer<I>
 where
     I: IntoIterator,
     <I as IntoIterator>::Item: Serialize,
 {
@@ -52,16 +51,15 @@
 where
     T: PolarsNumericType,
     T::Native: Serialize,
     S: Serializer,
 {
     let mut state = serializer.serialize_map(Some(3))?;
     state.serialize_entry("name", name)?;
-    let dtype: DeDataType = dtype.into();
-    state.serialize_entry("datatype", &dtype)?;
+    state.serialize_entry("datatype", dtype)?;
     state.serialize_entry("values", &IterSer::new(ca.into_iter()))?;
     state.end()
 }
 
 impl<T> Serialize for ChunkedArray<T>
 where
     T: PolarsNumericType,
@@ -103,16 +101,15 @@
                 serializer: S,
             ) -> std::result::Result<<S as Serializer>::Ok, <S as Serializer>::Error>
             where
                 S: Serializer,
             {
                 let mut state = serializer.serialize_map(Some(3))?;
                 state.serialize_entry("name", self.name())?;
-                let dtype: DeDataType = self.dtype().into();
-                state.serialize_entry("datatype", &dtype)?;
+                state.serialize_entry("datatype", self.dtype())?;
                 state.serialize_entry("values", &IterSer::new(self.into_iter()))?;
                 state.end()
             }
         }
     };
 }
 
@@ -129,16 +126,15 @@
     ) -> std::result::Result<<S as Serializer>::Ok, <S as Serializer>::Error>
     where
         S: Serializer,
     {
         {
             let mut state = serializer.serialize_map(Some(3))?;
             state.serialize_entry("name", self.name())?;
-            let dtype: DeDataType = self.dtype().into();
-            state.serialize_entry("datatype", &dtype)?;
+            state.serialize_entry("datatype", self.dtype())?;
             state.serialize_entry("values", &IterSer::new(self.iter_str()))?;
             state.end()
         }
     }
 }
 
 #[cfg(feature = "dtype-struct")]
@@ -149,14 +145,13 @@
     ) -> std::result::Result<<S as Serializer>::Ok, <S as Serializer>::Error>
     where
         S: Serializer,
     {
         {
             let mut state = serializer.serialize_map(Some(3))?;
             state.serialize_entry("name", self.name())?;
-            let dtype: DeDataType = self.dtype().into();
-            state.serialize_entry("datatype", &dtype)?;
+            state.serialize_entry("datatype", self.dtype())?;
             state.serialize_entry("values", self.fields())?;
             state.end()
         }
     }
 }
```

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/serde/df.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/serde/df.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/serde/mod.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/serde/mod.rs`

 * *Files 23% similar despite different names*

```diff
@@ -1,75 +1,15 @@
-use serde::{Deserialize, Serialize};
-
-use crate::prelude::*;
-
 pub mod chunked_array;
 mod df;
 pub mod series;
 
-/// Intermediate enum. Needed because [crate::datatypes::DataType] has
-/// a &static str and thus requires Deserialize<&static>
-#[derive(Serialize, Deserialize, Debug)]
-enum DeDataType<'a> {
-    Boolean,
-    UInt8,
-    UInt16,
-    UInt32,
-    UInt64,
-    Int8,
-    Int16,
-    Int32,
-    Int64,
-    Float32,
-    Float64,
-    Utf8,
-    Binary,
-    Date,
-    Datetime(TimeUnit, Option<TimeZone>),
-    Duration(TimeUnit),
-    Time,
-    List,
-    Object(&'a str),
-    Null,
-    Categorical,
-    Struct,
-}
-
-impl From<&DataType> for DeDataType<'_> {
-    fn from(dt: &DataType) -> Self {
-        match dt {
-            DataType::Int32 => DeDataType::Int32,
-            DataType::UInt32 => DeDataType::UInt32,
-            DataType::Int64 => DeDataType::Int64,
-            DataType::UInt64 => DeDataType::UInt64,
-            DataType::Date => DeDataType::Date,
-            DataType::Datetime(tu, tz) => DeDataType::Datetime(*tu, tz.clone()),
-            DataType::Duration(tu) => DeDataType::Duration(*tu),
-            DataType::Time => DeDataType::Time,
-            DataType::Float32 => DeDataType::Float32,
-            DataType::Float64 => DeDataType::Float64,
-            DataType::Utf8 => DeDataType::Utf8,
-            DataType::Boolean => DeDataType::Boolean,
-            DataType::Null => DeDataType::Null,
-            DataType::List(_) => DeDataType::List,
-            DataType::Binary => DeDataType::Binary,
-            #[cfg(feature = "object")]
-            DataType::Object(s) => DeDataType::Object(s),
-            #[cfg(feature = "dtype-struct")]
-            DataType::Struct(_) => DeDataType::Struct,
-            #[cfg(feature = "dtype-categorical")]
-            DataType::Categorical(_) => DeDataType::Categorical,
-            _ => unimplemented!(),
-        }
-    }
-}
-
 #[cfg(test)]
 mod test {
     use super::*;
+    use crate::prelude::*;
 
     #[test]
     fn test_serde() -> PolarsResult<()> {
         let ca = UInt32Chunked::new("foo", &[Some(1), None, Some(2)]);
 
         let json = serde_json::to_string(&ca).unwrap();
```

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/serde/series.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/serde/series.rs`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 use std::borrow::Cow;
 use std::fmt::Formatter;
 
 use serde::de::{MapAccess, Visitor};
 use serde::{de, Deserialize, Deserializer, Serialize, Serializer};
 
 use crate::prelude::*;
-use crate::serde::DeDataType;
 
 impl Serialize for Series {
     fn serialize<S>(
         &self,
         serializer: S,
     ) -> std::result::Result<<S as Serializer>::Ok, <S as Serializer>::Error>
     where
@@ -126,97 +125,107 @@
                     return Err(de::Error::missing_field("values"));
                 }
                 let name = name.ok_or_else(|| de::Error::missing_field("name"))?;
                 let dtype = dtype.ok_or_else(|| de::Error::missing_field("datatype"))?;
 
                 match dtype {
                     #[cfg(feature = "dtype-i8")]
-                    DeDataType::Int8 => {
+                    DataType::Int8 => {
                         let values: Vec<Option<i8>> = map.next_value()?;
                         Ok(Series::new(&name, values))
                     }
                     #[cfg(feature = "dtype-u8")]
-                    DeDataType::UInt8 => {
+                    DataType::UInt8 => {
                         let values: Vec<Option<u8>> = map.next_value()?;
                         Ok(Series::new(&name, values))
                     }
-                    DeDataType::Int32 => {
+                    #[cfg(feature = "dtype-i16")]
+                    DataType::Int16 => {
+                        let values: Vec<Option<i16>> = map.next_value()?;
+                        Ok(Series::new(&name, values))
+                    }
+                    #[cfg(feature = "dtype-u16")]
+                    DataType::UInt16 => {
+                        let values: Vec<Option<u16>> = map.next_value()?;
+                        Ok(Series::new(&name, values))
+                    }
+                    DataType::Int32 => {
                         let values: Vec<Option<i32>> = map.next_value()?;
                         Ok(Series::new(&name, values))
                     }
-                    DeDataType::UInt32 => {
+                    DataType::UInt32 => {
                         let values: Vec<Option<u32>> = map.next_value()?;
                         Ok(Series::new(&name, values))
                     }
-                    DeDataType::Int64 => {
+                    DataType::Int64 => {
                         let values: Vec<Option<i64>> = map.next_value()?;
                         Ok(Series::new(&name, values))
                     }
-                    DeDataType::UInt64 => {
+                    DataType::UInt64 => {
                         let values: Vec<Option<u64>> = map.next_value()?;
                         Ok(Series::new(&name, values))
                     }
                     #[cfg(feature = "dtype-date")]
-                    DeDataType::Date => {
+                    DataType::Date => {
                         let values: Vec<Option<i32>> = map.next_value()?;
                         Ok(Series::new(&name, values).cast(&DataType::Date).unwrap())
                     }
                     #[cfg(feature = "dtype-datetime")]
-                    DeDataType::Datetime(tu, tz) => {
+                    DataType::Datetime(tu, tz) => {
                         let values: Vec<Option<i64>> = map.next_value()?;
                         Ok(Series::new(&name, values)
                             .cast(&DataType::Datetime(tu, tz))
                             .unwrap())
                     }
                     #[cfg(feature = "dtype-duration")]
-                    DeDataType::Duration(tu) => {
+                    DataType::Duration(tu) => {
                         let values: Vec<Option<i64>> = map.next_value()?;
                         Ok(Series::new(&name, values)
                             .cast(&DataType::Duration(tu))
                             .unwrap())
                     }
                     #[cfg(feature = "dtype-time")]
-                    DeDataType::Time => {
+                    DataType::Time => {
                         let values: Vec<Option<i64>> = map.next_value()?;
                         Ok(Series::new(&name, values).cast(&DataType::Time).unwrap())
                     }
-                    DeDataType::Boolean => {
+                    DataType::Boolean => {
                         let values: Vec<Option<bool>> = map.next_value()?;
                         Ok(Series::new(&name, values))
                     }
-                    DeDataType::Float32 => {
+                    DataType::Float32 => {
                         let values: Vec<Option<f32>> = map.next_value()?;
                         Ok(Series::new(&name, values))
                     }
-                    DeDataType::Float64 => {
+                    DataType::Float64 => {
                         let values: Vec<Option<f64>> = map.next_value()?;
                         Ok(Series::new(&name, values))
                     }
-                    DeDataType::Utf8 => {
+                    DataType::Utf8 => {
                         let values: Vec<Option<Cow<str>>> = map.next_value()?;
                         Ok(Series::new(&name, values))
                     }
-                    DeDataType::List => {
+                    DataType::List(_) => {
                         let values: Vec<Option<Series>> = map.next_value()?;
                         Ok(Series::new(&name, values))
                     }
-                    DeDataType::Binary => {
+                    DataType::Binary => {
                         let values: Vec<Option<Cow<[u8]>>> = map.next_value()?;
                         Ok(Series::new(&name, values))
                     }
                     #[cfg(feature = "dtype-struct")]
-                    DeDataType::Struct => {
+                    DataType::Struct(_) => {
                         let values: Vec<Series> = map.next_value()?;
                         let ca = StructChunked::new(&name, &values).unwrap();
                         let mut s = ca.into_series();
                         s.rename(&name);
                         Ok(s)
                     }
                     #[cfg(feature = "dtype-categorical")]
-                    DeDataType::Categorical => {
+                    DataType::Categorical(_) => {
                         let values: Vec<Option<Cow<str>>> = map.next_value()?;
                         Ok(Series::new(&name, values)
                             .cast(&DataType::Categorical(None))
                             .unwrap())
                     }
                     dt => {
                         panic!("{dt:?} dtype deserialization not yet implemented")
```

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/series/any_value.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/series/any_value.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/series/arithmetic/borrowed.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/series/arithmetic/borrowed.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/series/arithmetic/owned.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/series/arithmetic/owned.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/series/comparison.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/series/comparison.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/series/from.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/series/from.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/series/implementations/array.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/series/implementations/array.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/series/implementations/binary.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/series/implementations/binary.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/series/implementations/boolean.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/series/implementations/boolean.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/series/implementations/categorical.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/series/implementations/categorical.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/series/implementations/dates_time.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/series/implementations/dates_time.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/series/implementations/datetime.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/series/implementations/datetime.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/series/implementations/decimal.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/series/implementations/decimal.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/series/implementations/duration.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/series/implementations/duration.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/series/implementations/floats.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/series/implementations/floats.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/series/implementations/list.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/series/implementations/list.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/series/implementations/mod.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/series/implementations/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/series/implementations/null.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/series/implementations/null.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/series/implementations/object.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/series/implementations/object.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/series/implementations/struct_.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/series/implementations/struct_.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/series/implementations/utf8.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/series/implementations/utf8.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/series/into.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/series/into.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/series/iterator.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/series/iterator.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/series/mod.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/series/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/series/ops/diff.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/series/ops/diff.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/series/ops/downcast.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/series/ops/downcast.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/series/ops/ewm.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/series/ops/ewm.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/series/ops/mod.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/series/ops/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/series/ops/moment.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/series/ops/moment.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/series/ops/null.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/series/ops/null.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/series/ops/pct_change.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/series/ops/pct_change.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/series/ops/round.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/series/ops/round.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/series/ops/to_list.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/series/ops/to_list.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/series/ops/unique.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/series/ops/unique.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/series/series_trait.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/series/series_trait.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/series/unstable.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/series/unstable.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/testing.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/testing.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/utils/flatten.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/utils/flatten.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/utils/mod.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/utils/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/utils/series.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/utils/series.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-core/src/utils/supertype.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-core/src/utils/supertype.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-algo/Cargo.toml` & `polars_u64_idx-0.18.4/local_dependencies/polars-algo/Cargo.toml`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-algo/LICENSE` & `polars_u64_idx-0.18.4/local_dependencies/polars-row/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-algo/src/algo.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-algo/src/algo.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-json/Cargo.toml` & `polars_u64_idx-0.18.4/local_dependencies/polars-json/Cargo.toml`

 * *Files 8% similar despite different names*

```diff
@@ -19,19 +19,19 @@
 polars-arrow = { version = "0.30.0", path = "../polars-arrow", default-features = false }
 polars-error = { version = "0.30.0", path = "../polars-error" }
 polars-utils = { version = "0.30.0", path = "../polars-utils" }
 simd-json = { version = "0.10", features = ["allow-non-simd", "known-key"] }
 
 [dependencies.arrow]
 package = "arrow2"
-git = "https://github.com/jorgecarleitao/arrow2"
-# git = "https://github.com/ritchie46/arrow2"
-rev = "2d2e7053f9a50810bfe9cecff25ab39089aef98e"
+# git = "https://github.com/jorgecarleitao/arrow2"
+git = "https://github.com/ritchie46/arrow2"
+# rev = "2d2e7053f9a50810bfe9cecff25ab39089aef98e"
 # path = "../arrow2"
-# branch = "polars_2023-05-25"
+branch = "polars_2023-06-23"
 version = "0.17"
 default-features = false
 features = [
   "compute_aggregate",
   "compute_arithmetics",
   "compute_boolean",
   "compute_boolean_kleene",
```

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-json/LICENSE` & `polars_u64_idx-0.18.4/local_dependencies/polars-algo/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-json/src/json/deserialize.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-json/src/json/deserialize.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-json/src/json/infer_schema.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-json/src/json/infer_schema.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-json/src/ndjson/deserialize.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-json/src/ndjson/deserialize.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-json/src/ndjson/file.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-json/src/ndjson/file.rs`

 * *Files 5% similar despite different names*

```diff
@@ -140,9 +140,10 @@
         let data_type = crate::json::infer(&v)?;
         if data_type != DataType::Null {
             data_types.insert(data_type);
         }
     }
 
     let v: Vec<&DataType> = data_types.iter().collect();
-    Ok(crate::json::infer_schema::coerce_data_type(&v))
+    dbg!(&v);
+    dbg!(Ok(crate::json::infer_schema::coerce_data_type(&v)))
 }
```

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars/Cargo.toml` & `polars_u64_idx-0.18.4/local_dependencies/polars/Cargo.toml`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 resolver = "2"
 
 [features]
 sql = ["polars-sql"]
 rows = ["polars-core/rows"]
 simd = ["polars-core/simd", "polars-io/simd", "polars-ops/simd"]
 avx512 = ["polars-core/avx512"]
-nightly = ["polars-core/nightly", "polars-ops/nightly", "simd"]
+nightly = ["polars-core/nightly", "polars-ops/nightly", "simd", "polars-lazy/nightly"]
 docs = ["polars-core/docs"]
 temporal = ["polars-core/temporal", "polars-lazy/temporal", "polars-io/temporal", "polars-time"]
 random = ["polars-core/random", "polars-lazy/random"]
 default = [
   "docs",
   "zip_with",
   "csv",
@@ -97,15 +97,20 @@
 concat_str = ["polars-core/concat_str", "polars-lazy/concat_str"]
 row_hash = ["polars-core/row_hash", "polars-lazy/row_hash"]
 reinterpret = ["polars-core/reinterpret"]
 decompress = ["polars-io/decompress"]
 decompress-fast = ["polars-io/decompress-fast"]
 mode = ["polars-core/mode", "polars-lazy/mode"]
 take_opt_iter = ["polars-core/take_opt_iter"]
-extract_jsonpath = ["polars-core/strings", "polars-ops/extract_jsonpath", "polars-ops/strings"]
+extract_jsonpath = [
+  "polars-core/strings",
+  "polars-ops/extract_jsonpath",
+  "polars-ops/strings",
+  "polars-lazy/extract_jsonpath",
+]
 string_encoding = ["polars-ops/string_encoding", "polars-core/strings"]
 binary_encoding = ["polars-ops/binary_encoding"]
 groupby_list = ["polars-core/groupby_list"]
 lazy_regex = ["polars-lazy/regex"]
 cum_agg = ["polars-core/cum_agg", "polars-core/cum_agg"]
 rolling_window = ["polars-core/rolling_window", "polars-lazy/rolling_window", "polars-time/rolling_window"]
 interpolate = ["polars-ops/interpolate", "polars-lazy/interpolate"]
```

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars/LICENSE` & `polars_u64_idx-0.18.4/local_dependencies/polars/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars/Makefile` & `polars_u64_idx-0.18.4/local_dependencies/polars/Makefile`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars/src/docs/eager.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars/src/docs/eager.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars/src/docs/lazy.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars/src/docs/lazy.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars/src/docs/performance.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars/src/docs/performance.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars/src/lib.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars/src/lib.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars/tests/it/core/date_like.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars/tests/it/core/date_like.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars/tests/it/core/groupby.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars/tests/it/core/groupby.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars/tests/it/core/joins.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars/tests/it/core/joins.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars/tests/it/core/list.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars/tests/it/core/list.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars/tests/it/core/pivot.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars/tests/it/core/pivot.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars/tests/it/core/random.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars/tests/it/core/random.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars/tests/it/core/rolling_window.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars/tests/it/core/rolling_window.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars/tests/it/core/series.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars/tests/it/core/series.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars/tests/it/io/csv.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars/tests/it/io/csv.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars/tests/it/io/ipc_stream.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars/tests/it/io/ipc_stream.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars/tests/it/io/json.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars/tests/it/io/json.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars/tests/it/io/parquet.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars/tests/it/io/parquet.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars/tests/it/joins.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars/tests/it/joins.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars/tests/it/lazy/aggregation.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars/tests/it/lazy/aggregation.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars/tests/it/lazy/cse.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars/tests/it/lazy/cse.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars/tests/it/lazy/expressions/apply.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars/tests/it/lazy/expressions/apply.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars/tests/it/lazy/expressions/arity.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars/tests/it/lazy/expressions/arity.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars/tests/it/lazy/expressions/expand.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars/tests/it/lazy/expressions/expand.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars/tests/it/lazy/expressions/filter.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars/tests/it/lazy/expressions/filter.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars/tests/it/lazy/expressions/slice.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars/tests/it/lazy/expressions/slice.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars/tests/it/lazy/expressions/window.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars/tests/it/lazy/expressions/window.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars/tests/it/lazy/folds.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars/tests/it/lazy/folds.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars/tests/it/lazy/functions.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars/tests/it/lazy/functions.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars/tests/it/lazy/groupby.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars/tests/it/lazy/groupby.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars/tests/it/lazy/groupby_dynamic.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars/tests/it/lazy/groupby_dynamic.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars/tests/it/lazy/mod.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars/tests/it/lazy/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars/tests/it/lazy/predicate_queries.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars/tests/it/lazy/predicate_queries.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars/tests/it/lazy/projection_queries.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars/tests/it/lazy/projection_queries.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars/tests/it/lazy/queries.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars/tests/it/lazy/queries.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars/tests/it/schema.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars/tests/it/schema.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-ops/Cargo.toml` & `polars_u64_idx-0.18.4/local_dependencies/polars-ops/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -76,19 +76,19 @@
 chunked_ids = ["polars-core/chunked_ids"]
 asof_join = ["polars-core/asof_join"]
 semi_anti_join = ["polars-core/semi_anti_join"]
 list_take = []
 
 [dependencies.arrow]
 package = "arrow2"
-git = "https://github.com/jorgecarleitao/arrow2"
-# git = "https://github.com/ritchie46/arrow2"
-rev = "2d2e7053f9a50810bfe9cecff25ab39089aef98e"
+# git = "https://github.com/jorgecarleitao/arrow2"
+git = "https://github.com/ritchie46/arrow2"
+# rev = "2d2e7053f9a50810bfe9cecff25ab39089aef98e"
 # path = "../arrow2"
-# branch = "polars_2023-05-25"
+branch = "polars_2023-06-23"
 version = "0.17"
 default-features = false
 features = [
   "compute_aggregate",
   "compute_arithmetics",
   "compute_boolean",
   "compute_boolean_kleene",
```

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-ops/LICENSE` & `polars_u64_idx-0.18.4/local_dependencies/polars-arrow/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-ops/src/chunked_array/array/min_max.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-ops/src/chunked_array/array/min_max.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-ops/src/chunked_array/array/namespace.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-ops/src/chunked_array/array/namespace.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-ops/src/chunked_array/array/sum_mean.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-ops/src/chunked_array/array/sum_mean.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-ops/src/chunked_array/binary/namespace.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-ops/src/chunked_array/binary/namespace.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-ops/src/chunked_array/interpolate.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-ops/src/chunked_array/interpolate.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-ops/src/chunked_array/list/count.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-ops/src/chunked_array/list/count.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-ops/src/chunked_array/list/hash.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-ops/src/chunked_array/list/hash.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-ops/src/chunked_array/list/min_max.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-ops/src/chunked_array/list/min_max.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-ops/src/chunked_array/list/namespace.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-ops/src/chunked_array/list/namespace.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-ops/src/chunked_array/list/sum_mean.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-ops/src/chunked_array/list/sum_mean.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-ops/src/chunked_array/list/to_struct.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-ops/src/chunked_array/list/to_struct.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-ops/src/chunked_array/mod.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-ops/src/chunked_array/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-ops/src/chunked_array/nan_propagating_aggregate.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-ops/src/chunked_array/nan_propagating_aggregate.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-ops/src/chunked_array/set.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-ops/src/chunked_array/set.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-ops/src/chunked_array/strings/case.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-ops/src/chunked_array/strings/case.rs`

 * *Files 14% similar despite different names*

```diff
@@ -68,72 +68,77 @@
         // lifetime is bound to 'a
         let slice = unsafe { std::str::from_utf8_unchecked(slice) };
         unsafe { std::mem::transmute::<&str, &'a str>(slice) }
     };
     ca.apply_mut(f)
 }
 
-// inlined from std
 #[cfg(feature = "nightly")]
-pub(super) fn to_lowercase<'a>(ca: &'a Utf8Chunked) -> Utf8Chunked {
-    // amortize allocation
-    let mut buf = Vec::new();
-    let f = |s: &'a str| {
-        convert_while_ascii(s.as_bytes(), u8::to_ascii_lowercase, &mut buf);
+fn to_lowercase_helper(s: &str, buf: &mut Vec<u8>) {
+    convert_while_ascii(s.as_bytes(), u8::to_ascii_lowercase, buf);
 
-        // Safety: we know this is a valid char boundary since
-        // out.len() is only progressed if ascii bytes are found
-        let rest = unsafe { s.get_unchecked(buf.len()..) };
-
-        // Safety: We have written only valid ASCII to our vec
-        let mut s = unsafe { String::from_utf8_unchecked(std::mem::take(&mut buf)) };
-
-        for (i, c) in rest[..].char_indices() {
-            if c == 'Σ' {
-                // Σ maps to σ, except at the end of a word where it maps to ς.
-                // This is the only conditional (contextual) but language-independent mapping
-                // in `SpecialCasing.txt`,
-                // so hard-code it rather than have a generic "condition" mechanism.
-                // See https://github.com/rust-lang/rust/issues/26035
-                map_uppercase_sigma(rest, i, &mut s)
-            } else {
-                match conversions::to_lower(c) {
-                    [a, '\0', _] => s.push(a),
-                    [a, b, '\0'] => {
-                        s.push(a);
-                        s.push(b);
-                    }
-                    [a, b, c] => {
-                        s.push(a);
-                        s.push(b);
-                        s.push(c);
-                    }
+    // Safety: we know this is a valid char boundary since
+    // out.len() is only progressed if ascii bytes are found
+    let rest = unsafe { s.get_unchecked(buf.len()..) };
+
+    // Safety: We have written only valid ASCII to our vec
+    let mut s = unsafe { String::from_utf8_unchecked(std::mem::take(buf)) };
+
+    for (i, c) in rest[..].char_indices() {
+        if c == 'Σ' {
+            // Σ maps to σ, except at the end of a word where it maps to ς.
+            // This is the only conditional (contextual) but language-independent mapping
+            // in `SpecialCasing.txt`,
+            // so hard-code it rather than have a generic "condition" mechanism.
+            // See https://github.com/rust-lang/rust/issues/26035
+            map_uppercase_sigma(rest, i, &mut s)
+        } else {
+            match conversions::to_lower(c) {
+                [a, '\0', _] => s.push(a),
+                [a, b, '\0'] => {
+                    s.push(a);
+                    s.push(b);
+                }
+                [a, b, c] => {
+                    s.push(a);
+                    s.push(b);
+                    s.push(c);
                 }
             }
         }
+    }
 
-        fn map_uppercase_sigma(from: &str, i: usize, to: &mut String) {
-            // See https://www.unicode.org/versions/Unicode7.0.0/ch03.pdf#G33992
-            // for the definition of `Final_Sigma`.
-            debug_assert!('Σ'.len_utf8() == 2);
-            let is_word_final = case_ignoreable_then_cased(from[..i].chars().rev())
-                && !case_ignoreable_then_cased(from[i + 2..].chars());
-            to.push_str(if is_word_final { "ς" } else { "σ" });
+    fn map_uppercase_sigma(from: &str, i: usize, to: &mut String) {
+        // See https://www.unicode.org/versions/Unicode7.0.0/ch03.pdf#G33992
+        // for the definition of `Final_Sigma`.
+        debug_assert!('Σ'.len_utf8() == 2);
+        let is_word_final = case_ignoreable_then_cased(from[..i].chars().rev())
+            && !case_ignoreable_then_cased(from[i + 2..].chars());
+        to.push_str(if is_word_final { "ς" } else { "σ" });
+    }
+
+    fn case_ignoreable_then_cased<I: Iterator<Item = char>>(iter: I) -> bool {
+        use core::unicode::{Case_Ignorable, Cased};
+        #[allow(clippy::skip_while_next)]
+        match iter.skip_while(|&c| Case_Ignorable(c)).next() {
+            Some(c) => Cased(c),
+            None => false,
         }
+    }
+    // put buf back for next iteration
+    *buf = s.into_bytes();
+}
 
-        fn case_ignoreable_then_cased<I: Iterator<Item = char>>(iter: I) -> bool {
-            use core::unicode::{Case_Ignorable, Cased};
-            #[allow(clippy::skip_while_next)]
-            match iter.skip_while(|&c| Case_Ignorable(c)).next() {
-                Some(c) => Cased(c),
-                None => false,
-            }
-        }
-        // put buf back for next iteration
-        buf = s.into_bytes();
+// inlined from std
+#[cfg(feature = "nightly")]
+pub(super) fn to_lowercase<'a>(ca: &'a Utf8Chunked) -> Utf8Chunked {
+    // amortize allocation
+    let mut buf = Vec::new();
+    let f = |s: &'a str| {
+        to_lowercase_helper(s, &mut buf);
 
         // extend lifetime
         // lifetime is bound to 'a
         let slice = unsafe { std::str::from_utf8_unchecked(&buf) };
         unsafe { std::mem::transmute::<&str, &'a str>(slice) }
     };
     ca.apply_mut(f)
@@ -160,14 +165,31 @@
         // lifetime is bound to 'a
         let slice = unsafe { std::str::from_utf8_unchecked(slice) };
         unsafe { std::mem::transmute::<&str, &'a str>(slice) }
     };
     ca.apply_mut(f)
 }
 
+#[inline]
+#[cfg(feature = "nightly")]
+fn push_char_to_upper(c: char, s: &mut String) {
+    match conversions::to_upper(c) {
+        [a, '\0', _] => s.push(a),
+        [a, b, '\0'] => {
+            s.push(a);
+            s.push(b);
+        }
+        [a, b, c] => {
+            s.push(a);
+            s.push(b);
+            s.push(c);
+        }
+    }
+}
+
 // inlined from std
 #[cfg(feature = "nightly")]
 pub(super) fn to_uppercase<'a>(ca: &'a Utf8Chunked) -> Utf8Chunked {
     // amortize allocation
     let mut buf = Vec::new();
     let f = |s: &'a str| {
         convert_while_ascii(s.as_bytes(), u8::to_ascii_uppercase, &mut buf);
@@ -176,25 +198,58 @@
         // out.len() is only progressed if ascii bytes are found
         let rest = unsafe { s.get_unchecked(buf.len()..) };
 
         // Safety: We have written only valid ASCII to our vec
         let mut s = unsafe { String::from_utf8_unchecked(std::mem::take(&mut buf)) };
 
         for c in rest.chars() {
-            match conversions::to_upper(c) {
-                [a, '\0', _] => s.push(a),
-                [a, b, '\0'] => {
-                    s.push(a);
-                    s.push(b);
-                }
-                [a, b, c] => {
-                    s.push(a);
-                    s.push(b);
-                    s.push(c);
-                }
+            push_char_to_upper(c, &mut s);
+        }
+
+        // put buf back for next iteration
+        buf = s.into_bytes();
+
+        // extend lifetime
+        // lifetime is bound to 'a
+        let slice = unsafe { std::str::from_utf8_unchecked(&buf) };
+        unsafe { std::mem::transmute::<&str, &'a str>(slice) }
+    };
+    ca.apply_mut(f)
+}
+
+#[cfg(feature = "nightly")]
+pub(super) fn to_titlecase<'a>(ca: &'a Utf8Chunked) -> Utf8Chunked {
+    // amortize allocation
+    let mut buf = Vec::new();
+
+    // temporary scratch
+    // we have a double copy as we first convert to lowercase
+    // and then copy to `buf`
+    let mut scratch = Vec::new();
+    let f = |s: &'a str| {
+        unsafe {
+            buf.set_len(0);
+        }
+        // this helper sets scratch len to 0
+        to_lowercase_helper(s, &mut scratch);
+
+        let mut next_is_upper = true;
+
+        let lowercased = unsafe { std::str::from_utf8_unchecked(&scratch) };
+
+        let mut s = unsafe { String::from_utf8_unchecked(std::mem::take(&mut buf)) };
+
+        for c in lowercased.chars() {
+            let is_whitespace = c.is_whitespace();
+            if is_whitespace || !next_is_upper {
+                next_is_upper = is_whitespace;
+                s.push(c);
+            } else {
+                next_is_upper = false;
+                push_char_to_upper(c, &mut s);
             }
         }
 
         // put buf back for next iteration
         buf = s.into_bytes();
 
         // extend lifetime
```

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-ops/src/chunked_array/strings/json_path.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-ops/src/chunked_array/strings/json_path.rs`

 * *Files 3% similar despite different names*

```diff
@@ -60,19 +60,23 @@
 
         polars_json::ndjson::infer_iter(values_iter)
             .map(|d| DataType::from(&d))
             .map_err(|e| polars_err!(ComputeError: "error inferring JSON: {}", e))
     }
 
     /// Extracts a typed-JSON value for each row in the Utf8Chunked
-    fn json_extract(&self, dtype: Option<DataType>) -> PolarsResult<Series> {
+    fn json_extract(
+        &self,
+        dtype: Option<DataType>,
+        infer_schema_len: Option<usize>,
+    ) -> PolarsResult<Series> {
         let ca = self.as_utf8();
         let dtype = match dtype {
             Some(dt) => dt,
-            None => ca.json_infer(None)?,
+            None => ca.json_infer(infer_schema_len)?,
         };
 
         let buf_size = ca.get_values_size() + ca.null_count() * "null".len();
         let iter = ca.into_iter().map(|x| x.unwrap_or("null"));
 
         let array = polars_json::ndjson::deserialize::deserialize_iter(
             iter,
@@ -88,17 +92,22 @@
         let pat = PathCompiled::compile(json_path)
             .map_err(|e| polars_err!(ComputeError: "error compiling JSONpath expression: {}", e))?;
         Ok(self
             .as_utf8()
             .apply_on_opt(|opt_s| opt_s.and_then(|s| select_json(&pat, s))))
     }
 
-    fn json_path_extract(&self, json_path: &str, dtype: Option<DataType>) -> PolarsResult<Series> {
+    fn json_path_extract(
+        &self,
+        json_path: &str,
+        dtype: Option<DataType>,
+        infer_schema_len: Option<usize>,
+    ) -> PolarsResult<Series> {
         let selected_json = self.as_utf8().json_path_select(json_path)?;
-        selected_json.json_extract(dtype)
+        selected_json.json_extract(dtype, infer_schema_len)
     }
 }
 
 impl Utf8JsonPathImpl for Utf8Chunked {}
 
 #[cfg(test)]
 mod tests {
@@ -174,19 +183,19 @@
             ],
         )
         .unwrap()
         .into_series();
         let expected_dtype = expected_series.dtype().clone();
 
         assert!(ca
-            .json_extract(None)
+            .json_extract(None, None)
             .unwrap()
             .series_equal_missing(&expected_series));
         assert!(ca
-            .json_extract(Some(expected_dtype))
+            .json_extract(Some(expected_dtype), None)
             .unwrap()
             .series_equal_missing(&expected_series));
     }
 
     #[test]
     fn test_json_path_select() {
         let s = Series::new(
@@ -249,13 +258,13 @@
                 Some(Series::new("", &[0, 1])),
                 Some(Series::new("", &[2, 5])),
                 None,
             ],
         );
 
         assert!(ca
-            .json_path_extract("$.b[:].c", None)
+            .json_path_extract("$.b[:].c", None, None)
             .unwrap()
             .into_series()
             .series_equal_missing(&c_series));
     }
 }
```

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-ops/src/chunked_array/strings/justify.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-ops/src/chunked_array/strings/justify.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-ops/src/chunked_array/strings/mod.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-ops/src/chunked_array/strings/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-ops/src/chunked_array/strings/namespace.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-ops/src/chunked_array/strings/namespace.rs`

 * *Files 2% similar despite different names*

```diff
@@ -376,14 +376,22 @@
     /// Modify the strings to their uppercase equivalent
     #[must_use]
     fn to_uppercase(&self) -> Utf8Chunked {
         let ca = self.as_utf8();
         case::to_uppercase(ca)
     }
 
+    /// Modify the strings to their titlecase equivalent
+    #[must_use]
+    #[cfg(feature = "nightly")]
+    fn to_titlecase(&self) -> Utf8Chunked {
+        let ca = self.as_utf8();
+        case::to_titlecase(ca)
+    }
+
     /// Concat with the values from a second Utf8Chunked
     #[must_use]
     fn concat(&self, other: &Utf8Chunked) -> Utf8Chunked {
         let ca = self.as_utf8();
         ca + other
     }
```

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-ops/src/chunked_array/strings/replace.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-ops/src/chunked_array/strings/replace.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-ops/src/chunked_array/top_k.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-ops/src/chunked_array/top_k.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-ops/src/frame/join/merge_sorted.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-ops/src/frame/join/merge_sorted.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-ops/src/frame/join/mod.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-ops/src/frame/join/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-ops/src/frame/mod.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-ops/src/frame/mod.rs`

 * *Files 5% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     ///
     ///  let df = df! {
     ///       "id" => &[1, 2, 3, 1, 2, 3, 1, 1],
     ///       "type" => &["A", "B", "B", "B", "C", "C", "C", "B"],
     ///       "code" => &["X1", "X2", "X3", "X3", "X2", "X2", "X1", "X1"]
     ///   }.unwrap();
     ///
-    ///   let dummies = df.to_dummies().unwrap();
+    ///   let dummies = df.to_dummies(None, false).unwrap();
     ///   dbg!(dummies);
     /// # }
     /// ```
     /// Outputs:
     /// ```text
     ///  +------+------+------+--------+--------+--------+---------+---------+---------+
     ///  | id_1 | id_3 | id_2 | type_A | type_B | type_C | code_X1 | code_X2 | code_X3 |
@@ -69,43 +69,45 @@
     ///  +------+------+------+--------+--------+--------+---------+---------+---------+
     ///  | 1    | 0    | 0    | 0      | 0      | 1      | 1       | 0       | 0       |
     ///  +------+------+------+--------+--------+--------+---------+---------+---------+
     ///  | 1    | 0    | 0    | 0      | 1      | 0      | 1       | 0       | 0       |
     ///  +------+------+------+--------+--------+--------+---------+---------+---------+
     /// ```
     #[cfg(feature = "to_dummies")]
-    fn to_dummies(&self, separator: Option<&str>) -> PolarsResult<DataFrame> {
-        self._to_dummies(None, separator)
+    fn to_dummies(&self, separator: Option<&str>, drop_first: bool) -> PolarsResult<DataFrame> {
+        self._to_dummies(None, separator, drop_first)
     }
 
     #[cfg(feature = "to_dummies")]
     fn columns_to_dummies(
         &self,
         columns: Vec<&str>,
         separator: Option<&str>,
+        drop_first: bool,
     ) -> PolarsResult<DataFrame> {
-        self._to_dummies(Some(columns), separator)
+        self._to_dummies(Some(columns), separator, drop_first)
     }
 
     #[cfg(feature = "to_dummies")]
     fn _to_dummies(
         &self,
         columns: Option<Vec<&str>>,
         separator: Option<&str>,
+        drop_first: bool,
     ) -> PolarsResult<DataFrame> {
         let df = self.to_df();
 
         let set: PlHashSet<&str> =
             PlHashSet::from_iter(columns.unwrap_or_else(|| df.get_column_names()));
 
         let cols = POOL.install(|| {
             df.get_columns()
                 .par_iter()
                 .map(|s| match set.contains(s.name()) {
-                    true => s.to_dummies(separator),
+                    true => s.to_dummies(separator, drop_first),
                     false => Ok(s.clone().into_frame()),
                 })
                 .collect::<PolarsResult<Vec<_>>>()
         })?;
 
         accumulate_dataframes_horizontal(cols)
     }
```

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-ops/src/frame/pivot/mod.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-ops/src/frame/pivot/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-ops/src/frame/pivot/positioning.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-ops/src/frame/pivot/positioning.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-ops/src/series/ops/approx_algo/hyperloglogplus.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-ops/src/series/ops/approx_algo/hyperloglogplus.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-ops/src/series/ops/approx_unique.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-ops/src/series/ops/approx_unique.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-ops/src/series/ops/arg_min_max.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-ops/src/series/ops/arg_min_max.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-ops/src/series/ops/floor_divide.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-ops/src/series/ops/floor_divide.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-ops/src/series/ops/fused.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-ops/src/series/ops/fused.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-ops/src/series/ops/is_first.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-ops/src/series/ops/is_first.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-ops/src/series/ops/is_unique.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-ops/src/series/ops/is_unique.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-ops/src/series/ops/log.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-ops/src/series/ops/log.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-ops/src/series/ops/mod.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-ops/src/series/ops/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-ops/src/series/ops/rolling.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-ops/src/series/ops/rolling.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-ops/src/series/ops/search_sorted.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-ops/src/series/ops/search_sorted.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-ops/src/series/ops/to_dummies.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-ops/src/series/ops/to_dummies.rs`

 * *Files 6% similar despite different names*

```diff
@@ -9,27 +9,27 @@
 
 #[cfg(not(feature = "dtype-u8"))]
 type DummyType = i32;
 #[cfg(not(feature = "dtype-u8"))]
 type DummyCa = Int32Chunked;
 
 pub trait ToDummies {
-    fn to_dummies(&self, separator: Option<&str>) -> PolarsResult<DataFrame>;
+    fn to_dummies(&self, separator: Option<&str>, drop_first: bool) -> PolarsResult<DataFrame>;
 }
 
 impl ToDummies for Series {
-    fn to_dummies(&self, separator: Option<&str>) -> PolarsResult<DataFrame> {
+    fn to_dummies(&self, separator: Option<&str>, drop_first: bool) -> PolarsResult<DataFrame> {
         let sep = separator.unwrap_or("_");
         let col_name = self.name();
-        let groups = self.group_tuples(true, false)?;
+        let groups = self.group_tuples(true, drop_first)?;
 
         // safety: groups are in bounds
-        let columns = unsafe { self.agg_first(&groups) }
-            .iter()
-            .zip(groups.iter())
+        let columns = unsafe { self.agg_first(&groups) };
+        let columns = columns.iter().zip(groups.iter()).skip(drop_first as usize);
+        let columns = columns
             .map(|(av, group)| {
                 // strings are formatted with extra \" \" in polars, so we
                 // extract the string
                 let name = if let Some(s) = av.get_str() {
                     format!("{col_name}{sep}{s}")
                 } else {
                     // other types don't have this formatting issue
```

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-ops/src/series/ops/various.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-ops/src/series/ops/various.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-lazy/Cargo.toml` & `polars_u64_idx-0.18.4/local_dependencies/polars-lazy/Cargo.toml`

 * *Files 4% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 polars-time = { version = "0.30.0", path = "../polars-time", optional = true }
 polars-utils = { version = "0.30.0", path = "../polars-utils" }
 pyo3 = { version = "0.19", optional = true }
 rayon= "1.6"
 smartstring= { version = "1" }
 
 [features]
-nightly = ["polars-core/nightly", "polars-pipe/nightly"]
+nightly = ["polars-core/nightly", "polars-pipe/nightly", "polars-plan/nightly"]
 compile = ["polars-plan/compile"]
 streaming = ["chunked_ids", "polars-pipe/compile", "polars-plan/streaming"]
 default = ["compile"]
 parquet = ["polars-core/parquet", "polars-io/parquet", "polars-plan/parquet", "polars-pipe/parquet"]
 async = [
   "polars-plan/async",
   "polars-io/cloud",
@@ -63,14 +63,15 @@
 trigonometry = ["polars-plan/trigonometry"]
 sign = ["polars-plan/sign"]
 timezones = ["polars-plan/timezones"]
 list_take = ["polars-ops/list_take", "polars-plan/list_take"]
 list_count = ["polars-ops/list_count", "polars-plan/list_count"]
 
 true_div = ["polars-plan/true_div"]
+extract_jsonpath = ["polars-plan/extract_jsonpath", "polars-ops/extract_jsonpath"]
 
 # operations
 approx_unique = ["polars-plan/approx_unique"]
 is_in = ["polars-plan/is_in"]
 repeat_by = ["polars-plan/repeat_by"]
 round_series = ["polars-plan/round_series", "polars-ops/round_series"]
 is_first = ["polars-plan/is_first"]
```

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-lazy/LICENSE` & `polars_u64_idx-0.18.4/local_dependencies/polars-utils/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-lazy/src/dot.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-lazy/src/dot.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-lazy/src/dsl/eval.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-lazy/src/dsl/eval.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-lazy/src/dsl/functions.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-lazy/src/dsl/functions.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-lazy/src/dsl/list.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-lazy/src/dsl/list.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-lazy/src/dsl/mod.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-lazy/src/dsl/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-lazy/src/frame/anonymous_scan.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-lazy/src/frame/anonymous_scan.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-lazy/src/frame/csv.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-lazy/src/frame/csv.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-lazy/src/frame/file_list_reader.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-lazy/src/frame/file_list_reader.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-lazy/src/frame/ipc.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-lazy/src/frame/ipc.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-lazy/src/frame/mod.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-lazy/src/frame/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-lazy/src/frame/ndjson.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-lazy/src/frame/ndjson.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-lazy/src/frame/parquet.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-lazy/src/frame/parquet.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-lazy/src/frame/pivot.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-lazy/src/frame/pivot.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-lazy/src/lib.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-lazy/src/lib.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-lazy/src/physical_plan/executors/cache.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-lazy/src/physical_plan/executors/cache.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-lazy/src/physical_plan/executors/executor.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-lazy/src/physical_plan/executors/executor.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-lazy/src/physical_plan/executors/ext_context.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-lazy/src/physical_plan/executors/ext_context.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-lazy/src/physical_plan/executors/filter.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-lazy/src/physical_plan/executors/filter.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-lazy/src/physical_plan/executors/groupby.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-lazy/src/physical_plan/executors/groupby.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-lazy/src/physical_plan/executors/groupby_dynamic.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-lazy/src/physical_plan/executors/groupby_dynamic.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-lazy/src/physical_plan/executors/groupby_partitioned.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-lazy/src/physical_plan/executors/groupby_partitioned.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-lazy/src/physical_plan/executors/groupby_rolling.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-lazy/src/physical_plan/executors/groupby_rolling.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-lazy/src/physical_plan/executors/join.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-lazy/src/physical_plan/executors/join.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-lazy/src/physical_plan/executors/mod.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-lazy/src/physical_plan/executors/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-lazy/src/physical_plan/executors/projection.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-lazy/src/physical_plan/executors/projection.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-lazy/src/physical_plan/executors/python_scan.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-lazy/src/physical_plan/executors/python_scan.rs`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 use polars_core::error::to_compute_err;
 use pyo3::prelude::*;
-use pyo3::types::PyBytes;
 
 use super::*;
 
 pub(crate) struct PythonScanExec {
     pub(crate) options: PythonOptions,
 }
 
@@ -18,23 +17,28 @@
         }
         let with_columns = self.options.with_columns.take();
         let pyarrow_predicate = self.options.predicate.take();
         let n_rows = self.options.n_rows.take();
         Python::with_gil(|py| {
             let pl = PyModule::import(py, "polars").unwrap();
             let utils = pl.getattr("utils").unwrap();
-            let deser_and_exec = utils.getattr("_deserialize_and_execute").unwrap();
+            let callable = utils.getattr("_execute_from_rust").unwrap();
 
-            let bytes = PyBytes::new(py, &self.options.scan_fn);
+            let python_scan_function = self.options.scan_fn.take().unwrap().0;
 
             let with_columns =
                 with_columns.map(|mut cols| std::mem::take(Arc::make_mut(&mut cols)));
 
-            let out = deser_and_exec
-                .call1((bytes, with_columns, pyarrow_predicate, n_rows))
+            let out = callable
+                .call1((
+                    python_scan_function,
+                    with_columns,
+                    pyarrow_predicate,
+                    n_rows,
+                ))
                 .map_err(to_compute_err)?;
             let pydf = out.getattr("_df").unwrap();
             let raw_parts = pydf.call_method0("into_raw_parts").unwrap();
             let raw_parts = raw_parts.extract::<(usize, usize, usize)>().unwrap();
 
             let (ptr, len, cap) = raw_parts;
             unsafe {
```

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-lazy/src/physical_plan/executors/scan/csv.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-lazy/src/physical_plan/executors/scan/csv.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-lazy/src/physical_plan/executors/scan/ipc.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-lazy/src/physical_plan/executors/scan/ipc.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-lazy/src/physical_plan/executors/scan/mod.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-lazy/src/physical_plan/executors/scan/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-lazy/src/physical_plan/executors/scan/ndjson.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-lazy/src/physical_plan/executors/scan/ndjson.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-lazy/src/physical_plan/executors/scan/parquet.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-lazy/src/physical_plan/executors/scan/parquet.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-lazy/src/physical_plan/executors/slice.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-lazy/src/physical_plan/executors/slice.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-lazy/src/physical_plan/executors/sort.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-lazy/src/physical_plan/executors/sort.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-lazy/src/physical_plan/executors/stack.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-lazy/src/physical_plan/executors/stack.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-lazy/src/physical_plan/executors/udf.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-lazy/src/physical_plan/executors/udf.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-lazy/src/physical_plan/executors/union.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-lazy/src/physical_plan/executors/union.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-lazy/src/physical_plan/executors/unique.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-lazy/src/physical_plan/executors/unique.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-lazy/src/physical_plan/exotic.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-lazy/src/physical_plan/exotic.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-lazy/src/physical_plan/expressions/aggregation.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-lazy/src/physical_plan/expressions/aggregation.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-lazy/src/physical_plan/expressions/alias.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-lazy/src/physical_plan/expressions/alias.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-lazy/src/physical_plan/expressions/apply.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-lazy/src/physical_plan/expressions/apply.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-lazy/src/physical_plan/expressions/binary.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-lazy/src/physical_plan/expressions/binary.rs`

 * *Files 2% similar despite different names*

```diff
@@ -151,21 +151,36 @@
         Some(&self.expr)
     }
 
     fn evaluate(&self, df: &DataFrame, state: &ExecutionState) -> PolarsResult<Series> {
         // window functions may set a global state that determine their output
         // state, so we don't let them run in parallel as they race
         // they also saturate the thread pool by themselves, so that's fine
-        let (lhs, rhs) = if state.has_window() {
+        let has_window = state.has_window();
+        // streaming takes care of parallelism, don't parallelize here, as it
+        // increases contention
+
+        #[cfg(feature = "streaming")]
+        let in_streaming = state.in_streaming_engine();
+
+        #[cfg(not(feature = "streaming"))]
+        let in_streaming = false;
+
+        let (lhs, rhs) = if has_window {
             let mut state = state.split();
             state.remove_cache_window_flag();
             (
                 self.left.evaluate(df, &state),
                 self.right.evaluate(df, &state),
             )
+        } else if in_streaming {
+            (
+                self.left.evaluate(df, state),
+                self.right.evaluate(df, state),
+            )
         } else {
             POOL.install(|| {
                 rayon::join(
                     || self.left.evaluate(df, state),
                     || self.right.evaluate(df, state),
                 )
             })
```

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-lazy/src/physical_plan/expressions/cache.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-lazy/src/physical_plan/expressions/cache.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-lazy/src/physical_plan/expressions/cast.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-lazy/src/physical_plan/expressions/cast.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-lazy/src/physical_plan/expressions/column.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-lazy/src/physical_plan/expressions/column.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-lazy/src/physical_plan/expressions/count.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-lazy/src/physical_plan/expressions/count.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-lazy/src/physical_plan/expressions/filter.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-lazy/src/physical_plan/expressions/filter.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-lazy/src/physical_plan/expressions/group_iter.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-lazy/src/physical_plan/expressions/group_iter.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-lazy/src/physical_plan/expressions/literal.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-lazy/src/physical_plan/expressions/literal.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-lazy/src/physical_plan/expressions/mod.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-lazy/src/physical_plan/expressions/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-lazy/src/physical_plan/expressions/slice.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-lazy/src/physical_plan/expressions/slice.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-lazy/src/physical_plan/expressions/sort.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-lazy/src/physical_plan/expressions/sort.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-lazy/src/physical_plan/expressions/sortby.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-lazy/src/physical_plan/expressions/sortby.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-lazy/src/physical_plan/expressions/take.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-lazy/src/physical_plan/expressions/take.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-lazy/src/physical_plan/expressions/ternary.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-lazy/src/physical_plan/expressions/ternary.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-lazy/src/physical_plan/expressions/window.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-lazy/src/physical_plan/expressions/window.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-lazy/src/physical_plan/file_cache.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-lazy/src/physical_plan/file_cache.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-lazy/src/physical_plan/node_timer.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-lazy/src/physical_plan/node_timer.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-lazy/src/physical_plan/planner/expr.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-lazy/src/physical_plan/planner/expr.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-lazy/src/physical_plan/planner/lp.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-lazy/src/physical_plan/planner/lp.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-lazy/src/physical_plan/state.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-lazy/src/physical_plan/state.rs`

 * *Files 11% similar despite different names*

```diff
@@ -23,14 +23,17 @@
     pub(super) struct StateFlags: u8 {
         /// More verbose logging
         const VERBOSE = 0x01;
         /// Indicates that window expression's [`GroupTuples`] may be cached.
         const CACHE_WINDOW_EXPR = 0x02;
         /// Indicates the expression has a window function
         const HAS_WINDOW = 0x04;
+        /// If set, the expression is evaluated in the
+        /// streaming engine.
+        const IN_STREAMING = 0x08;
     }
 }
 
 impl Default for StateFlags {
     fn default() -> Self {
         StateFlags::CACHE_WINDOW_EXPR
     }
@@ -263,14 +266,28 @@
     // this will trigger some conservative
     pub(super) fn insert_has_window_function_flag(&mut self) {
         self.set_flags(&|mut flags| {
             flags.insert(StateFlags::HAS_WINDOW);
             flags
         });
     }
+
+    #[cfg(feature = "streaming")]
+    pub(super) fn set_in_streaming_engine(&mut self) {
+        self.set_flags(&|mut flags| {
+            flags.insert(StateFlags::IN_STREAMING);
+            flags
+        });
+    }
+
+    #[cfg(feature = "streaming")]
+    pub(super) fn in_streaming_engine(&self) -> bool {
+        let flags: StateFlags = self.flags.load(Ordering::Relaxed).into();
+        flags.contains(StateFlags::IN_STREAMING)
+    }
 }
 
 impl Default for ExecutionState {
     fn default() -> Self {
         ExecutionState::new()
     }
 }
```

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-lazy/src/physical_plan/streaming/checks.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-lazy/src/physical_plan/streaming/checks.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-lazy/src/physical_plan/streaming/construct_pipeline.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-lazy/src/physical_plan/streaming/construct_pipeline.rs`

 * *Files 1% similar despite different names*

```diff
@@ -255,18 +255,19 @@
         projection: None,
         selection: None,
     });
 
     ALogicalPlan::MapFunction {
         function: FunctionNode::Pipeline {
             function: Arc::new(move |_df: DataFrame| {
-                let state = ExecutionState::new();
+                let mut state = ExecutionState::new();
                 if state.verbose() {
                     eprintln!("RUN STREAMING PIPELINE")
                 }
+                state.set_in_streaming_engine();
                 let state = Box::new(state) as Box<dyn SExecutionContext>;
                 pipeline.execute(state)
             }),
             schema,
             original: original_lp.map(Arc::new),
         },
         input: dummy,
```

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-lazy/src/physical_plan/streaming/convert_alp.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-lazy/src/physical_plan/streaming/convert_alp.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-lazy/src/physical_plan/streaming/tree.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-lazy/src/physical_plan/streaming/tree.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-lazy/src/prelude.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-lazy/src/prelude.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-lazy/src/tests/aggregations.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-lazy/src/tests/aggregations.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-lazy/src/tests/arity.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-lazy/src/tests/arity.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-lazy/src/tests/cse.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-lazy/src/tests/cse.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-lazy/src/tests/io.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-lazy/src/tests/io.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-lazy/src/tests/logical.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-lazy/src/tests/logical.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-lazy/src/tests/mod.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-lazy/src/tests/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-lazy/src/tests/optimization_checks.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-lazy/src/tests/optimization_checks.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-lazy/src/tests/predicate_queries.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-lazy/src/tests/predicate_queries.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-lazy/src/tests/projection_queries.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-lazy/src/tests/projection_queries.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-lazy/src/tests/queries.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-lazy/src/tests/queries.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-lazy/src/tests/streaming.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-lazy/src/tests/streaming.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-lazy/src/tests/tpch.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-lazy/src/tests/tpch.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-lazy/src/utils.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-lazy/src/utils.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-arrow/Cargo.toml` & `polars_u64_idx-0.18.4/local_dependencies/polars-arrow/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -32,19 +32,19 @@
 performant = []
 like = ["arrow/compute_like"]
 timezones = ["chrono-tz", "chrono"]
 simd = []
 
 [dependencies.arrow]
 package = "arrow2"
-git = "https://github.com/jorgecarleitao/arrow2"
-# git = "https://github.com/ritchie46/arrow2"
-rev = "2d2e7053f9a50810bfe9cecff25ab39089aef98e"
+# git = "https://github.com/jorgecarleitao/arrow2"
+git = "https://github.com/ritchie46/arrow2"
+# rev = "2d2e7053f9a50810bfe9cecff25ab39089aef98e"
 # path = "../arrow2"
-# branch = "polars_2023-05-25"
+branch = "polars_2023-06-23"
 version = "0.17"
 default-features = false
 features = [
   "compute_aggregate",
   "compute_arithmetics",
   "compute_boolean",
   "compute_boolean_kleene",
```

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-arrow/LICENSE` & `polars_u64_idx-0.18.4/local_dependencies/polars-time/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-arrow/src/array/default_arrays.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-arrow/src/array/default_arrays.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-arrow/src/array/fixed_size_list.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-arrow/src/array/fixed_size_list.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-arrow/src/array/get.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-arrow/src/array/get.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-arrow/src/array/list.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-arrow/src/array/list.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-arrow/src/array/mod.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-arrow/src/array/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-arrow/src/array/null.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-arrow/src/array/null.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-arrow/src/array/slice.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-arrow/src/array/slice.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-arrow/src/array/utf8.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-arrow/src/array/utf8.rs`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 use arrow::array::{BinaryArray, Utf8Array};
 use arrow::datatypes::DataType;
 use arrow::offset::Offsets;
 
-use crate::trusted_len::PushUnchecked;
+use crate::trusted_len::TrustedLenPush;
 
 #[inline]
 unsafe fn extend_from_trusted_len_values_iter<I, P>(
     offsets: &mut Vec<i64>,
     values: &mut Vec<u8>,
     iterator: I,
 ) where
```

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-arrow/src/bit_util.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-arrow/src/bit_util.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-arrow/src/bitmap/mutable.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-arrow/src/bitmap/mutable.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-arrow/src/compute/arithmetics/decimal/commutative.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-arrow/src/compute/arithmetics/decimal/commutative.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-arrow/src/compute/arithmetics/decimal/div.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-arrow/src/compute/arithmetics/decimal/div.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-arrow/src/compute/arithmetics/decimal/mod.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-arrow/src/compute/arithmetics/decimal/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-arrow/src/compute/arithmetics/decimal/mul.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-arrow/src/compute/arithmetics/decimal/mul.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-arrow/src/compute/bitwise.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-arrow/src/compute/bitwise.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-arrow/src/compute/cast.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-arrow/src/compute/cast.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-arrow/src/compute/decimal.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-arrow/src/compute/decimal.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-arrow/src/compute/mod.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-arrow/src/compute/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-arrow/src/compute/take/boolean.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-arrow/src/compute/take/boolean.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-arrow/src/compute/take/fixed_size_list.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-arrow/src/compute/take/fixed_size_list.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-arrow/src/compute/take/mod.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-arrow/src/compute/take/mod.rs`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 use arrow::buffer::Buffer;
 use arrow::datatypes::{DataType, PhysicalType};
 use arrow::offset::Offsets;
 use arrow::types::NativeType;
 
 use crate::bit_util::unset_bit_raw;
 use crate::prelude::*;
-use crate::trusted_len::{PushUnchecked, TrustedLen};
+use crate::trusted_len::{TrustedLen, TrustedLenPush};
 use crate::utils::{with_match_primitive_type, CustomIterTools};
 
 /// # Safety
 /// Does not do bounds checks
 pub unsafe fn take_unchecked(arr: &dyn Array, idx: &IdxArr) -> ArrayRef {
     if idx.null_count() == idx.len() {
         return new_null_array(arr.data_type().clone(), idx.len());
```

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-arrow/src/compute/tile.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-arrow/src/compute/tile.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-arrow/src/conversion.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-arrow/src/conversion.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-arrow/src/data_types.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-arrow/src/data_types.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-arrow/src/floats/ord.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-arrow/src/floats/ord.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-arrow/src/index.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-arrow/src/index.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-arrow/src/is_valid.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-arrow/src/is_valid.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-arrow/src/kernels/agg_mean.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-arrow/src/kernels/agg_mean.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-arrow/src/kernels/comparison.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-arrow/src/kernels/comparison.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-arrow/src/kernels/concatenate.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-arrow/src/kernels/concatenate.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-arrow/src/kernels/ewm/average.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-arrow/src/kernels/ewm/average.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-arrow/src/kernels/ewm/mod.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-arrow/src/kernels/ewm/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-arrow/src/kernels/ewm/variance.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-arrow/src/kernels/ewm/variance.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-arrow/src/kernels/float.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-arrow/src/kernels/float.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-arrow/src/kernels/list.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-arrow/src/kernels/list.rs`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 use arrow::array::ListArray;
 use arrow::offset::{Offsets, OffsetsBuffer};
 
 use crate::compute::take::take_unchecked;
 use crate::prelude::*;
-use crate::trusted_len::PushUnchecked;
+use crate::trusted_len::TrustedLenPush;
 use crate::utils::CustomIterTools;
 
 /// Get the indices that would result in a get operation on the lists values.
 /// for example, consider this list:
 /// ```text
 /// [[1, 2, 3],
 ///  [4, 5],
```

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-arrow/src/kernels/list_bytes_iter.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-arrow/src/kernels/list_bytes_iter.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-arrow/src/kernels/mod.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-arrow/src/kernels/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-arrow/src/kernels/rolling/mod.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-arrow/src/kernels/rolling/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/mean.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/mean.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/min_max.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/min_max.rs`

 * *Files 2% similar despite different names*

```diff
@@ -38,20 +38,16 @@
     min_idx: usize,
     last_start: usize,
     last_end: usize,
 }
 
 impl<'a, T: NativeType + IsFloat + PartialOrd> RollingAggWindowNoNulls<'a, T> for MinWindow<'a, T> {
     fn new(slice: &'a [T], start: usize, end: usize, _params: DynArgs) -> Self {
-        let (idx, min) = slice[start..end]
-            .iter()
-            .enumerate()
-            .rev()
-            .min_by(|&a, &b| compare_fn_nan_min(a.1, b.1))
-            .unwrap_or((0, &slice[start]));
+        let (idx, min) =
+            unsafe { get_min_and_idx(slice, start, end).unwrap_or((0, &slice[start])) };
         Self {
             slice,
             min: *min,
             min_idx: start + idx,
             last_start: start,
             last_end: end,
         }
@@ -61,21 +57,22 @@
         //For details see: https://github.com/pola-rs/polars/pull/9277#issuecomment-1581401692
         self.last_start = start; // Don't care where the last one started
         let old_last_end = self.last_end; // But we need this
         self.last_end = end;
 
         let entering_start = std::cmp::max(old_last_end, start);
         let entering = get_min_and_idx(self.slice, entering_start, end);
+        let empty_overlap = old_last_end <= start;
 
-        if entering.is_some_and(|em| compare_fn_nan_min(&self.min, em.1).is_ge()) {
+        if entering.is_some_and(|em| compare_fn_nan_min(&self.min, em.1).is_ge() || empty_overlap) {
             // If the entering min <= the current min return early, since no value in the overlap can be smaller than either.
             self.min = *entering.unwrap().1;
             self.min_idx = entering_start + entering.unwrap().0;
             return self.min;
-        } else if self.min_idx >= start {
+        } else if self.min_idx >= start || empty_overlap {
             // If the entering min isn't the smallest but the current min is between start and end we can still ignore the overlap
             return self.min;
         }
         // Otherwise get the min of the overlapping window and the entering min
         match (get_min_and_idx(self.slice, start, old_last_end), entering) {
             (Some(pm), Some(em)) => {
                 if compare_fn_nan_min(pm.1, em.1).is_ge() {
@@ -120,19 +117,16 @@
     max_idx: usize,
     last_start: usize,
     last_end: usize,
 }
 
 impl<'a, T: NativeType + IsFloat + PartialOrd> RollingAggWindowNoNulls<'a, T> for MaxWindow<'a, T> {
     fn new(slice: &'a [T], start: usize, end: usize, _params: DynArgs) -> Self {
-        let (idx, max) = slice[start..end]
-            .iter()
-            .enumerate()
-            .max_by(|&a, &b| compare_fn_nan_max(a.1, b.1))
-            .unwrap_or((0, &slice[start]));
+        let (idx, max) =
+            unsafe { get_max_and_idx(slice, start, end).unwrap_or((0, &slice[start])) };
         Self {
             slice,
             max: *max,
             max_idx: start + idx,
             last_start: start,
             last_end: end,
         }
@@ -141,21 +135,22 @@
     unsafe fn update(&mut self, start: usize, end: usize) -> T {
         self.last_start = start; // Don't care where the last one started
         let old_last_end = self.last_end; // But we need this
         self.last_end = end;
 
         let entering_start = std::cmp::max(old_last_end, start);
         let entering = get_max_and_idx(self.slice, entering_start, end);
+        let empty_overlap = old_last_end < start;
 
-        if entering.is_some_and(|em| compare_fn_nan_max(&self.max, em.1).is_le()) {
+        if entering.is_some_and(|em| compare_fn_nan_max(&self.max, em.1).is_le() || empty_overlap) {
             // If the entering max >= the current max return early, since no value in the overlap can be larger than either.
             self.max = *entering.unwrap().1;
             self.max_idx = entering_start + entering.unwrap().0;
             return self.max;
-        } else if self.max_idx >= start {
+        } else if self.max_idx >= start || empty_overlap {
             // If the entering max isn't the largest but the current max is between start and end we can still ignore the overlap
             return self.max;
         }
         // Otherwise get the max of the overlapping window and the entering max
         match (get_max_and_idx(self.slice, start, old_last_end), entering) {
             (Some(pm), Some(em)) => {
                 if compare_fn_nan_max(pm.1, em.1).is_le() {
```

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/mod.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/quantile.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/quantile.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/sum.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/sum.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/variance.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/variance.rs`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 use no_nulls::{rolling_apply_agg_window, RollingAggWindowNoNulls};
-use num_traits::pow::Pow;
 
 use super::mean::MeanWindow;
 use super::*;
 
 pub(super) struct SumSquaredWindow<'a, T> {
     slice: &'a [T],
     sum_of_squares: T,
@@ -191,93 +190,14 @@
                 compute_var_weights,
                 &weights,
             )
         }
     }
 }
 
-// E[(xi - E[x])^2]
-// can be expanded to
-// E[x^2] - E[x]^2
-pub struct StdWindow<'a, T> {
-    var: VarWindow<'a, T>,
-}
-
-impl<
-        'a,
-        T: NativeType
-            + IsFloat
-            + Float
-            + std::iter::Sum
-            + AddAssign
-            + SubAssign
-            + Div<Output = T>
-            + NumCast
-            + One
-            + Zero
-            + Sub<Output = T>
-            + PartialOrd
-            + Pow<T, Output = T>,
-    > RollingAggWindowNoNulls<'a, T> for StdWindow<'a, T>
-{
-    fn new(slice: &'a [T], start: usize, end: usize, params: DynArgs) -> Self {
-        Self {
-            var: VarWindow::new(slice, start, end, params),
-        }
-    }
-
-    unsafe fn update(&mut self, start: usize, end: usize) -> T {
-        let var = self.var.update(start, end);
-        var.pow(NumCast::from(0.5).unwrap())
-    }
-}
-
-pub fn rolling_std<T>(
-    values: &[T],
-    window_size: usize,
-    min_periods: usize,
-    center: bool,
-    weights: Option<&[f64]>,
-    params: DynArgs,
-) -> PolarsResult<ArrayRef>
-where
-    T: NativeType
-        + Float
-        + IsFloat
-        + std::iter::Sum
-        + AddAssign
-        + SubAssign
-        + Div<Output = T>
-        + NumCast
-        + One
-        + Zero
-        + Sub<Output = T>
-        + Pow<T, Output = T>,
-{
-    match (center, weights) {
-        (true, None) => rolling_apply_agg_window::<StdWindow<_>, _, _>(
-            values,
-            window_size,
-            min_periods,
-            det_offsets_center,
-            params,
-        ),
-        (false, None) => rolling_apply_agg_window::<StdWindow<_>, _, _>(
-            values,
-            window_size,
-            min_periods,
-            det_offsets,
-            params,
-        ),
-        (_, Some(_)) => {
-            panic!("weights not yet supported for rolling_std")
-        }
-    }
-}
-
 #[cfg(test)]
 mod test {
     use super::*;
 
     #[test]
     fn test_rolling_var() {
         let values = &[1.0f64, 5.0, 3.0, 4.0];
```

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-arrow/src/kernels/rolling/nulls/mean.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-arrow/src/kernels/rolling/nulls/mean.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-arrow/src/kernels/rolling/nulls/min_max.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-arrow/src/kernels/rolling/nulls/min_max.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-arrow/src/kernels/rolling/nulls/mod.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-arrow/src/kernels/rolling/nulls/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-arrow/src/kernels/rolling/nulls/quantile.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-arrow/src/kernels/rolling/nulls/quantile.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-arrow/src/kernels/rolling/nulls/sum.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-arrow/src/kernels/rolling/nulls/sum.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-arrow/src/kernels/rolling/nulls/variance.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-arrow/src/kernels/rolling/nulls/variance.rs`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 use mean::MeanWindow;
 use nulls;
 use nulls::{rolling_apply_agg_window, RollingAggWindowNulls};
-use num_traits::pow::Pow;
 
 use super::*;
 
 pub(super) struct SumSquaredWindow<'a, T> {
     slice: &'a [T],
     validity: &'a Bitmap,
     sum_of_squares: Option<T>,
@@ -219,88 +218,8 @@
         arr.values().as_slice(),
         arr.validity().as_ref().unwrap(),
         window_size,
         min_periods,
         offsets_fn,
         params,
     )
-}
-
-pub struct StdWindow<'a, T> {
-    var: VarWindow<'a, T>,
-}
-
-impl<
-        'a,
-        T: NativeType
-            + IsFloat
-            + Float
-            + std::iter::Sum
-            + AddAssign
-            + SubAssign
-            + Div<Output = T>
-            + NumCast
-            + One
-            + Zero
-            + PartialOrd
-            + Add<Output = T>
-            + Sub<Output = T>
-            + Pow<T, Output = T>,
-    > RollingAggWindowNulls<'a, T> for StdWindow<'a, T>
-{
-    unsafe fn new(
-        slice: &'a [T],
-        validity: &'a Bitmap,
-        start: usize,
-        end: usize,
-        params: DynArgs,
-    ) -> Self {
-        Self {
-            var: VarWindow::new(slice, validity, start, end, params),
-        }
-    }
-
-    unsafe fn update(&mut self, start: usize, end: usize) -> Option<T> {
-        self.var
-            .update(start, end)
-            .map(|var| var.pow(NumCast::from(0.5).unwrap()))
-    }
-    fn is_valid(&self, min_periods: usize) -> bool {
-        self.var.is_valid(min_periods)
-    }
-}
-
-pub fn rolling_std<T>(
-    arr: &PrimitiveArray<T>,
-    window_size: usize,
-    min_periods: usize,
-    center: bool,
-    weights: Option<&[f64]>,
-    params: DynArgs,
-) -> ArrayRef
-where
-    T: NativeType
-        + std::iter::Sum<T>
-        + Zero
-        + AddAssign
-        + SubAssign
-        + IsFloat
-        + Float
-        + Pow<T, Output = T>,
-{
-    if weights.is_some() {
-        panic!("weights not yet supported on array with null values")
-    }
-    let offsets_fn = if center {
-        det_offsets_center
-    } else {
-        det_offsets
-    };
-    rolling_apply_agg_window::<StdWindow<_>, _, _>(
-        arr.values().as_slice(),
-        arr.validity().as_ref().unwrap(),
-        window_size,
-        min_periods,
-        offsets_fn,
-        params,
-    )
 }
```

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-arrow/src/kernels/rolling/window.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-arrow/src/kernels/rolling/window.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-arrow/src/kernels/set.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-arrow/src/kernels/set.rs`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 use arrow::types::NativeType;
 use polars_error::polars_err;
 
 use crate::array::default_arrays::FromData;
 use crate::error::PolarsResult;
 use crate::index::IdxSize;
 use crate::kernels::BinaryMaskedSliceIterator;
-use crate::trusted_len::PushUnchecked;
+use crate::trusted_len::TrustedLenPush;
 
 /// Set values in a primitive array where the primitive array has null values.
 /// this is faster because we don't have to invert and combine bitmaps
 pub fn set_at_nulls<T>(array: &PrimitiveArray<T>, value: T) -> PrimitiveArray<T>
 where
     T: NativeType,
 {
```

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-arrow/src/kernels/sort_partition.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-arrow/src/kernels/sort_partition.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-arrow/src/kernels/sorted_join/inner.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-arrow/src/kernels/sorted_join/inner.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-arrow/src/kernels/sorted_join/left.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-arrow/src/kernels/sorted_join/left.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-arrow/src/kernels/string.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-arrow/src/kernels/string.rs`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 use arrow::array::{UInt32Array, Utf8Array};
 use arrow::buffer::Buffer;
 use arrow::datatypes::DataType;
 
 use crate::prelude::*;
-use crate::trusted_len::PushUnchecked;
+use crate::trusted_len::TrustedLenPush;
 
 pub fn string_lengths(array: &Utf8Array<i64>) -> ArrayRef {
     let values = array
         .offsets()
         .as_slice()
         .windows(2)
         .map(|x| (x[1] - x[0]) as u32);
```

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-arrow/src/kernels/take_agg/boolean.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-arrow/src/kernels/take_agg/boolean.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-arrow/src/kernels/take_agg/mod.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-arrow/src/kernels/take_agg/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-arrow/src/kernels/take_agg/var.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-arrow/src/kernels/take_agg/var.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-arrow/src/kernels/time.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-arrow/src/kernels/time.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-arrow/src/slice.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-arrow/src/slice.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-arrow/src/trusted_len/boolean.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-arrow/src/trusted_len/boolean.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-arrow/src/trusted_len/mod.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-arrow/src/trusted_len/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-arrow/src/trusted_len/push_unchecked.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-arrow/src/trusted_len/push_unchecked.rs`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 use super::*;
 
-pub trait PushUnchecked<T> {
+pub trait TrustedLenPush<T> {
     /// Will push an item and not check if there is enough capacity
     ///
     /// # Safety
     /// Caller must ensure the array has enough capacity to hold `T`.
     unsafe fn push_unchecked(&mut self, value: T);
 
     /// Extend the array with an iterator who's length can be trusted
@@ -28,15 +28,15 @@
         unsafe { Self::from_trusted_len_iter_unchecked(iter) }
     }
     /// # Safety
     /// Caller must ensure the iterators reported length is correct
     unsafe fn from_trusted_len_iter_unchecked<I: IntoIterator<Item = T>>(iter: I) -> Self;
 }
 
-impl<T> PushUnchecked<T> for Vec<T> {
+impl<T> TrustedLenPush<T> for Vec<T> {
     #[inline]
     unsafe fn push_unchecked(&mut self, value: T) {
         debug_assert!(self.capacity() > self.len());
         let end = self.as_mut_ptr().add(self.len());
         std::ptr::write(end, value);
         self.set_len(self.len() + 1);
     }
```

### Comparing `polars_u64_idx-0.18.3/local_dependencies/polars-arrow/src/utils.rs` & `polars_u64_idx-0.18.4/local_dependencies/polars-arrow/src/utils.rs`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 use std::ops::{BitAnd, BitOr};
 
 use arrow::array::PrimitiveArray;
 use arrow::bitmap::Bitmap;
 use arrow::types::NativeType;
 
-use crate::trusted_len::{FromIteratorReversed, PushUnchecked, TrustedLen};
+use crate::trusted_len::{FromIteratorReversed, TrustedLen, TrustedLenPush};
 
 #[derive(Clone)]
 pub struct TrustMyLength<I: Iterator<Item = J>, J> {
     iter: I,
     len: usize,
 }
```

### Comparing `polars_u64_idx-0.18.3/Cargo.toml` & `polars_u64_idx-0.18.4/Cargo.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "py-polars"
-version = "0.18.3"
+version = "0.18.4"
 edition = "2021"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 
 [workspace]
 # prevents package from thinking it's in the workspace
 [target.'cfg(any(not(target_os = "linux"), use_mimalloc))'.dependencies]
```

### Comparing `polars_u64_idx-0.18.3/LICENSE` & `polars_u64_idx-0.18.4/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/Makefile` & `polars_u64_idx-0.18.4/Makefile`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/README.md` & `polars_u64_idx-0.18.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -266,15 +266,15 @@
 
 Or for python users install `pip install polars-u64-idx`.
 
 Don't use this unless you hit the row boundary as the default polars is faster and consumes less memory.
 
 ## Legacy
 
-Do you want polars to run on an old CPU (e.g. dating from before 2011)? Install `pip polars-lts-cpu`. This polars project is
+Do you want polars to run on an old CPU (e.g. dating from before 2011)? Install `pip install polars-lts-cpu`. This polars project is
 compiled without [avx](https://en.wikipedia.org/wiki/Advanced_Vector_Extensions) target features.
 
 ## Acknowledgements
 
 Development of Polars is proudly powered by
 
 [![Xomnia](https://raw.githubusercontent.com/pola-rs/polars-static/master/sponsors/xomnia.png)](https://www.xomnia.com/)
```

#### html2text {}

```diff
@@ -106,15 +106,15 @@
 Extending polars with UDFs compiled in Rust is easy. We expose pyo3 extensions
 for `DataFrame` and `Series` data structures. See more in https://github.com/
 pola-rs/pyo3-polars. ## Going big... Do you expect more than `2^32` ~4,2
 billion rows? Compile polars with the `bigidx` feature flag. Or for python
 users install `pip install polars-u64-idx`. Don't use this unless you hit the
 row boundary as the default polars is faster and consumes less memory. ##
 Legacy Do you want polars to run on an old CPU (e.g. dating from before 2011)?
-Install `pip polars-lts-cpu`. This polars project is compiled without [avx]
-(https://en.wikipedia.org/wiki/Advanced_Vector_Extensions) target features. ##
-Acknowledgements Development of Polars is proudly powered by [![Xomnia](https:/
-/raw.githubusercontent.com/pola-rs/polars-static/master/sponsors/xomnia.png)]
-(https://www.xomnia.com/) ## Sponsors [[https://raw.githubusercontent.com/pola-
-rs/polars-static/master/sponsors/xomnia.png]](https://www.xomnia.com/) &emsp; [
-[https://www.jetbrains.com/company/brand/img/jetbrains_logo.png]](https://
-www.jetbrains.com)
+Install `pip install polars-lts-cpu`. This polars project is compiled without
+[avx](https://en.wikipedia.org/wiki/Advanced_Vector_Extensions) target
+features. ## Acknowledgements Development of Polars is proudly powered by [!
+[Xomnia](https://raw.githubusercontent.com/pola-rs/polars-static/master/
+sponsors/xomnia.png)](https://www.xomnia.com/) ## Sponsors [[https://
+raw.githubusercontent.com/pola-rs/polars-static/master/sponsors/xomnia.png]]
+(https://www.xomnia.com/) &emsp; [[https://www.jetbrains.com/company/brand/img/
+jetbrains_logo.png]](https://www.jetbrains.com)
```

### Comparing `polars_u64_idx-0.18.3/build.rs` & `polars_u64_idx-0.18.4/build.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/docs/Makefile` & `polars_u64_idx-0.18.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/docs/_templates/autosummary/class.rst` & `polars_u64_idx-0.18.4/docs/_templates/autosummary/class.rst`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/docs/run_live_docs_server.py` & `polars_u64_idx-0.18.4/docs/run_live_docs_server.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/docs/source/_static/css/custom.css` & `polars_u64_idx-0.18.4/docs/source/_static/css/custom.css`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/docs/source/conf.py` & `polars_u64_idx-0.18.4/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/docs/source/reference/api.rst` & `polars_u64_idx-0.18.4/docs/source/reference/api.rst`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/docs/source/reference/config.rst` & `polars_u64_idx-0.18.4/docs/source/reference/config.rst`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/docs/source/reference/dataframe/modify_select.rst` & `polars_u64_idx-0.18.4/docs/source/reference/dataframe/modify_select.rst`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/docs/source/reference/datatypes.rst` & `polars_u64_idx-0.18.4/docs/source/reference/datatypes.rst`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/docs/source/reference/expressions/computation.rst` & `polars_u64_idx-0.18.4/docs/source/reference/expressions/computation.rst`

 * *Files 11% similar despite different names*

```diff
@@ -19,14 +19,15 @@
     Expr.cosh
     Expr.cumcount
     Expr.cummax
     Expr.cummin
     Expr.cumprod
     Expr.cumsum
     Expr.cumulative_eval
+    Expr.degrees
     Expr.diff
     Expr.dot
     Expr.entropy
     Expr.ewm_mean
     Expr.ewm_std
     Expr.ewm_var
     Expr.exp
@@ -35,14 +36,15 @@
     Expr.log
     Expr.log10
     Expr.log1p
     Expr.mode
     Expr.n_unique
     Expr.null_count
     Expr.pct_change
+    Expr.radians
     Expr.rank
     Expr.rolling_apply
     Expr.rolling_max
     Expr.rolling_mean
     Expr.rolling_median
     Expr.rolling_min
     Expr.rolling_quantile
```

### Comparing `polars_u64_idx-0.18.3/docs/source/reference/expressions/functions.rst` & `polars_u64_idx-0.18.4/docs/source/reference/expressions/functions.rst`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/docs/source/reference/expressions/list.rst` & `polars_u64_idx-0.18.4/docs/source/reference/expressions/list.rst`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/docs/source/reference/expressions/modify_select.rst` & `polars_u64_idx-0.18.4/docs/source/reference/expressions/modify_select.rst`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/docs/source/reference/expressions/operators.rst` & `polars_u64_idx-0.18.4/docs/source/reference/expressions/operators.rst`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/docs/source/reference/expressions/string.rst` & `polars_u64_idx-0.18.4/docs/source/reference/expressions/string.rst`

 * *Files 8% similar despite different names*

```diff
@@ -35,11 +35,12 @@
     Expr.str.starts_with
     Expr.str.strip
     Expr.str.strptime
     Expr.str.to_date
     Expr.str.to_datetime
     Expr.str.to_decimal
     Expr.str.to_lowercase
+    Expr.str.to_titlecase
     Expr.str.to_time
     Expr.str.to_uppercase
     Expr.str.zfill
     Expr.str.parse_int
```

### Comparing `polars_u64_idx-0.18.3/docs/source/reference/expressions/temporal.rst` & `polars_u64_idx-0.18.4/docs/source/reference/expressions/temporal.rst`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/docs/source/reference/functions.rst` & `polars_u64_idx-0.18.4/docs/source/reference/functions.rst`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/docs/source/reference/io.rst` & `polars_u64_idx-0.18.4/docs/source/reference/io.rst`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/docs/source/reference/lazyframe/modify_select.rst` & `polars_u64_idx-0.18.4/docs/source/reference/lazyframe/modify_select.rst`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/docs/source/reference/selectors.rst` & `polars_u64_idx-0.18.4/docs/source/reference/selectors.rst`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/docs/source/reference/series/computation.rst` & `polars_u64_idx-0.18.4/docs/source/reference/series/computation.rst`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/docs/source/reference/series/descriptive.rst` & `polars_u64_idx-0.18.4/docs/source/reference/series/descriptive.rst`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/docs/source/reference/series/list.rst` & `polars_u64_idx-0.18.4/docs/source/reference/series/list.rst`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/docs/source/reference/series/modify_select.rst` & `polars_u64_idx-0.18.4/docs/source/reference/series/modify_select.rst`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/docs/source/reference/series/string.rst` & `polars_u64_idx-0.18.4/docs/source/reference/series/string.rst`

 * *Files 1% similar despite different names*

```diff
@@ -36,10 +36,11 @@
     Series.str.strip
     Series.str.strptime
     Series.str.to_date
     Series.str.to_datetime
     Series.str.to_decimal
     Series.str.to_lowercase
     Series.str.to_time
+    Series.str.to_titlecase
     Series.str.to_uppercase
     Series.str.zfill
     Series.str.parse_int
```

### Comparing `polars_u64_idx-0.18.3/docs/source/reference/series/temporal.rst` & `polars_u64_idx-0.18.4/docs/source/reference/series/temporal.rst`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/docs/source/reference/testing.rst` & `polars_u64_idx-0.18.4/docs/source/reference/testing.rst`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/polars/__init__.py` & `polars_u64_idx-0.18.4/polars/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 import contextlib
 import os
 
 with contextlib.suppress(ImportError):  # Module not available when building docs
     # ensure the object constructor is known by polars
     # we set this once on import
-    from polars.polars import register_object_builder
 
-    register_object_builder()
+    # we also set other function pointers needed
+    # on the rust side. This function is highly
+    # unsafe and should only be called once.
+    from polars.polars import __register_startup_deps
+
+    __register_startup_deps()
 
 from polars import api
 from polars.config import Config
 from polars.convert import (
     from_arrow,
     from_dataframe,
     from_dict,
```

### Comparing `polars_u64_idx-0.18.3/polars/api.py` & `polars_u64_idx-0.18.4/polars/api.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/polars/config.py` & `polars_u64_idx-0.18.4/polars/config.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/polars/convert.py` & `polars_u64_idx-0.18.4/polars/convert.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/polars/dataframe/_html.py` & `polars_u64_idx-0.18.4/polars/dataframe/_html.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/polars/dataframe/frame.py` & `polars_u64_idx-0.18.4/polars/dataframe/frame.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,32 +30,23 @@
 from polars.dataframe._html import NotebookFormatter
 from polars.dataframe.groupby import DynamicGroupBy, GroupBy, RollingGroupBy
 from polars.datatypes import (
     FLOAT_DTYPES,
     INTEGER_DTYPES,
     N_INFER_DEFAULT,
     NUMERIC_DTYPES,
-    SIGNED_INTEGER_DTYPES,
     Boolean,
     Categorical,
     DataTypeClass,
     Float64,
-    Int8,
-    Int16,
-    Int32,
-    Int64,
     List,
     Null,
     Object,
     Struct,
     Time,
-    UInt8,
-    UInt16,
-    UInt32,
-    UInt64,
     Utf8,
     py_type_to_dtype,
     unpack_dtypes,
 )
 from polars.dependencies import (
     _PYARROW_AVAILABLE,
     _check_for_numpy,
@@ -81,24 +72,24 @@
 from polars.slice import PolarsSlice
 from polars.utils import no_default
 from polars.utils._construction import (
     _post_apply_columns,
     arrow_to_pydf,
     dict_to_pydf,
     iterable_to_pydf,
+    numpy_to_idxs,
     numpy_to_pydf,
     pandas_to_pydf,
     sequence_to_pydf,
     series_to_pydf,
 )
 from polars.utils._parse_expr_input import parse_as_expression
 from polars.utils._wrap import wrap_expr, wrap_ldf, wrap_s
 from polars.utils.convert import _timedelta_to_pl_duration
 from polars.utils.decorators import deprecated_alias
-from polars.utils.meta import get_index_type
 from polars.utils.various import (
     _prepare_row_count_args,
     _process_null_values,
     find_stacklevel,
     handle_projection_columns,
     is_bool_sequence,
     is_int_sequence,
@@ -1412,85 +1403,16 @@
 
     def _pos_idx(self, idx: int, dim: int) -> int:
         if idx >= 0:
             return idx
         else:
             return self.shape[dim] + idx
 
-    def _pos_idxs(self, idxs: np.ndarray[Any, Any] | Series, dim: int) -> Series:
-        # pl.UInt32 (polars) or pl.UInt64 (polars_u64_idx).
-        idx_type = get_index_type()
-
-        if isinstance(idxs, pl.Series):
-            if idxs.dtype == idx_type:
-                return idxs
-            if idxs.dtype in {
-                UInt8,
-                UInt16,
-                UInt64 if idx_type == UInt32 else UInt32,
-                Int8,
-                Int16,
-                Int32,
-                Int64,
-            }:
-                if idx_type == UInt32:
-                    if idxs.dtype in {Int64, UInt64}:
-                        if idxs.max() >= 2**32:  # type: ignore[operator]
-                            raise ValueError(
-                                "Index positions should be smaller than 2^32."
-                            )
-                    if idxs.dtype == Int64:
-                        if idxs.min() < -(2**32):  # type: ignore[operator]
-                            raise ValueError(
-                                "Index positions should be bigger than -2^32 + 1."
-                            )
-                if idxs.dtype in SIGNED_INTEGER_DTYPES:
-                    if idxs.min() < 0:  # type: ignore[operator]
-                        if idx_type == UInt32:
-                            if idxs.dtype in {Int8, Int16}:
-                                idxs = idxs.cast(Int32)
-                        else:
-                            if idxs.dtype in {Int8, Int16, Int32}:
-                                idxs = idxs.cast(Int64)
-
-                        idxs = F.select(
-                            F.when(lit(idxs) < 0)
-                            .then(self.shape[dim] + lit(idxs))
-                            .otherwise(lit(idxs))
-                        ).to_series()
-
-                return idxs.cast(idx_type)
-
-        if _check_for_numpy(idxs) and isinstance(idxs, np.ndarray):
-            if idxs.ndim != 1:
-                raise ValueError("Only 1D numpy array is supported as index.")
-            if idxs.dtype.kind in ("i", "u"):
-                # Numpy array with signed or unsigned integers.
-
-                if idx_type == UInt32:
-                    if idxs.dtype in {np.int64, np.uint64} and idxs.max() >= 2**32:
-                        raise ValueError("Index positions should be smaller than 2^32.")
-                    if idxs.dtype == np.int64 and idxs.min() < -(2**32):
-                        raise ValueError(
-                            "Index positions should be bigger than -2^32 + 1."
-                        )
-                if idxs.dtype.kind == "i" and idxs.min() < 0:
-                    if idx_type == UInt32:
-                        if idxs.dtype in (np.int8, np.int16):
-                            idxs = idxs.astype(np.int32)
-                    else:
-                        if idxs.dtype in (np.int8, np.int16, np.int32):
-                            idxs = idxs.astype(np.int64)
-
-                    # Update negative indexes to absolute indexes.
-                    idxs = np.where(idxs < 0, self.shape[dim] + idxs, idxs)
-
-                return pl.Series("", idxs, dtype=idx_type)
-
-        raise NotImplementedError("Unsupported idxs datatype.")
+    def _take_with_series(self, s: Series) -> DataFrame:
+        return self._from_pydf(self._df.take_with_series(s._s))
 
     @overload
     def __getitem__(self, item: str) -> Series:
         ...
 
     @overload
     def __getitem__(
@@ -1536,14 +1458,20 @@
             raise KeyError(item)
 
         # select rows and columns at once
         # every 2d selection, i.e. tuple is row column order, just like numpy
         if isinstance(item, tuple) and len(item) == 2:
             row_selection, col_selection = item
 
+            # df[[], :]
+            if isinstance(row_selection, Sequence):
+                if len(row_selection) == 0:
+                    # handle empty list by falling through to slice
+                    row_selection = slice(0)
+
             # df[:, unknown]
             if isinstance(row_selection, slice):
                 # multiple slices
                 # df[:, :]
                 if isinstance(col_selection, slice):
                     # slice can be
                     # by index
@@ -1644,37 +1572,31 @@
         # df[np.array([1, 2, 3])]
         # df[np.array([True, False, True])]
         if _check_for_numpy(item) and isinstance(item, np.ndarray):
             if item.ndim != 1:
                 raise ValueError("Only a 1D-Numpy array is supported as index.")
             if item.dtype.kind in ("i", "u"):
                 # Numpy array with signed or unsigned integers.
-                return self._from_pydf(
-                    self._df.take_with_series(self._pos_idxs(item, dim=0)._s)
-                )
+                return self._take_with_series(numpy_to_idxs(item, self.shape[0]))
             if isinstance(item[0], str):
                 return self._from_pydf(self._df.select(item))
 
         if is_str_sequence(item, allow_str=False):
             # select multiple columns
             # df[["foo", "bar"]]
             return self._from_pydf(self._df.select(item))
         elif is_int_sequence(item):
             item = pl.Series("", item)  # fall through to next if isinstance
 
         if isinstance(item, pl.Series):
             dtype = item.dtype
             if dtype == Utf8:
                 return self._from_pydf(self._df.select(item))
-            elif dtype == UInt32:
-                return self._from_pydf(self._df.take_with_series(item._s))
             elif dtype in INTEGER_DTYPES:
-                return self._from_pydf(
-                    self._df.take_with_series(self._pos_idxs(item, dim=0)._s)
-                )
+                return self._take_with_series(item._pos_idxs(self.shape[0]))
 
         # if no data has been returned, the operation is not supported
         raise ValueError(
             f"Cannot __getitem__ on DataFrame with item: '{item}'"
             f" of type: '{type(item)}'."
         )
 
@@ -4826,15 +4748,15 @@
             This column must be sorted in ascending order. If not the output will not
             make sense.
 
             In case of a rolling groupby on indices, dtype needs to be one of
             {Int32, Int64}. Note that Int32 gets temporarily cast to Int64, so if
             performance matters use an Int64 column.
         period
-            length of the window
+            length of the window - must be non-negative
         offset
             offset of the window. Default is -period
         closed : {'right', 'left', 'both', 'none'}
             Define which sides of the temporal interval are closed (inclusive).
         by
             Also group by this column/these columns
         check_sorted
@@ -6375,16 +6297,22 @@
             Column values to aggregate. Can be multiple columns if the *columns*
             arguments contains multiple columns as well.
         index
             One or multiple keys to group by.
         columns
             Name of the column(s) whose values will be used as the header of the output
             DataFrame.
-        aggregate_function : {'first', 'sum', 'max', 'min', 'mean', 'median', 'last', 'count'}
-            A predefined aggregate function str or an expression.
+        aggregate_function
+            Choose from:
+
+            - None: no aggregation takes place, will raise error if multiple values are in group.
+            - A predefined aggregate function string, one of
+              {'first', 'sum', 'max', 'min', 'mean', 'median', 'last', 'count'}
+            - An expression to do the aggregation.
+
         maintain_order
             Sort the grouped keys so that the output order is predictable.
         sort_columns
             Sort the transposed columns by name. Default is by order of discovery.
         separator
             Used as separator/delimiter in generated column names.
 
@@ -7047,15 +6975,15 @@
         ...     {
         ...         "a": [None, 2, 3, 4],
         ...         "b": [0.5, None, 2.5, 13],
         ...         "c": [True, True, False, None],
         ...     }
         ... )
         >>> df.lazy()  # doctest: +ELLIPSIS
-        <polars.LazyFrame object at ...>
+        <LazyFrame [3 cols, {"a": Int64 … "c": Boolean}] at ...>
 
         """
         return wrap_ldf(self._df.lazy())
 
     def select(
         self, *exprs: IntoExpr | Iterable[IntoExpr], **named_exprs: IntoExpr
     ) -> DataFrame:
@@ -7765,26 +7693,32 @@
         │ 2.0 ┆ 7.0 ┆ null │
         └─────┴─────┴──────┘
 
         """
         return self._from_pydf(self._df.quantile(quantile, interpolation))
 
     def to_dummies(
-        self, columns: str | Sequence[str] | None = None, *, separator: str = "_"
+        self,
+        columns: str | Sequence[str] | None = None,
+        *,
+        separator: str = "_",
+        drop_first: bool = False,
     ) -> Self:
         """
         Convert categorical variables into dummy/indicator variables.
 
         Parameters
         ----------
         columns
             Name of the column(s) that should be converted to dummy variables.
             If set to ``None`` (default), convert all columns.
         separator
             Separator/delimiter used when generating column names.
+        drop_first
+            Remove the first category from the variables being encoded.
 
         Examples
         --------
         >>> df = pl.DataFrame(
         ...     {
         ...         "foo": [1, 2],
         ...         "bar": [3, 4],
@@ -7801,15 +7735,15 @@
         │ 1     ┆ 0     ┆ 1     ┆ 0     ┆ 1     ┆ 0     │
         │ 0     ┆ 1     ┆ 0     ┆ 1     ┆ 0     ┆ 1     │
         └───────┴───────┴───────┴───────┴───────┴───────┘
 
         """
         if isinstance(columns, str):
             columns = [columns]
-        return self._from_pydf(self._df.to_dummies(columns, separator))
+        return self._from_pydf(self._df.to_dummies(columns, separator, drop_first))
 
     def unique(
         self,
         subset: str | Sequence[str] | None = None,
         *,
         keep: UniqueKeepStrategy = "any",
         maintain_order: bool = False,
```

### Comparing `polars_u64_idx-0.18.3/polars/dataframe/groupby.py` & `polars_u64_idx-0.18.4/polars/dataframe/groupby.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/polars/datatypes/__init__.py` & `polars_u64_idx-0.18.4/polars/datatypes/__init__.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/polars/datatypes/classes.py` & `polars_u64_idx-0.18.4/polars/datatypes/classes.py`

 * *Files 14% similar despite different names*

```diff
@@ -404,21 +404,40 @@
 
 
 class List(NestedType):
     inner: PolarsDataType | None = None
 
     def __init__(self, inner: PolarsDataType | PythonDataType):
         """
-        Nested list/array type.
+        Nested list/array type with variable length of inner lists.
 
         Parameters
         ----------
         inner
             The `DataType` of values within the list
 
+        Examples
+        --------
+        >>> df = pl.DataFrame(
+        ...     {
+        ...         "integer_lists": [[1, 2], [3, 4]],
+        ...         "float_lists": [[1.0, 2.0], [3.0, 4.0]],
+        ...     }
+        ... )
+        >>> df
+        shape: (2, 2)
+        ┌───────────────┬─────────────┐
+        │ integer_lists ┆ float_lists │
+        │ ---           ┆ ---         │
+        │ list[i64]     ┆ list[f64]   │
+        ╞═══════════════╪═════════════╡
+        │ [1, 2]        ┆ [1.0, 2.0]  │
+        │ [3, 4]        ┆ [3.0, 4.0]  │
+        └───────────────┴─────────────┘
+
         """
         self.inner = polars.datatypes.py_type_to_dtype(inner)
 
     def __eq__(self, other: PolarsDataType) -> bool:  # type: ignore[override]
         # This equality check allows comparison of type classes and type instances.
         # If a parent type is not specific about its inner type, we infer it as equal:
         # > list[i64] == list[i64] -> True
@@ -446,22 +465,35 @@
 
 class Array(NestedType):
     inner: PolarsDataType | None = None
     width: int
 
     def __init__(self, width: int, inner: PolarsDataType | PythonDataType = Null):
         """
-        Nested list/array type.
+        Nested list/array type with fixed length of inner arrays.
 
         Parameters
         ----------
         width
             The fixed size length of the inner arrays.
         inner
-            The `DataType` of values within the list
+            The `DataType` of values within the inner arrays
+
+        Examples
+        --------
+        >>> s = pl.Series(
+        ...     "a", [[1, 2], [4, 3]], dtype=pl.Array(width=2, inner=pl.Int64)
+        ... )
+        >>> s
+        shape: (2,)
+        Series: 'a' [array[i64, 2]]
+        [
+                [1, 2]
+                [4, 3]
+        ]
 
         """
         self.width = width
         self.inner = polars.datatypes.py_type_to_dtype(inner)
 
     def __eq__(self, other: PolarsDataType) -> bool:  # type: ignore[override]
         # This equality check allows comparison of type classes and type instances.
@@ -522,14 +554,28 @@
         Struct composite type.
 
         Parameters
         ----------
         fields
             The sequence of fields that make up the struct
 
+        Examples
+        --------
+        >>> s = pl.Series(
+        ...     "struct_series",
+        ...     [{"a": [1], "b": [2], "c": [3]}, {"a": [4], "b": [5], "c": [6]}],
+        ... )
+        >>> s
+        shape: (2,)
+        Series: 'struct_series' [struct[3]]
+        [
+                {[1],[2],[3]}
+                {[4],[5],[6]}
+        ]
+
         """
         if isinstance(fields, Mapping):
             self.fields = [Field(name, dtype) for name, dtype in fields.items()]
         else:
             self.fields = list(fields)
 
     def __eq__(self, other: PolarsDataType) -> bool:  # type: ignore[override]
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `polars_u64_idx-0.18.3/polars/datatypes/constants.py` & `polars_u64_idx-0.18.4/polars/datatypes/constants.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/polars/datatypes/constructor.py` & `polars_u64_idx-0.18.4/polars/datatypes/constructor.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/polars/datatypes/convert.py` & `polars_u64_idx-0.18.4/polars/datatypes/convert.py`

 * *Files 1% similar despite different names*

```diff
@@ -397,15 +397,15 @@
 def py_type_to_dtype(
     data_type: Any, raise_unmatched: Literal[False]
 ) -> PolarsDataType | None:
     ...
 
 
 def py_type_to_dtype(
-    data_type: Any, raise_unmatched: bool = True
+    data_type: Any, raise_unmatched: bool = True, allow_strings: bool = False
 ) -> PolarsDataType | None:
     """Convert a Python dtype (or type annotation) to a Polars dtype."""
     if isinstance(data_type, ForwardRef):
         annotation = data_type.__forward_arg__
         data_type = (
             PY_STR_TO_DTYPE.get(
                 re.sub(r"(^None \|)|(\| None$)", "", annotation).strip(), data_type
@@ -422,15 +422,15 @@
     elif isinstance(data_type, (OptionType, UnionType)):
         # not exhaustive; handles the common "type | None" case, but
         # should probably pick appropriate supertype when n_types > 1?
         possible_types = [tp for tp in get_args(data_type) if tp is not NoneType]
         if len(possible_types) == 1:
             data_type = possible_types[0]
 
-    elif isinstance(data_type, str):
+    elif allow_strings and isinstance(data_type, str):
         data_type = DataTypeMappings.REPR_TO_DTYPE.get(
             re.sub(r"^(?:dataclasses\.)?InitVar\[(.+)\]$", r"\1", data_type),
             data_type,
         )
         if is_polars_dtype(data_type):
             return data_type
     try:
```

### Comparing `polars_u64_idx-0.18.3/polars/dependencies.py` & `polars_u64_idx-0.18.4/polars/dependencies.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/polars/exceptions.py` & `polars_u64_idx-0.18.4/polars/exceptions.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/polars/expr/array.py` & `polars_u64_idx-0.18.4/polars/expr/array.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/polars/expr/binary.py` & `polars_u64_idx-0.18.4/polars/expr/binary.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/polars/expr/categorical.py` & `polars_u64_idx-0.18.4/polars/expr/categorical.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/polars/expr/datetime.py` & `polars_u64_idx-0.18.4/polars/expr/datetime.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/polars/expr/expr.py` & `polars_u64_idx-0.18.4/polars/expr/expr.py`

 * *Files 12% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 from polars.expr.string import ExprStringNameSpace
 from polars.expr.struct import ExprStructNameSpace
 from polars.utils._parse_expr_input import (
     parse_as_expression,
     parse_as_list_of_expressions,
 )
 from polars.utils.convert import _timedelta_to_pl_duration
-from polars.utils.decorators import deprecated_alias
+from polars.utils.decorators import deprecated_alias, warn_closed_future_change
 from polars.utils.meta import threadpool_size
 from polars.utils.various import sphinx_accessor
 
 with contextlib.suppress(ImportError):  # Module not available when building docs
     from polars.polars import arg_where as py_arg_where
     from polars.polars import reduce as pyreduce
 
@@ -2322,14 +2322,15 @@
         strategy: FillNullStrategy | None = None,
         limit: int | None = None,
     ) -> Self:
         """
         Fill null values using the specified value or strategy.
 
         To interpolate over null values see interpolate.
+        See the examples below to fill nulls with an expression.
 
         Parameters
         ----------
         value
             Value used to fill null values.
         strategy : {None, 'forward', 'backward', 'min', 'max', 'mean', 'zero', 'one'}
             Strategy used to fill null values.
@@ -2341,46 +2342,68 @@
         --------
         >>> df = pl.DataFrame(
         ...     {
         ...         "a": [1, 2, None],
         ...         "b": [4, None, 6],
         ...     }
         ... )
-        >>> df.fill_null(strategy="zero")
+        >>> df.with_columns(pl.col("b").fill_null(strategy="zero"))
         shape: (3, 2)
-        ┌─────┬─────┐
-        │ a   ┆ b   │
-        │ --- ┆ --- │
-        │ i64 ┆ i64 │
-        ╞═════╪═════╡
-        │ 1   ┆ 4   │
-        │ 2   ┆ 0   │
-        │ 0   ┆ 6   │
-        └─────┴─────┘
-        >>> df.fill_null(99)
+        ┌──────┬─────┐
+        │ a    ┆ b   │
+        │ ---  ┆ --- │
+        │ i64  ┆ i64 │
+        ╞══════╪═════╡
+        │ 1    ┆ 4   │
+        │ 2    ┆ 0   │
+        │ null ┆ 6   │
+        └──────┴─────┘
+        >>> df.with_columns(pl.col("b").fill_null(99))
         shape: (3, 2)
-        ┌─────┬─────┐
-        │ a   ┆ b   │
-        │ --- ┆ --- │
-        │ i64 ┆ i64 │
-        ╞═════╪═════╡
-        │ 1   ┆ 4   │
-        │ 2   ┆ 99  │
-        │ 99  ┆ 6   │
-        └─────┴─────┘
-        >>> df.fill_null(strategy="forward")
+        ┌──────┬─────┐
+        │ a    ┆ b   │
+        │ ---  ┆ --- │
+        │ i64  ┆ i64 │
+        ╞══════╪═════╡
+        │ 1    ┆ 4   │
+        │ 2    ┆ 99  │
+        │ null ┆ 6   │
+        └──────┴─────┘
+        >>> df.with_columns(pl.col("b").fill_null(strategy="forward"))
+        shape: (3, 2)
+        ┌──────┬─────┐
+        │ a    ┆ b   │
+        │ ---  ┆ --- │
+        │ i64  ┆ i64 │
+        ╞══════╪═════╡
+        │ 1    ┆ 4   │
+        │ 2    ┆ 4   │
+        │ null ┆ 6   │
+        └──────┴─────┘
+        >>> df.with_columns(pl.col("b").fill_null(pl.col("b").median()))
+        shape: (3, 2)
+        ┌──────┬─────┐
+        │ a    ┆ b   │
+        │ ---  ┆ --- │
+        │ i64  ┆ f64 │
+        ╞══════╪═════╡
+        │ 1    ┆ 4.0 │
+        │ 2    ┆ 5.0 │
+        │ null ┆ 6.0 │
+        └──────┴─────┘
+        >>> df.with_columns(pl.all().fill_null(pl.all().median()))
         shape: (3, 2)
         ┌─────┬─────┐
         │ a   ┆ b   │
         │ --- ┆ --- │
-        │ i64 ┆ i64 │
+        │ f64 ┆ f64 │
         ╞═════╪═════╡
-        │ 1   ┆ 4   │
-        │ 2   ┆ 4   │
-        │ 2   ┆ 6   │
+        │ 1.0 ┆ 4.0 │
+        │ 2.0 ┆ 5.0 │
+        │ 1.5 ┆ 6.0 │
         └─────┴─────┘
 
         """
         if value is not None and strategy is not None:
             raise ValueError("cannot specify both 'value' and 'strategy'.")
         elif value is None and strategy is None:
             raise ValueError("must specify either a fill 'value' or 'strategy'")
@@ -2406,25 +2429,25 @@
         --------
         >>> df = pl.DataFrame(
         ...     {
         ...         "a": [1.0, None, float("nan")],
         ...         "b": [4.0, float("nan"), 6],
         ...     }
         ... )
-        >>> df.fill_nan("zero")
+        >>> df.with_columns(pl.col("b").fill_nan(0))
         shape: (3, 2)
-        ┌──────┬──────┐
-        │ a    ┆ b    │
-        │ ---  ┆ ---  │
-        │ str  ┆ str  │
-        ╞══════╪══════╡
-        │ 1.0  ┆ 4.0  │
-        │ null ┆ zero │
-        │ zero ┆ 6.0  │
-        └──────┴──────┘
+        ┌──────┬─────┐
+        │ a    ┆ b   │
+        │ ---  ┆ --- │
+        │ f64  ┆ f64 │
+        ╞══════╪═════╡
+        │ 1.0  ┆ 4.0 │
+        │ null ┆ 0.0 │
+        │ NaN  ┆ 6.0 │
+        └──────┴─────┘
 
         """
         fill_value = parse_as_expression(value, str_as_lit=True)
         return self._from_pyexpr(self._pyexpr.fill_nan(fill_value))
 
     def forward_fill(self, limit: int | None = None) -> Self:
         """
@@ -2469,27 +2492,39 @@
 
         Examples
         --------
         >>> df = pl.DataFrame(
         ...     {
         ...         "a": [1, 2, None],
         ...         "b": [4, None, 6],
+        ...         "c": [None, None, 2],
         ...     }
         ... )
         >>> df.select(pl.all().backward_fill())
-        shape: (3, 2)
-        ┌──────┬─────┐
-        │ a    ┆ b   │
-        │ ---  ┆ --- │
-        │ i64  ┆ i64 │
-        ╞══════╪═════╡
-        │ 1    ┆ 4   │
-        │ 2    ┆ 6   │
-        │ null ┆ 6   │
-        └──────┴─────┘
+        shape: (3, 3)
+        ┌──────┬─────┬─────┐
+        │ a    ┆ b   ┆ c   │
+        │ ---  ┆ --- ┆ --- │
+        │ i64  ┆ i64 ┆ i64 │
+        ╞══════╪═════╪═════╡
+        │ 1    ┆ 4   ┆ 2   │
+        │ 2    ┆ 6   ┆ 2   │
+        │ null ┆ 6   ┆ 2   │
+        └──────┴─────┴─────┘
+        >>> df.select(pl.all().backward_fill(limit=1))
+        shape: (3, 3)
+        ┌──────┬─────┬──────┐
+        │ a    ┆ b   ┆ c    │
+        │ ---  ┆ --- ┆ ---  │
+        │ i64  ┆ i64 ┆ i64  │
+        ╞══════╪═════╪══════╡
+        │ 1    ┆ 4   ┆ null │
+        │ 2    ┆ 6   ┆ 2    │
+        │ null ┆ 6   ┆ 2    │
+        └──────┴─────┴──────┘
 
         """
         return self._from_pyexpr(self._pyexpr.backward_fill(limit))
 
     def reverse(self) -> Self:
         """
         Reverse the selection.
@@ -3536,14 +3571,38 @@
         Exploded Series of same dtype
 
         See Also
         --------
         ExprListNameSpace.explode : Explode a list column.
         ExprStringNameSpace.explode : Explode a string column.
 
+        Examples
+        --------
+        >>> df = pl.DataFrame(
+        ...     {
+        ...         "group": ["a", "b"],
+        ...         "values": [
+        ...             [1, 2],
+        ...             [3, 4],
+        ...         ],
+        ...     }
+        ... )
+        >>> df.select(pl.col("values").explode())
+        shape: (4, 1)
+        ┌────────┐
+        │ values │
+        │ ---    │
+        │ i64    │
+        ╞════════╡
+        │ 1      │
+        │ 2      │
+        │ 3      │
+        │ 4      │
+        └────────┘
+
         """
         return self._from_pyexpr(self._pyexpr.explode())
 
     def implode(self) -> Self:
         """
         Aggregate values into a list.
 
@@ -3801,14 +3860,39 @@
         This differs from default ``eq`` where null values are propagated.
 
         Parameters
         ----------
         other
             A literal or expression value to compare with.
 
+        Examples
+        --------
+        >>> df = pl.DataFrame(
+        ...     data={
+        ...         "x": [1.0, 2.0, float("nan"), 4.0, None, None],
+        ...         "y": [2.0, 2.0, float("nan"), 4.0, 5.0, None],
+        ...     }
+        ... )
+        >>> df.with_columns(
+        ...     pl.col("x").eq_missing(pl.col("y")).alias("x == y"),
+        ... )
+        shape: (6, 3)
+        ┌──────┬──────┬────────┐
+        │ x    ┆ y    ┆ x == y │
+        │ ---  ┆ ---  ┆ ---    │
+        │ f64  ┆ f64  ┆ bool   │
+        ╞══════╪══════╪════════╡
+        │ 1.0  ┆ 2.0  ┆ false  │
+        │ 2.0  ┆ 2.0  ┆ true   │
+        │ NaN  ┆ NaN  ┆ false  │
+        │ 4.0  ┆ 4.0  ┆ true   │
+        │ null ┆ 5.0  ┆ false  │
+        │ null ┆ null ┆ true   │
+        └──────┴──────┴────────┘
+
         """
         return self._from_pyexpr(self._pyexpr.eq_missing(self._to_expr(other)._pyexpr))
 
     def ge(self, other: Any) -> Self:
         """
         Method equivalent of "greater than or equal" operator ``expr >= other``.
 
@@ -3990,14 +4074,39 @@
         This differs from default ``ne`` where null values are propagated.
 
         Parameters
         ----------
         other
             A literal or expression value to compare with.
 
+        Examples
+        --------
+        >>> df = pl.DataFrame(
+        ...     data={
+        ...         "x": [1.0, 2.0, float("nan"), 4.0, None, None],
+        ...         "y": [2.0, 2.0, float("nan"), 4.0, 5.0, None],
+        ...     }
+        ... )
+        >>> df.with_columns(
+        ...     pl.col("x").ne_missing(pl.col("y")).alias("x != y"),
+        ... )
+        shape: (6, 3)
+        ┌──────┬──────┬────────┐
+        │ x    ┆ y    ┆ x != y │
+        │ ---  ┆ ---  ┆ ---    │
+        │ f64  ┆ f64  ┆ bool   │
+        ╞══════╪══════╪════════╡
+        │ 1.0  ┆ 2.0  ┆ true   │
+        │ 2.0  ┆ 2.0  ┆ false  │
+        │ NaN  ┆ NaN  ┆ true   │
+        │ 4.0  ┆ 4.0  ┆ false  │
+        │ null ┆ 5.0  ┆ true   │
+        │ null ┆ null ┆ false  │
+        └──────┴──────┴────────┘
+
         """
         return self._from_pyexpr(self._pyexpr.neq_missing(self._to_expr(other)._pyexpr))
 
     def add(self, other: Any) -> Self:
         """
         Method equivalent of addition operator ``expr + other``.
 
@@ -4663,14 +4772,15 @@
         │ 9           ┆ 18.0   │
         │ 10          ┆ 20.0   │
         └─────────────┴────────┘
 
         """
         return self._from_pyexpr(self._pyexpr.interpolate(method))
 
+    @warn_closed_future_change()
     def rolling_min(
         self,
         window_size: int | timedelta | str,
         weights: list[float] | None = None,
         min_periods: int | None = None,
         *,
         center: bool = False,
@@ -4680,30 +4790,33 @@
         """
         Apply a rolling min (moving min) over the values in this array.
 
         A window of length `window_size` will traverse the array. The values that fill
         this window will (optionally) be multiplied with the weights given by the
         `weight` vector. The resulting values will be aggregated to their sum.
 
-        If you pass a ``by`` column ``<t_0, t_1, ..., t_2>``, then by default the
-        windows will be:
+        If ``by`` has not been specified (the default), the window at a given row will
+        include the row itself, and the `window_size - 1` elements before it.
+
+        If you pass a ``by`` column ``<t_0, t_1, ..., t_n>``, then `closed="left"`
+        means the windows will be:
 
             - [t_0 - window_size, t_0)
             - [t_1 - window_size, t_1)
             - ...
             - [t_n - window_size, t_n)
 
-        Otherwise, the window at a given row will include the row itself, and the
-        `window_size - 1` elements before it.
+        With `closed="right"`, the left endpoint is not included and the right
+        endpoint is included.
 
         Parameters
         ----------
         window_size
-            The length of the window. Can be a fixed integer size, or a dynamic temporal
-            size indicated by a timedelta or the following string language:
+            The length of the window. Can be a fixed integer size, or a dynamic
+            temporal size indicated by a timedelta or the following string language:
 
             - 1ns   (1 nanosecond)
             - 1us   (1 microsecond)
             - 1ms   (1 millisecond)
             - 1s    (1 second)
             - 1m    (1 minute)
             - 1h    (1 hour)
@@ -4729,15 +4842,16 @@
         center
             Set the labels at the center of the window
         by
             If the `window_size` is temporal for instance `"5h"` or `"3s"`, you must
             set the column that will be used to determine the windows. This column must
             be of dtype Datetime.
         closed : {'left', 'right', 'both', 'none'}
-            Define which sides of the temporal interval are closed (inclusive).
+            Define which sides of the temporal interval are closed (inclusive); only
+            applicable if `by` has been set.
 
         Warnings
         --------
         This functionality is experimental and may change without it being considered a
         breaking change.
 
         Notes
@@ -4745,43 +4859,129 @@
         If you want to compute multiple aggregation statistics over the same dynamic
         window, consider using `groupby_rolling` this method can cache the window size
         computation.
 
         Examples
         --------
         >>> df = pl.DataFrame({"A": [1.0, 2.0, 3.0, 4.0, 5.0, 6.0]})
-        >>> df.select(
-        ...     [
-        ...         pl.col("A").rolling_min(window_size=2),
-        ...     ]
+        >>> df.with_columns(
+        ...     rolling_min=pl.col("A").rolling_min(window_size=2),
         ... )
-        shape: (6, 1)
-        ┌──────┐
-        │ A    │
-        │ ---  │
-        │ f64  │
-        ╞══════╡
-        │ null │
-        │ 1.0  │
-        │ 2.0  │
-        │ 3.0  │
-        │ 4.0  │
-        │ 5.0  │
-        └──────┘
+        shape: (6, 2)
+        ┌─────┬─────────────┐
+        │ A   ┆ rolling_min │
+        │ --- ┆ ---         │
+        │ f64 ┆ f64         │
+        ╞═════╪═════════════╡
+        │ 1.0 ┆ null        │
+        │ 2.0 ┆ 1.0         │
+        │ 3.0 ┆ 2.0         │
+        │ 4.0 ┆ 3.0         │
+        │ 5.0 ┆ 4.0         │
+        │ 6.0 ┆ 5.0         │
+        └─────┴─────────────┘
+
+        Specify weights to multiply the values in the window with:
+
+        >>> df.with_columns(
+        ...     rolling_min=pl.col("A").rolling_min(
+        ...         window_size=2, weights=[0.25, 0.75]
+        ...     ),
+        ... )
+        shape: (6, 2)
+        ┌─────┬─────────────┐
+        │ A   ┆ rolling_min │
+        │ --- ┆ ---         │
+        │ f64 ┆ f64         │
+        ╞═════╪═════════════╡
+        │ 1.0 ┆ null        │
+        │ 2.0 ┆ 0.25        │
+        │ 3.0 ┆ 0.5         │
+        │ 4.0 ┆ 0.75        │
+        │ 5.0 ┆ 1.0         │
+        │ 6.0 ┆ 1.25        │
+        └─────┴─────────────┘
+
+        Center the values in the window
+
+        >>> df.with_columns(
+        ...     rolling_min=pl.col("A").rolling_min(window_size=3, center=True),
+        ... )
+        shape: (6, 2)
+        ┌─────┬─────────────┐
+        │ A   ┆ rolling_min │
+        │ --- ┆ ---         │
+        │ f64 ┆ f64         │
+        ╞═════╪═════════════╡
+        │ 1.0 ┆ null        │
+        │ 2.0 ┆ 1.0         │
+        │ 3.0 ┆ 2.0         │
+        │ 4.0 ┆ 3.0         │
+        │ 5.0 ┆ 4.0         │
+        │ 6.0 ┆ null        │
+        └─────┴─────────────┘
+
+        Create a DataFrame with a datetime column and a row number column
+
+        >>> from datetime import timedelta, datetime
+        >>> start = datetime(2001, 1, 1)
+        >>> stop = datetime(2001, 1, 2)
+        >>> df_temporal = pl.DataFrame(
+        ...     {"date": pl.date_range(start, stop, "1h", eager=True)}
+        ... ).with_row_count()
+        >>> df_temporal
+        shape: (25, 2)
+        ┌────────┬─────────────────────┐
+        │ row_nr ┆ date                │
+        │ ---    ┆ ---                 │
+        │ u32    ┆ datetime[μs]        │
+        ╞════════╪═════════════════════╡
+        │ 0      ┆ 2001-01-01 00:00:00 │
+        │ 1      ┆ 2001-01-01 01:00:00 │
+        │ 2      ┆ 2001-01-01 02:00:00 │
+        │ 3      ┆ 2001-01-01 03:00:00 │
+        │ …      ┆ …                   │
+        │ 21     ┆ 2001-01-01 21:00:00 │
+        │ 22     ┆ 2001-01-01 22:00:00 │
+        │ 23     ┆ 2001-01-01 23:00:00 │
+        │ 24     ┆ 2001-01-02 00:00:00 │
+        └────────┴─────────────────────┘
+        >>> df_temporal.with_columns(
+        ...     rolling_row_min=pl.col("row_nr").rolling_min(
+        ...         window_size="2h", by="date"
+        ...     )
+        ... )
+        shape: (25, 3)
+        ┌────────┬─────────────────────┬─────────────────┐
+        │ row_nr ┆ date                ┆ rolling_row_min │
+        │ ---    ┆ ---                 ┆ ---             │
+        │ u32    ┆ datetime[μs]        ┆ u32             │
+        ╞════════╪═════════════════════╪═════════════════╡
+        │ 0      ┆ 2001-01-01 00:00:00 ┆ null            │
+        │ 1      ┆ 2001-01-01 01:00:00 ┆ 0               │
+        │ 2      ┆ 2001-01-01 02:00:00 ┆ 0               │
+        │ 3      ┆ 2001-01-01 03:00:00 ┆ 1               │
+        │ …      ┆ …                   ┆ …               │
+        │ 21     ┆ 2001-01-01 21:00:00 ┆ 19              │
+        │ 22     ┆ 2001-01-01 22:00:00 ┆ 20              │
+        │ 23     ┆ 2001-01-01 23:00:00 ┆ 21              │
+        │ 24     ┆ 2001-01-02 00:00:00 ┆ 22              │
+        └────────┴─────────────────────┴─────────────────┘
 
         """
         window_size, min_periods = _prepare_rolling_window_args(
             window_size, min_periods
         )
         return self._from_pyexpr(
             self._pyexpr.rolling_min(
                 window_size, weights, min_periods, center, by, closed
             )
         )
 
+    @warn_closed_future_change()
     def rolling_max(
         self,
         window_size: int | timedelta | str,
         weights: list[float] | None = None,
         min_periods: int | None = None,
         *,
         center: bool = False,
@@ -4791,24 +4991,27 @@
         """
         Apply a rolling max (moving max) over the values in this array.
 
         A window of length `window_size` will traverse the array. The values that fill
         this window will (optionally) be multiplied with the weights given by the
         `weight` vector. The resulting values will be aggregated to their sum.
 
-        If you pass a ``by`` column ``<t_0, t_1, ..., t_2>``, then by default the
-        windows will be:
+        If ``by`` has not been specified (the default), the window at a given row will
+        include the row itself, and the `window_size - 1` elements before it.
+
+        If you pass a ``by`` column ``<t_0, t_1, ..., t_n>``, then `closed="left"`
+        means the windows will be:
 
             - [t_0 - window_size, t_0)
             - [t_1 - window_size, t_1)
             - ...
             - [t_n - window_size, t_n)
 
-        Otherwise, the window at a given row will include the row itself, and the
-        `window_size - 1` elements before it.
+        With `closed="right"`, the left endpoint is not included and the right
+        endpoint is included.
 
         Parameters
         ----------
         window_size
             The length of the window. Can be a fixed integer size, or a dynamic temporal
             size indicated by a timedelta or the following string language:
 
@@ -4840,15 +5043,16 @@
         center
             Set the labels at the center of the window
         by
             If the `window_size` is temporal, for instance `"5h"` or `"3s"`, you must
             set the column that will be used to determine the windows. This column must
             be of dtype Datetime.
         closed : {'left', 'right', 'both', 'none'}
-            Define which sides of the temporal interval are closed (inclusive).
+            Define which sides of the temporal interval are closed (inclusive); only
+            applicable if `by` has been set.
 
         Warnings
         --------
         This functionality is experimental and may change without it being considered a
         breaking change.
 
         Notes
@@ -4856,43 +5060,156 @@
         If you want to compute multiple aggregation statistics over the same dynamic
         window, consider using `groupby_rolling` this method can cache the window size
         computation.
 
         Examples
         --------
         >>> df = pl.DataFrame({"A": [1.0, 2.0, 3.0, 4.0, 5.0, 6.0]})
-        >>> df.select(
-        ...     [
-        ...         pl.col("A").rolling_max(window_size=2),
-        ...     ]
+        >>> df.with_columns(
+        ...     rolling_max=pl.col("A").rolling_max(window_size=2),
         ... )
-        shape: (6, 1)
-        ┌──────┐
-        │ A    │
-        │ ---  │
-        │ f64  │
-        ╞══════╡
-        │ null │
-        │ 2.0  │
-        │ 3.0  │
-        │ 4.0  │
-        │ 5.0  │
-        │ 6.0  │
-        └──────┘
+        shape: (6, 2)
+        ┌─────┬─────────────┐
+        │ A   ┆ rolling_max │
+        │ --- ┆ ---         │
+        │ f64 ┆ f64         │
+        ╞═════╪═════════════╡
+        │ 1.0 ┆ null        │
+        │ 2.0 ┆ 2.0         │
+        │ 3.0 ┆ 3.0         │
+        │ 4.0 ┆ 4.0         │
+        │ 5.0 ┆ 5.0         │
+        │ 6.0 ┆ 6.0         │
+        └─────┴─────────────┘
+
+        Specify weights to multiply the values in the window with:
+
+        >>> df.with_columns(
+        ...     rolling_max=pl.col("A").rolling_max(
+        ...         window_size=2, weights=[0.25, 0.75]
+        ...     ),
+        ... )
+        shape: (6, 2)
+        ┌─────┬─────────────┐
+        │ A   ┆ rolling_max │
+        │ --- ┆ ---         │
+        │ f64 ┆ f64         │
+        ╞═════╪═════════════╡
+        │ 1.0 ┆ null        │
+        │ 2.0 ┆ 1.5         │
+        │ 3.0 ┆ 2.25        │
+        │ 4.0 ┆ 3.0         │
+        │ 5.0 ┆ 3.75        │
+        │ 6.0 ┆ 4.5         │
+        └─────┴─────────────┘
+
+        Center the values in the window
+
+        >>> df.with_columns(
+        ...     rolling_max=pl.col("A").rolling_max(window_size=3, center=True),
+        ... )
+        shape: (6, 2)
+        ┌─────┬─────────────┐
+        │ A   ┆ rolling_max │
+        │ --- ┆ ---         │
+        │ f64 ┆ f64         │
+        ╞═════╪═════════════╡
+        │ 1.0 ┆ null        │
+        │ 2.0 ┆ 3.0         │
+        │ 3.0 ┆ 4.0         │
+        │ 4.0 ┆ 5.0         │
+        │ 5.0 ┆ 6.0         │
+        │ 6.0 ┆ null        │
+        └─────┴─────────────┘
+
+        Create a DataFrame with a datetime column and a row number column
+
+        >>> from datetime import timedelta, datetime
+        >>> start = datetime(2001, 1, 1)
+        >>> stop = datetime(2001, 1, 2)
+        >>> df_temporal = pl.DataFrame(
+        ...     {"date": pl.date_range(start, stop, "1h", eager=True)}
+        ... ).with_row_count()
+        >>> df_temporal
+        shape: (25, 2)
+        ┌────────┬─────────────────────┐
+        │ row_nr ┆ date                │
+        │ ---    ┆ ---                 │
+        │ u32    ┆ datetime[μs]        │
+        ╞════════╪═════════════════════╡
+        │ 0      ┆ 2001-01-01 00:00:00 │
+        │ 1      ┆ 2001-01-01 01:00:00 │
+        │ 2      ┆ 2001-01-01 02:00:00 │
+        │ 3      ┆ 2001-01-01 03:00:00 │
+        │ …      ┆ …                   │
+        │ 21     ┆ 2001-01-01 21:00:00 │
+        │ 22     ┆ 2001-01-01 22:00:00 │
+        │ 23     ┆ 2001-01-01 23:00:00 │
+        │ 24     ┆ 2001-01-02 00:00:00 │
+        └────────┴─────────────────────┘
+
+        Compute the rolling max with the default left closure of temporal windows
+
+        >>> df_temporal.with_columns(
+        ...     rolling_row_max=pl.col("row_nr").rolling_max(
+        ...         window_size="2h", by="date"
+        ...     )
+        ... )
+        shape: (25, 3)
+        ┌────────┬─────────────────────┬─────────────────┐
+        │ row_nr ┆ date                ┆ rolling_row_max │
+        │ ---    ┆ ---                 ┆ ---             │
+        │ u32    ┆ datetime[μs]        ┆ u32             │
+        ╞════════╪═════════════════════╪═════════════════╡
+        │ 0      ┆ 2001-01-01 00:00:00 ┆ null            │
+        │ 1      ┆ 2001-01-01 01:00:00 ┆ 0               │
+        │ 2      ┆ 2001-01-01 02:00:00 ┆ 1               │
+        │ 3      ┆ 2001-01-01 03:00:00 ┆ 2               │
+        │ …      ┆ …                   ┆ …               │
+        │ 21     ┆ 2001-01-01 21:00:00 ┆ 20              │
+        │ 22     ┆ 2001-01-01 22:00:00 ┆ 21              │
+        │ 23     ┆ 2001-01-01 23:00:00 ┆ 22              │
+        │ 24     ┆ 2001-01-02 00:00:00 ┆ 23              │
+        └────────┴─────────────────────┴─────────────────┘
+
+        Compute the rolling max with the closure of windows on both sides
+
+        >>> df_temporal.with_columns(
+        ...     rolling_row_max=pl.col("row_nr").rolling_max(
+        ...         window_size="2h", by="date", closed="both"
+        ...     )
+        ... )
+        shape: (25, 3)
+        ┌────────┬─────────────────────┬─────────────────┐
+        │ row_nr ┆ date                ┆ rolling_row_max │
+        │ ---    ┆ ---                 ┆ ---             │
+        │ u32    ┆ datetime[μs]        ┆ u32             │
+        ╞════════╪═════════════════════╪═════════════════╡
+        │ 0      ┆ 2001-01-01 00:00:00 ┆ 0               │
+        │ 1      ┆ 2001-01-01 01:00:00 ┆ 1               │
+        │ 2      ┆ 2001-01-01 02:00:00 ┆ 2               │
+        │ 3      ┆ 2001-01-01 03:00:00 ┆ 3               │
+        │ …      ┆ …                   ┆ …               │
+        │ 21     ┆ 2001-01-01 21:00:00 ┆ 21              │
+        │ 22     ┆ 2001-01-01 22:00:00 ┆ 22              │
+        │ 23     ┆ 2001-01-01 23:00:00 ┆ 23              │
+        │ 24     ┆ 2001-01-02 00:00:00 ┆ 24              │
+        └────────┴─────────────────────┴─────────────────┘
 
         """
         window_size, min_periods = _prepare_rolling_window_args(
             window_size, min_periods
         )
         return self._from_pyexpr(
             self._pyexpr.rolling_max(
                 window_size, weights, min_periods, center, by, closed
             )
         )
 
+    @warn_closed_future_change()
     def rolling_mean(
         self,
         window_size: int | timedelta | str,
         weights: list[float] | None = None,
         min_periods: int | None = None,
         *,
         center: bool = False,
@@ -4902,24 +5219,27 @@
         """
         Apply a rolling mean (moving mean) over the values in this array.
 
         A window of length `window_size` will traverse the array. The values that fill
         this window will (optionally) be multiplied with the weights given by the
         `weight` vector. The resulting values will be aggregated to their sum.
 
-        If you pass a ``by`` column ``<t_0, t_1, ..., t_2>``, then by default the
-        windows will be:
+        If ``by`` has not been specified (the default), the window at a given row will
+        include the row itself, and the `window_size - 1` elements before it.
+
+        If you pass a ``by`` column ``<t_0, t_1, ..., t_n>``, then `closed="left"`
+        means the windows will be:
 
             - [t_0 - window_size, t_0)
             - [t_1 - window_size, t_1)
             - ...
             - [t_n - window_size, t_n)
 
-        Otherwise, the window at a given row will include the row itself, and the
-        `window_size - 1` elements before it.
+        With `closed="right"`, the left endpoint is not included and the right
+        endpoint is included.
 
         Parameters
         ----------
         window_size
             The length of the window. Can be a fixed integer size, or a dynamic temporal
             size indicated by a timedelta or the following string language:
 
@@ -4951,59 +5271,173 @@
         center
             Set the labels at the center of the window
         by
             If the `window_size` is temporal for instance `"5h"` or `"3s"`, you must
             set the column that will be used to determine the windows. This column must
             be of dtype Datetime.
         closed : {'left', 'right', 'both', 'none'}
-            Define which sides of the temporal interval are closed (inclusive).
+            Define which sides of the temporal interval are closed (inclusive); only
+            applicable if `by` has been set.
 
         Warnings
         --------
         This functionality is experimental and may change without it being considered a
         breaking change.
 
         Notes
         -----
         If you want to compute multiple aggregation statistics over the same dynamic
         window, consider using `groupby_rolling` this method can cache the window size
         computation.
 
         Examples
         --------
-        >>> df = pl.DataFrame({"A": [1.0, 8.0, 6.0, 2.0, 16.0, 10.0]})
-        >>> df.select(
-        ...     [
-        ...         pl.col("A").rolling_mean(window_size=2),
-        ...     ]
+        >>> df = pl.DataFrame({"A": [1.0, 2.0, 3.0, 4.0, 5.0, 6.0]})
+        >>> df.with_columns(
+        ...     rolling_mean=pl.col("A").rolling_mean(window_size=2),
         ... )
-        shape: (6, 1)
-        ┌──────┐
-        │ A    │
-        │ ---  │
-        │ f64  │
-        ╞══════╡
-        │ null │
-        │ 4.5  │
-        │ 7.0  │
-        │ 4.0  │
-        │ 9.0  │
-        │ 13.0 │
-        └──────┘
+        shape: (6, 2)
+        ┌─────┬──────────────┐
+        │ A   ┆ rolling_mean │
+        │ --- ┆ ---          │
+        │ f64 ┆ f64          │
+        ╞═════╪══════════════╡
+        │ 1.0 ┆ null         │
+        │ 2.0 ┆ 1.5          │
+        │ 3.0 ┆ 2.5          │
+        │ 4.0 ┆ 3.5          │
+        │ 5.0 ┆ 4.5          │
+        │ 6.0 ┆ 5.5          │
+        └─────┴──────────────┘
+
+        Specify weights to multiply the values in the window with:
+
+        >>> df.with_columns(
+        ...     rolling_mean=pl.col("A").rolling_mean(
+        ...         window_size=2, weights=[0.25, 0.75]
+        ...     ),
+        ... )
+        shape: (6, 2)
+        ┌─────┬──────────────┐
+        │ A   ┆ rolling_mean │
+        │ --- ┆ ---          │
+        │ f64 ┆ f64          │
+        ╞═════╪══════════════╡
+        │ 1.0 ┆ null         │
+        │ 2.0 ┆ 1.75         │
+        │ 3.0 ┆ 2.75         │
+        │ 4.0 ┆ 3.75         │
+        │ 5.0 ┆ 4.75         │
+        │ 6.0 ┆ 5.75         │
+        └─────┴──────────────┘
+
+        Center the values in the window
+
+        >>> df.with_columns(
+        ...     rolling_mean=pl.col("A").rolling_mean(window_size=3, center=True),
+        ... )
+        shape: (6, 2)
+        ┌─────┬──────────────┐
+        │ A   ┆ rolling_mean │
+        │ --- ┆ ---          │
+        │ f64 ┆ f64          │
+        ╞═════╪══════════════╡
+        │ 1.0 ┆ null         │
+        │ 2.0 ┆ 2.0          │
+        │ 3.0 ┆ 3.0          │
+        │ 4.0 ┆ 4.0          │
+        │ 5.0 ┆ 5.0          │
+        │ 6.0 ┆ null         │
+        └─────┴──────────────┘
+
+        Create a DataFrame with a datetime column and a row number column
+
+        >>> from datetime import timedelta, datetime
+        >>> start = datetime(2001, 1, 1)
+        >>> stop = datetime(2001, 1, 2)
+        >>> df_temporal = pl.DataFrame(
+        ...     {"date": pl.date_range(start, stop, "1h", eager=True)}
+        ... ).with_row_count()
+        >>> df_temporal
+        shape: (25, 2)
+        ┌────────┬─────────────────────┐
+        │ row_nr ┆ date                │
+        │ ---    ┆ ---                 │
+        │ u32    ┆ datetime[μs]        │
+        ╞════════╪═════════════════════╡
+        │ 0      ┆ 2001-01-01 00:00:00 │
+        │ 1      ┆ 2001-01-01 01:00:00 │
+        │ 2      ┆ 2001-01-01 02:00:00 │
+        │ 3      ┆ 2001-01-01 03:00:00 │
+        │ …      ┆ …                   │
+        │ 21     ┆ 2001-01-01 21:00:00 │
+        │ 22     ┆ 2001-01-01 22:00:00 │
+        │ 23     ┆ 2001-01-01 23:00:00 │
+        │ 24     ┆ 2001-01-02 00:00:00 │
+        └────────┴─────────────────────┘
+
+        Compute the rolling mean with the default left closure of temporal windows
+
+        >>> df_temporal.with_columns(
+        ...     rolling_row_mean=pl.col("row_nr").rolling_mean(
+        ...         window_size="2h", by="date"
+        ...     )
+        ... )
+        shape: (25, 3)
+        ┌────────┬─────────────────────┬──────────────────┐
+        │ row_nr ┆ date                ┆ rolling_row_mean │
+        │ ---    ┆ ---                 ┆ ---              │
+        │ u32    ┆ datetime[μs]        ┆ f64              │
+        ╞════════╪═════════════════════╪══════════════════╡
+        │ 0      ┆ 2001-01-01 00:00:00 ┆ null             │
+        │ 1      ┆ 2001-01-01 01:00:00 ┆ 0.0              │
+        │ 2      ┆ 2001-01-01 02:00:00 ┆ 0.5              │
+        │ 3      ┆ 2001-01-01 03:00:00 ┆ 1.5              │
+        │ …      ┆ …                   ┆ …                │
+        │ 21     ┆ 2001-01-01 21:00:00 ┆ 19.5             │
+        │ 22     ┆ 2001-01-01 22:00:00 ┆ 20.5             │
+        │ 23     ┆ 2001-01-01 23:00:00 ┆ 21.5             │
+        │ 24     ┆ 2001-01-02 00:00:00 ┆ 22.5             │
+        └────────┴─────────────────────┴──────────────────┘
+
+        Compute the rolling mean with the closure of windows on both sides
+
+        >>> df_temporal.with_columns(
+        ...     rolling_row_mean=pl.col("row_nr").rolling_mean(
+        ...         window_size="2h", by="date", closed="both"
+        ...     )
+        ... )
+        shape: (25, 3)
+        ┌────────┬─────────────────────┬──────────────────┐
+        │ row_nr ┆ date                ┆ rolling_row_mean │
+        │ ---    ┆ ---                 ┆ ---              │
+        │ u32    ┆ datetime[μs]        ┆ f64              │
+        ╞════════╪═════════════════════╪══════════════════╡
+        │ 0      ┆ 2001-01-01 00:00:00 ┆ 0.0              │
+        │ 1      ┆ 2001-01-01 01:00:00 ┆ 0.5              │
+        │ 2      ┆ 2001-01-01 02:00:00 ┆ 1.0              │
+        │ 3      ┆ 2001-01-01 03:00:00 ┆ 2.0              │
+        │ …      ┆ …                   ┆ …                │
+        │ 21     ┆ 2001-01-01 21:00:00 ┆ 20.0             │
+        │ 22     ┆ 2001-01-01 22:00:00 ┆ 21.0             │
+        │ 23     ┆ 2001-01-01 23:00:00 ┆ 22.0             │
+        │ 24     ┆ 2001-01-02 00:00:00 ┆ 23.0             │
+        └────────┴─────────────────────┴──────────────────┘
 
         """
         window_size, min_periods = _prepare_rolling_window_args(
             window_size, min_periods
         )
         return self._from_pyexpr(
             self._pyexpr.rolling_mean(
                 window_size, weights, min_periods, center, by, closed
             )
         )
 
+    @warn_closed_future_change()
     def rolling_sum(
         self,
         window_size: int | timedelta | str,
         weights: list[float] | None = None,
         min_periods: int | None = None,
         *,
         center: bool = False,
@@ -5013,24 +5447,27 @@
         """
         Apply a rolling sum (moving sum) over the values in this array.
 
         A window of length `window_size` will traverse the array. The values that fill
         this window will (optionally) be multiplied with the weights given by the
         `weight` vector. The resulting values will be aggregated to their sum.
 
-        If you pass a ``by`` column ``<t_0, t_1, ..., t_2>``, then by default the
-        windows will be:
+        If ``by`` has not been specified (the default), the window at a given row will
+        include the row itself, and the `window_size - 1` elements before it.
+
+        If you pass a ``by`` column ``<t_0, t_1, ..., t_n>``, then `closed="left"`
+        means the windows will be:
 
             - [t_0 - window_size, t_0)
             - [t_1 - window_size, t_1)
             - ...
             - [t_n - window_size, t_n)
 
-        Otherwise, the window at a given row will include the row itself, and the
-        `window_size - 1` elements before it.
+        With `closed="right"`, the left endpoint is not included and the right
+        endpoint is included.
 
         Parameters
         ----------
         window_size
             The length of the window. Can be a fixed integer size, or a dynamic temporal
             size indicated by a timedelta or the following string language:
 
@@ -5062,15 +5499,16 @@
         center
             Set the labels at the center of the window
         by
             If the `window_size` is temporal for instance `"5h"` or `"3s"`, you must
             set the column that will be used to determine the windows. This column must
             of dtype `{Date, Datetime}`
         closed : {'left', 'right', 'both', 'none'}
-            Define which sides of the temporal interval are closed (inclusive).
+            Define which sides of the temporal interval are closed (inclusive); only
+            applicable if `by` has been set.
 
         Warnings
         --------
         This functionality is experimental and may change without it being considered a
         breaking change.
 
         Notes
@@ -5078,43 +5516,156 @@
         If you want to compute multiple aggregation statistics over the same dynamic
         window, consider using `groupby_rolling` this method can cache the window size
         computation.
 
         Examples
         --------
         >>> df = pl.DataFrame({"A": [1.0, 2.0, 3.0, 4.0, 5.0, 6.0]})
-        >>> df.select(
-        ...     [
-        ...         pl.col("A").rolling_sum(window_size=2),
-        ...     ]
+        >>> df.with_columns(
+        ...     rolling_sum=pl.col("A").rolling_sum(window_size=2),
         ... )
-        shape: (6, 1)
-        ┌──────┐
-        │ A    │
-        │ ---  │
-        │ f64  │
-        ╞══════╡
-        │ null │
-        │ 3.0  │
-        │ 5.0  │
-        │ 7.0  │
-        │ 9.0  │
-        │ 11.0 │
-        └──────┘
+        shape: (6, 2)
+        ┌─────┬─────────────┐
+        │ A   ┆ rolling_sum │
+        │ --- ┆ ---         │
+        │ f64 ┆ f64         │
+        ╞═════╪═════════════╡
+        │ 1.0 ┆ null        │
+        │ 2.0 ┆ 3.0         │
+        │ 3.0 ┆ 5.0         │
+        │ 4.0 ┆ 7.0         │
+        │ 5.0 ┆ 9.0         │
+        │ 6.0 ┆ 11.0        │
+        └─────┴─────────────┘
+
+        Specify weights to multiply the values in the window with:
+
+        >>> df.with_columns(
+        ...     rolling_sum=pl.col("A").rolling_sum(
+        ...         window_size=2, weights=[0.25, 0.75]
+        ...     ),
+        ... )
+        shape: (6, 2)
+        ┌─────┬─────────────┐
+        │ A   ┆ rolling_sum │
+        │ --- ┆ ---         │
+        │ f64 ┆ f64         │
+        ╞═════╪═════════════╡
+        │ 1.0 ┆ null        │
+        │ 2.0 ┆ 1.75        │
+        │ 3.0 ┆ 2.75        │
+        │ 4.0 ┆ 3.75        │
+        │ 5.0 ┆ 4.75        │
+        │ 6.0 ┆ 5.75        │
+        └─────┴─────────────┘
+
+        Center the values in the window
+
+        >>> df.with_columns(
+        ...     rolling_sum=pl.col("A").rolling_sum(window_size=3, center=True),
+        ... )
+        shape: (6, 2)
+        ┌─────┬─────────────┐
+        │ A   ┆ rolling_sum │
+        │ --- ┆ ---         │
+        │ f64 ┆ f64         │
+        ╞═════╪═════════════╡
+        │ 1.0 ┆ null        │
+        │ 2.0 ┆ 6.0         │
+        │ 3.0 ┆ 9.0         │
+        │ 4.0 ┆ 12.0        │
+        │ 5.0 ┆ 15.0        │
+        │ 6.0 ┆ null        │
+        └─────┴─────────────┘
+
+        Create a DataFrame with a datetime column and a row number column
+
+        >>> from datetime import timedelta, datetime
+        >>> start = datetime(2001, 1, 1)
+        >>> stop = datetime(2001, 1, 2)
+        >>> df_temporal = pl.DataFrame(
+        ...     {"date": pl.date_range(start, stop, "1h", eager=True)}
+        ... ).with_row_count()
+        >>> df_temporal
+        shape: (25, 2)
+        ┌────────┬─────────────────────┐
+        │ row_nr ┆ date                │
+        │ ---    ┆ ---                 │
+        │ u32    ┆ datetime[μs]        │
+        ╞════════╪═════════════════════╡
+        │ 0      ┆ 2001-01-01 00:00:00 │
+        │ 1      ┆ 2001-01-01 01:00:00 │
+        │ 2      ┆ 2001-01-01 02:00:00 │
+        │ 3      ┆ 2001-01-01 03:00:00 │
+        │ …      ┆ …                   │
+        │ 21     ┆ 2001-01-01 21:00:00 │
+        │ 22     ┆ 2001-01-01 22:00:00 │
+        │ 23     ┆ 2001-01-01 23:00:00 │
+        │ 24     ┆ 2001-01-02 00:00:00 │
+        └────────┴─────────────────────┘
+
+        Compute the rolling sum with the default left closure of temporal windows
+
+        >>> df_temporal.with_columns(
+        ...     rolling_row_sum=pl.col("row_nr").rolling_sum(
+        ...         window_size="2h", by="date"
+        ...     )
+        ... )
+        shape: (25, 3)
+        ┌────────┬─────────────────────┬─────────────────┐
+        │ row_nr ┆ date                ┆ rolling_row_sum │
+        │ ---    ┆ ---                 ┆ ---             │
+        │ u32    ┆ datetime[μs]        ┆ u32             │
+        ╞════════╪═════════════════════╪═════════════════╡
+        │ 0      ┆ 2001-01-01 00:00:00 ┆ null            │
+        │ 1      ┆ 2001-01-01 01:00:00 ┆ 0               │
+        │ 2      ┆ 2001-01-01 02:00:00 ┆ 1               │
+        │ 3      ┆ 2001-01-01 03:00:00 ┆ 3               │
+        │ …      ┆ …                   ┆ …               │
+        │ 21     ┆ 2001-01-01 21:00:00 ┆ 39              │
+        │ 22     ┆ 2001-01-01 22:00:00 ┆ 41              │
+        │ 23     ┆ 2001-01-01 23:00:00 ┆ 43              │
+        │ 24     ┆ 2001-01-02 00:00:00 ┆ 45              │
+        └────────┴─────────────────────┴─────────────────┘
+
+        Compute the rolling sum with the closure of windows on both sides
+
+        >>> df_temporal.with_columns(
+        ...     rolling_row_sum=pl.col("row_nr").rolling_sum(
+        ...         window_size="2h", by="date", closed="both"
+        ...     )
+        ... )
+        shape: (25, 3)
+        ┌────────┬─────────────────────┬─────────────────┐
+        │ row_nr ┆ date                ┆ rolling_row_sum │
+        │ ---    ┆ ---                 ┆ ---             │
+        │ u32    ┆ datetime[μs]        ┆ u32             │
+        ╞════════╪═════════════════════╪═════════════════╡
+        │ 0      ┆ 2001-01-01 00:00:00 ┆ 0               │
+        │ 1      ┆ 2001-01-01 01:00:00 ┆ 1               │
+        │ 2      ┆ 2001-01-01 02:00:00 ┆ 3               │
+        │ 3      ┆ 2001-01-01 03:00:00 ┆ 6               │
+        │ …      ┆ …                   ┆ …               │
+        │ 21     ┆ 2001-01-01 21:00:00 ┆ 60              │
+        │ 22     ┆ 2001-01-01 22:00:00 ┆ 63              │
+        │ 23     ┆ 2001-01-01 23:00:00 ┆ 66              │
+        │ 24     ┆ 2001-01-02 00:00:00 ┆ 69              │
+        └────────┴─────────────────────┴─────────────────┘
 
         """
         window_size, min_periods = _prepare_rolling_window_args(
             window_size, min_periods
         )
         return self._from_pyexpr(
             self._pyexpr.rolling_sum(
                 window_size, weights, min_periods, center, by, closed
             )
         )
 
+    @warn_closed_future_change()
     def rolling_std(
         self,
         window_size: int | timedelta | str,
         weights: list[float] | None = None,
         min_periods: int | None = None,
         *,
         center: bool = False,
@@ -5125,24 +5676,27 @@
         """
         Compute a rolling standard deviation.
 
         A window of length `window_size` will traverse the array. The values that fill
         this window will (optionally) be multiplied with the weights given by the
         `weight` vector. The resulting values will be aggregated to their sum.
 
-        If you pass a ``by`` column ``<t_0, t_1, ..., t_2>``, then by default the
-        windows will be:
+        If ``by`` has not been specified (the default), the window at a given row will
+        include the row itself, and the `window_size - 1` elements before it.
+
+        If you pass a ``by`` column ``<t_0, t_1, ..., t_n>``, then `closed="left"` means
+        the windows will be:
 
             - [t_0 - window_size, t_0)
             - [t_1 - window_size, t_1)
             - ...
             - [t_n - window_size, t_n)
 
-        Otherwise, the window at a given row will include the row itself, and the
-        `window_size - 1` elements before it.
+        With `closed="right"`, the left endpoint is not included and the right
+        endpoint is included.
 
         Parameters
         ----------
         window_size
             The length of the window. Can be a fixed integer size, or a dynamic temporal
             size indicated by a timedelta or the following string language:
 
@@ -5174,15 +5728,16 @@
         center
             Set the labels at the center of the window
         by
             If the `window_size` is temporal for instance `"5h"` or `"3s"`, you must
             set the column that will be used to determine the windows. This column must
             be of dtype Datetime.
         closed : {'left', 'right', 'both', 'none'}
-            Define which sides of the temporal interval are closed (inclusive).
+            Define which sides of the temporal interval are closed (inclusive); only
+            applicable if `by` has been set.
         ddof
             "Delta Degrees of Freedom": The divisor for a length N window is N - ddof
 
         Warnings
         --------
         This functionality is experimental and may change without it being considered a
         breaking change.
@@ -5191,44 +5746,157 @@
         -----
         If you want to compute multiple aggregation statistics over the same dynamic
         window, consider using `groupby_rolling` this method can cache the window size
         computation.
 
         Examples
         --------
-        >>> df = pl.DataFrame({"A": [1.0, 2.0, 3.0, 4.0, 6.0, 8.0]})
-        >>> df.select(
-        ...     [
-        ...         pl.col("A").rolling_std(window_size=3),
-        ...     ]
+        >>> df = pl.DataFrame({"A": [1.0, 2.0, 3.0, 4.0, 5.0, 6.0]})
+        >>> df.with_columns(
+        ...     rolling_std=pl.col("A").rolling_std(window_size=2),
         ... )
-        shape: (6, 1)
-        ┌──────────┐
-        │ A        │
-        │ ---      │
-        │ f64      │
-        ╞══════════╡
-        │ null     │
-        │ null     │
-        │ 1.0      │
-        │ 1.0      │
-        │ 1.527525 │
-        │ 2.0      │
-        └──────────┘
+        shape: (6, 2)
+        ┌─────┬─────────────┐
+        │ A   ┆ rolling_std │
+        │ --- ┆ ---         │
+        │ f64 ┆ f64         │
+        ╞═════╪═════════════╡
+        │ 1.0 ┆ null        │
+        │ 2.0 ┆ 0.707107    │
+        │ 3.0 ┆ 0.707107    │
+        │ 4.0 ┆ 0.707107    │
+        │ 5.0 ┆ 0.707107    │
+        │ 6.0 ┆ 0.707107    │
+        └─────┴─────────────┘
+
+        Specify weights to multiply the values in the window with:
+
+        >>> df.with_columns(
+        ...     rolling_std=pl.col("A").rolling_std(
+        ...         window_size=2, weights=[0.25, 0.75]
+        ...     ),
+        ... )
+        shape: (6, 2)
+        ┌─────┬─────────────┐
+        │ A   ┆ rolling_std │
+        │ --- ┆ ---         │
+        │ f64 ┆ f64         │
+        ╞═════╪═════════════╡
+        │ 1.0 ┆ null        │
+        │ 2.0 ┆ 0.883883    │
+        │ 3.0 ┆ 1.237437    │
+        │ 4.0 ┆ 1.59099     │
+        │ 5.0 ┆ 1.944544    │
+        │ 6.0 ┆ 2.298097    │
+        └─────┴─────────────┘
+
+        Center the values in the window
+
+        >>> df.with_columns(
+        ...     rolling_std=pl.col("A").rolling_std(window_size=3, center=True),
+        ... )
+        shape: (6, 2)
+        ┌─────┬─────────────┐
+        │ A   ┆ rolling_std │
+        │ --- ┆ ---         │
+        │ f64 ┆ f64         │
+        ╞═════╪═════════════╡
+        │ 1.0 ┆ null        │
+        │ 2.0 ┆ 1.0         │
+        │ 3.0 ┆ 1.0         │
+        │ 4.0 ┆ 1.0         │
+        │ 5.0 ┆ 1.0         │
+        │ 6.0 ┆ null        │
+        └─────┴─────────────┘
+
+        Create a DataFrame with a datetime column and a row number column
+
+        >>> from datetime import timedelta, datetime
+        >>> start = datetime(2001, 1, 1)
+        >>> stop = datetime(2001, 1, 2)
+        >>> df_temporal = pl.DataFrame(
+        ...     {"date": pl.date_range(start, stop, "1h", eager=True)}
+        ... ).with_row_count()
+        >>> df_temporal
+        shape: (25, 2)
+        ┌────────┬─────────────────────┐
+        │ row_nr ┆ date                │
+        │ ---    ┆ ---                 │
+        │ u32    ┆ datetime[μs]        │
+        ╞════════╪═════════════════════╡
+        │ 0      ┆ 2001-01-01 00:00:00 │
+        │ 1      ┆ 2001-01-01 01:00:00 │
+        │ 2      ┆ 2001-01-01 02:00:00 │
+        │ 3      ┆ 2001-01-01 03:00:00 │
+        │ …      ┆ …                   │
+        │ 21     ┆ 2001-01-01 21:00:00 │
+        │ 22     ┆ 2001-01-01 22:00:00 │
+        │ 23     ┆ 2001-01-01 23:00:00 │
+        │ 24     ┆ 2001-01-02 00:00:00 │
+        └────────┴─────────────────────┘
+
+        Compute the rolling std with the default left closure of temporal windows
+
+        >>> df_temporal.with_columns(
+        ...     rolling_row_std=pl.col("row_nr").rolling_std(
+        ...         window_size="2h", by="date"
+        ...     )
+        ... )
+        shape: (25, 3)
+        ┌────────┬─────────────────────┬─────────────────┐
+        │ row_nr ┆ date                ┆ rolling_row_std │
+        │ ---    ┆ ---                 ┆ ---             │
+        │ u32    ┆ datetime[μs]        ┆ f64             │
+        ╞════════╪═════════════════════╪═════════════════╡
+        │ 0      ┆ 2001-01-01 00:00:00 ┆ null            │
+        │ 1      ┆ 2001-01-01 01:00:00 ┆ 0.0             │
+        │ 2      ┆ 2001-01-01 02:00:00 ┆ 0.707107        │
+        │ 3      ┆ 2001-01-01 03:00:00 ┆ 0.707107        │
+        │ …      ┆ …                   ┆ …               │
+        │ 21     ┆ 2001-01-01 21:00:00 ┆ 0.707107        │
+        │ 22     ┆ 2001-01-01 22:00:00 ┆ 0.707107        │
+        │ 23     ┆ 2001-01-01 23:00:00 ┆ 0.707107        │
+        │ 24     ┆ 2001-01-02 00:00:00 ┆ 0.707107        │
+        └────────┴─────────────────────┴─────────────────┘
+
+        Compute the rolling std with the closure of windows on both sides
+
+        >>> df_temporal.with_columns(
+        ...     rolling_row_std=pl.col("row_nr").rolling_std(
+        ...         window_size="2h", by="date", closed="both"
+        ...     )
+        ... )
+        shape: (25, 3)
+        ┌────────┬─────────────────────┬─────────────────┐
+        │ row_nr ┆ date                ┆ rolling_row_std │
+        │ ---    ┆ ---                 ┆ ---             │
+        │ u32    ┆ datetime[μs]        ┆ f64             │
+        ╞════════╪═════════════════════╪═════════════════╡
+        │ 0      ┆ 2001-01-01 00:00:00 ┆ 0.0             │
+        │ 1      ┆ 2001-01-01 01:00:00 ┆ 0.707107        │
+        │ 2      ┆ 2001-01-01 02:00:00 ┆ 1.0             │
+        │ 3      ┆ 2001-01-01 03:00:00 ┆ 1.0             │
+        │ …      ┆ …                   ┆ …               │
+        │ 21     ┆ 2001-01-01 21:00:00 ┆ 1.0             │
+        │ 22     ┆ 2001-01-01 22:00:00 ┆ 1.0             │
+        │ 23     ┆ 2001-01-01 23:00:00 ┆ 1.0             │
+        │ 24     ┆ 2001-01-02 00:00:00 ┆ 1.0             │
+        └────────┴─────────────────────┴─────────────────┘
 
         """
         window_size, min_periods = _prepare_rolling_window_args(
             window_size, min_periods
         )
         return self._from_pyexpr(
             self._pyexpr.rolling_std(
                 window_size, weights, min_periods, center, by, closed, ddof
             )
         )
 
+    @warn_closed_future_change()
     def rolling_var(
         self,
         window_size: int | timedelta | str,
         weights: list[float] | None = None,
         min_periods: int | None = None,
         *,
         center: bool = False,
@@ -5239,24 +5907,27 @@
         """
         Compute a rolling variance.
 
         A window of length `window_size` will traverse the array. The values that fill
         this window will (optionally) be multiplied with the weights given by the
         `weight` vector. The resulting values will be aggregated to their sum.
 
-        If you pass a ``by`` column ``<t_0, t_1, ..., t_2>``, then by default the
-        windows will be:
+        If ``by`` has not been specified (the default), the window at a given row will
+        include the row itself, and the `window_size - 1` elements before it.
+
+        If you pass a ``by`` column ``<t_0, t_1, ..., t_n>``, then `closed="left"`
+        means the windows will be:
 
             - [t_0 - window_size, t_0)
             - [t_1 - window_size, t_1)
             - ...
             - [t_n - window_size, t_n)
 
-        Otherwise, the window at a given row will include the row itself, and the
-        `window_size - 1` elements before it.
+        With `closed="right"`, the left endpoint is not included and the right
+        endpoint is included.
 
         Parameters
         ----------
         window_size
             The length of the window. Can be a fixed integer size, or a dynamic temporal
             size indicated by a timedelta or the following string language:
 
@@ -5288,15 +5959,16 @@
         center
             Set the labels at the center of the window
         by
             If the `window_size` is temporal for instance `"5h"` or `"3s"`, you must
             set the column that will be used to determine the windows. This column must
             be of dtype Datetime.
         closed : {'left', 'right', 'both', 'none'}
-            Define which sides of the temporal interval are closed (inclusive).
+            Define which sides of the temporal interval are closed (inclusive); only
+            applicable if `by` has been set.
         ddof
             "Delta Degrees of Freedom": The divisor for a length N window is N - ddof
 
         Warnings
         --------
         This functionality is experimental and may change without it being considered a
         breaking change.
@@ -5305,33 +5977,145 @@
         -----
         If you want to compute multiple aggregation statistics over the same dynamic
         window, consider using `groupby_rolling` this method can cache the window size
         computation.
 
         Examples
         --------
-        >>> df = pl.DataFrame({"A": [1.0, 2.0, 3.0, 4.0, 6.0, 8.0]})
-        >>> df.select(
-        ...     [
-        ...         pl.col("A").rolling_var(window_size=3),
-        ...     ]
+        >>> df = pl.DataFrame({"A": [1.0, 2.0, 3.0, 4.0, 5.0, 6.0]})
+        >>> df.with_columns(
+        ...     rolling_var=pl.col("A").rolling_var(window_size=2),
         ... )
-        shape: (6, 1)
-        ┌──────────┐
-        │ A        │
-        │ ---      │
-        │ f64      │
-        ╞══════════╡
-        │ null     │
-        │ null     │
-        │ 1.0      │
-        │ 1.0      │
-        │ 2.333333 │
-        │ 4.0      │
-        └──────────┘
+        shape: (6, 2)
+        ┌─────┬─────────────┐
+        │ A   ┆ rolling_var │
+        │ --- ┆ ---         │
+        │ f64 ┆ f64         │
+        ╞═════╪═════════════╡
+        │ 1.0 ┆ null        │
+        │ 2.0 ┆ 0.5         │
+        │ 3.0 ┆ 0.5         │
+        │ 4.0 ┆ 0.5         │
+        │ 5.0 ┆ 0.5         │
+        │ 6.0 ┆ 0.5         │
+        └─────┴─────────────┘
+
+        Specify weights to multiply the values in the window with:
+
+        >>> df.with_columns(
+        ...     rolling_var=pl.col("A").rolling_var(
+        ...         window_size=2, weights=[0.25, 0.75]
+        ...     ),
+        ... )
+        shape: (6, 2)
+        ┌─────┬─────────────┐
+        │ A   ┆ rolling_var │
+        │ --- ┆ ---         │
+        │ f64 ┆ f64         │
+        ╞═════╪═════════════╡
+        │ 1.0 ┆ null        │
+        │ 2.0 ┆ 0.78125     │
+        │ 3.0 ┆ 1.53125     │
+        │ 4.0 ┆ 2.53125     │
+        │ 5.0 ┆ 3.78125     │
+        │ 6.0 ┆ 5.28125     │
+        └─────┴─────────────┘
+
+        Center the values in the window
+
+        >>> df.with_columns(
+        ...     rolling_var=pl.col("A").rolling_var(window_size=3, center=True),
+        ... )
+        shape: (6, 2)
+        ┌─────┬─────────────┐
+        │ A   ┆ rolling_var │
+        │ --- ┆ ---         │
+        │ f64 ┆ f64         │
+        ╞═════╪═════════════╡
+        │ 1.0 ┆ null        │
+        │ 2.0 ┆ 1.0         │
+        │ 3.0 ┆ 1.0         │
+        │ 4.0 ┆ 1.0         │
+        │ 5.0 ┆ 1.0         │
+        │ 6.0 ┆ null        │
+        └─────┴─────────────┘
+
+        Create a DataFrame with a datetime column and a row number column
+
+        >>> from datetime import timedelta, datetime
+        >>> start = datetime(2001, 1, 1)
+        >>> stop = datetime(2001, 1, 2)
+        >>> df_temporal = pl.DataFrame(
+        ...     {"date": pl.date_range(start, stop, "1h", eager=True)}
+        ... ).with_row_count()
+        >>> df_temporal
+        shape: (25, 2)
+        ┌────────┬─────────────────────┐
+        │ row_nr ┆ date                │
+        │ ---    ┆ ---                 │
+        │ u32    ┆ datetime[μs]        │
+        ╞════════╪═════════════════════╡
+        │ 0      ┆ 2001-01-01 00:00:00 │
+        │ 1      ┆ 2001-01-01 01:00:00 │
+        │ 2      ┆ 2001-01-01 02:00:00 │
+        │ 3      ┆ 2001-01-01 03:00:00 │
+        │ …      ┆ …                   │
+        │ 21     ┆ 2001-01-01 21:00:00 │
+        │ 22     ┆ 2001-01-01 22:00:00 │
+        │ 23     ┆ 2001-01-01 23:00:00 │
+        │ 24     ┆ 2001-01-02 00:00:00 │
+        └────────┴─────────────────────┘
+
+        Compute the rolling var with the default left closure of temporal windows
+
+        >>> df_temporal.with_columns(
+        ...     rolling_row_var=pl.col("row_nr").rolling_var(
+        ...         window_size="2h", by="date"
+        ...     )
+        ... )
+        shape: (25, 3)
+        ┌────────┬─────────────────────┬─────────────────┐
+        │ row_nr ┆ date                ┆ rolling_row_var │
+        │ ---    ┆ ---                 ┆ ---             │
+        │ u32    ┆ datetime[μs]        ┆ f64             │
+        ╞════════╪═════════════════════╪═════════════════╡
+        │ 0      ┆ 2001-01-01 00:00:00 ┆ null            │
+        │ 1      ┆ 2001-01-01 01:00:00 ┆ 0.0             │
+        │ 2      ┆ 2001-01-01 02:00:00 ┆ 0.5             │
+        │ 3      ┆ 2001-01-01 03:00:00 ┆ 0.5             │
+        │ …      ┆ …                   ┆ …               │
+        │ 21     ┆ 2001-01-01 21:00:00 ┆ 0.5             │
+        │ 22     ┆ 2001-01-01 22:00:00 ┆ 0.5             │
+        │ 23     ┆ 2001-01-01 23:00:00 ┆ 0.5             │
+        │ 24     ┆ 2001-01-02 00:00:00 ┆ 0.5             │
+        └────────┴─────────────────────┴─────────────────┘
+
+        Compute the rolling var with the closure of windows on both sides
+
+        >>> df_temporal.with_columns(
+        ...     rolling_row_var=pl.col("row_nr").rolling_var(
+        ...         window_size="2h", by="date", closed="both"
+        ...     )
+        ... )
+        shape: (25, 3)
+        ┌────────┬─────────────────────┬─────────────────┐
+        │ row_nr ┆ date                ┆ rolling_row_var │
+        │ ---    ┆ ---                 ┆ ---             │
+        │ u32    ┆ datetime[μs]        ┆ f64             │
+        ╞════════╪═════════════════════╪═════════════════╡
+        │ 0      ┆ 2001-01-01 00:00:00 ┆ 0.0             │
+        │ 1      ┆ 2001-01-01 01:00:00 ┆ 0.5             │
+        │ 2      ┆ 2001-01-01 02:00:00 ┆ 1.0             │
+        │ 3      ┆ 2001-01-01 03:00:00 ┆ 1.0             │
+        │ …      ┆ …                   ┆ …               │
+        │ 21     ┆ 2001-01-01 21:00:00 ┆ 1.0             │
+        │ 22     ┆ 2001-01-01 22:00:00 ┆ 1.0             │
+        │ 23     ┆ 2001-01-01 23:00:00 ┆ 1.0             │
+        │ 24     ┆ 2001-01-02 00:00:00 ┆ 1.0             │
+        └────────┴─────────────────────┴─────────────────┘
 
         """
         window_size, min_periods = _prepare_rolling_window_args(
             window_size, min_periods
         )
         return self._from_pyexpr(
             self._pyexpr.rolling_var(
@@ -5341,37 +6125,41 @@
                 center,
                 by,
                 closed,
                 ddof,
             )
         )
 
+    @warn_closed_future_change()
     def rolling_median(
         self,
         window_size: int | timedelta | str,
         weights: list[float] | None = None,
         min_periods: int | None = None,
         *,
         center: bool = False,
         by: str | None = None,
         closed: ClosedInterval = "left",
     ) -> Self:
         """
         Compute a rolling median.
 
-        If you pass a ``by`` column ``<t_0, t_1, ..., t_2>``, then by default the
-        windows will be:
+        If ``by`` has not been specified (the default), the window at a given row will
+        include the row itself, and the `window_size - 1` elements before it.
+
+        If you pass a ``by`` column ``<t_0, t_1, ..., t_n>``, then `closed="left"` means
+        the windows will be:
 
             - [t_0 - window_size, t_0)
             - [t_1 - window_size, t_1)
             - ...
             - [t_n - window_size, t_n)
 
-        Otherwise, the window at a given row will include the row itself, and the
-        `window_size - 1` elements before it.
+        With `closed="right"`, the left endpoint is not included and the right
+        endpoint is included.
 
         Parameters
         ----------
         window_size
             The length of the window. Can be a fixed integer size, or a dynamic temporal
             size indicated by a timedelta or the following string language:
 
@@ -5403,59 +6191,99 @@
         center
             Set the labels at the center of the window
         by
             If the `window_size` is temporal for instance `"5h"` or `"3s"`, you must
             set the column that will be used to determine the windows. This column must
             be of dtype Datetime.
         closed : {'left', 'right', 'both', 'none'}
-            Define which sides of the temporal interval are closed (inclusive).
+            Define which sides of the temporal interval are closed (inclusive); only
+            applicable if `by` has been set.
 
         Warnings
         --------
         This functionality is experimental and may change without it being considered a
         breaking change.
 
         Notes
         -----
         If you want to compute multiple aggregation statistics over the same dynamic
         window, consider using `groupby_rolling` this method can cache the window size
         computation.
 
         Examples
         --------
-        >>> df = pl.DataFrame({"A": [1.0, 2.0, 3.0, 4.0, 6.0, 8.0]})
-        >>> df.select(
-        ...     [
-        ...         pl.col("A").rolling_median(window_size=3),
-        ...     ]
+        >>> df = pl.DataFrame({"A": [1.0, 2.0, 3.0, 4.0, 5.0, 6.0]})
+        >>> df.with_columns(
+        ...     rolling_median=pl.col("A").rolling_median(window_size=2),
         ... )
-        shape: (6, 1)
-        ┌──────┐
-        │ A    │
-        │ ---  │
-        │ f64  │
-        ╞══════╡
-        │ null │
-        │ null │
-        │ 2.0  │
-        │ 3.0  │
-        │ 4.0  │
-        │ 6.0  │
-        └──────┘
+        shape: (6, 2)
+        ┌─────┬────────────────┐
+        │ A   ┆ rolling_median │
+        │ --- ┆ ---            │
+        │ f64 ┆ f64            │
+        ╞═════╪════════════════╡
+        │ 1.0 ┆ null           │
+        │ 2.0 ┆ 1.5            │
+        │ 3.0 ┆ 2.5            │
+        │ 4.0 ┆ 3.5            │
+        │ 5.0 ┆ 4.5            │
+        │ 6.0 ┆ 5.5            │
+        └─────┴────────────────┘
+
+        Specify weights to multiply the values in the window with:
+
+        >>> df.with_columns(
+        ...     rolling_median=pl.col("A").rolling_median(
+        ...         window_size=2, weights=[0.25, 0.75]
+        ...     ),
+        ... )
+        shape: (6, 2)
+        ┌─────┬────────────────┐
+        │ A   ┆ rolling_median │
+        │ --- ┆ ---            │
+        │ f64 ┆ f64            │
+        ╞═════╪════════════════╡
+        │ 1.0 ┆ null           │
+        │ 2.0 ┆ 0.875          │
+        │ 3.0 ┆ 1.375          │
+        │ 4.0 ┆ 1.875          │
+        │ 5.0 ┆ 2.375          │
+        │ 6.0 ┆ 2.875          │
+        └─────┴────────────────┘
+
+        Center the values in the window
+
+        >>> df.with_columns(
+        ...     rolling_median=pl.col("A").rolling_median(window_size=3, center=True),
+        ... )
+        shape: (6, 2)
+        ┌─────┬────────────────┐
+        │ A   ┆ rolling_median │
+        │ --- ┆ ---            │
+        │ f64 ┆ f64            │
+        ╞═════╪════════════════╡
+        │ 1.0 ┆ null           │
+        │ 2.0 ┆ 2.0            │
+        │ 3.0 ┆ 3.0            │
+        │ 4.0 ┆ 4.0            │
+        │ 5.0 ┆ 5.0            │
+        │ 6.0 ┆ null           │
+        └─────┴────────────────┘
 
         """
         window_size, min_periods = _prepare_rolling_window_args(
             window_size, min_periods
         )
         return self._from_pyexpr(
             self._pyexpr.rolling_median(
                 window_size, weights, min_periods, center, by, closed
             )
         )
 
+    @warn_closed_future_change()
     def rolling_quantile(
         self,
         quantile: float,
         interpolation: RollingInterpolationMethod = "nearest",
         window_size: int | timedelta | str = 2,
         weights: list[float] | None = None,
         min_periods: int | None = None,
@@ -5463,34 +6291,37 @@
         center: bool = False,
         by: str | None = None,
         closed: ClosedInterval = "left",
     ) -> Self:
         """
         Compute a rolling quantile.
 
-        If you pass a ``by`` column ``<t_0, t_1, ..., t_2>``, then by default the
-        windows will be:
+        If ``by`` has not been specified (the default), the window at a given row will
+        include the row itself, and the `window_size - 1` elements before it.
+
+        If you pass a ``by`` column ``<t_0, t_1, ..., t_n>``, then `closed="left"`
+        means the windows will be:
 
             - [t_0 - window_size, t_0)
             - [t_1 - window_size, t_1)
             - ...
             - [t_n - window_size, t_n)
 
-        Otherwise, the window at a given row will include the row itself, and the
-        `window_size - 1` elements before it.
+        With `closed="right"`, the left endpoint is not included and the right
+        endpoint is included.
 
         Parameters
         ----------
         quantile
             Quantile between 0.0 and 1.0.
         interpolation : {'nearest', 'higher', 'lower', 'midpoint', 'linear'}
             Interpolation method.
         window_size
-            The length of the window. Can be a fixed integer size, or a dynamic temporal
-            size indicated by a timedelta or the following string language:
+            The length of the window. Can be a fixed integer size, or a dynamic
+            temporal size indicated by a timedelta or the following string language:
 
             - 1ns   (1 nanosecond)
             - 1us   (1 microsecond)
             - 1ms   (1 millisecond)
             - 1s    (1 second)
             - 1m    (1 minute)
             - 1h    (1 hour)
@@ -5504,60 +6335,103 @@
             Suffix with `"_saturating"` to indicate that dates too large for
             their month should saturate at the largest date
             (e.g. 2022-02-29 -> 2022-02-28) instead of erroring.
 
             If a timedelta or the dynamic string language is used, the `by`
             and `closed` arguments must also be set.
         weights
-            An optional slice with the same length as the window that will be multiplied
-            elementwise with the values in the window.
+            An optional slice with the same length as the window that will be
+            multiplied elementwise with the values in the window.
         min_periods
             The number of values in the window that should be non-null before computing
             a result. If None, it will be set equal to window size.
         center
             Set the labels at the center of the window
         by
             If the `window_size` is temporal for instance `"5h"` or `"3s"`, you must
             set the column that will be used to determine the windows. This column must
             be of dtype Datetime.
         closed : {'left', 'right', 'both', 'none'}
-            Define which sides of the temporal interval are closed (inclusive).
+            Define which sides of the temporal interval are closed (inclusive); only
+            applicable if `by` has been set.
 
         Warnings
         --------
         This functionality is experimental and may change without it being considered a
         breaking change.
 
         Notes
         -----
         If you want to compute multiple aggregation statistics over the same dynamic
         window, consider using `groupby_rolling` this method can cache the window size
         computation.
 
         Examples
         --------
-        >>> df = pl.DataFrame({"A": [1.0, 2.0, 3.0, 4.0, 6.0, 8.0]})
-        >>> df.select(
-        ...     [
-        ...         pl.col("A").rolling_quantile(quantile=0.33, window_size=3),
-        ...     ]
+        >>> df = pl.DataFrame({"A": [1.0, 2.0, 3.0, 4.0, 5.0, 6.0]})
+        >>> df.with_columns(
+        ...     rolling_quantile=pl.col("A").rolling_quantile(
+        ...         quantile=0.25, window_size=4
+        ...     ),
         ... )
-        shape: (6, 1)
-        ┌──────┐
-        │ A    │
-        │ ---  │
-        │ f64  │
-        ╞══════╡
-        │ null │
-        │ null │
-        │ 1.0  │
-        │ 2.0  │
-        │ 3.0  │
-        │ 4.0  │
-        └──────┘
+        shape: (6, 2)
+        ┌─────┬──────────────────┐
+        │ A   ┆ rolling_quantile │
+        │ --- ┆ ---              │
+        │ f64 ┆ f64              │
+        ╞═════╪══════════════════╡
+        │ 1.0 ┆ null             │
+        │ 2.0 ┆ null             │
+        │ 3.0 ┆ null             │
+        │ 4.0 ┆ 2.0              │
+        │ 5.0 ┆ 3.0              │
+        │ 6.0 ┆ 4.0              │
+        └─────┴──────────────────┘
+
+        Specify weights to multiply the values in the window with:
+
+        >>> df.with_columns(
+        ...     rolling_quantile=pl.col("A").rolling_quantile(
+        ...         quantile=0.25, window_size=4, weights=[0.2, 0.4, 0.4, 0.2]
+        ...     ),
+        ... )
+        shape: (6, 2)
+        ┌─────┬──────────────────┐
+        │ A   ┆ rolling_quantile │
+        │ --- ┆ ---              │
+        │ f64 ┆ f64              │
+        ╞═════╪══════════════════╡
+        │ 1.0 ┆ null             │
+        │ 2.0 ┆ null             │
+        │ 3.0 ┆ null             │
+        │ 4.0 ┆ 0.8              │
+        │ 5.0 ┆ 1.0              │
+        │ 6.0 ┆ 1.2              │
+        └─────┴──────────────────┘
+
+        Center the values in the window
+
+        >>> df.with_columns(
+        ...     rolling_quantile=pl.col("A").rolling_quantile(
+        ...         quantile=0.2, window_size=5, center=True
+        ...     ),
+        ... )
+        shape: (6, 2)
+        ┌─────┬──────────────────┐
+        │ A   ┆ rolling_quantile │
+        │ --- ┆ ---              │
+        │ f64 ┆ f64              │
+        ╞═════╪══════════════════╡
+        │ 1.0 ┆ null             │
+        │ 2.0 ┆ null             │
+        │ 3.0 ┆ 2.0              │
+        │ 4.0 ┆ 3.0              │
+        │ 5.0 ┆ null             │
+        │ 6.0 ┆ null             │
+        └─────┴──────────────────┘
 
         """
         window_size, min_periods = _prepare_rolling_window_args(
             window_size, min_periods
         )
         return self._from_pyexpr(
             self._pyexpr.rolling_quantile(
@@ -6451,14 +7325,77 @@
         ╞═════╡
         │ inf │
         └─────┘
 
         """
         return self._from_pyexpr(self._pyexpr.arctanh())
 
+    def degrees(self) -> Self:
+        """
+        Convert from radians to degrees.
+
+        Returns
+        -------
+        Series of dtype Float64
+
+        Examples
+        --------
+        >>> import math
+        >>> df = pl.DataFrame({"a": [x * math.pi for x in range(-4, 5)]})
+        >>> df.select(pl.col("a").degrees())
+        shape: (9, 1)
+        ┌────────┐
+        │ a      │
+        │ ---    │
+        │ f64    │
+        ╞════════╡
+        │ -720.0 │
+        │ -540.0 │
+        │ -360.0 │
+        │ -180.0 │
+        │ 0.0    │
+        │ 180.0  │
+        │ 360.0  │
+        │ 540.0  │
+        │ 720.0  │
+        └────────┘
+        """
+        return self._from_pyexpr(self._pyexpr.degrees())
+
+    def radians(self) -> Self:
+        """
+        Convert from degrees to radians.
+
+        Returns
+        -------
+        Series of dtype Float64
+
+        Examples
+        --------
+        >>> df = pl.DataFrame({"a": [-720, -540, -360, -180, 0, 180, 360, 540, 720]})
+        >>> df.select(pl.col("a").radians())
+        shape: (9, 1)
+        ┌────────────┐
+        │ a          │
+        │ ---        │
+        │ f64        │
+        ╞════════════╡
+        │ -12.566371 │
+        │ -9.424778  │
+        │ -6.283185  │
+        │ -3.141593  │
+        │ 0.0        │
+        │ 3.141593   │
+        │ 6.283185   │
+        │ 9.424778   │
+        │ 12.566371  │
+        └────────────┘
+        """
+        return self._from_pyexpr(self._pyexpr.radians())
+
     def reshape(self, dimensions: tuple[int, ...]) -> Self:
         """
         Reshape this Expr to a flat Series or a Series of Lists.
 
         Parameters
         ----------
         dimensions
```

### Comparing `polars_u64_idx-0.18.3/polars/expr/list.py` & `polars_u64_idx-0.18.4/polars/expr/list.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/polars/expr/meta.py` & `polars_u64_idx-0.18.4/polars/expr/meta.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/polars/expr/string.py` & `polars_u64_idx-0.18.4/polars/expr/string.py`

 * *Files 2% similar despite different names*

```diff
@@ -487,14 +487,37 @@
         │ cat │
         │ dog │
         └─────┘
 
         """
         return wrap_expr(self._pyexpr.str_to_lowercase())
 
+    def to_titlecase(self) -> Expr:
+        """
+        Transform to titlecase variant.
+
+        Examples
+        --------
+        >>> df = pl.DataFrame(
+        ...     {"sing": ["welcome to my world", "THERE'S NO TURNING BACK"]}
+        ... )
+        >>> df.select(pl.col("sing").str.to_titlecase())
+        shape: (2, 1)
+        ┌─────────────────────────┐
+        │ sing                    │
+        │ ---                     │
+        │ str                     │
+        ╞═════════════════════════╡
+        │ Welcome To My World     │
+        │ There's No Turning Back │
+        └─────────────────────────┘
+
+        """
+        return wrap_expr(self._pyexpr.str_to_titlecase())
+
     def strip(self, characters: str | None = None) -> Expr:
         r"""
         Remove leading and trailing characters.
 
         Parameters
         ----------
         characters
@@ -915,25 +938,30 @@
         contains : Check if string contains a substring that matches a regex.
         ends_with : Check if string values end with a substring.
 
         """
         prefix = parse_as_expression(prefix, str_as_lit=True)
         return wrap_expr(self._pyexpr.str_starts_with(prefix))
 
-    def json_extract(self, dtype: PolarsDataType | None = None) -> Expr:
+    def json_extract(
+        self, dtype: PolarsDataType | None = None, infer_schema_length: int | None = 100
+    ) -> Expr:
         """
         Parse string values as JSON.
 
         Throw errors if encounter invalid JSON strings.
 
         Parameters
         ----------
         dtype
             The dtype to cast the extracted value to. If None, the dtype will be
             inferred from the JSON value.
+        infer_schema_length
+            How many rows to parse to determine the schema.
+            If ``None`` all rows are used.
 
         Examples
         --------
         >>> df = pl.DataFrame(
         ...     {"json": ['{"a":1, "b": true}', None, '{"a":2, "b": false}']}
         ... )
         >>> dtype = pl.Struct([pl.Field("a", pl.Int64), pl.Field("b", pl.Boolean)])
@@ -953,15 +981,15 @@
         --------
         json_path_match : Extract the first match of json string with provided JSONPath
             expression.
 
         """
         if dtype is not None:
             dtype = py_type_to_dtype(dtype)
-        return wrap_expr(self._pyexpr.str_json_extract(dtype))
+        return wrap_expr(self._pyexpr.str_json_extract(dtype, infer_schema_length))
 
     def json_path_match(self, json_path: str) -> Expr:
         """
         Extract the first match of json string with provided JSONPath expression.
 
         Throw errors if encounter invalid json strings.
         All return value will be casted to Utf8 regardless of the original value.
```

### Comparing `polars_u64_idx-0.18.3/polars/expr/struct.py` & `polars_u64_idx-0.18.4/polars/expr/struct.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/polars/functions/__init__.py` & `polars_u64_idx-0.18.4/polars/functions/__init__.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/polars/functions/as_datatype.py` & `polars_u64_idx-0.18.4/polars/functions/as_datatype.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/polars/functions/eager.py` & `polars_u64_idx-0.18.4/polars/functions/eager.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/polars/functions/lazy.py` & `polars_u64_idx-0.18.4/polars/functions/lazy.py`

 * *Files 0% similar despite different names*

```diff
@@ -1207,18 +1207,21 @@
     if isinstance(value, datetime):
         time_unit = "us" if dtype is None else getattr(dtype, "time_unit", "us")
         time_zone = (
             value.tzinfo
             if getattr(dtype, "time_zone", None) is None
             else getattr(dtype, "time_zone", None)
         )
-        if value.tzinfo is not None and getattr(dtype, "time_zone", None) is not None:
+        if (
+            value.tzinfo is not None
+            and getattr(dtype, "time_zone", None) is not None
+            and dtype.time_zone != str(value.tzinfo)  # type: ignore[union-attr]
+        ):
             raise TypeError(
-                "Cannot cast tz-aware value to tz-aware dtype. "
-                "Please drop the time zone from the dtype."
+                f"Time zone of dtype ({dtype.time_zone}) differs from time zone of value ({value.tzinfo})."  # type: ignore[union-attr]
             )
         e = lit(_datetime_to_pl_timestamp(value, time_unit)).cast(Datetime(time_unit))
         if time_zone is not None:
             return e.dt.replace_time_zone(str(time_zone))
         else:
             return e
 
@@ -1414,15 +1417,15 @@
 
     >>> df = pl.DataFrame({"a": [1, 8, 3], "b": [4, 5, 2], "c": ["foo", "bar", "foo"]})
     >>> df.select(pl.corr("a", "b", method="spearman"))
     shape: (1, 1)
     ┌─────┐
     │ a   │
     │ --- │
-    │ f64 │
+    │ f32 │
     ╞═════╡
     │ 0.5 │
     └─────┘
     """
     if isinstance(a, str):
         a = col(a)
     if isinstance(b, str):
```

### Comparing `polars_u64_idx-0.18.3/polars/functions/range.py` & `polars_u64_idx-0.18.4/polars/functions/range.py`

 * *Files 4% similar despite different names*

```diff
@@ -201,15 +201,21 @@
     start
         Lower bound of the date range, given as a date, datetime, Expr, or column name.
     end
         Upper bound of the date range, given as a date, datetime, Expr, or column name.
     interval
         Interval of the range periods; can be a python timedelta object like
         ``timedelta(days=10)`` or a polars duration string, such as ``3d12h4m25s``
-        (representing 3 days, 12 hours, 4 minutes, and 25 seconds).
+        (representing 3 days, 12 hours, 4 minutes, and 25 seconds). Append
+        ``_saturating`` to the interval string to restrict resulting invalid dates to
+        valid ranges.
+
+        It is common to attempt to create a month-end date series by using the "1mo"
+        offset string with a start date at the end of the month. This will not produce
+        the desired results. See Note #2 below for further information.
     closed : {'both', 'left', 'right', 'none'}
         Define whether the temporal window interval is closed or not.
     time_unit : {None, 'ns', 'us', 'ms'}
         Set the time unit.
     time_zone:
         Optional timezone
     eager
@@ -220,18 +226,52 @@
 
         .. deprecated:: 0.18.0
             This argument is deprecated. Use the ``alias`` method instead.
 
 
     Notes
     -----
-    If both ``start`` and ``end`` are passed as date types (not datetime), and the
+    1) If both ``start`` and ``end`` are passed as date types (not datetime), and the
     interval granularity is no finer than 1d, the returned range is also of
     type date. All other permutations return a datetime Series.
 
+    2) Because different months of the year have differing numbers of days, the offset
+    strings "1mo" and "1y" are not well-defined units of time, and vary according to
+    their starting point. For example, February 1st offset by one month returns a time
+    28 days later (in a non-leap year), whereas May 1st offset by one month returns a
+    time 31 days later. In general, an offset of one month selects the same day in the
+    following month. However, this is not always intended: when one begins Febrary 28th
+    and offsets by 1 month, does the user intend to target March 28th (the next month
+    but same day), or March 31st (the end of the month)?
+
+    Polars uses the first approach: February 28th offset by 1 month is March 28th. When
+    a date-series is generated, each date is offset as of the prior date, meaning that
+    if one began January 31st, 2023, and offset by ``1mo_saturating`` until May 31st,
+    the following dates would be generated:
+
+    ``2023-01-31``, ``2023-02-28``, ``2023-03-28``, ``2023-04-28``, ``2023-05-28``.
+
+    This is almost never the intended result. Instead, it is recommended to begin with
+    the first day of the month and use the ``.dt.month_end()`` conversion routine, as
+    in:
+
+    >>> from datetime import date
+    >>> pl.date_range(
+    ...     date(2023, 1, 1), date(2023, 5, 1), "1mo", eager=True
+    ... ).dt.month_end()
+    shape: (5,)
+    Series: 'date' [date]
+    [
+            2023-01-31
+            2023-02-28
+            2023-03-31
+            2023-04-30
+            2023-05-31
+    ]
+
     Returns
     -------
     A Series of type `Datetime` or `Date`.
 
     Examples
     --------
     Using polars duration string to specify the interval:
```

### Comparing `polars_u64_idx-0.18.3/polars/functions/repeat.py` & `polars_u64_idx-0.18.4/polars/functions/repeat.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/polars/functions/whenthen.py` & `polars_u64_idx-0.18.4/polars/functions/whenthen.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/polars/io/__init__.py` & `polars_u64_idx-0.18.4/polars/io/__init__.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/polars/io/_utils.py` & `polars_u64_idx-0.18.4/polars/io/_utils.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/polars/io/avro.py` & `polars_u64_idx-0.18.4/polars/io/avro.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/polars/io/csv/_utils.py` & `polars_u64_idx-0.18.4/polars/io/csv/_utils.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/polars/io/csv/batched_reader.py` & `polars_u64_idx-0.18.4/polars/io/csv/batched_reader.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/polars/io/csv/functions.py` & `polars_u64_idx-0.18.4/polars/io/csv/functions.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/polars/io/database.py` & `polars_u64_idx-0.18.4/polars/io/database.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/polars/io/delta.py` & `polars_u64_idx-0.18.4/polars/io/delta.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/polars/io/excel/_write_utils.py` & `polars_u64_idx-0.18.4/polars/io/excel/_write_utils.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/polars/io/excel/functions.py` & `polars_u64_idx-0.18.4/polars/io/excel/functions.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/polars/io/ipc/anonymous_scan.py` & `polars_u64_idx-0.18.4/polars/io/ipc/anonymous_scan.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/polars/io/ipc/functions.py` & `polars_u64_idx-0.18.4/polars/io/ipc/functions.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/polars/io/ndjson.py` & `polars_u64_idx-0.18.4/polars/io/ndjson.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/polars/io/parquet/anonymous_scan.py` & `polars_u64_idx-0.18.4/polars/io/parquet/anonymous_scan.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/polars/io/parquet/functions.py` & `polars_u64_idx-0.18.4/polars/io/parquet/functions.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/polars/io/pyarrow_dataset/anonymous_scan.py` & `polars_u64_idx-0.18.4/polars/io/pyarrow_dataset/anonymous_scan.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from __future__ import annotations
 
 from functools import partial
 from typing import TYPE_CHECKING
 
 import polars._reexport as pl
-from polars.dependencies import pickle
 from polars.dependencies import pyarrow as pa  # noqa: TCH001
 
 if TYPE_CHECKING:
     from polars import DataFrame, LazyFrame
 
 
 def _scan_pyarrow_dataset(
@@ -27,18 +26,15 @@
     allow_pyarrow_filter
         Allow predicates to be pushed down to pyarrow. This can lead to different
         results if comparisons are done with null values as pyarrow handles this
         different than polars does.
 
     """
     func = partial(_scan_pyarrow_dataset_impl, ds)
-    func_serialized = pickle.dumps(func)
-    return pl.LazyFrame._scan_python_function(
-        ds.schema, func_serialized, allow_pyarrow_filter
-    )
+    return pl.LazyFrame._scan_python_function(ds.schema, func, allow_pyarrow_filter)
 
 
 def _scan_pyarrow_dataset_impl(
     ds: pa.dataset.Dataset,
     with_columns: list[str] | None,
     predicate: str | None,
     n_rows: int | None,
```

### Comparing `polars_u64_idx-0.18.3/polars/io/pyarrow_dataset/functions.py` & `polars_u64_idx-0.18.4/polars/io/pyarrow_dataset/functions.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/polars/lazyframe/frame.py` & `polars_u64_idx-0.18.4/polars/lazyframe/frame.py`

 * *Files 1% similar despite different names*

```diff
@@ -501,15 +501,15 @@
         )
         return self
 
     @classmethod
     def _scan_python_function(
         cls,
         schema: pa.schema | dict[str, PolarsDataType],
-        scan_fn: bytes,
+        scan_fn: Any,
         pyarrow: bool = False,
     ) -> Self:
         self = cls.__new__(cls)
         if isinstance(schema, dict):
             self._ldf = PyLazyFrame.scan_from_python_function_pl_schema(
                 list(schema.items()), scan_fn, pyarrow
             )
@@ -559,15 +559,15 @@
             file = normalise_filepath(file)
 
         return cls._from_pyldf(PyLazyFrame.read_json(file))
 
     @property
     def columns(self) -> list[str]:
         """
-        Get or set column names.
+        Get column names.
 
         Examples
         --------
         >>> lf = pl.LazyFrame(
         ...     {
         ...         "foo": [1, 2, 3],
         ...         "bar": [6, 7, 8],
@@ -671,15 +671,23 @@
 naive plan: (run LazyFrame.explain(optimized=True) to see the optimized plan)
 
 {self.explain(optimized=False)}\
 """
 
     def __repr__(self) -> str:
         # don't expose internal/private classpath
-        return f"<polars.{self.__class__.__name__} object at 0x{id(self):X}>"
+        width = self.width
+        cols_str = "{} col{}".format(width, "" if width == 1 else "s")
+        schema_max_2 = (
+            item for i, item in enumerate(self.schema.items()) if i in (0, width - 1)
+        )
+        schema_str = (", " if width == 2 else " … ").join(
+            (f'"{k}": {v}' for k, v in schema_max_2)
+        )
+        return f"<{self.__class__.__name__} [{cols_str}, {{{schema_str}}}] at 0x{id(self):X}>"
 
     def _repr_html_(self) -> str:
         try:
             dot = self._ldf.to_dot(optimized=False)
             svg = subprocess.check_output(
                 ["dot", "-Nshape=box", "-Tsvg"], input=f"{dot}".encode()
             )
@@ -1006,15 +1014,15 @@
         --------
         >>> lf = pl.LazyFrame({"foo": [1, 1, -2, 3]})
         >>> (
         ...     lf.select(pl.col("foo").cumsum().alias("bar"))
         ...     .inspect()  # print the node before the filter
         ...     .filter(pl.col("bar") == pl.col("foo"))
         ... )  # doctest: +ELLIPSIS
-        <polars.LazyFrame object at ...>
+        <LazyFrame [1 col, {"bar": Int64}] at ...>
 
         """
 
         def inspect(s: DataFrame) -> DataFrame:
             print(fmt.format(s))
             return s
 
@@ -1778,15 +1786,15 @@
         ...     {
         ...         "a": [None, 2, 3, 4],
         ...         "b": [0.5, None, 2.5, 13],
         ...         "c": [True, True, False, None],
         ...     }
         ... )
         >>> lf.lazy()  # doctest: +ELLIPSIS
-        <polars.LazyFrame object at ...>
+        <LazyFrame [3 cols, {"a": Int64 … "c": Boolean}] at ...>
 
         """
         return self
 
     def cache(self) -> Self:
         """Cache the result once the execution of the physical plan hits this node."""
         return self._from_pyldf(self._ldf.cache())
@@ -1853,15 +1861,15 @@
         ...     {
         ...         "a": [None, 2, 3, 4],
         ...         "b": [0.5, None, 2.5, 13],
         ...         "c": [True, True, False, None],
         ...     }
         ... )
         >>> lf.clone()  # doctest: +ELLIPSIS
-        <polars.LazyFrame object at ...>
+        <LazyFrame [3 cols, {"a": Int64 … "c": Boolean}] at ...>
 
         """
         return self._from_pyldf(self._ldf.clone())
 
     def filter(self, predicate: Expr | str | Series | list[bool]) -> Self:
         """
         Filter the rows in the LazyFrame based on a predicate expression.
@@ -2209,15 +2217,15 @@
             This column must be sorted in ascending order. If not the output will not
             make sense.
 
             In case of a rolling groupby on indices, dtype needs to be one of
             {Int32, Int64}. Note that Int32 gets temporarily cast to Int64, so if
             performance matters use an Int64 column.
         period
-            length of the window
+            length of the window - must be non-negative
         offset
             offset of the window. Default is -period
         closed : {'right', 'left', 'both', 'none'}
             Define which sides of the temporal interval are closed (inclusive).
         by
             Also group by this column/these columns
         check_sorted
@@ -2281,15 +2289,15 @@
         └─────────────────────┴───────┴───────┴───────┘
 
         """
         index_column = parse_as_expression(index_column)
         if offset is None:
             offset = f"-{_timedelta_to_pl_duration(period)}"
 
-        pyexprs_by = parse_as_list_of_expressions(by)
+        pyexprs_by = parse_as_list_of_expressions(by) if by is not None else []
         period = _timedelta_to_pl_duration(period)
         offset = _timedelta_to_pl_duration(offset)
 
         lgb = self._ldf.groupby_rolling(
             index_column, period, offset, closed, pyexprs_by, check_sorted
         )
         return LazyGroupBy(lgb)
@@ -2624,15 +2632,15 @@
         if period is None:
             period = every
 
         period = _timedelta_to_pl_duration(period)
         offset = _timedelta_to_pl_duration(offset)
         every = _timedelta_to_pl_duration(every)
 
-        pyexprs_by = parse_as_list_of_expressions(by)
+        pyexprs_by = parse_as_list_of_expressions(by) if by is not None else []
         lgb = self._ldf.groupby_dynamic(
             index_column,
             every,
             period,
             offset,
             truncate,
             include_boundaries,
```

### Comparing `polars_u64_idx-0.18.3/polars/lazyframe/groupby.py` & `polars_u64_idx-0.18.4/polars/lazyframe/groupby.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/polars/selectors.py` & `polars_u64_idx-0.18.4/polars/selectors.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,17 +52,22 @@
             "raw_params": raw_parameters,
             "params": parameters,
             "name": name,
         }
 
     def __invert__(self) -> Self:
         """Invert the selector."""
+        if not hasattr(self, "_attrs"):
+            return ~self.as_expr()  # type: ignore[return-value]
+
         name = self._attrs["name"]
-        if name in ("first", "last", "sub", "and", "or"):
+        if name in ("sub", "and", "or"):
             raise ValueError(f"Cannot currently invert {name!r} selector")
+        elif name in ("first", "last"):
+            return all() - self  # type: ignore[return-value]
 
         params = self._attrs["params"] or {}
         raw_params = self._attrs["raw_params"] or []
         if not raw_params and params:
             raw_params = list(params.values())
 
         if name == "all":
@@ -77,63 +82,82 @@
             name=name,
             parameters=params,
             raw_parameters=raw_params,
             invert=not self._inverted,
         )
 
     def __repr__(self) -> str:
-        params = self._attrs["params"]
-        not_ = "~" if self._inverted else ""
-        str_params = ",".join(f"{k}={v!r}" for k, v in (params or {}).items())
-        return f"{not_}cs.{self._attrs['name']}({str_params})"
+        if not hasattr(self, "_attrs"):
+            return re.sub(
+                r"<[\w.]+_selector_proxy_[\w ]+>", "<selector>", super().__repr__()
+            )
+        else:
+            selector_name, params = self._attrs["name"], self._attrs["params"]
+            set_ops = {"and": "&", "or": "|", "sub": "-"}
+            if selector_name in set_ops:
+                op = set_ops[selector_name]
+                return f" {op} ".join(repr(p) for p in params.values())
+            else:
+                not_ = "~" if self._inverted else ""
+                str_params = ",".join(
+                    (repr(v)[1:-1] if k.startswith("*") else f"{k}={v!r}")
+                    for k, v in (params or {}).items()
+                )
+                return f"{not_}cs.{selector_name}({str_params})"
 
     def __sub__(self, other: Any) -> Expr:  # type: ignore[override]
-        if isinstance(other, _selector_proxy_):
+        if isinstance(other, _selector_proxy_) and hasattr(other, "_attrs"):
             return _selector_proxy_(
-                self.meta._as_selector().meta._selector_sub(other), name="sub"
+                self.meta._as_selector().meta._selector_sub(other),
+                parameters={"self": self, "other": other},
+                name="sub",
             )
         else:
             return self.as_expr().__sub__(other)
 
     def __and__(self, other: Any) -> Expr:  # type: ignore[override]
-        if isinstance(other, _selector_proxy_):
+        if isinstance(other, _selector_proxy_) and hasattr(other, "_attrs"):
             return _selector_proxy_(
-                self.meta._as_selector().meta._selector_and(other), name="and"
+                self.meta._as_selector().meta._selector_and(other),
+                parameters={"self": self, "other": other},
+                name="and",
             )
         else:
             return self.as_expr().__and__(other)
 
     def __or__(self, other: Any) -> Expr:  # type: ignore[override]
-        if isinstance(other, _selector_proxy_):
+        if isinstance(other, _selector_proxy_) and hasattr(other, "_attrs"):
             return _selector_proxy_(
-                self.meta._as_selector().meta._selector_add(other), name="or"
+                self.meta._as_selector().meta._selector_add(other),
+                parameters={"self": self, "other": other},
+                name="or",
             )
         else:
             return self.as_expr().__or__(other)
 
     def __rand__(self, other: Any) -> Expr:  # type: ignore[override]
         # order of operation doesn't matter
-        if isinstance(other, _selector_proxy_):
+        if isinstance(other, _selector_proxy_) and hasattr(other, "_attrs"):
             return self.__and__(other)
         else:
             return self.as_expr().__rand__(other)
 
     def __ror__(self, other: Any) -> Expr:  # type: ignore[override]
         # order of operation doesn't matter
-        if isinstance(other, _selector_proxy_):
+        if isinstance(other, _selector_proxy_) and hasattr(other, "_attrs"):
             return self.__or__(other)
         else:
             return self.as_expr().__ror__(other)
 
     def as_expr(self) -> Expr:
         """
         Materialize the ``selector`` into a normal expression.
 
         This ensures that the operators ``|``, ``&``, ``~`` and ``-``
-        are applied on the data and not no the selector sets.
+        are applied on the data and not on the selector sets.
         """
         return Expr._from_pyexpr(self._pyexpr)
 
 
 def _re_string(string: str | Collection[str]) -> str:
     """Return escaped regex, potentially representing multiple string fragments."""
     if isinstance(string, str):
@@ -345,15 +369,15 @@
                 if not isinstance(n, str):
                     raise TypeError(f"Invalid name: {n!r}")
                 all_names.append(n)
         else:
             TypeError(f"Invalid name: {nm!r}")
 
     return _selector_proxy_(
-        F.col(*all_names), name="by_name", parameters={"names": all_names}
+        F.col(*all_names), name="by_name", parameters={"*names": all_names}
     )
 
 
 def contains(substring: str | Collection[str]) -> Expr:
     """
     Select columns that contain the given literal substring(s).
 
@@ -572,15 +596,15 @@
     """
     escaped_suffix = _re_string(suffix)
     raw_params = f"^.*{escaped_suffix}$"
 
     return _selector_proxy_(
         F.col(raw_params),
         name="ends_with",
-        parameters={"suffix": escaped_suffix},
+        parameters={"*suffix": escaped_suffix},
         raw_parameters=[raw_params],
     )
 
 
 def first() -> Expr:
     """
     Select the first column in the current scope.
@@ -970,15 +994,15 @@
     """
     escaped_prefix = _re_string(prefix)
     raw_params = f"^{escaped_prefix}.*$"
 
     return _selector_proxy_(
         F.col(raw_params),
         name="starts_with",
-        parameters={"prefix": prefix},
+        parameters={"*prefix": prefix},
         raw_parameters=[raw_params],
     )
 
 
 def string(include_categorical: bool = False) -> Expr:
     """
     Select all Utf8 (and, optionally, Categorical) string columns.
```

### Comparing `polars_u64_idx-0.18.3/polars/series/_numpy.py` & `polars_u64_idx-0.18.4/polars/series/_numpy.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/polars/series/array.py` & `polars_u64_idx-0.18.4/polars/series/array.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/polars/series/binary.py` & `polars_u64_idx-0.18.4/polars/series/binary.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/polars/series/categorical.py` & `polars_u64_idx-0.18.4/polars/series/categorical.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/polars/series/datetime.py` & `polars_u64_idx-0.18.4/polars/series/datetime.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/polars/series/list.py` & `polars_u64_idx-0.18.4/polars/series/list.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/polars/series/series.py` & `polars_u64_idx-0.18.4/polars/series/series.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,16 +40,14 @@
     Int8,
     Int16,
     Int32,
     Int64,
     List,
     Object,
     Time,
-    UInt8,
-    UInt16,
     UInt32,
     UInt64,
     Unknown,
     Utf8,
     dtype_to_ctype,
     is_polars_dtype,
     maybe_cast,
@@ -75,14 +73,15 @@
 from polars.series.string import StringNameSpace
 from polars.series.struct import StructNameSpace
 from polars.series.utils import expr_dispatch, get_ffi_func
 from polars.slice import PolarsSlice
 from polars.utils._construction import (
     arrow_to_pyseries,
     iterable_to_pyseries,
+    numpy_to_idxs,
     numpy_to_pyseries,
     pandas_to_pyseries,
     sequence_to_pyseries,
     series_to_pyseries,
 )
 from polars.utils._wrap import wrap_df
 from polars.utils.convert import (
@@ -91,15 +90,14 @@
     _time_to_pl_time,
 )
 from polars.utils.decorators import deprecated_alias
 from polars.utils.meta import get_index_type
 from polars.utils.various import (
     _is_generator,
     find_stacklevel,
-    is_int_sequence,
     parse_version,
     range_to_series,
     range_to_slice,
     scale_bytes,
     sphinx_accessor,
 )
 
@@ -865,149 +863,89 @@
             for idx in range(0, self.len()):
                 yield get_idx(idx)
         else:
             buffer_size = 25_000
             for offset in range(0, self.len(), buffer_size):
                 yield from self.slice(offset, buffer_size).to_list()
 
-    def _pos_idxs(self, idxs: np.ndarray[Any, Any] | Series) -> Series:
+    def _pos_idxs(self, size: int) -> Series:
+        # Unsigned or signed Series (ordered from fastest to slowest).
+        #   - pl.UInt32 (polars) or pl.UInt64 (polars_u64_idx) Series indexes.
+        #   - Other unsigned Series indexes are converted to pl.UInt32 (polars)
+        #     or pl.UInt64 (polars_u64_idx).
+        #   - Signed Series indexes are converted pl.UInt32 (polars) or
+        #     pl.UInt64 (polars_u64_idx) after negative indexes are converted
+        #     to absolute indexes.
+
         # pl.UInt32 (polars) or pl.UInt64 (polars_u64_idx).
         idx_type = get_index_type()
 
-        if isinstance(idxs, Series):
-            if idxs.dtype == idx_type:
-                return idxs
-            if idxs.dtype in {
-                UInt8,
-                UInt16,
-                UInt64 if idx_type == UInt32 else UInt32,
-                Int8,
-                Int16,
-                Int32,
-                Int64,
-            }:
-                if idx_type == UInt32:
-                    if idxs.dtype in {Int64, UInt64}:
-                        if idxs.max() >= 2**32:  # type: ignore[operator]
-                            raise ValueError(
-                                "Index positions should be smaller than 2^32."
-                            )
-                    if idxs.dtype == Int64:
-                        if idxs.min() < -(2**32):  # type: ignore[operator]
-                            raise ValueError(
-                                "Index positions should be bigger than -2^32 + 1."
-                            )
-                if idxs.dtype in SIGNED_INTEGER_DTYPES:
-                    if idxs.min() < 0:  # type: ignore[operator]
-                        if idx_type == UInt32:
-                            if idxs.dtype in {Int8, Int16}:
-                                idxs = idxs.cast(Int32)
-                        else:
-                            if idxs.dtype in {Int8, Int16, Int32}:
-                                idxs = idxs.cast(Int64)
-
-                        # Update negative indexes to absolute indexes.
-                        return (
-                            idxs.to_frame()
-                            .select(
-                                F.when(F.col(idxs.name) < 0)
-                                .then(self.len() + F.col(idxs.name))
-                                .otherwise(F.col(idxs.name))
-                                .cast(idx_type)
-                            )
-                            .to_series(0)
-                        )
-
-                return idxs.cast(idx_type)
-
-        elif _check_for_numpy(idxs) and isinstance(idxs, np.ndarray):
-            if idxs.ndim != 1:
-                raise ValueError("Only 1D numpy array is supported as index.")
-            if idxs.dtype.kind in ("i", "u"):
-                # Numpy array with signed or unsigned integers.
+        if self.dtype == idx_type:
+            return self
+
+        if self.dtype not in INTEGER_DTYPES:
+            raise NotImplementedError("Unsupported idxs datatype.")
+
+        if self.len() == 0:
+            return Series(self.name, [], dtype=idx_type)
 
+        if idx_type == UInt32:
+            if self.dtype in {Int64, UInt64}:
+                if self.max() >= 2**32:  # type: ignore[operator]
+                    raise ValueError("Index positions should be smaller than 2^32.")
+            if self.dtype == Int64:
+                if self.min() < -(2**32):  # type: ignore[operator]
+                    raise ValueError("Index positions should be bigger than -2^32 + 1.")
+
+        if self.dtype in SIGNED_INTEGER_DTYPES:
+            if self.min() < 0:  # type: ignore[operator]
                 if idx_type == UInt32:
-                    if idxs.dtype in {np.int64, np.uint64} and idxs.max() >= 2**32:
-                        raise ValueError("Index positions should be smaller than 2^32.")
-                    if idxs.dtype == np.int64 and idxs.min() < -(2**32):
-                        raise ValueError(
-                            "Index positions should be bigger than -2^32 + 1."
-                        )
-                if idxs.dtype.kind == "i":
-                    if idxs.min() < 0:
-                        if idx_type == UInt32:
-                            if idxs.dtype in (np.int8, np.int16):
-                                idxs = idxs.astype(np.int32)
-                        else:
-                            if idxs.dtype in (np.int8, np.int16, np.int32):
-                                idxs = idxs.astype(np.int64)
-
-                        # Update negative indexes to absolute indexes.
-                        idxs = np.where(idxs < 0, self.len() + idxs, idxs)
-
-                    # Cast signed numpy array to unsigned numpy array as all indexes
-                    # are positive and casting signed Polars Series to unsigned
-                    # Polars series is much slower.
-                    if isinstance(idxs, np.ndarray):
-                        idxs = idxs.astype(
-                            np.uint32 if idx_type == UInt32 else np.uint64
-                        )
+                    idxs = self.cast(Int32) if self.dtype in {Int8, Int16} else self
+                else:
+                    idxs = (
+                        self.cast(Int64) if self.dtype in {Int8, Int16, Int32} else self
+                    )
+
+                # Update negative indexes to absolute indexes.
+                return (
+                    idxs.to_frame()
+                    .select(
+                        F.when(F.col(idxs.name) < 0)
+                        .then(size + F.col(idxs.name))
+                        .otherwise(F.col(idxs.name))
+                        .cast(idx_type)
+                    )
+                    .to_series(0)
+                )
 
-                return Series("", idxs, dtype=idx_type)
+        return self.cast(idx_type)
 
-        raise NotImplementedError("Unsupported idxs datatype.")
+    def _take_with_series(self, s: Series) -> Series:
+        return self._from_pyseries(self._s.take_with_series(s._s))
 
     @overload
     def __getitem__(self, item: int) -> Any:
         ...
 
     @overload
     def __getitem__(
         self,
-        item: Series | range | slice | np.ndarray[Any, Any] | list[int] | list[bool],
+        item: Series | range | slice | np.ndarray[Any, Any] | list[int],
     ) -> Series:
         ...
 
     def __getitem__(
         self,
-        item: (
-            int | Series | range | slice | np.ndarray[Any, Any] | list[int] | list[bool]
-        ),
+        item: (int | Series | range | slice | np.ndarray[Any, Any] | list[int]),
     ) -> Any:
         if isinstance(item, Series) and item.dtype in INTEGER_DTYPES:
-            # Unsigned or signed Series (ordered from fastest to slowest).
-            #   - pl.UInt32 (polars) or pl.UInt64 (polars_u64_idx) Series indexes.
-            #   - Other unsigned Series indexes are converted to pl.UInt32 (polars)
-            #     or pl.UInt64 (polars_u64_idx).
-            #   - Signed Series indexes are converted pl.UInt32 (polars) or
-            #     pl.UInt64 (polars_u64_idx) after negative indexes are converted
-            #     to absolute indexes.
-            return self._from_pyseries(
-                self._s.take_with_series(self._pos_idxs(item)._s)
-            )
+            return self._take_with_series(item._pos_idxs(self.len()))
 
-        elif (
-            _check_for_numpy(item)
-            and isinstance(item, np.ndarray)
-            and item.dtype.kind in ("i", "u")
-        ):
-            if item.ndim != 1:
-                raise ValueError("Only a 1D-Numpy array is supported as index.")
-
-            # Unsigned or signed Numpy array (ordered from fastest to slowest).
-            #   - np.uint32 (polars) or np.uint64 (polars_u64_idx) numpy array
-            #     indexes.
-            #   - Other unsigned numpy array indexes are converted to pl.UInt32
-            #     (polars) or pl.UInt64 (polars_u64_idx).
-            #   - Signed numpy array indexes are converted pl.UInt32 (polars) or
-            #     pl.UInt64 (polars_u64_idx) after negative indexes are converted
-            #     to absolute indexes.
-            return self._from_pyseries(
-                self._s.take_with_series(self._pos_idxs(item)._s)
-            )
+        elif _check_for_numpy(item) and isinstance(item, np.ndarray):
+            return self._take_with_series(numpy_to_idxs(item, self.len()))
 
         # Integer.
         elif isinstance(item, int):
             if item < 0:
                 item = self.len() + item
             return self._s.get_idx(item)
 
@@ -1015,19 +953,24 @@
         elif isinstance(item, slice):
             return PolarsSlice(self).apply(item)
 
         # Range.
         elif isinstance(item, range):
             return self[range_to_slice(item)]
 
-        # Sequence of integers (slow to check if sequence contains all integers).
-        elif is_int_sequence(item):
-            return self._from_pyseries(
-                self._s.take_with_series(self._pos_idxs(Series("", item))._s)
-            )
+        # Sequence of integers (also triggers on empty sequence)
+        elif isinstance(item, Sequence) and (
+            not item or (isinstance(item[0], int) and not isinstance(item[0], bool))  # type: ignore[redundant-expr]
+        ):
+            idx_series = Series("", item, dtype=Int64)._pos_idxs(self.len())
+            if idx_series.has_validity():
+                raise ValueError(
+                    "Cannot __getitem__ with index values containing nulls"
+                )
+            return self._take_with_series(idx_series)
 
         raise ValueError(
             f"Cannot __getitem__ on Series of dtype: '{self.dtype}' "
             f"with argument: '{item}' of type: '{type(item)}'."
         )
 
     def __setitem__(
@@ -1712,15 +1655,15 @@
     ) -> DataFrame:
         """
         Bin values into discrete values based on their quantiles.
 
         Parameters
         ----------
         quantiles
-            Quaniles to create.
+            List of quantiles to create.
             We expect quantiles ``0.0 <= quantile <= 1``
         labels
             Labels to assign to the quantiles. If given the length of labels must be
             len(bins) + 1.
         break_point_label
             Name given to the breakpoint column.
         category_label
```

### Comparing `polars_u64_idx-0.18.3/polars/series/string.py` & `polars_u64_idx-0.18.4/polars/series/string.py`

 * *Files 2% similar despite different names*

```diff
@@ -555,25 +555,30 @@
             "666f6f"
             "626172"
             null
         ]
 
         """
 
-    def json_extract(self, dtype: PolarsDataType | None = None) -> Series:
+    def json_extract(
+        self, dtype: PolarsDataType | None = None, infer_schema_length: int | None = 100
+    ) -> Series:
         """
         Parse string values as JSON.
 
         Throw errors if encounter invalid JSON strings.
 
         Parameters
         ----------
         dtype
             The dtype to cast the extracted value to. If None, the dtype will be
             inferred from the JSON value.
+        infer_schema_length
+            How many rows to parse to determine the schema.
+            If ``None`` all rows are used.
 
         Examples
         --------
         >>> s = pl.Series("json", ['{"a":1, "b": true}', None, '{"a":2, "b": false}'])
         >>> s.str.json_extract()
         shape: (3,)
         Series: 'json' [struct[2]]
@@ -1194,18 +1199,63 @@
             null
             "hippopotamus"
         ]
 
         """
 
     def to_lowercase(self) -> Series:
-        """Modify the strings to their lowercase equivalent."""
+        """
+        Modify the strings to their lowercase equivalent.
+
+        Examples
+        --------
+        >>> s = pl.Series("foo", ["CAT", "DOG"])
+        >>> s.str.to_lowercase()
+        shape: (2,)
+        Series: 'foo' [str]
+        [
+            "cat"
+            "dog"
+        ]
+
+        """
 
     def to_uppercase(self) -> Series:
-        """Modify the strings to their uppercase equivalent."""
+        """
+        Modify the strings to their uppercase equivalent.
+
+        Examples
+        --------
+        >>> s = pl.Series("foo", ["cat", "dog"])
+        >>> s.str.to_uppercase()
+        shape: (2,)
+        Series: 'foo' [str]
+        [
+            "CAT"
+            "DOG"
+        ]
+
+        """
+
+    def to_titlecase(self) -> Series:
+        """
+        Modify the strings to their titlecase equivalent.
+
+        Examples
+        --------
+        >>> s = pl.Series("sing", ["welcome to my world", "THERE'S NO TURNING BACK"])
+        >>> s.str.to_titlecase()
+        shape: (2,)
+        Series: 'sing' [str]
+        [
+            "Welcome To My …
+            "There's No Tur…
+        ]
+
+        """
 
     def slice(self, offset: int, length: int | None = None) -> Series:
         """
         Create subslices of the string values of a Utf8 Series.
 
         Parameters
         ----------
```

### Comparing `polars_u64_idx-0.18.3/polars/series/struct.py` & `polars_u64_idx-0.18.4/polars/series/struct.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/polars/series/utils.py` & `polars_u64_idx-0.18.4/polars/series/utils.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/polars/slice.py` & `polars_u64_idx-0.18.4/polars/slice.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/polars/sql/context.py` & `polars_u64_idx-0.18.4/polars/sql/context.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/polars/string_cache.py` & `polars_u64_idx-0.18.4/polars/string_cache.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/polars/testing/_private.py` & `polars_u64_idx-0.18.4/polars/testing/_private.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/polars/testing/asserts.py` & `polars_u64_idx-0.18.4/polars/testing/asserts.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/polars/testing/parametric/__init__.py` & `polars_u64_idx-0.18.4/polars/testing/parametric/__init__.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/polars/testing/parametric/primitives.py` & `polars_u64_idx-0.18.4/polars/testing/parametric/primitives.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
 import random
 import warnings
 from dataclasses import dataclass
 from math import isfinite
 from textwrap import dedent
-from typing import TYPE_CHECKING, Any, Collection, Sequence
+from typing import TYPE_CHECKING, Any, Collection, Sequence, overload
 
 from hypothesis.errors import InvalidArgument, NonInteractiveExampleWarning
 from hypothesis.strategies import (
     booleans,
     composite,
     lists,
     sampled_from,
@@ -37,19 +37,26 @@
     all_strategies,
     between,
     create_list_strategy,
     scalar_strategies,
 )
 
 if TYPE_CHECKING:
+    import sys
+
     from hypothesis.strategies import DrawFn, SearchStrategy
 
     from polars import LazyFrame
     from polars.type_aliases import OneOrMoreDataTypes, PolarsDataType
 
+    if sys.version_info >= (3, 8):
+        from typing import Literal
+    else:
+        from typing_extensions import Literal
+
 
 _time_units = list(DTYPE_TEMPORAL_UNITS)
 
 
 def empty_list(value: Any, nested: bool) -> bool:
     """Check if value is an empty list, or a list that contains only empty lists."""
     if isinstance(value, list):
@@ -440,19 +447,59 @@
 
     return draw_series()
 
 
 _failed_frame_init_msgs_: set[str] = set()
 
 
+@overload
+def dataframes(
+    cols: int | column | Sequence[column] | None = None,
+    *,
+    lazy: Literal[False] = ...,
+    min_cols: int | None = 0,
+    max_cols: int | None = MAX_COLS,
+    size: int | None = None,
+    min_size: int | None = 0,
+    max_size: int | None = MAX_DATA_SIZE,
+    chunked: bool | None = None,
+    include_cols: Sequence[column] | column | None = None,
+    null_probability: float | dict[str, float] = 0.0,
+    allow_infinities: bool = True,
+    allowed_dtypes: Collection[PolarsDataType] | PolarsDataType | None = None,
+    excluded_dtypes: Collection[PolarsDataType] | PolarsDataType | None = None,
+) -> SearchStrategy[DataFrame]:
+    ...
+
+
+@overload
+def dataframes(
+    cols: int | column | Sequence[column] | None = None,
+    *,
+    lazy: Literal[True],
+    min_cols: int | None = 0,
+    max_cols: int | None = MAX_COLS,
+    size: int | None = None,
+    min_size: int | None = 0,
+    max_size: int | None = MAX_DATA_SIZE,
+    chunked: bool | None = None,
+    include_cols: Sequence[column] | column | None = None,
+    null_probability: float | dict[str, float] = 0.0,
+    allow_infinities: bool = True,
+    allowed_dtypes: Collection[PolarsDataType] | PolarsDataType | None = None,
+    excluded_dtypes: Collection[PolarsDataType] | PolarsDataType | None = None,
+) -> SearchStrategy[LazyFrame]:
+    ...
+
+
 @defines_strategy()
 def dataframes(
     cols: int | column | Sequence[column] | None = None,
-    lazy: bool = False,
     *,
+    lazy: bool = False,
     min_cols: int | None = 0,
     max_cols: int | None = MAX_COLS,
     size: int | None = None,
     min_size: int | None = 0,
     max_size: int | None = MAX_DATA_SIZE,
     chunked: bool | None = None,
     include_cols: Sequence[column] | column | None = None,
```

### Comparing `polars_u64_idx-0.18.3/polars/testing/parametric/profiles.py` & `polars_u64_idx-0.18.4/polars/testing/parametric/profiles.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/polars/testing/parametric/strategies.py` & `polars_u64_idx-0.18.4/polars/testing/parametric/strategies.py`

 * *Files 1% similar despite different names*

```diff
@@ -105,14 +105,16 @@
 )
 strategy_time = times()
 strategy_date = dates()
 strategy_duration = timedeltas(
     min_value=timedelta(microseconds=-(2**46)),
     max_value=timedelta(microseconds=(2**46) - 1),
 )
+strategy_closed = sampled_from(["left", "right", "both", "none"])
+strategy_time_unit = sampled_from(["ns", "us", "ms"])
 
 
 @composite
 def strategy_decimal(draw: DrawFn) -> PyDecimal:
     """Draw a decimal value, varying the number of decimal places."""
     places = draw(integers(min_value=0, max_value=18))
     return draw(
```

### Comparing `polars_u64_idx-0.18.3/polars/type_aliases.py` & `polars_u64_idx-0.18.4/polars/type_aliases.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/polars/utils/__init__.py` & `polars_u64_idx-0.18.4/polars/utils/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 Utility functions.
 
 Functions that are part of the public API are re-exported here.
 """
-from polars.utils._scan import _deserialize_and_execute
+from polars.utils._scan import _execute_from_rust
 from polars.utils.build_info import build_info
 from polars.utils.convert import (
     _date_to_pl_date,
     _datetime_for_anyvalue,
     _datetime_for_anyvalue_windows,
     _time_to_pl_time,
     _timedelta_to_pl_timedelta,
@@ -27,15 +27,15 @@
     "build_info",
     "show_versions",
     "get_idx_type",
     "get_index_type",
     "threadpool_size",
     # Required for Rust bindings
     "_date_to_pl_date",
-    "_deserialize_and_execute",
+    "_execute_from_rust",
     "_time_to_pl_time",
     "_timedelta_to_pl_timedelta",
     "_to_python_date",
     "_to_python_datetime",
     "_to_python_decimal",
     "_to_python_time",
     "_to_python_timedelta",
```

### Comparing `polars_u64_idx-0.18.3/polars/utils/_construction.py` & `polars_u64_idx-0.18.4/polars/utils/_construction.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,14 +32,15 @@
     Datetime,
     Duration,
     Float32,
     List,
     Object,
     Struct,
     Time,
+    UInt32,
     Unknown,
     Utf8,
     dtype_to_py_type,
     is_polars_dtype,
     py_type_to_dtype,
 )
 from polars.datatypes.constructor import (
@@ -57,15 +58,15 @@
     pydantic,
 )
 from polars.dependencies import numpy as np
 from polars.dependencies import pandas as pd
 from polars.dependencies import pyarrow as pa
 from polars.exceptions import ComputeError, ShapeError, TimeZoneAwareConstructorWarning
 from polars.utils._wrap import wrap_df, wrap_s
-from polars.utils.meta import threadpool_size
+from polars.utils.meta import get_index_type, threadpool_size
 from polars.utils.various import _is_generator, arrlen, find_stacklevel, range_to_series
 
 with contextlib.suppress(ImportError):  # Module not available when building docs
     from polars.polars import PyDataFrame, PySeries
 
 if TYPE_CHECKING:
     from polars import DataFrame, Series
@@ -1539,7 +1540,51 @@
             or pa.types.is_uint16(array.type.index_type)
             or pa.types.is_int32(array.type.index_type)
         ):
             array = pc.cast(
                 array, pa.dictionary(pa.uint32(), pa.large_string())
             ).combine_chunks()
     return array
+
+
+def numpy_to_idxs(idxs: np.ndarray[Any, Any], size: int) -> pl.Series:
+    # Unsigned or signed Numpy array (ordered from fastest to slowest).
+    #   - np.uint32 (polars) or np.uint64 (polars_u64_idx) numpy array
+    #     indexes.
+    #   - Other unsigned numpy array indexes are converted to pl.UInt32
+    #     (polars) or pl.UInt64 (polars_u64_idx).
+    #   - Signed numpy array indexes are converted pl.UInt32 (polars) or
+    #     pl.UInt64 (polars_u64_idx) after negative indexes are converted
+    #     to absolute indexes.
+    if idxs.ndim != 1:
+        raise ValueError("Only 1D numpy array is supported as index.")
+
+    idx_type = get_index_type()
+
+    if len(idxs) == 0:
+        return pl.Series("", [], dtype=idx_type)
+
+    # Numpy array with signed or unsigned integers.
+    if idxs.dtype.kind not in ("i", "u"):
+        raise NotImplementedError("Unsupported idxs datatype.")
+
+    if idx_type == UInt32:
+        if idxs.dtype in {np.int64, np.uint64} and idxs.max() >= 2**32:
+            raise ValueError("Index positions should be smaller than 2^32.")
+        if idxs.dtype == np.int64 and idxs.min() < -(2**32):
+            raise ValueError("Index positions should be bigger than -2^32 + 1.")
+
+    if idxs.dtype.kind == "i" and idxs.min() < 0:
+        if idx_type == UInt32:
+            if idxs.dtype in (np.int8, np.int16):
+                idxs = idxs.astype(np.int32)
+        else:
+            if idxs.dtype in (np.int8, np.int16, np.int32):
+                idxs = idxs.astype(np.int64)
+
+        # Update negative indexes to absolute indexes.
+        idxs = np.where(idxs < 0, size + idxs, idxs)
+
+    # numpy conversion is much faster
+    idxs = idxs.astype(np.uint32) if idx_type == UInt32 else idxs.astype(np.uint64)
+
+    return pl.Series("", idxs, dtype=idx_type)
```

### Comparing `polars_u64_idx-0.18.3/polars/utils/_wrap.py` & `polars_u64_idx-0.18.4/polars/utils/_wrap.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/polars/utils/build_info.py` & `polars_u64_idx-0.18.4/polars/utils/build_info.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/polars/utils/convert.py` & `polars_u64_idx-0.18.4/polars/utils/convert.py`

 * *Files 4% similar despite different names*

```diff
@@ -80,26 +80,22 @@
         return f"{d}{s}{us}"
 
 
 def _datetime_to_pl_timestamp(dt: datetime, time_unit: TimeUnit | None) -> int:
     """Convert a python datetime to a timestamp in nanoseconds."""
     dt = dt.replace(tzinfo=timezone.utc)
     if time_unit == "ns":
-        nanos = dt.microsecond * 1000
-        return int(dt.timestamp()) * 1_000_000_000 + nanos
-    elif time_unit == "us":
         micros = dt.microsecond
-        return int(dt.timestamp()) * 1_000_000 + micros
+        return 1_000 * (int(dt.replace(microsecond=0).timestamp() * 1_000_000) + micros)
+    elif time_unit == "us" or time_unit is None:
+        micros = dt.microsecond
+        return int(dt.replace(microsecond=0).timestamp() * 1_000_000) + micros
     elif time_unit == "ms":
         millis = dt.microsecond // 1000
-        return int(dt.timestamp()) * 1_000 + millis
-    elif time_unit is None:
-        # python has us precision
-        micros = dt.microsecond
-        return int(dt.timestamp()) * 1_000_000 + micros
+        return int(dt.replace(microsecond=0).timestamp() * 1_000) + millis
     else:
         raise ValueError(
             f"time_unit must be one of {{'ns', 'us', 'ms'}}, got {time_unit}"
         )
 
 
 def _time_to_pl_time(t: time) -> int:
@@ -209,28 +205,36 @@
     except zoneinfo.ZoneInfoNotFoundError:
         # try fixed offset, which is not supported by ZoneInfo
         _tzinfo = _parse_fixed_tz_offset(time_zone)
 
     return dt.astimezone(_tzinfo)
 
 
-def _datetime_for_anyvalue(dt: datetime) -> tuple[float, int]:
+def _timestamp_in_seconds(dt: datetime) -> int:
+    du = dt - EPOCH_UTC
+    return du.days * 86400 + du.seconds
+
+
+def _datetime_for_anyvalue(dt: datetime) -> tuple[int, int]:
     """Used in pyo3 anyvalue conversion."""
-    if dt.tzinfo is None:
-        dt = dt.replace(tzinfo=timezone.utc)
     # returns (s, ms)
-    return (dt.replace(microsecond=0).timestamp(), dt.microsecond)
+    if dt.tzinfo is None:
+        return (
+            _timestamp_in_seconds(dt.replace(tzinfo=timezone.utc)),
+            dt.microsecond,
+        )
+    return (_timestamp_in_seconds(dt), dt.microsecond)
 
 
 def _datetime_for_anyvalue_windows(dt: datetime) -> tuple[float, int]:
     """Used in pyo3 anyvalue conversion."""
     if dt.tzinfo is None:
         dt = _localize(dt, "UTC")
     # returns (s, ms)
-    return (dt.replace(microsecond=0).timestamp(), dt.microsecond)
+    return (_timestamp_in_seconds(dt), dt.microsecond)
 
 
 # cache here as we have a single tz per column
 # and this function will be called on every conversion
 @lru_cache(16)
 def _parse_fixed_tz_offset(offset: str) -> tzinfo:
     try:
```

### Comparing `polars_u64_idx-0.18.3/polars/utils/decorators.py` & `polars_u64_idx-0.18.4/polars/utils/decorators.py`

 * *Files 11% similar despite different names*

```diff
@@ -37,14 +37,46 @@
             return function(*args, **kwargs)
 
         return wrapper
 
     return deco
 
 
+def warn_closed_future_change() -> Callable[[Callable[P, T]], Callable[P, T]]:
+    """
+    Warn that user should pass in 'closed' as default value will change.
+
+    Decorator for rolling function. Use as follows:
+
+    @warn_closed_future_change()
+    def myfunc():
+        ...
+    """
+
+    def deco(function: Callable[P, T]) -> Callable[P, T]:
+        @wraps(function)
+        def wrapper(*args: P.args, **kwargs: P.kwargs) -> T:
+            # we only warn if 'by' is passed in, otherwise 'closed' is not used
+            if (kwargs.get("by") is not None) and ("closed" not in kwargs):
+                warnings.warn(
+                    message=(
+                        "The default argument for closed, 'left', will be changed to 'right' in the future."
+                        "Fix this warning by explicitly passing in a value for closed"
+                    ),
+                    category=FutureWarning,
+                    stacklevel=find_stacklevel(),
+                )
+
+            return function(*args, **kwargs)
+
+        return wrapper
+
+    return deco
+
+
 def _rename_kwargs(
     func_name: str,
     kwargs: dict[str, object],
     aliases: dict[str, str],
 ) -> None:
     """
     Rename the keyword arguments of a function.
```

### Comparing `polars_u64_idx-0.18.3/polars/utils/meta.py` & `polars_u64_idx-0.18.4/polars/utils/meta.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/polars/utils/polars_version.py` & `polars_u64_idx-0.18.4/polars/utils/polars_version.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/polars/utils/show_versions.py` & `polars_u64_idx-0.18.4/polars/utils/show_versions.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     --------
     >>> pl.show_versions()  # doctest: +SKIP
     --------Version info---------
     Polars:      0.17.11
     Index type:  UInt32
     Platform:    Linux-5.15.90.1-microsoft-standard-WSL2-x86_64-with-glibc2.35
     Python:      3.11.3 (main, Apr 15 2023, 14:44:51) [GCC 11.3.0]
-
+    \b
     ----Optional dependencies----
     numpy:       1.24.2
     pandas:      2.0.0
     pyarrow:     11.0.0
     connectorx:  <not installed>
     deltalake:   0.8.1
     fsspec:      2023.4.0
```

### Comparing `polars_u64_idx-0.18.3/polars/utils/various.py` & `polars_u64_idx-0.18.4/polars/utils/various.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/pyproject.toml` & `polars_u64_idx-0.18.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -83,18 +83,14 @@
   "xlsx2csv",
   "xlsxwriter.*",
   "zoneinfo",
 ]
 ignore_missing_imports = true
 
 [[tool.mypy.overrides]]
-module = ["polars.testing._tempdir"]
-ignore_errors = true
-
-[[tool.mypy.overrides]]
 module = ["IPython.*"]
 follow_imports = "skip"
 
 [[tool.mypy.overrides]]
 module = ["polars.*"]
 # We exclude the polars module from warn_return_any, because the PyO3 api does not have Python
 # type annotations. See https://github.com/PyO3/pyo3/issues/1112 for a discussion on adding
@@ -161,14 +157,15 @@
 
 [tool.ruff.flake8-type-checking]
 strict = true
 
 [tool.ruff.per-file-ignores]
 "polars/datatypes.py" = ["B019"]
 "tests/**/*.py" = ["D100", "D103", "B018"]
+"polars/utils/show_versions.py" = ["D301"]
 
 [tool.pytest.ini_options]
 addopts = [
   "--strict-config",
   "--strict-markers",
   "--import-mode=importlib",
   # Default to running fast tests only. To run ALL tests, run: pytest -m ""
```

### Comparing `polars_u64_idx-0.18.3/requirements-dev.txt` & `polars_u64_idx-0.18.4/requirements-dev.txt`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/scripts/check_stacklevels.py` & `polars_u64_idx-0.18.4/scripts/check_stacklevels.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import subprocess
 import sys
 from ast import NodeVisitor
 
 # Files in which it's OK to set the stacklevel manually.
 # `git ls-files` lists files with forwards-slashes
 # even on Windows, so it's OK to list them like that.
-EXCLUDE = frozenset(["polars/utils/polars_version.py", "polars/testing/_tempdir.py"])
+EXCLUDE = frozenset(["polars/utils/polars_version.py"])
 
 
 class StackLevelChecker(NodeVisitor):
     def __init__(self, file) -> None:
         self.file = file
         self.violations = set()
```

### Comparing `polars_u64_idx-0.18.3/src/apply/dataframe.rs` & `polars_u64_idx-0.18.4/src/apply/dataframe.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/src/apply/lazy.rs` & `polars_u64_idx-0.18.4/src/apply/lazy.rs`

 * *Files 8% similar despite different names*

```diff
@@ -2,53 +2,62 @@
 use pyo3::prelude::*;
 use pyo3::types::PyList;
 
 use crate::py_modules::POLARS;
 use crate::series::PySeries;
 use crate::{PyExpr, Wrap};
 
-trait ToSeries {
-    fn to_series(&self, py: Python, py_polars_module: &PyObject, name: &str) -> Series;
+pub(crate) trait ToSeries {
+    fn to_series(
+        &self,
+        py: Python,
+        py_polars_module: &PyObject,
+        name: &str,
+    ) -> PolarsResult<Series>;
 }
 
 impl ToSeries for PyObject {
-    fn to_series(&self, py: Python, py_polars_module: &PyObject, name: &str) -> Series {
+    fn to_series(
+        &self,
+        py: Python,
+        py_polars_module: &PyObject,
+        name: &str,
+    ) -> PolarsResult<Series> {
         let py_pyseries = match self.getattr(py, "_s") {
             Ok(s) => s,
             // the lambda did not return a series, we try to create a new python Series
             _ => {
                 let res = py_polars_module
                     .getattr(py, "Series")
                     .unwrap()
                     .call1(py, (name, PyList::new(py, [self])));
 
                 match res {
                     Ok(python_s) => python_s.getattr(py, "_s").unwrap(),
                     Err(_) => {
-                        panic!(
+                        polars_bail!(ComputeError:
                             "expected a something that could convert to a `Series` but got: {}",
                             self.as_ref(py).get_type()
                         )
                     }
                 }
             }
         };
         let pyseries = py_pyseries.extract::<PySeries>(py).unwrap();
         // Finally get the actual Series
-        pyseries.series
+        Ok(pyseries.series)
     }
 }
 
 pub(crate) fn call_lambda_with_series(
     py: Python,
     s: Series,
     lambda: &PyObject,
-    polars_module: &PyObject,
 ) -> PyResult<PyObject> {
-    let pypolars = polars_module.downcast::<PyModule>(py).unwrap();
+    let pypolars = POLARS.downcast::<PyModule>(py).unwrap();
 
     // create a PySeries struct/object for Python
     let pyseries = PySeries::new(s);
     // Wrap this PySeries object in the python side Series wrapper
     let python_series_wrapper = pypolars
         .getattr("wrap_s")
         .unwrap()
@@ -101,19 +110,16 @@
                 .with_predicate_pushdown(false)
                 .with_projection_pushdown(false)
                 .collect()?;
 
             let s = out.select_at_idx(0).unwrap().clone();
             PySeries::new(s)
         } else {
-            return Ok(Some(result_series_wrapper.to_series(
-                py,
-                &pypolars.into_py(py),
-                "",
-            )));
+            return Some(result_series_wrapper.to_series(py, &pypolars.into_py(py), ""))
+                .transpose();
         };
 
         // Finally get the actual Series
         Ok(Some(pyseries.series))
     })
 }
 
@@ -121,46 +127,16 @@
     pyexpr: &PyExpr,
     lambda: PyObject,
     output_type: Option<Wrap<DataType>>,
     agg_list: bool,
 ) -> PyExpr {
     let output_type = output_type.map(|wrap| wrap.0);
 
-    let output_type2 = output_type.clone();
-    let function = move |s: Series| {
-        Python::with_gil(|py| {
-            let output_type = output_type2.clone().unwrap_or(DataType::Unknown);
-
-            // this is a python Series
-            let out = call_lambda_with_series(py, s.clone(), &lambda, &POLARS)
-                .map_err(|e| polars_err!(ComputeError: "{}", e))?;
-            let s = out.to_series(py, &POLARS, s.name());
-            polars_ensure!(
-                matches!(output_type, DataType::Unknown) || s.dtype() == &output_type,
-                SchemaMismatch:
-                "expected output type '{:?}', got '{:?}'; set `return_dtype` to the proper datatype",
-                output_type, s.dtype(),
-            );
-            Ok(Some(s))
-        })
-    };
-
-    let output_map = GetOutput::map_field(move |fld| match output_type {
-        Some(ref dt) => Field::new(fld.name(), dt.clone()),
-        None => {
-            let mut fld = fld.clone();
-            fld.coerce(DataType::Unknown);
-            fld
-        }
-    });
-    if agg_list {
-        pyexpr.clone().inner.map_list(function, output_map).into()
-    } else {
-        pyexpr.clone().inner.map(function, output_map).into()
-    }
+    let func = python_udf::PythonUdfExpression::new(lambda, output_type);
+    pyexpr.inner.clone().map_python(func, agg_list).into()
 }
 
 pub(crate) fn call_lambda_with_series_slice(
     py: Python,
     s: &mut [Series],
     lambda: &PyObject,
     polars_module: &PyObject,
@@ -203,15 +179,15 @@
             let out = call_lambda_with_series_slice(py, s, &lambda, &pypolars);
 
             // we return an error, because that will become a null value polars lazy apply list
             if apply_groups && out.is_none(py) {
                 return Ok(None);
             }
 
-            Ok(Some(out.to_series(py, &pypolars, "")))
+            Ok(Some(out.to_series(py, &pypolars, "")?))
         })
     };
 
     let exprs = pyexpr.iter().map(|pe| pe.clone().inner).collect::<Vec<_>>();
 
     let output_map = GetOutput::map_field(move |fld| match output_type {
         Some(ref dt) => Field::new(fld.name(), dt.0.clone()),
```

### Comparing `polars_u64_idx-0.18.3/src/apply/mod.rs` & `polars_u64_idx-0.18.4/src/apply/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/src/apply/series.rs` & `polars_u64_idx-0.18.4/src/apply/series.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/src/arrow_interop/to_py.rs` & `polars_u64_idx-0.18.4/src/arrow_interop/to_py.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/src/arrow_interop/to_rust.rs` & `polars_u64_idx-0.18.4/src/arrow_interop/to_rust.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/src/batched_csv.rs` & `polars_u64_idx-0.18.4/src/batched_csv.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/src/conversion.rs` & `polars_u64_idx-0.18.4/src/conversion.rs`

 * *Files 0% similar despite different names*

```diff
@@ -637,28 +637,28 @@
 fn convert_datetime(ob: &PyAny) -> PyResult<Wrap<AnyValue>> {
     Python::with_gil(|py| {
         // windows
         #[cfg(target_arch = "windows")]
         let (seconds, microseconds) = {
             let convert = UTILS.getattr(py, "_datetime_for_anyvalue_windows").unwrap();
             let out = convert.call1(py, (ob,)).unwrap();
-            let out: (f64, i64) = out.extract(py).unwrap();
+            let out: (i64, i64) = out.extract(py).unwrap();
             out
         };
         // unix
         #[cfg(not(target_arch = "windows"))]
         let (seconds, microseconds) = {
             let convert = UTILS.getattr(py, "_datetime_for_anyvalue").unwrap();
             let out = convert.call1(py, (ob,)).unwrap();
-            let out: (f64, i64) = out.extract(py).unwrap();
+            let out: (i64, i64) = out.extract(py).unwrap();
             out
         };
 
         // s to us
-        let mut v = (seconds as i64) * 1_000_000;
+        let mut v = seconds * 1_000_000;
         v += microseconds;
 
         // choose "us" as that is python's default unit
         Ok(AnyValue::Datetime(v, TimeUnit::Microseconds, &None).into())
     })
 }
```

### Comparing `polars_u64_idx-0.18.3/src/dataframe.rs` & `polars_u64_idx-0.18.4/src/dataframe.rs`

 * *Files 0% similar despite different names*

```diff
@@ -1231,24 +1231,28 @@
         let df = self
             .df
             .quantile(quantile, interpolation.0)
             .map_err(PyPolarsErr::from)?;
         Ok(df.into())
     }
 
+    #[pyo3(signature = (columns, separator, drop_first=false))]
     pub fn to_dummies(
         &self,
         columns: Option<Vec<String>>,
         separator: Option<&str>,
+        drop_first: bool,
     ) -> PyResult<Self> {
         let df = match columns {
-            Some(cols) => self
-                .df
-                .columns_to_dummies(cols.iter().map(|x| x as &str).collect(), separator),
-            None => self.df.to_dummies(separator),
+            Some(cols) => self.df.columns_to_dummies(
+                cols.iter().map(|x| x as &str).collect(),
+                separator,
+                drop_first,
+            ),
+            None => self.df.to_dummies(separator, drop_first),
         }
         .map_err(PyPolarsErr::from)?;
         Ok(df.into())
     }
 
     pub fn null_count(&self) -> Self {
         let df = self.df.null_count();
```

### Comparing `polars_u64_idx-0.18.3/src/datatypes.rs` & `polars_u64_idx-0.18.4/src/datatypes.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/src/error.rs` & `polars_u64_idx-0.18.4/src/error.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/src/expr/array.rs` & `polars_u64_idx-0.18.4/src/expr/array.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/src/expr/binary.rs` & `polars_u64_idx-0.18.4/src/expr/binary.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/src/expr/datetime.rs` & `polars_u64_idx-0.18.4/src/expr/datetime.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/src/expr/general.rs` & `polars_u64_idx-0.18.4/src/expr/general.rs`

 * *Files 0% similar despite different names*

```diff
@@ -455,14 +455,24 @@
     }
 
     #[cfg(feature = "trigonometry")]
     fn arctanh(&self) -> Self {
         self.clone().inner.arctanh().into()
     }
 
+    #[cfg(feature = "trigonometry")]
+    pub fn degrees(&self) -> Self {
+        self.clone().inner.degrees().into()
+    }
+
+    #[cfg(feature = "trigonometry")]
+    pub fn radians(&self) -> Self {
+        self.clone().inner.radians().into()
+    }
+
     #[cfg(feature = "sign")]
     fn sign(&self) -> Self {
         self.clone().inner.sign().into()
     }
 
     fn is_duplicated(&self) -> Self {
         self.clone().inner.is_duplicated().into()
@@ -525,35 +535,30 @@
     fn shrink_dtype(&self) -> Self {
         self.inner.clone().shrink_dtype().into()
     }
 
     #[pyo3(signature = (lambda, window_size, weights, min_periods, center))]
     fn rolling_apply(
         &self,
-        py: Python,
         lambda: PyObject,
         window_size: usize,
         weights: Option<Vec<f64>>,
         min_periods: usize,
         center: bool,
     ) -> Self {
         let options = RollingOptionsFixedWindow {
             window_size,
             weights,
             min_periods,
             center,
             ..Default::default()
         };
-        // get the pypolars module
-        // do the import outside of the function.
-        let pypolars = PyModule::import(py, "polars").unwrap().to_object(py);
-
         let function = move |s: &Series| {
             Python::with_gil(|py| {
-                let out = call_lambda_with_series(py, s.clone(), &lambda, &pypolars)
+                let out = call_lambda_with_series(py, s.clone(), &lambda)
                     .expect("python function failed");
                 match out.getattr(py, "_s") {
                     Ok(pyseries) => {
                         let pyseries = pyseries.extract::<PySeries>(py).unwrap();
                         pyseries.series
                     }
                     Err(_) => {
```

### Comparing `polars_u64_idx-0.18.3/src/expr/list.rs` & `polars_u64_idx-0.18.4/src/expr/list.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/src/expr/meta.rs` & `polars_u64_idx-0.18.4/src/expr/meta.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/src/expr/mod.rs` & `polars_u64_idx-0.18.4/src/expr/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/src/expr/string.rs` & `polars_u64_idx-0.18.4/src/expr/string.rs`

 * *Files 2% similar despite different names*

```diff
@@ -80,14 +80,18 @@
         self.inner.clone().str().to_uppercase().into()
     }
 
     fn str_to_lowercase(&self) -> Self {
         self.inner.clone().str().to_lowercase().into()
     }
 
+    fn str_to_titlecase(&self) -> Self {
+        self.inner.clone().str().to_titlecase().into()
+    }
+
     fn str_lengths(&self) -> Self {
         let function = |s: Series| {
             let ca = s.utf8()?;
             Ok(Some(ca.str_lengths().into_series()))
         };
         self.clone()
             .inner
@@ -211,34 +215,24 @@
             .str()
             .from_radix(radix, strict)
             .with_fmt("str.parse_int")
             .into()
     }
 
     #[cfg(feature = "extract_jsonpath")]
-    fn str_json_extract(&self, dtype: Option<Wrap<DataType>>) -> Self {
+    fn str_json_extract(
+        &self,
+        dtype: Option<Wrap<DataType>>,
+        infer_schema_len: Option<usize>,
+    ) -> Self {
         let dtype = dtype.map(|wrap| wrap.0);
-
-        let output_type = match dtype.clone() {
-            Some(dtype) => GetOutput::from_type(dtype),
-            None => GetOutput::from_type(DataType::Unknown),
-        };
-
-        let function = move |s: Series| {
-            let ca = s.utf8()?;
-            match ca.json_extract(dtype.clone()) {
-                Ok(ca) => Ok(Some(ca.into_series())),
-                Err(e) => Err(PolarsError::ComputeError(format!("{e:?}").into())),
-            }
-        };
-
-        self.clone()
-            .inner
-            .map(function, output_type)
-            .with_fmt("str.json_extract")
+        self.inner
+            .clone()
+            .str()
+            .json_extract(dtype, infer_schema_len)
             .into()
     }
 
     #[cfg(feature = "extract_jsonpath")]
     fn str_json_path_match(&self, pat: String) -> Self {
         let function = move |s: Series| {
             let ca = s.utf8()?;
```

### Comparing `polars_u64_idx-0.18.3/src/file.rs` & `polars_u64_idx-0.18.4/src/file.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/src/functions/eager.rs` & `polars_u64_idx-0.18.4/src/functions/eager.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/src/functions/io.rs` & `polars_u64_idx-0.18.4/src/functions/io.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/src/functions/lazy.rs` & `polars_u64_idx-0.18.4/src/functions/lazy.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/src/functions/meta.rs` & `polars_u64_idx-0.18.4/src/functions/meta.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/src/functions/whenthen.rs` & `polars_u64_idx-0.18.4/src/functions/whenthen.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/src/lazyframe.rs` & `polars_u64_idx-0.18.4/src/lazyframe.rs`

 * *Files 0% similar despite different names*

```diff
@@ -291,25 +291,25 @@
         let lf = LazyFrame::scan_ipc(path, args).map_err(PyPolarsErr::from)?;
         Ok(lf.into())
     }
 
     #[staticmethod]
     fn scan_from_python_function_arrow_schema(
         schema: &PyList,
-        scan_fn: Vec<u8>,
+        scan_fn: PyObject,
         pyarrow: bool,
     ) -> PyResult<Self> {
         let schema = pyarrow_schema_to_rust(schema)?;
         Ok(LazyFrame::scan_from_python_function(schema, scan_fn, pyarrow).into())
     }
 
     #[staticmethod]
     fn scan_from_python_function_pl_schema(
         schema: Vec<(&str, Wrap<DataType>)>,
-        scan_fn: Vec<u8>,
+        scan_fn: PyObject,
         pyarrow: bool,
     ) -> PyResult<Self> {
         let schema = Schema::from_iter(schema.into_iter().map(|(name, dt)| Field::new(name, dt.0)));
         Ok(LazyFrame::scan_from_python_function(schema, scan_fn, pyarrow).into())
     }
 
     fn describe_plan(&self) -> String {
```

### Comparing `polars_u64_idx-0.18.3/src/lazygroupby.rs` & `polars_u64_idx-0.18.4/src/lazygroupby.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/src/lib.rs` & `polars_u64_idx-0.18.4/src/lib.rs`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 pub mod utils;
 
 #[cfg(all(target_os = "linux", not(use_mimalloc)))]
 use jemallocator::Jemalloc;
 #[cfg(any(not(target_os = "linux"), use_mimalloc))]
 use mimalloc::MiMalloc;
 #[cfg(feature = "object")]
-pub use object::register_object_builder;
+pub use object::__register_startup_deps;
 use pyo3::panic::PanicException;
 use pyo3::prelude::*;
 use pyo3::wrap_pyfunction;
 
 use crate::conversion::Wrap;
 use crate::dataframe::PyDataFrame;
 use crate::error::{
@@ -194,15 +194,15 @@
     m.add_wrapped(wrap_pyfunction!(functions::meta::get_float_fmt))
         .unwrap();
 
     // Functions - misc
     m.add_wrapped(wrap_pyfunction!(functions::misc::dtype_str_repr))
         .unwrap();
     #[cfg(feature = "object")]
-    m.add_wrapped(wrap_pyfunction!(register_object_builder))
+    m.add_wrapped(wrap_pyfunction!(__register_startup_deps))
         .unwrap();
 
     // Exceptions
     m.add("ArrowError", py.get_type::<ArrowErrorException>())
         .unwrap();
     m.add("ColumnNotFoundError", py.get_type::<ColumnNotFoundError>())
         .unwrap();
```

### Comparing `polars_u64_idx-0.18.3/src/series/aggregation.rs` & `polars_u64_idx-0.18.4/src/series/aggregation.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/src/series/arithmetic.rs` & `polars_u64_idx-0.18.4/src/series/arithmetic.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/src/series/comparison.rs` & `polars_u64_idx-0.18.4/src/series/comparison.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/src/series/construction.rs` & `polars_u64_idx-0.18.4/src/series/construction.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/src/series/export.rs` & `polars_u64_idx-0.18.4/src/series/export.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/src/series/mod.rs` & `polars_u64_idx-0.18.4/src/series/mod.rs`

 * *Files 2% similar despite different names*

```diff
@@ -534,18 +534,19 @@
         let s = self
             .series
             .zip_with(mask, &other.series)
             .map_err(PyPolarsErr::from)?;
         Ok(s.into())
     }
 
-    fn to_dummies(&self, separator: Option<&str>) -> PyResult<PyDataFrame> {
+    #[pyo3(signature = (separator, drop_first=false))]
+    fn to_dummies(&self, separator: Option<&str>, drop_first: bool) -> PyResult<PyDataFrame> {
         let df = self
             .series
-            .to_dummies(separator)
+            .to_dummies(separator, drop_first)
             .map_err(PyPolarsErr::from)?;
         Ok(df.into())
     }
 
     fn get_list(&self, index: usize) -> Option<Self> {
         if let Ok(ca) = &self.series.list() {
             let s = ca.get(index);
```

### Comparing `polars_u64_idx-0.18.3/src/series/numpy_ufunc.rs` & `polars_u64_idx-0.18.4/src/series/numpy_ufunc.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/src/series/set_at_idx.rs` & `polars_u64_idx-0.18.4/src/series/set_at_idx.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/src/sql.rs` & `polars_u64_idx-0.18.4/src/sql.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/src/utils.rs` & `polars_u64_idx-0.18.4/src/utils.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/tests/README.md` & `polars_u64_idx-0.18.4/tests/README.md`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/tests/benchmark/groupby-datagen.R` & `polars_u64_idx-0.18.4/tests/benchmark/groupby-datagen.R`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/tests/benchmark/run_h2oai_benchmark.py` & `polars_u64_idx-0.18.4/tests/benchmark/run_h2oai_benchmark.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/tests/benchmark/test_release.py` & `polars_u64_idx-0.18.4/tests/benchmark/test_release.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/tests/docs/run_doctest.py` & `polars_u64_idx-0.18.4/tests/docs/run_doctest.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/tests/parametric/test_dataframe.py` & `polars_u64_idx-0.18.4/tests/parametric/test_dataframe.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/tests/parametric/test_lazyframe.py` & `polars_u64_idx-0.18.4/tests/parametric/test_lazyframe.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/tests/parametric/test_series.py` & `polars_u64_idx-0.18.4/tests/parametric/test_series.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/tests/parametric/test_testing.py` & `polars_u64_idx-0.18.4/tests/parametric/test_testing.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/tests/unit/conftest.py` & `polars_u64_idx-0.18.4/tests/unit/conftest.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/tests/unit/datatypes/test_array.py` & `polars_u64_idx-0.18.4/tests/unit/datatypes/test_array.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/tests/unit/datatypes/test_binary.py` & `polars_u64_idx-0.18.4/tests/unit/datatypes/test_binary.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/tests/unit/datatypes/test_bool.py` & `polars_u64_idx-0.18.4/tests/unit/datatypes/test_bool.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/tests/unit/datatypes/test_categorical.py` & `polars_u64_idx-0.18.4/tests/unit/datatypes/test_categorical.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/tests/unit/datatypes/test_decimal.py` & `polars_u64_idx-0.18.4/tests/unit/datatypes/test_decimal.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/tests/unit/datatypes/test_duration.py` & `polars_u64_idx-0.18.4/tests/unit/datatypes/test_duration.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/tests/unit/datatypes/test_list.py` & `polars_u64_idx-0.18.4/tests/unit/datatypes/test_list.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/tests/unit/datatypes/test_object.py` & `polars_u64_idx-0.18.4/tests/unit/datatypes/test_object.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/tests/unit/datatypes/test_struct.py` & `polars_u64_idx-0.18.4/tests/unit/datatypes/test_struct.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/tests/unit/datatypes/test_temporal.py` & `polars_u64_idx-0.18.4/tests/unit/datatypes/test_temporal.py`

 * *Files 0% similar despite different names*

```diff
@@ -1925,15 +1925,15 @@
     ), pytest.warns(
         FutureWarning,
         match="time zones other than those in `zoneinfo.available_timezones",
     ):
         pl.Series(["2020-01-01 03:00:00"]).str.strptime(pl.Datetime("us", "foo"))
     with pytest.raises(
         ComputeError,
-        match="cannot use strptime with both a tz-aware format and a tz-aware dtype",
+        match="Please either drop the time zone from the function call, or set it to UTC",
     ):
         pl.Series(["2020-01-01 03:00:00+01:00"]).str.strptime(
             pl.Datetime("us", "foo"), "%Y-%m-%d %H:%M:%S%z"
         )
 
 
 def test_utc_deprecation() -> None:
```

### Comparing `polars_u64_idx-0.18.3/tests/unit/functions/test_as_datatype.py` & `polars_u64_idx-0.18.4/tests/unit/functions/test_as_datatype.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/tests/unit/functions/test_functions.py` & `polars_u64_idx-0.18.4/tests/unit/functions/test_functions.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/tests/unit/functions/test_range.py` & `polars_u64_idx-0.18.4/tests/unit/functions/test_range.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/tests/unit/functions/test_repeat.py` & `polars_u64_idx-0.18.4/tests/unit/functions/test_repeat.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/tests/unit/io/files/delta-table/_delta_log/00000000000000000000.json` & `polars_u64_idx-0.18.4/tests/unit/io/files/delta-table/_delta_log/00000000000000000000.json`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/tests/unit/io/files/delta-table/_delta_log/00000000000000000001.json` & `polars_u64_idx-0.18.4/tests/unit/io/files/delta-table/_delta_log/00000000000000000001.json`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/tests/unit/io/files/delta-table/part-00000-e42312d7-60e5-454d-acbc-db192d220e73-c000.snappy.parquet` & `polars_u64_idx-0.18.4/tests/unit/io/files/delta-table/part-00000-e42312d7-60e5-454d-acbc-db192d220e73-c000.snappy.parquet`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/tests/unit/io/files/delta-table/part-00000-e4a999da-df45-4fb0-bdc4-d999fc0f58aa-c000.snappy.parquet` & `polars_u64_idx-0.18.4/tests/unit/io/files/delta-table/part-00000-e4a999da-df45-4fb0-bdc4-d999fc0f58aa-c000.snappy.parquet`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/tests/unit/io/files/example.xlsx` & `polars_u64_idx-0.18.4/tests/unit/io/files/example.xlsx`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/tests/unit/io/files/foods1.ipc` & `polars_u64_idx-0.18.4/tests/unit/io/files/foods1.ipc`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/tests/unit/io/files/foods1.ndjson` & `polars_u64_idx-0.18.4/tests/unit/io/files/foods1.ndjson`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/tests/unit/io/files/foods1.parquet` & `polars_u64_idx-0.18.4/tests/unit/io/files/foods1.parquet`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/tests/unit/io/files/foods2.ipc` & `polars_u64_idx-0.18.4/tests/unit/io/files/foods2.ipc`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/tests/unit/io/files/foods2.ndjson` & `polars_u64_idx-0.18.4/tests/unit/io/files/foods2.ndjson`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/tests/unit/io/files/foods2.parquet` & `polars_u64_idx-0.18.4/tests/unit/io/files/foods2.parquet`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/tests/unit/io/files/small.parquet` & `polars_u64_idx-0.18.4/tests/unit/io/files/small.parquet`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/tests/unit/io/test_avro.py` & `polars_u64_idx-0.18.4/tests/unit/io/test_avro.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/tests/unit/io/test_csv.py` & `polars_u64_idx-0.18.4/tests/unit/io/test_csv.py`

 * *Files 3% similar despite different names*

```diff
@@ -772,14 +772,44 @@
             ],
             "d": [2, 3],
         }
     )
     assert_frame_equal(result, expected)
 
 
+@pytest.mark.parametrize("try_parse_dates", [True, False])
+@pytest.mark.parametrize("time_unit", ["ms", "us", "ns"])
+def test_csv_overwrite_datetime_dtype(
+    try_parse_dates: bool, time_unit: TimeUnit
+) -> None:
+    data = """\
+    a
+    2020-1-1T00:00:00.123456789
+    2020-1-2T00:00:00.987654321
+    2020-1-3T00:00:00.132547698
+    """
+    result = pl.read_csv(
+        io.StringIO(data),
+        try_parse_dates=try_parse_dates,
+        dtypes={"a": pl.Datetime(time_unit)},
+    )
+    expected = pl.DataFrame(
+        {
+            "a": pl.Series(
+                [
+                    "2020-01-01T00:00:00.123456789",
+                    "2020-01-02T00:00:00.987654321",
+                    "2020-01-03T00:00:00.132547698",
+                ]
+            ).str.to_datetime(time_unit=time_unit)
+        }
+    )
+    assert_frame_equal(result, expected)
+
+
 def test_csv_string_escaping() -> None:
     df = pl.DataFrame({"a": ["Free trip to A,B", '''Special rate "1.79"''']})
     f = io.BytesIO()
     df.write_csv(f)
     f.seek(0)
     df_read = pl.read_csv(f)
     assert_frame_equal(df_read, df)
```

### Comparing `polars_u64_idx-0.18.3/tests/unit/io/test_database.py` & `polars_u64_idx-0.18.4/tests/unit/io/test_database.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/tests/unit/io/test_delta.py` & `polars_u64_idx-0.18.4/tests/unit/io/test_delta.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/tests/unit/io/test_excel.py` & `polars_u64_idx-0.18.4/tests/unit/io/test_excel.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/tests/unit/io/test_ipc.py` & `polars_u64_idx-0.18.4/tests/unit/io/test_ipc.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/tests/unit/io/test_json.py` & `polars_u64_idx-0.18.4/tests/unit/io/test_json.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/tests/unit/io/test_lazy_csv.py` & `polars_u64_idx-0.18.4/tests/unit/io/test_lazy_csv.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/tests/unit/io/test_lazy_ipc.py` & `polars_u64_idx-0.18.4/tests/unit/io/test_lazy_ipc.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/tests/unit/io/test_lazy_json.py` & `polars_u64_idx-0.18.4/tests/unit/io/test_lazy_json.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/tests/unit/io/test_lazy_parquet.py` & `polars_u64_idx-0.18.4/tests/unit/io/test_lazy_parquet.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/tests/unit/io/test_other.py` & `polars_u64_idx-0.18.4/tests/unit/io/test_other.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/tests/unit/io/test_parquet.py` & `polars_u64_idx-0.18.4/tests/unit/io/test_parquet.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/tests/unit/io/test_pickle.py` & `polars_u64_idx-0.18.4/tests/unit/io/test_pickle.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/tests/unit/io/test_pyarrow_dataset.py` & `polars_u64_idx-0.18.4/tests/unit/io/test_pyarrow_dataset.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/tests/unit/namespaces/test_array.py` & `polars_u64_idx-0.18.4/tests/unit/namespaces/test_array.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/tests/unit/namespaces/test_binary.py` & `polars_u64_idx-0.18.4/tests/unit/namespaces/test_binary.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/tests/unit/namespaces/test_categorical.py` & `polars_u64_idx-0.18.4/tests/unit/namespaces/test_categorical.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/tests/unit/namespaces/test_datetime.py` & `polars_u64_idx-0.18.4/tests/unit/namespaces/test_datetime.py`

 * *Files 2% similar despite different names*

```diff
@@ -109,14 +109,40 @@
     )
     result = ser.dt.datetime()
     expected = datetime(2022, 1, 1, 23)
     assert result.dtype == pl.Datetime(time_unit, None)
     assert result.item() == expected
 
 
+@pytest.mark.parametrize(
+    ("time_zone", "expected"),
+    [
+        (None, True),
+        ("Asia/Kathmandu", False),
+        ("UTC", True),
+    ],
+)
+@pytest.mark.parametrize("attribute", ["datetime", "date"])
+def test_local_datetime_sortedness(
+    time_zone: str | None, expected: bool, attribute: str
+) -> None:
+    ser = (pl.Series([datetime(2022, 1, 1, 23)]).dt.replace_time_zone(time_zone)).sort()
+    result = getattr(ser.dt, attribute)()
+    assert result.flags["SORTED_ASC"] == expected
+    assert result.flags["SORTED_DESC"] is False
+
+
+@pytest.mark.parametrize("time_zone", [None, "Asia/Kathmandu", "UTC"])
+def test_local_time_sortedness(time_zone: str | None) -> None:
+    ser = (pl.Series([datetime(2022, 1, 1, 23)]).dt.replace_time_zone(time_zone)).sort()
+    result = ser.dt.time()
+    assert result.flags["SORTED_ASC"] is False
+    assert result.flags["SORTED_DESC"] is False
+
+
 def test_dt_datetime_date_time_invalid() -> None:
     with pytest.raises(ComputeError, match="expected Datetime"):
         pl.Series([date(2021, 1, 2)]).dt.datetime()
     with pytest.raises(ComputeError, match="expected Datetime or Date"):
         pl.Series([time(23)]).dt.date()
     with pytest.raises(ComputeError, match="expected Datetime"):
         pl.Series([time(23)]).dt.datetime()
```

### Comparing `polars_u64_idx-0.18.3/tests/unit/namespaces/test_list.py` & `polars_u64_idx-0.18.4/tests/unit/namespaces/test_list.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/tests/unit/namespaces/test_meta.py` & `polars_u64_idx-0.18.4/tests/unit/namespaces/test_meta.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/tests/unit/namespaces/test_string.py` & `polars_u64_idx-0.18.4/tests/unit/namespaces/test_string.py`

 * *Files 1% similar despite different names*

```diff
@@ -697,7 +697,29 @@
 
     expected = pl.DataFrame(
         {"field_0": ["a", None, "b", "c"], "field_1": ["a", None, None, "c_c"]}
     )
 
     assert_frame_equal(out, expected)
     assert_frame_equal(df["x"].str.splitn("_", 2).to_frame().unnest("x"), expected)
+
+
+def test_titlecase() -> None:
+    df = pl.DataFrame(
+        {
+            "sing": [
+                "welcome to my world",
+                "THERE'S NO TURNING BACK",
+                "double  space",
+                "and\ta\t tab",
+            ]
+        }
+    )
+
+    assert df.select(pl.col("sing").str.to_titlecase()).to_dict(False) == {
+        "sing": [
+            "Welcome To My World",
+            "There's No Turning Back",
+            "Double  Space",
+            "And\tA\t Tab",
+        ]
+    }
```

### Comparing `polars_u64_idx-0.18.3/tests/unit/namespaces/test_strptime.py` & `polars_u64_idx-0.18.4/tests/unit/namespaces/test_strptime.py`

 * *Files 3% similar despite different names*

```diff
@@ -265,21 +265,47 @@
         time_unit=time_unit
     )
     assert result.dtype == pl.Datetime(time_unit, "UTC")
     assert result.item() == datetime(2020, 1, 2, 2, 0, tzinfo=timezone.utc)
 
 
 def test_infer_tz_aware_raises() -> None:
-    msg = "cannot parse tz-aware values with tz-aware dtype - please drop the time zone from the dtype"
+    msg = "Please either drop the time zone from the function call, or set it to UTC"
     with pytest.raises(ComputeError, match=msg):
         pl.Series(["2020-01-02T04:00:00+02:00"]).str.to_datetime(
             time_unit="us", time_zone="Europe/Vienna"
         )
 
 
+@pytest.mark.parametrize(
+    "result",
+    [
+        pl.Series(["2020-01-01T00:00:00+00:00"]).str.strptime(
+            pl.Datetime("us", "UTC"), format="%Y-%m-%dT%H:%M:%S%z"
+        ),
+        pl.Series(["2020-01-01T00:00:00+00:00"]).str.strptime(
+            pl.Datetime("us"), format="%Y-%m-%dT%H:%M:%S%z"
+        ),
+        pl.Series(["2020-01-01T00:00:00+00:00"]).str.strptime(pl.Datetime("us", "UTC")),
+        pl.Series(["2020-01-01T00:00:00+00:00"]).str.strptime(pl.Datetime("us")),
+        pl.Series(["2020-01-01T00:00:00+00:00"]).str.to_datetime(
+            time_zone="UTC", format="%Y-%m-%dT%H:%M:%S%z"
+        ),
+        pl.Series(["2020-01-01T00:00:00+00:00"]).str.to_datetime(
+            format="%Y-%m-%dT%H:%M:%S%z"
+        ),
+        pl.Series(["2020-01-01T00:00:00+00:00"]).str.to_datetime(time_zone="UTC"),
+        pl.Series(["2020-01-01T00:00:00+00:00"]).str.to_datetime(),
+    ],
+)
+def test_parsing_offset_aware_with_utc_dtype(result: pl.Series) -> None:
+    expected = pl.Series([datetime(2020, 1, 1, tzinfo=timezone.utc)])
+    assert_series_equal(result, expected)
+
+
 def test_datetime_strptime_patterns_consistent() -> None:
     # note that all should be year first
     df = pl.Series(
         "date",
         [
             "2018-09-05",
             "2018-09-05T04:05:01",
```

### Comparing `polars_u64_idx-0.18.3/tests/unit/namespaces/test_struct.py` & `polars_u64_idx-0.18.4/tests/unit/namespaces/test_struct.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/tests/unit/operations/test_aggregations.py` & `polars_u64_idx-0.18.4/tests/unit/operations/test_aggregations.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/tests/unit/operations/test_apply.py` & `polars_u64_idx-0.18.4/tests/unit/operations/test_apply.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/tests/unit/operations/test_arithmetic.py` & `polars_u64_idx-0.18.4/tests/unit/operations/test_arithmetic.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/tests/unit/operations/test_comparison.py` & `polars_u64_idx-0.18.4/tests/unit/operations/test_comparison.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/tests/unit/operations/test_drop.py` & `polars_u64_idx-0.18.4/tests/unit/operations/test_drop.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/tests/unit/operations/test_explode.py` & `polars_u64_idx-0.18.4/tests/unit/operations/test_explode.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/tests/unit/operations/test_filter.py` & `polars_u64_idx-0.18.4/tests/unit/operations/test_filter.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/tests/unit/operations/test_folds.py` & `polars_u64_idx-0.18.4/tests/unit/operations/test_folds.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/tests/unit/operations/test_groupby.py` & `polars_u64_idx-0.18.4/tests/unit/operations/test_groupby.py`

 * *Files 0% similar despite different names*

```diff
@@ -119,15 +119,16 @@
     expected = ["a", "b", "c"]
     assert df.groupby(["a", "b"]).agg("c").columns == expected
     # Column names as positional arguments
     assert df.groupby("a", "b").agg("c").columns == expected
     # With keyword argument
     assert df.groupby("a", "b", maintain_order=True).agg("c").columns == expected
     # Mixed
-    assert df.groupby(["a"], "b", maintain_order=True).agg("c").columns == expected
+    with pytest.deprecated_call():
+        assert df.groupby(["a"], "b", maintain_order=True).agg("c").columns == expected
     # Multiple aggregations as list
     assert df.groupby("a").agg(["b", "c"]).columns == expected
     # Multiple aggregations as positional arguments
     assert df.groupby("a").agg("b", "c").columns == expected
     # Multiple aggregations as keyword arguments
     assert df.groupby("a").agg(q="b", r="c").columns == ["a", "q", "r"]
```

### Comparing `polars_u64_idx-0.18.3/tests/unit/operations/test_groupby_rolling.py` & `polars_u64_idx-0.18.4/tests/unit/operations/test_groupby_rolling.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/tests/unit/operations/test_is_in.py` & `polars_u64_idx-0.18.4/tests/unit/operations/test_is_in.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/tests/unit/operations/test_join.py` & `polars_u64_idx-0.18.4/tests/unit/operations/test_join.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/tests/unit/operations/test_join_asof.py` & `polars_u64_idx-0.18.4/tests/unit/operations/test_join_asof.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/tests/unit/operations/test_melt.py` & `polars_u64_idx-0.18.4/tests/unit/operations/test_melt.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/tests/unit/operations/test_pivot.py` & `polars_u64_idx-0.18.4/tests/unit/operations/test_pivot.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/tests/unit/operations/test_rolling.py` & `polars_u64_idx-0.18.4/tests/unit/operations/test_rolling.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 import typing
 from datetime import date, datetime, timedelta
 from typing import TYPE_CHECKING
 
 import pytest
 from numpy import nan
 
+from polars.exceptions import ComputeError
+
 if sys.version_info >= (3, 9):
     from zoneinfo import ZoneInfo
 else:
     # Import from submodule due to typing issue with backports.zoneinfo package:
     # https://github.com/pganssle/zoneinfo/issues/125
     from backports.zoneinfo._zoneinfo import ZoneInfo
 
@@ -66,14 +68,104 @@
                 pl.col("values").std().alias("std"),
             ]
         )
     )
     assert_frame_equal(out1, out2)
 
 
+@pytest.mark.parametrize(
+    ("offset", "closed", "expected_values"),
+    [
+        pytest.param(
+            "-1d",
+            "left",
+            [[1], [1, 2], [2, 3], [3, 4]],
+            id="partial lookbehind, left",
+        ),
+        pytest.param(
+            "-1d",
+            "right",
+            [[1, 2], [2, 3], [3, 4], [4]],
+            id="partial lookbehind, right",
+        ),
+        pytest.param(
+            "-1d",
+            "both",
+            [[1, 2], [1, 2, 3], [2, 3, 4], [3, 4]],
+            id="partial lookbehind, both",
+        ),
+        pytest.param(
+            "-1d",
+            "none",
+            [[1], [2], [3], [4]],
+            id="partial lookbehind, none",
+        ),
+        pytest.param(
+            "-2d",
+            "left",
+            [[], [1], [1, 2], [2, 3]],
+            id="full lookbehind, left",
+        ),
+        pytest.param(
+            "-3d",
+            "left",
+            [[], [], [1], [1, 2]],
+            id="full lookbehind, offset > period, left",
+        ),
+        pytest.param(
+            "-3d",
+            "right",
+            [[], [1], [1, 2], [2, 3]],
+            id="full lookbehind, right",
+        ),
+        pytest.param(
+            "-3d",
+            "both",
+            [[], [1], [1, 2], [1, 2, 3]],
+            id="full lookbehind, both",
+        ),
+        pytest.param(
+            "-2d",
+            "none",
+            [[], [1], [2], [3]],
+            id="full lookbehind, none",
+        ),
+        pytest.param(
+            "-3d",
+            "none",
+            [[], [], [1], [2]],
+            id="full lookbehind, offset > period, none",
+        ),
+    ],
+)
+def test_rolling_negative_offset(
+    offset: str, closed: ClosedInterval, expected_values: list[list[int]]
+) -> None:
+    df = pl.DataFrame(
+        {
+            "ts": pl.date_range(
+                datetime(2021, 1, 1), datetime(2021, 1, 4), "1d", eager=True
+            ),
+            "value": [1, 2, 3, 4],
+        }
+    )
+    result = df.groupby_rolling("ts", period="2d", offset=offset, closed=closed).agg(
+        pl.col("value")
+    )
+    expected = pl.DataFrame(
+        {
+            "ts": pl.date_range(
+                datetime(2021, 1, 1), datetime(2021, 1, 4), "1d", eager=True
+            ),
+            "value": expected_values,
+        }
+    )
+    assert_frame_equal(result, expected)
+
+
 def test_rolling_skew() -> None:
     s = pl.Series([1, 2, 3, 3, 2, 10, 8])
     assert s.rolling_skew(window_size=4, bias=True).to_list() == pytest.approx(
         [
             None,
             None,
             None,
@@ -112,15 +204,17 @@
 def test_rolling_crossing_dst(
     time_zone: str | None, rolling_fn: str, expected_values: list[int | None | float]
 ) -> None:
     ts = pl.date_range(
         datetime(2021, 11, 5), datetime(2021, 11, 10), "1d", time_zone="UTC", eager=True
     ).dt.replace_time_zone(time_zone)
     df = pl.DataFrame({"ts": ts, "value": [1, 2, 3, 4, 5, 6]})
-    result = df.with_columns(getattr(pl.col("value"), rolling_fn)("1d", by="ts"))
+    result = df.with_columns(
+        getattr(pl.col("value"), rolling_fn)("1d", by="ts", closed="left")
+    )
     expected = pl.DataFrame({"ts": ts, "value": expected_values})
     assert_frame_equal(result, expected)
 
 
 def test_rolling_extrema() -> None:
     # sorted data and nulls flags trigger different kernels
     df = (
@@ -607,14 +701,38 @@
         ((1, date(2020, 1, 1)), (1, 3)),
         ((2, date(2020, 1, 2)), (1, 3)),
         ((2, date(2020, 1, 5)), (1, 3)),
     ]
     assert result2 == expected2
 
 
+def test_groupby_rolling_negative_period() -> None:
+    df = pl.DataFrame({"ts": [datetime(2020, 1, 1)], "value": [1]}).with_columns(
+        pl.col("ts").set_sorted()
+    )
+    with pytest.raises(
+        ComputeError, match="rolling window period should be strictly positive"
+    ):
+        df.groupby_rolling("ts", period="-1d", offset="-1d").agg(pl.col("value"))
+    with pytest.raises(
+        ComputeError, match="rolling window period should be strictly positive"
+    ):
+        df.lazy().groupby_rolling("ts", period="-1d", offset="-1d").agg(
+            pl.col("value")
+        ).collect()
+    with pytest.raises(ComputeError, match="window size should be strictly positive"):
+        df.select(
+            pl.col("value").rolling_min(by="ts", window_size="-1d", closed="left")
+        )
+    with pytest.raises(ComputeError, match="window size should be strictly positive"):
+        df.lazy().select(
+            pl.col("value").rolling_min(by="ts", window_size="-1d", closed="left")
+        ).collect()
+
+
 def test_rolling_skew_window_offset() -> None:
     assert (pl.arange(0, 20, eager=True) ** 2).rolling_skew(20)[
         -1
     ] == 0.6612545648596286
 
 
 def test_rolling_kernels_groupby_dynamic_7548() -> None:
@@ -654,7 +772,38 @@
 def test_rolling_window_size_9160() -> None:
     assert pl.Series([1, 5]).rolling_apply(
         lambda x: sum(x), window_size=2, min_periods=1
     ).to_list() == [1, 6]
     assert pl.Series([1]).rolling_apply(
         lambda x: sum(x), window_size=2, min_periods=1
     ).to_list() == [1]
+
+
+def test_rolling_empty_window_9406() -> None:
+    datecol = pl.Series(
+        "d",
+        [datetime(2019, 1, x) for x in [16, 17, 18, 22, 23]],
+        dtype=pl.Datetime(time_unit="us", time_zone=None),
+    )
+    rawdata = pl.Series("x", [1.1, 1.2, 1.3, 1.15, 1.25], dtype=pl.Float64)
+    rmin = pl.Series("x", [None, 1.1, 1.1, None, 1.15], dtype=pl.Float64)
+    rmax = pl.Series("x", [None, 1.1, 1.2, None, 1.15], dtype=pl.Float64)
+    df = pl.DataFrame([datecol, rawdata])
+
+    assert_frame_equal(
+        pl.DataFrame([datecol, rmax]),
+        df.select(
+            [
+                pl.col("d"),
+                pl.col("x").rolling_max(by="d", window_size="3d", closed="left"),
+            ]
+        ),
+    )
+    assert_frame_equal(
+        pl.DataFrame([datecol, rmin]),
+        df.select(
+            [
+                pl.col("d"),
+                pl.col("x").rolling_min(by="d", window_size="3d", closed="left"),
+            ]
+        ),
+    )
```

### Comparing `polars_u64_idx-0.18.3/tests/unit/operations/test_select.py` & `polars_u64_idx-0.18.4/tests/unit/operations/test_select.py`

 * *Files 18% similar despite different names*

```diff
@@ -30,25 +30,41 @@
 
     # Keyword arguments
     result = ldf.select(oof="foo")
     expected = pl.LazyFrame({"oof": [1, 2]})
     assert_frame_equal(result, expected)
 
     # Mixed
-    result = ldf.select(["bar"], "foo", oof="foo")
+    result = ldf.select("bar", "foo", oof="foo")
     expected = pl.LazyFrame({"bar": [3, 4], "foo": [1, 2], "oof": [1, 2]})
     assert_frame_equal(result, expected)
 
 
+def test_select_mixed_deprecated() -> None:
+    ldf = pl.LazyFrame({"foo": [1, 2], "bar": [3, 4], "ham": ["a", "b"]})
+
+    with pytest.deprecated_call():
+        result = ldf.select(["bar"], "foo")
+    expected = pl.LazyFrame({"bar": [3, 4], "foo": [1, 2]})
+    assert_frame_equal(result, expected)
+
+
 def test_select_empty() -> None:
     result = pl.select()
     expected = pl.DataFrame()
     assert_frame_equal(result, expected)
 
 
+def test_select_none() -> None:
+    with pytest.deprecated_call():
+        result = pl.select(None)
+    expected = pl.DataFrame()
+    assert_frame_equal(result, expected)
+
+
 def test_select_empty_list() -> None:
     result = pl.select([])
     expected = pl.DataFrame()
     assert_frame_equal(result, expected)
 
 
 def test_select_named_inputs_reserved() -> None:
```

### Comparing `polars_u64_idx-0.18.3/tests/unit/operations/test_sort.py` & `polars_u64_idx-0.18.4/tests/unit/operations/test_sort.py`

 * *Files 0% similar despite different names*

```diff
@@ -488,15 +488,16 @@
     assert_frame_equal(result, expected)
 
     # Column names as positional arguments
     result = df.sort("a", "b")
     assert_frame_equal(result, expected)
 
     # Mixed
-    result = df.sort(["a"], "b")
+    with pytest.deprecated_call():
+        result = df.sort(["a"], "b")
     assert_frame_equal(result, expected)
 
     # nulls_last
     result = df.sort("a", nulls_last=True)
     assert_frame_equal(result, df)
```

### Comparing `polars_u64_idx-0.18.3/tests/unit/operations/test_statistics.py` & `polars_u64_idx-0.18.4/tests/unit/operations/test_statistics.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/tests/unit/operations/test_transpose.py` & `polars_u64_idx-0.18.4/tests/unit/operations/test_transpose.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/tests/unit/operations/test_unique.py` & `polars_u64_idx-0.18.4/tests/unit/operations/test_unique.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/tests/unit/operations/test_window.py` & `polars_u64_idx-0.18.4/tests/unit/operations/test_window.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/tests/unit/operations/test_with_columns.py` & `polars_u64_idx-0.18.4/tests/unit/operations/test_with_columns.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,25 +75,26 @@
         j="a",  # Note: string interpreted as column name, resolves to `pl.col("a")`
         k=None,
         l=datetime.datetime(2001, 1, 1, 0, 0),
     )
     assert_frame_equal(dx, expected)
 
     # mixed
-    dx = df.with_columns(
-        [(pl.col("a") * pl.col("b")).alias("d")],
-        ~pl.col("c").alias("e"),
-        f=srs_unnamed,
-        g=True,
-        h=1,
-        i=3.2,
-        j="a",  # Note: string interpreted as column name, resolves to `pl.col("a")`
-        k=None,
-        l=datetime.datetime(2001, 1, 1, 0, 0),
-    )
+    with pytest.deprecated_call():
+        dx = df.with_columns(
+            [(pl.col("a") * pl.col("b")).alias("d")],
+            ~pl.col("c").alias("e"),
+            f=srs_unnamed,
+            g=True,
+            h=1,
+            i=3.2,
+            j="a",  # Note: string interpreted as column name, resolves to `pl.col("a")`
+            k=None,
+            l=datetime.datetime(2001, 1, 1, 0, 0),
+        )
     assert_frame_equal(dx, expected)
 
     # automatically upconvert multi-output expressions to struct
     with pl.Config() as cfg:
         cfg.set_auto_structify(True)
 
         ldf = (
```

### Comparing `polars_u64_idx-0.18.3/tests/unit/streaming/test_ooc.py` & `polars_u64_idx-0.18.4/tests/unit/streaming/test_ooc.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/tests/unit/streaming/test_streaming.py` & `polars_u64_idx-0.18.4/tests/unit/streaming/test_streaming.py`

 * *Files 10% similar despite different names*

```diff
@@ -526,7 +526,78 @@
         .groupby(["id2", "id3", "id3_right"])
         .agg(
             pl.col("value").apply(lambda x: x).sum() * pl.col("value").sum()
         )  # non-streamable UDF + nested_agg
     )
 
     assert """--- PIPELINE""" in res.explain(streaming=True)
+
+
+def test_streaming_sortedness_propagation_9494() -> None:
+    assert (
+        pl.DataFrame(
+            {
+                "when": [date(2023, 5, 10), date(2023, 5, 20), date(2023, 6, 10)],
+                "what": [1, 2, 3],
+            }
+        )
+        .lazy()
+        .sort("when")
+        .groupby_dynamic("when", every="1mo")
+        .agg(pl.col("what").sum())
+        .collect(streaming=True)
+    ).to_dict(False) == {"when": [date(2023, 5, 1), date(2023, 6, 1)], "what": [3, 3]}
+
+
+@pytest.mark.write_disk()
+def test_out_of_core_sort_9503(monkeypatch: Any) -> None:
+    monkeypatch.setenv("POLARS_FORCE_OOC", "1")
+    np.random.seed(0)
+
+    num_rows = 1_00_000
+    num_columns = 2
+    num_tables = 10
+
+    # ensure we create many chunks
+    # this will ensure we create more files
+    # and that creates contention while dumping
+    q = pl.concat(
+        [
+            pl.DataFrame(
+                [
+                    pl.Series(np.random.randint(0, 10000, size=num_rows))
+                    for _ in range(num_columns)
+                ]
+            )
+            for _ in range(num_tables)
+        ],
+        rechunk=False,
+    ).lazy()
+    q = q.sort(q.columns)
+    df = q.collect(streaming=True)
+    assert df.shape == (1_000_000, 2)
+    assert df["column_0"].flags["SORTED_ASC"]
+    assert df.head(20).to_dict(False) == {
+        "column_0": [0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0],
+        "column_1": [
+            242,
+            245,
+            588,
+            618,
+            732,
+            902,
+            925,
+            945,
+            1009,
+            1161,
+            1352,
+            1365,
+            1451,
+            1581,
+            1778,
+            1836,
+            1976,
+            2091,
+            2120,
+            2124,
+        ],
+    }
```

### Comparing `polars_u64_idx-0.18.3/tests/unit/test_api.py` & `polars_u64_idx-0.18.4/tests/unit/test_api.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/tests/unit/test_arity.py` & `polars_u64_idx-0.18.4/tests/unit/test_arity.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/tests/unit/test_cfg.py` & `polars_u64_idx-0.18.4/tests/unit/test_cfg.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/tests/unit/test_constructors.py` & `polars_u64_idx-0.18.4/tests/unit/test_constructors.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,22 +13,22 @@
 
 import polars as pl
 from polars.dependencies import _ZONEINFO_AVAILABLE, dataclasses, pydantic
 from polars.exceptions import TimeZoneAwareConstructorWarning
 from polars.testing import assert_frame_equal, assert_series_equal
 from polars.utils._construction import type_hints
 
+if sys.version_info >= (3, 8):
+    from typing import Literal
+else:
+    from typing_extensions import Literal  # noqa: TCH002
+
 if TYPE_CHECKING:
     from polars.datatypes import PolarsDataType
 
-    if sys.version_info >= (3, 8):
-        from typing import Literal
-    else:
-        from typing_extensions import Literal
-
 if sys.version_info >= (3, 9):
     from zoneinfo import ZoneInfo
 elif _ZONEINFO_AVAILABLE:
     # Import from submodule due to typing issue with backports.zoneinfo package:
     # https://github.com/pganssle/zoneinfo/issues/125
     from backports.zoneinfo._zoneinfo import ZoneInfo
 
@@ -178,14 +178,26 @@
     # empty nested objects
     for empty_val in [None, "", {}, []]:  # type: ignore[var-annotated]
         test = [{"field": {"sub_field": empty_val, "sub_field_2": 2}}]
         df = pl.DataFrame(test, schema={"field": pl.Object})
         assert df.to_dict(False)["field"][0] == test[0]["field"]
 
 
+@no_type_check
+def test_error_string_dtypes() -> None:
+    with pytest.raises(ValueError, match="Cannot infer dtype"):
+        pl.DataFrame(
+            data={"x": [1, 2], "y": [3, 4], "z": [5, 6]},
+            schema={"x": "i16", "y": "i32", "z": "f32"},
+        )
+
+    with pytest.raises(ValueError, match="not a valid Polars data type"):
+        pl.Series("n", [1, 2, 3], dtype="f32")
+
+
 def test_init_structured_objects(monkeypatch: Any) -> None:
     # validate init from dataclass, namedtuple, and pydantic model objects
     monkeypatch.setenv("POLARS_ACTIVATE_DECIMAL", "1")
 
     @dataclasses.dataclass
     class TradeDC:
         timestamp: datetime
```

### Comparing `polars_u64_idx-0.18.3/tests/unit/test_cse.py` & `polars_u64_idx-0.18.4/tests/unit/test_cse.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/tests/unit/test_datatypes.py` & `polars_u64_idx-0.18.4/tests/unit/test_datatypes.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/tests/unit/test_df.py` & `polars_u64_idx-0.18.4/tests/unit/test_df.py`

 * *Files 1% similar despite different names*

```diff
@@ -814,22 +814,14 @@
     a = df.shift(1)
     b = pl.DataFrame(
         {"A": [None, "a", "b"], "B": [None, 1, 3]},
     )
     assert_frame_equal(a, b)
 
 
-def test_to_dummies() -> None:
-    df = pl.DataFrame({"A": ["a", "b", "c"], "B": [1, 3, 5]})
-    dummies = df.to_dummies()
-    assert dummies["A_a"].to_list() == [1, 0, 0]
-    assert dummies["A_b"].to_list() == [0, 1, 0]
-    assert dummies["A_c"].to_list() == [0, 0, 1]
-
-
 def test_custom_groupby() -> None:
     df = pl.DataFrame({"a": [1, 2, 1, 1], "b": ["a", "b", "c", "c"]})
     out = df.groupby("b", maintain_order=True).agg(
         [pl.col("a").apply(lambda x: x.sum(), return_dtype=pl.Int64)]
     )
     assert out.rows() == [("a", 1), ("b", 2), ("c", 2)]
 
@@ -873,17 +865,25 @@
 
 
 def test_arg_where() -> None:
     s = pl.Series([True, False, True, False])
     assert_series_equal(pl.arg_where(s, eager=True).cast(int), pl.Series([0, 2]))
 
 
-def test_to_dummies2() -> None:
+def test_to_dummies() -> None:
+    df = pl.DataFrame({"A": ["a", "b", "c"], "B": [1, 3, 5]})
+    dummies = df.to_dummies()
+
+    assert dummies["A_a"].to_list() == [1, 0, 0]
+    assert dummies["A_b"].to_list() == [0, 1, 0]
+    assert dummies["A_c"].to_list() == [0, 0, 1]
+
     df = pl.DataFrame({"a": [1, 2, 3]})
     res = df.to_dummies()
+
     expected = pl.DataFrame(
         {"a_1": [1, 0, 0], "a_2": [0, 1, 0], "a_3": [0, 0, 1]}
     ).with_columns(pl.all().cast(pl.UInt8))
     assert_frame_equal(res, expected)
 
     df = pl.DataFrame(
         {"i": [1, 2, 3], "category": ["dog", "cat", "cat"]},
@@ -902,14 +902,35 @@
 
     # test sorted fast path
     assert pl.DataFrame({"x": pl.arange(0, 3, eager=True)}).to_dummies("x").to_dict(
         False
     ) == {"x_0": [1, 0, 0], "x_1": [0, 1, 0], "x_2": [0, 0, 1]}
 
 
+def test_to_dummies_drop_first() -> None:
+    df = pl.DataFrame(
+        {
+            "foo": [0, 1, 2],
+            "bar": [3, 4, 5],
+            "baz": ["x", "y", "z"],
+        }
+    )
+    dm = df.to_dummies()
+    dd = df.to_dummies(drop_first=True)
+
+    assert dd.columns == ["foo_1", "foo_2", "bar_4", "bar_5", "baz_y", "baz_z"]
+    assert set(dm.columns) - set(dd.columns) == {"foo_0", "bar_3", "baz_x"}
+    assert dm.select(dd.columns).frame_equal(dd)
+    assert dd.rows() == [
+        (0, 0, 0, 0, 0, 0),
+        (1, 0, 1, 0, 1, 0),
+        (0, 1, 0, 1, 0, 1),
+    ]
+
+
 def test_to_pandas(df: pl.DataFrame) -> None:
     # pyarrow cannot deal with unsigned dictionary integer yet.
     # pyarrow cannot convert a time64 w/ non-zero nanoseconds
     df = df.drop(["cat", "time"])
     df.to_arrow()
     df.to_pandas()
     # test shifted df
@@ -2541,17 +2562,30 @@
 
     # range, refers to rows
     assert_frame_equal(df[range(1, 3)], pl.DataFrame({"a": [2.0, 3.0], "b": [4, 5]}))
 
     # slice. Below an example of taking every second row
     assert_frame_equal(df[1::2], pl.DataFrame({"a": [2.0, 4.0], "b": [4, 6]}))
 
+    # slice, empty slice
+    assert df[:0].columns == ["a", "b"]
+    assert len(df[:0]) == 0
+
+    # make mypy happy
+    empty: list[int] = []
+
+    # empty list with column selector drops rows but keeps columns
+    assert_frame_equal(df[empty, :], df[:0])
+
+    # empty list without column select return empty frame
+    assert_frame_equal(df[empty], pl.DataFrame({}))
+
     # numpy array: assumed to be row indices if integers, or columns if strings
 
-    # numpy array: positive idxs.
+    # numpy array: positive idxs and empty idx
     for np_dtype in (
         np.int8,
         np.int16,
         np.int32,
         np.int64,
         np.uint8,
         np.uint16,
@@ -2560,14 +2594,15 @@
     ):
         assert_frame_equal(
             df[np.array([1, 0, 3, 2, 3, 0], dtype=np_dtype)],
             pl.DataFrame(
                 {"a": [2.0, 1.0, 4.0, 3.0, 4.0, 1.0], "b": [4, 3, 6, 5, 6, 3]}
             ),
         )
+        assert df[np.array([], dtype=np_dtype)].columns == ["a", "b"]
 
     # numpy array: positive and negative idxs.
     for np_dtype in (np.int8, np.int16, np.int32, np.int64):
         assert_frame_equal(
             df[np.array([-1, 0, -3, -2, 3, -4], dtype=np_dtype)],
             pl.DataFrame(
                 {"a": [4.0, 1.0, 2.0, 3.0, 4.0, 1.0], "b": [6, 3, 4, 5, 6, 3]}
@@ -2589,15 +2624,15 @@
         df[[1, -4, -1, 2, 1]],
         pl.DataFrame({"a": [2.0, 1.0, 4.0, 3.0, 2.0], "b": [4, 3, 6, 5, 4]}),
     )
 
     # pl.Series: strings for column selections.
     assert_frame_equal(df[pl.Series("", ["a", "b"])], df)
 
-    # pl.Series: positive idxs for row selection.
+    # pl.Series: positive idxs or empty idxs for row selection.
     for pl_dtype in (
         pl.Int8,
         pl.Int16,
         pl.Int32,
         pl.Int64,
         pl.UInt8,
         pl.UInt16,
@@ -2606,14 +2641,15 @@
     ):
         assert_frame_equal(
             df[pl.Series("", [1, 0, 3, 2, 3, 0], dtype=pl_dtype)],
             pl.DataFrame(
                 {"a": [2.0, 1.0, 4.0, 3.0, 4.0, 1.0], "b": [4, 3, 6, 5, 6, 3]}
             ),
         )
+        assert df[pl.Series("", [], dtype=pl_dtype)].columns == ["a", "b"]
 
     # pl.Series: positive and negative idxs for row selection.
     for pl_dtype in (pl.Int8, pl.Int16, pl.Int32, pl.Int64):
         assert_frame_equal(
             df[pl.Series("", [-1, 0, -3, -2, 3, -4], dtype=pl_dtype)],
             pl.DataFrame(
                 {"a": [4.0, 1.0, 2.0, 3.0, 4.0, 1.0], "b": [6, 3, 4, 5, 6, 3]}
```

### Comparing `polars_u64_idx-0.18.3/tests/unit/test_empty.py` & `polars_u64_idx-0.18.4/tests/unit/test_empty.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/tests/unit/test_errors.py` & `polars_u64_idx-0.18.4/tests/unit/test_errors.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/tests/unit/test_expr_multi_cols.py` & `polars_u64_idx-0.18.4/tests/unit/test_expr_multi_cols.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/tests/unit/test_exprs.py` & `polars_u64_idx-0.18.4/tests/unit/test_exprs.py`

 * *Files 0% similar despite different names*

```diff
@@ -919,21 +919,37 @@
         0,
         8,
         [1, 2, 3],
     )
 
 
 def test_incompatible_lit_dtype() -> None:
-    with pytest.raises(TypeError, match="Cannot cast tz-aware value to tz-aware dtype"):
+    with pytest.raises(
+        TypeError,
+        match=r"Time zone of dtype \(Asia/Kathmandu\) differs from time zone of value \(UTC\).",
+    ):
         pl.lit(
             datetime(2020, 1, 1, tzinfo=timezone.utc),
             dtype=pl.Datetime("us", "Asia/Kathmandu"),
         )
 
 
+def test_lit_dtype_utc() -> None:
+    result = pl.select(
+        pl.lit(
+            datetime(2020, 1, 1, tzinfo=ZoneInfo("Asia/Kathmandu")),
+            dtype=pl.Datetime("us", "Asia/Kathmandu"),
+        )
+    )
+    expected = pl.DataFrame(
+        {"literal": [datetime(2019, 12, 31, 18, 15, tzinfo=timezone.utc)]}
+    ).select(pl.col("literal").dt.convert_time_zone("Asia/Kathmandu"))
+    assert_frame_equal(result, expected)
+
+
 @pytest.mark.parametrize(
     ("input", "expected"),
     [
         (("a",), ["b", "c"]),
         (("a", "b"), ["c"]),
         ((["a", "b"],), ["c"]),
         ((pl.Int64,), ["c"]),
```

### Comparing `polars_u64_idx-0.18.3/tests/unit/test_fmt.py` & `polars_u64_idx-0.18.4/tests/unit/test_fmt.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/tests/unit/test_interchange.py` & `polars_u64_idx-0.18.4/tests/unit/test_interchange.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/tests/unit/test_interop.py` & `polars_u64_idx-0.18.4/tests/unit/test_interop.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/tests/unit/test_lazy.py` & `polars_u64_idx-0.18.4/tests/unit/test_lazy.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import annotations
 
+import warnings
 from datetime import date, datetime
 from functools import reduce
 from inspect import signature
 from operator import add
 from string import ascii_letters
 from typing import TYPE_CHECKING, Any, cast
 
@@ -51,14 +52,28 @@
     # │ optimization ┆ 0     ┆ 69  │
     # │ groupby(a)   ┆ 69    ┆ 342 │
     # └──────────────┴───────┴─────┘
     assert len(profiling_info) == 2
     assert profiling_info[1].columns == ["node", "start", "end"]
 
 
+@pytest.mark.parametrize(
+    ("data", "repr_"),
+    [
+        ({}, "0 cols, {}"),
+        ({"a": [1]}, '1 col, {"a": Int64}'),
+        ({"a": [1], "b": ["B"]}, '2 cols, {"a": Int64, "b": Utf8}'),
+        ({"a": [1], "b": ["B"], "c": [0.0]}, '3 cols, {"a": Int64 … "c": Float64}'),
+    ],
+)
+def test_repr(data: dict[str, list[Any]], repr_: str) -> None:
+    ldf = pl.LazyFrame(data)
+    assert repr(ldf).startswith(f"<LazyFrame [{repr_}] at ")
+
+
 def test_lazyframe_membership_operator() -> None:
     ldf = pl.LazyFrame({"name": ["Jane", "John"], "age": [20, 30]})
     assert "name" in ldf
     assert "phone" not in ldf
 
     # note: cannot use lazyframe in boolean context
     with pytest.raises(ValueError, match="ambiguous"):
@@ -707,14 +722,35 @@
         ]
     ).collect()
 
     assert cast(float, out_single_val_variance[0, "std"]) == 0.0
     assert cast(float, out_single_val_variance[0, "var"]) == 0.0
 
 
+def test_rolling_closed_decorator() -> None:
+    # no warning if we do not use by
+    with warnings.catch_warnings():
+        warnings.simplefilter("error")
+        _ = pl.col("a").rolling_min(2)
+
+    # if we pass in a by, but no closed, we expect a warning
+    with pytest.warns(FutureWarning):
+        _ = pl.col("a").rolling_min(2, by="b")
+
+    # if we pass in a by and a closed, we expect no warning
+    with warnings.catch_warnings():
+        warnings.simplefilter("error")
+        _ = pl.col("a").rolling_min(2, by="b", closed="left")
+
+    # regardless of the value
+    with warnings.catch_warnings():
+        warnings.simplefilter("error")
+        _ = pl.col("a").rolling_min(2, by="b", closed="right")
+
+
 def test_arr_namespace(fruits_cars: pl.DataFrame) -> None:
     ldf = fruits_cars.lazy()
     out = ldf.select(
         [
             "fruits",
             pl.col("B")
             .over("fruits", mapping_strategy="join")
@@ -975,14 +1011,33 @@
             pl.corr("prediction", "target", method="spearman").alias("c"),
         )
     ).collect()["c"]
     assert np.isclose(out[0], 0.5)
     assert np.isclose(out[1], -1.0)
 
 
+def test_spearman_corr_ties() -> None:
+    """In Spearman correlation, ranks are computed using the average method ."""
+    df = pl.DataFrame({"a": [1, 1, 1, 2, 3, 7, 4], "b": [4, 3, 2, 2, 4, 3, 1]})
+
+    result = df.select(
+        pl.corr("a", "b", method="spearman").alias("a1"),
+        pl.corr(pl.col("a").rank("min"), pl.col("b").rank("min")).alias("a2"),
+        pl.corr(pl.col("a").rank(), pl.col("b").rank()).alias("a3"),
+    )
+    expected = pl.DataFrame(
+        [
+            pl.Series("a1", [-0.19048483669757843], dtype=pl.Float32),
+            pl.Series("a2", [-0.17223653586587362], dtype=pl.Float64),
+            pl.Series("a3", [-0.19048483669757843], dtype=pl.Float32),
+        ]
+    )
+    assert_frame_equal(result, expected)
+
+
 def test_pearson_corr() -> None:
     ldf = pl.LazyFrame(
         {
             "era": [1, 1, 1, 2, 2, 2],
             "prediction": [2, 4, 5, 190, 1, 4],
             "target": [1, 3, 2, 1, 43, 3],
         }
```

### Comparing `polars_u64_idx-0.18.3/tests/unit/test_polars_import.py` & `polars_u64_idx-0.18.4/tests/unit/test_polars_import.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/tests/unit/test_predicates.py` & `polars_u64_idx-0.18.4/tests/unit/test_predicates.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/tests/unit/test_projections.py` & `polars_u64_idx-0.18.4/tests/unit/test_projections.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/tests/unit/test_queries.py` & `polars_u64_idx-0.18.4/tests/unit/test_queries.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/tests/unit/test_rows.py` & `polars_u64_idx-0.18.4/tests/unit/test_rows.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/tests/unit/test_schema.py` & `polars_u64_idx-0.18.4/tests/unit/test_schema.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/tests/unit/test_selectors.py` & `polars_u64_idx-0.18.4/tests/unit/test_selectors.py`

 * *Files 23% similar despite different names*

```diff
@@ -106,14 +106,18 @@
     ]
 
 
 def test_selector_first_last(df: pl.DataFrame) -> None:
     assert df.select(cs.first()).columns == ["abc"]
     assert df.select(cs.last()).columns == ["qqR"]
 
+    all_columns = set(df.columns)
+    assert set(df.select(~cs.first()).columns) == (all_columns - {"abc"})
+    assert set(df.select(~cs.last()).columns) == (all_columns - {"qqR"})
+
 
 def test_selector_float(df: pl.DataFrame) -> None:
     assert df.select(cs.float()).schema == {
         "cde": pl.Float64,
         "def": pl.Float32,
     }
     all_columns = set(df.columns)
@@ -221,14 +225,23 @@
     s2 = pl.col(["b", "c", "d"])
 
     s = s1.meta._as_selector()
     s = s.meta._selector_and(s2)
     assert df.select(s).columns == ["b", "c"]
 
 
+def test_selector_repr() -> None:
+    assert repr(cs.all() - cs.first()) == "cs.all() - cs.first()"
+    assert repr(~cs.starts_with("a", "b")) == "~cs.starts_with('a', 'b')"
+    assert repr(cs.float() | cs.by_name("x")) == "cs.float() | cs.by_name('x')"
+    assert (
+        repr(cs.integer() & cs.matches("z")) == "cs.integer() & cs.matches(pattern='z')"
+    )
+
+
 def test_selector_sets(df: pl.DataFrame) -> None:
     # or
     assert df.select(cs.temporal() | cs.string() | cs.starts_with("e")).schema == {
         "eee": pl.Boolean,
         "ghi": pl.Time,
         "JJK": pl.Date,
         "Lmn": pl.Duration,
@@ -268,7 +281,53 @@
     expected = pl.DataFrame(
         {
             "a": [2, 2],
             "b": [3, 3],
         }
     )
     assert_frame_equal(out, expected)
+
+
+def test_selector_expr_dispatch() -> None:
+    df = pl.DataFrame(
+        data={
+            "colx": [float("inf"), -1, float("nan"), 25],
+            "coly": [1, float("-inf"), 10, float("nan")],
+        },
+        schema={"colx": pl.Float64, "coly": pl.Float32},
+    )
+    expected = pl.DataFrame(
+        data={
+            "colx": [0.0, -1.0, 0.0, 25.0],
+            "coly": [1.0, 0.0, 10.0, 0.0],
+        },
+        schema={"colx": pl.Float64, "coly": pl.Float32},
+    )
+
+    # basic selector-broadcast expression
+    assert_frame_equal(
+        expected,
+        df.with_columns(
+            pl.when(cs.float().is_finite()).then(cs.float()).otherwise(0.0).keep_name()
+        ),
+    )
+
+    # inverted selector-broadcast expression
+    assert_frame_equal(
+        expected,
+        df.with_columns(
+            pl.when(~cs.float().is_finite()).then(0.0).otherwise(cs.float()).keep_name()
+        ),
+    )
+
+    # check that "as_expr" behaves, both explicitly and implicitly
+    for nan_or_inf in (
+        cs.float().is_nan().as_expr() | cs.float().is_infinite().as_expr(),  # type: ignore[attr-defined]
+        cs.float().is_nan().as_expr() | cs.float().is_infinite(),  # type: ignore[attr-defined]
+        cs.float().is_nan() | cs.float().is_infinite(),
+    ):
+        assert_frame_equal(
+            expected,
+            df.with_columns(
+                pl.when(nan_or_inf).then(0.0).otherwise(cs.float()).keep_name()
+            ).fill_null(0),
+        )
```

### Comparing `polars_u64_idx-0.18.3/tests/unit/test_serde.py` & `polars_u64_idx-0.18.4/tests/unit/test_serde.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 from __future__ import annotations
 
 import pickle
+import typing
 from datetime import datetime, timedelta
 
+import pytest
+
 import polars as pl
 from polars.testing import assert_frame_equal, assert_series_equal
 
 
 def test_pickling_simple_expression() -> None:
     e = pl.col("foo").sum()
     buf = pickle.dumps(e)
@@ -94,7 +97,46 @@
 
 def test_expression_json() -> None:
     e = pl.col("foo").sum().over("bar")
     json = e.meta.write_json()
 
     round_tripped = pl.Expr.from_json(json)
     assert round_tripped.meta == e
+
+
+@typing.no_type_check
+def times2(x):
+    return x * 2
+
+
+def test_pickle_udf_expression() -> None:
+    df = pl.DataFrame({"a": [1, 2, 3]})
+
+    e = pl.col("a").map(times2)
+    b = pickle.dumps(e)
+    e = pickle.loads(b)
+
+    assert df.select(e).to_dict(False) == {"a": [2, 4, 6]}
+
+    e = pl.col("a").map(times2, return_dtype=pl.Utf8)
+    b = pickle.dumps(e)
+    e = pickle.loads(b)
+
+    # tests that 'GetOutput' is also deserialized
+    with pytest.raises(
+        pl.SchemaError,
+        match=r"expected output type 'Utf8', got 'Int64'; set `return_dtype` to the proper datatype",
+    ):
+        df.select(e)
+
+
+def test_pickle_small_integers() -> None:
+    df = pl.DataFrame(
+        [
+            pl.Series([1, 2], dtype=pl.Int16),
+            pl.Series([3, 2], dtype=pl.Int8),
+            pl.Series([32, 2], dtype=pl.UInt8),
+            pl.Series([3, 3], dtype=pl.UInt16),
+        ]
+    )
+    b = pickle.dumps(df)
+    assert_frame_equal(pickle.loads(b), df)
```

### Comparing `polars_u64_idx-0.18.3/tests/unit/test_series.py` & `polars_u64_idx-0.18.4/tests/unit/test_series.py`

 * *Files 0% similar despite different names*

```diff
@@ -808,30 +808,37 @@
 
 def test_get() -> None:
     a = pl.Series("a", [1, 2, 3])
     pos_idxs = pl.Series("idxs", [2, 0, 1, 0], dtype=pl.Int8)
     neg_and_pos_idxs = pl.Series(
         "neg_and_pos_idxs", [-2, 1, 0, -1, 2, -3], dtype=pl.Int8
     )
+    empty_idxs = pl.Series("idxs", [], dtype=pl.Int8)
+    empty_ints: list[int] = []
     assert a[0] == 1
     assert a[:2].to_list() == [1, 2]
     assert a[range(1)].to_list() == [1]
     assert a[range(0, 4, 2)].to_list() == [1, 3]
+    assert a[:0].to_list() == []
+    assert a[empty_ints].to_list() == []
+    assert a[neg_and_pos_idxs.to_list()].to_list() == [2, 2, 1, 3, 3, 1]
     for dtype in (
         pl.UInt8,
         pl.UInt16,
         pl.UInt32,
         pl.UInt64,
         pl.Int8,
         pl.Int16,
         pl.Int32,
         pl.Int64,
     ):
         assert a[pos_idxs.cast(dtype)].to_list() == [3, 1, 2, 1]
         assert a[pos_idxs.cast(dtype).to_numpy()].to_list() == [3, 1, 2, 1]
+        assert a[empty_idxs.cast(dtype)].to_list() == []
+        assert a[empty_idxs.cast(dtype).to_numpy()].to_list() == []
 
     for dtype in (pl.Int8, pl.Int16, pl.Int32, pl.Int64):
         nps = a[neg_and_pos_idxs.cast(dtype).to_numpy()]
         assert nps.to_list() == [2, 2, 1, 3, 3, 1]
 
 
 def test_set() -> None:
```

### Comparing `polars_u64_idx-0.18.3/tests/unit/test_single.py` & `polars_u64_idx-0.18.4/tests/unit/test_single.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/tests/unit/test_sql.py` & `polars_u64_idx-0.18.4/tests/unit/test_sql.py`

 * *Files 27% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import warnings
 from pathlib import Path
 
 import pytest
 
 import polars as pl
 import polars.selectors as cs
-from polars.testing import assert_frame_equal
+from polars.testing import assert_frame_equal, assert_series_equal
 
 
 # TODO: Do not rely on I/O for these tests
 @pytest.fixture()
 def foods_ipc_path() -> str:
     return str(Path(os.path.dirname(__file__)) / "io" / "files" / "foods1.ipc")
 
@@ -109,14 +109,233 @@
         "3_neq_unaware": [False, None, False, True, None],
         "4_eq_aware": [True, True, True, False, False],
         "5_eq_aware": [True, True, True, False, False],
         "6_neq_aware": [False, False, False, True, True],
     }
 
 
+def test_sql_trig() -> None:
+    df = pl.DataFrame(
+        {
+            "a": [-4, -3, -2, -1.00001, 0, 1.00001, 2, 3, 4],
+        }
+    )
+
+    c = pl.SQLContext(df=df)
+    res = c.execute(
+        """
+        SELECT
+        asin(1.0)/a as "pi values",
+        cos(asin(1.0)/a) AS "cos",
+        cot(asin(1.0)/a) AS "cot",
+        sin(asin(1.0)/a) AS "sin",
+        tan(asin(1.0)/a) AS "tan",
+
+        cosd(asind(1.0)/a) AS "cosd",
+        cotd(asind(1.0)/a) AS "cotd",
+        sind(asind(1.0)/a) AS "sind",
+        tand(asind(1.0)/a) AS "tand",
+
+        1.0/a as "inverse pi values",
+        acos(1.0/a) AS "acos",
+        asin(1.0/a) AS "asin",
+        atan(1.0/a) AS "atan",
+
+        acosd(1.0/a) AS "acosd",
+        asind(1.0/a) AS "asind",
+        atand(1.0/a) AS "atand"
+        FROM df
+        """,
+        eager=True,
+    )
+
+    df_result = pl.DataFrame(
+        {
+            "pi values": [
+                -0.392699,
+                -0.523599,
+                -0.785398,
+                -1.570781,
+                float("inf"),
+                1.570781,
+                0.785398,
+                0.523599,
+                0.392699,
+            ],
+            "cos": [
+                0.92388,
+                0.866025,
+                0.707107,
+                0.000016,
+                float("NaN"),
+                0.000016,
+                0.707107,
+                0.866025,
+                0.92388,
+            ],
+            "cot": [
+                -2.414214,
+                -1.732051,
+                -1.0,
+                -0.000016,
+                float("NaN"),
+                0.000016,
+                1.0,
+                1.732051,
+                2.414214,
+            ],
+            "sin": [
+                -0.382683,
+                -0.5,
+                -0.707107,
+                -1.0,
+                float("NaN"),
+                1,
+                0.707107,
+                0.5,
+                0.382683,
+            ],
+            "tan": [
+                -0.414214,
+                -0.57735,
+                -1,
+                -63662.613851,
+                float("NaN"),
+                63662.613851,
+                1,
+                0.57735,
+                0.414214,
+            ],
+            "cosd": [
+                0.92388,
+                0.866025,
+                0.707107,
+                0.000016,
+                float("NaN"),
+                0.000016,
+                0.707107,
+                0.866025,
+                0.92388,
+            ],
+            "cotd": [
+                -2.414214,
+                -1.732051,
+                -1.0,
+                -0.000016,
+                float("NaN"),
+                0.000016,
+                1.0,
+                1.732051,
+                2.414214,
+            ],
+            "sind": [
+                -0.382683,
+                -0.5,
+                -0.707107,
+                -1.0,
+                float("NaN"),
+                1,
+                0.707107,
+                0.5,
+                0.382683,
+            ],
+            "tand": [
+                -0.414214,
+                -0.57735,
+                -1,
+                -63662.613851,
+                float("NaN"),
+                63662.613851,
+                1,
+                0.57735,
+                0.414214,
+            ],
+            "inverse pi values": [
+                -0.25,
+                -0.333333,
+                -0.5,
+                -0.99999,
+                float("inf"),
+                0.99999,
+                0.5,
+                0.333333,
+                0.25,
+            ],
+            "acos": [
+                1.823477,
+                1.910633,
+                2.094395,
+                3.137121,
+                float("NaN"),
+                0.004472,
+                1.047198,
+                1.230959,
+                1.318116,
+            ],
+            "asin": [
+                -0.25268,
+                -0.339837,
+                -0.523599,
+                -1.566324,
+                float("NaN"),
+                1.566324,
+                0.523599,
+                0.339837,
+                0.25268,
+            ],
+            "atan": [
+                -0.244979,
+                -0.321751,
+                -0.463648,
+                -0.785393,
+                1.570796,
+                0.785393,
+                0.463648,
+                0.321751,
+                0.244979,
+            ],
+            "acosd": [
+                104.477512,
+                109.471221,
+                120.0,
+                179.743767,
+                float("NaN"),
+                0.256233,
+                60.0,
+                70.528779,
+                75.522488,
+            ],
+            "asind": [
+                -14.477512,
+                -19.471221,
+                -30.0,
+                -89.743767,
+                float("NaN"),
+                89.743767,
+                30.0,
+                19.471221,
+                14.477512,
+            ],
+            "atand": [
+                -14.036243,
+                -18.434949,
+                -26.565051,
+                -44.999714,
+                90.0,
+                44.999714,
+                26.565051,
+                18.434949,
+                14.036243,
+            ],
+        }
+    )
+
+    assert_frame_equal(left=df_result, right=res, atol=1e-5)
+
+
 def test_sql_groupby(foods_ipc_path: Path) -> None:
     lf = pl.scan_ipc(foods_ipc_path)
 
     c = pl.SQLContext(eager_execution=True)
     c.register("foods", lf)
 
     out = c.execute(
@@ -302,14 +521,45 @@
         with pytest.raises(
             pl.ComputeError,
             match=r"""Invalid pattern for '!~\*' operator: col\("abcde"\)""",
         ):
             ctx.execute("SELECT * FROM df WHERE sval !~* abcde")
 
 
+@pytest.mark.parametrize(
+    ("decimals", "expected"),
+    [
+        (0, [-8192.0, -4.0, -2.0, 2.0, 4.0, 8193.0]),
+        (1, [-8192.5, -4.0, -1.5, 2.5, 3.6, 8192.5]),
+        (2, [-8192.5, -3.96, -1.54, 2.46, 3.6, 8192.5]),
+        (3, [-8192.499, -3.955, -1.543, 2.457, 3.599, 8192.5]),
+        (4, [-8192.499, -3.955, -1.5432, 2.4568, 3.599, 8192.5001]),
+    ],
+)
+def test_sql_round_ndigits(decimals: int, expected: list[float]) -> None:
+    df = pl.DataFrame(
+        {"n": [-8192.499, -3.9550, -1.54321, 2.45678, 3.59901, 8192.5001]},
+    )
+    with pl.SQLContext(df=df, eager_execution=True) as ctx:
+        if decimals == 0:
+            out = ctx.execute("SELECT ROUND(n) AS n FROM df")
+            assert_series_equal(out["n"], pl.Series("n", values=expected))
+
+        out = ctx.execute(f"""SELECT ROUND("n",{decimals}) AS n FROM df""")
+        assert_series_equal(out["n"], pl.Series("n", values=expected))
+
+
+def test_sql_round_ndigits_errors() -> None:
+    df = pl.DataFrame({"n": [99.999]})
+    with pl.SQLContext(df=df, eager_execution=True) as ctx, pytest.raises(
+        pl.InvalidOperationError, match="Invalid 'decimals' for Round: -1"
+    ):
+        ctx.execute("SELECT ROUND(n,-1) AS n FROM df")
+
+
 def test_sql_trim(foods_ipc_path: Path) -> None:
     with warnings.catch_warnings():
         warnings.simplefilter("ignore", DeprecationWarning)
 
         out = pl.SQLContext(foods1=pl.scan_ipc(foods_ipc_path)).query(  # type: ignore[attr-defined]
             """
             SELECT DISTINCT TRIM(LEADING 'vmf' FROM category)
```

### Comparing `polars_u64_idx-0.18.3/tests/unit/test_testing.py` & `polars_u64_idx-0.18.4/tests/unit/test_testing.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/tests/unit/utils/test_parse_expr_input.py` & `polars_u64_idx-0.18.4/tests/unit/utils/test_parse_expr_input.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,17 +18,21 @@
     WARNING: This is not a fully featured function - it's just to evaluate the tests in
     this module. Do not use it elsewhere.
     """
     df = pl.DataFrame({"a": [1, 2], "b": [3, 4]})
     assert_frame_equal(df.select(result), df.select(expected))
 
 
-@pytest.mark.parametrize("input", [None, []])
-def test_first_input_to_list_empty(input: Any) -> None:
-    assert _first_input_to_list(input) == []
+def test_first_input_to_list_empty() -> None:
+    assert _first_input_to_list([]) == []
+
+
+def test_first_input_to_list_none() -> None:
+    with pytest.deprecated_call():
+        assert _first_input_to_list(None) == []
 
 
 @pytest.mark.parametrize(
     "input",
     [5, 2.0, "a", pl.Series([1, 2, 3]), pl.lit(4)],
 )
 def test_first_input_to_list_single(input: Any) -> None:
```

### Comparing `polars_u64_idx-0.18.3/tests/unit/utils/test_utils.py` & `polars_u64_idx-0.18.4/tests/unit/utils/test_utils.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.18.3/Cargo.lock` & `polars_u64_idx-0.18.4/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -89,15 +89,15 @@
  "planus",
  "serde",
 ]
 
 [[package]]
 name = "arrow2"
 version = "0.17.1"
-source = "git+https://github.com/jorgecarleitao/arrow2?rev=2d2e7053f9a50810bfe9cecff25ab39089aef98e#2d2e7053f9a50810bfe9cecff25ab39089aef98e"
+source = "git+https://github.com/ritchie46/arrow2?branch=polars_2023-06-23#84f06d6bf9442394116ba2a083fbf1975bbd57f1"
 dependencies = [
  "ahash",
  "arrow-format",
  "avro-schema",
  "base64",
  "bytemuck",
  "chrono",
@@ -1594,14 +1594,15 @@
 name = "polars-plan"
 version = "0.30.0"
 dependencies = [
  "ahash",
  "arrow2",
  "chrono",
  "chrono-tz",
+ "ciborium",
  "once_cell",
  "polars-arrow",
  "polars-core",
  "polars-io",
  "polars-ops",
  "polars-time",
  "polars-utils",
@@ -1655,14 +1656,15 @@
 
 [[package]]
 name = "polars-utils"
 version = "0.30.0"
 dependencies = [
  "ahash",
  "hashbrown 0.13.2",
+ "num-traits",
  "once_cell",
  "rayon",
  "smartstring",
  "sysinfo",
 ]
 
 [[package]]
@@ -1678,15 +1680,15 @@
 checksum = "6aeca18b86b413c660b781aa319e4e2648a3e6f9eadc9b47e9038e6fe9f3451b"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "py-polars"
-version = "0.18.3"
+version = "0.18.4"
 dependencies = [
  "ahash",
  "built",
  "ciborium",
  "jemallocator",
  "lexical-core",
  "libc",
```

### Comparing `polars_u64_idx-0.18.3/PKG-INFO` & `polars_u64_idx-0.18.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polars-u64-idx
-Version: 0.18.3
+Version: 0.18.4
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -323,15 +323,15 @@
 
 Or for python users install `pip install polars-u64-idx`.
 
 Don't use this unless you hit the row boundary as the default polars is faster and consumes less memory.
 
 ## Legacy
 
-Do you want polars to run on an old CPU (e.g. dating from before 2011)? Install `pip polars-lts-cpu`. This polars project is
+Do you want polars to run on an old CPU (e.g. dating from before 2011)? Install `pip install polars-lts-cpu`. This polars project is
 compiled without [avx](https://en.wikipedia.org/wiki/Advanced_Vector_Extensions) target features.
 
 ## Acknowledgements
 
 Development of Polars is proudly powered by
 
 [![Xomnia](https://raw.githubusercontent.com/pola-rs/polars-static/master/sponsors/xomnia.png)](https://www.xomnia.com/)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: polars-u64-idx Version: 0.18.3 Classifier:
+Metadata-Version: 2.1 Name: polars-u64-idx Version: 0.18.4 Classifier:
 Development Status :: 5 - Production/Stable Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3 :: Only Classifier:
 Programming Language :: Python :: 3.7 Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
@@ -140,15 +140,15 @@
 Extending polars with UDFs compiled in Rust is easy. We expose pyo3 extensions
 for `DataFrame` and `Series` data structures. See more in https://github.com/
 pola-rs/pyo3-polars. ## Going big... Do you expect more than `2^32` ~4,2
 billion rows? Compile polars with the `bigidx` feature flag. Or for python
 users install `pip install polars-u64-idx`. Don't use this unless you hit the
 row boundary as the default polars is faster and consumes less memory. ##
 Legacy Do you want polars to run on an old CPU (e.g. dating from before 2011)?
-Install `pip polars-lts-cpu`. This polars project is compiled without [avx]
-(https://en.wikipedia.org/wiki/Advanced_Vector_Extensions) target features. ##
-Acknowledgements Development of Polars is proudly powered by [![Xomnia](https:/
-/raw.githubusercontent.com/pola-rs/polars-static/master/sponsors/xomnia.png)]
-(https://www.xomnia.com/) ## Sponsors [[https://raw.githubusercontent.com/pola-
-rs/polars-static/master/sponsors/xomnia.png]](https://www.xomnia.com/) &emsp; [
-[https://www.jetbrains.com/company/brand/img/jetbrains_logo.png]](https://
-www.jetbrains.com)
+Install `pip install polars-lts-cpu`. This polars project is compiled without
+[avx](https://en.wikipedia.org/wiki/Advanced_Vector_Extensions) target
+features. ## Acknowledgements Development of Polars is proudly powered by [!
+[Xomnia](https://raw.githubusercontent.com/pola-rs/polars-static/master/
+sponsors/xomnia.png)](https://www.xomnia.com/) ## Sponsors [[https://
+raw.githubusercontent.com/pola-rs/polars-static/master/sponsors/xomnia.png]]
+(https://www.xomnia.com/) &emsp; [[https://www.jetbrains.com/company/brand/img/
+jetbrains_logo.png]](https://www.jetbrains.com)
```

