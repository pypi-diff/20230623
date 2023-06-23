# Comparing `tmp/linkspace-0.1.4.tar.gz` & `tmp/linkspace-0.3.0rc2.tar.gz`

## Comparing `linkspace-0.1.4.tar` & `linkspace-0.3.0rc2.tar`

### file list

```diff
@@ -1,155 +1,166 @@
--rw-r--r--   0        0        0      666 1970-01-01 00:00:00.000000 linkspace-0.1.4/local_dependencies/ipcbus/Cargo.toml
--rw-r--r--   0        0        0    16725 2023-04-13 10:59:32.000000 linkspace-0.1.4/local_dependencies/ipcbus/LICENSE
--rw-r--r--   0        0        0       56 2023-04-13 10:59:32.000000 linkspace-0.1.4/local_dependencies/ipcbus/README.md
--rw-r--r--   0        0        0      526 2023-04-13 10:59:32.000000 linkspace-0.1.4/local_dependencies/ipcbus/src/lib.rs
--rw-r--r--   0        0        0     6038 2023-04-13 10:59:32.000000 linkspace-0.1.4/local_dependencies/ipcbus/src/procbus.rs
--rw-r--r--   0        0        0     4587 2023-04-13 10:59:32.000000 linkspace-0.1.4/local_dependencies/ipcbus/src/udp_multicast.rs
--rw-r--r--   0        0        0     1512 2023-04-13 10:59:32.000000 linkspace-0.1.4/local_dependencies/ipcbus/src/wasmbus.rs
--rw-r--r--   0        0        0      618 1970-01-01 00:00:00.000000 linkspace-0.1.4/local_dependencies/abe/Cargo.toml
--rw-r--r--   0        0        0    16725 2023-04-13 10:59:32.000000 linkspace-0.1.4/local_dependencies/abe/LICENSE
--rw-r--r--   0        0        0       61 2023-04-13 10:59:32.000000 linkspace-0.1.4/local_dependencies/abe/README.md
--rw-r--r--   0        0        0     1863 2023-04-13 10:59:32.000000 linkspace-0.1.4/local_dependencies/abe/src/abe_macro.rs
--rw-r--r--   0        0        0     9010 2023-04-13 10:59:32.000000 linkspace-0.1.4/local_dependencies/abe/src/abtxt.rs
--rw-r--r--   0        0        0    16329 2023-04-13 10:59:32.000000 linkspace-0.1.4/local_dependencies/abe/src/ast.rs
--rw-r--r--   0        0        0     6632 2023-04-13 10:59:32.000000 linkspace-0.1.4/local_dependencies/abe/src/convert.rs
--rw-r--r--   0        0        0    56481 2023-04-13 10:59:32.000000 linkspace-0.1.4/local_dependencies/abe/src/eval.rs
--rw-r--r--   0        0        0     2681 2023-04-13 10:59:32.000000 linkspace-0.1.4/local_dependencies/abe/src/lib.rs
--rw-r--r--   0        0        0     1201 1970-01-01 00:00:00.000000 linkspace-0.1.4/local_dependencies/linkspace-core/Cargo.toml
--rw-r--r--   0        0        0    16725 2023-04-13 10:59:32.000000 linkspace-0.1.4/local_dependencies/linkspace-core/LICENSE
--rw-r--r--   0        0        0       34 2023-04-13 10:59:32.000000 linkspace-0.1.4/local_dependencies/linkspace-core/README.md
--rw-r--r--   0        0        0     3048 2023-04-13 10:59:32.000000 linkspace-0.1.4/local_dependencies/linkspace-core/src/consts.rs
--rw-r--r--   0        0        0     7695 2023-04-13 10:59:32.000000 linkspace-0.1.4/local_dependencies/linkspace-core/src/env/db/inmem.rs
--rw-r--r--   0        0        0    19389 2023-04-13 10:59:32.000000 linkspace-0.1.4/local_dependencies/linkspace-core/src/env/db/lmdb.rs
--rw-r--r--   0        0        0     1631 2023-04-13 10:59:32.000000 linkspace-0.1.4/local_dependencies/linkspace-core/src/env/db/mod.rs
--rw-r--r--   0        0        0     6250 2023-04-13 10:59:32.000000 linkspace-0.1.4/local_dependencies/linkspace-core/src/env/mod.rs
--rw-r--r--   0        0        0    11280 2023-04-13 10:59:32.000000 linkspace-0.1.4/local_dependencies/linkspace-core/src/env/queries.rs
--rw-r--r--   0        0        0     9908 2023-04-13 10:59:32.000000 linkspace-0.1.4/local_dependencies/linkspace-core/src/env/queries2.rs
--rw-r--r--   0        0        0     1459 2023-04-13 10:59:32.000000 linkspace-0.1.4/local_dependencies/linkspace-core/src/env/query_mode.rs
--rw-r--r--   0        0        0     6982 2023-04-13 10:59:32.000000 linkspace-0.1.4/local_dependencies/linkspace-core/src/env/tree_key.rs
--rw-r--r--   0        0        0     2020 2023-04-13 10:59:32.000000 linkspace-0.1.4/local_dependencies/linkspace-core/src/env/write_result.rs
--rw-r--r--   0        0        0     1883 2023-04-13 10:59:32.000000 linkspace-0.1.4/local_dependencies/linkspace-core/src/env/write_trait.rs
--rw-r--r--   0        0        0     3727 2023-04-13 10:59:32.000000 linkspace-0.1.4/local_dependencies/linkspace-core/src/eval.rs
--rw-r--r--   0        0        0     1557 2023-04-13 10:59:32.000000 linkspace-0.1.4/local_dependencies/linkspace-core/src/lib.rs
--rw-r--r--   0        0        0   151768 2023-04-13 10:59:32.000000 linkspace-0.1.4/local_dependencies/linkspace-core/src/lnsroots.pkt
--rw-r--r--   0        0        0        0 2023-04-13 10:59:32.000000 linkspace-0.1.4/local_dependencies/linkspace-core/src/matcher/matcher2.rs
--rw-r--r--   0        0        0     8474 2023-04-13 10:59:32.000000 linkspace-0.1.4/local_dependencies/linkspace-core/src/matcher/mod.rs
--rw-r--r--   0        0        0     3092 2023-04-13 10:59:32.000000 linkspace-0.1.4/local_dependencies/linkspace-core/src/mut_header.rs
--rw-r--r--   0        0        0     4354 2023-04-13 10:59:32.000000 linkspace-0.1.4/local_dependencies/linkspace-core/src/partial_hash.rs
--rw-r--r--   0        0        0     4043 2023-04-13 10:59:32.000000 linkspace-0.1.4/local_dependencies/linkspace-core/src/predicate/bitset_test.rs
--rw-r--r--   0        0        0     2271 2023-04-13 10:59:32.000000 linkspace-0.1.4/local_dependencies/linkspace-core/src/predicate/builder.rs
--rw-r--r--   0        0        0     9176 2023-04-13 10:59:32.000000 linkspace-0.1.4/local_dependencies/linkspace-core/src/predicate/exprs.rs
--rw-r--r--   0        0        0      471 2023-04-13 10:59:32.000000 linkspace-0.1.4/local_dependencies/linkspace-core/src/predicate/mod.rs
--rw-r--r--   0        0        0    12714 2023-04-13 10:59:32.000000 linkspace-0.1.4/local_dependencies/linkspace-core/src/predicate/pkt_predicates.rs
--rw-r--r--   0        0        0     4480 2023-04-13 10:59:32.000000 linkspace-0.1.4/local_dependencies/linkspace-core/src/predicate/predicate_type.rs
--rw-r--r--   0        0        0     6453 2023-04-13 10:59:32.000000 linkspace-0.1.4/local_dependencies/linkspace-core/src/predicate/test_pkt.rs
--rw-r--r--   0        0        0     7298 2023-04-13 10:59:32.000000 linkspace-0.1.4/local_dependencies/linkspace-core/src/predicate/treekey.rs
--rw-r--r--   0        0        0    15031 2023-04-13 10:59:32.000000 linkspace-0.1.4/local_dependencies/linkspace-core/src/predicate/uint.rs
--rw-r--r--   0        0        0    20681 2023-04-13 10:59:32.000000 linkspace-0.1.4/local_dependencies/linkspace-core/src/predicate/value_test.rs
--rw-r--r--   0        0        0      788 2023-04-13 10:59:32.000000 linkspace-0.1.4/local_dependencies/linkspace-core/src/prelude.rs
--rw-r--r--   0        0        0     1213 2023-04-13 10:59:32.000000 linkspace-0.1.4/local_dependencies/linkspace-core/src/pull.rs
--rw-r--r--   0        0        0     7077 2023-04-13 10:59:32.000000 linkspace-0.1.4/local_dependencies/linkspace-core/src/query.rs
--rw-r--r--   0        0        0    10703 2023-04-13 10:59:32.000000 linkspace-0.1.4/local_dependencies/linkspace-core/src/stamp_fmt.rs
--rw-r--r--   0        0        0     5012 2023-04-13 10:59:32.000000 linkspace-0.1.4/local_dependencies/linkspace-core/src/stamp_range.rs
--rw-r--r--   0        0        0      727 1970-01-01 00:00:00.000000 linkspace-0.1.4/local_dependencies/linkspace/Cargo.toml
--rw-r--r--   0        0        0    16725 2023-04-13 10:59:32.000000 linkspace-0.1.4/local_dependencies/linkspace/LICENSE
--rw-r--r--   0        0        0     1607 2023-04-13 10:59:32.000000 linkspace-0.1.4/local_dependencies/linkspace/README.md
--rw-r--r--   0        0        0     1727 2023-04-13 10:59:32.000000 linkspace-0.1.4/local_dependencies/linkspace/src/conventions/mod.rs
--rw-r--r--   0        0        0     7454 2023-04-13 10:59:32.000000 linkspace-0.1.4/local_dependencies/linkspace/src/conventions/status.rs
--rw-r--r--   0        0        0     2476 2023-04-13 10:59:32.000000 linkspace-0.1.4/local_dependencies/linkspace/src/interop.rs
--rw-r--r--   0        0        0    31366 2023-04-13 10:59:32.000000 linkspace-0.1.4/local_dependencies/linkspace/src/lib.rs
--rw-r--r--   0        0        0      870 1970-01-01 00:00:00.000000 linkspace-0.1.4/local_dependencies/linkspace-cryptography/Cargo.toml
--rw-r--r--   0        0        0    16725 2023-04-13 10:59:32.000000 linkspace-0.1.4/local_dependencies/linkspace-cryptography/LICENSE
--rw-r--r--   0        0        0       59 2023-04-13 10:59:32.000000 linkspace-0.1.4/local_dependencies/linkspace-cryptography/README.md
--rw-r--r--   0        0        0      969 2023-04-13 10:59:32.000000 linkspace-0.1.4/local_dependencies/linkspace-cryptography/src/keygen.rs
--rw-r--r--   0        0        0     2609 2023-04-13 10:59:32.000000 linkspace-0.1.4/local_dependencies/linkspace-cryptography/src/lib.rs
--rw-r--r--   0        0        0      663 1970-01-01 00:00:00.000000 linkspace-0.1.4/local_dependencies/linkspace-argon2-identity/Cargo.toml
--rw-r--r--   0        0        0    16725 2023-04-13 10:59:32.000000 linkspace-0.1.4/local_dependencies/linkspace-argon2-identity/LICENSE
--rw-r--r--   0        0        0       38 2023-04-13 10:59:32.000000 linkspace-0.1.4/local_dependencies/linkspace-argon2-identity/README.md
--rw-r--r--   0        0        0     5387 2023-04-13 10:59:32.000000 linkspace-0.1.4/local_dependencies/linkspace-argon2-identity/src/lib.rs
--rw-r--r--   0        0        0     1432 1970-01-01 00:00:00.000000 linkspace-0.1.4/local_dependencies/linkspace-common/Cargo.toml
--rw-r--r--   0        0        0    16725 2023-04-13 10:59:32.000000 linkspace-0.1.4/local_dependencies/linkspace-common/LICENSE
--rw-r--r--   0        0        0       99 2023-04-13 10:59:32.000000 linkspace-0.1.4/local_dependencies/linkspace-common/README.md
--rw-r--r--   0        0        0     2114 2023-04-13 10:59:32.000000 linkspace-0.1.4/local_dependencies/linkspace-common/src/bus.rs
--rw-r--r--   0        0        0     8249 2023-04-13 10:59:32.000000 linkspace-0.1.4/local_dependencies/linkspace-common/src/cli/keys.rs
--rw-r--r--   0        0        0    12488 2023-04-13 10:59:32.000000 linkspace-0.1.4/local_dependencies/linkspace-common/src/cli/mod.rs
--rw-r--r--   0        0        0     7772 2023-04-13 10:59:32.000000 linkspace-0.1.4/local_dependencies/linkspace-common/src/cli/opts.rs
--rw-r--r--   0        0        0     7203 2023-04-13 10:59:32.000000 linkspace-0.1.4/local_dependencies/linkspace-common/src/dgp.rs
--rw-r--r--   0        0        0     7294 2023-04-13 10:59:32.000000 linkspace-0.1.4/local_dependencies/linkspace-common/src/eval.rs
--rw-r--r--   0        0        0     1070 2023-04-13 10:59:32.000000 linkspace-0.1.4/local_dependencies/linkspace-common/src/lib.rs
--rw-r--r--   0        0        0     3109 2023-04-13 10:59:32.000000 linkspace-0.1.4/local_dependencies/linkspace-common/src/pkt_reader.rs
--rw-r--r--   0        0        0     2135 2023-04-13 10:59:32.000000 linkspace-0.1.4/local_dependencies/linkspace-common/src/pkt_stream_utils.rs
--rw-r--r--   0        0        0     4095 2023-04-13 10:59:32.000000 linkspace-0.1.4/local_dependencies/linkspace-common/src/predicate_aliases.rs
--rw-r--r--   0        0        0      448 2023-04-13 10:59:32.000000 linkspace-0.1.4/local_dependencies/linkspace-common/src/prelude.rs
--rw-r--r--   0        0        0     5094 2023-04-13 10:59:32.000000 linkspace-0.1.4/local_dependencies/linkspace-common/src/protocols/handshake.rs
--rw-r--r--   0        0        0     5784 2023-04-13 10:59:32.000000 linkspace-0.1.4/local_dependencies/linkspace-common/src/protocols/impex/blob.rs
--rw-r--r--   0        0        0     4257 2023-04-13 10:59:32.000000 linkspace-0.1.4/local_dependencies/linkspace-common/src/protocols/impex/blobmap/checkin.rs
--rw-r--r--   0        0        0     3104 2023-04-13 10:59:32.000000 linkspace-0.1.4/local_dependencies/linkspace-common/src/protocols/impex/blobmap/checkout.rs
--rw-r--r--   0        0        0     3764 2023-04-13 10:59:32.000000 linkspace-0.1.4/local_dependencies/linkspace-common/src/protocols/impex/blobmap/mod.rs
--rw-r--r--   0        0        0     1029 2023-04-13 10:59:32.000000 linkspace-0.1.4/local_dependencies/linkspace-common/src/protocols/impex/mod.rs
--rw-r--r--   0        0        0     6689 2023-04-13 10:59:32.000000 linkspace-0.1.4/local_dependencies/linkspace-common/src/protocols/lns/admin.rs
--rw-r--r--   0        0        0     6976 2023-04-13 10:59:32.000000 linkspace-0.1.4/local_dependencies/linkspace-common/src/protocols/lns/claim.rs
--rw-r--r--   0        0        0      632 2023-04-13 10:59:32.000000 linkspace-0.1.4/local_dependencies/linkspace-common/src/protocols/lns/env_claim.rs
--rw-r--r--   0        0        0     8245 2023-04-13 10:59:32.000000 linkspace-0.1.4/local_dependencies/linkspace-common/src/protocols/lns/eval.rs
--rw-r--r--   0        0        0     1383 2023-04-13 10:59:32.000000 linkspace-0.1.4/local_dependencies/linkspace-common/src/protocols/lns/local_claim.rs
--rw-r--r--   0        0        0     6882 2023-04-13 10:59:32.000000 linkspace-0.1.4/local_dependencies/linkspace-common/src/protocols/lns/mod.rs
--rw-r--r--   0        0        0     5063 2023-04-13 10:59:32.000000 linkspace-0.1.4/local_dependencies/linkspace-common/src/protocols/lns/name.rs
--rw-r--r--   0        0        0     5694 2023-04-13 10:59:32.000000 linkspace-0.1.4/local_dependencies/linkspace-common/src/protocols/lns/public_claim.rs
--rw-r--r--   0        0        0      951 2023-04-13 10:59:32.000000 linkspace-0.1.4/local_dependencies/linkspace-common/src/protocols/lns/utils.rs
--rw-r--r--   0        0        0      398 2023-04-13 10:59:32.000000 linkspace-0.1.4/local_dependencies/linkspace-common/src/protocols/mod.rs
--rw-r--r--   0        0        0     4387 2023-04-13 10:59:32.000000 linkspace-0.1.4/local_dependencies/linkspace-common/src/runtime/handlers.rs
--rw-r--r--   0        0        0      292 2023-04-13 10:59:32.000000 linkspace-0.1.4/local_dependencies/linkspace-common/src/runtime/mod.rs
--rw-r--r--   0        0        0    20247 2023-04-13 10:59:32.000000 linkspace-0.1.4/local_dependencies/linkspace-common/src/runtime/rx.rs
--rw-r--r--   0        0        0     3083 2023-04-13 10:59:32.000000 linkspace-0.1.4/local_dependencies/linkspace-common/src/runtime/threads.rs
--rw-r--r--   0        0        0     2659 2023-04-13 10:59:32.000000 linkspace-0.1.4/local_dependencies/linkspace-common/src/static_env.rs
--rw-r--r--   0        0        0     2843 2023-04-13 10:59:32.000000 linkspace-0.1.4/local_dependencies/linkspace-common/src/tests.rs
--rw-r--r--   0        0        0      863 1970-01-01 00:00:00.000000 linkspace-0.1.4/local_dependencies/linkspace-pkt/Cargo.toml
--rw-r--r--   0        0        0    16725 2023-04-13 10:59:32.000000 linkspace-0.1.4/local_dependencies/linkspace-pkt/LICENSE
--rw-r--r--   0        0        0       45 2023-04-13 10:59:32.000000 linkspace-0.1.4/local_dependencies/linkspace-pkt/README.md
--rw-r--r--   0        0        0      247 2023-04-13 10:59:32.000000 linkspace-0.1.4/local_dependencies/linkspace-pkt/benches/spoints.rs
--rw-r--r--   0        0        0     2948 2023-04-13 10:59:32.000000 linkspace-0.1.4/local_dependencies/linkspace-pkt/src/asm_tests.rs
--rw-r--r--   0        0        0     6092 2023-04-13 10:59:32.000000 linkspace-0.1.4/local_dependencies/linkspace-pkt/src/builder.rs
--rw-r--r--   0        0        0     3602 2023-04-13 10:59:32.000000 linkspace-0.1.4/local_dependencies/linkspace-pkt/src/byte_segments.rs
--rw-r--r--   0        0        0     8654 2023-04-13 10:59:32.000000 linkspace-0.1.4/local_dependencies/linkspace-pkt/src/eval.rs
--rw-r--r--   0        0        0      813 2023-04-13 10:59:32.000000 linkspace-0.1.4/local_dependencies/linkspace-pkt/src/exprs.rs
--rw-r--r--   0        0        0    21120 2023-04-13 10:59:32.000000 linkspace-0.1.4/local_dependencies/linkspace-pkt/src/field_ids.rs
--rw-r--r--   0        0        0    11324 2023-04-13 10:59:32.000000 linkspace-0.1.4/local_dependencies/linkspace-pkt/src/ipath.rs
--rw-r--r--   0        0        0    11252 2023-04-13 10:59:32.000000 linkspace-0.1.4/local_dependencies/linkspace-pkt/src/lib.rs
--rw-r--r--   0        0        0     2133 2023-04-13 10:59:32.000000 linkspace-0.1.4/local_dependencies/linkspace-pkt/src/link.rs
--rw-r--r--   0        0        0     5000 2023-04-13 10:59:32.000000 linkspace-0.1.4/local_dependencies/linkspace-pkt/src/netpkt/header.rs
--rw-r--r--   0        0        0     5309 2023-04-13 10:59:32.000000 linkspace-0.1.4/local_dependencies/linkspace-pkt/src/netpkt/mod.rs
--rw-r--r--   0        0        0     5880 2023-04-13 10:59:32.000000 linkspace-0.1.4/local_dependencies/linkspace-pkt/src/netpkt/netpkt_arc.rs
--rw-r--r--   0        0        0     2262 2023-04-13 10:59:32.000000 linkspace-0.1.4/local_dependencies/linkspace-pkt/src/netpkt/netpkt_parts.rs
--rw-r--r--   0        0        0     6161 2023-04-13 10:59:32.000000 linkspace-0.1.4/local_dependencies/linkspace-pkt/src/netpkt/netpkt_ptr.rs
--rw-r--r--   0        0        0     1600 2023-04-13 10:59:32.000000 linkspace-0.1.4/local_dependencies/linkspace-pkt/src/netpkt/partial.rs
--rw-r--r--   0        0        0     4406 2023-04-13 10:59:32.000000 linkspace-0.1.4/local_dependencies/linkspace-pkt/src/netpkt/reroute.rs
--rw-r--r--   0        0        0     3141 2023-04-13 10:59:32.000000 linkspace-0.1.4/local_dependencies/linkspace-pkt/src/netpkt/slot.rs
--rw-r--r--   0        0        0      232 2023-04-13 10:59:32.000000 linkspace-0.1.4/local_dependencies/linkspace-pkt/src/pkt_bytes/mod.rs
--rw-r--r--   0        0        0     3526 2023-04-13 10:59:32.000000 linkspace-0.1.4/local_dependencies/linkspace-pkt/src/point.rs
--rw-r--r--   0        0        0     5294 2023-04-13 10:59:32.000000 linkspace-0.1.4/local_dependencies/linkspace-pkt/src/point_parts.rs
--rw-r--r--   0        0        0    13249 2023-04-13 10:59:32.000000 linkspace-0.1.4/local_dependencies/linkspace-pkt/src/point_ptr.rs
--rw-r--r--   0        0        0      968 2023-04-13 10:59:32.000000 linkspace-0.1.4/local_dependencies/linkspace-pkt/src/read.rs
--rw-r--r--   0        0        0     1177 2023-04-13 10:59:32.000000 linkspace-0.1.4/local_dependencies/linkspace-pkt/src/repr.rs
--rw-r--r--   0        0        0    20955 2023-04-13 10:59:32.000000 linkspace-0.1.4/local_dependencies/linkspace-pkt/src/spath.rs
--rw-r--r--   0        0        0    12080 2023-04-13 10:59:32.000000 linkspace-0.1.4/local_dependencies/linkspace-pkt/src/spath_fmt.rs
--rw-r--r--   0        0        0     2976 2023-04-13 10:59:32.000000 linkspace-0.1.4/local_dependencies/linkspace-pkt/src/spath_macro.rs
--rw-r--r--   0        0        0     2749 2023-04-13 10:59:32.000000 linkspace-0.1.4/local_dependencies/linkspace-pkt/src/stamp.rs
--rw-r--r--   0        0        0      662 2023-04-13 10:59:32.000000 linkspace-0.1.4/local_dependencies/linkspace-pkt/src/utils.rs
--rw-r--r--   0        0        0      660 1970-01-01 00:00:00.000000 linkspace-0.1.4/local_dependencies/byte-fmt/Cargo.toml
--rw-r--r--   0        0        0    16725 2023-04-13 10:59:32.000000 linkspace-0.1.4/local_dependencies/byte-fmt/LICENSE
--rw-r--r--   0        0        0       63 2023-04-13 10:59:32.000000 linkspace-0.1.4/local_dependencies/byte-fmt/README.md
--rw-r--r--   0        0        0    10790 2023-04-13 10:59:32.000000 linkspace-0.1.4/local_dependencies/byte-fmt/src/endian_types.rs
--rw-r--r--   0        0        0    16202 2023-04-13 10:59:32.000000 linkspace-0.1.4/local_dependencies/byte-fmt/src/lib.rs
--rw-r--r--   0        0        0     8551 2023-04-13 10:59:32.000000 linkspace-0.1.4/local_dependencies/byte-fmt/src/serde.rs
--rw-r--r--   0        0        0      510 1970-01-01 00:00:00.000000 linkspace-0.1.4/Cargo.toml
--rw-r--r--   0        0        0        0 2023-04-13 10:59:32.000000 linkspace-0.1.4/Cross.toml
--rw-r--r--   0        0        0     1055 2023-04-13 12:04:19.000000 linkspace-0.1.4/Makefile
--rw-r--r--   0        0        0      246 2023-04-13 10:59:32.000000 linkspace-0.1.4/README.md
--rw-r--r--   0        0        0     2885 2023-04-13 10:59:32.000000 linkspace-0.1.4/linkspace.pyi
--rw-r--r--   0        0        0      273 2023-04-13 12:04:38.000000 linkspace-0.1.4/publish.sh
--rw-r--r--   0        0        0      163 2023-04-13 10:59:32.000000 linkspace-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      144 2023-04-13 10:59:32.000000 linkspace-0.1.4/pyrightconfig.json
--rw-r--r--   0        0        0    19574 2023-04-13 10:59:32.000000 linkspace-0.1.4/src/lib.rs
--rw-r--r--   0        0        0     9185 2023-04-13 10:59:32.000000 linkspace-0.1.4/src/pynetpkt.rs
--rw-r--r--   0        0        0      638 2023-04-13 10:59:32.000000 linkspace-0.1.4/tests/nested_watch.py
--rw-r--r--   0        0        0    57811 2023-04-13 11:22:35.000000 linkspace-0.1.4/Cargo.lock
--rw-r--r--   0        0        0      369 1970-01-01 00:00:00.000000 linkspace-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1006 1970-01-01 00:00:00.000000 linkspace-0.3.0rc2/local_dependencies/linkspace/Cargo.toml
+-rw-r--r--   0        0        0    16725 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/linkspace/LICENSE
+-rw-r--r--   0        0        0       40 2023-06-23 08:46:36.000000 linkspace-0.3.0rc2/local_dependencies/linkspace/README.md
+-rw-r--r--   0        0        0      221 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/linkspace/build.rs
+-rw-r--r--   0        0        0     1728 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/linkspace/src/conventions/mod.rs
+-rw-r--r--   0        0        0     7874 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/linkspace/src/conventions/status.rs
+-rw-r--r--   0        0        0     2465 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/linkspace/src/interop.rs
+-rw-r--r--   0        0        0    35622 2023-06-23 08:46:36.000000 linkspace-0.3.0rc2/local_dependencies/linkspace/src/lib.rs
+-rw-r--r--   0        0        0      740 1970-01-01 00:00:00.000000 linkspace-0.3.0rc2/local_dependencies/ipcbus/Cargo.toml
+-rw-r--r--   0        0        0    16725 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/ipcbus/LICENSE
+-rw-r--r--   0        0        0       56 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/ipcbus/README.md
+-rw-r--r--   0        0        0      526 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/ipcbus/src/lib.rs
+-rw-r--r--   0        0        0     6034 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/ipcbus/src/procbus.rs
+-rw-r--r--   0        0        0     4587 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/ipcbus/src/udp_multicast.rs
+-rw-r--r--   0        0        0     1512 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/ipcbus/src/wasmbus.rs
+-rw-r--r--   0        0        0      684 1970-01-01 00:00:00.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-cryptography/Cargo.toml
+-rw-r--r--   0        0        0    16725 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-cryptography/LICENSE
+-rw-r--r--   0        0        0       59 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-cryptography/README.md
+-rw-r--r--   0        0        0      969 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-cryptography/src/keygen.rs
+-rw-r--r--   0        0        0     2699 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-cryptography/src/lib.rs
+-rw-r--r--   0        0        0      661 1970-01-01 00:00:00.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-argon2-identity/Cargo.toml
+-rw-r--r--   0        0        0    16725 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-argon2-identity/LICENSE
+-rw-r--r--   0        0        0       38 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-argon2-identity/README.md
+-rw-r--r--   0        0        0     6020 2023-06-21 12:25:29.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-argon2-identity/src/lib.rs
+-rw-r--r--   0        0        0     1225 1970-01-01 00:00:00.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-core/Cargo.toml
+-rw-r--r--   0        0        0    16725 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-core/LICENSE
+-rw-r--r--   0        0        0       34 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-core/README.md
+-rw-r--r--   0        0        0     1728 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-core/src/consts.rs
+-rw-r--r--   0        0        0    19369 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-core/src/env/lmdb/db.rs
+-rw-r--r--   0        0        0     1171 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-core/src/env/lmdb/misc.rs
+-rw-r--r--   0        0        0     5828 2023-06-20 15:25:28.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-core/src/env/lmdb/mod.rs
+-rw-r--r--   0        0        0    10165 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-core/src/env/lmdb/queries.rs
+-rw-r--r--   0        0        0    10061 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-core/src/env/lmdb/queries2.rs
+-rw-r--r--   0        0        0     5769 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-core/src/env/lmdb/tree_iter.rs
+-rw-r--r--   0        0        0      616 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-core/src/env/mod.rs
+-rw-r--r--   0        0        0     1459 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-core/src/env/query_mode.rs
+-rw-r--r--   0        0        0     7034 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-core/src/env/tree_key.rs
+-rw-r--r--   0        0        0     2020 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-core/src/env/write_result.rs
+-rw-r--r--   0        0        0     1883 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-core/src/env/write_trait.rs
+-rw-r--r--   0        0        0     3673 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-core/src/eval.rs
+-rw-r--r--   0        0        0     1499 2023-06-23 08:46:36.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-core/src/lib.rs
+-rw-r--r--   0        0        0        0 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-core/src/lnsroots.pkt
+-rw-r--r--   0        0        0        0 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-core/src/matcher/matcher2.rs
+-rw-r--r--   0        0        0     8686 2023-06-23 08:46:36.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-core/src/matcher/mod.rs
+-rw-r--r--   0        0        0     3092 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-core/src/mut_header.rs
+-rw-r--r--   0        0        0     4137 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-core/src/partial_hash.rs
+-rw-r--r--   0        0        0     4043 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-core/src/predicate/bitset_test.rs
+-rw-r--r--   0        0        0     2268 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-core/src/predicate/builder.rs
+-rw-r--r--   0        0        0     9173 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-core/src/predicate/exprs.rs
+-rw-r--r--   0        0        0      471 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-core/src/predicate/mod.rs
+-rw-r--r--   0        0        0    12662 2023-06-21 12:24:07.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-core/src/predicate/pkt_predicates.rs
+-rw-r--r--   0        0        0     4890 2023-06-21 12:24:07.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-core/src/predicate/predicate_type.rs
+-rw-r--r--   0        0        0     6439 2023-06-21 12:24:07.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-core/src/predicate/test_pkt.rs
+-rw-r--r--   0        0        0     1641 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-core/src/predicate/treekey.rs
+-rw-r--r--   0        0        0    15063 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-core/src/predicate/uint.rs
+-rw-r--r--   0        0        0    20779 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-core/src/predicate/value_test.rs
+-rw-r--r--   0        0        0      794 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-core/src/prelude.rs
+-rw-r--r--   0        0        0     1213 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-core/src/pull.rs
+-rw-r--r--   0        0        0     7194 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-core/src/query.rs
+-rw-r--r--   0        0        0    10689 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-core/src/stamp_fmt.rs
+-rw-r--r--   0        0        0     5270 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-core/src/stamp_range.rs
+-rw-r--r--   0        0        0      993 1970-01-01 00:00:00.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-pkt/Cargo.toml
+-rw-r--r--   0        0        0    16725 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-pkt/LICENSE
+-rw-r--r--   0        0        0       45 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-pkt/README.md
+-rw-r--r--   0        0        0      247 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-pkt/benches/spoints.rs
+-rw-r--r--   0        0        0     5881 2023-06-21 12:24:07.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-pkt/src/asm_tests.rs
+-rw-r--r--   0        0        0     6488 2023-06-21 12:24:07.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-pkt/src/builder.rs
+-rw-r--r--   0        0        0     3926 2023-06-20 14:52:26.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-pkt/src/byte_segments.rs
+-rw-r--r--   0        0        0     3314 2023-06-21 12:24:07.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-pkt/src/consts.rs
+-rw-r--r--   0        0        0     9167 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-pkt/src/eval.rs
+-rw-r--r--   0        0        0      577 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-pkt/src/exprs.rs
+-rw-r--r--   0        0        0    21374 2023-06-21 12:24:07.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-pkt/src/field_ids.rs
+-rw-r--r--   0        0        0    11774 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-pkt/src/ipath.rs
+-rw-r--r--   0        0        0    11232 2023-06-21 12:24:07.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-pkt/src/lib.rs
+-rw-r--r--   0        0        0     2208 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-pkt/src/link.rs
+-rw-r--r--   0        0        0     5000 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-pkt/src/netpkt/header.rs
+-rw-r--r--   0        0        0     5819 2023-06-21 12:24:07.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-pkt/src/netpkt/mod.rs
+-rw-r--r--   0        0        0     6641 2023-06-20 15:07:14.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-pkt/src/netpkt/netpkt_arc.rs
+-rw-r--r--   0        0        0     2301 2023-06-21 12:24:07.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-pkt/src/netpkt/netpkt_parts.rs
+-rw-r--r--   0        0        0     7054 2023-06-20 15:08:46.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-pkt/src/netpkt/netpkt_ptr.rs
+-rw-r--r--   0        0        0     1658 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-pkt/src/netpkt/partial.rs
+-rw-r--r--   0        0        0     4406 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-pkt/src/netpkt/reroute.rs
+-rw-r--r--   0        0        0     3121 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-pkt/src/netpkt/slot.rs
+-rw-r--r--   0        0        0     3888 2023-06-21 12:24:07.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-pkt/src/point.rs
+-rw-r--r--   0        0        0     5978 2023-06-21 12:24:07.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-pkt/src/point_parts.rs
+-rw-r--r--   0        0        0    13570 2023-06-21 12:24:07.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-pkt/src/point_ptr.rs
+-rw-r--r--   0        0        0     3617 2023-06-21 12:24:07.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-pkt/src/read.rs
+-rw-r--r--   0        0        0     6993 2023-06-21 12:24:07.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-pkt/src/repr.rs
+-rw-r--r--   0        0        0    21438 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-pkt/src/spath.rs
+-rw-r--r--   0        0        0    11507 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-pkt/src/spath_fmt.rs
+-rw-r--r--   0        0        0     2976 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-pkt/src/spath_macro.rs
+-rw-r--r--   0        0        0     2986 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-pkt/src/stamp.rs
+-rw-r--r--   0        0        0      506 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-pkt/src/utils.rs
+-rw-r--r--   0        0        0      803 1970-01-01 00:00:00.000000 linkspace-0.3.0rc2/local_dependencies/byte-fmt/Cargo.toml
+-rw-r--r--   0        0        0    16725 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/byte-fmt/LICENSE
+-rw-r--r--   0        0        0       63 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/byte-fmt/README.md
+-rw-r--r--   0        0        0    10893 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/byte-fmt/src/endian_types.rs
+-rw-r--r--   0        0        0    15089 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/byte-fmt/src/lib.rs
+-rw-r--r--   0        0        0     8551 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/byte-fmt/src/serde.rs
+-rw-r--r--   0        0        0      673 1970-01-01 00:00:00.000000 linkspace-0.3.0rc2/local_dependencies/abe/Cargo.toml
+-rw-r--r--   0        0        0    16725 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/abe/LICENSE
+-rw-r--r--   0        0        0       61 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/abe/README.md
+-rw-r--r--   0        0        0     1863 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/abe/src/abe_macro.rs
+-rw-r--r--   0        0        0     9010 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/abe/src/abtxt.rs
+-rw-r--r--   0        0        0    16329 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/abe/src/ast.rs
+-rw-r--r--   0        0        0     6637 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/abe/src/convert.rs
+-rw-r--r--   0        0        0    34386 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/abe/src/eval.rs
+-rw-r--r--   0        0        0     2717 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/abe/src/lib.rs
+-rw-r--r--   0        0        0     3570 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/abe/src/scope/argv.rs
+-rw-r--r--   0        0        0     3640 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/abe/src/scope/base.rs
+-rw-r--r--   0        0        0     7210 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/abe/src/scope/bytes.rs
+-rw-r--r--   0        0        0      462 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/abe/src/scope/comment.rs
+-rw-r--r--   0        0        0     3732 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/abe/src/scope/encode.rs
+-rw-r--r--   0        0        0     3627 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/abe/src/scope/help.rs
+-rw-r--r--   0        0        0     2677 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/abe/src/scope/logic.rs
+-rw-r--r--   0        0        0      875 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/abe/src/scope/mod.rs
+-rw-r--r--   0        0        0     5438 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/abe/src/scope/uint.rs
+-rw-r--r--   0        0        0     1585 1970-01-01 00:00:00.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-common/Cargo.toml
+-rw-r--r--   0        0        0    16725 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-common/LICENSE
+-rw-r--r--   0        0        0       99 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-common/README.md
+-rw-r--r--   0        0        0     2114 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-common/src/bus.rs
+-rw-r--r--   0        0        0     8214 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-common/src/cli/keys.rs
+-rw-r--r--   0        0        0     4693 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-common/src/cli/mod.rs
+-rw-r--r--   0        0        0     7787 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-common/src/cli/opts.rs
+-rw-r--r--   0        0        0     8801 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-common/src/cli/reader.rs
+-rw-r--r--   0        0        0     7337 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-common/src/dgp.rs
+-rw-r--r--   0        0        0     8479 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-common/src/eval.rs
+-rw-r--r--   0        0        0     1217 2023-06-23 08:46:36.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-common/src/lib.rs
+-rw-r--r--   0        0        0     2946 2023-06-21 12:24:07.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-common/src/pkt_reader.rs
+-rw-r--r--   0        0        0     2130 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-common/src/pkt_stream_utils.rs
+-rw-r--r--   0        0        0     4080 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-common/src/predicate_aliases.rs
+-rw-r--r--   0        0        0      448 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-common/src/prelude.rs
+-rw-r--r--   0        0        0     5170 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-common/src/protocols/handshake.rs
+-rw-r--r--   0        0        0     5964 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-common/src/protocols/impex/blob.rs
+-rw-r--r--   0        0        0     4257 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-common/src/protocols/impex/blobmap/checkin.rs
+-rw-r--r--   0        0        0     3093 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-common/src/protocols/impex/blobmap/checkout.rs
+-rw-r--r--   0        0        0     3757 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-common/src/protocols/impex/blobmap/mod.rs
+-rw-r--r--   0        0        0     1029 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-common/src/protocols/impex/mod.rs
+-rw-r--r--   0        0        0     6707 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-common/src/protocols/lns/admin.rs
+-rw-r--r--   0        0        0     6960 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-common/src/protocols/lns/claim.rs
+-rw-r--r--   0        0        0     8286 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-common/src/protocols/lns/eval.rs
+-rw-r--r--   0        0        0      635 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-common/src/protocols/lns/file_claim.rs
+-rw-r--r--   0        0        0     1390 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-common/src/protocols/lns/local_claim.rs
+-rw-r--r--   0        0        0     6873 2023-06-21 12:24:07.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-common/src/protocols/lns/mod.rs
+-rw-r--r--   0        0        0     5062 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-common/src/protocols/lns/name.rs
+-rw-r--r--   0        0        0     5898 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-common/src/protocols/lns/public_claim.rs
+-rw-r--r--   0        0        0      950 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-common/src/protocols/lns/utils.rs
+-rw-r--r--   0        0        0      398 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-common/src/protocols/mod.rs
+-rw-r--r--   0        0        0     4386 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-common/src/runtime/handlers.rs
+-rw-r--r--   0        0        0      292 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-common/src/runtime/mod.rs
+-rw-r--r--   0        0        0    19220 2023-06-23 08:46:36.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-common/src/runtime/rx.rs
+-rw-r--r--   0        0        0     3089 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-common/src/runtime/threads.rs
+-rw-r--r--   0        0        0     4895 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-common/src/static_env.rs
+-rw-r--r--   0        0        0     2843 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-common/src/tests.rs
+-rw-r--r--   0        0        0      787 1970-01-01 00:00:00.000000 linkspace-0.3.0rc2/Cargo.toml
+-rw-r--r--   0        0        0      811 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/Makefile
+-rw-r--r--   0        0        0      246 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/README.md
+-rw-r--r--   0        0        0    13672 2023-06-21 12:25:29.000000 linkspace-0.3.0rc2/linkspace.pyi
+-rw-r--r--   0        0        0      273 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/publish.sh
+-rw-r--r--   0        0        0      163 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/pyproject.toml
+-rw-r--r--   0        0        0      144 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/pyrightconfig.json
+-rw-r--r--   0        0        0    21874 2023-06-21 12:30:59.000000 linkspace-0.3.0rc2/src/lib.rs
+-rw-r--r--   0        0        0     9858 2023-06-21 12:30:16.000000 linkspace-0.3.0rc2/src/pynetpkt.rs
+-rw-r--r--   0        0        0      640 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/tests/nested_watch.py
+-rw-r--r--   0        0        0    68124 2023-06-23 09:29:07.000000 linkspace-0.3.0rc2/Cargo.lock
+-rw-r--r--   0        0        0      583 1970-01-01 00:00:00.000000 linkspace-0.3.0rc2/PKG-INFO
```

### Comparing `linkspace-0.1.4/local_dependencies/ipcbus/Cargo.toml` & `linkspace-0.3.0rc2/local_dependencies/ipcbus/Cargo.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 [package]
 name = "ipcbus"
 version = "0.1.0"
 edition = "2021"
 license = "MPL-2.0"
-authors = ["Azon <AntonSol919@gmail.com>"]
+authors = ["Anton Sol <AntonSol919@gmail.com>"]
 repository = "https://github.com/AntonSol919/linkspace"
 categories = []
 keywords = []
 description = "Cross platform IPC bus"
+resolver = "2"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [features]
 default = []
 [dependencies]
 
-tracing = "0.1.35"
-[target.'cfg(not(target_arch = "wasm32"))'.dependencies]
-fslock = {version="0.2.1"}
+tracing= {version = "=0.1.37",features=["release_max_level_info"]}
+libc= "=0.2.142"
+
 socket2 = { version = "0.4.4", features = ["all"]}
 nix = "0.24.1"
-libc = "0.2"
 event-listener = "2.5.2"
 
 [target.'cfg(target_arch = "wasm32")'.dependencies]
 futures = "0.3.21"
+
+[target.'cfg(not(target_arch = "wasm32"))'.dependencies]
+fslock = {version="0.2.1"}
```

### Comparing `linkspace-0.1.4/local_dependencies/ipcbus/LICENSE` & `linkspace-0.3.0rc2/local_dependencies/linkspace/LICENSE`

 * *Files identical despite different names*

### Comparing `linkspace-0.1.4/local_dependencies/ipcbus/src/lib.rs` & `linkspace-0.3.0rc2/local_dependencies/ipcbus/src/lib.rs`

 * *Files identical despite different names*

### Comparing `linkspace-0.1.4/local_dependencies/ipcbus/src/procbus.rs` & `linkspace-0.3.0rc2/local_dependencies/ipcbus/src/procbus.rs`

 * *Files 1% similar despite different names*

```diff
@@ -65,15 +65,15 @@
             proc: Default::default(),
         }
     }
     pub fn init_udp(self: &mut Arc<Self>) {
         self.init_udp_port(get_port(self.bus_id))
     }
     pub fn init_udp_port(self: &mut Arc<Self>, port: u16) {
-        let mut this = Arc::get_mut(self).expect("You must init_udp before cloning a env");
+        let this = Arc::get_mut(self).expect("You must init_udp before cloning a env");
         assert!(this.ipc.is_none());
         let pid = std::process::id();
         this.ipc = Some((pid, UdpIPC::new(port)));
         tracing::debug!(port = port, pid = pid, "Init udp")
     }
 
     pub fn emit(&self, val: u64) -> u64 {
```

### Comparing `linkspace-0.1.4/local_dependencies/ipcbus/src/udp_multicast.rs` & `linkspace-0.3.0rc2/local_dependencies/ipcbus/src/udp_multicast.rs`

 * *Files identical despite different names*

### Comparing `linkspace-0.1.4/local_dependencies/ipcbus/src/wasmbus.rs` & `linkspace-0.3.0rc2/local_dependencies/ipcbus/src/wasmbus.rs`

 * *Files identical despite different names*

### Comparing `linkspace-0.1.4/local_dependencies/abe/Cargo.toml` & `linkspace-0.3.0rc2/Cargo.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,20 +1,25 @@
 [package]
+name = "linkspace-py"
 
-name = "abe"
-version = "0.1.0"
-license = "MPL-2.0"
-edition = "2021"
-homepage = "https://antonsol919.github.io/linkspace/"
-documentation = "https://antonsol919.github.io/linkspace/docs/guide/index.html#ABE"
-authors = ["Azon <AntonSol919@gmail.com>"]
-repository = "https://github.com/AntonSol919/linkspace"
-categories = ["encoding","parsing"]
-keywords = ["ascii-byte-expr", "ascii-byte","abe"]
-description = "Ascii-byte-expression : a tiny byte templating language"
+version ="0.3.0-rc2"
+authors= ["Anton Sol <AntonSol919@gmail.com>"]
+edition= "2021"
+license= "MPL-2.0"
+homepage= "https://www.linkspace.dev"
+documentation= "https://www.linkspace.dev/docs/guide/index.html"
+repository= "https://github.com/AntonSol919/linkspace"
+resolver = "2"
+
+[lib]
+name = "linkspace"
+crate-type = ["cdylib"]
 
 [dependencies]
-thiserror = "1.0.31"
-hex = "0.4.3"
-serde = { version = "1.0.139", features = ["derive"] }
-arrayvec = "0.7.2"
-anyhow = "1.0.69"
+linkspace = { path = "local_dependencies/linkspace", version ="0.3.0-rc1"}
+
+anyhow= "=1.0.71"
+tracing= {version = "=0.1.37",features=["release_max_level_info"]}
+tracing-subscriber = { version = "=0.3.17", features = ["env-filter"] }
+
+pyo3 = { version = "0.18.2", features = ["extension-module","anyhow","abi3","serde","abi3-py38"]  }
+smallvec = {version="1.10.0",features=["const_new","const_generics","write"]}
```

### Comparing `linkspace-0.1.4/local_dependencies/abe/LICENSE` & `linkspace-0.3.0rc2/local_dependencies/ipcbus/LICENSE`

 * *Files identical despite different names*

### Comparing `linkspace-0.1.4/local_dependencies/abe/src/abe_macro.rs` & `linkspace-0.3.0rc2/local_dependencies/abe/src/abe_macro.rs`

 * *Files identical despite different names*

### Comparing `linkspace-0.1.4/local_dependencies/abe/src/abtxt.rs` & `linkspace-0.3.0rc2/local_dependencies/abe/src/abtxt.rs`

 * *Files identical despite different names*

### Comparing `linkspace-0.1.4/local_dependencies/abe/src/ast.rs` & `linkspace-0.3.0rc2/local_dependencies/abe/src/ast.rs`

 * *Files identical despite different names*

### Comparing `linkspace-0.1.4/local_dependencies/abe/src/convert.rs` & `linkspace-0.3.0rc2/local_dependencies/abe/src/convert.rs`

 * *Files 0% similar despite different names*

```diff
@@ -153,26 +153,27 @@
 pub type AnyABE = TypedABE<ABList>;
 impl From<Vec<ABE>> for AnyABE {
     fn from(value: Vec<ABE>) -> Self {
         TypedABE(value,PhantomData)
     }
 }
 
+
 impl ABEValidator for String {
     fn check(b: &[ABE]) -> Result<(), MatchError> {
         let [_] = exact(b)?;
         Ok(())
     }
 }
 impl TryFrom<ABList> for String {
     type Error = ABEError<FromUtf8Error>;
     fn try_from(value: ABList) -> Result<Self, Self::Error> {
         let b = value.into_exact_bytes().map_err(|_| {
             ABEError::MatchError(MatchError {
-                at: "".into(),
+                at: String::new(),
                 err: MatchErrorKind::ExpectedExpr,
             })
         })?;
         String::from_utf8(b).map_err(ABEError::TryFrom)
     }
 }
 pub fn eval_vec<A: ABEValidator>(
```

### Comparing `linkspace-0.1.4/local_dependencies/abe/src/lib.rs` & `linkspace-0.3.0rc2/local_dependencies/abe/src/lib.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 // Copyright Anton Sol
 //
 // This Source Code Form is subject to the terms of the Mozilla Public
 // License, v. 2.0. If a copy of the MPL was not distributed with this
 // file, You can obtain one at https://mozilla.org/MPL/2.0/.
 #![feature(
+    slice_as_chunks,
     split_as_slice,
     split_array,
     try_trait_v2,
     iterator_try_collect,
     array_chunks,
     associated_type_bounds,
     type_alias_impl_trait,
     bigint_helper_methods
 )]
 pub mod abe_macro;
 pub mod abtxt;
 pub mod ast;
 pub mod convert;
 pub mod eval;
+pub mod scope;
 pub use thiserror;
 
 use std::error::Error;
 use std::fmt::{Debug, Display};
 
 pub use ast::{parse_abe, parse_abe_b, print_abe, ABE};
 pub use convert::{ABEValidator, ToABE, TypedABE};
```

### Comparing `linkspace-0.1.4/local_dependencies/linkspace-core/LICENSE` & `linkspace-0.3.0rc2/local_dependencies/linkspace-cryptography/LICENSE`

 * *Files identical despite different names*

### Comparing `linkspace-0.1.4/local_dependencies/linkspace-core/src/env/db/lmdb.rs` & `linkspace-0.3.0rc2/local_dependencies/linkspace-core/src/env/lmdb/db.rs`

 * *Files 2% similar despite different names*

```diff
@@ -13,20 +13,20 @@
 use lmdb_sys as ffi;
 use std::io;
 use std::io::{ErrorKind, Result};
 use std::{fmt::Debug, io::Write, marker::PhantomData, mem::size_of, path::Path, sync::Arc};
 
 use crate::{env::write_result::WriteResult, prelude::TreeValueBytes};
 
-use super::{assert_align, IterDirection};
-
 #[derive(Clone)]
 pub struct RawBTreeEnv(Arc<LMDBEnv>);
 pub use lmdb::Error;
 
+use super::misc::{ Refreshable, assert_align,  Cursors};
+
 pub type WriteTxn<'o> = LMDBTxn<lmdb::RwTransaction<'o>>;
 pub type MutHashCursor<'o> = UniqCursor<'o, [u8; 32], RwCursor<'o>>;
 pub type MutTreeCursor<'o> = MultiCursor<'o, RwCursor<'o>>;
 pub type MutPktCursor<'o> = UniqCursor<'o, u64, RwCursor<'o>>;
 
 pub type ReadTxn = LMDBTxn<lmdb::RoTransaction<'static>>;
 pub type HashCursor<'o> = UniqCursor<'o, [u8; 32], RoCursor<'o>>;
@@ -64,15 +64,15 @@
             .open(path)
         {
             Ok(env) => return env,
             Err(e) => Err(e),
         };
         let os_err = std::io::Error::last_os_error();
         if os_err.kind() == ErrorKind::OutOfMemory {
-            panic!("{os_err:?}\nLINKSPACE_LMDB_MAPSIZE={mapsize}");
+            panic!("{os_err:?}\nLK_LMDB_MAPSIZE={mapsize}");
         }
         tracing::warn!(?i, ?err, ?os_err, "DB Open");
         if i == 5 {
             tracing::error!(?i, ?err, ?os_err, "DB Open");
         }
         std::thread::sleep(std::time::Duration::from_millis(50 + 200 * i));
     }
@@ -100,14 +100,15 @@
         io::Error::from_raw_os_error(i)
     } else {
         io::Error::other(e)
     }
 }
 
 pub fn open(path: &Path, make_dir: bool) -> std::io::Result<RawBTreeEnv> {
+    tracing::trace!(?path,make_dir,"open db");
     path.as_os_str().to_str().ok_or(io::Error::new(
         io::ErrorKind::Other,
         "Path must be valid utf8",
     ))?; // not really but it makes some api's easier
     if make_dir {
         std::fs::create_dir_all(path)?
     };
@@ -120,16 +121,16 @@
     }
     let idfile = path.join("id");
     if let Ok(mut file) = std::fs::File::create_new(&idfile) {
         let id: [u8; 8] = linkspace_pkt::now().0;
         file.write_all(&id)?;
         file.flush()?;
     }
-    let mapsize = std::env::var("LINKSPACE_LMDB_MAPSIZE")
-        .map(|v| v.parse().expect("LINKSPACE_LMDB_MAPSIZE to be u32"))
+    let mapsize = std::env::var("LK_LMDB_MAPSIZE")
+        .map(|v| v.parse().expect("LK_LMDB_MAPSIZE to be u32"))
         .unwrap_or(DEFAULT_MAP_SIZE);
     let env = Arc::new(open_env(
         path,
         mapsize,
         EnvironmentFlags::empty() | EnvironmentFlags::WRITE_MAP | EnvironmentFlags::NO_TLS,
     ));
     let primary = env
@@ -237,15 +238,15 @@
         tracing::trace!("commit txn");
         self.txn.take().unwrap().commit().map_err(as_io)?;
         self.txn =
             unsafe { std::mem::transmute(Some(self.env.0.env.begin_rw_txn().map_err(as_io)?)) };
         Ok(())
     }
 }
-impl<'o, TXN: 'o + lmdb::Transaction> super::Cursors for LMDBTxn<TXN> {
+impl<'o, TXN: 'o + lmdb::Transaction> Cursors for LMDBTxn<TXN> {
     fn pkt_cursor(&self) -> PktLogCursor {
         UniqCursor::new_pkt(
             self.txn
                 .as_ref()
                 .unwrap()
                 .open_ro_cursor(self.env.0.primary)
                 .unwrap(),
@@ -266,15 +267,15 @@
                 .as_ref()
                 .unwrap()
                 .open_ro_cursor(self.env.0.hash)
                 .unwrap(),
         )
     }
 }
-impl super::Refreshable for ReadTxn {
+impl Refreshable for ReadTxn {
     fn refresh(&mut self) {
         tracing::trace!("Refresh");
         self.txn = Some(self.txn.take().unwrap().reset().renew().unwrap());
     }
 }
 
 impl<'txn> PktLogCursor<'txn> {
@@ -404,15 +405,15 @@
     pub fn iter_dup(self, value_asc: bool) -> IterDup<'txn> {
         IterDup {
             cur: self.0,
             value_asc,
         }
     }
 
-    #[allow(dead_code)]
+    /*
     pub(crate) fn range_multi(
         self,
         start: &[u8],
         dir: IterDirection,
         uniq_keys: bool,
     ) -> impl Iterator<Item = (&'txn [u8], &'txn [u8; size_of::<TreeValueBytes>()])> {
         let mut op = ffi::MDB_GET_CURRENT;
@@ -464,25 +465,25 @@
                         Err(e) => panic!("Cast error? {val:?} {e:?}"),
                     }
                 }
             }
         })
     }
 
-    #[allow(dead_code)]
     pub(crate) fn read_next(
         &mut self,
         start: &[u8],
     ) -> Result<Option<(&'txn [u8], &'txn [u8; size_of::<TreeValueBytes>()])>> {
         match self.0.get(Some(start), None, lmdb_sys::MDB_SET_RANGE) {
             Ok((Some(key), val)) => Ok(Some((key, val.try_into().unwrap()))),
             Err(Error::NotFound) => Ok(None),
             e => todo!("{:?}", e),
         }
     }
+    */
 }
 
 impl<'txn> MutPktCursor<'txn> {
     pub(crate) fn last(&mut self) -> (u64, &'txn [u8]) {
         match self.0.get(None, None, ffi::MDB_LAST) {
             Ok((Some(v), bytes)) => return (u64::from_ne_bytes(v.try_into().unwrap()), bytes),
             Ok((None, _)) => tracing::error!("Error getting last idx"),
@@ -495,15 +496,15 @@
         &mut self,
         idx: u64,
         len: usize,
         insert: impl FnOnce(&mut [u8]),
     ) -> Result<()> {
         let cur = self.0.cursor();
         use std::ptr;
-        let len = ((len + 3) / 4) * 4; // proper allignment
+        assert!(len%4 == 0, "bad alignment?");
         let key = idx.to_ne_bytes();
         tracing::trace!(idx=?key,"Write new Pkt");
         let mut key_val: ffi::MDB_val = ffi::MDB_val {
             mv_size: key.len() as libc::size_t,
             mv_data: key.as_ptr() as *mut libc::c_void,
         };
         let mut data_val: ffi::MDB_val = ffi::MDB_val {
```

### Comparing `linkspace-0.1.4/local_dependencies/linkspace-core/src/env/mod.rs` & `linkspace-0.3.0rc2/local_dependencies/linkspace-core/src/env/lmdb/mod.rs`

 * *Files 13% similar despite different names*

```diff
@@ -1,59 +1,44 @@
-// Copyright Anton Sol
-//
-// This Source Code Form is subject to the terms of the Mozilla Public
-// License, v. 2.0. If a copy of the MPL was not distributed with this
-// file, You can obtain one at https://mozilla.org/MPL/2.0/.
-// the db is duck type compatible between inmem and lmdb
-use crate::{consts::PUBLIC_GROUP_PKT, LNS_ROOTS };
-use anyhow::{Context  };
-use linkspace_pkt::{NetPkt, Stamp, PointExt, AB };
+use std::{sync::{Arc, OnceLock}, path::{Path,PathBuf},fmt::Debug, io::{Write, self} };
+
+use anyhow::Context;
+pub use ipcbus::ProcBus;
+use linkspace_pkt::{ Stamp, PUBLIC_GROUP_PKT, NetPkt, AB, NetPktExt };
 use tracing::instrument;
-use std::{
-    fmt::Debug,
-    io::{self, Write},
-    path::{Path, PathBuf},
-    sync::Arc,
-    sync::OnceLock,
-};
-use write_trait::save_pkt;
-
-use self::queries::IReadTxn;
-pub use self::{
-    db::{Error, RawBTreeEnv, Refreshable, WriteTxn},
-    queries::ReadTxn,
-    write_trait::SWrite,
-};
+use crate::{env::write_trait::save_pkt, LNS_ROOTS};
+
+use self::{db::RawBTreeEnv, queries::{IReadTxn, ReadTxn}};
+
+use super::write_trait::SWrite;
+
 
 pub mod db;
-pub mod tree_key;
-//pub mod tree_query;
+pub mod misc;
+pub mod tree_iter;
 pub mod queries;
 pub mod queries2;
-pub mod query_mode;
-pub mod write_result;
-pub mod write_trait;
+
+/// A [NetPktPtr] and a recv stamp
+
 
 pub type BusCall = Arc<dyn Fn(Stamp) + Send + Sync + 'static>;
 pub static BUS: OnceLock<BusCall> = OnceLock::new();
 #[derive(Clone)]
 pub struct BTreeEnv {
     inner: RawBTreeEnv,
     location: Arc<PathBuf>,
     pub log_head: Arc<ipcbus::ProcBus>,
 }
 impl Debug for BTreeEnv {
     fn fmt(&self, f: &mut std::fmt::Formatter<'_>) -> std::fmt::Result {
         f.debug_struct("BTreeEnv").finish()
     }
 }
-pub use ipcbus::ProcBus;
-
 impl BTreeEnv {
-    pub fn location(&self) -> &Path {
+    pub fn dir(&self) -> &Path {
         &self.location
     }
     pub fn open(path: PathBuf, make_dir: bool) -> io::Result<BTreeEnv> {
         let inner = db::open(&path, make_dir)?;
         let location = Arc::new(path.canonicalize()?);
         tracing::debug!(?location, "Opening BTreeEnv");
         let log_head = ipcbus::ProcBus::new(inner.uid());
@@ -61,54 +46,52 @@
             inner,
             log_head: Arc::new(log_head),
             location,
         };
         {
             let mut writer = env.inner.write_txn()?;
             let new = save_pkt(&mut writer, &**PUBLIC_GROUP_PKT)?;
-            if new {
-            let mut bytes = LNS_ROOTS;
-            let roots:Vec<_> = std::iter::from_fn(||{
-                if bytes.len() == 0 { return None;}
-                let pkt = crate::pkt::read::parse_netpkt(bytes, false).unwrap().unwrap();
-                let pkt = pkt.as_netbox();
-                bytes = &bytes[pkt.net_pkt_size()..];
-                Some(pkt)
-            }).collect();
-            let mut it = roots.iter().map(|p| &*p as &dyn NetPkt);
-            let (i,_) = writer.write_many_state(&mut it, None).unwrap();
-                assert_eq!(i,464);
+            if new && std::env::var_os("LK_NO_LNS").is_none(){
+                let mut bytes = LNS_ROOTS;
+                let roots:Vec<_> = std::iter::from_fn(||{
+                    if bytes.is_empty() { return None;}
+                    let pkt = crate::pkt::read::read_pkt(bytes, true).unwrap();
+                    bytes = &bytes[pkt.size() as usize..];
+                    Some(pkt)
+                }).collect();
+                let mut it = roots.iter().map(|p| p.as_ref() as &dyn NetPkt);
+                let (_i,_) = writer.write_many_state(&mut it, None).unwrap();
             }
         }
         Ok(env)
     }
 
     pub fn local_enckey(&self) -> anyhow::Result<String> {
         // TODO this should prob check for read only access
         Ok(std::fs::read_to_string(self.location.join("local_auth"))?.lines().next().context("missing enckey")?.to_owned())
     }
     #[instrument(ret,skip(bytes))]
-    pub fn set_env_data(&self, path: impl AsRef<std::path::Path>+std::fmt::Debug, bytes: &[u8],overwrite:bool) -> anyhow::Result<()>{
+    pub fn set_files_data(&self, path: impl AsRef<std::path::Path>+std::fmt::Debug, bytes: &[u8],overwrite:bool) -> anyhow::Result<()>{
         tracing::trace!(bytes=%AB(bytes));
-        let path = self.location().join("env").join(check_path(path.as_ref())?);
+        let path = self.dir().join("files").join(check_path(path.as_ref())?);
         let r: anyhow::Result<()> = try {
             std::fs::create_dir_all(path.parent().unwrap())?;
             let mut file = if overwrite {
                 std::fs::OpenOptions::new().write(true).create(true).truncate(true).open(&path)?
             }else {
                 std::fs::OpenOptions::new().create_new(true).write(true).open(&path)?
             };
             file.write_all(bytes)?;
         };
         r.with_context(|| anyhow::anyhow!("Target {}",path.to_string_lossy()))
     }
     #[instrument(ret)]
     // notfound_err simplifies context errors
-    pub fn env_data(&self, path: impl AsRef<std::path::Path>+std::fmt::Debug,notfound_err:bool) -> anyhow::Result<Option<Vec<u8>>> {
-        let path = self.location().join("env").join(check_path(path.as_ref())?);
+    pub fn files_data(&self, path: impl AsRef<std::path::Path>+std::fmt::Debug,notfound_err:bool) -> anyhow::Result<Option<Vec<u8>>> {
+        let path = self.dir().join("files").join(check_path(path.as_ref())?);
         use std::io::ErrorKind::*;
         match std::fs::read(&path){
             Ok(k) => Ok(Some(k)),
             Err(e) if !notfound_err && e.kind() == NotFound =>Ok(None),
             Err(e) => Err(e).with_context(|| anyhow::anyhow!("could not open {}",path.to_string_lossy()))
         }
     }
@@ -136,15 +119,15 @@
 pub struct WriteTxn2<'o> {
     txn: Option<db::WriteTxn<'o>>,
     update: &'o ipcbus::ProcBus,
     last: Option<Stamp>,
 }
 
 impl<'o> WriteTxn2<'o> {
-    pub fn reader(&self) -> queries::IReadTxn<&(impl db::Cursors + '_)> {
+    pub fn reader(&self) -> queries::IReadTxn<&(impl misc::Cursors + '_)> {
         tracing::debug!("Peek reader of write txn");
         IReadTxn::new(self.txn.as_ref().unwrap())
     }
     fn set_last(
         &mut self,
         result: io::Result<(usize, Option<Stamp>)>,
     ) -> io::Result<(usize, Option<Stamp>)> {
```

### Comparing `linkspace-0.1.4/local_dependencies/linkspace-core/src/env/queries.rs` & `linkspace-0.3.0rc2/local_dependencies/linkspace-core/src/env/lmdb/queries.rs`

 * *Files 5% similar despite different names*

```diff
@@ -6,36 +6,34 @@
 use std::io;
 use std::io::Result;
 
 use super::db::MutHashCursor;
 use super::db::MutPktCursor;
 use super::db::MutTreeCursor;
 use super::db::PktLogCursor;
-use super::db::Refreshable;
+use super::misc::IterDirection;
+use super::misc::Refreshable;
 use super::db::WriteTxn;
-use super::tree_key::*;
-use super::write_result::WriteResult;
-use super::write_trait::SWrite;
-use crate::env::db::assert_align;
-use crate::env::db::IterDirection;
+use super::misc::assert_align;
+use crate::env::RecvPktPtr;
+use crate::env::tree_key::*;
+use crate::env::write_result::WriteResult;
+use crate::env::write_trait::SWrite;
 use crate::partial_hash::PartialHash;
 use crate::stamp_range::StampRange;
 use either::Either;
-use linkspace_pkt::reroute::RecvPkt;
 use linkspace_pkt::*;
 
 pub fn as_recv_ptr((llp, bytes): (u64, &[u8])) -> RecvPktPtr {
     RecvPktPtr {
         pkt: as_netpkt(bytes),
         recv: Stamp::new(llp),
     }
 }
 
-/// A [NetPktPtr] and a recv stamp
-pub type RecvPktPtr<'o> = RecvPkt<&'o NetPktPtr>;
 
 fn as_netpkt(bytes: &[u8]) -> &NetPktPtr {
     unsafe { NetPktPtr::from_bytes_unchecked(bytes) }
 }
 pub(crate) fn read_pkt<'txn>(
     cur: &PktLogCursor<'txn>,
     recv: Stamp,
@@ -66,52 +64,19 @@
         tracing::trace!("Dropping read txn");
     }
 }
 pub struct IReadTxn<C = super::db::ReadTxn> {
     pub(crate) btree_txn: C,
 }
 
-impl<C: super::db::Cursors> IReadTxn<C> {
+impl<C: super::misc::Cursors> IReadTxn<C> {
     pub(crate) fn new(btree_txn: C) -> Self {
         tracing::trace!("Open txn");
         IReadTxn { btree_txn }
     }
-    /*
-    pub fn validate(&self) -> anyhow::Result<DBStats>{
-        todo!()
-        let mut stats = DBStats::default();
-        {
-
-            let mut hashes = HashSet::new();
-            let mut logptr = 0;
-            let mut list = vec![];
-            for pkt in self.pkts_after(Stamp::ZERO){
-                assert!(logptr < pkt.recv.get());
-                logptr = pkt.recv.get();
-                list.push(logptr);
-                hashes.insert(*pkt.hash());
-            }
-            tracing::info!(list=?list,"pktlist");
-            for (hash,_) in self.partial_hashes(PartialHash::min()){
-                assert!(hashes.contains(hash));
-            }
-            let mut it = list.into_iter().rev();
-            for (pkt,idx) in self.history().zip(&mut it){
-                assert_eq!(idx,pkt.recv.get());
-                if !hashes.remove(pkt.hash()){
-                    panic!()
-                }
-            }
-            assert!(it.next().is_none());
-            stats.pkts = hashes.len();
-        }
-        tracing::info!(stats=?stats,"Validate ok");
-        Ok(stats)
-    }
-     */
 
     /// read a pkt and use the local net header
     pub fn read_ptr(&self, hash: &LkHash) -> Result<Option<Stamp>> {
         match self.btree_txn.hash_cursor().read_uniq(hash)? {
             Some(idx) => Ok(Some(Stamp::new(idx))),
             None => Ok(None),
         }
@@ -163,15 +128,14 @@
     ) -> impl Iterator<Item = &NetPktPtr> {
         let c = self.btree_txn.pkt_cursor();
         idx.filter_map(move |p| c.read_uniq(&p.get()).ok().flatten())
             .map(as_netpkt)
     }
     /*
     fn fixed_size_prefix_iter<const N:usize>(&self,_start:[u8;N]) -> impl Iterator<Item = TreeEntryRef<'_>>{
-        #[allow(unreachable_code)]
         std::iter::once(todo!())
         let mut c2 = self.btree_txn.tree_cursor();
         let mut prefix = Some(start);
         use crate::pkt::uint_native::u8_be;
         std::iter::from_fn(move || {
             match c2.read_next(&prefix?).expect("Read ok"){
                 Some((k,val)) => {
@@ -270,22 +234,21 @@
 ) -> Result<WriteResult<()>> {
     let last_idx = { log.last().0 };
     if last_idx > idx.get() {
         todo!()
     }
     let result = hash.try_put_unique(&pkt.hash(), idx.get())?;
     if result.is_new() {
-        log.insert(idx.get(), pkt.size(), |dest| {
+        log.insert(idx.get(), pkt.size() as usize , |dest| {
             assert_align(dest);
             let segments = pkt.byte_segments();
             unsafe { segments.write_segments_unchecked(dest.as_mut_ptr()) };
-            if true {
-                //dbg
+            if cfg!(debug_assertions){
                 let pkt = unsafe { NetPktFatPtr::from_bytes_unchecked(dest) };
-                pkt.check::<true>().unwrap();
+                pkt.check(true).unwrap();
             }
         })?;
         if let Some((key, val)) =
             TreeEntry::from_pkt(idx, pkt).map(|te| (te.btree_key.take(), te.val))
         {
             spk.put_append(&key, &val).unwrap();
         }
@@ -312,14 +275,16 @@
                     Err(e) => return Err(e),
                 };
                 if is_new {
                     tracing::trace!(logidx=?now,hash=%pkt.hash(),"New Written");
                     new += 1;
                     now = Stamp::new(now.get() + 1);
                     last = Some(now);
+                }else {
+                    tracing::trace!(hash=%pkt.hash(),"Old skipped Written");
                 }
                 match cb(pkt, is_new) {
                     Ok(true) => {}
                     Ok(false) => break,
                     Err(_) => return Ok((0, None)),
                 }
             }
```

### Comparing `linkspace-0.1.4/local_dependencies/linkspace-core/src/env/queries2.rs` & `linkspace-0.3.0rc2/local_dependencies/linkspace-core/src/env/lmdb/queries2.rs`

 * *Files 2% similar despite different names*

```diff
@@ -17,42 +17,43 @@
 - A Small stack machine. Something like  (Mem:[u8;256]) ++ vec![Enum{ChangeField, (TestOp,&[u8])}]
 
 
 */
 use crate::pkt::field_ids::FieldEnum;
 use crate::predicate::pkt_predicates::PktPredicates;
 use either::Either;
-use linkspace_pkt::{Stamp, B64, U256 };
+use linkspace_pkt::{Stamp, B64, U256, PktFmt };
 
 use crate::prelude::TestSet;
 use crate::{
     predicate::{
         exprs::RuleType,
         test_pkt::{compile_predicates, PktStreamTest},
     },
-    prelude::{
-        treekey::{spd, TreeKeysIter},
-        IReadTxn, RecvPktPtr, TreeEntryRef,
-    },
+    prelude::{TreeEntryRef}
 };
 
-use super::query_mode::{Mode, Order, Table};
-use super::tree_key::treekey_checked;
+use crate::env::query_mode::{Mode, Order, Table};
+use crate::env::tree_key::treekey_checked;
+
+use crate::env::RecvPktPtr;
+use super::queries::IReadTxn;
+use super::tree_iter::TreeKeysIter;
 
 
-impl<C: super::db::Cursors> IReadTxn<C> {
+impl<C: super::misc::Cursors> IReadTxn<C> {
     pub fn scope_iter<'o>(
         &'o self,
         rules: &PktPredicates,
         order: Order,
     ) -> Option<(TreeEntryRef<'o>, TreeKeysIter<'o>)> {
         let req = rules.compile_tree_keys(order.is_asc()).unwrap();
         let lower_bound = req.lower_bound().unwrap();
         let iter_dup = self.btree_txn.tree_cursor().iter_dup(order.is_asc());
-        let at = iter_dup.set_range(&lower_bound).map(spd)?;
+        let at = iter_dup.set_range(&lower_bound).map(super::tree_iter::spd)?;
         let mut it = TreeKeysIter {
             req,
             iter_dup,
             lower_bound,
         };
         let at = it.set_pointer_at_match(at)?;
         Some((at, it))
@@ -135,23 +136,25 @@
             .map(|(test,_)| test)
             .collect::<Vec<_>>();
         let c1 = self.btree_txn.pkt_cursor();
         let it = self
             .query_tree_entries(predicates, ord)
             .map(move |v| {
                 crate::prelude::read_pkt(&c1, v.local_log_ptr())
-                    .expect("BTree Is inconsistent")
-                    .expect("BTree Is inconsistent")
+                    .map_err(|e|("Btree Error - tree query",v.local_log_ptr(),e))
+                    .unwrap()
+                    .ok_or_else(||("BTree inconsistent - cant find",v.local_log_ptr()))
+                    .unwrap()
             })
             .filter(move |pkt| {
                 let ok = pkt_filter.test(pkt);
-                tracing::trace!(ok,pkt=%linkspace_pkt::pkt_fmt(pkt.pkt),"filter log");
+                tracing::trace!(ok,pkt=%PktFmt(pkt),"filter tree");
                 ok
             });
-        let nth_log_set = predicates.state.i_index.iter(0);
+        let nth_log_set = predicates.state.i_db.iter(0);
 
         it.zip(nth_log_set).filter_map(|(v, ok)| ok.then_some(v))
     }
 
     pub fn query_log2<'o>(
         &'o self,
         ord: Order,
@@ -166,15 +169,15 @@
 
         let nth_find_set = rules.state.i_branch.iter(0);
         let it = it.zip(nth_find_set).filter_map(|(v, ok)| ok.then_some(v));
         let it = it
             .inspect(|p| tracing::trace!(pkt=?&**p,"pkt"))
             .filter(move |pkt| tests.test(**pkt));
 
-        let nth_log_set = rules.state.i_index.iter(0);
+        let nth_log_set = rules.state.i_db.iter(0);
         it.zip(nth_log_set).filter_map(|(v, ok)| ok.then_some(v))
     }
 
     pub fn query_hash_entries(
         &self,
         hashset: TestSet<U256>,
         ord: Order,
@@ -226,15 +229,15 @@
                     .expect("BTree Is inconsistent")
             })
             .filter(move |pkt| {
                 let ok = pkt_filter.test(pkt);
                 tracing::trace!(ok,pkt=%linkspace_pkt::pkt_fmt(pkt.pkt),"filter log");
                 ok
             });
-        let nth_log_set = rules.state.i_index.iter(0);
+        let nth_log_set = rules.state.i_db.iter(0);
 
         it.zip(nth_log_set).filter_map(|(v, ok)| ok.then_some(v))
     }
 
     pub fn query<'o>(
         &'o self,
         mode: Mode,
```

### Comparing `linkspace-0.1.4/local_dependencies/linkspace-core/src/env/query_mode.rs` & `linkspace-0.3.0rc2/local_dependencies/linkspace-core/src/env/query_mode.rs`

 * *Files identical despite different names*

### Comparing `linkspace-0.1.4/local_dependencies/linkspace-core/src/env/tree_key.rs` & `linkspace-0.3.0rc2/local_dependencies/linkspace-core/src/env/tree_key.rs`

 * *Files 1% similar despite different names*

```diff
@@ -207,15 +207,16 @@
     }
 }
 
 
 /// check if this type can be answered by a treekey - currently conservative to simplify tree query impl
 pub const fn treekey_checked(r:RuleType) -> bool {
     match r {
-        RuleType::Field(f) =>match f{
+        #[allow(clippy::match_like_matches_macro)]
+        RuleType::Field(f) => match f{
             FieldEnum::PktHashF => true,
             FieldEnum::PubKeyF => true,
             FieldEnum::GroupIDF => true,
             FieldEnum::DomainF => true,
             FieldEnum::CreateF => true,
             FieldEnum::PathLenF => true,
             FieldEnum::LinksLenF => true,
```

### Comparing `linkspace-0.1.4/local_dependencies/linkspace-core/src/env/write_result.rs` & `linkspace-0.3.0rc2/local_dependencies/linkspace-core/src/env/write_result.rs`

 * *Files identical despite different names*

### Comparing `linkspace-0.1.4/local_dependencies/linkspace-core/src/env/write_trait.rs` & `linkspace-0.3.0rc2/local_dependencies/linkspace-core/src/env/write_trait.rs`

 * *Files identical despite different names*

### Comparing `linkspace-0.1.4/local_dependencies/linkspace-core/src/eval.rs` & `linkspace-0.3.0rc2/local_dependencies/linkspace-core/src/eval.rs`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 // Copyright Anton Sol
 //
 // This Source Code Form is subject to the terms of the Mozilla Public
 // License, v. 2.0. If a copy of the MPL was not distributed with this
 // file, You can obtain one at https://mozilla.org/MPL/2.0/.
 use crate::consts::PRIVATE;
 use crate::consts::PUBLIC;
-use crate::consts::TEST_GROUP_ID;
+use crate::consts::TEST_GROUP;
 pub use crate::stamp_fmt::StampEF;
 pub use linkspace_pkt::abe::eval::*;
 pub use linkspace_pkt::abe::*;
-pub use linkspace_pkt::abe::*;
-use linkspace_pkt::core_scope;
-pub use linkspace_pkt::B64EvalFnc;
-use linkspace_pkt::EvalCore;
 use linkspace_pkt::GroupID;
 use linkspace_pkt::PathFE;
 use linkspace_pkt::B64;
+use linkspace_pkt::abe::scope::EvalCore;
+use linkspace_pkt::abe::scope::core_scope;
 
 pub const EVAL0_1: &str = "0.1";
 
 pub fn std_ctx() -> EvalCtx<EvalStd> {
     std_ctx_v(EVAL0_1)
 }
 pub type EvalStd = (
@@ -46,15 +44,15 @@
     }
     fn list_funcs(&self) -> &[ScopeFunc<&Self>] {
         &[
             ScopeFunc {
                 apply: |_, i, _, _| match i[0] {
                     b"0" => ApplyResult::Value(PRIVATE.0.to_vec()),
                     b"pub" => ApplyResult::Value(PUBLIC.0.to_vec()),
-                    b"test" => ApplyResult::Value(TEST_GROUP_ID.0.to_vec()),
+                    b"test" => ApplyResult::Value(TEST_GROUP.0.to_vec()),
                     _ => ApplyResult::NoValue,
                 },
                 info: ScopeFuncInfo {
                     id: "#",
                     init_eq: Some(true),
                     argc: 1..=16,
                     help: "resolve #:0 , #:pub, and #:test without a db",
@@ -62,15 +60,15 @@
                 },
                 to_abe: |_, i, _| {
                     let g = GroupID::try_fit_slice(i).ok()?;
                     let b = if g == PRIVATE {
                         "[#:0]"
                     } else if g == PUBLIC {
                         "[#:pub]"
-                    } else if g == *TEST_GROUP_ID {
+                    } else if g == *TEST_GROUP {
                         "[#:test]"
                     } else {
                         return ApplyResult::NoValue;
                     };
                     ApplyResult::Value(b.to_string())
                 },
             },
@@ -98,15 +96,15 @@
         ]
     }
 }
 fn _rev_lookup(i: &[&[u8]], group_mode: Option<bool>) -> ApplyResult {
     let b = B64::try_fit_slice(i[0])?;
     match b {
         b if b == PUBLIC => Ok(b"[#:pub]".to_vec()),
-        b if b == *TEST_GROUP_ID => Ok(b"[#:test]".to_vec()),
+        b if b == *TEST_GROUP => Ok(b"[#:test]".to_vec()),
         b if b == PRIVATE => match group_mode {
             Some(false) => Ok(b"[@:none]".to_vec()),
             _ => Ok(b"[#:0]".to_vec()),
         },
         _ => return ApplyResult::NoValue,
     }
     .into()
```

### Comparing `linkspace-0.1.4/local_dependencies/linkspace-core/src/lib.rs` & `linkspace-0.3.0rc2/local_dependencies/linkspace-core/src/lib.rs`

 * *Files 14% similar despite different names*

```diff
@@ -1,48 +1,47 @@
 // Copyright Anton Sol
 //
 // This Source Code Form is subject to the terms of the Mozilla Public
 // License, v. 2.0. If a copy of the MPL was not distributed with this
 // file, You can obtain one at https://mozilla.org/MPL/2.0/.
 #![feature(
+    extract_if,
     thread_local,
     file_create_new,
     let_chains,
     try_blocks,
     io_error_other,
     const_option_ext,
-    const_ptr_read,
     const_bigint_helper_methods,
     concat_idents,
     exact_size_is_empty,
     split_array,
     option_get_or_insert_default,
-    array_zip,
     const_slice_index,
     const_try,
     const_option,
     cell_update,
     concat_bytes,
     bigint_helper_methods,
     control_flow_enum,
     try_trait_v2,
     type_alias_impl_trait,
     duration_constants,
     div_duration,
     never_type,
-    drain_filter,
-    hash_drain_filter,
     lazy_cell
 )]
 pub use parse_display;
 
 pub use linkspace_cryptography as crypto;
 pub use linkspace_pkt as pkt;
 pub mod consts;
+
 pub mod env;
+
 pub mod eval;
 pub mod matcher;
 pub mod mut_header;
 pub mod partial_hash;
 pub mod predicate;
 pub mod prelude;
 pub mod pull;
```

### Comparing `linkspace-0.1.4/local_dependencies/linkspace-core/src/matcher/mod.rs` & `linkspace-0.3.0rc2/local_dependencies/linkspace-core/src/matcher/mod.rs`

 * *Files 11% similar despite different names*

```diff
@@ -2,120 +2,122 @@
 use std::{ops::ControlFlow, cell::Cell};
 
 // Copyright Anton Sol
 //
 // This Source Code Form is subject to the terms of the Mozilla Public
 // License, v. 2.0. If a copy of the MPL was not distributed with this
 // file, You can obtain one at https://mozilla.org/MPL/2.0/.
-use anyhow::{ensure, Context};
+use anyhow::{ensure };
 use linkspace_pkt::{abe::TypedABE, reroute::RecvPkt, NetPkt, NetPktExt, Stamp};
-use tracing::Span;
+use tracing::{Span, instrument};
 
 use crate::{
-    env::queries::RecvPktPtr,
+    env::RecvPktPtr,
     predicate::{
-        pkt_predicates::StatePredicates,
         test_pkt::{compile_predicates, PktStreamTest},
         TestSet,
     },
     prelude::{Bound, Query},
 };
 
-pub type WatchID = Vec<u8>;
-pub type WatchIDRef = [u8];
-pub type WatchIDExpr = TypedABE<Vec<u8>>;
+pub type QueryID = Vec<u8>;
+pub type QueryIDRef = [u8];
+pub type QueryIDExpr = TypedABE<Vec<u8>>;
 
 /// [[WatchEntry]] with no associated context
 pub type BareWatch = WatchEntry<()>;
 #[thread_local]
-static ENTRY_ID:Cell<usize>=Cell::new(0);
+static WATCH_ID:Cell<usize>=Cell::new(0);
+
+#[derive(Copy,Clone)]
+pub struct WatchStatus{
+    pub watch_id : usize,
+    pub nth_query: u32
+}
 
 #[derive(Debug)]
 /// Stored predicates, predicate state, identity, and associated ctx \<C\> ( usually a callback )
 pub struct WatchEntry<C> {
-    pub entry_id: usize,
-    pub id: WatchID,
+    pub watch_id: usize,
+    pub query_id: QueryID,
     pub tests: Vec<Box<dyn PktStreamTest>>,
     pub nth_query: u32,
     pub i_query: TestSet<u32>,
     pub nth_new: u32,
     pub i_new: TestSet<u32>,
     pub recv_bounds: Bound<u64>,
     pub query: Box<Query>,
     pub last_test: (bool, ControlFlow<()>),
     pub ctx: C,
     pub span: tracing::Span,
 }
 impl<C> WatchEntry<C> {
+    pub fn status(&self) -> WatchStatus{
+        WatchStatus { watch_id: self.watch_id, nth_query:self.nth_query }
+    }
+
+    pub fn update_tests(&mut self) -> anyhow::Result<()>{
+        let (it, recv_bounds) = compile_predicates(&self.query.predicates);
+        self.tests = it.map(|(t, _)| t).collect();
+        self.i_new = self.query.predicates.state.i_new;
+        self.i_query = self.query.predicates.state.i_query;
+        self.recv_bounds = recv_bounds;
+        let has_pending = self.i_new.has_any() && self.i_new.info(self.nth_new).val.is_some();
+        ensure!(has_pending, "i_new watch budget empty");
+        let has_qnew = self.i_query.has_any() && self.i_query.info(self.nth_query).val.is_some();
+        ensure!(has_qnew, "i watch budget empty");
+        tracing::info!(parent:&self.span,q=?self.query,"update watch");
+        Ok(())
+    }
+
     pub fn new(
-        id: WatchID,
+        id: QueryID,
         query: Query,
         nth_query: u32,
         ctx: C,
         span: Span,
     ) -> anyhow::Result<Self> {
-        let (it, recv_bounds) = compile_predicates(&query.predicates);
-        let tests = it.map(|(t, _)| t).collect();
-        let StatePredicates {
-            mut i_new, i_query, ..
-        } = query.predicates.state;
-        let nth_new = 0;
-        ensure!(
-            recv_bounds.as_eq().is_none(),
-            "watching for 'eq' recv is nonsense"
-        );
-        // With this, we only need to check i_new.less_eq < i_new to determine if our watch has ended
-        if i_query.bound.high != u32::MAX {
-            let less = (i_query.bound.high + 1)
-                .checked_sub(nth_query)
-                .context("Empty i_new and i_query combo")?;
-            i_new
-                .try_add(crate::predicate::TestOp::Less, less)
-                .context("empty i_new and i_query combination")?;
-        }
-        tracing::trace!(?i_new, ?i_query, ?recv_bounds, ?nth_query, "Watch budgets");
-
-        ensure!(i_new.has_any(), "watch budget empty");
-        ensure!(i_query.info(nth_query).val.is_some(), "watch budget empty");
-        Ok(WatchEntry {
-            entry_id: ENTRY_ID.update(|i| i.saturating_add(1)),
-            id,
-            query: Box::new(query),
-            tests,
-            recv_bounds,
-            i_new,
-            nth_new,
-            i_query,
+        let mut watch = WatchEntry {
+            watch_id: WATCH_ID.update(|i| i.saturating_add(1)),
+            query_id: id,
+            tests:vec![],
+            recv_bounds:Bound::DEFAULT,
+            i_new:TestSet::DEFAULT,
+            nth_new:0,
+            i_query:TestSet::DEFAULT,
             nth_query,
             ctx,
             span,
+            query: Box::new(query),
             last_test: (false, ControlFlow::Continue(())),
-        })
+        };
+        watch.update_tests()?;
+        Ok(watch)
     }
     pub fn map<N>(self, new_ctx: N) -> (C, WatchEntry<N>) {
         let WatchEntry {
-            entry_id,
+            watch_id,
             tests,
-            id,
+            query_id: id,
             query,
             ctx,
             span,
             recv_bounds,
             nth_query,
             i_query,
             nth_new,
             i_new,
             last_test,
         } = self;
         (
             ctx,
             WatchEntry {
-                entry_id,
+                watch_id,
                 tests,
-                id,
+                query_id: id,
                 query,
                 ctx: new_ctx,
                 span,
                 recv_bounds,
                 nth_query,
                 i_query,
                 nth_new,
@@ -154,15 +156,15 @@
         }
         let accepted_nth = self.i_new.test(self.nth_new) && self.i_query.test(self.nth_query);
         tracing::trace!(accepted_nth, "accepted");
         self.nth_new += 1;
         self.nth_query += 1;
         (
             accepted_nth,
-            if self.i_new.bound.high < self.nth_new {
+            if self.nth_new > self.i_new.bound.high || self.nth_query > self.i_query.bound.high{
                 ControlFlow::Break(())
             } else {
                 ControlFlow::Continue(())
             },
         )
     }
 }
@@ -174,55 +176,55 @@
     fn default() -> Self {
         Self {
             watch_entries: Vec::new(),
         }
     }
 }
 impl<C> Matcher<C> {
-    pub fn get(&self, watch_id: &WatchIDRef) -> Option<&WatchEntry<C>>{
+    pub fn get(&self, id: &QueryIDRef) -> Option<&WatchEntry<C>>{
         self
             .watch_entries
-            .binary_search_by_key(&watch_id, |e| &e.id).ok().and_then(|i|self.watch_entries.get(i))
+            .binary_search_by_key(&id, |e| &e.query_id).ok().and_then(|i|self.watch_entries.get(i))
     }
     pub fn register(&mut self, watch_e: WatchEntry<C>) -> Option<WatchEntry<C>> {
         let ok = watch_e.recv_bounds.high > linkspace_pkt::now().get();
         tracing::debug!(register_ok=?ok);
         match (
             ok,
             self.watch_entries
-                .binary_search_by_key(&watch_e.id.as_ref(), |v| &v.id),
+                .binary_search_by_key(&watch_e.query_id.as_ref(), |v| &v.query_id),
         ) {
             (true, Ok(i)) => Some(::std::mem::replace(&mut self.watch_entries[i], watch_e)),
             (false, Ok(i)) => Some(self.watch_entries.remove(i)),
             (true, Err(i)) => {
                 self.watch_entries.insert(i, watch_e);
                 None
             }
             (false, Err(_i)) => None,
         }
     }
     pub fn deregister(
         &mut self,
-        watch_id: &WatchIDRef,
+        id: &QueryIDRef,
         range: bool,
         mut on_drop: impl FnMut(WatchEntry<C>),
     ) -> usize {
         match self
             .watch_entries
-            .binary_search_by_key(&watch_id, |e| &e.id)
+            .binary_search_by_key(&id, |e| &e.query_id)
         {
             Ok(i) => {
                 if !range {
                     let w = self.watch_entries.remove(i);
                     on_drop(w);
                     1
                 } else {
                     let c = self.watch_entries[i..]
                         .iter()
-                        .take_while(|v| v.id.starts_with(watch_id))
+                        .take_while(|v| v.query_id.starts_with(id))
                         .count();
                     for w in self.watch_entries.drain(i..c + i) {
                         on_drop(w)
                     }
                     c
                 }
             }
@@ -232,35 +234,38 @@
     pub fn trigger(
         &mut self,
         pkt: RecvPktPtr,
         mut on_match: impl FnMut(&mut C) -> ControlFlow<()>,
         on_drop: impl FnMut(WatchEntry<C>),
     ) {
         self.watch_entries
-            .drain_filter(|e| {
+            .extract_if(|e| {
                 let _g = e.span.clone().entered();
                 let (test_ok, test_finish) = e.test(pkt);
                 let callback_finish =
                     (test_ok && on_match(&mut e.ctx).is_break()) || test_finish.is_break();
                 tracing::debug!(test_ok, ?test_finish, callback_finish);
                 callback_finish
             })
             .for_each(on_drop);
     }
     /// clears out of bound watches and determine when the next gc should be run ( none means empty, Some(MAX) means no oob set)
+    #[instrument(skip(self))]
     pub fn gc(&mut self, logptr: Stamp) -> Option<Stamp> {
         let mut min: u64 = u64::MAX;
+        let old_len = self.watch_entries.len();
         self.watch_entries.retain(|e| {
             if e.recv_bounds.high > logptr.get() {
                 min = e.recv_bounds.high.min(min);
                 true
             } else {
                 false
             }
         });
+        tracing::trace!(old_len,len=self.watch_entries.len());
         if self.watch_entries.is_empty() {
             None
         } else {
             Some(min.into())
         }
     }
     pub fn entries(&self) -> &[WatchEntry<C>] {
```

### Comparing `linkspace-0.1.4/local_dependencies/linkspace-core/src/mut_header.rs` & `linkspace-0.3.0rc2/local_dependencies/linkspace-core/src/mut_header.rs`

 * *Files identical despite different names*

### Comparing `linkspace-0.1.4/local_dependencies/linkspace-core/src/partial_hash.rs` & `linkspace-0.3.0rc2/local_dependencies/linkspace-core/src/partial_hash.rs`

 * *Files 8% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 // file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
 
 use crate::consts::B64_HASH_LENGTH;
 pub use arrayvec;
 use arrayvec::ArrayString;
 use linkspace_pkt::{base64_crate, LkHash};
-use serde::{Deserialize, Serialize};
 use std::{convert::TryFrom, fmt, str::FromStr};
 use thiserror::Error;
+use base64_crate::prelude::*;
 
 #[derive(Error, Debug)]
 pub enum Error {
     #[error("Base 64 Error")]
     B64Decode(#[from] base64_crate::DecodeError),
     #[error("To many chars")]
     MaxLengthError,
@@ -26,33 +26,28 @@
 /*
 A partial b64 hash.
 Note that this is a string comparison.
 b64 decoding rules regarding 1 or 2 characters are ignored
 */
 
 #[derive(
-    Default, Debug, Clone, Copy, Eq, Hash, PartialEq, Serialize, Deserialize, PartialOrd, Ord,
+    Default, Debug, Clone, Copy, Eq, Hash, PartialEq, PartialOrd, Ord,
 )]
 
 pub struct PartialHash(pub ArrayString<B64_HASH_LENGTH>);
 impl PartialHash {
     pub fn min() -> PartialHash {
         PartialHash::from_str("AAAA").unwrap()
     }
     pub fn complete_try_into(&self) -> Option<linkspace_pkt::LkHash> {
         if !self.0.is_full() {
             return None;
         }
         let mut res = [0; 32];
-        base64_crate::decode_config_slice(
-            self.0.as_bytes(),
-            base64_crate::URL_SAFE_NO_PAD,
-            res.as_mut_slice(),
-        )
-        .ok()?;
+        BASE64_URL_SAFE_NO_PAD.decode_slice_unchecked(self.0.as_bytes(), res.as_mut_slice()).ok()?;
         Some(res.into())
     }
     pub fn as_str(&self) -> &str {
         self.0.as_str()
     }
     pub fn str_matches(&self, hash: &LkHash) -> bool {
         let t = self.0.as_str();
@@ -68,31 +63,28 @@
     // Gives a good starting point for searching in an ordered list of Hashes's
     // Because b64 encodes 6 bits per char we only give an aprox.
     // i.e. while searching dont forget to skip while cursor.b64() < partial.
     pub fn aprox_btree_idx(&self) -> [u8; 32] {
         let mut res = [0; 32];
         let mut st = [b'A'; B64_HASH_LENGTH];
         st[0..self.0.as_bytes().len()].copy_from_slice(self.0.as_bytes());
-        base64_crate::decode_config_slice(
-            unsafe { std::str::from_utf8_unchecked(&st) },
-            base64_crate::URL_SAFE_NO_PAD,
-            res.as_mut_slice(),
-        )
-        .unwrap();
+
+        let st = unsafe { std::str::from_utf8_unchecked(&st) };
+        BASE64_URL_SAFE_NO_PAD.decode_slice_unchecked(st,res.as_mut_slice()).unwrap();
         res
     }
     pub fn try_from_strlike(v: impl AsRef<[u8]>) -> Result<PartialHash, Error> {
         let b64 = v.as_ref();
         if b64.len() < 4 || b64.len() > B64_HASH_LENGTH {
             return Err(Error::MaxLengthError);
         }
         let mut b = [b'A'; B64_HASH_LENGTH];
         b[..b64.len()].copy_from_slice(b64);
-        // TODO , just  check character table ( hidden by b64 crate  -.-')
-        base64_crate::decode_config(&b[0..b64.len() & !3usize], base64_crate::URL_SAFE_NO_PAD)?;
+        // TODO , just  check character table 
+        BASE64_URL_SAFE_NO_PAD.decode(&b[0..b64.len() & !3usize])?;
         let mut arr = ArrayString::from_byte_string(&b).unwrap();
         arr.truncate(b64.len());
         Ok(PartialHash(arr))
     }
 }
 impl From<LkHash> for PartialHash {
     fn from(hash: LkHash) -> Self {
```

### Comparing `linkspace-0.1.4/local_dependencies/linkspace-core/src/predicate/bitset_test.rs` & `linkspace-0.3.0rc2/local_dependencies/linkspace-core/src/predicate/bitset_test.rs`

 * *Files identical despite different names*

### Comparing `linkspace-0.1.4/local_dependencies/linkspace-core/src/predicate/builder.rs` & `linkspace-0.3.0rc2/local_dependencies/linkspace-core/src/predicate/builder.rs`

 * *Files 1% similar despite different names*

```diff
@@ -28,23 +28,23 @@
     pub fn path(mut self, path: impl AsRef<SPath>) -> anyhow::Result<Self> {
         self.prefix(path)?;
         self.path_len.try_add(TestOp::Equal, *self.path_prefix.path_len())?;
         Ok(self)
     }
     pub fn prefix(&mut self, prefix: impl AsRef<SPath>) -> anyhow::Result<()> {
         let sp = prefix.as_ref();
-        if self.path_prefix.starts_with(&sp) {
+        if self.path_prefix.starts_with(sp) {
             tracing::trace!(old=%self.path_prefix,new=%sp,"Current prefix already more specific")
         } else if sp.starts_with(&self.path_prefix) {
             let sp = sp.try_ipath()?;
             tracing::trace!(old=%self.path_prefix,new=%sp,new_len=sp.path_len(),"Setting more specific prefix");
             self.path_prefix = sp;
             self.path_check()?;
         } else {
-            anyhow::bail!("disjoin spath {:?} <> {:?}", &*sp, &*self.path_prefix);
+            anyhow::bail!("disjoin spath {:?} <> {:?}", sp, &*self.path_prefix);
         };
         Ok(())
     }
     pub fn group(mut self, g: GroupID) -> anyhow::Result<Self> {
         self.group.try_add(TestOp::Equal, g.into())?;
         Ok(self)
     }
```

### Comparing `linkspace-0.1.4/local_dependencies/linkspace-core/src/predicate/exprs.rs` & `linkspace-0.3.0rc2/local_dependencies/linkspace-core/src/predicate/exprs.rs`

 * *Files 0% similar despite different names*

```diff
@@ -219,15 +219,15 @@
 use crate::predicate::TestOp;
 use crate::prelude::predicate_type::PredicateType;
 
 #[derive(Debug, Copy, Clone, Eq, PartialEq, Display, FromStr)]
 pub enum QScope {
     #[display("i_branch")]
     Branch,
-    #[display("i_index")]
+    #[display("i_db")]
     Index,
     #[display("i_new")]
     New,
     #[display("i")]
     Query,
 }
 pub const QSCOPES: [QScope; 4] = [QScope::Query, QScope::New, QScope::Index, QScope::Branch];
```

### Comparing `linkspace-0.1.4/local_dependencies/linkspace-core/src/predicate/pkt_predicates.rs` & `linkspace-0.3.0rc2/local_dependencies/linkspace-core/src/predicate/pkt_predicates.rs`

 * *Files 3% similar despite different names*

```diff
@@ -21,22 +21,22 @@
 
 #[derive(Debug, Clone, PartialEq)]
 pub struct PktPredicates {
     pub pkt_types: TestSet<u8>,
 
     pub var_flags: TestSet<u8>,
     pub var_hop: TestSet<u32>,
-    pub var_until: TestSet<u64>,
+    pub var_stamp: TestSet<u64>,
     pub var_ubits: [TestSet<u32>; 4],
 
     pub domain: TestSet<u128>,
     pub group: TestSet<U256>,
     pub pubkey: TestSet<U256>,
     pub hash: TestSet<U256>,
-    pub pkt_size: TestSet<u16>,
+    pub size: TestSet<u16>,
 
     pub data_size: TestSet<u16>,
     pub links_len: TestSet<u16>,
     pub path_len: TestSet<u8>,
     pub create: TestSet<u64>,
 
     pub recv_stamp: Bound<u64>,
@@ -45,36 +45,36 @@
 
     pub path_prefix: IPathBuf,
 }
 
 #[derive(Debug, Clone, PartialEq, Copy)]
 pub struct StatePredicates {
     pub i_branch: TestSet<u32>,
-    pub i_index: TestSet<u32>,
+    pub i_db: TestSet<u32>,
     pub i_new: TestSet<u32>,
     pub i_query: TestSet<u32>,
 }
 impl StatePredicates {
     pub fn check_db(&self) -> bool {
-        self.i_branch.has_any() && self.i_index.has_any()
+        self.i_branch.has_any() && self.i_db.has_any()
     }
 
     pub fn idx(&mut self, i: QScope) -> &mut TestSet<u32> {
         match i {
             QScope::Branch => &mut self.i_branch,
-            QScope::Index => &mut self.i_index,
+            QScope::Index => &mut self.i_db,
             QScope::New => &mut self.i_new,
             QScope::Query => &mut self.i_query,
         }
     }
     pub fn is_valid(&self) -> anyhow::Result<()> {
         if !self.i_query.has_any() {
             anyhow::bail!("maximum number of results is 0")
         }
-        if !self.i_new.has_any() && (!self.i_index.has_any() || !self.i_branch.has_any()) {
+        if !self.i_new.has_any() && (!self.i_db.has_any() || !self.i_branch.has_any()) {
             anyhow::bail!("both new and log have no accept conditions");
         }
         Ok(())
     }
 }
 
 impl Default for PktPredicates {
@@ -84,29 +84,29 @@
 }
 impl PktPredicates {
     pub const DEFAULT: PktPredicates = PktPredicates {
         pkt_types: TestSet::DEFAULT,
         path_prefix: IPathBuf::DEFAULT,
         var_flags: TestSet::DEFAULT,
         var_hop: TestSet::DEFAULT,
-        var_until: TestSet::DEFAULT,
+        var_stamp: TestSet::DEFAULT,
         var_ubits: [TestSet::DEFAULT; 4],
         domain: TestSet::DEFAULT,
         group: TestSet::DEFAULT,
         pubkey: TestSet::DEFAULT,
         hash: TestSet::DEFAULT,
-        pkt_size: TestSet::DEFAULT,
+        size: TestSet::DEFAULT,
         data_size: TestSet::DEFAULT,
         links_len: TestSet::DEFAULT,
         path_len: TestSet::DEFAULT,
         create: TestSet::DEFAULT,
         recv_stamp: Bound::DEFAULT,
         state: StatePredicates {
             i_branch: TestSet::DEFAULT,
-            i_index: TestSet::DEFAULT,
+            i_db: TestSet::DEFAULT,
             i_new: TestSet::DEFAULT,
             i_query: TestSet::DEFAULT,
         },
     };
 }
 impl std::fmt::Display for PktPredicates {
     fn fmt(&self, f: &mut std::fmt::Formatter<'_>) -> std::fmt::Result {
@@ -154,39 +154,39 @@
     pub fn iter(&self) -> impl Iterator<Item = Predicate> + '_ {
         let PktPredicates {
             pkt_types,
             domain,
             group,
             pubkey,
             hash,
-            pkt_size,
+            size,
             path_prefix,
             path_len,
             recv_stamp,
             create,
             state,
             data_size,
             links_len,
             var_flags,
             var_hop,
-            var_until,
+            var_stamp,
             var_ubits,
         } = self;
         use FieldEnum::*;
         let mut c = *state;
         let limits = crate::predicate::exprs::QSCOPES
             .into_iter()
             .flat_map(move |i| as_rules_it2(i, c.idx(i).rules(), U32::new));
         fn id<I>(i: I) -> I {
             i
         }
         as_rules_it2(PktTypeF, pkt_types.rules(), U8::new)
             .chain(as_rules_it2(VarNetFlagsF, var_flags.rules(), U8::new))
             .chain(as_rules_it2(VarHopF, var_hop.rules(), U32::new))
-            .chain(as_rules_it2(VarStampF, var_until.rules(), Stamp::new))
+            .chain(as_rules_it2(VarStampF, var_stamp.rules(), Stamp::new))
             .chain(as_rules_it2(VarUBits0F, var_ubits[0].rules(), U32::new))
             .chain(as_rules_it2(VarUBits1F, var_ubits[1].rules(), U32::new))
             .chain(as_rules_it2(VarUBits2F, var_ubits[2].rules(), U32::new))
             .chain(as_rules_it2(VarUBits3F, var_ubits[3].rules(), U32::new))
             .chain(as_rules_it2(DomainF, domain.map(Domain::from).rules(), id))
             .chain(as_rules_it2(
                 GroupIDF,
@@ -202,15 +202,15 @@
                 Predicate::from(RuleType::PrefixPath, TestOp::Equal, path_prefix.ablist())
             }))
             .chain(as_rules_it2(
                 PktHashF,
                 hash.map(|v| -> LkHash { v.into() }).rules(),
                 id,
             ))
-            .chain(as_rules_it2(PointSizeF, pkt_size.rules(), U16::new))
+            .chain(as_rules_it2(SizeF, size.rules(), U16::new))
             .chain(as_rules_it2(DataSizeF, data_size.rules(), U16::new))
             .chain(as_rules_it2(LinksLenF, links_len.rules(), U16::new))
             .chain(as_rules_it2(PathLenF, path_len.rules(), U8::new))
             .chain(as_rules_it2(
                 RuleType::RecvStamp,
                 recv_stamp.iter(),
                 Stamp::new,
@@ -243,21 +243,21 @@
         match kind {
             RuleType::Field(f) => {
                 self.pkt_types
                     .try_add(TestOp::Mask1, f.info().pkts.bits())
                     .with_context(|| format!("incompatible pkt typs:{rule:?}" ))?;
                 match f {
                     FieldEnum::PktTypeF => self.pkt_types.try_add(op, U8::try_from(val)?.0)?,
-                    FieldEnum::PointSizeF => {
-                        self.pkt_size.try_add(op, U16::try_from(val)?.get())?
+                    FieldEnum::SizeF => {
+                        self.size.try_add(op, U16::try_from(val)?.get())?
                     }
                     FieldEnum::PktHashF => {
                         self.hash.try_add(op, LkHash::try_from(val)?.into())?;
                         if op == TestOp::Equal {
-                            self.state.i_query.try_add(TestOp::Equal, 0u32.into())?;
+                            self.state.i_query.try_add(TestOp::Equal, 0u32)?;
                         }
                     },
                     FieldEnum::DomainF => self
                         .domain
                         .try_add(op, Domain::try_from(val)?.uint().get())?,
                     FieldEnum::PathF => {
                         ensure!(op == TestOp::Equal, "path only supports equallity");
@@ -282,15 +282,15 @@
                         self.pubkey.try_add(op, PubKey::try_from(val)?.into())?;
                     }
                     FieldEnum::SignatureF => todo!(),
                     FieldEnum::DataF => todo!(),
                     FieldEnum::VarNetFlagsF => self.var_flags.try_add(op, U8::try_from(val)?.0)?,
                     FieldEnum::VarHopF => self.var_hop.try_add(op, U32::try_from(val)?.get())?,
                     FieldEnum::VarStampF => {
-                        self.var_until.try_add(op, U64::try_from(val)?.get())?
+                        self.var_stamp.try_add(op, U64::try_from(val)?.get())?
                     }
                     FieldEnum::VarUBits0F => {
                         self.var_ubits[0].try_add(op, U32::try_from(val)?.get())?
                     }
                     FieldEnum::VarUBits1F => {
                         self.var_ubits[1].try_add(op, U32::try_from(val)?.get())?
                     }
```

### Comparing `linkspace-0.1.4/local_dependencies/linkspace-core/src/predicate/predicate_type.rs` & `linkspace-0.3.0rc2/local_dependencies/linkspace-core/src/predicate/predicate_type.rs`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+use anyhow::Context;
 // Copyright Anton Sol
 //
 // This Source Code Form is subject to the terms of the Mozilla Public
 // License, v. 2.0. If a copy of the MPL was not distributed with this
 // file, You can obtain one at https://mozilla.org/MPL/2.0/.
 // The relation between this and the 'RuleType' type is currently very hacky.
 use linkspace_pkt::PointTypeFlags;
@@ -27,17 +28,22 @@
                 #[doc=concat!(" e.g. " ,$example, " ( implies ",stringify!($ptype),")")]
                 $(#[$outer:meta])*
                 $fname
             ),*
         }
         impl PredicateType{
             pub const ALL : [PredicateType;24] = [$(PredicateType::$fname),*];
+
             pub fn try_from_id(id:&[u8]) -> Option<Self> {
-                $( if id == $name.as_bytes() { return Some(PredicateType::$fname);})*
-                    None
+                #![allow(non_upper_case_globals)]
+                $(const $fname: &'static [u8] = $name.as_bytes();)*
+                    match id {
+                        $( $fname => Some(PredicateType::$fname), )*
+                            _ => None
+                    }
             }
             pub const fn info(self) -> PredInfo{
                 match self {
                 $(PredicateType::$fname =>
                         PredInfo{
                             implies: PointTypeFlags::$ptype,
                             name:$name,
@@ -52,40 +58,48 @@
                 match self {
                     $(PredicateType::$fname => f.write_str($name)),*
                 }
             }
         }
     };
 }
+impl std::str::FromStr for PredicateType{
+    type Err = anyhow::Error;
+
+    fn from_str(s: &str) -> Result<Self, Self::Err> {
+        Self::try_from_id(s.as_bytes()).context("unknown predicate")
+    }
+}
+
 
 predty!( enum PredicateType {
     Hash => ("hash",DATA,r"\[b:AAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAA\]","the point hash"),
     Group => ("group",LINK,r"\[#:pub\]","group id"),
     Domain => ("domain",LINK,r"\[a:example\]","domain - if fewer than 16 bytes, prepadded with \0"),
     Prefix => ("prefix",LINK,r"/hello/world","path prefix - only accepts '=' op"),
     Path => ("path",LINK,r"/hello/world","exact path - only accepts '=' op"),
     Pubkey => ("pubkey",SIGNATURE,r"\[@:me:local\]","public key used to sign point"),
     Create => ("create",LINK,r"\[now:-1H\]","the create stamp"),
     PathLen => ("path_len",LINK,r"\[u8:0\]","the total number of path components - max 8"),
     LinksLen => ("links_len",LINK,r"\[u16:0\]","the number of links in a packet"),
     DataSize => ("data_size",LINK,r"\[u16:0\]","the byte size of the data field"),
     Recv => ("recv",DATA,r"\[now:+1D\]","the recv time of a packet"),
     IBranch => ("i_branch",LINK,r"\[u32:0\]","total packets per uniq (group,domain,path,key) - only applicable during local tree index, ignored otherwise"),
-    IIndex  => ("i_index",EMPTY,r"\[u32:0\]","total packets read from local index"),
+    IDb  => ("i_db",EMPTY,r"\[u32:0\]","total packets read from local instance"),
     INew  => ("i_new",EMPTY,r"\[u32:0\]","total newly received packets"),
     I => ("i",EMPTY,r"\[u32:0\]","total matched packets"),
     Hop => ("hop",EMPTY,r"\[u16:5\]","(mutable) number of hops"),
     Stamp => ("stamp",EMPTY,r"\[now\]","(mutable) variable stamp"),
     Ubits0 => ("ubits0",EMPTY,r"\[u32:0\]","(mutable) user defined bits"),
     Ubits1 => ("ubits1",EMPTY,r"\[u32:0\]","(mutable) user defined bits"),
     Ubits2 => ("ubits2",EMPTY,r"\[u32:0\]","(mutable) user defined bits"),
     Ubits3 => ("ubits3",EMPTY,r"\[u32:0\]","(mutable) user defined bits"),
     Type => ("type",EMPTY,r"\[b2:00000001\]","the field type bits - implied by other predicates"),
     Netflags => ("netflags",EMPTY,r"\[b2:00000000\]","(mutable) netflags"),
-    PointSize => ("point_size",DATA,r"\[u16:4\]","exact point size - (netpkt_size - 32b header - 32b hash)")
+    Size => ("size",DATA,r"\[u16:4\]","exact size of the netpkt when using lk_write or lk_read - includes netheader and hash ")
 });
 impl From<PredicateType> for RuleType {
     fn from(val: PredicateType) -> Self {
         val.to_string().parse().unwrap()
     }
 }
```

### Comparing `linkspace-0.1.4/local_dependencies/linkspace-core/src/predicate/test_pkt.rs` & `linkspace-0.3.0rc2/local_dependencies/linkspace-core/src/predicate/test_pkt.rs`

 * *Files 5% similar despite different names*

```diff
@@ -60,15 +60,15 @@
 }
 
 #[derive(Debug)]
 pub struct SPathPrefix(SPathBuf);
 impl PktStreamTest for SPathPrefix {
     fn test(&self, pkt: &NetPktPtr) -> bool {
         // FIXME: impl ipath starts_with and replace this
-        pkt.spath().map(|p| p.starts_with(&self.0)).unwrap_or(false)
+        pkt.path().map(|p| p.starts_with(&self.0)).unwrap_or(false)
     }
     fn get_field(&self) -> RuleType {
         RuleType::PrefixPath
     }
 
     fn as_rules(&self) -> Box<(dyn Iterator<Item = Predicate> + 'static)> {
         Box::new(std::iter::once(Predicate::from(
@@ -106,42 +106,42 @@
 ) {
     let PktPredicates {
         pkt_types,
         domain,
         group,
         pubkey,
         hash,
-        pkt_size,
+        size,
         path_prefix,
         path_len,
         create,
         links_len,
         data_size,
         recv_stamp,
         state: _,
         var_flags,
         var_hop,
-        var_until,
+        var_stamp,
         var_ubits,
     } = r;
 
     let it = into_tests::<PktTypeF, _>(pkt_types)
         .chain(into_tests::<VarNetFlagsF, _>(var_flags))
         .chain(into_tests::<VarHopF, _>(var_hop))
-        .chain(into_tests::<VarStampF, _>(var_until))
+        .chain(into_tests::<VarStampF, _>(var_stamp))
         .chain(into_tests::<VarUBits0F, _>(&var_ubits[0]))
         .chain(into_tests::<VarUBits1F, _>(&var_ubits[1]))
         .chain(into_tests::<VarUBits2F, _>(&var_ubits[2]))
         .chain(into_tests::<VarUBits3F, _>(&var_ubits[3]))
         .chain(into_tests::<PktHashF, _>(hash))
         .chain(into_tests::<GroupIDF, _>(group))
         .chain(into_tests::<PubKeyF, _>(pubkey))
         .chain(into_tests::<DomainF, _>(domain))
         .chain(into_tests::<CreateF, _>(create))
-        .chain(into_tests::<PointSizeF, _>(pkt_size))
+        .chain(into_tests::<SizeF, _>(size))
         .chain(into_tests::<DataSizeF, _>(data_size))
         .chain(into_tests::<LinksLenF, _>(links_len))
         .chain(into_tests::<PathLenF, _>(path_len))
         //.chain( into_tests::<LinksLenF,_>(&links))
         .chain(is_some(path_prefix.clone()).map(|v| {
             (
                 Box::new(SPathPrefix(v.spath().to_owned())) as Box<dyn PktStreamTest>,
```

### Comparing `linkspace-0.1.4/local_dependencies/linkspace-core/src/predicate/treekey.rs` & `linkspace-0.3.0rc2/local_dependencies/linkspace-core/src/env/lmdb/tree_iter.rs`

 * *Files 26% similar despite different names*

```diff
@@ -1,74 +1,24 @@
-// Copyright Anton Sol
-//
-// This Source Code Form is subject to the terms of the Mozilla Public
-// License, v. 2.0. If a copy of the MPL was not distributed with this
-// file, You can obtain one at https://mozilla.org/MPL/2.0/.
-/*
-TODO. components needs to be integrated here
-
-
-*/
-
-use anyhow::Context;
-use linkspace_pkt::*;
-
-use crate::{
-    prelude::{TreeEntryRef, TreeKey, TreeValueBytes},
-    stamp_range::{IterCmp, StampRange},
-};
-
-use super::{bitset_test::BitTestSet, TestSet, UInt};
-
-#[derive(Clone, PartialEq, Eq, Debug, Default)]
-pub struct TreeKeys {
-    pub domain: TestSet<u128>,
-    pub group: TestSet<U256>,
-    pub ipath: IPathBuf,
-    pub depth: BitTestSet,
-    pub pubkey: TestSet<U256>,
-    pub cstamp: StampRange,
-}
+use linkspace_pkt::{GroupID, Domain};
+
+use crate::{prelude::treekey::{TreeKeys }, env::tree_key::{TreeEntryRef, TreeValueBytes, TreeKey}, stamp_range::IterCmp};
+
+use super::db::IterDup;
 
-impl TreeKeys {
-    pub fn lower_bound(&self) -> anyhow::Result<Vec<u8>> {
-        let mut btree_key = vec![];
-        let (group, domain, depth, spath, pubkey) = (
-            self.group.info(UInt::MIN).val.context("Empty group set")?,
-            self.domain
-                .info(UInt::MIN)
-                .val
-                .context("Empty domain set")?,
-            self.depth.info(0).val.context("Empty depthset")?,
-            &self.ipath,
-            self.pubkey
-                .info(UInt::MIN)
-                .val
-                .context("Empty pubkey set")?,
-        );
-        tracing::trace!(?group,?domain,?depth,%spath,?pubkey, "lowerbounds");
-        btree_key.extend_from_slice(&group.to_be_bytes::<32>());
-        btree_key.extend_from_slice(&Domain::from(domain).0);
-        btree_key.push(depth);
-        btree_key.extend(spath.spath_bytes());
-        btree_key.extend_from_slice(&pubkey.to_be_bytes::<32>());
-        Ok(btree_key)
-    }
-}
 
-use crate::env::db::IterDup;
 #[derive(Debug)]
 pub struct TreeKeysIter<'txn> {
     pub iter_dup: IterDup<'txn>,
     pub req: TreeKeys,
     pub lower_bound: Vec<u8>,
 }
-pub fn spd<'o>(kv: (&'o [u8], &'o TreeValueBytes)) -> TreeEntryRef<'o> {
-    TreeEntryRef::from_db(kv)
-}
+
+// alias
+pub (super) fn  spd<'o>(kv: (&'o [u8], &'o TreeValueBytes)) -> TreeEntryRef<'o> {TreeEntryRef::from_db(kv) }
+
 
 impl<'txn> TreeKeysIter<'txn> {
     pub fn next_entry(&mut self) -> Option<TreeEntryRef<'txn>> {
         self.iter_dup
             .get_next_entry()
             .map(spd)
             .filter(|v| self.req.cstamp.contains(v.create()))
```

### Comparing `linkspace-0.1.4/local_dependencies/linkspace-core/src/predicate/uint.rs` & `linkspace-0.3.0rc2/local_dependencies/linkspace-core/src/predicate/uint.rs`

 * *Files 3% similar despite different names*

```diff
@@ -197,19 +197,19 @@
     const MIN: Self = B64([0; 32]);
     const MAX: Self = B64([255; 32]);
     const ONE: Self = B64(u8_be::one());
     const BITS: u32 = 32 * 8;
 
     #[inline(always)]
     fn bit_and(self, other: Self) -> Self {
-        B64(self.0.zip(other.0).map(|(a, b)| a & b))
+        B64(std::array::from_fn(|i| self.0[i] & other.0[i]))
     }
     #[inline(always)]
     fn bit_or(self, other: Self) -> Self {
-        B64(self.0.zip(other.0).map(|(a, b)| a | b))
+        B64(std::array::from_fn(|i| self.0[i] | other.0[i]))
     }
     #[inline(always)]
     fn not(self) -> Self {
         B64(self.0.map(|i| !i))
     }
     fn inc(self) -> Option<Self> {
         u8_be::add(self.0, u8_be::one()).map(B64)
@@ -270,19 +270,19 @@
     const BITS: u32 = 16 * 8;
     fn as_be_bytes(&self, out: &mut dyn FnMut(&[u8])) {
         out(&self.0)
     }
   
     #[inline(always)]
     fn bit_and(self, other: Self) -> Self {
-        AB(self.0.zip(other.0).map(|(a, b)| a & b))
+        AB(std::array::from_fn(|i| self.0[i] & other.0[i]))
     }
     #[inline(always)]
     fn bit_or(self, other: Self) -> Self {
-        AB(self.0.zip(other.0).map(|(a, b)| a | b))
+        AB(std::array::from_fn(|i| self.0[i] | other.0[i]))
     }
     #[inline(always)]
     fn not(self) -> Self {
         AB(self.0.map(|i| !i))
     }
     fn inc(self) -> Option<Self> {
         u8_be::add(self.0, u8_be::one()).map(AB)
```

### Comparing `linkspace-0.1.4/local_dependencies/linkspace-core/src/predicate/value_test.rs` & `linkspace-0.3.0rc2/local_dependencies/linkspace-core/src/predicate/value_test.rs`

 * *Files 1% similar despite different names*

```diff
@@ -196,14 +196,19 @@
 
 /// the set of numbers between bound.greater_eq <= number <= bound.less_eq
 #[derive(Copy, Clone, Eq, PartialEq, Debug)]
 pub struct Bound<U> {
     pub low: U,
     pub high: U,
 }
+impl<U:UInt> Default for Bound<U>{
+    fn default() -> Self {
+        Self::DEFAULT
+    }
+}
 impl<U: UInt> Bound<U> {
     pub const DEFAULT: Self = Bound {
         high: U::MAX,
         low: U::MIN,
     };
     pub const EMPTY: Self = Bound {
         high: U::MIN,
@@ -369,26 +374,25 @@
             .bit_or(freemask.overflowing_shr(1).0)
             .overflowing_add(U::ONE);
         let fix_mask = U::MAX.overflowing_shl(pivot).0.not();
         let v = incval.bit_and(fix_mask.not()).bit_or(min.bit_and(fix_mask));
         (over, v)
     }
 }
+#[ignore]
 #[test]
-fn test_inset() {
-    #![allow(unreachable_code)]
-    return;
+fn _disabled_test_inset() {
     for zeros in 0..=255 {
         for ones in 0..=255 {
             for val in 0..=255 {
                 let mask = Mask { zeros, ones };
                 if !mask.has_any() {
                     continue;
                 };
-                let iter_find = (val..=u8::MAX).filter(|v| mask.test(v)).next();
+                let iter_find = (val..=u8::MAX).find(|v| mask.test(v));
                 assert_eq!(mask.in_set(val), iter_find)
             }
         }
     }
 }
 
 /// Tests to test a value. To pass the test value must have 1's for all 1's in ones, and all 0's for all 0's in zeros!!
@@ -499,14 +503,15 @@
             mask: Mask::<U>::DEFAULT,
         }
     };
 
     #[inline]
     /// Warning - This is only valid if TestSet.has_any;
     pub fn info(&self, val: U) -> SetValueInfo<U> {
+        debug_assert!(self.has_any());
         let cmp = self.bound.bound_cmp(val);
         match cmp {
             std::cmp::Ordering::Less => SetValueInfo {
                 in_set: false,
                 val: self.mask.in_set(self.bound.low),
             },
             std::cmp::Ordering::Equal => match self.mask.in_set(val) {
```

### Comparing `linkspace-0.1.4/local_dependencies/linkspace-core/src/prelude.rs` & `linkspace-0.3.0rc2/local_dependencies/linkspace-core/src/prelude.rs`

 * *Files 11% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 // file, You can obtain one at https://mozilla.org/MPL/2.0/.
 pub use std::ops::ControlFlow::*;
 pub use std::sync::Arc;
 
 pub use linkspace_pkt::{*,eval,exprs,Error};
 
 pub use crate::consts::*;
-pub use crate::env::queries::*;
+pub use crate::env::lmdb::queries::*;
 pub use crate::env::tree_key::*;
 pub use crate::env::write_result::*;
 pub use crate::env::write_trait::*;
 pub use crate::env::*;
 pub use crate::eval::*;
 pub use crate::matcher::*;
 pub use crate::partial_hash::PartialHash;
```

### Comparing `linkspace-0.1.4/local_dependencies/linkspace-core/src/pull.rs` & `linkspace-0.3.0rc2/local_dependencies/linkspace-core/src/pull.rs`

 * *Files 12% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     reader: &ReadTxn,
     ctx: EvalCtx<&dyn Scope>,
 ) -> anyhow::Result<()> {
     if !pkt.is_datapoint(){
         let stamp = pkt.create_stamp().copied();
         let subc= ctx.pre_scope(EScope(StampEF{fixed_now:stamp}));
         let subc= pkt_ctx(subc.reref(), &pkt);
-        tracing::debug!(ctx=pkt_fmt(pkt), "set pkt ctx");
+        tracing::debug!(ctx=%PktFmt(pkt), "set pkt ctx");
         
         for l in pkt.get_links() {
             let inner = reader
                 .read(&l.ptr)?
                 .context("Missing pointer")?;
             read_pull_pkt(query, &inner, reader, subc.dynr())?;
         }
```

### Comparing `linkspace-0.1.4/local_dependencies/linkspace-core/src/query.rs` & `linkspace-0.3.0rc2/local_dependencies/linkspace-core/src/query.rs`

 * *Files 4% similar despite different names*

```diff
@@ -53,33 +53,37 @@
 }
 
 #[derive(Copy, Clone, parse_display::Display, parse_display::FromStr)]
 #[display(style = "kebab-case")]
 pub enum KnownOptions {
     /// which index to walk when reading from the database
     Mode,
-    /// The arg is the ID under which to operate. Can be overwritten or closed. Is required for lk_watch but not for lk_get*.
-    Id,
+    /// The arg is the query id under which to operate. Can be overwritten or closed. Is required for lk_watch but not for lk_get*.
+    Qid,
     /// try and also return the linked packets.
     Follow,
     /// (not supported by lk_watch) - append the request on finish - ignores the first callback Break to deliver the request on dropping
     NotifyClose,
 }
 impl KnownOptions {
     //todo make static
     pub fn as_bytes(self) -> Vec<u8>{
         self.to_string().into_bytes()
     }
     pub fn iter_all() -> impl Iterator<Item = Self> {
         use KnownOptions::*;
-        [Mode, Id, Follow, NotifyClose ].into_iter()
+        [Mode, Qid, Follow, NotifyClose ].into_iter()
     }
 }
 
 impl Query {
+    pub const DEFAULT : Self = Query{
+        predicates: PktPredicates::DEFAULT,
+        options: vec![],
+    };
     pub fn to_str(&self, canonical: bool) -> String {
         use std::fmt::Write;
         let mut out = String::new();
         for opt in &self.options {
             writeln!(out, "{opt}").unwrap();
         }
         for p in self.predicates.iter() {
@@ -120,16 +124,16 @@
             ensure!(
                 abl.lst.len() < 4 && abl.lst[1].1 != Some(Ctr::FSlash),
                 "Bad options argument expected at most 1 arg, got {abl}"
             );
             Ok(abl.lst.get(2).map(|v| v.0.as_slice()).unwrap_or(&[]))
         })
     }
-    pub fn id(&self) -> Option<anyhow::Result<&[u8]>> {
-        self.get_option_bytes(KnownOptions::Id.to_string().as_bytes())
+    pub fn qid(&self) -> Option<anyhow::Result<&[u8]>> {
+        self.get_option_bytes(KnownOptions::Qid.to_string().as_bytes())
     }
     pub fn mode(&self) -> Option<anyhow::Result<Mode>> {
         self.get_option_bytes(KnownOptions::Mode.to_string().as_bytes())
             .map(|r| r.and_then(|b| Ok(std::str::from_utf8(b)?.parse()?)))
     }
     pub fn get_mode(&self) -> anyhow::Result<Mode> {
         Ok(self.mode().transpose()?.unwrap_or(Mode::TREE_DESC))
@@ -149,15 +153,15 @@
         }
         Ok(())
     }
 
     pub fn hash_eq(h: linkspace_pkt::LkHash) -> Self {
         let mut predicates = PktPredicates::default();
         predicates.hash.add(TestOp::Equal, h.into());
-        predicates.state.i_query.add(TestOp::Equal,0u32.into());
+        predicates.state.i_query.add(TestOp::Equal,0u32);
         let mut q= Query {
             predicates,
             options: Default::default()
         };
         q.add_option(&KnownOptions::Mode.to_string(), &[Mode::HASH_ASC.to_string().as_bytes()]);
         q
     }
```

### Comparing `linkspace-0.1.4/local_dependencies/linkspace-core/src/stamp_fmt.rs` & `linkspace-0.3.0rc2/local_dependencies/linkspace-core/src/stamp_fmt.rs`

 * *Files 1% similar despite different names*

```diff
@@ -270,19 +270,19 @@
                     let st: String = dt
                         .ok()
                         .and_then(|dt| dt.format(&default).ok())
                         .unwrap_or_else(|| delta_stamp_p(Stamp::ZERO,stamp,9,9));
                     result = Some(st.into_bytes());
                     break;
                 }
-                e => return Err(anyhow!("unknown args '{}'", clist(e)).into()),
+                e => return Err(anyhow!("unknown args '{}'", clist(e))),
             };
         }
         if !args.is_empty() {
-            return Err(anyhow!("bad trailing args '{}'", clist(args)).into());
+            return Err(anyhow!("bad trailing args '{}'", clist(args)));
         }
         Ok(result.unwrap_or_else(|| stamp.0.to_vec()))
     }
 }
 
 impl EvalScopeImpl for StampEF {
     fn about(&self) -> (String, String) {
```

### Comparing `linkspace-0.1.4/local_dependencies/linkspace-core/src/stamp_range.rs` & `linkspace-0.3.0rc2/local_dependencies/linkspace-core/src/stamp_range.rs`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 // Copyright Anton Sol
 //
 // This Source Code Form is subject to the terms of the Mozilla Public
 // License, v. 2.0. If a copy of the MPL was not distributed with this
 // file, You can obtain one at https://mozilla.org/MPL/2.0/.
 use core::fmt;
-use std::{cmp::Ordering, ops::RangeInclusive, str::FromStr};
+use std::{cmp::Ordering, ops::RangeInclusive, str::FromStr, hint::unreachable_unchecked};
 
 use linkspace_pkt::Stamp;
 
 use crate::stamp_fmt::stamp_from_str;
 
 /// By default runs from MAX value to 0 ( new to old )
 #[derive(Debug, Clone, Eq, PartialEq, Copy, Hash)]
@@ -76,15 +76,15 @@
         let end = self.end.cmp(&i) as i8;
         let i = if start == end { start } else { 0 };
         let dir = self.start.cmp(&self.end) as i8;
         let r = match (dir, i) {
             (0, v) => -v,
             (a, b) => a * b,
         };
-        unsafe { std::mem::transmute(r) }
+        IterCmp::unchecked_from(r)
     }
     pub fn lower_bound(&self) -> Stamp {
         Stamp::new(self.start.min(self.end))
     }
 
     pub fn upper_bound(&self) -> Stamp {
         Stamp::new(self.start.max(self.end))
@@ -136,14 +136,24 @@
 #[derive(Clone, Copy, PartialEq, Eq, Debug)]
 #[repr(i8)]
 pub enum IterCmp {
     Pre = -1,
     In = 0,
     Post = 1,
 }
+impl IterCmp {
+    pub fn unchecked_from(i:i8) -> Self {
+        match i {
+            -1 => IterCmp::Pre,
+            0 => IterCmp::In,
+            1 => IterCmp::Post,
+            _ => unsafe{unreachable_unchecked()}
+        }
+    }
+}
 
 #[test]
 fn cmp() {
     use IterCmp::*;
     fn c(a: u64, b: u64, c: u64, r: IterCmp) {
         println!("Expect {:?}", r);
         assert_eq!(
```

### Comparing `linkspace-0.1.4/local_dependencies/linkspace/Cargo.toml` & `linkspace-0.3.0rc2/local_dependencies/linkspace/Cargo.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,33 @@
 [package]
 name = "linkspace"
-version = "0.1.4"
+version = "0.3.0-rc1"
 edition = "2021"
-authors = ["Azon <AntonSol919@gmail.com>"]
+authors = ["Anton Sol <AntonSol919@gmail.com>"]
 license = "MPL-2.0"
 homepage = "https://antonsol919.github.io/linkspace/"
-documentation = "https://antonsol919.github.io/linkspace/docs/guide/index.html"
+documentation = "https://www.linkspace.dev/docs/guide/index.html"
 repository = "https://github.com/AntonSol919/linkspace"
 categories = ["database","network-programming","asynchronous"]
 keywords = ["linkspace", "supernet"]
 description = "linkspace - a general purpose supernet"
+resolver = "2"
 
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 
 [features]
+default = ["full", "lmdb"]
+lmdb=["linkspace-common/lmdb"]
+full = ["linkspace-common/full"]
+
 
 [dependencies]
-anyhow = "1.0.69"
+anyhow= "=1.0.71"
 backtrace = "0.3.67"
-linkspace-common = { path = "../linkspace-common", version = "0.1.1"}
-tracing = "0.1.37"
+linkspace-common = { path = "../linkspace-common", version = "0.3.0-rc1", default-features = false}
+tracing= {version = "=0.1.37",features=["release_max_level_info"]}
+build-info= { version = "=0.0.31"}
+
+[build-dependencies]
+build-info-build= { version = "=0.0.31"}
+
```

### Comparing `linkspace-0.1.4/local_dependencies/linkspace/LICENSE` & `linkspace-0.3.0rc2/local_dependencies/linkspace-argon2-identity/LICENSE`

 * *Files identical despite different names*

### Comparing `linkspace-0.1.4/local_dependencies/linkspace/src/conventions/mod.rs` & `linkspace-0.3.0rc2/local_dependencies/linkspace/src/conventions/mod.rs`

 * *Files 0% similar despite different names*

```diff
@@ -37,21 +37,21 @@
     let domain: Domain = query
         .0
         .predicates
         .domain
         .as_eq()
         .context("requires exact domain predicate")?
         .into();
-    let id = query.0.id().transpose()?.context("missing :id option")?;
+    let id = query.0.qid().transpose()?.context("missing :qid option")?;
     let data = query.0.to_string();
     tracing::trace!(data);
-    let pull_path = ipath_buf(&[b"pull", &*group, &*domain, &id]);
+    let pull_path = ipath_buf(&[b"pull", &*group, &*domain, id]);
     let pkt = lk_linkpoint(
+        data.as_bytes(),
         EXCHANGE_DOMAIN,
         PRIVATE,
         &pull_path,
         &[],
-        data.as_bytes(),
         None,
     )?;
     Ok(pkt.as_netbox())
 }
```

### Comparing `linkspace-0.1.4/local_dependencies/linkspace/src/conventions/status.rs` & `linkspace-0.3.0rc2/local_dependencies/linkspace/src/conventions/status.rs`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-use linkspace_common::prelude::{U16, pkt_fmt, U32 };
+
+use linkspace_common::prelude::{U16, U32 };
 use tracing::debug_span;
 
 // Copyright Anton Sol
 //
 // This Source Code Form is subject to the terms of the Mozilla Public
 // License, v. 2.0. If a copy of the MPL was not distributed with this
 // file, You can obtain one at https://mozilla.org/MPL/2.0/.
@@ -18,35 +19,44 @@
 The current expected formats are:
 
 exchange GROUP process
 exchange GROUP connection PUBKEY
 exchnage GROUP pull PULL PULL_HASH
 
 A request is a packet in the form DOMAIN:[#:0]:/\fstatus/GROUP/type(/instance?) , with no data and no links.
-A reply is of the form DOMAIN:[#:0]/\status/GROUP/type/instance with some data and links.
+A reply is of the form DOMAIN:[#:0]/\status/GROUP/type/instance with some data and at least some links.
 
-A request without 'instance' is be answered by all instances.
+A request without 'instance' should be answered by all instances.
 
 The reply must have an 'instance' set. It defaults to 'default'.
 The reply data should be either "OK\n" or "ERR\n" followed by more info.
 The reply process links can start with init:[#:0] at first and should point to previous replies after that.
 
-A request is only made 'once' per timeout.
+A new request is not made if one was made after now-timeout.
 I.e. a process checks if a request was made since now-timeout, before making a new request, and returns after last_req+timeout.
+A reply is accepted if it was made now-timeout.
+
+This might change
 **/
 use crate::{*, runtime::{lk_get_all, lk_watch2}};
-pub const STATUS_PATH: IPathC<16> = ipath1(concat_bytes!([255], b"status"));
+pub const STATUS_PATH: IPathC<16> = ipath1::<7>(concat_bytes!([255], b"status"));
 
 #[derive(Copy, Clone)]
 #[repr(C)]
 pub struct LkStatus<'o> {
     pub domain: Domain,
     pub group: GroupID,
     pub objtype: &'o [u8],
     pub instance: Option<&'o [u8]>,
+    pub qid: &'o [u8]
+}
+impl Default for LkStatus<'static> {
+    fn default() -> Self {
+        Self { domain: domain(), group: group(), objtype: &[], instance: None, qid: b"status" }
+    }
 }
 impl<'o> std::fmt::Debug for LkStatus<'o>{
     fn fmt(&self, f: &mut std::fmt::Formatter<'_>) -> std::fmt::Result {
         f.debug_struct("LkStatus")
             .field("domain", &self.domain)
             .field("group", &self.group)
             .field("objtype", &AB(&self.objtype))
@@ -62,71 +72,64 @@
         path.try_append_component(v)?;
     }
     Ok(path)
 }
 
 /// A query that returns both requests and updates
 pub fn lk_status_request(status:LkStatus) -> LkResult<NetPktBox>{
-    lk_linkpoint(status.domain, PRIVATE, &lk_status_path(status)?, &[],&[], None)
+    lk_linkpoint(&[],status.domain, PRIVATE, &lk_status_path(status)?,&[], None)
 }
 
 /// A query that returns both requests and updates
 pub fn lk_status_overwatch(status:LkStatus,max_age:Stamp) -> LkResult<Query> {
     let LkStatus { domain,  ..} = status;
     let path = lk_status_path(status)?;
-    let mut q = lk_query(None);
+    let mut q = lk_query(&Q);
     let create_after = now().saturating_sub(max_age);
     q = lk_query_push(q, "group", "=", &*PRIVATE)?;
     q = lk_query_push(q, "domain", "=", &*domain)?;
     q = lk_query_push(q, "create", ">", &*create_after)?;
     q = lk_query_push(q, "prefix", "=", path.spath_bytes())?;
     Ok(q)
 }
 
-
-/// It is up to the caller to ensure 'lk_process' is called accodingly. Impl [PktHandler::stopped] to capture the timeout event.
-pub fn lk_status_poll(lk:&Linkspace,status:LkStatus, d_timeout:Stamp, mut cb: impl PktHandler + 'static,watch_id:Option<&[u8]>) -> LkResult<()>{
+pub fn lk_status_poll(lk:&Linkspace,status:LkStatus, d_timeout:Stamp, mut cb: impl PktHandler + 'static) -> LkResult<bool>{
     let span = debug_span!("status_poll",?status,?d_timeout);
     let _ = span.enter();
     let mut ok = false;
     let mut last_request = Stamp::ZERO;
     let mut query : Query= lk_status_overwatch(status, d_timeout)?;
-
+    // We want to capture any old request, so we first lk_get_all both requests and replies.
     lk_get_all(lk, &query, &mut |pkt| {
         if pkt.get_links().is_empty() && pkt.data().is_empty() {
             last_request = *pkt.get_create_stamp();
-            tracing::debug!(pkt=%pkt_fmt(&pkt),"recently requested");
-            true
+            tracing::debug!(pkt=%PktFmt(&pkt),"recently requested");
+            false
         }else {
             ok =true;
             let cnt = (cb).handle_pkt(pkt,lk);
             tracing::debug!("recently replied");
-            cnt.is_continue()
+            cnt.is_break()
         }
     })?;
     if last_request == Stamp::ZERO{
         tracing::debug!("creating new req");
         let req = lk_status_request(status).unwrap();
         last_request = *req.get_create_stamp();
         lk_save(lk,&req)?;
     }
     let wait_until = last_request.saturating_add(d_timeout);
     tracing::debug!(?wait_until,"Waiting until");
     query = lk_query_push(query, "data_size", ">", &*U16::ZERO)?;
     query = lk_query_push(query, "links_len", ">", &*U16::ZERO)?;
     query = lk_query_push(query, "recv", "<", &*wait_until)?;
-    query = match watch_id{
-        Some(id) => lk_query_push(query, "", "id", id)?,
-        None => {
-            let id = [b"status" as &[u8],&*now()].concat(); 
-            lk_query_push(query, "", "id", &id)?
-        },
-    };
+    query = lk_query_push(query, "i_db", "<", &*U32::ZERO)?;
+    query = lk_query_push(query, "", "qid", status.qid)?;
     lk_watch2(lk, &query, cb,span)?;
-    Ok(())
+    Ok(ok)
 }
 
 fn is_status_reply(status:LkStatus,path:&IPath,pkt:&NetPktPtr) -> LkResult<()>{
     anyhow::ensure!(*pkt.get_domain() == status.domain
                     && *pkt.get_group() == PRIVATE
                     && pkt.get_ipath() == path
                     && !pkt.get_links().is_empty()
@@ -135,45 +138,55 @@
     Ok(())
 }
 
 /// Insert a callback that is triggered on a request. Must yield a valid response. Don't forget to process
 pub fn lk_status_set(lk:&Linkspace,status:LkStatus,mut update:impl FnMut(&Linkspace,Domain,GroupID,&IPath,Link) -> LkResult<NetPktBox> +'static)-> LkResult<()>{
     let span = debug_span!("status_set",?status);
     let _ = span.enter();
-    let LkStatus { domain, group, objtype, instance }= status;
+    let LkStatus { domain, group, objtype, instance,qid }= status;
 
     let objtype = objtype.to_vec();
     let instance = instance.or(Some(b"default")).map(Vec::from);
-    let status = LkStatus { instance: instance.as_deref(), domain , group, objtype:&objtype};
+    let status = LkStatus { instance: instance.as_deref(), domain , group, objtype:&objtype, qid};
     let path = lk_status_path(status)?;
     let link = Link{tag:ab(b"init"),ptr:PRIVATE};
     let initpkt = update(lk,status.domain, PRIVATE, &path,link)?;
     is_status_reply(status, &path, &initpkt)?;
     let mut prev = initpkt.hash();
     tracing::debug!(?initpkt,"init status");
-    lk_save(&lk,&initpkt )?;
+    lk_save(lk,&initpkt )?;
     std::mem::drop(initpkt);
 
-    let mut q = lk_query(None);
+    let mut q = lk_query(&Q);
     let prefix = lk_status_path(LkStatus { instance:None, ..status})?;
     q = lk_query_push(q, "data_size", "=", &*U16::ZERO)?;
     q = lk_query_push(q, "links_len", "=", &*U16::ZERO)?;
     q = lk_query_push(q, "prefix", "=", prefix.spath_bytes())?;
     // We only care about new packets. Worst case a request was received and timeout between our init and this cb.
-    q = lk_query_push(q, "i_index", "<", &*U32::ZERO)?;
-    q = lk_query_push(q, "", "id", &[b"status-update" as &[u8],&*now()].concat())?;
-    lk_watch2(&lk, &q, cb(move |pkt:&dyn NetPkt, lk:&Linkspace| -> LkResult<()>{
-        let status = LkStatus { instance: instance.as_deref(), domain , group, objtype:&objtype};
+    q = lk_query_push(q, "i_db", "<", &*U32::ZERO)?;
+    q = lk_query_push(q, "", "qid", qid)?;
+    lk_watch2(lk, &q, try_cb(move |pkt:&dyn NetPkt, lk:&Linkspace| -> LkResult<()>{
+        let status = LkStatus { instance: instance.as_deref(), domain , group, objtype:&objtype,qid:&[]};
         let p = pkt.get_ipath();
         if p.len() == path.len() && p.spath() != path.as_ref() { return Ok(())}
         let link = Link{tag:ab(b"prev"),ptr:prev};
         let reply = update(lk,status.domain,PRIVATE,&path,link)?;
         is_status_reply(status, &path, &reply)?;
         prev  = reply.hash();
         tracing::debug!(?reply,"Reply status");
         lk_save(lk,&reply)?;
         Ok(())
     }),span)?;
     Ok(())
 }
 
 
+pub fn testu32(b:&[u32]) -> u64{
+    let a = u64::from_ne_bytes(unsafe{*b.as_ptr().cast()});
+    let b = u64::from_ne_bytes(unsafe{*b[2..].as_ptr().cast()});
+    a+b
+}
+pub fn testu8(b:&[u8]) -> u64{
+    let a = u64::from_ne_bytes(unsafe{*b.as_ptr().cast()});
+    let b = u64::from_ne_bytes(unsafe{*b[8..].as_ptr().cast()});
+    a+b
+}
```

### Comparing `linkspace-0.1.4/local_dependencies/linkspace/src/interop.rs` & `linkspace-0.3.0rc2/local_dependencies/linkspace/src/interop.rs`

 * *Files 4% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 // This Source Code Form is subject to the terms of the Mozilla Public
 // License, v. 2.0. If a copy of the MPL was not distributed with this
 // file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
 use linkspace_common::core::query::Query as QueryImpl;
 use crate::Query;
 #[doc(hidden)]
-impl Into<QueryImpl> for crate::Query {
-    fn into(self) -> QueryImpl {
-        self.0
+impl From<crate::Query> for QueryImpl {
+    fn from(val: crate::Query) -> Self {
+        val.0
     }
 }
 #[doc(hidden)]
 impl From<QueryImpl> for crate::Query {
     fn from(value: QueryImpl) -> Self {
         crate::Query(value)
     }
@@ -25,26 +25,24 @@
     }
     #[doc(hidden)]
     pub fn from_impl(q:&QueryImpl) -> &Query{
         unsafe { &*(q as *const QueryImpl as *const Query) }
     }
 }
 
-
-
 #[doc(hidden)]
 impl From<linkspace_common::runtime::Linkspace> for crate::Linkspace {
     fn from(value: linkspace_common::runtime::Linkspace) -> Self {
         crate::Linkspace(value)
     }
 }
 #[doc(hidden)]
-impl Into<linkspace_common::runtime::Linkspace> for crate::Linkspace {
-    fn into(self) -> linkspace_common::runtime::Linkspace {
-        self.0
+impl From<crate::Linkspace> for linkspace_common::runtime::Linkspace {
+    fn from(val: crate::Linkspace) -> Self {
+        val.0
     }
 }
 impl crate::Linkspace{
     #[doc(hidden)]
     pub fn as_impl(&self) -> &LinkspaceImpl{
         unsafe{&*(self as *const Linkspace as *const LinkspaceImpl)}
     }
```

### Comparing `linkspace-0.1.4/local_dependencies/linkspace/src/lib.rs` & `linkspace-0.3.0rc2/local_dependencies/linkspace/src/lib.rs`

 * *Files 7% similar despite different names*

```diff
@@ -18,31 +18,34 @@
 
 The functions re-exported below is essentially the entire linkspace interface.
 Bindings in other languages follow the same pattern.
 
 [prelude] includes some additional utilities.
 Some internals structs defs are currently leaking and will be removed.
 "#]
-use std::ops::ControlFlow;
+use std::{ops::ControlFlow};
 
-use linkspace_common::{pkt, runtime::handlers::StopReason};
+use linkspace_common::{pkt, runtime::handlers::StopReason,};
 
 pub type LkError = anyhow::Error;
 pub type LkResult<T = ()> = std::result::Result<T, LkError>;
 
 pub mod prelude {
     pub use super::*;
     pub use linkspace_common::{
         byte_fmt::{endian_types, AB, B64},
-        core::env::queries::RecvPktPtr,
+        core::env::RecvPktPtr,
+        static_env::{group,set_group,domain,set_domain},
         pkt::{
             ab, as_abtxt_c, ipath1, ipath_buf, now, spath_buf, try_ab, Domain, GroupID, IPath,
-            IPathBuf, IPathC, Link, LkHash, NetFlags, NetPkt, NetPktArc, NetPktBox, NetPktExt,
-            NetPktHeader, NetPktParts, NetPktPtr, PointTypeFlags, Point, PointExt, Ptr, PubKey,
+            IPathBuf, IPathC,PathError, Link, LkHash, NetFlags, NetPkt, NetPktArc, NetPktBox, NetPktExt,
+            NetPktHeader, NetPktParts, NetPktPtr, PointTypeFlags, Point, PointExt, PubKey,
             SPath, SPathBuf, SigningExt, SigningKey, Stamp, Tag,
+            Error as PktError,
+            repr::PktFmt
         },
     };
 }
 use prelude::*;
 
 pub use prelude::SigningKey;
 
@@ -63,15 +66,15 @@
     fn stopped(&mut self, query: Query, lk: &Linkspace, reason: StopReason, total: u32, new: u32) {
         (**self).stopped(query, lk, reason, total, new)
     }
 }
 
 pub use point::{lk_datapoint, lk_keypoint, lk_linkpoint};
 pub mod point {
-    use std::io;
+    use std::{io, borrow::Cow};
 
     use super::*;
     /**
 
     create a datapoint with upto MAX_CONTENT_SIZE bytes and wrap it as a [NetPktBox]
 
     ```
@@ -80,19 +83,19 @@
     let datap = lk_datapoint(b"Some data")?;
     assert_eq!(datap.hash().to_string(), "ay01_aEzVcp0scyCgKqfugoQSXGW4iefLgAZRxRp9sY");
     assert_eq!(datap.data() , b"Some data");
     # Ok(())}
     ```
 
     **/
-    pub fn lk_datapoint<'o>(data: &'o [u8]) -> LkResult<NetPktBox> {
+    pub fn lk_datapoint(data: &[u8]) -> LkResult<NetPktBox> {
         lk_datapoint_ref(data).map(|v| v.as_netbox())
     }
-    pub fn lk_datapoint_ref<'o>(data: &'o [u8]) -> LkResult<NetPktParts<'o>> {
-        Ok(pkt::try_datapoint_ref(data, pkt::NetOpts::Default)?.into())
+    pub fn lk_datapoint_ref(data: &[u8]) -> LkResult<NetPktParts<'_>> {
+        Ok(pkt::try_datapoint_ref(data, pkt::NetOpts::Default)?)
     }
     /**
 
     create a new linkpoint [NetPktBox]
     ```
     # use linkspace::{*,prelude::{*,endian_types::*},abe::*};
     # fn main() -> LkResult{
@@ -112,84 +115,92 @@
     assert_eq!(*linkpoint.get_group(), PUBLIC);
 
     # Ok(())}
 
     ```
     **/
     pub fn lk_linkpoint(
+        data: &[u8],
         domain: Domain,
         group: GroupID,
         path: &IPath,
         links: &[Link],
-        data: &[u8],
         create_stamp: Option<Stamp>,
     ) -> LkResult<NetPktBox> {
-        lk_linkpoint_ref(domain, group, path, links, data, create_stamp).map(|v| v.as_netbox())
+        lk_linkpoint_ref(data,domain, group, path, links, create_stamp).map(|v| v.as_netbox())
     }
     pub fn lk_linkpoint_ref<'o>(
+        data: &'o [u8],
         domain: Domain,
         group: GroupID,
         path: &'o IPath,
         links: &'o [Link],
-        data: &'o [u8],
         create_stamp: Option<Stamp>,
     ) -> LkResult<NetPktParts<'o>> {
         Ok(pkt::try_linkpoint_ref(
             group,
             domain,
             path,
             links,
             data,
             create_stamp.unwrap_or_else(pkt::now),
             pkt::NetOpts::Default,
         )?)
     }
     /// create a keypoint and wrap it as a [NetPktBox]. i.e. a signed [lk_linkpoint]
     pub fn lk_keypoint(
+        signkey: &SigningKey,
+        data: &[u8],
         domain: Domain,
         group: GroupID,
         path: &IPath,
         links: &[Link],
-        data: &[u8],
         create_stamp: Option<Stamp>,
-        signkey: &SigningKey,
     ) -> LkResult<NetPktBox> {
-        lk_keypoint_ref(domain, group, path, links, data, create_stamp, signkey)
+        lk_keypoint_ref(signkey,data,domain, group, path, links, create_stamp)
             .map(|v| v.as_netbox())
     }
     pub fn lk_keypoint_ref<'o>(
+        signkey: &SigningKey,
+        data: &'o [u8],
         domain: Domain,
         group: GroupID,
         path: &'o IPath,
         links: &'o [Link],
-        data: &'o [u8],
         create_stamp: Option<Stamp>,
-        signkey: &SigningKey,
     ) -> LkResult<NetPktParts<'o>> {
         let create_stamp = create_stamp.unwrap_or_else(now);
         Ok(pkt::try_keypoint_ref(
             group,
             domain,
             path,
             links,
             data,
             create_stamp,
             signkey,
             pkt::NetOpts::Default,
         )?)
     }
 
-    pub fn lk_read(buf: &[u8], validate: bool, allow_private: bool) -> LkResult<NetPktBox> {
-        let pkt = super::misc::read::parse_netpkt(buf, validate)?
-            .map_err(|i| anyhow::anyhow!("pkt size is (at least) {i}"))?;
-        anyhow::ensure!(allow_private || pkt.group() != Some(&PRIVATE), "prevent reading private group");
-        Ok(pkt.as_netbox())
-    }
-
-    pub fn lk_write(p: &dyn NetPkt, out: &mut dyn io::Write) -> io::Result<()> {
+    
+    pub fn lk_read(buf: &[u8],allow_private:bool) -> Result<(Cow<NetPktPtr>,&[u8]),PktError> {
+        let pkt = linkspace_common::pkt::read::read_pkt(buf,false )?;
+        if !allow_private{pkt.check_private()?};
+        let size : usize = pkt.size().into();
+        Ok((pkt,&buf[size..]))
+    }
+    pub fn lk_read_unchecked(buf:&[u8],allow_private:bool) -> Result<(Cow<NetPktPtr>,&[u8]),PktError>{
+        let pkt = linkspace_common::pkt::read::read_pkt(buf,cfg!(debug_assertions))?;
+        if !allow_private{pkt.check_private()?};
+        let size : usize = pkt.size().into();
+        Ok((pkt,&buf[size..]))
+    }
+    
+    pub fn lk_write(p: &dyn NetPkt, allow_private:bool,out: &mut dyn io::Write) -> io::Result<()> {
+        if !allow_private{p.check_private().map_err(io::Error::other)?}
         let mut segments = p.byte_segments().io_slices();
         out.write_all_vectored(&mut segments)
     }
 }
 
 pub use abe::{lk_encode, lk_eval, lk_split_abe};
 /** ascii byte expression utilities
@@ -309,64 +320,68 @@
 
     // This function can also be called with the encode '/?' evaluator
     assert_eq!(lk_eval(r#"[/?:\0\0\0[u8:8]:u32]"#,())?,b"[u32:8]");
 
     // the options are a list of '/' separated functions
     // In this example 'u32' wont fit, LNS '#' lookup will succeed, if not the encoding would be base64
 
-    let mut public_grp = PUBLIC;
+    let public_grp = PUBLIC;
     assert_eq!(lk_encode(&*public_grp,"u32/#/b"), "[#:pub]");
 
     # Ok(())
     # }
     ```
     encode doesn't error, it falls back on plain abtxt.
     this variant also swallows bad options, see [lk_try_encode] to avoid doing so.
     **/
-    pub fn lk_encode(bytes: &[u8], options: &str) -> String {
+    pub fn lk_encode(bytes: impl AsRef<[u8]>, options: &str) -> String {
+        let bytes = bytes.as_ref();
         varctx::lk_try_encode(ctx::ctx(().into()).unwrap(), bytes, options,true)
             .unwrap_or_else(|_v| as_abtxt(bytes).to_string())
     }
     /** [lk_encode] with Err on:
     - wrong options
     - no result ( use a /: to fallback to abtxt)
     - if !ignore_encoder_err on any encoder error
     **/
-    pub fn lk_try_encode(bytes: &[u8], options: &str,ignore_encoder_err:bool) -> LkResult<String> {
-        Ok(varctx::lk_try_encode(
+    pub fn lk_try_encode(bytes: impl AsRef<[u8]>, options: &str,ignore_encoder_err:bool) -> LkResult<String> {
+        let bytes = bytes.as_ref();
+        varctx::lk_try_encode(
             ctx::ctx(().into()).unwrap(),
             bytes,
             options,
             ignore_encoder_err
-        )?)
+        )
     }
     /// Custom context for use in [varctx]
     pub mod ctx {
         #[thread_local]
         pub static LK_EVAL_CTX_RT: RefCell<Option<Linkspace>> = RefCell::new(None);
 
         use anyhow::Context;
         use linkspace_common::abe::eval::{EvalCtx, Scope};
-        use linkspace_common::prelude::{ArgV, EScope, NetPkt};
+        use linkspace_common::prelude::scope::ArgV;
+        use linkspace_common::prelude::{EScope, NetPkt};
         use linkspace_common::runtime::Linkspace;
         use std::cell::RefCell;
 
         use crate::LkResult;
-        type StdCtx<'o> = impl Scope + 'o;
+        pub(crate) type StdCtx<'o> = impl Scope + 'o;
         /// Create a new context for use in [crate::varctx] with [empty_ctx], [core_ctx], [ctx], or [lk_ctx] (default)
         pub struct LkCtx<'o>(pub(crate) InlineCtx<'o>);
         // we optimise for the instance where contains _ctx, but we expose several other context situations
+        #[allow(clippy::large_enum_variant)]
         pub(crate) enum InlineCtx<'o> {
             Std(StdCtx<'o>),
             // TODO UserCb
             Core,
             Empty,
         }
 
-        #[derive(Copy, Clone)]
+        #[derive(Copy, Clone,Default)]
         #[repr(C)]
         /// User config for setting additional context to evaluation.
         pub struct UserData<'o> {
             pub pkt: Option<&'o dyn NetPkt>,
             pub argv: Option<&'o [&'o [u8]]>,
         }
         impl From<()> for UserData<'static> {
@@ -407,28 +422,28 @@
                 UserData {
                     argv: Some(inp),
                     pkt: None,
                 }
             }
         }
 
-        pub fn ctx<'o>(udata: UserData<'o>) -> LkResult<LkCtx<'o>> {
-            _ctx(None, udata)
+        pub fn ctx(udata: UserData<'_>) -> LkResult<LkCtx<'_>> {
+            _ctx(None, udata,false)
         }
         pub const fn core_ctx() -> LkCtx<'static> {
             LkCtx(InlineCtx::Core)
         }
         pub const fn empty_ctx() -> LkCtx<'static> {
             LkCtx(InlineCtx::Empty)
         }
-        pub fn lk_ctx<'o>(lk: Option<&'o Linkspace>, udata: UserData<'o>) -> LkResult<LkCtx<'o>> {
-            _ctx(Some(lk), udata)
+        pub fn lk_ctx<'o>(lk: Option<&'o crate::Linkspace>, udata: UserData<'o>,enable_env:bool) -> LkResult<LkCtx<'o>> {
+            _ctx(Some(lk.map(|o|&o.0)), udata,enable_env)
         }
         /// lk:None => get threadlocal Lk . Some(None) => no linkspace
-        fn _ctx<'o>(lk: Option<Option<&'o Linkspace>>, udata: UserData<'o>) -> LkResult<LkCtx<'o>> {
+        fn _ctx<'o>(lk: Option<Option<&'o Linkspace>>, udata: UserData<'o>,enable_env:bool) -> LkResult<LkCtx<'o>> {
             let inp_ctx = udata
                 .argv
                 .map(|v| ArgV::try_fit(v).context("Too many inp values"))
                 .transpose()?
                 .map(EScope);
             use linkspace_common::core::eval::EVAL0_1;
             use linkspace_common::eval::std_ctx_v;
@@ -437,92 +452,94 @@
                 match lk {
                     None => LK_EVAL_CTX_RT.borrow().as_ref().cloned(),
                     Some(v) => v.cloned(),
                 }
                 .ok_or_else(|| anyhow::anyhow!("no linkspace instance was set"))
             };
             Ok(LkCtx(InlineCtx::Std((
-                opt_pkt_ctx(std_ctx_v(get, EVAL0_1), udata.pkt.map(|v| v as &dyn NetPkt)).scope,
+                opt_pkt_ctx(std_ctx_v(get, EVAL0_1,enable_env), udata.pkt.map(|v| v as &dyn NetPkt)).scope,
                 inp_ctx,
             ))))
         }
         impl<'o> LkCtx<'o> {
             pub(crate) fn as_dyn(&self) -> EvalCtx<&(dyn Scope + 'o)> {
                 match &self.0 {
                     InlineCtx::Std(scope) => EvalCtx { scope },
                     InlineCtx::Core => EvalCtx {
-                        scope: &linkspace_common::prelude::EVAL_SCOPE,
+                        scope: &linkspace_common::prelude::scope::EVAL_SCOPE,
                     },
                     InlineCtx::Empty => EvalCtx { scope: &() },
                 }
             }
         }
     }
 }
 
-pub use query::{lk_query, lk_query_parse, lk_query_print, lk_query_push, Query};
+pub use query::{lk_query, lk_query_parse, lk_query_print, lk_query_push, Query,Q};
 pub mod query {
     /**
     A set of predicates and options used to select packets
 
     The supported predicate fields are found in [PredicateType].
     The known options are found in [KnownOptions].
 
     ```
     # use linkspace::{*,prelude::*,abe::*};
     # fn main() -> LkResult{
 
-    let mut query = lk_query(None);
+    let mut query = lk_query(&Q);
 
-    // Add an entire set
-    let query_str = "
-    group:=:[#:pub]
-    domain:=:[a:hello]
-    prefix:=:/some/path
-    :id:default
-    ";
-    lk_query_parse(&mut query,query_str,())?;
+    // Add multiple predicates and options at once.
+    let query_str = [
+      "group:=:[#:pub]",
+      "domain:=:[a:hello]",
+      "prefix:=:/some/path",
+      ":qid:default"
+    ];
+    query = lk_query_parse(query,&query_str,())?;
     // Optionally with user data such as an argv
-    lk_query_parse(&mut query,"prefix:=:/some/[0]",&[b"path" as &[u8]]);
+    query = lk_query_parse(query,&["prefix:=:/some/[0]"],&[b"path" as &[u8]])?;
 
     // conflicting predicates return an error
-    let result = lk_query_parse(&mut query, "path_len:=:\0",());
+    let result = lk_query_parse(lk_query(&query), &["path_len:=:[u8:0]"],());
     assert!( result.is_err());
 
     // You can add a single statement directly
-    lk_query_push(&mut query,"create","<", &*now())?;
+    query = lk_query_push(query,"create","<", &*now())?;
     // Predicates get merged if they overlap
-    lk_query_push(&mut query,"create","<",&lk_eval("[now:-1D]",())?)?;
+    query = lk_query_push(query,"create","<",&lk_eval("[now:-1D]",())?)?;
 
-    // As you can see with
+    // As shown with:
     println!("{}",lk_query_print(&query,false));
-    # Ok(())}
+    # Ok(()) }
     ```
 
-    **/
-    #[derive(Default, Clone)]
+    */
+    #[derive(Clone)]
     pub struct Query(pub(crate) linkspace_common::core::query::Query);
 
+    pub static Q : Query = Query(linkspace_common::core::query::Query::DEFAULT);
+
     impl std::fmt::Display for Query {
         fn fmt(&self, f: &mut std::fmt::Formatter<'_>) -> std::fmt::Result {
             self.0.fmt(f)
         }
     }
     use std::ops::ControlFlow;
 
     pub use linkspace_common::core::predicate::predicate_type::PredicateType;
     pub use linkspace_common::core::query::KnownOptions;
     use linkspace_common::prelude::{ExtPredicate, PktPredicates};
 
     use crate::abe::ctx::UserData;
 
     use super::*;
-    /// Create a new [Query]. Optionally copy from a template
-    pub fn lk_query(copy_from: Option<&Query>) -> Query {
-        copy_from.map(|v| v.clone()).unwrap_or_default()
+    /// Create a new [Query]. Copy from a template. [Q] is the empty query.
+    pub fn lk_query(copy_from: &Query) -> Query {
+        Query(copy_from.0.clone())
     }
     /// Create a new [Query] specifically for a hash. Sets the right mode and 'i' count.
     pub fn lk_hash_query(hash: LkHash) -> Query {
         Query(linkspace_common::core::query::Query::hash_eq(hash))
     }
 
     /// Add a single statement to a [Query], potentially skipping an encode step.
@@ -558,58 +575,63 @@
     }
     /// Get the string representation of a [Query]
     pub fn lk_query_print(query: &Query, as_expr: bool) -> String {
         query.0.to_str(as_expr)
     }
 
     /// Compile a [Query] into a function which tests packets to deteremine if they match - WARN - slow and subject to change.
+    #[allow(clippy::type_complexity)]
     pub fn lk_query_compile(
         q: Query,
     ) -> LkResult<Box<dyn FnMut(&dyn NetPkt) -> (bool, ControlFlow<()>)>> {
         Ok(q.0.compile()?)
     }
 }
 
 pub use key::lk_key;
 pub mod key {
     use super::prelude::*;
     use super::LkResult;
     use linkspace_common::identity;
 
-    pub fn lk_keystr(key: &SigningKey, password: &[u8]) -> String {
+    pub fn lk_key_encrypt(key: &SigningKey, password: &[u8]) -> String {
         identity::encrypt(
             key,
             password,
             if password.is_empty() {
                 Some(identity::INSECURE_COST)
             } else {
                 None
             },
         )
     }
-    pub fn lk_keyopen(key: &str, password: &[u8]) -> LkResult<SigningKey> {
+    pub fn lk_key_decrypt(key: &str, password: &[u8]) -> LkResult<SigningKey> {
         Ok(linkspace_common::identity::decrypt(key, password)?)
     }
+    /// read the public key from a [lk_key_encrypt] string
+    pub fn lk_key_pubkey(key:&str) -> LkResult<PubKey>{
+        Ok(linkspace_common::identity::pubkey(key)?.into())
+    }
     pub fn lk_keygen() -> SigningKey {
         SigningKey::generate()
     }
 
     /** linkspace stored identity
 
     open (or generate) the key `name` which is also accessible as \[@:name:local\].
-    empty name defaults to ( i.e. \[@:local\] )
+    empty name defaults to ( i.e. \[@:me:local\] )
     **/
     pub fn lk_key(
         linkspace: &Linkspace,
-        password: &[u8],
-        name: &str,
+        password: Option<&[u8]>,
+        name: Option<&str>,
         create: bool,
     ) -> LkResult<SigningKey> {
         super::varctx::lk_key(super::abe::ctx::ctx(().into())?,linkspace,password,name,create)
-        
+
     }
 }
 
 pub use runtime::{
     lk_get, lk_open, lk_process, lk_process_while, lk_save, lk_stop, lk_watch, Linkspace,
 };
 pub mod runtime {
@@ -623,29 +645,31 @@
     Use [lk_process] or [lk_process_while] to update the reader
     and get packets with [lk_get], [lk_get_all], and [lk_watch].
     **/
     #[derive(Clone)]
     #[repr(transparent)]
     pub struct Linkspace(pub(crate) linkspace_common::runtime::Linkspace);
 
-    use linkspace_common::prelude::WatchIDRef;
+    use std::time::Instant;
+
+    use linkspace_common::{prelude::QueryIDRef, saturating_cast, saturating_neg_cast};
     use tracing::{debug_span };
 
     use super::*;
     /// open a linkspace runtime.
     ///
-    /// will look at `path` or $LINKSPACE or '$HOME'
+    /// will look at `path` or $LK_DIR or '$HOME'
     /// and open 'PATH/linkspace' unless the basename of PATH is linkspacel 'linkspace'
     ///
     /// A runtime is used in many arguments.
     /// Most notable to [lk_save], [lk_get], and [lk_watch] packets.
     /// You can open the same instance in multiple threads (sharing their db session & ipc ) and across multiple processes.
     /// moving an open linkspace across threads is not supported.
-    pub fn lk_open(path: Option<&std::path::Path>, create: bool) -> std::io::Result<Linkspace> {
-        let rt = linkspace_common::static_env::open_linkspace_root(path, create)?;
+    pub fn lk_open(dir: Option<&std::path::Path>, create: bool) -> std::io::Result<Linkspace> {
+        let rt = linkspace_common::static_env::open_linkspace_dir(dir, create)?;
         let mut eval_ctx = crate::abe::ctx::LK_EVAL_CTX_RT.borrow_mut();
         if eval_ctx.is_none() {
             *eval_ctx = Some(rt.clone())
         }
         Ok(Linkspace(rt))
     }
     /*
@@ -658,162 +682,184 @@
     /// save a packet. Returns true if new and false if its old.
     pub fn lk_save(lk: &Linkspace, pkt: &dyn NetPkt) -> std::io::Result<bool> {
         linkspace_common::core::env::write_trait::save_pkt(&mut lk.0.get_writer(), pkt)
     }
     pub fn lk_save_all(lk: &Linkspace, pkts: &[&dyn NetPkt]) -> std::io::Result<usize> {
         linkspace_common::core::env::write_trait::save_pkts(&mut lk.0.get_writer(), pkts).map(|(i,_)|i)
     }
-    /// [lk_watch] but only for currently indexed packets. Don't forget to [lk_process]
-    /// Terminates early when `cb` returns false
+    
+    /// Run callback for every match for the query in the database.
+    /// Break early if the callback returns true. 
+    /// If break => number of matches
+    /// If no break ( cb only returned false ) => -1 * Number of matches
     pub fn lk_get_all(
         lk: &Linkspace,
         query: &Query,
         cb: &mut dyn FnMut(&dyn NetPkt) -> bool,
-    ) -> LkResult<u32> {
+    ) -> LkResult<i32> {
         let mut c = 0;
         let r = lk.0.get_reader();
         let mode = query.0.get_mode()?;
+        let mut breaks = false;
         for p in r.query(mode, &query.0.predicates, &mut c)? {
-            let cont = (cb)(&p);
-            if !cont {
-                break;
-            }
+            breaks = (cb)(&p);
+            if breaks{break}
         }
-        Ok(c)
+        Ok(if breaks { saturating_cast(c)}else {saturating_neg_cast(c)})
     }
 
-    /// get a single packet. Don't forget to [lk_process]
+
+    /// get the first result from the database matching the query.
     pub fn lk_get(lk: &Linkspace, query: &Query) -> LkResult<Option<NetPktBox>> {
         lk_get_ref(lk, query, &mut |v| v.as_netbox())
     }
-    /** read a single packet mmap-ed packet. Don't forget to [lk_process]
+    /** read a single packet directly without copying. 
     This means that [NetPkt::net_header_mut] is unavailable.
-    You can wrap it in a [crate::misc::ReroutePkt] to change this or [NetPkt::as_netbox] to allocate and mutate.
+    To mutate the header, wrap the result in [crate::misc::ReroutePkt] or copy with [NetPkt::as_netbox]..
     **/
     pub fn lk_get_ref<A>(
         lk: &Linkspace,
         query: &Query,
         cb: &mut dyn FnMut(RecvPktPtr) -> A,
     ) -> LkResult<Option<A>> {
         let mode = query.0.get_mode()?;
         let mut i = 0;
         let reader = lk.0.get_reader();
         let opt_pkt = reader.query(mode, &query.0.predicates, &mut i)?.next();
         Ok(opt_pkt.map(|v| (cb)(v)))
     }
-    /**
-    watch packets matching the query - both already in the db and new packets on arrival
+    pub fn lk_get_hash<A>(lk:&Linkspace,hash: LkHash,
+                       cb: &mut dyn FnMut(RecvPktPtr) -> A,
+    ) -> anyhow::Result<Option<A>> {
+        let reader = lk.0.get_reader();
+        let opt = reader.read(&hash)?;
+        Ok(opt.map(|v|(cb)(v)))
+    }
 
-    Calls `cb` for each matching packet.
-    If the `query` contains the id option ( e.g. ':id:example' ) the `cb` is also called for all new packets during [[lk_process]] and [[lk_process_while]].
-    The watch is dropped when
-    - the cb returns 'break' ( usually false )
+    /**
+    Registers the query under its 'qid' ( .e.g. set by lk_query_parse(q,":qid:myqid) )
+    Before returning, calls cb for every packet in the database.
+    The absolute return value is the number of times the callback was called.
+    A positive value means the callback finished already.
+
+    A 0 or negative value means it is registered and shall be called during
+    a [[lk_process]] or [[lk_process_while]] call,
+    for every new packet matching the query.
+    
+    The watch is finished when
+    - the cb returns 'break' (In other languages we map this to the boolean 'true')
+    - the predicate set will never match again (e.g. the 'i_*' or 'recv' predicate shall never match again )
     - [[lk_stop]] is called with the matching id
-    - the predicate set will never match again ( 'i' counters and recv )
 
-    returns the number matches in the local index.
-    i.e. the number of times cb was called immediatly.
     **/
-    pub fn lk_watch(lk: &Linkspace, query: &Query, cb: impl PktHandler + 'static) -> LkResult<u32> {
+    pub fn lk_watch(lk: &Linkspace, query: &Query, cb: impl PktHandler + 'static) -> LkResult<i32> {
         lk_watch2(lk, query, cb, debug_span!("lk_watch - (untraced)"))
     }
 
     /// [lk_watch] with a custom log [tracing::Span]
     /// The span will be entered on every callback.
     /// If you do not care for structured options you can use [vspan] `lk_watch2(.. , .. ,.. , vspan("my function"))`
     pub fn lk_watch2(
         lk: &Linkspace,
         query: &Query,
         cb: impl PktHandler + 'static,
         span: tracing::Span,
-    ) -> LkResult<u32> {
-        Ok(lk.0.watch_query(&query.0, interop::Handler(cb), span)?)
+    ) -> LkResult<i32> {
+        lk.0.watch_query(&query.0, interop::Handler(cb), span)
     }
     /// See [lk_watch2]
     pub fn vspan(name: &str) -> tracing::Span {
         tracing::debug_span!("{}", name)
     }
 
-    /// close lk_watch watches based on the watch id ':id:example' in the query.
+    /// close lk_watch watches based on the query id ':qid:example' in the query.
     pub fn lk_stop(rt: &Linkspace, id: &[u8], range: bool) {
         if range {
             rt.0.close_range(id)
         } else {
             rt.0.close(id)
         }
     }
 
     /// process the log of new packets and trigger callbacks. Updates the reader to the latest state.
     pub fn lk_process(rt: &Linkspace) -> Stamp {
         rt.0.process()
     }
-    /** process the log of new packets continuously
-
-    will return when:
-    - max_wait has elapsed between new packets - return false
-      e.g. lk_eval("[s:+1M]") or 0u64 to ignore
-    - until time has been reached - returns false
-      e.g. lk_eval("[now:+1M]") or 0u64 to ignore
-    - (watch_id,false) was triggered - returns true
-    - (watch_id,true) was finished - returns true
-    - no more watch callbacks exists - returns true
-    **/
-    pub fn lk_process_while(lk: &Linkspace,watch_id:Option<(&WatchIDRef,bool)>, d_max_wait: Stamp, at_until: Stamp) -> LkResult<bool> {
-        let max_wait = (d_max_wait != Stamp::ZERO)
-            .then_some(std::time::Duration::from_micros(d_max_wait.get()));
-
-        let until = (at_until != Stamp::ZERO).then(|| pkt::as_instance(at_until).into());
-        lk.0.run_while(max_wait, until,watch_id)
+    /**
+    continuously process callbacks until:
+    - timeout time has passed
+    - qid = Some and qid is matched at least once => if removed returns 1, if still registered returns -1
+    - qid = None => no more callbacks (1) 
+     **/
+    pub fn lk_process_while(lk: &Linkspace,qid:Option<&QueryIDRef>, timeout: Stamp) -> LkResult<isize> {
+        let timeout = (timeout != Stamp::ZERO).then(|| Instant::now() + std::time::Duration::from_micros(timeout.get()));
+        _lk_process_while(lk, qid, timeout)
+    }
+    #[doc(hidden)]
+    // simplifies python ffi bindings
+    pub fn _lk_process_while(lk: &Linkspace,qid:Option<&QueryIDRef>, timeout: Option<Instant>) -> LkResult<isize> {
+        lk.0.run_while(timeout,qid)
     }
-
     pub fn lk_list_watches(lk: &Linkspace, cb: &mut dyn FnMut(&[u8], &Query)) {
         for el in lk.0.dbg_watches().0.entries() {
-            cb(&el.id, Query::from_impl(&*el.query))
+            cb(&el.query_id, Query::from_impl(&el.query))
         }
     }
     #[derive(Debug)]
     pub struct LkInfo<'o> {
-        pub path: &'o std::path::Path,
+        pub dir: &'o std::path::Path,
     }
     pub fn lk_info(lk: &Linkspace) -> LkInfo {
         LkInfo {
-            path: lk.0.env().location(),
+            dir: lk.0.env().dir(),
         }
     }
 }
 
 /// A set of functions that adhere to conventions
 pub mod conventions;
 pub use conventions::lk_pull;
 
 pub use consts::{PRIVATE, PUBLIC};
 pub mod consts {
     pub use linkspace_common::core::consts::pkt_consts::*;
-    pub use linkspace_common::core::consts::{EXCHANGE_DOMAIN, PRIVATE, PUBLIC};
+    pub use linkspace_common::core::consts::{EXCHANGE_DOMAIN, PRIVATE, PUBLIC,TEST_GROUP};
 }
-pub use misc::cb;
+pub use misc::try_cb;
 pub mod misc {
+    #![allow(clippy::type_complexity)]
     use std::ops::{ControlFlow, Try};
 
     pub use linkspace_common::core::env::tree_key::TreeEntry;
     pub use linkspace_common::pkt::netpkt::DEFAULT_ROUTING_BITS;
     pub use linkspace_common::pkt::reroute::{RecvPkt, ReroutePkt, ShareArcPkt};
     pub use linkspace_common::pkt::FieldEnum;
     pub use linkspace_common::pkt::read;
-    use linkspace_common::prelude::NetPkt;
+    use linkspace_common::prelude::{NetPkt, B64 };
     pub use linkspace_common::runtime::handlers::StopReason;
 
     use crate::{Linkspace, PktHandler, Query};
 
+    #[derive(Copy,Clone)]
     pub struct Cb<A, B> {
         pub handle_pkt: A,
         pub stopped: B,
     }
     pub fn nop_stopped(_: Query, _: &Linkspace, _: StopReason, _: u32, _: u32) {}
-    pub fn cb<A, R, E>(
+
+
+    pub fn cb<A>(mut handle_pkt:A) -> Cb<impl FnMut(&dyn NetPkt,&Linkspace) -> ControlFlow<()>,fn(Query,&Linkspace,StopReason,u32,u32)>
+    where A: FnMut(&dyn NetPkt,&Linkspace) -> bool {
+        Cb{
+            stopped:nop_stopped,
+            handle_pkt : move |pkt:&dyn NetPkt,lk:&Linkspace| { if (handle_pkt)(pkt,lk) { ControlFlow::Break(())} else { ControlFlow::Continue(())}}
+        }
+    } 
+
+    pub fn try_cb<A, R, E>(
         mut handle_pkt: A,
     ) -> Cb<
         impl FnMut(&dyn NetPkt, &Linkspace) -> ControlFlow<()> + 'static,
         fn(Query, &Linkspace, StopReason, u32, u32),
     >
     where
         R: Try<Output = (), Residual = E>,
@@ -846,19 +892,59 @@
             reason: StopReason,
             total: u32,
             new: u32,
         ) {
             (self.stopped)(query, lk, reason, total, new)
         }
     }
+
+    /// Blake3 hash
+    pub fn blake3_hash(val:&[u8]) -> B64<[u8;32]>{
+        B64(*linkspace_common::core::crypto::blake3_hash(val).as_bytes())
+    }
+
+
+    /**
+    Read bytes as a [0,1) float by reading the first 52 bits.
+    Panics if fewer than 8 bytes are supplied
+    Primary use is to produces the same 'random' value by using NetPkt::hash or [blake3_hash],
+    regardless of language, and without an additional RNG dependencies,
+     */
+    pub fn bytes2uniform(val:&[u8]) -> f64{
+        let rand_u64 = u64::from_be_bytes(val[..8].try_into().expect("bytes2uniform requires at least 8 bytes"));
+        let f64_exponent_bits: u64 = 1023u64 << 52;
+        // Generate a value in the range [1, 2)
+        let value1_2 = f64::from_bits((rand_u64 >> (64-52)) | f64_exponent_bits);
+        value1_2 - 1.0
+    }
+
+    /* TODO: remove
+    /**
+    Read a float [0,1) into 32 bytes (big endian).
+    Its primary use is for the result can be compared to [NetPkt::hash] or [blake3_hash].
+    These emulates randomness, regardless of language and without an additional RNG dependencies.
+    i.e. if uniform2bytes(0.1) > pkt.hash { println!("This has a 0.1 chance")}
+    */
+    pub fn uniform2bytes(val:f64) -> anyhow::Result<B64<[u8;32]>>{
+        let mut result = B64([0;32]);
+        if val < 0.0 || val >= 1.0 { anyhow::bail!("function is inverse of bytes2uniform, thus undefined outside of [0,1)")}
+        let bits = (val + 1.0).to_bits();
+        let headbytes = (bits << (64-52)).to_be_bytes();
+        result.0[0..8].copy_from_slice(&headbytes);
+        result
+    }
+    */
+
 }
 
 /// Functions with a custom eval context
 pub mod varctx {
 
+    use std::borrow::{Cow };
+
     use super::*;
     use crate::abe::ctx::LkCtx;
     use linkspace_common::abe::{eval::eval, parse_abe};
 
     pub fn lk_eval(ctx: LkCtx, expr: &str) -> LkResult<Vec<u8>> {
         let expr = parse_abe(expr)?;
         let val = eval(&ctx.as_dyn(), &expr)?;
@@ -878,36 +964,50 @@
             query.0.parse(stmnt.as_bytes(), &ctx.as_dyn())?;
         }
         Ok(query)
     }
     pub fn lk_key(
         ctx:LkCtx,
         linkspace: &Linkspace,
-        password: &[u8],
-        name: &str,
+        password: Option<&[u8]>,
+        name: Option<&str>,
         create: bool,
     ) -> LkResult<SigningKey> {
         use linkspace_common::protocols::lns;
+
+        let name = match name {
+            Some(v) => Cow::Borrowed(v),
+            None => std::env::var("LK_KEYNAME").map(Cow::Owned).unwrap_or(Cow::Borrowed("me:local"))
+        };
+        let password = match password{
+            Some(v) => Cow::Borrowed(v),
+            None => match std::env::var("LK_PASS"){
+                Ok(abe) => Cow::Owned(eval(&ctx.as_dyn(),&parse_abe(&abe)?)?.concat()),
+                Err(_e) => Cow::Borrowed(&[] as &[u8]),
+            }
+        };
         let expr = parse_abe(&name)?;
-        let name : lns::name::Name= eval(&ctx.as_dyn(), &expr)?.try_into()?;
+        let name : lns::name::Name = eval(&ctx.as_dyn(), &expr)?.try_into()?;
         match lns::lookup_enckey(&linkspace.0, &name)?{
             Some((_,enckey)) => {
-                Ok(linkspace_common::identity::decrypt(&enckey, password)?)
+                Ok(linkspace_common::identity::decrypt(&enckey, &password)?)
             }
             None => {
                 if create {
                     use super::key::*;
                     let key = lk_keygen();
-                    let enckey = super::key::lk_keystr(&key, password);
+                    let enckey = super::key::lk_key_encrypt(&key, &password);
                     lns::setup_special_keyclaim(&linkspace.0, name, &enckey, false)?;
                     Ok(key)
                 } else {
                     anyhow::bail!("no matching entry found")
                 }
             }
         }
     }
 }
 
 // Allow for interop when importing linkspace_common
 #[doc(hidden)]
 pub mod interop;
+
+pub static BUILD_INFO : &str = build_info::format!("{}", $);
```

### Comparing `linkspace-0.1.4/local_dependencies/linkspace-cryptography/LICENSE` & `linkspace-0.3.0rc2/local_dependencies/linkspace-core/LICENSE`

 * *Files identical despite different names*

### Comparing `linkspace-0.1.4/local_dependencies/linkspace-cryptography/src/keygen.rs` & `linkspace-0.3.0rc2/local_dependencies/linkspace-cryptography/src/keygen.rs`

 * *Files identical despite different names*

### Comparing `linkspace-0.1.4/local_dependencies/linkspace-cryptography/src/lib.rs` & `linkspace-0.3.0rc2/local_dependencies/linkspace-cryptography/src/lib.rs`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,15 @@
 // Copyright Anton Sol
 //
 // This Source Code Form is subject to the terms of the Mozilla Public
 // License, v. 2.0. If a copy of the MPL was not distributed with this
 // file, You can obtain one at https://mozilla.org/MPL/2.0/.
 use std::fmt::Debug;
 
-#[cfg(feature = "keygen")]
 pub mod keygen;
-#[cfg(feature = "keygen")]
-pub use rand;
 
 pub use k256;
 pub use k256::ecdsa::Error;
 pub use k256::schnorr;
 
 #[derive(Clone)]
 pub struct SigningKey(pub schnorr::SigningKey);
@@ -37,28 +34,33 @@
 pub type Hash = [u8; 32];
 pub type PublicKey = [u8; 32];
 pub type Signature = [u8; 64];
 
 pub use ops::*;
 #[cfg(not(miri))]
 pub mod ops {
+
+    use k256::schnorr::signature::hazmat::PrehashVerifier;
+    use rand::{Rng};
+
     use super::*;
     pub fn sign_hash(key: &SigningKey, hash: &Hash) -> Signature {
-        *key.0
-            .try_sign_prehashed(hash, &Default::default())
+        let mut aux_rand = [0;32];
+        if false { rand::thread_rng().fill(&mut aux_rand);}
+        key.0.sign_prehash_with_aux_rand(hash,&aux_rand)
             .unwrap()
-            .as_bytes()
+            .to_bytes()
     }
     pub fn validate_signature(
         pubkey: &PublicKey,
         signature: &Signature,
         hash: &Hash,
     ) -> Result<(), k256::ecdsa::Error> {
         schnorr::VerifyingKey::from_bytes(pubkey)?
-            .verify_prehashed(hash, &schnorr::Signature::try_from(signature.as_slice())?)
+            .verify_prehash(hash, &schnorr::Signature::try_from(signature.as_slice())?)
     }
     pub fn hash_segments(s: &[&[u8]]) -> Hash {
         let mut hasher = blake3::Hasher::new();
         for segm in s {
             hasher.update(segm);
         }
         let hash = hasher.finalize();
```

### Comparing `linkspace-0.1.4/local_dependencies/linkspace-argon2-identity/Cargo.toml` & `linkspace-0.3.0rc2/local_dependencies/abe/Cargo.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,24 @@
 [package]
-name = "linkspace-argon2-identity"
-version = "0.1.0"
-edition = "2021"
-license = "MPL-2.0"
-homepage = "https://antonsol919.github.io/linkspace/"
-documentation = "https://antonsol919.github.io/linkspace/docs/guide/index.html"
-authors = ["Azon <AntonSol919@gmail.com>"]
-repository = "https://github.com/AntonSol919/linkspace"
-categories = []
-keywords = []
-description = "argon2 encrypted schnorr keys"
 
-# See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
+name = "abe"
+version = "0.3.0-rc1"
+authors = ["Anton Sol <AntonSol919@gmail.com>"]
+categories = ["encoding","parsing"]
+keywords = ["ascii-byte-expr", "ascii-byte","abe"]
+description = "Ascii-byte-expression : a tiny byte templating language"
+
+edition= "2021"
+license= "MPL-2.0"
+homepage= "https://www.linkspace.dev"
+documentation= "https://www.linkspace.dev/docs/guide/index.html"
+repository= "https://github.com/AntonSol919/linkspace"
+resolver = "2"
+
 [dependencies]
-linkspace-cryptography = { path = "../linkspace-cryptography", version="0.1.0"}
-rust-argon2 = "1.0.0"
-thiserror = "1.0.31"
-base64 = "0.13.0"
+anyhow= "=1.0.71"
+serde= { version = "=1.0.160", features = ["derive"] }
+thiserror=  "=1.0.40"
+arrayvec= "=0.7.2  "
+hex= "=0.4.3"
+base64="=0.21"
+bstr= {version = "1.5.0" ,default-features=false}
```

### Comparing `linkspace-0.1.4/local_dependencies/linkspace-argon2-identity/LICENSE` & `linkspace-0.3.0rc2/local_dependencies/linkspace-pkt/LICENSE`

 * *Files identical despite different names*

### Comparing `linkspace-0.1.4/local_dependencies/linkspace-argon2-identity/src/lib.rs` & `linkspace-0.3.0rc2/local_dependencies/linkspace-argon2-identity/src/lib.rs`

 * *Files 24% similar despite different names*

```diff
@@ -4,92 +4,116 @@
 // License, v. 2.0. If a copy of the MPL was not distributed with this
 // file, You can obtain one at https://mozilla.org/MPL/2.0/.
 /**
 Encrypt public and private key with argon2.
 Uses public key as salt, xors private key with the encoded hash.
 **/
 // This is not ideal but both the package argon2 and rust-argon2 are hiding implementation details. 
+#[derive(Copy,Clone,PartialEq)]
+pub struct Costs{
+    pub mem:u32,
+    pub time:u32,
+    pub parallelism:u32
+}
+
+pub const DEFAULT_COST: Costs = Costs{
+    mem:  16384,
+    time: 4,
+    parallelism: 4,
+};
+pub const EXPENSIVE_COST: Costs = Costs{
+    mem:  16384*2,
+    time: 8,
+    parallelism: 8,
+};
+pub const INSECURE_COST: Costs = Costs{
+    mem:  8,
+    time: 1,
+    parallelism: 1,
+};
+
+
+impl Default for Costs{
+    fn default() -> Self {
+        DEFAULT_COST
+    }
+}
 mod params {
     pub struct Decoded {
-        pub mem_cost: u32,
-        pub time_cost: u32,
-        pub parallelism: u32,
+        pub costs:crate::Costs,
         pub salt: Vec<u8>,
-        pub hash: Vec<u8>,
+        pub hash: [u8;32],
     }
     /// Attempts to decode the encoded string slice.
     pub fn decode_string(encoded: &str) -> Option<Decoded> {
+        use base64::prelude::*;
         let items = encoded.strip_prefix("$argon2d$v=19$")?;
-        let mut items_it = items.split("$");
+        let mut items_it = items.split('$');
         let options = items_it.next()?;
-        let salt = base64::decode(items_it.next()?).ok()?;
-        let hash = base64::decode(items_it.next()?).ok()?;
-        let mut opt_it = options.split(",").filter_map(|st| st.split_once("="))
+        let salt = BASE64_STANDARD_NO_PAD.decode(items_it.next()?).ok()?;
+        let hash = BASE64_STANDARD_NO_PAD.decode(items_it.next()?).ok()?.try_into().ok()?;
+        let mut opt_it = options.split(',').filter_map(|st| st.split_once('='))
             .zip(["m","t","p"])
             .filter(|((kind,_val),expect)| (kind == expect))
             .filter_map(|((_,val),_)| val.parse::<u32>().ok());
-        let (mem_cost,time_cost,parallelism) = (opt_it.next()?,opt_it.next()?,opt_it.next()?);
+        let (mem,time,parallelism) = (opt_it.next()?,opt_it.next()?,opt_it.next()?);
         if opt_it.next().is_some() { return None}
         Some(Decoded {
-            mem_cost,
-            time_cost,
-            parallelism,
+            costs: crate::Costs { mem, time, parallelism},
             salt,
             hash,
         })
     }
 }
 
 
 use argon2::Config;
-use linkspace_cryptography::*;
+use linkspace_cryptography::{* };
 
 pub use linkspace_cryptography::keygen;
 use thiserror::Error;
 
-pub const DEFAULT_MEM_COST: u32 = 16384;
-pub const DEFAULT_TIME_COST: u32 = 4;
-
-pub const DEFAULT_COST: (u32, u32) = (DEFAULT_MEM_COST, DEFAULT_TIME_COST);
-pub const EXPENSIVE_COST: (u32, u32) = (DEFAULT_MEM_COST*2, DEFAULT_TIME_COST*2);
-pub const INSECURE_COST: (u32, u32) = (8, 1);
-
 #[derive(Error, Debug)]
 pub enum KeyError {
     #[error("The data supplied is in an unknown format")]
     BadData,
     #[error("The password is incorrect")]
     WrongPassword,
 }
 
-pub fn encrypt(key: &SigningKey, password: &[u8], cost: Option<(u32, u32)>) -> String {
-    let (mem_cost, time_cost) = cost.unwrap_or(DEFAULT_COST);
+pub fn encrypt(key: &SigningKey, password: &[u8], cost:Option<Costs>) -> String{
+    _encrypt(key, password, cost.unwrap_or(DEFAULT_COST)).expect("bug - key encryption errror?")
+}
+fn _encrypt(key: &SigningKey, password: &[u8], cost: Costs) -> Option<String>{
+    use base64::prelude::*;
+    let Costs { mem, time, parallelism }=cost;
     let config = Config {
         variant: argon2::Variant::Argon2d,
-        mem_cost,
-        time_cost,
+        mem_cost:mem,
+        time_cost:time,
+        lanes:parallelism,
         ..Config::default()
     };
-    let encoded = argon2::hash_encoded(password, &key.pubkey_bytes(), &config).unwrap();
+    let encoded = argon2::hash_encoded(password, &key.pubkey_bytes(), &config).ok()?;
     // This is some dirty work to decode the internal argon representation so we can xor our secret
-    let (conf,digest) = encoded.rsplit_once('$').unwrap();
-    let digest = base64::decode(digest).unwrap();
-
+    let (conf,digest) = encoded.rsplit_once('$')?;
+    let digest = BASE64_STANDARD_NO_PAD.decode(digest).ok()?;
+    
     let xored = digest
         .into_iter()
         .zip(key.0.to_bytes().iter())
         .map(|(a, b)| a ^ b)
         .collect::<Vec<_>>();
 
-    let encrypted_secret = base64::encode(xored);
+    let encrypted_secret = BASE64_STANDARD_NO_PAD.encode(xored);
     let result = String::from_iter([conf, "$", &*encrypted_secret]);
     if cfg!(debug_assertions) {
-        decrypt(&result, password).unwrap();
+        decrypt(&result, password).expect("encrypt/decrypt bug!");
     }
-    result
+    Some(result)
 }
 pub fn pubkey(identity: &str) -> Result<PublicKey, KeyError> {
     let argon_param = params::decode_string(identity).ok_or(KeyError::BadData)?;
     if argon_param.salt.len() != std::mem::size_of::<PublicKey>() {
         return Err(KeyError::BadData);
     }
 
@@ -99,54 +123,55 @@
     let mut pubkey = [0; 32];
     pubkey.copy_from_slice(&argon_param.salt);
     Ok(pubkey)
 }
 
 pub fn decrypt(enckey: &str, password: &[u8]) -> Result<SigningKey, KeyError> {
     let argon_param = params::decode_string(enckey).ok_or(KeyError::BadData)?;
+    let Costs { mem, time, parallelism } = argon_param.costs;
     let config = Config {
         variant: argon2::Variant::Argon2d,
         version: argon2::Version::Version13,
-        mem_cost: argon_param.mem_cost,
-        time_cost: argon_param.time_cost,
-        lanes: argon_param.parallelism,
+        mem_cost: mem,
+        time_cost: time,
+        lanes: parallelism,
         thread_mode: argon2::ThreadMode::Sequential,
         secret: &[],
         ad: &[],
         hash_length: 32,
     };
 
-    let mut digest =
-        argon2::hash_raw(password, &argon_param.salt, &config).map_err(|_| KeyError::BadData)?;
-
-    digest
-        .iter_mut()
-        .zip(argon_param.hash)
-        .for_each(|(a, b)| *a ^= b);
-    let secret =
-        SigningKey::try_from(digest.try_into().unwrap()).map_err(|_| KeyError::WrongPassword)?;
+    let digest = argon2::hash_raw(password, &argon_param.salt, &config).map_err(|_| KeyError::BadData)?;
+    let digest : [u8;32] = digest.try_into().map_err(|_| KeyError::BadData)?;
+    let secret = std::array::from_fn(|i| digest[i] ^ argon_param.hash[i]);
+    let secret = SigningKey::try_from(secret).map_err(|_| KeyError::WrongPassword)?;
 
     let pubkey = secret.pubkey_bytes();
     if pubkey.as_ref() != argon_param.salt {
         return Err(KeyError::WrongPassword);
     }
     Ok(secret)
 }
 
 
 #[test]
 pub fn test_encoding_decoding(){
     fn check_key(i:&str,pass:&[u8]){
+        println!("Checking {i}");
         let key = decrypt(i, pass).unwrap();
         let pubkey = pubkey(i).unwrap();
         let from_key = key.pubkey_bytes();
         assert_eq!(pubkey,from_key);
         let st = encrypt(&key, pass, None);
         assert_eq!(i,st)
     }
-    let empty = "$argon2d$v=19$m=16384,t=4,p=1$WXRa3NqtPwBpbyQPhEx1rCaMBKqiUDyZaecjdgIPLbY$EoCRQphpbp05CiLWEVncNE5zEqs4/K6KU2rrCtiSf0Y=";
+    let key = SigningKey::generate();
+    let e = encrypt(&key, b"hello", None);
+    check_key(&e, b"hello");
+
+    let empty = "$argon2d$v=19$m=16384,t=4,p=1$WXRa3NqtPwBpbyQPhEx1rCaMBKqiUDyZaecjdgIPLbY$EoCRQphpbp05CiLWEVncNE5zEqs4/K6KU2rrCtiSf0Y";
     check_key(empty,b"");
-    let hello = "$argon2d$v=19$m=16384,t=4,p=1$Au5RqvgqltiHj8ajyxwHrYBmaOudIx1XExjeM4zxS5I$mt8Q/Gq+jTM/4Ci9bW0P/4AJFWNuY5PWxzzsDyeBCb0=";
+    let hello = "$argon2d$v=19$m=16384,t=4,p=1$Au5RqvgqltiHj8ajyxwHrYBmaOudIx1XExjeM4zxS5I$mt8Q/Gq+jTM/4Ci9bW0P/4AJFWNuY5PWxzzsDyeBCb0";
     check_key(hello,b"hello");
-    let hello = "$argon2d$v=19$m=16384,t=4,p=1$Au5RqvgqltiHj8ajyxwHrYBmaOudIx1XExjeM4zxS5I$mt8Q/Gq+jTM/4Ci9bW0P/4AJFWNuY5PWxzzsDyeBCb0=";
+    let hello = "$argon2d$v=19$m=16384,t=4,p=1$Au5RqvgqltiHj8ajyxwHrYBmaOudIx1XExjeM4zxS5I$mt8Q/Gq+jTM/4Ci9bW0P/4AJFWNuY5PWxzzsDyeBCb0";
     assert!(decrypt(hello,b"not hello").is_err());
 }
```

### Comparing `linkspace-0.1.4/local_dependencies/linkspace-common/Cargo.toml` & `linkspace-0.3.0rc2/local_dependencies/linkspace-core/Cargo.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,42 +1,39 @@
 [package]
-name = "linkspace-common"
-version = "0.1.1"
-edition = "2021"
-license = "MPL-2.0"
-authors = ["Azon <AntonSol919@gmail.com>"]
-repository = "https://github.com/AntonSol919/linkspace"
+name = "linkspace-core"
 categories = []
 keywords = ["linkspace"]
-description = "linkspace common"
+description = "linkspace core"
 
-# See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
+version= "0.3.0-rc1"
+authors= ["Anton Sol <AntonSol919@gmail.com>"]
+edition= "2021"
+license= "MPL-2.0"
+homepage= "https://www.linkspace.dev"
+documentation= "https://www.linkspace.dev/docs/guide/index.html"
+repository= "https://github.com/AntonSol919/linkspace"
+resolver = "2"
 
+# See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [features]
-default = ["full", "lmdb"]
-lmdb=["linkspace-core/lmdb"]
-inmem=["linkspace-core/inmem"]
-fs=["memmap2", "notify"]
-cli=["clap", "clap/env", "clap/derive", "rpassword"]
-full=["fs", "cli"]
+default=["lmdb"]
+lmdb = ["lmdb-rkv", "lmdb-rkv-sys", "libc"]
 
 [dependencies]
-abe = { path = "../abe", version = "0.1.0"}
-byte-fmt = { path = "../byte-fmt", version = "0.1.0"}
-linkspace-pkt = { path = "../linkspace-pkt", version = "0.1.1"}
-linkspace-core= { path = "../linkspace-core",default-features=false, version = "0.1.1"}
-linkspace-argon2-identity = { path = "../linkspace-argon2-identity", version = "0.1.0"}
-
-anyhow = "1.0.69"
-serde = { version = "1.0.139", features = ["derive"] }
-rand = {version="0.8.5"}
-tracing = "0.1.35"
-thiserror = "1.0.31"
-memmap2 = { version = "0.5.5", optional = true }
-notify = { version = "5.0", optional = true }
-rpassword = { version = "7.1" , optional = true }
-clap = { version = "^4.0.6", features = ["derive"], optional = true }
-async_executors = { version = "0.6.0", features = ["timer","async_global","bindgen","localpool"] }
-futures = "0.3.21"
-either = "1.7.0"
-tracing-subscriber = "0.3.14"
 
+linkspace-pkt = { path = "../linkspace-pkt", version="0.3.0-rc1"}
+linkspace-cryptography = { path = "../linkspace-cryptography",version="0.3.0-rc1"}
+
+arrayvec= "=0.7.2  "
+anyhow= "=1.0.71"
+thiserror=  "=1.0.40"
+tracing= {version = "=0.1.37",features=["release_max_level_info"]}
+either= "=1.8.1"
+serde = { version = "=1.0.160", features = ["derive","rc"] }
+libc = { version = "=0.2.142", optional =true}
+
+dunce = "1.0.2"
+ipcbus = { path = "../ipcbus", version = "0.1.0"}
+lmdb-rkv = { version = "0.14.0", optional = true }
+lmdb-rkv-sys = { version = "0.11", optional = true }
+time = {version="0.3",features=["parsing","formatting"]}
+parse-display = "0.6.0"
```

### Comparing `linkspace-0.1.4/local_dependencies/linkspace-common/LICENSE` & `linkspace-0.3.0rc2/local_dependencies/byte-fmt/LICENSE`

 * *Files identical despite different names*

### Comparing `linkspace-0.1.4/local_dependencies/linkspace-common/src/bus.rs` & `linkspace-0.3.0rc2/local_dependencies/linkspace-common/src/bus.rs`

 * *Files identical despite different names*

### Comparing `linkspace-0.1.4/local_dependencies/linkspace-common/src/cli/keys.rs` & `linkspace-0.3.0rc2/local_dependencies/linkspace-common/src/cli/keys.rs`

 * *Files 2% similar despite different names*

```diff
@@ -9,39 +9,39 @@
 use clap::Parser;
 
 use super::{opts::CommonOpts };
 
 #[derive(Parser, Clone, Debug)]
 pub struct KeyOpts {
     /// (abe) password argon2 encrypted signing key
-    #[clap(long, alias = "pass", env = "LINKSPACE_PASS")]
+    #[clap(long, alias = "pass", env = "LK_PASS")]
     password: Option<String>,
     /// print password - is always in abtxt format
     #[clap(long)]
     display_pass: bool,
     /// use utf8 encoding for password instead of ABE
     #[clap(short, long)]
     utf8_password: bool,
     /// local key name - e.g. my:home:local
-    #[clap(short, long, env = "LINKSPACE_KEY",default_value="me:local")]
+    #[clap(short, long, env = "LK_KEYNAME",default_value="me:local")]
     key: NameExpr,
     /// use specific enckey instead of looking for key. can be $argon str or (claim) hash
     #[clap(short, long)]
     enckey: Option<String>,
     #[clap(skip)]
     signing_key: std::sync::OnceLock<SigningKey>,
 }
 impl KeyOpts {
 
     pub fn enckey(&self, _common:&CommonOpts) ->anyhow::Result<Option<(PubKey,String)>>{
         let enckey = match &self.enckey {
             None => return Ok(None),
             Some(k) => k,
         };
-        if enckey.starts_with("$"){
+        if enckey.starts_with('$'){
             let pubkey = crate::identity::pubkey(enckey)?.into();
             return Ok(Some((pubkey,enckey.to_string())))
         };
         todo!()
     }
 
     pub fn identity<'i>(
@@ -154,15 +154,15 @@
     });
 
     let mut generate = |password: &[u8]| {
         let key = SigningKey::generate();
         no_check = true;
         encrypt(
             &key,
-            &password,
+            password,
             cost
         )
     };
     let print = |enckey,pubkey|{
         if !no_enckey {println!("{enckey}")};
         if !no_pubkey {println!("{pubkey}")};
     };
@@ -182,19 +182,19 @@
         }
     };
     tracing::debug!(?enckey);
     if new_pass || new_pass_str.is_some(){
         let keystr = enckey.context("new_pass but no --enckey found")?;
         let old_password = key.password_bytes_prompt(common, true,"old password: ")?;
         let skey = decrypt(&keystr, &old_password)?;
-        key.password = new_pass_str.clone();
+        key.password = new_pass_str;
         let new_password =key.password_bytes_prompt(common, true,"new password: ")?;
         key.password = Some(abtxt::as_abtxt(&new_password).to_string());
         key.utf8_password = false;
-        enckey = Some(encrypt(&skey, &new_password, cost));
+        enckey = Some(encrypt(&skey, &new_password, cost))
     }
 
     let rt = &common.runtime()?;
 
     if overwrite {
         let enckey = match user_enckey_input {
             true => {
@@ -210,15 +210,15 @@
                 generate(&password)
             }
         };
 
         let pubkey = if no_lk {
             B64(pubkey(&enckey)?)
         } else {
-            lns::setup_special_keyclaim(&rt, name, &enckey,true)?
+            lns::setup_special_keyclaim(rt, name, &enckey,true)?
         };
         print(enckey,pubkey);
         return Ok(());
     }
 
     if user_enckey_input && !no_lk{
         bail!("missing --overwrite to setup new enckey")
@@ -235,15 +235,14 @@
         }
         None => {
             let password = key.password_bytes_prompt(common, true,"generating new - password>")?;
             let enckey = generate(&password);
             let pubkey = if no_lk {
                 B64(pubkey(&enckey)?)
             }else{
-                lns::setup_special_keyclaim(&rt, name, &enckey,false)?
+                lns::setup_special_keyclaim(rt, name, &enckey,false)?
             };
             print(enckey,pubkey)
-            
         }
     }
     Ok(())
 }
```

### Comparing `linkspace-0.1.4/local_dependencies/linkspace-common/src/cli/opts.rs` & `linkspace-0.3.0rc2/local_dependencies/linkspace-common/src/cli/opts.rs`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 // Copyright Anton Sol
 //
 // This Source Code Form is subject to the terms of the Mozilla Public
 // License, v. 2.0. If a copy of the MPL was not distributed with this
 // file, You can obtain one at https://mozilla.org/MPL/2.0/.
 use std::{
-    io::{self, stdin, Stdin},
-    path::PathBuf,
+    io::{self },
+    path::PathBuf, 
 };
 
 use crate::{
     pkt_reader::NetPktDecoder,
     prelude::*,
     runtime::{handlers::PktStreamHandler, Linkspace},
 };
 use anyhow::Context;
 use clap::Parser;
+use linkspace_core::prelude::lmdb::BTreeEnv;
 
-use super::{write_pkt2, ReadSource, Reader, WriteDest, WriteDestSpec};
+use super::{write_pkt2, WriteDest, WriteDestSpec, reader::PktReadOpts};
 #[derive(Parser, Debug, Clone)]
 pub struct CommonOpts {
     #[clap(flatten)]
     pub linkspace: LinkspaceOpts,
     #[clap(flatten)]
     pub io: IOOpts,
 }
@@ -31,172 +32,165 @@
     }
 }
 #[derive(Parser, Debug, Clone)]
 pub struct LinkspaceOpts {
     #[clap(
         short,
         long,
-        env = "LINKSPACE",
-        help = "linkspace root - defaults to $HOME/linkspace"
+        env = "LK_DIR",
+        help = "location of the linkspace instance - defaults to $HOME/linkspace"
     )]
-    pub root: Option<PathBuf>,
+    pub dir: Option<PathBuf>,
     #[clap(
         long,
-        env = "LINKSPACE_INIT",
-        help = "create root if it does not exists"
+        env = "LK_INIT",
+        help = "create dir if it does not exists"
     )]
     pub init: bool,
+    #[clap(long,help="enable [env:OS_VAR] abe scope",default_value_t)]
+    pub env: bool,
 }
 impl LinkspaceOpts {
     pub fn root(&self) -> io::Result<PathBuf> {
-        crate::static_env::find_linkspace(self.root.as_deref())
+        crate::static_env::find_linkspace(self.dir.as_deref())
     }
     pub fn eval(&self, v: &str) -> anyhow::Result<ABList> {
         Ok(eval(&self.eval_ctx(), &parse_abe(v)?)?)
     }
     pub fn fake_eval_ctx(
     ) -> crate::eval::RTCtx<impl Fn() -> anyhow::Result<Linkspace> + Copy + 'static> {
-        crate::eval::std_ctx_v(|| anyhow::bail!("no linkspace instance "), EVAL0_1)
+        crate::eval::std_ctx_v(|| anyhow::bail!("no linkspace instance "), EVAL0_1,false)
     }
-    pub fn eval_ctx<'o>(
-        &'o self,
-    ) -> crate::eval::RTCtx<impl Fn() -> anyhow::Result<Linkspace> + Copy + 'o> {
-        crate::eval::std_ctx_v(|| self.runtime_io().context("could not open linkspace instance"), EVAL0_1)
+    pub fn eval_ctx(
+        &self,
+    ) -> crate::eval::RTCtx<impl Fn() -> anyhow::Result<Linkspace> + Copy + '_> {
+        crate::eval::std_ctx_v(|| self.runtime_io().context("could not open linkspace instance"), EVAL0_1,self.env)
     }
     pub fn keys_dir(&self) -> io::Result<PathBuf> {
         Ok(self.root()?.join("keys"))
     }
     pub fn runtime_io(&self) -> io::Result<Linkspace> {
-        crate::static_env::open_linkspace_root(self.root.as_deref(), self.init)
+        crate::static_env::open_linkspace_dir(self.dir.as_deref(), self.init)
     }
     pub fn runtime(&self) -> anyhow::Result<Linkspace> {
         self.runtime_io().context("error opening runtime")
     }
     pub fn env_io(&self) -> io::Result<&BTreeEnv> {
         crate::static_env::get_env(&self.root()?, self.init)
     }
     pub fn env(&self) -> anyhow::Result<&BTreeEnv> {
         self.env_io()
             .context("missing env. try opening with --init or set the --root")
     }
 }
 
-#[derive(Parser, Debug, Clone)]
+#[derive(Parser, Debug, Clone,Copy)]
 pub struct IOOpts {
     #[clap(
         global = true,
         alias = "private_group",
         long,
-        env = "PRIVATE_GROUP",
+        env = "LK_PRIVATE",
         help = "enable io of linkpoints in [#:0]"
     )]
     private: bool,
     #[clap(flatten)]
     pub inp: InOpts,
     #[clap(flatten)]
     pub out: OutOpts,
 }
 
-#[derive(Parser, Debug, Clone)]
+#[derive(Parser, Debug, Clone,Copy)]
 pub struct OutOpts {
     #[clap(
         long,
-        env = "WRITE_PRIVATE",
+        env = "LK_PRIVATE_WRITE",
         help = "enable output of linkpoints in [#:0]"
     )]
-    write_private: Option<bool>,
+    private_write: Option<bool>,
 }
-#[derive(Parser, Debug, Clone, Copy)]
+#[derive(Parser, Debug, Clone,Copy )]
 pub struct InOpts {
     #[clap(
         long,
-        env = "READ_PRIVATE",
+        env = "LK_PRIVATE_READ",
         help = "enable input of linkpoints in [#:0]"
     )]
-    pub(crate) read_private: Option<bool>,
+    pub(crate) private_read: Option<bool>,
     #[clap(
         long,
-        env = "LINKSPACE_HOP",
+        env = "LK_HOP",
         help = "toggle hop netheader incr. true for commands unless stated otherwise"
     )]
     pub(crate) hop: Option<bool>,
     #[clap(
         long,
-        env = "LINKSPACE_NO_CHECK",
+        env = "LK_SKIP_HASH",
         help = "skip validating hashes and signatures"
     )]
-    pub no_check: bool,
+    pub skip_hash: bool,
 }
 impl InOpts {
     pub fn pkt_reader<P: std::io::Read>(self, reader: P) -> NetPktDecoder<P> {
         NetPktDecoder {
-            allow_private: self.read_private.unwrap_or(false),
+            allow_private: self.private_read.unwrap_or(false),
             reader,
             hop: self.hop.unwrap_or(true),
-            validate: !self.no_check,
+            skip_hash: self.skip_hash,
         }
     }
 }
 
 impl CommonOpts {
     pub fn default_hop(&mut self) {
         self.io.inp.hop.get_or_insert(true);
     }
     pub fn enable_private_group(&mut self) {
         self.io.private = true;
-        self.io.inp.read_private = Some(true);
-        self.io.out.write_private = Some(true)
+        self.io.inp.private_read = Some(true);
+        self.io.out.private_write = Some(true)
     }
     pub fn mut_write_private(&mut self) -> &mut Option<bool> {
-        &mut self.io.out.write_private
+        &mut self.io.out.private_write
     }
     pub fn mut_read_private(&mut self) -> &mut Option<bool> {
-        &mut self.io.inp.read_private
+        &mut self.io.inp.private_read
     }
     pub fn write_private(&self) -> Option<bool> {
         if self.io.private {
             Some(true)
         } else {
-            self.io.out.write_private
+            self.io.out.private_write
         }
     }
     pub fn read_private(&self) -> Option<bool> {
         if self.io.private {
             Some(true)
         } else {
-            self.io.inp.read_private
+            self.io.inp.private_read
         }
     }
-    pub fn check_private(&self, pkt: impl NetPkt) -> Option<impl NetPkt> {
+    pub fn check_private<S:NetPkt>(&self, pkt:S ) -> Result<S,linkspace_pkt::Error> {
         let write_private = self.write_private().unwrap_or(false);
-        if !write_private && pkt.as_point().group() == Some(&PRIVATE) {
-            tracing::warn!(pkt=%pkt_fmt(&pkt),"Skip writing private (null) group");
-            return None;
-        }
-        Some(pkt)
+        if !write_private { pkt.check_private().map_err(|e| {tracing::warn!(?e,pkt=%PktFmt(&pkt),"enable private writing");e})?}
+        Ok(pkt)
     }
     pub fn open(&self, lst: &[WriteDestSpec]) -> std::io::Result<Vec<WriteDest>> {
         let ctx = self.eval_ctx();
         lst.iter()
             .filter_map(|v| v.open(&ctx).transpose())
             .try_collect()
     }
-    pub fn open_read(&self, r: Option<&ReadSource>) -> anyhow::Result<Reader> {
-        ReadSource::into_reader(r, self.io.inp, &self.eval_ctx())
-    }
     pub fn write_dest(
         &self,
         dest: &mut WriteDest,
         pkt: &dyn NetPkt,
         buffer: &mut Option<&mut dyn std::io::Write>,
     ) -> std::io::Result<()> {
-        let pkt = match self.check_private(pkt) {
-            Some(p) => p,
-            None => return Ok(()),
-        };
+        let pkt = self.check_private(pkt).map_err(linkspace_pkt::Error::io)?;
         let out: &mut dyn std::io::Write = match &mut dest.out {
             super::Out::Db => {
                 return save_pkt(&mut self.linkspace.env_io()?.get_writer()?, pkt).map(|_| ())
             }
             super::Out::Fd(f) => f,
             super::Out::Buffer => buffer
                 .as_mut()
@@ -207,15 +201,15 @@
 
     pub fn write_multi_dest(
         &self,
         mdest: &mut [WriteDest],
         pkt: &dyn NetPkt,
         mut buffer: Option<&mut dyn std::io::Write>,
     ) -> std::io::Result<()> {
-        let _ = tracing::debug_span!("Writing",pkt=%pkt_fmt(pkt)).entered();
+        let _ = tracing::debug_span!("Writing",pkt=%PktFmt(pkt)).entered();
         for dest in mdest.iter_mut() {
             self.write_dest(dest, pkt, &mut buffer)?;
         }
         tracing::debug!("finish writing");
         Ok(())
     }
 
@@ -224,24 +218,25 @@
         move |p: &dyn NetPkt, _rx: &Linkspace| -> std::io::Result<()> {
             this.write_multi_dest(&mut mdest, p, None)?;
             Ok(())
         }
     }
     pub fn stdout_writer(&self) -> impl PktStreamHandler {
         let allow_private = self.write_private().unwrap_or(false);
-        tracing::trace!(allow_private);
         let mut out = std::io::stdout();
         let ctx = self.clone();
         move |p: &dyn NetPkt, _rx: &Linkspace| -> std::io::Result<()> {
+            if!allow_private{p.check_private().map_err(|e|e.io())?}
             write_pkt2(&None, p, &ctx.eval_ctx(), &mut out)
         }
     }
-    pub fn inp_reader(&self) -> io::Result<NetPktDecoder<Stdin>> {
-        let inp = stdin(); // Do not buffer. cli like handshake must not buffer partial packets and have  subsequent programs fail
+    pub fn inp_reader(&self,inp: &PktReadOpts) -> io::Result<NetPktDecoder<Box<dyn std::io::Read>>> {
+        // Do not buffer. cli like handshake must not buffer partial packets and have  subsequent programs fail
+        let reader = inp.open()?.expect("bug: - should be empty reader").into_read();
         Ok(NetPktDecoder {
+            reader,
             allow_private: self.read_private().unwrap_or(false),
-            reader: inp,
             hop: self.io.inp.hop.unwrap_or_default(),
-            validate: !self.io.inp.no_check,
+            skip_hash: self.io.inp.skip_hash,
         })
     }
 }
```

### Comparing `linkspace-0.1.4/local_dependencies/linkspace-common/src/dgp.rs` & `linkspace-0.3.0rc2/local_dependencies/linkspace-common/src/dgp.rs`

 * *Files 16% similar despite different names*

```diff
@@ -36,15 +36,15 @@
             path: SPathExpr::from_unchecked(dgp.path.to_abe()),
         };
         debug_assert_eq!(self.eval(ctx).unwrap(), dgp);
         Ok(dgp)
     }
     pub fn eval(&self, ctx: &EvalCtx<impl Scope>) -> anyhow::Result<DGP> {
         let domain = self.domain.eval(ctx);
-        let group = self.group.eval_default(PUBLIC, ctx);
+        let group = self.group.eval(ctx);
         let path = self.path.eval(ctx)?.try_ipath();
         match (domain, group, path) {
             (Ok(domain), Ok(group), Ok(path)) => Ok(DGP {
                 domain,
                 group,
                 path,
             }),
@@ -134,21 +134,18 @@
 pub struct DGPDExpr {
     pub dgp: DGPExpr,
     pub subsegment_limit: u8,
 }
 impl DGPDExpr {
     pub fn predicate_exprs(self) -> anyhow::Result<impl Iterator<Item = Vec<ABE>>> {
         let mut prefix_rule = None;
-        if self.subsegment_limit != MAX_PATH_LEN as u8{
-            if !self.dgp.path.is_empty() && !self.dgp.path.0.iter().any(|v| v.is_fslash()) {
-                anyhow::bail!("can't use subrange expr with an evaluated spath ( dont know its length ).
-Must add ':**' and manually set -- path_len ...")
-            }
-        }
-
+        if self.subsegment_limit != MAX_PATH_LEN as u8 && !self.dgp.path.is_empty() && !self.dgp.path.0.iter().any(|v| v.is_fslash()) {
+                        anyhow::bail!("can't use subrange expr with an evaluated spath ( dont know its length ).
+        Must add ':**' and manually set -- path_len ...")
+                    }
 
         if self.subsegment_limit < MAX_PATH_LEN as u8 {
             let prefix_len = self
                 .dgp
                 .path
                 .0
                 .iter()
@@ -161,31 +158,23 @@
         Ok(self.dgp.as_test_exprs().chain(prefix_rule))
     }
 }
 
 pub fn try_take_dgp(ast: &[ABE]) -> anyhow::Result<(DGPExpr, &[ABE])> {
     use abe::*;
     let mut it = ast.split(|v| matches!(v, ABE::Ctr(Ctr::Colon)));
-    let mut domain = it
-        .next()
-        .map(|v| v.try_into())
-        .transpose()?
-        .unwrap_or(default_domain_expr());
-    if domain.is_empty() {
-        domain = default_domain_expr();
-    }
-    let mut group = it
-        .next()
-        .map(|v| v.try_into())
-        .transpose()?
-        .unwrap_or(default_group_expr());
-    if group.is_empty() {
-        group = default_group_expr();
-    }
 
+    let domain = match it.next().unwrap_or(&[]){
+        &[] => TypedABE::from_unchecked(crate::static_env::domain().to_abe()),
+        v => v.try_into()?,
+    };
+    let group = match it.next().unwrap_or(&[]){
+        &[] => TypedABE::from_unchecked(crate::static_env::group().to_abe()),
+        v => v.try_into()?
+    };
     let path = it.next().unwrap_or_default().try_into()?;
     Ok((
         DGPExpr {
             domain,
             group,
             path,
         },
@@ -222,19 +211,26 @@
     use abe::ast::*;
     let ([e], rest) = match take(ast) {
         Ok(e) => e,
         Err(_) => return Ok((0, &[])),
     };
     let depth = match as_expr(e)? {
         Expr::Bytes(s) => {
-            if s == b"*" {
-                1
-            } else if s == b"**" {
-                MAX_PATH_LEN as u8
-            } else {
-                bail!("??")
+            match s.as_slice() {
+                b"0" => 0,
+                b"1" => 1,
+                b"2" => 2,
+                b"3" => 3,
+                b"4" => 4,
+                b"5" => 5,
+                b"6" => 6,
+                b"7" => 7,
+                b"8" => 8,
+                b"*" => 1,
+                b"**" => MAX_PATH_LEN as u8,
+                _e => bail!("{} is an invalid depth",e)
             }
         }
         Expr::Lst(_) => bail!("todo"),
     };
     Ok((depth, rest))
 }
```

### Comparing `linkspace-0.1.4/local_dependencies/linkspace-common/src/eval.rs` & `linkspace-0.3.0rc2/local_dependencies/linkspace-common/src/eval.rs`

 * *Files 13% similar despite different names*

```diff
@@ -1,92 +1,97 @@
-use anyhow::Context;
 // Copyright Anton Sol
 //
 // This Source Code Form is subject to the terms of the Mozilla Public
 // License, v. 2.0. If a copy of the MPL was not distributed with this
 // file, You can obtain one at https://mozilla.org/MPL/2.0/.
+use std::{ffi::OsStr, os::unix::prelude::OsStrExt};
+
+use anyhow::Context;
+
 use linkspace_core::prelude::*;
 /// Various ABE eval Scope's with database access.
 
 use crate::{
-    runtime::Linkspace, protocols::lns::eval::{NetLNS, PrivateLNS},
+    runtime::Linkspace, protocols::lns::eval::{NetLNS, PrivateLNS}, 
 };
 pub trait LKS  where Self: Fn() -> anyhow::Result<Linkspace> + Sized + Copy{
     fn lk(self) -> anyhow::Result<Linkspace>{ (self)()}
 }
 impl<F> LKS for F where F: Fn() -> anyhow::Result<Linkspace>+Copy{
     fn lk(self) -> anyhow::Result<Linkspace> {
         (self)()
     }
 }
 
 pub type RTScope<GT> = (
     EScope<NetLNS<GT>>,
     EScope<PrivateLNS<GT>>,
-    (EScope<FileEnv<GT>>, EScope<ReadHash<GT>>),
+    (EScope<FileEnv<GT>>, EScope<ReadHash<GT>>,Option<EScope<OSEnv>>),
 );
 pub type RTCtx<GT> = EvalCtx<(EvalStd, RTScope<GT>)>;
 
-pub const fn rt_scope<'o, GT>(rt: GT) -> RTScope<GT>
+pub const fn rt_scope<'o, GT>(rt: GT,enable_env:bool) -> RTScope<GT>
 where
     GT: 'o + LKS
 {
-    let env = EScope(FileEnv(rt));
+    let files= EScope(FileEnv(rt));
     let readhash = EScope(ReadHash(rt));
     let local_lns = EScope(PrivateLNS { rt });
+    let env = if enable_env{ Some(EScope(OSEnv))} else {None};
     let lns = EScope(NetLNS {
         rt,
         timeout: std::time::Duration::from_secs(1),
     });
-    (lns, local_lns, (env, readhash))
+    (lns, local_lns, (files, readhash,env))
 }
 pub fn rt_ctx<'o, GT>(
     ctx: EvalCtx<impl Scope + 'o>,
     rt: GT,
+    enable_env:bool
 ) -> EvalCtx<(impl Scope + 'o, RTScope<GT>)>
 where
     GT: 'o + LKS
 {
-    ctx.scope(rt_scope(rt))
+    ctx.scope(rt_scope(rt,enable_env))
 }
 
-pub const fn std_ctx_v<'o, GT>(rt: GT, version: &str) -> RTCtx<GT>
+pub const fn std_ctx_v<'o, GT>(rt: GT, version: &str,enable_env:bool) -> RTCtx<GT>
 where
     GT: 'o + LKS
 {
     EvalCtx {
-        scope: (linkspace_core::eval::std_ctx_v(version).scope, rt_scope(rt)),
+        scope : (linkspace_core::eval::std_ctx_v(version).scope, rt_scope(rt,enable_env)),
     }
 }
 
 #[derive(Copy, Clone)]
 pub struct FileEnv<R>(R);
 
 impl<R: LKS> EvalScopeImpl for FileEnv<R> {
     fn about(&self) -> (String, String) {
         (
             "filesystem env".into(),
             format!(
-                "read files from {:?} ",
-                self.0.lk().map(|v| v.env().location().to_owned())
+                "read files from {:?}/files ",
+                self.0.lk().map(|v| v.env().dir().to_owned())
             ),
         )
     }
     fn list_funcs(&self) -> &[ScopeFunc<&Self>] {
         &[ScopeFunc {
             apply: |this: &Self, inp: &[&[u8]], _, _scope| {
                 let p = std::str::from_utf8(inp[0])?;
-                Ok(this.0.lk()?.env().env_data(p,true)?.unwrap()).into()
+                Ok(this.0.lk()?.env().files_data(p,true)?.unwrap()).into()
             },
             info: ScopeFuncInfo {
-                id: "conf",
+                id: "files",
                 init_eq: None,
                 argc: 1..=1,
                 to_abe: false,
-                help: "read a file from the conf directory",
+                help: "read a file from the LK_DIR/files directory",
             },
             to_abe: none,
         }]
     }
 }
 
 #[derive(Copy, Clone)]
@@ -118,16 +123,15 @@
         let predicates = Query::dgpk(domain, group, path, key).predicates;
         let pkt = reader
             .query_tree(query_mode::Order::Desc, &predicates)
             .next()
             .context("no matching packet")?;
         let id = inp.get(4).copied().unwrap_or(b"pkt");
         let args = inp.get(5..).unwrap_or(&[]);
-        let r = pkt_scope(&*pkt).lookup_apply(id, args, true, scope);
-        drop(pkt);
+        let r = pkt_scope(&*pkt).try_apply_func(id, args, true, scope);
         drop(reader);
         match r.into_opt() {
             Some(o) => o,
             None => Err(EvalError::NoSuchFunc(id.to_vec()).into()),
         }
     }
 }
@@ -142,48 +146,48 @@
         &[
             ScopeFunc {
                 apply : |this:&Self,inp:&[&[u8]],_,scope|{
                     let hash = B64::try_fit_slice(inp[0])?;
                     let reader = this.0.lk()?.get_reader();
                     let pkt = reader.read(&hash)?.with_context(||format!("could not find pkt {}",hash))?;
                     let (id, args) = inp[1..].split_first().unwrap_or((&{b"pkt" as &[u8]},&[]));
-                    let r = pkt_scope(&*pkt).lookup_apply(id, args, true,scope);
-                    drop(pkt); drop(reader);
+                    let r = pkt_scope(&*pkt).try_apply_func(id, args, true,scope);
+                    drop(reader);
                     r
                 },
                 info: ScopeFuncInfo {
                     id:  "readhash", init_eq: None, argc: 1..=16,to_abe:false,
                     help:"open a pkt by hash and use tail args as if calling in a netpkt scope"
                 },
                 to_abe:none
             },
             ScopeFunc {
                 apply : |this:&Self,inp:&[&[u8]],_,scope|{
                     this.read_dgpk(inp, scope).into()
                 },
                 info: ScopeFuncInfo {
                     id:  "read", init_eq: None, argc: 2..=16,to_abe:false,
-                    help:"read but accesses open a pkt by dgpk path and apply args. e.g. [read:mydomain:[#:pub]:[//a/path]:[@:me]::data:str], prefer eval ctx"
+                    help:"read but accesses open a pkt by dgpk path and apply args. e.g. [read:mydomain:[#:pub]:[//a/path]:[@:me]::data:str] - does not use default group/domain - prefer eval ctx"
                 },
                 to_abe:none
             },
         ]
     }
-    fn list_eval(&self) -> &[ScopeEval<&Self>] {
-        &[ScopeEval {
+    fn list_macros(&self) -> &[ScopeMacro<&Self>] {
+        &[ScopeMacro {
             apply: |this, abe: &[ABE], scope| {
                 let ctx = EvalCtx { scope };
                 let mut it = abe.split(|v| v.is_colon());
                 let _empty = it.next().context("arg delimited with ':'")?;
                 ast::exact::<0>(_empty)?;
                 let hash = it.next().context("missing hash")?;
                 let expr = it.next().context("missing expr")?;
                 let alt = it.next();
                 let hash = eval(&ctx, hash)?.concat();
-                let hash: Ptr = Ptr::try_fit_slice(&hash)?;
+                let hash: LkHash = LkHash::try_fit_slice(&hash)?;
                 let reader = this.0.lk()?.get_reader();
                 match reader.read(&hash)? {
                     None => {
                         let alt = alt.with_context(|| format!("could not find pkt {}", hash))?;
                         it.next().context("to many args?")?;
                         let r = eval(&ctx, alt)?.concat();
                         ApplyResult::Value(r)
@@ -191,14 +195,45 @@
                     Some(pkt) => {
                         let r = eval(&pkt_ctx(ctx, &pkt), expr)?.concat();
                         //drop(pkt); drop(reader);
                         ApplyResult::Value(r)
                     }
                 }
             },
-            info: ScopeEvalInfo {
+            info: ScopeMacroInfo {
                 id: "readhash",
                 help: "HASH ':' expr (':' alt if not found) ",
             },
         }]
     }
 }
+
+#[derive(Copy, Clone)]
+pub struct OSEnv;
+
+impl EvalScopeImpl for OSEnv{
+    fn about(&self) -> (String, String) {
+        (
+            "env".into(),
+            "os environment variables".into()
+        )
+    }
+    fn list_funcs(&self) -> &[ScopeFunc<&Self>] {
+        &[ScopeFunc {
+            apply: |_this: &Self, inp: &[&[u8]], _, _scope| {
+                let st : &OsStr = OsStr::from_bytes(inp[0]); // TODO this might be wrong
+                std::env::var_os(st)
+                    .with_context(|| format!("{st:?} env variable not set"))
+                    .map(|o| o.as_bytes().to_vec())
+                    .into()
+            },
+            info: ScopeFuncInfo {
+                id: "env",
+                init_eq: None,
+                argc: 1..=1,
+                to_abe: false,
+                help: "read the raw OS environment variables as bytes",
+            },
+            to_abe: none,
+        }]
+    }
+}
```

### Comparing `linkspace-0.1.4/local_dependencies/linkspace-common/src/pkt_reader.rs` & `linkspace-0.3.0rc2/local_dependencies/linkspace-common/src/pkt_reader.rs`

 * *Files 9% similar despite different names*

```diff
@@ -10,32 +10,30 @@
 
 #[derive(Error, Debug)]
 pub enum Error {
     #[error("Pkt Error")]
     Pkt(#[from] linkspace_core::pkt::Error),
     #[error("Io Error")]
     IO(#[from] IoError),
-    #[error("private null group not allowed in this context")]
-    PrivateGroup,
 }
 
 #[derive(Debug)]
 pub struct NetPktDecoder<T> {
     pub allow_private: bool,
     pub reader: T,
     pub hop: bool,
-    pub validate: bool,
+    pub skip_hash: bool,
 }
 impl<T> NetPktDecoder<T> {
     pub fn new(reader: T) -> Self {
         NetPktDecoder {
             allow_private: false,
             reader,
             hop: true,
-            validate: true,
+            skip_hash: false,
         }
     }
 }
 
 
 
 impl<T: Read> Iterator for NetPktDecoder<T> {
@@ -64,35 +62,31 @@
                     Err(ref e) if e.kind() == ErrorKind::UnexpectedEof => return None,
                     //Err(ref e) if e.kind() == ErrorKind::Interrupted && buf.len() == UPTO_PKT_SIZE => {return None}
                     Err(e) => return Some(Err(Error::IO(e))),
                 }
             }
         }
         try_opt!(partial_header.point_header.check());
-        let len = partial_header.point_header.net_pkt_size();
+        let len = partial_header.point_header.size();
         let mut pkt = unsafe { partial_header.alloc() };
         {
             let s: &mut [u8] = unsafe {
-                std::slice::from_raw_parts_mut((&mut *pkt) as *mut NetPktFatPtr as *mut u8, len)
+                std::slice::from_raw_parts_mut((&mut *pkt) as *mut NetPktFatPtr as *mut u8, len as usize)
             };
             tracing::trace!("Read rest");
             let r = self
                 .reader
                 .read_exact(&mut s[std::mem::size_of::<PartialNetHeader>()..]);
             try_opt!(r);
         };
-
-        let check = if self.validate {
-            pkt.check::<true>()
-        } else {
-            pkt.check::<false>()
-        };
-        try_opt!(check);
-        if !self.allow_private && pkt.group() == Some(&PRIVATE) {
-            return Some(Err(Error::PrivateGroup));
+        try_opt!(pkt.check(self.skip_hash));
+        if !self.allow_private{
+            if let Err(e) = pkt.check_private(){
+                return Some(Err(Error::Pkt(e)));
+            }
         }
         if self.hop {
             let head = &mut pkt._net_header;
             *head = head.hop();
         }
         Some(Ok(pkt))
     }
```

### Comparing `linkspace-0.1.4/local_dependencies/linkspace-common/src/pkt_stream_utils.rs` & `linkspace-0.3.0rc2/local_dependencies/linkspace-common/src/pkt_stream_utils.rs`

 * *Files 5% similar despite different names*

```diff
@@ -27,15 +27,15 @@
                     vec![pkt]
                 } else {
                     self.forward_buf.push(pkt);
                     vec![]
                 }
             }
             Some(links) => {
-                self.latest_links = links.into_iter().map(|r| r.ptr).collect();
+                self.latest_links = links.iter().map(|r| r.ptr).collect();
                 //self.forward_buf.drain(..).filter(|v| self.latest_links.remove(&v.hash())).chain(pkt).collect()
                 let (mut unlocked, dropped): (Vec<_>, Vec<_>) = self
                     .forward_buf
                     .drain(..)
                     .partition(|v| self.latest_links.contains(v.hash_ref()));
                 unlocked.push(pkt);
                 if dropped.is_empty() {
```

### Comparing `linkspace-0.1.4/local_dependencies/linkspace-common/src/predicate_aliases.rs` & `linkspace-0.3.0rc2/local_dependencies/linkspace-common/src/predicate_aliases.rs`

 * *Files 4% similar despite different names*

```diff
@@ -21,55 +21,55 @@
     #[clap(last = true)]
     pub exprs: Vec<AnyABE>,
 }
 
 #[derive(Debug, Clone, Default, Args)]
 /// aliases for a set of common predicates
 pub struct PredicateAliases {
-    /// only match locally indexed pkts           | i_new:=:{u32:0}
+    /// only match locally indexed pkts           | i_new:=:[u32:0]
     #[clap(long, alias = "no-new")]
     pub index: bool,
-    /// only match new unindexed pkts             | i_index:=:{u32:0}
-    #[clap(long, alias = "no-index")]
+    /// only match new unindexed pkts             | i_db:=:[u32:0]
+    #[clap(long, alias = "no-db")]
     pub new: bool,
 
-    /// match upto max packets.                   | i:<:{u32:max}
+    /// match upto max packets.                   | i:<:[u32:max]
     #[clap(long)]
     pub max: Option<u32>,
 
-    /// match upto max per (dm,grp,path,key) pkts | i:<:{u32:max_branch}
+    /// match upto max per (dm,grp,path,key) pkts | i_branch:<:[u32:max_branch]
     #[clap(long)]
     pub max_branch: Option<u32>,
-    /// match upto max from local index           | i_index:<:{u32:max_index}
+    /// match upto max from local index           | i_db:<:[u32:max_index]
     #[clap(long)]
     pub max_index: Option<u32>,
-    /// match upto max unindexed pkts             | i_new:<:{u32:max_new}
+    /// match upto max unindexed pkts             | i_new:<:[u32:max_new]
     #[clap(long)]
     pub max_new: Option<u32>,
 
-    /// match only signed pkts                    | pubkey:>:{@:none}
+    /// match only signed pkts                    | pubkey:>:[@:none]
     #[clap(long, conflicts_with = "unsigned")]
     pub signed: bool,
 
-    /// match only unsigned pkts                  | pubkey:=:{@:none}
+    /// match only unsigned pkts                  | pubkey:=:[@:none]
     #[clap(long)]
     pub unsigned: bool,
 
     #[clap(long)]
-    /// Add :id option
+    /// Add :qid option (generates qid)
     pub watch: bool,
     #[clap(long)]
-    /// set :id option id (implies --watch)
-    pub watch_id: Option<AnyABE>,
+    /// set :qid option (implies --watch)
+    pub qid: Option<AnyABE>,
     #[clap(long)]
     /// Add :follow option
     pub follow: bool,
 
     #[clap(long)]
-    /// add recv:<:{now:+..} 
+    /// add recv:<:[now:+..] 
     pub ttl : Option<String>
 }
 
 impl PredicateAliases {
     // TODO use PredicateType instead of RuleType
     pub fn as_predicates(self) -> impl Iterator<Item = Vec<ABE>> {
         let PredicateAliases {
@@ -78,15 +78,15 @@
             unsigned,
             index,
             new,
             max_branch,
             max_index,
             max_new,
             watch,
-            watch_id,
+            qid,
             follow,
             ttl,
         } = self;
         let signed = signed
             .then(||
                   abev!((PktTypeF::NAME) : "1" : +(U8::new(PointTypeFlags::SIGNATURE.bits()).abe_bits()))
             );
@@ -103,18 +103,18 @@
         let max_branch = max_branch
             .map(|i| abev!( (QScope::Branch.to_string()) : "<" : +(U32::from(i).to_abe())));
 
 
         let new = new.then(|| abev!( (QScope::Index.to_string()) : "<" : +(U32::ZERO.to_abe())));
         let log = index.then(|| abev!( (QScope::New.to_string()) : "<" : +(U32::ZERO.to_abe())));
 
-        let watch = watch_id.map(|v| v.unwrap()).or(watch.then(|| abev!("default")))
-            .map(|v| abev!( : (KnownOptions::Id.to_string()) : +(v)).into());
+        let watch = qid.map(|v| v.unwrap()).or(watch.then(|| abev!("default")))
+            .map(|v| abev!( : (KnownOptions::Qid.to_string()) : +(v)));
 
-        let ttl = ttl.map(|v| abev!( (PredicateType::Recv.to_string()) : "<" : { "now" : "+" v}).into());
+        let ttl = ttl.map(|v| abev!( (PredicateType::Recv.to_string()) : "<" : { "now" : "+" v}));
 
         let follow = follow.then(|| abev!(: (KnownOptions::Follow.to_string())));
 
         watch.into_iter()
             .chain(ttl)
             .chain(follow)
             .chain(signed)
```

### Comparing `linkspace-0.1.4/local_dependencies/linkspace-common/src/protocols/handshake.rs` & `linkspace-0.3.0rc2/local_dependencies/linkspace-common/src/protocols/handshake.rs`

 * *Files 2% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 // This Source Code Form is subject to the terms of the Mozilla Public
 // License, v. 2.0. If a copy of the MPL was not distributed with this
 // file, You can obtain one at https://mozilla.org/MPL/2.0/.
 /// basic response-reply proving each side can sign with a key
 use std::time::Duration;
 
 use crate::{prelude::*, protocols::unicast_group};
-use anyhow::ensure;
+use anyhow::{ensure };
 pub const HANDSHAKE_D: Domain = ab(b"\xFFhandshake");
 
-pub const ID_SENTINAL_SPATH : IPathC<17>= ipath1(b"sentinal");
-pub const ANONYMOUSE_SPATH : IPathC<18>= ipath1(b"anonymous");
+pub const ID_SENTINAL_SPATH : IPathC<17>= ipath1::<8>(b"sentinal");
+pub const ANONYMOUSE_SPATH : IPathC<18>= ipath1::<9>(b"anonymous");
 
 const MAX_DIFF_SECONDS: usize = 15;
 pub fn valid_stamp_range(stamp: Stamp, max_diff_sec: Option<usize>) -> anyhow::Result<()> {
     let dur = Duration::from_secs(max_diff_sec.unwrap_or(MAX_DIFF_SECONDS) as u64);
     match stamp_age(stamp) {
         Ok(d) => ensure!(
             d < dur,
@@ -34,21 +34,21 @@
 pub struct Phase2(pub NetPktBox);
 pub struct Phase3(pub NetPktBox);
 pub fn phase0_client_init(id: &SigningKey) -> Phase0 {
     tracing::trace!("Build phase0");
     let now = now();
     Phase0(
         keypoint(
-            id.pubkey().into(),
+            id.pubkey(),
             HANDSHAKE_D,
             &ID_SENTINAL_SPATH,
             &[],
             &[],
             now,
-            &id,
+            id,
             ()
         )
         .as_netbox(),
     )
 }
 pub fn phase1_server_signs(
     theirs: &Phase0,
@@ -63,39 +63,40 @@
         theirs.net_header()
     );
     let their_key = match theirs.pubkey() {
         Some(their_key) => *their_key,
         None => anyhow::bail!("not signed"),
     };
     valid_stamp_range(*theirs.get_create_stamp(), max_diff_sec)?;
-    let our_group = unicast_group(their_key, id.pubkey().into());
+    let our_group = unicast_group(their_key, id.pubkey());
+    ensure!(our_group != PRIVATE,"Connecting to yourself (using the same key) is currently not supported");
     let links = [Link::new("auth", *theirs.hash())];
     Ok(Phase1(
         keypoint(
             our_group,
             HANDSHAKE_D,
             &ID_SENTINAL_SPATH,
             &links,
             &[],
             now(),
-            &id,
+            id,
             (),
         )
         .as_netbox(),
     ))
 }
 pub fn phase2_client_signs(
     my_phase0: &Phase0,
     server_reply: &Phase1,
     id: &SigningKey,
     max_diff_sec: Option<usize>,
 ) -> anyhow::Result<(Phase2, PubKey)> {
     tracing::trace!("Build Phase2");
     ensure!(
-        my_phase0.0.pubkey() == Some(&id.pubkey().into()),
+        my_phase0.0.pubkey() == Some(&id.pubkey()),
         "identity mismatch"
     );
     let mine_hash = my_phase0.0.hash();
     let theirs = &server_reply.0;
     assert!(
         theirs.net_header().hop.get() > 0,
         "the rx channel is not calling net_header.hop() {:?}",
@@ -111,15 +112,15 @@
         "did not validate my hash {}",
         mine_hash
     );
     ensure!(
         theirs.domain() == Some(&HANDSHAKE_D),
         "not in the session domain"
     );
-    let our_group = unicast_group(id.pubkey().into(), their_key);
+    let our_group = unicast_group(id.pubkey(), their_key);
     ensure!(
         theirs.group() == Some(&our_group),
         "not in the right group "
     );
     ensure!(
         theirs.get_ipath() == ID_SENTINAL_SPATH.as_ref(),
         "wrong spath "
@@ -128,40 +129,40 @@
     let proof = keypoint(
         our_group,
         HANDSHAKE_D,
         &ID_SENTINAL_SPATH,
         &[Link::new("signed", *theirs.hash())],
         &[],
         now,
-        &id,
+        id,
         ()
     )
     .as_netbox();
     Ok((Phase2(proof), their_key))
 }
 pub fn phase3_server_verify(
     their_init: &Phase0,
     my_phase1: &Phase1,
     theirs: &Phase2,
     id: &SigningKey,
 ) -> anyhow::Result<PubKey> {
     ensure!(
-        my_phase1.0.pubkey() == Some(&id.pubkey().into()),
+        my_phase1.0.pubkey() == Some(&id.pubkey()),
         "your identity mismatch"
     );
     let theirs = theirs.0.as_netbox();
     let mine_hash = my_phase1.0.hash();
     let their_key = match theirs.pubkey() {
         Some(p) => {
             ensure!(theirs.pubkey() == their_init.0.pubkey(), "switched keys");
             *p
         }
         None => anyhow::bail!("hello pkt not signed"),
     };
-    let our_group = unicast_group(id.pubkey().into(), their_key);
+    let our_group = unicast_group(id.pubkey(), their_key);
     ensure!(
         theirs.get_links().iter().any(|r| r.ptr == mine_hash),
         "did not validate my hash {}",
         mine_hash
     );
     ensure!(
         theirs.get_ipath() == ID_SENTINAL_SPATH.as_ref(),
```

### Comparing `linkspace-0.1.4/local_dependencies/linkspace-common/src/protocols/impex/blob.rs` & `linkspace-0.3.0rc2/local_dependencies/linkspace-common/src/protocols/impex/blob.rs`

 * *Files 5% similar despite different names*

```diff
@@ -2,16 +2,21 @@
 //
 // This Source Code Form is subject to the terms of the Mozilla Public
 // License, v. 2.0. If a copy of the MPL was not distributed with this
 // file, You can obtain one at https://mozilla.org/MPL/2.0/.
 use anyhow::{self};
 use linkspace_core::{crypto::blake3, prelude::*};
 
-// This is completely made up. No testing was done.
-pub const MMAP_IF_LARGER_THEN: u64 = 1 << 26;
+pub static LK_MMAP_FILE_SIZE : std::sync::OnceLock<u64> = OnceLock::new();
+pub fn should_mmap(file_size:u64) -> bool {
+    let min_mmap_size = *LK_MMAP_FILE_SIZE.get_or_init(|| {
+        std::env::var("LK_MMAP_FILE_SIZE").ok().and_then(|v|v.parse().ok()).unwrap_or(u64::MAX)
+    });
+    min_mmap_size <= file_size
+}
 pub static EMPTY_DATA_PKT : LazyLock<NetPktBox> = LazyLock::new(||datapoint(b"", NetPktHeader::EMPTY).as_netbox());
 pub static EMPTY_DATA_HASH : LazyLock<LkHash> = LazyLock::new(|| EMPTY_DATA_PKT.hash());
 //spath!(pub const BLOB_SP = [b"\0blob"]);
 pub const BLOB_SP: ConstSPath<6> = ConstSPath::from_raw(*b"\x05\0blob");
 
 use thiserror::Error;
 
@@ -26,31 +31,30 @@
     #[error("Other Err {0}")]
     Other(anyhow::Error),
 }
 
 pub use std::path::Path;
 use std::{
     io::IoSlice,
-    ops::{FromResidual, Try}, sync::LazyLock,
+    ops::{FromResidual, Try}, sync::{LazyLock, OnceLock}, 
 };
 
 pub fn datapkt_path_reader<F, R>(path: &Path, netopts: impl Into<NetOpts>, f: F) -> R
 where
     F: FnMut(NetPktParts) -> R,
     R: Try<Output = ()> + FromResidual<Result<std::convert::Infallible, std::io::Error>>,
 {
     let file = std::fs::File::open(path)?;
     let meta = file.metadata()?;
-    match meta.len() {
-        0..=MMAP_IF_LARGER_THEN => datapkt_io_reader(file, netopts, f),
-        _ => {
-            let mmap = unsafe { memmap2::Mmap::map(&file)? };
-            let bytes = mmap.as_ref();
-            datapkt_buf_reader(bytes, netopts, f)
-        }
+    if !should_mmap(meta.len()){
+        datapkt_io_reader(file, netopts, f)
+    }else {
+        let mmap = unsafe { memmap2::Mmap::map(&file)? };
+        let bytes = mmap.as_ref();
+        datapkt_buf_reader(bytes, netopts, f)
     }
 }
 
 pub fn datapkt_buf_reader<R: Try<Output = ()>>(
     buf: &[u8],
     netopts: impl Into<NetOpts>,
     for_each: impl FnMut(NetPktParts) -> R,
@@ -86,15 +90,15 @@
     R: Try<Output = ()> + FromResidual<Result<std::convert::Infallible, std::io::Error>>,
     O: Try<Output = LkHash> + FromResidual<<R as Try>::Residual>,
 {
     let mut hasher = blake3::Hasher::new();
     let mut links = vec![];
     super::chunk_reader_try_fold::<_, _, _, MAX_DATA_SIZE>(reader, (), |(), buf| {
         hasher.update(buf);
-        let pkt = datapoint(&buf, ());
+        let pkt = datapoint(buf, ());
         links.push(Link {
             tag: ab(b"bytes"),
             ptr: pkt.hash(),
         });
         for_each(pkt)
     })?;
     if links.is_empty() {
@@ -102,15 +106,15 @@
     }
     if links.len() == 1 {
         return O::from_output(links[0].ptr);
     }
     let blob_hash = hasher.finalize();
     let mut spath = BLOB_SP.to_owned().try_ipath().unwrap();
     spath
-        .extend_from_iter(&[blob_hash.as_bytes() as &[u8], b"part"])
+        .extend_from_iter([blob_hash.as_bytes() as &[u8], b"part"])
         .unwrap();
     let mut links: &mut [Link] = &mut links;
     while links.len() > MAX_LINKS_LEN {
         let part_hash = {
             let part = linkpoint(
                 group,
                 domain,
@@ -125,15 +129,15 @@
         };
         links = &mut links[MAX_LINKS_LEN - 1..];
         links[0] = Link {
             tag: ab(b"list"),
             ptr: part_hash,
         };
     }
-    let bloblist = linkpoint(group, domain, &spath, &links, &[], Stamp::ZERO, ());
+    let bloblist = linkpoint(group, domain, &spath, links, &[], Stamp::ZERO, ());
     let hash = bloblist.hash();
     for_each(bloblist)?;
     O::from_output(hash)
 }
 
 pub fn checkout_from(
     reader: &ReadTxn,
@@ -144,15 +148,15 @@
     if pkt.as_point().is_datapoint() {
         out.write_all(pkt.as_point().data())?;
         return Ok(());
     }
     let mut data_ptrs = vec![];
     open(
         &mut data_ptrs,
-        &reader,
+        reader,
         pkt.as_point().get_links(),
         &mut incomplete,
     )?;
     if !incomplete.is_empty() {
         return Err(Error::Incomplete(incomplete));
     }
     let mut datablks = reader
@@ -160,15 +164,15 @@
         .map(|pkt| IoSlice::new(pkt.data()))
         .collect::<Vec<_>>();
     out.write_all_vectored(&mut datablks)?;
     out.flush()?;
     Ok(())
 }
 
-pub fn checkout<'o>(reader: &ReadTxn, out: impl std::io::Write, hash: LkHash) -> Result<(), Error> {
+pub fn checkout(reader: &ReadTxn, out: impl std::io::Write, hash: LkHash) -> Result<(), Error> {
     let outer = reader.read(&hash)?.ok_or(Error::Incomplete(vec![hash]))?;
     checkout_from(reader, out, &*outer)
 }
 
 fn open(
     lst: &mut Vec<Stamp>,
     reader: &ReadTxn,
```

### Comparing `linkspace-0.1.4/local_dependencies/linkspace-common/src/protocols/impex/blobmap/checkin.rs` & `linkspace-0.3.0rc2/local_dependencies/linkspace-common/src/protocols/impex/blobmap/checkin.rs`

 * *Files identical despite different names*

### Comparing `linkspace-0.1.4/local_dependencies/linkspace-common/src/protocols/impex/blobmap/checkout.rs` & `linkspace-0.3.0rc2/local_dependencies/linkspace-common/src/protocols/impex/blobmap/checkout.rs`

 * *Files 3% similar despite different names*

```diff
@@ -38,21 +38,21 @@
                     std::fs::remove_file(&root)?
                 }
             } else {
                 anyhow::bail!("nothing to do ")
             }
         }
     }
-    std::fs::create_dir_all(&root.parent().unwrap())?;
-    let sp = dgp.path.clone();
+    std::fs::create_dir_all(root.parent().unwrap())?;
+    let sp = dgp.path;
     for pkt in reader.query_tree(query_mode::Order::Desc, &watch) {
-        let p = match resolve_path(&root, &sp, pkt.get_spath(), &[])? {
+        let p = match resolve_path(&root, &sp, pkt.get_path(), &[])? {
             Some(p) => p,
             None => {
-                tracing::warn!("Ignoring {}", pkt.get_spath());
+                tracing::warn!("Ignoring {}", pkt.get_path());
                 continue;
             }
         };
         let e = state.entry(p).or_insert_with(|| (Stamp::ZERO, None));
         if e.0.get() < pkt.get_create_stamp().get() {
             *e = (
                 *pkt.get_create_stamp(),
```

### Comparing `linkspace-0.1.4/local_dependencies/linkspace-common/src/protocols/impex/blobmap/mod.rs` & `linkspace-0.3.0rc2/local_dependencies/linkspace-common/src/protocols/impex/blobmap/mod.rs`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     Checkin,
     Checkout,
 }
 #[derive(Parser, Debug, Clone)]
 pub struct FsSyncOpts {
     #[clap(short, long)]
     pub file_first: bool,
-    #[clap(long, env = "LINKSPACE_SYNC", default_value = "./ssync")]
+    #[clap(long, env = "LK_SYNC", default_value = "./ssync")]
     pub root: PathBuf,
     #[clap(short, long,action=clap::ArgAction::Count)]
     pub clean: u8,
     #[clap(short, long)]
     pub r#async: bool,
     #[clap(subcommand)]
     pub mode: Mode,
```

### Comparing `linkspace-0.1.4/local_dependencies/linkspace-common/src/protocols/impex/mod.rs` & `linkspace-0.3.0rc2/local_dependencies/linkspace-common/src/protocols/impex/mod.rs`

 * *Files identical despite different names*

### Comparing `linkspace-0.1.4/local_dependencies/linkspace-common/src/protocols/lns/admin.rs` & `linkspace-0.3.0rc2/local_dependencies/linkspace-common/src/protocols/lns/admin.rs`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 // This Source Code Form is subject to the terms of the Mozilla Public
 // License, v. 2.0. If a copy of the MPL was not distributed with this
 // file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
 /// The lns:[#:0] lookup entries.
 
 use crate::{prelude::*, protocols::lns::{GROUP_TAG, LNS, BY_TAG_P, PUBKEY_TAG}};
-use linkspace_core::prelude::query_mode::Order;
+use linkspace_core::prelude::{query_mode::Order, RecvPktPtr};
 use tracing::instrument;
 
 use super::claim::Claim;
 
 
 // only call this with a valid claim
 #[instrument(ret,skip(lk),level="debug")]
@@ -81,20 +81,20 @@
         .chain(and.iter().copied())
         .collect();
     save_pkts(wr, &txn)?;
     Ok(true)
 }
 
 #[instrument(ret,skip(reader),level="debug")]
-pub fn ptr_lookup(reader: &ReadTxn, tag: Tag, ptr: Ptr,admin:Option<PubKey>) -> ApplyResult<Claim> {
+pub fn ptr_lookup(reader: &ReadTxn, tag: Tag, ptr: LkHash,admin:Option<PubKey>) -> ApplyResult<Claim> {
     let ple = ptr_lookup_entry(reader, tag, ptr, admin);
     read_claims(reader, ple.into_ok()??.pkt, now()).find_map(|(_,p)| p.ok()?).into()
 }
 #[instrument(ret,skip(reader),level="debug")]
-pub fn ptr_lookup_entry(reader: &ReadTxn, tag: Tag, ptr: Ptr,admin:Option<PubKey>) -> ApplyResult<RecvPktPtr> {
+pub fn ptr_lookup_entry(reader: &ReadTxn, tag: Tag, ptr: LkHash,admin:Option<PubKey>) -> ApplyResult<RecvPktPtr> {
     let path = BY_TAG_P.into_spathbuf().push(tag).push(ptr);
     let mut preds = PktPredicates::from_gd(PRIVATE, LNS).path(path)?.create_before(now()).unwrap();
     // entries have the form /by-tag/TAG/PTR
     if let Some(v) = admin {
         preds.pubkey.add(TestOp::Equal, v.into())
     }
     tracing::debug!(%preds,"by-tag");
@@ -106,17 +106,17 @@
 fn read_claims<'o>(reader: &'o ReadTxn,pkt: &'o impl NetPkt,valid_at:Stamp) -> impl Iterator<Item=TaggedClaim> +'o{
     pkt.get_links().iter()
         .map(|v| (rtag(v.tag),v.ptr))
         .filter(move |((until,_),_)| *until > valid_at)
         .map(|(rt,p)| (rt,Claim::read(reader,&p)))
 }
 
-pub fn list_ptr_lookups<'o>(reader: &'o ReadTxn, tag: AB<[u8; 16]>,ptr:Option<Ptr>,admin:Option<PubKey>) -> impl Iterator<Item=Vec<TaggedClaim>> +'o {
+pub fn list_ptr_lookups(reader: &ReadTxn, tag: AB<[u8; 16]>,ptr:Option<LkHash>,admin:Option<PubKey>) -> impl Iterator<Item=Vec<TaggedClaim>> +'_ {
     let path = BY_TAG_P.into_spathbuf().push(tag);
-    let path = if let Some(p) = ptr { path.push(&*p)} else { path}; 
+    let path = if let Some(p) = ptr { path.push(*p)} else { path}; 
     let mut preds = PktPredicates::from_gd(PRIVATE, LNS).create_before(now()).unwrap();
     preds.prefix(path).unwrap();
     preds.path_len.add(TestOp::Equal,3);
     preds.state.i_branch.add(TestOp::Equal,0);
     if let Some(v) = admin {
         preds.pubkey.add(TestOp::Equal, v.into())
     }
@@ -124,15 +124,15 @@
     let it = reader.query_tree(Order::Desc, &preds).peekable();
     let now = now();
     it.map(move |tagpkt| read_claims(reader,&tagpkt.pkt,now).collect())
 }
 
 
 #[instrument(ret,level="trace")]
-pub fn mut_ptrlookup_entry(links:&[Link],path:&IPath,remove:Option<Ptr>,add_link_first:Option<(bool,Link)>,admin:Option<&SigningKey>,now:Stamp) -> NetPktBox{
+pub fn mut_ptrlookup_entry(links:&[Link],path:&IPath,remove:Option<LkHash>,add_link_first:Option<(bool,Link)>,admin:Option<&SigningKey>,now:Stamp) -> NetPktBox{
     let (pre,post) = match add_link_first {
         Some((true,link)) => (Some(link),None),
         Some((false,link)) => (None,Some(link)),
         None => (None,None),
     };
     let lks =  links.iter().copied().filter(|l| Some(l.ptr) != remove).filter(|l| rtag(l.tag).0 > now);
     let new : Vec<_> = pre.into_iter().chain(lks).chain(post.into_iter()).collect();
```

### Comparing `linkspace-0.1.4/local_dependencies/linkspace-common/src/protocols/lns/claim.rs` & `linkspace-0.3.0rc2/local_dependencies/linkspace-common/src/protocols/lns/claim.rs`

 * *Files 1% similar despite different names*

```diff
@@ -79,35 +79,35 @@
 }
 
 impl Claim {
     pub fn new(name:Name,until:Stamp,links:&[Link],misc:Vec<ABList>) -> anyhow::Result<Self>{
         let path = name.claim_ipath();
         let data = ClaimData::new(until, misc).to_vec();
         let group =name.claim_group().unwrap_or(PRIVATE);
-        let pkt = linkpoint(group, LNS, &path, &links, &data, Stamp::ZERO, ()).as_netbox(); 
+        let pkt = linkpoint(group, LNS, &path, links, &data, Stamp::ZERO, ()).as_netbox(); 
         ensure!(*pkt.get_create_stamp() < until);
         Self::from(pkt)
     }
     pub fn read(reader: &ReadTxn,ptr: &LkHash) -> anyhow::Result<Option<Self>>{
-        Ok(reader.read(&ptr)?.map(|p| Claim::from(p)).transpose()?)
+        reader.read(ptr)?.map(Claim::from).transpose()
     }
     
     pub fn enckey(&self) -> anyhow::Result<Option<Either<&str,LkHash>>>{
         match self.data.get_value(b"enckey").transpose()?{
             Some(val) => Ok(Some(Either::Left(std::str::from_utf8(val)?))),
             None => match self.links().first_eq(ENCKEY_TAG){
                 Some(lnk) => Ok(Some(Either::Right(lnk.ptr))),
                 None => Ok(None),
             },
         }
     }
     
     pub fn from(pkt: impl NetPkt)-> anyhow::Result<Self>{
         ensure!(pkt.is_linkpoint(),"claim is always a linkpoint");
-        let spath = pkt.get_spath();
+        let spath = pkt.get_path();
         ensure!(spath.starts_with(&CLAIM_PREFIX));
         ensure!(*pkt.get_domain() == LNS);
         let mut it = spath.iter();
         it.next().unwrap();
         let namep= it.spath();
         let name = Name::from_spath(namep)?;
         ensure!(*pkt.get_group() == name.claim_group().unwrap_or(PRIVATE),"claim point in the wrong group");
@@ -139,15 +139,15 @@
     Ok(keypoint(claim.name.claim_group().unwrap(), LNS, claim.pkt.get_ipath(), &vote_link, &[], now(), key, ()).as_netbox())
 }
 
 
 pub struct ClaimData(Vec<ABList>);
 impl ClaimData {
     pub fn new(until:Stamp,mut values:Vec<ABList>) -> Self {
-        values.splice(0..0, [clist(&[b"until" as &[u8],&until.0])]);
+        values.splice(0..0, [clist([b"until" as &[u8],&until.0])]);
         ClaimData(values)
     }
     pub fn get_value(&self,b:&[u8]) -> Option<anyhow::Result<&[u8]>>{
         let abl = self.get(b)?;
         match abl.lst.as_slice() {
             [(_,Some(Ctr::Colon)),(b,None)] => Some(Ok(b)),
             _ => Some(Err(anyhow::anyhow!("expected key:val , got {}",abl)))
```

### Comparing `linkspace-0.1.4/local_dependencies/linkspace-common/src/protocols/lns/eval.rs` & `linkspace-0.3.0rc2/local_dependencies/linkspace-common/src/protocols/lns/eval.rs`

 * *Files 12% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 //
 // This Source Code Form is subject to the terms of the Mozilla Public
 // License, v. 2.0. If a copy of the MPL was not distributed with this
 // file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
 use std::time::Duration;
 
-use abe::{fncs, eval::{ScopeEval,  EvalScopeImpl, ScopeFunc, EvalCtx,eval, ApplyResult, ScopeEvalInfo}, ABE, ast};
+use abe::{fncs, eval::{ScopeMacro,  EvalScopeImpl, ScopeFunc, EvalCtx,eval, ApplyResult, ScopeMacroInfo}, ABE, ast};
 use anyhow::{anyhow, Context, bail };
-use linkspace_pkt::{Tag, Ptr, pkt_ctx, ptrv};
+use linkspace_pkt::{Tag, LkHash, pkt_ctx, ptrv};
 
 use crate::{ eval::LKS };
 
 use super::{claim::{Claim }, name::Name, GROUP_TAG, PUBKEY_TAG, public_claim::Issue};
 
 
 
@@ -31,19 +31,19 @@
     fn get_claim_link_ptr(&self, name: Name, tag: Tag) -> ApplyResult{
         let claim = self.get_claim(name)??;
         claim.links().first_eq(tag).map(ptrv).into()
     }
     fn get_claim(&self, name: Name) -> anyhow::Result<Option<Claim>>{
         super::lookup_claim(&self.rt.lk()?, &name)
     }
-    fn get_by_tag(&self, tag: Tag,ptr:Ptr) -> anyhow::Result<Option<Name>>{
+    fn get_by_tag(&self, tag: Tag,ptr:LkHash) -> anyhow::Result<Option<Name>>{
         Ok(super::reverse_lookup(&self.rt.lk()?, tag,ptr).into_ok()?.map(|o| o.name))
     }
     
-    fn get_by_tag_abe(&self,tag:Tag,ptr:Ptr) -> ApplyResult<String> {
+    fn get_by_tag_abe(&self,tag:Tag,ptr:LkHash) -> ApplyResult<String> {
         let name :Name= self.get_by_tag(tag, ptr)??;
         if tag == GROUP_TAG { Ok(format!("[#:{name}]")).into()}
         else if tag == PUBKEY_TAG { Ok(format!("[@:{name}]")).into()}
         else {Err(anyhow!("bug! weird tag{tag}")).into()}
     }
 }
 
@@ -58,87 +58,87 @@
     fn get_claim_link_ptr(&self, name: Name, tag: Tag) -> anyhow::Result<Vec<u8>>{
         let claim = self.get_claim(name)?;
         claim.links().first_eq(tag).map(ptrv).context("tag not set in claim")
     }
     // TODO - this and get by_tag needs to probe the lns resolver instead of doing it themselves.
     fn get_claim(&self, name: Name) -> anyhow::Result<Claim>{
         match self.private().get_claim(name.clone())?{
-            Some(c) => return Ok(c),
+            Some(c) => Ok(c),
             None => {
                 let mut issue :Result<(),Issue>= Ok(());
                 match super::lookup_live_chain(&self.rt.lk()?, &name, &mut |i| {issue = Err(i);Ok(())})?{
                     Ok(c) => Ok(c.claim),
                     Err(_e) => bail!("couldn't find claim - last-issue: {issue:?}"), // make udp call
                 }
             }
         }
     }
-    fn get_by_tag(&self, tag: Tag,ptr:Ptr) -> anyhow::Result<Option<Name>>{
+    fn get_by_tag(&self, tag: Tag,ptr:LkHash) -> anyhow::Result<Option<Name>>{
         match self.private().get_by_tag(tag, ptr)?{
-            Some(v) => return Ok(Some(v)),
+            Some(v) => Ok(Some(v)),
             None => Ok(None)
         }
     }
-    fn get_by_tag_abe(&self,tag:Tag,ptr:Ptr) -> ApplyResult<String> {
+    fn get_by_tag_abe(&self,tag:Tag,ptr:LkHash) -> ApplyResult<String> {
         let name :Name= self.get_by_tag(tag, ptr)??;
         if tag == GROUP_TAG { Ok(format!("[#:{name}]")).into()}
         else if tag == PUBKEY_TAG { Ok(format!("[@:{name}]")).into()}
         else {Err(anyhow!("bug! weird tag{tag}")).into()}
     }
 }
 
 impl<R: LKS > EvalScopeImpl for NetLNS<R> {
     fn about(&self) -> (String, String) {
-        ("lns".into(), "".into())
+        ("lns".into(), String::new())
     }
     fn list_funcs(&self) -> &[ScopeFunc<&Self>] {
         fncs!([
             (
                 "#",
                 1..=7,
                 Some(true),
                 "(namecomp)* - get the associated lns group",
                 // error on get failure
                 |this: &Self, args: &[&[u8]]| this.get_claim_link_ptr(Name::from(args)?, GROUP_TAG ),
                 // pass on get failure
-                |this: &Self, phash: &[u8], _| this.get_by_tag_abe(GROUP_TAG, Ptr::try_fit_bytes_or_b64(phash)?)
+                |this: &Self, phash: &[u8], _| this.get_by_tag_abe(GROUP_TAG, LkHash::try_fit_bytes_or_b64(phash)?)
             ),
             // error on get failure
-            ("?#", 1..=1, "find by group# tag", |this:&Self, i: &[&[u8]]| name_str(this.get_by_tag(GROUP_TAG, Ptr::try_fit_bytes_or_b64(i[0])?))),
+            ("?#", 1..=1, "find by group# tag", |this:&Self, i: &[&[u8]]| name_str(this.get_by_tag(GROUP_TAG, LkHash::try_fit_bytes_or_b64(i[0])?))),
             (
                 "@",
                 1..=7,
                 Some(true),
                 "(namecomp)* - get the associated lns key",
                 // error on get failure
                 |this: &Self, args: &[&[u8]]| this.get_claim_link_ptr(Name::from(args)?, PUBKEY_TAG),
                 // pass on get failure
-                |this: &Self, phash: &[u8], _| this.get_by_tag_abe(PUBKEY_TAG, Ptr::try_fit_bytes_or_b64(phash)?)
+                |this: &Self, phash: &[u8], _| this.get_by_tag_abe(PUBKEY_TAG, LkHash::try_fit_bytes_or_b64(phash)?)
             ),
             // error on get failure
-            ("?@", 1..=1, "find by pubkey@ tag", |this:&Self, i: &[&[u8]]| name_str(this.get_by_tag(PUBKEY_TAG, Ptr::try_fit_bytes_or_b64(i[0])?)))
+            ("?@", 1..=1, "find by pubkey@ tag", |this:&Self, i: &[&[u8]]| name_str(this.get_by_tag(PUBKEY_TAG, LkHash::try_fit_bytes_or_b64(i[0])?)))
         ])
     }
 
-    fn list_eval(&self) -> &[ScopeEval<&Self>] {
-        &[ScopeEval {
+    fn list_macros(&self) -> &[ScopeMacro<&Self>] {
+        &[ScopeMacro {
             apply: |this, abe: &[ABE], scope| {
                 let ctx = EvalCtx { scope };
                 let mut it = abe.split(|v| v.is_fslash());
                 let name = it.next().context("missing name")?;
                 let expr = it.as_slice();
                 let mut it = name.split(|v| v.is_colon());
                 let _empty = it.next().context("arg delimited with ':'")?;
                 ast::exact::<0>(_empty)?;
                 let name : Name = eval(&ctx,it.as_slice())?.try_into()?;
                 let claim = this.get_claim(name)?;
                 let v: ApplyResult = eval(&pkt_ctx(ctx, &claim.pkt), expr).map(|v| v.concat()).map_err(|e| anyhow!(e.to_string())).into();
                 v
             },
-            info: ScopeEvalInfo {
+            info: ScopeMacroInfo {
                 id: "lns",
                 help: "[:comp]*/expr",
             },
         }]
     }
 }
 
@@ -150,50 +150,50 @@
         fncs!([
             (
                 "private#",
                 1..=7,
                 Some(true),
                 "(namecomp)* - get the associated lns group",
                 |this: &Self, args: &[&[u8]]| this.get_claim_link_ptr(Name::from(args)?, GROUP_TAG ).require("no private claim set"),
-                |this: &Self, phash: &[u8], _| this.get_by_tag_abe(GROUP_TAG, Ptr::try_fit_bytes_or_b64(phash)?)
+                |this: &Self, phash: &[u8], _| this.get_by_tag_abe(GROUP_TAG, LkHash::try_fit_bytes_or_b64(phash)?)
             ),
             ("?private#", 1..=1, "find by group# tag",
              
-             |this:&Self, i: &[&[u8]]| name_str(this.get_by_tag(GROUP_TAG, Ptr::try_fit_bytes_or_b64(i[0])?))
+             |this:&Self, i: &[&[u8]]| name_str(this.get_by_tag(GROUP_TAG, LkHash::try_fit_bytes_or_b64(i[0])?))
             ),
             (
                 "private@",
                 1..=7,
                 Some(true),
                 "(namecomp)* - get the associated lns key",
                 |this: &Self, args: &[&[u8]]| this.get_claim_link_ptr(Name::from(args)?, PUBKEY_TAG).require("no private claim set"),
-                |this: &Self, phash: &[u8], _| this.get_by_tag_abe(PUBKEY_TAG, Ptr::try_fit_bytes_or_b64(phash)?)
+                |this: &Self, phash: &[u8], _| this.get_by_tag_abe(PUBKEY_TAG, LkHash::try_fit_bytes_or_b64(phash)?)
             ),
             ("?private@", 1..=1, "find by pubkey@ tag",
-             |this:&Self, i: &[&[u8]]| name_str(this.get_by_tag(PUBKEY_TAG, Ptr::try_fit_bytes_or_b64(i[0])?))
+             |this:&Self, i: &[&[u8]]| name_str(this.get_by_tag(PUBKEY_TAG, LkHash::try_fit_bytes_or_b64(i[0])?))
             )
         ])
     }
 
-    fn list_eval(&self) -> &[ScopeEval<&Self>] {
-        &[ScopeEval {
+    fn list_macros(&self) -> &[ScopeMacro<&Self>] {
+        &[ScopeMacro {
             apply: |this, abe: &[ABE], scope| {
                 let ctx = EvalCtx { scope };
                 let mut it = abe.split(|v| v.is_fslash());
                 let name = it.next().context("missing name")?;
                 let mut expr = it.as_slice();
                 if expr.is_empty() { expr = &linkspace_pkt::DEFAULT_POINT_FMT;}
                 let mut it = name.split(|v| v.is_colon());
                 let _empty = it.next().context("arg delimited with ':'")?;
                 ast::exact::<0>(_empty)?;
                 let name : Name = eval(&ctx,it.as_slice())?.try_into()?;
                 let claim = this.get_claim(name)?.context("cant find claim")?;
                 let v: ApplyResult = eval(&pkt_ctx(ctx, &claim.pkt), expr).map(|v| v.concat()).map_err(|e| anyhow!(e.to_string())).into();
                 v
             },
-            info: ScopeEvalInfo {
+            info: ScopeMacroInfo {
                 id: "private-lns",
                 help: "[:comp]*/expr",
             },
         }]
     }
 }
```

### Comparing `linkspace-0.1.4/local_dependencies/linkspace-common/src/protocols/lns/local_claim.rs` & `linkspace-0.3.0rc2/local_dependencies/linkspace-common/src/protocols/lns/local_claim.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 // Copyright Anton Sol
 //
 // This Source Code Form is subject to the terms of the Mozilla Public
 // License, v. 2.0. If a copy of the MPL was not distributed with this
 // file, You can obtain one at https://mozilla.org/MPL/2.0/.
 use linkspace_core::{
-    prelude::{query_mode::Order, *}
+    prelude::{query_mode::Order, *, RecvPktPtr}
 };
 use crate::{runtime::Linkspace, protocols::lns::{ admin::save_private_claim }};
 
 use super::{*, name::Name, claim::Claim};
 
 pub fn get_private_claim<'o>(
     reader: &'o ReadTxn,
@@ -35,11 +35,11 @@
 
 
 pub (crate) fn setup_local_keyclaim(
     lk: &Linkspace,
     claim: Claim,
     admin: Option<&SigningKey>,
 ) -> anyhow::Result<()> {
-    // We fake a claim chain and just insert it into the admin tree.
+    // We fake a claim chain and insert it into the admin tree.
     save_private_claim(lk, &claim, admin, &[],true)?;
     Ok(())
 }
```

### Comparing `linkspace-0.1.4/local_dependencies/linkspace-common/src/protocols/lns/mod.rs` & `linkspace-0.3.0rc2/local_dependencies/linkspace-common/src/protocols/lns/mod.rs`

 * *Files 6% similar despite different names*

```diff
@@ -1,77 +1,77 @@
 // Copyright Anton Sol
 //
 // This Source Code Form is subject to the terms of the Mozilla Public
 // License, v. 2.0. If a copy of the MPL was not distributed with this
 // file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
 /**
-LNS is a little complex because it supports 3 modes.
+LNS is quite a bit complex because it supports 3 modes.
 A mode defines when a claim is 'live'.
 
 The modes are :
 - the public roots (:com , :dev, :free etc) - authorities vote and claims have fast path based lookup.
 - a :local admin, creates keypoints to other 'roots' creating a chain of names. 
-- the :env claims are simply claims stored as files in the LINKSPACE directory
+- the :files claims are claims stored as files in the LK_DIR/files/ directory
 
 an admin key/process creates a local lookup & reverse-lookup table such that each can quickly be resolved.
 Every part of this is not yet fully implemented.
 
 **/
 
 
 
 use abe::eval::{clist, ApplyResult};
 use anyhow::{Context };
 use byte_fmt::ab;
 use linkspace_argon2_identity::pubkey;
-use linkspace_pkt::{spath, Domain, Tag, PubKey, GroupID, Ptr, Stamp, Link };
+use linkspace_pkt::{ Domain, Tag, PubKey, GroupID, LkHash, Stamp, Link, ipath1, IPathC };
 use tracing::instrument;
 
 use crate::runtime::Linkspace;
 
 use self::{claim::{LiveClaim, Claim, resolve_enckey}, name::{Name, SpecialName}, public_claim::IssueHandler};
 
 
 pub mod name;
 pub mod claim;
 
 pub mod public_claim;
 pub mod local_claim;
-pub mod env_claim;
+pub mod file_claim;
 
 pub mod eval;
 pub mod utils;
 pub mod admin;
 
 pub const LNS: Domain = ab(b"lns");
-spath!(pub const CLAIM_PREFIX = [b"claims"]);
+pub const CLAIM_PREFIX : IPathC<15> = ipath1::<6>(b"claims");
 /// tag expected for local claims pointing to a (live) lns:[#:pub] claim
 pub const PUB_CLAIM_TAG : Tag = ab(b"pub-claim");
 pub const PUBKEY_TAG : Tag = ab(b"pubkey@");
 pub const VOTE_TAG : Tag = ab(b"vote");
 pub const GROUP_TAG: Tag = ab(b"group#");
 pub const ENCKEY_TAG : Tag = ab(b"enckey");
 /// A linkpoint at lns:[#:0]:by-tag/../PTR will contain by-claim:CLAIM_HASH
 pub const BY_CLAIM_TAG : Tag = ab(b"by-claim");
 
-pub const BY_TAG_P : linkspace_pkt::IPathC<15> = linkspace_pkt::ipath1(b"by-tag");
-spath!(pub const BY_GROUP_TAG = [b"by-tag",&GROUP_TAG.0]);
-spath!(pub const BY_PUBKEY_TAG= [b"by-tag",&PUBKEY_TAG.0]);
+pub const BY_TAG_P : linkspace_pkt::IPathC<15> = linkspace_pkt::ipath1::<6>(b"by-tag");
+pub static BY_GROUP_TAG : [&[u8];2] = [b"by-tag",&GROUP_TAG.0];
+pub static BY_PUBKEY_TAG : [&[u8];2] = [b"by-tag",&PUBKEY_TAG.0];
 
 
 pub fn auth_tag(b:&[u8]) -> Tag {
     let mut auth = ab(b"^");
     auth[0..15][15-b.len()..].copy_from_slice(b);
     auth
 }
 /// Get the parent claim
 pub fn lookup_authority_claim(lk:&Linkspace,name:&Name,issue_handler:IssueHandler) -> anyhow::Result<Result<Claim,Claim>>{
     match name.special() {
-        Some(SpecialName::Env) => Ok(Ok(Claim::new(name.clone(),Stamp::MAX,&[],vec![]).unwrap())),
+        Some(SpecialName::File) => Ok(Ok(Claim::new(name.clone(),Stamp::MAX,&[],vec![]).unwrap())),
         Some(SpecialName::Local) => todo!(),
         None => {
             let (parent,_val) = name.spath().pop();
             let name = Name::from_spath(parent).ok().unwrap_or_else(Name::root);
             Ok(lookup_live_chain(lk, &name, issue_handler)?.map(|p| p.claim).map_err(|p|p.claim))
         },
     }
@@ -85,51 +85,51 @@
     }
 }
 
 
 /// Lookup the chain of claims that gave a name
 pub fn lookup_live_chain(lk:&Linkspace, name: &Name,issue_handler:IssueHandler) -> anyhow::Result<Result<LiveClaim,LiveClaim>>{
     match name.special(){
-        Some(SpecialName::Env) => {
-            let path = name.fs_env_path()?;
+        Some(SpecialName::File) => {
+            let path = name.file_path()?;
             let claim : anyhow::Result<Claim>= try {
-                let pbytes = match lk.env().env_data(&path, false)?{
+                let pbytes = match lk.env().files_data(&path, false)?{
                     Some(p) => p,
                     None => return Ok(Err(dummy_root(name)))
                 };
-                let pkt = linkspace_pkt::read::parse_netpkt(&pbytes, false)?.map_err(|_| anyhow::anyhow!("not a valid packet"))?;
-                Claim::from(pkt)?
+                let pkt = linkspace_pkt::read::read_pkt(&pbytes, false)?;
+                Claim::from(pkt.as_ref())?
             };
             Ok(Ok(LiveClaim{
                 claim: claim.with_context(||anyhow::anyhow!("Reading claim at {}",path.to_string_lossy()))?,
                 signatures: vec![],
                 parent: None,
             }))
         },
         Some(SpecialName::Local) => {
-            // No admin process exists yet so we just pretend something setup the correct :local claims
+            // No admin process exists yet so we pretend something setup the correct :local claims
              match local_claim::get_private_claim(&lk.get_reader(), name, None).into_ok()?{
                 Some(claim) => {
                     Ok(Ok(LiveClaim{
                         claim:Claim::from(claim)?,
                         signatures: vec![],parent:None
                     }))
                 }
                 None => Ok(Err(dummy_root(name))),
              }
         }
-        // The admin process doesn't exist yet so we just walk the chain for now
+        // The admin process doesn't exist yet so we walk the chain for now
         None => public_claim::walk_live_claims(&lk.get_reader(), public_claim::root_claim(), &mut name.spath().iter(), issue_handler),
     }
 }
 
 pub fn lookup_enckey(lk:&Linkspace,name:&Name) -> anyhow::Result<Option<(PubKey,String)>>{
     let claim = lookup_claim(lk, name)?;
     match claim{
-        None => return Ok(None),
+        None => Ok(None),
         Some(c) => match c.enckey()?{
             Some(k) => resolve_enckey(&lk.get_reader(), k).map(Some),
             None => Ok(None)
         },
     }
 }
 
@@ -143,15 +143,15 @@
 }
 
 pub fn lookup_claim(lk:&Linkspace,name:&Name) -> anyhow::Result<Option<Claim>>{
     lookup_live_chain(lk, name, &mut |_|Ok(())).map(|o|o.ok().map(|o|o.claim))
 }
 
 #[instrument(skip(lk),ret)]
-pub fn reverse_lookup(lk:&Linkspace,tag:Tag,ptr:Ptr) -> ApplyResult<Claim>{
+pub fn reverse_lookup(lk:&Linkspace,tag:Tag,ptr:LkHash) -> ApplyResult<Claim>{
     // Because we can't yet trust the admin, we have to do a forward lookup as well to validate this is a valid claim.
     let claim = admin::ptr_lookup(&lk.get_reader(), tag, ptr, None)?;
     let name = &claim.name;
     let by_name = lookup_claim(lk, name)??;
     if by_name.links().first_eq(tag).map(|p|p.ptr == ptr).unwrap_or(false){
         Some(by_name).into()
     }else {
@@ -161,23 +161,23 @@
 
 pub fn setup_special_keyclaim(
     lk: &Linkspace,
     name: Name,
     enckey: &str,
     overwrite:bool
 ) -> anyhow::Result<PubKey> {
-    let sp = name.special().context("will only setup :local or :env keys")?;
+    let sp = name.special().context("will only setup :local or :file keys")?;
     if let Ok(Some(c)) = lookup_claim(lk, &name){
         if !overwrite {anyhow::bail!("claim already set but overwrite is false")}
         else { tracing::debug!(old_claim=%c)}
     }
     let pubkey = pubkey(enckey)?.into();
-    let claim = Claim::new(name, Stamp::MAX, &[Link{tag: PUBKEY_TAG,ptr:pubkey}], vec![clist(&["enckey",enckey])])?;
+    let claim = Claim::new(name, Stamp::MAX, &[Link{tag: PUBKEY_TAG,ptr:pubkey}], vec![clist(["enckey",enckey])])?;
     match sp {
         SpecialName::Local => {
             if claim.name.spath().collect().len() > 2 { anyhow::bail!("Local is currently limited to single component name")}
             local_claim::setup_local_keyclaim(lk, claim,None)?;
         },
-        SpecialName::Env => env_claim::setup(lk,claim,overwrite)?
+        SpecialName::File => file_claim::setup(lk,claim,overwrite)?
     }
     Ok(pubkey)
 }
```

### Comparing `linkspace-0.1.4/local_dependencies/linkspace-common/src/protocols/lns/name.rs` & `linkspace-0.3.0rc2/local_dependencies/linkspace-common/src/protocols/lns/name.rs`

 * *Files 4% similar despite different names*

```diff
@@ -36,58 +36,58 @@
 
 #[derive(Clone,PartialEq,Eq)]
 /// A reversed spath constrained to fit the lns path
 pub struct Name { spath: SPathBuf,special:Option<SpecialName>}
 #[derive(Copy,Clone,PartialEq,Eq)]
 pub enum SpecialName {
     Local,
-    Env
+    File
 }
 impl SpecialName {
     pub fn from(b:&[u8]) -> Option<Self>{
         match b {
             b"local" => Some(SpecialName::Local),
-            b"env" => Some(SpecialName::Env),
+            b"file" | b"~" => Some(SpecialName::File),
             _ => None
         }
     }
 }
 
 
 impl Name {
     pub fn root() -> Self { Name{spath: SPathBuf::new(), special:None}}
     pub fn local() -> Self { Name{spath: spath_buf(&[b"local"]), special:Some(SpecialName::Local)}}
-    pub(crate) fn fs_env_path(&self) -> anyhow::Result<std::path::PathBuf>{
-        ensure!(matches!(self.special , Some(SpecialName::Env)));
+    pub(crate) fn file_path(&self) -> anyhow::Result<std::path::PathBuf>{
+        ensure!(matches!(self.special , Some(SpecialName::File)));
         self.claim_ipath().collect().into_iter()
             .map(|s| match std::str::from_utf8(s)?{
-                 "key" => anyhow::bail!("env keyname can't contain the word 'key'"),
+                 "key" => anyhow::bail!("file keyname can't contain the word 'key'"),
                 c => Ok(c)
             }).chain([Ok("key")]).try_collect()
     }
-    pub fn claim_ipath(&self) -> IPathBuf { CLAIM_PREFIX.join(&self.spath).ipath()}
+    pub fn claim_ipath(&self) -> IPathBuf { CLAIM_PREFIX.ipath().join(&self.spath).ipath()}
     pub fn claim_group(&self) -> Option<GroupID> {
         match self.special{
             Some(SpecialName::Local) => Some(PRIVATE),
-            Some(SpecialName::Env) => None,
+            Some(SpecialName::File) => None,
             None => Some(PUBLIC),
         }
     }
     pub fn from_spath(path:&SPath) -> Result<Name,NameError>{
         let rcomps = path.collect();
         if rcomps.is_empty(){ return Err(NameError::MinLen)}
         if rcomps.len() > MAX_LNS_NAME_LEN { return Err(NameError::MaxLen)}
-        let special = SpecialName::from(*rcomps.first().unwrap());
+        let special = SpecialName::from(rcomps.first().unwrap());
         if path.spath_bytes().len() > MAX_LNS_NAME_SIZE { return Err(NameError::MaxSize)}
         Ok(Name { spath: path.into_spathbuf() ,special})
     }
     pub fn from(comps: &[&[u8]]) -> Result<Name,NameError>{
         if comps.is_empty(){ return Err(NameError::MinLen)}
         if comps.len() > MAX_LNS_NAME_LEN { return Err(NameError::MaxLen)}
-        let special = SpecialName::from(*comps.last().unwrap());
+        let special = SpecialName::from(comps.last().unwrap());
         let it = comps.iter().rev();
         let path = SPathBuf::try_from_iter(it)?;
         if path.spath_bytes().len() > MAX_LNS_NAME_SIZE { return Err(NameError::MaxSize)}
         Ok(Name { spath: path ,special})
     }
     pub fn spath(&self) -> &SPath {
         &self.spath
@@ -112,15 +112,15 @@
         if self.spath.is_empty(){
             return out(ABE::Expr(ast::Expr::Lst(abev!({ "LNS-ROOT" }))))
         }
         let arr = self.spath.collect();
         let mut it = arr.iter().rev();
         let first = it.next().unwrap();
         out(ABE::Expr(ast::Expr::Bytes(first.to_vec())));
-        while let Some(comp) = it.next(){
+        for comp in it{
             abe!( : (**comp) ).for_each(&mut *out)
         }
     }
 }
 impl Display for Name {
     fn fmt(&self, f: &mut std::fmt::Formatter<'_>) -> std::fmt::Result {
         f.write_str(&self.to_abe_str())
```

### Comparing `linkspace-0.1.4/local_dependencies/linkspace-common/src/protocols/lns/public_claim.rs` & `linkspace-0.3.0rc2/local_dependencies/linkspace-common/src/protocols/lns/public_claim.rs`

 * *Files 7% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     let data = ClaimData::try_from(claim_pkt.data()).unwrap();
     let claim = Claim{pkt:RecvPkt::from_dyn(&claim_pkt),data,name:Name::root()};
     let signatures = it.take(nsigns).map(|p| RecvPkt::from_dyn(&p)).collect();
     LiveClaim { claim, signatures, parent: None }
 }
 
 pub fn lns_root_claims() -> impl Iterator<Item=NetPktBox>{
-    crate::pkt_reader::NetPktDecoder::new(linkspace_core::LNS_ROOTS).into_iter().map(|v| v.unwrap().as_netbox())
+    crate::pkt_reader::NetPktDecoder::new(linkspace_core::LNS_ROOTS).map(|v| v.unwrap().as_netbox())
 }
 
 pub type IssueHandler<'o> = &'o mut dyn FnMut(Issue) -> anyhow::Result<()>;
 
 pub type Voteing = (LkHash,(Option<Claim>,Vec<RecvPkt>));
 
 #[derive(Error,Debug)]
@@ -56,23 +56,27 @@
         None => return Ok(Ok(parent)),
     };
     let ipath = parent.claim.pkt.get_ipath().into_ipathbuf().append(sub);
     let mut predicates = Query::dgpk(LNS, *parent.claim.pkt.get_group(), ipath,B64([255;32])).predicates;
     predicates.path_len.add(crate::core::prelude::TestOp::Equal, 2);
     let mut claim_votes : LkHashMap<(Option<Claim>,Vec<RecvPkt>)>= Default::default();
     let mut _count = 0;
+    let max_required_votes = (parent.claim.authorities().count()+1)/2;
     for auth in parent.claim.authorities(){
         _count = 0;
         predicates.pubkey = TestSet::new_eq(auth.into());
         match reader.query(Mode::TREE_DESC,&predicates,&mut _count)?.next(){
             Some(vote) => {
                 match vote.get_links().first(){
                     Some(l) if l.tag == VOTE_TAG =>{
                         match claim_votes.entry(l.ptr){
-                            std::collections::hash_map::Entry::Occupied(mut o) => {o.get_mut().1.push(vote.owned());},
+                            std::collections::hash_map::Entry::Occupied(mut o) => {
+                                o.get_mut().1.push(vote.owned());
+                                if o.get().1.len() >= max_required_votes { break};
+                            },
                             std::collections::hash_map::Entry::Vacant(v) =>{
                                 let o_claim = reader.read(&l.ptr)?;
                                 let claim = match o_claim {
                                     Some(claim_pkt) => match Claim::from(claim_pkt){
                                         Ok(o) => Some(o),
                                         Err(error) => {
                                             issue_handler(Issue::BadClaimInVote{ claim:claim_pkt.owned(), vote: l.ptr ,error})?;
```

### Comparing `linkspace-0.1.4/local_dependencies/linkspace-common/src/protocols/lns/utils.rs` & `linkspace-0.3.0rc2/local_dependencies/linkspace-common/src/protocols/lns/utils.rs`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 use crate::prelude::*;
 
 use super::{claim::Claim, name::{Name }, LNS};
 
 pub fn list_all_potential_claims_with_prefix<'o>(reader:&'o ReadTxn,name: &Name) -> impl Iterator<Item=anyhow::Result<Claim>> +'o{
     let path = name.claim_ipath();
     let now = now();
-    let mut preds = PktPredicates::from_gd(name.claim_group().expect("env names don't do claims"), LNS).create_before(now).unwrap();
+    let mut preds = PktPredicates::from_gd(name.claim_group().expect("'file' names don't do claims"), LNS).create_before(now).unwrap();
     let _ = preds.prefix(&**path);
     //preds.state.i_branch.add(TestOp::Equal, 0);
     reader.query_tree(query_mode::Order::Desc, &preds).flat_map(move |pkt| -> Option<anyhow::Result<Claim>> {
         match Claim::from(pkt){
             Ok(c) => if c.until() > now {Some(Ok(c))} else {None}
             Err(e) => Some(Err(e)),
         }
     })
 }
 
 
 pub type TaggedClaim = ((Stamp,[u8;8]),anyhow::Result<Option<Claim>>);
-pub fn list_all_reverse_lookups<'o>(_reader: &'o ReadTxn, _tag: AB<[u8; 16]>,_ptr:Option<Ptr>) -> Vec<Vec<TaggedClaim>> {
+pub fn list_all_reverse_lookups(_reader: &ReadTxn, _tag: AB<[u8; 16]>,_ptr:Option<LkHash>) -> Vec<Vec<TaggedClaim>> {
     todo!()
 }
```

### Comparing `linkspace-0.1.4/local_dependencies/linkspace-common/src/runtime/handlers.rs` & `linkspace-0.3.0rc2/local_dependencies/linkspace-common/src/runtime/handlers.rs`

 * *Files 0% similar despite different names*

```diff
@@ -81,15 +81,15 @@
         }
     }
     
 }
 
 impl<F: PktStreamHandler> PktStreamHandler for NotifyClose<F> {
     fn handle_pkt(&mut self, pkt: &dyn NetPkt, lk: &Linkspace) -> ControlFlow<()> {
-        self.inner.handle_pkt(pkt, &lk)
+        self.inner.handle_pkt(pkt, lk)
     }
 
     fn stopped(&mut self, _watch: BareWatch, _rx: &Linkspace, _reason: StopReason) {
         if let Some(echo) = self.origin.take(){
             self.inner.handle_pkt(&echo, _rx);
         }
         self.inner.stopped(_watch, _rx, _reason)
```

### Comparing `linkspace-0.1.4/local_dependencies/linkspace-common/src/runtime/rx.rs` & `linkspace-0.3.0rc2/local_dependencies/linkspace-common/src/runtime/rx.rs`

 * *Files 3% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 // License, v. 2.0. If a copy of the MPL was not distributed with this
 // file, You can obtain one at https://mozilla.org/MPL/2.0/.
 use super::handlers::{FollowHandler, PktStreamHandler, SinglePktHandler, StopReason};
 use anyhow::{bail, Context};
 pub use async_executors::{Timer, TimerExt};
 use futures::future::Either;
 pub use futures::task::{LocalSpawn, LocalSpawnExt};
-use linkspace_core::prelude::*;
+use linkspace_core::prelude::{*, lmdb::{BTreeEnv, WriteTxn2, misc::Refreshable}};
 use linkspace_pkt::reroute::ShareArcPkt;
 use std::{
     borrow::{Borrow, Cow},
     cell::{Cell, OnceCell, RefCell},
-    ops::{Add, ControlFlow},
+    ops::{ ControlFlow},
     rc::{Rc, Weak},
     time::{Duration, Instant},
 };
 use tracing::{warn, Span, debug_span, instrument};
 
 pub type PktStream = Box<dyn PktStreamHandler + 'static>;
 pub type Matcher = linkspace_core::matcher::Matcher<PktStream>;
@@ -35,15 +35,15 @@
     fn fmt(&self, f: &mut std::fmt::Formatter<'_>) -> std::fmt::Result {
         f.debug_struct("Runtime").field("exec", &"todo").finish()
     }
 }
 enum Pending {
     PostWatch { cb: PostTxnHandler, span: Span },
     NewWatch { watch_entry: RxEntry },
-    Close { id: WatchID, range: bool },
+    Close { id: QueryID, range: bool },
 }
 
 struct _ExecutorTxn {
     last: Stamp,
     txn: Either<Rc<ReadTxn>, Weak<ReadTxn>>,
 }
 
@@ -66,15 +66,15 @@
 
 impl Linkspace {
     pub fn get_reader(&self) -> Rc<ReadTxn> {
         //Rc::new(self.exec.env.get_reader().unwrap())
         self.exec.process_txn.borrow().clone()
     }
     pub fn get_writer(&self) -> WriteTxn2 {
-        if self.exec.written.get() == false {
+        if !self.exec.written.get() {
             tracing::trace!("Set Written true")
         }
         self.exec.written.set(true);
         self.exec.env.get_writer().unwrap()
     }
     pub fn env(&self) -> &BTreeEnv {
         &self.exec.env
@@ -87,31 +87,30 @@
 impl Linkspace {
     fn rt_log_head(&self) -> Stamp {
         self.exec.process_upto.get()
     }
     /** return when next to process.
      Ok(None) means immediatly, Ok(Some(stamp)) means at stamp a watch can be dropped, Err means no current watches
     **/
+    #[instrument(skip(self),ret)]
     fn next_work(&self) -> Result<Option<Stamp>, ()> {
         if self.exec.is_running.get() {
             tracing::warn!("has_work called during work");
             panic!();
             //return true;
         }
         if !self.exec.pending.borrow().is_empty() {
             return Ok(None);
         };
         self.exec.cbs.borrow_mut().0.gc(now()).ok_or(()).map(Some)
     }
-    #[must_use]
     pub fn new(env: BTreeEnv, spawner: Rc<dyn LocalAsync>) -> Linkspace {
         Self::new_opt_rt(env, OnceCell::from(spawner))
     }
 
-    #[must_use]
     pub fn new_opt_rt(env: BTreeEnv, spawner: OnceCell<Rc<dyn LocalAsync>>) -> Linkspace {
         let reader = env.get_reader().unwrap();
         let at = reader.log_head();
         Linkspace {
             exec: Rc::new(Executor {
                 env,
                 written: Cell::new(false),
@@ -126,34 +125,34 @@
         }
     }
 
     pub fn insert_watch(&self, watch_entry: RxEntry) {
         match self.exec.cbs.try_borrow_mut() {
             Ok(mut lk) => {
                 if let Some(w) = lk.0.register(watch_entry) {
-                    drop_watch(w, &self, StopReason::Replaced)
+                    drop_watch(w, self, StopReason::Replaced)
                 }
             }
             Err(_) => self
                 .exec
                 .pending
                 .borrow_mut()
                 .push(Pending::NewWatch { watch_entry }),
         };
     }
     pub fn drain_pending(&self, lk: &mut (Matcher, PostTxnList)) {
         for cmd in self.exec.pending.borrow_mut().drain(..) {
             match cmd {
                 Pending::NewWatch { watch_entry } => {
                     if let Some(w) = lk.0.register(watch_entry) {
-                        drop_watch(w, &self, StopReason::Replaced)
+                        drop_watch(w, self, StopReason::Replaced)
                     }
                 }
                 Pending::Close { id, range } => {
-                    lk.0.deregister(&id, range, |w| drop_watch(w, &self, StopReason::Closed));
+                    lk.0.deregister(&id, range, |w| drop_watch(w, self, StopReason::Closed));
                 }
                 Pending::PostWatch { cb, span } => lk.1.push((cb, span)),
             }
         }
     }
     pub async fn poll(&self) -> Stamp {
         loop {
@@ -170,103 +169,77 @@
             if let Some(v) = self.inner().log_head.next_d(None) {
                 if self.rt_log_head().get() < v {
                     self.process();
                 }
             }
         }
     }
-    fn watch_state(&self,id:&WatchIDRef) -> Option<(u32,usize)>{
+
+    fn watch_status(&self,id:&QueryIDRef) -> Option<WatchStatus>{
         let cbs = self.exec.cbs.borrow();
-        let e = cbs.0.get(id)?;
-        Some((e.nth_query,e.entry_id))
+        Some(cbs.0.get(id)?.status())
     }
 
     /**
-    continiously trigger watch callbacks unless
-    - max_wait has elapsed between new packets - return false
-    - until time has been reached - returns false
-    - watch_id has matched at least once - returns true
-    - no more watch callbacks exists - returns true
+    continuously process callbacks until:
+    - now > last_step => returns 0
+    - qid = Some and qid is matched => if removed 1, if waiting for more -1
+    - qid = None => no more callbacks (1) 
      **/
     #[instrument(skip(self))]
     pub fn run_while(
         &self,
-        max_wait: Option<Duration>,
         last_step: Option<Instant>,
-        watch_id: Option<(&WatchIDRef,bool)>
-    ) -> anyhow::Result<bool> {
+        user_qid: Option<&QueryIDRef>
+    ) -> anyhow::Result<isize> {
         if self.exec.is_running.get() {
             bail!("already running")
         }
         tracing::trace!(
             last_step_in=?last_step.map(|i| i-Instant::now()),
-            ?max_wait,
             "run while");
-        let mut latest_processed_id = Stamp::ZERO;
-        let mut last_new_pkt = Instant::now();
-        let current_state = match watch_id{
-            Some((id,is_done)) => Some((id,is_done,self.watch_state(id).context("watch id not found")?)),
-            None => None
+        let last_new_pkt = Instant::now();
+        let current_state = match user_qid{
+            Some(id) => Some((id,self.watch_status(id).with_context(||anyhow::anyhow!("watch id '{}' not found",AB(id)))?)),
+            _ => None
         };
-        // check the 4 break conditions, and update 'next_check' as required for next check
+        // check the break conditions, and update 'next_check' as required for next check
         loop {
-            let new_recv_id = self.process();
-            if let Some((wid,is_done,(qid,eid))) = current_state{
-                let (v_qid,v_eid) = match self.watch_state(wid){
+            let _log_head = self.process();
+            if let Some((user_qid,old_status)) = current_state{
+                let status = match self.watch_status(user_qid){
                     Some(v) => v,
                     None => {
                         tracing::debug!("watch was dropped");
-                        return Ok(true);
+                        return Ok(1);
                     }
                 };
-                if v_eid != eid { tracing::debug!("Watch was overwritten"); return Ok(true);}
-                if !is_done && v_qid != qid { tracing::debug!("Watch was triggered (is_done=false)"); return Ok(true);}
+                if status.watch_id != old_status.watch_id { tracing::debug!("Watch was overwritten"); return Ok(1);}
+                if status.nth_query != old_status.nth_query { tracing::debug!("Watch was triggered (is_done=false)"); return Ok(-1);}
             }
             let mut next_check = last_new_pkt + Duration::from_micros(Stamp::MAX.get());
             let newtime = Instant::now();
             let d = |i| i-newtime;
 
             if let Some(term) = last_step {
                 let wait_dur = match term.checked_duration_since(newtime) {
                     Some(v) => v,
                     None => {
                         tracing::debug!("last_step reached");
-                        return Ok(false);
+                        return Ok(0);
                     }
                 };
                 let last_step_constraint = newtime+wait_dur;
                 tracing::trace!(
                     next_check=?d(next_check),
                     last_step_constraint=?d(last_step_constraint),
                     "set Until constraining");
                 next_check = next_check.min(last_step_constraint);
             }
 
-            if latest_processed_id == new_recv_id {
-                // wait condition depends on last update
-                if let Some(mw) = max_wait {
-                    let wait_next = match last_new_pkt.add(mw).checked_duration_since(newtime) {
-                        Some(v) => newtime + v,
-                        None => {
-                            tracing::debug!("max_wait reached");
-                            return Ok(false);
-                        }
-                    };
-                    tracing::trace!(
-                        next_check=?d(next_check),
-                        wait_next =?d(next_check),
-                        "Set no_new_packet constraint"
-                    );
-                    next_check = next_check.min(wait_next);
-                }
-            } else {
-                latest_processed_id = new_recv_id;
-                last_new_pkt = newtime;
-            }
-
             match self.next_work() {
                 Ok(Some(next_oob)) => {
                     if next_oob != Stamp::MAX {
                         match next_oob.get().checked_sub(now().get()) {
                             Some(micros) => {
                                 let next_recv_oob = newtime + Duration::from_micros(micros);
                                 tracing::trace!(
@@ -281,15 +254,15 @@
                     }
                 }
                 Ok(None) => {
                     continue;
                 }
                 Err(_) => {
                     tracing::debug!("no more callbacks");
-                    return Ok(true);
+                    return Ok(1);
                 }
             };
 
             tracing::debug!(wakeup=?d(next_check), "waiting for new event");
             self.inner().log_head.next_d(Some(next_check));
         }
     }
@@ -318,38 +291,38 @@
                 return rx_last;
             }
             (txn.clone(), rx_last, txn_last)
         };
         let _g = tracing::error_span!("Processing txn", ?from, ?upto).entered();
         let txn = txn;
         tracing::trace!("Lock cbs");
-        let mut lk = self.exec.cbs.borrow_mut();
-        self.drain_pending(&mut lk);
+        let mut lock = self.exec.cbs.borrow_mut();
+        self.drain_pending(&mut lock);
         self.exec.is_running.set(true);
         let i = 0;
         let mut count = Rc::strong_count(&txn);
         let mut validate = || {
             if Rc::strong_count(&txn) != count {
                 warn!("holding txn");
             }
             count = Rc::strong_count(&txn)
         };
         for pkt in txn.pkts_after(from) {
             if pkt.net_header().flags.contains(NetFlags::SILENT) {
                 tracing::trace!("(not) skipping silent pkt - TODO make this a option");
             }
-            let _g = tracing::error_span!("Matching",logptr=?pkt.recv,pkt=%pkt_fmt(&pkt.pkt)).entered();
+            let _g = tracing::error_span!("Matching",logptr=?pkt.recv,pkt=%PktFmt(&pkt.pkt)).entered();
             tracing::debug!("Testing New Pkt");
 
             let pkt = ShareArcPkt {
                 arc: OnceCell::new(),
                 pkt,
             };
 
-            lk.0.trigger(
+            lock.0.trigger(
                 *pkt,
                 |p| {
                     let r = p.handle_pkt(&pkt, self);
                     validate();
                     r
                 },
                 |w| {
@@ -359,37 +332,37 @@
                         StopReason::Finish
                     };
                     drop_watch(w, self, reason)
                 },
             );
         }
         tracing::debug!(npkts = i, "Updated Finished");
-        self.drain_pending(&mut lk);
-        // We don't do things setup in post_funcs
-        lk.1.drain_filter(|(func, span)| {
+        self.drain_pending(&mut lock);
+        // We don't do any setup in post_funcs
+        lock.1.retain_mut(|(func, span)| {
             let _ = span.enter();
             {
                 let cont = func(from, &this);
                 tracing::info!(?cont, "PostTxn");
                 validate();
-                cont.is_break()
+                cont.is_continue()
             }
         });
         self.exec.is_running.set(false);
         self.exec.process_upto.set(upto);
-        std::mem::drop((txn, lk));
+        std::mem::drop((txn, lock));
         if self.exec.written.get() {
             tracing::trace!("Written true");
-            return self.process();
+            self.process()
         } else {
             upto
         }
     }
 
-    pub fn read<F>(&self, hash: LkHash, rx: F, watchid: WatchID, span: Span) -> anyhow::Result<()>
+    pub fn read<F>(&self, hash: LkHash, rx: F, watchid: QueryID, span: Span) -> anyhow::Result<()>
     where
         F: FnOnce(&dyn NetPkt, &Linkspace) + 'static,
     {
         let reader = self.get_reader();
         if let Some(dbp) = reader.read(&hash)? {
             let _g = tracing::debug_span!(parent: &span, "Local").entered();
             rx(&dbp, self);
@@ -409,53 +382,53 @@
     }
     /// automatically handle the options 'follow', 'start', 'mode', and 'id'
     pub fn watch_query(
         &self,
         query: &Query,
         onmatch: impl PktStreamHandler + 'static,
         span: Span,
-    ) -> anyhow::Result<u32> {
+    ) -> anyhow::Result<i32> {
         let mode = query.get_mode()?;
-        let id = query.id().transpose()?.context("watch_query now always requires the :id option")?;
+        let id = query.qid().transpose()?.context("watch always requires the :id option")?;
         let follow = query.get_known_opt(KnownOptions::Follow);
         let start = None; //query.get_known_opt(KnownOptions::Start).map(|v| Ptr::try_from(v.clone())).transpose()?;
                           // TODO span should already have these fields.
         let span = tracing::debug_span!(parent: &span, "with_opts", id=?AB(id), ?follow, ?mode, ?start);
         match follow {
             Some(_p) => {
                 let onmatch = FollowHandler { inner: onmatch };
                 Ok(self.watch(
                     id,
                     mode,
-                    Cow::Borrowed(&query),
+                    Cow::Borrowed(query),
                     onmatch,
                     start,
                     span,
                 )?)
             }
             None => Ok(self.watch(
                 id,
                 mode,
-                Cow::Borrowed(&query),
+                Cow::Borrowed(query),
                 onmatch,
                 start,
                 span,
             )?),
         }
     }
     /// only checks predicates, does not handle any options.
     pub fn watch(
         &self,
-        watch_id: &WatchIDRef,
+        watch_id: &QueryIDRef,
         mode: query_mode::Mode,
         q: Cow<Query>,
         mut onmatch: impl PktStreamHandler + 'static,
         start: Option<LkHash>,
         span: Span,
-    ) -> anyhow::Result<u32> {
+    ) -> anyhow::Result<i32> {
         if start.is_some() {
             panic!("todo")
         }
         let span = debug_span!(parent:&span,"query", preds=%q.predicates);
         let mut counter = 0;
         let check_db = q.predicates.state.check_db();
         self.close(watch_id); // this is not ideal. But other close semantics seem worse.
@@ -463,33 +436,33 @@
             let local_span = tracing::debug_span!(parent: &span, "DB Callback").entered();
             tracing::trace!(?mode);
             let reader = self.get_reader();
             let r = reader
                 .query(mode, &q.predicates, &mut counter)?
                 .try_for_each(|dbp| {
                     let _g = local_span.enter();
-                    tracing::debug!(pkt=%pkt_fmt(&dbp.pkt),"Match");
+                    tracing::debug!(pkt=%PktFmt(&dbp.pkt),"Match");
                     onmatch.handle_pkt(&dbp, self)
                 });
             if Rc::strong_count(&reader) > 2 {
                 warn!("Holding txn open");
             }
             tracing::debug!(?r,"Done with DB");
             if matches!(r, ControlFlow::Break(_)) {
-                return Ok(counter);
+                return Ok(crate::saturating_cast(counter))
             }
         }
         match RxEntry::new(watch_id.to_vec(), q.into_owned(), counter, Box::new(onmatch), span) {
             Ok(e) => {
                 tracing::debug!("Setup Watch");
                 self.insert_watch(e)
             }
             Err(r) => tracing::info!(e=?r,"Did not register"),
         }
-        Ok(counter)
+        Ok(crate::saturating_neg_cast(counter))
     }
 
     /// Add a function to be run after a txn.
     /// Will run during _this_ transaction.
     /// But any further mutations are ignored this transaction.
     pub fn add_post_txn(&self, cb: PostTxnHandler, span: Span) {
         match self.exec.cbs.try_borrow_mut() {
@@ -500,32 +473,32 @@
                 .borrow_mut()
                 .push(Pending::PostWatch { cb, span }),
         }
     }
     pub fn inner(&self) -> &BTreeEnv {
         &self.exec.env
     }
-    pub fn close(&self, id: impl AsRef<WatchIDRef>) {
+    pub fn close(&self, id: impl AsRef<QueryIDRef>) {
         match self.exec.cbs.try_borrow_mut() {
             Ok(mut lk) => {
                 lk.0.deregister(id.as_ref(), false, |w| {
-                    drop_watch(w, &self, StopReason::Closed)
+                    drop_watch(w, self, StopReason::Closed)
                 });
             }
             Err(_) => self.exec.pending.borrow_mut().push(Pending::Close {
                 id: id.as_ref().to_vec(),
                 range: false,
             }),
         }
     }
-    pub fn close_range(&self, prefix: impl AsRef<WatchIDRef>) {
+    pub fn close_range(&self, prefix: impl AsRef<QueryIDRef>) {
         match self.exec.cbs.try_borrow_mut() {
             Ok(mut lk) => {
                 lk.0.deregister(prefix.as_ref(), true, |w| {
-                    drop_watch(w, &self, StopReason::Closed)
+                    drop_watch(w, self, StopReason::Closed)
                 });
             }
             Err(_) => self.exec.pending.borrow_mut().push(Pending::Close {
                 id: prefix.as_ref().to_vec(),
                 range: true,
             }),
         }
```

### Comparing `linkspace-0.1.4/local_dependencies/linkspace-common/src/runtime/threads.rs` & `linkspace-0.3.0rc2/local_dependencies/linkspace-common/src/runtime/threads.rs`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 use crate::prelude::LocalAsync;
 use futures::channel::mpsc::*;
 use futures::{
     executor::LocalPool,
     task::{LocalSpawnExt, SpawnError},
     Future, StreamExt,
 };
-use linkspace_core::env::BTreeEnv;
+use linkspace_core::env::lmdb::BTreeEnv;
 use std::rc::Rc;
 
 pub fn attach(env: BTreeEnv, spawner: Rc<dyn LocalAsync>) -> Linkspace {
     let rx = Linkspace::new(env, spawner.clone());
     let rx2 = rx.clone();
     spawner
         .spawn_local(async move {
```

### Comparing `linkspace-0.1.4/local_dependencies/linkspace-common/src/tests.rs` & `linkspace-0.3.0rc2/local_dependencies/linkspace-common/src/tests.rs`

 * *Files identical despite different names*

### Comparing `linkspace-0.1.4/local_dependencies/linkspace-pkt/Cargo.toml` & `linkspace-0.3.0rc2/local_dependencies/linkspace-pkt/Cargo.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,31 +1,39 @@
 [package]
 name = "linkspace-pkt"
-version = "0.1.1"
-edition = "2021"
-license = "MPL-2.0"
-authors = ["Azon <AntonSol919@gmail.com>"]
-repository = "https://github.com/AntonSol919/linkspace"
 categories = []
 keywords = ["linkspace"]
 description = "Library for reading and writing linkspace packets"
 
+version= "0.3.0-rc1"
+authors= ["Anton Sol <AntonSol919@gmail.com>"]
+edition= "2021"
+license= "MPL-2.0"
+homepage= "https://www.linkspace.dev"
+documentation= "https://www.linkspace.dev/docs/guide/index.html"
+repository= "https://github.com/AntonSol919/linkspace"
+resolver = "2"
 
 [features]
-default=["serde", "keygen"]
-keygen=["linkspace-cryptography/keygen"]
-
+default = ["abe"]
+abe = []
 [dependencies]
-static_assertions = "1.1.0"
-auto_impl = "1.0.1"
-linkspace-cryptography = { path = "../linkspace-cryptography", version = "0.1.0"}
-byte-fmt = { path = "../byte-fmt", version = "0.1.0"}
-serde = { version = "1.0.131", features = ["derive"], default-features = false, optional = true }
-thiserror = "1.0.31"
-bytes = "1.1.0"
-bitflags = "1.3.2"
-triomphe = "0.1.8"
-arrayvec = "0.7.2"
-anyhow = "1.0.69"
+linkspace-cryptography = { path = "../linkspace-cryptography", version = "0.3.0-rc1"}
+byte-fmt = { path = "../byte-fmt", version = "0.3.0-rc1"}
+
+serde= "=1.0.160"
+thiserror=  "=1.0.40"
+arrayvec= "=0.7.2  "
+anyhow= "=1.0.71"
+static_assertions= "=1.1.0"
+auto_impl= "=1.0.1"
+bytes= "=1.1.0"
+bstr= {version = "1.5.0" ,default-features=false}
+bitflags= "=1.3.2"
+
+
+triomphe = { version = "0.1.8-fn", git = "https://github.com/AntonSol919/triomphe"}
 
 [target.'cfg(target_arch = "wasm32")'.dependencies]
 wasm-bindgen = "0.2.80"
+
+
```

### Comparing `linkspace-0.1.4/local_dependencies/linkspace-pkt/LICENSE` & `linkspace-0.3.0rc2/local_dependencies/abe/LICENSE`

 * *Files identical despite different names*

### Comparing `linkspace-0.1.4/local_dependencies/linkspace-pkt/src/builder.rs` & `linkspace-0.3.0rc2/local_dependencies/linkspace-pkt/src/builder.rs`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 use crate::*;
 
 pub fn datapoint(data: &[u8], netopts: impl Into<NetOpts>) -> NetPktParts<'_> {
     try_datapoint_ref(data, netopts.into()).unwrap()
 }
 pub fn try_datapoint_ref(data: &[u8], netopts: NetOpts) -> Result<NetPktParts<'_>, Error> {
     let pkt_parts = PointParts {
-        pkt_header: PointHeader::new(PointTypeFlags::DATA_POINT, data.len())?,
+        pkt_header: PointHeader::new_content_len(PointTypeFlags::DATA_POINT, data.len())?,
         fields: PointFields::DataPoint(data),
     };
     let hash = pkt_parts.compute_hash();
     Ok(NetPktParts {
         net_header: netopts.into(),
         hash,
         point_parts: pkt_parts,
@@ -99,19 +99,18 @@
     links: &'t [Link],
     data: &'t [u8],
     stamp: Stamp,
 ) -> Result<(PointHeader, LinkPoint<'t>), Error> {
     ipath.check_components().unwrap();
     let tail = Tail { links, data, ipath };
     let ipath_size = ipath.ipath_bytes().len();
-    let offset_ipathu =
-        size_of::<PointHeader>() + size_of::<LinkPointHeader>() + (links.len() * size_of::<Link>());
-    let offset_ipath = U16::new(offset_ipathu as u16);
-    let offset_data = U16::new((offset_ipathu + ipath_size) as u16);
-    let pkt_header = PointHeader::new(
+    let offset_ipathu = (size_of::<PointHeader>() + size_of::<LinkPointHeader>()).saturating_add(std::mem::size_of_val(links));
+    let offset_ipath = U16::new( offset_ipathu.try_into().map_err(|_| Error::ContentLen)?);
+    let offset_data = U16::new((offset_ipathu + ipath_size).try_into().map_err(|_| Error::ContentLen)?);
+    let pkt_header = PointHeader::new_content_len(
         PointTypeFlags::LINK_POINT,
         size_of::<LinkPointHeader>() + tail.byte_len(),
     )?;
     let sp = LinkPoint {
         head: LinkPointHeader {
             info: LinkPointInfo {
                 offset_ipath,
@@ -155,39 +154,27 @@
     ipath: &'t IPath,
     links: &'t [Link],
     data: &'t [u8],
     stamp: Stamp,
     signkey: &SigningKey,
     netopts: NetOpts,
 ) -> Result<NetPktParts<'t>, Error> {
-    let (linkpoint_pkt_header, sp) = linkp(group, domain, ipath, links, data, stamp)?;
+    let (pkt_header, lp_head) = linkp(group, domain, ipath, links, data, stamp)?;
+    let pkt_header = PointHeader::new_point_size(
+        pkt_header.point_type | PointTypeFlags::SIGNATURE ,
+        pkt_header.uset_bytes.get() as usize + size_of::<Signed>()
+    )?;
     let linkpoint_hash = PointParts {
-        pkt_header: linkpoint_pkt_header,
-        fields: PointFields::LinkPoint(sp),
-    }
-    .compute_hash();
+        pkt_header,
+        fields: PointFields::LinkPoint(lp_head),
+    }.compute_hash();
     let signature = linkspace_cryptography::sign_hash(signkey, &linkpoint_hash.0).into();
     let pkt_parts = PointParts {
-        pkt_header: PointHeader::new(
-            PointTypeFlags::KEY_POINT,
-            size_of::<KeyPointHeader>() + sp.tail.byte_len(),
-        )?,
-        fields: PointFields::KeyPoint(KeyPoint {
-            head: KeyPointHeader {
-                reserved: KeyPointPadding::default(),
-                signed: Signed {
-                    pubkey: signkey.pubkey(),
-                    signature,
-                    linkpoint_hash,
-                },
-                inner_point: linkpoint_pkt_header,
-                linkpoint: sp.head,
-            },
-            tail: sp.tail,
-        }),
+        pkt_header,
+        fields: PointFields::KeyPoint(lp_head,Signed{ pubkey: signkey.pubkey(), signature })
     };
     let hash = pkt_parts.compute_hash();
     Ok(NetPktParts {
         net_header: netopts.into(),
         hash,
         point_parts: pkt_parts,
     })
@@ -195,17 +182,35 @@
 
 pub fn errorpoint(error: &[u8], netopts: impl Into<NetOpts>) -> NetPktParts<'_> {
     __error_blk_ref(error, netopts.into())
 }
 
 fn __error_blk_ref(error: &[u8], netopts: NetOpts) -> NetPktParts<'_> {
     let pkt_parts = PointParts {
-        pkt_header: PointHeader::new(PointTypeFlags::ERROR_POINT, error.len()).unwrap(),
+        pkt_header: PointHeader::new_content_len(PointTypeFlags::ERROR_POINT, error.len()).unwrap(),
         fields: PointFields::Error(error),
     };
     let hash = pkt_parts.compute_hash();
     NetPktParts {
         net_header: netopts.into(),
         hash,
         point_parts: pkt_parts,
     }
 }
+
+/// Calculate the free space left in bytes. Negative values means it will not fit.
+#[inline]
+#[allow(clippy::as_conversions)]
+pub const fn calc_free_space(
+    path: &SPath,
+    links: &[Link],
+    data : &[u8],
+    signed:bool
+) -> isize {
+    let mut size = if signed { MAX_KEYPOINT_DATA_SIZE } else { MAX_LINKPOINT_DATA_SIZE} as isize;
+    size = size.saturating_sub_unsigned(links.len() * std::mem::size_of::<Link>());
+    if !path.spath_bytes().is_empty(){
+        size = size.saturating_sub_unsigned(path.spath_bytes().len() + 8);
+    }
+    size = size.saturating_sub_unsigned(data.len());
+    size
+}
```

### Comparing `linkspace-0.1.4/local_dependencies/linkspace-pkt/src/byte_segments.rs` & `linkspace-0.3.0rc2/local_dependencies/linkspace-pkt/src/byte_segments.rs`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,32 @@
 // Copyright Anton Sol
-//
 // This Source Code Form is subject to the terms of the Mozilla Public
 // License, v. 2.0. If a copy of the MPL was not distributed with this
 // file, You can obtain one at https://mozilla.org/MPL/2.0/.
 /**
 Utility to create packets from multiple byte slices without allocating.
 **/
-#[derive(Copy, Clone)]
+#[derive(Clone,Debug)]
 pub struct ByteSegments<'a>(pub(crate) [&'a [u8]; 8]);
 
 impl<'a> ExactSizeIterator for ByteSegments<'a> {
     #[inline(always)]
     fn len(&self) -> usize {
-        self.0.iter().fold(0, |a, b| a + b.len())
+        // Wrapping ok because Self is only created from valid packets. 
+        self.0.iter().fold(0, |a, b| a.wrapping_add( b.len()))
+    }
+    #[inline]
+    fn is_empty(&self) -> bool {
+        self.0 == [&[] as &[u8];8]
     }
 }
+
 impl<'a> Iterator for ByteSegments<'a> {
     type Item = u8;
+    #[inline]
     fn size_hint(&self) -> (usize, Option<usize>) {
         let len = self.len();
         (len, Some(len))
     }
     #[inline(always)]
     fn next(&mut self) -> Option<Self::Item> {
         if let Some((h, tail)) = self.0[0].split_first() {
@@ -67,53 +73,56 @@
     assert_eq!(b.len(), len);
     assert_eq!(b, b"helloworld")
 }
 
 impl<'a> ByteSegments<'a> {
     #[inline(always)]
     pub const fn from_array<const N: usize>(segments: [&'a [u8]; N]) -> Self {
-        assert!(N < 8);
-        let mut r = [&[] as &'a [u8]; 8];
+        assert!(N < 8,"not supported");
+        let mut r : [&'a [u8];8]= [&[]; 8];
         let mut i = 0;
         while i < N {
             r[i] = segments[i];
-            i += 1;
+            i = i.wrapping_add(1);
         }
         ByteSegments(r)
     }
+    #[inline]
     pub const fn as_slice(&self) -> &[&'a [u8]] {
         &self.0
     }
 
     #[must_use]
     #[inline(always)]
     pub(crate) fn push_front(self, head: &'a [u8]) -> Self {
         let [a, b, c, d, e, f, g, h] = self.0;
-        debug_assert!(h.is_empty());
+        debug_assert!(h.is_empty(), "segmented packet construction stacked to deep");
         ByteSegments([head, a, b, c, d, e, f, g])
     }
+    #[inline]
     pub fn to_bytes(self) -> Box<[u8]> {
         self.0.concat().into_boxed_slice()
     }
 
     /// # Safety
     ///
     /// dest needs to be initialized to fit the entire length;
     #[inline(always)]
-    pub unsafe fn write_segments_unchecked(self, mut dest: *mut u8) {
+    pub const unsafe fn write_segments_unchecked(self, mut dest: *mut u8)  -> *mut u8{
         let mut i = 0;
         while i < 8 {
             let len = self.0[i].len();
             core::ptr::copy_nonoverlapping(self.0[i].as_ptr(), dest, len);
             dest = dest.add(len);
-            i += 1;
+            i = i.wrapping_add(1);
         }
+        dest
     }
     #[inline(always)]
     pub fn io_slices(self) -> [std::io::IoSlice<'a>; 8] {
         self.0.map(std::io::IoSlice::new)
     }
     #[inline(always)]
     pub fn write_into(self, mut dest: impl std::io::Write) -> std::io::Result<()> {
-        dest.write_all_vectored(&mut self.0.map(std::io::IoSlice::new))
+        dest.write_all_vectored(&mut self.io_slices())
     }
 }
```

### Comparing `linkspace-0.1.4/local_dependencies/linkspace-pkt/src/eval.rs` & `linkspace-0.3.0rc2/local_dependencies/linkspace-pkt/src/eval.rs`

 * *Files 12% similar despite different names*

```diff
@@ -2,32 +2,34 @@
 //
 // This Source Code Form is subject to the terms of the Mozilla Public
 // License, v. 2.0. If a copy of the MPL was not distributed with this
 // file, You can obtain one at https://mozilla.org/MPL/2.0/.
 use crate::*;
 use anyhow::{anyhow, bail, Context};
 use byte_fmt::abe::ast::Ctr;
+use byte_fmt::abe::scope::core_ctx;
 use byte_fmt::abe::{eval::*, ToABE, ABE};
-use byte_fmt::abe::{eval_fnc, fncs};
+use byte_fmt::abe::{scope_macro, fncs};
 
 pub fn pkt_scope(pkt: &dyn NetPkt) -> impl Scope + '_ {
     let pkt_env = EScope(NetPktFieldsEval(pkt));
     let pkt_def = EScope(NetPktPrintDefault(pkt));
     let link_select = EScope(SelectLink(pkt.as_point().get_links()));
     let recv = EScope(RecvStamp { pkt });
     (pkt_env, pkt_def, (link_select, recv))
 }
+
 pub fn pkt_ctx<'o>(ctx: EvalCtx<impl Scope + 'o>, pkt: &'o dyn NetPkt) -> EvalCtx<impl Scope + 'o> {
     ctx.scope(pkt_scope(pkt))
 }
 pub fn opt_pkt_ctx<'o>(
     ctx: EvalCtx<impl Scope + 'o>,
     pkt: Option<&'o dyn NetPkt>,
 ) -> EvalCtx<impl Scope + 'o> {
-    let pkt_scope = pkt.map(|pkt| pkt_scope(pkt));
+    let pkt_scope = pkt.map(pkt_scope);
     ctx.scope(pkt_scope)
 }
 
 #[track_caller]
 pub fn pkt_fmt(pkt: &dyn NetPkt) -> String {
     let ctx = pkt_ctx(core_ctx(), pkt);
     String::from_utf8(abe::eval::eval(&ctx, &DEFAULT_FMT).unwrap().concat()).unwrap()
@@ -79,15 +81,15 @@
     fn list_funcs(&self) -> &[ScopeFunc<&Self>] {
         &fixed_fields_arr!(as_scopefn)
     }
 }
 pub struct NetPktPrintDefault<'o>(&'o dyn NetPkt);
 impl<'o> EvalScopeImpl for NetPktPrintDefault<'o> {
     fn about(&self) -> (String, String) {
-        ("print pkt default".into(), "".into())
+        ("print pkt default".into(), String::new())
     }
     fn list_funcs(&self) -> &[ScopeFunc<&Self>] {
         fncs!([
             ( @C "pkt",0..=0,Some(true),"default pk fmt",|pkt:&Self,_,_,scope| {
                 let ctx = EvalCtx{scope}.scope(pkt_scope(pkt.0));
                 Ok(abe::eval::eval(&ctx,&DEFAULT_FMT).unwrap().concat())
             }, none),
@@ -95,20 +97,31 @@
                 let ctx = EvalCtx{scope}.pre_scope(pkt_scope(pkt.0));
                 Ok(abe::eval::eval(&ctx,&DEFAULT_FMT).unwrap().concat())
             }, none),
             ( @C "point",0..=0,Some(true),"TODO default point fmt",|pkt:&Self,_,_,scope| {
                 let ctx = EvalCtx{scope}.pre_scope(pkt_scope(pkt.0));
                 Ok(abe::eval::eval(&ctx,&DEFAULT_FMT).unwrap().concat())
             }, none),
+            ( @C "pkt-quick",0..=0,Some(true),"same as pkt but without dynamic lookup",|pkt:&Self,_,_,_| {
+                Ok(PktFmt(pkt.0).to_string().into_bytes())
+            }, none),
+
+
+            ( @C "html-quick",0..=0,Some(true),"same as html but without dynamic lookup",|pkt:&Self,_,_,_| {
+                let mut buf = String::new();
+                PktFmt(pkt.0).to_html(&mut buf,true,None)?;
+                Ok(buf.into_bytes())
+            }, none),
+
             ( "netbytes", 0..=0, Some(true),"raw netpkt bytes",|pkt:&Self,_| Ok(pkt.0.byte_segments().to_bytes().into_vec()))
         ])
     }
 }
 
-pub fn lptr(l:&Link)->&Ptr{&l.ptr}
+pub fn lptr(l:&Link)->&LkHash{&l.ptr}
 pub fn ptrv(l:&Link)->Vec<u8>{l.ptr.to_vec()}
 #[derive(Copy,Clone)]
 pub struct SelectLink<'o>(pub &'o [Link]);
 // TODO . this should be done with ExtendedTestOp 
 impl<'o> SelectLink<'o> {
     pub fn first_eq(self,tag:Tag) -> Option<&'o Link>{
         self.0.iter().find(|l| l.tag == tag)
@@ -116,40 +129,40 @@
     pub fn first_tailmask(self,tail:&[u8]) -> Option<&'o Link>{
         self.0.iter().find(|l| l.tag.ends_with(tail))
     }
 }
 
 impl<'o> EvalScopeImpl for SelectLink<'o> {
     fn about(&self) -> (String, String) {
-        ("select link".into(), "".into())
+        ("select link".into(), String::new())
     }
     fn list_funcs(&self) -> &[ScopeFunc<&Self>] {
         fncs!([(
             "*=",
             1..=1,
             "[suffix] get first link with tag ending in suffix",
             |links: &Self, i: &[&[u8]]| {
                 links.first_tailmask(i[0]).map(ptrv).context("no such link")
             }
         )])
     }
-    fn list_eval(&self) -> &[ScopeEval<&Self>] {
-        &[eval_fnc!(
+    fn list_macros(&self) -> &[ScopeMacro<&Self>] {
+        &[scope_macro!(
             "links",
             ":{EXPR} where expr is repeated for each link binding 'ptr' and 'tag'",
             |links: &Self, abe: &[ABE], scope| {
-                let abe = match abe {
-                    &[ABE::Ctr(Ctr::Colon), ref r @ ..] => r,
+                let abe = match &abe {
+                    &[ABE::Ctr(Ctr::Colon), r @ ..] => r,
                     _ => anyhow::bail!("links expects")
                 };
                 let mut out = vec![];
                 for link in links.0 {
                     let ctx = EvalCtx { scope }.scope(EScope(LinkEnv { link }));
                     match eval(&ctx, abe) {
-                        Ok(abl) => match abl.into_exact_bytes() {
+                        Ok(ablist) => match ablist.into_exact_bytes() {
                             Ok(o) => {
                                 out.extend_from_slice(&o);
                             }
                             Err(_e) => bail!("links expects result to be undelimited bytes (fixme)")
                         },
                         Err(e) => return Err(e.into()),
                     }
```

### Comparing `linkspace-0.1.4/local_dependencies/linkspace-pkt/src/field_ids.rs` & `linkspace-0.3.0rc2/local_dependencies/linkspace-pkt/src/field_ids.rs`

 * *Files 3% similar despite different names*

```diff
@@ -69,17 +69,27 @@
         #[repr(u8)]
         /// An enum that provides access to the fields in a [NetPkt]
         pub enum FieldEnum {
             $( $fname = $token ),*
         }
         impl FieldEnum {
             pub const LIST : [FieldEnum;29]= [$(FieldEnum::$fname,)*];
+            pub fn try_from_name(id:&str) -> Option<Self> {
+                match id {
+                    $( $name => Some(FieldEnum::$fname), )*
+                    _ => None
+               }
+            }
             pub fn try_from_id(id:&[u8]) -> Option<Self> {
-                $( if id == &[$token] || id == $name.as_bytes() { return Some(FieldEnum::$fname);})*
-                    None
+                #![allow(non_upper_case_globals)]
+                $(const $fname: &'static [u8] = $name.as_bytes();)*
+                match id {
+                    $( &[$token] | $fname => Some(FieldEnum::$fname), )*
+                    _ => None
+                }
             }
             pub const fn info(self) -> FieldInfo{
                 match self {
                     $(FieldEnum::$fname => as_info::<$fname>() ),*
                 }
             }
         }
@@ -101,15 +111,15 @@
             | FieldEnum::VarUBits0F
             | FieldEnum::VarUBits1F
             | FieldEnum::VarUBits2F
             | FieldEnum::VarUBits3F => U32::try_from(abl).ok().map(|v| v.to_abe()),
             FieldEnum::PubKeyF | FieldEnum::GroupIDF | FieldEnum::PktHashF => {
                 LkHash::try_from(abl).ok().map(|v| v.to_abe())
             }
-            FieldEnum::LinksLenF | FieldEnum::DataSizeF | FieldEnum::PointSizeF => {
+            FieldEnum::LinksLenF | FieldEnum::DataSizeF | FieldEnum::SizeF => {
                 U16::try_from(abl).ok().map(|v| v.to_abe())
             }
             FieldEnum::DomainF => Domain::try_from(abl).ok().map(|v| v.to_abe()),
             FieldEnum::PathComp0F
             | FieldEnum::PathComp1F
             | FieldEnum::PathComp2F
             | FieldEnum::PathComp3F
@@ -131,21 +141,21 @@
     }
 }
 
 use thiserror::Error;
 
 #[derive(Error, Debug)]
 pub enum FieldEnumErr {
-    #[error("No Such field")]
+    #[error("no such field")]
     NoSuchField,
 }
 impl FromStr for FieldEnum {
     type Err = FieldEnumErr;
     fn from_str(s: &str) -> Result<Self, Self::Err> {
-        FieldEnum::try_from_id(s.as_bytes()).ok_or(FieldEnumErr::NoSuchField)
+        FieldEnum::try_from_name(s).ok_or(FieldEnumErr::NoSuchField)
     }
 }
 
 pub const VAR_FIELDS: [FieldEnum; 7] = [
     FieldEnum::VarNetFlagsF,
     FieldEnum::VarHopF,
     FieldEnum::VarStampF,
@@ -161,33 +171,33 @@
     (VarStampF,b's',"stamp" , PointTypeFlags::DATA),
     (VarUBits0F,b'q',"ubits0" , PointTypeFlags::DATA),
     (VarUBits1F,b'Q',"ubits1" , PointTypeFlags::DATA),
     (VarUBits2F,b'w',"ubits2" , PointTypeFlags::DATA),
     (VarUBits3F,b'W',"ubits3" , PointTypeFlags::DATA),
     (PktHashF,b'h',"hash" , PointTypeFlags::DATA),
     (PktTypeF,b'y',"type", PointTypeFlags::DATA),
-    (PointSizeF,b'o',"point_size", PointTypeFlags::DATA ),
+    (SizeF,b'o',"size", PointTypeFlags::DATA ),
     (PubKeyF,b'k',"pubkey",PointTypeFlags::SIGNATURE),
     (SignatureF,b'v',"signature",PointTypeFlags::SIGNATURE),
     (GroupIDF,b'g',"group",PointTypeFlags::LINK),
     (DomainF,b'd',"domain",PointTypeFlags::LINK),
     (CreateF,b'c',"create",PointTypeFlags::LINK),
     (PathLenF,b'x',"path_len",PointTypeFlags::LINK),
     (LinksLenF,b'l',"links_len",PointTypeFlags::LINK),
     (DataSizeF,b'B',"data_size",PointTypeFlags::DATA),
     (PathF,b'p',"path",PointTypeFlags::LINK),
     (IPathF,b'P',"ipath",PointTypeFlags::LINK),
-    (PathComp0F,b'0',"comp0",PointTypeFlags::LINK),
-    (PathComp1F,b'1',"comp1",PointTypeFlags::LINK),
-    (PathComp2F,b'2',"comp2",PointTypeFlags::LINK),
-    (PathComp3F,b'3',"comp3",PointTypeFlags::LINK),
-    (PathComp4F,b'4',"comp4",PointTypeFlags::LINK),
-    (PathComp5F,b'5',"comp5",PointTypeFlags::LINK),
-    (PathComp6F,b'6',"comp6",PointTypeFlags::LINK),
-    (PathComp7F,b'7',"comp7",PointTypeFlags::LINK),
+    (PathComp0F,b'0',"path0",PointTypeFlags::LINK),
+    (PathComp1F,b'1',"path1",PointTypeFlags::LINK),
+    (PathComp2F,b'2',"path2",PointTypeFlags::LINK),
+    (PathComp3F,b'3',"path3",PointTypeFlags::LINK),
+    (PathComp4F,b'4',"path4",PointTypeFlags::LINK),
+    (PathComp5F,b'5',"path5",PointTypeFlags::LINK),
+    (PathComp6F,b'6',"path6",PointTypeFlags::LINK),
+    (PathComp7F,b'7',"path7",PointTypeFlags::LINK),
     (DataF,b'b',"data",PointTypeFlags::DATA)
 ]}
 
 impl FieldEnum {
     pub fn mut_route(self, header: &mut NetPktHeader) -> Option<&mut [u8]> {
         Some(match self {
             FieldEnum::VarNetFlagsF => std::slice::from_mut(header.mut_flags_u8()),
@@ -250,25 +260,23 @@
         .get()),
     (PktHashF, U256, |pkt: &'o T| pkt.hash().into()),
     (PktTypeF, u8, |pkt: &'o T| (pkt
         .as_point()
         .point_header()
         .point_type
         .bits)),
-    (PointSizeF, u16, |pkt: &'o T| (pkt
+    (SizeF, u16, |pkt: &'o T| (pkt
         .as_point()
-        .point_header()
-        .point_size
-        .get())),
-    (DataSizeF, u16, |pkt: &'o T| pkt.as_point().data().len()
-        as u16),
+        .point_header().size()
+        )),
+    (DataSizeF, u16, |pkt: &'o T| pkt.as_point().data().len().try_into().expect("bug: impossible tail")),
     (
         LinksLenF,
         u16,
-        |pkt: &'o T| pkt.as_point().get_links().len() as u16
+        |pkt: &'o T| pkt.as_point().get_links().len().try_into().expect("bug: impossible links")
     ),
     (CreateF, u64, |pkt: &'o T| pkt
         .as_point()
         .get_create_stamp()
         .get()),
     (GroupIDF, U256, |pkt: &'o T| (*pkt.as_point().get_group())
         .into()),
@@ -281,65 +289,61 @@
         .get_signature())
     .into()),
     (PathLenF, u8, |pkt: &'o T| *pkt.as_point().get_path_len())
 ]);
 
 field_ptr!([
     (IPathF, IPath, |pkt: &'o T| pkt.as_point().get_ipath()),
-    (PathF, SPath, |pkt: &'o T| pkt.as_point().get_spath()),
+    (PathF, SPath, |pkt: &'o T| pkt.as_point().get_path()),
     (PathComp0F, [u8], |pkt: &'o T| pkt
         .as_point()
         .get_ipath()
-        .comp0()),
+        .path0()),
     (PathComp1F, [u8], |pkt: &'o T| pkt
         .as_point()
         .get_ipath()
-        .comp1()),
+        .path1()),
     (PathComp2F, [u8], |pkt: &'o T| pkt
         .as_point()
         .get_ipath()
-        .comp2()),
+        .path2()),
     (PathComp3F, [u8], |pkt: &'o T| pkt
         .as_point()
         .get_ipath()
-        .comp3()),
+        .path3()),
     (PathComp4F, [u8], |pkt: &'o T| pkt
         .as_point()
         .get_ipath()
-        .comp4()),
+        .path4()),
     (PathComp5F, [u8], |pkt: &'o T| pkt
         .as_point()
         .get_ipath()
-        .comp5()),
+        .path5()),
     (PathComp6F, [u8], |pkt: &'o T| pkt
         .as_point()
         .get_ipath()
-        .comp6()),
+        .path6()),
     (PathComp7F, [u8], |pkt: &'o T| pkt
         .as_point()
         .get_ipath()
-        .comp7()),
+        .path7()),
     (VarNetFlagsF, NetFlags, |pkt: &'o T| &pkt
         .net_header_ref()
         .flags),
     (VarHopF, U32, |pkt: &'o T| &pkt.net_header_ref().hop),
     (VarStampF, Stamp, |pkt: &'o T| &pkt.net_header_ref().stamp),
     (VarUBits0F, U32, |pkt: &'o T| &pkt.net_header_ref().ubits[0]),
     (VarUBits1F, U32, |pkt: &'o T| &pkt.net_header_ref().ubits[1]),
     (VarUBits2F, U32, |pkt: &'o T| &pkt.net_header_ref().ubits[2]),
     (VarUBits3F, U32, |pkt: &'o T| &pkt.net_header_ref().ubits[3]),
     (PktHashF, LkHash, |pkt: &'o T| pkt.hash_ref()),
     (PktTypeF, PointTypeFlags, |pkt: &'o T| &pkt
         .as_point()
         .point_header_ref()
         .point_type),
-    (PointSizeF, U16, |pkt: &'o T| &pkt
-        .as_point()
-        .point_header_ref()
-        .point_size),
     (CreateF, Stamp, |pkt: &'o T| pkt
         .as_point()
         .get_create_stamp()),
     (GroupIDF, GroupID, |pkt: &'o T| pkt.as_point().get_group()),
     (DomainF, Domain, |pkt: &'o T| pkt.as_point().get_domain()),
     (PubKeyF, PubKey, |pkt: &'o T| pkt.as_point().get_pubkey()),
     (SignatureF, Signature, |pkt: &'o T| pkt
@@ -348,15 +352,15 @@
     (PathLenF, u8, |pkt: &'o T| pkt.as_point().get_path_len())
 ]);
 
 impl FieldEnum {
     pub fn fixed_size(self) -> Option<usize> {
         let v = match self {
             FieldEnum::PathLenF | FieldEnum::PktTypeF | FieldEnum::VarNetFlagsF => 1,
-            FieldEnum::LinksLenF | FieldEnum::DataSizeF | FieldEnum::PointSizeF => 2,
+            FieldEnum::LinksLenF | FieldEnum::DataSizeF | FieldEnum::SizeF => 2,
             FieldEnum::VarHopF
             | FieldEnum::VarUBits0F
             | FieldEnum::VarUBits1F
             | FieldEnum::VarUBits2F
             | FieldEnum::VarUBits3F => 4,
             FieldEnum::CreateF | FieldEnum::VarStampF => 8,
             FieldEnum::DomainF => 16,
@@ -388,15 +392,15 @@
             FieldEnum::VarUBits1F => out.write_all(&VarUBits1F::get_ptr(pkt).0),
             FieldEnum::VarUBits2F => out.write_all(&VarUBits2F::get_ptr(pkt).0),
             FieldEnum::VarUBits3F => out.write_all(&VarUBits3F::get_ptr(pkt).0),
             FieldEnum::PktHashF => out.write_all(&PktHashF::get_ptr(pkt).0),
             FieldEnum::PktTypeF => out.write_all(std::slice::from_ref(
                 &pkt.as_point().point_header_ref().point_type.bits,
             )),
-            FieldEnum::PointSizeF => out.write_all(&PointSizeF::get_ptr(pkt).0),
+            FieldEnum::SizeF => out.write_all( &U16::from(pkt.size()).0),
             FieldEnum::DataSizeF => out.write_all(&DataSizeF::get_val(pkt).to_be_bytes()),
             FieldEnum::LinksLenF => out.write_all(&LinksLenF::get_val(pkt).to_be_bytes()),
             FieldEnum::DomainF => out.write_all(&DomainF::get_ptr(pkt).0),
             FieldEnum::PathF => out.write_all(PathF::get_ptr(pkt).spath_bytes()),
             FieldEnum::IPathF => out.write_all(IPathF::get_ptr(pkt).ipath_bytes()),
             FieldEnum::PathLenF => {
                 out.write_all(std::slice::from_ref(pkt.as_point().get_path_len()))
@@ -423,15 +427,15 @@
             FieldEnum::VarStampF => write!(out, "{}", VarStampF::get_ptr(pkt)),
             FieldEnum::VarUBits0F => write!(out, "{}", VarUBits0F::get_ptr(pkt)),
             FieldEnum::VarUBits1F => write!(out, "{}", VarUBits1F::get_ptr(pkt)),
             FieldEnum::VarUBits2F => write!(out, "{}", VarUBits2F::get_ptr(pkt)),
             FieldEnum::VarUBits3F => write!(out, "{}", VarUBits3F::get_ptr(pkt)),
             FieldEnum::PktHashF => write!(out, "{}", PktHashF::get_ptr(pkt)),
             FieldEnum::PktTypeF => write!(out, "{}", PktTypeF::get_ptr(pkt)),
-            FieldEnum::PointSizeF => write!(out, "{}", PointSizeF::get_ptr(pkt)),
+            FieldEnum::SizeF => write!(out, "{}", SizeF::get_val(pkt)),
             FieldEnum::DataSizeF => write!(out, "{}", DataSizeF::get_val(pkt)),
             FieldEnum::LinksLenF => write!(out, "{}", LinksLenF::get_val(pkt)),
             FieldEnum::DomainF => write!(out, "{}", DomainF::get_ptr(pkt).as_str(true)),
             FieldEnum::PathF => write!(out, "{}", PathF::get_ptr(pkt)),
             FieldEnum::IPathF => write!(out, "{}", IPathF::get_ptr(pkt).spath()),// TODO might be wrong
             FieldEnum::PathLenF => write!(out, "{}", PathLenF::get_ptr(pkt)),
             FieldEnum::PathComp0F => write!(out, "{}", AB(PathComp0F::get_ptr(pkt))),
@@ -467,15 +471,15 @@
             FieldEnum::VarStampF => VarStampF::get_ptr(pkt).to_abe_str(),
             FieldEnum::VarUBits0F => VarUBits0F::get_ptr(pkt).to_abe_str(),
             FieldEnum::VarUBits1F => VarUBits1F::get_ptr(pkt).to_abe_str(),
             FieldEnum::VarUBits2F => VarUBits2F::get_ptr(pkt).to_abe_str(),
             FieldEnum::VarUBits3F => VarUBits3F::get_ptr(pkt).to_abe_str(),
             FieldEnum::PktHashF => PktHashF::get_ptr(pkt).to_abe_str(),
             FieldEnum::PktTypeF => print_abe(U8::new(PktTypeF::get_val(pkt)).abe_bits()),
-            FieldEnum::PointSizeF => PointSizeF::get_ptr(pkt).to_abe_str(),
+            FieldEnum::SizeF => U16::from(SizeF::get_val(pkt)).to_abe_str(),
             FieldEnum::DomainF => DomainF::get_ptr(pkt).to_abe_str(),
             FieldEnum::IPathF => PathF::get_ptr(pkt).to_abe_str(), // TODO might be the wrong choice
             FieldEnum::PathF => PathF::get_ptr(pkt).to_abe_str(),
             FieldEnum::PathLenF => U8::new(PathLenF::get_val(pkt)).to_abe_str(),
             FieldEnum::PathComp0F => AB(PathComp0F::get_ptr(pkt)).to_abe_str(),
             FieldEnum::PathComp1F => AB(PathComp1F::get_ptr(pkt)).to_abe_str(),
             FieldEnum::PathComp2F => AB(PathComp2F::get_ptr(pkt)).to_abe_str(),
@@ -494,16 +498,18 @@
         };
         out.write_all(string.as_bytes())
     }
 }
 
 #[test]
 fn fields(){
+    use abe::scope::*;
     let ipath = ipath_buf(&[b"hello",b"world"]);
     let p = linkpoint([1;32].into(), [2;16].into(), &ipath, &[], &[], now(), ());
     let abe = abe::parse_abe("[path]").unwrap();
     let path = abe::eval::eval(&pkt_ctx(core_ctx(), &p),&abe).unwrap().into_exact_bytes().unwrap();
     let pbox = p.as_netbox();
     let path1 = abe::eval::eval(&pkt_ctx(core_ctx(), &pbox),&abe).unwrap().into_exact_bytes().unwrap();
     assert_eq!(path,ipath.spath_bytes());
     assert_eq!(path,path1)
 }
+
```

### Comparing `linkspace-0.1.4/local_dependencies/linkspace-pkt/src/ipath.rs` & `linkspace-0.3.0rc2/local_dependencies/linkspace-pkt/src/ipath.rs`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 Copyright Anton Sol
 
 This Source Code Form is subject to the terms of the Mozilla Public
 License, v. 2.0. If a copy of the MPL was not distributed with this
 file, You can obtain one at https://mozilla.org/MPL/2.0/.
 */
 use crate::{spath::*, MAX_IPATH_SIZE, MAX_PATH_LEN, MAX_SPATH_COMPONENT_SIZE};
-use std::{borrow::Borrow, ops::Deref};
+use std::{borrow::Borrow, ops::Deref, ptr};
 
 /// An IPath is an [[SPath]] with 8 bytes prefix: (length, \[component_offset;7\])
 #[derive(Copy, Clone, PartialEq, Eq, PartialOrd, Ord, Hash)]
 #[repr(transparent)]
 pub struct IPathBytes<X: ?Sized> {
     ipath_bytes: X,
 }
@@ -32,15 +32,18 @@
 }
 impl<const U: usize> AsRef<IPath> for IPathC<U> {
     fn as_ref(&self) -> &IPath {
         IPath::from_unchecked(&self.ipath_bytes)
     }
 }
 
+
+#[allow(clippy::as_conversions,clippy::cast_possible_truncation)]
 pub const fn ipath1<const C0: usize>(c0: &[u8; C0]) -> IPathC<{ C0 + 9 }> {
+    assert!(C0 < MAX_SPATH_COMPONENT_SIZE );
     let mut r = [0u8; C0 + 9];
     r[0] = 1;
     let mut i = 1;
     while i < 8 {
         r[i] = (C0 + 1) as u8;
         i += 1;
     }
@@ -106,26 +109,28 @@
         IPathBuf { ipath_bytes }
     }
     #[track_caller]
     pub fn append(mut self, component: &[u8]) -> Self {
         self.try_append_component(component).unwrap();
         self
     }
+
+    #[allow(clippy::as_conversions,clippy::cast_possible_truncation)]
     pub fn try_append_component(&mut self, component: &[u8]) -> Result<&mut Self, PathError> {
         let bs = &mut self.ipath_bytes;
         if component.len() > MAX_SPATH_COMPONENT_SIZE {
             return Err(PathError::ComponentSize);
         }
         if component.is_empty() {
             return Err(PathError::ZeroComponent);
         }
         if bs.is_empty() {
             *bs = vec![0; 8]
         }
-        if bs[0] >= MAX_PATH_LEN as u8 {
+        if bs[0] >= MAX_PATH_LEN as u8{
             return Err(PathError::CapacityError);
         }
         if bs.len() + component.len() + 1 > MAX_IPATH_SIZE {
             return Err(PathError::MaxLen);
         }
 
         let new_len = bs[0] + 1;
@@ -186,15 +191,16 @@
     pub const fn ipath_bytes(&self) -> &[u8] {
         &self.ipath_bytes
     }
     pub const fn empty() -> &'static IPath {
         Self::EMPTY
     }
     pub const fn from_unchecked(b: &[u8]) -> &IPath {
-        unsafe { std::mem::transmute(b) }
+
+        unsafe { &*ptr::from_raw_parts(b.as_ptr().cast(), b.len())}
     }
 
     pub const fn check_components(&self) -> Result<(), PathError> {
         if self.ipath_bytes.is_empty() {
             return Ok(());
         }
         if self.ipath_bytes.len() < 8 {
@@ -232,14 +238,15 @@
         Ok(())
     }
 
     pub fn spath(&self) -> &SPath {
         self.fields().2
     }
     #[inline(always)]
+    #[allow(clippy::as_conversions)]
     pub const fn fields(&self) -> (u8, [u8; 9], &SPath) {
         let b = &self.ipath_bytes;
         if b.is_empty() {
             return (0, [0; 9], SPath::empty());
         }
         let (h, spath) = b.split_at(8);
         let len = if spath.len() > 255 {
@@ -252,82 +259,89 @@
             [0, h[1], h[2], h[3], h[4], h[5], h[6], h[7], len],
             SPath::from_unchecked(spath),
         )
     }
 
     /// component count
     pub const fn path_len(&self) -> &u8 {
-        self.ipath_bytes.first().unwrap_or(&0)
+        match self.ipath_bytes.first(){
+            Some(v) => v,
+            None => &0,
+        }
     }
     pub const fn is_empty(&self) -> bool {
         self.len() == 0
     }
     #[allow(clippy::len_without_is_empty)] // wtf?
+    #[allow(clippy::as_conversions)]
     pub const fn len(&self) -> usize {
         *self.path_len() as usize
     }
     pub const fn components(&self) -> [&SPath; 8] {
         pre_idx_comp(&self.ipath_bytes)
     }
 
     pub fn iter(&self) -> impl Iterator<Item = &[u8]> {
         (0..self.len()).map(|i| self.comp(i))
     }
     pub fn comps_bytes(&self) -> [&[u8]; 8] {
         pre_idx_comp(&self.ipath_bytes).map(|b| b.first())
     }
+    #[allow(clippy::as_conversions)]
     pub fn range(&self, r: std::ops::Range<usize>) -> &SPath {
         let (_, segm, bytes) = self.fields();
         let bytes = &bytes.spath_bytes()[segm[r.start] as usize..segm[r.end] as usize];
         SPath::from_unchecked(bytes)
     }
+    #[allow(clippy::as_conversions)]
     pub fn last(&self) -> &[u8] {
         self.comp((*self.path_len() as usize).saturating_sub(1))
     }
     #[inline(always)]
     pub fn comp(&self, i: usize) -> &[u8] {
         static COMPS: [fn(&IPath) -> &[u8]; 8] = [
-            IPath::comp0,
-            IPath::comp1,
-            IPath::comp2,
-            IPath::comp3,
-            IPath::comp4,
-            IPath::comp5,
-            IPath::comp6,
-            IPath::comp7,
+            IPath::path0,
+            IPath::path1,
+            IPath::path2,
+            IPath::path3,
+            IPath::path4,
+            IPath::path5,
+            IPath::path6,
+            IPath::path7,
         ];
         COMPS[i](self)
     }
-    pub const fn comp0(&self) -> &[u8] {
+    pub const fn path0(&self) -> &[u8] {
         pre_idx_comp(&self.ipath_bytes)[0].first()
     }
-    pub const fn comp1(&self) -> &[u8] {
+    pub const fn path1(&self) -> &[u8] {
         pre_idx_comp(&self.ipath_bytes)[1].first()
     }
-    pub const fn comp2(&self) -> &[u8] {
+    pub const fn path2(&self) -> &[u8] {
         pre_idx_comp(&self.ipath_bytes)[2].first()
     }
-    pub const fn comp3(&self) -> &[u8] {
+    pub const fn path3(&self) -> &[u8] {
         pre_idx_comp(&self.ipath_bytes)[3].first()
     }
-    pub const fn comp4(&self) -> &[u8] {
+    pub const fn path4(&self) -> &[u8] {
         pre_idx_comp(&self.ipath_bytes)[4].first()
     }
-    pub const fn comp5(&self) -> &[u8] {
+    pub const fn path5(&self) -> &[u8] {
         pre_idx_comp(&self.ipath_bytes)[5].first()
     }
-    pub const fn comp6(&self) -> &[u8] {
+    pub const fn path6(&self) -> &[u8] {
         pre_idx_comp(&self.ipath_bytes)[6].first()
     }
-    pub const fn comp7(&self) -> &[u8] {
+    pub const fn path7(&self) -> &[u8] {
         pre_idx_comp(&self.ipath_bytes)[7].first()
     }
 }
 
 #[inline(always)]
+#[allow(clippy::as_conversions)]
 const fn pre_idx_comp(b: &[u8]) -> [&SPath; 8] {
     let mut result = [SPath::from_unchecked(b); 8];
     if b.is_empty() {
         return result;
     }
     let (h, rest) = b.split_at(8);
     let p = rest.as_ptr();
@@ -390,7 +404,9 @@
     assert_eq!(it.next().unwrap().unwrap(), b"he");
     assert_eq!(it.next().unwrap().unwrap(), b"llo");
     assert_eq!(it.next(), None);
     sp.check_components().unwrap();
     i.check_components().unwrap();
     //    let arrr = [0,1,2,3,4,5,6,7].map(|v|i.comp(v));
 }
+
+
```

### Comparing `linkspace-0.1.4/local_dependencies/linkspace-pkt/src/lib.rs` & `linkspace-0.3.0rc2/local_dependencies/linkspace-pkt/src/lib.rs`

 * *Files 13% similar despite different names*

```diff
@@ -1,68 +1,70 @@
 // Copyright Anton Sol
 //
 // This Source Code Form is subject to the terms of the Mozilla Public
 // License, v. 2.0. If a copy of the MPL was not distributed with this
 // file, You can obtain one at https://mozilla.org/MPL/2.0/.
+
 #![allow(incomplete_features)]
 #![feature(
+    int_roundings,
+    concat_bytes,
+    exact_size_is_empty,
+    pointer_is_aligned,
+    ptr_from_ref,
+    io_error_other,
+    try_blocks,
+    slice_split_at_unchecked,
     doc_notable_trait,
     thread_local,
-    array_zip,
     slice_from_ptr_range,
-    slice_ptr_get,
     ptr_metadata,
     alloc_layout_extra,
-    const_slice_split_at_not_mut,
     const_option,
     const_try,
     const_option_ext,
     const_slice_index,
-    array_windows,
-    split_array,
-    let_chains,
-    slice_group_by,
-    try_blocks,
-    concat_bytes,
-    never_type,
     iter_advance_by,
-    vec_into_raw_parts,
     generic_const_exprs,
     write_all_vectored,
-    new_uninit,
-    get_mut_unchecked,
-    type_alias_impl_trait,
     lazy_cell
 )]
 pub use byte_fmt::*;
+use byte_fmt::abe::FitSliceErr;
 use core::mem::size_of;
 use core::ops::Deref;
 use core::slice::from_raw_parts;
+use core::fmt::Display;
 use serde::{Deserialize, Serialize};
 pub use spath::*;
 pub use spath_fmt::*;
-use utils::as_bytes;
 
 pub mod byte_segments;
 pub mod eval;
+pub mod consts;
 pub mod exprs;
 pub mod field_ids;
 pub mod ipath;
 pub mod link;
 pub mod netpkt;
 pub mod point;
 pub mod point_parts;
 pub mod point_ptr;
 pub mod repr;
 pub mod spath;
 pub mod spath_fmt;
 pub mod spath_macro;
 pub mod utils;
 pub mod read;
+mod builder;
+mod stamp;
+
+
 
+pub use consts::*;
 pub use byte_segments::*;
 pub use endian_types::*;
 pub use eval::*;
 pub use exprs::*;
 pub use field_ids::*;
 pub use ipath::*;
 pub use linkspace_cryptography::SigningKey;
@@ -70,72 +72,62 @@
 pub use point::*;
 pub use point_parts::*;
 pub use point_ptr::*;
 pub use repr::*;
 pub use spath::*;
 pub use spath_fmt::*;
 pub use stamp::*;
+pub use builder::*;
 
-//#[cfg(test)]
 pub mod asm_tests;
 
-mod builder;
-mod pkt_bytes;
-mod stamp;
-
-pub use builder::*;
-pub use pkt_bytes::*;
 
 // ==== pkt field types
 /// Blake3 hash of the packet content. Alias for `B64<[u8;32]\>`
 pub type LkHash = B64<[u8; 32]>;
 /// Alias for `B64<[u8;32]\>`
-pub type Ptr = B64<[u8; 32]>;
-/// Alias for `B64<[u8;32]\>`
 pub type GroupID = B64<[u8; 32]>;
 /// Alias for `AB<[u8;16]>`
 pub type Domain = AB<[u8; 16]>;
 /// Alias for `AB<[u8;16]>`
 pub type Tag = AB<[u8; 16]>;
 
-/// A [Tag] and [Ptr] 
+/// A [Tag] and [LkHash] 
 #[derive(Copy, Clone, Debug, PartialEq, Eq, Ord, PartialOrd, Hash)]
 #[repr(C, align(4))]
 pub struct Link {
     pub tag: Tag,
     /// Usually a [LkHash], sometimes a [PubKey] or [GroupID]
-    pub ptr: Ptr,
+    pub ptr: LkHash,
+}
+impl From<(Tag,LkHash)> for Link {
+    fn from((tag,ptr): (Tag,LkHash)) -> Self {
+        Link{tag,ptr}
+    }
+}
+impl TryFrom<(&str,LkHash)> for Link {
+    type Error = FitSliceErr;
+
+    fn try_from((tag,ptr): (&str,LkHash)) -> Result<Self, Self::Error> {
+        Ok(Link{tag: Tag::try_fit_byte_slice(tag.as_bytes())?,ptr})
+    }
+}
+impl Display for Link{
+    fn fmt(&self, f: &mut std::fmt::Formatter<'_>) -> std::fmt::Result {
+        write!(f,"{}:{}",self.tag,self.ptr)
+    }
 }
 /// Taproot Schnorr publickey. Alias for `B64<[u8;32]>`
 pub type PubKey = B64<[u8; 32]>;
 /// Taproot Schnorr signature
 pub type Signature = B64<[u8; 64]>;
 /// A Big endian u64 of microseconds since EPOCH
 pub type Stamp = U64;
 
-// === size/len constraints. By Convention '_size' is n bytes . '_len' is number of elements
-pub mod consts {
-    use super::*;
-    use std::mem::size_of;
-
-    pub const MIN_POINT_SIZE: usize = size_of::<LkHash>() + size_of::<PointHeader>();
-    pub const MIN_LINKPOINT_SIZE: usize = MIN_POINT_SIZE + size_of::<LinkPointHeader>();
-    pub const MIN_NETPKT_SIZE: usize = size_of::<NetPktHeader>() + MIN_POINT_SIZE;
-    pub const MAX_NETPKT_SIZE: usize = u16::MAX as usize - 256;
-    pub const MAX_POINT_SIZE: usize =
-        MAX_NETPKT_SIZE - size_of::<NetPktHeader>() + size_of::<LkHash>();
-    pub const MAX_CONTENT_SIZE: usize = MAX_POINT_SIZE - size_of::<PartialNetHeader>();
-    pub const MAX_DATA_SIZE: usize = MAX_CONTENT_SIZE;
-    pub const MAX_LINKS_LEN: usize = (MAX_POINT_SIZE - MAX_SPATH_SIZE) / size_of::<Link>();
-    pub const MAX_SPATH_SIZE: usize = 242;
-    pub const MAX_IPATH_SIZE: usize = MAX_SPATH_SIZE + 8;
-    pub const MAX_SPATH_COMPONENT_SIZE: usize = 200;
-    pub const MAX_PATH_LEN: usize = 8;
-}
-pub use consts::*;
+
 
 /** General trait for accessing point field.
 
 Fields are included in [LkHash].
 
 Various fields are accessed through [[PointExt]]
 
@@ -150,17 +142,19 @@
     fn parts(&self) -> PointParts;
     fn fields(&self) -> PointFields {
         self.parts().fields
     }
     
     fn data(&self) -> &[u8];
     fn tail(&self) -> Option<Tail>;
+    /// Points are padded with upto 7 \xFF bytes and are u64 aligned - this is accessible here for completeness sake.
+    fn padding(&self) -> &[u8];
     /// Return a LinkPointHeader, works for both key and link points.
     fn linkpoint_header(&self) -> Option<&LinkPointHeader>;
-    fn keypoint_header(&self) -> Option<&KeyPointHeader>;
+    fn signed(&self) -> Option<&Signed> ;
     /// A utility function to translate this format into bytes for hashing & io
     fn pkt_segments(&self) -> ByteSegments;
     fn point_header_ref(&self) -> &PointHeader;
 }
 
 impl<T: Point + ?Sized> PointExt for T {}
 
@@ -193,60 +187,60 @@
     }
     fn as_linkpoint(&self) -> Option<LinkPoint> {
         if let PointFields::LinkPoint(a) = self.parts().fields {
             return Some(a);
         }
         None
     }
-    fn as_keypoint(&self) -> Option<KeyPoint> {
-        if let PointFields::KeyPoint(a) = self.parts().fields {
-            return Some(a);
+    fn as_keypoint(&self) -> Option<(LinkPoint,Signed)> {
+        if let PointFields::KeyPoint(a,b) = self.parts().fields {
+            return Some((a,b));
         }
         None
     }
 
     fn group(&self) -> Option<&GroupID> {
         self.linkpoint_header().map(|v| &v.group)
     }
     fn get_group(&self) -> &GroupID {
         self.group().unwrap_or(&B64([0; 32]))
     }
     fn domain(&self) -> Option<&Domain> {
         self.linkpoint_header().map(|v| &v.domain)
     }
     fn get_domain(&self) -> &Domain {
-        self.domain().unwrap_or(&AB([0; 16]))
+        unwrap_or(self.domain(), &AB([0;16]))
     }
     fn create_stamp(&self) -> Option<&Stamp> {
         self.linkpoint_header().map(|v| &v.create_stamp)
     }
     fn get_create_stamp(&self) -> &Stamp {
         self.create_stamp().unwrap_or(&Stamp::ZERO)
     }
     fn signature(&self) -> Option<&Signature> {
-        self.keypoint_header().map(|h| &h.signed.signature)
+        self.signed().map(|h| &h.signature)
     }
 
     fn get_signature(&self) -> &Signature {
         self.signature().unwrap_or(&B64([0; 64]))
     }
 
     fn pubkey(&self) -> Option<&PubKey> {
-        self.keypoint_header().map(|h| &h.signed.pubkey)
+        self.signed().map(|h| &h.pubkey)
     }
 
     fn get_pubkey(&self) -> &PubKey {
         self.pubkey().unwrap_or(&B64([0; 32]))
     }
 
     fn ipath(&self) -> Option<&IPath> {
         self.tail().map(|v| v.ipath)
     }
 
-    fn spath(&self) -> Option<&SPath> {
+    fn path(&self) -> Option<&SPath> {
         self.tail().map(|v| v.ipath.spath())
     }
 
     fn links(&self) -> Option<&[Link]> {
         self.tail().map(|v| v.links)
     }
 
@@ -258,47 +252,51 @@
         self.path_len().unwrap_or(&0)
     }
 
     fn get_ipath(&self) -> &IPath {
         self.ipath().unwrap_or(IPath::EMPTY)
     }
 
-    fn get_spath(&self) -> &SPath {
-        self.spath().unwrap_or_else(|| SPath::empty())
+    fn get_path(&self) -> &SPath {
+        self.path().unwrap_or_else(|| SPath::empty())
     }
 
     fn get_data_str(&self) -> Result<&str, core::str::Utf8Error> {
         std::str::from_utf8(self.data())
     }
     fn get_links(&self) -> &[Link] {
         self.links().unwrap_or_default()
     }
     fn select(&self) -> SelectLink{ SelectLink(self.get_links())}
     fn compute_hash(&self) -> LkHash {
         linkspace_cryptography::hash_segments(&self.pkt_segments().0).into()
     }
-    fn net_pkt_size(&self) -> usize {
-        self.point_header_ref().net_pkt_size()
+    fn aligned_net_pkt_size(&self) -> u16 {
+        self.point_header_ref().size()
+    }
+
+    fn check_private(&self) -> Result<(),crate::Error>{
+        if self.group().copied() == Some(PRIVATE) { Err(crate::Error::PrivateGroup)}
+        else {Ok(())}
     }
 }
 
 use bitflags::bitflags;
 bitflags! {
     #[derive(Serialize,Deserialize)]
     /// Pkt flag indicating its type.
     ///
     /// Only the _POINT combinations are valid in a packet.
     pub struct PointTypeFlags: u8 {
         /// Indicate that the chances of anybody interested in this packet are zero.
         /// Implementations can ignore this, mostly useful for importing many datablocks.
-        const EMPTY = 0b00000000;
-        const ANY_PKT = 0b00000001;
-        const DATA = 0b00000001;
-        const LINK = 0b00000010;
-        const SIGNATURE = 0b00000100;
+        const EMPTY = 0b0000_0000;
+        const DATA = 0b000_00001;
+        const LINK = 0b0000_0010;
+        const SIGNATURE = 0b0000_0100;
         const ERROR = 0b1000_0000;
 
         const DATA_POINT = Self::DATA.bits;
         const LINK_POINT = Self::DATA.bits | Self::LINK.bits;
         const KEY_POINT = Self::DATA.bits | Self::LINK.bits | Self::SIGNATURE.bits;
         const ERROR_POINT = Self::ERROR.bits;
     }
@@ -315,15 +313,15 @@
             PointTypeFlags::LINK_POINT => "LinkPoint",
             PointTypeFlags::KEY_POINT => "KeyPoint",
             PointTypeFlags::ERROR_POINT => "ErrorPoint",
             _ => "UnknownPointType",
         }
     }
     pub fn unchecked_from(b: u8) -> Self {
-        unsafe { std::mem::transmute(b) }
+        unsafe {PointTypeFlags::from_bits_unchecked(b)}
     }
 }
 
 #[track_caller]
 #[deprecated]
 pub const fn as_domain(b: &[u8]) -> Domain {
     ab(b)
@@ -337,64 +335,84 @@
     }
 }
 
 use thiserror::Error;
 
 #[derive(Error, Debug, Clone)]
 pub enum Error {
-    #[error("SPath segments are incorrectly set in the header")]
-    SPathSegmentMismatch,
-    #[error("An unknown pkt type {0} was encountered")]
+    #[error("an unknown pkt type {0} was encountered")]
     UnknownPktType(u8),
-    #[error("The packet length does not agree with tail lengths")]
+    #[error("the packet length does not agree with tail lengths")]
     TailLength,
-    #[error("Invalid SPath")]
+    #[error("invalid path")]
     SPath(#[from] crate::spath::PathError),
-    #[error("Signed Invalid Pkt type")]
+    #[error("signed invalid pkt type")]
     SignedInvalidPkt,
-    #[error("Assert and inner LinkPoint do not agree on length")]
+    #[error("the signed and unsigned header do not agree on length")]
     KeyPointLength,
-    #[error("Hash does not match pkt")]
+    #[error("hash does not match pkt")]
     HashMismatch,
-    #[error("Assert holds invalid signature")]
+    #[error("invalid signature")]
     InvalidSignature,
-    #[error("The memory for this packet has trailing data")]
+    #[error("packet has trailing data")]
     InvalidPktDataLength,
-    #[error("Content len exceeds max")] // TODO ambigues use
+    #[error("content len exceeds max")] // TODO ambigues use
     ContentLen,
-    #[error("Too little data to repr a pkt")]
+    #[error("missing bytes {MIN_NETPKT_SIZE} required to read pkt size")]
     MissingHeader,
-    #[error("Reserved bits not null")]
+    #[error("reserved bits not null")]
     ReservedBitsSet,
-    #[error("Links have a size of 48 bytes. The offset must be wrong")]
+    #[error("The padding bits aren't set right")]
+    PaddingBitsNotU8Max,
+    #[error("bad link size")]
     IndivisableLinkbytes,
-    #[error("Data offset should be between spi_offset and pkt_size")]
+    #[error("data offset should be between spi_offset and pkt_size")]
     DataOffsetIncompatible,
-    #[error("ISPOffset should be after the header")]
+    #[error("offset should be after header")]
     ISPOffsetIncompatible,
-    #[error("The pointheader has its reserved bit set {0}")]
+    #[error("pointheader has reserved bit set {0}")]
     HeaderReservedSet(u8),
+    #[error("missing bytes - pkt is {netpkt_size} long")]
+    MissingBytes{netpkt_size:u16},
+    #[error("the [#:0] group can't be used in this context")]
+    PrivateGroup
 }
-
-/*
-pub fn xor<const N:usize>(mut a: [u8;N],b:&[u8;N]) -> [u8;N]{
-a.iter_mut().zip(b.iter()).for_each(|(a,b)| *a ^= b);
-a
-}
-
-
-pub fn nbytes(nf: &impl NetFields) -> usize {
-nf.pkt_header().pkt_size() + size_of::<PktHash>() + size_of::<RoutingHeader>()
+impl Error {
+    pub fn requires_more(self) -> Option<usize>{
+        match self {
+            Error::MissingHeader => Some(MIN_NETPKT_SIZE),
+            Error::MissingBytes{netpkt_size} => Some(netpkt_size.into()),
+            _ => None
+        }
+    }
+    pub fn io(self) -> std::io::Error { std::io::Error::other(self)}
 }
-pub fn nwords(nf: &impl NetFields) -> usize {
-    (nbytes(nf) + 3) / 4
+impl From<Error> for std::io::Error {
+    fn from(val: Error) -> Self {
+        val.io()
+    }
 }
-*/
+
 
 pub trait SigningExt {
     fn pubkey(&self) -> PubKey;
 }
 impl SigningExt for SigningKey {
     fn pubkey(&self) -> PubKey {
         self.pubkey_bytes().into()
     }
 }
+
+
+// Seems to be better at generating cmov instructions
+#[inline(always)]
+pub const fn unwrap_or<'o,T>(opt:Option<&'o T>, mut default:&'o T) -> &'o T{
+    if let Some(val) = opt {
+        default = val;
+    }
+    default
+}
+
+
+
+
+
```

### Comparing `linkspace-0.1.4/local_dependencies/linkspace-pkt/src/link.rs` & `linkspace-0.3.0rc2/local_dependencies/linkspace-pkt/src/link.rs`

 * *Files 5% similar despite different names*

```diff
@@ -11,16 +11,17 @@
     l.iter()
         .map(|Link { tag, ptr: pointer }| format!("{tag}\t{pointer}"))
         .collect::<Vec<String>>()
         .join("\n")
 }
 
 impl Link {
+    pub const DEFAULT : Link = Link { ptr: B64([0;32]),tag:AB([0;16])};
     #[track_caller]
-    pub fn new(tag: impl AsRef<[u8]>, ptr: impl Into<Ptr>) -> Link {
+    pub fn new(tag: impl AsRef<[u8]>, ptr: impl Into<LkHash>) -> Link {
         Link {
             ptr: ptr.into(),
             tag: ab(tag.as_ref()),
         }
     }
     pub fn try_from(tag: impl AsRef<[u8]>, pointer: LkHash) -> Result<Link, FitSliceErr> {
         AB::try_fit_byte_slice(tag.as_ref()).map(|tag| Link { tag, ptr: pointer })
```

### Comparing `linkspace-0.1.4/local_dependencies/linkspace-pkt/src/netpkt/header.rs` & `linkspace-0.3.0rc2/local_dependencies/linkspace-pkt/src/netpkt/header.rs`

 * *Files 15% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 // License, v. 2.0. If a copy of the MPL was not distributed with this
 // file, You can obtain one at https://mozilla.org/MPL/2.0/.
 use byte_fmt::{
     abe::ToABE,
     endian_types::{U32, U8},
      AB, B64,
 };
+use std::ptr;
 use core::fmt;
 use serde::{Deserialize, Serialize};
 
 use crate::Stamp;
 use std::{cell::Cell };
 
 /// A thread local default net header value when creating new netpackets
@@ -66,14 +67,16 @@
 
 impl fmt::Display for NetPktHeader {
     fn fmt(&self, fmt: &mut fmt::Formatter<'_>) -> fmt::Result {
         write!(fmt, "{}", self.to_abe_str())
     }
 }
 
+
+
 impl Default for NetPktHeader {
     /// DEFAULT_ROUTING_BITS
     fn default() -> Self {
         DEFAULT_ROUTING_BITS.get()
     }
 }
 impl NetPktHeader {
@@ -83,23 +86,23 @@
         stamp: Stamp::MAX,
         hop: U32::ZERO,
         ubits: [U32::ZERO; 4],
     };
 
     #[inline(always)]
     pub const fn as_bytes(&self) -> &[u8; 32] {
-        unsafe { &*(self as *const Self as *const [u8; 32]) }
+        unsafe { &*ptr::from_ref(self).cast::<[u8;32]>()}
     }
     #[inline(always)]
     pub const fn cfrom(b: [u8; 32]) -> Self {
-        unsafe { *(b.as_ptr() as *const [u8; 32] as *const Self) }
+        unsafe { b.as_ptr().cast::<Self>().read_unaligned()}
     }
     #[inline(always)]
     pub const fn cinto(self) -> [u8; 32] {
-        unsafe { *(&self as *const Self as *const [u8; 32]) }
+        unsafe{*ptr::from_ref(&self).cast::<[u8;32]>()}
     }
 
     #[must_use]
     pub fn hop(mut self) -> Self {
         self.hop = self.hop.incr();
         self.flags.remove(NetFlags::ALWAYS_ZERO);
         self
@@ -113,32 +116,32 @@
     #[must_use]
     pub fn and_flags(mut self, remove: NetFlags, insert: NetFlags) -> Self {
         self.flags.remove(remove);
         self.flags.insert(insert);
         self
     }
     pub fn flags_u8(&self) -> &u8 {
-        unsafe { &*(&self.flags as *const NetFlags as *const u8) }
+        unsafe { &*(ptr::from_ref(&self.flags).cast::<u8>()) }
     }
     pub fn mut_flags_u8(&mut self) -> &mut u8 {
-        unsafe { &mut *(&mut self.flags as *mut NetFlags as *mut u8) }
+        unsafe {  &mut *(ptr::from_mut(&mut self.flags).cast::<u8>()) }
     }
 }
 
 use bitflags::bitflags;
 
 bitflags! {
     /// Variable flags used in transit
     #[derive(Serialize,Deserialize)]
     pub struct NetFlags: u8 {
         /// Indicate that the chances of anybody interested in this packet are zero.
         /// Implementations can ignore this, mostly useful for importing many datablocks.
-        const SILENT = 0b00000001;
-        const LINKED_IN_FUTURE_PKT = 0b00000010;
-        const LINKED_IN_PREVIOUS_PKT = 0b00000100;
+        const SILENT = 0b0000_0001;
+        const LINKED_IN_FUTURE_PKT = 0b0000_0010;
+        const LINKED_IN_PREVIOUS_PKT = 0b0000_0100;
         /// Request that this packet is not forwarded
         const DONT_FORWARD = 0b0000_1000;
         const ALWAYS_ZERO = 0b1000_0000;
     }
 }
 impl From<NetFlags> for byte_fmt::endian_types::U8 {
     fn from(val: NetFlags) -> Self {
```

### Comparing `linkspace-0.1.4/local_dependencies/linkspace-pkt/src/netpkt/mod.rs` & `linkspace-0.3.0rc2/local_dependencies/linkspace-pkt/src/netpkt/mod.rs`

 * *Files 8% similar despite different names*

```diff
@@ -15,17 +15,14 @@
 pub use eval::*;
 pub use header::*;
 pub use netpkt_arc::*;
 pub use netpkt_parts::*;
 pub use netpkt_ptr::*;
 pub use partial::*;
 use std::fmt::Debug;
-use triomphe::Arc;
-
-
 /// Heap allocated repr of a [NetPkt].
 pub type NetPktBox = Box<NetPktFatPtr>;
 impl From<&dyn NetPkt> for NetPktBox {
     fn from(value: &dyn NetPkt) -> Self {
         value.as_netbox()
     }
 }
@@ -45,50 +42,58 @@
 pub trait NetPkt: Debug {
     fn as_point(&self) -> &dyn Point;
     fn hash_ref(&self) -> &LkHash;
     fn net_header_ref(&self) -> &NetPktHeader;
     fn net_header_mut(&mut self) -> Option<&mut NetPktHeader> {
         None
     }
+    /**
+    recv is somewhat special.
+    It depends on the context. Reading directly from the database it should return the stamp at which it was inserted.
+    NOTE: Do not rely on this value being unique - in the db or otherwise.
+    */
     fn recv(&self) -> Option<Stamp>;
 
     fn byte_segments(&self) -> ByteSegments;
-    #[inline(always)]
     fn as_netbox(&self) -> NetPktBox {
         use std::alloc;
         let segm = self.byte_segments();
         let b = unsafe {
             let (layout, metadata) = netpktbox_layout(self.as_point().point_header_ref());
             let ptr: *mut u8 = alloc::alloc(layout);
             if ptr.is_null() {
                 alloc::handle_alloc_error(layout);
             }
-            let ptr: *mut NetPktFatPtr =
-                std::ptr::from_raw_parts_mut::<NetPktFatPtr>(ptr as *mut (), metadata);
+            let ptr: *mut NetPktFatPtr =std::ptr::from_raw_parts_mut::<NetPktFatPtr>(ptr.cast(), metadata);
+
             {
-                let s = std::slice::from_raw_parts_mut(ptr as *mut u8, layout.size());
+                let s = std::slice::from_raw_parts_mut(ptr.cast::<u8>(), layout.size());
                 segm.write_segments_unchecked(s.as_mut_ptr());
             }
             Box::from_raw(ptr)
         };
         if cfg!(debug_assertions) {
-            b.thin_netpkt().check::<false>().unwrap();
+            b.thin_netpkt().check(false).unwrap();
         }
         b
     }
     fn as_netarc(&self) -> NetPktArc {
         let h = NetPktPtr {
             net_header: self.net_header(),
             hash: self.hash(),
             point: PointThinPtr(self.as_point().point_header()),
         };
+        
         // TODO. we can avoid this copy
-        let byte_segments = self.byte_segments();
-        let arc = Arc::from_header_and_iter(h, byte_segments.skip(size_of::<NetPktPtr>()));
-        NetPktArc(arc)
+        let mut segments = self.as_point().pkt_segments();
+        segments.0[0] = &segments.0[0][size_of::<PointHeader>()..];
+        let arc = unsafe{NetPktArc::from_header_and_copy(h.into(), false,|o:&mut [u8]| {
+            segments.write_segments_unchecked(o.as_mut_ptr());
+        })}.expect("a copy should be valid");
+        arc
     }
 }
 
 impl<T: NetPkt + ?Sized> NetPkt for &T {
     fn as_point(&self) -> &dyn Point {
         (**self).as_point()
     }
@@ -122,62 +127,71 @@
 
 #[doc(notable_trait)]
 /// Utilities for [NetPkt]
 pub trait NetPktExt
 where
     Self: NetPkt,
 {
+    /// see [NetPkt::recv]
     fn get_recv(&self) -> Stamp {
         self.recv().unwrap_or_else(now)
     }
     fn hash(&self) -> LkHash {
         *self.hash_ref()
     }
     fn net_header(&self) -> NetPktHeader {
         *self.net_header_ref()
     }
-    fn size(&self) -> usize {
-        self.as_point().point_header_ref().net_pkt_size()
+    /// Padded size 
+    fn size(&self) -> u16 {
+        self.as_point().point_header_ref().size()
     }
     fn as_netparts(&self) -> NetPktParts
     where
         Self: Sized,
     {
         NetPktParts::from(self)
     }
+    fn to_default_str(&self) -> String{ PktFmt(&self).to_string()}
 }
 
 impl<T> Point for T where T: NetPktExt{
     
     fn parts(&self) -> PointParts {
         self.as_point().parts()
     }
+    
     fn data(&self) -> &[u8] {
         self.as_point().data()
     }
 
     fn tail(&self) -> Option<Tail> {
         self.as_point().tail()
     }
-
+    fn padding(&self) -> &[u8]{
+        self.as_point().padding()
+    }
+    
     fn linkpoint_header(&self) -> Option<&LinkPointHeader> {
         self.as_point().linkpoint_header()
     }
 
-    fn keypoint_header(&self) -> Option<&KeyPointHeader> {
-        self.as_point().keypoint_header()
-    }
+
 
     fn pkt_segments(&self) -> ByteSegments {
         self.as_point().pkt_segments()
     }
 
     fn point_header_ref(&self) -> &PointHeader {
         self.as_point().point_header_ref()
     }
+
+    fn signed(&self) -> Option<&Signed>  {
+        self.as_point().signed()
+    }
 }
 
 #[test]
 pub fn basic() {
     use crate::NetPkt;
     let _pkt = crate::datapoint(&[], ()).as_netbox();
 }
@@ -195,10 +209,10 @@
         crate::now(),
         (),
     )
     .as_netbox();
     let upto_header_bytes = sp.as_netpkt_bytes()[0..MIN_NETPKT_SIZE].try_into().unwrap();
     let calculated = PartialNetHeader::from(upto_header_bytes)
         .point_header
-        .net_pkt_size();
+        .size();
     assert_eq!(sp.size(), calculated)
 }
```

### Comparing `linkspace-0.1.4/local_dependencies/linkspace-pkt/src/netpkt/netpkt_arc.rs` & `linkspace-0.3.0rc2/local_dependencies/linkspace-pkt/src/netpkt/netpkt_arc.rs`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 // Copyright Anton Sol
 //
 // This Source Code Form is subject to the terms of the Mozilla Public
 // License, v. 2.0. If a copy of the MPL was not distributed with this
 // file, You can obtain one at https://mozilla.org/MPL/2.0/.
-use crate::{NetPkt, NetPktPtr};
+use crate::{NetPkt, NetPktPtr, PartialNetHeader, Error };
 use std::{
-    borrow::Borrow, fmt::Debug, mem::size_of, ops::Deref, ptr::NonNull, sync::atomic::AtomicUsize,
+    borrow::Borrow, fmt::Debug, mem::size_of, ops::Deref, ptr::{ self}, sync::atomic::AtomicUsize,
 };
 use triomphe::{Arc, HeaderSlice};
 
 #[derive(Clone)]
 /// Arc around the byte repr [NetPkt]
 /// 
 /// Send + Sync + cheap Clone, [super::NetPktHeader] is immutable
@@ -43,24 +43,25 @@
     data: HeaderSlice<NetPktPtr, [u8]>,
 }
 
 impl NetPktArcPtr {
     pub fn netpktptr(&self) -> &NetPktPtr {
         &self.0
     }
+    /// Get a look at the outer [NetPktArc] 
     #[inline]
     pub fn with_arc<U>(&self, f: impl FnOnce(&NetPktArc) -> U) -> U {
-        let size = self.as_point().point_header_ref().content_size();
-        let ptr: *const NetPktPtr = { self.netpktptr() as *const NetPktPtr };
-        let inner_arc: *const () =
-            unsafe { (ptr as *const u8).sub(size_of::<AtomicUsize>()) as *const () };
+        let size : usize = self.as_point().point_header_ref().padded_content_size().into();
+        let ptr: *const NetPktPtr = ptr::from_ref(self.netpktptr());
+        let inner_arc : *const () =unsafe{ ptr.cast::<u8>().sub(size_of::<AtomicUsize>()).cast::<()>()};
+
         let inner: *const ArcInner = std::ptr::from_raw_parts(inner_arc, size);
-        let i: NonNull<ArcInner> = NonNull::new(inner as *mut ArcInner).unwrap();
-        let arc: &NetPktArc = unsafe { std::mem::transmute(&i) };
-        f(arc)
+        let ptr : &(*const ArcInner,()) = &(inner,()); // Yes we're casting a reference to a pointer 
+        let npa : &NetPktArc = unsafe { &*std::ptr::from_ref(ptr).cast::<NetPktArc>()};
+        f(npa)
     }
 }
 
 impl Debug for NetPktArcPtr {
     fn fmt(&self, f: &mut std::fmt::Formatter<'_>) -> std::fmt::Result {
         self.with_arc(|a| Debug::fmt(a, f))
     }
@@ -71,31 +72,47 @@
             .field(&Arc::count(&self.0))
             .field(&self.thin_arc().0)
             .finish()
     }
 }
 impl NetPktArc {
     pub fn thin_arc(&self) -> &NetPktArcPtr {
-        unsafe { &*(&self.0.header as *const NetPktPtr as *const NetPktArcPtr) }
+        unsafe { &*(ptr::from_ref(&self.0.header).cast::<NetPktArcPtr>())}
     }
     pub fn into_raw_arc(self) -> *const NetPktArcPtr {
-        Arc::into_raw(self.0) as *const NetPktArcPtr
+        Arc::into_raw(self.0).cast() 
     }
     /// # Safety
     ///
     /// must be created through [Self::into_raw_arc]
     pub unsafe fn from_raw_arc(ptr: *const NetPktArcPtr) -> Self {
         assert!(!ptr.is_null());
-        let size = unsafe { (*ptr).as_point().point_header_ref().content_size() };
-        let inner_arc: *const () =
-            unsafe { (ptr as *const u8).sub(size_of::<AtomicUsize>()) as *const () };
-        let inner: *const ArcInner = std::ptr::from_raw_parts(inner_arc, size);
+        let byte_size : usize = unsafe { (*ptr).as_point().point_header_ref().padded_content_size() }.into();
+        let inner_arc: *const () = ptr.cast::<u8>().sub(size_of::<AtomicUsize>()).cast::<()>();
+        let inner: *const ArcInner = std::ptr::from_raw_parts(inner_arc, byte_size);
         let arc: Arc<HeaderSlice<NetPktPtr, [u8]>> = unsafe { std::mem::transmute(inner) };
         NetPktArc(arc)
     }
+    /// # Safety
+    ///
+    /// copy_from must input the correct bytes.
+    pub unsafe fn from_header_and_copy(partial: PartialNetHeader,skip_hash:bool, copy_from:impl FnOnce(&mut [u8])) -> Result<Self,Error>{
+        let h = crate::NetPktPtr {
+            net_header: partial.net_header,
+            hash: partial.hash,
+            point: crate::PointThinPtr(partial.point_header),
+        };
+        let byte_size : usize= h.point.point_header().padded_content_size().into() ;
+        let arc = triomphe::Arc::from_header_and_fn(
+            h,byte_size,copy_from
+        );
+        let pkt= NetPktArc(arc);
+        pkt.check(skip_hash)?;
+        Ok(pkt)
+    }
 }
 impl Deref for NetPktArc {
     type Target = NetPktArcPtr;
     fn deref(&self) -> &Self::Target {
         self.thin_arc()
     }
 }
@@ -166,15 +183,15 @@
     let boxed = parts.as_netbox();
     let arced = parts.as_netarc();
     let p2 = boxed.as_netparts();
     let p3 = arced.as_netparts();
     assert_eq!(p2.point_parts, p3.point_parts);
     let a2 = boxed.as_netarc();
     use std::mem::size_of_val;
-    assert_eq!(size_of_val(&*a2.0), 32 + 32 + 4 + 5 + 3); // 3 is padding
+    assert_eq!(size_of_val(&*a2.0), 32 + 32 + 4 + 5 + 7); // 3 is padding
     assert_eq!(size_of_val(&*a2.0), size_of_val(&*a2.0));
 
     println!("Outer {:p}", arced.0.heap_ptr());
     println!("Arced {:p}", arced.0);
     println!("arced data {:p}", arced.net_header_ref());
 
     let raw = arced.into_raw_arc();
```

### Comparing `linkspace-0.1.4/local_dependencies/linkspace-pkt/src/netpkt/netpkt_parts.rs` & `linkspace-0.3.0rc2/local_dependencies/linkspace-pkt/src/netpkt/netpkt_parts.rs`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,29 @@
+use std::ptr;
+
 // Copyright Anton Sol
 //
 // This Source Code Form is subject to the terms of the Mozilla Public
 // License, v. 2.0. If a copy of the MPL was not distributed with this
 // file, You can obtain one at https://mozilla.org/MPL/2.0/.
 use crate::*;
 
 
 /// Rust enum repr of a [NetPkt]
-#[derive(Clone, Copy, Debug)]
+#[derive(Clone, Copy, Debug,PartialEq)]
 #[repr(C, align(4))]
 pub struct NetPktParts<'a> {
     pub net_header: NetPktHeader,
     pub(crate) hash: LkHash,
     // we dont give out &mut links to pkt parts, this invalidates the hash
     pub(crate) point_parts: PointParts<'a>,
 }
 impl<'a> NetPktParts<'a> {
     /// The caller must ensure PktHash matches the Pkt
+    #[track_caller]
     pub fn from_unchecked(net_header: NetPktHeader, hash: LkHash, pkt_parts: PointParts<'a>) -> Self {
         debug_assert_eq!(pkt_parts.compute_hash(), hash);
         NetPktParts {
             net_header,
             hash,
             point_parts: pkt_parts,
         }
@@ -46,15 +49,15 @@
     fn net_header_ref(&self) -> &NetPktHeader {
         &self.net_header
     }
     #[inline(always)]
     fn byte_segments(&self) -> ByteSegments {
         let segments = self.point_parts.pkt_segments();
         let head = unsafe {
-            let ptr: *const u8 = self as *const Self as *const u8;
+            let ptr: *const u8 = ptr::from_ref(self).cast();
             core::slice::from_raw_parts(ptr, size_of::<NetPktHeader>() + size_of::<LkHash>())
         };
         segments.push_front(head)
     }
 
     fn as_point(&self) -> &dyn Point {
         &self.point_parts
```

### Comparing `linkspace-0.1.4/local_dependencies/linkspace-pkt/src/netpkt/netpkt_ptr.rs` & `linkspace-0.3.0rc2/local_dependencies/linkspace-pkt/src/netpkt/netpkt_ptr.rs`

 * *Files 6% similar despite different names*

```diff
@@ -2,16 +2,15 @@
 //
 // This Source Code Form is subject to the terms of the Mozilla Public
 // License, v. 2.0. If a copy of the MPL was not distributed with this
 // file, You can obtain one at https://mozilla.org/MPL/2.0/.
 use super::*;
 use crate::{netpkt::reroute::ReroutePkt, *};
 use core::fmt;
-use std::borrow::Borrow;
-
+use std::{borrow::Borrow, ptr};
 
 #[doc(hidden)]
 /// A (fat) pointer to valid netpkt bytes
 /// 
 /// A fat pointer to it can only be constructed through a valid NetPktBytes
 /// WARN: it is likely that this will be removed. NetPktPtr does everything but better except please miri
 #[derive(Debug)]
@@ -26,14 +25,15 @@
 #[repr(C, align(4))]
 pub struct NetPktPtr {
     pub net_header: NetPktHeader,
     pub(crate) hash: LkHash,
     pub(crate) point: PointThinPtr,
 }
 
+
 impl ToOwned for NetPktPtr {
     type Owned = NetPktBox;
 
     fn to_owned(&self) -> Self::Owned {
         self.as_netbox()
     }
 }
@@ -50,86 +50,101 @@
 }
 impl NetPktPtr {
     //pub(crate) const EMPTY : Self = NetPktThin { net_header: NetPktHeader::EMPTY, hash: B64([0;32]), point: PointThinPtr::EMPTY };
 
     #[inline(always)]
     pub fn as_sized(&self) -> &NetPktFatPtr {
         let (_layout, metadata) = netpktbox_layout(self.point.point_header());
-        unsafe { &*std::ptr::from_raw_parts(self as *const NetPktPtr as *const (), metadata) }
+        unsafe { &*ptr::from_raw_parts( ptr::from_ref(self).cast::<()>(), metadata) }
+    }
+    #[inline(always)]
+    pub fn as_mut_sized(&mut self) -> &mut NetPktFatPtr {
+        let (_layout, metadata) = netpktbox_layout(self.point.point_header());
+        unsafe { &mut *ptr::from_raw_parts_mut( ptr::from_mut(self).cast::<()>(), metadata) }
     }
     /// # Safety
     ///
     /// Must be aligned valid netpkt bytes.
     pub unsafe fn from_bytes_unchecked(b: &[u8]) -> &Self {
         assert!(
             b.len() >= MIN_NETPKT_SIZE,
             "Never gone work {} < {} with b= {:?}",
             b.len(),
             MIN_NETPKT_SIZE,
             &b
         );
         assert!(b.as_ptr().align_offset(4) == 0, "Unaligned cast");
-        let netpkt = &*{ b.as_ptr() as *const Self };
-        debug_assert!(netpkt.check::<true>().is_ok());
+        let netpkt = &*{ b.as_ptr().cast::<Self>()};
+        debug_assert!(netpkt.check(true).is_ok());
+        assert!(netpkt.size() as usize == b.len());
         netpkt
     }
     pub fn reroute(&self, route: NetPktHeader) -> ReroutePkt<&Self> {
         ReroutePkt {
             net_header: route,
             pkt: self,
         }
     }
 
-    pub fn check<const CHECK_HASH: bool>(&self) -> Result<&[u8], Error> {
+    pub fn check(&self, skip_hash:bool) -> Result<&[u8], Error> {
         let _ = self.point.internal_consitent_length()?;
-        if CHECK_HASH {
+        if !skip_hash{
             self.point.check_signature()?;
             if self.hash() != self.point.compute_hash() {
                 return Err(Error::HashMismatch);
             }
         }
         Ok(self.as_netpkt_bytes())
     }
     pub fn as_netpkt_bytes(&self) -> &[u8] {
-        unsafe { from_raw_parts(self as *const Self as *const u8, self.size()) }
+        unsafe { from_raw_parts(ptr::from_ref(self).cast::<u8>(), usize::from(self.size())) }
     }
 }
 
 impl Clone for NetPktBox {
     fn clone(&self) -> Self {
         self.thin_netpkt().as_netbox()
     }
 }
 
 impl NetPktFatPtr {
     pub fn thin_netpkt(&self) -> &NetPktPtr {
-        unsafe { &*(self as *const Self as *const NetPktPtr) }
+        unsafe { &*(ptr::from_ref(self).cast::<NetPktPtr>()) }
     }
     /// # Safety
     ///
     /// Must be a aligned buffer of at least self.pkt_header.net_pkt_size len with the correct hash
     pub unsafe fn from_bytes_unchecked(b: &[u8]) -> &Self {
         NetPktPtr::from_bytes_unchecked(b).as_sized()
     }
-    pub fn into_raw_box(this: Box<Self>) -> *const NetPktPtr {
-        Box::into_raw(this) as *const NetPktPtr
+    pub fn into_raw_box(this: Box<Self>) -> *mut NetPktPtr {
+        Box::into_raw(this).cast()
     }
     /// # Safety
     ///
     /// Must be constructed with [Self::into_raw_box]
-    pub unsafe fn from_raw_box(ptr: *const NetPktPtr) -> Box<Self> {
+    pub unsafe fn from_raw_box(ptr: *mut NetPktPtr) -> Box<Self> {
         Box::from_raw(
-            (*ptr).as_sized() as *const NetPktFatPtr as *mut NetPktFatPtr as *mut NetPktFatPtr,
+            ptr::from_mut((*ptr).as_mut_sized())
         )
     }
 }
 
 impl NetPkt for NetPktPtr {
-    #[inline(always)]
+    fn as_netarc(&self) -> NetPktArc {
+        let header = NetPktPtr {
+            net_header: self.net_header,
+            hash: self.hash,
+            point: PointThinPtr(self.point.0)
+        };
+        let bytes = &self.as_netpkt_bytes()[size_of::<NetPktPtr>()..];
+        unsafe {NetPktArc::from_header_and_copy(header.into(),true,|d:&mut [u8]| d.copy_from_slice(bytes)).unwrap()}
+    }
 
+    #[inline(always)]
     fn net_header_mut(&mut self) -> Option<&mut NetPktHeader> {
         Some(&mut self.net_header)
     }
 
     #[inline(always)]
     fn byte_segments(&self) -> ByteSegments {
         ByteSegments::from_array([self.as_netpkt_bytes()])
@@ -192,26 +207,24 @@
     }
 }
 
 pub fn netpktbox_layout(
     pkt_header: &PointHeader,
 ) -> (
     std::alloc::Layout,
-    <NetPktFatPtr as std::ptr::Pointee>::Metadata,
+    <NetPktFatPtr as ptr::Pointee>::Metadata,
 ) {
     use std::alloc::Layout;
-    let clen = pkt_header.content_size();
-    (
-        Layout::new::<PartialNetHeader>()
-            .extend(Layout::new::<u8>().repeat(clen).unwrap().0)
+    let clen : usize = pkt_header.padded_content_size().div_ceil(8).into();
+    let layout =         Layout::new::<PartialNetHeader>()
+            .extend(Layout::new::<u64>().repeat(clen).unwrap().0)
             .unwrap()
             .0
-            .pad_to_align(),
-        clen,
-    )
+            .pad_to_align();
+    (layout,clen)
 }
 
 #[test]
 pub fn build() {
     let sp = linkpoint(
         B64([0; 32]),
         AB([0; 16]),
@@ -229,7 +242,14 @@
 
     let raw = NetPktFatPtr::into_raw_box(sp);
     let h2 = unsafe { &*raw }.hash();
     assert_eq!(h, h2);
     let b = unsafe{NetPktFatPtr::from_raw_box(raw)};
     assert_eq!(h, b.hash())
 }
+
+impl Into<PartialNetHeader> for NetPktPtr{
+    fn into(self) -> PartialNetHeader {
+        let NetPktPtr { net_header, hash, point } = self;
+        PartialNetHeader { net_header, hash, point_header:point.0}
+    }
+}
```

### Comparing `linkspace-0.1.4/local_dependencies/linkspace-pkt/src/netpkt/partial.rs` & `linkspace-0.3.0rc2/local_dependencies/linkspace-pkt/src/netpkt/partial.rs`

 * *Files 20% similar despite different names*

```diff
@@ -2,41 +2,42 @@
 //
 // This Source Code Form is subject to the terms of the Mozilla Public
 // License, v. 2.0. If a copy of the MPL was not distributed with this
 // file, You can obtain one at https://mozilla.org/MPL/2.0/.
 use super::*;
 static_assertions::assert_eq_size!([u8; MIN_NETPKT_SIZE], PartialNetHeader);
 /// Utility struct used for decoding from stream
+// Essentially the same as NetPktPtr but explicitly not complete.
 #[derive(Copy, Clone, Debug)]
 #[repr(C)]
 pub struct PartialNetHeader {
     pub net_header: crate::NetPktHeader,
     pub hash: crate::LkHash,
     pub point_header: crate::PointHeader,
 }
 impl PartialNetHeader {
     pub const EMPTY: Self = PartialNetHeader {
         net_header: NetPktHeader::EMPTY,
         hash: B64([0; 32]),
         point_header: PointHeader::ERROR,
     };
     pub fn from(bytes: &[u8; MIN_NETPKT_SIZE]) -> PartialNetHeader {
-        unsafe { std::ptr::read_unaligned(bytes.as_ptr() as *const Self) }
+        unsafe { std::ptr::read_unaligned(bytes.as_ptr().cast::<Self>()) }
     }
     /// # Safety
     ///
-    /// This must be a reference to a buffer of at least self.pkt_header.net_pkt_size len with the correct hash
+    /// The caller is responsible for checking the headers validity and filling the allocated buffer.
     pub unsafe fn alloc(self) -> NetPktBox {
         let (layout, metadata) = crate::netpktbox_layout(&self.point_header);
         let ptr: *mut u8 = std::alloc::alloc(layout);
         if ptr.is_null() {
             std::alloc::handle_alloc_error(layout);
         }
         let ptr: *mut NetPktFatPtr =
-            std::ptr::from_raw_parts_mut::<NetPktFatPtr>(ptr as *mut (), metadata);
+            std::ptr::from_raw_parts_mut::<NetPktFatPtr>(ptr.cast::<()>(), metadata);
         let mut val = Box::from_raw(ptr);
         val._net_header = self.net_header;
         val.hash = self.hash;
         val.pkt.pkt_header = self.point_header;
         val
     }
 }
```

### Comparing `linkspace-0.1.4/local_dependencies/linkspace-pkt/src/netpkt/reroute.rs` & `linkspace-0.3.0rc2/local_dependencies/linkspace-pkt/src/netpkt/reroute.rs`

 * *Files identical despite different names*

### Comparing `linkspace-0.1.4/local_dependencies/linkspace-pkt/src/netpkt/slot.rs` & `linkspace-0.3.0rc2/local_dependencies/linkspace-pkt/src/netpkt/slot.rs`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 */
 
 use crate::{ NetPktPtr, NetPktHeader, reroute::{Reroute, RecvPkt, PktShareArc}, NetFields, NetPktArc, NetPktParts, NetPktBox, Point };
 
 #[derive(Debug,Clone)]
 pub struct IPkt<'o>(InnerIPkt<'o>);
 #[derive(Debug,Clone)]
-#[allow(dead_code)]
 enum InnerIPkt<'o>{
     Constr(PktShareArc<NetPktParts<'o>>),
     Ref(Reroute<RecvPkt<PktShareArc<&'o NetPktPtr>>>),
     Box(RecvPkt<PktShareArc<NetPktBox>>),
     Arc(Reroute<RecvPkt<NetPktArc>>)
 }
 pub fn from_arc(_pkt:NetPktArc,_recv:Option<crate::Stamp>) -> IPkt<'static>{
```

### Comparing `linkspace-0.1.4/local_dependencies/linkspace-pkt/src/point.rs` & `linkspace-0.3.0rc2/local_dependencies/linkspace-pkt/src/point.rs`

 * *Files 17% similar despite different names*

```diff
@@ -6,15 +6,16 @@
 use crate::{netpkt::NetPktHeader, *};
 
 #[derive(Copy, Clone, Debug, Eq, PartialEq)]
 #[repr(C, align(4))]
 pub struct PointHeader {
     pub reserved: u8,
     pub point_type: PointTypeFlags,
-    pub point_size: U16,
+    /// You surely don't want this raw value - the size of all fields - without the padding between the path and optional signature. 
+    pub uset_bytes: U16,
 }
 
 #[derive(Copy, Clone, Debug, Eq, PartialEq)]
 #[repr(C, align(4))]
 pub struct LinkPointInfo {
     pub offset_ipath: U16,
     pub offset_data: U16,
@@ -25,94 +26,80 @@
     pub info: LinkPointInfo,
     pub create_stamp: Stamp,
     pub group: GroupID,
     pub domain: Domain,
 }
 impl LinkPointHeader {
     pub fn as_bytes(&self) -> &[u8; size_of::<Self>()] {
-        as_bytes(self)
-    }
-}
-
-pub type KeyPointPadding = [u8; 4];
-
-#[derive(Copy, Clone, Debug, Eq, PartialEq)]
-#[repr(C, align(4))]
-pub struct KeyPointHeader {
-    pub reserved: KeyPointPadding,
-    pub signed: Signed,
-    pub inner_point: PointHeader,
-    pub linkpoint: LinkPointHeader,
-}
-impl KeyPointHeader {
-    pub fn as_bytes(&self) -> &[u8; size_of::<Self>()] {
-        as_bytes(self)
-    }
-}
-#[derive(Copy, Clone, Debug, Eq, PartialEq)]
-#[repr(C, align(4))]
-pub struct Signed {
-    pub pubkey: PubKey,
-    pub signature: Signature,
-    pub linkpoint_hash: LkHash,
-}
-impl Signed {
-    pub fn validate(&self) -> Result<(), linkspace_cryptography::Error> {
-        linkspace_cryptography::validate_signature(
-            &self.pubkey.0,
-            &self.signature.0,
-            &self.linkpoint_hash.0,
-        )
+        unsafe {&*std::ptr::from_ref(self).cast()}
     }
 }
 
 impl PointHeader {
-    pub const ERROR: Self = PointHeader {
-        point_type: PointTypeFlags::ERROR_POINT,
-        reserved: 0,
-        point_size: U16::new(4),
+    pub const ERROR: Self = match PointHeader::new_content_len(PointTypeFlags::ERROR_POINT,0){
+        Ok(o) => o,
+        Err(_) => panic!(),
     };
-    pub const fn new(kind: PointTypeFlags, content_len: usize) -> Result<Self, Error> {
+
+    #[allow(clippy::as_conversions)]
+    pub (crate) const fn new_content_len(kind: PointTypeFlags, content_len: usize) -> Result<Self, Error> {
+        let point_size = content_len.saturating_add(size_of::<PointHeader>());
+        Self::new_point_size(kind, point_size)
+    }
+    pub (crate) const fn new_point_size(kind: PointTypeFlags, point_size: usize) -> Result<Self, Error> {
+        if point_size > MAX_POINT_SIZE { return Err(Error::ContentLen)};
         PointHeader {
             point_type: kind,
             reserved: 0,
-            point_size: U16::new(content_len as u16 + 4),
+            uset_bytes: U16::new(point_size as u16) 
         }
         .check()
     }
+    #[allow(clippy::as_conversions)]
     pub const fn check(self) -> Result<Self, Error> {
         if self.reserved != 0 {
             return Err(Error::HeaderReservedSet(self.reserved));
         }
-        let len = self.content_size();
+        let len = self.ucontent_size() as usize ;
         if len > MAX_CONTENT_SIZE {
             return Err(Error::ContentLen);
         }
         let ok = match self.point_type {
             PointTypeFlags::DATA_POINT => true,
             PointTypeFlags::LINK_POINT => len >= size_of::<LinkPointHeader>(),
-            PointTypeFlags::KEY_POINT => len >= size_of::<KeyPointHeader>(),
+            PointTypeFlags::KEY_POINT => len >= size_of::<LinkPointHeader>()+size_of::<Signed>(),
             PointTypeFlags::ERROR_POINT => true,
             e => return Err(Error::UnknownPktType(e.bits)),
         };
         if ok {
             Ok(self)
         } else {
             Err(Error::ContentLen)
         }
     }
     pub fn as_bytes(&self) -> &[u8; 4] {
-        as_bytes(self)
+        unsafe {&*std::ptr::from_ref(self).cast()}
     }
-    /// Size of a point (type,length,content). This is without the hash.
-    pub const fn point_size(&self) -> usize {
-        self.point_size.get() as usize
-    }
-    /// size of a point's content. If it is a datapoint, this is the size of the data.
-    pub const fn content_size(&self) -> usize {
-        self.point_size() - size_of::<PointHeader>()
-    }
-    /// Size of a netpkt. The pointsize plus pointhash and netpktheader
-    pub const fn net_pkt_size(&self) -> usize {
-        self.point_size() + size_of::<LkHash>() + size_of::<NetPktHeader>()
+    /// Size of a point (type,length,content,?signature). This is without the hash or padding between content and signature.
+    pub (crate) const fn upoint_size(&self) -> u16{
+        self.uset_bytes.get() 
+    }
+    pub (crate) const fn padding(&self) -> u16 {
+        self.padded_point_size() - self.upoint_size()
+    }
+    pub (crate)const fn padded_point_size(&self) -> u16 {
+        assert!(std::mem::size_of::<usize>()<= 8, "some code depends on this assumption");
+        self.upoint_size().div_ceil(8)*8
+    }
+    #[allow(clippy::as_conversions)]
+    pub (crate) const fn ucontent_size(&self) -> u16{
+        self.upoint_size().saturating_sub( size_of::<PointHeader>() as u16)
+    }
+    pub (crate) const fn padded_content_size(&self) -> u16 {
+        self.padded_point_size().saturating_sub( size_of::<PointHeader>() as u16)
+    }
+    /// Size of a netpkt. The pointsize plus pointhash and netpktheader + padding 
+    #[allow(clippy::as_conversions)]
+    pub const fn size(&self) -> u16{
+        self.padded_point_size() + size_of::<LkHash>() as u16 + size_of::<NetPktHeader>() as u16
     }
 }
```

### Comparing `linkspace-0.1.4/local_dependencies/linkspace-pkt/src/point_parts.rs` & `linkspace-0.3.0rc2/local_dependencies/linkspace-pkt/src/point_parts.rs`

 * *Files 19% similar despite different names*

```diff
@@ -11,29 +11,49 @@
 #[derive(Clone, Copy, Debug, Eq, PartialEq)]
 #[repr(C, align(4))]
 pub struct PointParts<'a> {
     pub pkt_header: PointHeader,
     pub fields: PointFields<'a>,
 }
 
+
+#[derive(Clone, Copy, Eq, PartialEq,Debug)]
+#[repr(C,align(4))]
+pub struct Signed{
+    pub pubkey:PubKey,
+    pub signature:Signature
+}
+impl Signed {
+    fn as_bytes(&self) -> &[u8] {
+        unsafe{&*std::slice::from_raw_parts(std::ptr::from_ref(self).cast(),size_of::<Self>())}
+    }
+    pub(crate) fn validate(&self,hash:&[u8;32]) -> Result<(), linkspace_cryptography::Error> {
+        linkspace_cryptography::validate_signature(
+            &self.pubkey.0,
+            &self.signature.0,
+            &hash,
+        )
+    }
+}
+
 #[derive(Clone, Copy, Eq, PartialEq)]
 #[non_exhaustive]
 pub enum PointFields<'a> {
     DataPoint(&'a [u8]),
     LinkPoint(LinkPoint<'a>),
-    KeyPoint(KeyPoint<'a>),
+    KeyPoint(LinkPoint<'a>, Signed),
     Error(&'a [u8]),
     Unknown(&'a [u8]),
 }
 impl<'a> PointFields<'a> {
     pub fn common_idx(&self) -> Option<(&LinkPointHeader, &IPath, Option<&PubKey>)> {
         match self {
             PointFields::LinkPoint(sp) => Some((&sp.head, sp.tail.ipath, None)),
-            PointFields::KeyPoint(a) => {
-                Some((&a.head.linkpoint, a.tail.ipath, Some(&a.head.signed.pubkey)))
+            PointFields::KeyPoint(sp,signed) => {
+                Some((&sp.head, sp.tail.ipath, Some(&signed.pubkey)))
             }
             _ => None,
         }
     }
 }
 
 #[derive(Debug, Clone, Copy, Eq, PartialEq)]
@@ -46,105 +66,108 @@
 #[derive(Clone, Copy, Debug, Eq, PartialEq)]
 pub struct Tail<'a> {
     pub links: &'a [Link],
     pub data: &'a [u8],
     pub ipath: &'a IPath,
 }
 
-/// A signed [[LinkPoint]]
-#[derive(Debug, Clone, Copy, Eq, PartialEq)]
-pub struct KeyPoint<'a> {
-    pub head: KeyPointHeader,
-    pub tail: Tail<'a>,
-}
-
 impl<'a> Tail<'a> {
     pub fn links_as_bytes(&'a self) -> &'a [u8] {
         unsafe {
             from_raw_parts(
-                self.links.as_ptr() as *const u8,
-                self.links.len() * size_of::<Link>(),
+                self.links.as_ptr().cast::<u8>(),
+                std::mem::size_of_val(self.links),
             )
         }
     }
     pub fn byte_len(&self) -> usize {
         self.data.len() + self.ipath.ipath_bytes().len() + self.links_as_bytes().len()
     }
 }
 
 impl<'tail> PointParts<'tail> {
     pub fn data_ptr(&self) -> &'tail [u8] {
         match self.fields {
             PointFields::DataPoint(b) => b,
-            PointFields::LinkPoint(LinkPoint { head: _, tail }) => tail.data,
-            PointFields::KeyPoint(KeyPoint { head: _, tail }) => tail.data,
+            PointFields::LinkPoint(LinkPoint {  tail, .. }) => tail.data,
+            PointFields::KeyPoint(LinkPoint{tail,..}, _) => tail.data,
             PointFields::Error(b) => b,
             PointFields::Unknown(o) => o,
         }
     }
 }
 
 impl<'tail> Point for PointParts<'tail> {
     #[inline(always)]
     fn parts(&self) -> PointParts<'tail> {
         *self
     }
     #[inline(always)]
     fn pkt_segments(&self) -> ByteSegments {
-        let pkt_head = self.pkt_header.as_bytes() as &[u8];
+        let pkt_head = self.pkt_header.as_bytes();
+
+        let padding = self.padding();
         match &self.fields {
-            PointFields::Unknown(b) => ByteSegments::from_array([pkt_head, b]),
-            PointFields::DataPoint(b) => ByteSegments::from_array([pkt_head, b]),
-            PointFields::Error(b) => ByteSegments::from_array([pkt_head, b]),
+            PointFields::Unknown(b) => ByteSegments::from_array([pkt_head, b,padding]),
+            PointFields::DataPoint(b) => ByteSegments::from_array([pkt_head, b,padding]),
+            PointFields::Error(b) => ByteSegments::from_array([pkt_head, b,padding]),
             PointFields::LinkPoint(LinkPoint { head, tail }) => ByteSegments::from_array([
                 pkt_head,
                 head.as_bytes(),
                 tail.links_as_bytes(),
                 tail.ipath.ipath_bytes(),
                 tail.data,
+                padding
             ]),
-            PointFields::KeyPoint(KeyPoint { head, tail }) => ByteSegments::from_array([
+            PointFields::KeyPoint(LinkPoint{head, tail}, signed) => ByteSegments::from_array([
                 pkt_head,
                 head.as_bytes(),
                 tail.links_as_bytes(),
                 tail.ipath.ipath_bytes(),
                 tail.data,
+                padding,
+                signed.as_bytes()
             ]),
         }
     }
 
     #[inline(always)]
     fn data(&self) -> &[u8] {
         self.data_ptr()
     }
+    fn padding(&self) -> &[u8]{
+        let pad_len = self.pkt_header.padded_point_size() - self.pkt_header.upoint_size();
+        static PAD : [u8;8] = [255;8];
+        &PAD[..pad_len as usize]
+    }
 
     #[inline(always)]
     fn tail(&self) -> Option<Tail> {
         match self.fields {
-            PointFields::LinkPoint(LinkPoint { head: _, tail }) => Some(tail),
-            PointFields::KeyPoint(KeyPoint { head: _, tail }) => Some(tail),
+            PointFields::LinkPoint(LinkPoint {  tail ,.. }) => Some(tail),
+            PointFields::KeyPoint(LinkPoint{  tail , .. },_) => Some(tail),
             _ => None,
         }
     }
     #[inline(always)]
     fn point_header_ref(&self) -> &PointHeader {
         &self.pkt_header
     }
     #[inline(always)]
     fn linkpoint_header(&self) -> Option<&LinkPointHeader> {
         match &self.fields {
-            PointFields::LinkPoint(LinkPoint { head, tail: _ }) => Some(head),
-            PointFields::KeyPoint(KeyPoint { head, tail: _ }) => Some(&head.linkpoint),
+            PointFields::LinkPoint(LinkPoint { head, ..}) => Some(head),
+            PointFields::KeyPoint(LinkPoint{ head, ..},_) => Some(head),
             _ => None,
         }
     }
 
-    fn keypoint_header(&self) -> Option<&KeyPointHeader> {
+    fn signed(&self) -> Option<&Signed> {
         match &self.fields {
-            PointFields::KeyPoint(h) => Some(&h.head),
+            PointFields::KeyPoint(_,t) => Some(&t),
             _ => None,
         }
     }
 }
 
 impl<'o> core::fmt::Debug for PointFields<'o> {
     fn fmt(&self, f: &mut core::fmt::Formatter<'_>) -> core::fmt::Result {
@@ -157,12 +180,12 @@
                     "DataPoint".to_string()
                 };
                 f.debug_tuple(&name)
                     .field(&AB(&arg0[0..arg0.len().min(400)]))
                     .finish()
             }
             Self::LinkPoint(arg0) => f.debug_tuple("LinkPoint").field(arg0).finish(),
-            Self::KeyPoint(arg0) => f.debug_tuple("KeyPoint").field(arg0).finish(),
+            Self::KeyPoint(arg0,arg1) => f.debug_tuple("NewKeyPoint").field(arg0).field(arg1).finish(),
             Self::Error(arg0) => f.debug_tuple("Error").field(&AB(&arg0)).finish(),
         }
     }
 }
```

### Comparing `linkspace-0.1.4/local_dependencies/linkspace-pkt/src/point_ptr.rs` & `linkspace-0.3.0rc2/local_dependencies/linkspace-pkt/src/point_ptr.rs`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,20 @@
 // Copyright Anton Sol
 //
 // This Source Code Form is subject to the terms of the Mozilla Public
 // License, v. 2.0. If a copy of the MPL was not distributed with this
 // file, You can obtain one at https://mozilla.org/MPL/2.0/.
-use std::fmt::{self, Debug};
+use std::{
+    fmt::{self, Debug},
+    ptr,
+};
 
 use super::*;
 use crate::utils::none;
 
-// starting from the first pkt_byte, if the type is keypoint, this is the offset for the inner linkpoint pkt
-pub(crate) const LINKPOINT_IN_KEYPOINT_OFFSET: usize = size_of::<PointHeader>()
-    + size_of::<KeyPointHeader>()
-    - size_of::<PointHeader>()
-    - size_of::<LinkPointHeader>();
-
 /// Flat [u8] repr of a [Point]
 #[repr(C, align(4))]
 pub struct PointPtr {
     pub(crate) pkt_header: PointHeader,
     content: [u8],
 }
 #[repr(C)]
@@ -34,16 +31,16 @@
     pub fn point_header(&self) -> &PointHeader {
         &self.0
     }
     #[inline(always)]
     pub fn as_sized(&self) -> &PointPtr {
         unsafe {
             &*(std::ptr::from_raw_parts(
-                self as *const PointThinPtr as *const (),
-                self.0.content_size(),
+                ptr::from_ref(self).cast::<()>(),
+                usize::from(self.0.padded_content_size()),
             ))
         }
     }
 }
 
 impl fmt::Debug for PointPtr {
     fn fmt(&self, f: &mut fmt::Formatter<'_>) -> fmt::Result {
@@ -54,213 +51,205 @@
             .finish()
     }
 }
 
 impl PointPtr {
     #[inline(always)]
     pub fn thin_point(&self) -> &PointThinPtr {
-        unsafe { &*((&self.pkt_header) as *const PointHeader as *const PointThinPtr) }
+        unsafe { &*(ptr::from_ref(&self.pkt_header).cast::<PointThinPtr>()) }
     }
     /// # Safety
     ///
     /// should be well aligned valid netpktbytes.
     pub unsafe fn from_bytes_unchecked(b: &[u8]) -> &PointPtr {
         PointThinPtr::from_bytes_unchecked(b).as_sized()
     }
-    pub fn internal_consitent_length(&self) -> Result<usize, Error> {
+    pub fn internal_consitent_length(&self) -> Result<(), Error> {
         self.thin_point().internal_consitent_length()
     }
-    #[inline(always)]
-    pub fn pkt_bytes(&self) -> &[u8] {
-        unsafe {
-            core::slice::from_raw_parts(
-                self as *const Self as *const u8,
-                self.pkt_header.point_size(),
-            )
-        }
-    }
 }
 impl PointThinPtr {
     /// # Safety
     ///
     /// This is a unchecked cast, meaning accessing fields is dangerous
     /// to validate, first ensure you have enough bytes to read a PktHeader,
     /// Then call internal_consistent_length and compare the lengths
-    /// finally call check_signature to ensure if its an assert pkt that its valid.
+    /// finally call check_signature to ensure if its signed that its valid.
     pub unsafe fn from_bytes_unchecked(b: &[u8]) -> &PointThinPtr {
         assert!(b.len() >= size_of::<PointHeader>(), "Never gone work");
-        assert!(b.as_ptr().align_offset(4) == 0, "Unaligned cast");
-        &*(b.as_ptr() as *const PointThinPtr)
+        assert!(b.as_ptr().align_offset(8) == 0, "Unaligned cast");
+        assert!(b.len() % 8 == 0, "missing padding");
+        &*(b.as_ptr().cast::<PointThinPtr>())
     }
     #[inline(always)]
-    fn fixed(&self) -> BarePointFields {
-        let mem = &self.content_memory();
-        match self.0.point_type {
-            PointTypeFlags::DATA_POINT => BarePointFields::DataPoint(mem),
-            PointTypeFlags::LINK_POINT => {
-                let (linkpoint, tail) = mem.split_at(size_of::<LinkPointHeader>());
-                let linkpoint = unsafe { &*(linkpoint.as_ptr() as *const LinkPointHeader) };
-                BarePointFields::LinkPoint {
-                    lp_header: linkpoint,
-                    tail,
-                }
-            }
-            PointTypeFlags::KEY_POINT => {
-                let (assert, tail) = mem.split_at(size_of::<KeyPointHeader>());
-                let assert = unsafe { &*(assert.as_ptr() as *const KeyPointHeader) };
-                BarePointFields::KeyPoint {
-                    a_header: assert,
-                    tail,
+    pub (crate) fn linkpoint_header(&self) -> Option<&LinkPointHeader>{
+        let mut v = None;
+        if self.0.point_type.contains(PointTypeFlags::LINK) {
+            v = Some(unsafe {&*self.pkt_bytes().as_ptr().add(size_of::<PointHeader>()).cast::<LinkPointHeader>()});
+        }
+        v
+    }
+    /// This must be called with a verified point type.
+    #[inline(always)]
+    pub(crate)fn fixed(&self) -> BarePointFields {
+        let (_point, rest) = unsafe {
+            self.pkt_bytes()
+                .split_at_unchecked(size_of::<PointHeader>())
+        };
+        let padding_len: usize = self.0.padding().into();
+
+        if self.0.point_type.contains(PointTypeFlags::LINK) {
+            unsafe {
+                let (lp, mut rest) = rest.split_at_unchecked(size_of::<LinkPointHeader>());
+                let header = &*lp.as_ptr().cast::<LinkPointHeader>();
+                let mut signed: Option<&Signed> = None;
+                if self.0.point_type.contains(PointTypeFlags::SIGNATURE) {
+                    let (tail, signed_b) =
+                        rest.split_at_unchecked(rest.len() - size_of::<Signed>());
+                    rest = tail;
+                    signed = Some(&*signed_b.as_ptr().cast::<Signed>());
                 }
+                let (_tail, padding) =
+                    rest.split_at_unchecked(rest.len() - self.0.padding() as usize);
+
+                return BarePointFields::LinkPoint {
+                    header,
+                    padding,
+                    signed,
+                };
             }
-            PointTypeFlags::ERROR_POINT => BarePointFields::Error(mem),
-            _ => panic!("Working with invalid packets."),
+        }
+        let (mem, padding) = unsafe { rest.split_at_unchecked(rest.len() - padding_len) };
+        match self.0.point_type {
+            PointTypeFlags::DATA_POINT => BarePointFields::DataPoint { data: mem, padding },
+            PointTypeFlags::ERROR_POINT => BarePointFields::Error { msg: mem, padding },
+            _ => BarePointFields::Unknown(rest),
         }
     }
 
     /// Check the header length fields and return the point size. This is the length without the hash.
     #[inline(always)]
-    pub fn internal_consitent_length(&self) -> Result<usize, Error> {
+    pub fn internal_consitent_length(&self) -> Result<(), Error> {
         self.point_header().check()?;
-        let point_size = self.point_header().point_size();
-        match self.fixed() {
-            BarePointFields::DataPoint(_) => (),
-            BarePointFields::LinkPoint { lp_header, tail: _ } => {
-                let isp_offset = lp_header.info.offset_ipath.get();
-                let data_offset = lp_header.info.offset_data.get();
-                if data_offset as usize > point_size {
+        let mut point_size = self.point_header().upoint_size();
+        let padding = match self.fixed() {
+            BarePointFields::DataPoint { padding, .. } => padding,
+            BarePointFields::LinkPoint {
+                padding,
+                header,
+                signed: _,
+            } => {
+                if self.0.point_type.contains(PointTypeFlags::SIGNATURE) {
+                    // signed.is_some(
+                    point_size -= size_of::<Signed>() as u16;
+                }
+                let isp_offset = header.info.offset_ipath.get();
+                let data_offset = header.info.offset_data.get();
+                if data_offset > point_size {
                     return Err(Error::DataOffsetIncompatible);
                 }
                 if isp_offset > data_offset {
                     return Err(Error::DataOffsetIncompatible);
                 }
                 let link_size = isp_offset
-                    .checked_sub((size_of::<PointHeader>() + size_of::<LinkPointHeader>()) as u16)
+                    .checked_sub(
+                        (size_of::<PointHeader>() + size_of::<LinkPointHeader>())
+                            .try_into()
+                            .unwrap(),
+                    )
                     .ok_or(Error::ISPOffsetIncompatible)?;
-                if link_size % size_of::<Link>() as u16 != 0 {
+                if link_size % u16::try_from(size_of::<Link>()).unwrap() != 0 {
                     return Err(Error::IndivisableLinkbytes);
                 }
-                unsafe { self.unchecked_linkpoint_tail() }
-                    .ipath
-                    .check_components()?;
-            }
-            BarePointFields::KeyPoint {
-                a_header: assert,
-                tail: _,
-            } => {
-                let inner_linkpoint_size = self.point_header().content_size()
-                    - size_of::<KeyPointPadding>()
-                    - size_of::<PubKey>()
-                    - size_of::<Signature>();
-                if inner_linkpoint_size < MIN_LINKPOINT_SIZE {
-                    return Err(Error::KeyPointLength);
-                }
-                if assert.inner_point.point_type != PointTypeFlags::LINK_POINT {
-                    return Err(Error::SignedInvalidPkt);
-                }
-                let inner_lp_bytes = &self.pkt_bytes()[LINKPOINT_IN_KEYPOINT_OFFSET..];
-                let linkpoint = unsafe { PointThinPtr::from_bytes_unchecked(inner_lp_bytes) };
-                let lp_size = linkpoint.internal_consitent_length()?;
-                if inner_linkpoint_size != lp_size + size_of::<LkHash>() {
-                    return Err(Error::KeyPointLength);
-                }
+                unsafe { self.unchecked_tail() }.ipath.check_components()?;
+                padding
             }
-            BarePointFields::Error(_) => (),
-            BarePointFields::Unknown(_) => (),
+            BarePointFields::Error { padding, .. } => padding,
+            BarePointFields::Unknown(_) => &[],
         };
-        Ok(point_size)
+        if padding.len() > 7 {return Err(Error::PaddingBitsNotU8Max);}
+        if !padding.iter().all(|o|*o ==255){return Err(Error::PaddingBitsNotU8Max);}
+        Ok(())
     }
 
     pub fn check_signature(&self) -> Result<(), Error> {
-        if let BarePointFields::KeyPoint {
-            a_header: assert,
-            tail: _,
-        } = self.fixed()
-        {
-            if assert.reserved != KeyPointPadding::default() {
-                return Err(Error::ReservedBitsSet);
-            }
-            let inner_ptr = &assert.inner_point as *const PointHeader;
-            let inner_linkpoint: &PointPtr = unsafe {
-                &*std::ptr::from_raw_parts(
-                    inner_ptr as *const (),
-                    assert.inner_point.content_size(),
-                )
-            };
-            let hash = inner_linkpoint.compute_hash();
-            if hash != assert.signed.linkpoint_hash {
-                return Err(Error::HashMismatch);
+        match self.fixed() {
+            BarePointFields::LinkPoint {
+                header: _,
+                padding: _,
+                signed: Some(signed),
+            } => {
+                let pbytes = self.pkt_bytes();
+                let sans_signature = &pbytes[..pbytes.len() - size_of::<Signed>()];
+                let hash = linkspace_cryptography::blake3_hash(sans_signature);
+                signed
+                    .validate(hash.as_bytes())
+                    .map_err(|_| Error::InvalidSignature)?;
             }
-            assert
-                .signed
-                .validate()
-                .map_err(|_| Error::InvalidSignature)?;
+            _ => (),
         };
         Ok(())
     }
     fn self_ptr(&self) -> *const u8 {
-        self as *const Self as *const u8
+        ptr::from_ref(self).cast()
     }
+    /// include padding
     pub fn pkt_bytes(&self) -> &[u8] {
         unsafe {
             core::slice::from_raw_parts(
-                self as *const Self as *const u8,
-                self.point_header().point_size(),
+                ptr::from_ref(self).cast(),
+                usize::from(self.point_header().padded_point_size()),
             )
         }
     }
 
-    fn content_memory(&self) -> &[u8] {
-        &self.pkt_bytes()[size_of::<PointHeader>()..]
-    }
-
     #[inline(always)]
     fn map_fixed<'a, A: 'a>(
         &'a self,
         onunknown: impl FnOnce(&'a ()) -> A,
         ondata: impl FnOnce(&'a ()) -> A,
         onlinkpoint: impl FnOnce(&'a LinkPointHeader) -> A,
-        onassert: impl FnOnce(&'a KeyPointHeader) -> A,
+        onkeypoint: impl FnOnce(&'a LinkPointHeader, &'a Signed) -> A,
         onerror: impl FnOnce(&'a ()) -> A,
     ) -> A {
         match self.fixed() {
-            BarePointFields::DataPoint(_) => ondata(&()),
+            BarePointFields::DataPoint { .. } => ondata(&()),
+            BarePointFields::LinkPoint {
+                header,
+                signed: None,
+                ..
+            } => onlinkpoint(header),
             BarePointFields::LinkPoint {
-                lp_header: linkpoint,
-                tail: _,
-            } => onlinkpoint(linkpoint),
-            BarePointFields::KeyPoint {
-                a_header: assert,
-                tail: _,
-            } => onassert(assert),
-            BarePointFields::Error(_) => onerror(&()),
+                header,
+                signed: Some(signed),
+                ..
+            } => onkeypoint(header, signed),
+            BarePointFields::Error { .. } => onerror(&()),
             BarePointFields::Unknown(_) => onunknown(&()),
         }
     }
 
     #[inline(always)]
-    unsafe fn unchecked_assert_tail(&self) -> Tail {
-        let inner_linkpoint =
-            self.self_ptr().add(LINKPOINT_IN_KEYPOINT_OFFSET) as *const PointThinPtr;
-        (*inner_linkpoint).unchecked_linkpoint_tail()
-    }
-    #[inline(always)]
-    unsafe fn unchecked_linkpoint_tail(&self) -> Tail {
+    unsafe fn unchecked_tail(&self) -> Tail {
         let ptr = self.self_ptr();
-        let p = &*{ ptr.add(size_of::<PointHeader>()) as *const LinkPointHeader };
+        let p = &*{ ptr.add(size_of::<PointHeader>()).cast::<LinkPointHeader>() };
         let start = size_of::<PointHeader>() + size_of::<LinkPointHeader>();
-        let is_offset = p.info.offset_ipath.get() as usize;
-        let data_offset = p.info.offset_data.get() as usize;
-        let size = self.point_header().point_size();
+        let is_offset = usize::from(p.info.offset_ipath.get());
+        let data_offset = usize::from(p.info.offset_data.get());
+        let mut size = self.point_header().upoint_size();
+        if self.0.point_type.contains(PointTypeFlags::SIGNATURE) {
+            size -= size_of::<Signed>() as u16;
+        }
         //assert!(start <= is_offset && is_offset <= data_offset && data_offset <= size , "bad sizes");
-        let links: &[Link] = core::slice::from_ptr_range(
-            ptr.add(start) as *const Link..ptr.add(is_offset) as *const Link,
-        );
+        let start = ptr.add(start).cast::<Link>();
+        let end = ptr.add(is_offset).cast::<Link>();
+        assert!(start.is_aligned());
+        let links: &[Link] = core::slice::from_ptr_range(start..end);
         let isp_bytes = core::slice::from_ptr_range(ptr.add(is_offset)..ptr.add(data_offset));
-        let data = core::slice::from_ptr_range(ptr.add(data_offset)..ptr.add(size));
+        let data = core::slice::from_ptr_range(ptr.add(data_offset)..ptr.add(size.into()));
         let spath_idx = IPath::from_unchecked(isp_bytes);
         debug_assert!(spath_idx.check_components().is_ok(), "{spath_idx:?}");
         Tail {
             ipath: spath_idx,
             data,
             links,
         }
@@ -271,42 +260,58 @@
     #[inline(always)]
     fn data(&self) -> &[u8] {
         self.parts().data_ptr()
     }
     #[inline(always)]
     fn tail(&self) -> Option<Tail> {
         match self.parts().fields {
-            PointFields::LinkPoint(LinkPoint { head: _, tail }) => Some(tail),
-            PointFields::KeyPoint(KeyPoint { head: _, tail }) => Some(tail),
+            PointFields::LinkPoint(LinkPoint { tail, .. }) => Some(tail),
+            PointFields::KeyPoint(LinkPoint { tail, .. }, _) => Some(tail),
             _ => None,
         }
     }
     #[inline(always)]
-    fn keypoint_header(&self) -> Option<&KeyPointHeader> {
-        self.map_fixed(none, none, none, Some, none)
+    fn signed(&self) -> Option<&Signed> {
+        self.map_fixed(none, none, none, |_, a| Some(a), none)
     }
     #[inline(always)]
     fn linkpoint_header(&self) -> Option<&LinkPointHeader> {
-        self.map_fixed(none, none, Some, |a| Some(&a.linkpoint), none)
+        self.map_fixed(none, none, Some, |a, _| Some(a), none)
     }
     #[inline(always)]
     fn parts(&self) -> PointParts {
-        let fields = match self.point_header().point_type {
-            PointTypeFlags::DATA_POINT => PointFields::DataPoint(self.content_memory()),
-            PointTypeFlags::LINK_POINT => {
-                let head = unsafe { &*(self.content_memory().as_ptr() as *const LinkPointHeader) };
-                let tail = unsafe { self.unchecked_linkpoint_tail() };
-                PointFields::LinkPoint(LinkPoint { head: *head, tail })
+        let fields = match self.fixed() {
+            BarePointFields::DataPoint { data, padding: _ } => PointFields::DataPoint(data),
+            BarePointFields::LinkPoint {
+                header,
+                signed: None,
+                padding: _,
+            } => {
+                let tail = unsafe { self.unchecked_tail() };
+                PointFields::LinkPoint(LinkPoint {
+                    head: *header,
+                    tail,
+                })
             }
-            PointTypeFlags::KEY_POINT => {
-                let head = unsafe { &*(self.content_memory().as_ptr() as *const KeyPointHeader) };
-                let tail = unsafe { self.unchecked_assert_tail() };
-                PointFields::KeyPoint(KeyPoint { head: *head, tail })
+            BarePointFields::LinkPoint {
+                header,
+                signed: Some(signed),
+                padding: _,
+            } => {
+                let tail = unsafe { self.unchecked_tail() };
+                PointFields::KeyPoint(
+                    LinkPoint {
+                        head: *header,
+                        tail,
+                    },
+                    *signed,
+                )
             }
-            _ => PointFields::Error(self.content_memory()),
+            BarePointFields::Error { msg, padding: _ } => PointFields::Error(msg),
+            BarePointFields::Unknown(o) => PointFields::Unknown(o),
         };
         PointParts {
             pkt_header: *self.point_header(),
             fields,
         }
     }
 
@@ -315,29 +320,38 @@
         self.point_header()
     }
 
     #[inline(always)]
     fn pkt_segments(&self) -> ByteSegments {
         ByteSegments::from_array([self.pkt_bytes()])
     }
+
+    fn padding(&self) -> &[u8] {
+        match self.fixed() {
+            BarePointFields::DataPoint { padding, .. }
+            | BarePointFields::LinkPoint { padding, .. }
+            | BarePointFields::Error { padding, .. }
+            | BarePointFields::Unknown(padding) => padding,
+        }
+    }
 }
 
 impl Point for PointPtr {
     #[inline(always)]
     fn data(&self) -> &[u8] {
         self.thin_point().data()
     }
     #[inline(always)]
     fn tail(&self) -> Option<Tail> {
         self.thin_point().tail()
     }
-    #[inline(always)]
-    fn keypoint_header(&self) -> Option<&KeyPointHeader> {
-        self.thin_point().map_fixed(none, none, none, Some, none)
+    fn padding(&self) -> &[u8] {
+        self.thin_point().padding()
     }
+
     #[inline(always)]
     fn linkpoint_header(&self) -> Option<&LinkPointHeader> {
         self.thin_point().linkpoint_header()
     }
     #[inline(always)]
     fn parts(&self) -> PointParts {
         self.thin_point().parts()
@@ -346,26 +360,37 @@
     #[inline(always)]
     fn point_header_ref(&self) -> &PointHeader {
         &self.pkt_header
     }
 
     #[inline(always)]
     fn pkt_segments(&self) -> ByteSegments {
-        ByteSegments::from_array([self.pkt_bytes()])
+        self.thin_point().pkt_segments()
+    }
+
+    fn signed(&self) -> Option<&Signed> {
+        self.thin_point()
+            .map_fixed(none, none, none, |_, o| Some(o), none)
     }
 }
 
-#[allow(dead_code)]
-#[repr(align(4))]
-enum BarePointFields<'o> {
-    DataPoint(&'o [u8]),
+// This layout can produce cmov instructions
+#[derive(Debug)]
+pub(crate) enum BarePointFields<'o> {
+    DataPoint {
+        data: &'o [u8],
+        #[allow(unused)]
+        padding: &'o [u8],
+    },
     LinkPoint {
-        lp_header: &'o LinkPointHeader,
-        tail: &'o [u8],
+        header: &'o LinkPointHeader,
+        signed: Option<&'o Signed>,
+        #[allow(unused)]
+        padding: &'o [u8],
     },
-    KeyPoint {
-        a_header: &'o KeyPointHeader,
-        tail: &'o [u8],
+    Error {
+        msg: &'o [u8],
+        #[allow(unused)]
+        padding: &'o [u8],
     },
-    Error(&'o [u8]),
     Unknown(&'o [u8]),
 }
```

### Comparing `linkspace-0.1.4/local_dependencies/linkspace-pkt/src/spath.rs` & `linkspace-0.3.0rc2/local_dependencies/linkspace-pkt/src/spath.rs`

 * *Files 10% similar despite different names*

```diff
@@ -3,49 +3,53 @@
 // This Source Code Form is subject to the terms of the Mozilla Public
 // License, v. 2.0. If a copy of the MPL was not distributed with this
 // file, You can obtain one at https://mozilla.org/MPL/2.0/.
 use crate::*;
 /**
 Serializable length delimited &[&[u8]]. e.g. /hello/world.
 Holds an upto 8 components.
-Components are non-empty, length delimited, and have no strict encoding.
-They might contain arbitrary bytes such as '\\0' and '/'
+Components are non-empty, length delimited, bytes.
 
-[SPath] and [SPathBuf] are length delimited component. ( Simmilar to [std::path::Path] and [std::path::PathBuf]).
-[IPath] and [IPathBuf] are spath's with a [u8;8] prefix that holds the offset of each component.
+[SPath] and [SPathBuf] are similar to [std::path::Path] and [std::path::PathBuf].
+[IPath] and [IPathBuf] are SPath's with a [u8;8] prefix that holds the number of components and their offset.
 */
-use std::{borrow::Borrow, ops::Deref};
+use std::{borrow::Borrow, ops::Deref, ptr};
 
 #[derive(Copy, Clone, PartialEq, Eq, Default, PartialOrd, Ord, Hash)]
 #[repr(transparent)]
 pub struct SPathBytes<X: ?Sized> {
     spath_bytes: X,
 }
+impl<X> SPathBytes<X> where Self: AsRef<SPath>{
+    pub fn try_from_inner(spath_bytes: X) -> Result<Self,PathError> {
+        let sp = SPathBytes { spath_bytes };
+        sp.as_ref().check_components()?;
+        Ok(sp)
+    }
+}
 
 use thiserror::Error;
 #[derive(Error, Debug, PartialEq, Copy, Clone)]
 pub enum PathError {
-    #[error("Path only allows upto {MAX_PATH_LEN} components")]
+    #[error("path only allows upto {MAX_PATH_LEN} components")]
     MaxLen,
-    #[error("Exceeded maximum component size ({MAX_SPATH_COMPONENT_SIZE} bytes)")]
+    #[error("exceeded maximum component size ({MAX_SPATH_COMPONENT_SIZE} bytes)")]
     ComponentSize,
-    #[error("Component cant be of size 0")]
+    #[error("component cant be of size 0")]
     ZeroComponent,
-    #[error("Mismatch length for last component")]
+    #[error("mismatch length for last component")]
     TailLength,
-    #[error("Exceeds Max SPath size ({MAX_SPATH_SIZE})")]
+    #[error("exceeds max path size ({MAX_SPATH_SIZE})")]
     CapacityError,
 
-    #[error("TODO")]
-    IdxError,
-    #[error("Missing Index. Expected at least 8 bytes (or none)")]
+    #[error("bad path index")]
     MissingIdx,
-    #[error("The offset of the non components is wrong")]
+    #[error("empty component offset")]
     EmptyComponentIdx,
-    #[error("The offset does  not agree with the spath")]
+    #[error("path index is wrong")]
     BadOffset,
 }
 
 /// Explicitly SPath bytes (analogous to [[str]])
 pub type SPath = SPathBytes<[u8]>;
 
 
@@ -55,14 +59,15 @@
 
 impl AsRef<SPath> for SPath {
     fn as_ref(&self) -> &SPath {
         self
     }
 }
 impl<X: AsRef<[u8]>> FromIterator<X> for SPathBuf {
+    #[track_caller]
     fn from_iter<T: IntoIterator<Item = X>>(iter: T) -> Self {
         SPathBuf::try_from_iter(iter).unwrap()
     }
 }
 
 impl Deref for SPathBuf {
     type Target = SPath;
@@ -118,29 +123,30 @@
     }
     pub fn into_spathbuf(&self) -> SPathBuf {
         SPathBytes {
             spath_bytes: self.spath_bytes().to_vec(),
         }
     }
     pub const fn from_unchecked(b: &[u8]) -> &SPath {
-        unsafe { std::mem::transmute(b) }
+        unsafe { &*ptr::from_raw_parts(b.as_ptr().cast(),b.len())}
     }
     pub const fn spath_bytes(&self) -> &[u8] {
         &self.spath_bytes
     }
 }
 
 impl<const N: usize> ConstSPath<N> {
     #[track_caller]
     pub const fn from_raw(bytes: [u8; N]) -> ConstSPath<N> {
         if let Err(_e) = SPath::from_slice(&bytes) {
             panic!("Invalid raw bytes")
         }
         SPathBytes { spath_bytes: bytes }
     }
+    
 
     pub const fn as_static(&'static self) -> &'static SPath {
         SPath::from_unchecked(&self.spath_bytes)
     }
     pub fn to_owned(&self) -> SPathBuf {
         SPathBuf {
             spath_bytes: self.spath_bytes.to_vec(),
@@ -180,23 +186,24 @@
     #[track_caller]
     pub fn join(&self, path: &SPath) -> SPathBuf {
         self.try_join(path).unwrap()
     }
 }
 
 pub fn spath_buf(components: &[&[u8]]) -> SPathBuf {
-    SPathBuf::from(components)
+    SPathBuf::from_iter(components)
 }
 
 impl SPathBuf {
     pub const fn new() -> SPathBuf {
         SPathBytes {
             spath_bytes: vec![],
         }
     }
+    
     pub const fn from_vec_unchecked(bytes: Vec<u8>) -> SPathBuf {
         SPathBuf { spath_bytes: bytes }
     }
     pub fn extend_from_iter(
         mut self,
         i: impl IntoIterator<Item = impl AsRef<[u8]>>,
     ) -> Result<Self, PathError> {
@@ -211,18 +218,15 @@
         Ok(self)
     }
     pub fn try_from_iter(
         iter: impl IntoIterator<Item = impl AsRef<[u8]>>,
     ) -> Result<SPathBuf, PathError> {
         SPathBytes::new().extend_from_iter(iter)
     }
-    #[track_caller]
-    pub fn from(iter: impl IntoIterator<Item = impl AsRef<[u8]>>) -> SPathBuf {
-        SPathBuf::try_from_iter(iter).unwrap()
-    }
+
 
     pub fn truncate_last(&mut self) {
         if let Some(l) = self.iter().last().map(|v| v.len() + 1) {
             self.spath_bytes.truncate(self.spath_bytes.len() - l);
         }
     }
 
@@ -256,15 +260,15 @@
         }
         if component.is_empty() {
             return Err(PathError::ZeroComponent);
         }
         if self.spath_bytes.len() + component.len() + 1 > MAX_SPATH_SIZE {
             return Err(PathError::CapacityError);
         }
-        self.spath_bytes.push(component.len() as u8);
+        self.spath_bytes.push(component.len().try_into().unwrap());
         self.spath_bytes.extend_from_slice(component);
         Ok(self)
     }
     #[must_use]
     pub fn push_front(self, component: &[u8]) -> SPathBuf {
         self.try_push_front(component).unwrap()
     }
@@ -276,22 +280,23 @@
             return Err(PathError::ZeroComponent);
         }
         if self.spath_bytes.len() + component.len() + 1 > MAX_SPATH_SIZE {
             return Err(PathError::CapacityError);
         }
         self.spath_bytes.splice(
             0..0,
-            [component.len() as u8]
+            [component.len().try_into().unwrap()]
                 .into_iter()
                 .chain(component.iter().cloned()),
         );
         Ok(self)
     }
 }
 
+
 impl SPath {
     pub const fn is_empty(&self) -> bool {
         self.spath_bytes.is_empty()
     }
     pub fn head(&self) -> Option<&[u8]> {
         self.iter().next()
     }
@@ -312,15 +317,15 @@
     }
     pub fn split_last(&self) -> (&SPath, Option<&SPath>) {
         let mut this = self;
         let mut last = None;
 
         while !this.is_empty() {
             last = Some(this);
-            let len = this.spath_bytes[0] as usize;
+            let len :usize = this.spath_bytes[0].into();
             this = SPath::from_unchecked(&this.spath_bytes[len + 1..]);
         }
         match last {
             None => (this, None),
             Some(v) => {
                 let mid = self.spath_bytes.len() - v.spath_bytes.len();
                 let (a, b) = self.byte_split_at(mid);
@@ -345,18 +350,19 @@
         }
     }
 
     pub fn split_first(&self) -> Option<(&[u8], &SPath)> {
         if self.is_empty() {
             return None;
         }
-        let len = self.spath_bytes[0] as usize;
+        let len = usize::from(self.spath_bytes[0]);
         let bytes = &self.spath_bytes[1..len + 1];
         Some((bytes, SPath::from_unchecked(&self.spath_bytes[len + 1..])))
     }
+    #[allow(clippy::as_conversions)]
     pub const fn first(&self) -> &[u8] {
         match self.spath_bytes.split_first() {
             Some((len, bytes)) => bytes.split_at(*len as usize).0,
             None => &[],
         }
     }
 
@@ -389,21 +395,21 @@
         self.strip_prefix(prefix)
             .expect(" Target does not start with prefix")
     }
     pub fn collect(&self) -> arrayvec::ArrayVec<&[u8],MAX_PATH_LEN>{
         arrayvec::ArrayVec::from_iter(self.iter())
     }
     pub fn iter(&self) -> &SPathIter {
-        unsafe { std::mem::transmute(self) }
+        unsafe{&*ptr::from_raw_parts(ptr::from_ref(self).cast(),self.spath_bytes.len())}
     }
     pub const fn checked_iter(&self) -> Result<&CheckedSPathIter, PathError> {
         if self.spath_bytes.len() > MAX_SPATH_SIZE {
             return Err(PathError::MaxLen);
         };
-        Ok(unsafe { std::mem::transmute(self) })
+        Ok(unsafe{&*ptr::from_raw_parts(ptr::from_ref(self).cast(),self.spath_bytes.len())})
     }
     /// Return the components and the spath upto and including that component
     pub fn track(&self) -> Track {
         Track {
             full: self,
             at: self,
         }
@@ -429,38 +435,37 @@
 
 #[repr(transparent)]
 pub struct CheckedSPathIter {
     spath: SPath,
 }
 
 impl CheckedSPathIter {
-    pub const EMPTY: &Self = unsafe { std::mem::transmute(&[] as &[u8]) };
+    pub const EMPTY: &Self = unsafe { &*ptr::from_raw_parts(ptr::from_ref(SPath::empty()).cast(), 0)};
+    #[allow(clippy::as_conversions)]
     pub const fn next_sp_c(&self) -> Option<Result<(&SPath, &Self), PathError>> {
         if self.spath.spath_bytes.is_empty() {
             return None;
         }
         let len = self.spath.spath_bytes[0] as usize;
         if len > MAX_SPATH_COMPONENT_SIZE {
             return Some(Err(PathError::ComponentSize));
         }
         if len == 0 {
             return Some(Err(PathError::ZeroComponent));
         }
-        match self.spath.spath_bytes.get(..=len) {
-            None => Some(Err(PathError::TailLength)),
-            Some(segm) => {
-                let n = self.spath.spath_bytes.get(len + 1..).unwrap_or(&[]);
-                let n = unsafe { std::mem::transmute(n) };
-                Some(Ok((SPath::from_unchecked(segm), n)))
-            }
+        if self.spath.spath_bytes.len() <= len {
+            return Some(Err(PathError::TailLength));
         }
+        let (segm,rest) = self.spath.spath_bytes.split_at(len+1);
+        let rest : *const Self= std::ptr::from_raw_parts(rest.as_ptr().cast(),rest.len());
+        Some(Ok((SPath::from_unchecked(segm),unsafe{&*rest})))
     }
     pub const fn next_c(&self) -> Option<Result<(&[u8], &Self), PathError>> {
         match self.next_sp_c() {
-            Some(Ok((s, r))) => Some(Ok((s.spath_bytes.get(1..).unwrap(), r))),
+            Some(Ok((s, r))) => Some(Ok((s.spath_bytes.split_at(1).1, r))),
             Some(Err(e)) => Some(Err(e)),
             None => None,
         }
     }
 }
 
 impl<'a> Iterator for &'a CheckedSPathIter {
@@ -495,15 +500,15 @@
 }
 impl<'a> Iterator for &'a SPathIter {
     type Item = &'a [u8];
     fn next(&mut self) -> Option<&'a [u8]> {
         if self.spath.spath_bytes.is_empty() {
             return None;
         }
-        let len = self.spath.spath_bytes[0] as usize;
+        let len = usize::from(self.spath.spath_bytes[0]);
         if len > MAX_SPATH_COMPONENT_SIZE || len == 0 {
             panic!("Invalid spath");
         }
         let bytes = &self.spath.spath_bytes.get(1..=len)?;
         *self = match self.spath.spath_bytes.get(len + 1..) {
             Some(b) => SPath::from_unchecked(b).iter(),
             None => SPath::from_unchecked(&[]).iter(),
@@ -531,14 +536,15 @@
 
     common.spath_bytes[2] = 7;
     assert_eq!(common.check_components(), Err(PathError::TailLength));
     common.spath_bytes[2] = 251;
     assert_eq!(common.check_components(), Err(PathError::ComponentSize));
 }
 
+
 #[macro_export]
 macro_rules! len_prefix_concat {
     ($e:expr) => { $crate::prefix_len(*$e)};
     ($e:expr, $($tail:expr),*) => {
         $crate::concat_components($crate::len_prefix_concat!($e),$crate::len_prefix_concat!($($tail),*))
     };
 }
@@ -563,14 +569,15 @@
 	  };
     ($($e:expr),*) => {
         $crate::const_spath!($($e),*)
     }
 }
 
 #[track_caller]
+#[allow(clippy::as_conversions)]
 pub const fn prefix_len<const N: usize>(component: [u8; N]) -> [u8; N + 1] {
     if N > MAX_SPATH_COMPONENT_SIZE {
         panic!()
     }
     if N == 0 {
         panic!()
     }
@@ -607,36 +614,40 @@
 
 #[test]
 fn concat() {
     assert_eq!([1, 0, 2, 0, 0], len_prefix_concat!(&[0], &[0, 0]));
 }
 #[test]
 fn pop_slice() {
-    let mut v = SPathBuf::from(&[b"hello", b"world"]);
-    let x = SPathBuf::from(&[b"hello"]);
-    assert_eq!(v.drop_prefix(&*x), &*SPathBuf::from(&[b"world"]));
+    let mut v = SPathBuf::from_iter(&[b"hello", b"world"]);
+    let x = SPathBuf::from_iter(&[b"hello"]);
+    assert_eq!(v.drop_prefix(&*x), &*SPathBuf::from_iter(&[b"world"]));
     v.truncate_last();
     assert_eq!(v, x)
 }
 
 #[test]
 fn check() {
+    let mut empty = CheckedSPathIter::EMPTY;
+    assert!(empty.next().is_none(), "bad empty iter?");
+    assert!(CheckedSPathIter::EMPTY.spath.spath_bytes.is_empty(), "bad empty iter?");
+
     use crate::*;
     let spath = SPathBuf::try_from_iter(&["hello", "world"]).unwrap();
     let mut it = spath.checked_iter().unwrap();
     assert_eq!(it.next().unwrap().unwrap(), b"hello" as &[u8]);
     assert_eq!(it.next().unwrap().unwrap(), b"world" as &[u8]);
     assert!(it.next().is_none());
-    let v = SPathBuf::from(&[b"a", b"b", b"c"]);
+    let v = SPathBuf::from_iter(&[b"a", b"b", b"c"]);
     assert_eq!(v.check_components().unwrap(), 3);
 }
 
 #[test]
 fn track() {
-    let v = SPathBuf::from(&[b"a", b"b", b"c"]);
+    let v = SPathBuf::from_iter(&[b"a", b"b", b"c"]);
     let mut track = v.track();
     assert_eq!(&track.upto().spath_bytes, &[] as &[u8]);
     track = track.next().unwrap();
     assert_eq!(&track.upto().spath_bytes, &[1, b'a']);
     track = track.next().unwrap();
     assert_eq!(&track.upto().spath_bytes, &[1, b'a', 1, b'b']);
     track = track.next().unwrap();
@@ -680,17 +691,17 @@
         }
         let mut data = Vec::with_capacity(self.size() + 8);
         data.extend_from_slice(&[0; 8]);
 
         let mut it = self.checked_iter()?;
         let mut count = 0u8;
         for i in 0..8 {
-            data[i] = data.len() as u8 - 8;
+            data[i] = unsafe {u8::try_from(data.len()).unwrap_unchecked().checked_sub(8).unwrap_unchecked()};
             if let Some(v) = it.next().transpose()? {
-                data.push(v.len() as u8);
+                data.push( unsafe {v.len().try_into().unwrap_unchecked()});
                 data.extend_from_slice(v);
                 count += 1;
             }
         }
         data[0] = count;
         let v = IPathBuf::from_unchecked(data);
         debug_assert!(
```

### Comparing `linkspace-0.1.4/local_dependencies/linkspace-pkt/src/spath_fmt.rs` & `linkspace-0.3.0rc2/local_dependencies/linkspace-pkt/src/spath_fmt.rs`

 * *Files 8% similar despite different names*

```diff
@@ -7,18 +7,18 @@
 use byte_fmt::{
     abe::{
         self,
         abtxt::as_abtxt,
         ast::{is_fslash, take_ctr_expr, ABEError, Ctr, MatchError},
         convert::TypedABE,
         eval::ABList,
-        ABEValidator, ToABE, ABE,
+        ABEValidator, ToABE, ABE, scope::{core_scope, uint::parse_b},
     },
     eval::{
-        parse_b, ApplyErr, ApplyResult, EvalCtx, EvalScopeImpl, Scope, ScopeEval, ScopeEvalInfo,
+         ApplyErr, ApplyResult, EvalCtx, EvalScopeImpl, Scope, ScopeMacro, ScopeMacroInfo,
         ScopeFunc,
     },
     *,
 };
 use core::fmt::{self, Debug, Display};
 use serde::{Deserialize, Serialize};
 use std::{ops::Range, str::FromStr};
@@ -140,16 +140,18 @@
     }
 }
 pub fn fmt_segm2(seg: &[u8], f: &mut fmt::Formatter) -> fmt::Result {
     if let Ok(b) = <[u8; 32]>::try_from(seg) {
         let b64 = B64(b).to_string();
         write!(f, "/[b:{b64}]")?;
     } else if let Ok(b) = <[u8; 16]>::try_from(seg) {
-        let abt = AB(b).to_abe_str();
-        write!(f, "/{abt}")?;
+        match as_abtxt(&b){
+            std::borrow::Cow::Borrowed(b) => write!(f,"/{b}")?,
+            std::borrow::Cow::Owned(_) => write!(f,"/{}",AB(b).to_abe_str())?,
+        }
     } else {
         write!(f, "/{}", AB(seg))?
     }
     Ok(())
 }
 
 impl ToABE for SPath {
@@ -277,16 +279,16 @@
         }
     }
 }
 #[cfg(test)]
 fn generate_valid() -> Vec<SPathBuf> {
     vec![
         SPathBuf::new(),
-        SPathBuf::from(&[b"hello", b"world"]),
-        SPathBuf::from(&[b"hello" as &[u8], &[255; MAX_SPATH_COMPONENT_SIZE]]),
+        SPathBuf::from_iter(&[b"hello", b"world"]),
+        SPathBuf::from_iter(&[b"hello" as &[u8], &[255; MAX_SPATH_COMPONENT_SIZE]]),
     ]
 }
 #[cfg(test)]
 #[test]
 fn string_fmt() {
     for sp in generate_valid() {
         let st = sp.to_string();
@@ -296,15 +298,15 @@
 }
 
 #[test]
 fn test_encode() {
     #[track_caller]
     fn eq(st: &str, r: &[&[u8]]) {
         let x = spath_str(st).unwrap();
-        let b = SPathBuf::from(r);
+        let b = SPathBuf::from_iter(r);
         assert_eq!(x, b)
     }
     assert!(spath_str("noopen").is_err());
     eq("/ok", &[b"ok"]);
     assert!(spath_str("/trail/").is_err());
     assert!(spath_str(r#"/kk[kk"#).is_err());
     eq("/\\[k", &[b"[k"]);
@@ -313,15 +315,15 @@
 #[derive(Copy, Clone, Debug)]
 pub struct PathFE;
 
 impl EvalScopeImpl for PathFE {
     fn about(&self) -> (String, String) {
         (
             "path".into(),
-            r"spath and ipath utils. Usually [//some/path] is the most readable".into(),
+            r"path utils. Usually [//some/path] is the most readable".into(),
         )
     }
     fn list_funcs(&self) -> &[ScopeFunc<&Self>] {
         fn parse_range(i: &[&[u8]]) -> Result<Range<usize>, ApplyErr> {
             let start = parse_b::<usize>(i[1])?;
             let end = i
                 .get(2)
@@ -334,76 +336,55 @@
             Ok(start..end)
         }
         fn encode_sp(_:&PathFE,b:&[u8],_:&[ABE]) -> ApplyResult<String>{
            SPath::from_slice(b).ok().map(|p|format!("[/{p}]")).into()
         }
         
         crate::abe::fncs!([
-            ("?sp", 1..=1, "decode spath", |_, i: &[&[u8]]| Ok(
+            ("?p", 1..=1, "decode path", |_, i: &[&[u8]]| Ok(
                 SPath::from_slice(i[0])?.to_string().into_bytes()
             )),
-            ("?ip", 1..=1, "decode ipath", |_, i: &[&[u8]]| Ok(
-                IPath::from(i[0])?.to_string().into_bytes()
-            )),
             (
-                "ipcomp",
+                "path_idx",
                 2..=3,
-                "ipath select [start,?end]",
-                |_, i: &[&[u8]]| {
-                    Ok(IPath::from(i[0])?
-                        .range(parse_range(i)?)
-                        .ipath()
-                        .ipath_bytes()
-                        .to_vec())
-                }
-            ),
-            (
-                "spcomp",
-                2..=3,
-                "ipath select [start,?end]",
+                "path idx [start,?end]",
                 |_, i: &[&[u8]]| {
                     Ok(SPath::from_slice(i[0])?
                         .ipath()
                         .range(parse_range(i)?)
                         .spath_bytes()
                         .to_vec())
                 }
             ),
-            (
-                "ip",
-                1..=8,
-                "build ipath from arguments",
-                |_, i: &[&[u8]]| { Ok(IPathBuf::try_from_iter(i)?.ipath_bytes().to_vec()) }
-            ),
             (@C
-                "sp",
+                "p",
                 1..=8,
                 None,
-                "build spath from arguments",
+                "build path from arguments",
                 |_, i: &[&[u8]],_,_| { Ok(SPathBuf::try_from_iter(i)?.spath_bytes().to_vec()) },
                 encode_sp
             )
         ])
     }
-    fn list_eval(&self) -> &[ScopeEval<&Self>] {
+    fn list_macros(&self) -> &[ScopeMacro<&Self>] {
         &[
-            ScopeEval {
+            ScopeMacro {
                 apply: |_,inp:&[ABE],scope:&dyn Scope| {
                     let lst = abe::eval::eval(&EvalCtx { scope }, inp)?;
                     let p = SPathBuf::try_from(lst)?;
                     ApplyResult::Value(p.unwrap())
                 },
-                info: ScopeEvalInfo { id: "", help: "the 'empty' eval for build spath. i.e. [//some/spath/val] creates the byte for /some/spath/val" }
+                info: ScopeMacroInfo { id: "", help: "the 'empty' eval for encoding paths . i.e. [//some/spath/val] creates the byte for /some/spath/val" }
             },
-            ScopeEval {
+            ScopeMacro {
                 apply: |_,inp:&[ABE],scope:&dyn Scope| {
                     let mut lst = abe::eval::eval(&EvalCtx { scope }, inp)?;
                     let mut skip_first = true;
                     lst.lst.retain(|v| std::mem::take(&mut skip_first) ||  !v.0.is_empty());
                     let p = SPathBuf::try_from(lst)?;
                     ApplyResult::Value(p.unwrap())
                 },
-                info: ScopeEvalInfo { id: "~", help: "similar to '//' but forgiving on empty components" }
+                info: ScopeMacroInfo { id: "~", help: "similar to '//' but forgiving on empty components" }
             }
         ]
     }
 }
```

### Comparing `linkspace-0.1.4/local_dependencies/linkspace-pkt/src/spath_macro.rs` & `linkspace-0.3.0rc2/local_dependencies/linkspace-pkt/src/spath_macro.rs`

 * *Files identical despite different names*

### Comparing `linkspace-0.1.4/local_dependencies/linkspace-pkt/src/stamp.rs` & `linkspace-0.3.0rc2/local_dependencies/linkspace-pkt/src/stamp.rs`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 // Copyright Anton Sol
 //
 // This Source Code Form is subject to the terms of the Mozilla Public
 // License, v. 2.0. If a copy of the MPL was not distributed with this
 // file, You can obtain one at https://mozilla.org/MPL/2.0/.
-use std::time::{Duration, Instant, SystemTime, UNIX_EPOCH};
+use std::time::{Duration, Instant,  UNIX_EPOCH};
 
 /// current time as big endian u64 microseconds since epoch
 #[cfg(not(target_arch = "wasm32"))]
 pub fn now() -> Stamp {
-    from_systime(SystemTime::now())
+    from_systime(std::time::SystemTime::now())
 }
 pub fn from_systime(time: std::time::SystemTime) -> Stamp {
     let v = time
         .duration_since(UNIX_EPOCH)
         .expect("Time went backwards")
-        .as_micros() as u64;
-    Stamp::new(v)
+        .as_micros();
+    Stamp::new(unsafe{v.try_into().unwrap_unchecked()})
 }
 pub fn as_systime(stamp: Stamp) -> std::time::SystemTime {
     std::time::UNIX_EPOCH + Duration::from_micros(stamp.get())
 }
 pub fn as_instance(stamp: Stamp) -> Instant {
     // this seems dumb required 'now' twice.
     let now = now().get();
@@ -49,40 +49,45 @@
         return Err(Duration::from_micros(stamp - now));
     }
     Ok(Duration::from_micros(now - stamp))
 }
 
 /// saturating add
 pub fn stamp_add(stamp: Stamp, dur: Duration) -> Stamp {
-    let plus = dur.as_micros().min(u64::MAX as u128) as u64;
+    let plus = dur.as_micros().min(u64::MAX.into());
+    let plus = unsafe {u64::try_from(plus).unwrap_unchecked()};
     Stamp::new(stamp.get().saturating_add(plus))
 }
 pub fn checked_stamp_add(stamp: Stamp, dur: Duration) -> Option<Stamp> {
-    let plus = dur.as_micros().min(u64::MAX as u128) as u64;
+    let plus = dur.as_micros().min(u64::MAX.into());
+    let plus = unsafe {u64::try_from(plus).unwrap_unchecked()};
     stamp.get().checked_add(plus).map(Stamp::new)
 }
 /// saturating sub
 pub fn stamp_sub(stamp: Stamp, dur: Duration) -> Stamp {
-    let sub = dur.as_micros().min(u64::MAX as u128) as u64;
+    let sub = dur.as_micros().min(u64::MAX.into());
+    let sub = unsafe {u64::try_from(sub).unwrap_unchecked()};
     Stamp::new(stamp.get().saturating_sub(sub))
 }
 pub fn checked_stamp_sub(stamp: Stamp, dur: Duration) -> Option<Stamp> {
-    let sub = dur.as_micros().min(u64::MAX as u128) as u64;
+    let sub = dur.as_micros().min(u64::MAX.into());
+    let sub = unsafe {u64::try_from(sub).unwrap_unchecked()};
     stamp.get().checked_sub(sub).map(Stamp::new)
 }
-#[cfg(all(target_arch = "wasm32"))]
+#[cfg(target_arch = "wasm32")]
 use wasm_bindgen::prelude::*;
 
 use crate::Stamp;
 #[wasm_bindgen(inline_js = r#"
 export function date_now() {
   return Date.now();
 }"#)]
-#[cfg(all(target_arch = "wasm32"))]
+#[cfg(target_arch = "wasm32")]
 extern "C" {
     fn date_now() -> f64;
 }
 
-#[cfg(all(target_arch = "wasm32"))]
+#[cfg(target_arch = "wasm32")]
 pub fn now() -> Stamp {
     Stamp::new((date_now() * 1000.0) as u64)
 }
+
```

### Comparing `linkspace-0.1.4/local_dependencies/byte-fmt/Cargo.toml` & `linkspace-0.3.0rc2/local_dependencies/byte-fmt/Cargo.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,29 @@
 [package]
 name = "byte-fmt"
-version = "0.1.0"
-license = "MPL-2.0"
-edition = "2021"
-homepage = "https://antonsol919.github.io/linkspace/"
-authors = ["Azon <AntonSol919@gmail.com>"]
-repository = "https://github.com/AntonSol919/linkspace"
+version = "0.3.0-rc1"
+authors = ["Anton Sol <AntonSol919@gmail.com>"]
 categories = ["encoding","parsing"]
 keywords = ["base64","abe","newtype"]
 description = "B64 and AB newtype for parsing and printing"
 
+edition= "2021"
+license= "MPL-2.0"
+homepage= "https://www.linkspace.dev"
+documentation= "https://www.linkspace.dev/docs/guide/index.html"
+repository= "https://github.com/AntonSol919/linkspace"
+resolver = "2"
+
+
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 
 [dependencies]
+abe = { path = "../abe", version = "0.3.0-rc1"}
+
+serde= "=1.0.160"
+base64="=0.21"
+tracing= {version = "=0.1.37",features=["release_max_level_info"]}
 
-abe = { path = "../abe", version = "0.1.0"}
-serde = { version = "1.0.139", features = ["derive"] }
-base64 = "0.13.0"
-tracing = "0.1.35"
 serde_bytes = "0.11.6"
 ruint = "1.7.0"
+bytemuck = { version = "1.13.1", features = ["derive"] }
+
```

### Comparing `linkspace-0.1.4/local_dependencies/byte-fmt/LICENSE` & `linkspace-0.3.0rc2/local_dependencies/linkspace-common/LICENSE`

 * *Files identical despite different names*

### Comparing `linkspace-0.1.4/local_dependencies/byte-fmt/src/endian_types.rs` & `linkspace-0.3.0rc2/local_dependencies/byte-fmt/src/endian_types.rs`

 * *Files 2% similar despite different names*

```diff
@@ -32,14 +32,15 @@
             fn from(value: $name) -> Self{
                 $alt_endian::new(value.get())
             }
         }
 		    impl $name {
             #[inline(always)] pub const fn new(val: $native) -> $name{ $name(val.$to_bytes())}
             #[inline(always)] pub const fn get(self) -> $native{ $native::$from_bytes(self.0)}
+            #[inline(always)] pub fn set(&mut self,val:$native){ self.0 = val.$to_bytes()}
             pub const MAX : $name = $name::new($native::MAX);
             pub const ZERO : $name = $name::new(0);
             #[must_use]
             #[inline(always)] pub const fn incr(self) -> $name { $name::new(self.get().saturating_add(1))}
             #[inline(always)] pub const fn align(self) -> [$native;1] { [$native::from_ne_bytes(self.0)]}
             #[inline(always)] pub const fn to_bytes(self) -> [u8;$size] { self.0}
             pub const fn saturating_sub(self, rhs:Self) -> Self {
@@ -324,15 +325,15 @@
 fn fits() {
     assert_eq!(LU64::try_fit_slice(&[12]).unwrap().get(), 12)
 }
 
 #[test]
 fn abe() {
     fn io<T: ABEValidator + ToABE + PartialEq + std::fmt::Debug>(val: T) {
-        let ctx = crate::core_ctx();
+        let ctx = crate::abe::scope::core_ctx();
         let abe = val.to_abe();
         println!("{:?}", abe);
         let evals = crate::abe::TypedABE::<T>::from_unchecked(abe)
             .eval(&ctx)
             .map_err(|_| "err")
             .unwrap();
         assert_eq!(evals, val);
```

### Comparing `linkspace-0.1.4/local_dependencies/byte-fmt/src/lib.rs` & `linkspace-0.3.0rc2/local_dependencies/byte-fmt/src/lib.rs`

 * *Files 12% similar despite different names*

```diff
@@ -1,101 +1,88 @@
 // Copyright Anton Sol
 //
 // This Source Code Form is subject to the terms of the Mozilla Public
 // License, v. 2.0. If a copy of the MPL was not distributed with this
 // file, You can obtain one at https://mozilla.org/MPL/2.0/.
 #![allow(incomplete_features)]
 #![feature(
+    ptr_from_ref,
     array_windows,
     slice_flatten,
     int_roundings,
-    const_ptr_read,
     generic_const_exprs,
     bigint_helper_methods,
     const_bigint_helper_methods,
     const_option_ext
 )]
 pub mod endian_types;
 
 pub use base64 as base64_crate;
 use base64_crate::DecodeError;
 use core::ops::{Deref, DerefMut};
 use std::{
     borrow::{Borrow, Cow},
     mem::size_of,
-    str::FromStr,
+    str::FromStr, ptr,
 };
 
 
 pub use abe;
 pub use abe::eval;
 use abe::{
     abtxt::{ABTxtError, MAX_STR, as_abtxt},
-    ast::{as_bytes, no_ctrs, MatchError},
+    ast::{no_ctrs, MatchError},
     cut_prefix_nulls, cut_prefixeq,
-    eval::{ABList, ApplyResult, EScope, EvalScopeImpl, ScopeFunc, Comment},
-    fit_back, fncs, thiserror, ABEValidator, FitSliceErr, ToABE, ABE,
+    eval::{ABList },
+    fit_back, thiserror, ABEValidator, FitSliceErr, ToABE, ABE,
 };
 
 use std::fmt::{self, Debug, Display};
 
 pub fn as_abtxt_c(mut b: &[u8], cut: bool) -> std::borrow::Cow<'_, str> {
     if cut {
         b = cut_prefix_nulls(b)
     }
     abe::abtxt::as_abtxt(b)
 }
 
 pub fn ab_slice<X>(i: &[X]) -> &[AB<X>] {
-    unsafe { std::mem::transmute(i) }
+    unsafe { std::slice::from_raw_parts(i.as_ptr().cast(), i.len())}
 }
 
-pub fn base64(b: impl AsRef<[u8]>) -> String {
-    base64_crate::encode_config(b.as_ref(), base64_crate::URL_SAFE_NO_PAD)
-}
-pub fn base64_decode(st: impl AsRef<[u8]>) -> Result<Vec<u8>, DecodeError> {
-    base64::decode_config(st, base64::URL_SAFE_NO_PAD)
-}
+use base64_crate::prelude::*;
 
 pub fn b64(b: &[u8], mini: bool) -> String {
     if mini{
         mini_b64(b)
     } else {
         base64(b)
     }
 }
-pub fn mini_b64(v: &[u8]) -> String {
-    let mut r = String::with_capacity(10);
-    let len = v.len();
-    let padc = len / 8;
-    let st = base64::encode_config(v, base64::URL_SAFE_NO_PAD);
-    if v.len() <= 12 {
-        return st;
-    }
-    r.push_str(&st[0..6]);
-    r.push_str(&":".repeat(padc / 2));
-    if padc % 2 != 0 {
-        r.push('.');
-    }
-    r.push_str(&st[st.len() - 2..]);
-    r
-}
+pub use abe::scope::base::{base64,base64_decode,mini_b64};
 
-#[derive(Default, Copy, Clone, Hash, PartialEq, Eq, PartialOrd, Ord)]
+use bytemuck::{Pod,Zeroable};
+
+#[derive(Default, Copy, Clone, Hash, PartialEq, Eq, PartialOrd, Ord,Pod,Zeroable)]
 #[repr(transparent)]
 /// newtype around bytes to print/parse [[abe]] text
 pub struct AB<N: ?Sized = Vec<u8>>(pub N);
-#[derive(Default, Copy, Clone, Hash, PartialEq, Eq, PartialOrd, Ord)]
+#[derive(Default, Copy, Clone, Hash, PartialEq, Eq, PartialOrd, Ord,Pod,Zeroable)]
 #[repr(transparent)]
 /// newtype around bytes to print/parse b64 (url-safe no-padding)
 pub struct B64<N = [u8; 32]>(pub N);
 
 impl<'o> From<&'o [u8]> for &'o AB<[u8]> {
     fn from(d: &'o [u8]) -> Self {
-        unsafe { *(d.as_ptr() as *const Self) }
+        AB::from_ref(d)
+    }
+}
+impl<N:?Sized> AB<N>{
+    pub fn from_ref(b: &N) -> &AB<N> {
+        unsafe { std::mem::transmute(b)}
     }
 }
 
 impl<N> AB<N>
 where
     Self: AsRef<[u8]>,
 {
@@ -149,14 +136,25 @@
         let st : &str= st.borrow();
         if self.as_ref().len() == 16 {
             abe::abe!({ mode : st  }).for_each(out)
         } else {
             abe::abe!({ mode : st : (self.as_ref().len().to_string()) }).for_each(out)
         }
     }
+    fn to_abe_str(&self) -> String {
+        let (max_padded, bytes) = self.x_prefix_cut();
+        let mode = if max_padded { MAX_STR } else { "a" };
+        let st = abe::abtxt::as_abtxt(bytes);
+        let st : &str= st.borrow();
+        if self.as_ref().len() == 16 {
+            format!("[{mode}:{st}]")
+        } else {
+            format!("[{mode}:{st}:{}]",self.as_ref().len())
+        }
+    }
 }
 
 #[derive(thiserror::Error, Debug)]
 pub struct ParseErr<E: std::error::Error> {
     pub source: E,
     pub st: String,
 }
@@ -363,36 +361,40 @@
     fn as_ref(&self) -> &N {
         &self.0
     }
 }
 
 impl AsRef<[u8; 32]> for B64<[u128; 2]> {
     fn as_ref(&self) -> &[u8; 32] {
-        unsafe { std::mem::transmute(self) }
+        unsafe { &*std::ptr::from_ref(self).cast()}
     }
 }
 impl<N> ToABE for B64<N>
 where
     Self: AsRef<[u8]>{
 
     fn write_abe(&self, out: &mut dyn FnMut(ABE)) {
         abe::abe!( { "b" : (self.b64()) } ).for_each(out)
     }
+
+    fn to_abe_str(&self) -> String {
+        format!("[b:{}]",self)
+    }
 }
 
 impl<N> B64<N> {
     #[inline(always)]
     pub fn into_bytes(self) -> [u8; size_of::<Self>()] {
-        unsafe { *(&self as *const Self as *const [u8; size_of::<Self>()]) }
+        unsafe { *(ptr::from_ref(&self).cast::<[u8;size_of::<Self>()]>()) }
     }
     pub fn inner(self) -> N {
         self.0
     }
     pub fn from_ref(b: &N) -> &B64<N> {
-        unsafe { std::mem::transmute(b) }
+        unsafe { &*ptr::from_ref(b).cast() }
     }
 }
 
 impl<const L: usize> TryFrom<ABList> for B64<[u8; L]> {
     type Error = DecodeError;
     fn try_from(value: ABList) -> Result<Self, Self::Error> {
         let bytes = value.as_exact_bytes().map_err(|_| {
@@ -425,14 +427,17 @@
 {
     pub fn b64(&self) -> String {
         base64(self.as_ref())
     }
     pub fn b64_mini(&self) -> String {
         mini_b64(self.as_ref())
     }
+    pub fn b64_into(&self, output_buf:&mut String){
+        BASE64_URL_SAFE_NO_PAD.encode_string(self.as_ref(), output_buf)
+    }
 }
 
 
 impl<N> Borrow<N> for B64<N> {
     fn borrow(&self) -> &N {
         &self.0
     }
@@ -474,18 +479,16 @@
     }
     pub fn parse_str(st: impl AsRef<[u8]>) -> Result<Self, base64::DecodeError> {
         let s = st.as_ref();
         if s.len() != (N * 4).div_ceil(3) {
             return Err(base64::DecodeError::InvalidLength);
         }
         let mut this: [u8; N] = [0; N];
-        let r = base64::decode_config_slice(s, base64::URL_SAFE_NO_PAD, &mut this)?;
-        if r != N {
-            panic!()
-        };
+        let r = BASE64_URL_SAFE_NO_PAD.decode_slice_unchecked(s,&mut this)?;
+        debug_assert!(r == N);
         Ok(B64(this))
     }
 }
 impl<const L: usize> TryFrom<&[u8]> for B64<[u8; L]> {
     type Error = FitSliceErr;
     fn try_from(value: &[u8]) -> Result<Self, Self::Error> {
         Self::try_fit_slice(value)
@@ -500,73 +503,27 @@
     }
 }
 impl<N> Display for B64<N>
 where
     Self: AsRef<[u8]>,
 {
     fn fmt(&self, f: &mut fmt::Formatter<'_>) -> fmt::Result {
-        f.write_str(&base64(self.as_ref()))
+        base64_crate::display::Base64Display::new(&self.as_ref(), &BASE64_URL_SAFE_NO_PAD).fmt(f)
     }
 }
 impl<N> std::fmt::Debug for B64<N>
 where
     Self: AsRef<[u8]>,
 {
     fn fmt(&self, f: &mut fmt::Formatter<'_>) -> fmt::Result {
-        f.write_str(&base64(self.as_ref()))
-    }
-}
-/// Implements [AAAAAA/b64] and [\0\0\xff/2b64]
-#[derive(Copy, Clone, Debug)]
-pub struct B64EvalFnc;
-impl EvalScopeImpl for B64EvalFnc {
-    fn about(&self) -> (String, String) {
-        ("b64".into(), "base64 url-safe no-padding".into())
-    }
-    fn list_funcs(&self) -> &[ScopeFunc<&Self>] {
-        fncs!([
-            ("?b",1..=1,"encode base64",|_,i:&[&[u8]]| Ok(base64(i[0]).into_bytes())),
-            ("2mini",1..=1,"encode mini",|_,i:&[&[u8]]| Ok(mini_b64(i[0]).into_bytes())),
-            ( @C "b", 1..=1, None, "decode base64",
-               |_,i:&[&[u8]],_,_| Ok(base64_decode(i[0])?),
-               |_,b:&[u8],opts:&[ABE]| -> ApplyResult<String>{
-                   if opts.is_empty(){
-                       return ApplyResult::Value(format!("[b:{}]",base64(b)));
-                   }
-                   for len_st in opts.iter().filter_map(|v| as_bytes(v).ok()){
-                       let len = std::str::from_utf8(len_st)?.parse::<u32>()?;
-                       if len as usize == b.len() {
-                           return ApplyResult::Value(format!("[b:{}]",base64(b)));
-                       }
-                   }
-                   ApplyResult::NoValue
-               }
-             )
-        ])
+        Display::fmt(self, f)
     }
 }
 
-use abe::eval::{BytesFE, Encode, EvalCtx, Help, LogicOps, UIntFE};
-pub type EvalCore = (
-    (EScope<BytesFE>, EScope<UIntFE>, EScope<B64EvalFnc>),
-    ((EScope<Comment>,EScope<Help>), EScope<LogicOps>, EScope<Encode>),
-);
-pub type EvalCoreCtx = EvalCtx<EvalCore>;
-pub const EVAL_SCOPE: EvalCore = core_scope();
-pub const fn core_scope() -> EvalCore {
-    (
-        (EScope(BytesFE), EScope(UIntFE), EScope(B64EvalFnc)),
-        ((EScope(Comment),EScope(Help)), EScope(LogicOps), EScope(Encode)),
-    )
-}
-pub const fn core_ctx() -> EvalCoreCtx {
-    EvalCtx {
-        scope: core_scope()
-    }
-}
+
 
 impl AB<[u8;16]> {
     pub const fn to_u128(self) -> u128 {
         u128::from_be_bytes(self.0)
         
     }
     pub const fn from_u128(value:u128) -> Self {
@@ -613,7 +570,25 @@
     }
 }
 impl From<U512> for B64<[u8; 64]> {
     fn from(val: U512) -> Self {
         B64(val.to_be_bytes())
     }
 }
+
+#[test]
+fn casts(){
+    let s = ab_slice(&[b"abc",b"123"]);
+    assert_eq!(s[0].0 , b"abc");
+    assert_eq!(s[1].0 , b"123");
+    assert_eq!("abc",AB::from_ref(b"abc").to_string());
+    assert_eq!(B64([1;32]) ^ B64([3;32]),B64([2;32]));
+    assert_eq!(B64([1;32]) ^ B64([3;32]),B64([2;32]));
+    assert_eq!(B64([1u8;32]).into_bytes(), [1;32]);
+    assert_eq!(&[32;32],&B64::from_ref(&[32;32]).0);
+
+
+    let o : &[u8;32] = B64([1u128;2]).as_ref();
+    let i = u128::from_ne_bytes(o[0..16].try_into().unwrap());
+    assert_eq!(i,1);
+    panic!("ok")
+}
```

### Comparing `linkspace-0.1.4/local_dependencies/byte-fmt/src/serde.rs` & `linkspace-0.3.0rc2/local_dependencies/byte-fmt/src/serde.rs`

 * *Files identical despite different names*

### Comparing `linkspace-0.1.4/Makefile` & `linkspace-0.3.0rc2/Makefile`

 * *Files 16% similar despite different names*

```diff
@@ -12,21 +12,14 @@
 
 watch-dev: setup_env
 	. .env/bin/activate && ( watchexec -r -e rs -- maturin develop )
 
 doc: build
 	. .env/bin/activate && pdoc linkspace
 
-# this is a temporary hack https://pyo3.rs/v0.18.2/python_typing_hints
-typestub: setup_env
-	. .env/bin/activate && (pip install mypy ; stubgen -p linkspace)
-	mv out/linkspace/linkspace.pyi ./
-	cp ./linkspace.pyi ../../target/debug/
-	rm -r out
-
 build: setup_env
 	. .env/bin/activate && (  maturin build )
 
 install: build
 	pip install --force-reinstall ../../target/wheels/linkspace-*.whl
 
 publish: setup_env
```

### Comparing `linkspace-0.1.4/src/lib.rs` & `linkspace-0.3.0rc2/src/lib.rs`

 * *Files 5% similar despite different names*

```diff
@@ -7,17 +7,16 @@
     control_flow_enum,
     io_error_other,
     iterator_try_collect,
     thread_local,
     duration_constants
 )]
 
-use anyhow::Context;
-use ref_cast::RefCast;
-use std::{ops::ControlFlow, path::{Path, PathBuf}, time::Duration};
+use anyhow::{Context, anyhow};
+use std::{ops::ControlFlow, path::{Path, PathBuf}, time::{Duration, Instant}};
 
 use ::linkspace as linkspace_rs;
 use ::linkspace::{prelude::*, abe::ctx::{UserData, self} };
 use pyo3::{
     prelude::*,
     types::{PyBytes,  PyTuple},
 };
@@ -44,40 +43,54 @@
         ("<unknown>", line_num)
     }
 }
 
 pub type PyFunc = Py<PyAny>;
 
 struct PyPktStreamHandler {
-    on_match: PyFunc,
+    on_match: Option<PyFunc>,
     on_close: Option<PyFunc>,
     on_err: Option<PyFunc>
 }
+
 impl PktHandler for PyPktStreamHandler {
     fn handle_pkt(
         &mut self,
         pkt: &dyn NetPkt,
         _lk: &linkspace_rs::Linkspace,
     ) -> std::ops::ControlFlow<()> {
         let apkt = Pkt::from_dyn(pkt);
-        match Python::with_gil(|py| call_cont_py(py, &self.on_match, (apkt,))) {
-            Ok(true) => ControlFlow::Continue(()),
-            Ok(false) => ControlFlow::Break(()),
-            Err(e) => {
-                if let Some(f) = &self.on_err{
-                    let apkt = Pkt::from_dyn(pkt);
-                    match Python::with_gil(|py| call_cont_py(py, f, (e,apkt,&self.on_match))){
-                        Ok(true) => return ControlFlow::Continue(()),
-                        Ok(false) => {},
-                        Err(e) => tracing::warn!(?e,"Yo dog i heard i liked errors"),
+        let on_match = match &self.on_match{
+            Some(f) => f,
+            None => return ControlFlow::Continue(())
+        };
+        Python::with_gil(|py| {
+            match call_cont_py(py, on_match, (apkt,)) {
+                Ok(true) => ControlFlow::Break(()),
+                Ok(false) => ControlFlow::Continue(()),
+                Err(e) => {
+                    if let Some(f) = &self.on_err{
+                        let apkt = Pkt::from_dyn(pkt);
+                        match call_cont_py(py, f, (&e,apkt,&self.on_match)){
+                            Ok(true) => return ControlFlow::Continue(()),
+                            Ok(false) => {},
+                            Err(on_err_err) => {
+                                tracing::warn!(%e,tb=e.traceback(py).map(|v| v.format().unwrap()).unwrap_or(format!("?")),
+                                               %on_err_err,tbee=on_err_err.traceback(py).map(|v| v.format().unwrap()).unwrap_or(format!("?")),
+                                               "Yo dog i heard you liked errors")
+                            },
+                        }
+                    }else {
+                        let tb = e.traceback(py).map(|v| v.format().unwrap()).unwrap_or(format!("?"));
+                        tracing::warn!(%e,tb,"default error handler (add on_err function to capture this event) ")
                     }
-                }else { tracing::warn!("default error handler " )}
-                return ControlFlow::Break(());
+                    return ControlFlow::Break(());
+                }
             }
-        }
+        })
     }
     fn stopped(
         &mut self,
         _query: linkspace_rs::Query,
         _lk: &linkspace_rs::Linkspace,
         _reason: misc::StopReason,
         _total: u32,
@@ -86,29 +99,36 @@
         if let Some(_f) = &self.on_close {
             todo!("handle stopped");
             //if let Err(e) = Python::with_gil(|py|f.call0(py));
         }
     }
 }
 
+fn grp_arg(group:Option<&[u8]>) -> anyhow::Result<GroupID>{
+    match group{
+        None => Ok(linkspace_rs::prelude::group()),
+        Some(bytes) => Ok(GroupID::try_fit_bytes_or_b64(bytes)?)
+    }
+}
+fn domain_arg(domain:Option<&[u8]>) -> anyhow::Result<Domain>{
+    match domain{
+        None => Ok(linkspace_rs::prelude::domain()),
+        Some(bytes) => Ok(Domain::try_fit_byte_slice(bytes)?) 
+    }
+}
+
 fn common_args(
     group: Option<&[u8]>,
     domain: Option<&[u8]>,
     path: Option<&PyAny>,
     links: Option<Vec<crate::pynetpkt::Link>>,
     create_stamp: Option<&[u8]>,
 ) -> anyhow::Result<(GroupID, Domain, IPathBuf, Vec<Link>, Option<Stamp>)> {
-    let group = group
-        .map(|group| GroupID::try_fit_bytes_or_b64(group))
-        .transpose()?
-        .unwrap_or(consts::PUBLIC);
-    let domain = domain
-        .map(|domain| Domain::try_fit_byte_slice(domain))
-        .transpose()?
-        .unwrap_or(AB::default());
+    let group = grp_arg(group)?;
+    let domain = domain_arg(domain)?;
     let path = match path {
         None => IPathBuf::new(),
         Some(p) => {
             if let Ok(p) = p.downcast::<PyBytes>(){
                 SPath::from_slice(p.as_bytes())?.into_spathbuf().try_ipath()?
             }else {
                 let path = p
@@ -144,87 +164,87 @@
 use tracing::debug_span;
 
 #[pyfunction]
 pub fn lk_keygen() -> SigningKey {
     SigningKey(linkspace_rs::key::lk_keygen())
 }
 #[pyfunction]
-pub fn lk_keystr(key: &SigningKey, password: &[u8]) -> String {
-    linkspace_rs::key::lk_keystr(&key.0, password)
+pub fn lk_key_encrypt(key: &SigningKey, password: &[u8]) -> String {
+    linkspace_rs::key::lk_key_encrypt(&key.0, password)
 }
 #[pyfunction]
-pub fn lk_keyopen(_py: Python, id: &str, password: &[u8]) -> anyhow::Result<SigningKey> {
-    Ok(SigningKey(linkspace_rs::key::lk_keyopen(id, password)?))
+pub fn lk_key_decrypt(_py: Python, id: &str, password: &[u8]) -> anyhow::Result<SigningKey> {
+    Ok(SigningKey(linkspace_rs::key::lk_key_decrypt(id, password)?))
 }
 
-const E:&[u8]=&[];
 #[pyfunction]
-#[pyo3(signature =(lk,password=E,name="me:local",create=false))]
 pub fn lk_key(
     lk: &Linkspace,
-    password: &[u8],
-    name: &str,
-    create: bool,
+    password: Option<&[u8]>,
+    name: Option<&str>,
+    create: Option<bool>,
 ) -> anyhow::Result<SigningKey> {
-    linkspace_rs::lk_key(&lk.0, password, name, create).map(SigningKey)
+    linkspace_rs::lk_key(&lk.0, password, name, create.unwrap_or(false)).map(SigningKey)
 }
 
 #[pyfunction]
 pub fn lk_datapoint(data: &PyAny) -> anyhow::Result<Pkt> {
     Ok(pynetpkt::Pkt::from_dyn(
         &linkspace_rs::point::lk_datapoint_ref(bytelike(data)?)?,
     ))
 }
 #[pyfunction]
 pub fn lk_linkpoint(
+    data: Option<&PyAny>,
     group: Option<&[u8]>,
     domain: Option<&[u8]>,
     path: Option<&PyAny>,
     links: Option<Vec<crate::pynetpkt::Link>>,
-    data: Option<&PyAny>,
     create: Option<&[u8]>,
 ) -> anyhow::Result<Pkt> {
     let data = data.map(bytelike).transpose()?.unwrap_or(&[]);
     let (group, domain, path, links, create) = common_args(group, domain, path, links, create)?;
-    let pkt = linkspace_rs::point::lk_linkpoint_ref(domain, group, &*path, &*links, data, create)?;
+    let pkt = linkspace_rs::point::lk_linkpoint_ref(data,domain, group, &*path, &*links, create)?;
     Ok(pynetpkt::Pkt::from_dyn(&pkt))
 }
 #[pyfunction]
 pub fn lk_keypoint(
     key: &SigningKey,
+    data: Option<&PyAny>,
     group: Option<&[u8]>,
     domain: Option<&[u8]>,
     path: Option<&PyAny>,
     links: Option<Vec<crate::pynetpkt::Link>>,
-    data: Option<&PyAny>,
     create: Option<&[u8]>,
 ) -> anyhow::Result<Pkt> {
     let data = data.map(bytelike).transpose()?.unwrap_or(&[]);
     let (group, domain, path, links, create) = common_args(group, domain, path, links, create)?;
     let pkt =
-        linkspace_rs::point::lk_keypoint_ref(domain, group, &*path, &*links, data, create, &key.0)?;
+        linkspace_rs::point::lk_keypoint_ref(&key.0,data,domain, group, &*path, &*links, create)?;
     Ok(pynetpkt::Pkt::from_dyn(&pkt))
 }
 
 fn pptr(p: Option<&Pkt>) -> Option<&dyn NetPkt> {
     p.map(|p| &p.0 as &dyn NetPkt)
 }
 
 #[pyfunction]
-pub fn lk_write<'a>(py: Python<'a>, pkt: &Pkt) -> anyhow::Result<&'a PyBytes> {
+#[pyo3(signature =(pkt,allow_private=false))]
+pub fn lk_write<'a>(py: Python<'a>, pkt: &Pkt, allow_private:bool) -> PyResult<&'a PyBytes> {
     // TODO remove this copy
-    let mut v = vec![];
-    linkspace_rs::point::lk_write(&pkt.0, &mut v)?;
-    Ok(PyBytes::new(py, &v))
+    PyBytes::new_with(py, pkt.0.size() as usize, |dest|{
+        Ok(linkspace_rs::point::lk_write(&pkt.0,allow_private,&mut std::io::Cursor::new(dest))?)
+    })
 }
+
 #[pyfunction]
-pub fn lk_read(buf: &[u8], validate: bool, allow_private: bool) -> anyhow::Result<(Pkt, &[u8])> {
-    let p = linkspace_rs::point::lk_read(buf, validate, allow_private)?;
-    let size = p.size();
-    Ok((Pkt::from_dyn(&p), &buf[size..]))
+#[pyo3(signature =(buf,allow_private=false))]
+pub fn lk_read(buf: &[u8], allow_private: bool) -> std::io::Result<(Pkt, &[u8])> {
+    let (pkt,rest) = linkspace_rs::point::lk_read(buf, allow_private).map_err(std::io::Error::other)?;
+    Ok((Pkt::from_dyn(pkt.as_ref()),rest))
 }
 
 #[pyfunction]
 pub fn lk_eval<'a>(
     py: Python<'a>,
     expr: &str,
     pkt: Option<&Pkt>,
@@ -257,23 +277,23 @@
     }
 }
 #[pyfunction]
 pub fn lk_encode(bytes: &[u8], options: Option<&str>) -> anyhow::Result<String> {
     Ok(linkspace_rs::abe::lk_encode(bytes, options.unwrap_or("")))
 }
 #[pyclass(unsendable)]
-#[derive(Clone, RefCast)]
+#[derive(Clone )]
 #[repr(transparent)]
 pub struct Linkspace(pub(crate) linkspace_rs::Linkspace);
 
 #[pyfunction]
-#[pyo3(signature =(path="",create=false))]
-pub fn lk_open(path: &str, create: bool) -> anyhow::Result<Linkspace> {
+#[pyo3(signature =(dir="",create=false))]
+pub fn lk_open(dir: &str, create: bool) -> anyhow::Result<Linkspace> {
     Ok(Linkspace(linkspace_rs::lk_open(
-        if path.is_empty(){None} else {Some(Path::new(path))},
+        if dir.is_empty(){None} else {Some(Path::new(dir))},
         create,
     )?))
 }
 #[pyfunction]
 pub fn lk_save(runtime: &Linkspace, pkt: &Pkt) -> anyhow::Result<bool> {
     Ok(linkspace_rs::lk_save(&runtime.0, pkt.0.netpktptr())?)
 }
@@ -290,15 +310,15 @@
 #[pymethods]
 impl Query{
     pub fn __str__(&self) -> String { lk_query_print(self, true) }
 }
 
 #[pyfunction]
 pub fn lk_query(copy_from: Option<&Query>) -> Query {
-    Query(linkspace_rs::lk_query(copy_from.map(|v| &v.0)))
+    Query(linkspace_rs::lk_query(copy_from.map(|v| &v.0).unwrap_or(&Q)))
 }
 #[pyfunction]
 pub fn lk_hash_query(hash: &PyAny) -> anyhow::Result<Query> {
     let hash = LkHash::try_fit_bytes_or_b64(bytelike(hash)?)?;
     Ok(Query(linkspace_rs::query::lk_hash_query(hash)))
 }
 fn bytelike(p: &PyAny) -> PyResult<&[u8]> {
@@ -344,49 +364,48 @@
     func: &PyFunc,
     args: impl IntoPy<Py<PyTuple>>,
 ) -> PyResult<bool> {
     let result = func.call1(py, args)?;
     let as_bool = result.extract::<bool>(py);
     match as_bool {
         Ok(b) => Ok(b) as PyResult<bool>,
-        Err(_) => Ok(true),
+        Err(_) => Ok(false),
     }
 }
 
 #[pyfunction]
 pub fn lk_get(lk: &Linkspace, query: &Query) -> anyhow::Result<Option<Pkt>> {
     linkspace_rs::runtime::lk_get_ref(&lk.0, &query.0, &mut |pkt| Pkt::from_dyn(&pkt))
 }
 #[pyfunction]
-// Returning an iterator would force us to keep the readtxn open
 pub fn lk_get_all(
     py: Python,
     lk: &Linkspace,
     query: &Query,
     cb: PyFunc,
-) -> anyhow::Result<u32> {
+) -> anyhow::Result<i32> {
     let mut cb_err = Ok(());
     let count = linkspace_rs::runtime::lk_get_all(&lk.0, &query.0, &mut |pkt| {
         let pkt = Pkt::from_dyn(pkt);
-        let mut cont = false;
-        cb_err = call_cont_py(py, &cb, (pkt,)).map(|c| cont = c);
-        cont
+        let mut breaks = false;
+        cb_err = call_cont_py(py, &cb, (pkt,)).map(|c| breaks = c);
+        breaks
     })?;
     cb_err?;
     Ok(count)
 }
 #[pyfunction]
 pub fn lk_watch(
     py: Python,
     lk: &Linkspace,
     query: &Query,
-    on_match: PyFunc,
+    on_match: Option<PyFunc>,
     on_close: Option<PyFunc>,
     on_err: Option<PyFunc>,
-) -> anyhow::Result<u32> {
+) -> anyhow::Result<i32> {
     let watch_handler = PyPktStreamHandler { on_match, on_close,on_err };
     let (file, line) = call_ctx(py);
     let span = debug_span!("lk_watch",%file,%line);
     linkspace_rs::runtime::lk_watch2(&lk.0, &query.0, watch_handler, span)
 }
 #[pyfunction]
 pub fn lk_list_watches(py: Python, lk: &Linkspace, cb: PyFunc) -> PyResult<PyObject> {
@@ -404,155 +423,152 @@
 pub fn lk_process(lk: &Linkspace) -> [u8; 8] {
     linkspace_rs::lk_process(&lk.0).0
 }
 
 #[pyfunction]
 pub fn lk_process_while(
     lk: &Linkspace,
-    watch: Option<&[u8]>,
-    watch_finish:Option<bool>,
-    max_wait: Option<&[u8]>,
-    until: Option<&[u8]>,
-) -> anyhow::Result<bool> {
-    let as_stamp = |opt| match opt{
-        None => Ok(Stamp::MAX),
-        Some(v) if v == &[0;8] => Ok(Stamp::MAX),
-        Some(v) => Stamp::try_from(v)
-    };
-    let max_wait = as_stamp(max_wait)?;
-    let until = as_stamp(until)?;
-
+    qid: Option<&[u8]>,
+    timeout: Option<&[u8]>,
+) -> anyhow::Result<isize> {
     // we do a little dance to check signals ( Ctr+C )  every 1 second
-    const CHECK_SIGNALS_INTERVAL: Stamp = Stamp::new(Duration::SECOND.as_micros() as u64);
-    let mut check_at = now().saturating_add(CHECK_SIGNALS_INTERVAL);
-    let mut empty_watches = false;
-    let watch = watch.map(|id| (id,watch_finish.unwrap_or(false)));
-    while !empty_watches && until > check_at {
-        empty_watches = linkspace_rs::lk_process_while(&lk.0,watch, max_wait, check_at)?;
-        tracing::trace!("Checking signals");
+    let timeout = timeout.map(Stamp::try_from).transpose()?.filter(|v| *v != Stamp::ZERO);
+    let until =  timeout.map(|t| Instant::now() + Duration::from_micros(t.get()));
+    loop{
+        let mut check_at = Instant::now() + Duration::SECOND;
+        if let Some(u) = until { check_at = check_at.min(u) };
+        let result = linkspace_rs::runtime::_lk_process_while(&lk.0,qid, Some(check_at))?;
         Python::with_gil(|py| py.check_signals())?;
-        check_at = check_at.saturating_add(CHECK_SIGNALS_INTERVAL);
-        check_at = check_at.max(now());
+        if result != 0 || Some(check_at) ==  until { return Ok(result)}
     }
-    Ok(empty_watches)
+}
+
+#[pyfunction]
+#[pyo3(signature =(lk,id,range=false))]
+pub fn lk_stop(lk: &Linkspace, id: &[u8], range: bool) {
+    linkspace_rs::runtime::lk_stop(&lk.0, id, range)
 }
 #[pyfunction]
 pub fn lk_status_set(
     lk: &Linkspace,
-    callback: PyFunc,
-    group: &[u8],
-    domain: &[u8],
+    qid: &[u8],
     objtype: &[u8],
+    callback: PyFunc,
+    group: Option<&[u8]>,
+    domain: Option<&[u8]>,
     instance: Option<&[u8]>,
 ) -> anyhow::Result<()> {
     use linkspace_rs::conventions::status::*;
-    let group = GroupID::try_fit_bytes_or_b64(group)?;
-    let domain = Domain::try_fit_byte_slice(domain)?;
+    let group = grp_arg(group)?;
+    let domain = domain_arg(domain)?;
     let status_ctx = LkStatus {
         domain,
         group,
         objtype,
         instance,
+        qid
     };
     tracing::info!("setup status {:?}",status_ctx);
     lk_status_set(&lk.0, status_ctx, move |_lk, domain, group, path, link| {
         tracing::info!("get gil status");
         Python::with_gil(|py| {
             let val = callback.call0(py)?;
             let bytes = bytelike(val.as_ref(py))?;
 
-            let pkt = linkspace_rs::lk_linkpoint(domain, group, path, &[link], bytes, None);
+            let pkt = linkspace_rs::lk_linkpoint(bytes, domain, group, path, &[link], None);
             tracing::info!("Status result {:?}",pkt);
             pkt
         })
     })
 }
 #[pyfunction]
 pub fn lk_status_poll(
     lk: &Linkspace,
-    callback: PyFunc,
-    timeout: &[u8],
-    group: &[u8],
-    domain: &[u8],
+    qid: &[u8],
     objtype: &[u8],
+    timeout: &[u8],
     instance: Option<&[u8]>,
-    watch_id: Option<&[u8]>
-) -> anyhow::Result<()> {
+    callback: Option<PyFunc>,
+    group: Option<&[u8]>,
+    domain: Option<&[u8]>,
+) -> anyhow::Result<bool> {
     use linkspace_rs::conventions::status::*;
     let timeout = Stamp::try_from(timeout)?;
-    let group = GroupID::try_fit_bytes_or_b64(group)?;
-    let domain = Domain::try_fit_byte_slice(domain)?;
+    let group = grp_arg(group)?;
+    let domain = domain_arg(domain)?;
     let status_ctx = LkStatus {
         domain,
         group,
         objtype,
         instance,
+        qid
     };
     let handler = PyPktStreamHandler {
         on_match: callback,
         on_close: None,
         on_err:None
     };
-    lk_status_poll(&lk.0, status_ctx, timeout, handler,watch_id)
+    lk_status_poll(&lk.0, status_ctx, timeout, handler)
 }
 
+
 #[pyfunction]
 pub fn lk_pull<'o>(py: Python<'o>, lk: &Linkspace, query: &Query) -> anyhow::Result<&'o PyBytes> {
     let hash = linkspace_rs::conventions::lk_pull(&lk.0, &query.0)?;
     Ok(PyBytes::new(py, &hash.0))
 }
 
 
 #[pyclass]
 #[pyo3(get_all)]
 pub struct LkInfo {
-    pub path:PathBuf
+    pub dir:PathBuf
 }
 #[pyfunction]
 pub fn lk_info<'o>(lk: &Linkspace) -> anyhow::Result<LkInfo> {
     let linkspace_rs::runtime::LkInfo{
-        path
+        dir
     }= linkspace_rs::runtime::lk_info(&lk.0);
-    Ok(LkInfo{path:path.into()})
+    Ok(LkInfo{dir:dir.into()})
 }
 
 
 
 
-/** linkspace python bindings. follows the linkspace api (https://antonsol919.github.io/linkspace/docs/cargo-doc/linkspace/index.html)
+/** linkspace python bindings. follows the linkspace api (https://www.linkspace.dev/docs/cargo-doc/linkspace/index.html)
 **/
 #[pymodule]
 fn linkspace(py: Python, m: &PyModule) -> PyResult<()> {
-    let filter = tracing_subscriber::EnvFilter::from_default_env();
+    let filter = tracing_subscriber::EnvFilter::builder()
+        .with_default_directive(tracing::metadata::LevelFilter::WARN.into())
+        .from_env().map_err(|e| anyhow!("RUST_LOG error {:?}",e))?;
     tracing_subscriber::fmt()
         .with_env_filter(filter)
         .pretty()
         .with_thread_ids(true)
         .with_thread_names(true)
         .init();
 
     m.add_class::<pynetpkt::Pkt>()?;
     m.add_class::<pynetpkt::Links>()?;
     m.add_class::<pynetpkt::Link>()?;
     m.add_class::<crate::Linkspace>()?;
     m.add_class::<crate::Query>()?;
 
-    m.add_function(wrap_pyfunction!(crate::b64, m)?)?;
-    m.add_function(wrap_pyfunction!(crate::spath, m)?)?;
 
     m.add_function(wrap_pyfunction!(crate::lk_datapoint, m)?)?;
     m.add_function(wrap_pyfunction!(crate::lk_linkpoint, m)?)?;
     m.add_function(wrap_pyfunction!(crate::lk_keypoint, m)?)?;
 
     m.add_function(wrap_pyfunction!(crate::lk_read, m)?)?;
     m.add_function(wrap_pyfunction!(crate::lk_write, m)?)?;
 
     m.add_function(wrap_pyfunction!(crate::lk_keygen, m)?)?;
-    m.add_function(wrap_pyfunction!(crate::lk_keystr, m)?)?;
-    m.add_function(wrap_pyfunction!(crate::lk_keyopen, m)?)?;
+    m.add_function(wrap_pyfunction!(crate::lk_key_encrypt, m)?)?;
+    m.add_function(wrap_pyfunction!(crate::lk_key_decrypt, m)?)?;
 
     m.add_function(wrap_pyfunction!(crate::lk_eval, m)?)?;
     m.add_function(wrap_pyfunction!(crate::lk_eval2str, m)?)?;
     m.add_function(wrap_pyfunction!(crate::lk_encode, m)?)?;
 
     m.add_function(wrap_pyfunction!(crate::lk_query, m)?)?;
     m.add_function(wrap_pyfunction!(crate::lk_hash_query, m)?)?;
@@ -570,20 +586,34 @@
     m.add_function(wrap_pyfunction!(crate::lk_watch, m)?)?;
     m.add_function(wrap_pyfunction!(crate::lk_process, m)?)?;
     m.add_function(wrap_pyfunction!(crate::lk_process_while, m)?)?;
 
     m.add_function(wrap_pyfunction!(crate::lk_list_watches, m)?)?;
     m.add_function(wrap_pyfunction!(crate::lk_info, m)?)?;
 
+    m.add_function(wrap_pyfunction!(crate::lk_list_watches, m)?)?;
+    m.add_function(wrap_pyfunction!(crate::lk_info, m)?)?;
+
     m.add_function(wrap_pyfunction!(crate::lk_key, m)?)?;
     m.add_function(wrap_pyfunction!(crate::lk_pull, m)?)?;
     m.add_function(wrap_pyfunction!(crate::lk_status_poll, m)?)?;
     m.add_function(wrap_pyfunction!(crate::lk_status_set, m)?)?;
 
+    m.add_function(wrap_pyfunction!(crate::b64, m)?)?;
+    m.add_function(wrap_pyfunction!(crate::spath, m)?)?;
+    m.add_function(wrap_pyfunction!(crate::blake3_hash, m)?)?;
+    m.add_function(wrap_pyfunction!(crate::bytes2uniform, m)?)?;
+
+    m.add_function(wrap_pyfunction!(crate::group, m)?)?;
+    m.add_function(wrap_pyfunction!(crate::set_group, m)?)?;
+    m.add_function(wrap_pyfunction!(crate::domain, m)?)?;
+    m.add_function(wrap_pyfunction!(crate::set_domain, m)?)?;
+
     m.add("PRIVATE", PyBytes::new(py, &consts::PRIVATE.0))?;
+    m.add("TEST_GROUP", PyBytes::new(py, &**consts::TEST_GROUP))?;
     m.add("PUBLIC", PyBytes::new(py, &consts::PUBLIC.0))?;
     m.add("DEFAULT_PKT", abe::DEFAULT_PKT)?;
 
     Ok(())
 }
 
 #[pyfunction]
@@ -597,8 +627,34 @@
     let path = components
         .iter()?
         .map(|i| i.and_then(PyAny::extract::<&[u8]>))
         .try_collect::<Vec<_>>()?;
     let sp = linkspace_rs::prelude::spath_buf(&path);
     Ok(PyBytes::new(py, &sp.spath_bytes()))
 }
+#[pyfunction]
+pub fn blake3_hash<'p>(py: Python<'p>,bytes:&PyAny) -> anyhow::Result<&'p PyBytes>{
+    Ok(PyBytes::new(py,&*linkspace_rs::misc::blake3_hash(bytelike(bytes)?)))
+}
+#[pyfunction]
+pub fn bytes2uniform<'p>(bytes:&[u8]) -> anyhow::Result<f64> {
+    let b : &[u8;8] = bytes[..8].try_into()?;
+    Ok(linkspace_rs::misc::bytes2uniform(b))
+}
+
+#[pyfunction]
+pub fn set_group(group:&[u8]){
+    linkspace_rs::prelude::set_group(GroupID::try_fit_bytes_or_b64(group).unwrap())
+}
+#[pyfunction]
+pub fn group<'p>(py:Python<'p>) -> &'p PyBytes{
+    PyBytes::new(py,&linkspace_rs::prelude::group().0)
+}
+#[pyfunction]
+pub fn set_domain(domain:&[u8]){
+    linkspace_rs::prelude::set_domain(Domain::try_fit_byte_slice(domain).unwrap())
+}
+#[pyfunction]
+pub fn domain<'p>(py:Python<'p>) -> &'p PyBytes{
+    PyBytes::new(py,&linkspace_rs::prelude::domain().0)
+}
```

### Comparing `linkspace-0.1.4/src/pynetpkt.rs` & `linkspace-0.3.0rc2/src/pynetpkt.rs`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,33 @@
 // Copyright Anton Sol
 //
 // This Source Code Form is subject to the terms of the Mozilla Public
 // License, v. 2.0. If a copy of the MPL was not distributed with this
 // file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
-use std::str::FromStr;
+use std::{str::FromStr, hash::{Hash, Hasher}};
 
 use ::linkspace::misc::FieldEnum;
 use ::linkspace::prelude::*;
 use pyo3::{basic::CompareOp, prelude::*, types::PyBytes};
+use std::collections::hash_map::DefaultHasher;
 
 use misc::{RecvPkt, ReroutePkt};
 
 use crate::bytelike;
 #[pyclass(mapping)]
 #[derive(Clone)]
 pub struct Pkt(pub(crate) ReroutePkt<RecvPkt<NetPktArc>>);
 impl Pkt {
+    pub fn from_arc(p: NetPktArc) -> Self {
+        Pkt(ReroutePkt::new(RecvPkt {
+            recv: p.recv().unwrap_or_else(now),
+            pkt: p
+        }))
+    }
     pub fn from_dyn(p: &dyn NetPkt) -> Self {
         Pkt(ReroutePkt::new(RecvPkt {
             recv: p.recv().unwrap_or_else(now),
             pkt: p.as_netarc(),
         }))
     }
 }
@@ -84,33 +91,33 @@
         self.0.create_stamp().map(|b| PyBytes::new(py, &b.0))
     }
     #[getter]
     pub fn group<'p>(&self, py: Python<'p>) -> Option<&'p PyBytes> {
         self.0.group().map(|g| PyBytes::new(py, &g.0))
     }
     #[getter]
-    pub fn spath<'p>(&self, py: Python<'p>) -> Option<&'p PyBytes> {
-        self.0.spath().map(|p| PyBytes::new(py, p.spath_bytes()))
+    pub fn path<'p>(&self, py: Python<'p>) -> Option<&'p PyBytes> {
+        self.0.path().map(|p| PyBytes::new(py, p.spath_bytes()))
     }
     #[getter]
     pub fn ipath<'p>(&self, py: Python<'p>) -> Option<&'p PyBytes> {
         self.0.ipath().map(|p| PyBytes::new(py, p.ipath_bytes()))
     }
     #[getter]
     pub fn recv<'p>(&self, py: Python<'p>) -> Option<&'p PyBytes> {
         self.0.recv().map(|p| PyBytes::new(py, &p.0))
     }
-    #[getter] pub fn comp0<'p>(&self, py: Python<'p>) -> &'p PyBytes {PyBytes::new(py,self.0.get_ipath().comp0())}
-    #[getter] pub fn comp1<'p>(&self, py: Python<'p>) -> &'p PyBytes {PyBytes::new(py,self.0.get_ipath().comp1())}
-    #[getter] pub fn comp2<'p>(&self, py: Python<'p>) -> &'p PyBytes {PyBytes::new(py,self.0.get_ipath().comp2())}
-    #[getter] pub fn comp3<'p>(&self, py: Python<'p>) -> &'p PyBytes {PyBytes::new(py,self.0.get_ipath().comp3())}
-    #[getter] pub fn comp4<'p>(&self, py: Python<'p>) -> &'p PyBytes {PyBytes::new(py,self.0.get_ipath().comp4())}
-    #[getter] pub fn comp5<'p>(&self, py: Python<'p>) -> &'p PyBytes {PyBytes::new(py,self.0.get_ipath().comp5())}
-    #[getter] pub fn comp6<'p>(&self, py: Python<'p>) -> &'p PyBytes {PyBytes::new(py,self.0.get_ipath().comp6())}
-    #[getter] pub fn comp7<'p>(&self, py: Python<'p>) -> &'p PyBytes {PyBytes::new(py,self.0.get_ipath().comp7())}
+    #[getter] pub fn path0<'p>(&self, py: Python<'p>) -> &'p PyBytes {PyBytes::new(py,self.0.get_ipath().path0())}
+    #[getter] pub fn path1<'p>(&self, py: Python<'p>) -> &'p PyBytes {PyBytes::new(py,self.0.get_ipath().path1())}
+    #[getter] pub fn path2<'p>(&self, py: Python<'p>) -> &'p PyBytes {PyBytes::new(py,self.0.get_ipath().path2())}
+    #[getter] pub fn path3<'p>(&self, py: Python<'p>) -> &'p PyBytes {PyBytes::new(py,self.0.get_ipath().path3())}
+    #[getter] pub fn path4<'p>(&self, py: Python<'p>) -> &'p PyBytes {PyBytes::new(py,self.0.get_ipath().path4())}
+    #[getter] pub fn path5<'p>(&self, py: Python<'p>) -> &'p PyBytes {PyBytes::new(py,self.0.get_ipath().path5())}
+    #[getter] pub fn path6<'p>(&self, py: Python<'p>) -> &'p PyBytes {PyBytes::new(py,self.0.get_ipath().path6())}
+    #[getter] pub fn path7<'p>(&self, py: Python<'p>) -> &'p PyBytes {PyBytes::new(py,self.0.get_ipath().path7())}
     pub fn path_list<'p>(&self, py: Python<'p>) -> Option<Vec<&'p PyBytes>> {
         self.0.ipath().map(|p| {
             p.comps_bytes()[0..*p.path_len() as usize]
                 .into_iter()
                 .map(|s| PyBytes::new(py, s))
                 .collect()
         })
@@ -132,22 +139,17 @@
     /// public key
     fn pubkey<'p>(&self, py: Python<'p>) -> Option<&'p PyBytes> {
         self.0.pubkey().map(|b| PyBytes::new(py, &b.0))
     }
     #[getter]
     /// signature
     fn signature<'p>(&self, py: Python<'p>) -> Option<&'p PyBytes> {
-        self.0.signature().map(|b| PyBytes::new(py, &b.0))
-    }
-
-    #[getter]
-    /// point size
-    fn point_size<'p>(&self, py: Python<'p>) -> &'p PyBytes {
-        PyBytes::new(py, &self.0.point_header_ref().point_size.0)
+        self.0.signed().map(|b| PyBytes::new(py, &b.signature.0))
     }
+    
     #[getter]
     /// number of components in the path
     fn path_len<'p>(&self) -> Option<u8> {
         self.0.path_len().map(|b| *b)
     }
     #[setter]
     pub fn set_netflags(&mut self, f: u8) {
@@ -155,16 +157,16 @@
             unsafe { linkspace::prelude::NetFlags::from_bits_unchecked(f) };
     }
     #[setter]
     pub fn set_hop(&mut self, b: [u8; 4]) {
         self.0.net_header.hop.0 = b
     }
     #[setter]
-    pub fn set_until(&mut self, until: [u8; 8]) {
-        self.0.net_header.stamp.0 = until;
+    pub fn set_stamp(&mut self, stamp: [u8; 8]) {
+        self.0.net_header.stamp.0 = stamp;
     }
     #[setter]
     pub fn set_ubits0(&mut self, b: [u8; 4]) {
         self.0.net_header.ubits[0].0 = b;
     }
     #[setter]
     pub fn set_ubits1(&mut self, b: [u8; 4]) {
@@ -207,49 +209,60 @@
     }
     #[getter]
     pub fn ubits3(&self) -> [u8; 4] {
         self.0.net_header.ubits[3].0
     }
 
     #[getter]
-    pub fn links(slf: PyRef<Self>) -> Option<Links> {
-        let _ = slf.0.links()?;
+    pub fn links(&self) -> Option<Links> {
+        let _ = self.0.links()?;
         Some(Links {
-            pkt: slf.into(),
+            pkt: self.0.pkt.pkt.clone(),
             idx: 0,
         })
     }
+
+    #[getter]
+    fn size(&self) -> u16{
+        self.0.size()
+    }
 }
 
 #[pyclass]
-#[pyo3(get_all)]
 pub struct Links {
-    pub pkt: Py<Pkt>,
-    pub idx: usize,
+    pkt: NetPktArc,
+    idx: usize,
 }
 
 #[pymethods]
 impl Links {
     fn __iter__(slf: PyRef<'_, Self>) -> PyRef<'_, Self> {
         slf
     }
+    fn __len__(&self) -> usize{ self.pkt.get_links().len()}
+    fn __getitem__(&self,idx:isize) -> Option<Link>{
+        let idx = if idx < 0 { self.__len__().wrapping_add_signed(idx)} else {idx as usize};
+        self.pkt.get_links().get(idx).copied().map(Into::into)
+    }
 
-    fn __next__(mut slf: PyRefMut<'_, Self>, py: Python<'_>) -> Option<Link> {
-        let this = slf.pkt.borrow(py).0.get_links().get(slf.idx).copied();
-        slf.idx += 1;
+    fn __next__(&mut self) -> Option<Link> {
+        let this = self.pkt.get_links().get(self.idx).copied();
+        self.idx += 1;
         this.map(Into::into)
     }
-    fn __traverse__(&self, visit: pyo3::PyVisit<'_>) -> Result<(), pyo3::PyTraverseError> {
-        visit.call(&self.pkt)
+    fn __hash__(&self) -> u64{
+        let mut hasher = DefaultHasher::new();
+        self.pkt.get_links().hash(&mut hasher);
+        hasher.finish()
     }
 }
 
 /// Link for a linkpoint
 #[pyclass]
-#[derive(Clone,Copy)]
+#[derive(Clone,Copy,Eq,PartialEq,Ord,PartialOrd,Hash)]
 #[repr(C)]
 pub struct Link {
     pub tag: [u8; 16],
     pub ptr: [u8; 32],
 }
 #[pymethods]
 impl Link {
@@ -271,14 +284,22 @@
         })
     }
     pub fn __repr__(&self, py: Python<'_>) -> String {
         let tag = PyBytes::new(py, &self.tag).repr().unwrap();
         let ptr = PyBytes::new(py, &self.ptr).repr().unwrap();
         format!("Link({tag},{ptr})")
     }
+    pub fn __hash__(&self) -> u64{
+        let mut hasher = DefaultHasher::new();
+        self.hash(&mut hasher);
+        hasher.finish()
+    }
+    fn __richcmp__(&self, other: &Self, op: CompareOp) -> bool {
+        op.matches(self.cmp(&other))
+    }
 }
 
 impl Into<linkspace::prelude::Link> for Link {
     fn into(self) -> linkspace::prelude::Link {
         prelude::Link {
             tag: self.tag.into(),
             ptr: self.ptr.into(),
```

### Comparing `linkspace-0.1.4/tests/nested_watch.py` & `linkspace-0.3.0rc2/tests/nested_watch.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 from datetime import datetime
 
 lk = lk_open("./private",create=True)
 lk_process(lk)
 
 q = lk_query()
 lk_query_parse(q,"""
-:id:test
+:qid:test
 :mode:log-asc
-i_index:<:[u32:0]
+i_db:<:[u32:0]
 """)
 
 outer_l = []
 inner_l = []
 
 def inner(pkt):
     print("inner triggered",pkt)
@@ -20,14 +20,14 @@
 
 def outer(pkt):
     print("outer triggered",pkt)
     outer_l.append(pkt)
     lk_watch(lk,q,inner)
 
 lk_watch(lk,q,outer)
-lk_process_while(lk,until=lk_eval("[now:+1s]"))
+lk_process_while(lk,timeout=lk_eval("[now:+1s]"))
 
 lk_save(lk,lk_datapoint("one"+str(datetime.now())))
 lk_save(lk,lk_datapoint("two"+str(datetime.now())))
-lk_process_while(lk,until=lk_eval("[now:+1s]"))
+lk_process_while(lk,timeout=lk_eval("[now:+1s]"))
 
 print(outer_l,inner_l)
```

### Comparing `linkspace-0.1.4/Cargo.lock` & `linkspace-0.3.0rc2/Cargo.lock`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 # This file is automatically @generated by Cargo.
 # It is not intended for manual editing.
 version = 3
 
 [[package]]
 name = "abe"
-version = "0.1.0"
+version = "0.3.0-rc1"
 dependencies = [
  "anyhow",
- "arrayvec 0.7.2",
+ "arrayvec",
+ "base64 0.21.2",
+ "bstr",
  "hex",
  "serde",
  "thiserror",
 ]
 
 [[package]]
 name = "addr2line"
@@ -25,84 +27,120 @@
 [[package]]
 name = "adler"
 version = "1.0.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f26201604c87b1e01bd3d98f8d5d9a8fcbb815e8cedb41ffccbeb4bf593a35fe"
 
 [[package]]
-name = "adoto"
-version = "0.1.0"
+name = "aho-corasick"
+version = "1.0.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "43f6cb1bf222025340178f382c426f13757b2960e89779dfcb319c32542a5a41"
 dependencies = [
- "anyhow",
- "pretty",
- "serde",
- "serde_json",
+ "memchr",
 ]
 
 [[package]]
-name = "aho-corasick"
-version = "0.7.20"
+name = "android-tzdata"
+version = "0.1.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e999941b234f3131b00bc13c22d06e8c5ff726d1b6318ac7eb276997bbb4fef0"
+
+[[package]]
+name = "android_system_properties"
+version = "0.1.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cc936419f96fa211c1b9166887b38e5e40b19958e5b895be7c1f93adec7071ac"
+checksum = "819e7219dbd41043ac279b19830f2efc897156490d7fd6ea916720117ee66311"
 dependencies = [
- "memchr",
+ "libc",
 ]
 
 [[package]]
-name = "anyhow"
-version = "1.0.70"
+name = "anstream"
+version = "0.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7de8ce5e0f9f8d88245311066a578d72b7af3e7088f32783804676302df237e4"
+checksum = "0ca84f3628370c59db74ee214b3263d58f9aadd9b4fe7e711fd87dc452b7f163"
+dependencies = [
+ "anstyle",
+ "anstyle-parse",
+ "anstyle-query",
+ "anstyle-wincon",
+ "colorchoice",
+ "is-terminal",
+ "utf8parse",
+]
 
 [[package]]
-name = "archery"
-version = "0.4.0"
+name = "anstyle"
+version = "1.0.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "3a30da5c5f2d5e72842e00bcb57657162cdabef0931f40e2deb9b4140440cecd"
+
+[[package]]
+name = "anstyle-parse"
+version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0a8da9bc4c4053ee067669762bcaeea6e241841295a2b6c948312dad6ef4cc02"
+checksum = "938874ff5980b03a87c5524b3ae5b59cf99b1d6bc836848df7bc5ada9643c333"
 dependencies = [
- "static_assertions",
+ "utf8parse",
 ]
 
 [[package]]
-name = "arrayref"
-version = "0.3.6"
+name = "anstyle-query"
+version = "1.0.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "5ca11d4be1bab0c8bc8734a9aa7bf4ee8316d462a08c6ac5052f888fef5b494b"
+dependencies = [
+ "windows-sys 0.48.0",
+]
+
+[[package]]
+name = "anstyle-wincon"
+version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a4c527152e37cf757a3f78aae5a06fbeefdb07ccc535c980a3208ee3060dd544"
+checksum = "180abfa45703aebe0093f79badacc01b8fd4ea2e35118747e5811127f926e188"
+dependencies = [
+ "anstyle",
+ "windows-sys 0.48.0",
+]
 
 [[package]]
-name = "arrayvec"
-version = "0.5.2"
+name = "anyhow"
+version = "1.0.71"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "9c7d0618f0e0b7e8ff11427422b64564d5fb0be1940354bfe2e0529b18a9d9b8"
+
+[[package]]
+name = "arrayref"
+version = "0.3.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "23b62fc65de8e4e7f52534fb52b0f3ed04746ae267519eef2a83941e8085068b"
+checksum = "6b4930d2cb77ce62f89ee5d5289b4ac049559b1c45539271f5ed4fdc7db34545"
 
 [[package]]
 name = "arrayvec"
 version = "0.7.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8da52d66c7071e2e3fa2a1e5c6d088fec47b593032b254f5e980de8ea54454d6"
-dependencies = [
- "serde",
-]
 
 [[package]]
 name = "async-channel"
 version = "1.8.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "cf46fee83e5ccffc220104713af3292ff9bc7c64c7de289f66dae8e38d826833"
 dependencies = [
  "concurrent-queue",
  "event-listener",
  "futures-core",
 ]
 
 [[package]]
 name = "async-executor"
-version = "1.5.0"
+version = "1.5.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "17adb73da160dfb475c183343c8cccd80721ea5a605d3eb57125f0a7b7a92d0b"
+checksum = "6fa3dc5f2a8564f07759c008b9109dc0d39de92a88d5588b8a5036d286383afb"
 dependencies = [
  "async-lock",
  "async-task",
  "concurrent-queue",
  "fastrand",
  "futures-lite",
  "slab",
@@ -120,27 +158,26 @@
  "blocking",
  "futures-lite",
  "once_cell",
 ]
 
 [[package]]
 name = "async-lock"
-version = "2.6.0"
+version = "2.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c8101efe8695a6c17e02911402145357e718ac92d3ff88ae8419e84b1707b685"
+checksum = "fa24f727524730b077666307f2734b4a1a1c57acb79193127dcc8914d5242dd7"
 dependencies = [
  "event-listener",
- "futures-lite",
 ]
 
 [[package]]
 name = "async-task"
-version = "4.3.0"
+version = "4.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7a40729d2133846d9ed0ea60a8b9541bccddab49cd30f0715a1da672fe9a2524"
+checksum = "ecc7ab41815b3c653ccd2978ec3255c81349336702dfdf62ee6f7069b12a3aae"
 
 [[package]]
 name = "async_executors"
 version = "0.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c0b2463773401e1f684136f9cdb956cf611f22172472cf3f049e72123f59e359"
 dependencies = [
@@ -154,28 +191,28 @@
  "pin-project",
  "rustc_version",
  "wasm-bindgen-futures",
 ]
 
 [[package]]
 name = "atomic-waker"
-version = "1.1.0"
+version = "1.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "debc29dde2e69f9e47506b525f639ed42300fc014a3e007832592448fa8e4599"
+checksum = "1181e1e0d1fce796a03db1ae795d67167da795f9cf4a39c37589e85ef57f26d3"
 
 [[package]]
 name = "auto_impl"
 version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8a8c1df849285fbacd587de7818cc7d13be6cd2cbcd47a04fb1801b0e2706e33"
 dependencies = [
  "proc-macro-error",
  "proc-macro2",
  "quote",
- "syn 1.0.107",
+ "syn 1.0.109",
 ]
 
 [[package]]
 name = "autocfg"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d468802bab17cbc0cc575e9b053f41e72aa36bfa6b7f55e3529ffa43161b97fa"
@@ -193,29 +230,35 @@
  "miniz_oxide",
  "object",
  "rustc-demangle",
 ]
 
 [[package]]
 name = "base16ct"
-version = "0.1.1"
+version = "0.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "349a06037c7bf932dd7e7d1f653678b2038b9ad46a74102f1fc7bd7872678cce"
+checksum = "4c7f02d4ea65f2c1853089ffd8d2787bdbc63de2f0d29dedbcf8ccdfa0ccd4cf"
 
 [[package]]
 name = "base64"
 version = "0.13.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9e1b586273c5702936fe7b7d6896644d8be71e6314cfe09d3167c95f712589e8"
 
 [[package]]
+name = "base64"
+version = "0.21.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "604178f6c5c21f02dc555784810edfb88d34ac2c73b2eae109655649ee73ce3d"
+
+[[package]]
 name = "base64ct"
-version = "1.5.3"
+version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b645a089122eccb6111b4f81cbc1a49f5900ac4666bb93ac027feaecf15607bf"
+checksum = "8c3c1a368f70d6cf7302d78f8f7093da241fb8e8807c05cc9e51a125895a6d5b"
 
 [[package]]
 name = "bincode"
 version = "1.3.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b1f45e9417d87227c7a56d22e471c6206462cba514c7590c09aff4cf6d1ddcad"
 dependencies = [
@@ -225,245 +268,378 @@
 [[package]]
 name = "bitflags"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
 
 [[package]]
-name = "bitflags"
-version = "2.0.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "487f1e0fcbe47deb8b0574e646def1c903389d95241dd1bbcc6ce4a715dfc0c1"
-
-[[package]]
-name = "bitvec"
-version = "1.0.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1bc2832c24239b0141d5674bb9174f9d68a8b5b3f2753311927c172ca46f7e9c"
-dependencies = [
- "funty",
- "radium",
- "tap",
- "wyz",
-]
-
-[[package]]
 name = "blake2b_simd"
 version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3c2f0dc9a68c6317d884f97cc36cf5a3d20ba14ce404227df55e1af708ab04bc"
 dependencies = [
  "arrayref",
- "arrayvec 0.7.2",
- "constant_time_eq 0.2.4",
+ "arrayvec",
+ "constant_time_eq 0.2.6",
 ]
 
 [[package]]
 name = "blake3"
-version = "1.3.3"
+version = "1.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "42ae2468a89544a466886840aa467a25b766499f4f04bf7d9fcd10ecee9fccef"
+checksum = "a08e53fc5a564bb15bfe6fae56bd71522205f1f91893f9c0116edad6496c183f"
 dependencies = [
  "arrayref",
- "arrayvec 0.7.2",
+ "arrayvec",
  "cc",
  "cfg-if",
- "constant_time_eq 0.2.4",
+ "constant_time_eq 0.1.5",
  "digest",
 ]
 
 [[package]]
 name = "blanket"
 version = "0.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7b04ce3d2372d05d1ef4ea3fdf427da6ae3c17ca06d688a107b5344836276bc3"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 1.0.107",
+ "syn 1.0.109",
 ]
 
 [[package]]
 name = "block-buffer"
-version = "0.10.3"
+version = "0.10.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "69cce20737498f97b993470a6e536b8523f0af7892a4f928cceb1ac5e52ebe7e"
+checksum = "3078c7629b62d3f0439517fa394996acacc5cbc91c5a20d8c658e77abd503a71"
 dependencies = [
  "generic-array",
 ]
 
 [[package]]
 name = "blocking"
-version = "1.3.0"
+version = "1.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3c67b173a56acffd6d2326fb7ab938ba0b00a71480e14902b2591c87bc5741e8"
+checksum = "77231a1c8f801696fc0123ec6150ce92cffb8e164a02afb9c8ddee0e9b65ad65"
 dependencies = [
  "async-channel",
  "async-lock",
  "async-task",
  "atomic-waker",
  "fastrand",
  "futures-lite",
+ "log",
 ]
 
 [[package]]
-name = "bloomhash"
-version = "0.1.0"
+name = "bstr"
+version = "1.5.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "a246e68bb43f6cd9db24bea052a53e40405417c5fb372e3d1a8a7f770a564ef5"
+dependencies = [
+ "memchr",
+]
+
+[[package]]
+name = "build-info"
+version = "0.0.31"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "8b301350c1c448e35b896f32b68c49c8ecd969a71978fbafc4ebd09ec3f4eee2"
+dependencies = [
+ "build-info-common",
+ "build-info-proc",
+ "once_cell",
+]
+
+[[package]]
+name = "build-info-build"
+version = "0.0.31"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "2b314717755dd6a06fc11ad3f7909ba4c0ae2ab516f5cb0404fe924c71bfc7d0"
 dependencies = [
  "anyhow",
- "bitvec",
- "linkspace-pkt",
+ "base64 0.21.2",
+ "bincode",
+ "build-info-common",
+ "cargo_metadata",
+ "chrono",
+ "git2",
+ "glob",
+ "once_cell",
+ "pretty_assertions",
+ "rustc_version",
+ "serde_json",
+ "xz2",
+]
+
+[[package]]
+name = "build-info-common"
+version = "0.0.31"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "5e040d36472d40ec9424c36a7b54be589072e605596b6f20b0c56c5230b460cc"
+dependencies = [
+ "chrono",
+ "derive_more",
+ "semver",
+ "serde",
+]
+
+[[package]]
+name = "build-info-proc"
+version = "0.0.31"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ffd5f241ddd417436c48d35da9869480891449ddd1ae3fd483bbcfbae741a422"
+dependencies = [
+ "anyhow",
+ "base64 0.21.2",
+ "bincode",
+ "build-info-common",
+ "chrono",
+ "num-bigint",
+ "num-traits",
+ "proc-macro-error",
+ "proc-macro2",
+ "quote",
+ "serde_json",
+ "syn 2.0.18",
+ "xz2",
 ]
 
 [[package]]
 name = "bumpalo"
-version = "3.12.0"
+version = "3.13.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0d261e256854913907f67ed06efbc3338dfe6179796deefc1ff763fc1aee5535"
+checksum = "a3e2c3daef883ecc1b5d58c15adae93470a91d425f3532ba1695849656af3fc1"
 
 [[package]]
 name = "byte-fmt"
-version = "0.1.0"
+version = "0.3.0-rc1"
 dependencies = [
  "abe",
- "base64",
+ "base64 0.21.2",
+ "bytemuck",
  "ruint",
  "serde",
  "serde_bytes",
- "serde_json",
  "tracing",
 ]
 
 [[package]]
+name = "bytemuck"
+version = "1.13.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "17febce684fd15d89027105661fec94afb475cb995fbc59d2865198446ba2eea"
+dependencies = [
+ "bytemuck_derive",
+]
+
+[[package]]
+name = "bytemuck_derive"
+version = "1.4.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "fdde5c9cd29ebd706ce1b35600920a33550e402fc998a2e53ad3b42c3c47a192"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "syn 2.0.18",
+]
+
+[[package]]
 name = "byteorder"
 version = "1.4.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "14c189c53d098945499cdfa7ecc63567cf3886b3332b312a5b4585d8d3a6a610"
 
 [[package]]
 name = "bytes"
-version = "1.4.0"
+version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "89b2fd2a0dcf38d7971e2194b6b6eebab45ae01067456a7fd93d5547a61b70be"
+checksum = "c4872d67bab6358e59559027aa3b9157c53d9358c51423c17554809a8858e0f8"
+
+[[package]]
+name = "camino"
+version = "1.1.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "c530edf18f37068ac2d977409ed5cd50d53d73bc653c7647b48eb78976ac9ae2"
+dependencies = [
+ "serde",
+]
+
+[[package]]
+name = "cargo-platform"
+version = "0.1.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "cbdb825da8a5df079a43676dbe042702f1707b1109f713a01420fbb4cc71fa27"
+dependencies = [
+ "serde",
+]
+
+[[package]]
+name = "cargo_metadata"
+version = "0.15.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "eee4243f1f26fc7a42710e7439c149e2b10b05472f88090acce52632f231a73a"
+dependencies = [
+ "camino",
+ "cargo-platform",
+ "semver",
+ "serde",
+ "serde_json",
+ "thiserror",
+]
 
 [[package]]
 name = "cc"
 version = "1.0.79"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "50d30906286121d95be3d479533b458f87493b30a4b5f79a607db8f5d11aa91f"
+dependencies = [
+ "jobserver",
+]
 
 [[package]]
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
+name = "chrono"
+version = "0.4.26"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ec837a71355b28f6556dbd569b37b3f363091c0bd4b2e735674521b4c5fd9bc5"
+dependencies = [
+ "android-tzdata",
+ "iana-time-zone",
+ "num-traits",
+ "serde",
+ "winapi",
+]
+
+[[package]]
 name = "clap"
-version = "4.1.11"
+version = "4.3.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "42dfd32784433290c51d92c438bb72ea5063797fc3cc9a21a8c4346bebbb2098"
+checksum = "80672091db20273a15cf9fdd4e47ed43b5091ec9841bf4c6145c9dfbbcae09ed"
 dependencies = [
- "bitflags 2.0.2",
+ "clap_builder",
  "clap_derive",
- "clap_lex",
- "is-terminal",
  "once_cell",
+]
+
+[[package]]
+name = "clap_builder"
+version = "4.3.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "c1458a1df40e1e2afebb7ab60ce55c1fa8f431146205aa5f4887e0b111c27636"
+dependencies = [
+ "anstream",
+ "anstyle",
+ "bitflags",
+ "clap_lex",
  "strsim",
- "termcolor",
 ]
 
 [[package]]
 name = "clap_derive"
-version = "4.1.9"
+version = "4.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fddf67631444a3a3e3e5ac51c36a5e01335302de677bd78759eaa90ab1f46644"
+checksum = "b8cd2b2a819ad6eec39e8f1d6b53001af1e5469f8c177579cdaeb313115b825f"
 dependencies = [
  "heck",
- "proc-macro-error",
  "proc-macro2",
  "quote",
- "syn 1.0.107",
+ "syn 2.0.18",
 ]
 
 [[package]]
 name = "clap_lex"
-version = "0.3.1"
+version = "0.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "783fe232adfca04f90f56201b26d79682d4cd2625e0bc7290b95123afe558ade"
-dependencies = [
- "os_str_bytes",
-]
+checksum = "2da6da31387c7e4ef160ffab6d5e7f00c42626fe39aea70a7b0f1773f7dd6c1b"
+
+[[package]]
+name = "colorchoice"
+version = "1.0.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "acbf1af155f9b9ef647e42cdc158db4b64a1b61f743629225fde6f3e0be2a7c7"
 
 [[package]]
 name = "concurrent-queue"
-version = "2.1.0"
+version = "2.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c278839b831783b70278b14df4d45e1beb1aad306c07bb796637de9a0e323e8e"
+checksum = "62ec6771ecfa0762d24683ee5a32ad78487a3d3afdc0fb8cae19d2c5deb50b7c"
 dependencies = [
  "crossbeam-utils",
 ]
 
 [[package]]
 name = "const-oid"
-version = "0.9.1"
+version = "0.9.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cec318a675afcb6a1ea1d4340e2d377e56e47c266f28043ceccbf4412ddfdd3b"
+checksum = "520fbf3c07483f94e3e3ca9d0cfd913d7718ef2483d2cfd91c0d9e91474ab913"
 
 [[package]]
 name = "constant_time_eq"
 version = "0.1.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "245097e9a4535ee1e3e3931fcfcd55a796a44c643e8596ff6566d68f09b87bbc"
 
 [[package]]
 name = "constant_time_eq"
-version = "0.2.4"
+version = "0.2.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f3ad85c1f65dc7b37604eb0e89748faf0b9653065f2a8ef69f96a687ec1e9279"
+checksum = "21a53c0a4d288377e7415b53dcfc3c04da5cdc2cc95c8d5ac178b58f0b861ad6"
 
 [[package]]
 name = "convert_case"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6245d59a3e82a7fc217c5828a6692dbc6dfb63a0c8c90495621f7b9d79704a0e"
 
 [[package]]
+name = "core-foundation-sys"
+version = "0.8.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e496a50fda8aacccc86d7529e2c1e0892dbd0f898a6b5645b5561b89c3210efa"
+
+[[package]]
 name = "cpufeatures"
-version = "0.2.5"
+version = "0.2.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "28d997bd5e24a5928dd43e46dc529867e207907fe0b239c3477d924f7f2ca320"
+checksum = "03e69e28e9f7f77debdedbaafa2866e1de9ba56df55a8bd7cfc724c25a09987c"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "crossbeam-channel"
-version = "0.5.6"
+version = "0.5.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c2dd04ddaf88237dc3b8d8f9a3c1004b506b54b3313403944054d23c0870c521"
+checksum = "a33c2bf77f2df06183c3aa30d1e96c0695a313d4f9c453cc3762a6db39f99200"
 dependencies = [
  "cfg-if",
  "crossbeam-utils",
 ]
 
 [[package]]
 name = "crossbeam-utils"
-version = "0.8.14"
+version = "0.8.16"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4fb766fa798726286dbbb842f174001dab8abc7b627a1dd86e0b7222a95d929f"
+checksum = "5a22b2d63d4d1dc0b7f1b6b2747dd0088008a9be28b6ddf0b1e7d335e3037294"
 dependencies = [
  "cfg-if",
 ]
 
 [[package]]
 name = "crypto-bigint"
-version = "0.4.9"
+version = "0.5.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ef2b4b23cddf68b89b8f8069890e8c270d54e2d5fe1b143820234805e4cb17ef"
+checksum = "cf4c2f4e1afd912bc40bfd6fed5d9dc1f288e0ba01bfcc835cc5bc3eb13efe15"
 dependencies = [
  "generic-array",
  "rand_core",
  "subtle",
  "zeroize",
 ]
 
@@ -474,18 +650,28 @@
 checksum = "1bfb12502f3fc46cca1bb51ac28df9d618d813cdc3d2f25b9fe775a34af26bb3"
 dependencies = [
  "generic-array",
  "typenum",
 ]
 
 [[package]]
+name = "ctor"
+version = "0.1.26"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "6d2301688392eb071b0bf1a37be05c469d3cc4dbbd95df672fe28ab021e6a096"
+dependencies = [
+ "quote",
+ "syn 1.0.109",
+]
+
+[[package]]
 name = "der"
-version = "0.6.1"
+version = "0.7.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f1a467a65c5e759bce6e65eaf91cc29f466cdc57cb65777bd646872a8a1fd4de"
+checksum = "56acb310e15652100da43d130af8d97b509e95af61aab1c5a7939ef24337ee17"
 dependencies = [
  "const-oid",
  "zeroize",
 ]
 
 [[package]]
 name = "derive_more"
@@ -493,84 +679,89 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4fb810d30a7c1953f91334de7244731fc3f3c10d7fe163338a35b9f640960321"
 dependencies = [
  "convert_case",
  "proc-macro2",
  "quote",
  "rustc_version",
- "syn 1.0.107",
+ "syn 1.0.109",
 ]
 
 [[package]]
+name = "diff"
+version = "0.1.13"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "56254986775e3233ffa9c4d7d3faaf6d36a2c09d30b20687e9f88bc8bafc16c8"
+
+[[package]]
 name = "digest"
-version = "0.10.6"
+version = "0.10.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8168378f4e5023e7218c89c891c0fd8ecdb5e5e4f18cb78f38cf245dd021e76f"
+checksum = "9ed9a281f7bc9b7576e61468ba615a66a5c8cfdff42420a70aa82701a3b1e292"
 dependencies = [
  "block-buffer",
+ "const-oid",
  "crypto-common",
  "subtle",
 ]
 
 [[package]]
 name = "dunce"
-version = "1.0.3"
+version = "1.0.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0bd4b30a6560bbd9b4620f4de34c3f14f60848e58a9b7216801afcb4c7b31c3c"
+checksum = "56ce8c6da7551ec6c462cbaf3bfbc75131ebbfa1c944aeaa9dab51ca1c5f0c3b"
 
 [[package]]
 name = "ecdsa"
-version = "0.14.8"
+version = "0.16.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "413301934810f597c1d19ca71c8710e99a3f1ba28a0d2ebc01551a2daeea3c5c"
+checksum = "0997c976637b606099b9985693efa3581e84e41f5c11ba5255f88711058ad428"
 dependencies = [
  "der",
+ "digest",
  "elliptic-curve",
  "rfc6979",
  "signature",
+ "spki",
 ]
 
 [[package]]
 name = "either"
 version = "1.8.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7fcaabb2fef8c910e7f4c7ce9f67a1283a1715879a7c230ca9d6d1ae31f16d91"
-dependencies = [
- "serde",
-]
 
 [[package]]
 name = "elliptic-curve"
-version = "0.12.3"
+version = "0.13.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e7bb888ab5300a19b8e5bceef25ac745ad065f3c9f7efc6de1b91958110891d3"
+checksum = "968405c8fdc9b3bf4df0a6638858cc0b52462836ab6b1c87377785dd09cf1c0b"
 dependencies = [
  "base16ct",
  "crypto-bigint",
- "der",
  "digest",
  "ff",
  "generic-array",
  "group",
  "pkcs8",
  "rand_core",
  "sec1",
  "subtle",
  "zeroize",
 ]
 
 [[package]]
 name = "errno"
-version = "0.2.8"
+version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f639046355ee4f37944e44f60642c6f3a7efa3cf6b78c78a0d989a8ce6c396a1"
+checksum = "4bcfec3a70f97c962c307b2d2c56e358cf1d00b558d74262b5f929ee8cc7e73a"
 dependencies = [
  "errno-dragonfly",
  "libc",
- "winapi",
+ "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "errno-dragonfly"
 version = "0.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "aa68f1b12764fab894d2755d2518754e71b4fd80ecfb822714a1206c2aab39bf"
@@ -583,41 +774,50 @@
 name = "event-listener"
 version = "2.5.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0206175f82b8d6bf6652ff7d71a1e27fd2e4efde587fd368662814d6ec1d9ce0"
 
 [[package]]
 name = "fastrand"
-version = "1.8.0"
+version = "1.9.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a7a407cfaa3385c4ae6b23e84623d48c2798d06e3e6a1878f7f59f17b3f86499"
+checksum = "e51093e27b0797c359783294ca4f0a911c270184cb10f85783b118614a1501be"
 dependencies = [
  "instant",
 ]
 
 [[package]]
 name = "ff"
-version = "0.12.1"
+version = "0.13.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d013fc25338cc558c5c2cfbad646908fb23591e2404481826742b651c9af7160"
+checksum = "ded41244b729663b1e574f1b4fb731469f69f79c17667b5d776b16cda0479449"
 dependencies = [
  "rand_core",
  "subtle",
 ]
 
 [[package]]
 name = "filetime"
-version = "0.2.19"
+version = "0.2.21"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4e884668cd0c7480504233e951174ddc3b382f7c2666e3b7310b5c4e7b0c37f9"
+checksum = "5cbc844cecaee9d4443931972e1289c8ff485cb4cc2767cb03ca139ed6885153"
 dependencies = [
  "cfg-if",
  "libc",
- "redox_syscall",
- "windows-sys 0.42.0",
+ "redox_syscall 0.2.16",
+ "windows-sys 0.48.0",
+]
+
+[[package]]
+name = "form_urlencoded"
+version = "1.2.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "a62bc1cf6f830c2ec14a513a9fb124d0a213a629668a4186f329db21fe045652"
+dependencies = [
+ "percent-encoding",
 ]
 
 [[package]]
 name = "fsevent-sys"
 version = "4.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "76ee7a02da4d231650c7cea31349b889be2f45ddb3ef3032d2ec8185f6313fd2"
@@ -632,120 +832,114 @@
 checksum = "04412b8935272e3a9bae6f48c7bfff74c2911f60525404edfdd28e49884c3bfb"
 dependencies = [
  "libc",
  "winapi",
 ]
 
 [[package]]
-name = "funty"
-version = "2.0.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e6d5a32815ae3f33302d95fdcb2ce17862f8c65363dcfd29360480ba1001fc9c"
-
-[[package]]
 name = "futures"
-version = "0.3.26"
+version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "13e2792b0ff0340399d58445b88fd9770e3489eff258a4cbc1523418f12abf84"
+checksum = "23342abe12aba583913b2e62f22225ff9c950774065e4bfb61a19cd9770fec40"
 dependencies = [
  "futures-channel",
  "futures-core",
  "futures-executor",
  "futures-io",
  "futures-sink",
  "futures-task",
  "futures-util",
 ]
 
 [[package]]
 name = "futures-channel"
-version = "0.3.26"
+version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2e5317663a9089767a1ec00a487df42e0ca174b61b4483213ac24448e4664df5"
+checksum = "955518d47e09b25bbebc7a18df10b81f0c766eaf4c4f1cccef2fca5f2a4fb5f2"
 dependencies = [
  "futures-core",
  "futures-sink",
 ]
 
 [[package]]
 name = "futures-core"
-version = "0.3.26"
+version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ec90ff4d0fe1f57d600049061dc6bb68ed03c7d2fbd697274c41805dcb3f8608"
+checksum = "4bca583b7e26f571124fe5b7561d49cb2868d79116cfa0eefce955557c6fee8c"
 
 [[package]]
 name = "futures-executor"
-version = "0.3.26"
+version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e8de0a35a6ab97ec8869e32a2473f4b1324459e14c29275d14b10cb1fd19b50e"
+checksum = "ccecee823288125bd88b4d7f565c9e58e41858e47ab72e8ea2d64e93624386e0"
 dependencies = [
  "futures-core",
  "futures-task",
  "futures-util",
 ]
 
 [[package]]
 name = "futures-io"
-version = "0.3.26"
+version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bfb8371b6fb2aeb2d280374607aeabfc99d95c72edfe51692e42d3d7f0d08531"
+checksum = "4fff74096e71ed47f8e023204cfd0aa1289cd54ae5430a9523be060cdb849964"
 
 [[package]]
 name = "futures-lite"
-version = "1.12.0"
+version = "1.13.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7694489acd39452c77daa48516b894c153f192c3578d5a839b62c58099fcbf48"
+checksum = "49a9d51ce47660b1e808d3c990b4709f2f415d928835a17dfd16991515c46bce"
 dependencies = [
  "fastrand",
  "futures-core",
  "futures-io",
  "memchr",
  "parking",
  "pin-project-lite",
  "waker-fn",
 ]
 
 [[package]]
 name = "futures-macro"
-version = "0.3.26"
+version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "95a73af87da33b5acf53acfebdc339fe592ecf5357ac7c0a7734ab9d8c876a70"
+checksum = "89ca545a94061b6365f2c7355b4b32bd20df3ff95f02da9329b34ccc3bd6ee72"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 1.0.107",
+ "syn 2.0.18",
 ]
 
 [[package]]
 name = "futures-sink"
-version = "0.3.26"
+version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f310820bb3e8cfd46c80db4d7fb8353e15dfff853a127158425f31e0be6c8364"
+checksum = "f43be4fe21a13b9781a69afa4985b0f6ee0e1afab2c6f454a8cf30e2b2237b6e"
 
 [[package]]
 name = "futures-task"
-version = "0.3.26"
+version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dcf79a1bf610b10f42aea489289c5a2c478a786509693b80cd39c44ccd936366"
+checksum = "76d3d132be6c0e6aa1534069c705a74a5997a356c0dc2f86a47765e5617c5b65"
 
 [[package]]
 name = "futures-timer"
 version = "3.0.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e64b03909df88034c26dc1547e8970b91f98bdb65165d6a4e9110d94263dbb2c"
 dependencies = [
  "gloo-timers",
  "send_wrapper",
 ]
 
 [[package]]
 name = "futures-util"
-version = "0.3.26"
+version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9c1d6de3acfef38d2be4b1f543f553131788603495be83da675e180c8d6b7bd1"
+checksum = "26b01e40b772d54cf6c6d721c1d1abd0647a0106a12ecaa1c186273392a69533"
 dependencies = [
  "futures-channel",
  "futures-core",
  "futures-io",
  "futures-macro",
  "futures-sink",
  "futures-task",
@@ -753,40 +947,60 @@
  "pin-project-lite",
  "pin-utils",
  "slab",
 ]
 
 [[package]]
 name = "generic-array"
-version = "0.14.6"
+version = "0.14.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bff49e947297f3312447abdca79f45f4738097cc82b06e72054d2223f601f1b9"
+checksum = "85649ca51fd72272d7821adaf274ad91c288277713d9c18820d8499a7ff69e9a"
 dependencies = [
  "typenum",
  "version_check",
+ "zeroize",
 ]
 
 [[package]]
 name = "getrandom"
-version = "0.2.8"
+version = "0.2.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c05aeb6a22b8f62540c194aac980f2115af067bfe15a0734d7277a768d396b31"
+checksum = "c85e1d9ab2eadba7e5040d4e09cbd6d072b76a557ad64e797c2cb9d4da21d7e4"
 dependencies = [
  "cfg-if",
  "js-sys",
  "libc",
  "wasi",
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "gimli"
-version = "0.27.1"
+version = "0.27.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "221996f774192f0f718773def8201c4ae31f02616a54ccfc2d358bb0e5cefdec"
+checksum = "b6c80984affa11d98d1b88b66ac8853f143217b399d3c74116778ff8fdb4ed2e"
+
+[[package]]
+name = "git2"
+version = "0.17.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7b989d6a7ca95a362cf2cfc5ad688b3a467be1f87e480b8dad07fee8c79b0044"
+dependencies = [
+ "bitflags",
+ "libc",
+ "libgit2-sys",
+ "log",
+ "url",
+]
+
+[[package]]
+name = "glob"
+version = "0.3.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d2fabcfbdc87f4758337ca535fb41a6d701b65693ce38287d856d1674551ec9b"
 
 [[package]]
 name = "gloo-timers"
 version = "0.2.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9b995a66bb87bebce9a0f4a95aed01daca4872c050bfcb21653361c03bc35e5c"
 dependencies = [
@@ -794,34 +1008,34 @@
  "futures-core",
  "js-sys",
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "group"
-version = "0.12.1"
+version = "0.13.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5dfbfb3a6cfbd390d5c9564ab283a0349b9b9fcd46a706c1eb10e0db70bfbac7"
+checksum = "f0f9ef7462f7c099f518d754361858f86d8a07af53ba9af0fe635bbccb151a63"
 dependencies = [
  "ff",
  "rand_core",
  "subtle",
 ]
 
 [[package]]
 name = "heck"
 version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "95505c38b4572b2d910cecb0281560f54b440a19336cbbcb27bf6ce6adc6f5a8"
 
 [[package]]
 name = "hermit-abi"
-version = "0.3.0"
+version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "856b5cb0902c2b6d65d5fd97dfa30f9b70c7538e770b98eab5ed52d8db923e01"
+checksum = "fed44880c466736ef9a5c5b5facefb5ed0785676d0c02d612db14e54f0d84286"
 
 [[package]]
 name = "hex"
 version = "0.4.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7f24254aa9a54b5c858eaee2f5bccdb46aaf0e486a595ed5fd8f86ba55232a70"
 
@@ -831,26 +1045,59 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6c49c37c09c17a53d937dfbb742eb3a961d65a994e6bcdcf37e7399d0cc8ab5e"
 dependencies = [
  "digest",
 ]
 
 [[package]]
+name = "iana-time-zone"
+version = "0.1.57"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "2fad5b825842d2b38bd206f3e81d6957625fd7f0a361e345c30e01a0ae2dd613"
+dependencies = [
+ "android_system_properties",
+ "core-foundation-sys",
+ "iana-time-zone-haiku",
+ "js-sys",
+ "wasm-bindgen",
+ "windows",
+]
+
+[[package]]
+name = "iana-time-zone-haiku"
+version = "0.1.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f31827a206f56af32e590ba56d5d2d085f558508192593743f16b2306495269f"
+dependencies = [
+ "cc",
+]
+
+[[package]]
+name = "idna"
+version = "0.4.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7d20d6b07bfbc108882d88ed8e37d39636dcc260e15e30c45e6ba089610b917c"
+dependencies = [
+ "unicode-bidi",
+ "unicode-normalization",
+]
+
+[[package]]
 name = "indoc"
 version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bfa799dd5ed20a7e349f3b4639aa80d74549c81716d9ec4f994c9b5815598306"
 
 [[package]]
 name = "inotify"
 version = "0.9.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f8069d3ec154eb856955c1c0fbffefbf5f3c40a104ec912d4797314c1801abff"
 dependencies = [
- "bitflags 1.3.2",
+ "bitflags",
  "inotify-sys",
  "libc",
 ]
 
 [[package]]
 name = "inotify-sys"
 version = "0.1.5"
@@ -867,20 +1114,21 @@
 checksum = "7a5bbe824c507c5da5956355e86a746d82e0e1464f65d862cc5e71da70e94b2c"
 dependencies = [
  "cfg-if",
 ]
 
 [[package]]
 name = "io-lifetimes"
-version = "1.0.5"
+version = "1.0.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1abeb7a0dd0f8181267ff8adc397075586500b81b28a73e8a0208b00fc170fb3"
+checksum = "eae7b9aee968036d54dce06cebaefd919e4472e753296daccd6d344e3e2df0c2"
 dependencies = [
+ "hermit-abi",
  "libc",
- "windows-sys 0.45.0",
+ "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "ipcbus"
 version = "0.1.0"
 dependencies = [
  "event-listener",
@@ -890,49 +1138,60 @@
  "nix",
  "socket2",
  "tracing",
 ]
 
 [[package]]
 name = "is-terminal"
-version = "0.4.3"
+version = "0.4.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "22e18b0a45d56fe973d6db23972bf5bc46f988a4a2385deac9cc29572f09daef"
+checksum = "adcf93614601c8129ddf72e2d5633df827ba6551541c6d8c59520a371475be1f"
 dependencies = [
  "hermit-abi",
  "io-lifetimes",
  "rustix",
- "windows-sys 0.45.0",
+ "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "itoa"
-version = "1.0.5"
+version = "1.0.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fad582f4b9e86b6caa621cabeb0963332d92eea04729ab12892c2533951e6440"
+checksum = "453ad9f582a441959e5f0d088b02ce04cfe8d51a8eaf077f12ac6d3e94164ca6"
+
+[[package]]
+name = "jobserver"
+version = "0.1.26"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "936cfd212a0155903bcbc060e316fb6cc7cbf2e1907329391ebadc1fe0ce77c2"
+dependencies = [
+ "libc",
+]
 
 [[package]]
 name = "js-sys"
-version = "0.3.61"
+version = "0.3.64"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "445dde2150c55e483f3d8416706b97ec8e8237c307e5b7b4b8dd15e6af2a0730"
+checksum = "c5f195fe497f702db0f318b07fdd68edb16955aed830df8363d837542f8f935a"
 dependencies = [
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "k256"
-version = "0.11.6"
+version = "0.13.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "72c1e0b51e7ec0a97369623508396067a486bd0cbed95a2659a4b863d28cfc8b"
+checksum = "cadb76004ed8e97623117f3df85b17aaa6626ab0b0831e6573f104df16cd1bcc"
 dependencies = [
  "cfg-if",
  "ecdsa",
  "elliptic-curve",
+ "once_cell",
  "sha2",
+ "signature",
 ]
 
 [[package]]
 name = "kqueue"
 version = "1.0.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2c8fc60ba15bf51257aa9807a48a61013db043fcf3a78cb0d916e8e396dcad98"
@@ -943,186 +1202,216 @@
 
 [[package]]
 name = "kqueue-sys"
 version = "1.0.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8367585489f01bc55dd27404dcf56b95e6da061a256a666ab23be9ba96a2e587"
 dependencies = [
- "bitflags 1.3.2",
+ "bitflags",
  "libc",
 ]
 
 [[package]]
 name = "lazy_static"
 version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e2abad23fbc42b3700f2f279844dc832adb2b2eb069b2df918f455c4e18cc646"
 
 [[package]]
 name = "libc"
-version = "0.2.141"
+version = "0.2.142"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "6a987beff54b60ffa6d51982e1aa1146bc42f19bd26be28b0586f252fccf5317"
+
+[[package]]
+name = "libgit2-sys"
+version = "0.15.2+1.6.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3304a64d199bb964be99741b7a14d26972741915b3649639149b2479bb46f4b5"
+checksum = "a80df2e11fb4a61f4ba2ab42dbe7f74468da143f1a75c74e11dee7c813f694fa"
+dependencies = [
+ "cc",
+ "libc",
+ "libz-sys",
+ "pkg-config",
+]
+
+[[package]]
+name = "libz-sys"
+version = "1.1.9"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "56ee889ecc9568871456d42f603d6a0ce59ff328d291063a45cbdf0036baf6db"
+dependencies = [
+ "cc",
+ "libc",
+ "pkg-config",
+ "vcpkg",
+]
 
 [[package]]
 name = "linkspace"
-version = "0.1.4"
+version = "0.3.0-rc1"
 dependencies = [
  "anyhow",
  "backtrace",
+ "build-info",
+ "build-info-build",
  "linkspace-common",
  "tracing",
 ]
 
 [[package]]
 name = "linkspace-argon2-identity"
-version = "0.1.0"
+version = "0.3.0-rc1"
 dependencies = [
- "base64",
+ "base64 0.21.2",
  "linkspace-cryptography",
  "rust-argon2",
  "thiserror",
 ]
 
 [[package]]
 name = "linkspace-cli"
-version = "0.1.4"
+version = "0.3.0-rc1"
 dependencies = [
  "anyhow",
+ "build-info",
+ "build-info-build",
+ "crossbeam-channel",
+ "either",
  "linkspace",
  "linkspace-common",
+ "memmap2 0.6.2",
  "serde_json",
+ "tracing",
  "tracing-subscriber",
 ]
 
 [[package]]
 name = "linkspace-common"
-version = "0.1.1"
+version = "0.3.0-rc1"
 dependencies = [
  "abe",
  "anyhow",
  "async_executors",
  "byte-fmt",
  "clap",
  "either",
  "futures",
  "linkspace-argon2-identity",
  "linkspace-core",
  "linkspace-pkt",
- "memmap2",
+ "memmap2 0.5.10",
  "notify",
  "rand",
  "rand_chacha",
  "rpassword",
  "serde",
  "thiserror",
  "tracing",
  "tracing-subscriber",
- "tracing-test",
 ]
 
 [[package]]
 name = "linkspace-core"
-version = "0.1.1"
+version = "0.3.0-rc1"
 dependencies = [
  "anyhow",
- "arrayvec 0.7.2",
+ "arrayvec",
  "dunce",
  "either",
  "ipcbus",
  "libc",
  "linkspace-cryptography",
  "linkspace-pkt",
  "lmdb-rkv",
  "lmdb-rkv-sys",
  "parse-display",
- "rpds",
  "serde",
  "thiserror",
  "time",
  "tracing",
 ]
 
 [[package]]
 name = "linkspace-cryptography"
-version = "0.1.0"
+version = "0.3.0-rc1"
 dependencies = [
  "blake3",
  "getrandom",
  "k256",
  "rand",
  "rand_chacha",
  "rand_core",
  "thiserror",
 ]
 
 [[package]]
 name = "linkspace-handshake"
-version = "0.1.0"
+version = "0.3.0-rc1"
 dependencies = [
  "linkspace",
  "linkspace-common",
  "tracing-subscriber",
 ]
 
 [[package]]
 name = "linkspace-lns"
-version = "0.1.0"
+version = "0.3.0-rc1"
 dependencies = [
  "linkspace",
  "linkspace-common",
  "tracing-subscriber",
 ]
 
 [[package]]
 name = "linkspace-pkt"
-version = "0.1.1"
+version = "0.3.0-rc1"
 dependencies = [
  "anyhow",
- "arrayvec 0.7.2",
+ "arrayvec",
  "auto_impl",
  "bincode",
- "bitflags 1.3.2",
+ "bitflags",
+ "bstr",
  "byte-fmt",
  "bytes",
  "linkspace-cryptography",
  "serde",
  "serde_json",
  "static_assertions",
  "thiserror",
  "triomphe",
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "linkspace-py"
-version = "0.1.4"
+version = "0.3.0-rc2"
 dependencies = [
  "anyhow",
  "linkspace",
  "pyo3",
- "ref-cast",
  "smallvec",
  "tracing",
  "tracing-subscriber",
 ]
 
 [[package]]
 name = "linux-raw-sys"
-version = "0.1.4"
+version = "0.3.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f051f77a7c8e6957c0696eac88f26b0117e54f52d3fc682ab19397a8812846a4"
+checksum = "ef53942eb7bf7ff43a617b3e2c1c4a5ecf5944a7c1bc12d7ee39bbb15e5c1519"
 
 [[package]]
 name = "lmdb-rkv"
 version = "0.14.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "447a296f7aca299cfbb50f4e4f3d49451549af655fb7215d7f8c0c3d64bad42b"
 dependencies = [
- "bitflags 1.3.2",
+ "bitflags",
  "byteorder",
  "libc",
  "lmdb-rkv-sys",
 ]
 
 [[package]]
 name = "lmdb-rkv-sys"
@@ -1133,29 +1422,37 @@
  "cc",
  "libc",
  "pkg-config",
 ]
 
 [[package]]
 name = "lock_api"
-version = "0.4.9"
+version = "0.4.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "435011366fe56583b16cf956f9df0095b405b82d76425bc8981c0e22e60ec4df"
+checksum = "c1cc9717a20b1bb222f333e6a92fd32f7d8a18ddc5a3191a11af45dcbf4dcd16"
 dependencies = [
  "autocfg",
  "scopeguard",
 ]
 
 [[package]]
 name = "log"
-version = "0.4.17"
+version = "0.4.19"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "abb12e687cfb44aa40f41fc3978ef76448f9b6038cad6aef4259d3c095a2382e"
+checksum = "b06a4cde4c0f271a446782e3eff8de789548ce57dbc8eca9292c27f4a42004b4"
+
+[[package]]
+name = "lzma-sys"
+version = "0.1.20"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "5fda04ab3764e6cde78b9974eec4f779acaba7c4e84b36eca3cf77c581b85d27"
 dependencies = [
- "cfg-if",
+ "cc",
+ "libc",
+ "pkg-config",
 ]
 
 [[package]]
 name = "matchers"
 version = "0.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8263075bb86c5a1b1427b5ae862e8889656f126e9f77c484496e8b47cf5c5558"
@@ -1167,17 +1464,26 @@
 name = "memchr"
 version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2dffe52ecf27772e601905b7522cb4ef790d2cc203488bbd0e2fe85fcb74566d"
 
 [[package]]
 name = "memmap2"
-version = "0.5.8"
+version = "0.5.10"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "83faa42c0a078c393f6b29d5db232d8be22776a891f8f56e5284faee4a20b327"
+dependencies = [
+ "libc",
+]
+
+[[package]]
+name = "memmap2"
+version = "0.6.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4b182332558b18d807c4ce1ca8ca983b34c3ee32765e47b3f0f69b90355cc1dc"
+checksum = "6d28bba84adfe6646737845bc5ebbfa2c08424eb1c37e94a1fd2a82adb56a872"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "memoffset"
 version = "0.6.5"
@@ -1203,118 +1509,151 @@
 checksum = "b275950c28b37e794e8c55d88aeb5e139d0ce23fdbbeda68f8d7174abdf9e8fa"
 dependencies = [
  "adler",
 ]
 
 [[package]]
 name = "mio"
-version = "0.8.5"
+version = "0.8.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e5d732bc30207a6423068df043e3d02e0735b155ad7ce1a6f76fe2baa5b158de"
+checksum = "927a765cd3fc26206e66b296465fa9d3e5ab003e651c1b3c060e7956d96b19d2"
 dependencies = [
  "libc",
  "log",
  "wasi",
- "windows-sys 0.42.0",
+ "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "nix"
 version = "0.24.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fa52e972a9a719cecb6864fb88568781eb706bac2cd1d4f04a648542dbf78069"
 dependencies = [
- "bitflags 1.3.2",
+ "bitflags",
  "cfg-if",
  "libc",
  "memoffset 0.6.5",
 ]
 
 [[package]]
 name = "notify"
-version = "5.1.0"
+version = "5.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "58ea850aa68a06e48fdb069c0ec44d0d64c8dbffa49bf3b6f7f0a901fdea1ba9"
+checksum = "729f63e1ca555a43fe3efa4f3efdf4801c479da85b432242a7b726f353c88486"
 dependencies = [
- "bitflags 1.3.2",
+ "bitflags",
  "crossbeam-channel",
  "filetime",
  "fsevent-sys",
  "inotify",
  "kqueue",
  "libc",
  "mio",
  "walkdir",
- "windows-sys 0.42.0",
+ "windows-sys 0.45.0",
 ]
 
 [[package]]
 name = "nu-ansi-term"
 version = "0.46.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "77a8165726e8236064dbb45459242600304b42a5ea24ee2948e18e023bf7ba84"
 dependencies = [
  "overload",
  "winapi",
 ]
 
 [[package]]
+name = "num-bigint"
+version = "0.4.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f93ab6289c7b344a8a9f60f88d80aa20032336fe78da341afc91c8a2341fc75f"
+dependencies = [
+ "autocfg",
+ "num-integer",
+ "num-traits",
+]
+
+[[package]]
+name = "num-integer"
+version = "0.1.45"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "225d3389fb3509a24c93f5c29eb6bde2586b98d9f016636dff58d7c6f7569cd9"
+dependencies = [
+ "autocfg",
+ "num-traits",
+]
+
+[[package]]
+name = "num-traits"
+version = "0.2.15"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "578ede34cf02f8924ab9447f50c28075b4d3e5b269972345e7e0372b38c6cdcd"
+dependencies = [
+ "autocfg",
+]
+
+[[package]]
 name = "object"
-version = "0.30.3"
+version = "0.30.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ea86265d3d3dcb6a27fc51bd29a4bf387fae9d2986b823079d4986af253eb439"
+checksum = "03b4680b86d9cfafba8fc491dc9b6df26b68cf40e9e6cd73909194759a63c385"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "once_cell"
-version = "1.17.0"
+version = "1.18.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6f61fba1741ea2b3d6a1e3178721804bb716a68a6aeba1149b5d52e3d464ea66"
+checksum = "dd8b5dd2ae5ed71462c540258bedcb51965123ad7e7ccf4b9a8cafaa4a63576d"
 
 [[package]]
-name = "os_str_bytes"
-version = "6.4.1"
+name = "output_vt100"
+version = "0.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9b7820b9daea5457c9f21c69448905d723fbd21136ccf521748f23fd49e723ee"
+checksum = "628223faebab4e3e40667ee0b2336d34a5b960ff60ea743ddfdbcf7770bcfb66"
+dependencies = [
+ "winapi",
+]
 
 [[package]]
 name = "overload"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b15813163c1d831bf4a13c3610c05c0d03b39feb07f7e09fa234dac9b15aaf39"
 
 [[package]]
 name = "parking"
-version = "2.0.0"
+version = "2.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "427c3892f9e783d91cc128285287e70a59e206ca452770ece88a76f7a3eddd72"
+checksum = "14f2252c834a40ed9bb5422029649578e63aa341ac401f74e719dd1afda8394e"
 
 [[package]]
 name = "parking_lot"
 version = "0.12.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3742b2c103b9f06bc9fff0a37ff4912935851bee6d36f3c02bcc755bcfec228f"
 dependencies = [
  "lock_api",
  "parking_lot_core",
 ]
 
 [[package]]
 name = "parking_lot_core"
-version = "0.9.7"
+version = "0.9.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9069cbb9f99e3a5083476ccb29ceb1de18b9118cafa53e90c9551235de2b9521"
+checksum = "93f00c865fe7cabf650081affecd3871070f26767e7b2070a3ffae14c654b447"
 dependencies = [
  "cfg-if",
  "libc",
- "redox_syscall",
+ "redox_syscall 0.3.5",
  "smallvec",
- "windows-sys 0.45.0",
+ "windows-targets 0.48.0",
 ]
 
 [[package]]
 name = "parse-display"
 version = "0.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3b25af4ef94a8528b41fb49a696e361dc6ef975c782417268072d987ac327964"
@@ -1330,37 +1669,43 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "73f106cced1f4b645e3fca6125105cdf7407e35d1af710f290aac530f6b826b9"
 dependencies = [
  "once_cell",
  "proc-macro2",
  "quote",
  "regex",
- "regex-syntax",
+ "regex-syntax 0.6.29",
  "structmeta",
- "syn 1.0.107",
+ "syn 1.0.109",
 ]
 
 [[package]]
+name = "percent-encoding"
+version = "2.3.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "9b2a4787296e9989611394c33f193f676704af1686e70b8f8033ab5ba9a35a94"
+
+[[package]]
 name = "pin-project"
-version = "1.0.12"
+version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ad29a609b6bcd67fee905812e544992d216af9d755757c05ed2d0e15a74c6ecc"
+checksum = "c95a7476719eab1e366eaf73d0260af3021184f18177925b07f54b30089ceead"
 dependencies = [
  "pin-project-internal",
 ]
 
 [[package]]
 name = "pin-project-internal"
-version = "1.0.12"
+version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "069bdb1e05adc7a8990dce9cc75370895fbe4e3d58b9b73bf1aee56359344a55"
+checksum = "39407670928234ebc5e6e580247dd567ad73a3578460c5990f9503df207e8f07"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 1.0.107",
+ "syn 2.0.18",
 ]
 
 [[package]]
 name = "pin-project-lite"
 version = "0.2.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e0a7ae3ac2f1173085d398531c705756c94a4c56843785df85a60c1a0afac116"
@@ -1369,56 +1714,56 @@
 name = "pin-utils"
 version = "0.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8b870d8c151b6f2fb93e84a13146138f05d02ed11c7e7c54f8826aaaf7c9f184"
 
 [[package]]
 name = "pkcs8"
-version = "0.9.0"
+version = "0.10.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9eca2c590a5f85da82668fa685c09ce2888b9430e83299debf1f34b65fd4a4ba"
+checksum = "f950b2377845cebe5cf8b5165cb3cc1a5e0fa5cfa3e1f7f55707d8fd82e0a7b7"
 dependencies = [
  "der",
  "spki",
 ]
 
 [[package]]
 name = "pkg-config"
-version = "0.3.26"
+version = "0.3.27"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6ac9a59f73473f1b8d852421e59e64809f025994837ef743615c6d0c5b305160"
+checksum = "26072860ba924cbfa98ea39c8c19b4dd6a4a25423dbdf219c1eca91aa0cf6964"
 
 [[package]]
 name = "ppv-lite86"
 version = "0.2.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5b40af805b3121feab8a3c29f04d8ad262fa8e0561883e7653e024ae4479e6de"
 
 [[package]]
-name = "pretty"
-version = "0.11.3"
+name = "pretty_assertions"
+version = "1.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "83f3aa1e3ca87d3b124db7461265ac176b40c277f37e503eaa29c9c75c037846"
+checksum = "a25e9bcb20aa780fd0bb16b72403a9064d6b3f22f026946029acb941a50af755"
 dependencies = [
- "arrayvec 0.5.2",
- "log",
- "typed-arena",
- "unicode-segmentation",
+ "ctor",
+ "diff",
+ "output_vt100",
+ "yansi",
 ]
 
 [[package]]
 name = "proc-macro-error"
 version = "1.0.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "da25490ff9892aab3fcf7c36f08cfb902dd3e71ca0f9f9517bea02a73a5ce38c"
 dependencies = [
  "proc-macro-error-attr",
  "proc-macro2",
  "quote",
- "syn 1.0.107",
+ "syn 1.0.109",
  "version_check",
 ]
 
 [[package]]
 name = "proc-macro-error-attr"
 version = "1.0.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -1427,26 +1772,26 @@
  "proc-macro2",
  "quote",
  "version_check",
 ]
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.54"
+version = "1.0.60"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e472a104799c74b514a57226160104aa483546de37e839ec50e3c2e41dd87534"
+checksum = "dec2b086b7a862cf4de201096214fa870344cf922b2b30c167badb3af3195406"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
-version = "0.18.2"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cfb848f80438f926a9ebddf0a539ed6065434fd7aae03a89312a9821f81b8501"
+checksum = "e3b1ac5b3731ba34fdaa9785f8d74d17448cd18f30cf19e0c7e7b1fdb5272109"
 dependencies = [
  "anyhow",
  "cfg-if",
  "indoc",
  "libc",
  "memoffset 0.8.0",
  "parking_lot",
@@ -1455,71 +1800,65 @@
  "pyo3-macros",
  "serde",
  "unindent",
 ]
 
 [[package]]
 name = "pyo3-build-config"
-version = "0.18.2"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "98a42e7f42e917ce6664c832d5eee481ad514c98250c49e0b03b20593e2c7ed0"
+checksum = "9cb946f5ac61bb61a5014924910d936ebd2b23b705f7a4a3c40b05c720b079a3"
 dependencies = [
  "once_cell",
  "target-lexicon",
 ]
 
 [[package]]
 name = "pyo3-ffi"
-version = "0.18.2"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a0707f0ab26826fe4ccd59b69106e9df5e12d097457c7b8f9c0fd1d2743eec4d"
+checksum = "fd4d7c5337821916ea2a1d21d1092e8443cf34879e53a0ac653fbb98f44ff65c"
 dependencies = [
  "libc",
  "pyo3-build-config",
 ]
 
 [[package]]
 name = "pyo3-macros"
-version = "0.18.2"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "978d18e61465ecd389e1f235ff5a467146dc4e3c3968b90d274fe73a5dd4a438"
+checksum = "a9d39c55dab3fc5a4b25bbd1ac10a2da452c4aca13bb450f22818a002e29648d"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
- "syn 1.0.107",
+ "syn 1.0.109",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
-version = "0.18.2"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8e0e1128f85ce3fca66e435e08aa2089a2689c1c48ce97803e13f63124058462"
+checksum = "97daff08a4c48320587b5224cc98d609e3c27b6d437315bd40b605c98eeb5918"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 1.0.107",
+ "syn 1.0.109",
 ]
 
 [[package]]
 name = "quote"
-version = "1.0.26"
+version = "1.0.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4424af4bf778aae2051a77b60283332f386554255d722233d09fbfc7e30da2fc"
+checksum = "1b9ab9c7eadfd8df19006f1cf1a4aed13540ed5cbc047010ece5826e10825488"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
-name = "radium"
-version = "0.7.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dc33ff2d4973d518d823d61aa239014831e521c75da58e3df4840d3f47749d09"
-
-[[package]]
 name = "rand"
 version = "0.8.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "34af8d1a0e25924bc5b7c43c079c942339d8f0a8b57c39049bef581b46327404"
 dependencies = [
  "libc",
  "rand_chacha",
@@ -1547,109 +1886,94 @@
 
 [[package]]
 name = "redox_syscall"
 version = "0.2.16"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fb5a58c1855b4b6819d59012155603f0b22ad30cad752600aadfcb695265519a"
 dependencies = [
- "bitflags 1.3.2",
-]
-
-[[package]]
-name = "ref-cast"
-version = "1.0.14"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8c78fb8c9293bcd48ef6fce7b4ca950ceaf21210de6e105a883ee280c0f7b9ed"
-dependencies = [
- "ref-cast-impl",
+ "bitflags",
 ]
 
 [[package]]
-name = "ref-cast-impl"
-version = "1.0.14"
+name = "redox_syscall"
+version = "0.3.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9f9c0c92af03644e4806106281fe2e068ac5bc0ae74a707266d06ea27bccee5f"
+checksum = "567664f262709473930a4bf9e51bf2ebf3348f2e748ccc50dea20646858f8f29"
 dependencies = [
- "proc-macro2",
- "quote",
- "syn 1.0.107",
+ "bitflags",
 ]
 
 [[package]]
 name = "regex"
-version = "1.7.1"
+version = "1.8.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "48aaa5748ba571fb95cd2c85c09f629215d3a6ece942baa100950af03a34f733"
+checksum = "d0ab3ca65655bb1e41f2a8c8cd662eb4fb035e67c3f78da1d61dffe89d07300f"
 dependencies = [
  "aho-corasick",
  "memchr",
- "regex-syntax",
+ "regex-syntax 0.7.2",
 ]
 
 [[package]]
 name = "regex-automata"
 version = "0.1.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6c230d73fb8d8c1b9c0b3135c5142a8acee3a0558fb8db5cf1cb65f8d7862132"
 dependencies = [
- "regex-syntax",
+ "regex-syntax 0.6.29",
 ]
 
 [[package]]
 name = "regex-syntax"
-version = "0.6.28"
+version = "0.6.29"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f162c6dd7b008981e4d40210aca20b4bd0f9b60ca9271061b07f78537722f2e1"
+
+[[package]]
+name = "regex-syntax"
+version = "0.7.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "456c603be3e8d448b072f410900c09faf164fbce2d480456f50eea6e25f9c848"
+checksum = "436b050e76ed2903236f032a59761c1eb99e1b0aead2c257922771dab1fc8c78"
 
 [[package]]
 name = "rfc6979"
-version = "0.3.1"
+version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7743f17af12fa0b03b803ba12cd6a8d9483a587e89c69445e3909655c0b9fabb"
+checksum = "f8dd2a808d456c4a54e300a23e9f5a67e122c3024119acbfd73e3bf664491cb2"
 dependencies = [
- "crypto-bigint",
  "hmac",
- "zeroize",
+ "subtle",
 ]
 
 [[package]]
 name = "rpassword"
 version = "7.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6678cf63ab3491898c0d021b493c94c9b221d91295294a2a5746eacbe5928322"
 dependencies = [
  "libc",
  "rtoolbox",
  "winapi",
 ]
 
 [[package]]
-name = "rpds"
-version = "0.12.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "66262ea963eff99163e6b741fbc3417a52cc13074728c1047e9911789df9b000"
-dependencies = [
- "archery",
-]
-
-[[package]]
 name = "rtoolbox"
 version = "0.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "034e22c514f5c0cb8a10ff341b9b048b5ceb21591f31c8f44c43b960f9b3524a"
 dependencies = [
  "libc",
  "winapi",
 ]
 
 [[package]]
 name = "ruint"
-version = "1.7.0"
+version = "1.8.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0ad3a104dc8c3867f653b0fec89c65e00b0ceb752718ad282177a7e0f33257ac"
+checksum = "9d470e29e933dac4101180fd6574971892315c414cf2961a192729089687cc9b"
 dependencies = [
  "derive_more",
  "ruint-macro",
  "rustc_version",
  "thiserror",
 ]
 
@@ -1661,54 +1985,53 @@
 
 [[package]]
 name = "rust-argon2"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b50162d19404029c1ceca6f6980fe40d45c8b369f6f44446fa14bb39573b5bb9"
 dependencies = [
- "base64",
+ "base64 0.13.1",
  "blake2b_simd",
  "constant_time_eq 0.1.5",
- "crossbeam-utils",
 ]
 
 [[package]]
 name = "rustc-demangle"
-version = "0.1.21"
+version = "0.1.23"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7ef03e0a2b150c7a90d01faf6254c9c48a41e95fb2a8c2ac1c6f0d2b9aefc342"
+checksum = "d626bb9dae77e28219937af045c257c28bfd3f69333c512553507f5f9798cb76"
 
 [[package]]
 name = "rustc_version"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bfa0f585226d2e68097d4f95d113b15b83a82e819ab25717ec0590d9584ef366"
 dependencies = [
  "semver",
 ]
 
 [[package]]
 name = "rustix"
-version = "0.36.8"
+version = "0.37.19"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f43abb88211988493c1abb44a70efa56ff0ce98f233b7b276146f1f3f7ba9644"
+checksum = "acf8729d8542766f1b2cf77eb034d52f40d375bb8b615d0b147089946e16613d"
 dependencies = [
- "bitflags 1.3.2",
+ "bitflags",
  "errno",
  "io-lifetimes",
  "libc",
  "linux-raw-sys",
- "windows-sys 0.45.0",
+ "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "ryu"
-version = "1.0.12"
+version = "1.0.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7b4b9743ed687d4b4bcedf9ff5eaa7398495ae14e61cba0a295704edbc7decde"
+checksum = "f91339c0467de62360649f8d3e185ca8de4224ff281f66000de5eb2a77a79041"
 
 [[package]]
 name = "same-file"
 version = "1.0.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "93fc1dc3aaa9bfed95e02e6eadabb4baf7e3078b0bd1b4d7b6b0b68378900502"
 dependencies = [
@@ -1719,43 +2042,46 @@
 name = "scopeguard"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d29ab0c6d3fc0ee92fe66e2d99f700eab17a8d57d1c1d3b748380fb20baa78cd"
 
 [[package]]
 name = "sec1"
-version = "0.3.0"
+version = "0.7.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3be24c1842290c45df0a7bf069e0c268a747ad05a192f2fd7dcfdbc1cba40928"
+checksum = "f0aec48e813d6b90b15f0b8948af3c63483992dee44c03e9930b3eebdabe046e"
 dependencies = [
  "base16ct",
  "der",
  "generic-array",
  "pkcs8",
  "subtle",
  "zeroize",
 ]
 
 [[package]]
 name = "semver"
-version = "1.0.16"
+version = "1.0.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "58bc9567378fc7690d6b2addae4e60ac2eeea07becb2c64b9f218b53865cba2a"
+checksum = "bebd363326d05ec3e2f532ab7660680f3b02130d780c299bca73469d521bc0ed"
+dependencies = [
+ "serde",
+]
 
 [[package]]
 name = "send_wrapper"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f638d531eccd6e23b980caf34876660d38e265409d8e99b397ab71eb3612fad0"
 
 [[package]]
 name = "serde"
-version = "1.0.159"
+version = "1.0.160"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3c04e8343c3daeec41f58990b9d77068df31209f2af111e059e9fe9646693065"
+checksum = "bb2f3770c8bce3bcda7e149193a069a0f4365bda1fa5cd88e03bca26afc1216c"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde_bytes"
 version = "0.11.9"
@@ -1763,39 +2089,39 @@
 checksum = "416bda436f9aab92e02c8e10d49a15ddd339cea90b6e340fe51ed97abb548294"
 dependencies = [
  "serde",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.159"
+version = "1.0.160"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4c614d17805b093df4b147b51339e7e44bf05ef59fba1e45d83500bcfb4d8585"
+checksum = "291a097c63d8497e00160b166a967a4a79c64f3facdd01cbd7502231688d77df"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.11",
+ "syn 2.0.18",
 ]
 
 [[package]]
 name = "serde_json"
-version = "1.0.94"
+version = "1.0.97"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1c533a59c9d8a93a09c6ab31f0fd5e5f4dd1b8fc9434804029839884765d04ea"
+checksum = "bdf3bf93142acad5821c99197022e170842cdbc1c30482b98750c688c640842a"
 dependencies = [
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
 name = "sha2"
-version = "0.10.6"
+version = "0.10.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "82e6b795fe2e3b1e845bafcb27aa35405c4d47cdfc92af5fc8d3002f76cebdc0"
+checksum = "479fb9d862239e610720565ca91403019f2f00410f1864c5aa7479b950a76ed8"
 dependencies = [
  "cfg-if",
  "cpufeatures",
  "digest",
 ]
 
 [[package]]
@@ -1805,52 +2131,52 @@
 checksum = "900fba806f70c630b0a382d0d825e17a0f19fcd059a2ade1ff237bcddf446b31"
 dependencies = [
  "lazy_static",
 ]
 
 [[package]]
 name = "signature"
-version = "1.6.4"
+version = "2.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "74233d3b3b2f6d4b006dc19dee745e73e2a6bfb6f93607cd3b02bd5b00797d7c"
+checksum = "5e1788eed21689f9cf370582dfc467ef36ed9c707f073528ddafa8d83e3b8500"
 dependencies = [
  "digest",
  "rand_core",
 ]
 
 [[package]]
 name = "slab"
-version = "0.4.7"
+version = "0.4.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4614a76b2a8be0058caa9dbbaf66d988527d86d003c11a94fbd335d7661edcef"
+checksum = "6528351c9bc8ab22353f9d776db39a20288e8d6c37ef8cfe3317cf875eecfc2d"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "smallvec"
 version = "1.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a507befe795404456341dfab10cef66ead4c041f62b8b11bbb92bffe5d0953e0"
 
 [[package]]
 name = "socket2"
-version = "0.4.7"
+version = "0.4.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "02e2d2db9033d13a1567121ddd7a095ee144db4e1ca1b1bda3419bc0da294ebd"
+checksum = "64a4a911eed85daf18834cfaa86a79b7d266ff93ff5ba14005426219480ed662"
 dependencies = [
  "libc",
  "winapi",
 ]
 
 [[package]]
 name = "spki"
-version = "0.6.0"
+version = "0.7.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "67cf02bbac7a337dc36e4f5a693db6c21e7863f45070f7064577eb4367a3212b"
+checksum = "9d1e996ef02c474957d681f1b05213dfb0abab947b446a62d37770b23500184a"
 dependencies = [
  "base64ct",
  "der",
 ]
 
 [[package]]
 name = "stable_deref_trait"
@@ -1868,168 +2194,169 @@
 name = "strsim"
 version = "0.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "73473c0e59e6d5812c5dfe2a064a6444949f089e20eec9a2e5506596494e4623"
 
 [[package]]
 name = "structmeta"
-version = "0.1.5"
+version = "0.1.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1bd9c2155aa89fb2c2cb87d99a610c689e7c47099b3e9f1c8a8f53faf4e3d2e3"
+checksum = "104842d6278bf64aa9d2f182ba4bde31e8aec7a131d29b7f444bb9b344a09e2a"
 dependencies = [
  "proc-macro2",
  "quote",
  "structmeta-derive",
- "syn 1.0.107",
+ "syn 1.0.109",
 ]
 
 [[package]]
 name = "structmeta-derive"
-version = "0.1.5"
+version = "0.1.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bafede0d0a2f21910f36d47b1558caae3076ed80f6f3ad0fc85a91e6ba7e5938"
+checksum = "24420be405b590e2d746d83b01f09af673270cf80e9b003a5fa7b651c58c7d93"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 1.0.107",
+ "syn 1.0.109",
 ]
 
 [[package]]
 name = "subtle"
-version = "2.4.1"
+version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6bdef32e8150c2a081110b42772ffe7d7c9032b606bc226c8260fd97e0976601"
+checksum = "81cdd64d312baedb58e21336b31bc043b77e01cc99033ce76ef539f78e965ebc"
 
 [[package]]
 name = "syn"
-version = "1.0.107"
+version = "1.0.109"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1f4064b5b16e03ae50984a5a8ed5d4f8803e6bc1fd170a3cda91a1be4b18e3f5"
+checksum = "72b64191b275b66ffe2469e8af2c1cfe3bafa67b529ead792a6d0160888b4237"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "syn"
-version = "2.0.11"
+version = "2.0.18"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "21e3787bb71465627110e7d87ed4faaa36c1f61042ee67badb9e2ef173accc40"
+checksum = "32d41677bcbe24c20c52e7c70b0d8db04134c5d1066bf98662e2871ad200ea3e"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
-name = "tap"
-version = "1.0.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "55937e1799185b12863d447f42597ed69d9928686b8d88a1df17376a097d8369"
-
-[[package]]
 name = "target-lexicon"
-version = "0.12.5"
+version = "0.12.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9410d0f6853b1d94f0e519fb95df60f29d2c1eff2d921ffdf01a4c8a3b54f12d"
-
-[[package]]
-name = "termcolor"
-version = "1.2.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "be55cf8942feac5c765c2c993422806843c9a9a45d4d5c407ad6dd2ea95eb9b6"
-dependencies = [
- "winapi-util",
-]
+checksum = "1b1c7f239eb94671427157bd93b3694320f3668d4e1eff08c7285366fd777fac"
 
 [[package]]
 name = "thiserror"
-version = "1.0.38"
+version = "1.0.40"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6a9cd18aa97d5c45c6603caea1da6628790b37f7a34b6ca89522331c5180fed0"
+checksum = "978c9a314bd8dc99be594bc3c175faaa9794be04a5a5e153caba6915336cebac"
 dependencies = [
  "thiserror-impl",
 ]
 
 [[package]]
 name = "thiserror-impl"
-version = "1.0.38"
+version = "1.0.40"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1fb327af4685e4d03fa8cbcf1716380da910eeb2bb8be417e7f9fd3fb164f36f"
+checksum = "f9456a42c5b0d803c8cd86e73dd7cc9edd429499f37a3550d286d5e86720569f"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 1.0.107",
+ "syn 2.0.18",
 ]
 
 [[package]]
 name = "thread_local"
-version = "1.1.4"
+version = "1.1.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5516c27b78311c50bf42c071425c560ac799b11c30b31f87e3081965fe5e0180"
+checksum = "3fdd6f064ccff2d6567adcb3873ca630700f00b5ad3f060c25b5dcfd9a4ce152"
 dependencies = [
+ "cfg-if",
  "once_cell",
 ]
 
 [[package]]
 name = "time"
-version = "0.3.17"
+version = "0.3.22"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a561bf4617eebd33bca6434b988f39ed798e527f51a1e797d0ee4f61c0a38376"
+checksum = "ea9e1b3cf1243ae005d9e74085d4d542f3125458f3a81af210d901dcd7411efd"
 dependencies = [
  "itoa",
  "serde",
  "time-core",
  "time-macros",
 ]
 
 [[package]]
 name = "time-core"
-version = "0.1.0"
+version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2e153e1f1acaef8acc537e68b44906d2db6436e2b35ac2c6b42640fff91f00fd"
+checksum = "7300fbefb4dadc1af235a9cef3737cea692a9d97e1b9cbcd4ebdae6f8868e6fb"
 
 [[package]]
 name = "time-macros"
-version = "0.2.6"
+version = "0.2.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d967f99f534ca7e495c575c62638eebc2898a8c84c119b89e250477bc4ba16b2"
+checksum = "372950940a5f07bf38dbe211d7283c9e6d7327df53794992d293e534c733d09b"
 dependencies = [
  "time-core",
 ]
 
 [[package]]
+name = "tinyvec"
+version = "1.6.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "87cc5ceb3875bb20c2890005a4e226a4651264a5c75edb2421b52861a0a0cb50"
+dependencies = [
+ "tinyvec_macros",
+]
+
+[[package]]
+name = "tinyvec_macros"
+version = "0.1.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "1f3ccbac311fea05f86f61904b462b55fb3df8837a366dfc601a0161d0532f20"
+
+[[package]]
 name = "tracing"
 version = "0.1.37"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8ce8c33a8d48bd45d624a6e523445fd21ec13d3653cd51f681abf67418f54eb8"
 dependencies = [
  "cfg-if",
  "pin-project-lite",
  "tracing-attributes",
  "tracing-core",
 ]
 
 [[package]]
 name = "tracing-attributes"
-version = "0.1.23"
+version = "0.1.25"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4017f8f45139870ca7e672686113917c71c7a6e02d4924eda67186083c03081a"
+checksum = "8803eee176538f94ae9a14b55b2804eb7e1441f8210b1c31290b3bccdccff73b"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 1.0.107",
+ "syn 2.0.18",
 ]
 
 [[package]]
 name = "tracing-core"
-version = "0.1.30"
+version = "0.1.31"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "24eb03ba0eab1fd845050058ce5e616558e8f8d8fca633e6b163fe25c797213a"
+checksum = "0955b8137a1df6f1a2e9a37d8a6656291ff0297c1a97c24e0d8425fe2312f79a"
 dependencies = [
  "once_cell",
  "valuable",
 ]
 
 [[package]]
 name = "tracing-log"
@@ -2040,199 +2367,200 @@
  "lazy_static",
  "log",
  "tracing-core",
 ]
 
 [[package]]
 name = "tracing-subscriber"
-version = "0.3.16"
+version = "0.3.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a6176eae26dd70d0c919749377897b54a9276bd7061339665dd68777926b5a70"
+checksum = "30a651bc37f915e81f087d86e62a18eec5f79550c7faff886f7090b4ea757c77"
 dependencies = [
  "matchers",
  "nu-ansi-term",
  "once_cell",
  "regex",
  "sharded-slab",
  "smallvec",
  "thread_local",
  "tracing",
  "tracing-core",
  "tracing-log",
 ]
 
 [[package]]
-name = "tracing-test"
-version = "0.2.4"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3a2c0ff408fe918a94c428a3f2ad04e4afd5c95bbc08fcf868eff750c15728a4"
-dependencies = [
- "lazy_static",
- "tracing-core",
- "tracing-subscriber",
- "tracing-test-macro",
-]
-
-[[package]]
-name = "tracing-test-macro"
-version = "0.2.4"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "258bc1c4f8e2e73a977812ab339d503e6feeb92700f6d07a6de4d321522d5c08"
-dependencies = [
- "lazy_static",
- "quote",
- "syn 1.0.107",
-]
-
-[[package]]
 name = "triomphe"
 version = "0.1.8"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f1ee9bd9239c339d714d657fac840c6d2a4f9c45f4f9ec7b0975113458be78db"
+source = "git+https://github.com/AntonSol919/triomphe#25f7047119235a7f705b8a73eb5e7089bafb3ae4"
 dependencies = [
  "serde",
  "stable_deref_trait",
 ]
 
 [[package]]
-name = "typed-arena"
-version = "2.0.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6af6ae20167a9ece4bcb41af5b80f8a1f1df981f6391189ce00fd257af04126a"
-
-[[package]]
 name = "typenum"
 version = "1.16.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "497961ef93d974e23eb6f433eb5fe1b7930b659f06d12dec6fc44a8f554c0bba"
 
 [[package]]
+name = "unicode-bidi"
+version = "0.3.13"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "92888ba5573ff080736b3648696b70cafad7d250551175acbaa4e0385b3e1460"
+
+[[package]]
 name = "unicode-ident"
-version = "1.0.6"
+version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "84a22b9f218b40614adcb3f4ff08b703773ad44fa9423e4e0d346d5db86e4ebc"
+checksum = "b15811caf2415fb889178633e7724bad2509101cde276048e013b9def5e51fa0"
 
 [[package]]
-name = "unicode-segmentation"
-version = "1.10.1"
+name = "unicode-normalization"
+version = "0.1.22"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1dd624098567895118886609431a7c3b8f516e41d30e0643f03d94592a147e36"
+checksum = "5c5713f0fc4b5db668a2ac63cdb7bb4469d8c9fed047b1d0292cc7b0ce2ba921"
+dependencies = [
+ "tinyvec",
+]
 
 [[package]]
 name = "unindent"
 version = "0.1.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e1766d682d402817b5ac4490b3c3002d91dfa0d22812f341609f97b08757359c"
 
 [[package]]
+name = "url"
+version = "2.4.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "50bff7831e19200a85b17131d085c25d7811bc4e186efdaf54bbd132994a88cb"
+dependencies = [
+ "form_urlencoded",
+ "idna",
+ "percent-encoding",
+]
+
+[[package]]
+name = "utf8parse"
+version = "0.2.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "711b9620af191e0cdc7468a8d14e709c3dcdb115b36f838e601583af800a370a"
+
+[[package]]
 name = "valuable"
 version = "0.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "830b7e5d4d90034032940e4ace0d9a9a057e7a45cd94e6c007832e39edb82f6d"
 
 [[package]]
+name = "vcpkg"
+version = "0.2.15"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "accd4ea62f7bb7a82fe23066fb0957d48ef677f6eeb8215f372f52e48bb32426"
+
+[[package]]
 name = "version_check"
 version = "0.9.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "49874b5167b65d7193b8aba1567f5c7d93d001cafc34600cee003eda787e483f"
 
 [[package]]
 name = "waker-fn"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9d5b2c62b4012a3e1eca5a7e077d13b3bf498c4073e33ccd58626607748ceeca"
 
 [[package]]
 name = "walkdir"
-version = "2.3.2"
+version = "2.3.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "808cf2735cd4b6866113f648b791c6adc5714537bc222d9347bb203386ffda56"
+checksum = "36df944cda56c7d8d8b7496af378e6b16de9284591917d307c9b4d313c44e698"
 dependencies = [
  "same-file",
- "winapi",
  "winapi-util",
 ]
 
 [[package]]
 name = "wasi"
 version = "0.11.0+wasi-snapshot-preview1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9c8d87e72b64a3b4db28d11ce29237c246188f4f51057d65a7eab63b7987e423"
 
 [[package]]
 name = "wasm-bindgen"
-version = "0.2.84"
+version = "0.2.87"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "31f8dcbc21f30d9b8f2ea926ecb58f6b91192c17e9d33594b3df58b2007ca53b"
+checksum = "7706a72ab36d8cb1f80ffbf0e071533974a60d0a308d01a5d0375bf60499a342"
 dependencies = [
  "cfg-if",
  "wasm-bindgen-macro",
 ]
 
 [[package]]
 name = "wasm-bindgen-backend"
-version = "0.2.84"
+version = "0.2.87"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "95ce90fd5bcc06af55a641a86428ee4229e44e07033963a2290a8e241607ccb9"
+checksum = "5ef2b6d3c510e9625e5fe6f509ab07d66a760f0885d858736483c32ed7809abd"
 dependencies = [
  "bumpalo",
  "log",
  "once_cell",
  "proc-macro2",
  "quote",
- "syn 1.0.107",
+ "syn 2.0.18",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-futures"
-version = "0.4.34"
+version = "0.4.37"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f219e0d211ba40266969f6dbdd90636da12f75bee4fc9d6c23d1260dadb51454"
+checksum = "c02dbc21516f9f1f04f187958890d7e6026df8d16540b7ad9492bc34a67cea03"
 dependencies = [
  "cfg-if",
  "js-sys",
  "wasm-bindgen",
  "web-sys",
 ]
 
 [[package]]
 name = "wasm-bindgen-macro"
-version = "0.2.84"
+version = "0.2.87"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4c21f77c0bedc37fd5dc21f897894a5ca01e7bb159884559461862ae90c0b4c5"
+checksum = "dee495e55982a3bd48105a7b947fd2a9b4a8ae3010041b9e0faab3f9cd028f1d"
 dependencies = [
  "quote",
  "wasm-bindgen-macro-support",
 ]
 
 [[package]]
 name = "wasm-bindgen-macro-support"
-version = "0.2.84"
+version = "0.2.87"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2aff81306fcac3c7515ad4e177f521b5c9a15f2b08f4e32d823066102f35a5f6"
+checksum = "54681b18a46765f095758388f2d0cf16eb8d4169b639ab575a8f5693af210c7b"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 1.0.107",
+ "syn 2.0.18",
  "wasm-bindgen-backend",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-shared"
-version = "0.2.84"
+version = "0.2.87"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0046fef7e28c3804e5e38bfa31ea2a0f73905319b677e57ebe37e49358989b5d"
+checksum = "ca6ad05a4870b2bf5fe995117d3728437bd27d7cd5f06f13c17443ef369775a1"
 
 [[package]]
 name = "web-sys"
-version = "0.3.61"
+version = "0.3.64"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e33b99f4b23ba3eec1a53ac264e35a755f00e966e0065077d6027c0f575b0b97"
+checksum = "9b85cbef8c220a6abc02aefd892dfc0fc23afb1c6a426316ec33253a3877249b"
 dependencies = [
  "js-sys",
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "winapi"
@@ -2262,101 +2590,167 @@
 [[package]]
 name = "winapi-x86_64-pc-windows-gnu"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "712e227841d057c1ee1cd2fb22fa7e5a5461ae8e48fa2ca79ec42cfc1931183f"
 
 [[package]]
-name = "windows-sys"
-version = "0.42.0"
+name = "windows"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5a3e1820f08b8513f676f7ab6c1f99ff312fb97b553d30ff4dd86f9f15728aa7"
+checksum = "e686886bc078bc1b0b600cac0147aadb815089b6e4da64016cbd754b6342700f"
 dependencies = [
- "windows_aarch64_gnullvm",
- "windows_aarch64_msvc",
- "windows_i686_gnu",
- "windows_i686_msvc",
- "windows_x86_64_gnu",
- "windows_x86_64_gnullvm",
- "windows_x86_64_msvc",
+ "windows-targets 0.48.0",
 ]
 
 [[package]]
 name = "windows-sys"
 version = "0.45.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "75283be5efb2831d37ea142365f009c02ec203cd29a3ebecbc093d52315b66d0"
 dependencies = [
- "windows-targets",
+ "windows-targets 0.42.2",
+]
+
+[[package]]
+name = "windows-sys"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "677d2418bec65e3338edb076e806bc1ec15693c5d0104683f2efe857f61056a9"
+dependencies = [
+ "windows-targets 0.48.0",
 ]
 
 [[package]]
 name = "windows-targets"
-version = "0.42.1"
+version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8e2522491fbfcd58cc84d47aeb2958948c4b8982e9a2d8a2a35bbaed431390e7"
+checksum = "8e5180c00cd44c9b1c88adb3693291f1cd93605ded80c250a75d472756b4d071"
 dependencies = [
- "windows_aarch64_gnullvm",
- "windows_aarch64_msvc",
- "windows_i686_gnu",
- "windows_i686_msvc",
- "windows_x86_64_gnu",
- "windows_x86_64_gnullvm",
- "windows_x86_64_msvc",
+ "windows_aarch64_gnullvm 0.42.2",
+ "windows_aarch64_msvc 0.42.2",
+ "windows_i686_gnu 0.42.2",
+ "windows_i686_msvc 0.42.2",
+ "windows_x86_64_gnu 0.42.2",
+ "windows_x86_64_gnullvm 0.42.2",
+ "windows_x86_64_msvc 0.42.2",
+]
+
+[[package]]
+name = "windows-targets"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7b1eb6f0cd7c80c79759c929114ef071b87354ce476d9d94271031c0497adfd5"
+dependencies = [
+ "windows_aarch64_gnullvm 0.48.0",
+ "windows_aarch64_msvc 0.48.0",
+ "windows_i686_gnu 0.48.0",
+ "windows_i686_msvc 0.48.0",
+ "windows_x86_64_gnu 0.48.0",
+ "windows_x86_64_gnullvm 0.48.0",
+ "windows_x86_64_msvc 0.48.0",
 ]
 
 [[package]]
 name = "windows_aarch64_gnullvm"
-version = "0.42.1"
+version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8c9864e83243fdec7fc9c5444389dcbbfd258f745e7853198f365e3c4968a608"
+checksum = "597a5118570b68bc08d8d59125332c54f1ba9d9adeedeef5b99b02ba2b0698f8"
+
+[[package]]
+name = "windows_aarch64_gnullvm"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "91ae572e1b79dba883e0d315474df7305d12f569b400fcf90581b06062f7e1bc"
+
+[[package]]
+name = "windows_aarch64_msvc"
+version = "0.42.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e08e8864a60f06ef0d0ff4ba04124db8b0fb3be5776a5cd47641e942e58c4d43"
 
 [[package]]
 name = "windows_aarch64_msvc"
-version = "0.42.1"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b2ef27e0d7bdfcfc7b868b317c1d32c641a6fe4629c171b8928c7b08d98d7cf3"
+
+[[package]]
+name = "windows_i686_gnu"
+version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4c8b1b673ffc16c47a9ff48570a9d85e25d265735c503681332589af6253c6c7"
+checksum = "c61d927d8da41da96a81f029489353e68739737d3beca43145c8afec9a31a84f"
 
 [[package]]
 name = "windows_i686_gnu"
-version = "0.42.1"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "622a1962a7db830d6fd0a69683c80a18fda201879f0f447f065a3b7467daa241"
+
+[[package]]
+name = "windows_i686_msvc"
+version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "de3887528ad530ba7bdbb1faa8275ec7a1155a45ffa57c37993960277145d640"
+checksum = "44d840b6ec649f480a41c8d80f9c65108b92d89345dd94027bfe06ac444d1060"
 
 [[package]]
 name = "windows_i686_msvc"
-version = "0.42.1"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bf4d1122317eddd6ff351aa852118a2418ad4214e6613a50e0191f7004372605"
+checksum = "4542c6e364ce21bf45d69fdd2a8e455fa38d316158cfd43b3ac1c5b1b19f8e00"
 
 [[package]]
 name = "windows_x86_64_gnu"
-version = "0.42.1"
+version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c1040f221285e17ebccbc2591ffdc2d44ee1f9186324dd3e84e99ac68d699c45"
+checksum = "8de912b8b8feb55c064867cf047dda097f92d51efad5b491dfb98f6bbb70cb36"
+
+[[package]]
+name = "windows_x86_64_gnu"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ca2b8a661f7628cbd23440e50b05d705db3686f894fc9580820623656af974b1"
+
+[[package]]
+name = "windows_x86_64_gnullvm"
+version = "0.42.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "26d41b46a36d453748aedef1486d5c7a85db22e56aff34643984ea85514e94a3"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
-version = "0.42.1"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "628bfdf232daa22b0d64fdb62b09fcc36bb01f05a3939e20ab73aaf9470d0463"
+checksum = "7896dbc1f41e08872e9d5e8f8baa8fdd2677f29468c4e156210174edc7f7b953"
 
 [[package]]
 name = "windows_x86_64_msvc"
-version = "0.42.1"
+version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "447660ad36a13288b1db4d4248e857b510e8c3a225c822ba4fb748c0aafecffd"
+checksum = "9aec5da331524158c6d1a4ac0ab1541149c0b9505fde06423b02f5ef0106b9f0"
 
 [[package]]
-name = "wyz"
-version = "0.5.1"
+name = "windows_x86_64_msvc"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "05f360fc0b24296329c78fda852a1e9ae82de9cf7b27dae4b7f62f118f77b9ed"
+checksum = "1a515f5799fe4961cb532f983ce2b23082366b898e52ffbce459c86f67c8378a"
+
+[[package]]
+name = "xz2"
+version = "0.1.7"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "388c44dc09d76f1536602ead6d325eb532f5c122f17782bd57fb47baeeb767e2"
 dependencies = [
- "tap",
+ "lzma-sys",
 ]
 
 [[package]]
+name = "yansi"
+version = "0.5.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "09041cd90cf85f7f8b2df60c646f853b7f535ce68f85244eb6731cf89fa498ec"
+
+[[package]]
 name = "zeroize"
-version = "1.5.7"
+version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c394b5bd0c6f669e7275d9c20aa90ae064cb22e75a1cad54e1b34088034b149f"
+checksum = "2a0956f1ba7c7909bfb66c2e9e4124ab6f6482560f6628b5aaeba39207c9aad9"
```

