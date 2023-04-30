# Comparing `tmp/polars_u64_idx-0.17.8.tar.gz` & `tmp/polars_u64_idx-0.17.9.tar.gz`

## Comparing `polars_u64_idx-0.17.8.tar` & `polars_u64_idx-0.17.9.tar`

### file list

```diff
@@ -1,1113 +1,1114 @@
--rw-r--r--   0        0        0     1431 1970-01-01 00:00:00.000000 polars_u64_idx-0.17.8/local_dependencies/polars-arrow/Cargo.toml
--rw-r--r--   0     1001      123     1055 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-arrow/LICENSE
--rw-r--r--   0     1001      123     1975 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-arrow/src/array/default_arrays.rs
--rw-r--r--   0     1001      123     3160 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-arrow/src/array/get.rs
--rw-r--r--   0     1001      123     6459 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-arrow/src/array/list.rs
--rw-r--r--   0     1001      123     7771 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-arrow/src/array/mod.rs
--rw-r--r--   0     1001      123      878 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-arrow/src/array/null.rs
--rw-r--r--   0     1001      123     1125 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-arrow/src/array/slice.rs
--rw-r--r--   0     1001      123     1807 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-arrow/src/array/utf8.rs
--rw-r--r--   0     1001      123     2294 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-arrow/src/bit_util.rs
--rw-r--r--   0     1001      123       17 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-arrow/src/bitmap/mod.rs
--rw-r--r--   0     1001      123      819 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-arrow/src/bitmap/mutable.rs
--rw-r--r--   0     1001      123      232 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-arrow/src/compute/cast.rs
--rw-r--r--   0     1001      123       56 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-arrow/src/compute/mod.rs
--rw-r--r--   0     1001      123     2962 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-arrow/src/compute/take/boolean.rs
--rw-r--r--   0     1001      123    24907 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-arrow/src/compute/take/mod.rs
--rw-r--r--   0     1001      123     1042 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-arrow/src/conversion.rs
--rw-r--r--   0     1001      123     1609 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-arrow/src/data_types.rs
--rw-r--r--   0     1001      123       25 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-arrow/src/error.rs
--rw-r--r--   0     1001      123       28 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-arrow/src/export.rs
--rw-r--r--   0     1001      123       26 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-arrow/src/floats/mod.rs
--rw-r--r--   0     1001      123     2066 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-arrow/src/floats/ord.rs
--rw-r--r--   0     1001      123     1273 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-arrow/src/index.rs
--rw-r--r--   0     1001      123      915 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-arrow/src/is_valid.rs
--rw-r--r--   0     1001      123     4740 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-arrow/src/kernels/agg_mean.rs
--rw-r--r--   0     1001      123     1015 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-arrow/src/kernels/concatenate.rs
--rw-r--r--   0     1001      123     5161 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-arrow/src/kernels/ewm/average.rs
--rw-r--r--   0     1001      123     1808 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-arrow/src/kernels/ewm/mod.rs
--rw-r--r--   0     1001      123    25065 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-arrow/src/kernels/ewm/variance.rs
--rw-r--r--   0     1001      123     1406 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-arrow/src/kernels/float.rs
--rw-r--r--   0     1001      123     4907 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-arrow/src/kernels/list.rs
--rw-r--r--   0     1001      123     1895 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-arrow/src/kernels/list_bytes_iter.rs
--rw-r--r--   0     1001      123     9731 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-arrow/src/kernels/mod.rs
--rw-r--r--   0     1001      123     3703 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-arrow/src/kernels/rolling/mod.rs
--rw-r--r--   0     1001      123     2022 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/mean.rs
--rw-r--r--   0     1001      123    18684 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/min_max.rs
--rw-r--r--   0     1001      123     3924 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/mod.rs
--rw-r--r--   0     1001      123    11659 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/quantile.rs
--rw-r--r--   0     1001      123     5504 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/sum.rs
--rw-r--r--   0     1001      123     8683 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/variance.rs
--rw-r--r--   0     1001      123     1749 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-arrow/src/kernels/rolling/nulls/mean.rs
--rw-r--r--   0     1001      123    14367 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-arrow/src/kernels/rolling/nulls/min_max.rs
--rw-r--r--   0     1001      123     9070 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-arrow/src/kernels/rolling/nulls/mod.rs
--rw-r--r--   0     1001      123    11609 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-arrow/src/kernels/rolling/nulls/quantile.rs
--rw-r--r--   0     1001      123     4698 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-arrow/src/kernels/rolling/nulls/sum.rs
--rw-r--r--   0     1001      123     8335 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-arrow/src/kernels/rolling/nulls/variance.rs
--rw-r--r--   0     1001      123     8109 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-arrow/src/kernels/rolling/window.rs
--rw-r--r--   0     1001      123     4752 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-arrow/src/kernels/set.rs
--rw-r--r--   0     1001      123     4529 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-arrow/src/kernels/sort_partition.rs
--rw-r--r--   0     1001      123     2948 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-arrow/src/kernels/sorted_join/inner.rs
--rw-r--r--   0     1001      123     5974 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-arrow/src/kernels/sorted_join/left.rs
--rw-r--r--   0     1001      123      231 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-arrow/src/kernels/sorted_join/mod.rs
--rw-r--r--   0     1001      123      841 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-arrow/src/kernels/string.rs
--rw-r--r--   0     1001      123     2310 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-arrow/src/kernels/take_agg/boolean.rs
--rw-r--r--   0     1001      123     4343 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-arrow/src/kernels/take_agg/mod.rs
--rw-r--r--   0     1001      123     2606 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-arrow/src/kernels/take_agg/var.rs
--rw-r--r--   0     1001      123     4417 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-arrow/src/kernels/time.rs
--rw-r--r--   0     1001      123      341 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-arrow/src/lib.rs
--rw-r--r--   0     1001      123      434 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-arrow/src/prelude.rs
--rw-r--r--   0     1001      123      534 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-arrow/src/slice.rs
--rw-r--r--   0     1001      123      762 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-arrow/src/time_zone.rs
--rw-r--r--   0     1001      123      998 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-arrow/src/trusted_len/boolean.rs
--rw-r--r--   0     1001      123     2821 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-arrow/src/trusted_len/mod.rs
--rw-r--r--   0     1001      123     2533 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-arrow/src/trusted_len/push_unchecked.rs
--rw-r--r--   0     1001      123      158 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-arrow/src/trusted_len/rev.rs
--rw-r--r--   0     1001      123     5232 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-arrow/src/utils.rs
--rw-r--r--   0        0        0      994 1970-01-01 00:00:00.000000 polars_u64_idx-0.17.8/local_dependencies/polars-sql/Cargo.toml
--rw-r--r--   0     1001      123     1055 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-sql/LICENSE
--rw-r--r--   0     1001      123    16037 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-sql/src/context.rs
--rw-r--r--   0     1001      123    20245 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-sql/src/functions.rs
--rw-r--r--   0     1001      123     1920 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-sql/src/keywords.rs
--rw-r--r--   0     1001      123      211 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-sql/src/lib.rs
--rw-r--r--   0     1001      123    15240 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-sql/src/sql_expr.rs
--rw-r--r--   0     1001      123     4572 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-sql/src/table_functions.rs
--rw-r--r--   0     1001      123     1682 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-sql/tests/functions_cumulative.rs
--rw-r--r--   0     1001      123     3063 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-sql/tests/functions_io.rs
--rw-r--r--   0     1001      123     1539 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-sql/tests/functions_math.rs
--rw-r--r--   0     1001      123     2982 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-sql/tests/functions_string.rs
--rw-r--r--   0     1001      123     1056 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-sql/tests/iss_7436.rs
--rw-r--r--   0     1001      123      888 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-sql/tests/iss_7437.rs
--rw-r--r--   0     1001      123      652 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-sql/tests/iss_7440.rs
--rw-r--r--   0     1001      123      700 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-sql/tests/iss_8395.rs
--rw-r--r--   0     1001      123     1062 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-sql/tests/iss_8419.rs
--rw-r--r--   0     1001      123    14296 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-sql/tests/simple_exprs.rs
--rw-r--r--   0        0        0     3268 1970-01-01 00:00:00.000000 polars_u64_idx-0.17.8/local_dependencies/polars-ops/Cargo.toml
--rw-r--r--   0     1001      123     1055 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-ops/LICENSE
--rw-r--r--   0     1001      123      234 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-ops/src/chunked_array/binary/mod.rs
--rw-r--r--   0     1001      123     3549 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-ops/src/chunked_array/binary/namespace.rs
--rw-r--r--   0     1001      123    11023 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-ops/src/chunked_array/interpolate.rs
--rw-r--r--   0     1001      123     1679 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-ops/src/chunked_array/list/count.rs
--rw-r--r--   0     1001      123     2452 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-ops/src/chunked_array/list/hash.rs
--rw-r--r--   0     1001      123     7861 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-ops/src/chunked_array/list/min_max.rs
--rw-r--r--   0     1001      123      511 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-ops/src/chunked_array/list/mod.rs
--rw-r--r--   0     1001      123    22005 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-ops/src/chunked_array/list/namespace.rs
--rw-r--r--   0     1001      123     5269 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-ops/src/chunked_array/list/sum_mean.rs
--rw-r--r--   0     1001      123     2435 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-ops/src/chunked_array/list/to_struct.rs
--rw-r--r--   0     1001      123      489 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-ops/src/chunked_array/mod.rs
--rw-r--r--   0     1001      123     9380 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-ops/src/chunked_array/nan_propagating_aggregate.rs
--rw-r--r--   0     1001      123     6795 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-ops/src/chunked_array/set.rs
--rw-r--r--   0     1001      123     7490 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-ops/src/chunked_array/strings/case.rs
--rw-r--r--   0     1001      123     8251 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-ops/src/chunked_array/strings/json_path.rs
--rw-r--r--   0     1001      123     2345 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-ops/src/chunked_array/strings/justify.rs
--rw-r--r--   0     1001      123      514 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-ops/src/chunked_array/strings/mod.rs
--rw-r--r--   0     1001      123    14731 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-ops/src/chunked_array/strings/namespace.rs
--rw-r--r--   0     1001      123     4053 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-ops/src/chunked_array/strings/replace.rs
--rw-r--r--   0     1001      123     2486 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-ops/src/chunked_array/top_k.rs
--rw-r--r--   0     1001      123     7727 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-ops/src/frame/join/merge_sorted.rs
--rw-r--r--   0     1001      123    18025 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-ops/src/frame/join/mod.rs
--rw-r--r--   0     1001      123     4174 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-ops/src/frame/mod.rs
--rw-r--r--   0     1001      123    10257 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-ops/src/frame/pivot/mod.rs
--rw-r--r--   0     1001      123    13486 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-ops/src/frame/pivot/positioning.rs
--rw-r--r--   0     1001      123      217 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-ops/src/lib.rs
--rw-r--r--   0     1001      123      290 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-ops/src/prelude.rs
--rw-r--r--   0     1001      123       25 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-ops/src/series/mod.rs
--rw-r--r--   0     1001      123     9623 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-ops/src/series/ops/approx_algo/hyperloglogplus.rs
--rw-r--r--   0     1001      123      118 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-ops/src/series/ops/approx_algo/mod.rs
--rw-r--r--   0     1001      123     2016 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-ops/src/series/ops/approx_unique.rs
--rw-r--r--   0     1001      123    11872 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-ops/src/series/ops/arg_min_max.rs
--rw-r--r--   0     1001      123     3688 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-ops/src/series/ops/floor_divide.rs
--rw-r--r--   0     1001      123     3423 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-ops/src/series/ops/is_first.rs
--rw-r--r--   0     1001      123     2975 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-ops/src/series/ops/is_unique.rs
--rw-r--r--   0     1001      123     3626 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-ops/src/series/ops/log.rs
--rw-r--r--   0     1001      123     1106 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-ops/src/series/ops/mod.rs
--rw-r--r--   0     1001      123     1769 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-ops/src/series/ops/rolling.rs
--rw-r--r--   0     1001      123     7642 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-ops/src/series/ops/search_sorted.rs
--rw-r--r--   0     1001      123     2500 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-ops/src/series/ops/to_dummies.rs
--rw-r--r--   0     1001      123     2067 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-ops/src/series/ops/various.rs
--rw-r--r--   0        0        0      879 1970-01-01 00:00:00.000000 polars_u64_idx-0.17.8/local_dependencies/polars-error/Cargo.toml
--rw-r--r--   0     1001      123     1055 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-error/LICENSE
--rw-r--r--   0     1001      123     6297 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-error/src/lib.rs
--rw-r--r--   0        0        0     4343 1970-01-01 00:00:00.000000 polars_u64_idx-0.17.8/local_dependencies/polars-io/Cargo.toml
--rw-r--r--   0     1001      123     1055 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-io/LICENSE
--rw-r--r--   0     1001      123     2383 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-io/src/avro/mod.rs
--rw-r--r--   0     1001      123     3608 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-io/src/avro/read.rs
--rw-r--r--   0     1001      123     2622 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-io/src/avro/write.rs
--rw-r--r--   0     1001      123     4505 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-io/src/cloud/adaptors.rs
--rw-r--r--   0     1001      123     9506 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-io/src/cloud/glob.rs
--rw-r--r--   0     1001      123     3089 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-io/src/cloud/mod.rs
--rw-r--r--   0     1001      123    28678 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-io/src/csv/buffer.rs
--rw-r--r--   0     1001      123     1898 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-io/src/csv/mod.rs
--rw-r--r--   0     1001      123    19712 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-io/src/csv/parser.rs
--rw-r--r--   0     1001      123    21432 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-io/src/csv/read.rs
--rw-r--r--   0     1001      123    10817 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-io/src/csv/read_impl/batched_mmap.rs
--rw-r--r--   0     1001      123    13909 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-io/src/csv/read_impl/batched_read.rs
--rw-r--r--   0     1001      123    31242 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-io/src/csv/read_impl/mod.rs
--rw-r--r--   0     1001      123    11466 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-io/src/csv/splitfields.rs
--rw-r--r--   0     1001      123    25183 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-io/src/csv/utils.rs
--rw-r--r--   0     1001      123     2796 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-io/src/csv/write.rs
--rw-r--r--   0     1001      123    13265 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-io/src/csv/write_impl.rs
--rw-r--r--   0     1001      123      184 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-io/src/export.rs
--rw-r--r--   0     1001      123     7586 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-io/src/ipc/ipc_file.rs
--rw-r--r--   0     1001      123     9222 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-io/src/ipc/ipc_stream.rs
--rw-r--r--   0     1001      123     3253 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-io/src/ipc/mmap.rs
--rw-r--r--   0     1001      123      401 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-io/src/ipc/mod.rs
--rw-r--r--   0     1001      123     8282 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-io/src/ipc/write.rs
--rw-r--r--   0     1001      123     1471 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-io/src/ipc/write_async.rs
--rw-r--r--   0     1001      123    11046 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-io/src/json.rs
--rw-r--r--   0     1001      123     4864 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-io/src/lib.rs
--rw-r--r--   0     1001      123     1969 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-io/src/mmap.rs
--rw-r--r--   0     1001      123     7215 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-io/src/ndjson_core/buffer.rs
--rw-r--r--   0     1001      123       39 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-io/src/ndjson_core/mod.rs
--rw-r--r--   0     1001      123    12172 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-io/src/ndjson_core/ndjson.rs
--rw-r--r--   0     1001      123      273 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-io/src/options.rs
--rw-r--r--   0     1001      123     7360 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-io/src/parquet/async_impl.rs
--rw-r--r--   0     1001      123     3093 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-io/src/parquet/mmap.rs
--rw-r--r--   0     1001      123     3132 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-io/src/parquet/mod.rs
--rw-r--r--   0     1001      123     4784 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-io/src/parquet/predicates.rs
--rw-r--r--   0     1001      123     9606 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-io/src/parquet/read.rs
--rw-r--r--   0     1001      123    16886 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-io/src/parquet/read_impl.rs
--rw-r--r--   0     1001      123    10106 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-io/src/parquet/write.rs
--rw-r--r--   0     1001      123     5334 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-io/src/partition.rs
--rw-r--r--   0     1001      123     1455 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-io/src/predicates.rs
--rw-r--r--   0     1001      123      628 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-io/src/prelude.rs
--rw-r--r--   0     1001      123      417 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-io/src/tests.rs
--rw-r--r--   0     1001      123     4467 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-io/src/utils.rs
--rw-r--r--   0        0        0     1765 1970-01-01 00:00:00.000000 polars_u64_idx-0.17.8/local_dependencies/polars-pipe/Cargo.toml
--rw-r--r--   0     1001      123     1055 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-pipe/LICENSE
--rw-r--r--   0     1001      123       98 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-pipe/src/executors/mod.rs
--rw-r--r--   0     1001      123     1219 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-pipe/src/executors/operators/filter.rs
--rw-r--r--   0     1001      123     4103 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-pipe/src/executors/operators/function.rs
--rw-r--r--   0     1001      123      229 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-pipe/src/executors/operators/mod.rs
--rw-r--r--   0     1001      123      548 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-pipe/src/executors/operators/placeholder.rs
--rw-r--r--   0     1001      123     3247 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-pipe/src/executors/operators/projection.rs
--rw-r--r--   0     1001      123     2324 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-pipe/src/executors/operators/reproject.rs
--rw-r--r--   0     1001      123     6479 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-pipe/src/executors/sinks/file_sink.rs
--rw-r--r--   0     1001      123    10473 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/convert.rs
--rw-r--r--   0     1001      123     1207 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/count.rs
--rw-r--r--   0     1001      123     1888 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/first.rs
--rw-r--r--   0     1001      123     4554 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/interface.rs
--rw-r--r--   0     1001      123     1746 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/last.rs
--rw-r--r--   0     1001      123     5413 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/mean.rs
--rw-r--r--   0     1001      123     4951 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/min_max.rs
--rw-r--r--   0     1001      123      211 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/mod.rs
--rw-r--r--   0     1001      123      856 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/null.rs
--rw-r--r--   0     1001      123     4294 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/sum.rs
--rw-r--r--   0     1001      123     3030 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/eval.rs
--rw-r--r--   0     1001      123     6275 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/global.rs
--rw-r--r--   0     1001      123    13665 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/hash_table.rs
--rw-r--r--   0     1001      123     2681 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/mod.rs
--rw-r--r--   0     1001      123     2534 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/ooc_state.rs
--rw-r--r--   0     1001      123     5961 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/sink.rs
--rw-r--r--   0     1001      123    10673 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/thread_local.rs
--rw-r--r--   0     1001      123     2164 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-pipe/src/executors/sinks/groupby/mod.rs
--rw-r--r--   0     1001      123     4666 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-pipe/src/executors/sinks/groupby/ooc.rs
--rw-r--r--   0     1001      123     3906 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-pipe/src/executors/sinks/groupby/ooc_state.rs
--rw-r--r--   0     1001      123    20859 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-pipe/src/executors/sinks/groupby/primitive/mod.rs
--rw-r--r--   0     1001      123    23518 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-pipe/src/executors/sinks/groupby/string.rs
--rw-r--r--   0     1001      123     2457 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-pipe/src/executors/sinks/groupby/utils.rs
--rw-r--r--   0     1001      123     8395 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-pipe/src/executors/sinks/io.rs
--rw-r--r--   0     1001      123     5485 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-pipe/src/executors/sinks/joins/cross.rs
--rw-r--r--   0     1001      123    14279 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-pipe/src/executors/sinks/joins/generic_build.rs
--rw-r--r--   0     1001      123    11824 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-pipe/src/executors/sinks/joins/inner_left.rs
--rw-r--r--   0     1001      123      178 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-pipe/src/executors/sinks/joins/mod.rs
--rw-r--r--   0     1001      123     2002 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-pipe/src/executors/sinks/memory.rs
--rw-r--r--   0     1001      123      589 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-pipe/src/executors/sinks/mod.rs
--rw-r--r--   0     1001      123     1492 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-pipe/src/executors/sinks/ordered.rs
--rw-r--r--   0     1001      123     1824 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-pipe/src/executors/sinks/reproject.rs
--rw-r--r--   0     1001      123     3108 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-pipe/src/executors/sinks/slice.rs
--rw-r--r--   0     1001      123      130 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-pipe/src/executors/sinks/sort/mod.rs
--rw-r--r--   0     1001      123     3808 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-pipe/src/executors/sinks/sort/ooc.rs
--rw-r--r--   0     1001      123     6295 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-pipe/src/executors/sinks/sort/sink.rs
--rw-r--r--   0     1001      123     5953 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-pipe/src/executors/sinks/sort/sink_multiple.rs
--rw-r--r--   0     1001      123     3801 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-pipe/src/executors/sinks/sort/source.rs
--rw-r--r--   0     1001      123      635 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-pipe/src/executors/sinks/utils.rs
--rw-r--r--   0     1001      123     5076 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-pipe/src/executors/sources/csv.rs
--rw-r--r--   0     1001      123     1231 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-pipe/src/executors/sources/frame.rs
--rw-r--r--   0     1001      123      987 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-pipe/src/executors/sources/ipc_one_shot.rs
--rw-r--r--   0     1001      123      366 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-pipe/src/executors/sources/mod.rs
--rw-r--r--   0     1001      123     3387 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-pipe/src/executors/sources/parquet.rs
--rw-r--r--   0     1001      123     1146 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-pipe/src/executors/sources/reproject.rs
--rw-r--r--   0     1001      123     1022 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-pipe/src/executors/sources/union.rs
--rw-r--r--   0     1001      123      448 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-pipe/src/expressions.rs
--rw-r--r--   0     1001      123      272 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-pipe/src/lib.rs
--rw-r--r--   0     1001      123      719 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-pipe/src/operators/chunks.rs
--rw-r--r--   0     1001      123      474 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-pipe/src/operators/context.rs
--rw-r--r--   0     1001      123      223 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-pipe/src/operators/mod.rs
--rw-r--r--   0     1001      123      430 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-pipe/src/operators/operator.rs
--rw-r--r--   0     1001      123      626 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-pipe/src/operators/sink.rs
--rw-r--r--   0     1001      123      241 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-pipe/src/operators/source.rs
--rw-r--r--   0     1001      123        1 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-pipe/src/pipeline/config.rs
--rw-r--r--   0     1001      123    20481 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-pipe/src/pipeline/convert.rs
--rw-r--r--   0     1001      123    13982 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-pipe/src/pipeline/dispatcher.rs
--rw-r--r--   0     1001      123     1237 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-pipe/src/pipeline/mod.rs
--rw-r--r--   0        0        0     5450 1970-01-01 00:00:00.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/Cargo.toml
--rw-r--r--   0     1001      123     1055 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/LICENSE
--rw-r--r--   0     1001      123    19606 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/arithmetic.rs
--rw-r--r--   0     1001      123     8699 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/bitwise.rs
--rw-r--r--   0     1001      123     2298 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/builder/binary.rs
--rw-r--r--   0     1001      123     1207 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/builder/boolean.rs
--rw-r--r--   0     1001      123     1556 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/builder/from.rs
--rw-r--r--   0     1001      123    20366 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/builder/list.rs
--rw-r--r--   0     1001      123     8845 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/builder/mod.rs
--rw-r--r--   0     1001      123     1410 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/builder/primitive.rs
--rw-r--r--   0     1001      123     2291 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/builder/utf8.rs
--rw-r--r--   0     1001      123    11560 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/cast.rs
--rw-r--r--   0     1001      123    48300 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/comparison/mod.rs
--rw-r--r--   0     1001      123     9463 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/comparison/scalar.rs
--rw-r--r--   0     1001      123      551 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/drop.rs
--rw-r--r--   0     1001      123      963 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/float.rs
--rw-r--r--   0     1001      123     5069 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/from.rs
--rw-r--r--   0     1001      123    38411 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/iterator/mod.rs
--rw-r--r--   0     1001      123     1395 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/iterator/par/list.rs
--rw-r--r--   0     1001      123       28 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/iterator/par/mod.rs
--rw-r--r--   0     1001      123     1129 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/iterator/par/utf8.rs
--rw-r--r--   0     1001      123       21 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/kernels/mod.rs
--rw-r--r--   0     1001      123     2986 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/kernels/take.rs
--rw-r--r--   0     1001      123     7728 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/list/iterator.rs
--rw-r--r--   0     1001      123     2802 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/list/mod.rs
--rw-r--r--   0     1001      123    19796 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/logical/categorical/builder.rs
--rw-r--r--   0     1001      123     3688 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/logical/categorical/from.rs
--rw-r--r--   0     1001      123     4270 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/logical/categorical/merge.rs
--rw-r--r--   0     1001      123    10220 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/logical/categorical/mod.rs
--rw-r--r--   0     1001      123     1400 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/append.rs
--rw-r--r--   0     1001      123      358 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/full.rs
--rw-r--r--   0     1001      123      192 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/mod.rs
--rw-r--r--   0     1001      123     2731 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/take_random.rs
--rw-r--r--   0     1001      123     2172 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/unique.rs
--rw-r--r--   0     1001      123      925 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/zip.rs
--rw-r--r--   0     1001      123     6453 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/logical/categorical/stringcache.rs
--rw-r--r--   0     1001      123     1604 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/logical/date.rs
--rw-r--r--   0     1001      123     4105 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/logical/datetime.rs
--rw-r--r--   0     1001      123     4443 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/logical/decimal.rs
--rw-r--r--   0     1001      123     2434 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/logical/duration.rs
--rw-r--r--   0     1001      123     2549 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/logical/mod.rs
--rw-r--r--   0     1001      123      476 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/logical/struct_/from.rs
--rw-r--r--   0     1001      123    15081 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/logical/struct_/mod.rs
--rw-r--r--   0     1001      123     1182 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/logical/time.rs
--rw-r--r--   0     1001      123    23524 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/mod.rs
--rw-r--r--   0     1001      123     7200 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/ndarray.rs
--rw-r--r--   0     1001      123     4484 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/object/builder.rs
--rw-r--r--   0     1001      123     1547 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/object/extension/drop.rs
--rw-r--r--   0     1001      123     3124 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/object/extension/list.rs
--rw-r--r--   0     1001      123     7054 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/object/extension/mod.rs
--rw-r--r--   0     1001      123     3410 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/object/extension/polars_extension.rs
--rw-r--r--   0     1001      123      137 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/object/is_valid.rs
--rw-r--r--   0     1001      123     4419 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/object/iterator.rs
--rw-r--r--   0     1001      123     4826 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/object/mod.rs
--rw-r--r--   0     1001      123     2853 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/object/registry.rs
--rw-r--r--   0     1001      123      272 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/ops/abs.rs
--rw-r--r--   0     1001      123    32120 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/ops/aggregate/mod.rs
--rw-r--r--   0     1001      123     9946 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/ops/aggregate/quantile.rs
--rw-r--r--   0     1001      123     2875 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/ops/aggregate/var.rs
--rw-r--r--   0     1001      123     9670 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/ops/any_value.rs
--rw-r--r--   0     1001      123     2365 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/ops/append.rs
--rw-r--r--   0     1001      123    27269 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/ops/apply.rs
--rw-r--r--   0     1001      123    12799 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/ops/bit_repr.rs
--rw-r--r--   0     1001      123     6214 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/ops/chunkops.rs
--rw-r--r--   0     1001      123    11537 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/ops/compare_inner.rs
--rw-r--r--   0     1001      123     1737 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/ops/concat_str.rs
--rw-r--r--   0     1001      123     4801 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/ops/cum_agg.rs
--rw-r--r--   0     1001      123     6264 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/ops/downcast.rs
--rw-r--r--   0     1001      123    25614 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/ops/explode.rs
--rw-r--r--   0     1001      123     8339 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/ops/extend.rs
--rw-r--r--   0     1001      123    13777 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/ops/fill_null.rs
--rw-r--r--   0     1001      123     5308 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/ops/filter.rs
--rw-r--r--   0     1001      123     4436 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/ops/full.rs
--rw-r--r--   0     1001      123        1 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/ops/interpolate.rs
--rw-r--r--   0     1001      123    15385 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/ops/is_in.rs
--rw-r--r--   0     1001      123        1 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/ops/len.rs
--rw-r--r--   0     1001      123     2658 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/ops/min_max_binary.rs
--rw-r--r--   0     1001      123    22407 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/ops/mod.rs
--rw-r--r--   0     1001      123     2403 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/ops/nulls.rs
--rw-r--r--   0     1001      123      593 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/ops/peaks.rs
--rw-r--r--   0     1001      123     2585 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/ops/repeat_by.rs
--rw-r--r--   0     1001      123     1539 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/ops/reverse.rs
--rw-r--r--   0     1001      123    10234 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/ops/rolling_window.rs
--rw-r--r--   0     1001      123    12518 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/ops/set.rs
--rw-r--r--   0     1001      123     6151 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/ops/shift.rs
--rw-r--r--   0     1001      123     2299 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/ops/sort/arg_sort.rs
--rw-r--r--   0     1001      123     5467 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/ops/sort/arg_sort_multiple.rs
--rw-r--r--   0     1001      123     7430 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/ops/sort/categorical.rs
--rw-r--r--   0     1001      123    30762 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/ops/sort/mod.rs
--rw-r--r--   0     1001      123      380 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/ops/sort/slice.rs
--rw-r--r--   0     1001      123    20472 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/ops/take/mod.rs
--rw-r--r--   0     1001      123     6630 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/ops/take/take_chunked.rs
--rw-r--r--   0     1001      123     1859 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/ops/take/take_every.rs
--rw-r--r--   0     1001      123    16256 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/ops/take/take_random.rs
--rw-r--r--   0     1001      123     5041 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/ops/take/take_single.rs
--rw-r--r--   0     1001      123     6064 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/ops/take/traits.rs
--rw-r--r--   0     1001      123    11229 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/ops/unique/mod.rs
--rw-r--r--   0     1001      123    14620 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/ops/unique/rank.rs
--rw-r--r--   0     1001      123     7753 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/ops/zip.rs
--rw-r--r--   0     1001      123     9093 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/random.rs
--rw-r--r--   0     1001      123     1959 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/temporal/conversion.rs
--rw-r--r--   0     1001      123     2501 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/temporal/date.rs
--rw-r--r--   0     1001      123    11998 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/temporal/datetime.rs
--rw-r--r--   0     1001      123     3201 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/temporal/duration.rs
--rw-r--r--   0     1001      123      533 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/temporal/mod.rs
--rw-r--r--   0     1001      123     2724 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/temporal/time.rs
--rw-r--r--   0     1001      123      872 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/to_vec.rs
--rw-r--r--   0     1001      123     8113 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/trusted_len.rs
--rw-r--r--   0     1001      123    25182 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/upstream_traits.rs
--rw-r--r--   0     1001      123     7689 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/cloud.rs
--rw-r--r--   0     1001      123     1549 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/config.rs
--rw-r--r--   0     1001      123     3946 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/datatypes/_serde.rs
--rw-r--r--   0     1001      123     2650 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/datatypes/aliases.rs
--rw-r--r--   0     1001      123    42410 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/datatypes/any_value.rs
--rw-r--r--   0     1001      123    12083 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/datatypes/dtype.rs
--rw-r--r--   0     1001      123     5456 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/datatypes/field.rs
--rw-r--r--   0     1001      123     7675 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/datatypes/mod.rs
--rw-r--r--   0     1001      123     2016 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/datatypes/time_unit.rs
--rw-r--r--   0     1001      123      118 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/doc/changelog/mod.rs
--rw-r--r--   0     1001      123      898 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/doc/changelog/v0_10_0_11.rs
--rw-r--r--   0     1001      123      481 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/doc/changelog/v0_3.rs
--rw-r--r--   0     1001      123      293 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/doc/changelog/v0_4.rs
--rw-r--r--   0     1001      123      499 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/doc/changelog/v0_5.rs
--rw-r--r--   0     1001      123      288 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/doc/changelog/v0_6.rs
--rw-r--r--   0     1001      123     1071 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/doc/changelog/v0_7.rs
--rw-r--r--   0     1001      123      819 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/doc/changelog/v0_8.rs
--rw-r--r--   0     1001      123      596 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/doc/changelog/v0_9.rs
--rw-r--r--   0     1001      123       43 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/doc/mod.rs
--rw-r--r--   0     1001      123       25 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/error.rs
--rw-r--r--   0     1001      123      433 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/export.rs
--rw-r--r--   0     1001      123    36116 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/fmt.rs
--rw-r--r--   0     1001      123     5177 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/frame/arithmetic.rs
--rw-r--r--   0     1001      123     7874 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/frame/asof_join/asof.rs
--rw-r--r--   0     1001      123    33715 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/frame/asof_join/groups.rs
--rw-r--r--   0     1001      123     6634 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/frame/asof_join/mod.rs
--rw-r--r--   0     1001      123      559 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/frame/chunks.rs
--rw-r--r--   0     1001      123     5179 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/frame/cross_join.rs
--rw-r--r--   0     1001      123    16609 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/frame/explode.rs
--rw-r--r--   0     1001      123     1019 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/frame/from.rs
--rw-r--r--   0     1001      123    16518 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/frame/groupby/aggregations/agg_list.rs
--rw-r--r--   0     1001      123     4115 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/frame/groupby/aggregations/boolean.rs
--rw-r--r--   0     1001      123     7643 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/frame/groupby/aggregations/dispatch.rs
--rw-r--r--   0     1001      123    39255 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/frame/groupby/aggregations/mod.rs
--rw-r--r--   0     1001      123     5636 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/frame/groupby/aggregations/utf8.rs
--rw-r--r--   0     1001      123      218 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/frame/groupby/expr.rs
--rw-r--r--   0     1001      123    19976 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/frame/groupby/hashing.rs
--rw-r--r--   0     1001      123    14075 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/frame/groupby/into_groups.rs
--rw-r--r--   0     1001      123    39375 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/frame/groupby/mod.rs
--rw-r--r--   0     1001      123    10593 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/frame/groupby/perfect.rs
--rw-r--r--   0     1001      123    18842 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/frame/groupby/proxy.rs
--rw-r--r--   0     1001      123    18264 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/frame/hash_join/mod.rs
--rw-r--r--   0     1001      123    22392 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/frame/hash_join/multiple_keys.rs
--rw-r--r--   0     1001      123     2413 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/frame/hash_join/single_keys.rs
--rw-r--r--   0     1001      123    16352 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/frame/hash_join/single_keys_dispatch.rs
--rw-r--r--   0     1001      123     4295 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/frame/hash_join/single_keys_inner.rs
--rw-r--r--   0     1001      123     6076 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/frame/hash_join/single_keys_left.rs
--rw-r--r--   0     1001      123     4247 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/frame/hash_join/single_keys_outer.rs
--rw-r--r--   0     1001      123     3913 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/frame/hash_join/single_keys_semi_anti.rs
--rw-r--r--   0     1001      123    11884 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/frame/hash_join/sort_merge.rs
--rw-r--r--   0     1001      123   124136 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/frame/mod.rs
--rw-r--r--   0     1001      123    27513 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/frame/row/av_buffer.rs
--rw-r--r--   0     1001      123     3732 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/frame/row/dataframe.rs
--rw-r--r--   0     1001      123     5976 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/frame/row/mod.rs
--rw-r--r--   0     1001      123     8795 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/frame/row/transpose.rs
--rw-r--r--   0     1001      123     2183 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/frame/top_k.rs
--rw-r--r--   0     1001      123     1388 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/frame/upstream_traits.rs
--rw-r--r--   0     1001      123    10935 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/functions.rs
--rw-r--r--   0     1001      123     2149 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/hashing/fx.rs
--rw-r--r--   0     1001      123     1503 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/hashing/identity.rs
--rw-r--r--   0     1001      123      457 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/hashing/mod.rs
--rw-r--r--   0     1001      123     2684 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/hashing/partition.rs
--rw-r--r--   0     1001      123    17653 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/hashing/vector_hasher.rs
--rw-r--r--   0     1001      123     1896 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/lib.rs
--rw-r--r--   0     1001      123    15733 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/named_from.rs
--rw-r--r--   0     1001      123     2411 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/prelude.rs
--rw-r--r--   0     1001      123    16652 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/schema.rs
--rw-r--r--   0     1001      123     4218 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/serde/chunked_array.rs
--rw-r--r--   0     1001      123     6551 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/serde/mod.rs
--rw-r--r--   0     1001      123     9929 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/serde/series.rs
--rw-r--r--   0     1001      123    18441 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/series/any_value.rs
--rw-r--r--   0     1001      123    28511 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/series/arithmetic/borrowed.rs
--rw-r--r--   0     1001      123      222 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/series/arithmetic/mod.rs
--rw-r--r--   0     1001      123     3546 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/series/arithmetic/owned.rs
--rw-r--r--   0     1001      123    13187 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/series/comparison.rs
--rw-r--r--   0     1001      123    25008 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/series/from.rs
--rw-r--r--   0     1001      123     9217 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/series/implementations/binary.rs
--rw-r--r--   0     1001      123    10850 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/series/implementations/boolean.rs
--rw-r--r--   0     1001      123    12962 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/series/implementations/categorical.rs
--rw-r--r--   0     1001      123    18304 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/series/implementations/dates_time.rs
--rw-r--r--   0     1001      123    15242 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/series/implementations/datetime.rs
--rw-r--r--   0     1001      123     5829 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/series/implementations/decimal.rs
--rw-r--r--   0     1001      123    15106 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/series/implementations/duration.rs
--rw-r--r--   0     1001      123    14223 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/series/implementations/floats.rs
--rw-r--r--   0     1001      123     6207 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/series/implementations/list.rs
--rw-r--r--   0     1001      123    18305 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/series/implementations/mod.rs
--rw-r--r--   0     1001      123     5336 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/series/implementations/null.rs
--rw-r--r--   0     1001      123     8004 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/series/implementations/object.rs
--rw-r--r--   0     1001      123    11029 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/series/implementations/struct_.rs
--rw-r--r--   0     1001      123     9735 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/series/implementations/utf8.rs
--rw-r--r--   0     1001      123     4471 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/series/into.rs
--rw-r--r--   0     1001      123     6297 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/series/iterator.rs
--rw-r--r--   0     1001      123    37684 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/series/mod.rs
--rw-r--r--   0     1001      123      853 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/series/ops/diff.rs
--rw-r--r--   0     1001      123     5204 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/series/ops/downcast.rs
--rw-r--r--   0     1001      123     3601 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/series/ops/ewm.rs
--rw-r--r--   0     1001      123      413 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/series/ops/extend.rs
--rw-r--r--   0     1001      123      562 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/series/ops/mod.rs
--rw-r--r--   0     1001      123     5974 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/series/ops/moment.rs
--rw-r--r--   0     1001      123     2908 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/series/ops/null.rs
--rw-r--r--   0     1001      123     1347 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/series/ops/pct_change.rs
--rw-r--r--   0     1001      123     4247 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/series/ops/round.rs
--rw-r--r--   0     1001      123     5072 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/series/ops/to_list.rs
--rw-r--r--   0     1001      123     1476 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/series/ops/unique.rs
--rw-r--r--   0     1001      123    18204 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/series/series_trait.rs
--rw-r--r--   0     1001      123     2840 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/series/unstable.rs
--rw-r--r--   0     1001      123     8117 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/testing.rs
--rw-r--r--   0     1001      123      508 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/tests.rs
--rw-r--r--   0     1001      123     2494 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/utils/flatten.rs
--rw-r--r--   0     1001      123    31704 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/utils/mod.rs
--rw-r--r--   0     1001      123     1598 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/utils/series.rs
--rw-r--r--   0     1001      123    13773 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-core/src/utils/supertype.rs
--rw-r--r--   0        0        0      476 1970-01-01 00:00:00.000000 polars_u64_idx-0.17.8/local_dependencies/polars-utils/Cargo.toml
--rw-r--r--   0     1001      123     1055 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-utils/LICENSE
--rw-r--r--   0     1001      123     2645 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-utils/src/arena.rs
--rw-r--r--   0     1001      123     1373 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-utils/src/atomic.rs
--rw-r--r--   0     1001      123     2659 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-utils/src/cell.rs
--rw-r--r--   0     1001      123     1015 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-utils/src/contention_pool.rs
--rw-r--r--   0     1001      123      509 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-utils/src/error.rs
--rw-r--r--   0     1001      123      271 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-utils/src/fmt.rs
--rw-r--r--   0     1001      123      763 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-utils/src/functions.rs
--rw-r--r--   0     1001      123      514 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-utils/src/hash.rs
--rw-r--r--   0     1001      123     2709 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-utils/src/iter/enumerate_idx.rs
--rw-r--r--   0     1001      123       61 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-utils/src/iter/mod.rs
--rw-r--r--   0     1001      123      583 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-utils/src/lib.rs
--rw-r--r--   0     1001      123      573 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-utils/src/macros.rs
--rw-r--r--   0     1001      123      282 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-utils/src/mem.rs
--rw-r--r--   0     1001      123     1792 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-utils/src/slice.rs
--rw-r--r--   0     1001      123     2467 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-utils/src/sort.rs
--rw-r--r--   0     1001      123     1115 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-utils/src/sync.rs
--rw-r--r--   0     1001      123      504 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-utils/src/sys.rs
--rw-r--r--   0     1001      123      697 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-utils/src/unwrap.rs
--rw-r--r--   0     1001      123      616 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-utils/src/wasm.rs
--rw-r--r--   0        0        0     5241 1970-01-01 00:00:00.000000 polars_u64_idx-0.17.8/local_dependencies/polars-plan/Cargo.toml
--rw-r--r--   0     1001      123     1055 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-plan/LICENSE
--rw-r--r--   0     1001      123       45 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/constants.rs
--rw-r--r--   0     1001      123    17248 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/dot.rs
--rw-r--r--   0     1001      123     4171 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/dsl/arithmetic.rs
--rw-r--r--   0     1001      123      935 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/dsl/binary.rs
--rw-r--r--   0     1001      123      650 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/dsl/cat.rs
--rw-r--r--   0     1001      123     9880 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/dsl/dt.rs
--rw-r--r--   0     1001      123    13169 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/dsl/expr.rs
--rw-r--r--   0     1001      123      753 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/dsl/from.rs
--rw-r--r--   0     1001      123       85 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/dsl/function_expr/abs.rs
--rw-r--r--   0     1001      123     1431 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/dsl/function_expr/arg_where.rs
--rw-r--r--   0     1001      123     1327 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/dsl/function_expr/binary.rs
--rw-r--r--   0     1001      123     4221 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/dsl/function_expr/boolean.rs
--rw-r--r--   0     1001      123     1910 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/dsl/function_expr/bounds.rs
--rw-r--r--   0     1001      123     1216 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/dsl/function_expr/cat.rs
--rw-r--r--   0     1001      123      344 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/dsl/function_expr/clip.rs
--rw-r--r--   0     1001      123     1593 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/dsl/function_expr/cum.rs
--rw-r--r--   0     1001      123    15231 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/dsl/function_expr/datetime.rs
--rw-r--r--   0     1001      123      810 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/dsl/function_expr/dispatch.rs
--rw-r--r--   0     1001      123     2541 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/dsl/function_expr/fill_null.rs
--rw-r--r--   0     1001      123     8119 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/dsl/function_expr/list.rs
--rw-r--r--   0     1001      123      581 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/dsl/function_expr/log.rs
--rw-r--r--   0     1001      123    19416 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/dsl/function_expr/mod.rs
--rw-r--r--   0     1001      123      462 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/dsl/function_expr/nan.rs
--rw-r--r--   0     1001      123     3132 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/dsl/function_expr/pow.rs
--rw-r--r--   0     1001      123      152 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/dsl/function_expr/rolling.rs
--rw-r--r--   0     1001      123      260 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/dsl/function_expr/round.rs
--rw-r--r--   0     1001      123      200 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/dsl/function_expr/row_hash.rs
--rw-r--r--   0     1001      123    13668 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/dsl/function_expr/schema.rs
--rw-r--r--   0     1001      123      306 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/dsl/function_expr/search_sorted.rs
--rw-r--r--   0     1001      123     3812 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/dsl/function_expr/shift_and_fill.rs
--rw-r--r--   0     1001      123     1238 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/dsl/function_expr/shrink_type.rs
--rw-r--r--   0     1001      123      972 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/dsl/function_expr/sign.rs
--rw-r--r--   0     1001      123    19923 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/dsl/function_expr/strings.rs
--rw-r--r--   0     1001      123     1017 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/dsl/function_expr/struct_.rs
--rw-r--r--   0     1001      123     2700 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/dsl/function_expr/temporal.rs
--rw-r--r--   0     1001      123     5122 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/dsl/function_expr/trigonometry.rs
--rw-r--r--   0     1001      123      170 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/dsl/function_expr/unique.rs
--rw-r--r--   0     1001      123    43864 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/dsl/functions.rs
--rw-r--r--   0     1001      123    10196 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/dsl/list.rs
--rw-r--r--   0     1001      123     2181 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/dsl/meta.rs
--rw-r--r--   0     1001      123    64804 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/dsl/mod.rs
--rw-r--r--   0     1001      123       40 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/dsl/names.rs
--rw-r--r--   0     1001      123     2100 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/dsl/options.rs
--rw-r--r--   0     1001      123    15238 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/dsl/string.rs
--rw-r--r--   0     1001      123     2715 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/dsl/struct_.rs
--rw-r--r--   0     1001      123       38 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/frame/mod.rs
--rw-r--r--   0     1001      123      933 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/frame/opt_state.rs
--rw-r--r--   0     1001      123      466 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/global.rs
--rw-r--r--   0     1001      123      175 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/lib.rs
--rw-r--r--   0     1001      123     6825 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/logical_plan/aexpr/mod.rs
--rw-r--r--   0     1001      123    11393 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/logical_plan/aexpr/schema.rs
--rw-r--r--   0     1001      123    25656 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/logical_plan/alp.rs
--rw-r--r--   0     1001      123     1622 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/logical_plan/anonymous_scan.rs
--rw-r--r--   0     1001      123     1428 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/logical_plan/apply.rs
--rw-r--r--   0     1001      123    24898 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/logical_plan/builder.rs
--rw-r--r--   0     1001      123    29652 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/logical_plan/conversion.rs
--rw-r--r--   0     1001      123      301 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/logical_plan/debug.rs
--rw-r--r--   0     1001      123    15191 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/logical_plan/format.rs
--rw-r--r--   0     1001      123      895 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/logical_plan/functions/drop.rs
--rw-r--r--   0     1001      123      137 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/logical_plan/functions/explode.rs
--rw-r--r--   0     1001      123     1169 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/logical_plan/functions/merge_sorted.rs
--rw-r--r--   0     1001      123    11905 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/logical_plan/functions/mod.rs
--rw-r--r--   0     1001      123     1330 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/logical_plan/functions/rename.rs
--rw-r--r--   0     1001      123     9752 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/logical_plan/iterator.rs
--rw-r--r--   0     1001      123    10463 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/logical_plan/lit.rs
--rw-r--r--   0     1001      123     8115 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/logical_plan/mod.rs
--rw-r--r--   0     1001      123     7416 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/logical_plan/optimizer/cache_states.rs
--rw-r--r--   0     1001      123    15277 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/logical_plan/optimizer/cse.rs
--rw-r--r--   0     1001      123     3250 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/logical_plan/optimizer/delay_rechunk.rs
--rw-r--r--   0     1001      123     3236 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/logical_plan/optimizer/drop_nulls.rs
--rw-r--r--   0     1001      123     3994 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/logical_plan/optimizer/fast_projection.rs
--rw-r--r--   0     1001      123    14479 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/logical_plan/optimizer/file_caching.rs
--rw-r--r--   0     1001      123     1556 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/logical_plan/optimizer/flatten_union.rs
--rw-r--r--   0     1001      123     6644 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/logical_plan/optimizer/mod.rs
--rw-r--r--   0     1001      123     1222 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/logical_plan/optimizer/predicate_pushdown/keys.rs
--rw-r--r--   0     1001      123    28276 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/logical_plan/optimizer/predicate_pushdown/mod.rs
--rw-r--r--   0     1001      123     2571 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/logical_plan/optimizer/predicate_pushdown/rename.rs
--rw-r--r--   0     1001      123    15130 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/logical_plan/optimizer/predicate_pushdown/utils.rs
--rw-r--r--   0     1001      123     1755 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/functions/melt.rs
--rw-r--r--   0     1001      123     3930 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/functions/mod.rs
--rw-r--r--   0     1001      123     1799 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/generic.rs
--rw-r--r--   0     1001      123     3269 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/groupby.rs
--rw-r--r--   0     1001      123     2638 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/hstack.rs
--rw-r--r--   0     1001      123    15747 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/joins.rs
--rw-r--r--   0     1001      123    26502 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/mod.rs
--rw-r--r--   0     1001      123     3707 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/projection.rs
--rw-r--r--   0     1001      123     2639 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/rename.rs
--rw-r--r--   0     1001      123     3501 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/semi_anti_join.rs
--rw-r--r--   0     1001      123    27361 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/logical_plan/optimizer/simplify_expr.rs
--rw-r--r--   0     1001      123     3492 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/logical_plan/optimizer/slice_pushdown_expr.rs
--rw-r--r--   0     1001      123    13845 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/logical_plan/optimizer/slice_pushdown_lp.rs
--rw-r--r--   0     1001      123     3161 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/logical_plan/optimizer/stack_opt.rs
--rw-r--r--   0     1001      123     9725 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/logical_plan/optimizer/type_coercion/binary.rs
--rw-r--r--   0     1001      123    19820 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/logical_plan/optimizer/type_coercion/mod.rs
--rw-r--r--   0     1001      123    10187 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/logical_plan/options.rs
--rw-r--r--   0     1001      123    15276 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/logical_plan/projection.rs
--rw-r--r--   0     1001      123     4584 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/logical_plan/pyarrow.rs
--rw-r--r--   0     1001      123    13038 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/logical_plan/schema.rs
--rw-r--r--   0     1001      123      809 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/prelude.rs
--rw-r--r--   0     1001      123    11879 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/utils.rs
--rw-r--r--   0        0        0     2055 1970-01-01 00:00:00.000000 polars_u64_idx-0.17.8/local_dependencies/polars-time/Cargo.toml
--rw-r--r--   0     1001      123     1055 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-time/LICENSE
--rw-r--r--   0     1001      123     3565 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-time/src/chunkedarray/date.rs
--rw-r--r--   0     1001      123     6465 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-time/src/chunkedarray/datetime.rs
--rw-r--r--   0     1001      123     3305 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-time/src/chunkedarray/duration.rs
--rw-r--r--   0     1001      123     5607 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-time/src/chunkedarray/kernels.rs
--rw-r--r--   0     1001      123     1062 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-time/src/chunkedarray/mod.rs
--rw-r--r--   0     1001      123     7302 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-time/src/chunkedarray/rolling_window/floats.rs
--rw-r--r--   0     1001      123     2582 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-time/src/chunkedarray/rolling_window/ints.rs
--rw-r--r--   0     1001      123    10495 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-time/src/chunkedarray/rolling_window/mod.rs
--rw-r--r--   0     1001      123      428 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-time/src/chunkedarray/rolling_window/rolling_kernels/mod.rs
--rw-r--r--   0     1001      123     7642 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-time/src/chunkedarray/rolling_window/rolling_kernels/no_nulls.rs
--rw-r--r--   0     1001      123     2717 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-time/src/chunkedarray/time.rs
--rw-r--r--   0     1001      123    21192 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-time/src/chunkedarray/utf8/infer.rs
--rw-r--r--   0     1001      123    20108 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-time/src/chunkedarray/utf8/mod.rs
--rw-r--r--   0     1001      123     4115 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-time/src/chunkedarray/utf8/patterns.rs
--rw-r--r--   0     1001      123     9692 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-time/src/chunkedarray/utf8/strptime.rs
--rw-r--r--   0     1001      123     2960 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-time/src/date_range.rs
--rw-r--r--   0     1001      123    31461 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-time/src/groupby/dynamic.rs
--rw-r--r--   0     1001      123       88 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-time/src/groupby/mod.rs
--rw-r--r--   0     1001      123      613 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-time/src/lib.rs
--rw-r--r--   0     1001      123     3262 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-time/src/month_end.rs
--rw-r--r--   0     1001      123     3468 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-time/src/month_start.rs
--rw-r--r--   0     1001      123      320 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-time/src/prelude.rs
--rw-r--r--   0     1001      123     1568 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-time/src/round.rs
--rw-r--r--   0     1001      123     4028 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-time/src/series/_trait.rs
--rw-r--r--   0     1001      123      136 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-time/src/series/implementations/boolean.rs
--rw-r--r--   0     1001      123      140 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-time/src/series/implementations/categoricals.rs
--rw-r--r--   0     1001      123      133 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-time/src/series/implementations/date.rs
--rw-r--r--   0     1001      123      137 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-time/src/series/implementations/datetime.rs
--rw-r--r--   0     1001      123      137 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-time/src/series/implementations/duration.rs
--rw-r--r--   0     1001      123     1863 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-time/src/series/implementations/floats.rs
--rw-r--r--   0     1001      123     1792 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-time/src/series/implementations/integers.rs
--rw-r--r--   0     1001      123      133 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-time/src/series/implementations/list.rs
--rw-r--r--   0     1001      123      486 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-time/src/series/implementations/mod.rs
--rw-r--r--   0     1001      123      155 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-time/src/series/implementations/object.rs
--rw-r--r--   0     1001      123      135 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-time/src/series/implementations/struct_.rs
--rw-r--r--   0     1001      123      133 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-time/src/series/implementations/time.rs
--rw-r--r--   0     1001      123      133 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-time/src/series/implementations/utf8.rs
--rw-r--r--   0     1001      123    12466 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-time/src/series/mod.rs
--rw-r--r--   0     1001      123     1630 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-time/src/truncate.rs
--rw-r--r--   0     1001      123     7255 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-time/src/upsample.rs
--rw-r--r--   0     1001      123     2567 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-time/src/utils.rs
--rw-r--r--   0     1001      123     1524 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-time/src/windows/bounds.rs
--rw-r--r--   0     1001      123     2491 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-time/src/windows/calendar.rs
--rw-r--r--   0     1001      123    25599 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-time/src/windows/duration.rs
--rw-r--r--   0     1001      123    19317 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-time/src/windows/groupby.rs
--rw-r--r--   0     1001      123      503 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-time/src/windows/mod.rs
--rw-r--r--   0     1001      123    24372 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-time/src/windows/test.rs
--rw-r--r--   0     1001      123    11624 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-time/src/windows/window.rs
--rw-r--r--   0        0        0     5977 1970-01-01 00:00:00.000000 polars_u64_idx-0.17.8/local_dependencies/polars-lazy/Cargo.toml
--rw-r--r--   0     1001      123     1055 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-lazy/LICENSE
--rw-r--r--   0     1001      123     1796 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-lazy/src/dot.rs
--rw-r--r--   0     1001      123     4359 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-lazy/src/dsl/eval.rs
--rw-r--r--   0     1001      123     4505 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-lazy/src/dsl/functions.rs
--rw-r--r--   0     1001      123      164 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-lazy/src/dsl/into.rs
--rw-r--r--   0     1001      123     6754 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-lazy/src/dsl/list.rs
--rw-r--r--   0     1001      123     2899 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-lazy/src/dsl/mod.rs
--rw-r--r--   0     1001      123     1182 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-lazy/src/frame/anonymous_scan.rs
--rw-r--r--   0     1001      123     9278 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-lazy/src/frame/csv.rs
--rw-r--r--   0     1001      123     4309 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-lazy/src/frame/file_list_reader.rs
--rw-r--r--   0     1001      123     2261 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-lazy/src/frame/ipc.rs
--rw-r--r--   0     1001      123    47176 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-lazy/src/frame/mod.rs
--rw-r--r--   0     1001      123     3414 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-lazy/src/frame/ndjson.rs
--rw-r--r--   0     1001      123     3440 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-lazy/src/frame/parquet.rs
--rw-r--r--   0     1001      123     2892 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-lazy/src/frame/pivot.rs
--rw-r--r--   0     1001      123      416 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-lazy/src/frame/python.rs
--rw-r--r--   0     1001      123     6376 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-lazy/src/lib.rs
--rw-r--r--   0     1001      123     1049 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-lazy/src/physical_plan/executors/cache.rs
--rw-r--r--   0     1001      123      776 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-lazy/src/physical_plan/executors/executor.rs
--rw-r--r--   0     1001      123      670 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-lazy/src/physical_plan/executors/ext_context.rs
--rw-r--r--   0     1001      123     1284 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-lazy/src/physical_plan/executors/filter.rs
--rw-r--r--   0     1001      123     3908 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-lazy/src/physical_plan/executors/groupby.rs
--rw-r--r--   0     1001      123     3577 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-lazy/src/physical_plan/executors/groupby_dynamic.rs
--rw-r--r--   0     1001      123    13439 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-lazy/src/physical_plan/executors/groupby_partitioned.rs
--rw-r--r--   0     1001      123     4335 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-lazy/src/physical_plan/executors/groupby_rolling.rs
--rw-r--r--   0     1001      123     6058 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-lazy/src/physical_plan/executors/join.rs
--rw-r--r--   0     1001      123     7074 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-lazy/src/physical_plan/executors/mod.rs
--rw-r--r--   0     1001      123     2045 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-lazy/src/physical_plan/executors/projection.rs
--rw-r--r--   0     1001      123     1677 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-lazy/src/physical_plan/executors/python_scan.rs
--rw-r--r--   0     1001      123     2986 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-lazy/src/physical_plan/executors/scan/csv.rs
--rw-r--r--   0     1001      123     1963 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-lazy/src/physical_plan/executors/scan/ipc.rs
--rw-r--r--   0     1001      123     4151 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-lazy/src/physical_plan/executors/scan/mod.rs
--rw-r--r--   0     1001      123     1208 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-lazy/src/physical_plan/executors/scan/ndjson.rs
--rw-r--r--   0     1001      123     2421 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-lazy/src/physical_plan/executors/scan/parquet.rs
--rw-r--r--   0     1001      123      548 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-lazy/src/physical_plan/executors/slice.rs
--rw-r--r--   0     1001      123     2197 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-lazy/src/physical_plan/executors/sort.rs
--rw-r--r--   0     1001      123     1922 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-lazy/src/physical_plan/executors/stack.rs
--rw-r--r--   0     1001      123      663 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-lazy/src/physical_plan/executors/udf.rs
--rw-r--r--   0     1001      123     3702 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-lazy/src/physical_plan/executors/union.rs
--rw-r--r--   0     1001      123      838 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-lazy/src/physical_plan/executors/unique.rs
--rw-r--r--   0     1001      123     1284 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-lazy/src/physical_plan/exotic.rs
--rw-r--r--   0     1001      123    21873 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-lazy/src/physical_plan/expressions/aggregation.rs
--rw-r--r--   0     1001      123     2689 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-lazy/src/physical_plan/expressions/alias.rs
--rw-r--r--   0     1001      123    17432 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-lazy/src/physical_plan/expressions/apply.rs
--rw-r--r--   0     1001      123    17488 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-lazy/src/physical_plan/expressions/binary.rs
--rw-r--r--   0     1001      123     3153 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-lazy/src/physical_plan/expressions/cast.rs
--rw-r--r--   0     1001      123     6326 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-lazy/src/physical_plan/expressions/column.rs
--rw-r--r--   0     1001      123     2003 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-lazy/src/physical_plan/expressions/count.rs
--rw-r--r--   0     1001      123     5809 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-lazy/src/physical_plan/expressions/filter.rs
--rw-r--r--   0     1001      123     4131 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-lazy/src/physical_plan/expressions/group_iter.rs
--rw-r--r--   0     1001      123     5304 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-lazy/src/physical_plan/expressions/literal.rs
--rw-r--r--   0     1001      123    21103 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-lazy/src/physical_plan/expressions/mod.rs
--rw-r--r--   0     1001      123    10091 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-lazy/src/physical_plan/expressions/slice.rs
--rw-r--r--   0     1001      123     3929 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-lazy/src/physical_plan/expressions/sort.rs
--rw-r--r--   0     1001      123    11541 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-lazy/src/physical_plan/expressions/sortby.rs
--rw-r--r--   0     1001      123     8331 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-lazy/src/physical_plan/expressions/take.rs
--rw-r--r--   0     1001      123    14360 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-lazy/src/physical_plan/expressions/ternary.rs
--rw-r--r--   0     1001      123    31819 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-lazy/src/physical_plan/expressions/window.rs
--rw-r--r--   0     1001      123     2039 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-lazy/src/physical_plan/file_cache.rs
--rw-r--r--   0     1001      123      414 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-lazy/src/physical_plan/mod.rs
--rw-r--r--   0     1001      123     2005 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-lazy/src/physical_plan/node_timer.rs
--rw-r--r--   0     1001      123    27366 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-lazy/src/physical_plan/planner/expr.rs
--rw-r--r--   0     1001      123    18862 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-lazy/src/physical_plan/planner/lp.rs
--rw-r--r--   0     1001      123       87 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-lazy/src/physical_plan/planner/mod.rs
--rw-r--r--   0     1001      123     9425 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-lazy/src/physical_plan/state.rs
--rw-r--r--   0     1001      123    20891 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-lazy/src/physical_plan/streaming/convert.rs
--rw-r--r--   0     1001      123      219 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-lazy/src/physical_plan/streaming/mod.rs
--rw-r--r--   0     1001      123     3333 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-lazy/src/physical_plan/streaming/tree.rs
--rw-r--r--   0     1001      123      722 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-lazy/src/prelude.rs
--rw-r--r--   0     1001      123    14990 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-lazy/src/tests/aggregations.rs
--rw-r--r--   0     1001      123     2339 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-lazy/src/tests/arity.rs
--rw-r--r--   0     1001      123     7031 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-lazy/src/tests/cse.rs
--rw-r--r--   0     1001      123    12749 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-lazy/src/tests/io.rs
--rw-r--r--   0     1001      123     4207 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-lazy/src/tests/logical.rs
--rw-r--r--   0     1001      123     4288 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-lazy/src/tests/mod.rs
--rw-r--r--   0     1001      123    14812 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-lazy/src/tests/optimization_checks.rs
--rw-r--r--   0     1001      123     6799 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-lazy/src/tests/predicate_queries.rs
--rw-r--r--   0     1001      123     3158 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-lazy/src/tests/projection_queries.rs
--rw-r--r--   0     1001      123    47910 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-lazy/src/tests/queries.rs
--rw-r--r--   0     1001      123     8358 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-lazy/src/tests/streaming.rs
--rw-r--r--   0     1001      123     2886 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-lazy/src/tests/tpch.rs
--rw-r--r--   0     1001      123     1028 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-lazy/src/utils.rs
--rw-r--r--   0        0        0    10541 1970-01-01 00:00:00.000000 polars_u64_idx-0.17.8/local_dependencies/polars/Cargo.toml
--rw-r--r--   0     1001      123     1055 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars/LICENSE
--rw-r--r--   0     1001      123     3592 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars/Makefile
--rw-r--r--   0     1001      123      215 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars/build.rs
--rw-r--r--   0     1001      123       78 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars/clippy.toml
--rw-r--r--   0     1001      123    17602 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars/src/docs/eager.rs
--rw-r--r--   0     1001      123     8778 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars/src/docs/lazy.rs
--rw-r--r--   0     1001      123       50 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars/src/docs/mod.rs
--rw-r--r--   0     1001      123     3797 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars/src/docs/performance.rs
--rw-r--r--   0     1001      123       59 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars/src/export.rs
--rw-r--r--   0     1001      123    20207 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars/src/lib.rs
--rw-r--r--   0     1001      123      387 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars/src/prelude.rs
--rw-r--r--   0     1001      123       44 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars/src/sql.rs
--rw-r--r--   0     1001      123     4272 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars/tests/it/core/date_like.rs
--rw-r--r--   0     1001      123     2401 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars/tests/it/core/groupby.rs
--rw-r--r--   0     1001      123    17826 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars/tests/it/core/joins.rs
--rw-r--r--   0     1001      123      545 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars/tests/it/core/list.rs
--rw-r--r--   0     1001      123      189 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars/tests/it/core/mod.rs
--rw-r--r--   0     1001      123     6258 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars/tests/it/core/pivot.rs
--rw-r--r--   0     1001      123     1102 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars/tests/it/core/random.rs
--rw-r--r--   0     1001      123    10844 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars/tests/it/core/rolling_window.rs
--rw-r--r--   0     1001      123     1093 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars/tests/it/core/series.rs
--rw-r--r--   0     1001      123      370 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars/tests/it/core/utils.rs
--rw-r--r--   0     1001      123    30013 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars/tests/it/io/csv.rs
--rw-r--r--   0     1001      123     4490 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars/tests/it/io/ipc_stream.rs
--rw-r--r--   0     1001      123     7044 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars/tests/it/io/json.rs
--rw-r--r--   0     1001      123      378 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars/tests/it/io/mod.rs
--rw-r--r--   0     1001      123      988 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars/tests/it/io/parquet.rs
--rw-r--r--   0     1001      123     1530 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars/tests/it/joins.rs
--rw-r--r--   0     1001      123     2452 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars/tests/it/lazy/aggregation.rs
--rw-r--r--   0     1001      123      702 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars/tests/it/lazy/cse.rs
--rw-r--r--   0     1001      123      500 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars/tests/it/lazy/explodes.rs
--rw-r--r--   0     1001      123     2279 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars/tests/it/lazy/expressions/apply.rs
--rw-r--r--   0     1001      123    10285 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars/tests/it/lazy/expressions/arity.rs
--rw-r--r--   0     1001      123     1064 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars/tests/it/lazy/expressions/expand.rs
--rw-r--r--   0     1001      123     1008 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars/tests/it/lazy/expressions/filter.rs
--rw-r--r--   0     1001      123      428 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars/tests/it/lazy/expressions/is_in.rs
--rw-r--r--   0     1001      123      121 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars/tests/it/lazy/expressions/mod.rs
--rw-r--r--   0     1001      123      659 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars/tests/it/lazy/expressions/slice.rs
--rw-r--r--   0     1001      123    10139 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars/tests/it/lazy/expressions/window.rs
--rw-r--r--   0     1001      123      579 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars/tests/it/lazy/folds.rs
--rw-r--r--   0     1001      123      557 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars/tests/it/lazy/functions.rs
--rw-r--r--   0     1001      123     4482 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars/tests/it/lazy/groupby.rs
--rw-r--r--   0     1001      123     1655 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars/tests/it/lazy/groupby_dynamic.rs
--rw-r--r--   0     1001      123      691 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars/tests/it/lazy/mod.rs
--rw-r--r--   0     1001      123     5381 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars/tests/it/lazy/predicate_queries.rs
--rw-r--r--   0     1001      123     4476 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars/tests/it/lazy/projection_queries.rs
--rw-r--r--   0     1001      123     6444 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars/tests/it/lazy/queries.rs
--rw-r--r--   0     1001      123      141 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars/tests/it/main.rs
--rw-r--r--   0     1001      123    12591 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars/tests/it/schema.rs
--rw-r--r--   0        0        0      940 1970-01-01 00:00:00.000000 polars_u64_idx-0.17.8/local_dependencies/polars-row/Cargo.toml
--rw-r--r--   0     1001      123     1055 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-row/LICENSE
--rw-r--r--   0     1001      123     8985 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-row/src/encode.rs
--rw-r--r--   0     1001      123     4591 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-row/src/encodings/fixed.rs
--rw-r--r--   0     1001      123       47 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-row/src/encodings/mod.rs
--rw-r--r--   0     1001      123     4508 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-row/src/encodings/variable.rs
--rw-r--r--   0     1001      123    13678 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-row/src/lib.rs
--rw-r--r--   0     1001      123     2079 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-row/src/row.rs
--rw-r--r--   0     1001      123      682 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-row/src/utils.rs
--rw-r--r--   0        0        0      823 1970-01-01 00:00:00.000000 polars_u64_idx-0.17.8/local_dependencies/polars-algo/Cargo.toml
--rw-r--r--   0     1001      123     1055 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-algo/LICENSE
--rw-r--r--   0     1001      123     7393 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-algo/src/algo.rs
--rw-r--r--   0     1001      123       88 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-algo/src/lib.rs
--rw-r--r--   0     1001      123       28 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/local_dependencies/polars-algo/src/prelude.rs
--rw-r--r--   0        0        0     4398 1970-01-01 00:00:00.000000 polars_u64_idx-0.17.8/Cargo.toml
--rw-r--r--   0     1001      123       76 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/.gitignore
--rw-r--r--   0     1001      123     1055 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/LICENSE
--rw-r--r--   0     1001      123     2414 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/Makefile
--rw-r--r--   0     1001      123    12625 2023-04-24 15:07:25.000000 polars_u64_idx-0.17.8/README.md
--rw-r--r--   0     1001      123      651 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/build.rs
--rw-r--r--   0     1001      123       32 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/docs/.gitignore
--rw-r--r--   0     1001      123      679 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/docs/Makefile
--rw-r--r--   0     1001      123      318 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/docs/_templates/api_redirect.html
--rw-r--r--   0     1001      123      151 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/docs/_templates/autosummary/accessor.rst
--rw-r--r--   0     1001      123      160 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/docs/_templates/autosummary/accessor_attribute.rst
--rw-r--r--   0     1001      123      168 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/docs/_templates/autosummary/accessor_callable.rst
--rw-r--r--   0     1001      123      157 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/docs/_templates/autosummary/accessor_method.rst
--rw-r--r--   0     1001      123      836 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/docs/_templates/autosummary/class.rst
--rw-r--r--   0     1001      123       94 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/docs/_templates/autosummary/class_without_autosummary.rst
--rw-r--r--   0     1001      123      406 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/docs/_templates/sidebar-nav-bs.html
--rw-r--r--   0     1001      123      468 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/docs/requirements-docs.txt
--rw-r--r--   0     1001      123     1164 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/docs/run_live_docs_server.py
--rw-r--r--   0     1001      123     1567 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/docs/source/_static/css/custom.css
--rw-r--r--   0     1001      123     7326 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/docs/source/conf.py
--rw-r--r--   0     1001      123       51 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/docs/source/index.rst
--rw-r--r--   0     1001      123     6767 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/docs/source/reference/api.rst
--rw-r--r--   0     1001      123     1694 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/docs/source/reference/config.rst
--rw-r--r--   0     1001      123      274 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/docs/source/reference/dataframe/aggregation.rst
--rw-r--r--   0     1001      123      221 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/docs/source/reference/dataframe/attributes.rst
--rw-r--r--   0     1001      123      142 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/docs/source/reference/dataframe/computation.rst
--rw-r--r--   0     1001      123      319 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/docs/source/reference/dataframe/descriptive.rst
--rw-r--r--   0     1001      123      319 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/docs/source/reference/dataframe/export.rst
--rw-r--r--   0     1001      123      464 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/docs/source/reference/dataframe/groupby.rst
--rw-r--r--   0     1001      123      379 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/docs/source/reference/dataframe/index.rst
--rw-r--r--   0     1001      123      189 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/docs/source/reference/dataframe/miscellaneous.rst
--rw-r--r--   0     1001      123     1513 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/docs/source/reference/dataframe/modify_select.rst
--rw-r--r--   0     1001      123      663 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/docs/source/reference/datatypes.rst
--rw-r--r--   0     1001      123      421 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/docs/source/reference/exceptions.rst
--rw-r--r--   0     1001      123      391 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/docs/source/reference/expressions/aggregation.rst
--rw-r--r--   0     1001      123      309 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/docs/source/reference/expressions/binary.rst
--rw-r--r--   0     1001      123      338 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/docs/source/reference/expressions/boolean.rst
--rw-r--r--   0     1001      123      237 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/docs/source/reference/expressions/categories.rst
--rw-r--r--   0     1001      123      221 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/docs/source/reference/expressions/columns.rst
--rw-r--r--   0     1001      123     1061 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/docs/source/reference/expressions/computation.rst
--rw-r--r--   0     1001      123     1114 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/docs/source/reference/expressions/functions.rst
--rw-r--r--   0     1001      123      461 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/docs/source/reference/expressions/index.rst
--rw-r--r--   0     1001      123      695 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/docs/source/reference/expressions/list.rst
--rw-r--r--   0     1001      123      374 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/docs/source/reference/expressions/meta.rst
--rw-r--r--   0     1001      123      125 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/docs/source/reference/expressions/miscellaneous.rst
--rw-r--r--   0     1001      123      977 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/docs/source/reference/expressions/modify_select.rst
--rw-r--r--   0     1001      123      639 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/docs/source/reference/expressions/operators.rst
--rw-r--r--   0     1001      123      860 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/docs/source/reference/expressions/string.rst
--rw-r--r--   0     1001      123      254 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/docs/source/reference/expressions/struct.rst
--rw-r--r--   0     1001      123     1014 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/docs/source/reference/expressions/temporal.rst
--rw-r--r--   0     1001      123       98 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/docs/source/reference/expressions/window.rst
--rw-r--r--   0     1001      123      692 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/docs/source/reference/functions.rst
--rw-r--r--   0     1001      123      392 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/docs/source/reference/index.rst
--rw-r--r--   0     1001      123     1269 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/docs/source/reference/io.rst
--rw-r--r--   0     1001      123      252 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/docs/source/reference/lazyframe/aggregation.rst
--rw-r--r--   0     1001      123      179 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/docs/source/reference/lazyframe/attributes.rst
--rw-r--r--   0     1001      123      146 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/docs/source/reference/lazyframe/descriptive.rst
--rw-r--r--   0     1001      123      497 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/docs/source/reference/lazyframe/groupby.rst
--rw-r--r--   0     1001      123      354 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/docs/source/reference/lazyframe/index.rst
--rw-r--r--   0     1001      123      455 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/docs/source/reference/lazyframe/miscellaneous.rst
--rw-r--r--   0     1001      123      988 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/docs/source/reference/lazyframe/modify_select.rst
--rw-r--r--   0     1001      123      358 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/docs/source/reference/series/aggregation.rst
--rw-r--r--   0     1001      123      256 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/docs/source/reference/series/attributes.rst
--rw-r--r--   0     1001      123      321 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/docs/source/reference/series/binary.rst
--rw-r--r--   0     1001      123      117 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/docs/source/reference/series/boolean.rst
--rw-r--r--   0     1001      123      241 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/docs/source/reference/series/categories.rst
--rw-r--r--   0     1001      123     1103 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/docs/source/reference/series/computation.rst
--rw-r--r--   0     1001      123      744 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/docs/source/reference/series/descriptive.rst
--rw-r--r--   0     1001      123      240 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/docs/source/reference/series/export.rst
--rw-r--r--   0     1001      123      428 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/docs/source/reference/series/index.rst
--rw-r--r--   0     1001      123      749 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/docs/source/reference/series/list.rst
--rw-r--r--   0     1001      123      236 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/docs/source/reference/series/miscellaneous.rst
--rw-r--r--   0     1001      123     1077 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/docs/source/reference/series/modify_select.rst
--rw-r--r--   0     1001      123      922 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/docs/source/reference/series/string.rst
--rw-r--r--   0     1001      123      396 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/docs/source/reference/series/struct.rst
--rw-r--r--   0     1001      123     1168 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/docs/source/reference/series/temporal.rst
--rw-r--r--   0     1001      123      302 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/docs/source/reference/sql.rst
--rw-r--r--   0     1001      123     8067 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/docs/source/reference/testing.rst
--rw-r--r--   0     1001      123      168 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/docs/source/reference/utils.rst
--rw-r--r--   0     1001      123     6335 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/polars/__init__.py
--rw-r--r--   0     1001      123    13396 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/polars/api.py
--rw-r--r--   0     1001      123    25956 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/polars/config.py
--rw-r--r--   0     1001      123    27169 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/polars/convert.py
--rw-r--r--   0     1001      123       77 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/polars/dataframe/__init__.py
--rw-r--r--   0     1001      123     5237 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/polars/dataframe/_html.py
--rw-r--r--   0     1001      123   304748 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/polars/dataframe/frame.py
--rw-r--r--   0     1001      123    33240 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/polars/dataframe/groupby.py
--rw-r--r--   0     1001      123     2668 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/polars/datatypes/__init__.py
--rw-r--r--   0     1001      123    12133 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/polars/datatypes/classes.py
--rw-r--r--   0     1001      123     1603 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/polars/datatypes/constants.py
--rw-r--r--   0     1001      123     4430 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/polars/datatypes/constructor.py
--rw-r--r--   0     1001      123    15109 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/polars/datatypes/convert.py
--rw-r--r--   0     1001      123     7338 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/polars/dependencies.py
--rw-r--r--   0     1001      123     3436 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/polars/exceptions.py
--rw-r--r--   0     1001      123       61 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/polars/expr/__init__.py
--rw-r--r--   0     1001      123     2730 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/polars/expr/binary.py
--rw-r--r--   0     1001      123     1708 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/polars/expr/categorical.py
--rw-r--r--   0     1001      123    72692 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/polars/expr/datetime.py
--rw-r--r--   0     1001      123   251875 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/polars/expr/expr.py
--rw-r--r--   0     1001      123    22899 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/polars/expr/list.py
--rw-r--r--   0     1001      123     2059 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/polars/expr/meta.py
--rw-r--r--   0     1001      123    44737 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/polars/expr/string.py
--rw-r--r--   0     1001      123     5436 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/polars/expr/struct.py
--rw-r--r--   0     1001      123     1981 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/polars/functions/__init__.py
--rw-r--r--   0     1001      123    29637 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/polars/functions/eager.py
--rw-r--r--   0     1001      123    90827 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/polars/functions/lazy.py
--rw-r--r--   0     1001      123     6293 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/polars/functions/whenthen.py
--rw-r--r--   0     1001      123      280 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/polars/internals.py
--rw-r--r--   0     1001      123      978 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/polars/io/__init__.py
--rw-r--r--   0     1001      123     6264 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/polars/io/_utils.py
--rw-r--r--   0     1001      123      878 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/polars/io/avro.py
--rw-r--r--   0     1001      123      144 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/polars/io/csv/__init__.py
--rw-r--r--   0     1001      123     1082 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/polars/io/csv/_utils.py
--rw-r--r--   0     1001      123     4691 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/polars/io/csv/batched_reader.py
--rw-r--r--   0     1001      123    35533 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/polars/io/csv/functions.py
--rw-r--r--   0     1001      123     8655 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/polars/io/database.py
--rw-r--r--   0     1001      123    10988 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/polars/io/delta.py
--rw-r--r--   0     1001      123       75 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/polars/io/excel/__init__.py
--rw-r--r--   0     1001      123    18459 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/polars/io/excel/_write_utils.py
--rw-r--r--   0     1001      123     6476 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/polars/io/excel/functions.py
--rw-r--r--   0     1001      123      142 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/polars/io/ipc/__init__.py
--rw-r--r--   0     1001      123     1271 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/polars/io/ipc/anonymous_scan.py
--rw-r--r--   0     1001      123     5840 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/polars/io/ipc/functions.py
--rw-r--r--   0     1001      123      519 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/polars/io/json.py
--rw-r--r--   0     1001      123     2257 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/polars/io/ndjson.py
--rw-r--r--   0     1001      123      170 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/polars/io/parquet/__init__.py
--rw-r--r--   0     1001      123     1299 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/polars/io/parquet/anonymous_scan.py
--rw-r--r--   0     1001      123     7212 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/polars/io/parquet/functions.py
--rw-r--r--   0     1001      123      136 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/polars/io/pyarrow_dataset/__init__.py
--rw-r--r--   0     1001      123     2331 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/polars/io/pyarrow_dataset/anonymous_scan.py
--rw-r--r--   0     1001      123     3611 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/polars/io/pyarrow_dataset/functions.py
--rw-r--r--   0     1001      123       77 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/polars/lazyframe/__init__.py
--rw-r--r--   0     1001      123   167301 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/polars/lazyframe/frame.py
--rw-r--r--   0     1001      123    24178 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/polars/lazyframe/groupby.py
--rw-r--r--   0     1001      123        0 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/polars/py.typed
--rw-r--r--   0     1001      123       69 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/polars/series/__init__.py
--rw-r--r--   0     1001      123     1579 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/polars/series/_numpy.py
--rw-r--r--   0     1001      123     1920 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/polars/series/binary.py
--rw-r--r--   0     1001      123     1699 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/polars/series/categorical.py
--rw-r--r--   0     1001      123    49474 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/polars/series/datetime.py
--rw-r--r--   0     1001      123    12385 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/polars/series/list.py
--rw-r--r--   0     1001      123   164038 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/polars/series/series.py
--rw-r--r--   0     1001      123    27401 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/polars/series/string.py
--rw-r--r--   0     1001      123     2287 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/polars/series/struct.py
--rw-r--r--   0     1001      123     5375 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/polars/series/utils.py
--rw-r--r--   0     1001      123     7638 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/polars/slice.py
--rw-r--r--   0     1001      123       75 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/polars/sql/__init__.py
--rw-r--r--   0     1001      123     1351 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/polars/sql/context.py
--rw-r--r--   0     1001      123     4764 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/polars/string_cache.py
--rw-r--r--   0     1001      123      362 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/polars/testing/__init__.py
--rw-r--r--   0     1001      123      929 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/polars/testing/_private.py
--rw-r--r--   0     1001      123     3689 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/polars/testing/_tempdir.py
--rw-r--r--   0     1001      123    13597 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/polars/testing/asserts.py
--rw-r--r--   0     1001      123      800 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/polars/testing/parametric/__init__.py
--rw-r--r--   0     1001      123    25149 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/polars/testing/parametric/primitives.py
--rw-r--r--   0     1001      123     3409 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/polars/testing/parametric/profiles.py
--rw-r--r--   0     1001      123     7711 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/polars/testing/parametric/strategies.py
--rw-r--r--   0     1001      123     5824 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/polars/type_aliases.py
--rw-r--r--   0     1001      123     1211 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/polars/utils/__init__.py
--rw-r--r--   0     1001      123    50687 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/polars/utils/_construction.py
--rw-r--r--   0     1001      123     2782 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/polars/utils/_parse_expr_input.py
--rw-r--r--   0     1001      123      721 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/polars/utils/_scan.py
--rw-r--r--   0     1001      123      687 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/polars/utils/_wrap.py
--rw-r--r--   0     1001      123      683 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/polars/utils/build_info.py
--rw-r--r--   0     1001      123     8812 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/polars/utils/convert.py
--rw-r--r--   0     1001      123     5789 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/polars/utils/decorators.py
--rw-r--r--   0     1001      123     1660 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/polars/utils/meta.py
--rw-r--r--   0     1001      123      514 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/polars/utils/polars_version.py
--rw-r--r--   0     1001      123     2339 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/polars/utils/show_versions.py
--rw-r--r--   0     1001      123    11592 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/polars/utils/various.py
--rw-r--r--   0     1001      123     5378 2023-04-24 15:07:25.000000 polars_u64_idx-0.17.8/pyproject.toml
--rw-r--r--   0     1001      123      699 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/requirements-dev.txt
--rw-r--r--   0     1001      123       70 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/requirements-lint.txt
--rw-r--r--   0     1001      123     1640 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/scripts/check_stacklevels.py
--rw-r--r--   0     1001      123    11023 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/src/apply/dataframe.rs
--rw-r--r--   0     1001      123     8388 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/src/apply/mod.rs
--rw-r--r--   0     1001      123    71480 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/src/apply/series.rs
--rw-r--r--   0     1001      123       32 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/src/arrow_interop/mod.rs
--rw-r--r--   0     1001      123     1306 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/src/arrow_interop/to_py.rs
--rw-r--r--   0     1001      123     3902 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/src/arrow_interop/to_rust.rs
--rw-r--r--   0     1001      123     5250 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/src/batched_csv.rs
--rw-r--r--   0     1001      123    46606 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/src/conversion.rs
--rw-r--r--   0     1001      123    45472 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/src/dataframe.rs
--rw-r--r--   0     1001      123     3799 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/src/datatypes.rs
--rw-r--r--   0     1001      123     3288 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/src/error.rs
--rw-r--r--   0     1001      123     9482 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/src/file.rs
--rw-r--r--   0     1001      123     7468 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/src/lazy/apply.rs
--rw-r--r--   0     1001      123    33439 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/src/lazy/dataframe.rs
--rw-r--r--   0     1001      123    62598 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/src/lazy/dsl.rs
--rw-r--r--   0     1001      123     1082 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/src/lazy/meta.rs
--rw-r--r--   0     1001      123      727 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/src/lazy/mod.rs
--rw-r--r--   0     1001      123      212 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/src/lazy/utils.rs
--rw-r--r--   0     1001      123    20992 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/src/lib.rs
--rw-r--r--   0     1001      123     8642 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/src/npy.rs
--rw-r--r--   0     1001      123     1029 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/src/object.rs
--rw-r--r--   0     1001      123      122 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/src/prelude.rs
--rw-r--r--   0     1001      123      435 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/src/py_modules.rs
--rw-r--r--   0     1001      123    54535 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/src/series.rs
--rw-r--r--   0     1001      123     3478 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/src/set.rs
--rw-r--r--   0     1001      123      843 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/src/sql.rs
--rw-r--r--   0     1001      123     2335 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/src/utils.rs
--rw-r--r--   0     1001      123     6165 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/tests/README.md
--rw-r--r--   0     1001      123     2189 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/tests/benchmark/groupby-datagen.R
--rw-r--r--   0     1001      123     7945 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/tests/benchmark/run_h2oai_benchmark.py
--rw-r--r--   0     1001      123     6530 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/tests/benchmark/test_release.py
--rw-r--r--   0     1001      123     4589 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/tests/docs/run_doctest.py
--rw-r--r--   0     1001      123      179 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/tests/parametric/conftest.py
--rw-r--r--   0     1001      123     3823 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/tests/parametric/test_dataframe.py
--rw-r--r--   0     1001      123     1692 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/tests/parametric/test_lazyframe.py
--rw-r--r--   0     1001      123     6863 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/tests/parametric/test_series.py
--rw-r--r--   0     1001      123     8299 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/tests/parametric/test_testing.py
--rw-r--r--   0     1001      123        0 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/tests/unit/__init__.py
--rw-r--r--   0     1001      123     3382 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/tests/unit/conftest.py
--rw-r--r--   0     1001      123       86 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/tests/unit/datatypes/__init__.py
--rw-r--r--   0     1001      123      351 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/tests/unit/datatypes/test_binary.py
--rw-r--r--   0     1001      123     1420 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/tests/unit/datatypes/test_bool.py
--rw-r--r--   0     1001      123    12662 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/tests/unit/datatypes/test_categorical.py
--rw-r--r--   0     1001      123     2826 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/tests/unit/datatypes/test_decimal.py
--rw-r--r--   0     1001      123      280 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/tests/unit/datatypes/test_duration.py
--rw-r--r--   0     1001      123    16033 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/tests/unit/datatypes/test_list.py
--rw-r--r--   0     1001      123      284 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/tests/unit/datatypes/test_null.py
--rw-r--r--   0     1001      123     2801 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/tests/unit/datatypes/test_object.py
--rw-r--r--   0     1001      123    29644 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/tests/unit/datatypes/test_struct.py
--rw-r--r--   0     1001      123    91697 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/tests/unit/datatypes/test_temporal.py
--rw-r--r--   0     1001      123      418 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/tests/unit/datatypes/test_time.py
--rw-r--r--   0     1001      123      218 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/tests/unit/io/conftest.py
--rw-r--r--   0     1001      123       16 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/tests/unit/io/files/delta-table/.part-00000-e42312d7-60e5-454d-acbc-db192d220e73-c000.snappy.parquet.crc
--rw-r--r--   0     1001      123       16 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/tests/unit/io/files/delta-table/.part-00000-e4a999da-df45-4fb0-bdc4-d999fc0f58aa-c000.snappy.parquet.crc
--rw-r--r--   0     1001      123       16 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/tests/unit/io/files/delta-table/_delta_log/.00000000000000000000.json.crc
--rw-r--r--   0     1001      123       16 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/tests/unit/io/files/delta-table/_delta_log/.00000000000000000001.json.crc
--rw-r--r--   0     1001      123      905 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/tests/unit/io/files/delta-table/_delta_log/00000000000000000000.json
--rw-r--r--   0     1001      123      936 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/tests/unit/io/files/delta-table/_delta_log/00000000000000000001.json
--rw-r--r--   0     1001      123      972 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/tests/unit/io/files/delta-table/part-00000-e42312d7-60e5-454d-acbc-db192d220e73-c000.snappy.parquet
--rw-r--r--   0     1001      123      690 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/tests/unit/io/files/delta-table/part-00000-e4a999da-df45-4fb0-bdc4-d999fc0f58aa-c000.snappy.parquet
--rw-r--r--   0     1001      123        0 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/tests/unit/io/files/empty.csv
--rw-r--r--   0     1001      123     5959 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/tests/unit/io/files/example.xlsx
--rw-r--r--   0     1001      123      457 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/tests/unit/io/files/foods1.csv
--rw-r--r--   0     1001      123     2351 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/tests/unit/io/files/foods1.ipc
--rw-r--r--   0     1001      123     1713 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/tests/unit/io/files/foods1.ndjson
--rw-r--r--   0     1001      123     1427 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/tests/unit/io/files/foods1.parquet
--rw-r--r--   0     1001      123      455 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/tests/unit/io/files/foods2.csv
--rw-r--r--   0     1001      123     2351 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/tests/unit/io/files/foods2.ipc
--rw-r--r--   0     1001      123     1711 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/tests/unit/io/files/foods2.ndjson
--rw-r--r--   0     1001      123     1916 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/tests/unit/io/files/foods2.parquet
--rw-r--r--   0     1001      123      455 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/tests/unit/io/files/foods3.csv
--rw-r--r--   0     1001      123      457 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/tests/unit/io/files/foods4.csv
--rw-r--r--   0     1001      123      452 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/tests/unit/io/files/foods5.csv
--rw-r--r--   0     1001      123       49 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/tests/unit/io/files/gzipped.csv
--rw-r--r--   0     1001      123       57 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/tests/unit/io/files/small.csv
--rw-r--r--   0     1001      123      756 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/tests/unit/io/files/small.parquet
--rw-r--r--   0     1001      123     1937 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/tests/unit/io/test_avro.py
--rw-r--r--   0     1001      123    39498 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/tests/unit/io/test_csv.py
--rw-r--r--   0     1001      123     6360 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/tests/unit/io/test_database.py
--rw-r--r--   0     1001      123     3456 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/tests/unit/io/test_delta.py
--rw-r--r--   0     1001      123    11169 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/tests/unit/io/test_excel.py
--rw-r--r--   0     1001      123     5919 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/tests/unit/io/test_ipc.py
--rw-r--r--   0     1001      123     3720 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/tests/unit/io/test_json.py
--rw-r--r--   0     1001      123     6849 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/tests/unit/io/test_lazy_csv.py
--rw-r--r--   0     1001      123     2060 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/tests/unit/io/test_lazy_ipc.py
--rw-r--r--   0     1001      123     2881 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/tests/unit/io/test_lazy_json.py
--rw-r--r--   0     1001      123    11849 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/tests/unit/io/test_lazy_parquet.py
--rw-r--r--   0     1001      123     2012 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/tests/unit/io/test_other.py
--rw-r--r--   0     1001      123    13735 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/tests/unit/io/test_parquet.py
--rw-r--r--   0     1001      123      612 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/tests/unit/io/test_pickle.py
--rw-r--r--   0     1001      123     3259 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/tests/unit/io/test_pyarrow_dataset.py
--rw-r--r--   0     1001      123      509 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/tests/unit/namespaces/__init__.py
--rw-r--r--   0     1001      123     3218 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/tests/unit/namespaces/test_binary.py
--rw-r--r--   0     1001      123     2489 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/tests/unit/namespaces/test_categorical.py
--rw-r--r--   0     1001      123    18655 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/tests/unit/namespaces/test_datetime.py
--rw-r--r--   0     1001      123    12750 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/tests/unit/namespaces/test_list.py
--rw-r--r--   0     1001      123     1748 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/tests/unit/namespaces/test_meta.py
--rw-r--r--   0     1001      123    23698 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/tests/unit/namespaces/test_string.py
--rw-r--r--   0     1001      123    16930 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/tests/unit/namespaces/test_strptime.py
--rw-r--r--   0     1001      123      982 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/tests/unit/namespaces/test_struct.py
--rw-r--r--   0     1001      123       85 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/tests/unit/operations/__init__.py
--rw-r--r--   0     1001      123     6238 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/tests/unit/operations/test_aggregations.py
--rw-r--r--   0     1001      123     9412 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/tests/unit/operations/test_apply.py
--rw-r--r--   0     1001      123     4390 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/tests/unit/operations/test_arithmetic.py
--rw-r--r--   0     1001      123      956 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/tests/unit/operations/test_comparison.py
--rw-r--r--   0     1001      123     2906 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/tests/unit/operations/test_drop.py
--rw-r--r--   0     1001      123     8252 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/tests/unit/operations/test_explode.py
--rw-r--r--   0     1001      123     3664 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/tests/unit/operations/test_filter.py
--rw-r--r--   0     1001      123     1801 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/tests/unit/operations/test_folds.py
--rw-r--r--   0     1001      123    22696 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/tests/unit/operations/test_groupby.py
--rw-r--r--   0     1001      123     2959 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/tests/unit/operations/test_is_in.py
--rw-r--r--   0     1001      123    16937 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/tests/unit/operations/test_join.py
--rw-r--r--   0     1001      123    10467 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/tests/unit/operations/test_join_asof.py
--rw-r--r--   0     1001      123      643 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/tests/unit/operations/test_melt.py
--rw-r--r--   0     1001      123    10253 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/tests/unit/operations/test_pivot.py
--rw-r--r--   0     1001      123    18639 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/tests/unit/operations/test_rolling.py
--rw-r--r--   0     1001      123    19550 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/tests/unit/operations/test_sort.py
--rw-r--r--   0     1001      123     3643 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/tests/unit/operations/test_statistics.py
--rw-r--r--   0     1001      123     3631 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/tests/unit/operations/test_transpose.py
--rw-r--r--   0     1001      123      771 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/tests/unit/operations/test_unique.py
--rw-r--r--   0     1001      123     9814 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/tests/unit/operations/test_window.py
--rw-r--r--   0     1001      123     4775 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/tests/unit/test_api.py
--rw-r--r--   0     1001      123     1077 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/tests/unit/test_arity.py
--rw-r--r--   0     1001      123    19856 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/tests/unit/test_cfg.py
--rw-r--r--   0     1001      123    39286 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/tests/unit/test_constructors.py
--rw-r--r--   0     1001      123      454 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/tests/unit/test_context.py
--rw-r--r--   0     1001      123     1628 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/tests/unit/test_cse.py
--rw-r--r--   0     1001      123     3817 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/tests/unit/test_datatypes.py
--rw-r--r--   0     1001      123   121069 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/tests/unit/test_df.py
--rw-r--r--   0     1001      123     1196 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/tests/unit/test_empty.py
--rw-r--r--   0     1001      123    16867 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/tests/unit/test_errors.py
--rw-r--r--   0     1001      123     2387 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/tests/unit/test_expr_multi_cols.py
--rw-r--r--   0     1001      123    32643 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/tests/unit/test_exprs.py
--rw-r--r--   0     1001      123     3305 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/tests/unit/test_fmt.py
--rw-r--r--   0     1001      123    11420 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/tests/unit/test_functions.py
--rw-r--r--   0     1001      123     3763 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/tests/unit/test_interchange.py
--rw-r--r--   0     1001      123    33952 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/tests/unit/test_interop.py
--rw-r--r--   0     1001      123    49534 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/tests/unit/test_lazy.py
--rw-r--r--   0     1001      123     2369 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/tests/unit/test_polars_import.py
--rw-r--r--   0     1001      123     4014 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/tests/unit/test_predicates.py
--rw-r--r--   0     1001      123     6995 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/tests/unit/test_projections.py
--rw-r--r--   0     1001      123    11550 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/tests/unit/test_queries.py
--rw-r--r--   0     1001      123     4743 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/tests/unit/test_rows.py
--rw-r--r--   0     1001      123    13181 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/tests/unit/test_schema.py
--rw-r--r--   0     1001      123     2634 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/tests/unit/test_serde.py
--rw-r--r--   0     1001      123    84354 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/tests/unit/test_series.py
--rw-r--r--   0     1001      123     2561 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/tests/unit/test_sql.py
--rw-r--r--   0     1001      123    13877 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/tests/unit/test_streaming.py
--rw-r--r--   0     1001      123    10700 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/tests/unit/test_testing.py
--rw-r--r--   0     1001      123       41 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/tests/unit/utils/__init__.py
--rw-r--r--   0     1001      123      306 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/tests/unit/utils/test_build_info.py
--rw-r--r--   0     1001      123      247 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/tests/unit/utils/test_show_versions.py
--rw-r--r--   0     1001      123     4307 2023-04-24 15:07:24.000000 polars_u64_idx-0.17.8/tests/unit/utils/test_utils.py
--rw-r--r--   0     1001      123    65631 2023-04-24 15:08:28.000000 polars_u64_idx-0.17.8/Cargo.lock
--rw-r--r--   0        0        0    15163 1970-01-01 00:00:00.000000 polars_u64_idx-0.17.8/PKG-INFO
+-rw-r--r--   0        0        0     5450 1970-01-01 00:00:00.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/Cargo.toml
+-rw-r--r--   0     1001      123     1055 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/LICENSE
+-rw-r--r--   0     1001      123    19606 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/arithmetic.rs
+-rw-r--r--   0     1001      123     8699 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/bitwise.rs
+-rw-r--r--   0     1001      123     2298 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/builder/binary.rs
+-rw-r--r--   0     1001      123     1207 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/builder/boolean.rs
+-rw-r--r--   0     1001      123     1556 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/builder/from.rs
+-rw-r--r--   0     1001      123    20366 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/builder/list.rs
+-rw-r--r--   0     1001      123     8845 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/builder/mod.rs
+-rw-r--r--   0     1001      123     1410 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/builder/primitive.rs
+-rw-r--r--   0     1001      123     2291 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/builder/utf8.rs
+-rw-r--r--   0     1001      123    11683 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/cast.rs
+-rw-r--r--   0     1001      123    48300 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/comparison/mod.rs
+-rw-r--r--   0     1001      123     9463 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/comparison/scalar.rs
+-rw-r--r--   0     1001      123      551 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/drop.rs
+-rw-r--r--   0     1001      123      963 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/float.rs
+-rw-r--r--   0     1001      123     5069 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/from.rs
+-rw-r--r--   0     1001      123    38411 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/iterator/mod.rs
+-rw-r--r--   0     1001      123     1395 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/iterator/par/list.rs
+-rw-r--r--   0     1001      123       28 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/iterator/par/mod.rs
+-rw-r--r--   0     1001      123     1129 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/iterator/par/utf8.rs
+-rw-r--r--   0     1001      123       21 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/kernels/mod.rs
+-rw-r--r--   0     1001      123     2986 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/kernels/take.rs
+-rw-r--r--   0     1001      123     7728 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/list/iterator.rs
+-rw-r--r--   0     1001      123     2802 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/list/mod.rs
+-rw-r--r--   0     1001      123    19796 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/logical/categorical/builder.rs
+-rw-r--r--   0     1001      123     3688 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/logical/categorical/from.rs
+-rw-r--r--   0     1001      123     4270 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/logical/categorical/merge.rs
+-rw-r--r--   0     1001      123    10220 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/logical/categorical/mod.rs
+-rw-r--r--   0     1001      123     1400 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/append.rs
+-rw-r--r--   0     1001      123      358 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/full.rs
+-rw-r--r--   0     1001      123      192 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/mod.rs
+-rw-r--r--   0     1001      123     2731 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/take_random.rs
+-rw-r--r--   0     1001      123     2172 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/unique.rs
+-rw-r--r--   0     1001      123      925 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/zip.rs
+-rw-r--r--   0     1001      123     6453 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/logical/categorical/stringcache.rs
+-rw-r--r--   0     1001      123     1604 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/logical/date.rs
+-rw-r--r--   0     1001      123     4105 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/logical/datetime.rs
+-rw-r--r--   0     1001      123     4443 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/logical/decimal.rs
+-rw-r--r--   0     1001      123     2434 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/logical/duration.rs
+-rw-r--r--   0     1001      123     2549 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/logical/mod.rs
+-rw-r--r--   0     1001      123      476 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/logical/struct_/from.rs
+-rw-r--r--   0     1001      123    15081 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/logical/struct_/mod.rs
+-rw-r--r--   0     1001      123     1182 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/logical/time.rs
+-rw-r--r--   0     1001      123    23524 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/mod.rs
+-rw-r--r--   0     1001      123     7200 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/ndarray.rs
+-rw-r--r--   0     1001      123     4484 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/object/builder.rs
+-rw-r--r--   0     1001      123     1547 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/object/extension/drop.rs
+-rw-r--r--   0     1001      123     3124 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/object/extension/list.rs
+-rw-r--r--   0     1001      123     7054 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/object/extension/mod.rs
+-rw-r--r--   0     1001      123     3410 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/object/extension/polars_extension.rs
+-rw-r--r--   0     1001      123      137 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/object/is_valid.rs
+-rw-r--r--   0     1001      123     4419 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/object/iterator.rs
+-rw-r--r--   0     1001      123     4826 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/object/mod.rs
+-rw-r--r--   0     1001      123     2853 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/object/registry.rs
+-rw-r--r--   0     1001      123      272 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/ops/abs.rs
+-rw-r--r--   0     1001      123    32120 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/ops/aggregate/mod.rs
+-rw-r--r--   0     1001      123     9946 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/ops/aggregate/quantile.rs
+-rw-r--r--   0     1001      123     2875 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/ops/aggregate/var.rs
+-rw-r--r--   0     1001      123     9670 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/ops/any_value.rs
+-rw-r--r--   0     1001      123     2365 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/ops/append.rs
+-rw-r--r--   0     1001      123    27269 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/ops/apply.rs
+-rw-r--r--   0     1001      123    12799 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/ops/bit_repr.rs
+-rw-r--r--   0     1001      123     6214 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/ops/chunkops.rs
+-rw-r--r--   0     1001      123    11537 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/ops/compare_inner.rs
+-rw-r--r--   0     1001      123     1737 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/ops/concat_str.rs
+-rw-r--r--   0     1001      123     4801 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/ops/cum_agg.rs
+-rw-r--r--   0     1001      123     6264 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/ops/downcast.rs
+-rw-r--r--   0     1001      123    25614 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/ops/explode.rs
+-rw-r--r--   0     1001      123     8339 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/ops/extend.rs
+-rw-r--r--   0     1001      123    13777 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/ops/fill_null.rs
+-rw-r--r--   0     1001      123     5308 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/ops/filter.rs
+-rw-r--r--   0     1001      123     4436 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/ops/full.rs
+-rw-r--r--   0     1001      123        1 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/ops/interpolate.rs
+-rw-r--r--   0     1001      123    15385 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/ops/is_in.rs
+-rw-r--r--   0     1001      123        1 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/ops/len.rs
+-rw-r--r--   0     1001      123     2658 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/ops/min_max_binary.rs
+-rw-r--r--   0     1001      123    22407 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/ops/mod.rs
+-rw-r--r--   0     1001      123     2403 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/ops/nulls.rs
+-rw-r--r--   0     1001      123      593 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/ops/peaks.rs
+-rw-r--r--   0     1001      123     2585 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/ops/repeat_by.rs
+-rw-r--r--   0     1001      123     1539 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/ops/reverse.rs
+-rw-r--r--   0     1001      123    10234 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/ops/rolling_window.rs
+-rw-r--r--   0     1001      123    12518 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/ops/set.rs
+-rw-r--r--   0     1001      123     6151 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/ops/shift.rs
+-rw-r--r--   0     1001      123     2299 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/ops/sort/arg_sort.rs
+-rw-r--r--   0     1001      123     5467 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/ops/sort/arg_sort_multiple.rs
+-rw-r--r--   0     1001      123     7430 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/ops/sort/categorical.rs
+-rw-r--r--   0     1001      123    30762 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/ops/sort/mod.rs
+-rw-r--r--   0     1001      123      380 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/ops/sort/slice.rs
+-rw-r--r--   0     1001      123    20472 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/ops/take/mod.rs
+-rw-r--r--   0     1001      123     6630 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/ops/take/take_chunked.rs
+-rw-r--r--   0     1001      123     1859 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/ops/take/take_every.rs
+-rw-r--r--   0     1001      123    16256 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/ops/take/take_random.rs
+-rw-r--r--   0     1001      123     5041 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/ops/take/take_single.rs
+-rw-r--r--   0     1001      123     6064 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/ops/take/traits.rs
+-rw-r--r--   0     1001      123    11229 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/ops/unique/mod.rs
+-rw-r--r--   0     1001      123    14620 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/ops/unique/rank.rs
+-rw-r--r--   0     1001      123     7753 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/ops/zip.rs
+-rw-r--r--   0     1001      123     9093 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/random.rs
+-rw-r--r--   0     1001      123     1959 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/temporal/conversion.rs
+-rw-r--r--   0     1001      123     2501 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/temporal/date.rs
+-rw-r--r--   0     1001      123    12123 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/temporal/datetime.rs
+-rw-r--r--   0     1001      123     3201 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/temporal/duration.rs
+-rw-r--r--   0     1001      123      533 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/temporal/mod.rs
+-rw-r--r--   0     1001      123     2724 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/temporal/time.rs
+-rw-r--r--   0     1001      123      872 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/to_vec.rs
+-rw-r--r--   0     1001      123     8113 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/trusted_len.rs
+-rw-r--r--   0     1001      123    25182 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/upstream_traits.rs
+-rw-r--r--   0     1001      123     7689 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/cloud.rs
+-rw-r--r--   0     1001      123     1549 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/config.rs
+-rw-r--r--   0     1001      123     3946 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/datatypes/_serde.rs
+-rw-r--r--   0     1001      123     2650 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/datatypes/aliases.rs
+-rw-r--r--   0     1001      123    42410 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/datatypes/any_value.rs
+-rw-r--r--   0     1001      123    12083 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/datatypes/dtype.rs
+-rw-r--r--   0     1001      123     5456 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/datatypes/field.rs
+-rw-r--r--   0     1001      123     7675 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/datatypes/mod.rs
+-rw-r--r--   0     1001      123     2016 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/datatypes/time_unit.rs
+-rw-r--r--   0     1001      123      118 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/doc/changelog/mod.rs
+-rw-r--r--   0     1001      123      898 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/doc/changelog/v0_10_0_11.rs
+-rw-r--r--   0     1001      123      481 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/doc/changelog/v0_3.rs
+-rw-r--r--   0     1001      123      293 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/doc/changelog/v0_4.rs
+-rw-r--r--   0     1001      123      499 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/doc/changelog/v0_5.rs
+-rw-r--r--   0     1001      123      288 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/doc/changelog/v0_6.rs
+-rw-r--r--   0     1001      123     1071 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/doc/changelog/v0_7.rs
+-rw-r--r--   0     1001      123      819 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/doc/changelog/v0_8.rs
+-rw-r--r--   0     1001      123      596 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/doc/changelog/v0_9.rs
+-rw-r--r--   0     1001      123       43 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/doc/mod.rs
+-rw-r--r--   0     1001      123       25 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/error.rs
+-rw-r--r--   0     1001      123      433 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/export.rs
+-rw-r--r--   0     1001      123    36116 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/fmt.rs
+-rw-r--r--   0     1001      123     5177 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/frame/arithmetic.rs
+-rw-r--r--   0     1001      123     7874 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/frame/asof_join/asof.rs
+-rw-r--r--   0     1001      123    33865 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/frame/asof_join/groups.rs
+-rw-r--r--   0     1001      123     6660 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/frame/asof_join/mod.rs
+-rw-r--r--   0     1001      123      559 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/frame/chunks.rs
+-rw-r--r--   0     1001      123     5179 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/frame/cross_join.rs
+-rw-r--r--   0     1001      123    16609 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/frame/explode.rs
+-rw-r--r--   0     1001      123     1019 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/frame/from.rs
+-rw-r--r--   0     1001      123    16518 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/frame/groupby/aggregations/agg_list.rs
+-rw-r--r--   0     1001      123     4115 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/frame/groupby/aggregations/boolean.rs
+-rw-r--r--   0     1001      123     7643 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/frame/groupby/aggregations/dispatch.rs
+-rw-r--r--   0     1001      123    39255 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/frame/groupby/aggregations/mod.rs
+-rw-r--r--   0     1001      123     5636 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/frame/groupby/aggregations/utf8.rs
+-rw-r--r--   0     1001      123      218 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/frame/groupby/expr.rs
+-rw-r--r--   0     1001      123    19976 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/frame/groupby/hashing.rs
+-rw-r--r--   0     1001      123    14075 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/frame/groupby/into_groups.rs
+-rw-r--r--   0     1001      123    39383 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/frame/groupby/mod.rs
+-rw-r--r--   0     1001      123    10593 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/frame/groupby/perfect.rs
+-rw-r--r--   0     1001      123    18842 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/frame/groupby/proxy.rs
+-rw-r--r--   0     1001      123    18264 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/frame/hash_join/mod.rs
+-rw-r--r--   0     1001      123    22392 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/frame/hash_join/multiple_keys.rs
+-rw-r--r--   0     1001      123     2413 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/frame/hash_join/single_keys.rs
+-rw-r--r--   0     1001      123    16352 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/frame/hash_join/single_keys_dispatch.rs
+-rw-r--r--   0     1001      123     4295 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/frame/hash_join/single_keys_inner.rs
+-rw-r--r--   0     1001      123     6076 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/frame/hash_join/single_keys_left.rs
+-rw-r--r--   0     1001      123     4247 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/frame/hash_join/single_keys_outer.rs
+-rw-r--r--   0     1001      123     3913 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/frame/hash_join/single_keys_semi_anti.rs
+-rw-r--r--   0     1001      123    11884 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/frame/hash_join/sort_merge.rs
+-rw-r--r--   0     1001      123   124136 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/frame/mod.rs
+-rw-r--r--   0     1001      123    27513 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/frame/row/av_buffer.rs
+-rw-r--r--   0     1001      123     3732 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/frame/row/dataframe.rs
+-rw-r--r--   0     1001      123     5976 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/frame/row/mod.rs
+-rw-r--r--   0     1001      123     8795 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/frame/row/transpose.rs
+-rw-r--r--   0     1001      123     2183 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/frame/top_k.rs
+-rw-r--r--   0     1001      123     1388 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/frame/upstream_traits.rs
+-rw-r--r--   0     1001      123    10935 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/functions.rs
+-rw-r--r--   0     1001      123     2149 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/hashing/fx.rs
+-rw-r--r--   0     1001      123     1503 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/hashing/identity.rs
+-rw-r--r--   0     1001      123      457 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/hashing/mod.rs
+-rw-r--r--   0     1001      123     2684 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/hashing/partition.rs
+-rw-r--r--   0     1001      123    17653 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/hashing/vector_hasher.rs
+-rw-r--r--   0     1001      123     1896 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/lib.rs
+-rw-r--r--   0     1001      123    15733 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/named_from.rs
+-rw-r--r--   0     1001      123     2411 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/prelude.rs
+-rw-r--r--   0     1001      123    16652 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/schema.rs
+-rw-r--r--   0     1001      123     4218 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/serde/chunked_array.rs
+-rw-r--r--   0     1001      123     6551 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/serde/mod.rs
+-rw-r--r--   0     1001      123     9929 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/serde/series.rs
+-rw-r--r--   0     1001      123    18441 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/series/any_value.rs
+-rw-r--r--   0     1001      123    28511 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/series/arithmetic/borrowed.rs
+-rw-r--r--   0     1001      123      222 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/series/arithmetic/mod.rs
+-rw-r--r--   0     1001      123     3546 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/series/arithmetic/owned.rs
+-rw-r--r--   0     1001      123    13187 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/series/comparison.rs
+-rw-r--r--   0     1001      123    25008 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/series/from.rs
+-rw-r--r--   0     1001      123     9217 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/series/implementations/binary.rs
+-rw-r--r--   0     1001      123    10850 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/series/implementations/boolean.rs
+-rw-r--r--   0     1001      123    12962 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/series/implementations/categorical.rs
+-rw-r--r--   0     1001      123    18304 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/series/implementations/dates_time.rs
+-rw-r--r--   0     1001      123    15242 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/series/implementations/datetime.rs
+-rw-r--r--   0     1001      123     5829 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/series/implementations/decimal.rs
+-rw-r--r--   0     1001      123    14917 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/series/implementations/duration.rs
+-rw-r--r--   0     1001      123    14223 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/series/implementations/floats.rs
+-rw-r--r--   0     1001      123     6207 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/series/implementations/list.rs
+-rw-r--r--   0     1001      123    18305 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/series/implementations/mod.rs
+-rw-r--r--   0     1001      123     5336 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/series/implementations/null.rs
+-rw-r--r--   0     1001      123     8004 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/series/implementations/object.rs
+-rw-r--r--   0     1001      123    11029 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/series/implementations/struct_.rs
+-rw-r--r--   0     1001      123     9735 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/series/implementations/utf8.rs
+-rw-r--r--   0     1001      123     4471 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/series/into.rs
+-rw-r--r--   0     1001      123     6297 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/series/iterator.rs
+-rw-r--r--   0     1001      123    37684 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/series/mod.rs
+-rw-r--r--   0     1001      123      853 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/series/ops/diff.rs
+-rw-r--r--   0     1001      123     5204 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/series/ops/downcast.rs
+-rw-r--r--   0     1001      123     3601 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/series/ops/ewm.rs
+-rw-r--r--   0     1001      123      413 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/series/ops/extend.rs
+-rw-r--r--   0     1001      123      562 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/series/ops/mod.rs
+-rw-r--r--   0     1001      123     5974 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/series/ops/moment.rs
+-rw-r--r--   0     1001      123     2908 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/series/ops/null.rs
+-rw-r--r--   0     1001      123     1347 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/series/ops/pct_change.rs
+-rw-r--r--   0     1001      123     4247 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/series/ops/round.rs
+-rw-r--r--   0     1001      123     5072 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/series/ops/to_list.rs
+-rw-r--r--   0     1001      123     1476 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/series/ops/unique.rs
+-rw-r--r--   0     1001      123    18204 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/series/series_trait.rs
+-rw-r--r--   0     1001      123     2840 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/series/unstable.rs
+-rw-r--r--   0     1001      123     8117 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/testing.rs
+-rw-r--r--   0     1001      123      508 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/tests.rs
+-rw-r--r--   0     1001      123     2494 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/utils/flatten.rs
+-rw-r--r--   0     1001      123    31704 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/utils/mod.rs
+-rw-r--r--   0     1001      123     1646 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/utils/series.rs
+-rw-r--r--   0     1001      123    13773 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-core/src/utils/supertype.rs
+-rw-r--r--   0        0        0     1431 1970-01-01 00:00:00.000000 polars_u64_idx-0.17.9/local_dependencies/polars-arrow/Cargo.toml
+-rw-r--r--   0     1001      123     1055 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-arrow/LICENSE
+-rw-r--r--   0     1001      123     1975 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-arrow/src/array/default_arrays.rs
+-rw-r--r--   0     1001      123     3160 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-arrow/src/array/get.rs
+-rw-r--r--   0     1001      123     6459 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-arrow/src/array/list.rs
+-rw-r--r--   0     1001      123     7771 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-arrow/src/array/mod.rs
+-rw-r--r--   0     1001      123      878 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-arrow/src/array/null.rs
+-rw-r--r--   0     1001      123     1125 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-arrow/src/array/slice.rs
+-rw-r--r--   0     1001      123     1807 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-arrow/src/array/utf8.rs
+-rw-r--r--   0     1001      123     2294 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-arrow/src/bit_util.rs
+-rw-r--r--   0     1001      123       17 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-arrow/src/bitmap/mod.rs
+-rw-r--r--   0     1001      123      819 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-arrow/src/bitmap/mutable.rs
+-rw-r--r--   0     1001      123      232 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-arrow/src/compute/cast.rs
+-rw-r--r--   0     1001      123       56 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-arrow/src/compute/mod.rs
+-rw-r--r--   0     1001      123     2962 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-arrow/src/compute/take/boolean.rs
+-rw-r--r--   0     1001      123    24907 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-arrow/src/compute/take/mod.rs
+-rw-r--r--   0     1001      123     1042 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-arrow/src/conversion.rs
+-rw-r--r--   0     1001      123     1609 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-arrow/src/data_types.rs
+-rw-r--r--   0     1001      123       25 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-arrow/src/error.rs
+-rw-r--r--   0     1001      123       28 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-arrow/src/export.rs
+-rw-r--r--   0     1001      123       26 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-arrow/src/floats/mod.rs
+-rw-r--r--   0     1001      123     2066 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-arrow/src/floats/ord.rs
+-rw-r--r--   0     1001      123     1273 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-arrow/src/index.rs
+-rw-r--r--   0     1001      123      915 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-arrow/src/is_valid.rs
+-rw-r--r--   0     1001      123     4740 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-arrow/src/kernels/agg_mean.rs
+-rw-r--r--   0     1001      123     1015 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-arrow/src/kernels/concatenate.rs
+-rw-r--r--   0     1001      123     5161 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-arrow/src/kernels/ewm/average.rs
+-rw-r--r--   0     1001      123     1808 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-arrow/src/kernels/ewm/mod.rs
+-rw-r--r--   0     1001      123    25065 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-arrow/src/kernels/ewm/variance.rs
+-rw-r--r--   0     1001      123     1406 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-arrow/src/kernels/float.rs
+-rw-r--r--   0     1001      123     4907 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-arrow/src/kernels/list.rs
+-rw-r--r--   0     1001      123     1895 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-arrow/src/kernels/list_bytes_iter.rs
+-rw-r--r--   0     1001      123     9731 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-arrow/src/kernels/mod.rs
+-rw-r--r--   0     1001      123     3703 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-arrow/src/kernels/rolling/mod.rs
+-rw-r--r--   0     1001      123     2022 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/mean.rs
+-rw-r--r--   0     1001      123    18684 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/min_max.rs
+-rw-r--r--   0     1001      123     3924 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/mod.rs
+-rw-r--r--   0     1001      123    11659 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/quantile.rs
+-rw-r--r--   0     1001      123     5504 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/sum.rs
+-rw-r--r--   0     1001      123     8683 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/variance.rs
+-rw-r--r--   0     1001      123     1749 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-arrow/src/kernels/rolling/nulls/mean.rs
+-rw-r--r--   0     1001      123    14367 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-arrow/src/kernels/rolling/nulls/min_max.rs
+-rw-r--r--   0     1001      123     9070 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-arrow/src/kernels/rolling/nulls/mod.rs
+-rw-r--r--   0     1001      123    11609 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-arrow/src/kernels/rolling/nulls/quantile.rs
+-rw-r--r--   0     1001      123     4698 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-arrow/src/kernels/rolling/nulls/sum.rs
+-rw-r--r--   0     1001      123     8335 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-arrow/src/kernels/rolling/nulls/variance.rs
+-rw-r--r--   0     1001      123     8109 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-arrow/src/kernels/rolling/window.rs
+-rw-r--r--   0     1001      123     4752 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-arrow/src/kernels/set.rs
+-rw-r--r--   0     1001      123     4529 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-arrow/src/kernels/sort_partition.rs
+-rw-r--r--   0     1001      123     2948 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-arrow/src/kernels/sorted_join/inner.rs
+-rw-r--r--   0     1001      123     5974 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-arrow/src/kernels/sorted_join/left.rs
+-rw-r--r--   0     1001      123      231 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-arrow/src/kernels/sorted_join/mod.rs
+-rw-r--r--   0     1001      123      841 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-arrow/src/kernels/string.rs
+-rw-r--r--   0     1001      123     2310 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-arrow/src/kernels/take_agg/boolean.rs
+-rw-r--r--   0     1001      123     4343 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-arrow/src/kernels/take_agg/mod.rs
+-rw-r--r--   0     1001      123     2606 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-arrow/src/kernels/take_agg/var.rs
+-rw-r--r--   0     1001      123     4417 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-arrow/src/kernels/time.rs
+-rw-r--r--   0     1001      123      341 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-arrow/src/lib.rs
+-rw-r--r--   0     1001      123      434 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-arrow/src/prelude.rs
+-rw-r--r--   0     1001      123      534 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-arrow/src/slice.rs
+-rw-r--r--   0     1001      123      762 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-arrow/src/time_zone.rs
+-rw-r--r--   0     1001      123      998 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-arrow/src/trusted_len/boolean.rs
+-rw-r--r--   0     1001      123     2821 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-arrow/src/trusted_len/mod.rs
+-rw-r--r--   0     1001      123     2533 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-arrow/src/trusted_len/push_unchecked.rs
+-rw-r--r--   0     1001      123      158 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-arrow/src/trusted_len/rev.rs
+-rw-r--r--   0     1001      123     5232 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-arrow/src/utils.rs
+-rw-r--r--   0        0        0      879 1970-01-01 00:00:00.000000 polars_u64_idx-0.17.9/local_dependencies/polars-error/Cargo.toml
+-rw-r--r--   0     1001      123     1055 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-error/LICENSE
+-rw-r--r--   0     1001      123     6297 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-error/src/lib.rs
+-rw-r--r--   0        0        0      994 1970-01-01 00:00:00.000000 polars_u64_idx-0.17.9/local_dependencies/polars-sql/Cargo.toml
+-rw-r--r--   0     1001      123     1055 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-sql/LICENSE
+-rw-r--r--   0     1001      123    16037 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-sql/src/context.rs
+-rw-r--r--   0     1001      123    20245 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-sql/src/functions.rs
+-rw-r--r--   0     1001      123     1920 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-sql/src/keywords.rs
+-rw-r--r--   0     1001      123      211 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-sql/src/lib.rs
+-rw-r--r--   0     1001      123    15240 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-sql/src/sql_expr.rs
+-rw-r--r--   0     1001      123     4572 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-sql/src/table_functions.rs
+-rw-r--r--   0     1001      123     1682 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-sql/tests/functions_cumulative.rs
+-rw-r--r--   0     1001      123     3063 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-sql/tests/functions_io.rs
+-rw-r--r--   0     1001      123     1539 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-sql/tests/functions_math.rs
+-rw-r--r--   0     1001      123     2982 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-sql/tests/functions_string.rs
+-rw-r--r--   0     1001      123     1056 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-sql/tests/iss_7436.rs
+-rw-r--r--   0     1001      123      888 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-sql/tests/iss_7437.rs
+-rw-r--r--   0     1001      123      652 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-sql/tests/iss_7440.rs
+-rw-r--r--   0     1001      123      700 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-sql/tests/iss_8395.rs
+-rw-r--r--   0     1001      123     1062 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-sql/tests/iss_8419.rs
+-rw-r--r--   0     1001      123    14296 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-sql/tests/simple_exprs.rs
+-rw-r--r--   0        0        0      940 1970-01-01 00:00:00.000000 polars_u64_idx-0.17.9/local_dependencies/polars-row/Cargo.toml
+-rw-r--r--   0     1001      123     1055 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-row/LICENSE
+-rw-r--r--   0     1001      123     8985 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-row/src/encode.rs
+-rw-r--r--   0     1001      123     4591 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-row/src/encodings/fixed.rs
+-rw-r--r--   0     1001      123       47 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-row/src/encodings/mod.rs
+-rw-r--r--   0     1001      123     4508 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-row/src/encodings/variable.rs
+-rw-r--r--   0     1001      123    13678 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-row/src/lib.rs
+-rw-r--r--   0     1001      123     2079 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-row/src/row.rs
+-rw-r--r--   0     1001      123      682 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-row/src/utils.rs
+-rw-r--r--   0        0        0    10541 1970-01-01 00:00:00.000000 polars_u64_idx-0.17.9/local_dependencies/polars/Cargo.toml
+-rw-r--r--   0     1001      123     1055 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars/LICENSE
+-rw-r--r--   0     1001      123     3592 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars/Makefile
+-rw-r--r--   0     1001      123      215 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars/build.rs
+-rw-r--r--   0     1001      123       78 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars/clippy.toml
+-rw-r--r--   0     1001      123    17602 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars/src/docs/eager.rs
+-rw-r--r--   0     1001      123     8778 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars/src/docs/lazy.rs
+-rw-r--r--   0     1001      123       50 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars/src/docs/mod.rs
+-rw-r--r--   0     1001      123     3797 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars/src/docs/performance.rs
+-rw-r--r--   0     1001      123       59 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars/src/export.rs
+-rw-r--r--   0     1001      123    20207 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars/src/lib.rs
+-rw-r--r--   0     1001      123      387 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars/src/prelude.rs
+-rw-r--r--   0     1001      123       44 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars/src/sql.rs
+-rw-r--r--   0     1001      123     4272 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars/tests/it/core/date_like.rs
+-rw-r--r--   0     1001      123     2401 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars/tests/it/core/groupby.rs
+-rw-r--r--   0     1001      123    17826 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars/tests/it/core/joins.rs
+-rw-r--r--   0     1001      123      545 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars/tests/it/core/list.rs
+-rw-r--r--   0     1001      123      189 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars/tests/it/core/mod.rs
+-rw-r--r--   0     1001      123     6258 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars/tests/it/core/pivot.rs
+-rw-r--r--   0     1001      123     1102 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars/tests/it/core/random.rs
+-rw-r--r--   0     1001      123    10844 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars/tests/it/core/rolling_window.rs
+-rw-r--r--   0     1001      123     1093 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars/tests/it/core/series.rs
+-rw-r--r--   0     1001      123      370 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars/tests/it/core/utils.rs
+-rw-r--r--   0     1001      123    30013 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars/tests/it/io/csv.rs
+-rw-r--r--   0     1001      123     4490 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars/tests/it/io/ipc_stream.rs
+-rw-r--r--   0     1001      123     7044 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars/tests/it/io/json.rs
+-rw-r--r--   0     1001      123      378 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars/tests/it/io/mod.rs
+-rw-r--r--   0     1001      123      988 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars/tests/it/io/parquet.rs
+-rw-r--r--   0     1001      123     1530 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars/tests/it/joins.rs
+-rw-r--r--   0     1001      123     2452 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars/tests/it/lazy/aggregation.rs
+-rw-r--r--   0     1001      123      702 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars/tests/it/lazy/cse.rs
+-rw-r--r--   0     1001      123      500 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars/tests/it/lazy/explodes.rs
+-rw-r--r--   0     1001      123     2279 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars/tests/it/lazy/expressions/apply.rs
+-rw-r--r--   0     1001      123    10285 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars/tests/it/lazy/expressions/arity.rs
+-rw-r--r--   0     1001      123     1064 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars/tests/it/lazy/expressions/expand.rs
+-rw-r--r--   0     1001      123     1008 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars/tests/it/lazy/expressions/filter.rs
+-rw-r--r--   0     1001      123      428 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars/tests/it/lazy/expressions/is_in.rs
+-rw-r--r--   0     1001      123      121 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars/tests/it/lazy/expressions/mod.rs
+-rw-r--r--   0     1001      123      659 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars/tests/it/lazy/expressions/slice.rs
+-rw-r--r--   0     1001      123    10139 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars/tests/it/lazy/expressions/window.rs
+-rw-r--r--   0     1001      123      579 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars/tests/it/lazy/folds.rs
+-rw-r--r--   0     1001      123      557 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars/tests/it/lazy/functions.rs
+-rw-r--r--   0     1001      123     4482 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars/tests/it/lazy/groupby.rs
+-rw-r--r--   0     1001      123     1655 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars/tests/it/lazy/groupby_dynamic.rs
+-rw-r--r--   0     1001      123      691 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars/tests/it/lazy/mod.rs
+-rw-r--r--   0     1001      123     5381 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars/tests/it/lazy/predicate_queries.rs
+-rw-r--r--   0     1001      123     4476 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars/tests/it/lazy/projection_queries.rs
+-rw-r--r--   0     1001      123     6444 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars/tests/it/lazy/queries.rs
+-rw-r--r--   0     1001      123      141 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars/tests/it/main.rs
+-rw-r--r--   0     1001      123    12591 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars/tests/it/schema.rs
+-rw-r--r--   0        0        0     5241 1970-01-01 00:00:00.000000 polars_u64_idx-0.17.9/local_dependencies/polars-plan/Cargo.toml
+-rw-r--r--   0     1001      123     1055 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-plan/LICENSE
+-rw-r--r--   0     1001      123       45 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/constants.rs
+-rw-r--r--   0     1001      123    17248 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/dot.rs
+-rw-r--r--   0     1001      123     4171 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/dsl/arithmetic.rs
+-rw-r--r--   0     1001      123      935 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/dsl/binary.rs
+-rw-r--r--   0     1001      123      650 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/dsl/cat.rs
+-rw-r--r--   0     1001      123     9880 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/dsl/dt.rs
+-rw-r--r--   0     1001      123    13169 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/dsl/expr.rs
+-rw-r--r--   0     1001      123      753 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/dsl/from.rs
+-rw-r--r--   0     1001      123       85 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/dsl/function_expr/abs.rs
+-rw-r--r--   0     1001      123     1431 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/dsl/function_expr/arg_where.rs
+-rw-r--r--   0     1001      123     1327 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/dsl/function_expr/binary.rs
+-rw-r--r--   0     1001      123     4221 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/dsl/function_expr/boolean.rs
+-rw-r--r--   0     1001      123     1910 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/dsl/function_expr/bounds.rs
+-rw-r--r--   0     1001      123     1216 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/dsl/function_expr/cat.rs
+-rw-r--r--   0     1001      123      344 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/dsl/function_expr/clip.rs
+-rw-r--r--   0     1001      123     1593 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/dsl/function_expr/cum.rs
+-rw-r--r--   0     1001      123    15231 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/dsl/function_expr/datetime.rs
+-rw-r--r--   0     1001      123      810 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/dsl/function_expr/dispatch.rs
+-rw-r--r--   0     1001      123     2541 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/dsl/function_expr/fill_null.rs
+-rw-r--r--   0     1001      123     8119 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/dsl/function_expr/list.rs
+-rw-r--r--   0     1001      123      581 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/dsl/function_expr/log.rs
+-rw-r--r--   0     1001      123    19416 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/dsl/function_expr/mod.rs
+-rw-r--r--   0     1001      123      462 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/dsl/function_expr/nan.rs
+-rw-r--r--   0     1001      123     3132 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/dsl/function_expr/pow.rs
+-rw-r--r--   0     1001      123      152 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/dsl/function_expr/rolling.rs
+-rw-r--r--   0     1001      123      260 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/dsl/function_expr/round.rs
+-rw-r--r--   0     1001      123      200 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/dsl/function_expr/row_hash.rs
+-rw-r--r--   0     1001      123    13668 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/dsl/function_expr/schema.rs
+-rw-r--r--   0     1001      123      306 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/dsl/function_expr/search_sorted.rs
+-rw-r--r--   0     1001      123     3812 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/dsl/function_expr/shift_and_fill.rs
+-rw-r--r--   0     1001      123     1238 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/dsl/function_expr/shrink_type.rs
+-rw-r--r--   0     1001      123      972 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/dsl/function_expr/sign.rs
+-rw-r--r--   0     1001      123    19923 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/dsl/function_expr/strings.rs
+-rw-r--r--   0     1001      123     1017 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/dsl/function_expr/struct_.rs
+-rw-r--r--   0     1001      123     3010 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/dsl/function_expr/temporal.rs
+-rw-r--r--   0     1001      123     5122 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/dsl/function_expr/trigonometry.rs
+-rw-r--r--   0     1001      123      170 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/dsl/function_expr/unique.rs
+-rw-r--r--   0     1001      123    43864 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/dsl/functions.rs
+-rw-r--r--   0     1001      123    10196 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/dsl/list.rs
+-rw-r--r--   0     1001      123     2181 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/dsl/meta.rs
+-rw-r--r--   0     1001      123    64804 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/dsl/mod.rs
+-rw-r--r--   0     1001      123       40 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/dsl/names.rs
+-rw-r--r--   0     1001      123     2100 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/dsl/options.rs
+-rw-r--r--   0     1001      123    15238 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/dsl/string.rs
+-rw-r--r--   0     1001      123     2715 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/dsl/struct_.rs
+-rw-r--r--   0     1001      123       38 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/frame/mod.rs
+-rw-r--r--   0     1001      123      933 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/frame/opt_state.rs
+-rw-r--r--   0     1001      123      466 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/global.rs
+-rw-r--r--   0     1001      123      175 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/lib.rs
+-rw-r--r--   0     1001      123     6825 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/logical_plan/aexpr/mod.rs
+-rw-r--r--   0     1001      123    11393 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/logical_plan/aexpr/schema.rs
+-rw-r--r--   0     1001      123    25656 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/logical_plan/alp.rs
+-rw-r--r--   0     1001      123     1622 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/logical_plan/anonymous_scan.rs
+-rw-r--r--   0     1001      123     1428 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/logical_plan/apply.rs
+-rw-r--r--   0     1001      123    24898 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/logical_plan/builder.rs
+-rw-r--r--   0     1001      123    29652 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/logical_plan/conversion.rs
+-rw-r--r--   0     1001      123      301 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/logical_plan/debug.rs
+-rw-r--r--   0     1001      123    15191 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/logical_plan/format.rs
+-rw-r--r--   0     1001      123      895 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/logical_plan/functions/drop.rs
+-rw-r--r--   0     1001      123      137 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/logical_plan/functions/explode.rs
+-rw-r--r--   0     1001      123     1169 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/logical_plan/functions/merge_sorted.rs
+-rw-r--r--   0     1001      123    11905 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/logical_plan/functions/mod.rs
+-rw-r--r--   0     1001      123     1330 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/logical_plan/functions/rename.rs
+-rw-r--r--   0     1001      123     9752 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/logical_plan/iterator.rs
+-rw-r--r--   0     1001      123    10463 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/logical_plan/lit.rs
+-rw-r--r--   0     1001      123     8115 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/logical_plan/mod.rs
+-rw-r--r--   0     1001      123     7416 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/logical_plan/optimizer/cache_states.rs
+-rw-r--r--   0     1001      123    15277 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/logical_plan/optimizer/cse.rs
+-rw-r--r--   0     1001      123     3250 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/logical_plan/optimizer/delay_rechunk.rs
+-rw-r--r--   0     1001      123     3236 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/logical_plan/optimizer/drop_nulls.rs
+-rw-r--r--   0     1001      123     3994 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/logical_plan/optimizer/fast_projection.rs
+-rw-r--r--   0     1001      123    14479 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/logical_plan/optimizer/file_caching.rs
+-rw-r--r--   0     1001      123     1556 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/logical_plan/optimizer/flatten_union.rs
+-rw-r--r--   0     1001      123     6644 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/logical_plan/optimizer/mod.rs
+-rw-r--r--   0     1001      123     1222 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/logical_plan/optimizer/predicate_pushdown/keys.rs
+-rw-r--r--   0     1001      123    28276 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/logical_plan/optimizer/predicate_pushdown/mod.rs
+-rw-r--r--   0     1001      123     2571 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/logical_plan/optimizer/predicate_pushdown/rename.rs
+-rw-r--r--   0     1001      123    15130 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/logical_plan/optimizer/predicate_pushdown/utils.rs
+-rw-r--r--   0     1001      123     1755 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/functions/melt.rs
+-rw-r--r--   0     1001      123     3930 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/functions/mod.rs
+-rw-r--r--   0     1001      123     1799 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/generic.rs
+-rw-r--r--   0     1001      123     3269 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/groupby.rs
+-rw-r--r--   0     1001      123     2638 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/hstack.rs
+-rw-r--r--   0     1001      123    15747 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/joins.rs
+-rw-r--r--   0     1001      123    26502 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/mod.rs
+-rw-r--r--   0     1001      123     3707 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/projection.rs
+-rw-r--r--   0     1001      123     2639 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/rename.rs
+-rw-r--r--   0     1001      123     3501 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/semi_anti_join.rs
+-rw-r--r--   0     1001      123    27361 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/logical_plan/optimizer/simplify_expr.rs
+-rw-r--r--   0     1001      123     3492 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/logical_plan/optimizer/slice_pushdown_expr.rs
+-rw-r--r--   0     1001      123    13845 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/logical_plan/optimizer/slice_pushdown_lp.rs
+-rw-r--r--   0     1001      123     3161 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/logical_plan/optimizer/stack_opt.rs
+-rw-r--r--   0     1001      123     9725 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/logical_plan/optimizer/type_coercion/binary.rs
+-rw-r--r--   0     1001      123    19820 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/logical_plan/optimizer/type_coercion/mod.rs
+-rw-r--r--   0     1001      123    10187 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/logical_plan/options.rs
+-rw-r--r--   0     1001      123    15276 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/logical_plan/projection.rs
+-rw-r--r--   0     1001      123     4584 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/logical_plan/pyarrow.rs
+-rw-r--r--   0     1001      123    13038 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/logical_plan/schema.rs
+-rw-r--r--   0     1001      123      809 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/prelude.rs
+-rw-r--r--   0     1001      123    11879 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/utils.rs
+-rw-r--r--   0        0        0     2055 1970-01-01 00:00:00.000000 polars_u64_idx-0.17.9/local_dependencies/polars-time/Cargo.toml
+-rw-r--r--   0     1001      123     1055 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-time/LICENSE
+-rw-r--r--   0     1001      123     3565 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-time/src/chunkedarray/date.rs
+-rw-r--r--   0     1001      123     6465 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-time/src/chunkedarray/datetime.rs
+-rw-r--r--   0     1001      123     3305 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-time/src/chunkedarray/duration.rs
+-rw-r--r--   0     1001      123     5607 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-time/src/chunkedarray/kernels.rs
+-rw-r--r--   0     1001      123     1062 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-time/src/chunkedarray/mod.rs
+-rw-r--r--   0     1001      123     7302 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-time/src/chunkedarray/rolling_window/floats.rs
+-rw-r--r--   0     1001      123     2582 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-time/src/chunkedarray/rolling_window/ints.rs
+-rw-r--r--   0     1001      123    10495 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-time/src/chunkedarray/rolling_window/mod.rs
+-rw-r--r--   0     1001      123      428 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-time/src/chunkedarray/rolling_window/rolling_kernels/mod.rs
+-rw-r--r--   0     1001      123     7642 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-time/src/chunkedarray/rolling_window/rolling_kernels/no_nulls.rs
+-rw-r--r--   0     1001      123     2717 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-time/src/chunkedarray/time.rs
+-rw-r--r--   0     1001      123    21192 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-time/src/chunkedarray/utf8/infer.rs
+-rw-r--r--   0     1001      123    20108 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-time/src/chunkedarray/utf8/mod.rs
+-rw-r--r--   0     1001      123     4115 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-time/src/chunkedarray/utf8/patterns.rs
+-rw-r--r--   0     1001      123     9692 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-time/src/chunkedarray/utf8/strptime.rs
+-rw-r--r--   0     1001      123     2960 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-time/src/date_range.rs
+-rw-r--r--   0     1001      123    31843 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-time/src/groupby/dynamic.rs
+-rw-r--r--   0     1001      123       88 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-time/src/groupby/mod.rs
+-rw-r--r--   0     1001      123      613 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-time/src/lib.rs
+-rw-r--r--   0     1001      123     3080 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-time/src/month_end.rs
+-rw-r--r--   0     1001      123     3468 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-time/src/month_start.rs
+-rw-r--r--   0     1001      123      320 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-time/src/prelude.rs
+-rw-r--r--   0     1001      123     1568 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-time/src/round.rs
+-rw-r--r--   0     1001      123     4028 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-time/src/series/_trait.rs
+-rw-r--r--   0     1001      123      136 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-time/src/series/implementations/boolean.rs
+-rw-r--r--   0     1001      123      140 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-time/src/series/implementations/categoricals.rs
+-rw-r--r--   0     1001      123      133 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-time/src/series/implementations/date.rs
+-rw-r--r--   0     1001      123      137 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-time/src/series/implementations/datetime.rs
+-rw-r--r--   0     1001      123      137 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-time/src/series/implementations/duration.rs
+-rw-r--r--   0     1001      123     1863 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-time/src/series/implementations/floats.rs
+-rw-r--r--   0     1001      123     1792 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-time/src/series/implementations/integers.rs
+-rw-r--r--   0     1001      123      133 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-time/src/series/implementations/list.rs
+-rw-r--r--   0     1001      123      486 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-time/src/series/implementations/mod.rs
+-rw-r--r--   0     1001      123      155 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-time/src/series/implementations/object.rs
+-rw-r--r--   0     1001      123      135 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-time/src/series/implementations/struct_.rs
+-rw-r--r--   0     1001      123      133 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-time/src/series/implementations/time.rs
+-rw-r--r--   0     1001      123      133 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-time/src/series/implementations/utf8.rs
+-rw-r--r--   0     1001      123    12466 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-time/src/series/mod.rs
+-rw-r--r--   0     1001      123     1630 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-time/src/truncate.rs
+-rw-r--r--   0     1001      123     7308 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-time/src/upsample.rs
+-rw-r--r--   0     1001      123     2567 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-time/src/utils.rs
+-rw-r--r--   0     1001      123     1524 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-time/src/windows/bounds.rs
+-rw-r--r--   0     1001      123     2650 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-time/src/windows/calendar.rs
+-rw-r--r--   0     1001      123    25110 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-time/src/windows/duration.rs
+-rw-r--r--   0     1001      123    19317 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-time/src/windows/groupby.rs
+-rw-r--r--   0     1001      123      503 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-time/src/windows/mod.rs
+-rw-r--r--   0     1001      123    24372 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-time/src/windows/test.rs
+-rw-r--r--   0     1001      123    11624 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-time/src/windows/window.rs
+-rw-r--r--   0        0        0     5977 1970-01-01 00:00:00.000000 polars_u64_idx-0.17.9/local_dependencies/polars-lazy/Cargo.toml
+-rw-r--r--   0     1001      123     1055 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-lazy/LICENSE
+-rw-r--r--   0     1001      123     1796 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-lazy/src/dot.rs
+-rw-r--r--   0     1001      123     4359 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-lazy/src/dsl/eval.rs
+-rw-r--r--   0     1001      123     4505 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-lazy/src/dsl/functions.rs
+-rw-r--r--   0     1001      123      164 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-lazy/src/dsl/into.rs
+-rw-r--r--   0     1001      123     6754 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-lazy/src/dsl/list.rs
+-rw-r--r--   0     1001      123     2899 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-lazy/src/dsl/mod.rs
+-rw-r--r--   0     1001      123     1182 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-lazy/src/frame/anonymous_scan.rs
+-rw-r--r--   0     1001      123     9278 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-lazy/src/frame/csv.rs
+-rw-r--r--   0     1001      123     4309 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-lazy/src/frame/file_list_reader.rs
+-rw-r--r--   0     1001      123     2261 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-lazy/src/frame/ipc.rs
+-rw-r--r--   0     1001      123    47176 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-lazy/src/frame/mod.rs
+-rw-r--r--   0     1001      123     3414 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-lazy/src/frame/ndjson.rs
+-rw-r--r--   0     1001      123     3440 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-lazy/src/frame/parquet.rs
+-rw-r--r--   0     1001      123     2892 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-lazy/src/frame/pivot.rs
+-rw-r--r--   0     1001      123      416 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-lazy/src/frame/python.rs
+-rw-r--r--   0     1001      123     6376 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-lazy/src/lib.rs
+-rw-r--r--   0     1001      123     1049 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-lazy/src/physical_plan/executors/cache.rs
+-rw-r--r--   0     1001      123      776 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-lazy/src/physical_plan/executors/executor.rs
+-rw-r--r--   0     1001      123      670 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-lazy/src/physical_plan/executors/ext_context.rs
+-rw-r--r--   0     1001      123     1284 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-lazy/src/physical_plan/executors/filter.rs
+-rw-r--r--   0     1001      123     3908 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-lazy/src/physical_plan/executors/groupby.rs
+-rw-r--r--   0     1001      123     3577 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-lazy/src/physical_plan/executors/groupby_dynamic.rs
+-rw-r--r--   0     1001      123    13439 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-lazy/src/physical_plan/executors/groupby_partitioned.rs
+-rw-r--r--   0     1001      123     4335 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-lazy/src/physical_plan/executors/groupby_rolling.rs
+-rw-r--r--   0     1001      123     6058 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-lazy/src/physical_plan/executors/join.rs
+-rw-r--r--   0     1001      123     7074 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-lazy/src/physical_plan/executors/mod.rs
+-rw-r--r--   0     1001      123     2045 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-lazy/src/physical_plan/executors/projection.rs
+-rw-r--r--   0     1001      123     1677 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-lazy/src/physical_plan/executors/python_scan.rs
+-rw-r--r--   0     1001      123     2986 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-lazy/src/physical_plan/executors/scan/csv.rs
+-rw-r--r--   0     1001      123     1963 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-lazy/src/physical_plan/executors/scan/ipc.rs
+-rw-r--r--   0     1001      123     4151 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-lazy/src/physical_plan/executors/scan/mod.rs
+-rw-r--r--   0     1001      123     1208 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-lazy/src/physical_plan/executors/scan/ndjson.rs
+-rw-r--r--   0     1001      123     2421 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-lazy/src/physical_plan/executors/scan/parquet.rs
+-rw-r--r--   0     1001      123      548 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-lazy/src/physical_plan/executors/slice.rs
+-rw-r--r--   0     1001      123     2197 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-lazy/src/physical_plan/executors/sort.rs
+-rw-r--r--   0     1001      123     1922 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-lazy/src/physical_plan/executors/stack.rs
+-rw-r--r--   0     1001      123      663 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-lazy/src/physical_plan/executors/udf.rs
+-rw-r--r--   0     1001      123     3702 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-lazy/src/physical_plan/executors/union.rs
+-rw-r--r--   0     1001      123      838 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-lazy/src/physical_plan/executors/unique.rs
+-rw-r--r--   0     1001      123     1284 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-lazy/src/physical_plan/exotic.rs
+-rw-r--r--   0     1001      123    21873 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-lazy/src/physical_plan/expressions/aggregation.rs
+-rw-r--r--   0     1001      123     2689 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-lazy/src/physical_plan/expressions/alias.rs
+-rw-r--r--   0     1001      123    17432 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-lazy/src/physical_plan/expressions/apply.rs
+-rw-r--r--   0     1001      123    17488 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-lazy/src/physical_plan/expressions/binary.rs
+-rw-r--r--   0     1001      123     3153 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-lazy/src/physical_plan/expressions/cast.rs
+-rw-r--r--   0     1001      123     6326 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-lazy/src/physical_plan/expressions/column.rs
+-rw-r--r--   0     1001      123     2003 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-lazy/src/physical_plan/expressions/count.rs
+-rw-r--r--   0     1001      123     5809 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-lazy/src/physical_plan/expressions/filter.rs
+-rw-r--r--   0     1001      123     4131 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-lazy/src/physical_plan/expressions/group_iter.rs
+-rw-r--r--   0     1001      123     5304 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-lazy/src/physical_plan/expressions/literal.rs
+-rw-r--r--   0     1001      123    21175 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-lazy/src/physical_plan/expressions/mod.rs
+-rw-r--r--   0     1001      123    10091 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-lazy/src/physical_plan/expressions/slice.rs
+-rw-r--r--   0     1001      123     3929 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-lazy/src/physical_plan/expressions/sort.rs
+-rw-r--r--   0     1001      123    11541 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-lazy/src/physical_plan/expressions/sortby.rs
+-rw-r--r--   0     1001      123     8331 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-lazy/src/physical_plan/expressions/take.rs
+-rw-r--r--   0     1001      123    14360 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-lazy/src/physical_plan/expressions/ternary.rs
+-rw-r--r--   0     1001      123    32007 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-lazy/src/physical_plan/expressions/window.rs
+-rw-r--r--   0     1001      123     2039 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-lazy/src/physical_plan/file_cache.rs
+-rw-r--r--   0     1001      123      414 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-lazy/src/physical_plan/mod.rs
+-rw-r--r--   0     1001      123     2005 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-lazy/src/physical_plan/node_timer.rs
+-rw-r--r--   0     1001      123    27366 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-lazy/src/physical_plan/planner/expr.rs
+-rw-r--r--   0     1001      123    18862 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-lazy/src/physical_plan/planner/lp.rs
+-rw-r--r--   0     1001      123       87 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-lazy/src/physical_plan/planner/mod.rs
+-rw-r--r--   0     1001      123     9425 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-lazy/src/physical_plan/state.rs
+-rw-r--r--   0     1001      123    20891 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-lazy/src/physical_plan/streaming/convert.rs
+-rw-r--r--   0     1001      123      219 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-lazy/src/physical_plan/streaming/mod.rs
+-rw-r--r--   0     1001      123     3333 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-lazy/src/physical_plan/streaming/tree.rs
+-rw-r--r--   0     1001      123      722 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-lazy/src/prelude.rs
+-rw-r--r--   0     1001      123    14990 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-lazy/src/tests/aggregations.rs
+-rw-r--r--   0     1001      123     2339 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-lazy/src/tests/arity.rs
+-rw-r--r--   0     1001      123     7031 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-lazy/src/tests/cse.rs
+-rw-r--r--   0     1001      123    12749 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-lazy/src/tests/io.rs
+-rw-r--r--   0     1001      123     4207 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-lazy/src/tests/logical.rs
+-rw-r--r--   0     1001      123     4288 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-lazy/src/tests/mod.rs
+-rw-r--r--   0     1001      123    14812 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-lazy/src/tests/optimization_checks.rs
+-rw-r--r--   0     1001      123     6799 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-lazy/src/tests/predicate_queries.rs
+-rw-r--r--   0     1001      123     3158 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-lazy/src/tests/projection_queries.rs
+-rw-r--r--   0     1001      123    47910 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-lazy/src/tests/queries.rs
+-rw-r--r--   0     1001      123     8358 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-lazy/src/tests/streaming.rs
+-rw-r--r--   0     1001      123     2886 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-lazy/src/tests/tpch.rs
+-rw-r--r--   0     1001      123     1028 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-lazy/src/utils.rs
+-rw-r--r--   0        0        0      823 1970-01-01 00:00:00.000000 polars_u64_idx-0.17.9/local_dependencies/polars-algo/Cargo.toml
+-rw-r--r--   0     1001      123     1055 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-algo/LICENSE
+-rw-r--r--   0     1001      123     7477 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-algo/src/algo.rs
+-rw-r--r--   0     1001      123       88 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-algo/src/lib.rs
+-rw-r--r--   0     1001      123       28 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-algo/src/prelude.rs
+-rw-r--r--   0        0        0      476 1970-01-01 00:00:00.000000 polars_u64_idx-0.17.9/local_dependencies/polars-utils/Cargo.toml
+-rw-r--r--   0     1001      123     1055 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-utils/LICENSE
+-rw-r--r--   0     1001      123     2645 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-utils/src/arena.rs
+-rw-r--r--   0     1001      123     1373 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-utils/src/atomic.rs
+-rw-r--r--   0     1001      123     2659 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-utils/src/cell.rs
+-rw-r--r--   0     1001      123     1015 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-utils/src/contention_pool.rs
+-rw-r--r--   0     1001      123      509 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-utils/src/error.rs
+-rw-r--r--   0     1001      123      271 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-utils/src/fmt.rs
+-rw-r--r--   0     1001      123      763 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-utils/src/functions.rs
+-rw-r--r--   0     1001      123      514 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-utils/src/hash.rs
+-rw-r--r--   0     1001      123     2709 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-utils/src/iter/enumerate_idx.rs
+-rw-r--r--   0     1001      123       61 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-utils/src/iter/mod.rs
+-rw-r--r--   0     1001      123      583 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-utils/src/lib.rs
+-rw-r--r--   0     1001      123      573 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-utils/src/macros.rs
+-rw-r--r--   0     1001      123      282 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-utils/src/mem.rs
+-rw-r--r--   0     1001      123     1792 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-utils/src/slice.rs
+-rw-r--r--   0     1001      123     2467 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-utils/src/sort.rs
+-rw-r--r--   0     1001      123     1115 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-utils/src/sync.rs
+-rw-r--r--   0     1001      123      504 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-utils/src/sys.rs
+-rw-r--r--   0     1001      123      697 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-utils/src/unwrap.rs
+-rw-r--r--   0     1001      123      616 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-utils/src/wasm.rs
+-rw-r--r--   0        0        0     4343 1970-01-01 00:00:00.000000 polars_u64_idx-0.17.9/local_dependencies/polars-io/Cargo.toml
+-rw-r--r--   0     1001      123     1055 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-io/LICENSE
+-rw-r--r--   0     1001      123     2383 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-io/src/avro/mod.rs
+-rw-r--r--   0     1001      123     3608 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-io/src/avro/read.rs
+-rw-r--r--   0     1001      123     2622 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-io/src/avro/write.rs
+-rw-r--r--   0     1001      123     4505 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-io/src/cloud/adaptors.rs
+-rw-r--r--   0     1001      123     9506 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-io/src/cloud/glob.rs
+-rw-r--r--   0     1001      123     3089 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-io/src/cloud/mod.rs
+-rw-r--r--   0     1001      123    28678 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-io/src/csv/buffer.rs
+-rw-r--r--   0     1001      123     1898 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-io/src/csv/mod.rs
+-rw-r--r--   0     1001      123    19712 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-io/src/csv/parser.rs
+-rw-r--r--   0     1001      123    21432 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-io/src/csv/read.rs
+-rw-r--r--   0     1001      123    10817 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-io/src/csv/read_impl/batched_mmap.rs
+-rw-r--r--   0     1001      123    13909 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-io/src/csv/read_impl/batched_read.rs
+-rw-r--r--   0     1001      123    31365 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-io/src/csv/read_impl/mod.rs
+-rw-r--r--   0     1001      123    11466 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-io/src/csv/splitfields.rs
+-rw-r--r--   0     1001      123    25183 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-io/src/csv/utils.rs
+-rw-r--r--   0     1001      123     2796 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-io/src/csv/write.rs
+-rw-r--r--   0     1001      123    13265 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-io/src/csv/write_impl.rs
+-rw-r--r--   0     1001      123      184 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-io/src/export.rs
+-rw-r--r--   0     1001      123     7586 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-io/src/ipc/ipc_file.rs
+-rw-r--r--   0     1001      123     9222 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-io/src/ipc/ipc_stream.rs
+-rw-r--r--   0     1001      123     3253 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-io/src/ipc/mmap.rs
+-rw-r--r--   0     1001      123      401 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-io/src/ipc/mod.rs
+-rw-r--r--   0     1001      123     8282 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-io/src/ipc/write.rs
+-rw-r--r--   0     1001      123     1471 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-io/src/ipc/write_async.rs
+-rw-r--r--   0     1001      123    11046 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-io/src/json.rs
+-rw-r--r--   0     1001      123     4864 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-io/src/lib.rs
+-rw-r--r--   0     1001      123     1969 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-io/src/mmap.rs
+-rw-r--r--   0     1001      123     7215 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-io/src/ndjson_core/buffer.rs
+-rw-r--r--   0     1001      123       39 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-io/src/ndjson_core/mod.rs
+-rw-r--r--   0     1001      123    12172 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-io/src/ndjson_core/ndjson.rs
+-rw-r--r--   0     1001      123      273 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-io/src/options.rs
+-rw-r--r--   0     1001      123     7360 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-io/src/parquet/async_impl.rs
+-rw-r--r--   0     1001      123     3093 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-io/src/parquet/mmap.rs
+-rw-r--r--   0     1001      123     3132 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-io/src/parquet/mod.rs
+-rw-r--r--   0     1001      123     4784 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-io/src/parquet/predicates.rs
+-rw-r--r--   0     1001      123     9606 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-io/src/parquet/read.rs
+-rw-r--r--   0     1001      123    16886 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-io/src/parquet/read_impl.rs
+-rw-r--r--   0     1001      123    10106 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-io/src/parquet/write.rs
+-rw-r--r--   0     1001      123     5334 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-io/src/partition.rs
+-rw-r--r--   0     1001      123     1455 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-io/src/predicates.rs
+-rw-r--r--   0     1001      123      628 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-io/src/prelude.rs
+-rw-r--r--   0     1001      123      417 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-io/src/tests.rs
+-rw-r--r--   0     1001      123     4467 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-io/src/utils.rs
+-rw-r--r--   0        0        0     3268 1970-01-01 00:00:00.000000 polars_u64_idx-0.17.9/local_dependencies/polars-ops/Cargo.toml
+-rw-r--r--   0     1001      123     1055 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-ops/LICENSE
+-rw-r--r--   0     1001      123      234 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-ops/src/chunked_array/binary/mod.rs
+-rw-r--r--   0     1001      123     3549 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-ops/src/chunked_array/binary/namespace.rs
+-rw-r--r--   0     1001      123    11023 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-ops/src/chunked_array/interpolate.rs
+-rw-r--r--   0     1001      123     1679 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-ops/src/chunked_array/list/count.rs
+-rw-r--r--   0     1001      123     2452 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-ops/src/chunked_array/list/hash.rs
+-rw-r--r--   0     1001      123     7861 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-ops/src/chunked_array/list/min_max.rs
+-rw-r--r--   0     1001      123      511 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-ops/src/chunked_array/list/mod.rs
+-rw-r--r--   0     1001      123    22005 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-ops/src/chunked_array/list/namespace.rs
+-rw-r--r--   0     1001      123     5269 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-ops/src/chunked_array/list/sum_mean.rs
+-rw-r--r--   0     1001      123     2435 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-ops/src/chunked_array/list/to_struct.rs
+-rw-r--r--   0     1001      123      489 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-ops/src/chunked_array/mod.rs
+-rw-r--r--   0     1001      123     9380 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-ops/src/chunked_array/nan_propagating_aggregate.rs
+-rw-r--r--   0     1001      123     6795 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-ops/src/chunked_array/set.rs
+-rw-r--r--   0     1001      123     7490 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-ops/src/chunked_array/strings/case.rs
+-rw-r--r--   0     1001      123     8251 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-ops/src/chunked_array/strings/json_path.rs
+-rw-r--r--   0     1001      123     2345 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-ops/src/chunked_array/strings/justify.rs
+-rw-r--r--   0     1001      123      514 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-ops/src/chunked_array/strings/mod.rs
+-rw-r--r--   0     1001      123    14731 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-ops/src/chunked_array/strings/namespace.rs
+-rw-r--r--   0     1001      123     4053 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-ops/src/chunked_array/strings/replace.rs
+-rw-r--r--   0     1001      123     2486 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-ops/src/chunked_array/top_k.rs
+-rw-r--r--   0     1001      123     7727 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-ops/src/frame/join/merge_sorted.rs
+-rw-r--r--   0     1001      123    18025 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-ops/src/frame/join/mod.rs
+-rw-r--r--   0     1001      123     4174 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-ops/src/frame/mod.rs
+-rw-r--r--   0     1001      123    10257 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-ops/src/frame/pivot/mod.rs
+-rw-r--r--   0     1001      123    13486 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-ops/src/frame/pivot/positioning.rs
+-rw-r--r--   0     1001      123      217 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-ops/src/lib.rs
+-rw-r--r--   0     1001      123      290 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-ops/src/prelude.rs
+-rw-r--r--   0     1001      123       25 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-ops/src/series/mod.rs
+-rw-r--r--   0     1001      123     9623 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-ops/src/series/ops/approx_algo/hyperloglogplus.rs
+-rw-r--r--   0     1001      123      118 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-ops/src/series/ops/approx_algo/mod.rs
+-rw-r--r--   0     1001      123     2016 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-ops/src/series/ops/approx_unique.rs
+-rw-r--r--   0     1001      123    11872 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-ops/src/series/ops/arg_min_max.rs
+-rw-r--r--   0     1001      123     3688 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-ops/src/series/ops/floor_divide.rs
+-rw-r--r--   0     1001      123     3423 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-ops/src/series/ops/is_first.rs
+-rw-r--r--   0     1001      123     2975 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-ops/src/series/ops/is_unique.rs
+-rw-r--r--   0     1001      123     3626 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-ops/src/series/ops/log.rs
+-rw-r--r--   0     1001      123     1106 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-ops/src/series/ops/mod.rs
+-rw-r--r--   0     1001      123     1769 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-ops/src/series/ops/rolling.rs
+-rw-r--r--   0     1001      123     7642 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-ops/src/series/ops/search_sorted.rs
+-rw-r--r--   0     1001      123     2500 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-ops/src/series/ops/to_dummies.rs
+-rw-r--r--   0     1001      123     2067 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-ops/src/series/ops/various.rs
+-rw-r--r--   0        0        0     1765 1970-01-01 00:00:00.000000 polars_u64_idx-0.17.9/local_dependencies/polars-pipe/Cargo.toml
+-rw-r--r--   0     1001      123     1055 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-pipe/LICENSE
+-rw-r--r--   0     1001      123       98 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-pipe/src/executors/mod.rs
+-rw-r--r--   0     1001      123     1219 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-pipe/src/executors/operators/filter.rs
+-rw-r--r--   0     1001      123     4103 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-pipe/src/executors/operators/function.rs
+-rw-r--r--   0     1001      123      229 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-pipe/src/executors/operators/mod.rs
+-rw-r--r--   0     1001      123      548 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-pipe/src/executors/operators/placeholder.rs
+-rw-r--r--   0     1001      123     3247 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-pipe/src/executors/operators/projection.rs
+-rw-r--r--   0     1001      123     2324 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-pipe/src/executors/operators/reproject.rs
+-rw-r--r--   0     1001      123     6479 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-pipe/src/executors/sinks/file_sink.rs
+-rw-r--r--   0     1001      123    10473 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/convert.rs
+-rw-r--r--   0     1001      123     1207 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/count.rs
+-rw-r--r--   0     1001      123     1888 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/first.rs
+-rw-r--r--   0     1001      123     4554 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/interface.rs
+-rw-r--r--   0     1001      123     1746 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/last.rs
+-rw-r--r--   0     1001      123     5413 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/mean.rs
+-rw-r--r--   0     1001      123     4951 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/min_max.rs
+-rw-r--r--   0     1001      123      211 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/mod.rs
+-rw-r--r--   0     1001      123      856 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/null.rs
+-rw-r--r--   0     1001      123     4294 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/sum.rs
+-rw-r--r--   0     1001      123     3030 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/eval.rs
+-rw-r--r--   0     1001      123     6275 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/global.rs
+-rw-r--r--   0     1001      123    13665 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/hash_table.rs
+-rw-r--r--   0     1001      123     2681 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/mod.rs
+-rw-r--r--   0     1001      123     2534 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/ooc_state.rs
+-rw-r--r--   0     1001      123     5961 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/sink.rs
+-rw-r--r--   0     1001      123    10673 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/thread_local.rs
+-rw-r--r--   0     1001      123     2164 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-pipe/src/executors/sinks/groupby/mod.rs
+-rw-r--r--   0     1001      123     4666 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-pipe/src/executors/sinks/groupby/ooc.rs
+-rw-r--r--   0     1001      123     3906 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-pipe/src/executors/sinks/groupby/ooc_state.rs
+-rw-r--r--   0     1001      123    20859 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-pipe/src/executors/sinks/groupby/primitive/mod.rs
+-rw-r--r--   0     1001      123    23518 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-pipe/src/executors/sinks/groupby/string.rs
+-rw-r--r--   0     1001      123     2457 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-pipe/src/executors/sinks/groupby/utils.rs
+-rw-r--r--   0     1001      123     8395 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-pipe/src/executors/sinks/io.rs
+-rw-r--r--   0     1001      123     5485 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-pipe/src/executors/sinks/joins/cross.rs
+-rw-r--r--   0     1001      123    14279 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-pipe/src/executors/sinks/joins/generic_build.rs
+-rw-r--r--   0     1001      123    11824 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-pipe/src/executors/sinks/joins/inner_left.rs
+-rw-r--r--   0     1001      123      178 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-pipe/src/executors/sinks/joins/mod.rs
+-rw-r--r--   0     1001      123     2002 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-pipe/src/executors/sinks/memory.rs
+-rw-r--r--   0     1001      123      589 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-pipe/src/executors/sinks/mod.rs
+-rw-r--r--   0     1001      123     1492 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-pipe/src/executors/sinks/ordered.rs
+-rw-r--r--   0     1001      123     1824 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-pipe/src/executors/sinks/reproject.rs
+-rw-r--r--   0     1001      123     3108 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-pipe/src/executors/sinks/slice.rs
+-rw-r--r--   0     1001      123      130 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-pipe/src/executors/sinks/sort/mod.rs
+-rw-r--r--   0     1001      123     3808 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-pipe/src/executors/sinks/sort/ooc.rs
+-rw-r--r--   0     1001      123     6295 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-pipe/src/executors/sinks/sort/sink.rs
+-rw-r--r--   0     1001      123     5953 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-pipe/src/executors/sinks/sort/sink_multiple.rs
+-rw-r--r--   0     1001      123     3801 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-pipe/src/executors/sinks/sort/source.rs
+-rw-r--r--   0     1001      123      635 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-pipe/src/executors/sinks/utils.rs
+-rw-r--r--   0     1001      123     5076 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-pipe/src/executors/sources/csv.rs
+-rw-r--r--   0     1001      123     1231 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-pipe/src/executors/sources/frame.rs
+-rw-r--r--   0     1001      123      987 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-pipe/src/executors/sources/ipc_one_shot.rs
+-rw-r--r--   0     1001      123      366 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-pipe/src/executors/sources/mod.rs
+-rw-r--r--   0     1001      123     3387 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-pipe/src/executors/sources/parquet.rs
+-rw-r--r--   0     1001      123     1146 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-pipe/src/executors/sources/reproject.rs
+-rw-r--r--   0     1001      123     1022 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-pipe/src/executors/sources/union.rs
+-rw-r--r--   0     1001      123      448 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-pipe/src/expressions.rs
+-rw-r--r--   0     1001      123      272 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-pipe/src/lib.rs
+-rw-r--r--   0     1001      123      719 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-pipe/src/operators/chunks.rs
+-rw-r--r--   0     1001      123      474 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-pipe/src/operators/context.rs
+-rw-r--r--   0     1001      123      223 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-pipe/src/operators/mod.rs
+-rw-r--r--   0     1001      123      430 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-pipe/src/operators/operator.rs
+-rw-r--r--   0     1001      123      626 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-pipe/src/operators/sink.rs
+-rw-r--r--   0     1001      123      241 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-pipe/src/operators/source.rs
+-rw-r--r--   0     1001      123        1 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-pipe/src/pipeline/config.rs
+-rw-r--r--   0     1001      123    20492 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-pipe/src/pipeline/convert.rs
+-rw-r--r--   0     1001      123    13982 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-pipe/src/pipeline/dispatcher.rs
+-rw-r--r--   0     1001      123     1237 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/local_dependencies/polars-pipe/src/pipeline/mod.rs
+-rw-r--r--   0        0        0     4398 1970-01-01 00:00:00.000000 polars_u64_idx-0.17.9/Cargo.toml
+-rw-r--r--   0     1001      123       76 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/.gitignore
+-rw-r--r--   0     1001      123     1055 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/LICENSE
+-rw-r--r--   0     1001      123     2414 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/Makefile
+-rw-r--r--   0     1001      123    12625 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/README.md
+-rw-r--r--   0     1001      123      651 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/build.rs
+-rw-r--r--   0     1001      123       32 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/docs/.gitignore
+-rw-r--r--   0     1001      123      679 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/docs/Makefile
+-rw-r--r--   0     1001      123      318 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/docs/_templates/api_redirect.html
+-rw-r--r--   0     1001      123      151 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/docs/_templates/autosummary/accessor.rst
+-rw-r--r--   0     1001      123      160 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/docs/_templates/autosummary/accessor_attribute.rst
+-rw-r--r--   0     1001      123      168 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/docs/_templates/autosummary/accessor_callable.rst
+-rw-r--r--   0     1001      123      157 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/docs/_templates/autosummary/accessor_method.rst
+-rw-r--r--   0     1001      123      836 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/docs/_templates/autosummary/class.rst
+-rw-r--r--   0     1001      123       94 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/docs/_templates/autosummary/class_without_autosummary.rst
+-rw-r--r--   0     1001      123      406 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/docs/_templates/sidebar-nav-bs.html
+-rw-r--r--   0     1001      123      468 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/docs/requirements-docs.txt
+-rw-r--r--   0     1001      123     1164 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/docs/run_live_docs_server.py
+-rw-r--r--   0     1001      123     1567 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/docs/source/_static/css/custom.css
+-rw-r--r--   0     1001      123     7326 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/docs/source/conf.py
+-rw-r--r--   0     1001      123       51 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/docs/source/index.rst
+-rw-r--r--   0     1001      123     6767 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/docs/source/reference/api.rst
+-rw-r--r--   0     1001      123     1694 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/docs/source/reference/config.rst
+-rw-r--r--   0     1001      123      274 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/docs/source/reference/dataframe/aggregation.rst
+-rw-r--r--   0     1001      123      221 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/docs/source/reference/dataframe/attributes.rst
+-rw-r--r--   0     1001      123      142 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/docs/source/reference/dataframe/computation.rst
+-rw-r--r--   0     1001      123      319 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/docs/source/reference/dataframe/descriptive.rst
+-rw-r--r--   0     1001      123      319 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/docs/source/reference/dataframe/export.rst
+-rw-r--r--   0     1001      123      464 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/docs/source/reference/dataframe/groupby.rst
+-rw-r--r--   0     1001      123      379 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/docs/source/reference/dataframe/index.rst
+-rw-r--r--   0     1001      123      189 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/docs/source/reference/dataframe/miscellaneous.rst
+-rw-r--r--   0     1001      123     1538 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/docs/source/reference/dataframe/modify_select.rst
+-rw-r--r--   0     1001      123      663 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/docs/source/reference/datatypes.rst
+-rw-r--r--   0     1001      123      421 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/docs/source/reference/exceptions.rst
+-rw-r--r--   0     1001      123      391 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/docs/source/reference/expressions/aggregation.rst
+-rw-r--r--   0     1001      123      309 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/docs/source/reference/expressions/binary.rst
+-rw-r--r--   0     1001      123      338 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/docs/source/reference/expressions/boolean.rst
+-rw-r--r--   0     1001      123      237 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/docs/source/reference/expressions/categories.rst
+-rw-r--r--   0     1001      123      221 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/docs/source/reference/expressions/columns.rst
+-rw-r--r--   0     1001      123     1061 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/docs/source/reference/expressions/computation.rst
+-rw-r--r--   0     1001      123     1114 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/docs/source/reference/expressions/functions.rst
+-rw-r--r--   0     1001      123      461 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/docs/source/reference/expressions/index.rst
+-rw-r--r--   0     1001      123      695 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/docs/source/reference/expressions/list.rst
+-rw-r--r--   0     1001      123      374 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/docs/source/reference/expressions/meta.rst
+-rw-r--r--   0     1001      123      125 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/docs/source/reference/expressions/miscellaneous.rst
+-rw-r--r--   0     1001      123      977 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/docs/source/reference/expressions/modify_select.rst
+-rw-r--r--   0     1001      123      639 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/docs/source/reference/expressions/operators.rst
+-rw-r--r--   0     1001      123      860 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/docs/source/reference/expressions/string.rst
+-rw-r--r--   0     1001      123      254 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/docs/source/reference/expressions/struct.rst
+-rw-r--r--   0     1001      123     1014 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/docs/source/reference/expressions/temporal.rst
+-rw-r--r--   0     1001      123       98 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/docs/source/reference/expressions/window.rst
+-rw-r--r--   0     1001      123      692 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/docs/source/reference/functions.rst
+-rw-r--r--   0     1001      123      392 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/docs/source/reference/index.rst
+-rw-r--r--   0     1001      123     1269 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/docs/source/reference/io.rst
+-rw-r--r--   0     1001      123      252 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/docs/source/reference/lazyframe/aggregation.rst
+-rw-r--r--   0     1001      123      179 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/docs/source/reference/lazyframe/attributes.rst
+-rw-r--r--   0     1001      123      146 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/docs/source/reference/lazyframe/descriptive.rst
+-rw-r--r--   0     1001      123      497 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/docs/source/reference/lazyframe/groupby.rst
+-rw-r--r--   0     1001      123      354 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/docs/source/reference/lazyframe/index.rst
+-rw-r--r--   0     1001      123      455 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/docs/source/reference/lazyframe/miscellaneous.rst
+-rw-r--r--   0     1001      123     1013 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/docs/source/reference/lazyframe/modify_select.rst
+-rw-r--r--   0     1001      123      358 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/docs/source/reference/series/aggregation.rst
+-rw-r--r--   0     1001      123      256 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/docs/source/reference/series/attributes.rst
+-rw-r--r--   0     1001      123      321 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/docs/source/reference/series/binary.rst
+-rw-r--r--   0     1001      123      117 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/docs/source/reference/series/boolean.rst
+-rw-r--r--   0     1001      123      241 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/docs/source/reference/series/categories.rst
+-rw-r--r--   0     1001      123     1103 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/docs/source/reference/series/computation.rst
+-rw-r--r--   0     1001      123      744 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/docs/source/reference/series/descriptive.rst
+-rw-r--r--   0     1001      123      240 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/docs/source/reference/series/export.rst
+-rw-r--r--   0     1001      123      428 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/docs/source/reference/series/index.rst
+-rw-r--r--   0     1001      123      749 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/docs/source/reference/series/list.rst
+-rw-r--r--   0     1001      123      236 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/docs/source/reference/series/miscellaneous.rst
+-rw-r--r--   0     1001      123     1077 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/docs/source/reference/series/modify_select.rst
+-rw-r--r--   0     1001      123      922 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/docs/source/reference/series/string.rst
+-rw-r--r--   0     1001      123      396 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/docs/source/reference/series/struct.rst
+-rw-r--r--   0     1001      123     1168 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/docs/source/reference/series/temporal.rst
+-rw-r--r--   0     1001      123      302 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/docs/source/reference/sql.rst
+-rw-r--r--   0     1001      123     8067 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/docs/source/reference/testing.rst
+-rw-r--r--   0     1001      123      168 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/docs/source/reference/utils.rst
+-rw-r--r--   0     1001      123     6335 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/polars/__init__.py
+-rw-r--r--   0     1001      123    13396 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/polars/api.py
+-rw-r--r--   0     1001      123    25956 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/polars/config.py
+-rw-r--r--   0     1001      123    27169 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/polars/convert.py
+-rw-r--r--   0     1001      123       77 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/polars/dataframe/__init__.py
+-rw-r--r--   0     1001      123     5237 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/polars/dataframe/_html.py
+-rw-r--r--   0     1001      123   305755 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/polars/dataframe/frame.py
+-rw-r--r--   0     1001      123    33240 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/polars/dataframe/groupby.py
+-rw-r--r--   0     1001      123     2668 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/polars/datatypes/__init__.py
+-rw-r--r--   0     1001      123    12133 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/polars/datatypes/classes.py
+-rw-r--r--   0     1001      123     1603 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/polars/datatypes/constants.py
+-rw-r--r--   0     1001      123     4430 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/polars/datatypes/constructor.py
+-rw-r--r--   0     1001      123    15109 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/polars/datatypes/convert.py
+-rw-r--r--   0     1001      123     7338 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/polars/dependencies.py
+-rw-r--r--   0     1001      123     3436 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/polars/exceptions.py
+-rw-r--r--   0     1001      123       61 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/polars/expr/__init__.py
+-rw-r--r--   0     1001      123     2730 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/polars/expr/binary.py
+-rw-r--r--   0     1001      123     1708 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/polars/expr/categorical.py
+-rw-r--r--   0     1001      123    73000 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/polars/expr/datetime.py
+-rw-r--r--   0     1001      123   252403 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/polars/expr/expr.py
+-rw-r--r--   0     1001      123    22899 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/polars/expr/list.py
+-rw-r--r--   0     1001      123     2059 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/polars/expr/meta.py
+-rw-r--r--   0     1001      123    44648 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/polars/expr/string.py
+-rw-r--r--   0     1001      123     5436 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/polars/expr/struct.py
+-rw-r--r--   0     1001      123     1981 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/polars/functions/__init__.py
+-rw-r--r--   0     1001      123    29637 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/polars/functions/eager.py
+-rw-r--r--   0     1001      123    90827 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/polars/functions/lazy.py
+-rw-r--r--   0     1001      123     6293 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/polars/functions/whenthen.py
+-rw-r--r--   0     1001      123      280 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/polars/internals.py
+-rw-r--r--   0     1001      123      978 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/polars/io/__init__.py
+-rw-r--r--   0     1001      123     6264 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/polars/io/_utils.py
+-rw-r--r--   0     1001      123      878 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/polars/io/avro.py
+-rw-r--r--   0     1001      123      144 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/polars/io/csv/__init__.py
+-rw-r--r--   0     1001      123     1082 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/polars/io/csv/_utils.py
+-rw-r--r--   0     1001      123     4691 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/polars/io/csv/batched_reader.py
+-rw-r--r--   0     1001      123    35533 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/polars/io/csv/functions.py
+-rw-r--r--   0     1001      123     8655 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/polars/io/database.py
+-rw-r--r--   0     1001      123    10988 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/polars/io/delta.py
+-rw-r--r--   0     1001      123       75 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/polars/io/excel/__init__.py
+-rw-r--r--   0     1001      123    18459 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/polars/io/excel/_write_utils.py
+-rw-r--r--   0     1001      123     6476 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/polars/io/excel/functions.py
+-rw-r--r--   0     1001      123      142 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/polars/io/ipc/__init__.py
+-rw-r--r--   0     1001      123     1271 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/polars/io/ipc/anonymous_scan.py
+-rw-r--r--   0     1001      123     5840 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/polars/io/ipc/functions.py
+-rw-r--r--   0     1001      123      519 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/polars/io/json.py
+-rw-r--r--   0     1001      123     2257 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/polars/io/ndjson.py
+-rw-r--r--   0     1001      123      170 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/polars/io/parquet/__init__.py
+-rw-r--r--   0     1001      123     1299 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/polars/io/parquet/anonymous_scan.py
+-rw-r--r--   0     1001      123     7212 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/polars/io/parquet/functions.py
+-rw-r--r--   0     1001      123      136 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/polars/io/pyarrow_dataset/__init__.py
+-rw-r--r--   0     1001      123     2331 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/polars/io/pyarrow_dataset/anonymous_scan.py
+-rw-r--r--   0     1001      123     3611 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/polars/io/pyarrow_dataset/functions.py
+-rw-r--r--   0     1001      123       77 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/polars/lazyframe/__init__.py
+-rw-r--r--   0     1001      123   168293 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/polars/lazyframe/frame.py
+-rw-r--r--   0     1001      123    24178 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/polars/lazyframe/groupby.py
+-rw-r--r--   0     1001      123        0 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/polars/py.typed
+-rw-r--r--   0     1001      123       69 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/polars/series/__init__.py
+-rw-r--r--   0     1001      123     1579 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/polars/series/_numpy.py
+-rw-r--r--   0     1001      123     1920 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/polars/series/binary.py
+-rw-r--r--   0     1001      123     1699 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/polars/series/categorical.py
+-rw-r--r--   0     1001      123    49664 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/polars/series/datetime.py
+-rw-r--r--   0     1001      123    12385 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/polars/series/list.py
+-rw-r--r--   0     1001      123   164038 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/polars/series/series.py
+-rw-r--r--   0     1001      123    27401 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/polars/series/string.py
+-rw-r--r--   0     1001      123     2287 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/polars/series/struct.py
+-rw-r--r--   0     1001      123     5375 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/polars/series/utils.py
+-rw-r--r--   0     1001      123     7638 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/polars/slice.py
+-rw-r--r--   0     1001      123       75 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/polars/sql/__init__.py
+-rw-r--r--   0     1001      123     1351 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/polars/sql/context.py
+-rw-r--r--   0     1001      123     4764 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/polars/string_cache.py
+-rw-r--r--   0     1001      123      362 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/polars/testing/__init__.py
+-rw-r--r--   0     1001      123      929 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/polars/testing/_private.py
+-rw-r--r--   0     1001      123     3689 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/polars/testing/_tempdir.py
+-rw-r--r--   0     1001      123    13597 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/polars/testing/asserts.py
+-rw-r--r--   0     1001      123      800 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/polars/testing/parametric/__init__.py
+-rw-r--r--   0     1001      123    26499 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/polars/testing/parametric/primitives.py
+-rw-r--r--   0     1001      123     3409 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/polars/testing/parametric/profiles.py
+-rw-r--r--   0     1001      123     7711 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/polars/testing/parametric/strategies.py
+-rw-r--r--   0     1001      123     5824 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/polars/type_aliases.py
+-rw-r--r--   0     1001      123     1211 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/polars/utils/__init__.py
+-rw-r--r--   0     1001      123    50687 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/polars/utils/_construction.py
+-rw-r--r--   0     1001      123     2782 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/polars/utils/_parse_expr_input.py
+-rw-r--r--   0     1001      123      721 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/polars/utils/_scan.py
+-rw-r--r--   0     1001      123      687 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/polars/utils/_wrap.py
+-rw-r--r--   0     1001      123      683 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/polars/utils/build_info.py
+-rw-r--r--   0     1001      123     8812 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/polars/utils/convert.py
+-rw-r--r--   0     1001      123     5789 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/polars/utils/decorators.py
+-rw-r--r--   0     1001      123     1660 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/polars/utils/meta.py
+-rw-r--r--   0     1001      123      514 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/polars/utils/polars_version.py
+-rw-r--r--   0     1001      123     2339 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/polars/utils/show_versions.py
+-rw-r--r--   0     1001      123    11592 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/polars/utils/various.py
+-rw-r--r--   0     1001      123     5378 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/pyproject.toml
+-rw-r--r--   0     1001      123      699 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/requirements-dev.txt
+-rw-r--r--   0     1001      123       70 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/requirements-lint.txt
+-rw-r--r--   0     1001      123     1640 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/scripts/check_stacklevels.py
+-rw-r--r--   0     1001      123    11023 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/src/apply/dataframe.rs
+-rw-r--r--   0     1001      123     8388 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/src/apply/mod.rs
+-rw-r--r--   0     1001      123    71480 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/src/apply/series.rs
+-rw-r--r--   0     1001      123       32 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/src/arrow_interop/mod.rs
+-rw-r--r--   0     1001      123     1306 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/src/arrow_interop/to_py.rs
+-rw-r--r--   0     1001      123     3902 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/src/arrow_interop/to_rust.rs
+-rw-r--r--   0     1001      123     5250 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/src/batched_csv.rs
+-rw-r--r--   0     1001      123    46606 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/src/conversion.rs
+-rw-r--r--   0     1001      123    45472 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/src/dataframe.rs
+-rw-r--r--   0     1001      123     3799 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/src/datatypes.rs
+-rw-r--r--   0     1001      123     3288 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/src/error.rs
+-rw-r--r--   0     1001      123     9482 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/src/file.rs
+-rw-r--r--   0     1001      123     7468 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/src/lazy/apply.rs
+-rw-r--r--   0     1001      123    33439 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/src/lazy/dataframe.rs
+-rw-r--r--   0     1001      123    62598 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/src/lazy/dsl.rs
+-rw-r--r--   0     1001      123     1082 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/src/lazy/meta.rs
+-rw-r--r--   0     1001      123      727 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/src/lazy/mod.rs
+-rw-r--r--   0     1001      123      212 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/src/lazy/utils.rs
+-rw-r--r--   0     1001      123    20992 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/src/lib.rs
+-rw-r--r--   0     1001      123     8642 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/src/npy.rs
+-rw-r--r--   0     1001      123     1029 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/src/object.rs
+-rw-r--r--   0     1001      123      122 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/src/prelude.rs
+-rw-r--r--   0     1001      123      435 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/src/py_modules.rs
+-rw-r--r--   0     1001      123    54535 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/src/series.rs
+-rw-r--r--   0     1001      123     3478 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/src/set.rs
+-rw-r--r--   0     1001      123      843 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/src/sql.rs
+-rw-r--r--   0     1001      123     2335 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/src/utils.rs
+-rw-r--r--   0     1001      123     6165 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/tests/README.md
+-rw-r--r--   0     1001      123     2189 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/tests/benchmark/groupby-datagen.R
+-rw-r--r--   0     1001      123     7945 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/tests/benchmark/run_h2oai_benchmark.py
+-rw-r--r--   0     1001      123     6530 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/tests/benchmark/test_release.py
+-rw-r--r--   0     1001      123     4589 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/tests/docs/run_doctest.py
+-rw-r--r--   0     1001      123      179 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/tests/parametric/conftest.py
+-rw-r--r--   0     1001      123     3823 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/tests/parametric/test_dataframe.py
+-rw-r--r--   0     1001      123     1692 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/tests/parametric/test_lazyframe.py
+-rw-r--r--   0     1001      123     6863 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/tests/parametric/test_series.py
+-rw-r--r--   0     1001      123     8299 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/tests/parametric/test_testing.py
+-rw-r--r--   0     1001      123        0 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/tests/unit/__init__.py
+-rw-r--r--   0     1001      123     3382 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/tests/unit/conftest.py
+-rw-r--r--   0     1001      123       86 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/tests/unit/datatypes/__init__.py
+-rw-r--r--   0     1001      123      351 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/tests/unit/datatypes/test_binary.py
+-rw-r--r--   0     1001      123     1420 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/tests/unit/datatypes/test_bool.py
+-rw-r--r--   0     1001      123    12683 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/tests/unit/datatypes/test_categorical.py
+-rw-r--r--   0     1001      123     2826 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/tests/unit/datatypes/test_decimal.py
+-rw-r--r--   0     1001      123      280 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/tests/unit/datatypes/test_duration.py
+-rw-r--r--   0     1001      123    16033 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/tests/unit/datatypes/test_list.py
+-rw-r--r--   0     1001      123      284 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/tests/unit/datatypes/test_null.py
+-rw-r--r--   0     1001      123     2801 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/tests/unit/datatypes/test_object.py
+-rw-r--r--   0     1001      123    29644 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/tests/unit/datatypes/test_struct.py
+-rw-r--r--   0     1001      123    92213 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/tests/unit/datatypes/test_temporal.py
+-rw-r--r--   0     1001      123      418 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/tests/unit/datatypes/test_time.py
+-rw-r--r--   0     1001      123      218 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/tests/unit/io/conftest.py
+-rw-r--r--   0     1001      123       16 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/tests/unit/io/files/delta-table/.part-00000-e42312d7-60e5-454d-acbc-db192d220e73-c000.snappy.parquet.crc
+-rw-r--r--   0     1001      123       16 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/tests/unit/io/files/delta-table/.part-00000-e4a999da-df45-4fb0-bdc4-d999fc0f58aa-c000.snappy.parquet.crc
+-rw-r--r--   0     1001      123       16 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/tests/unit/io/files/delta-table/_delta_log/.00000000000000000000.json.crc
+-rw-r--r--   0     1001      123       16 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/tests/unit/io/files/delta-table/_delta_log/.00000000000000000001.json.crc
+-rw-r--r--   0     1001      123      905 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/tests/unit/io/files/delta-table/_delta_log/00000000000000000000.json
+-rw-r--r--   0     1001      123      936 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/tests/unit/io/files/delta-table/_delta_log/00000000000000000001.json
+-rw-r--r--   0     1001      123      972 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/tests/unit/io/files/delta-table/part-00000-e42312d7-60e5-454d-acbc-db192d220e73-c000.snappy.parquet
+-rw-r--r--   0     1001      123      690 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/tests/unit/io/files/delta-table/part-00000-e4a999da-df45-4fb0-bdc4-d999fc0f58aa-c000.snappy.parquet
+-rw-r--r--   0     1001      123        0 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/tests/unit/io/files/empty.csv
+-rw-r--r--   0     1001      123     5959 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/tests/unit/io/files/example.xlsx
+-rw-r--r--   0     1001      123      457 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/tests/unit/io/files/foods1.csv
+-rw-r--r--   0     1001      123     2351 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/tests/unit/io/files/foods1.ipc
+-rw-r--r--   0     1001      123     1713 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/tests/unit/io/files/foods1.ndjson
+-rw-r--r--   0     1001      123     1427 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/tests/unit/io/files/foods1.parquet
+-rw-r--r--   0     1001      123      455 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/tests/unit/io/files/foods2.csv
+-rw-r--r--   0     1001      123     2351 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/tests/unit/io/files/foods2.ipc
+-rw-r--r--   0     1001      123     1711 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/tests/unit/io/files/foods2.ndjson
+-rw-r--r--   0     1001      123     1916 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/tests/unit/io/files/foods2.parquet
+-rw-r--r--   0     1001      123      455 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/tests/unit/io/files/foods3.csv
+-rw-r--r--   0     1001      123      457 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/tests/unit/io/files/foods4.csv
+-rw-r--r--   0     1001      123      452 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/tests/unit/io/files/foods5.csv
+-rw-r--r--   0     1001      123       49 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/tests/unit/io/files/gzipped.csv
+-rw-r--r--   0     1001      123       57 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/tests/unit/io/files/small.csv
+-rw-r--r--   0     1001      123      756 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/tests/unit/io/files/small.parquet
+-rw-r--r--   0     1001      123     1937 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/tests/unit/io/test_avro.py
+-rw-r--r--   0     1001      123    39498 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/tests/unit/io/test_csv.py
+-rw-r--r--   0     1001      123     6360 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/tests/unit/io/test_database.py
+-rw-r--r--   0     1001      123     3456 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/tests/unit/io/test_delta.py
+-rw-r--r--   0     1001      123    11169 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/tests/unit/io/test_excel.py
+-rw-r--r--   0     1001      123     5919 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/tests/unit/io/test_ipc.py
+-rw-r--r--   0     1001      123     3720 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/tests/unit/io/test_json.py
+-rw-r--r--   0     1001      123     7232 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/tests/unit/io/test_lazy_csv.py
+-rw-r--r--   0     1001      123     2060 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/tests/unit/io/test_lazy_ipc.py
+-rw-r--r--   0     1001      123     2881 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/tests/unit/io/test_lazy_json.py
+-rw-r--r--   0     1001      123    11849 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/tests/unit/io/test_lazy_parquet.py
+-rw-r--r--   0     1001      123     2012 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/tests/unit/io/test_other.py
+-rw-r--r--   0     1001      123    13735 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/tests/unit/io/test_parquet.py
+-rw-r--r--   0     1001      123      612 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/tests/unit/io/test_pickle.py
+-rw-r--r--   0     1001      123     3259 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/tests/unit/io/test_pyarrow_dataset.py
+-rw-r--r--   0     1001      123      509 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/tests/unit/namespaces/__init__.py
+-rw-r--r--   0     1001      123     3218 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/tests/unit/namespaces/test_binary.py
+-rw-r--r--   0     1001      123     2489 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/tests/unit/namespaces/test_categorical.py
+-rw-r--r--   0     1001      123    18949 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/tests/unit/namespaces/test_datetime.py
+-rw-r--r--   0     1001      123    12750 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/tests/unit/namespaces/test_list.py
+-rw-r--r--   0     1001      123     1748 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/tests/unit/namespaces/test_meta.py
+-rw-r--r--   0     1001      123    23698 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/tests/unit/namespaces/test_string.py
+-rw-r--r--   0     1001      123    16930 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/tests/unit/namespaces/test_strptime.py
+-rw-r--r--   0     1001      123      982 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/tests/unit/namespaces/test_struct.py
+-rw-r--r--   0     1001      123       85 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/tests/unit/operations/__init__.py
+-rw-r--r--   0     1001      123     6238 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/tests/unit/operations/test_aggregations.py
+-rw-r--r--   0     1001      123     9412 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/tests/unit/operations/test_apply.py
+-rw-r--r--   0     1001      123     4390 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/tests/unit/operations/test_arithmetic.py
+-rw-r--r--   0     1001      123      956 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/tests/unit/operations/test_comparison.py
+-rw-r--r--   0     1001      123     2906 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/tests/unit/operations/test_drop.py
+-rw-r--r--   0     1001      123     8252 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/tests/unit/operations/test_explode.py
+-rw-r--r--   0     1001      123     3664 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/tests/unit/operations/test_filter.py
+-rw-r--r--   0     1001      123     1801 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/tests/unit/operations/test_folds.py
+-rw-r--r--   0     1001      123    22867 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/tests/unit/operations/test_groupby.py
+-rw-r--r--   0     1001      123     2959 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/tests/unit/operations/test_is_in.py
+-rw-r--r--   0     1001      123    16937 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/tests/unit/operations/test_join.py
+-rw-r--r--   0     1001      123    10891 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/tests/unit/operations/test_join_asof.py
+-rw-r--r--   0     1001      123      643 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/tests/unit/operations/test_melt.py
+-rw-r--r--   0     1001      123    10253 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/tests/unit/operations/test_pivot.py
+-rw-r--r--   0     1001      123    18016 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/tests/unit/operations/test_rolling.py
+-rw-r--r--   0     1001      123    19550 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/tests/unit/operations/test_sort.py
+-rw-r--r--   0     1001      123     4038 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/tests/unit/operations/test_statistics.py
+-rw-r--r--   0     1001      123     3631 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/tests/unit/operations/test_transpose.py
+-rw-r--r--   0     1001      123      771 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/tests/unit/operations/test_unique.py
+-rw-r--r--   0     1001      123     9814 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/tests/unit/operations/test_window.py
+-rw-r--r--   0     1001      123     4775 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/tests/unit/test_api.py
+-rw-r--r--   0     1001      123     1077 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/tests/unit/test_arity.py
+-rw-r--r--   0     1001      123    19856 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/tests/unit/test_cfg.py
+-rw-r--r--   0     1001      123    39286 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/tests/unit/test_constructors.py
+-rw-r--r--   0     1001      123      454 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/tests/unit/test_context.py
+-rw-r--r--   0     1001      123     1628 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/tests/unit/test_cse.py
+-rw-r--r--   0     1001      123     3817 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/tests/unit/test_datatypes.py
+-rw-r--r--   0     1001      123   121217 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/tests/unit/test_df.py
+-rw-r--r--   0     1001      123     1594 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/tests/unit/test_empty.py
+-rw-r--r--   0     1001      123    16914 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/tests/unit/test_errors.py
+-rw-r--r--   0     1001      123     2387 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/tests/unit/test_expr_multi_cols.py
+-rw-r--r--   0     1001      123    32643 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/tests/unit/test_exprs.py
+-rw-r--r--   0     1001      123     3305 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/tests/unit/test_fmt.py
+-rw-r--r--   0     1001      123    11420 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/tests/unit/test_functions.py
+-rw-r--r--   0     1001      123     3763 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/tests/unit/test_interchange.py
+-rw-r--r--   0     1001      123    33952 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/tests/unit/test_interop.py
+-rw-r--r--   0     1001      123    49534 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/tests/unit/test_lazy.py
+-rw-r--r--   0     1001      123     2369 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/tests/unit/test_polars_import.py
+-rw-r--r--   0     1001      123     4222 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/tests/unit/test_predicates.py
+-rw-r--r--   0     1001      123     7102 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/tests/unit/test_projections.py
+-rw-r--r--   0     1001      123    11550 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/tests/unit/test_queries.py
+-rw-r--r--   0     1001      123     4743 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/tests/unit/test_rows.py
+-rw-r--r--   0     1001      123    13202 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/tests/unit/test_schema.py
+-rw-r--r--   0     1001      123     2634 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/tests/unit/test_serde.py
+-rw-r--r--   0     1001      123    84354 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/tests/unit/test_series.py
+-rw-r--r--   0     1001      123      657 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/tests/unit/test_single.py
+-rw-r--r--   0     1001      123     2561 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/tests/unit/test_sql.py
+-rw-r--r--   0     1001      123    13877 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/tests/unit/test_streaming.py
+-rw-r--r--   0     1001      123    10700 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/tests/unit/test_testing.py
+-rw-r--r--   0     1001      123       41 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/tests/unit/utils/__init__.py
+-rw-r--r--   0     1001      123      306 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/tests/unit/utils/test_build_info.py
+-rw-r--r--   0     1001      123      247 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/tests/unit/utils/test_show_versions.py
+-rw-r--r--   0     1001      123     4307 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/tests/unit/utils/test_utils.py
+-rw-r--r--   0     1001      123    65631 2023-04-25 13:58:34.000000 polars_u64_idx-0.17.9/Cargo.lock
+-rw-r--r--   0        0        0    15163 1970-01-01 00:00:00.000000 polars_u64_idx-0.17.9/PKG-INFO
```

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-arrow/Cargo.toml` & `polars_u64_idx-0.17.9/local_dependencies/polars-arrow/Cargo.toml`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-arrow/LICENSE` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-arrow/src/array/default_arrays.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-arrow/src/array/default_arrays.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-arrow/src/array/get.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-arrow/src/array/get.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-arrow/src/array/list.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-arrow/src/array/list.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-arrow/src/array/mod.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-arrow/src/array/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-arrow/src/array/null.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-arrow/src/array/null.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-arrow/src/array/slice.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-arrow/src/array/slice.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-arrow/src/array/utf8.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-arrow/src/array/utf8.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-arrow/src/bit_util.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-arrow/src/bit_util.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-arrow/src/bitmap/mutable.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-arrow/src/bitmap/mutable.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-arrow/src/compute/take/boolean.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-arrow/src/compute/take/boolean.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-arrow/src/compute/take/mod.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-arrow/src/compute/take/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-arrow/src/conversion.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-arrow/src/conversion.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-arrow/src/data_types.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-arrow/src/data_types.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-arrow/src/floats/ord.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-arrow/src/floats/ord.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-arrow/src/index.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-arrow/src/index.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-arrow/src/is_valid.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-arrow/src/is_valid.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-arrow/src/kernels/agg_mean.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-arrow/src/kernels/agg_mean.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-arrow/src/kernels/concatenate.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-arrow/src/kernels/concatenate.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-arrow/src/kernels/ewm/average.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-arrow/src/kernels/ewm/average.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-arrow/src/kernels/ewm/mod.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-arrow/src/kernels/ewm/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-arrow/src/kernels/ewm/variance.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-arrow/src/kernels/ewm/variance.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-arrow/src/kernels/float.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-arrow/src/kernels/float.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-arrow/src/kernels/list.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-arrow/src/kernels/list.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-arrow/src/kernels/list_bytes_iter.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-arrow/src/kernels/list_bytes_iter.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-arrow/src/kernels/mod.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-arrow/src/kernels/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-arrow/src/kernels/rolling/mod.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-arrow/src/kernels/rolling/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/mean.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/mean.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/min_max.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/min_max.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/mod.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/quantile.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/quantile.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/sum.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/sum.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/variance.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/variance.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-arrow/src/kernels/rolling/nulls/mean.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-arrow/src/kernels/rolling/nulls/mean.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-arrow/src/kernels/rolling/nulls/min_max.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-arrow/src/kernels/rolling/nulls/min_max.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-arrow/src/kernels/rolling/nulls/mod.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-arrow/src/kernels/rolling/nulls/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-arrow/src/kernels/rolling/nulls/quantile.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-arrow/src/kernels/rolling/nulls/quantile.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-arrow/src/kernels/rolling/nulls/sum.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-arrow/src/kernels/rolling/nulls/sum.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-arrow/src/kernels/rolling/nulls/variance.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-arrow/src/kernels/rolling/nulls/variance.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-arrow/src/kernels/rolling/window.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-arrow/src/kernels/rolling/window.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-arrow/src/kernels/set.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-arrow/src/kernels/set.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-arrow/src/kernels/sort_partition.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-arrow/src/kernels/sort_partition.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-arrow/src/kernels/sorted_join/inner.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-arrow/src/kernels/sorted_join/inner.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-arrow/src/kernels/sorted_join/left.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-arrow/src/kernels/sorted_join/left.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-arrow/src/kernels/string.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-arrow/src/kernels/string.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-arrow/src/kernels/take_agg/boolean.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-arrow/src/kernels/take_agg/boolean.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-arrow/src/kernels/take_agg/mod.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-arrow/src/kernels/take_agg/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-arrow/src/kernels/take_agg/var.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-arrow/src/kernels/take_agg/var.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-arrow/src/kernels/time.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-arrow/src/kernels/time.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-arrow/src/slice.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-arrow/src/slice.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-arrow/src/time_zone.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-arrow/src/time_zone.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-arrow/src/trusted_len/boolean.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-arrow/src/trusted_len/boolean.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-arrow/src/trusted_len/mod.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-arrow/src/trusted_len/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-arrow/src/trusted_len/push_unchecked.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-arrow/src/trusted_len/push_unchecked.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-arrow/src/utils.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-arrow/src/utils.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-sql/Cargo.toml` & `polars_u64_idx-0.17.9/local_dependencies/polars-sql/Cargo.toml`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-sql/LICENSE` & `polars_u64_idx-0.17.9/local_dependencies/polars-arrow/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-sql/src/context.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-sql/src/context.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-sql/src/functions.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-sql/src/functions.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-sql/src/keywords.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-sql/src/keywords.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-sql/src/sql_expr.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-sql/src/sql_expr.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-sql/src/table_functions.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-sql/src/table_functions.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-sql/tests/functions_cumulative.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-sql/tests/functions_cumulative.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-sql/tests/functions_io.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-sql/tests/functions_io.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-sql/tests/functions_math.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-sql/tests/functions_math.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-sql/tests/functions_string.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-sql/tests/functions_string.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-sql/tests/iss_7436.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-sql/tests/iss_7436.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-sql/tests/iss_7437.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-sql/tests/iss_7437.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-sql/tests/iss_7440.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-sql/tests/iss_7440.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-sql/tests/iss_8395.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-sql/tests/iss_8395.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-sql/tests/iss_8419.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-sql/tests/iss_8419.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-sql/tests/simple_exprs.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-sql/tests/simple_exprs.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-ops/Cargo.toml` & `polars_u64_idx-0.17.9/local_dependencies/polars-ops/Cargo.toml`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-ops/LICENSE` & `polars_u64_idx-0.17.9/local_dependencies/polars-error/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-ops/src/chunked_array/binary/namespace.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-ops/src/chunked_array/binary/namespace.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-ops/src/chunked_array/interpolate.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-ops/src/chunked_array/interpolate.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-ops/src/chunked_array/list/count.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-ops/src/chunked_array/list/count.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-ops/src/chunked_array/list/hash.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-ops/src/chunked_array/list/hash.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-ops/src/chunked_array/list/min_max.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-ops/src/chunked_array/list/min_max.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-ops/src/chunked_array/list/namespace.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-ops/src/chunked_array/list/namespace.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-ops/src/chunked_array/list/sum_mean.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-ops/src/chunked_array/list/sum_mean.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-ops/src/chunked_array/list/to_struct.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-ops/src/chunked_array/list/to_struct.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-ops/src/chunked_array/nan_propagating_aggregate.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-ops/src/chunked_array/nan_propagating_aggregate.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-ops/src/chunked_array/set.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-ops/src/chunked_array/set.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-ops/src/chunked_array/strings/case.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-ops/src/chunked_array/strings/case.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-ops/src/chunked_array/strings/json_path.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-ops/src/chunked_array/strings/json_path.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-ops/src/chunked_array/strings/justify.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-ops/src/chunked_array/strings/justify.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-ops/src/chunked_array/strings/mod.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-ops/src/chunked_array/strings/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-ops/src/chunked_array/strings/namespace.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-ops/src/chunked_array/strings/namespace.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-ops/src/chunked_array/strings/replace.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-ops/src/chunked_array/strings/replace.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-ops/src/chunked_array/top_k.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-ops/src/chunked_array/top_k.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-ops/src/frame/join/merge_sorted.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-ops/src/frame/join/merge_sorted.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-ops/src/frame/join/mod.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-ops/src/frame/join/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-ops/src/frame/mod.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-ops/src/frame/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-ops/src/frame/pivot/mod.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-ops/src/frame/pivot/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-ops/src/frame/pivot/positioning.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-ops/src/frame/pivot/positioning.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-ops/src/series/ops/approx_algo/hyperloglogplus.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-ops/src/series/ops/approx_algo/hyperloglogplus.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-ops/src/series/ops/approx_unique.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-ops/src/series/ops/approx_unique.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-ops/src/series/ops/arg_min_max.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-ops/src/series/ops/arg_min_max.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-ops/src/series/ops/floor_divide.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-ops/src/series/ops/floor_divide.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-ops/src/series/ops/is_first.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-ops/src/series/ops/is_first.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-ops/src/series/ops/is_unique.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-ops/src/series/ops/is_unique.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-ops/src/series/ops/log.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-ops/src/series/ops/log.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-ops/src/series/ops/mod.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-ops/src/series/ops/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-ops/src/series/ops/rolling.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-ops/src/series/ops/rolling.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-ops/src/series/ops/search_sorted.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-ops/src/series/ops/search_sorted.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-ops/src/series/ops/to_dummies.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-ops/src/series/ops/to_dummies.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-ops/src/series/ops/various.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-ops/src/series/ops/various.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-error/Cargo.toml` & `polars_u64_idx-0.17.9/local_dependencies/polars-error/Cargo.toml`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-error/LICENSE` & `polars_u64_idx-0.17.9/local_dependencies/polars-sql/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-error/src/lib.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-error/src/lib.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-io/Cargo.toml` & `polars_u64_idx-0.17.9/local_dependencies/polars-io/Cargo.toml`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-io/LICENSE` & `polars_u64_idx-0.17.9/local_dependencies/polars-row/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-io/src/avro/mod.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-io/src/avro/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-io/src/avro/read.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-io/src/avro/read.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-io/src/avro/write.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-io/src/avro/write.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-io/src/cloud/adaptors.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-io/src/cloud/adaptors.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-io/src/cloud/glob.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-io/src/cloud/glob.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-io/src/cloud/mod.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-io/src/cloud/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-io/src/csv/buffer.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-io/src/csv/buffer.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-io/src/csv/mod.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-io/src/csv/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-io/src/csv/parser.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-io/src/csv/parser.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-io/src/csv/read.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-io/src/csv/read.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-io/src/csv/read_impl/batched_mmap.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-io/src/csv/read_impl/batched_mmap.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-io/src/csv/read_impl/batched_read.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-io/src/csv/read_impl/batched_read.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-io/src/csv/read_impl/mod.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-io/src/csv/read_impl/mod.rs`

 * *Files 1% similar despite different names*

```diff
@@ -62,15 +62,18 @@
                 }
             })
             .collect::<PolarsResult<Vec<_>>>()?;
         *df = DataFrame::new_no_checks(cols)
     } else {
         // cast to the original dtypes in the schema
         for fld in to_cast {
-            df.try_apply(fld.name(), |s| cast_fn(s, fld))?;
+            // field may not be projected
+            if let Some(idx) = df.find_idx_by_name(fld.name()) {
+                df.try_apply_at_idx(idx, |s| cast_fn(s, fld))?;
+            }
         }
     }
     Ok(())
 }
 
 /// CSV file reader
 pub(crate) struct CoreReader<'a> {
@@ -674,15 +677,15 @@
                             self.schema.as_ref(),
                             self.ignore_errors,
                             &projection,
                             bytes_offset_thread,
                             self.quote_char,
                             self.eol_char,
                             self.comment_char,
-                            chunk_size,
+                            capacity,
                             &str_capacities,
                             self.encoding,
                             self.null_values.as_ref(),
                             self.missing_is_null,
                             usize::MAX,
                             stop_at_nbytes,
                             starting_point_offset,
```

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-io/src/csv/splitfields.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-io/src/csv/splitfields.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-io/src/csv/utils.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-io/src/csv/utils.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-io/src/csv/write.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-io/src/csv/write.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-io/src/csv/write_impl.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-io/src/csv/write_impl.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-io/src/ipc/ipc_file.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-io/src/ipc/ipc_file.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-io/src/ipc/ipc_stream.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-io/src/ipc/ipc_stream.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-io/src/ipc/mmap.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-io/src/ipc/mmap.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-io/src/ipc/write.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-io/src/ipc/write.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-io/src/ipc/write_async.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-io/src/ipc/write_async.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-io/src/json.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-io/src/json.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-io/src/lib.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-io/src/lib.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-io/src/mmap.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-io/src/mmap.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-io/src/ndjson_core/buffer.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-io/src/ndjson_core/buffer.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-io/src/ndjson_core/ndjson.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-io/src/ndjson_core/ndjson.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-io/src/parquet/async_impl.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-io/src/parquet/async_impl.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-io/src/parquet/mmap.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-io/src/parquet/mmap.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-io/src/parquet/mod.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-io/src/parquet/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-io/src/parquet/predicates.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-io/src/parquet/predicates.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-io/src/parquet/read.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-io/src/parquet/read.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-io/src/parquet/read_impl.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-io/src/parquet/read_impl.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-io/src/parquet/write.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-io/src/parquet/write.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-io/src/partition.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-io/src/partition.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-io/src/predicates.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-io/src/predicates.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-io/src/prelude.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-io/src/prelude.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-io/src/utils.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-io/src/utils.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-pipe/Cargo.toml` & `polars_u64_idx-0.17.9/local_dependencies/polars-pipe/Cargo.toml`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-pipe/LICENSE` & `polars_u64_idx-0.17.9/local_dependencies/polars/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-pipe/src/executors/operators/filter.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-pipe/src/executors/operators/filter.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-pipe/src/executors/operators/function.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-pipe/src/executors/operators/function.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-pipe/src/executors/operators/placeholder.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-pipe/src/executors/operators/placeholder.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-pipe/src/executors/operators/projection.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-pipe/src/executors/operators/projection.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-pipe/src/executors/operators/reproject.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-pipe/src/executors/operators/reproject.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-pipe/src/executors/sinks/file_sink.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-pipe/src/executors/sinks/file_sink.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/convert.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/convert.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/count.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/count.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/first.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/first.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/interface.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/interface.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/last.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/last.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/mean.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/mean.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/min_max.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/min_max.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/null.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/null.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/sum.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/sum.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/eval.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/eval.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/global.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/global.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/hash_table.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/hash_table.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/mod.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/ooc_state.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/ooc_state.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/sink.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/sink.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/thread_local.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/thread_local.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-pipe/src/executors/sinks/groupby/mod.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-pipe/src/executors/sinks/groupby/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-pipe/src/executors/sinks/groupby/ooc.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-pipe/src/executors/sinks/groupby/ooc.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-pipe/src/executors/sinks/groupby/ooc_state.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-pipe/src/executors/sinks/groupby/ooc_state.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-pipe/src/executors/sinks/groupby/primitive/mod.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-pipe/src/executors/sinks/groupby/primitive/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-pipe/src/executors/sinks/groupby/string.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-pipe/src/executors/sinks/groupby/string.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-pipe/src/executors/sinks/groupby/utils.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-pipe/src/executors/sinks/groupby/utils.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-pipe/src/executors/sinks/io.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-pipe/src/executors/sinks/io.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-pipe/src/executors/sinks/joins/cross.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-pipe/src/executors/sinks/joins/cross.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-pipe/src/executors/sinks/joins/generic_build.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-pipe/src/executors/sinks/joins/generic_build.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-pipe/src/executors/sinks/joins/inner_left.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-pipe/src/executors/sinks/joins/inner_left.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-pipe/src/executors/sinks/memory.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-pipe/src/executors/sinks/memory.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-pipe/src/executors/sinks/mod.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-pipe/src/executors/sinks/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-pipe/src/executors/sinks/ordered.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-pipe/src/executors/sinks/ordered.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-pipe/src/executors/sinks/reproject.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-pipe/src/executors/sinks/reproject.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-pipe/src/executors/sinks/slice.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-pipe/src/executors/sinks/slice.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-pipe/src/executors/sinks/sort/ooc.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-pipe/src/executors/sinks/sort/ooc.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-pipe/src/executors/sinks/sort/sink.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-pipe/src/executors/sinks/sort/sink.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-pipe/src/executors/sinks/sort/sink_multiple.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-pipe/src/executors/sinks/sort/sink_multiple.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-pipe/src/executors/sinks/sort/source.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-pipe/src/executors/sinks/sort/source.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-pipe/src/executors/sinks/utils.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-pipe/src/executors/sinks/utils.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-pipe/src/executors/sources/csv.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-pipe/src/executors/sources/csv.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-pipe/src/executors/sources/frame.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-pipe/src/executors/sources/frame.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-pipe/src/executors/sources/ipc_one_shot.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-pipe/src/executors/sources/ipc_one_shot.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-pipe/src/executors/sources/parquet.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-pipe/src/executors/sources/parquet.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-pipe/src/executors/sources/reproject.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-pipe/src/executors/sources/reproject.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-pipe/src/executors/sources/union.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-pipe/src/executors/sources/union.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-pipe/src/operators/chunks.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-pipe/src/operators/chunks.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-pipe/src/operators/sink.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-pipe/src/operators/sink.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-pipe/src/pipeline/convert.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-pipe/src/pipeline/convert.rs`

 * *Files 0% similar despite different names*

```diff
@@ -494,15 +494,15 @@
                         // only push predicate of first source
                         get_source(
                             lp.clone(),
                             &mut operator_objects,
                             expr_arena,
                             &to_physical,
                             i == 0,
-                            i == 0,
+                            verbose && i == 0,
                         )
                     })
                     .collect::<PolarsResult<Vec<_>>>()?;
                 Box::new(sources::UnionSource::new(sources)) as Box<dyn Source>
             }
             lp => {
                 panic!("source {lp:?} not (yet) supported")
```

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-pipe/src/pipeline/dispatcher.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-pipe/src/pipeline/dispatcher.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-pipe/src/pipeline/mod.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-pipe/src/pipeline/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/Cargo.toml` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/Cargo.toml`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/LICENSE` & `polars_u64_idx-0.17.9/local_dependencies/polars-plan/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/arithmetic.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/arithmetic.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/bitwise.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/bitwise.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/builder/binary.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/builder/binary.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/builder/boolean.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/builder/boolean.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/builder/from.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/builder/from.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/builder/list.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/builder/list.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/builder/mod.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/builder/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/builder/primitive.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/builder/primitive.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/builder/utf8.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/builder/utf8.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/cast.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/cast.rs`

 * *Files 1% similar despite different names*

```diff
@@ -96,14 +96,16 @@
             DataType::Struct(fields) => cast_single_to_struct(self.name(), &self.chunks, fields),
             _ => cast_impl_inner(self.name(), &self.chunks, data_type, checked).map(|mut s| {
                 // maintain sorted if data types remain signed
                 // this may still fail with overflow?
                 if ((self.dtype().is_signed() && data_type.is_signed())
                     || (self.dtype().is_unsigned() && data_type.is_unsigned()))
                     && (s.null_count() == self.null_count())
+                    // physical to logicals
+                    || (self.dtype().to_physical() == data_type.to_physical())
                 {
                     let is_sorted = self.is_sorted_flag2();
                     s.set_sorted_flag(is_sorted)
                 }
                 s
             }),
         }
```

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/comparison/mod.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/comparison/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/comparison/scalar.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/comparison/scalar.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/drop.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/drop.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/float.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/float.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/from.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/from.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/iterator/mod.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/iterator/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/iterator/par/list.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/iterator/par/list.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/iterator/par/utf8.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/iterator/par/utf8.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/kernels/take.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/kernels/take.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/list/iterator.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/list/iterator.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/list/mod.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/list/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/logical/categorical/builder.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/logical/categorical/builder.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/logical/categorical/from.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/logical/categorical/from.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/logical/categorical/merge.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/logical/categorical/merge.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/logical/categorical/mod.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/logical/categorical/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/append.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/append.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/take_random.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/take_random.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/unique.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/unique.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/zip.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/zip.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/logical/categorical/stringcache.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/logical/categorical/stringcache.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/logical/date.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/logical/date.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/logical/datetime.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/logical/datetime.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/logical/decimal.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/logical/decimal.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/logical/duration.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/logical/duration.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/logical/mod.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/logical/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/logical/struct_/mod.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/logical/struct_/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/logical/time.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/logical/time.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/mod.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/ndarray.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/ndarray.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/object/builder.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/object/builder.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/object/extension/drop.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/object/extension/drop.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/object/extension/list.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/object/extension/list.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/object/extension/mod.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/object/extension/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/object/extension/polars_extension.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/object/extension/polars_extension.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/object/iterator.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/object/iterator.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/object/mod.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/object/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/object/registry.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/object/registry.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/ops/aggregate/mod.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/ops/aggregate/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/ops/aggregate/quantile.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/ops/aggregate/quantile.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/ops/aggregate/var.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/ops/aggregate/var.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/ops/any_value.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/ops/any_value.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/ops/append.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/ops/append.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/ops/apply.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/ops/apply.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/ops/bit_repr.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/ops/bit_repr.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/ops/chunkops.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/ops/chunkops.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/ops/compare_inner.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/ops/compare_inner.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/ops/concat_str.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/ops/concat_str.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/ops/cum_agg.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/ops/cum_agg.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/ops/downcast.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/ops/downcast.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/ops/explode.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/ops/explode.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/ops/extend.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/ops/extend.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/ops/fill_null.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/ops/fill_null.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/ops/filter.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/ops/filter.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/ops/full.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/ops/full.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/ops/is_in.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/ops/is_in.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/ops/min_max_binary.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/ops/min_max_binary.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/ops/mod.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/ops/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/ops/nulls.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/ops/nulls.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/ops/peaks.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/ops/peaks.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/ops/repeat_by.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/ops/repeat_by.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/ops/reverse.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/ops/reverse.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/ops/rolling_window.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/ops/rolling_window.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/ops/set.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/ops/set.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/ops/shift.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/ops/shift.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/ops/sort/arg_sort.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/ops/sort/arg_sort.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/ops/sort/arg_sort_multiple.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/ops/sort/arg_sort_multiple.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/ops/sort/categorical.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/ops/sort/categorical.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/ops/sort/mod.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/ops/sort/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/ops/take/mod.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/ops/take/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/ops/take/take_chunked.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/ops/take/take_chunked.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/ops/take/take_every.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/ops/take/take_every.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/ops/take/take_random.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/ops/take/take_random.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/ops/take/take_single.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/ops/take/take_single.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/ops/take/traits.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/ops/take/traits.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/ops/unique/mod.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/ops/unique/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/ops/unique/rank.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/ops/unique/rank.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/ops/zip.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/ops/zip.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/random.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/random.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/temporal/conversion.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/temporal/conversion.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/temporal/date.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/temporal/date.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/temporal/datetime.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/temporal/datetime.rs`

 * *Files 4% similar despite different names*

```diff
@@ -120,15 +120,15 @@
 
     #[cfg(feature = "timezones")]
     pub fn replace_time_zone(
         &self,
         time_zone: Option<&str>,
         use_earliest: Option<bool>,
     ) -> PolarsResult<DatetimeChunked> {
-        match (self.time_zone(), time_zone) {
+        let out: PolarsResult<_> = match (self.time_zone(), time_zone) {
             (Some(from), Some(to)) => {
                 let chunks = self
                     .downcast_iter()
                     .map(|arr| {
                         replace_timezone(arr, self.time_unit().to_arrow(), to, from, use_earliest)
                     })
                     .collect::<PolarsResult<_>>()?;
@@ -158,15 +158,18 @@
                         replace_timezone(arr, self.time_unit().to_arrow(), to, "UTC", use_earliest)
                     })
                     .collect::<PolarsResult<_>>()?;
                 let out = unsafe { ChunkedArray::from_chunks(self.name(), chunks) };
                 Ok(out.into_datetime(self.time_unit(), Some(to.to_string())))
             }
             (None, None) => Ok(self.clone()),
-        }
+        };
+        let mut out = out?;
+        out.set_sorted_flag(self.is_sorted_flag2());
+        Ok(out)
     }
 
     /// Format Datetime with a `format` rule. See [chrono strftime/strptime](https://docs.rs/chrono/0.4.19/chrono/format/strftime/index.html).
     pub fn strftime(&self, format: &str) -> PolarsResult<Utf8Chunked> {
         #[cfg(feature = "timezones")]
         use chrono::Utc;
         let conversion_f = match self.time_unit() {
```

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/temporal/duration.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/temporal/duration.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/temporal/mod.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/temporal/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/temporal/time.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/temporal/time.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/to_vec.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/to_vec.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/trusted_len.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/trusted_len.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/chunked_array/upstream_traits.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/chunked_array/upstream_traits.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/cloud.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/cloud.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/config.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/config.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/datatypes/_serde.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/datatypes/_serde.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/datatypes/aliases.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/datatypes/aliases.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/datatypes/any_value.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/datatypes/any_value.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/datatypes/dtype.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/datatypes/dtype.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/datatypes/field.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/datatypes/field.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/datatypes/mod.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/datatypes/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/datatypes/time_unit.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/datatypes/time_unit.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/doc/changelog/v0_10_0_11.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/doc/changelog/v0_10_0_11.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/doc/changelog/v0_7.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/doc/changelog/v0_7.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/doc/changelog/v0_8.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/doc/changelog/v0_8.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/doc/changelog/v0_9.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/doc/changelog/v0_9.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/fmt.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/fmt.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/frame/arithmetic.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/frame/arithmetic.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/frame/asof_join/asof.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/frame/asof_join/asof.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/frame/asof_join/groups.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/frame/asof_join/groups.rs`

 * *Files 2% similar despite different names*

```diff
@@ -615,15 +615,17 @@
                         &left_by, &right_by, left_asof, right_asof, tolerance, strategy,
                     )?
                 }
             }
         }
     } else {
         for (lhs, rhs) in left_by.get_columns().iter().zip(right_by.get_columns()) {
-            check_asof_columns(lhs, rhs)?;
+            polars_ensure!(lhs.dtype() == rhs.dtype(),
+                ComputeError: "mismatching dtypes in 'on' parameter of asof-join: `{}` and `{}`", lhs.dtype(), rhs.dtype()
+            );
             #[cfg(feature = "dtype-categorical")]
             _check_categorical_src(lhs.dtype(), rhs.dtype())?;
         }
         asof_join_by_multiple(
             left_by, right_by, left_asof, right_asof, tolerance, strategy,
         )
     };
```

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/frame/asof_join/mod.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/frame/asof_join/mod.rs`

 * *Files 2% similar despite different names*

```diff
@@ -35,16 +35,16 @@
         ComputeError: "mismatching key dtypes in asof-join: `{}` and `{}`",
         a.dtype(), b.dtype()
     );
     polars_ensure!(
         a.null_count() == 0 && b.null_count() == 0,
         ComputeError: "asof join must not have null values in 'on' arguments"
     );
-    ensure_sorted_arg(a);
-    ensure_sorted_arg(b);
+    ensure_sorted_arg(a, "asof_join");
+    ensure_sorted_arg(b, "asof_join");
     Ok(())
 }
 
 #[derive(Clone, Copy, Debug, PartialEq, Eq, Default)]
 #[cfg_attr(feature = "serde", derive(Serialize, Deserialize))]
 pub enum AsofStrategy {
     /// selects the last row in the right DataFrame whose ‘on’ key is less than or equal to the left’s key
```

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/frame/chunks.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/frame/chunks.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/frame/cross_join.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/frame/cross_join.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/frame/explode.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/frame/explode.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/frame/from.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/frame/from.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/frame/groupby/aggregations/agg_list.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/frame/groupby/aggregations/agg_list.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/frame/groupby/aggregations/boolean.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/frame/groupby/aggregations/boolean.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/frame/groupby/aggregations/dispatch.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/frame/groupby/aggregations/dispatch.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/frame/groupby/aggregations/mod.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/frame/groupby/aggregations/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/frame/groupby/aggregations/utf8.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/frame/groupby/aggregations/utf8.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/frame/groupby/hashing.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/frame/groupby/hashing.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/frame/groupby/into_groups.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/frame/groupby/into_groups.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/frame/groupby/mod.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/frame/groupby/mod.rs`

 * *Files 0% similar despite different names*

```diff
@@ -800,15 +800,15 @@
                 // groups are in bounds
                 let sub_df = unsafe { take_df(&df, g) };
                 f(sub_df)
             })
             .collect::<PolarsResult<Vec<_>>>()?;
 
         let mut df = accumulate_dataframes_vertical(dfs)?;
-        df.as_single_chunk();
+        df.as_single_chunk_par();
         Ok(df)
     }
 
     /// Apply a closure over the groups as a new DataFrame.
     pub fn apply<F>(&self, mut f: F) -> PolarsResult<DataFrame>
     where
         F: FnMut(DataFrame) -> PolarsResult<DataFrame> + Send + Sync,
@@ -822,15 +822,15 @@
                 // groups are in bounds
                 let sub_df = unsafe { take_df(&df, g) };
                 f(sub_df)
             })
             .collect::<PolarsResult<Vec<_>>>()?;
 
         let mut df = accumulate_dataframes_vertical(dfs)?;
-        df.as_single_chunk();
+        df.as_single_chunk_par();
         Ok(df)
     }
 }
 
 unsafe fn take_df(df: &DataFrame, g: GroupsIndicator) -> DataFrame {
     match g {
         GroupsIndicator::Idx(idx) => df.take_iter_unchecked(idx.1.iter().map(|i| *i as usize)),
```

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/frame/groupby/perfect.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/frame/groupby/perfect.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/frame/groupby/proxy.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/frame/groupby/proxy.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/frame/hash_join/mod.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/frame/hash_join/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/frame/hash_join/multiple_keys.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/frame/hash_join/multiple_keys.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/frame/hash_join/single_keys.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/frame/hash_join/single_keys.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/frame/hash_join/single_keys_dispatch.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/frame/hash_join/single_keys_dispatch.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/frame/hash_join/single_keys_inner.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/frame/hash_join/single_keys_inner.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/frame/hash_join/single_keys_left.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/frame/hash_join/single_keys_left.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/frame/hash_join/single_keys_outer.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/frame/hash_join/single_keys_outer.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/frame/hash_join/single_keys_semi_anti.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/frame/hash_join/single_keys_semi_anti.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/frame/hash_join/sort_merge.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/frame/hash_join/sort_merge.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/frame/mod.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/frame/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/frame/row/av_buffer.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/frame/row/av_buffer.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/frame/row/dataframe.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/frame/row/dataframe.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/frame/row/mod.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/frame/row/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/frame/row/transpose.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/frame/row/transpose.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/frame/top_k.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/frame/top_k.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/frame/upstream_traits.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/frame/upstream_traits.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/functions.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/functions.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/hashing/fx.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/hashing/fx.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/hashing/identity.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/hashing/identity.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/hashing/partition.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/hashing/partition.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/hashing/vector_hasher.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/hashing/vector_hasher.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/lib.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/lib.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/named_from.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/named_from.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/prelude.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/prelude.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/schema.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/schema.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/serde/chunked_array.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/serde/chunked_array.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/serde/mod.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/serde/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/serde/series.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/serde/series.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/series/any_value.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/series/any_value.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/series/arithmetic/borrowed.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/series/arithmetic/borrowed.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/series/arithmetic/owned.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/series/arithmetic/owned.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/series/comparison.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/series/comparison.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/series/from.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/series/from.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/series/implementations/binary.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/series/implementations/binary.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/series/implementations/boolean.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/series/implementations/boolean.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/series/implementations/categorical.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/series/implementations/categorical.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/series/implementations/dates_time.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/series/implementations/dates_time.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/series/implementations/datetime.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/series/implementations/datetime.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/series/implementations/decimal.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/series/implementations/decimal.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/series/implementations/duration.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/series/implementations/duration.rs`

 * *Files 3% similar despite different names*

```diff
@@ -425,36 +425,31 @@
     fn max_as_series(&self) -> Series {
         self.0.max_as_series().into_duration(self.0.time_unit())
     }
     fn min_as_series(&self) -> Series {
         self.0.min_as_series().into_duration(self.0.time_unit())
     }
     fn median_as_series(&self) -> Series {
-        Int32Chunked::full_null(self.name(), 1)
-            .cast(self.dtype())
-            .unwrap()
-    }
-    fn var_as_series(&self, _ddof: u8) -> Series {
-        Int32Chunked::full_null(self.name(), 1)
-            .cast(self.dtype())
+        self.0
+            .median_as_series()
+            .cast(&self.dtype().to_physical())
             .unwrap()
-    }
-    fn std_as_series(&self, _ddof: u8) -> Series {
-        Int32Chunked::full_null(self.name(), 1)
             .cast(self.dtype())
             .unwrap()
     }
     fn quantile_as_series(
         &self,
-        _quantile: f64,
-        _interpol: QuantileInterpolOptions,
+        quantile: f64,
+        interpol: QuantileInterpolOptions,
     ) -> PolarsResult<Series> {
-        Ok(Int32Chunked::full_null(self.name(), 1)
+        self.0
+            .quantile_as_series(quantile, interpol)?
+            .cast(&self.dtype().to_physical())
+            .unwrap()
             .cast(self.dtype())
-            .unwrap())
     }
 
     fn clone_inner(&self) -> Arc<dyn SeriesTrait> {
         Arc::new(SeriesWrap(Clone::clone(&self.0)))
     }
 
     fn peak_max(&self) -> BooleanChunked {
```

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/series/implementations/floats.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/series/implementations/floats.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/series/implementations/list.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/series/implementations/list.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/series/implementations/mod.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/series/implementations/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/series/implementations/null.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/series/implementations/null.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/series/implementations/object.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/series/implementations/object.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/series/implementations/struct_.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/series/implementations/struct_.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/series/implementations/utf8.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/series/implementations/utf8.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/series/into.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/series/into.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/series/iterator.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/series/iterator.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/series/mod.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/series/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/series/ops/diff.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/series/ops/diff.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/series/ops/downcast.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/series/ops/downcast.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/series/ops/ewm.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/series/ops/ewm.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/series/ops/mod.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/series/ops/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/series/ops/moment.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/series/ops/moment.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/series/ops/null.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/series/ops/null.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/series/ops/pct_change.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/series/ops/pct_change.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/series/ops/round.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/series/ops/round.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/series/ops/to_list.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/series/ops/to_list.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/series/ops/unique.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/series/ops/unique.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/series/series_trait.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/series/series_trait.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/series/unstable.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/series/unstable.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/testing.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/testing.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/utils/flatten.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/utils/flatten.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/utils/mod.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/utils/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/utils/series.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/utils/series.rs`

 * *Files 10% similar despite different names*

```diff
@@ -27,20 +27,21 @@
 {
     let mut container = Series::full_null("", 0, dtype);
     let mut us = UnstableSeries::new(&mut container);
 
     f(&mut us)
 }
 
-pub fn ensure_sorted_arg(s: &Series) {
-    if !matches!(s.is_sorted_flag(), IsSorted::Ascending) {
+pub fn ensure_sorted_arg(s: &Series, operation: &str) {
+    if matches!(s.is_sorted_flag(), IsSorted::Not) {
         eprintln!(
-            r#"argument is not explicitly sorted
+            "argument in operation '{}' is not explicitly sorted
 
 - If your data is ALREADY sorted, set the sorted flag with: '.set_sorted()'.
 - If your data is NOT sorted, sort the 'expr/series/column' first.
 
 This might become an error in a future version.
-    "#
+    ",
+            operation
         );
     }
 }
```

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-core/src/utils/supertype.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-core/src/utils/supertype.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-utils/LICENSE` & `polars_u64_idx-0.17.9/local_dependencies/polars-time/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-utils/src/arena.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-utils/src/arena.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-utils/src/atomic.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-utils/src/atomic.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-utils/src/cell.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-utils/src/cell.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-utils/src/contention_pool.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-utils/src/contention_pool.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-utils/src/functions.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-utils/src/functions.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-utils/src/hash.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-utils/src/hash.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-utils/src/iter/enumerate_idx.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-utils/src/iter/enumerate_idx.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-utils/src/lib.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-utils/src/lib.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-utils/src/macros.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-utils/src/macros.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-utils/src/slice.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-utils/src/slice.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-utils/src/sort.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-utils/src/sort.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-utils/src/sync.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-utils/src/sync.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-utils/src/unwrap.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-utils/src/unwrap.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-utils/src/wasm.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-utils/src/wasm.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-plan/Cargo.toml` & `polars_u64_idx-0.17.9/local_dependencies/polars-plan/Cargo.toml`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-plan/LICENSE` & `polars_u64_idx-0.17.9/local_dependencies/polars-lazy/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/dot.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/dot.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/dsl/arithmetic.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/dsl/arithmetic.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/dsl/binary.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/dsl/binary.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/dsl/cat.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/dsl/cat.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/dsl/dt.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/dsl/dt.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/dsl/expr.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/dsl/expr.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/dsl/from.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/dsl/from.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/dsl/function_expr/arg_where.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/dsl/function_expr/arg_where.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/dsl/function_expr/binary.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/dsl/function_expr/binary.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/dsl/function_expr/boolean.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/dsl/function_expr/boolean.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/dsl/function_expr/bounds.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/dsl/function_expr/bounds.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/dsl/function_expr/cat.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/dsl/function_expr/cat.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/dsl/function_expr/cum.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/dsl/function_expr/cum.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/dsl/function_expr/datetime.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/dsl/function_expr/datetime.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/dsl/function_expr/dispatch.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/dsl/function_expr/dispatch.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/dsl/function_expr/fill_null.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/dsl/function_expr/fill_null.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/dsl/function_expr/list.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/dsl/function_expr/list.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/dsl/function_expr/log.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/dsl/function_expr/log.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/dsl/function_expr/mod.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/dsl/function_expr/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/dsl/function_expr/pow.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/dsl/function_expr/pow.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/dsl/function_expr/schema.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/dsl/function_expr/schema.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/dsl/function_expr/shift_and_fill.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/dsl/function_expr/shift_and_fill.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/dsl/function_expr/shrink_type.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/dsl/function_expr/shrink_type.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/dsl/function_expr/sign.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/dsl/function_expr/sign.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/dsl/function_expr/strings.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/dsl/function_expr/strings.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/dsl/function_expr/struct_.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/dsl/function_expr/struct_.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/dsl/function_expr/temporal.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/dsl/function_expr/temporal.rs`

 * *Files 16% similar despite different names*

```diff
@@ -17,34 +17,43 @@
                 .cast(&DataType::Datetime(TimeUnit::Milliseconds, None))
                 .unwrap();
             date_offset(s, offset).and_then(|s| s.cast(&DataType::Date))
         }
         DataType::Datetime(tu, tz) => {
             let ca = s.datetime().unwrap();
 
-            fn adder<T: PolarsTimeZone>(
+            fn offset_fn<T: PolarsTimeZone>(
                 tu: TimeUnit,
             ) -> fn(&Duration, i64, Option<&T>) -> PolarsResult<i64> {
                 match tu {
                     TimeUnit::Nanoseconds => Duration::add_ns,
                     TimeUnit::Microseconds => Duration::add_us,
                     TimeUnit::Milliseconds => Duration::add_ms,
                 }
             }
 
             let out = match tz {
                 #[cfg(feature = "timezones")]
                 Some(ref tz) => match tz.parse::<Tz>() {
-                    Ok(tz) => ca.0.try_apply(|v| adder(tu)(&offset, v, Some(&tz))),
+                    Ok(tz) => {
+                        let offset_fn = offset_fn(tu);
+                        ca.0.try_apply(|v| offset_fn(&offset, v, Some(&tz)))
+                    }
                     Err(_) => match parse_offset(tz) {
-                        Ok(tz) => ca.0.try_apply(|v| adder(tu)(&offset, v, Some(&tz))),
+                        Ok(tz) => {
+                            let offset_fn = offset_fn(tu);
+                            ca.0.try_apply(|v| offset_fn(&offset, v, Some(&tz)))
+                        }
                         Err(_) => unreachable!(),
                     },
                 },
-                _ => ca.0.try_apply(|v| adder(tu)(&offset, v, NO_TIMEZONE)),
+                _ => {
+                    let offset_fn = offset_fn(tu);
+                    ca.0.try_apply(|v| offset_fn(&offset, v, NO_TIMEZONE))
+                }
             }?;
             out.cast(&DataType::Datetime(tu, tz))
         }
         dt => polars_bail!(
             ComputeError: "cannot use 'date_offset' on Series of datatype {}", dt,
         ),
     }
```

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/dsl/function_expr/trigonometry.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/dsl/function_expr/trigonometry.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/dsl/functions.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/dsl/functions.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/dsl/list.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/dsl/list.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/dsl/meta.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/dsl/meta.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/dsl/mod.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/dsl/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/dsl/options.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/dsl/options.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/dsl/string.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/dsl/string.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/dsl/struct_.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/dsl/struct_.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/frame/opt_state.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/frame/opt_state.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/logical_plan/aexpr/mod.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/logical_plan/aexpr/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/logical_plan/aexpr/schema.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/logical_plan/aexpr/schema.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/logical_plan/alp.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/logical_plan/alp.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/logical_plan/anonymous_scan.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/logical_plan/anonymous_scan.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/logical_plan/apply.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/logical_plan/apply.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/logical_plan/builder.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/logical_plan/builder.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/logical_plan/conversion.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/logical_plan/conversion.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/logical_plan/format.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/logical_plan/format.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/logical_plan/functions/drop.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/logical_plan/functions/drop.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/logical_plan/functions/merge_sorted.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/logical_plan/functions/merge_sorted.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/logical_plan/functions/mod.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/logical_plan/functions/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/logical_plan/functions/rename.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/logical_plan/functions/rename.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/logical_plan/iterator.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/logical_plan/iterator.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/logical_plan/lit.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/logical_plan/lit.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/logical_plan/mod.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/logical_plan/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/logical_plan/optimizer/cache_states.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/logical_plan/optimizer/cache_states.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/logical_plan/optimizer/cse.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/logical_plan/optimizer/cse.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/logical_plan/optimizer/delay_rechunk.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/logical_plan/optimizer/delay_rechunk.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/logical_plan/optimizer/drop_nulls.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/logical_plan/optimizer/drop_nulls.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/logical_plan/optimizer/fast_projection.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/logical_plan/optimizer/fast_projection.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/logical_plan/optimizer/file_caching.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/logical_plan/optimizer/file_caching.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/logical_plan/optimizer/flatten_union.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/logical_plan/optimizer/flatten_union.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/logical_plan/optimizer/mod.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/logical_plan/optimizer/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/logical_plan/optimizer/predicate_pushdown/keys.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/logical_plan/optimizer/predicate_pushdown/keys.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/logical_plan/optimizer/predicate_pushdown/mod.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/logical_plan/optimizer/predicate_pushdown/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/logical_plan/optimizer/predicate_pushdown/rename.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/logical_plan/optimizer/predicate_pushdown/rename.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/logical_plan/optimizer/predicate_pushdown/utils.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/logical_plan/optimizer/predicate_pushdown/utils.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/functions/melt.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/functions/melt.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/functions/mod.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/functions/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/generic.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/generic.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/groupby.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/groupby.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/hstack.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/hstack.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/joins.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/joins.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/mod.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/projection.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/projection.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/rename.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/rename.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/semi_anti_join.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/semi_anti_join.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/logical_plan/optimizer/simplify_expr.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/logical_plan/optimizer/simplify_expr.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/logical_plan/optimizer/slice_pushdown_expr.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/logical_plan/optimizer/slice_pushdown_expr.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/logical_plan/optimizer/slice_pushdown_lp.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/logical_plan/optimizer/slice_pushdown_lp.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/logical_plan/optimizer/stack_opt.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/logical_plan/optimizer/stack_opt.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/logical_plan/optimizer/type_coercion/binary.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/logical_plan/optimizer/type_coercion/binary.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/logical_plan/optimizer/type_coercion/mod.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/logical_plan/optimizer/type_coercion/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/logical_plan/options.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/logical_plan/options.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/logical_plan/projection.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/logical_plan/projection.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/logical_plan/pyarrow.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/logical_plan/pyarrow.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/logical_plan/schema.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/logical_plan/schema.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/prelude.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/prelude.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-plan/src/utils.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-plan/src/utils.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-time/Cargo.toml` & `polars_u64_idx-0.17.9/local_dependencies/polars-time/Cargo.toml`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-time/LICENSE` & `polars_u64_idx-0.17.9/local_dependencies/polars-algo/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-time/src/chunkedarray/date.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-time/src/chunkedarray/date.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-time/src/chunkedarray/datetime.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-time/src/chunkedarray/datetime.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-time/src/chunkedarray/duration.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-time/src/chunkedarray/duration.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-time/src/chunkedarray/kernels.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-time/src/chunkedarray/kernels.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-time/src/chunkedarray/mod.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-time/src/chunkedarray/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-time/src/chunkedarray/rolling_window/floats.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-time/src/chunkedarray/rolling_window/floats.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-time/src/chunkedarray/rolling_window/ints.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-time/src/chunkedarray/rolling_window/ints.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-time/src/chunkedarray/rolling_window/mod.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-time/src/chunkedarray/rolling_window/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-time/src/chunkedarray/rolling_window/rolling_kernels/no_nulls.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-time/src/chunkedarray/rolling_window/rolling_kernels/no_nulls.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-time/src/chunkedarray/time.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-time/src/chunkedarray/time.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-time/src/chunkedarray/utf8/infer.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-time/src/chunkedarray/utf8/infer.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-time/src/chunkedarray/utf8/mod.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-time/src/chunkedarray/utf8/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-time/src/chunkedarray/utf8/patterns.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-time/src/chunkedarray/utf8/patterns.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-time/src/chunkedarray/utf8/strptime.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-time/src/chunkedarray/utf8/strptime.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-time/src/date_range.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-time/src/date_range.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-time/src/groupby/dynamic.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-time/src/groupby/dynamic.rs`

 * *Files 1% similar despite different names*

```diff
@@ -103,15 +103,18 @@
 impl Wrap<&DataFrame> {
     fn groupby_rolling(
         &self,
         by: Vec<Series>,
         options: &RollingGroupOptions,
     ) -> PolarsResult<(Series, Vec<Series>, GroupsProxy)> {
         let time = self.0.column(&options.index_column)?.clone();
-        ensure_sorted_arg(&time);
+        if by.is_empty() && !options.period.parsed_int {
+            // if by is given, the column must be sorted in the 'by' arg, which we can not check now
+            ensure_sorted_arg(&time, "groupby_rolling");
+        }
         let time_type = time.dtype();
 
         polars_ensure!(time.null_count() == 0, ComputeError: "null values in dynamic groupby not supported, fill nulls.");
 
         use DataType::*;
         let (dt, tu, tz): (Series, TimeUnit, Option<TimeZone>) = match time_type {
             Datetime(tu, tz) => (time.clone(), *tu, tz.clone()),
@@ -179,15 +182,18 @@
                     && (options.every.parsed_int || options.every.is_zero())
                     && (options.period.parsed_int || options.period.is_zero())),
                 ComputeError: "you cannot combine time durations like '2h' with integer durations like '3i'"
             )
         }
 
         let time = self.0.column(&options.index_column)?.rechunk();
-        ensure_sorted_arg(&time);
+        if by.is_empty() && !options.period.parsed_int {
+            // if by is given, the column must be sorted in the 'by' arg, which we can not check now
+            ensure_sorted_arg(&time, "groupby_dynamic");
+        }
         let time_type = time.dtype();
 
         polars_ensure!(time.null_count() == 0, ComputeError: "null values in dynamic groupby not supported, fill nulls.");
 
         use DataType::*;
         let (dt, tu) = match time_type {
             Datetime(tu, _) => (time.clone(), *tu),
```

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-time/src/lib.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-time/src/lib.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-time/src/month_end.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-time/src/month_end.rs`

 * *Files 13% similar despite different names*

```diff
@@ -11,72 +11,66 @@
 
 // roll forward to the last day of the month
 fn roll_forward<T: PolarsTimeZone>(
     t: i64,
     time_zone: Option<&T>,
     timestamp_to_datetime: fn(i64) -> NaiveDateTime,
     datetime_to_timestamp: fn(NaiveDateTime) -> i64,
-    adder: fn(&Duration, i64, Option<&T>) -> PolarsResult<i64>,
+    offset_fn: fn(&Duration, i64, Option<&T>) -> PolarsResult<i64>,
 ) -> PolarsResult<i64> {
     let t = roll_backward(t, time_zone, timestamp_to_datetime, datetime_to_timestamp)?;
-    let t = adder(&Duration::parse("1mo"), t, time_zone)?;
-    adder(&Duration::parse("-1d"), t, time_zone)
+    let t = offset_fn(&Duration::parse("1mo"), t, time_zone)?;
+    offset_fn(&Duration::parse("-1d"), t, time_zone)
 }
 
 pub trait PolarsMonthEnd {
-    fn month_end(&self, time_zone: Option<&impl PolarsTimeZone>) -> PolarsResult<Self>
+    fn month_end<T: PolarsTimeZone>(&self, time_zone: Option<&T>) -> PolarsResult<Self>
     where
         Self: Sized;
 }
 
 impl PolarsMonthEnd for DatetimeChunked {
-    fn month_end(&self, time_zone: Option<&impl PolarsTimeZone>) -> PolarsResult<Self> {
+    fn month_end<T: PolarsTimeZone>(&self, time_zone: Option<&T>) -> PolarsResult<Self> {
         let timestamp_to_datetime: fn(i64) -> NaiveDateTime;
         let datetime_to_timestamp: fn(NaiveDateTime) -> i64;
+        let offset_fn: fn(&Duration, i64, Option<&T>) -> PolarsResult<i64>;
         match self.time_unit() {
             TimeUnit::Nanoseconds => {
                 timestamp_to_datetime = timestamp_ns_to_datetime;
                 datetime_to_timestamp = datetime_to_timestamp_ns;
+                offset_fn = Duration::add_ns;
             }
             TimeUnit::Microseconds => {
                 timestamp_to_datetime = timestamp_us_to_datetime;
                 datetime_to_timestamp = datetime_to_timestamp_us;
+                offset_fn = Duration::add_us;
             }
             TimeUnit::Milliseconds => {
                 timestamp_to_datetime = timestamp_ms_to_datetime;
                 datetime_to_timestamp = datetime_to_timestamp_ms;
+                offset_fn = Duration::add_ms;
             }
         };
-        fn adder<T: PolarsTimeZone>(
-            time_unit: TimeUnit,
-        ) -> fn(&Duration, i64, Option<&T>) -> PolarsResult<i64> {
-            match time_unit {
-                TimeUnit::Nanoseconds => Duration::add_ns,
-                TimeUnit::Microseconds => Duration::add_us,
-                TimeUnit::Milliseconds => Duration::add_ms,
-            }
-        }
-        let adder = adder(self.time_unit());
         Ok(self
             .0
             .try_apply(|t| {
                 roll_forward(
                     t,
                     time_zone,
                     timestamp_to_datetime,
                     datetime_to_timestamp,
-                    adder,
+                    offset_fn,
                 )
             })?
             .into_datetime(self.time_unit(), self.time_zone().clone()))
     }
 }
 
 impl PolarsMonthEnd for DateChunked {
-    fn month_end(&self, _time_zone: Option<&impl PolarsTimeZone>) -> PolarsResult<Self> {
+    fn month_end<T: PolarsTimeZone>(&self, _time_zone: Option<&T>) -> PolarsResult<Self> {
         const MSECS_IN_DAY: i64 = MILLISECONDS * SECONDS_IN_DAY;
         Ok(self
             .0
             .try_apply(|t| {
                 Ok((roll_forward(
                     MSECS_IN_DAY * t as i64,
                     NO_TIMEZONE,
```

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-time/src/month_start.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-time/src/month_start.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-time/src/round.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-time/src/round.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-time/src/series/_trait.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-time/src/series/_trait.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-time/src/series/implementations/floats.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-time/src/series/implementations/floats.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-time/src/series/implementations/integers.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-time/src/series/implementations/integers.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-time/src/series/mod.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-time/src/series/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-time/src/truncate.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-time/src/truncate.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-time/src/upsample.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-time/src/upsample.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 #[cfg(feature = "timezones")]
 use arrow::temporal_conversions::parse_offset;
 use polars_core::prelude::*;
+use polars_core::utils::ensure_sorted_arg;
 use polars_ops::prelude::*;
 
 use crate::prelude::*;
 #[cfg(feature = "timezones")]
 use crate::utils::unlocalize_timestamp;
 
 pub trait PolarsUpsample {
@@ -24,21 +25,21 @@
     /// - 1ms   (1 millisecond)
     /// - 1s    (1 second)
     /// - 1m    (1 minute)
     /// - 1h    (1 hour)
     /// - 1d    (1 day)
     /// - 1w    (1 week)
     /// - 1mo   (1 calendar month)
-    /// - 1mo_saturating (calendar month, but "saturates" to the last day of the month
-    ///   instead of erroring. For example, 2022-01-29 plus `'1mo_saturating'` goes to
-    ///   2022-02-28)
     /// - 1y    (1 calendar year)
     /// - 1i    (1 index count)
     /// Or combine them:
     /// "3d12h4m25s" # 3 days, 12 hours, 4 minutes, and 25 seconds
+    /// Suffix with `"_saturating"` to saturate dates with days too
+    /// large for their month to the last day of the month (e.g.
+    /// 2022-02-29 to 2022-02-28).
     fn upsample<I: IntoVec<String>>(
         &self,
         by: I,
         time_column: &str,
         every: Duration,
         offset: Duration,
     ) -> PolarsResult<DataFrame>;
@@ -105,14 +106,15 @@
     by: Vec<String>,
     index_column: &str,
     every: Duration,
     offset: Duration,
     stable: bool,
 ) -> PolarsResult<DataFrame> {
     let s = source.column(index_column)?;
+    ensure_sorted_arg(s, "upsample");
     if matches!(s.dtype(), DataType::Date) {
         let mut df = source.clone();
         df.try_apply(index_column, |s| {
             s.cast(&DataType::Datetime(TimeUnit::Milliseconds, None))
         })
         .unwrap();
         let mut out = upsample_impl(&df, by, index_column, every, offset, stable).unwrap();
```

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-time/src/utils.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-time/src/utils.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-time/src/windows/bounds.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-time/src/windows/bounds.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-time/src/windows/calendar.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-time/src/windows/calendar.rs`

 * *Files 24% similar despite different names*

```diff
@@ -31,59 +31,66 @@
 pub const NS_MILLISECOND: i64 = 1_000_000;
 pub const NS_SECOND: i64 = 1_000_000_000;
 pub const NS_MINUTE: i64 = 60 * NS_SECOND;
 pub const NS_HOUR: i64 = 60 * NS_MINUTE;
 pub const NS_DAY: i64 = 24 * NS_HOUR;
 pub const NS_WEEK: i64 = 7 * NS_DAY;
 
-pub fn date_range(
+pub fn date_range<T: PolarsTimeZone>(
     start: i64,
     stop: i64,
     every: Duration,
     closed: ClosedWindow,
     tu: TimeUnit,
-    tz: Option<&impl PolarsTimeZone>,
+    tz: Option<&T>,
 ) -> PolarsResult<Vec<i64>> {
-    let size = match tu {
-        TimeUnit::Nanoseconds => ((stop - start) / every.duration_ns() + 1) as usize,
-        TimeUnit::Microseconds => ((stop - start) / every.duration_us() + 1) as usize,
-        TimeUnit::Milliseconds => ((stop - start) / every.duration_ms() + 1) as usize,
-    };
+    let size: usize;
+    let offset_fn: fn(&Duration, i64, Option<&T>) -> PolarsResult<i64>;
+
+    match tu {
+        TimeUnit::Nanoseconds => {
+            size = ((stop - start) / every.duration_ns() + 1) as usize;
+            offset_fn = Duration::add_ns;
+        }
+        TimeUnit::Microseconds => {
+            size = ((stop - start) / every.duration_us() + 1) as usize;
+            offset_fn = Duration::add_us;
+        }
+        TimeUnit::Milliseconds => {
+            size = ((stop - start) / every.duration_ms() + 1) as usize;
+            offset_fn = Duration::add_ms;
+        }
+    }
     let mut ts = Vec::with_capacity(size);
 
     let mut t = start;
-    let f = match tu {
-        TimeUnit::Nanoseconds => <Duration>::add_ns,
-        TimeUnit::Microseconds => <Duration>::add_us,
-        TimeUnit::Milliseconds => <Duration>::add_ms,
-    };
     match closed {
         ClosedWindow::Both => {
             while t <= stop {
                 ts.push(t);
-                t = f(&every, t, tz)?
+                t = offset_fn(&every, t, tz)?
             }
         }
         ClosedWindow::Left => {
             while t < stop {
                 ts.push(t);
-                t = f(&every, t, tz)?
+                t = offset_fn(&every, t, tz)?
             }
         }
         ClosedWindow::Right => {
-            t = f(&every, t, tz)?;
+            t = offset_fn(&every, t, tz)?;
             while t <= stop {
                 ts.push(t);
-                t = f(&every, t, tz)?
+                t = offset_fn(&every, t, tz)?
             }
         }
         ClosedWindow::None => {
-            t = f(&every, t, tz)?;
+            t = offset_fn(&every, t, tz)?;
             while t < stop {
                 ts.push(t);
-                t = f(&every, t, tz)?
+                t = offset_fn(&every, t, tz)?
             }
         }
     }
     debug_assert!(size >= ts.len());
     Ok(ts)
 }
```

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-time/src/windows/duration.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-time/src/windows/duration.rs`

 * *Files 5% similar despite different names*

```diff
@@ -34,17 +34,17 @@
     days: i64,
     // the number of nanoseconds for the duration
     nsecs: i64,
     // indicates if the duration is negative
     pub(crate) negative: bool,
     // indicates if an integer string was passed. e.g. "2i"
     pub parsed_int: bool,
-    // indicates if a '1mo' offset to a non-existent date (e.g. 2022-02-29)
-    // should saturate to 2022-02-28 (as opposed to erroring)
-    pub(crate) saturating_months: Option<bool>,
+    // indicates if an offset to a non-existent date (e.g. 2022-02-29)
+    // should saturate (to 2022-02-28) as opposed to erroring
+    pub(crate) saturating: bool,
 }
 
 impl PartialOrd<Self> for Duration {
     fn partial_cmp(&self, other: &Self) -> Option<Ordering> {
         self.duration_ns().partial_cmp(&other.duration_ns())
     }
 }
@@ -61,15 +61,15 @@
         Duration {
             months: 0,
             weeks: 0,
             days: 0,
             nsecs: fixed_slots.abs(),
             negative: fixed_slots < 0,
             parsed_int: true,
-            saturating_months: None,
+            saturating: false,
         }
     }
 
     /// Parse a string into a `Duration`
     ///
     /// Strings are composed of a sequence of number-unit pairs, such as `5d` (5 days). A string may begin with a minus
     /// sign, in which case it is interpreted as a negative duration. Some examples:
@@ -88,20 +88,21 @@
     /// * `ms`: millisecond
     /// * `s`:  second
     /// * `m`:  minute
     /// * `h`:  hour
     /// * `d`:  day
     /// * `w`:  week
     /// * `mo`: calendar month
-    /// * `mo_saturating`: calendar month, but "saturates" to the last day of the month
-    ///    instead of erroring. For example, 2022-01-29 plus `'1mo_saturating'` goes to
-    ///    2022-02-28.
     /// * `y`:  calendar year
     /// * `i`:  index value (only for {Int32, Int64} dtypes)
     ///
+    /// Suffix with `"_saturating"` to indicate that dates too large for
+    /// their month should saturate at the largest date (e.g. 2022-02-29 -> 2022-02-28)
+    /// instead of erroring.
+    ///
     /// # Panics
     /// If the given str is invalid for any reason.
     pub fn parse(duration: &str) -> Self {
         let num_minus_signs = duration.matches('-').count();
         if num_minus_signs > 1 {
             panic!("a Duration string can only have a single minus sign")
         }
@@ -109,18 +110,23 @@
             panic!("only a single minus sign is allowed, at the front of the string")
         }
 
         let mut nsecs = 0;
         let mut weeks = 0;
         let mut days = 0;
         let mut months = 0;
-        let mut iter = duration.char_indices();
         let negative = duration.starts_with('-');
+        let (saturating, mut iter) = match duration.ends_with("_saturating") {
+            true => (
+                true,
+                duration[..duration.len() - "_saturating".len()].char_indices(),
+            ),
+            false => (false, duration.char_indices()),
+        };
         let mut start = 0;
-        let mut saturating_months: Option<bool> = None;
 
         // skip the '-' char
         if negative {
             start += 1;
             iter.next().unwrap();
         }
 
@@ -130,15 +136,15 @@
         while let Some((i, mut ch)) = iter.next() {
             if !ch.is_ascii_digit() {
                 let n = duration[start..i]
                     .parse::<i64>()
                     .expect("expected an integer in the duration string");
 
                 loop {
-                    if ch.is_ascii_alphabetic() || ch == '_' {
+                    if ch.is_ascii_alphabetic() {
                         unit.push(ch)
                     } else {
                         break;
                     }
                     match iter.next() {
                         Some((i, ch_)) => {
                             ch = ch_;
@@ -159,25 +165,14 @@
                     "ms" => nsecs += n * NS_MILLISECOND,
                     "s" => nsecs += n * NS_SECOND,
                     "m" => nsecs += n * NS_MINUTE,
                     "h" => nsecs += n * NS_HOUR,
                     "d" => days += n,
                     "w" => weeks += n,
                     "mo" => {
-                        if let Some(true) = saturating_months {
-                            panic!("cannot use both saturating and non-saturating months")
-                        }
-                        saturating_months = Some(false);
-                        months += n
-                    }
-                    "mo_saturating" => {
-                        if let Some(false) = saturating_months {
-                            panic!("cannot use both saturating and non-saturating months")
-                        }
-                        saturating_months = Some(true);
                         months += n
                     }
                     "y" => months += n * 12,
                     // we will read indexes as nanoseconds
                     "i" => {
                         nsecs += n;
                         parsed_int = true;
@@ -190,15 +185,15 @@
         Duration {
             nsecs: nsecs.abs(),
             days: days.abs(),
             weeks: weeks.abs(),
             months: months.abs(),
             negative,
             parsed_int,
-            saturating_months,
+            saturating,
         }
     }
 
     fn to_positive(v: i64) -> (bool, i64) {
         if v < 0 {
             (true, -v)
         } else {
@@ -257,57 +252,57 @@
         Self {
             months: 0,
             weeks: 0,
             days: 0,
             nsecs,
             negative,
             parsed_int: false,
-            saturating_months: None,
+            saturating: false,
         }
     }
 
     /// Creates a [`Duration`] that represents a fixed number of months.
     pub(crate) fn from_months(v: i64) -> Self {
         let (negative, months) = Self::to_positive(v);
         Self {
             months,
             weeks: 0,
             days: 0,
             nsecs: 0,
             negative,
             parsed_int: false,
-            saturating_months: None,
+            saturating: false,
         }
     }
 
     /// Creates a [`Duration`] that represents a fixed number of weeks.
     pub(crate) fn from_weeks(v: i64) -> Self {
         let (negative, weeks) = Self::to_positive(v);
         Self {
             months: 0,
             weeks,
             days: 0,
             nsecs: 0,
             negative,
             parsed_int: false,
-            saturating_months: None,
+            saturating: false,
         }
     }
 
     /// Creates a [`Duration`] that represents a fixed number of days.
     pub(crate) fn from_days(v: i64) -> Self {
         let (negative, days) = Self::to_positive(v);
         Self {
             months: 0,
             weeks: 0,
             days,
             nsecs: 0,
             negative,
             parsed_int: false,
-            saturating_months: None,
+            saturating: false,
         }
     }
 
     /// `true` if zero duration.
     pub fn is_zero(&self) -> bool {
         self.months == 0 && self.weeks == 0 && self.days == 0 && self.nsecs == 0
     }
@@ -559,15 +554,15 @@
                 year += 1;
                 month -= 12;
             } else if month <= 0 {
                 year -= 1;
                 month += 12;
             }
 
-            if let Some(true) = d.saturating_months {
+            if d.saturating {
                 // Normalize the day if we are past the end of the month.
                 let mut last_day_of_month = last_day_of_month(month);
                 if month == (chrono::Month::February.number_from_month() as i32)
                     && is_leap_year(year)
                 {
                     last_day_of_month += 1;
                 }
```

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-time/src/windows/groupby.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-time/src/windows/groupby.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-time/src/windows/test.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-time/src/windows/test.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-time/src/windows/window.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-time/src/windows/window.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-lazy/Cargo.toml` & `polars_u64_idx-0.17.9/local_dependencies/polars-lazy/Cargo.toml`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-lazy/LICENSE` & `polars_u64_idx-0.17.9/local_dependencies/polars-utils/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-lazy/src/dot.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-lazy/src/dot.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-lazy/src/dsl/eval.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-lazy/src/dsl/eval.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-lazy/src/dsl/functions.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-lazy/src/dsl/functions.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-lazy/src/dsl/list.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-lazy/src/dsl/list.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-lazy/src/dsl/mod.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-lazy/src/dsl/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-lazy/src/frame/anonymous_scan.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-lazy/src/frame/anonymous_scan.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-lazy/src/frame/csv.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-lazy/src/frame/csv.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-lazy/src/frame/file_list_reader.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-lazy/src/frame/file_list_reader.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-lazy/src/frame/ipc.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-lazy/src/frame/ipc.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-lazy/src/frame/mod.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-lazy/src/frame/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-lazy/src/frame/ndjson.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-lazy/src/frame/ndjson.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-lazy/src/frame/parquet.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-lazy/src/frame/parquet.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-lazy/src/frame/pivot.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-lazy/src/frame/pivot.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-lazy/src/lib.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-lazy/src/lib.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-lazy/src/physical_plan/executors/cache.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-lazy/src/physical_plan/executors/cache.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-lazy/src/physical_plan/executors/executor.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-lazy/src/physical_plan/executors/executor.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-lazy/src/physical_plan/executors/ext_context.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-lazy/src/physical_plan/executors/ext_context.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-lazy/src/physical_plan/executors/filter.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-lazy/src/physical_plan/executors/filter.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-lazy/src/physical_plan/executors/groupby.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-lazy/src/physical_plan/executors/groupby.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-lazy/src/physical_plan/executors/groupby_dynamic.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-lazy/src/physical_plan/executors/groupby_dynamic.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-lazy/src/physical_plan/executors/groupby_partitioned.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-lazy/src/physical_plan/executors/groupby_partitioned.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-lazy/src/physical_plan/executors/groupby_rolling.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-lazy/src/physical_plan/executors/groupby_rolling.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-lazy/src/physical_plan/executors/join.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-lazy/src/physical_plan/executors/join.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-lazy/src/physical_plan/executors/mod.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-lazy/src/physical_plan/executors/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-lazy/src/physical_plan/executors/projection.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-lazy/src/physical_plan/executors/projection.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-lazy/src/physical_plan/executors/python_scan.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-lazy/src/physical_plan/executors/python_scan.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-lazy/src/physical_plan/executors/scan/csv.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-lazy/src/physical_plan/executors/scan/csv.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-lazy/src/physical_plan/executors/scan/ipc.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-lazy/src/physical_plan/executors/scan/ipc.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-lazy/src/physical_plan/executors/scan/mod.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-lazy/src/physical_plan/executors/scan/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-lazy/src/physical_plan/executors/scan/ndjson.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-lazy/src/physical_plan/executors/scan/ndjson.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-lazy/src/physical_plan/executors/scan/parquet.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-lazy/src/physical_plan/executors/scan/parquet.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-lazy/src/physical_plan/executors/slice.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-lazy/src/physical_plan/executors/slice.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-lazy/src/physical_plan/executors/sort.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-lazy/src/physical_plan/executors/sort.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-lazy/src/physical_plan/executors/stack.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-lazy/src/physical_plan/executors/stack.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-lazy/src/physical_plan/executors/udf.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-lazy/src/physical_plan/executors/udf.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-lazy/src/physical_plan/executors/union.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-lazy/src/physical_plan/executors/union.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-lazy/src/physical_plan/executors/unique.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-lazy/src/physical_plan/executors/unique.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-lazy/src/physical_plan/exotic.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-lazy/src/physical_plan/exotic.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-lazy/src/physical_plan/expressions/aggregation.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-lazy/src/physical_plan/expressions/aggregation.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-lazy/src/physical_plan/expressions/alias.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-lazy/src/physical_plan/expressions/alias.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-lazy/src/physical_plan/expressions/apply.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-lazy/src/physical_plan/expressions/apply.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-lazy/src/physical_plan/expressions/binary.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-lazy/src/physical_plan/expressions/binary.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-lazy/src/physical_plan/expressions/cast.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-lazy/src/physical_plan/expressions/cast.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-lazy/src/physical_plan/expressions/column.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-lazy/src/physical_plan/expressions/column.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-lazy/src/physical_plan/expressions/count.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-lazy/src/physical_plan/expressions/count.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-lazy/src/physical_plan/expressions/filter.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-lazy/src/physical_plan/expressions/filter.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-lazy/src/physical_plan/expressions/group_iter.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-lazy/src/physical_plan/expressions/group_iter.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-lazy/src/physical_plan/expressions/literal.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-lazy/src/physical_plan/expressions/literal.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-lazy/src/physical_plan/expressions/mod.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-lazy/src/physical_plan/expressions/mod.rs`

 * *Files 1% similar despite different names*

```diff
@@ -344,15 +344,17 @@
             (true, _) => AggState::AggregatedFlat(series),
             _ => {
                 match self.state {
                     // already aggregated to sum, min even this series was flattened it never could
                     // retrieve the length before grouping, so it stays  in this state.
                     AggState::AggregatedFlat(_) => AggState::AggregatedFlat(series),
                     // applying a function on a literal, keeps the literal state
-                    AggState::Literal(_) if series.len() == 1 => AggState::Literal(series),
+                    AggState::Literal(_) if series.len() == 1 && self.groups.len() > 1 => {
+                        AggState::Literal(series)
+                    }
                     _ => AggState::NotAggregated(series),
                 }
             }
         };
         Ok(self)
     }
```

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-lazy/src/physical_plan/expressions/slice.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-lazy/src/physical_plan/expressions/slice.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-lazy/src/physical_plan/expressions/sort.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-lazy/src/physical_plan/expressions/sort.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-lazy/src/physical_plan/expressions/sortby.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-lazy/src/physical_plan/expressions/sortby.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-lazy/src/physical_plan/expressions/take.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-lazy/src/physical_plan/expressions/take.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-lazy/src/physical_plan/expressions/ternary.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-lazy/src/physical_plan/expressions/ternary.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-lazy/src/physical_plan/expressions/window.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-lazy/src/physical_plan/expressions/window.rs`

 * *Files 1% similar despite different names*

```diff
@@ -403,14 +403,20 @@
         //
         //      - 3.3. MAP to original locations
         //          This will be done for list aggregations that are not explicitly aggregated as list
         //              `(col("x").sum() * col("y")).over("groups")
         //          This can be used to reverse, sort, shuffle etc. the values in a group
 
         // 4. select the final column and return
+
+        if df.height() == 0 {
+            let field = self.phys_function.to_field(&df.schema())?;
+            return Ok(Series::full_null(field.name(), 0, field.data_type()));
+        }
+
         let groupby_columns = self
             .group_by
             .iter()
             .map(|e| e.evaluate(df, state))
             .collect::<PolarsResult<Vec<_>>>()?;
 
         // if the keys are sorted
```

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-lazy/src/physical_plan/file_cache.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-lazy/src/physical_plan/file_cache.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-lazy/src/physical_plan/node_timer.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-lazy/src/physical_plan/node_timer.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-lazy/src/physical_plan/planner/expr.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-lazy/src/physical_plan/planner/expr.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-lazy/src/physical_plan/planner/lp.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-lazy/src/physical_plan/planner/lp.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-lazy/src/physical_plan/state.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-lazy/src/physical_plan/state.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-lazy/src/physical_plan/streaming/convert.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-lazy/src/physical_plan/streaming/convert.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-lazy/src/physical_plan/streaming/tree.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-lazy/src/physical_plan/streaming/tree.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-lazy/src/prelude.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-lazy/src/prelude.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-lazy/src/tests/aggregations.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-lazy/src/tests/aggregations.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-lazy/src/tests/arity.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-lazy/src/tests/arity.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-lazy/src/tests/cse.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-lazy/src/tests/cse.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-lazy/src/tests/io.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-lazy/src/tests/io.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-lazy/src/tests/logical.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-lazy/src/tests/logical.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-lazy/src/tests/mod.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-lazy/src/tests/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-lazy/src/tests/optimization_checks.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-lazy/src/tests/optimization_checks.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-lazy/src/tests/predicate_queries.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-lazy/src/tests/predicate_queries.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-lazy/src/tests/projection_queries.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-lazy/src/tests/projection_queries.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-lazy/src/tests/queries.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-lazy/src/tests/queries.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-lazy/src/tests/streaming.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-lazy/src/tests/streaming.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-lazy/src/tests/tpch.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-lazy/src/tests/tpch.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-lazy/src/utils.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-lazy/src/utils.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars/Cargo.toml` & `polars_u64_idx-0.17.9/local_dependencies/polars/Cargo.toml`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars/LICENSE` & `polars_u64_idx-0.17.9/local_dependencies/polars-io/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars/Makefile` & `polars_u64_idx-0.17.9/local_dependencies/polars/Makefile`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars/src/docs/eager.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars/src/docs/eager.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars/src/docs/lazy.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars/src/docs/lazy.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars/src/docs/performance.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars/src/docs/performance.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars/src/lib.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars/src/lib.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars/tests/it/core/date_like.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars/tests/it/core/date_like.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars/tests/it/core/groupby.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars/tests/it/core/groupby.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars/tests/it/core/joins.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars/tests/it/core/joins.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars/tests/it/core/list.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars/tests/it/core/list.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars/tests/it/core/pivot.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars/tests/it/core/pivot.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars/tests/it/core/random.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars/tests/it/core/random.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars/tests/it/core/rolling_window.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars/tests/it/core/rolling_window.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars/tests/it/core/series.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars/tests/it/core/series.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars/tests/it/io/csv.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars/tests/it/io/csv.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars/tests/it/io/ipc_stream.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars/tests/it/io/ipc_stream.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars/tests/it/io/json.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars/tests/it/io/json.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars/tests/it/io/parquet.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars/tests/it/io/parquet.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars/tests/it/joins.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars/tests/it/joins.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars/tests/it/lazy/aggregation.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars/tests/it/lazy/aggregation.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars/tests/it/lazy/cse.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars/tests/it/lazy/cse.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars/tests/it/lazy/expressions/apply.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars/tests/it/lazy/expressions/apply.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars/tests/it/lazy/expressions/arity.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars/tests/it/lazy/expressions/arity.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars/tests/it/lazy/expressions/expand.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars/tests/it/lazy/expressions/expand.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars/tests/it/lazy/expressions/filter.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars/tests/it/lazy/expressions/filter.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars/tests/it/lazy/expressions/slice.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars/tests/it/lazy/expressions/slice.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars/tests/it/lazy/expressions/window.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars/tests/it/lazy/expressions/window.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars/tests/it/lazy/folds.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars/tests/it/lazy/folds.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars/tests/it/lazy/functions.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars/tests/it/lazy/functions.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars/tests/it/lazy/groupby.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars/tests/it/lazy/groupby.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars/tests/it/lazy/groupby_dynamic.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars/tests/it/lazy/groupby_dynamic.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars/tests/it/lazy/mod.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars/tests/it/lazy/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars/tests/it/lazy/predicate_queries.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars/tests/it/lazy/predicate_queries.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars/tests/it/lazy/projection_queries.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars/tests/it/lazy/projection_queries.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars/tests/it/lazy/queries.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars/tests/it/lazy/queries.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars/tests/it/schema.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars/tests/it/schema.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-row/Cargo.toml` & `polars_u64_idx-0.17.9/local_dependencies/polars-row/Cargo.toml`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-row/LICENSE` & `polars_u64_idx-0.17.9/local_dependencies/polars-ops/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-row/src/encode.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-row/src/encode.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-row/src/encodings/fixed.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-row/src/encodings/fixed.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-row/src/encodings/variable.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-row/src/encodings/variable.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-row/src/lib.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-row/src/lib.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-row/src/row.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-row/src/row.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-row/src/utils.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-row/src/utils.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-algo/Cargo.toml` & `polars_u64_idx-0.17.9/local_dependencies/polars-algo/Cargo.toml`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-algo/LICENSE` & `polars_u64_idx-0.17.9/local_dependencies/polars-pipe/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/local_dependencies/polars-algo/src/algo.rs` & `polars_u64_idx-0.17.9/local_dependencies/polars-algo/src/algo.rs`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 pub fn hist(s: &Series, bins: Option<&Series>, bin_count: Option<usize>) -> Result<DataFrame> {
     let breakpoint_str = &"break_point";
     let s = s.cast(&DataType::Float64)?.sort(false);
 
     // if the bins are provided, then we can just use them
     let bins = if let Some(bins_in) = bins {
-        Series::new(breakpoint_str, bins_in)
+        Series::new(breakpoint_str, bins_in).sort(false)
     } else {
         // data is sorted, so this is O(1)
         let start = s.min::<f64>().unwrap().floor() - 1.0;
         let stop = s.max::<f64>().unwrap().ceil() + 1.0;
 
         // If bin_count is omitted, default to the difference between start and stop (unit bins)
         let bin_count = if let Some(bin_count) = bin_count {
@@ -46,17 +46,19 @@
         DataType::UInt32 => (lit(u32::MIN), AnyValue::UInt32(u32::MAX)),
         DataType::UInt16 => (lit(u32::MIN), AnyValue::UInt16(u16::MAX)),
         _ => polars_bail!(
             InvalidOperation:
             "cannot take histogram of non-numeric types; consider a groupby and count"
         ),
     };
+    let mut bins = bins.extend_constant(max_value, 1)?;
+    bins.set_sorted_flag(IsSorted::Ascending);
 
     let cuts_df = df![
-        breakpoint_str => bins.extend_constant(max_value, 1)?
+        breakpoint_str => bins
     ]?;
 
     let cuts_df = cuts_df
         .lazy()
         .with_column(
             format_str(
                 "({}, {}]",
```

### Comparing `polars_u64_idx-0.17.8/Cargo.toml` & `polars_u64_idx-0.17.9/Cargo.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "py-polars"
-version = "0.17.8"
+version = "0.17.9"
 edition = "2021"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 
 [workspace]
 # prevents package from thinking it's in the workspace
 [target.'cfg(any(not(target_os = "linux"), use_mimalloc))'.dependencies]
```

### Comparing `polars_u64_idx-0.17.8/LICENSE` & `polars_u64_idx-0.17.9/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/Makefile` & `polars_u64_idx-0.17.9/Makefile`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/README.md` & `polars_u64_idx-0.17.9/README.md`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/build.rs` & `polars_u64_idx-0.17.9/build.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/docs/Makefile` & `polars_u64_idx-0.17.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/docs/_templates/autosummary/class.rst` & `polars_u64_idx-0.17.9/docs/_templates/autosummary/class.rst`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/docs/run_live_docs_server.py` & `polars_u64_idx-0.17.9/docs/run_live_docs_server.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/docs/source/_static/css/custom.css` & `polars_u64_idx-0.17.9/docs/source/_static/css/custom.css`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/docs/source/conf.py` & `polars_u64_idx-0.17.9/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/docs/source/reference/api.rst` & `polars_u64_idx-0.17.9/docs/source/reference/api.rst`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/docs/source/reference/config.rst` & `polars_u64_idx-0.17.9/docs/source/reference/config.rst`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/docs/source/reference/dataframe/modify_select.rst` & `polars_u64_idx-0.17.9/docs/source/reference/dataframe/modify_select.rst`

 * *Files 4% similar despite different names*

```diff
@@ -43,14 +43,15 @@
     DataFrame.replace
     DataFrame.replace_at_idx
     DataFrame.reverse
     DataFrame.row
     DataFrame.rows
     DataFrame.sample
     DataFrame.select
+    DataFrame.set_sorted
     DataFrame.shift
     DataFrame.shift_and_fill
     DataFrame.shrink_to_fit
     DataFrame.slice
     DataFrame.sort
     DataFrame.tail
     DataFrame.take_every
```

### Comparing `polars_u64_idx-0.17.8/docs/source/reference/datatypes.rst` & `polars_u64_idx-0.17.9/docs/source/reference/datatypes.rst`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/docs/source/reference/expressions/computation.rst` & `polars_u64_idx-0.17.9/docs/source/reference/expressions/computation.rst`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/docs/source/reference/expressions/functions.rst` & `polars_u64_idx-0.17.9/docs/source/reference/expressions/functions.rst`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/docs/source/reference/expressions/list.rst` & `polars_u64_idx-0.17.9/docs/source/reference/expressions/list.rst`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/docs/source/reference/expressions/modify_select.rst` & `polars_u64_idx-0.17.9/docs/source/reference/expressions/modify_select.rst`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/docs/source/reference/expressions/operators.rst` & `polars_u64_idx-0.17.9/docs/source/reference/expressions/operators.rst`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/docs/source/reference/expressions/string.rst` & `polars_u64_idx-0.17.9/docs/source/reference/expressions/string.rst`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/docs/source/reference/expressions/temporal.rst` & `polars_u64_idx-0.17.9/docs/source/reference/expressions/temporal.rst`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/docs/source/reference/functions.rst` & `polars_u64_idx-0.17.9/docs/source/reference/functions.rst`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/docs/source/reference/io.rst` & `polars_u64_idx-0.17.9/docs/source/reference/io.rst`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/docs/source/reference/lazyframe/modify_select.rst` & `polars_u64_idx-0.17.9/docs/source/reference/lazyframe/modify_select.rst`

 * *Files 1% similar despite different names*

```diff
@@ -27,14 +27,15 @@
     LazyFrame.last
     LazyFrame.limit
     LazyFrame.melt
     LazyFrame.merge_sorted
     LazyFrame.rename
     LazyFrame.reverse
     LazyFrame.select
+    LazyFrame.set_sorted
     LazyFrame.shift
     LazyFrame.shift_and_fill
     LazyFrame.slice
     LazyFrame.sort
     LazyFrame.tail
     LazyFrame.take_every
     LazyFrame.top_k
```

### Comparing `polars_u64_idx-0.17.8/docs/source/reference/series/computation.rst` & `polars_u64_idx-0.17.9/docs/source/reference/series/computation.rst`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/docs/source/reference/series/descriptive.rst` & `polars_u64_idx-0.17.9/docs/source/reference/series/descriptive.rst`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/docs/source/reference/series/list.rst` & `polars_u64_idx-0.17.9/docs/source/reference/series/list.rst`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/docs/source/reference/series/modify_select.rst` & `polars_u64_idx-0.17.9/docs/source/reference/series/modify_select.rst`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/docs/source/reference/series/string.rst` & `polars_u64_idx-0.17.9/docs/source/reference/series/string.rst`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/docs/source/reference/series/temporal.rst` & `polars_u64_idx-0.17.9/docs/source/reference/series/temporal.rst`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/docs/source/reference/testing.rst` & `polars_u64_idx-0.17.9/docs/source/reference/testing.rst`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/polars/__init__.py` & `polars_u64_idx-0.17.9/polars/__init__.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/polars/api.py` & `polars_u64_idx-0.17.9/polars/api.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/polars/config.py` & `polars_u64_idx-0.17.9/polars/config.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/polars/convert.py` & `polars_u64_idx-0.17.9/polars/convert.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/polars/dataframe/_html.py` & `polars_u64_idx-0.17.9/polars/dataframe/_html.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/polars/dataframe/frame.py` & `polars_u64_idx-0.17.9/polars/dataframe/frame.py`

 * *Files 1% similar despite different names*

```diff
@@ -3662,29 +3662,29 @@
         metrics = ["count", "null_count", "mean", "std", "min", "max", "median"]
         percentile_exprs = []
         for p in percentiles or ():
             percentile_exprs.append(F.all().quantile(p).prefix(f"{p}:"))
             metrics.append(f"{p:.0%}")
 
         # execute metrics in parallel
-        res = self.select(
+        df_metrics = self.select(
             F.all().count().prefix("count:"),
             F.all().null_count().prefix("null_count:"),
             F.all().mean().prefix("mean:"),
             F.all().std().prefix("std:"),
             F.all().min().prefix("min:"),
             F.all().max().prefix("max:"),
             F.all().median().prefix("median:"),
             *percentile_exprs,
         ).row(0)
 
         # reshape/cast wide result
         n_cols = len(self.columns)
         described = [
-            res[(n * n_cols) : (n + 1) * n_cols] for n in range(0, len(metrics))
+            df_metrics[(n * n_cols) : (n + 1) * n_cols] for n in range(0, len(metrics))
         ]
         summary = dict(zip(self.columns, list(zip(*described))))
         num_or_bool = NUMERIC_DTYPES | {Boolean}
         for c, tp in self.schema.items():
             summary[c] = [
                 None
                 if (v is None or isinstance(v, dict))
@@ -4595,22 +4595,24 @@
         - 1ms   (1 millisecond)
         - 1s    (1 second)
         - 1m    (1 minute)
         - 1h    (1 hour)
         - 1d    (1 day)
         - 1w    (1 week)
         - 1mo   (1 calendar month)
-        - 1mo_saturating (same as above, but saturates to the last day of the month
-          if the target date does not exist)
         - 1y    (1 calendar year)
         - 1i    (1 index count)
 
         Or combine them:
         "3d12h4m25s" # 3 days, 12 hours, 4 minutes, and 25 seconds
 
+        Suffix with `"_saturating"` to indicate that dates too large for
+        their month should saturate at the largest date (e.g. 2022-02-29 -> 2022-02-28)
+        instead of erroring.
+
         In case of a groupby_rolling on an integer column, the windows are defined by:
 
         - **"1i"      # length 1**
         - **"10i"     # length 10**
 
         Parameters
         ----------
@@ -4643,15 +4645,15 @@
         ...     "2020-01-01 16:42:13",
         ...     "2020-01-01 16:45:09",
         ...     "2020-01-02 18:12:48",
         ...     "2020-01-03 19:45:32",
         ...     "2020-01-08 23:16:43",
         ... ]
         >>> df = pl.DataFrame({"dt": dates, "a": [3, 7, 5, 9, 2, 1]}).with_columns(
-        ...     pl.col("dt").str.strptime(pl.Datetime)
+        ...     pl.col("dt").str.strptime(pl.Datetime).set_sorted()
         ... )
         >>> out = df.groupby_rolling(index_column="dt", period="2d").agg(
         ...     [
         ...         pl.sum("a").alias("sum_a"),
         ...         pl.min("a").alias("min_a"),
         ...         pl.max("a").alias("max_a"),
         ...     ]
@@ -4712,22 +4714,24 @@
         - 1ms   (1 millisecond)
         - 1s    (1 second)
         - 1m    (1 minute)
         - 1h    (1 hour)
         - 1d    (1 day)
         - 1w    (1 week)
         - 1mo   (1 calendar month)
-        - 1mo_saturating (same as above, but saturates to the last day of the month
-          if the target date does not exist)
         - 1y    (1 calendar year)
         - 1i    (1 index count)
 
         Or combine them:
         "3d12h4m25s" # 3 days, 12 hours, 4 minutes, and 25 seconds
 
+        Suffix with `"_saturating"` to indicate that dates too large for
+        their month should saturate at the largest date (e.g. 2022-02-29 -> 2022-02-28)
+        instead of erroring.
+
         In case of a groupby_dynamic on an integer column, the windows are defined by:
 
         - "1i"      # length 1
         - "10i"     # length 10
 
         .. warning::
             The index column must be sorted in ascending order.
@@ -4998,22 +5002,24 @@
         - 1ms   (1 millisecond)
         - 1s    (1 second)
         - 1m    (1 minute)
         - 1h    (1 hour)
         - 1d    (1 day)
         - 1w    (1 week)
         - 1mo   (1 calendar month)
-        - 1mo_saturating (same as above, but saturates to the last day of the month
-          if the target date does not exist)
         - 1y    (1 calendar year)
         - 1i    (1 index count)
 
         Or combine them:
         "3d12h4m25s" # 3 days, 12 hours, 4 minutes, and 25 seconds
 
+        Suffix with `"_saturating"` to indicate that dates too large for
+        their month should saturate at the largest date (e.g. 2022-02-29 -> 2022-02-28)
+        instead of erroring.
+
         Examples
         --------
         Upsample a DataFrame by a certain interval.
 
         >>> from datetime import datetime
         >>> df = pl.DataFrame(
         ...     {
@@ -5022,15 +5028,15 @@
         ...             datetime(2021, 4, 1),
         ...             datetime(2021, 5, 1),
         ...             datetime(2021, 6, 1),
         ...         ],
         ...         "groups": ["A", "B", "A", "B"],
         ...         "values": [0, 1, 2, 3],
         ...     }
-        ... )
+        ... ).set_sorted("time")
         >>> df.upsample(
         ...     time_column="time", every="1mo", by="groups", maintain_order=True
         ... ).select(pl.all().forward_fill())
         shape: (7, 3)
         ┌─────────────────────┬────────┬────────┐
         │ time                ┆ groups ┆ values │
         │ ---                 ┆ ---    ┆ ---    │
@@ -5126,22 +5132,24 @@
                 - 1ms   (1 millisecond)
                 - 1s    (1 second)
                 - 1m    (1 minute)
                 - 1h    (1 hour)
                 - 1d    (1 day)
                 - 1w    (1 week)
                 - 1mo   (1 calendar month)
-                - 1mo_saturating (same as above, but saturates to the last day of the
-                  month if the target date does not exist)
                 - 1y    (1 calendar year)
                 - 1i    (1 index count)
 
                 Or combine them:
                 "3d12h4m25s" # 3 days, 12 hours, 4 minutes, and 25 seconds
 
+                Suffix with `"_saturating"` to indicate that dates too large for
+                their month should saturate at the largest date
+                (e.g. 2022-02-29 -> 2022-02-28) instead of erroring.
+
         allow_parallel
             Allow the physical plan to optionally evaluate the computation of both
             DataFrames up to the join in parallel.
         force_parallel
             Force the physical plan to evaluate the computation of both DataFrames up to
             the join in parallel.
 
@@ -5154,29 +5162,27 @@
         ...             datetime(2016, 1, 1),
         ...             datetime(2017, 1, 1),
         ...             datetime(2018, 1, 1),
         ...             datetime(2019, 1, 1),
         ...         ],  # note record date: Jan 1st (sorted!)
         ...         "gdp": [4164, 4411, 4566, 4696],
         ...     }
-        ... )
+        ... ).set_sorted("date")
         >>> population = pl.DataFrame(
         ...     {
         ...         "date": [
         ...             datetime(2016, 5, 12),
         ...             datetime(2017, 5, 12),
         ...             datetime(2018, 5, 12),
         ...             datetime(2019, 5, 12),
         ...         ],  # note record date: May 12th (sorted!)
         ...         "population": [82.19, 82.66, 83.12, 83.52],
         ...     }
-        ... )
-        >>> population.join_asof(
-        ...     gdp, left_on="date", right_on="date", strategy="backward"
-        ... )
+        ... ).set_sorted("date")
+        >>> population.join_asof(gdp, on="date", strategy="backward")
         shape: (4, 3)
         ┌─────────────────────┬────────────┬──────┐
         │ date                ┆ population ┆ gdp  │
         │ ---                 ┆ ---        ┆ ---  │
         │ datetime[μs]        ┆ f64        ┆ i64  │
         ╞═════════════════════╪════════════╪══════╡
         │ 2016-05-12 00:00:00 ┆ 82.19      ┆ 4164 │
@@ -8496,14 +8502,39 @@
         return self._from_pydf(
             self.lazy()
             .merge_sorted(other.lazy(), key)
             .collect(no_optimization=True)
             ._df
         )
 
+    def set_sorted(
+        self,
+        column: IntoExpr | Iterable[IntoExpr],
+        *more_columns: IntoExpr,
+        descending: bool = False,
+    ) -> Self:
+        """
+        Indicate that one or multiple columns are sorted.
+
+        Parameters
+        ----------
+        column
+            Columns that are sorted
+        more_columns
+            Additional columns that are sorted, specified as positional arguments.
+        descending
+            Whether the columns are sorted in descending order.
+        """
+        return self._from_pydf(
+            self.lazy()
+            .set_sorted(column, *more_columns, descending=descending)
+            .collect(no_optimization=True)
+            ._df
+        )
+
     def update(
         self,
         other: DataFrame,
         on: str | Sequence[str] | None = None,
         how: Literal["left", "inner"] = "left",
     ) -> Self:
         """
```

### Comparing `polars_u64_idx-0.17.8/polars/dataframe/groupby.py` & `polars_u64_idx-0.17.9/polars/dataframe/groupby.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/polars/datatypes/__init__.py` & `polars_u64_idx-0.17.9/polars/datatypes/__init__.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/polars/datatypes/classes.py` & `polars_u64_idx-0.17.9/polars/datatypes/classes.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/polars/datatypes/constants.py` & `polars_u64_idx-0.17.9/polars/datatypes/constants.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/polars/datatypes/constructor.py` & `polars_u64_idx-0.17.9/polars/datatypes/constructor.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/polars/datatypes/convert.py` & `polars_u64_idx-0.17.9/polars/datatypes/convert.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/polars/dependencies.py` & `polars_u64_idx-0.17.9/polars/dependencies.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/polars/exceptions.py` & `polars_u64_idx-0.17.9/polars/exceptions.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/polars/expr/binary.py` & `polars_u64_idx-0.17.9/polars/expr/binary.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/polars/expr/categorical.py` & `polars_u64_idx-0.17.9/polars/expr/categorical.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/polars/expr/datetime.py` & `polars_u64_idx-0.17.9/polars/expr/datetime.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,14 +61,18 @@
           if the target date does not exist
         - 1y  # 1 calendar year
 
         These strings can be combined:
 
         - 3d12h4m25s # 3 days, 12 hours, 4 minutes, and 25 seconds
 
+        Suffix with `"_saturating"` to indicate that dates too large for
+        their month should saturate at the largest date (e.g. 2022-02-29 -> 2022-02-28)
+        instead of erroring.
+
         Returns
         -------
         Date/Datetime series
 
         Examples
         --------
         >>> from datetime import timedelta, datetime
@@ -172,20 +176,22 @@
         1ms  # 1 millisecond
         1s   # 1 second
         1m   # 1 minute
         1h   # 1 hour
         1d   # 1 day
         1w   # 1 calendar week
         1mo  # 1 calendar month
-        1mo_saturating  # same as above, but saturates to the last day of the month
-        # if the target date does not exist
         1y   # 1 calendar year
 
         eg: 3d12h4m25s  # 3 days, 12 hours, 4 minutes, and 25 seconds
 
+        Suffix with `"_saturating"` to indicate that dates too large for
+        their month should saturate at the largest date (e.g. 2022-02-29 -> 2022-02-28)
+        instead of erroring.
+
         Returns
         -------
         Date/Datetime series
 
         Warnings
         --------
         This functionality is currently experimental and may
@@ -1670,19 +1676,21 @@
             - 1ms   (1 millisecond)
             - 1s    (1 second)
             - 1m    (1 minute)
             - 1h    (1 hour)
             - 1d    (1 day)
             - 1w    (1 week)
             - 1mo   (1 calendar month)
-            - 1mo_saturating (same as above, but saturates to the last day of the month
-              if the target date does not exist)
             - 1y    (1 calendar year)
             - 1i    (1 index count)
 
+        Suffix with `"_saturating"` to indicate that dates too large for
+        their month should saturate at the largest date (e.g. 2022-02-29 -> 2022-02-28)
+        instead of erroring.
+
         Returns
         -------
         Date/Datetime expression
 
         Examples
         --------
         >>> from datetime import datetime
```

### Comparing `polars_u64_idx-0.17.8/polars/expr/expr.py` & `polars_u64_idx-0.17.9/polars/expr/expr.py`

 * *Files 0% similar despite different names*

```diff
@@ -4577,19 +4577,21 @@
             - 1ms   (1 millisecond)
             - 1s    (1 second)
             - 1m    (1 minute)
             - 1h    (1 hour)
             - 1d    (1 day)
             - 1w    (1 week)
             - 1mo   (1 calendar month)
-            - 1mo_saturating (same as above, but saturates to the last day of the month
-              if the target date does not exist)
             - 1y    (1 calendar year)
             - 1i    (1 index count)
 
+            Suffix with `"_saturating"` to indicate that dates too large for
+            their month should saturate at the largest date
+            (e.g. 2022-02-29 -> 2022-02-28) instead of erroring.
+
             If a timedelta or the dynamic string language is used, the `by`
             and `closed` arguments must also be set.
         weights
             An optional slice with the same length as the window that will be multiplied
             elementwise with the values in the window.
         min_periods
             The number of values in the window that should be non-null before computing
@@ -4674,19 +4676,21 @@
             - 1ms   (1 millisecond)
             - 1s    (1 second)
             - 1m    (1 minute)
             - 1h    (1 hour)
             - 1d    (1 day)
             - 1w    (1 week)
             - 1mo   (1 calendar month)
-            - 1mo_saturating (same as above, but saturates to the last day of the month
-              if the target date does not exist)
             - 1y    (1 calendar year)
             - 1i    (1 index count)
 
+            Suffix with `"_saturating"` to indicate that dates too large for
+            their month should saturate at the largest date
+            (e.g. 2022-02-29 -> 2022-02-28) instead of erroring.
+
             If a timedelta or the dynamic string language is used, the `by`
             and `closed` arguments must also be set.
         weights
             An optional slice with the same length as the window that will be multiplied
             elementwise with the values in the window.
         min_periods
             The number of values in the window that should be non-null before computing
@@ -4771,19 +4775,21 @@
             - 1ms   (1 millisecond)
             - 1s    (1 second)
             - 1m    (1 minute)
             - 1h    (1 hour)
             - 1d    (1 day)
             - 1w    (1 week)
             - 1mo   (1 calendar month)
-            - 1mo_saturating (same as above, but saturates to the last day of the month
-              if the target date does not exist)
             - 1y    (1 calendar year)
             - 1i    (1 index count)
 
+            Suffix with `"_saturating"` to indicate that dates too large for
+            their month should saturate at the largest date
+            (e.g. 2022-02-29 -> 2022-02-28) instead of erroring.
+
             If a timedelta or the dynamic string language is used, the `by`
             and `closed` arguments must also be set.
         weights
             An optional slice with the same length as the window that will be multiplied
             elementwise with the values in the window.
         min_periods
             The number of values in the window that should be non-null before computing
@@ -4868,19 +4874,21 @@
             - 1ms   (1 millisecond)
             - 1s    (1 second)
             - 1m    (1 minute)
             - 1h    (1 hour)
             - 1d    (1 day)
             - 1w    (1 week)
             - 1mo   (1 calendar month)
-            - 1mo_saturating (same as above, but saturates to the last day of the month
-              if the target date does not exist)
             - 1y    (1 calendar year)
             - 1i    (1 index count)
 
+            Suffix with `"_saturating"` to indicate that dates too large for
+            their month should saturate at the largest date
+            (e.g. 2022-02-29 -> 2022-02-28) instead of erroring.
+
             If a timedelta or the dynamic string language is used, the `by`
             and `closed` arguments must also be set.
         weights
             An optional slice with the same length of the window that will be multiplied
             elementwise with the values in the window.
         min_periods
             The number of values in the window that should be non-null before computing
@@ -4965,19 +4973,21 @@
             - 1ms   (1 millisecond)
             - 1s    (1 second)
             - 1m    (1 minute)
             - 1h    (1 hour)
             - 1d    (1 day)
             - 1w    (1 week)
             - 1mo   (1 calendar month)
-            - 1mo_saturating (same as above, but saturates to the last day of the month
-              if the target date does not exist)
             - 1y    (1 calendar year)
             - 1i    (1 index count)
 
+            Suffix with `"_saturating"` to indicate that dates too large for
+            their month should saturate at the largest date
+            (e.g. 2022-02-29 -> 2022-02-28) instead of erroring.
+
             If a timedelta or the dynamic string language is used, the `by`
             and `closed` arguments must also be set.
         weights
             An optional slice with the same length as the window that will be multiplied
             elementwise with the values in the window.
         min_periods
             The number of values in the window that should be non-null before computing
@@ -5062,19 +5072,21 @@
             - 1ms   (1 millisecond)
             - 1s    (1 second)
             - 1m    (1 minute)
             - 1h    (1 hour)
             - 1d    (1 day)
             - 1w    (1 week)
             - 1mo   (1 calendar month)
-            - 1mo_saturating (same as above, but saturates to the last day of the month
-              if the target date does not exist)
             - 1y    (1 calendar year)
             - 1i    (1 index count)
 
+            Suffix with `"_saturating"` to indicate that dates too large for
+            their month should saturate at the largest date
+            (e.g. 2022-02-29 -> 2022-02-28) instead of erroring.
+
             If a timedelta or the dynamic string language is used, the `by`
             and `closed` arguments must also be set.
         weights
             An optional slice with the same length as the window that will be multiplied
             elementwise with the values in the window.
         min_periods
             The number of values in the window that should be non-null before computing
@@ -5155,19 +5167,21 @@
             - 1ms   (1 millisecond)
             - 1s    (1 second)
             - 1m    (1 minute)
             - 1h    (1 hour)
             - 1d    (1 day)
             - 1w    (1 week)
             - 1mo   (1 calendar month)
-            - 1mo_saturating (same as above, but saturates to the last day of the month
-              if the target date does not exist)
             - 1y    (1 calendar year)
             - 1i    (1 index count)
 
+            Suffix with `"_saturating"` to indicate that dates too large for
+            their month should saturate at the largest date
+            (e.g. 2022-02-29 -> 2022-02-28) instead of erroring.
+
             If a timedelta or the dynamic string language is used, the `by`
             and `closed` arguments must also be set.
         weights
             An optional slice with the same length as the window that will be multiplied
             elementwise with the values in the window.
         min_periods
             The number of values in the window that should be non-null before computing
@@ -5254,19 +5268,21 @@
             - 1ms   (1 millisecond)
             - 1s    (1 second)
             - 1m    (1 minute)
             - 1h    (1 hour)
             - 1d    (1 day)
             - 1w    (1 week)
             - 1mo   (1 calendar month)
-            - 1mo_saturating (same as above, but saturates to the last day of the month
-              if the target date does not exist)
             - 1y    (1 calendar year)
             - 1i    (1 index count)
 
+            Suffix with `"_saturating"` to indicate that dates too large for
+            their month should saturate at the largest date
+            (e.g. 2022-02-29 -> 2022-02-28) instead of erroring.
+
             If a timedelta or the dynamic string language is used, the `by`
             and `closed` arguments must also be set.
         weights
             An optional slice with the same length as the window that will be multiplied
             elementwise with the values in the window.
         min_periods
             The number of values in the window that should be non-null before computing
```

### Comparing `polars_u64_idx-0.17.8/polars/expr/list.py` & `polars_u64_idx-0.17.9/polars/expr/list.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/polars/expr/meta.py` & `polars_u64_idx-0.17.9/polars/expr/meta.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/polars/expr/string.py` & `polars_u64_idx-0.17.9/polars/expr/string.py`

 * *Files 1% similar despite different names*

```diff
@@ -129,27 +129,26 @@
             )
 
         if dtype == Date:
             return wrap_expr(self._pyexpr.str_to_date(format, strict, exact, cache))
         elif dtype == Datetime:
             time_unit = dtype.time_unit  # type: ignore[union-attr]
             time_zone = dtype.time_zone  # type: ignore[union-attr]
-            dtcol = wrap_expr(
+            return wrap_expr(
                 self._pyexpr.str_to_datetime(
                     format,
                     time_unit,
                     time_zone,
                     strict,
                     exact,
                     cache,
                     tz_aware,
                     utc,
                 )
             )
-            return dtcol if (time_unit is None) else dtcol.dt.cast_time_unit(time_unit)
         elif dtype == Time:
             return wrap_expr(self._pyexpr.str_to_time(format, strict, exact, cache))
         else:
             raise ValueError("dtype should be of type {Date, Datetime, Time}")
 
     def lengths(self) -> Expr:
         """
```

### Comparing `polars_u64_idx-0.17.8/polars/expr/struct.py` & `polars_u64_idx-0.17.9/polars/expr/struct.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/polars/functions/__init__.py` & `polars_u64_idx-0.17.9/polars/functions/__init__.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/polars/functions/eager.py` & `polars_u64_idx-0.17.9/polars/functions/eager.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/polars/functions/lazy.py` & `polars_u64_idx-0.17.9/polars/functions/lazy.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/polars/functions/whenthen.py` & `polars_u64_idx-0.17.9/polars/functions/whenthen.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/polars/io/__init__.py` & `polars_u64_idx-0.17.9/polars/io/__init__.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/polars/io/_utils.py` & `polars_u64_idx-0.17.9/polars/io/_utils.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/polars/io/avro.py` & `polars_u64_idx-0.17.9/polars/io/avro.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/polars/io/csv/_utils.py` & `polars_u64_idx-0.17.9/polars/io/csv/_utils.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/polars/io/csv/batched_reader.py` & `polars_u64_idx-0.17.9/polars/io/csv/batched_reader.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/polars/io/csv/functions.py` & `polars_u64_idx-0.17.9/polars/io/csv/functions.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/polars/io/database.py` & `polars_u64_idx-0.17.9/polars/io/database.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/polars/io/delta.py` & `polars_u64_idx-0.17.9/polars/io/delta.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/polars/io/excel/_write_utils.py` & `polars_u64_idx-0.17.9/polars/io/excel/_write_utils.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/polars/io/excel/functions.py` & `polars_u64_idx-0.17.9/polars/io/excel/functions.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/polars/io/ipc/anonymous_scan.py` & `polars_u64_idx-0.17.9/polars/io/ipc/anonymous_scan.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/polars/io/ipc/functions.py` & `polars_u64_idx-0.17.9/polars/io/ipc/functions.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/polars/io/json.py` & `polars_u64_idx-0.17.9/polars/io/json.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/polars/io/ndjson.py` & `polars_u64_idx-0.17.9/polars/io/ndjson.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/polars/io/parquet/anonymous_scan.py` & `polars_u64_idx-0.17.9/polars/io/parquet/anonymous_scan.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/polars/io/parquet/functions.py` & `polars_u64_idx-0.17.9/polars/io/parquet/functions.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/polars/io/pyarrow_dataset/anonymous_scan.py` & `polars_u64_idx-0.17.9/polars/io/pyarrow_dataset/anonymous_scan.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/polars/io/pyarrow_dataset/functions.py` & `polars_u64_idx-0.17.9/polars/io/pyarrow_dataset/functions.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/polars/lazyframe/frame.py` & `polars_u64_idx-0.17.9/polars/lazyframe/frame.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 from polars.dependencies import subprocess
 from polars.io._utils import _is_local_file
 from polars.io.ipc.anonymous_scan import _scan_ipc_fsspec
 from polars.io.parquet.anonymous_scan import _scan_parquet_fsspec
 from polars.lazyframe.groupby import LazyGroupBy
 from polars.slice import LazyPolarsSlice
 from polars.utils._parse_expr_input import expr_to_lit_or_expr, selection_to_pyexpr_list
-from polars.utils._wrap import wrap_df
+from polars.utils._wrap import wrap_df, wrap_expr
 from polars.utils.convert import _timedelta_to_pl_duration
 from polars.utils.various import (
     _in_notebook,
     _prepare_row_count_args,
     _process_null_values,
     find_stacklevel,
     normalise_filepath,
@@ -2281,22 +2281,24 @@
         - 1ms   (1 millisecond)
         - 1s    (1 second)
         - 1m    (1 minute)
         - 1h    (1 hour)
         - 1d    (1 day)
         - 1w    (1 week)
         - 1mo   (1 calendar month)
-        - 1mo_saturating (same as above, but saturates to the last day of the month
-          if the target date does not exist)
         - 1y    (1 calendar year)
         - 1i    (1 index count)
 
         Or combine them:
         "3d12h4m25s" # 3 days, 12 hours, 4 minutes, and 25 seconds
 
+        Suffix with `"_saturating"` to indicate that dates too large for
+        their month should saturate at the largest date (e.g. 2022-02-29 -> 2022-02-28)
+        instead of erroring.
+
         In case of a groupby_rolling on an integer column, the windows are defined by:
 
         - "1i"      # length 1
         - "10i"     # length 10
 
         Parameters
         ----------
@@ -2329,15 +2331,15 @@
         ...     "2020-01-01 16:42:13",
         ...     "2020-01-01 16:45:09",
         ...     "2020-01-02 18:12:48",
         ...     "2020-01-03 19:45:32",
         ...     "2020-01-08 23:16:43",
         ... ]
         >>> df = pl.LazyFrame({"dt": dates, "a": [3, 7, 5, 9, 2, 1]}).with_columns(
-        ...     pl.col("dt").str.strptime(pl.Datetime)
+        ...     pl.col("dt").str.strptime(pl.Datetime).set_sorted()
         ... )
         >>> out = (
         ...     df.groupby_rolling(index_column="dt", period="2d")
         ...     .agg(
         ...         [
         ...             pl.sum("a").alias("sum_a"),
         ...             pl.min("a").alias("min_a"),
@@ -2412,22 +2414,24 @@
         - 1ms   (1 millisecond)
         - 1s    (1 second)
         - 1m    (1 minute)
         - 1h    (1 hour)
         - 1d    (1 day)
         - 1w    (1 week)
         - 1mo   (1 calendar month)
-        - 1mo_saturating (same as above, but saturates to the last day of the month
-          if the target date does not exist)
         - 1y    (1 calendar year)
         - 1i    (1 index count)
 
         Or combine them:
         "3d12h4m25s" # 3 days, 12 hours, 4 minutes, and 25 seconds
 
+        Suffix with `"_saturating"` to indicate that dates too large for
+        their month should saturate at the largest date (e.g. 2022-02-29 -> 2022-02-28)
+        instead of erroring.
+
         In case of a groupby_dynamic on an integer column, the windows are defined by:
 
         - "1i"      # length 1
         - "10i"     # length 10
 
         .. warning::
             The index column must be sorted in ascending order.
@@ -2745,22 +2749,24 @@
                 - 1ms   (1 millisecond)
                 - 1s    (1 second)
                 - 1m    (1 minute)
                 - 1h    (1 hour)
                 - 1d    (1 day)
                 - 1w    (1 week)
                 - 1mo   (1 calendar month)
-                - 1mo_saturating (same as above, but saturates to the last day of the
-                  month if the target date does not exist)
                 - 1y    (1 calendar year)
                 - 1i    (1 index count)
 
                 Or combine them:
                 "3d12h4m25s" # 3 days, 12 hours, 4 minutes, and 25 seconds
 
+                Suffix with `"_saturating"` to indicate that dates too large for
+                their month should saturate at the largest date
+                (e.g. 2022-02-29 -> 2022-02-28) instead of erroring.
+
         allow_parallel
             Allow the physical plan to optionally evaluate the computation of both
             DataFrames up to the join in parallel.
         force_parallel
             Force the physical plan to evaluate the computation of both DataFrames up to
             the join in parallel.
 
@@ -2773,29 +2779,27 @@
         ...             datetime(2016, 1, 1),
         ...             datetime(2017, 1, 1),
         ...             datetime(2018, 1, 1),
         ...             datetime(2019, 1, 1),
         ...         ],  # note record date: Jan 1st (sorted!)
         ...         "gdp": [4164, 4411, 4566, 4696],
         ...     }
-        ... )
+        ... ).set_sorted("date")
         >>> population = pl.LazyFrame(
         ...     {
         ...         "date": [
         ...             datetime(2016, 5, 12),
         ...             datetime(2017, 5, 12),
         ...             datetime(2018, 5, 12),
         ...             datetime(2019, 5, 12),
         ...         ],  # note record date: May 12th (sorted!)
         ...         "population": [82.19, 82.66, 83.12, 83.52],
         ...     }
-        ... )
-        >>> population.join_asof(
-        ...     gdp, left_on="date", right_on="date", strategy="backward"
-        ... ).collect()
+        ... ).set_sorted("date")
+        >>> population.join_asof(gdp, on="date", strategy="backward").collect()
         shape: (4, 3)
         ┌─────────────────────┬────────────┬──────┐
         │ date                ┆ population ┆ gdp  │
         │ ---                 ┆ ---        ┆ ---  │
         │ datetime[μs]        ┆ f64        ┆ i64  │
         ╞═════════════════════╪════════════╪══════╡
         │ 2016-05-12 00:00:00 ┆ 82.19      ┆ 4164 │
@@ -4675,14 +4679,39 @@
             Other DataFrame that must be merged
         key
             Key that is sorted.
 
         """
         return self._from_pyldf(self._ldf.merge_sorted(other._ldf, key))
 
+    def set_sorted(
+        self,
+        column: IntoExpr | Iterable[IntoExpr],
+        *more_columns: IntoExpr,
+        descending: bool = False,
+    ) -> Self:
+        """
+        Indicate that one or multiple columns are sorted.
+
+        Parameters
+        ----------
+        column
+            Columns that are sorted
+        more_columns
+            Additional columns that are sorted, specified as positional arguments.
+        descending
+            Whether the columns are sorted in descending order.
+        """
+        columns = selection_to_pyexpr_list(column)
+        if more_columns:
+            columns.extend(selection_to_pyexpr_list(more_columns))
+        return self.with_columns(
+            [wrap_expr(e).set_sorted(descending=descending) for e in columns]
+        )
+
     def update(
         self,
         other: LazyFrame,
         on: str | Sequence[str] | None = None,
         how: Literal["left", "inner"] = "left",
     ) -> Self:
         """
```

### Comparing `polars_u64_idx-0.17.8/polars/lazyframe/groupby.py` & `polars_u64_idx-0.17.9/polars/lazyframe/groupby.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/polars/series/_numpy.py` & `polars_u64_idx-0.17.9/polars/series/_numpy.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/polars/series/binary.py` & `polars_u64_idx-0.17.9/polars/series/binary.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/polars/series/categorical.py` & `polars_u64_idx-0.17.9/polars/series/categorical.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/polars/series/datetime.py` & `polars_u64_idx-0.17.9/polars/series/datetime.py`

 * *Files 1% similar despite different names*

```diff
@@ -1438,19 +1438,21 @@
             - 1ms   (1 millisecond)
             - 1s    (1 second)
             - 1m    (1 minute)
             - 1h    (1 hour)
             - 1d    (1 day)
             - 1w    (1 week)
             - 1mo   (1 calendar month)
-            - 1mo_saturating (same as above, but saturates to the last day of the month
-              if the target date does not exist)
             - 1y    (1 calendar year)
             - 1i    (1 index count)
 
+            Suffix with `"_saturating"` to indicate that dates too large for
+            their month should saturate at the largest date
+            (e.g. 2022-02-29 -> 2022-02-28) instead of erroring.
+
         Returns
         -------
         Date/Datetime expression
 
         Examples
         --------
         >>> from datetime import datetime
@@ -1531,22 +1533,24 @@
         - 1ms # 1 millisecond
         - 1s  # 1 second
         - 1m  # 1 minute
         - 1h  # 1 hour
         - 1d  # 1 day
         - 1w  # 1 calendar week
         - 1mo # 1 calendar month
-        - 1mo_saturating  # same as above, but saturates to the last day of the month
-          if the target date does not exist
         - 1y  # 1 calendar year
 
         These strings can be combined:
 
         - 3d12h4m25s # 3 days, 12 hours, 4 minutes, and 25 seconds
 
+        Suffix with `"_saturating"` to indicate that dates too large for
+        their month should saturate at the largest date (e.g. 2022-02-29 -> 2022-02-28)
+        instead of erroring.
+
         Returns
         -------
         Date/Datetime series
 
         Examples
         --------
         >>> from datetime import timedelta, datetime
@@ -1635,20 +1639,22 @@
         1ms # 1 millisecond
         1s  # 1 second
         1m  # 1 minute
         1h  # 1 hour
         1d  # 1 day
         1w  # 1 calendar week
         1mo # 1 calendar month
-        1mo_saturating  # same as above, but saturates to the last day of the month
-        # if the target date does not exist
         1y  # 1 calendar year
 
         3d12h4m25s # 3 days, 12 hours, 4 minutes, and 25 seconds
 
+        Suffix with `"_saturating"` to indicate that dates too large for
+        their month should saturate at the largest date (e.g. 2022-02-29 -> 2022-02-28)
+        instead of erroring.
+
         Parameters
         ----------
         every
             Every interval start and period length
         offset
             Offset the window
```

### Comparing `polars_u64_idx-0.17.8/polars/series/list.py` & `polars_u64_idx-0.17.9/polars/series/list.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/polars/series/series.py` & `polars_u64_idx-0.17.9/polars/series/series.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/polars/series/string.py` & `polars_u64_idx-0.17.9/polars/series/string.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/polars/series/struct.py` & `polars_u64_idx-0.17.9/polars/series/struct.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/polars/series/utils.py` & `polars_u64_idx-0.17.9/polars/series/utils.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/polars/slice.py` & `polars_u64_idx-0.17.9/polars/slice.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/polars/sql/context.py` & `polars_u64_idx-0.17.9/polars/sql/context.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/polars/string_cache.py` & `polars_u64_idx-0.17.9/polars/string_cache.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/polars/testing/_private.py` & `polars_u64_idx-0.17.9/polars/testing/_private.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/polars/testing/_tempdir.py` & `polars_u64_idx-0.17.9/polars/testing/_tempdir.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/polars/testing/asserts.py` & `polars_u64_idx-0.17.9/polars/testing/asserts.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/polars/testing/parametric/__init__.py` & `polars_u64_idx-0.17.9/polars/testing/parametric/__init__.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/polars/testing/parametric/primitives.py` & `polars_u64_idx-0.17.9/polars/testing/parametric/primitives.py`

 * *Files 7% similar despite different names*

```diff
@@ -86,14 +86,15 @@
     unique : bool, optional
         flag indicating that all values generated for the column should be unique.
 
     Examples
     --------
     >>> from hypothesis.strategies import sampled_from
     >>> from polars.testing.parametric import column
+    >>>
     >>> column(name="unique_small_ints", dtype=pl.UInt8, unique=True)
     column(name='unique_small_ints', dtype=UInt8, strategy=None, null_probability=None, unique=True)
     >>> column(name="ccy", strategy=sampled_from(["GBP", "EUR", "JPY"]))
     column(name='ccy', dtype=Utf8, strategy=sampled_from(['GBP', 'EUR', 'JPY']), null_probability=None, unique=False)
 
     """  # noqa: W505
 
@@ -199,29 +200,31 @@
         MAX_COLS).
     unique : bool, optional
         indicate if the values generated for these columns should be unique
         (per-column).
 
     Examples
     --------
-    >>> from polars.testing.parametric import columns
+    >>> from polars.testing.parametric import columns, dataframes
+    >>> from hypothesis import given
+    >>>
+    >>> @given(dataframes(columns(["x", "y", "z"], unique=True)))
+    ... def test_unique_xyz(df: pl.DataFrame) -> None:
+    ...     assert_something(df)
+
+    Note, as 'columns' creates a list of native polars column definitions it can
+    also be used independently of parametric/hypothesis tests:
+
     >>> from string import punctuation
     >>>
     >>> def test_special_char_colname_init() -> None:
-    ...     schema = [(c.name, c.dtype) for c in columns(punctuation)]
-    ...     df = pl.DataFrame(schema=schema)
+    ...     df = pl.DataFrame(schema=[(c.name, c.dtype) for c in columns(punctuation)])
     ...     assert len(cols) == len(df.columns)
     ...     assert 0 == len(df.rows())
     ...
-    >>> from polars.testing.parametric import columns
-    >>> from hypothesis import given
-    >>>
-    >>> @given(dataframes(columns(["x", "y", "z"], unique=True)))
-    ... def test_unique_xyz(df: pl.DataFrame) -> None:
-    ...     assert_something(df)
 
     """
     # create/assign named columns
     if cols is None:
         cols = random.randint(
             a=min_cols or 0,
             b=max_cols or MAX_COLS,
@@ -259,15 +262,15 @@
     allow_infinities: bool = True,
     unique: bool = False,
     chunked: bool | None = None,
     allowed_dtypes: Collection[PolarsDataType] | PolarsDataType | None = None,
     excluded_dtypes: Collection[PolarsDataType] | PolarsDataType | None = None,
 ) -> SearchStrategy[Series]:
     """
-    Hypothesis strategy for producing a polars Series.
+    Hypothesis strategy for producing polars Series.
 
     Parameters
     ----------
     name : {str, strategy}, optional
         literal string or a strategy for strings (or None), passed to the Series
         constructor name-param.
     dtype : PolarsDataType, optional
@@ -307,28 +310,40 @@
     `.example()` directly on a given strategy to see concrete instances of the
     generated data.
 
     Examples
     --------
     >>> from polars.testing.parametric import series
     >>> from hypothesis import given
-    >>>
-    >>> @given(df=series())
-    ... def test_repr(s: pl.Series) -> None:
+
+    In normal usage, as a simple unit test:
+
+    >>> @given(s=series(null_probability=0.1))
+    ... def test_repr_is_valid_string(s: pl.Series) -> None:
     ...     assert isinstance(repr(s), str)
-    >>>
-    >>> s = series(dtype=pl.Int32, max_size=5)
+
+    Experimenting locally with a custom List dtype strategy:
+
+    >>> from polars.testing.parametric import create_list_strategy
+    >>> s = series(
+    ...     strategy=create_list_strategy(
+    ...         inner_dtype=pl.Utf8,
+    ...         select_from=["xx", "yy", "zz"],
+    ...     ),
+    ...     min_size=2,
+    ...     max_size=4,
+    ... )
     >>> s.example()  # doctest: +SKIP
     shape: (4,)
-    Series: '' [i64]
+    Series: '' [list[str]]
     [
-        54666
-        -35
-        6414
-        -63290
+        []
+        ["yy", "yy", "zz"]
+        ["zz", "yy", "zz"]
+        ["xx"]
     ]
 
     """
     if isinstance(allowed_dtypes, (DataType, DataTypeClass)):
         allowed_dtypes = [allowed_dtypes]
     if isinstance(excluded_dtypes, (DataType, DataTypeClass)):
         excluded_dtypes = [excluded_dtypes]
@@ -435,15 +450,15 @@
     include_cols: Sequence[column] | None = None,
     null_probability: float | dict[str, float] = 0.0,
     allow_infinities: bool = True,
     allowed_dtypes: Collection[PolarsDataType] | PolarsDataType | None = None,
     excluded_dtypes: Collection[PolarsDataType] | PolarsDataType | None = None,
 ) -> SearchStrategy[DataFrame | LazyFrame]:
     """
-    Hypothesis strategy for producing a polars DataFrame or LazyFrame.
+    Hypothesis strategy for producing polars DataFrames or LazyFrames.
 
     Parameters
     ----------
     cols : {int, columns}, optional
         integer number of columns to create, or a sequence of `column` objects
         that describe the desired DataFrame column data.
     lazy : bool, optional
@@ -494,47 +509,63 @@
     --------
     Use `column` or `columns` to specify the schema of the types of DataFrame to
     generate. Note: in actual use the strategy is applied as a test decorator, not
     used standalone.
 
     >>> from polars.testing.parametric import column, columns, dataframes
     >>> from hypothesis import given
-    >>>
-    >>> # generate arbitrary DataFrames
+
+    Generate arbitrary DataFrames (as part of a unit test):
+
     >>> @given(df=dataframes())
     ... def test_repr(df: pl.DataFrame) -> None:
     ...     assert isinstance(repr(df), str)
-    >>>
-    >>> # generate LazyFrames with at least 1 column, random dtypes, and specific size:
-    >>> df = dataframes(min_cols=1, lazy=True, max_size=5)
-    >>> df.example()  # doctest: +SKIP
-    >>>
-    >>> # generate DataFrames with known colnames, random dtypes (per test, not per-frame):
-    >>> df_strategy = dataframes(columns(["x", "y", "z"]))
-    >>> df.example()  # doctest: +SKIP
-    >>>
-    >>> # generate frames with explicitly named/typed columns and a fixed size:
-    >>> df_strategy = dataframes(
+
+    Generate LazyFrames with at least 1 column, random dtypes, and specific size:
+
+    >>> dfs = dataframes(min_cols=1, max_size=5, lazy=True)
+    >>> dfs.example()  # doctest: +SKIP
+    <polars.LazyFrame object at 0x11F561580>
+
+    Generate DataFrames with known colnames, random dtypes (per test, not per-frame):
+
+    >>> dfs = dataframes(columns(["x", "y", "z"]))
+    >>> dfs.example()  # doctest: +SKIP
+    shape: (3, 3)
+    ┌────────────┬───────┬────────────────────────────┐
+    │ x          ┆ y     ┆ z                          │
+    │ ---        ┆ ---   ┆ ---                        │
+    │ date       ┆ u16   ┆ datetime[μs]               │
+    ╞════════════╪═══════╪════════════════════════════╡
+    │ 0565-08-12 ┆ 34715 ┆ 5844-09-20 00:33:31.076854 │
+    │ 3382-10-17 ┆ 48662 ┆ 7540-01-29 11:20:14.836271 │
+    │ 4063-06-17 ┆ 39092 ┆ 1889-05-05 13:25:41.874455 │
+    └────────────┴───────┴────────────────────────────┘
+
+    Generate frames with explicitly named/typed columns and a fixed size:
+
+    >>> dfs = dataframes(
     ...     [
     ...         column("x", dtype=pl.Int32),
     ...         column("y", dtype=pl.Float64),
     ...     ],
     ...     size=2,
     ... )
-    >>> df_strategy.example()  # doctest: +SKIP
+    >>> dfs.example()  # doctest: +SKIP
     shape: (2, 2)
     ┌───────────┬────────────┐
     │ x         ┆ y          │
     │ ---       ┆ ---        │
     │ i32       ┆ f64        │
     ╞═══════════╪════════════╡
     │ -15836    ┆ 1.1755e-38 │
     │ 575050513 ┆ NaN        │
     └───────────┴────────────┘
-    """  # noqa: 501
+
+    """
     _failed_frame_init_msgs_.clear()
 
     if isinstance(min_size, int) and min_cols in (0, None):
         min_cols = 1
     if isinstance(allowed_dtypes, (DataType, DataTypeClass)):
         allowed_dtypes = [allowed_dtypes]
     if isinstance(excluded_dtypes, (DataType, DataTypeClass)):
```

### Comparing `polars_u64_idx-0.17.8/polars/testing/parametric/profiles.py` & `polars_u64_idx-0.17.9/polars/testing/parametric/profiles.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/polars/testing/parametric/strategies.py` & `polars_u64_idx-0.17.9/polars/testing/parametric/strategies.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/polars/type_aliases.py` & `polars_u64_idx-0.17.9/polars/type_aliases.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/polars/utils/__init__.py` & `polars_u64_idx-0.17.9/polars/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/polars/utils/_construction.py` & `polars_u64_idx-0.17.9/polars/utils/_construction.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/polars/utils/_parse_expr_input.py` & `polars_u64_idx-0.17.9/polars/utils/_parse_expr_input.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/polars/utils/_scan.py` & `polars_u64_idx-0.17.9/polars/utils/_scan.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/polars/utils/_wrap.py` & `polars_u64_idx-0.17.9/polars/utils/_wrap.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/polars/utils/build_info.py` & `polars_u64_idx-0.17.9/polars/utils/build_info.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/polars/utils/convert.py` & `polars_u64_idx-0.17.9/polars/utils/convert.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/polars/utils/decorators.py` & `polars_u64_idx-0.17.9/polars/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/polars/utils/meta.py` & `polars_u64_idx-0.17.9/polars/utils/meta.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/polars/utils/polars_version.py` & `polars_u64_idx-0.17.9/polars/utils/polars_version.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/polars/utils/show_versions.py` & `polars_u64_idx-0.17.9/polars/utils/show_versions.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/polars/utils/various.py` & `polars_u64_idx-0.17.9/polars/utils/various.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/pyproject.toml` & `polars_u64_idx-0.17.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/requirements-dev.txt` & `polars_u64_idx-0.17.9/requirements-dev.txt`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/scripts/check_stacklevels.py` & `polars_u64_idx-0.17.9/scripts/check_stacklevels.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/src/apply/dataframe.rs` & `polars_u64_idx-0.17.9/src/apply/dataframe.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/src/apply/mod.rs` & `polars_u64_idx-0.17.9/src/apply/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/src/apply/series.rs` & `polars_u64_idx-0.17.9/src/apply/series.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/src/arrow_interop/to_py.rs` & `polars_u64_idx-0.17.9/src/arrow_interop/to_py.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/src/arrow_interop/to_rust.rs` & `polars_u64_idx-0.17.9/src/arrow_interop/to_rust.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/src/batched_csv.rs` & `polars_u64_idx-0.17.9/src/batched_csv.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/src/conversion.rs` & `polars_u64_idx-0.17.9/src/conversion.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/src/dataframe.rs` & `polars_u64_idx-0.17.9/src/dataframe.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/src/datatypes.rs` & `polars_u64_idx-0.17.9/src/datatypes.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/src/error.rs` & `polars_u64_idx-0.17.9/src/error.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/src/file.rs` & `polars_u64_idx-0.17.9/src/file.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/src/lazy/apply.rs` & `polars_u64_idx-0.17.9/src/lazy/apply.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/src/lazy/dataframe.rs` & `polars_u64_idx-0.17.9/src/lazy/dataframe.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/src/lazy/dsl.rs` & `polars_u64_idx-0.17.9/src/lazy/dsl.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/src/lazy/meta.rs` & `polars_u64_idx-0.17.9/src/lazy/meta.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/src/lazy/mod.rs` & `polars_u64_idx-0.17.9/src/lazy/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/src/lib.rs` & `polars_u64_idx-0.17.9/src/lib.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/src/npy.rs` & `polars_u64_idx-0.17.9/src/npy.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/src/object.rs` & `polars_u64_idx-0.17.9/src/object.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/src/series.rs` & `polars_u64_idx-0.17.9/src/series.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/src/set.rs` & `polars_u64_idx-0.17.9/src/set.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/src/sql.rs` & `polars_u64_idx-0.17.9/src/sql.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/src/utils.rs` & `polars_u64_idx-0.17.9/src/utils.rs`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/tests/README.md` & `polars_u64_idx-0.17.9/tests/README.md`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/tests/benchmark/groupby-datagen.R` & `polars_u64_idx-0.17.9/tests/benchmark/groupby-datagen.R`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/tests/benchmark/run_h2oai_benchmark.py` & `polars_u64_idx-0.17.9/tests/benchmark/run_h2oai_benchmark.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/tests/benchmark/test_release.py` & `polars_u64_idx-0.17.9/tests/benchmark/test_release.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/tests/docs/run_doctest.py` & `polars_u64_idx-0.17.9/tests/docs/run_doctest.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/tests/parametric/test_dataframe.py` & `polars_u64_idx-0.17.9/tests/parametric/test_dataframe.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/tests/parametric/test_lazyframe.py` & `polars_u64_idx-0.17.9/tests/parametric/test_lazyframe.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/tests/parametric/test_series.py` & `polars_u64_idx-0.17.9/tests/parametric/test_series.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/tests/parametric/test_testing.py` & `polars_u64_idx-0.17.9/tests/parametric/test_testing.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/tests/unit/conftest.py` & `polars_u64_idx-0.17.9/tests/unit/conftest.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/tests/unit/datatypes/test_bool.py` & `polars_u64_idx-0.17.9/tests/unit/datatypes/test_bool.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/tests/unit/datatypes/test_categorical.py` & `polars_u64_idx-0.17.9/tests/unit/datatypes/test_categorical.py`

 * *Files 0% similar despite different names*

```diff
@@ -309,15 +309,15 @@
             pl.Series("x", [1, 2, 3, 4] * 2, dtype=pl.Int32),
         ]
     )
     with pytest.raises(
         pl.ComputeError,
         match=r"joins/or comparisons on categoricals can only happen if they were created under the same global string cache",
     ):
-        df1.join_asof(df2, on="time", by="cat")
+        df1.join_asof(df2, on=pl.col("time").set_sorted(), by="cat")
 
 
 def test_categorical_list_get_item() -> None:
     out = pl.Series([["a"]]).cast(pl.List(pl.Categorical)).item()
     assert isinstance(out, pl.Series)
     assert out.dtype == pl.Categorical
```

### Comparing `polars_u64_idx-0.17.8/tests/unit/datatypes/test_decimal.py` & `polars_u64_idx-0.17.9/tests/unit/datatypes/test_decimal.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/tests/unit/datatypes/test_list.py` & `polars_u64_idx-0.17.9/tests/unit/datatypes/test_list.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/tests/unit/datatypes/test_object.py` & `polars_u64_idx-0.17.9/tests/unit/datatypes/test_object.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/tests/unit/datatypes/test_struct.py` & `polars_u64_idx-0.17.9/tests/unit/datatypes/test_struct.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/tests/unit/datatypes/test_temporal.py` & `polars_u64_idx-0.17.9/tests/unit/datatypes/test_temporal.py`

 * *Files 1% similar despite different names*

```diff
@@ -680,15 +680,15 @@
             "event_date": [
                 datetime(2021, 4, 11, tzinfo=tzinfo),
                 datetime(2021, 4, 29, tzinfo=tzinfo),
                 datetime(2021, 5, 29, tzinfo=tzinfo),
             ],
             "adm1_code": [1, 2, 1],
         }
-    )
+    ).set_sorted("event_date")
     out = df.groupby_dynamic(
         index_column="event_date",
         every="1mo",
         period="2mo",
         offset="-1mo",
         include_boundaries=True,
     ).agg(
@@ -711,35 +711,39 @@
             ],
             "adm1_code": [1, 2, 1],
             "five_type": ["a", "b", "a"],
             "actor": ["a", "a", "a"],
             "admin": ["a", "a", "a"],
             "fatalities": [10, 20, 30],
         }
-    )
+    ).set_sorted("event_date")
 
     out = df.groupby_dynamic(
         index_column="event_date",
         every="1mo",
         by=["admin", "five_type", "actor"],
     ).agg([pl.col("adm1_code").unique(), (pl.col("fatalities") > 0).sum()])
 
     assert out["event_date"].to_list() == [
         datetime(2021, 4, 1, tzinfo=tzinfo),
         datetime(2021, 5, 1, tzinfo=tzinfo),
         datetime(2021, 4, 1, tzinfo=tzinfo),
     ]
 
     for dt in [pl.Int32, pl.Int64]:
-        df = pl.DataFrame(
-            {
-                "idx": np.arange(6),
-                "A": ["A", "A", "B", "B", "B", "C"],
-            }
-        ).with_columns(pl.col("idx").cast(dt))
+        df = (
+            pl.DataFrame(
+                {
+                    "idx": np.arange(6),
+                    "A": ["A", "A", "B", "B", "B", "C"],
+                }
+            )
+            .with_columns(pl.col("idx").cast(dt))
+            .set_sorted("idx")
+        )
 
         out = df.groupby_dynamic(
             "idx", every="2i", period="3i", include_boundaries=True
         ).agg(pl.col("A"))
 
         assert out.shape == (3, 4)
         assert out["A"].to_list() == [["A", "A", "B"], ["B", "B", "B"], ["B", "C"]]
@@ -793,18 +797,23 @@
         pl.DataFrame(
             data={
                 "timestamp": ["1970-01-01 00:00:00+01:00", "1970-01-01 01:00:00+01:00"],
                 "value": [1, 1],
             }
         )
         .with_columns(
-            pl.col("timestamp").str.strptime(pl.Datetime, format="%Y-%m-%d %H:%M:%S%:z")
+            pl.col("timestamp")
+            .str.strptime(pl.Datetime, format="%Y-%m-%d %H:%M:%S%:z")
+            .set_sorted()
         )
         .with_columns(
-            pl.col("timestamp").dt.convert_time_zone("UTC").alias("timestamp_utc")
+            pl.col("timestamp")
+            .dt.convert_time_zone("UTC")
+            .alias("timestamp_utc")
+            .set_sorted()
         )
     )
     result = df.groupby_dynamic(
         index_column="timestamp", every="1d", closed="left"
     ).agg(pl.col("value").count())
     expected = pl.DataFrame({"timestamp": [datetime(1970, 1, 1)], "value": [2]})
     expected = expected.with_columns(
@@ -834,16 +843,18 @@
         "2020-01-01 16:42:13",
         "2020-01-01 16:45:09",
         "2020-01-02 18:12:48",
         "2020-01-03 19:45:32",
         "2020-01-08 23:16:43",
     ]
 
-    df = pl.DataFrame({"dt": dates, "a": [3, 7, 5, 9, 2, 1]}).with_columns(
-        pl.col("dt").str.strptime(pl.Datetime)
+    df = (
+        pl.DataFrame({"dt": dates, "a": [3, 7, 5, 9, 2, 1]})
+        .with_columns(pl.col("dt").str.strptime(pl.Datetime))
+        .set_sorted("dt")
     )
 
     period: str | timedelta
     for period in ("2d", timedelta(days=2)):  # type: ignore[assignment]
         out = df.groupby_rolling(index_column="dt", period=period).agg(
             [
                 pl.sum("a").alias("sum_a"),
@@ -872,15 +883,15 @@
                 datetime(2021, 4, 1),
                 datetime(2021, 5, 1),
                 datetime(2021, 6, 1),
             ],
             "admin": ["Åland", "Netherlands", "Åland", "Netherlands"],
             "test2": [0, 1, 2, 3],
         }
-    ).with_columns(pl.col("time").dt.replace_time_zone(time_zone))
+    ).with_columns(pl.col("time").dt.replace_time_zone(time_zone).set_sorted())
 
     up = df.upsample(
         time_column="time", every="1mo", by="admin", maintain_order=True
     ).select(pl.all().forward_fill())
     # this print will panic if timezones feature is not activated
     # don't remove
     print(up)
@@ -1027,15 +1038,15 @@
     # 2791
     dts = [
         datetime(2020, 1, 1, tzinfo=tzinfo),
         datetime(2020, 1, 2, tzinfo=tzinfo),
         datetime(2020, 2, 1, tzinfo=tzinfo),
         datetime(2020, 3, 1, tzinfo=tzinfo),
     ]
-    df = pl.DataFrame({"dt": dts, "idx": range(len(dts))})
+    df = pl.DataFrame({"dt": dts, "idx": range(len(dts))}).set_sorted("dt")
     out = df.groupby_dynamic(index_column="dt", every="1mo", closed="right").agg(
         pl.col("idx")
     )
 
     expected = pl.DataFrame(
         {
             "dt": [
@@ -1111,15 +1122,15 @@
         {
             "date": [date(2020, 1, 5), date(2020, 1, 6)],
             "by": [1, 1],
             "values": [100, 200],
         }
     )
 
-    out = df1.join_asof(df2, by="by", on="date", tolerance="3d")
+    out = df1.join_asof(df2, by="by", on=pl.col("date").set_sorted(), tolerance="3d")
 
     expected = pl.DataFrame(
         {
             "date": [date(2020, 1, 5), date(2020, 1, 10)],
             "by": [1, 1],
             "values": [100, None],
         }
@@ -1272,15 +1283,15 @@
                 "1998-05-03",
                 "1998-05-10",
                 "1998-05-17",
                 "1998-05-24",
             ],
             "val": range(7),
         }
-    ).with_columns(pl.col("Date").str.strptime(pl.Date))
+    ).with_columns(pl.col("Date").str.strptime(pl.Date).set_sorted())
 
     period: str | timedelta
     for period in ("1w", timedelta(days=7)):  # type: ignore[assignment]
         result = df.groupby_rolling(index_column="Date", period=period).agg(
             pl.col("val").mean().alias("val_mean")
         )
         expected = pl.DataFrame(
@@ -1324,15 +1335,15 @@
     ]
     quotes = pl.DataFrame(
         {
             "dates": pl.Series(dates).str.strptime(pl.Datetime, format=format),
             "ticker": ticker,
             "bid": [720.5, 51.95, 51.97, 51.99, 720.50, 97.99, 720.50, 52.01],
         }
-    )
+    ).set_sorted("dates")
     dates = [
         "2016-05-25 13:30:00.023",
         "2016-05-25 13:30:00.038",
         "2016-05-25 13:30:00.048",
         "2016-05-25 13:30:00.048",
         "2016-05-25 13:30:00.048",
     ]
@@ -1345,15 +1356,15 @@
     ]
     trades = pl.DataFrame(
         {
             "dates": pl.Series(dates).str.strptime(pl.Datetime, format=format),
             "ticker": ticker,
             "bid": [51.95, 51.95, 720.77, 720.92, 98.0],
         }
-    )
+    ).set_sorted("dates")
     assert trades.schema == {
         "dates": pl.Datetime("ms"),
         "ticker": pl.Utf8,
         "bid": pl.Float64,
     }
     out = trades.join_asof(quotes, on="dates", strategy="backward")
 
@@ -1666,15 +1677,15 @@
                 datetime(2022, 1, 1, 0, 5),
                 datetime(2022, 1, 1, 0, 6),
                 datetime(2022, 1, 1, 0, 7),
             ],
             "key": ["A", "A", "B", "B", "A", "B", "A"],
             "val": [1, 1, 1, 1, 1, 1, 1],
         }
-    )
+    ).set_sorted("dt")
 
     assert df.groupby_rolling(
         index_column="dt",
         period="2m",
         closed="both",
         offset="-1m",
         by="key",
@@ -2438,17 +2449,17 @@
         ],
     }
 
 
 def test_asof_join_by_forward() -> None:
     dfa = pl.DataFrame(
         {"category": ["a", "a", "a", "a", "a"], "value_one": [1, 2, 3, 5, 12]}
-    )
+    ).set_sorted("value_one")
 
-    dfb = pl.DataFrame({"category": ["a"], "value_two": [3]})
+    dfb = pl.DataFrame({"category": ["a"], "value_two": [3]}).set_sorted("value_two")
 
     assert dfa.join_asof(
         dfb,
         left_on="value_one",
         right_on="value_two",
         by="category",
         strategy="forward",
@@ -2653,21 +2664,25 @@
             datetime(2023, 1, 3, 0, 0),
             datetime(2023, 1, 4, 0, 0),
         ],
     }
 
 
 def test_rolling_groupby_empty_groups_by_take_6330() -> None:
-    df = pl.DataFrame({"Event": ["Rain", "Sun"]}).join(
-        pl.DataFrame(
-            {
-                "Date": [1, 2, 3, 4],
-            }
-        ),
-        how="cross",
+    df = (
+        pl.DataFrame({"Event": ["Rain", "Sun"]})
+        .join(
+            pl.DataFrame(
+                {
+                    "Date": [1, 2, 3, 4],
+                }
+            ),
+            how="cross",
+        )
+        .set_sorted("Date")
     )
     assert (
         df.groupby_rolling(
             index_column="Date",
             period="2i",
             offset="-2i",
             by="Event",
```

### Comparing `polars_u64_idx-0.17.8/tests/unit/io/files/delta-table/_delta_log/00000000000000000000.json` & `polars_u64_idx-0.17.9/tests/unit/io/files/delta-table/_delta_log/00000000000000000000.json`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/tests/unit/io/files/delta-table/_delta_log/00000000000000000001.json` & `polars_u64_idx-0.17.9/tests/unit/io/files/delta-table/_delta_log/00000000000000000001.json`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/tests/unit/io/files/delta-table/part-00000-e42312d7-60e5-454d-acbc-db192d220e73-c000.snappy.parquet` & `polars_u64_idx-0.17.9/tests/unit/io/files/delta-table/part-00000-e42312d7-60e5-454d-acbc-db192d220e73-c000.snappy.parquet`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/tests/unit/io/files/delta-table/part-00000-e4a999da-df45-4fb0-bdc4-d999fc0f58aa-c000.snappy.parquet` & `polars_u64_idx-0.17.9/tests/unit/io/files/delta-table/part-00000-e4a999da-df45-4fb0-bdc4-d999fc0f58aa-c000.snappy.parquet`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/tests/unit/io/files/example.xlsx` & `polars_u64_idx-0.17.9/tests/unit/io/files/example.xlsx`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/tests/unit/io/files/foods1.ipc` & `polars_u64_idx-0.17.9/tests/unit/io/files/foods1.ipc`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/tests/unit/io/files/foods1.ndjson` & `polars_u64_idx-0.17.9/tests/unit/io/files/foods1.ndjson`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/tests/unit/io/files/foods1.parquet` & `polars_u64_idx-0.17.9/tests/unit/io/files/foods1.parquet`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/tests/unit/io/files/foods2.ipc` & `polars_u64_idx-0.17.9/tests/unit/io/files/foods2.ipc`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/tests/unit/io/files/foods2.ndjson` & `polars_u64_idx-0.17.9/tests/unit/io/files/foods2.ndjson`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/tests/unit/io/files/foods2.parquet` & `polars_u64_idx-0.17.9/tests/unit/io/files/foods2.parquet`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/tests/unit/io/files/small.parquet` & `polars_u64_idx-0.17.9/tests/unit/io/files/small.parquet`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/tests/unit/io/test_avro.py` & `polars_u64_idx-0.17.9/tests/unit/io/test_avro.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/tests/unit/io/test_csv.py` & `polars_u64_idx-0.17.9/tests/unit/io/test_csv.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/tests/unit/io/test_database.py` & `polars_u64_idx-0.17.9/tests/unit/io/test_database.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/tests/unit/io/test_delta.py` & `polars_u64_idx-0.17.9/tests/unit/io/test_delta.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/tests/unit/io/test_excel.py` & `polars_u64_idx-0.17.9/tests/unit/io/test_excel.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/tests/unit/io/test_ipc.py` & `polars_u64_idx-0.17.9/tests/unit/io/test_ipc.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/tests/unit/io/test_json.py` & `polars_u64_idx-0.17.9/tests/unit/io/test_json.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/tests/unit/io/test_lazy_csv.py` & `polars_u64_idx-0.17.9/tests/unit/io/test_lazy_csv.py`

 * *Files 3% similar despite different names*

```diff
@@ -212,7 +212,20 @@
     # take first and last rows
     assert df[[0, 39]].to_dict(False) == {
         "category": ["vegetables", "seafood"],
         "calories": [45, 146],
         "fats_g": [0.5, 6.0],
         "sugars_g": [2, 2],
     }
+
+
+def test_scan_csv_schema_overwrite_not_projected_8483(foods_file_path: str) -> None:
+    df = (
+        pl.scan_csv(
+            foods_file_path,
+            dtypes={"calories": pl.Utf8, "sugars_g": pl.Int8},
+        )
+        .select(pl.count())
+        .collect()
+    )
+    expected = pl.DataFrame({"count": 27}, schema={"count": pl.UInt32})
+    assert_frame_equal(df, expected)
```

### Comparing `polars_u64_idx-0.17.8/tests/unit/io/test_lazy_ipc.py` & `polars_u64_idx-0.17.9/tests/unit/io/test_lazy_ipc.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/tests/unit/io/test_lazy_json.py` & `polars_u64_idx-0.17.9/tests/unit/io/test_lazy_json.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/tests/unit/io/test_lazy_parquet.py` & `polars_u64_idx-0.17.9/tests/unit/io/test_lazy_parquet.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/tests/unit/io/test_other.py` & `polars_u64_idx-0.17.9/tests/unit/io/test_other.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/tests/unit/io/test_parquet.py` & `polars_u64_idx-0.17.9/tests/unit/io/test_parquet.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/tests/unit/io/test_pickle.py` & `polars_u64_idx-0.17.9/tests/unit/io/test_pickle.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/tests/unit/io/test_pyarrow_dataset.py` & `polars_u64_idx-0.17.9/tests/unit/io/test_pyarrow_dataset.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/tests/unit/namespaces/test_binary.py` & `polars_u64_idx-0.17.9/tests/unit/namespaces/test_binary.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/tests/unit/namespaces/test_categorical.py` & `polars_u64_idx-0.17.9/tests/unit/namespaces/test_categorical.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/tests/unit/namespaces/test_datetime.py` & `polars_u64_idx-0.17.9/tests/unit/namespaces/test_datetime.py`

 * *Files 1% similar despite different names*

```diff
@@ -527,17 +527,26 @@
 def test_negative_offset_by_err_msg_8464() -> None:
     with pytest.raises(
         ComputeError, match=r"cannot advance '2022-03-30 00:00:00' by -1 month\(s\)"
     ):
         pl.Series([datetime(2022, 3, 30)]).dt.offset_by("-1mo")
 
 
-def test_offset_by_saturating_8217() -> None:
-    result = pl.Series([date(2018, 1, 31)]).dt.offset_by("1mo_saturating").item()
-    expected = date(2018, 2, 28)
+@pytest.mark.parametrize(
+    ("duration", "input_date", "expected"),
+    [
+        ("1mo_saturating", date(2018, 1, 31), date(2018, 2, 28)),
+        ("1y_saturating", date(2024, 2, 29), date(2025, 2, 28)),
+        ("1y1mo_saturating", date(2024, 1, 30), date(2025, 2, 28)),
+    ],
+)
+def test_offset_by_saturating_8217_8474(
+    duration: str, input_date: date, expected: date
+) -> None:
+    result = pl.Series([input_date]).dt.offset_by(duration).item()
     assert result == expected
 
 
 def test_year_empty_df() -> None:
     df = pl.DataFrame(pl.Series(name="date", dtype=pl.Date))
     assert df.select(pl.col("date").dt.year()).dtypes == [pl.Int32]
```

### Comparing `polars_u64_idx-0.17.8/tests/unit/namespaces/test_list.py` & `polars_u64_idx-0.17.9/tests/unit/namespaces/test_list.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/tests/unit/namespaces/test_meta.py` & `polars_u64_idx-0.17.9/tests/unit/namespaces/test_meta.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/tests/unit/namespaces/test_string.py` & `polars_u64_idx-0.17.9/tests/unit/namespaces/test_string.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/tests/unit/namespaces/test_strptime.py` & `polars_u64_idx-0.17.9/tests/unit/namespaces/test_strptime.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/tests/unit/namespaces/test_struct.py` & `polars_u64_idx-0.17.9/tests/unit/namespaces/test_struct.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/tests/unit/operations/test_aggregations.py` & `polars_u64_idx-0.17.9/tests/unit/operations/test_aggregations.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/tests/unit/operations/test_apply.py` & `polars_u64_idx-0.17.9/tests/unit/operations/test_apply.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/tests/unit/operations/test_arithmetic.py` & `polars_u64_idx-0.17.9/tests/unit/operations/test_arithmetic.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/tests/unit/operations/test_comparison.py` & `polars_u64_idx-0.17.9/tests/unit/operations/test_comparison.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/tests/unit/operations/test_drop.py` & `polars_u64_idx-0.17.9/tests/unit/operations/test_drop.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/tests/unit/operations/test_explode.py` & `polars_u64_idx-0.17.9/tests/unit/operations/test_explode.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/tests/unit/operations/test_filter.py` & `polars_u64_idx-0.17.9/tests/unit/operations/test_filter.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/tests/unit/operations/test_folds.py` & `polars_u64_idx-0.17.9/tests/unit/operations/test_folds.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/tests/unit/operations/test_groupby.py` & `polars_u64_idx-0.17.9/tests/unit/operations/test_groupby.py`

 * *Files 1% similar despite different names*

```diff
@@ -196,15 +196,17 @@
         if lazy:
             result = result.collect()  # type: ignore[union-attr]
         assert_frame_equal(result, expected)
 
 
 @pytest.mark.parametrize("lazy", [True, False])
 def test_groupby_rolling_agg_input_types(lazy: bool) -> None:
-    df = pl.DataFrame({"index_column": [0, 1, 2, 3], "b": [1, 3, 1, 2]})
+    df = pl.DataFrame({"index_column": [0, 1, 2, 3], "b": [1, 3, 1, 2]}).set_sorted(
+        "index_column"
+    )
     df_or_lazy: pl.DataFrame | pl.LazyFrame = df.lazy() if lazy else df
 
     for bad_param in bad_agg_parameters():
         with pytest.raises(TypeError):  # noqa: PT012
             result = df_or_lazy.groupby_rolling(
                 index_column="index_column", period="2i"
             ).agg(bad_param)
@@ -220,15 +222,17 @@
         if lazy:
             result = result.collect()  # type: ignore[union-attr]
         assert_frame_equal(result, expected)
 
 
 @pytest.mark.parametrize("lazy", [True, False])
 def test_groupby_dynamic_agg_input_types(lazy: bool) -> None:
-    df = pl.DataFrame({"index_column": [0, 1, 2, 3], "b": [1, 3, 1, 2]})
+    df = pl.DataFrame({"index_column": [0, 1, 2, 3], "b": [1, 3, 1, 2]}).set_sorted(
+        "index_column"
+    )
     df_or_lazy: pl.DataFrame | pl.LazyFrame = df.lazy() if lazy else df
 
     for bad_param in bad_agg_parameters():
         with pytest.raises(TypeError):  # noqa: PT012
             result = df_or_lazy.groupby_dynamic(
                 index_column="index_column", every="2i", closed="right"
             ).agg(bad_param)
@@ -420,15 +424,15 @@
     assert df.unique(keep="first", subset="a", maintain_order=True).to_dict(False) == {
         "row_nr": [0, 1],
         "a": [1, 2],
     }
 
 
 def test_groupby_dynamic_flat_agg_4814() -> None:
-    df = pl.DataFrame({"a": [1, 2, 2], "b": [1, 8, 12]})
+    df = pl.DataFrame({"a": [1, 2, 2], "b": [1, 8, 12]}).set_sorted("a")
 
     assert df.groupby_dynamic("a", every="1i", period="2i").agg(
         [
             (pl.col("b").sum() / pl.col("a").sum()).alias("sum_ratio_1"),
             (pl.col("b").last() / pl.col("a").last()).alias("last_ratio_1"),
             (pl.col("b") / pl.col("a")).last().alias("last_ratio_2"),
         ]
@@ -458,14 +462,15 @@
                     datetime(2021, 1, 1, tzinfo=tzinfo) + timedelta(seconds=2**i)
                     for i in range(10)
                 ],
                 "b": [float(i) for i in range(10)],
             }
         )
         .lazy()
+        .set_sorted("a")
         .groupby_dynamic("a", every=every, period=period)
         .agg([pl.col("b").var().sqrt().alias("corr")])
     ).collect().sum().to_dict(False) == pytest.approx(
         {"a": [None], "corr": [6.988674024215477]}
     )
 
 
@@ -554,15 +559,15 @@
                 datetime(2020, 1, 1, 10, 0, tzinfo=tzinfo),
                 datetime(2020, 1, 1, 10, 50, tzinfo=tzinfo),
                 datetime(2020, 1, 1, 11, 10, tzinfo=tzinfo),
             ],
             "a": [1, 2, 2],
             "b": [4, 5, 6],
         }
-    )
+    ).set_sorted("datetime")
 
     # Without 'by' argument
     result1 = [
         (name, data.shape)
         for name, data in df.groupby_dynamic("datetime", every=every, closed="left")
     ]
     expected1 = [
@@ -653,14 +658,15 @@
                     datetime(2021, 1, 1, tzinfo=tzinfo) + timedelta(seconds=2**i)
                     for i in range(5)
                 ],
                 "b": [float(i) for i in range(5)],
             }
         )
         .lazy()
+        .set_sorted("a")
         .groupby_dynamic("a", every="10s", period="100s")
         .agg([pl.col("b").mean().sin().alias("c")])
         .collect()
     )
     assert_frame_equal(
         df,
         pl.DataFrame(
```

### Comparing `polars_u64_idx-0.17.8/tests/unit/operations/test_is_in.py` & `polars_u64_idx-0.17.9/tests/unit/operations/test_is_in.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/tests/unit/operations/test_join.py` & `polars_u64_idx-0.17.9/tests/unit/operations/test_join.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/tests/unit/operations/test_join_asof.py` & `polars_u64_idx-0.17.9/tests/unit/operations/test_join_asof.py`

 * *Files 18% similar despite different names*

```diff
@@ -30,15 +30,15 @@
             ],
             "stock": ["A", "B", "C", "A"],
             "quote": [100, 300, 501, 102],
         }
     ).with_columns([pl.col("time").dt.cast_time_unit("ns")])
 
     assert df_trades.join_asof(
-        df_quotes, on=pl.col("time").cast(pl.Datetime("ns")), by="stock"
+        df_quotes, on=pl.col("time").cast(pl.Datetime("ns")).set_sorted(), by="stock"
     ).to_dict(False) == {
         "time": [
             datetime(2020, 1, 1, 9, 1),
             datetime(2020, 1, 1, 9, 1),
             datetime(2020, 1, 1, 9, 3),
             datetime(2020, 1, 1, 9, 6),
         ],
@@ -47,15 +47,15 @@
         "quote": [100, None, 300, 501],
     }
 
 
 def test_asof_join_projection_resolution_4606() -> None:
     a = pl.DataFrame({"a": [1], "b": [2], "c": [3]}).lazy()
     b = pl.DataFrame({"a": [1], "b": [2], "d": [4]}).lazy()
-    joined_tbl = a.join_asof(b, on="a", by="b")
+    joined_tbl = a.join_asof(b, on=pl.col("a").set_sorted(), by="b")
     assert joined_tbl.groupby("a").agg(
         [pl.col("c").sum().alias("c")]
     ).collect().columns == ["a", "c"]
 
 
 def test_asof_join_schema_5211() -> None:
     df1 = pl.DataFrame({"today": [1, 2]})
@@ -68,28 +68,36 @@
             df2.lazy(), left_on="today", right_on="next_friday", strategy="forward"
         )
         .schema
     ) == {"today": pl.Int64, "next_friday": pl.Int64}
 
 
 def test_asof_join_schema_5684() -> None:
-    df_a = pl.DataFrame(
-        {
-            "id": [1],
-            "a": [1],
-            "b": [1],
-        }
-    ).lazy()
+    df_a = (
+        pl.DataFrame(
+            {
+                "id": [1],
+                "a": [1],
+                "b": [1],
+            }
+        )
+        .lazy()
+        .set_sorted("a")
+    )
 
-    df_b = pl.DataFrame(
-        {
-            "id": [1, 1, 2],
-            "b": [3, -3, 6],
-        }
-    ).lazy()
+    df_b = (
+        pl.DataFrame(
+            {
+                "id": [1, 1, 2],
+                "b": [-3, -3, 6],
+            }
+        )
+        .lazy()
+        .set_sorted("b")
+    )
 
     q = (
         df_a.join_asof(df_b, by="id", left_on="a", right_on="b")
         .drop("b")
         .join_asof(df_b, by="id", left_on="a", right_on="b")
         .drop("b")
     )
@@ -104,15 +112,17 @@
         == {"id": pl.Int64, "a": pl.Int64, "b_right": pl.Int64}
     )
 
 
 def test_join_asof_floats() -> None:
     df1 = pl.DataFrame({"a": [1.0, 2.0, 3.0], "b": ["lrow1", "lrow2", "lrow3"]})
     df2 = pl.DataFrame({"a": [0.59, 1.49, 2.89], "b": ["rrow1", "rrow2", "rrow3"]})
-    assert df1.join_asof(df2, on="a", strategy="backward").to_dict(False) == {
+    assert df1.join_asof(df2, on=pl.col("a").set_sorted(), strategy="backward").to_dict(
+        False
+    ) == {
         "a": [1.0, 2.0, 3.0],
         "b": ["lrow1", "lrow2", "lrow3"],
         "b_right": ["rrow1", "rrow2", "rrow3"],
     }
 
     # with by argument
     # 5740
@@ -121,15 +131,15 @@
     )
     df2 = pl.DataFrame(
         {
             "val": [0, 2.5, 2.6, 2.7, 3.4, 4, 5],
             "c": ["x", "x", "x", "y", "y", "y", "y"],
         }
     ).with_columns(pl.col("val").alias("b"))
-    assert df1.join_asof(df2, on="b", by="c").to_dict(False) == {
+    assert df1.join_asof(df2, on=pl.col("b").set_sorted(), by="c").to_dict(False) == {
         "b": [
             0.0,
             0.8333333333333334,
             1.6666666666666667,
             2.5,
             3.3333333333333335,
             4.166666666666667,
@@ -148,28 +158,28 @@
                 datetime(2020, 1, 1, 9, 0, 1),
                 datetime(2020, 1, 1, 9, 0, 3),
                 datetime(2020, 1, 1, 9, 0, 6),
             ],
             "stock": ["A", "B", "B", "C"],
             "trade": [101, 299, 301, 500],
         }
-    )
+    ).set_sorted("time")
 
     df_quotes = pl.DataFrame(
         {
             "time": [
                 datetime(2020, 1, 1, 9, 0, 0),
                 datetime(2020, 1, 1, 9, 0, 2),
                 datetime(2020, 1, 1, 9, 0, 4),
                 datetime(2020, 1, 1, 9, 0, 6),
             ],
             "stock": ["A", "B", "C", "A"],
             "quote": [100, 300, 501, 102],
         }
-    )
+    ).set_sorted("time")
 
     assert df_trades.join_asof(
         df_quotes, on="time", by="stock", tolerance="2s"
     ).to_dict(False) == {
         "time": [
             datetime(2020, 1, 1, 9, 0, 1),
             datetime(2020, 1, 1, 9, 0, 1),
@@ -205,29 +215,29 @@
                 datetime(2020, 1, 1, 9, 0, 4),
                 datetime(2020, 1, 1, 9, 0, 6),
                 datetime(2020, 1, 1, 9, 0, 7),
             ],
             "stock": ["A", "B", "C", "A", "D"],
             "quote": [100, 300, 501, 102, 10],
         }
-    )
+    ).set_sorted("time")
 
     df_trades = pl.DataFrame(
         {
             "time": [
                 datetime(2020, 1, 1, 9, 0, 2),
                 datetime(2020, 1, 1, 9, 0, 1),
                 datetime(2020, 1, 1, 9, 0, 3),
                 datetime(2020, 1, 1, 9, 0, 6),
                 datetime(2020, 1, 1, 9, 0, 7),
             ],
             "stock": ["A", "B", "B", "C", "D"],
             "trade": [101, 299, 301, 500, 10],
         }
-    )
+    ).set_sorted("time")
 
     assert df_quotes.join_asof(
         df_trades, on="time", by="stock", tolerance="2s", strategy="forward"
     ).to_dict(False) == {
         "time": [
             datetime(2020, 1, 1, 9, 0, 0),
             datetime(2020, 1, 1, 9, 0, 2),
@@ -275,23 +285,23 @@
 def test_join_asof_projection() -> None:
     df1 = pl.DataFrame(
         {
             "df1_date": [20221011, 20221012, 20221013, 20221014, 20221016],
             "df1_col1": ["foo", "bar", "foo", "bar", "foo"],
             "key": ["a", "b", "b", "a", "b"],
         }
-    )
+    ).set_sorted("df1_date")
 
     df2 = pl.DataFrame(
         {
             "df2_date": [20221012, 20221015, 20221018],
             "df2_col1": ["1", "2", "3"],
             "key": ["a", "b", "b"],
         }
-    )
+    ).set_sorted("df2_date")
 
     assert (
         (
             df1.lazy().join_asof(df2.lazy(), left_on="df1_date", right_on="df2_date")
         ).select([pl.col("df2_date"), "df1_date"])
     ).collect().to_dict(False) == {
         "df2_date": [None, 20221012, 20221012, 20221012, 20221015],
@@ -310,15 +320,17 @@
 def test_asof_join_by_logical_types() -> None:
     dates = (
         pl.date_range(datetime(2022, 1, 1), datetime(2022, 1, 2), interval="2h")
         .cast(pl.Datetime("ns"))
         .head(9)
     )
     x = pl.DataFrame({"a": dates, "b": map(float, range(9)), "c": ["1", "2", "3"] * 3})
-    assert x.join_asof(x, on="b", by=["c", "a"]).to_dict(False) == {
+    assert x.join_asof(x, on=pl.col("b").set_sorted(), by=["c", "a"]).to_dict(
+        False
+    ) == {
         "a": [
             datetime(2022, 1, 1, 0, 0),
             datetime(2022, 1, 1, 2, 0),
             datetime(2022, 1, 1, 4, 0),
             datetime(2022, 1, 1, 6, 0),
             datetime(2022, 1, 1, 8, 0),
             datetime(2022, 1, 1, 10, 0),
@@ -328,13 +340,13 @@
         ],
         "b": [0.0, 1.0, 2.0, 3.0, 4.0, 5.0, 6.0, 7.0, 8.0],
         "c": ["1", "2", "3", "1", "2", "3", "1", "2", "3"],
     }
 
 
 def test_join_asof_projection_7481() -> None:
-    ldf1 = pl.DataFrame({"a": [1, 2, 2], "b": "bleft"}).lazy()
-    ldf2 = pl.DataFrame({"a": 2, "b": [1, 2, 2]}).lazy()
+    ldf1 = pl.DataFrame({"a": [1, 2, 2], "b": "bleft"}).lazy().set_sorted("a")
+    ldf2 = pl.DataFrame({"a": 2, "b": [1, 2, 2]}).lazy().set_sorted("b")
 
     assert (
         ldf1.join_asof(ldf2, left_on="a", right_on="b").select("a", "b")
     ).collect().to_dict(False) == {"a": [1, 2, 2], "b": ["bleft", "bleft", "bleft"]}
```

### Comparing `polars_u64_idx-0.17.8/tests/unit/operations/test_melt.py` & `polars_u64_idx-0.17.9/tests/unit/operations/test_melt.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/tests/unit/operations/test_pivot.py` & `polars_u64_idx-0.17.9/tests/unit/operations/test_pivot.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/tests/unit/operations/test_rolling.py` & `polars_u64_idx-0.17.9/tests/unit/operations/test_rolling.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,21 +50,25 @@
             pl.col("dt"),
             pl.col("values").rolling_sum(period, by="dt", closed=closed).alias("sum"),
             pl.col("values").rolling_var(period, by="dt", closed=closed).alias("var"),
             pl.col("values").rolling_mean(period, by="dt", closed=closed).alias("mean"),
             pl.col("values").rolling_std(period, by="dt", closed=closed).alias("std"),
         ]
     )
-    out2 = example_df.groupby_rolling("dt", period=period, closed=closed).agg(
-        [
-            pl.col("values").sum().alias("sum"),
-            pl.col("values").var().alias("var"),
-            pl.col("values").mean().alias("mean"),
-            pl.col("values").std().alias("std"),
-        ]
+    out2 = (
+        example_df.set_sorted("dt")
+        .groupby_rolling("dt", period=period, closed=closed)
+        .agg(
+            [
+                pl.col("values").sum().alias("sum"),
+                pl.col("values").var().alias("var"),
+                pl.col("values").mean().alias("mean"),
+                pl.col("values").std().alias("std"),
+            ]
+        )
     )
     assert_frame_equal(out1, out2)
 
 
 def test_rolling_skew() -> None:
     s = pl.Series([1, 2, 3, 3, 2, 10, 8])
     assert s.rolling_skew(window_size=4, bias=True).to_list() == pytest.approx(
@@ -163,103 +167,90 @@
         "col1_nulls": [None, None, None, None, None, 5, 5],
         "col2_nulls": [None, None, None, None, None, 4, 4],
     }
 
 
 def test_rolling_groupby_extrema() -> None:
     # ensure we hit different branches so create
-    # two dfs, but ensure that one does not have a sorted flag
-
-    # descending order
-    not_sorted_flag = pl.DataFrame({"col1": [6, 5, 4, 3, 2, 1, 0]}).with_columns(
-        pl.col("col1").reverse().alias("row_nr")
-    )
-    assert not not_sorted_flag["col1"].flags["SORTED_DESC"]
 
-    sorted_flag = pl.DataFrame(
+    df = pl.DataFrame(
         {
             "col1": pl.arange(0, 7, eager=True).reverse(),
         }
     ).with_columns(pl.col("col1").reverse().alias("row_nr"))
 
-    for df in [sorted_flag, not_sorted_flag]:
-        assert (
-            df.groupby_rolling(
-                index_column="row_nr",
-                period="3i",
-            )
-            .agg(
-                [
-                    pl.col("col1").suffix("_list"),
-                    pl.col("col1").min().suffix("_min"),
-                    pl.col("col1").max().suffix("_max"),
-                    pl.col("col1").first().alias("col1_first"),
-                    pl.col("col1").last().alias("col1_last"),
-                ]
-            )
-            .select(["col1_list", "col1_min", "col1_max", "col1_first", "col1_last"])
-        ).to_dict(False) == {
-            "col1_list": [
-                [6],
-                [6, 5],
-                [6, 5, 4],
-                [5, 4, 3],
-                [4, 3, 2],
-                [3, 2, 1],
-                [2, 1, 0],
-            ],
-            "col1_min": [6, 5, 4, 3, 2, 1, 0],
-            "col1_max": [6, 6, 6, 5, 4, 3, 2],
-            "col1_first": [6, 6, 6, 5, 4, 3, 2],
-            "col1_last": [6, 5, 4, 3, 2, 1, 0],
-        }
+    assert (
+        df.groupby_rolling(
+            index_column="row_nr",
+            period="3i",
+        )
+        .agg(
+            [
+                pl.col("col1").suffix("_list"),
+                pl.col("col1").min().suffix("_min"),
+                pl.col("col1").max().suffix("_max"),
+                pl.col("col1").first().alias("col1_first"),
+                pl.col("col1").last().alias("col1_last"),
+            ]
+        )
+        .select(["col1_list", "col1_min", "col1_max", "col1_first", "col1_last"])
+    ).to_dict(False) == {
+        "col1_list": [
+            [6],
+            [6, 5],
+            [6, 5, 4],
+            [5, 4, 3],
+            [4, 3, 2],
+            [3, 2, 1],
+            [2, 1, 0],
+        ],
+        "col1_min": [6, 5, 4, 3, 2, 1, 0],
+        "col1_max": [6, 6, 6, 5, 4, 3, 2],
+        "col1_first": [6, 6, 6, 5, 4, 3, 2],
+        "col1_last": [6, 5, 4, 3, 2, 1, 0],
+    }
 
     # ascending order
 
-    sorted_df = pl.DataFrame(
+    df = pl.DataFrame(
         {
             "col1": pl.arange(0, 7, eager=True),
         }
     ).with_columns(pl.col("col1").alias("row_nr"))
 
-    not_sorted_df = pl.DataFrame({"col1": [0, 1, 2, 3, 4, 5, 6]}).with_columns(
-        pl.col("col1").alias("row_nr")
-    )
-
-    for df in [sorted_df, not_sorted_df]:
-        assert (
-            df.groupby_rolling(
-                index_column="row_nr",
-                period="3i",
-            )
-            .agg(
-                [
-                    pl.col("col1").suffix("_list"),
-                    pl.col("col1").min().suffix("_min"),
-                    pl.col("col1").max().suffix("_max"),
-                    pl.col("col1").first().alias("col1_first"),
-                    pl.col("col1").last().alias("col1_last"),
-                ]
-            )
-            .select(["col1_list", "col1_min", "col1_max", "col1_first", "col1_last"])
-        ).to_dict(False) == {
-            "col1_list": [
-                [0],
-                [0, 1],
-                [0, 1, 2],
-                [1, 2, 3],
-                [2, 3, 4],
-                [3, 4, 5],
-                [4, 5, 6],
-            ],
-            "col1_min": [0, 0, 0, 1, 2, 3, 4],
-            "col1_max": [0, 1, 2, 3, 4, 5, 6],
-            "col1_first": [0, 0, 0, 1, 2, 3, 4],
-            "col1_last": [0, 1, 2, 3, 4, 5, 6],
-        }
+    assert (
+        df.groupby_rolling(
+            index_column="row_nr",
+            period="3i",
+        )
+        .agg(
+            [
+                pl.col("col1").suffix("_list"),
+                pl.col("col1").min().suffix("_min"),
+                pl.col("col1").max().suffix("_max"),
+                pl.col("col1").first().alias("col1_first"),
+                pl.col("col1").last().alias("col1_last"),
+            ]
+        )
+        .select(["col1_list", "col1_min", "col1_max", "col1_first", "col1_last"])
+    ).to_dict(False) == {
+        "col1_list": [
+            [0],
+            [0, 1],
+            [0, 1, 2],
+            [1, 2, 3],
+            [2, 3, 4],
+            [3, 4, 5],
+            [4, 5, 6],
+        ],
+        "col1_min": [0, 0, 0, 1, 2, 3, 4],
+        "col1_max": [0, 1, 2, 3, 4, 5, 6],
+        "col1_first": [0, 0, 0, 1, 2, 3, 4],
+        "col1_last": [0, 1, 2, 3, 4, 5, 6],
+    }
 
     # shuffled data.
     df = pl.DataFrame(
         {
             "col1": pl.arange(0, 7, eager=True).shuffle(1),
         }
     ).with_columns(pl.col("col1").sort().alias("row_nr"))
@@ -342,15 +333,15 @@
 
 def test_overlapping_groups_4628() -> None:
     df = pl.DataFrame(
         {
             "index": [1, 2, 3, 4, 5, 6],
             "val": [10, 20, 40, 70, 110, 160],
         }
-    )
+    ).set_sorted("index")
     assert (
         df.groupby_rolling(index_column="index", period="3i").agg(
             [
                 pl.col("val").diff(n=1).alias("val.diff"),
                 (pl.col("val") - pl.col("val").shift(1)).alias("val - val.shift"),
             ]
         )
@@ -527,15 +518,15 @@
                 "2022-11-08",
                 "2022-11-09",
                 "2022-11-10",
             ],
             "label": ["a", "b", "a", "a", "b", "a", "b"],
             "value": [1, 2, 3, 4, 5, 6, 7],
         }
-    ).with_columns(pl.col("date").str.strptime(pl.Date, "%Y-%m-%d"))
+    ).with_columns(pl.col("date").str.strptime(pl.Date, "%Y-%m-%d").set_sorted())
 
     result = df.groupby_dynamic(
         "date", every="1w", offset="1d", by="label", start_by="monday"
     ).agg(pl.col("value").sum())
 
     assert result.to_dict(False) == {
         "label": ["a", "a", "b", "b"],
@@ -560,15 +551,15 @@
 def test_groupby_rolling_iter() -> None:
     df = pl.DataFrame(
         {
             "date": [date(2020, 1, 1), date(2020, 1, 2), date(2020, 1, 5)],
             "a": [1, 2, 2],
             "b": [4, 5, 6],
         }
-    )
+    ).set_sorted("date")
 
     # Without 'by' argument
     result1 = [
         (name, data.shape)
         for name, data in df.groupby_rolling(index_column="date", period="2d")
     ]
     expected1 = [
```

### Comparing `polars_u64_idx-0.17.8/tests/unit/operations/test_sort.py` & `polars_u64_idx-0.17.9/tests/unit/operations/test_sort.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/tests/unit/operations/test_statistics.py` & `polars_u64_idx-0.17.9/tests/unit/operations/test_statistics.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from datetime import timedelta
+
 import numpy as np
 
 import polars as pl
 from polars.testing import assert_frame_equal
 
 
 def test_corr() -> None:
@@ -87,7 +89,17 @@
         str(s.qcut([0.2, 0.3], maintain_order=True).to_dict(False))
         == "{'': [-1.0, None, 1.0, 2.0, None, 8.0, 4.0], 'break_point': [0.5999999999999996, None, 1.2000000000000002, inf, None, inf, inf], 'category': ['(-inf, 0.5999999999999996]', None, '(0.5999999999999996, 1.2000000000000002]', '(1.2000000000000002, inf]', None, '(1.2000000000000002, inf]', '(1.2000000000000002, inf]']}"
     )
     assert (
         str(s.qcut([0.2, 0.3], maintain_order=False).to_dict(False))
         == "{'': [-1.0, 1.0, 2.0, 4.0, 8.0, None, None], 'break_point': [0.5999999999999996, 1.2000000000000002, inf, inf, inf, None, None], 'category': ['(-inf, 0.5999999999999996]', '(0.5999999999999996, 1.2000000000000002]', '(1.2000000000000002, inf]', '(1.2000000000000002, inf]', '(1.2000000000000002, inf]', None, None]}"
     )
+
+
+def test_median_quantile_duration() -> None:
+    df = pl.DataFrame({"A": [timedelta(days=0), timedelta(days=1)]})
+    assert df.select(pl.col("A").median()).to_dict(False) == {
+        "A": [timedelta(seconds=43200)]
+    }
+    assert df.select(pl.col("A").quantile(0.5, interpolation="linear")).to_dict(
+        False
+    ) == {"A": [timedelta(seconds=43200)]}
```

### Comparing `polars_u64_idx-0.17.8/tests/unit/operations/test_transpose.py` & `polars_u64_idx-0.17.9/tests/unit/operations/test_transpose.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/tests/unit/operations/test_unique.py` & `polars_u64_idx-0.17.9/tests/unit/operations/test_unique.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/tests/unit/operations/test_window.py` & `polars_u64_idx-0.17.9/tests/unit/operations/test_window.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/tests/unit/test_api.py` & `polars_u64_idx-0.17.9/tests/unit/test_api.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/tests/unit/test_arity.py` & `polars_u64_idx-0.17.9/tests/unit/test_arity.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/tests/unit/test_cfg.py` & `polars_u64_idx-0.17.9/tests/unit/test_cfg.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/tests/unit/test_constructors.py` & `polars_u64_idx-0.17.9/tests/unit/test_constructors.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/tests/unit/test_cse.py` & `polars_u64_idx-0.17.9/tests/unit/test_cse.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/tests/unit/test_datatypes.py` & `polars_u64_idx-0.17.9/tests/unit/test_datatypes.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/tests/unit/test_df.py` & `polars_u64_idx-0.17.9/tests/unit/test_df.py`

 * *Files 1% similar despite different names*

```diff
@@ -1713,16 +1713,20 @@
         }
     )
     out = df.join(df, on="datetime")
     assert len(out) == len(df)
 
 
 def test_asof_cross_join() -> None:
-    left = pl.DataFrame({"a": [-10, 5, 10], "left_val": ["a", "b", "c"]})
-    right = pl.DataFrame({"a": [1, 2, 3, 6, 7], "right_val": [1, 2, 3, 6, 7]})
+    left = pl.DataFrame({"a": [-10, 5, 10], "left_val": ["a", "b", "c"]}).with_columns(
+        pl.col("a").set_sorted()
+    )
+    right = pl.DataFrame(
+        {"a": [1, 2, 3, 6, 7], "right_val": [1, 2, 3, 6, 7]}
+    ).with_columns(pl.col("a").set_sorted())
 
     # only test dispatch of asof join
     out = left.join_asof(right, on="a")
     assert out.shape == (3, 3)
 
     left.lazy().join_asof(right.lazy(), on="a").collect()
     assert out.shape == (3, 3)
@@ -2692,15 +2696,15 @@
     df_b = pl.DataFrame({"A": [1], "B": [1]})
 
     join_strategies: list[JoinStrategy] = ["left", "inner", "outer", "cross"]
     for how in join_strategies:
         # no need for an assert, we error if wrong
         df_a.join(df_b, on="A", suffix="_y", how=how)["B_y"]
 
-    df_a.join_asof(df_b, on="A", suffix="_y")["B_y"]
+    df_a.join_asof(df_b, on=pl.col("A").set_sorted(), suffix="_y")["B_y"]
 
 
 def test_preservation_of_subclasses_after_groupby_statements() -> None:
     """Group by operations should preserve inherited dataframe classes."""
 
     class SubClassedDataFrame(pl.DataFrame):
         pass
@@ -2747,17 +2751,17 @@
         {
             "a": [-19, -15, 3, 5, 13],
             "by": [1, 1, 2, 2, 2],
             "by2": [1, 1, 2, 2, 2],
         }
     )
 
-    result = lhs.join_asof(rhs, on="a", by=["by", "by2"], strategy="backward").select(
-        ["a", "by"]
-    )
+    result = lhs.join_asof(
+        rhs, on=pl.col("a").set_sorted(), by=["by", "by2"], strategy="backward"
+    ).select(["a", "by"])
     expected = pl.DataFrame({"a": [-20, -19, 8, 12, 14], "by": [1, 1, 2, 2, 2]})
     assert_frame_equal(result, expected)
 
 
 @typing.no_type_check
 def test_partition_by() -> None:
     df = pl.DataFrame(
```

### Comparing `polars_u64_idx-0.17.8/tests/unit/test_empty.py` & `polars_u64_idx-0.17.9/tests/unit/test_empty.py`

 * *Files 12% similar despite different names*

```diff
@@ -32,7 +32,18 @@
     assert s.str.replace("ab", "b").series_equal(s)
 
 
 def test_empty_duration() -> None:
     s = pl.DataFrame([], {"days": pl.Int32}).select(pl.duration(days="days"))
     assert s.dtypes == [pl.Duration("ns")]
     assert s.shape == (0, 1)
+
+
+def test_empty_window_function() -> None:
+    expr = (pl.col("VAL") / pl.col("VAL").sum()).over("KEY")
+
+    df = pl.DataFrame(schema={"KEY": pl.Utf8, "VAL": pl.Float64})
+    df.select(expr)  # ComputeError
+
+    lf = pl.DataFrame(schema={"KEY": pl.Utf8, "VAL": pl.Float64}).lazy()
+    expected = pl.DataFrame(schema={"VAL": pl.Float64})
+    assert_frame_equal(lf.select(expr).collect(), expected)
```

### Comparing `polars_u64_idx-0.17.8/tests/unit/test_errors.py` & `polars_u64_idx-0.17.9/tests/unit/test_errors.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 def test_error_on_invalid_by_in_asof_join() -> None:
     df1 = pl.DataFrame(
         {
             "a": ["a", "b", "a"],
             "b": [1, 2, 3],
             "c": ["a", "b", "a"],
         }
-    )
+    ).set_sorted("b")
 
     df2 = df1.with_columns(pl.col("a").cast(pl.Categorical))
     with pytest.raises(pl.ComputeError):
         df1.join_asof(df2, on="b", by=["a", "c"])
 
 
 def test_error_on_invalid_struct_field() -> None:
@@ -581,8 +581,8 @@
     df = pl.DataFrame(
         {
             "dt": [datetime(2001, 1, 1), datetime(2001, 1, 2)],
         }
     )
     df.groupby_dynamic("dt", every="1h").agg(pl.all().count().suffix("_foo"))
     (_, err) = capfd.readouterr()
-    assert "argument is not explicitly sorted" in err
+    assert "argument in operation 'groupby_dynamic' is not explicitly sorted" in err
```

### Comparing `polars_u64_idx-0.17.8/tests/unit/test_expr_multi_cols.py` & `polars_u64_idx-0.17.9/tests/unit/test_expr_multi_cols.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/tests/unit/test_exprs.py` & `polars_u64_idx-0.17.9/tests/unit/test_exprs.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/tests/unit/test_fmt.py` & `polars_u64_idx-0.17.9/tests/unit/test_fmt.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/tests/unit/test_functions.py` & `polars_u64_idx-0.17.9/tests/unit/test_functions.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/tests/unit/test_interchange.py` & `polars_u64_idx-0.17.9/tests/unit/test_interchange.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/tests/unit/test_interop.py` & `polars_u64_idx-0.17.9/tests/unit/test_interop.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/tests/unit/test_lazy.py` & `polars_u64_idx-0.17.9/tests/unit/test_lazy.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/tests/unit/test_polars_import.py` & `polars_u64_idx-0.17.9/tests/unit/test_polars_import.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/tests/unit/test_predicates.py` & `polars_u64_idx-0.17.9/tests/unit/test_predicates.py`

 * *Files 6% similar despite different names*

```diff
@@ -40,40 +40,48 @@
     ).to_dict(False) == {
         "literal": ["Foo", "Foo", "Foo", None, None, None],
         "bar": ["Foo", "Foo", "Foo", None, None, None],
     }
 
 
 def test_predicate_null_block_asof_join() -> None:
-    left = pl.DataFrame(
-        {
-            "id": [1, 2, 3, 4],
-            "timestamp": [
-                datetime(2022, 1, 1, 10, 0),
-                datetime(2022, 1, 1, 10, 1),
-                datetime(2022, 1, 1, 10, 2),
-                datetime(2022, 1, 1, 10, 3),
-            ],
-        }
-    ).lazy()
+    left = (
+        pl.DataFrame(
+            {
+                "id": [1, 2, 3, 4],
+                "timestamp": [
+                    datetime(2022, 1, 1, 10, 0),
+                    datetime(2022, 1, 1, 10, 1),
+                    datetime(2022, 1, 1, 10, 2),
+                    datetime(2022, 1, 1, 10, 3),
+                ],
+            }
+        )
+        .lazy()
+        .set_sorted("timestamp")
+    )
 
-    right = pl.DataFrame(
-        {
-            "id": [1, 2, 3] * 2,
-            "timestamp": [
-                datetime(2022, 1, 1, 9, 59, 50),
-                datetime(2022, 1, 1, 10, 0, 50),
-                datetime(2022, 1, 1, 10, 1, 50),
-                datetime(2022, 1, 1, 8, 0, 0),
-                datetime(2022, 1, 1, 8, 0, 0),
-                datetime(2022, 1, 1, 8, 0, 0),
-            ],
-            "value": ["a", "b", "c"] * 2,
-        }
-    ).lazy()
+    right = (
+        pl.DataFrame(
+            {
+                "id": [1, 2, 3] * 2,
+                "timestamp": [
+                    datetime(2022, 1, 1, 9, 59, 50),
+                    datetime(2022, 1, 1, 10, 0, 50),
+                    datetime(2022, 1, 1, 10, 1, 50),
+                    datetime(2022, 1, 1, 8, 0, 0),
+                    datetime(2022, 1, 1, 8, 0, 0),
+                    datetime(2022, 1, 1, 8, 0, 0),
+                ],
+                "value": ["a", "b", "c"] * 2,
+            }
+        )
+        .lazy()
+        .set_sorted("timestamp")
+    )
 
     assert left.join_asof(right, by="id", on="timestamp").filter(
         pl.col("value").is_not_null()
     ).collect().to_dict(False) == {
         "id": [1, 2, 3],
         "timestamp": [
             datetime(2022, 1, 1, 10, 0),
```

### Comparing `polars_u64_idx-0.17.8/tests/unit/test_projections.py` & `polars_u64_idx-0.17.9/tests/unit/test_projections.py`

 * *Files 2% similar despite different names*

```diff
@@ -158,33 +158,38 @@
         "c": [1, 2, 3],
         "a": [[1, 2, 5, 7], [3, 4, 6], [8]],
     }
 
 
 @typing.no_type_check
 def test_asof_join_projection_() -> None:
-    lf1 = pl.DataFrame(
-        {
-            "m": np.linspace(0, 5, 7),
-            "a": np.linspace(0, 5, 7),
-            "b": np.linspace(0, 5, 7),
-            "c": pl.Series(np.linspace(0, 5, 7)).cast(str),
-            "d": np.linspace(0, 5, 7),
-        }
-    ).lazy()
+    lf1 = (
+        pl.DataFrame(
+            {
+                "m": np.linspace(0, 5, 7),
+                "a": np.linspace(0, 5, 7),
+                "b": np.linspace(0, 5, 7),
+                "c": pl.Series(np.linspace(0, 5, 7)).cast(str),
+                "d": np.linspace(0, 5, 7),
+            }
+        )
+        .lazy()
+        .set_sorted("b")
+    )
     lf2 = (
         pl.DataFrame(
             {
                 "group": [0, 2, 3, 0, 1, 2, 3],
                 "val": [0, 2.5, 2.6, 2.7, 3.4, 4, 5],
                 "c": ["x", "x", "x", "y", "y", "y", "y"],
             }
         )
         .with_columns(pl.col("val").alias("b"))
         .lazy()
+        .set_sorted("b")
     )
 
     joined = lf1.join_asof(
         lf2,
         on="b",
         by=["c"],
         strategy="backward",
```

### Comparing `polars_u64_idx-0.17.8/tests/unit/test_queries.py` & `polars_u64_idx-0.17.9/tests/unit/test_queries.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/tests/unit/test_rows.py` & `polars_u64_idx-0.17.9/tests/unit/test_rows.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/tests/unit/test_schema.py` & `polars_u64_idx-0.17.9/tests/unit/test_schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -140,15 +140,15 @@
         False
     ) == {"a": ["1", "2", "3"], "b": ["a", "b", "c"]}
 
 
 def test_join_as_of_by_schema() -> None:
     a = pl.DataFrame({"a": [1], "b": [2], "c": [3]}).lazy()
     b = pl.DataFrame({"a": [1], "b": [2], "d": [4]}).lazy()
-    q = a.join_asof(b, on="a", by="b")
+    q = a.join_asof(b, on=pl.col("a").set_sorted(), by="b")
     assert q.collect().columns == q.columns
 
 
 def test_unknown_apply() -> None:
     df = pl.DataFrame(
         {"Amount": [10, 1, 1, 5], "Flour": ["1000g", "100g", "50g", "75g"]}
     )
```

### Comparing `polars_u64_idx-0.17.8/tests/unit/test_serde.py` & `polars_u64_idx-0.17.9/tests/unit/test_serde.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/tests/unit/test_series.py` & `polars_u64_idx-0.17.9/tests/unit/test_series.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/tests/unit/test_sql.py` & `polars_u64_idx-0.17.9/tests/unit/test_sql.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/tests/unit/test_streaming.py` & `polars_u64_idx-0.17.9/tests/unit/test_streaming.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/tests/unit/test_testing.py` & `polars_u64_idx-0.17.9/tests/unit/test_testing.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/tests/unit/utils/test_utils.py` & `polars_u64_idx-0.17.9/tests/unit/utils/test_utils.py`

 * *Files identical despite different names*

### Comparing `polars_u64_idx-0.17.8/Cargo.lock` & `polars_u64_idx-0.17.9/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -1733,15 +1733,15 @@
 checksum = "2b63bdb0cd06f1f4dedf69b254734f9b45af66e4a031e42a7480257d9898b435"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "py-polars"
-version = "0.17.8"
+version = "0.17.9"
 dependencies = [
  "ahash",
  "built",
  "ciborium",
  "jemallocator",
  "lexical-core",
  "libc",
```

### Comparing `polars_u64_idx-0.17.8/PKG-INFO` & `polars_u64_idx-0.17.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polars-u64-idx
-Version: 0.17.8
+Version: 0.17.9
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -13,50 +13,50 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Rust
 Classifier: Topic :: Scientific/Engineering
 Requires-Dist: typing_extensions >= 4.0.1; python_version < '3.11'
-Requires-Dist: xlsx2csv >= 0.8.0; extra == 'xlsx2csv'
-Requires-Dist: connectorx; extra == 'connectorx'
+Requires-Dist: pyarrow>=7.0.0; extra == 'pyarrow'
 Requires-Dist: backports.zoneinfo; (python_version < '3.9') and extra == 'timezone'
 Requires-Dist: tzdata; (platform_system == 'Windows') and extra == 'timezone'
-Requires-Dist: numpy >= 1.16.0; extra == 'numpy'
-Requires-Dist: pyarrow>=7.0.0; extra == 'pandas'
-Requires-Dist: pandas; extra == 'pandas'
+Requires-Dist: xlsxwriter; extra == 'xlsxwriter'
 Requires-Dist: matplotlib; extra == 'matplotlib'
-Requires-Dist: pyarrow>=7.0.0; extra == 'pyarrow'
+Requires-Dist: deltalake >= 0.8.0; extra == 'deltalake'
+Requires-Dist: xlsx2csv >= 0.8.0; extra == 'xlsx2csv'
 Requires-Dist: sqlalchemy; extra == 'sqlalchemy'
 Requires-Dist: pandas; extra == 'sqlalchemy'
-Requires-Dist: xlsxwriter; extra == 'xlsxwriter'
 Requires-Dist: fsspec; extra == 'fsspec'
+Requires-Dist: pyarrow>=7.0.0; extra == 'pandas'
+Requires-Dist: pandas; extra == 'pandas'
+Requires-Dist: numpy >= 1.16.0; extra == 'numpy'
+Requires-Dist: connectorx; extra == 'connectorx'
 Requires-Dist: polars[pyarrow,pandas,numpy,fsspec,connectorx,xlsx2csv,deltalake,timezone,matplotlib,sqlalchemy,xlsxwriter]; extra == 'all'
-Requires-Dist: deltalake >= 0.8.0; extra == 'deltalake'
-Provides-Extra: xlsx2csv
-Provides-Extra: connectorx
+Provides-Extra: pyarrow
 Provides-Extra: timezone
-Provides-Extra: numpy
-Provides-Extra: pandas
+Provides-Extra: xlsxwriter
 Provides-Extra: matplotlib
-Provides-Extra: pyarrow
+Provides-Extra: deltalake
+Provides-Extra: xlsx2csv
 Provides-Extra: sqlalchemy
-Provides-Extra: xlsxwriter
 Provides-Extra: fsspec
+Provides-Extra: pandas
+Provides-Extra: numpy
+Provides-Extra: connectorx
 Provides-Extra: all
-Provides-Extra: deltalake
 License-File: LICENSE
 Summary: Blazingly fast DataFrame library
 Keywords: dataframe,arrow,out-of-core
 Author-email: Ritchie Vink <ritchie46@gmail.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
+Project-URL: Repository, https://github.com/pola-rs/polars
 Project-URL: Homepage, https://www.pola.rs/
 Project-URL: Changelog, https://github.com/pola-rs/polars/releases
-Project-URL: Repository, https://github.com/pola-rs/polars
 Project-URL: Documentation, https://pola-rs.github.io/polars/py-polars/html/reference/index.html
 
 <h1 align="center">
   <img src="https://raw.githubusercontent.com/pola-rs/polars-static/master/logos/polars_github_logo_rect_dark_name.svg">
   <br>
 </h1>
```

#### html2text {}

```diff
@@ -1,41 +1,41 @@
-Metadata-Version: 2.1 Name: polars-u64-idx Version: 0.17.8 Classifier:
+Metadata-Version: 2.1 Name: polars-u64-idx Version: 0.17.9 Classifier:
 Development Status :: 5 - Production/Stable Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3 :: Only Classifier:
 Programming Language :: Python :: 3.7 Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Programming Language :: Rust Classifier: Topic ::
 Scientific/Engineering Requires-Dist: typing_extensions >= 4.0.1;
-python_version < '3.11' Requires-Dist: xlsx2csv >= 0.8.0; extra == 'xlsx2csv'
-Requires-Dist: connectorx; extra == 'connectorx' Requires-Dist:
-backports.zoneinfo; (python_version < '3.9') and extra == 'timezone' Requires-
-Dist: tzdata; (platform_system == 'Windows') and extra == 'timezone' Requires-
-Dist: numpy >= 1.16.0; extra == 'numpy' Requires-Dist: pyarrow>=7.0.0; extra ==
-'pandas' Requires-Dist: pandas; extra == 'pandas' Requires-Dist: matplotlib;
-extra == 'matplotlib' Requires-Dist: pyarrow>=7.0.0; extra == 'pyarrow'
-Requires-Dist: sqlalchemy; extra == 'sqlalchemy' Requires-Dist: pandas; extra
-== 'sqlalchemy' Requires-Dist: xlsxwriter; extra == 'xlsxwriter' Requires-Dist:
-fsspec; extra == 'fsspec' Requires-Dist: polars
+python_version < '3.11' Requires-Dist: pyarrow>=7.0.0; extra == 'pyarrow'
+Requires-Dist: backports.zoneinfo; (python_version < '3.9') and extra ==
+'timezone' Requires-Dist: tzdata; (platform_system == 'Windows') and extra ==
+'timezone' Requires-Dist: xlsxwriter; extra == 'xlsxwriter' Requires-Dist:
+matplotlib; extra == 'matplotlib' Requires-Dist: deltalake >= 0.8.0; extra ==
+'deltalake' Requires-Dist: xlsx2csv >= 0.8.0; extra == 'xlsx2csv' Requires-
+Dist: sqlalchemy; extra == 'sqlalchemy' Requires-Dist: pandas; extra ==
+'sqlalchemy' Requires-Dist: fsspec; extra == 'fsspec' Requires-Dist:
+pyarrow>=7.0.0; extra == 'pandas' Requires-Dist: pandas; extra == 'pandas'
+Requires-Dist: numpy >= 1.16.0; extra == 'numpy' Requires-Dist: connectorx;
+extra == 'connectorx' Requires-Dist: polars
 [pyarrow,pandas,numpy,fsspec,connectorx,xlsx2csv,deltalake,timezone,matplotlib,sqlalchemy,xlsxwriter];
-extra == 'all' Requires-Dist: deltalake >= 0.8.0; extra == 'deltalake'
-Provides-Extra: xlsx2csv Provides-Extra: connectorx Provides-Extra: timezone
-Provides-Extra: numpy Provides-Extra: pandas Provides-Extra: matplotlib
-Provides-Extra: pyarrow Provides-Extra: sqlalchemy Provides-Extra: xlsxwriter
-Provides-Extra: fsspec Provides-Extra: all Provides-Extra: deltalake License-
-File: LICENSE Summary: Blazingly fast DataFrame library Keywords:
+extra == 'all' Provides-Extra: pyarrow Provides-Extra: timezone Provides-Extra:
+xlsxwriter Provides-Extra: matplotlib Provides-Extra: deltalake Provides-Extra:
+xlsx2csv Provides-Extra: sqlalchemy Provides-Extra: fsspec Provides-Extra:
+pandas Provides-Extra: numpy Provides-Extra: connectorx Provides-Extra: all
+License-File: LICENSE Summary: Blazingly fast DataFrame library Keywords:
 dataframe,arrow,out-of-core Author-email: Ritchie Vink
 gmail.com> Requires-Python: >=3.7 Description-Content-Type: text/markdown;
-charset=UTF-8; variant=GFM Project-URL: Homepage, https://www.pola.rs/ Project-
-URL: Changelog, https://github.com/pola-rs/polars/releases Project-URL:
-Repository, https://github.com/pola-rs/polars Project-URL: Documentation,
-https://pola-rs.github.io/polars/py-polars/html/reference/index.html
+charset=UTF-8; variant=GFM Project-URL: Repository, https://github.com/pola-rs/
+polars Project-URL: Homepage, https://www.pola.rs/ Project-URL: Changelog,
+https://github.com/pola-rs/polars/releases Project-URL: Documentation, https://
+pola-rs.github.io/polars/py-polars/html/reference/index.html
  ****** [https://raw.githubusercontent.com/pola-rs/polars-static/master/logos/
                     polars_github_logo_rect_dark_name.svg]
                                      ******
 [rust_docs] [Build_and_test] [https://img.shields.io/crates/v/polars.svg] [PyPi
  Latest_Release] [NPM_Latest_Release] [R-universe_Latest_Release] [DOI_Latest
                                    Release]
   Documentation: Python - Rust - Node.js - R | StackOverflow: Python - Rust -
```

