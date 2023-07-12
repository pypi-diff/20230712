# Comparing `tmp/gpboost-1.2.1.1.tar.gz` & `tmp/gpboost-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpboost-1.2.1.1.tar", last modified: Mon Jun 19 06:52:41 2023, max compression
+gzip compressed data, was "gpboost-1.2.2.tar", last modified: Wed Jul 12 05:46:21 2023, max compression
```

## Comparing `gpboost-1.2.1.1.tar` & `gpboost-1.2.2.tar`

### file list

```diff
@@ -1,1001 +1,999 @@
-drwxrwxrwx   0        0        0        0 2023-06-19 06:52:41.442449 gpboost-1.2.1.1/
--rw-rw-rw-   0        0        0    11248 2023-06-19 06:52:40.000000 gpboost-1.2.1.1/LICENSE
--rw-rw-rw-   0        0        0     3530 2022-02-01 20:40:50.000000 gpboost-1.2.1.1/MANIFEST.in
--rw-rw-rw-   0        0        0     8738 2023-06-19 06:52:41.440441 gpboost-1.2.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     7731 2023-01-24 07:52:28.000000 gpboost-1.2.1.1/README.md
--rw-rw-rw-   0        0        0        0 2023-06-19 06:52:40.000000 gpboost-1.2.1.1/_IS_SOURCE_PACKAGE.txt
-drwxrwxrwx   0        0        0        0 2023-06-19 06:52:40.986628 gpboost-1.2.1.1/compile/
--rw-rw-rw-   0        0        0     4828 2023-06-19 06:52:40.000000 gpboost-1.2.1.1/compile/CMakeIntegratedOpenCL.cmake
--rw-rw-rw-   0        0        0    16679 2023-06-19 06:52:40.000000 gpboost-1.2.1.1/compile/CMakeLists.txt
-drwxrwxrwx   0        0        0        0 2023-06-19 06:52:40.986628 gpboost-1.2.1.1/compile/Release/
--rw-rw-rw-   0        0        0  3895808 2023-06-19 06:49:53.000000 gpboost-1.2.1.1/compile/Release/lib_gpboost.dll
-drwxrwxrwx   0        0        0        0 2023-06-19 06:52:40.978039 gpboost-1.2.1.1/compile/external_libs/
-drwxrwxrwx   0        0        0        0 2023-06-19 06:52:40.960393 gpboost-1.2.1.1/compile/external_libs/CSparse/
-drwxrwxrwx   0        0        0        0 2023-06-19 06:52:40.989632 gpboost-1.2.1.1/compile/external_libs/CSparse/Doc/
--rw-rw-rw-   0        0        0      879 2014-03-21 19:14:15.000000 gpboost-1.2.1.1/compile/external_libs/CSparse/Doc/LICENSE.txt
-drwxrwxrwx   0        0        0        0 2023-06-19 06:52:40.989632 gpboost-1.2.1.1/compile/external_libs/CSparse/Include/
--rw-rw-rw-   0        0        0     3202 2023-01-18 08:20:43.000000 gpboost-1.2.1.1/compile/external_libs/CSparse/Include/cs.h
-drwxrwxrwx   0        0        0        0 2023-06-19 06:52:40.991628 gpboost-1.2.1.1/compile/external_libs/CSparse/Source/
--rw-rw-rw-   0        0        0     1624 2014-03-21 19:14:08.000000 gpboost-1.2.1.1/compile/external_libs/CSparse/Source/cs_dfs.c
--rw-rw-rw-   0        0        0      682 2020-03-25 11:28:02.000000 gpboost-1.2.1.1/compile/external_libs/CSparse/Source/cs_reach.c
--rw-rw-rw-   0        0        0     1364 2020-03-25 11:28:05.000000 gpboost-1.2.1.1/compile/external_libs/CSparse/Source/cs_spsolve.c
-drwxrwxrwx   0        0        0        0 2023-06-19 06:52:40.992628 gpboost-1.2.1.1/compile/external_libs/OptimLib/
--rw-rw-rw-   0        0        0    11558 2021-04-01 05:47:35.000000 gpboost-1.2.1.1/compile/external_libs/OptimLib/LICENSE
--rw-rw-rw-   0        0        0      211 2021-04-01 05:47:35.000000 gpboost-1.2.1.1/compile/external_libs/OptimLib/NOTICE.txt
-drwxrwxrwx   0        0        0        0 2023-06-19 06:52:40.992628 gpboost-1.2.1.1/compile/external_libs/OptimLib/constrained/
--rw-rw-rw-   0        0        0     7773 2021-04-01 05:49:27.000000 gpboost-1.2.1.1/compile/external_libs/OptimLib/constrained/sumt.hpp
-drwxrwxrwx   0        0        0        0 2023-06-19 06:52:40.993628 gpboost-1.2.1.1/compile/external_libs/OptimLib/line_search/
--rw-rw-rw-   0        0        0    11032 2021-04-01 05:49:27.000000 gpboost-1.2.1.1/compile/external_libs/OptimLib/line_search/more_thuente.hpp
-drwxrwxrwx   0        0        0        0 2023-06-19 06:52:41.000800 gpboost-1.2.1.1/compile/external_libs/OptimLib/misc/
--rw-rw-rw-   0        0        0     1975 2021-04-01 05:49:27.000000 gpboost-1.2.1.1/compile/external_libs/OptimLib/misc/determine_bounds_type.hpp
--rw-rw-rw-   0        0        0     3102 2021-04-01 05:49:27.000000 gpboost-1.2.1.1/compile/external_libs/OptimLib/misc/error_reporting.hpp
--rw-rw-rw-   0        0        0     7593 2021-04-01 12:25:42.000000 gpboost-1.2.1.1/compile/external_libs/OptimLib/misc/error_reporting.ipp
--rw-rw-rw-   0        0        0     2060 2021-04-01 05:49:27.000000 gpboost-1.2.1.1/compile/external_libs/OptimLib/misc/jacobian_adjust.hpp
-drwxrwxrwx   0        0        0        0 2023-06-19 06:52:41.019513 gpboost-1.2.1.1/compile/external_libs/OptimLib/misc/matrix_ops/
--rw-rw-rw-   0        0        0     1179 2021-04-01 05:49:27.000000 gpboost-1.2.1.1/compile/external_libs/OptimLib/misc/matrix_ops/abs.hpp
--rw-rw-rw-   0        0        0     1700 2021-04-01 05:49:27.000000 gpboost-1.2.1.1/compile/external_libs/OptimLib/misc/matrix_ops/abs_max.hpp
--rw-rw-rw-   0        0        0     1652 2021-04-01 05:49:27.000000 gpboost-1.2.1.1/compile/external_libs/OptimLib/misc/matrix_ops/access.hpp
--rw-rw-rw-   0        0        0     1256 2021-04-01 05:49:27.000000 gpboost-1.2.1.1/compile/external_libs/OptimLib/misc/matrix_ops/accu.hpp
--rw-rw-rw-   0        0        0     1178 2021-04-01 05:49:27.000000 gpboost-1.2.1.1/compile/external_libs/OptimLib/misc/matrix_ops/array_add.hpp
--rw-rw-rw-   0        0        0     1460 2021-04-01 05:49:27.000000 gpboost-1.2.1.1/compile/external_libs/OptimLib/misc/matrix_ops/array_div.hpp
--rw-rw-rw-   0        0        0     1181 2021-04-01 05:49:27.000000 gpboost-1.2.1.1/compile/external_libs/OptimLib/misc/matrix_ops/array_mult.hpp
--rw-rw-rw-   0        0        0     1156 2021-04-01 05:49:27.000000 gpboost-1.2.1.1/compile/external_libs/OptimLib/misc/matrix_ops/as_scalar.hpp
--rw-rw-rw-   0        0        0     1147 2021-04-01 05:49:27.000000 gpboost-1.2.1.1/compile/external_libs/OptimLib/misc/matrix_ops/cos.hpp
--rw-rw-rw-   0        0        0     1150 2021-04-01 05:49:27.000000 gpboost-1.2.1.1/compile/external_libs/OptimLib/misc/matrix_ops/cout.hpp
--rw-rw-rw-   0        0        0     1201 2021-04-01 05:49:27.000000 gpboost-1.2.1.1/compile/external_libs/OptimLib/misc/matrix_ops/diagmat.hpp
--rw-rw-rw-   0        0        0     1210 2021-04-01 05:49:27.000000 gpboost-1.2.1.1/compile/external_libs/OptimLib/misc/matrix_ops/diagvec.hpp
--rw-rw-rw-   0        0        0     1179 2021-04-01 05:49:27.000000 gpboost-1.2.1.1/compile/external_libs/OptimLib/misc/matrix_ops/dot.hpp
--rw-rw-rw-   0        0        0     1155 2021-04-01 05:49:27.000000 gpboost-1.2.1.1/compile/external_libs/OptimLib/misc/matrix_ops/endl.hpp
--rw-rw-rw-   0        0        0     1123 2021-04-01 05:49:27.000000 gpboost-1.2.1.1/compile/external_libs/OptimLib/misc/matrix_ops/eval.hpp
--rw-rw-rw-   0        0        0     1147 2021-04-01 05:49:27.000000 gpboost-1.2.1.1/compile/external_libs/OptimLib/misc/matrix_ops/exp.hpp
--rw-rw-rw-   0        0        0     1184 2021-04-01 05:49:27.000000 gpboost-1.2.1.1/compile/external_libs/OptimLib/misc/matrix_ops/eye.hpp
--rw-rw-rw-   0        0        0     1443 2021-04-11 01:03:04.000000 gpboost-1.2.1.1/compile/external_libs/OptimLib/misc/matrix_ops/get_sort_index.hpp
--rw-rw-rw-   0        0        0     1206 2021-04-01 05:49:27.000000 gpboost-1.2.1.1/compile/external_libs/OptimLib/misc/matrix_ops/hadamard.hpp
--rw-rw-rw-   0        0        0     1270 2021-04-01 05:49:27.000000 gpboost-1.2.1.1/compile/external_libs/OptimLib/misc/matrix_ops/index_min.hpp
--rw-rw-rw-   0        0        0     1176 2021-04-01 05:49:27.000000 gpboost-1.2.1.1/compile/external_libs/OptimLib/misc/matrix_ops/inv.hpp
--rw-rw-rw-   0        0        0     1263 2021-04-01 05:49:27.000000 gpboost-1.2.1.1/compile/external_libs/OptimLib/misc/matrix_ops/is_finite.hpp
--rw-rw-rw-   0        0        0     1147 2021-04-01 05:49:27.000000 gpboost-1.2.1.1/compile/external_libs/OptimLib/misc/matrix_ops/log.hpp
--rw-rw-rw-   0        0        0     1557 2021-04-01 05:49:27.000000 gpboost-1.2.1.1/compile/external_libs/OptimLib/misc/matrix_ops/max.hpp
--rw-rw-rw-   0        0        0     1502 2021-04-01 05:49:27.000000 gpboost-1.2.1.1/compile/external_libs/OptimLib/misc/matrix_ops/min.hpp
--rw-rw-rw-   0        0        0     1132 2021-04-01 05:49:27.000000 gpboost-1.2.1.1/compile/external_libs/OptimLib/misc/matrix_ops/ncol.hpp
--rw-rw-rw-   0        0        0     1748 2021-04-01 05:49:27.000000 gpboost-1.2.1.1/compile/external_libs/OptimLib/misc/matrix_ops/norm.hpp
--rw-rw-rw-   0        0        0     1432 2021-04-01 05:49:27.000000 gpboost-1.2.1.1/compile/external_libs/OptimLib/misc/matrix_ops/ones.hpp
--rw-rw-rw-   0        0        0     1154 2021-04-01 05:49:27.000000 gpboost-1.2.1.1/compile/external_libs/OptimLib/misc/matrix_ops/pow.hpp
--rw-rw-rw-   0        0        0     1833 2021-04-01 05:49:27.000000 gpboost-1.2.1.1/compile/external_libs/OptimLib/misc/matrix_ops/randi.hpp
--rw-rw-rw-   0        0        0     2125 2021-04-11 01:02:01.000000 gpboost-1.2.1.1/compile/external_libs/OptimLib/misc/matrix_ops/randn.hpp
--rw-rw-rw-   0        0        0     1594 2021-04-01 05:49:27.000000 gpboost-1.2.1.1/compile/external_libs/OptimLib/misc/matrix_ops/randu.hpp
--rw-rw-rw-   0        0        0     1525 2021-04-01 05:49:27.000000 gpboost-1.2.1.1/compile/external_libs/OptimLib/misc/matrix_ops/reset_negative_values.hpp
--rw-rw-rw-   0        0        0     1312 2021-04-01 05:49:27.000000 gpboost-1.2.1.1/compile/external_libs/OptimLib/misc/matrix_ops/set_size.hpp
--rw-rw-rw-   0        0        0     1174 2021-04-01 05:49:27.000000 gpboost-1.2.1.1/compile/external_libs/OptimLib/misc/matrix_ops/size.hpp
--rw-rw-rw-   0        0        0     1208 2021-04-01 05:49:27.000000 gpboost-1.2.1.1/compile/external_libs/OptimLib/misc/matrix_ops/solve.hpp
--rw-rw-rw-   0        0        0     1152 2021-04-01 05:49:27.000000 gpboost-1.2.1.1/compile/external_libs/OptimLib/misc/matrix_ops/sqrt.hpp
--rw-rw-rw-   0        0        0     1506 2021-04-01 05:49:27.000000 gpboost-1.2.1.1/compile/external_libs/OptimLib/misc/matrix_ops/sum.hpp
--rw-rw-rw-   0        0        0     1310 2021-04-01 05:49:27.000000 gpboost-1.2.1.1/compile/external_libs/OptimLib/misc/matrix_ops/transpose.hpp
--rw-rw-rw-   0        0        0     1442 2021-04-01 05:49:27.000000 gpboost-1.2.1.1/compile/external_libs/OptimLib/misc/matrix_ops/zeros.hpp
--rw-rw-rw-   0        0        0     1129 2021-04-01 05:49:27.000000 gpboost-1.2.1.1/compile/external_libs/OptimLib/misc/misc.hpp
--rw-rw-rw-   0        0        0     2220 2021-04-01 05:49:27.000000 gpboost-1.2.1.1/compile/external_libs/OptimLib/misc/numerical_gradient.hpp
--rw-rw-rw-   0        0        0     3957 2021-04-01 05:49:27.000000 gpboost-1.2.1.1/compile/external_libs/OptimLib/misc/numerical_hessian.hpp
--rw-rw-rw-   0        0        0     2228 2021-04-01 05:49:27.000000 gpboost-1.2.1.1/compile/external_libs/OptimLib/misc/optim_matdefs.hpp
--rw-rw-rw-   0        0        0     3152 2021-04-01 05:49:27.000000 gpboost-1.2.1.1/compile/external_libs/OptimLib/misc/optim_options.hpp
--rw-rw-rw-   0        0        0     5754 2021-04-01 05:49:27.000000 gpboost-1.2.1.1/compile/external_libs/OptimLib/misc/optim_structs.hpp
--rw-rw-rw-   0        0        0    38503 2021-04-01 05:49:27.000000 gpboost-1.2.1.1/compile/external_libs/OptimLib/misc/optim_trace.hpp
--rw-rw-rw-   0        0        0     4071 2021-04-01 05:49:27.000000 gpboost-1.2.1.1/compile/external_libs/OptimLib/misc/transform_vals.hpp
--rw-rw-rw-   0        0        0     1106 2021-04-01 05:49:27.000000 gpboost-1.2.1.1/compile/external_libs/OptimLib/misc/unit_vec.hpp
--rw-rw-rw-   0        0        0     1082 2021-04-01 05:49:27.000000 gpboost-1.2.1.1/compile/external_libs/OptimLib/misc/unit_vec.ipp
--rw-rw-rw-   0        0        0     2062 2022-05-16 08:23:28.000000 gpboost-1.2.1.1/compile/external_libs/OptimLib/optim.hpp
-drwxrwxrwx   0        0        0        0 2023-06-19 06:52:41.024520 gpboost-1.2.1.1/compile/external_libs/OptimLib/unconstrained/
--rw-rw-rw-   0        0        0    10816 2022-05-16 08:34:45.000000 gpboost-1.2.1.1/compile/external_libs/OptimLib/unconstrained/bfgs.hpp
--rw-rw-rw-   0        0        0    11427 2021-04-01 05:49:27.000000 gpboost-1.2.1.1/compile/external_libs/OptimLib/unconstrained/cg.hpp
--rw-rw-rw-   0        0        0    10693 2021-04-01 05:49:27.000000 gpboost-1.2.1.1/compile/external_libs/OptimLib/unconstrained/de.hpp
--rw-rw-rw-   0        0        0    15780 2021-04-01 05:49:27.000000 gpboost-1.2.1.1/compile/external_libs/OptimLib/unconstrained/de_prmm.hpp
--rw-rw-rw-   0        0        0     9250 2022-08-16 12:43:27.000000 gpboost-1.2.1.1/compile/external_libs/OptimLib/unconstrained/gd.hpp
--rw-rw-rw-   0        0        0     7776 2022-06-08 13:34:35.000000 gpboost-1.2.1.1/compile/external_libs/OptimLib/unconstrained/gd.ipp
--rw-rw-rw-   0        0        0     9955 2021-04-01 05:49:28.000000 gpboost-1.2.1.1/compile/external_libs/OptimLib/unconstrained/lbfgs.hpp
--rw-rw-rw-   0        0        0     6505 2021-04-01 05:49:28.000000 gpboost-1.2.1.1/compile/external_libs/OptimLib/unconstrained/newton.hpp
--rw-rw-rw-   0        0        0    14178 2022-05-11 15:58:43.000000 gpboost-1.2.1.1/compile/external_libs/OptimLib/unconstrained/nm.hpp
--rw-rw-rw-   0        0        0    11188 2021-04-01 05:49:28.000000 gpboost-1.2.1.1/compile/external_libs/OptimLib/unconstrained/pso.hpp
--rw-rw-rw-   0        0        0    10573 2021-04-01 05:49:28.000000 gpboost-1.2.1.1/compile/external_libs/OptimLib/unconstrained/pso_dv.hpp
-drwxrwxrwx   0        0        0        0 2023-06-19 06:52:41.025513 gpboost-1.2.1.1/compile/external_libs/OptimLib/zeros/
--rw-rw-rw-   0        0        0    13567 2021-04-01 05:49:28.000000 gpboost-1.2.1.1/compile/external_libs/OptimLib/zeros/broyden.hpp
--rw-rw-rw-   0        0        0    16983 2021-04-01 05:49:28.000000 gpboost-1.2.1.1/compile/external_libs/OptimLib/zeros/broyden_df.hpp
-drwxrwxrwx   0        0        0        0 2023-06-19 06:52:41.026517 gpboost-1.2.1.1/compile/external_libs/compute/
--rw-rw-rw-   0        0        0     4455 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/CMakeLists.txt
-drwxrwxrwx   0        0        0        0 2023-06-19 06:52:41.029537 gpboost-1.2.1.1/compile/external_libs/compute/cmake/
--rw-rw-rw-   0        0        0      253 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/cmake/BoostComputeConfig.cmake.in
--rw-rw-rw-   0        0        0     5760 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/cmake/FindBolt.cmake
--rw-rw-rw-   0        0        0     7541 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/cmake/FindEigen.cmake
--rw-rw-rw-   0        0        0    13242 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/cmake/FindTBB.cmake
-drwxrwxrwx   0        0        0        0 2023-06-19 06:52:41.030472 gpboost-1.2.1.1/compile/external_libs/compute/cmake/opencl/
--rw-rw-rw-   0        0        0     3395 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/cmake/opencl/FindOpenCL.cmake
-drwxrwxrwx   0        0        0        0 2023-06-19 06:52:40.963035 gpboost-1.2.1.1/compile/external_libs/compute/include/
-drwxrwxrwx   0        0        0        0 2023-06-19 06:52:41.030472 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/
-drwxrwxrwx   0        0        0        0 2023-06-19 06:52:41.050511 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/
-drwxrwxrwx   0        0        0        0 2023-06-19 06:52:41.091504 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/
--rw-rw-rw-   0        0        0     6568 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/accumulate.hpp
--rw-rw-rw-   0        0        0     4542 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/adjacent_difference.hpp
--rw-rw-rw-   0        0        0     5482 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/adjacent_find.hpp
--rw-rw-rw-   0        0        0     1469 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/all_of.hpp
--rw-rw-rw-   0        0        0     1590 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/any_of.hpp
--rw-rw-rw-   0        0        0     1523 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/binary_search.hpp
--rw-rw-rw-   0        0        0    32364 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/copy.hpp
--rw-rw-rw-   0        0        0     2641 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/copy_if.hpp
--rw-rw-rw-   0        0        0     1995 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/copy_n.hpp
--rw-rw-rw-   0        0        0     2165 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/count.hpp
--rw-rw-rw-   0        0        0     2457 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/count_if.hpp
-drwxrwxrwx   0        0        0        0 2023-06-19 06:52:41.110474 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/detail/
--rw-rw-rw-   0        0        0     6429 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/detail/balanced_path.hpp
--rw-rw-rw-   0        0        0     4759 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/detail/binary_find.hpp
--rw-rw-rw-   0        0        0     2265 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/detail/compact.hpp
--rw-rw-rw-   0        0        0     7581 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/detail/copy_on_device.hpp
--rw-rw-rw-   0        0        0     6935 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/detail/copy_to_device.hpp
--rw-rw-rw-   0        0        0     6865 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/detail/copy_to_host.hpp
--rw-rw-rw-   0        0        0     2683 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/detail/count_if_with_ballot.hpp
--rw-rw-rw-   0        0        0     2735 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/detail/count_if_with_reduce.hpp
--rw-rw-rw-   0        0        0     4370 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/detail/count_if_with_threads.hpp
--rw-rw-rw-   0        0        0     2511 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/detail/find_extrema.hpp
--rw-rw-rw-   0        0        0     5471 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/detail/find_extrema_on_cpu.hpp
--rw-rw-rw-   0        0        0     4359 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/detail/find_extrema_with_atomics.hpp
--rw-rw-rw-   0        0        0    19116 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/detail/find_extrema_with_reduce.hpp
--rw-rw-rw-   0        0        0     8722 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/detail/find_if_with_atomics.hpp
--rw-rw-rw-   0        0        0     4975 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/detail/inplace_reduce.hpp
--rw-rw-rw-   0        0        0     6195 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/detail/insertion_sort.hpp
--rw-rw-rw-   0        0        0     3990 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/detail/merge_path.hpp
--rw-rw-rw-   0        0        0    15020 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/detail/merge_sort_on_cpu.hpp
--rw-rw-rw-   0        0        0    22695 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/detail/merge_sort_on_gpu.hpp
--rw-rw-rw-   0        0        0     7542 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/detail/merge_with_merge_path.hpp
--rw-rw-rw-   0        0        0    15971 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/detail/radix_sort.hpp
--rw-rw-rw-   0        0        0     1937 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/detail/random_fill.hpp
--rw-rw-rw-   0        0        0     5362 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/detail/reduce_by_key.hpp
--rw-rw-rw-   0        0        0    24276 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/detail/reduce_by_key_with_scan.hpp
--rw-rw-rw-   0        0        0     4059 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/detail/reduce_on_cpu.hpp
--rw-rw-rw-   0        0        0    10677 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/detail/reduce_on_gpu.hpp
--rw-rw-rw-   0        0        0     1590 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/detail/scan.hpp
--rw-rw-rw-   0        0        0     7261 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/detail/scan_on_cpu.hpp
--rw-rw-rw-   0        0        0    11650 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/detail/scan_on_gpu.hpp
--rw-rw-rw-   0        0        0     2665 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/detail/search_all.hpp
--rw-rw-rw-   0        0        0     2046 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/detail/serial_accumulate.hpp
--rw-rw-rw-   0        0        0     2311 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/detail/serial_count_if.hpp
--rw-rw-rw-   0        0        0     3238 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/detail/serial_find_extrema.hpp
--rw-rw-rw-   0        0        0     3601 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/detail/serial_merge.hpp
--rw-rw-rw-   0        0        0     2208 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/detail/serial_reduce.hpp
--rw-rw-rw-   0        0        0     4346 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/detail/serial_reduce_by_key.hpp
--rw-rw-rw-   0        0        0     3287 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/detail/serial_scan.hpp
--rw-rw-rw-   0        0        0     2271 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/equal.hpp
--rw-rw-rw-   0        0        0     1684 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/equal_range.hpp
--rw-rw-rw-   0        0        0     4151 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/exclusive_scan.hpp
--rw-rw-rw-   0        0        0    10343 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/fill.hpp
--rw-rw-rw-   0        0        0     1409 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/fill_n.hpp
--rw-rw-rw-   0        0        0     2067 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/find.hpp
--rw-rw-rw-   0        0        0     4916 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/find_end.hpp
--rw-rw-rw-   0        0        0     1545 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/find_if.hpp
--rw-rw-rw-   0        0        0     1701 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/find_if_not.hpp
--rw-rw-rw-   0        0        0     2203 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/for_each.hpp
--rw-rw-rw-   0        0        0     1464 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/for_each_n.hpp
--rw-rw-rw-   0        0        0     2887 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/gather.hpp
--rw-rw-rw-   0        0        0     1958 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/generate.hpp
--rw-rw-rw-   0        0        0     1314 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/generate_n.hpp
--rw-rw-rw-   0        0        0     5777 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/includes.hpp
--rw-rw-rw-   0        0        0     3494 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/inclusive_scan.hpp
--rw-rw-rw-   0        0        0     3952 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/inner_product.hpp
--rw-rw-rw-   0        0        0     2113 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/inplace_merge.hpp
--rw-rw-rw-   0        0        0     1789 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/iota.hpp
--rw-rw-rw-   0        0        0     1834 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/is_partitioned.hpp
--rw-rw-rw-   0        0        0     2817 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/is_permutation.hpp
--rw-rw-rw-   0        0        0     2507 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/is_sorted.hpp
--rw-rw-rw-   0        0        0     5076 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/lexicographical_compare.hpp
--rw-rw-rw-   0        0        0     1623 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/lower_bound.hpp
--rw-rw-rw-   0        0        0     2863 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/max_element.hpp
--rw-rw-rw-   0        0        0     5153 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/merge.hpp
--rw-rw-rw-   0        0        0     2862 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/min_element.hpp
--rw-rw-rw-   0        0        0     2746 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/minmax_element.hpp
--rw-rw-rw-   0        0        0     3507 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/mismatch.hpp
--rw-rw-rw-   0        0        0     5878 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/next_permutation.hpp
--rw-rw-rw-   0        0        0     1468 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/none_of.hpp
--rw-rw-rw-   0        0        0     2962 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/nth_element.hpp
--rw-rw-rw-   0        0        0     1722 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/partial_sum.hpp
--rw-rw-rw-   0        0        0     1568 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/partition.hpp
--rw-rw-rw-   0        0        0     2664 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/partition_copy.hpp
--rw-rw-rw-   0        0        0     1910 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/partition_point.hpp
--rw-rw-rw-   0        0        0     5870 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/prev_permutation.hpp
--rw-rw-rw-   0        0        0     3100 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/random_shuffle.hpp
--rw-rw-rw-   0        0        0    11764 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/reduce.hpp
--rw-rw-rw-   0        0        0     6070 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/reduce_by_key.hpp
--rw-rw-rw-   0        0        0     2062 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/remove.hpp
--rw-rw-rw-   0        0        0     1903 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/remove_if.hpp
--rw-rw-rw-   0        0        0     2684 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/replace.hpp
--rw-rw-rw-   0        0        0     2300 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/replace_copy.hpp
--rw-rw-rw-   0        0        0     2518 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/reverse.hpp
--rw-rw-rw-   0        0        0     2765 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/reverse_copy.hpp
--rw-rw-rw-   0        0        0     1869 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/rotate.hpp
--rw-rw-rw-   0        0        0     1572 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/rotate_copy.hpp
--rw-rw-rw-   0        0        0     3542 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/scatter.hpp
--rw-rw-rw-   0        0        0     4861 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/scatter_if.hpp
--rw-rw-rw-   0        0        0     3047 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/search.hpp
--rw-rw-rw-   0        0        0     4574 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/search_n.hpp
--rw-rw-rw-   0        0        0     7132 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/set_difference.hpp
--rw-rw-rw-   0        0        0     6825 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/set_intersection.hpp
--rw-rw-rw-   0        0        0     7737 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/set_symmetric_difference.hpp
--rw-rw-rw-   0        0        0     7588 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/set_union.hpp
--rw-rw-rw-   0        0        0     6776 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/sort.hpp
--rw-rw-rw-   0        0        0     6324 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/sort_by_key.hpp
--rw-rw-rw-   0        0        0     2815 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/stable_partition.hpp
--rw-rw-rw-   0        0        0     3924 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/stable_sort.hpp
--rw-rw-rw-   0        0        0     6239 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/stable_sort_by_key.hpp
--rw-rw-rw-   0        0        0     1922 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/swap_ranges.hpp
--rw-rw-rw-   0        0        0     3339 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/transform.hpp
--rw-rw-rw-   0        0        0     4860 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/transform_if.hpp
--rw-rw-rw-   0        0        0     3783 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/transform_reduce.hpp
--rw-rw-rw-   0        0        0     2638 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/unique.hpp
--rw-rw-rw-   0        0        0     6604 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/unique_copy.hpp
--rw-rw-rw-   0        0        0     1610 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/upper_bound.hpp
--rw-rw-rw-   0        0        0     4493 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm.hpp
-drwxrwxrwx   0        0        0        0 2023-06-19 06:52:41.110474 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/allocator/
--rw-rw-rw-   0        0        0     3108 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/allocator/buffer_allocator.hpp
--rw-rw-rw-   0        0        0     1445 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/allocator/pinned_allocator.hpp
--rw-rw-rw-   0        0        0      769 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/allocator.hpp
-drwxrwxrwx   0        0        0        0 2023-06-19 06:52:41.112442 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/async/
--rw-rw-rw-   0        0        0     4178 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/async/future.hpp
--rw-rw-rw-   0        0        0     1708 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/async/wait.hpp
--rw-rw-rw-   0        0        0     1925 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/async/wait_guard.hpp
--rw-rw-rw-   0        0        0      724 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/async.hpp
--rw-rw-rw-   0        0        0     7010 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/buffer.hpp
--rw-rw-rw-   0        0        0     1677 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/cl.hpp
--rw-rw-rw-   0        0        0      686 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/cl_ext.hpp
--rw-rw-rw-   0        0        0    10458 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/closure.hpp
--rw-rw-rw-   0        0        0    64508 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/command_queue.hpp
--rw-rw-rw-   0        0        0     2425 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/config.hpp
-drwxrwxrwx   0        0        0        0 2023-06-19 06:52:41.117476 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/container/
--rw-rw-rw-   0        0        0     7987 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/container/array.hpp
--rw-rw-rw-   0        0        0     8185 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/container/basic_string.hpp
-drwxrwxrwx   0        0        0        0 2023-06-19 06:52:41.117476 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/container/detail/
--rw-rw-rw-   0        0        0     1569 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/container/detail/scalar.hpp
--rw-rw-rw-   0        0        0     7089 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/container/dynamic_bitset.hpp
--rw-rw-rw-   0        0        0    11201 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/container/flat_map.hpp
--rw-rw-rw-   0        0        0     8698 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/container/flat_set.hpp
--rw-rw-rw-   0        0        0     7160 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/container/mapped_view.hpp
--rw-rw-rw-   0        0        0     1668 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/container/stack.hpp
--rw-rw-rw-   0        0        0      826 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/container/string.hpp
--rw-rw-rw-   0        0        0    17204 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/container/valarray.hpp
--rw-rw-rw-   0        0        0    24764 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/container/vector.hpp
--rw-rw-rw-   0        0        0     1048 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/container.hpp
--rw-rw-rw-   0        0        0     6839 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/context.hpp
--rw-rw-rw-   0        0        0     1174 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/core.hpp
-drwxrwxrwx   0        0        0        0 2023-06-19 06:52:41.131442 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/detail/
--rw-rw-rw-   0        0        0      875 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/detail/assert_cl_success.hpp
--rw-rw-rw-   0        0        0     4242 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/detail/buffer_value.hpp
--rw-rw-rw-   0        0        0     3194 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/detail/cl_versions.hpp
--rw-rw-rw-   0        0        0     5609 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/detail/device_ptr.hpp
--rw-rw-rw-   0        0        0     5308 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/detail/diagnostic.hpp
--rw-rw-rw-   0        0        0     1695 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/detail/duration.hpp
--rw-rw-rw-   0        0        0     8600 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/detail/get_object_info.hpp
--rw-rw-rw-   0        0        0      972 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/detail/getenv.hpp
--rw-rw-rw-   0        0        0     1474 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/detail/global_static.hpp
--rw-rw-rw-   0        0        0      990 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/detail/is_buffer_iterator.hpp
--rw-rw-rw-   0        0        0     3838 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/detail/is_contiguous_iterator.hpp
--rw-rw-rw-   0        0        0     1715 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/detail/iterator_plus_distance.hpp
--rw-rw-rw-   0        0        0     1458 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/detail/iterator_range_size.hpp
--rw-rw-rw-   0        0        0     1193 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/detail/iterator_traits.hpp
--rw-rw-rw-   0        0        0     1497 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/detail/literal.hpp
--rw-rw-rw-   0        0        0     3606 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/detail/lru_cache.hpp
--rw-rw-rw-   0        0        0    33188 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/detail/meta_kernel.hpp
--rw-rw-rw-   0        0        0     2335 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/detail/mpl_vector_to_tuple.hpp
--rw-rw-rw-   0        0        0     2134 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/detail/nvidia_compute_capability.hpp
--rw-rw-rw-   0        0        0     7414 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/detail/parameter_cache.hpp
--rw-rw-rw-   0        0        0     2173 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/detail/path.hpp
--rw-rw-rw-   0        0        0     2670 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/detail/print_range.hpp
--rw-rw-rw-   0        0        0     2620 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/detail/read_write_single_value.hpp
--rw-rw-rw-   0        0        0     1603 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/detail/sha1.hpp
--rw-rw-rw-   0        0        0     1871 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/detail/variadic_macros.hpp
--rw-rw-rw-   0        0        0     1541 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/detail/vendor.hpp
--rw-rw-rw-   0        0        0     1279 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/detail/work_size.hpp
--rw-rw-rw-   0        0        0    21876 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/device.hpp
--rw-rw-rw-   0        0        0    10618 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/event.hpp
-drwxrwxrwx   0        0        0        0 2023-06-19 06:52:41.134478 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/exception/
--rw-rw-rw-   0        0        0     2663 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/exception/context_error.hpp
--rw-rw-rw-   0        0        0     1369 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/exception/no_device_found.hpp
--rw-rw-rw-   0        0        0     6865 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/exception/opencl_error.hpp
--rw-rw-rw-   0        0        0     1765 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/exception/program_build_failure.hpp
--rw-rw-rw-   0        0        0     2271 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/exception/unsupported_extension_error.hpp
--rw-rw-rw-   0        0        0      881 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/exception.hpp
-drwxrwxrwx   0        0        0        0 2023-06-19 06:52:41.136442 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/experimental/
--rw-rw-rw-   0        0        0     1517 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/experimental/clamp_range.hpp
--rw-rw-rw-   0        0        0     1500 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/experimental/malloc.hpp
--rw-rw-rw-   0        0        0     2055 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/experimental/sort_by_transform.hpp
--rw-rw-rw-   0        0        0     1380 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/experimental/tabulate.hpp
--rw-rw-rw-   0        0        0    12605 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/function.hpp
-drwxrwxrwx   0        0        0        0 2023-06-19 06:52:41.144442 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/functional/
--rw-rw-rw-   0        0        0     1251 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/functional/as.hpp
--rw-rw-rw-   0        0        0     3090 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/functional/atomic.hpp
--rw-rw-rw-   0        0        0     7491 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/functional/bind.hpp
--rw-rw-rw-   0        0        0     1146 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/functional/common.hpp
--rw-rw-rw-   0        0        0     1281 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/functional/convert.hpp
-drwxrwxrwx   0        0        0        0 2023-06-19 06:52:41.146490 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/functional/detail/
--rw-rw-rw-   0        0        0     1291 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/functional/detail/macros.hpp
--rw-rw-rw-   0        0        0     1483 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/functional/detail/nvidia_ballot.hpp
--rw-rw-rw-   0        0        0     1268 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/functional/detail/nvidia_popcount.hpp
--rw-rw-rw-   0        0        0     4349 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/functional/detail/unpack.hpp
--rw-rw-rw-   0        0        0     2183 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/functional/field.hpp
--rw-rw-rw-   0        0        0     1479 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/functional/geometry.hpp
--rw-rw-rw-   0        0        0     1959 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/functional/get.hpp
--rw-rw-rw-   0        0        0     2664 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/functional/hash.hpp
--rw-rw-rw-   0        0        0     1617 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/functional/identity.hpp
--rw-rw-rw-   0        0        0     1206 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/functional/integer.hpp
--rw-rw-rw-   0        0        0     4931 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/functional/logical.hpp
--rw-rw-rw-   0        0        0     4361 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/functional/math.hpp
--rw-rw-rw-   0        0        0     3173 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/functional/operator.hpp
--rw-rw-rw-   0        0        0     1857 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/functional/popcount.hpp
--rw-rw-rw-   0        0        0     2022 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/functional/relational.hpp
--rw-rw-rw-   0        0        0     1377 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/functional.hpp
-drwxrwxrwx   0        0        0        0 2023-06-19 06:52:41.149470 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/image/
--rw-rw-rw-   0        0        0     5859 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/image/image1d.hpp
--rw-rw-rw-   0        0        0     8038 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/image/image2d.hpp
--rw-rw-rw-   0        0        0     8315 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/image/image3d.hpp
--rw-rw-rw-   0        0        0     4125 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/image/image_format.hpp
--rw-rw-rw-   0        0        0     4810 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/image/image_object.hpp
--rw-rw-rw-   0        0        0     6334 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/image/image_sampler.hpp
--rw-rw-rw-   0        0        0      919 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/image.hpp
--rw-rw-rw-   0        0        0      561 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/image2d.hpp
--rw-rw-rw-   0        0        0      561 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/image3d.hpp
--rw-rw-rw-   0        0        0      571 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/image_format.hpp
--rw-rw-rw-   0        0        0      573 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/image_sampler.hpp
-drwxrwxrwx   0        0        0        0 2023-06-19 06:52:41.151442 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/interop/
-drwxrwxrwx   0        0        0        0 2023-06-19 06:52:41.152442 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/interop/eigen/
--rw-rw-rw-   0        0        0     2738 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/interop/eigen/core.hpp
--rw-rw-rw-   0        0        0      633 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/interop/eigen.hpp
-drwxrwxrwx   0        0        0        0 2023-06-19 06:52:41.153443 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/interop/opencv/
--rw-rw-rw-   0        0        0     4886 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/interop/opencv/core.hpp
--rw-rw-rw-   0        0        0     1092 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/interop/opencv/highgui.hpp
--rw-rw-rw-   0        0        0     1433 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/interop/opencv/ocl.hpp
--rw-rw-rw-   0        0        0      690 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/interop/opencv.hpp
-drwxrwxrwx   0        0        0        0 2023-06-19 06:52:41.158443 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/interop/opengl/
--rw-rw-rw-   0        0        0     3851 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/interop/opengl/acquire.hpp
--rw-rw-rw-   0        0        0      745 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/interop/opengl/cl_gl.hpp
--rw-rw-rw-   0        0        0      765 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/interop/opengl/cl_gl_ext.hpp
--rw-rw-rw-   0        0        0     4704 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/interop/opengl/context.hpp
--rw-rw-rw-   0        0        0      679 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/interop/opengl/gl.hpp
--rw-rw-rw-   0        0        0     2934 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/interop/opengl/opengl_buffer.hpp
--rw-rw-rw-   0        0        0     3767 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/interop/opengl/opengl_renderbuffer.hpp
--rw-rw-rw-   0        0        0     4075 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/interop/opengl/opengl_texture.hpp
--rw-rw-rw-   0        0        0      965 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/interop/opengl.hpp
-drwxrwxrwx   0        0        0        0 2023-06-19 06:52:41.161443 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/interop/qt/
--rw-rw-rw-   0        0        0     2242 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/interop/qt/qimage.hpp
--rw-rw-rw-   0        0        0      712 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/interop/qt/qpoint.hpp
--rw-rw-rw-   0        0        0      719 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/interop/qt/qpointf.hpp
--rw-rw-rw-   0        0        0      742 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/interop/qt/qtcore.hpp
--rw-rw-rw-   0        0        0      641 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/interop/qt/qtgui.hpp
--rw-rw-rw-   0        0        0     1430 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/interop/qt/qvector.hpp
--rw-rw-rw-   0        0        0      670 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/interop/qt.hpp
-drwxrwxrwx   0        0        0        0 2023-06-19 06:52:41.163442 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/interop/vtk/
--rw-rw-rw-   0        0        0     2113 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/interop/vtk/bounds.hpp
--rw-rw-rw-   0        0        0     2742 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/interop/vtk/data_array.hpp
--rw-rw-rw-   0        0        0     1339 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/interop/vtk/matrix4x4.hpp
--rw-rw-rw-   0        0        0     1896 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/interop/vtk/points.hpp
--rw-rw-rw-   0        0        0      781 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/interop/vtk.hpp
-drwxrwxrwx   0        0        0        0 2023-06-19 06:52:41.168443 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/iterator/
--rw-rw-rw-   0        0        0     8565 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/iterator/buffer_iterator.hpp
--rw-rw-rw-   0        0        0     5785 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/iterator/constant_buffer_iterator.hpp
--rw-rw-rw-   0        0        0     4415 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/iterator/constant_iterator.hpp
--rw-rw-rw-   0        0        0     4787 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/iterator/counting_iterator.hpp
-drwxrwxrwx   0        0        0        0 2023-06-19 06:52:41.169442 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/iterator/detail/
--rw-rw-rw-   0        0        0     1726 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/iterator/detail/get_base_iterator_buffer.hpp
--rw-rw-rw-   0        0        0     6076 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/iterator/detail/swizzle_iterator.hpp
--rw-rw-rw-   0        0        0     4078 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/iterator/discard_iterator.hpp
--rw-rw-rw-   0        0        0     5169 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/iterator/function_input_iterator.hpp
--rw-rw-rw-   0        0        0     6505 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/iterator/permutation_iterator.hpp
--rw-rw-rw-   0        0        0     9894 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/iterator/strided_iterator.hpp
--rw-rw-rw-   0        0        0     7979 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/iterator/transform_iterator.hpp
--rw-rw-rw-   0        0        0    10751 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/iterator/zip_iterator.hpp
--rw-rw-rw-   0        0        0     1168 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/iterator.hpp
--rw-rw-rw-   0        0        0    18118 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/kernel.hpp
-drwxrwxrwx   0        0        0        0 2023-06-19 06:52:41.175442 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/lambda/
--rw-rw-rw-   0        0        0    11279 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/lambda/context.hpp
--rw-rw-rw-   0        0        0    25620 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/lambda/functional.hpp
--rw-rw-rw-   0        0        0     4373 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/lambda/get.hpp
--rw-rw-rw-   0        0        0     2302 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/lambda/make_pair.hpp
--rw-rw-rw-   0        0        0     5041 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/lambda/make_tuple.hpp
--rw-rw-rw-   0        0        0      816 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/lambda/placeholder.hpp
--rw-rw-rw-   0        0        0     2589 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/lambda/placeholders.hpp
--rw-rw-rw-   0        0        0     4232 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/lambda/result_of.hpp
--rw-rw-rw-   0        0        0      884 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/lambda.hpp
-drwxrwxrwx   0        0        0        0 2023-06-19 06:52:41.176442 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/memory/
--rw-rw-rw-   0        0        0     2343 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/memory/local_buffer.hpp
--rw-rw-rw-   0        0        0     4630 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/memory/svm_ptr.hpp
--rw-rw-rw-   0        0        0      738 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/memory.hpp
--rw-rw-rw-   0        0        0     7258 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/memory_object.hpp
--rw-rw-rw-   0        0        0     4162 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/pipe.hpp
--rw-rw-rw-   0        0        0     7678 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/platform.hpp
--rw-rw-rw-   0        0        0    26141 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/program.hpp
-drwxrwxrwx   0        0        0        0 2023-06-19 06:52:41.181443 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/random/
--rw-rw-rw-   0        0        0     3068 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/random/bernoulli_distribution.hpp
--rw-rw-rw-   0        0        0      825 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/random/default_random_engine.hpp
--rw-rw-rw-   0        0        0     5557 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/random/discrete_distribution.hpp
--rw-rw-rw-   0        0        0     7736 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/random/linear_congruential_engine.hpp
--rw-rw-rw-   0        0        0     8542 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/random/mersenne_twister_engine.hpp
--rw-rw-rw-   0        0        0     4782 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/random/normal_distribution.hpp
--rw-rw-rw-   0        0        0    14255 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/random/threefry_engine.hpp
--rw-rw-rw-   0        0        0     3717 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/random/uniform_int_distribution.hpp
--rw-rw-rw-   0        0        0     3590 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/random/uniform_real_distribution.hpp
--rw-rw-rw-   0        0        0     1176 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/random.hpp
--rw-rw-rw-   0        0        0      563 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/source.hpp
--rw-rw-rw-   0        0        0     2041 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/svm.hpp
--rw-rw-rw-   0        0        0     9676 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/system.hpp
-drwxrwxrwx   0        0        0        0 2023-06-19 06:52:41.188443 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/type_traits/
--rw-rw-rw-   0        0        0     2253 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/type_traits/common_type.hpp
-drwxrwxrwx   0        0        0        0 2023-06-19 06:52:41.189442 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/type_traits/detail/
--rw-rw-rw-   0        0        0      992 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/type_traits/detail/capture_traits.hpp
--rw-rw-rw-   0        0        0     1390 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/type_traits/is_device_iterator.hpp
--rw-rw-rw-   0        0        0     2616 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/type_traits/is_fundamental.hpp
--rw-rw-rw-   0        0        0     1143 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/type_traits/is_vector_type.hpp
--rw-rw-rw-   0        0        0     2415 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/type_traits/make_vector_type.hpp
--rw-rw-rw-   0        0        0     1351 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/type_traits/result_of.hpp
--rw-rw-rw-   0        0        0     2438 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/type_traits/scalar_type.hpp
--rw-rw-rw-   0        0        0     1175 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/type_traits/type_definition.hpp
--rw-rw-rw-   0        0        0     3833 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/type_traits/type_name.hpp
--rw-rw-rw-   0        0        0     2258 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/type_traits/vector_size.hpp
--rw-rw-rw-   0        0        0     1131 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/type_traits.hpp
-drwxrwxrwx   0        0        0        0 2023-06-19 06:52:41.192442 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/types/
--rw-rw-rw-   0        0        0      569 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/types/builtin.hpp
--rw-rw-rw-   0        0        0     5102 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/types/complex.hpp
--rw-rw-rw-   0        0        0     6195 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/types/fundamental.hpp
--rw-rw-rw-   0        0        0     3294 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/types/pair.hpp
--rw-rw-rw-   0        0        0     1800 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/types/size_t.hpp
--rw-rw-rw-   0        0        0     5886 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/types/struct.hpp
--rw-rw-rw-   0        0        0     9023 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/types/tuple.hpp
--rw-rw-rw-   0        0        0      895 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/types.hpp
--rw-rw-rw-   0        0        0     2502 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/user_event.hpp
-drwxrwxrwx   0        0        0        0 2023-06-19 06:52:41.195442 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/utility/
--rw-rw-rw-   0        0        0     2262 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/utility/dim.hpp
--rw-rw-rw-   0        0        0     4040 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/utility/extents.hpp
--rw-rw-rw-   0        0        0     2857 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/utility/invoke.hpp
--rw-rw-rw-   0        0        0     5665 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/utility/program_cache.hpp
--rw-rw-rw-   0        0        0     1366 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/utility/source.hpp
--rw-rw-rw-   0        0        0     5956 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/utility/wait_list.hpp
--rw-rw-rw-   0        0        0      844 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/utility.hpp
--rw-rw-rw-   0        0        0      683 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/version.hpp
--rw-rw-rw-   0        0        0      569 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/wait_list.hpp
--rw-rw-rw-   0        0        0     1567 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute.hpp
-drwxrwxrwx   0        0        0        0 2023-06-19 06:52:41.195442 gpboost-1.2.1.1/compile/external_libs/compute/meta/
--rw-rw-rw-   0        0        0      282 2021-01-29 13:27:37.000000 gpboost-1.2.1.1/compile/external_libs/compute/meta/libraries.json
-drwxrwxrwx   0        0        0        0 2023-06-19 06:52:41.196442 gpboost-1.2.1.1/compile/external_libs/eigen/
--rw-rw-rw-   0        0        0    25206 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/CMakeLists.txt
-drwxrwxrwx   0        0        0        0 2023-06-19 06:52:41.204441 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/
--rw-rw-rw-   0        0        0     1206 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/Cholesky
--rw-rw-rw-   0        0        0    12843 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/Core
--rw-rw-rw-   0        0        0      129 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/Dense
--rw-rw-rw-   0        0        0     1837 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/Eigenvalues
--rw-rw-rw-   0        0        0     1999 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/Geometry
--rw-rw-rw-   0        0        0      858 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/Householder
--rw-rw-rw-   0        0        0     2131 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/IterativeLinearSolvers
--rw-rw-rw-   0        0        0      926 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/Jacobi
--rw-rw-rw-   0        0        0     1472 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/LU
--rw-rw-rw-   0        0        0     2521 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/OrderingMethods
--rw-rw-rw-   0        0        0     1322 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/QR
--rw-rw-rw-   0        0        0     1634 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/SVD
--rw-rw-rw-   0        0        0      922 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/Sparse
--rw-rw-rw-   0        0        0     1272 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/SparseCholesky
--rw-rw-rw-   0        0        0     2309 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/SparseCore
--rw-rw-rw-   0        0        0     1864 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/SparseLU
--rw-rw-rw-   0        0        0     1231 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/SparseQR
-drwxrwxrwx   0        0        0        0 2023-06-19 06:52:40.977038 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/
-drwxrwxrwx   0        0        0        0 2023-06-19 06:52:41.206442 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Cholesky/
--rw-rw-rw-   0        0        0    25560 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Cholesky/LDLT.h
--rw-rw-rw-   0        0        0    19398 2023-01-16 16:29:13.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Cholesky/LLT.h
--rw-rw-rw-   0        0        0     4073 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Cholesky/LLT_LAPACKE.h
-drwxrwxrwx   0        0        0        0 2023-06-19 06:52:41.243442 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/
--rw-rw-rw-   0        0        0    19627 2021-08-16 05:28:02.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/ArithmeticSequence.h
--rw-rw-rw-   0        0        0    17144 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/Array.h
--rw-rw-rw-   0        0        0     8443 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/ArrayBase.h
--rw-rw-rw-   0        0        0     6984 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/ArrayWrapper.h
--rw-rw-rw-   0        0        0     2828 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/Assign.h
--rw-rw-rw-   0        0        0    41938 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/AssignEvaluator.h
--rw-rw-rw-   0        0        0    12666 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/Assign_MKL.h
--rw-rw-rw-   0        0        0    14263 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/BandMatrix.h
--rw-rw-rw-   0        0        0    18852 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/Block.h
--rw-rw-rw-   0        0        0     4571 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/BooleanRedux.h
--rw-rw-rw-   0        0        0     6145 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/CommaInitializer.h
--rw-rw-rw-   0        0        0     7165 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/ConditionEstimator.h
--rw-rw-rw-   0        0        0    65712 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/CoreEvaluators.h
--rw-rw-rw-   0        0        0     4877 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/CoreIterators.h
--rw-rw-rw-   0        0        0     8131 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/CwiseBinaryOp.h
--rw-rw-rw-   0        0        0    37252 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/CwiseNullaryOp.h
--rw-rw-rw-   0        0        0     8453 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/CwiseTernaryOp.h
--rw-rw-rw-   0        0        0     3980 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/CwiseUnaryOp.h
--rw-rw-rw-   0        0        0     5583 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/CwiseUnaryView.h
--rw-rw-rw-   0        0        0    31179 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/DenseBase.h
--rw-rw-rw-   0        0        0    24905 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/DenseCoeffsBase.h
--rw-rw-rw-   0        0        0    23343 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/DenseStorage.h
--rw-rw-rw-   0        0        0     9967 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/Diagonal.h
--rw-rw-rw-   0        0        0    15061 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/DiagonalMatrix.h
--rw-rw-rw-   0        0        0     1016 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/DiagonalProduct.h
--rw-rw-rw-   0        0        0    11964 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/Dot.h
--rw-rw-rw-   0        0        0     5911 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/EigenBase.h
--rw-rw-rw-   0        0        0     4915 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/ForceAlignedAccess.h
--rw-rw-rw-   0        0        0     5914 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/Fuzzy.h
--rw-rw-rw-   0        0        0    22144 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/GeneralProduct.h
--rw-rw-rw-   0        0        0    35664 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/GenericPacketMath.h
--rw-rw-rw-   0        0        0    11737 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/GlobalFunctions.h
--rw-rw-rw-   0        0        0     8496 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/IO.h
--rw-rw-rw-   0        0        0     9857 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/IndexedView.h
--rw-rw-rw-   0        0        0     3566 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/Inverse.h
--rw-rw-rw-   0        0        0     7398 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/Map.h
--rw-rw-rw-   0        0        0    11520 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/MapBase.h
--rw-rw-rw-   0        0        0    60856 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/MathFunctions.h
--rw-rw-rw-   0        0        0     7092 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/MathFunctionsImpl.h
--rw-rw-rw-   0        0        0    24859 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/Matrix.h
--rw-rw-rw-   0        0        0    24403 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/MatrixBase.h
--rw-rw-rw-   0        0        0     2543 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/NestByValue.h
--rw-rw-rw-   0        0        0     3729 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/NoAlias.h
--rw-rw-rw-   0        0        0    11924 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/NumTraits.h
--rw-rw-rw-   0        0        0     9429 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/PartialReduxEvaluator.h
--rw-rw-rw-   0        0        0    21353 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/PermutationMatrix.h
--rw-rw-rw-   0        0        0    50200 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/PlainObjectBase.h
--rw-rw-rw-   0        0        0     7524 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/Product.h
--rw-rw-rw-   0        0        0    54996 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/ProductEvaluators.h
--rw-rw-rw-   0        0        0     7974 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/Random.h
--rw-rw-rw-   0        0        0    19685 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/Redux.h
--rw-rw-rw-   0        0        0    18392 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/Ref.h
--rw-rw-rw-   0        0        0     5773 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/Replicate.h
--rw-rw-rw-   0        0        0    17455 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/Reshaped.h
--rw-rw-rw-   0        0        0     4335 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/ReturnByValue.h
--rw-rw-rw-   0        0        0     7672 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/Reverse.h
--rw-rw-rw-   0        0        0     6236 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/Select.h
--rw-rw-rw-   0        0        0    15238 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/SelfAdjointView.h
--rw-rw-rw-   0        0        0     1744 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/SelfCwiseBinaryOp.h
--rw-rw-rw-   0        0        0     6985 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/Solve.h
--rw-rw-rw-   0        0        0     9514 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/SolveTriangular.h
--rw-rw-rw-   0        0        0     6338 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/SolverBase.h
--rw-rw-rw-   0        0        0     8974 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/StableNorm.h
--rw-rw-rw-   0        0        0    21903 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/StlIterators.h
--rw-rw-rw-   0        0        0     4299 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/Stride.h
--rw-rw-rw-   0        0        0     2833 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/Swap.h
--rw-rw-rw-   0        0        0    18010 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/Transpose.h
--rw-rw-rw-   0        0        0    13860 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/Transpositions.h
--rw-rw-rw-   0        0        0    39110 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/TriangularMatrix.h
--rw-rw-rw-   0        0        0     3584 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/VectorBlock.h
--rw-rw-rw-   0        0        0    35901 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/VectorwiseOp.h
--rw-rw-rw-   0        0        0     9613 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/Visitor.h
-drwxrwxrwx   0        0        0        0 2023-06-19 06:52:40.973037 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/arch/
-drwxrwxrwx   0        0        0        0 2023-06-19 06:52:41.245441 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/arch/AVX/
--rw-rw-rw-   0        0        0    17687 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/arch/AVX/Complex.h
--rw-rw-rw-   0        0        0     8330 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/arch/AVX/MathFunctions.h
--rw-rw-rw-   0        0        0    66422 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/arch/AVX/PacketMath.h
--rw-rw-rw-   0        0        0     2679 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/arch/AVX/TypeCasting.h
-drwxrwxrwx   0        0        0        0 2023-06-19 06:52:41.247442 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/arch/AVX512/
--rw-rw-rw-   0        0        0    18628 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/arch/AVX512/Complex.h
--rw-rw-rw-   0        0        0    16230 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/arch/AVX512/MathFunctions.h
--rw-rw-rw-   0        0        0    90467 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/arch/AVX512/PacketMath.h
--rw-rw-rw-   0        0        0     2223 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/arch/AVX512/TypeCasting.h
-drwxrwxrwx   0        0        0        0 2023-06-19 06:52:41.250442 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/arch/AltiVec/
--rw-rw-rw-   0        0        0    16847 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/arch/AltiVec/Complex.h
--rw-rw-rw-   0        0        0     2413 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/arch/AltiVec/MathFunctions.h
--rw-rw-rw-   0        0        0   120436 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/arch/AltiVec/MatrixProduct.h
--rw-rw-rw-   0        0        0     5908 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/arch/AltiVec/MatrixProductCommon.h
--rw-rw-rw-   0        0        0    31464 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/arch/AltiVec/MatrixProductMMA.h
--rw-rw-rw-   0        0        0   102544 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/arch/AltiVec/PacketMath.h
-drwxrwxrwx   0        0        0        0 2023-06-19 06:52:41.251442 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/arch/CUDA/
--rw-rw-rw-   0        0        0    16946 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/arch/CUDA/Complex.h
-drwxrwxrwx   0        0        0        0 2023-06-19 06:52:41.254442 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/arch/Default/
--rw-rw-rw-   0        0        0    27842 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/arch/Default/BFloat16.h
--rw-rw-rw-   0        0        0     2018 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/arch/Default/ConjHelper.h
--rw-rw-rw-   0        0        0    69591 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/arch/Default/GenericPacketMathFunctions.h
--rw-rw-rw-   0        0        0     4110 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/arch/Default/GenericPacketMathFunctionsFwd.h
--rw-rw-rw-   0        0        0    35763 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/arch/Default/Half.h
--rw-rw-rw-   0        0        0     1795 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/arch/Default/Settings.h
--rw-rw-rw-   0        0        0     3866 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/arch/Default/TypeCasting.h
-drwxrwxrwx   0        0        0        0 2023-06-19 06:52:41.256442 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/arch/GPU/
--rw-rw-rw-   0        0        0     2798 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/arch/GPU/MathFunctions.h
--rw-rw-rw-   0        0        0    58732 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/arch/GPU/PacketMath.h
--rw-rw-rw-   0        0        0     2336 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/arch/GPU/TypeCasting.h
-drwxrwxrwx   0        0        0        0 2023-06-19 06:52:40.972032 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/arch/HIP/
-drwxrwxrwx   0        0        0        0 2023-06-19 06:52:41.256442 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/arch/HIP/hcc/
--rw-rw-rw-   0        0        0      714 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/arch/HIP/hcc/math_constants.h
-drwxrwxrwx   0        0        0        0 2023-06-19 06:52:41.257442 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/arch/MSA/
--rw-rw-rw-   0        0        0    20551 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/arch/MSA/Complex.h
--rw-rw-rw-   0        0        0    16546 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/arch/MSA/MathFunctions.h
--rw-rw-rw-   0        0        0    34948 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/arch/MSA/PacketMath.h
-drwxrwxrwx   0        0        0        0 2023-06-19 06:52:41.260442 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/arch/NEON/
--rw-rw-rw-   0        0        0    26566 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/arch/NEON/Complex.h
--rw-rw-rw-   0        0        0     6998 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/arch/NEON/GeneralBlockPanelKernel.h
--rw-rw-rw-   0        0        0     3158 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/arch/NEON/MathFunctions.h
--rw-rw-rw-   0        0        0   200985 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/arch/NEON/PacketMath.h
--rw-rw-rw-   0        0        0    52705 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/arch/NEON/TypeCasting.h
-drwxrwxrwx   0        0        0        0 2023-06-19 06:52:41.262443 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/arch/SSE/
--rw-rw-rw-   0        0        0    19911 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/arch/SSE/Complex.h
--rw-rw-rw-   0        0        0     6964 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/arch/SSE/MathFunctions.h
--rw-rw-rw-   0        0        0    65976 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/arch/SSE/PacketMath.h
--rw-rw-rw-   0        0        0     3792 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/arch/SSE/TypeCasting.h
-drwxrwxrwx   0        0        0        0 2023-06-19 06:52:41.263443 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/arch/SVE/
--rw-rw-rw-   0        0        0     1238 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/arch/SVE/MathFunctions.h
--rw-rw-rw-   0        0        0    22052 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/arch/SVE/PacketMath.h
--rw-rw-rw-   0        0        0     1400 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/arch/SVE/TypeCasting.h
-drwxrwxrwx   0        0        0        0 2023-06-19 06:52:41.267442 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/arch/SYCL/
--rw-rw-rw-   0        0        0     7660 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/arch/SYCL/InteropHeaders.h
--rw-rw-rw-   0        0        0    12840 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/arch/SYCL/MathFunctions.h
--rw-rw-rw-   0        0        0    28456 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/arch/SYCL/PacketMath.h
--rw-rw-rw-   0        0        0    22550 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/arch/SYCL/SyclMemoryModel.h
--rw-rw-rw-   0        0        0     2711 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/arch/SYCL/TypeCasting.h
-drwxrwxrwx   0        0        0        0 2023-06-19 06:52:41.269442 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/arch/ZVector/
--rw-rw-rw-   0        0        0    20370 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/arch/ZVector/Complex.h
--rw-rw-rw-   0        0        0     8257 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/arch/ZVector/MathFunctions.h
--rw-rw-rw-   0        0        0    37940 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/arch/ZVector/PacketMath.h
-drwxrwxrwx   0        0        0        0 2023-06-19 06:52:41.271442 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/functors/
--rw-rw-rw-   0        0        0     6863 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/functors/AssignmentFunctors.h
--rw-rw-rw-   0        0        0    21424 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/functors/BinaryFunctors.h
--rw-rw-rw-   0        0        0     8523 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/functors/NullaryFunctors.h
--rw-rw-rw-   0        0        0     4481 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/functors/StlFunctors.h
--rw-rw-rw-   0        0        0      632 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/functors/TernaryFunctors.h
--rw-rw-rw-   0        0        0    41300 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/functors/UnaryFunctors.h
-drwxrwxrwx   0        0        0        0 2023-06-19 06:52:41.281442 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/products/
--rw-rw-rw-   0        0        0   112056 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/products/GeneralBlockPanelKernel.h
--rw-rw-rw-   0        0        0    20621 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/products/GeneralMatrixMatrix.h
--rw-rw-rw-   0        0        0    16265 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/products/GeneralMatrixMatrixTriangular.h
--rw-rw-rw-   0        0        0     7081 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/products/GeneralMatrixMatrixTriangular_BLAS.h
--rw-rw-rw-   0        0        0     5230 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/products/GeneralMatrixMatrix_BLAS.h
--rw-rw-rw-   0        0        0    22242 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/products/GeneralMatrixVector.h
--rw-rw-rw-   0        0        0     6504 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/products/GeneralMatrixVector_BLAS.h
--rw-rw-rw-   0        0        0     5762 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/products/Parallelizer.h
--rw-rw-rw-   0        0        0    21898 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/products/SelfadjointMatrixMatrix.h
--rw-rw-rw-   0        0        0    11865 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/products/SelfadjointMatrixMatrix_BLAS.h
--rw-rw-rw-   0        0        0    10220 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/products/SelfadjointMatrixVector.h
--rw-rw-rw-   0        0        0     5327 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/products/SelfadjointMatrixVector_BLAS.h
--rw-rw-rw-   0        0        0     6297 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/products/SelfadjointProduct.h
--rw-rw-rw-   0        0        0     4198 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/products/SelfadjointRank2Update.h
--rw-rw-rw-   0        0        0    21459 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/products/TriangularMatrixMatrix.h
--rw-rw-rw-   0        0        0    14184 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/products/TriangularMatrixMatrix_BLAS.h
--rw-rw-rw-   0        0        0    15072 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/products/TriangularMatrixVector.h
--rw-rw-rw-   0        0        0    10826 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/products/TriangularMatrixVector_BLAS.h
--rw-rw-rw-   0        0        0    15015 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/products/TriangularSolverMatrix.h
--rw-rw-rw-   0        0        0     6874 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/products/TriangularSolverMatrix_BLAS.h
--rw-rw-rw-   0        0        0     6030 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/products/TriangularSolverVector.h
-drwxrwxrwx   0        0        0        0 2023-06-19 06:52:41.292442 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/util/
--rw-rw-rw-   0        0        0    27402 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/util/BlasUtil.h
--rw-rw-rw-   0        0        0    20388 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/util/ConfigureVectorization.h
--rw-rw-rw-   0        0        0    22493 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/util/Constants.h
--rw-rw-rw-   0        0        0     4998 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/util/DisableStupidWarnings.h
--rw-rw-rw-   0        0        0    15877 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/util/ForwardDeclarations.h
--rw-rw-rw-   0        0        0     6711 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/util/IndexedViewHelper.h
--rw-rw-rw-   0        0        0    11167 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/util/IntegralConstant.h
--rw-rw-rw-   0        0        0     4405 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/util/MKL_support.h
--rw-rw-rw-   0        0        0    53933 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/util/Macros.h
--rw-rw-rw-   0        0        0    47516 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/util/Memory.h
--rw-rw-rw-   0        0        0    29449 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/util/Meta.h
--rw-rw-rw-   0        0        0       88 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/util/NonMPL2.h
--rw-rw-rw-   0        0        0     1055 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/util/ReenableStupidWarnings.h
--rw-rw-rw-   0        0        0     1483 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/util/ReshapedHelper.h
--rw-rw-rw-   0        0        0    10897 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/util/StaticAssert.h
--rw-rw-rw-   0        0        0    12280 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/util/SymbolicIndex.h
--rw-rw-rw-   0        0        0    36712 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/util/XprHelper.h
-drwxrwxrwx   0        0        0        0 2023-06-19 06:52:41.300444 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Eigenvalues/
--rw-rw-rw-   0        0        0    12905 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Eigenvalues/ComplexEigenSolver.h
--rw-rw-rw-   0        0        0    17736 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Eigenvalues/ComplexSchur.h
--rw-rw-rw-   0        0        0     4269 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Eigenvalues/ComplexSchur_LAPACKE.h
--rw-rw-rw-   0        0        0    23592 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Eigenvalues/EigenSolver.h
--rw-rw-rw-   0        0        0    17594 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Eigenvalues/GeneralizedEigenSolver.h
--rw-rw-rw-   0        0        0     9942 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Eigenvalues/GeneralizedSelfAdjointEigenSolver.h
--rw-rw-rw-   0        0        0    14713 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Eigenvalues/HessenbergDecomposition.h
--rw-rw-rw-   0        0        0     5733 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Eigenvalues/MatrixBaseEigenvalues.h
--rw-rw-rw-   0        0        0    24297 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Eigenvalues/RealQZ.h
--rw-rw-rw-   0        0        0    21636 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Eigenvalues/RealSchur.h
--rw-rw-rw-   0        0        0     3727 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Eigenvalues/RealSchur_LAPACKE.h
--rw-rw-rw-   0        0        0    34768 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Eigenvalues/SelfAdjointEigenSolver.h
--rw-rw-rw-   0        0        0     4191 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Eigenvalues/SelfAdjointEigenSolver_LAPACKE.h
--rw-rw-rw-   0        0        0    23099 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Eigenvalues/Tridiagonalization.h
-drwxrwxrwx   0        0        0        0 2023-06-19 06:52:41.306442 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Geometry/
--rw-rw-rw-   0        0        0    19425 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Geometry/AlignedBox.h
--rw-rw-rw-   0        0        0     8650 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Geometry/AngleAxis.h
--rw-rw-rw-   0        0        0     3738 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Geometry/EulerAngles.h
--rw-rw-rw-   0        0        0    21036 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Geometry/Homogeneous.h
--rw-rw-rw-   0        0        0    12244 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Geometry/Hyperplane.h
--rw-rw-rw-   0        0        0     9190 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Geometry/OrthoMethods.h
--rw-rw-rw-   0        0        0    10044 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Geometry/ParametrizedLine.h
--rw-rw-rw-   0        0        0    35237 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Geometry/Quaternion.h
--rw-rw-rw-   0        0        0     7061 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Geometry/Rotation2D.h
--rw-rw-rw-   0        0        0     8269 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Geometry/RotationBase.h
--rw-rw-rw-   0        0        0     6912 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Geometry/Scaling.h
--rw-rw-rw-   0        0        0    63473 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Geometry/Transform.h
--rw-rw-rw-   0        0        0     7866 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Geometry/Translation.h
--rw-rw-rw-   0        0        0     6356 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Geometry/Umeyama.h
-drwxrwxrwx   0        0        0        0 2023-06-19 06:52:41.307442 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Geometry/arch/
--rw-rw-rw-   0        0        0     5841 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Geometry/arch/Geometry_SIMD.h
-drwxrwxrwx   0        0        0        0 2023-06-19 06:52:41.308442 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Householder/
--rw-rw-rw-   0        0        0     4894 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Householder/BlockHouseholder.h
--rw-rw-rw-   0        0        0     5541 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Householder/Householder.h
--rw-rw-rw-   0        0        0    24114 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Householder/HouseholderSequence.h
-drwxrwxrwx   0        0        0        0 2023-06-19 06:52:41.312441 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/IterativeLinearSolvers/
--rw-rw-rw-   0        0        0     6981 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/IterativeLinearSolvers/BasicPreconditioners.h
--rw-rw-rw-   0        0        0     7062 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/IterativeLinearSolvers/BiCGSTAB.h
--rw-rw-rw-   0        0        0     9116 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/IterativeLinearSolvers/ConjugateGradient.h
--rw-rw-rw-   0        0        0    15442 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/IterativeLinearSolvers/IncompleteCholesky.h
--rw-rw-rw-   0        0        0    15415 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/IterativeLinearSolvers/IncompleteLUT.h
--rw-rw-rw-   0        0        0    13793 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/IterativeLinearSolvers/IterativeSolverBase.h
--rw-rw-rw-   0        0        0     7547 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/IterativeLinearSolvers/LeastSquareConjugateGradient.h
--rw-rw-rw-   0        0        0     4273 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/IterativeLinearSolvers/SolveWithGuess.h
-drwxrwxrwx   0        0        0        0 2023-06-19 06:52:41.314443 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Jacobi/
--rw-rw-rw-   0        0        0    16866 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Jacobi/Jacobi.h
-drwxrwxrwx   0        0        0        0 2023-06-19 06:52:41.316442 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/LU/
--rw-rw-rw-   0        0        0     3556 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/LU/Determinant.h
--rw-rw-rw-   0        0        0    33188 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/LU/FullPivLU.h
--rw-rw-rw-   0        0        0    15519 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/LU/InverseImpl.h
--rw-rw-rw-   0        0        0    22475 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/LU/PartialPivLU.h
--rw-rw-rw-   0        0        0     3638 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/LU/PartialPivLU_LAPACKE.h
-drwxrwxrwx   0        0        0        0 2023-06-19 06:52:41.317442 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/LU/arch/
--rw-rw-rw-   0        0        0    13796 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/LU/arch/InverseSize4.h
-drwxrwxrwx   0        0        0        0 2023-06-19 06:52:41.318442 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/OrderingMethods/
--rw-rw-rw-   0        0        0    16540 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/OrderingMethods/Amd.h
--rw-rw-rw-   0        0        0    63544 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/OrderingMethods/Eigen_Colamd.h
--rw-rw-rw-   0        0        0     5401 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/OrderingMethods/Ordering.h
-drwxrwxrwx   0        0        0        0 2023-06-19 06:52:41.321442 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/QR/
--rw-rw-rw-   0        0        0    26172 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/QR/ColPivHouseholderQR.h
--rw-rw-rw-   0        0        0     4759 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/QR/ColPivHouseholderQR_LAPACKE.h
--rw-rw-rw-   0        0        0    24064 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/QR/CompleteOrthogonalDecomposition.h
--rw-rw-rw-   0        0        0    27481 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/QR/FullPivHouseholderQR.h
--rw-rw-rw-   0        0        0    15075 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/QR/HouseholderQR.h
--rw-rw-rw-   0        0        0     3061 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/QR/HouseholderQR_LAPACKE.h
-drwxrwxrwx   0        0        0        0 2023-06-19 06:52:41.323442 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/SVD/
--rw-rw-rw-   0        0        0    54995 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/SVD/BDCSVD.h
--rw-rw-rw-   0        0        0    33798 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/SVD/JacobiSVD.h
--rw-rw-rw-   0        0        0     5190 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/SVD/JacobiSVD_LAPACKE.h
--rw-rw-rw-   0        0        0    14620 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/SVD/SVDBase.h
--rw-rw-rw-   0        0        0    16371 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/SVD/UpperBidiagonalization.h
-drwxrwxrwx   0        0        0        0 2023-06-19 06:52:41.324442 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/SparseCholesky/
--rw-rw-rw-   0        0        0    25058 2023-01-16 21:22:35.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/SparseCholesky/SimplicialCholesky.h
--rw-rw-rw-   0        0        0     6121 2023-01-17 05:50:15.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/SparseCholesky/SimplicialCholesky_impl.h
-drwxrwxrwx   0        0        0        0 2023-06-19 06:52:41.339442 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/SparseCore/
--rw-rw-rw-   0        0        0    11048 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/SparseCore/AmbiVector.h
--rw-rw-rw-   0        0        0     9017 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/SparseCore/CompressedStorage.h
--rw-rw-rw-   0        0        0    13518 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/SparseCore/ConservativeSparseSparseProduct.h
--rw-rw-rw-   0        0        0     2258 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/SparseCore/MappedSparseMatrix.h
--rw-rw-rw-   0        0        0    11638 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/SparseCore/SparseAssign.h
--rw-rw-rw-   0        0        0    24931 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/SparseCore/SparseBlock.h
--rw-rw-rw-   0        0        0     6691 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/SparseCore/SparseColEtree.h
--rw-rw-rw-   0        0        0    13976 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/SparseCore/SparseCompressedBase.h
--rw-rw-rw-   0        0        0    26156 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/SparseCore/SparseCwiseBinaryOp.h
--rw-rw-rw-   0        0        0     4887 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/SparseCore/SparseCwiseUnaryOp.h
--rw-rw-rw-   0        0        0    13598 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/SparseCore/SparseDenseProduct.h
--rw-rw-rw-   0        0        0     5946 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/SparseCore/SparseDiagonalProduct.h
--rw-rw-rw-   0        0        0     3178 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/SparseCore/SparseDot.h
--rw-rw-rw-   0        0        0     1136 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/SparseCore/SparseFuzzy.h
--rw-rw-rw-   0        0        0    12894 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/SparseCore/SparseMap.h
--rw-rw-rw-   0        0        0    58993 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/SparseCore/SparseMatrix.h
--rw-rw-rw-   0        0        0    17849 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/SparseCore/SparseMatrixBase.h
--rw-rw-rw-   0        0        0     7507 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/SparseCore/SparsePermutation.h
--rw-rw-rw-   0        0        0     7774 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/SparseCore/SparseProduct.h
--rw-rw-rw-   0        0        0     1748 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/SparseCore/SparseRedux.h
--rw-rw-rw-   0        0        0    15997 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/SparseCore/SparseRef.h
--rw-rw-rw-   0        0        0    26548 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/SparseCore/SparseSelfAdjointView.h
--rw-rw-rw-   0        0        0     4548 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/SparseCore/SparseSolverBase.h
--rw-rw-rw-   0        0        0     8902 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/SparseCore/SparseSparseProductWithPruning.h
--rw-rw-rw-   0        0        0     3267 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/SparseCore/SparseTranspose.h
--rw-rw-rw-   0        0        0     6626 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/SparseCore/SparseTriangularView.h
--rw-rw-rw-   0        0        0     7013 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/SparseCore/SparseUtil.h
--rw-rw-rw-   0        0        0    15310 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/SparseCore/SparseVector.h
--rw-rw-rw-   0        0        0     8381 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/SparseCore/SparseView.h
--rw-rw-rw-   0        0        0     9972 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/SparseCore/TriangularSolver.h
-drwxrwxrwx   0        0        0        0 2023-06-19 06:52:41.349475 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/SparseLU/
--rw-rw-rw-   0        0        0    34239 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/SparseLU/SparseLU.h
--rw-rw-rw-   0        0        0     4369 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/SparseLU/SparseLUImpl.h
--rw-rw-rw-   0        0        0     7828 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/SparseLU/SparseLU_Memory.h
--rw-rw-rw-   0        0        0     5084 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/SparseLU/SparseLU_Structs.h
--rw-rw-rw-   0        0        0    13212 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/SparseLU/SparseLU_SupernodalMatrix.h
--rw-rw-rw-   0        0        0     2129 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/SparseLU/SparseLU_Utils.h
--rw-rw-rw-   0        0        0     6893 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/SparseLU/SparseLU_column_bmod.h
--rw-rw-rw-   0        0        0     6763 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/SparseLU/SparseLU_column_dfs.h
--rw-rw-rw-   0        0        0     3788 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/SparseLU/SparseLU_copy_to_ucol.h
--rw-rw-rw-   0        0        0    10497 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/SparseLU/SparseLU_gemm_kernel.h
--rw-rw-rw-   0        0        0     4307 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/SparseLU/SparseLU_heap_relax_snode.h
--rw-rw-rw-   0        0        0     5853 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/SparseLU/SparseLU_kernel_bmod.h
--rw-rw-rw-   0        0        0     8708 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/SparseLU/SparseLU_panel_bmod.h
--rw-rw-rw-   0        0        0     9286 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/SparseLU/SparseLU_panel_dfs.h
--rw-rw-rw-   0        0        0     5116 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/SparseLU/SparseLU_pivotL.h
--rw-rw-rw-   0        0        0     4681 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/SparseLU/SparseLU_pruneL.h
--rw-rw-rw-   0        0        0     2972 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/SparseLU/SparseLU_relax_snode.h
-drwxrwxrwx   0        0        0        0 2023-06-19 06:52:41.349475 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/SparseQR/
--rw-rw-rw-   0        0        0    29925 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/SparseQR/SparseQR.h
-drwxrwxrwx   0        0        0        0 2023-06-19 06:52:41.353455 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/misc/
--rw-rw-rw-   0        0        0     2995 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/misc/Image.h
--rw-rw-rw-   0        0        0     2821 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/misc/Kernel.h
--rw-rw-rw-   0        0        0     1803 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/misc/RealSvd2x2.h
--rw-rw-rw-   0        0        0    31000 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/misc/blas.h
--rw-rw-rw-   0        0        0     7986 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/misc/lapack.h
--rw-rw-rw-   0        0        0  1074661 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/misc/lapacke.h
--rw-rw-rw-   0        0        0      491 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/misc/lapacke_mangling.h
-drwxrwxrwx   0        0        0        0 2023-06-19 06:52:41.357441 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/plugins/
--rw-rw-rw-   0        0        0    14418 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/plugins/ArrayCwiseBinaryOps.h
--rw-rw-rw-   0        0        0    21084 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/plugins/ArrayCwiseUnaryOps.h
--rw-rw-rw-   0        0        0    60448 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/plugins/BlockMethods.h
--rw-rw-rw-   0        0        0     4943 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/plugins/CommonCwiseBinaryOps.h
--rw-rw-rw-   0        0        0     7431 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/plugins/CommonCwiseUnaryOps.h
--rw-rw-rw-   0        0        0    12545 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/plugins/IndexedViewMethods.h
--rw-rw-rw-   0        0        0     6527 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/plugins/MatrixCwiseBinaryOps.h
--rw-rw-rw-   0        0        0     3445 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/plugins/MatrixCwiseUnaryOps.h
--rw-rw-rw-   0        0        0     7064 2021-03-12 08:57:32.000000 gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/plugins/ReshapedMethods.h
-drwxrwxrwx   0        0        0        0 2023-06-19 06:52:41.358477 gpboost-1.2.1.1/compile/external_libs/fast_double_parser/
--rw-rw-rw-   0        0        0     2661 2021-01-29 13:27:40.000000 gpboost-1.2.1.1/compile/external_libs/fast_double_parser/CMakeLists.txt
--rw-rw-rw-   0        0        0    11544 2021-01-29 13:27:40.000000 gpboost-1.2.1.1/compile/external_libs/fast_double_parser/LICENSE
--rw-rw-rw-   0        0        0     1392 2021-01-29 13:27:40.000000 gpboost-1.2.1.1/compile/external_libs/fast_double_parser/LICENSE.BSL
-drwxrwxrwx   0        0        0        0 2023-06-19 06:52:41.359470 gpboost-1.2.1.1/compile/external_libs/fast_double_parser/include/
--rw-rw-rw-   0        0        0    50746 2021-01-29 13:27:40.000000 gpboost-1.2.1.1/compile/external_libs/fast_double_parser/include/fast_double_parser.h
-drwxrwxrwx   0        0        0        0 2023-06-19 06:52:41.360479 gpboost-1.2.1.1/compile/external_libs/fmt/
--rw-rw-rw-   0        0        0    13412 2021-01-29 13:27:53.000000 gpboost-1.2.1.1/compile/external_libs/fmt/CMakeLists.txt
--rw-rw-rw-   0        0        0     1435 2021-01-29 13:27:53.000000 gpboost-1.2.1.1/compile/external_libs/fmt/LICENSE.rst
-drwxrwxrwx   0        0        0        0 2023-06-19 06:52:40.978039 gpboost-1.2.1.1/compile/external_libs/fmt/include/
-drwxrwxrwx   0        0        0        0 2023-06-19 06:52:41.367442 gpboost-1.2.1.1/compile/external_libs/fmt/include/fmt/
--rw-rw-rw-   0        0        0    36920 2021-01-29 13:27:53.000000 gpboost-1.2.1.1/compile/external_libs/fmt/include/fmt/chrono.h
--rw-rw-rw-   0        0        0    24252 2021-01-29 13:27:53.000000 gpboost-1.2.1.1/compile/external_libs/fmt/include/fmt/color.h
--rw-rw-rw-   0        0        0    24772 2021-01-29 13:27:53.000000 gpboost-1.2.1.1/compile/external_libs/fmt/include/fmt/compile.h
--rw-rw-rw-   0        0        0    73420 2021-01-29 13:27:53.000000 gpboost-1.2.1.1/compile/external_libs/fmt/include/fmt/core.h
--rw-rw-rw-   0        0        0   112636 2021-01-29 13:27:53.000000 gpboost-1.2.1.1/compile/external_libs/fmt/include/fmt/format-inl.h
--rw-rw-rw-   0        0        0   136849 2021-01-29 13:27:53.000000 gpboost-1.2.1.1/compile/external_libs/fmt/include/fmt/format.h
--rw-rw-rw-   0        0        0     2383 2021-01-29 13:27:53.000000 gpboost-1.2.1.1/compile/external_libs/fmt/include/fmt/locale.h
--rw-rw-rw-   0        0        0    14160 2021-01-29 13:27:53.000000 gpboost-1.2.1.1/compile/external_libs/fmt/include/fmt/os.h
--rw-rw-rw-   0        0        0     6082 2021-01-29 13:27:53.000000 gpboost-1.2.1.1/compile/external_libs/fmt/include/fmt/ostream.h
--rw-rw-rw-   0        0        0       77 2021-01-29 13:27:53.000000 gpboost-1.2.1.1/compile/external_libs/fmt/include/fmt/posix.h
--rw-rw-rw-   0        0        0    24008 2021-01-29 13:27:53.000000 gpboost-1.2.1.1/compile/external_libs/fmt/include/fmt/printf.h
--rw-rw-rw-   0        0        0    12939 2021-01-29 13:27:53.000000 gpboost-1.2.1.1/compile/external_libs/fmt/include/fmt/ranges.h
-drwxrwxrwx   0        0        0        0 2023-06-19 06:52:40.978039 gpboost-1.2.1.1/compile/include/
-drwxrwxrwx   0        0        0        0 2023-06-19 06:52:41.372442 gpboost-1.2.1.1/compile/include/GPBoost/
--rw-rw-rw-   0        0        0     3291 2023-02-22 08:53:45.000000 gpboost-1.2.1.1/compile/include/GPBoost/DF_utils.h
--rw-rw-rw-   0        0        0    10592 2023-06-16 12:23:42.000000 gpboost-1.2.1.1/compile/include/GPBoost/GP_utils.h
--rw-rw-rw-   0        0        0     2966 2023-02-16 13:06:27.000000 gpboost-1.2.1.1/compile/include/GPBoost/Vecchia_utils.h
--rw-rw-rw-   0        0        0    37137 2023-03-21 14:12:45.000000 gpboost-1.2.1.1/compile/include/GPBoost/cov_fcts.h
--rw-rw-rw-   0        0        0   150529 2023-06-12 14:03:44.000000 gpboost-1.2.1.1/compile/include/GPBoost/likelihoods.h
--rw-rw-rw-   0        0        0    58750 2023-03-23 10:35:29.000000 gpboost-1.2.1.1/compile/include/GPBoost/re_comp.h
--rw-rw-rw-   0        0        0    25805 2023-06-08 12:21:36.000000 gpboost-1.2.1.1/compile/include/GPBoost/re_model.h
--rw-rw-rw-   0        0        0   372194 2023-06-14 19:22:56.000000 gpboost-1.2.1.1/compile/include/GPBoost/re_model_template.h
--rw-rw-rw-   0        0        0    20177 2023-03-01 14:13:16.000000 gpboost-1.2.1.1/compile/include/GPBoost/sparse_matrix_utils.h
--rw-rw-rw-   0        0        0     2519 2023-01-18 12:49:42.000000 gpboost-1.2.1.1/compile/include/GPBoost/type_defs.h
--rw-rw-rw-   0        0        0     5255 2023-06-12 14:01:00.000000 gpboost-1.2.1.1/compile/include/GPBoost/utils.h
-drwxrwxrwx   0        0        0        0 2023-06-19 06:52:41.382442 gpboost-1.2.1.1/compile/include/LightGBM/
--rw-rw-rw-   0        0        0     2442 2021-01-29 13:27:06.000000 gpboost-1.2.1.1/compile/include/LightGBM/application.h
--rw-rw-rw-   0        0        0    17644 2021-01-29 13:27:06.000000 gpboost-1.2.1.1/compile/include/LightGBM/bin.h
--rw-rw-rw-   0        0        0    11258 2021-01-29 13:27:06.000000 gpboost-1.2.1.1/compile/include/LightGBM/boosting.h
--rw-rw-rw-   0        0        0    92126 2023-06-08 12:32:18.000000 gpboost-1.2.1.1/compile/include/LightGBM/c_api.h
--rw-rw-rw-   0        0        0    69980 2023-06-08 08:36:07.000000 gpboost-1.2.1.1/compile/include/LightGBM/config.h
-drwxrwxrwx   0        0        0        0 2023-06-19 06:52:41.382442 gpboost-1.2.1.1/compile/include/LightGBM/cuda/
--rw-rw-rw-   0        0        0      716 2021-01-29 13:27:06.000000 gpboost-1.2.1.1/compile/include/LightGBM/cuda/cuda_utils.h
--rw-rw-rw-   0        0        0     2550 2021-01-29 13:27:06.000000 gpboost-1.2.1.1/compile/include/LightGBM/cuda/vector_cudahost.h
--rw-rw-rw-   0        0        0    25455 2021-01-29 13:27:06.000000 gpboost-1.2.1.1/compile/include/LightGBM/dataset.h
--rw-rw-rw-   0        0        0     3760 2021-01-29 13:27:06.000000 gpboost-1.2.1.1/compile/include/LightGBM/dataset_loader.h
--rw-rw-rw-   0        0        0      643 2022-01-18 10:17:34.000000 gpboost-1.2.1.1/compile/include/LightGBM/export.h
--rw-rw-rw-   0        0        0    19974 2021-01-29 13:27:06.000000 gpboost-1.2.1.1/compile/include/LightGBM/feature_group.h
--rw-rw-rw-   0        0        0     2992 2023-05-26 15:59:37.000000 gpboost-1.2.1.1/compile/include/LightGBM/meta.h
--rw-rw-rw-   0        0        0     4618 2022-07-18 13:57:09.000000 gpboost-1.2.1.1/compile/include/LightGBM/metric.h
--rw-rw-rw-   0        0        0     1305 2023-03-08 16:18:29.000000 gpboost-1.2.1.1/compile/include/LightGBM/nesterov_boosting.h
--rw-rw-rw-   0        0        0    12281 2021-08-17 07:03:57.000000 gpboost-1.2.1.1/compile/include/LightGBM/network.h
--rw-rw-rw-   0        0        0     5021 2022-07-18 13:42:05.000000 gpboost-1.2.1.1/compile/include/LightGBM/objective_function.h
--rw-rw-rw-   0        0        0     1312 2021-01-29 13:27:06.000000 gpboost-1.2.1.1/compile/include/LightGBM/prediction_early_stop.h
--rw-rw-rw-   0        0        0     8210 2021-01-29 13:27:06.000000 gpboost-1.2.1.1/compile/include/LightGBM/train_share_states.h
--rw-rw-rw-   0        0        0    26928 2021-01-29 13:27:06.000000 gpboost-1.2.1.1/compile/include/LightGBM/tree.h
--rw-rw-rw-   0        0        0     4000 2021-02-02 09:08:55.000000 gpboost-1.2.1.1/compile/include/LightGBM/tree_learner.h
-drwxrwxrwx   0        0        0        0 2023-06-19 06:52:41.387441 gpboost-1.2.1.1/compile/include/LightGBM/utils/
--rw-rw-rw-   0        0        0     5094 2021-01-29 13:27:06.000000 gpboost-1.2.1.1/compile/include/LightGBM/utils/array_args.h
--rw-rw-rw-   0        0        0    35505 2022-11-18 12:31:49.000000 gpboost-1.2.1.1/compile/include/LightGBM/utils/common.h
--rw-rw-rw-   0        0        0     5331 2021-01-29 13:27:06.000000 gpboost-1.2.1.1/compile/include/LightGBM/utils/common_legacy_solaris.h
--rw-rw-rw-   0        0        0     2753 2021-01-29 13:27:06.000000 gpboost-1.2.1.1/compile/include/LightGBM/utils/file_io.h
--rw-rw-rw-   0        0        0     9232 2021-01-29 13:27:06.000000 gpboost-1.2.1.1/compile/include/LightGBM/utils/json11.h
--rw-rw-rw-   0        0        0     7042 2022-12-14 12:42:54.000000 gpboost-1.2.1.1/compile/include/LightGBM/utils/log.h
--rw-rw-rw-   0        0        0     2391 2021-01-29 13:27:06.000000 gpboost-1.2.1.1/compile/include/LightGBM/utils/openmp_wrapper.h
--rw-rw-rw-   0        0        0     2170 2021-01-29 13:27:06.000000 gpboost-1.2.1.1/compile/include/LightGBM/utils/pipeline_reader.h
--rw-rw-rw-   0        0        0     3025 2021-01-29 13:27:06.000000 gpboost-1.2.1.1/compile/include/LightGBM/utils/random.h
--rw-rw-rw-   0        0        0    11689 2021-01-29 13:27:06.000000 gpboost-1.2.1.1/compile/include/LightGBM/utils/text_reader.h
--rw-rw-rw-   0        0        0     6744 2021-01-29 13:27:06.000000 gpboost-1.2.1.1/compile/include/LightGBM/utils/threading.h
-drwxrwxrwx   0        0        0        0 2023-06-19 06:52:41.388441 gpboost-1.2.1.1/compile/include/LightGBM/utils/yamc/
--rw-rw-rw-   0        0        0     6461 2021-01-29 13:27:06.000000 gpboost-1.2.1.1/compile/include/LightGBM/utils/yamc/alternate_shared_mutex.hpp
--rw-rw-rw-   0        0        0     4492 2021-01-29 13:27:06.000000 gpboost-1.2.1.1/compile/include/LightGBM/utils/yamc/yamc_rwlock_sched.hpp
--rw-rw-rw-   0        0        0     5247 2021-01-29 13:27:06.000000 gpboost-1.2.1.1/compile/include/LightGBM/utils/yamc/yamc_shared_lock.hpp
-drwxrwxrwx   0        0        0        0 2023-06-19 06:52:40.979035 gpboost-1.2.1.1/compile/src/
-drwxrwxrwx   0        0        0        0 2023-06-19 06:52:41.391471 gpboost-1.2.1.1/compile/src/GPBoost/
--rw-rw-rw-   0        0        0     5769 2023-06-05 13:51:38.000000 gpboost-1.2.1.1/compile/src/GPBoost/DF_utils.cpp
--rw-rw-rw-   0        0        0     1688 2023-03-23 08:06:54.000000 gpboost-1.2.1.1/compile/src/GPBoost/GP_utils.cpp
--rw-rw-rw-   0        0        0    12100 2023-03-22 13:36:07.000000 gpboost-1.2.1.1/compile/src/GPBoost/Vecchia_utils.cpp
--rw-rw-rw-   0        0        0    35151 2023-06-08 12:23:19.000000 gpboost-1.2.1.1/compile/src/GPBoost/re_model.cpp
--rw-rw-rw-   0        0        0    11520 2023-01-18 10:31:49.000000 gpboost-1.2.1.1/compile/src/GPBoost/sparse_matrix_utils.cpp
-drwxrwxrwx   0        0        0        0 2023-06-19 06:52:41.392478 gpboost-1.2.1.1/compile/src/LightGBM/
-drwxrwxrwx   0        0        0        0 2023-06-19 06:52:41.392478 gpboost-1.2.1.1/compile/src/LightGBM/application/
--rw-rw-rw-   0        0        0    10556 2021-01-29 13:27:06.000000 gpboost-1.2.1.1/compile/src/LightGBM/application/application.cpp
--rw-rw-rw-   0        0        0    12217 2021-01-29 13:27:06.000000 gpboost-1.2.1.1/compile/src/LightGBM/application/predictor.hpp
-drwxrwxrwx   0        0        0        0 2023-06-19 06:52:41.399442 gpboost-1.2.1.1/compile/src/LightGBM/boosting/
--rw-rw-rw-   0        0        0     2299 2021-01-29 13:27:06.000000 gpboost-1.2.1.1/compile/src/LightGBM/boosting/boosting.cpp
--rw-rw-rw-   0        0        0     7604 2021-01-29 13:27:06.000000 gpboost-1.2.1.1/compile/src/LightGBM/boosting/dart.hpp
--rw-rw-rw-   0        0        0    35974 2023-06-07 14:42:25.000000 gpboost-1.2.1.1/compile/src/LightGBM/boosting/gbdt.cpp
--rw-rw-rw-   0        0        0    21149 2023-03-08 16:27:29.000000 gpboost-1.2.1.1/compile/src/LightGBM/boosting/gbdt.h
--rw-rw-rw-   0        0        0    25165 2023-03-08 16:17:44.000000 gpboost-1.2.1.1/compile/src/LightGBM/boosting/gbdt_model_text.cpp
--rw-rw-rw-   0        0        0     5028 2023-03-08 16:18:13.000000 gpboost-1.2.1.1/compile/src/LightGBM/boosting/gbdt_prediction.cpp
--rw-rw-rw-   0        0        0     6952 2021-01-29 13:27:06.000000 gpboost-1.2.1.1/compile/src/LightGBM/boosting/goss.hpp
--rw-rw-rw-   0        0        0     2643 2021-01-29 13:27:06.000000 gpboost-1.2.1.1/compile/src/LightGBM/boosting/prediction_early_stop.cpp
--rw-rw-rw-   0        0        0     8180 2021-01-29 13:27:06.000000 gpboost-1.2.1.1/compile/src/LightGBM/boosting/rf.hpp
--rw-rw-rw-   0        0        0     6352 2023-03-08 16:18:22.000000 gpboost-1.2.1.1/compile/src/LightGBM/boosting/score_updater.hpp
--rw-rw-rw-   0        0        0   102606 2023-06-10 06:06:39.000000 gpboost-1.2.1.1/compile/src/LightGBM/c_api.cpp
-drwxrwxrwx   0        0        0        0 2023-06-19 06:52:41.408442 gpboost-1.2.1.1/compile/src/LightGBM/io/
--rw-rw-rw-   0        0        0    30211 2021-01-29 13:27:06.000000 gpboost-1.2.1.1/compile/src/LightGBM/io/bin.cpp
--rw-rw-rw-   0        0        0    17277 2023-06-08 05:27:49.000000 gpboost-1.2.1.1/compile/src/LightGBM/io/config.cpp
--rw-rw-rw-   0        0        0    27684 2023-06-08 10:01:19.000000 gpboost-1.2.1.1/compile/src/LightGBM/io/config_auto.cpp
--rw-rw-rw-   0        0        0    58412 2023-05-26 15:43:08.000000 gpboost-1.2.1.1/compile/src/LightGBM/io/dataset.cpp
--rw-rw-rw-   0        0        0    61416 2021-01-29 13:27:06.000000 gpboost-1.2.1.1/compile/src/LightGBM/io/dataset_loader.cpp
--rw-rw-rw-   0        0        0    18916 2021-01-29 13:27:06.000000 gpboost-1.2.1.1/compile/src/LightGBM/io/dense_bin.hpp
--rw-rw-rw-   0        0        0     5635 2021-01-29 13:27:06.000000 gpboost-1.2.1.1/compile/src/LightGBM/io/file_io.cpp
--rw-rw-rw-   0        0        0    23192 2023-01-11 16:33:16.000000 gpboost-1.2.1.1/compile/src/LightGBM/io/json11.cpp
--rw-rw-rw-   0        0        0    20698 2022-11-18 12:33:52.000000 gpboost-1.2.1.1/compile/src/LightGBM/io/metadata.cpp
--rw-rw-rw-   0        0        0     8717 2021-01-29 13:27:06.000000 gpboost-1.2.1.1/compile/src/LightGBM/io/multi_val_dense_bin.hpp
--rw-rw-rw-   0        0        0    12550 2021-01-29 13:27:06.000000 gpboost-1.2.1.1/compile/src/LightGBM/io/multi_val_sparse_bin.hpp
--rw-rw-rw-   0        0        0     8131 2021-01-29 13:27:06.000000 gpboost-1.2.1.1/compile/src/LightGBM/io/parser.cpp
--rw-rw-rw-   0        0        0     3643 2021-01-29 13:27:06.000000 gpboost-1.2.1.1/compile/src/LightGBM/io/parser.hpp
--rw-rw-rw-   0        0        0    23759 2021-01-29 13:27:06.000000 gpboost-1.2.1.1/compile/src/LightGBM/io/sparse_bin.hpp
--rw-rw-rw-   0        0        0    16886 2021-01-29 13:27:06.000000 gpboost-1.2.1.1/compile/src/LightGBM/io/train_share_states.cpp
--rw-rw-rw-   0        0        0    42401 2021-01-29 13:27:06.000000 gpboost-1.2.1.1/compile/src/LightGBM/io/tree.cpp
--rw-rw-rw-   0        0        0      954 2021-01-29 13:27:06.000000 gpboost-1.2.1.1/compile/src/LightGBM/main.cpp
-drwxrwxrwx   0        0        0        0 2023-06-19 06:52:41.413442 gpboost-1.2.1.1/compile/src/LightGBM/metric/
--rw-rw-rw-   0        0        0    14303 2023-06-08 12:34:32.000000 gpboost-1.2.1.1/compile/src/LightGBM/metric/binary_metric.hpp
--rw-rw-rw-   0        0        0     5842 2021-01-29 13:27:06.000000 gpboost-1.2.1.1/compile/src/LightGBM/metric/dcg_calculator.cpp
--rw-rw-rw-   0        0        0     5697 2022-07-18 14:03:05.000000 gpboost-1.2.1.1/compile/src/LightGBM/metric/map_metric.hpp
--rw-rw-rw-   0        0        0     3330 2023-06-05 15:51:25.000000 gpboost-1.2.1.1/compile/src/LightGBM/metric/metric.cpp
--rw-rw-rw-   0        0        0    13595 2022-07-18 14:03:24.000000 gpboost-1.2.1.1/compile/src/LightGBM/metric/multiclass_metric.hpp
--rw-rw-rw-   0        0        0     3295 2022-07-18 13:57:02.000000 gpboost-1.2.1.1/compile/src/LightGBM/metric/random_effects_metric.hpp
--rw-rw-rw-   0        0        0     6163 2022-07-18 14:03:36.000000 gpboost-1.2.1.1/compile/src/LightGBM/metric/rank_metric.hpp
--rw-rw-rw-   0        0        0    18729 2023-06-08 12:34:13.000000 gpboost-1.2.1.1/compile/src/LightGBM/metric/regression_metric.hpp
--rw-rw-rw-   0        0        0    13207 2022-07-18 14:03:59.000000 gpboost-1.2.1.1/compile/src/LightGBM/metric/xentropy_metric.hpp
-drwxrwxrwx   0        0        0        0 2023-06-19 06:52:41.417442 gpboost-1.2.1.1/compile/src/LightGBM/network/
--rw-rw-rw-   0        0        0     3607 2021-01-29 13:27:06.000000 gpboost-1.2.1.1/compile/src/LightGBM/network/ifaddrs_patch.cpp
--rw-rw-rw-   0        0        0      944 2021-01-29 13:27:06.000000 gpboost-1.2.1.1/compile/src/LightGBM/network/ifaddrs_patch.h
--rw-rw-rw-   0        0        0     6410 2021-01-29 13:27:06.000000 gpboost-1.2.1.1/compile/src/LightGBM/network/linker_topo.cpp
--rw-rw-rw-   0        0        0     9330 2021-01-29 13:27:06.000000 gpboost-1.2.1.1/compile/src/LightGBM/network/linkers.h
--rw-rw-rw-   0        0        0     1901 2021-01-29 13:27:06.000000 gpboost-1.2.1.1/compile/src/LightGBM/network/linkers_mpi.cpp
--rw-rw-rw-   0        0        0     7905 2021-01-29 13:27:06.000000 gpboost-1.2.1.1/compile/src/LightGBM/network/linkers_socket.cpp
--rw-rw-rw-   0        0        0    14102 2021-08-17 07:04:55.000000 gpboost-1.2.1.1/compile/src/LightGBM/network/network.cpp
--rw-rw-rw-   0        0        0     8890 2022-01-14 16:36:55.000000 gpboost-1.2.1.1/compile/src/LightGBM/network/socket_wrapper.hpp
-drwxrwxrwx   0        0        0        0 2023-06-19 06:52:41.420442 gpboost-1.2.1.1/compile/src/LightGBM/objective/
--rw-rw-rw-   0        0        0     7605 2021-02-03 09:55:22.000000 gpboost-1.2.1.1/compile/src/LightGBM/objective/binary_objective.hpp
--rw-rw-rw-   0        0        0     9194 2021-01-29 13:27:06.000000 gpboost-1.2.1.1/compile/src/LightGBM/objective/multiclass_objective.hpp
--rw-rw-rw-   0        0        0     5549 2023-06-08 04:45:15.000000 gpboost-1.2.1.1/compile/src/LightGBM/objective/objective_function.cpp
--rw-rw-rw-   0        0        0    13401 2021-01-29 13:27:06.000000 gpboost-1.2.1.1/compile/src/LightGBM/objective/rank_objective.hpp
--rw-rw-rw-   0        0        0    35283 2023-06-10 06:07:26.000000 gpboost-1.2.1.1/compile/src/LightGBM/objective/regression_objective.hpp
--rw-rw-rw-   0        0        0     9779 2021-01-29 13:27:06.000000 gpboost-1.2.1.1/compile/src/LightGBM/objective/xentropy_objective.hpp
-drwxrwxrwx   0        0        0        0 2023-06-19 06:52:41.431450 gpboost-1.2.1.1/compile/src/LightGBM/treelearner/
--rw-rw-rw-   0        0        0     8004 2021-01-29 13:27:06.000000 gpboost-1.2.1.1/compile/src/LightGBM/treelearner/col_sampler.hpp
--rw-rw-rw-   0        0        0     6267 2021-01-29 13:27:06.000000 gpboost-1.2.1.1/compile/src/LightGBM/treelearner/cost_effective_gradient_boosting.hpp
--rw-rw-rw-   0        0        0     7898 2021-01-29 13:27:06.000000 gpboost-1.2.1.1/compile/src/LightGBM/treelearner/cuda_kernel_launcher.cu
--rw-rw-rw-   0        0        0     2662 2021-01-29 13:27:06.000000 gpboost-1.2.1.1/compile/src/LightGBM/treelearner/cuda_kernel_launcher.h
--rw-rw-rw-   0        0        0    41258 2021-01-29 13:27:06.000000 gpboost-1.2.1.1/compile/src/LightGBM/treelearner/cuda_tree_learner.cpp
--rw-rw-rw-   0        0        0    11541 2021-01-29 13:27:06.000000 gpboost-1.2.1.1/compile/src/LightGBM/treelearner/cuda_tree_learner.h
--rw-rw-rw-   0        0        0    12159 2021-01-29 13:27:06.000000 gpboost-1.2.1.1/compile/src/LightGBM/treelearner/data_parallel_tree_learner.cpp
--rw-rw-rw-   0        0        0     5831 2021-01-29 13:27:06.000000 gpboost-1.2.1.1/compile/src/LightGBM/treelearner/data_partition.hpp
--rw-rw-rw-   0        0        0    52366 2021-09-20 10:49:45.000000 gpboost-1.2.1.1/compile/src/LightGBM/treelearner/feature_histogram.hpp
--rw-rw-rw-   0        0        0     3634 2021-01-29 13:27:06.000000 gpboost-1.2.1.1/compile/src/LightGBM/treelearner/feature_parallel_tree_learner.cpp
--rw-rw-rw-   0        0        0    54339 2021-01-29 13:27:06.000000 gpboost-1.2.1.1/compile/src/LightGBM/treelearner/gpu_tree_learner.cpp
--rw-rw-rw-   0        0        0    11788 2021-01-29 13:27:06.000000 gpboost-1.2.1.1/compile/src/LightGBM/treelearner/gpu_tree_learner.h
-drwxrwxrwx   0        0        0        0 2023-06-19 06:52:41.432442 gpboost-1.2.1.1/compile/src/LightGBM/treelearner/kernels/
--rw-rw-rw-   0        0        0    37797 2021-01-29 13:27:06.000000 gpboost-1.2.1.1/compile/src/LightGBM/treelearner/kernels/histogram_16_64_256.cu
--rw-rw-rw-   0        0        0     5555 2021-01-29 13:27:06.000000 gpboost-1.2.1.1/compile/src/LightGBM/treelearner/kernels/histogram_16_64_256.hu
--rw-rw-rw-   0        0        0     5328 2021-01-29 13:27:06.000000 gpboost-1.2.1.1/compile/src/LightGBM/treelearner/leaf_splits.hpp
--rw-rw-rw-   0        0        0    15019 2021-01-29 13:27:06.000000 gpboost-1.2.1.1/compile/src/LightGBM/treelearner/linear_tree_learner.cpp
--rw-rw-rw-   0        0        0     4837 2021-01-29 13:27:06.000000 gpboost-1.2.1.1/compile/src/LightGBM/treelearner/linear_tree_learner.h
--rw-rw-rw-   0        0        0    49014 2021-01-29 13:27:06.000000 gpboost-1.2.1.1/compile/src/LightGBM/treelearner/monotone_constraints.hpp
-drwxrwxrwx   0        0        0        0 2023-06-19 06:52:41.433441 gpboost-1.2.1.1/compile/src/LightGBM/treelearner/ocl/
--rw-rw-rw-   0        0        0    42887 2021-01-29 13:27:06.000000 gpboost-1.2.1.1/compile/src/LightGBM/treelearner/ocl/histogram16.cl
--rw-rw-rw-   0        0        0    34143 2021-01-29 13:27:06.000000 gpboost-1.2.1.1/compile/src/LightGBM/treelearner/ocl/histogram256.cl
--rw-rw-rw-   0        0        0    34823 2021-01-29 13:27:06.000000 gpboost-1.2.1.1/compile/src/LightGBM/treelearner/ocl/histogram64.cl
--rw-rw-rw-   0        0        0     8669 2021-01-29 13:27:06.000000 gpboost-1.2.1.1/compile/src/LightGBM/treelearner/parallel_tree_learner.h
--rw-rw-rw-   0        0        0    36564 2021-02-02 10:54:50.000000 gpboost-1.2.1.1/compile/src/LightGBM/treelearner/serial_tree_learner.cpp
--rw-rw-rw-   0        0        0     9578 2021-02-02 10:42:52.000000 gpboost-1.2.1.1/compile/src/LightGBM/treelearner/serial_tree_learner.h
--rw-rw-rw-   0        0        0     9312 2021-01-29 13:27:06.000000 gpboost-1.2.1.1/compile/src/LightGBM/treelearner/split_info.hpp
--rw-rw-rw-   0        0        0     2336 2021-01-29 13:27:06.000000 gpboost-1.2.1.1/compile/src/LightGBM/treelearner/tree_learner.cpp
--rw-rw-rw-   0        0        0    22729 2021-01-29 13:27:06.000000 gpboost-1.2.1.1/compile/src/LightGBM/treelearner/voting_parallel_tree_learner.cpp
-drwxrwxrwx   0        0        0        0 2023-06-19 06:52:41.437442 gpboost-1.2.1.1/gpboost/
--rw-rw-rw-   0        0        0        8 2023-06-19 06:52:38.000000 gpboost-1.2.1.1/gpboost/VERSION.txt
--rw-rw-rw-   0        0        0     1455 2022-08-25 10:12:18.000000 gpboost-1.2.1.1/gpboost/__init__.py
--rw-rw-rw-   0        0        0   290536 2023-06-19 06:45:59.000000 gpboost-1.2.1.1/gpboost/basic.py
--rw-rw-rw-   0        0        0     9214 2021-03-03 12:29:59.000000 gpboost-1.2.1.1/gpboost/callback.py
--rw-rw-rw-   0        0        0     3434 2021-02-05 14:38:10.000000 gpboost-1.2.1.1/gpboost/compat.py
--rw-rw-rw-   0        0        0    61257 2023-06-10 06:13:10.000000 gpboost-1.2.1.1/gpboost/engine.py
--rw-rw-rw-   0        0        0     1556 2021-02-05 14:41:41.000000 gpboost-1.2.1.1/gpboost/libpath.py
--rw-rw-rw-   0        0        0    25829 2021-02-05 14:43:16.000000 gpboost-1.2.1.1/gpboost/plotting.py
--rw-rw-rw-   0        0        0    60507 2023-06-19 06:45:32.000000 gpboost-1.2.1.1/gpboost/sklearn.py
-drwxrwxrwx   0        0        0        0 2023-06-19 06:52:41.440441 gpboost-1.2.1.1/gpboost.egg-info/
--rw-rw-rw-   0        0        0     8738 2023-06-19 06:52:40.000000 gpboost-1.2.1.1/gpboost.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    56239 2023-06-19 06:52:40.000000 gpboost-1.2.1.1/gpboost.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 06:52:40.000000 gpboost-1.2.1.1/gpboost.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-19 06:47:48.000000 gpboost-1.2.1.1/gpboost.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      128 2023-06-19 06:52:40.000000 gpboost-1.2.1.1/gpboost.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-19 06:52:40.000000 gpboost-1.2.1.1/gpboost.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-19 06:52:41.442449 gpboost-1.2.1.1/setup.cfg
--rw-rw-rw-   0        0        0    16099 2022-05-06 08:19:13.000000 gpboost-1.2.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-12 05:46:21.081087 gpboost-1.2.2/
+-rw-rw-rw-   0        0        0    11248 2023-07-12 05:46:16.000000 gpboost-1.2.2/LICENSE
+-rw-rw-rw-   0        0        0     3530 2022-02-01 20:40:50.000000 gpboost-1.2.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     8581 2023-07-12 05:46:21.080086 gpboost-1.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0     7576 2023-07-10 14:50:18.000000 gpboost-1.2.2/README.md
+-rw-rw-rw-   0        0        0        0 2023-07-12 05:46:16.000000 gpboost-1.2.2/_IS_SOURCE_PACKAGE.txt
+drwxrwxrwx   0        0        0        0 2023-07-12 05:46:17.436952 gpboost-1.2.2/compile/
+-rw-rw-rw-   0        0        0     4828 2023-07-12 05:46:16.000000 gpboost-1.2.2/compile/CMakeIntegratedOpenCL.cmake
+-rw-rw-rw-   0        0        0    16679 2023-07-12 05:46:16.000000 gpboost-1.2.2/compile/CMakeLists.txt
+drwxrwxrwx   0        0        0        0 2023-07-12 05:46:17.411985 gpboost-1.2.2/compile/external_libs/
+drwxrwxrwx   0        0        0        0 2023-07-12 05:46:17.377087 gpboost-1.2.2/compile/external_libs/CSparse/
+drwxrwxrwx   0        0        0        0 2023-07-12 05:46:17.440951 gpboost-1.2.2/compile/external_libs/CSparse/Doc/
+-rw-rw-rw-   0        0        0      879 2014-03-21 19:14:15.000000 gpboost-1.2.2/compile/external_libs/CSparse/Doc/LICENSE.txt
+drwxrwxrwx   0        0        0        0 2023-07-12 05:46:17.444951 gpboost-1.2.2/compile/external_libs/CSparse/Include/
+-rw-rw-rw-   0        0        0     3202 2023-01-18 08:20:43.000000 gpboost-1.2.2/compile/external_libs/CSparse/Include/cs.h
+drwxrwxrwx   0        0        0        0 2023-07-12 05:46:17.455985 gpboost-1.2.2/compile/external_libs/CSparse/Source/
+-rw-rw-rw-   0        0        0     1624 2014-03-21 19:14:08.000000 gpboost-1.2.2/compile/external_libs/CSparse/Source/cs_dfs.c
+-rw-rw-rw-   0        0        0      682 2020-03-25 11:28:02.000000 gpboost-1.2.2/compile/external_libs/CSparse/Source/cs_reach.c
+-rw-rw-rw-   0        0        0     1364 2020-03-25 11:28:05.000000 gpboost-1.2.2/compile/external_libs/CSparse/Source/cs_spsolve.c
+drwxrwxrwx   0        0        0        0 2023-07-12 05:46:17.462991 gpboost-1.2.2/compile/external_libs/OptimLib/
+-rw-rw-rw-   0        0        0    11558 2021-04-01 05:47:35.000000 gpboost-1.2.2/compile/external_libs/OptimLib/LICENSE
+-rw-rw-rw-   0        0        0      211 2021-04-01 05:47:35.000000 gpboost-1.2.2/compile/external_libs/OptimLib/NOTICE.txt
+drwxrwxrwx   0        0        0        0 2023-07-12 05:46:17.463956 gpboost-1.2.2/compile/external_libs/OptimLib/constrained/
+-rw-rw-rw-   0        0        0     7773 2021-04-01 05:49:27.000000 gpboost-1.2.2/compile/external_libs/OptimLib/constrained/sumt.hpp
+drwxrwxrwx   0        0        0        0 2023-07-12 05:46:17.469980 gpboost-1.2.2/compile/external_libs/OptimLib/line_search/
+-rw-rw-rw-   0        0        0    11032 2021-04-01 05:49:27.000000 gpboost-1.2.2/compile/external_libs/OptimLib/line_search/more_thuente.hpp
+drwxrwxrwx   0        0        0        0 2023-07-12 05:46:17.490952 gpboost-1.2.2/compile/external_libs/OptimLib/misc/
+-rw-rw-rw-   0        0        0     1975 2021-04-01 05:49:27.000000 gpboost-1.2.2/compile/external_libs/OptimLib/misc/determine_bounds_type.hpp
+-rw-rw-rw-   0        0        0     3102 2021-04-01 05:49:27.000000 gpboost-1.2.2/compile/external_libs/OptimLib/misc/error_reporting.hpp
+-rw-rw-rw-   0        0        0     7593 2021-04-01 12:25:42.000000 gpboost-1.2.2/compile/external_libs/OptimLib/misc/error_reporting.ipp
+-rw-rw-rw-   0        0        0     2060 2021-04-01 05:49:27.000000 gpboost-1.2.2/compile/external_libs/OptimLib/misc/jacobian_adjust.hpp
+drwxrwxrwx   0        0        0        0 2023-07-12 05:46:17.530834 gpboost-1.2.2/compile/external_libs/OptimLib/misc/matrix_ops/
+-rw-rw-rw-   0        0        0     1179 2021-04-01 05:49:27.000000 gpboost-1.2.2/compile/external_libs/OptimLib/misc/matrix_ops/abs.hpp
+-rw-rw-rw-   0        0        0     1700 2021-04-01 05:49:27.000000 gpboost-1.2.2/compile/external_libs/OptimLib/misc/matrix_ops/abs_max.hpp
+-rw-rw-rw-   0        0        0     1652 2021-04-01 05:49:27.000000 gpboost-1.2.2/compile/external_libs/OptimLib/misc/matrix_ops/access.hpp
+-rw-rw-rw-   0        0        0     1256 2021-04-01 05:49:27.000000 gpboost-1.2.2/compile/external_libs/OptimLib/misc/matrix_ops/accu.hpp
+-rw-rw-rw-   0        0        0     1178 2021-04-01 05:49:27.000000 gpboost-1.2.2/compile/external_libs/OptimLib/misc/matrix_ops/array_add.hpp
+-rw-rw-rw-   0        0        0     1460 2021-04-01 05:49:27.000000 gpboost-1.2.2/compile/external_libs/OptimLib/misc/matrix_ops/array_div.hpp
+-rw-rw-rw-   0        0        0     1181 2021-04-01 05:49:27.000000 gpboost-1.2.2/compile/external_libs/OptimLib/misc/matrix_ops/array_mult.hpp
+-rw-rw-rw-   0        0        0     1156 2021-04-01 05:49:27.000000 gpboost-1.2.2/compile/external_libs/OptimLib/misc/matrix_ops/as_scalar.hpp
+-rw-rw-rw-   0        0        0     1147 2021-04-01 05:49:27.000000 gpboost-1.2.2/compile/external_libs/OptimLib/misc/matrix_ops/cos.hpp
+-rw-rw-rw-   0        0        0     1150 2021-04-01 05:49:27.000000 gpboost-1.2.2/compile/external_libs/OptimLib/misc/matrix_ops/cout.hpp
+-rw-rw-rw-   0        0        0     1201 2021-04-01 05:49:27.000000 gpboost-1.2.2/compile/external_libs/OptimLib/misc/matrix_ops/diagmat.hpp
+-rw-rw-rw-   0        0        0     1210 2021-04-01 05:49:27.000000 gpboost-1.2.2/compile/external_libs/OptimLib/misc/matrix_ops/diagvec.hpp
+-rw-rw-rw-   0        0        0     1179 2021-04-01 05:49:27.000000 gpboost-1.2.2/compile/external_libs/OptimLib/misc/matrix_ops/dot.hpp
+-rw-rw-rw-   0        0        0     1155 2021-04-01 05:49:27.000000 gpboost-1.2.2/compile/external_libs/OptimLib/misc/matrix_ops/endl.hpp
+-rw-rw-rw-   0        0        0     1123 2021-04-01 05:49:27.000000 gpboost-1.2.2/compile/external_libs/OptimLib/misc/matrix_ops/eval.hpp
+-rw-rw-rw-   0        0        0     1147 2021-04-01 05:49:27.000000 gpboost-1.2.2/compile/external_libs/OptimLib/misc/matrix_ops/exp.hpp
+-rw-rw-rw-   0        0        0     1184 2021-04-01 05:49:27.000000 gpboost-1.2.2/compile/external_libs/OptimLib/misc/matrix_ops/eye.hpp
+-rw-rw-rw-   0        0        0     1443 2021-04-11 01:03:04.000000 gpboost-1.2.2/compile/external_libs/OptimLib/misc/matrix_ops/get_sort_index.hpp
+-rw-rw-rw-   0        0        0     1206 2021-04-01 05:49:27.000000 gpboost-1.2.2/compile/external_libs/OptimLib/misc/matrix_ops/hadamard.hpp
+-rw-rw-rw-   0        0        0     1270 2021-04-01 05:49:27.000000 gpboost-1.2.2/compile/external_libs/OptimLib/misc/matrix_ops/index_min.hpp
+-rw-rw-rw-   0        0        0     1176 2021-04-01 05:49:27.000000 gpboost-1.2.2/compile/external_libs/OptimLib/misc/matrix_ops/inv.hpp
+-rw-rw-rw-   0        0        0     1263 2021-04-01 05:49:27.000000 gpboost-1.2.2/compile/external_libs/OptimLib/misc/matrix_ops/is_finite.hpp
+-rw-rw-rw-   0        0        0     1147 2021-04-01 05:49:27.000000 gpboost-1.2.2/compile/external_libs/OptimLib/misc/matrix_ops/log.hpp
+-rw-rw-rw-   0        0        0     1557 2021-04-01 05:49:27.000000 gpboost-1.2.2/compile/external_libs/OptimLib/misc/matrix_ops/max.hpp
+-rw-rw-rw-   0        0        0     1502 2021-04-01 05:49:27.000000 gpboost-1.2.2/compile/external_libs/OptimLib/misc/matrix_ops/min.hpp
+-rw-rw-rw-   0        0        0     1132 2021-04-01 05:49:27.000000 gpboost-1.2.2/compile/external_libs/OptimLib/misc/matrix_ops/ncol.hpp
+-rw-rw-rw-   0        0        0     1748 2021-04-01 05:49:27.000000 gpboost-1.2.2/compile/external_libs/OptimLib/misc/matrix_ops/norm.hpp
+-rw-rw-rw-   0        0        0     1432 2021-04-01 05:49:27.000000 gpboost-1.2.2/compile/external_libs/OptimLib/misc/matrix_ops/ones.hpp
+-rw-rw-rw-   0        0        0     1154 2021-04-01 05:49:27.000000 gpboost-1.2.2/compile/external_libs/OptimLib/misc/matrix_ops/pow.hpp
+-rw-rw-rw-   0        0        0     1833 2021-04-01 05:49:27.000000 gpboost-1.2.2/compile/external_libs/OptimLib/misc/matrix_ops/randi.hpp
+-rw-rw-rw-   0        0        0     2125 2021-04-11 01:02:01.000000 gpboost-1.2.2/compile/external_libs/OptimLib/misc/matrix_ops/randn.hpp
+-rw-rw-rw-   0        0        0     1594 2021-04-01 05:49:27.000000 gpboost-1.2.2/compile/external_libs/OptimLib/misc/matrix_ops/randu.hpp
+-rw-rw-rw-   0        0        0     1525 2021-04-01 05:49:27.000000 gpboost-1.2.2/compile/external_libs/OptimLib/misc/matrix_ops/reset_negative_values.hpp
+-rw-rw-rw-   0        0        0     1312 2021-04-01 05:49:27.000000 gpboost-1.2.2/compile/external_libs/OptimLib/misc/matrix_ops/set_size.hpp
+-rw-rw-rw-   0        0        0     1174 2021-04-01 05:49:27.000000 gpboost-1.2.2/compile/external_libs/OptimLib/misc/matrix_ops/size.hpp
+-rw-rw-rw-   0        0        0     1208 2021-04-01 05:49:27.000000 gpboost-1.2.2/compile/external_libs/OptimLib/misc/matrix_ops/solve.hpp
+-rw-rw-rw-   0        0        0     1152 2021-04-01 05:49:27.000000 gpboost-1.2.2/compile/external_libs/OptimLib/misc/matrix_ops/sqrt.hpp
+-rw-rw-rw-   0        0        0     1506 2021-04-01 05:49:27.000000 gpboost-1.2.2/compile/external_libs/OptimLib/misc/matrix_ops/sum.hpp
+-rw-rw-rw-   0        0        0     1310 2021-04-01 05:49:27.000000 gpboost-1.2.2/compile/external_libs/OptimLib/misc/matrix_ops/transpose.hpp
+-rw-rw-rw-   0        0        0     1442 2021-04-01 05:49:27.000000 gpboost-1.2.2/compile/external_libs/OptimLib/misc/matrix_ops/zeros.hpp
+-rw-rw-rw-   0        0        0     1129 2021-04-01 05:49:27.000000 gpboost-1.2.2/compile/external_libs/OptimLib/misc/misc.hpp
+-rw-rw-rw-   0        0        0     2220 2021-04-01 05:49:27.000000 gpboost-1.2.2/compile/external_libs/OptimLib/misc/numerical_gradient.hpp
+-rw-rw-rw-   0        0        0     3957 2021-04-01 05:49:27.000000 gpboost-1.2.2/compile/external_libs/OptimLib/misc/numerical_hessian.hpp
+-rw-rw-rw-   0        0        0     2228 2021-04-01 05:49:27.000000 gpboost-1.2.2/compile/external_libs/OptimLib/misc/optim_matdefs.hpp
+-rw-rw-rw-   0        0        0     3152 2021-04-01 05:49:27.000000 gpboost-1.2.2/compile/external_libs/OptimLib/misc/optim_options.hpp
+-rw-rw-rw-   0        0        0     5754 2021-04-01 05:49:27.000000 gpboost-1.2.2/compile/external_libs/OptimLib/misc/optim_structs.hpp
+-rw-rw-rw-   0        0        0    38503 2021-04-01 05:49:27.000000 gpboost-1.2.2/compile/external_libs/OptimLib/misc/optim_trace.hpp
+-rw-rw-rw-   0        0        0     4071 2021-04-01 05:49:27.000000 gpboost-1.2.2/compile/external_libs/OptimLib/misc/transform_vals.hpp
+-rw-rw-rw-   0        0        0     1106 2021-04-01 05:49:27.000000 gpboost-1.2.2/compile/external_libs/OptimLib/misc/unit_vec.hpp
+-rw-rw-rw-   0        0        0     1082 2021-04-01 05:49:27.000000 gpboost-1.2.2/compile/external_libs/OptimLib/misc/unit_vec.ipp
+-rw-rw-rw-   0        0        0     2062 2022-05-16 08:23:28.000000 gpboost-1.2.2/compile/external_libs/OptimLib/optim.hpp
+drwxrwxrwx   0        0        0        0 2023-07-12 05:46:17.574310 gpboost-1.2.2/compile/external_libs/OptimLib/unconstrained/
+-rw-rw-rw-   0        0        0    10816 2022-05-16 08:34:45.000000 gpboost-1.2.2/compile/external_libs/OptimLib/unconstrained/bfgs.hpp
+-rw-rw-rw-   0        0        0    11427 2021-04-01 05:49:27.000000 gpboost-1.2.2/compile/external_libs/OptimLib/unconstrained/cg.hpp
+-rw-rw-rw-   0        0        0    10693 2021-04-01 05:49:27.000000 gpboost-1.2.2/compile/external_libs/OptimLib/unconstrained/de.hpp
+-rw-rw-rw-   0        0        0    15780 2021-04-01 05:49:27.000000 gpboost-1.2.2/compile/external_libs/OptimLib/unconstrained/de_prmm.hpp
+-rw-rw-rw-   0        0        0     9250 2022-08-16 12:43:27.000000 gpboost-1.2.2/compile/external_libs/OptimLib/unconstrained/gd.hpp
+-rw-rw-rw-   0        0        0     7776 2022-06-08 13:34:35.000000 gpboost-1.2.2/compile/external_libs/OptimLib/unconstrained/gd.ipp
+-rw-rw-rw-   0        0        0     9955 2021-04-01 05:49:28.000000 gpboost-1.2.2/compile/external_libs/OptimLib/unconstrained/lbfgs.hpp
+-rw-rw-rw-   0        0        0     6505 2021-04-01 05:49:28.000000 gpboost-1.2.2/compile/external_libs/OptimLib/unconstrained/newton.hpp
+-rw-rw-rw-   0        0        0    14178 2022-05-11 15:58:43.000000 gpboost-1.2.2/compile/external_libs/OptimLib/unconstrained/nm.hpp
+-rw-rw-rw-   0        0        0    11188 2021-04-01 05:49:28.000000 gpboost-1.2.2/compile/external_libs/OptimLib/unconstrained/pso.hpp
+-rw-rw-rw-   0        0        0    10573 2021-04-01 05:49:28.000000 gpboost-1.2.2/compile/external_libs/OptimLib/unconstrained/pso_dv.hpp
+drwxrwxrwx   0        0        0        0 2023-07-12 05:46:17.583310 gpboost-1.2.2/compile/external_libs/OptimLib/zeros/
+-rw-rw-rw-   0        0        0    13567 2021-04-01 05:49:28.000000 gpboost-1.2.2/compile/external_libs/OptimLib/zeros/broyden.hpp
+-rw-rw-rw-   0        0        0    16983 2021-04-01 05:49:28.000000 gpboost-1.2.2/compile/external_libs/OptimLib/zeros/broyden_df.hpp
+drwxrwxrwx   0        0        0        0 2023-07-12 05:46:17.587311 gpboost-1.2.2/compile/external_libs/compute/
+-rw-rw-rw-   0        0        0     4455 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/CMakeLists.txt
+drwxrwxrwx   0        0        0        0 2023-07-12 05:46:17.608326 gpboost-1.2.2/compile/external_libs/compute/cmake/
+-rw-rw-rw-   0        0        0      253 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/cmake/BoostComputeConfig.cmake.in
+-rw-rw-rw-   0        0        0     5760 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/cmake/FindBolt.cmake
+-rw-rw-rw-   0        0        0     7541 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/cmake/FindEigen.cmake
+-rw-rw-rw-   0        0        0    13242 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/cmake/FindTBB.cmake
+drwxrwxrwx   0        0        0        0 2023-07-12 05:46:17.612309 gpboost-1.2.2/compile/external_libs/compute/cmake/opencl/
+-rw-rw-rw-   0        0        0     3395 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/cmake/opencl/FindOpenCL.cmake
+drwxrwxrwx   0        0        0        0 2023-07-12 05:46:17.381087 gpboost-1.2.2/compile/external_libs/compute/include/
+drwxrwxrwx   0        0        0        0 2023-07-12 05:46:17.616308 gpboost-1.2.2/compile/external_libs/compute/include/boost/
+drwxrwxrwx   0        0        0        0 2023-07-12 05:46:17.787390 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/
+drwxrwxrwx   0        0        0        0 2023-07-12 05:46:18.137368 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/
+-rw-rw-rw-   0        0        0     6568 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/accumulate.hpp
+-rw-rw-rw-   0        0        0     4542 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/adjacent_difference.hpp
+-rw-rw-rw-   0        0        0     5482 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/adjacent_find.hpp
+-rw-rw-rw-   0        0        0     1469 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/all_of.hpp
+-rw-rw-rw-   0        0        0     1590 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/any_of.hpp
+-rw-rw-rw-   0        0        0     1523 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/binary_search.hpp
+-rw-rw-rw-   0        0        0    32364 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/copy.hpp
+-rw-rw-rw-   0        0        0     2641 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/copy_if.hpp
+-rw-rw-rw-   0        0        0     1995 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/copy_n.hpp
+-rw-rw-rw-   0        0        0     2165 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/count.hpp
+-rw-rw-rw-   0        0        0     2457 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/count_if.hpp
+drwxrwxrwx   0        0        0        0 2023-07-12 05:46:18.302357 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/detail/
+-rw-rw-rw-   0        0        0     6429 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/detail/balanced_path.hpp
+-rw-rw-rw-   0        0        0     4759 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/detail/binary_find.hpp
+-rw-rw-rw-   0        0        0     2265 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/detail/compact.hpp
+-rw-rw-rw-   0        0        0     7581 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/detail/copy_on_device.hpp
+-rw-rw-rw-   0        0        0     6935 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/detail/copy_to_device.hpp
+-rw-rw-rw-   0        0        0     6865 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/detail/copy_to_host.hpp
+-rw-rw-rw-   0        0        0     2683 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/detail/count_if_with_ballot.hpp
+-rw-rw-rw-   0        0        0     2735 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/detail/count_if_with_reduce.hpp
+-rw-rw-rw-   0        0        0     4370 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/detail/count_if_with_threads.hpp
+-rw-rw-rw-   0        0        0     2511 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/detail/find_extrema.hpp
+-rw-rw-rw-   0        0        0     5471 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/detail/find_extrema_on_cpu.hpp
+-rw-rw-rw-   0        0        0     4359 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/detail/find_extrema_with_atomics.hpp
+-rw-rw-rw-   0        0        0    19116 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/detail/find_extrema_with_reduce.hpp
+-rw-rw-rw-   0        0        0     8722 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/detail/find_if_with_atomics.hpp
+-rw-rw-rw-   0        0        0     4975 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/detail/inplace_reduce.hpp
+-rw-rw-rw-   0        0        0     6195 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/detail/insertion_sort.hpp
+-rw-rw-rw-   0        0        0     3990 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/detail/merge_path.hpp
+-rw-rw-rw-   0        0        0    15020 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/detail/merge_sort_on_cpu.hpp
+-rw-rw-rw-   0        0        0    22695 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/detail/merge_sort_on_gpu.hpp
+-rw-rw-rw-   0        0        0     7542 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/detail/merge_with_merge_path.hpp
+-rw-rw-rw-   0        0        0    15971 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/detail/radix_sort.hpp
+-rw-rw-rw-   0        0        0     1937 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/detail/random_fill.hpp
+-rw-rw-rw-   0        0        0     5362 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/detail/reduce_by_key.hpp
+-rw-rw-rw-   0        0        0    24276 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/detail/reduce_by_key_with_scan.hpp
+-rw-rw-rw-   0        0        0     4059 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/detail/reduce_on_cpu.hpp
+-rw-rw-rw-   0        0        0    10677 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/detail/reduce_on_gpu.hpp
+-rw-rw-rw-   0        0        0     1590 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/detail/scan.hpp
+-rw-rw-rw-   0        0        0     7261 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/detail/scan_on_cpu.hpp
+-rw-rw-rw-   0        0        0    11650 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/detail/scan_on_gpu.hpp
+-rw-rw-rw-   0        0        0     2665 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/detail/search_all.hpp
+-rw-rw-rw-   0        0        0     2046 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/detail/serial_accumulate.hpp
+-rw-rw-rw-   0        0        0     2311 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/detail/serial_count_if.hpp
+-rw-rw-rw-   0        0        0     3238 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/detail/serial_find_extrema.hpp
+-rw-rw-rw-   0        0        0     3601 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/detail/serial_merge.hpp
+-rw-rw-rw-   0        0        0     2208 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/detail/serial_reduce.hpp
+-rw-rw-rw-   0        0        0     4346 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/detail/serial_reduce_by_key.hpp
+-rw-rw-rw-   0        0        0     3287 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/detail/serial_scan.hpp
+-rw-rw-rw-   0        0        0     2271 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/equal.hpp
+-rw-rw-rw-   0        0        0     1684 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/equal_range.hpp
+-rw-rw-rw-   0        0        0     4151 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/exclusive_scan.hpp
+-rw-rw-rw-   0        0        0    10343 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/fill.hpp
+-rw-rw-rw-   0        0        0     1409 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/fill_n.hpp
+-rw-rw-rw-   0        0        0     2067 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/find.hpp
+-rw-rw-rw-   0        0        0     4916 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/find_end.hpp
+-rw-rw-rw-   0        0        0     1545 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/find_if.hpp
+-rw-rw-rw-   0        0        0     1701 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/find_if_not.hpp
+-rw-rw-rw-   0        0        0     2203 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/for_each.hpp
+-rw-rw-rw-   0        0        0     1464 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/for_each_n.hpp
+-rw-rw-rw-   0        0        0     2887 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/gather.hpp
+-rw-rw-rw-   0        0        0     1958 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/generate.hpp
+-rw-rw-rw-   0        0        0     1314 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/generate_n.hpp
+-rw-rw-rw-   0        0        0     5777 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/includes.hpp
+-rw-rw-rw-   0        0        0     3494 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/inclusive_scan.hpp
+-rw-rw-rw-   0        0        0     3952 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/inner_product.hpp
+-rw-rw-rw-   0        0        0     2113 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/inplace_merge.hpp
+-rw-rw-rw-   0        0        0     1789 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/iota.hpp
+-rw-rw-rw-   0        0        0     1834 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/is_partitioned.hpp
+-rw-rw-rw-   0        0        0     2817 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/is_permutation.hpp
+-rw-rw-rw-   0        0        0     2507 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/is_sorted.hpp
+-rw-rw-rw-   0        0        0     5076 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/lexicographical_compare.hpp
+-rw-rw-rw-   0        0        0     1623 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/lower_bound.hpp
+-rw-rw-rw-   0        0        0     2863 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/max_element.hpp
+-rw-rw-rw-   0        0        0     5153 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/merge.hpp
+-rw-rw-rw-   0        0        0     2862 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/min_element.hpp
+-rw-rw-rw-   0        0        0     2746 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/minmax_element.hpp
+-rw-rw-rw-   0        0        0     3507 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/mismatch.hpp
+-rw-rw-rw-   0        0        0     5878 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/next_permutation.hpp
+-rw-rw-rw-   0        0        0     1468 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/none_of.hpp
+-rw-rw-rw-   0        0        0     2962 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/nth_element.hpp
+-rw-rw-rw-   0        0        0     1722 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/partial_sum.hpp
+-rw-rw-rw-   0        0        0     1568 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/partition.hpp
+-rw-rw-rw-   0        0        0     2664 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/partition_copy.hpp
+-rw-rw-rw-   0        0        0     1910 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/partition_point.hpp
+-rw-rw-rw-   0        0        0     5870 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/prev_permutation.hpp
+-rw-rw-rw-   0        0        0     3100 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/random_shuffle.hpp
+-rw-rw-rw-   0        0        0    11764 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/reduce.hpp
+-rw-rw-rw-   0        0        0     6070 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/reduce_by_key.hpp
+-rw-rw-rw-   0        0        0     2062 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/remove.hpp
+-rw-rw-rw-   0        0        0     1903 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/remove_if.hpp
+-rw-rw-rw-   0        0        0     2684 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/replace.hpp
+-rw-rw-rw-   0        0        0     2300 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/replace_copy.hpp
+-rw-rw-rw-   0        0        0     2518 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/reverse.hpp
+-rw-rw-rw-   0        0        0     2765 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/reverse_copy.hpp
+-rw-rw-rw-   0        0        0     1869 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/rotate.hpp
+-rw-rw-rw-   0        0        0     1572 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/rotate_copy.hpp
+-rw-rw-rw-   0        0        0     3542 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/scatter.hpp
+-rw-rw-rw-   0        0        0     4861 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/scatter_if.hpp
+-rw-rw-rw-   0        0        0     3047 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/search.hpp
+-rw-rw-rw-   0        0        0     4574 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/search_n.hpp
+-rw-rw-rw-   0        0        0     7132 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/set_difference.hpp
+-rw-rw-rw-   0        0        0     6825 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/set_intersection.hpp
+-rw-rw-rw-   0        0        0     7737 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/set_symmetric_difference.hpp
+-rw-rw-rw-   0        0        0     7588 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/set_union.hpp
+-rw-rw-rw-   0        0        0     6776 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/sort.hpp
+-rw-rw-rw-   0        0        0     6324 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/sort_by_key.hpp
+-rw-rw-rw-   0        0        0     2815 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/stable_partition.hpp
+-rw-rw-rw-   0        0        0     3924 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/stable_sort.hpp
+-rw-rw-rw-   0        0        0     6239 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/stable_sort_by_key.hpp
+-rw-rw-rw-   0        0        0     1922 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/swap_ranges.hpp
+-rw-rw-rw-   0        0        0     3339 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/transform.hpp
+-rw-rw-rw-   0        0        0     4860 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/transform_if.hpp
+-rw-rw-rw-   0        0        0     3783 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/transform_reduce.hpp
+-rw-rw-rw-   0        0        0     2638 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/unique.hpp
+-rw-rw-rw-   0        0        0     6604 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/unique_copy.hpp
+-rw-rw-rw-   0        0        0     1610 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/upper_bound.hpp
+-rw-rw-rw-   0        0        0     4493 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm.hpp
+drwxrwxrwx   0        0        0        0 2023-07-12 05:46:18.311356 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/allocator/
+-rw-rw-rw-   0        0        0     3108 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/allocator/buffer_allocator.hpp
+-rw-rw-rw-   0        0        0     1445 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/allocator/pinned_allocator.hpp
+-rw-rw-rw-   0        0        0      769 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/allocator.hpp
+drwxrwxrwx   0        0        0        0 2023-07-12 05:46:18.325357 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/async/
+-rw-rw-rw-   0        0        0     4178 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/async/future.hpp
+-rw-rw-rw-   0        0        0     1708 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/async/wait.hpp
+-rw-rw-rw-   0        0        0     1925 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/async/wait_guard.hpp
+-rw-rw-rw-   0        0        0      724 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/async.hpp
+-rw-rw-rw-   0        0        0     7010 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/buffer.hpp
+-rw-rw-rw-   0        0        0     1677 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/cl.hpp
+-rw-rw-rw-   0        0        0      686 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/cl_ext.hpp
+-rw-rw-rw-   0        0        0    10458 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/closure.hpp
+-rw-rw-rw-   0        0        0    64508 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/command_queue.hpp
+-rw-rw-rw-   0        0        0     2425 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/config.hpp
+drwxrwxrwx   0        0        0        0 2023-07-12 05:46:18.369356 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/container/
+-rw-rw-rw-   0        0        0     7987 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/container/array.hpp
+-rw-rw-rw-   0        0        0     8185 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/container/basic_string.hpp
+drwxrwxrwx   0        0        0        0 2023-07-12 05:46:18.373357 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/container/detail/
+-rw-rw-rw-   0        0        0     1569 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/container/detail/scalar.hpp
+-rw-rw-rw-   0        0        0     7089 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/container/dynamic_bitset.hpp
+-rw-rw-rw-   0        0        0    11201 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/container/flat_map.hpp
+-rw-rw-rw-   0        0        0     8698 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/container/flat_set.hpp
+-rw-rw-rw-   0        0        0     7160 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/container/mapped_view.hpp
+-rw-rw-rw-   0        0        0     1668 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/container/stack.hpp
+-rw-rw-rw-   0        0        0      826 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/container/string.hpp
+-rw-rw-rw-   0        0        0    17204 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/container/valarray.hpp
+-rw-rw-rw-   0        0        0    24764 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/container/vector.hpp
+-rw-rw-rw-   0        0        0     1048 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/container.hpp
+-rw-rw-rw-   0        0        0     6839 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/context.hpp
+-rw-rw-rw-   0        0        0     1174 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/core.hpp
+drwxrwxrwx   0        0        0        0 2023-07-12 05:46:18.492355 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/detail/
+-rw-rw-rw-   0        0        0      875 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/detail/assert_cl_success.hpp
+-rw-rw-rw-   0        0        0     4242 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/detail/buffer_value.hpp
+-rw-rw-rw-   0        0        0     3194 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/detail/cl_versions.hpp
+-rw-rw-rw-   0        0        0     5609 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/detail/device_ptr.hpp
+-rw-rw-rw-   0        0        0     5308 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/detail/diagnostic.hpp
+-rw-rw-rw-   0        0        0     1695 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/detail/duration.hpp
+-rw-rw-rw-   0        0        0     8600 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/detail/get_object_info.hpp
+-rw-rw-rw-   0        0        0      972 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/detail/getenv.hpp
+-rw-rw-rw-   0        0        0     1474 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/detail/global_static.hpp
+-rw-rw-rw-   0        0        0      990 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/detail/is_buffer_iterator.hpp
+-rw-rw-rw-   0        0        0     3838 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/detail/is_contiguous_iterator.hpp
+-rw-rw-rw-   0        0        0     1715 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/detail/iterator_plus_distance.hpp
+-rw-rw-rw-   0        0        0     1458 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/detail/iterator_range_size.hpp
+-rw-rw-rw-   0        0        0     1193 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/detail/iterator_traits.hpp
+-rw-rw-rw-   0        0        0     1497 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/detail/literal.hpp
+-rw-rw-rw-   0        0        0     3606 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/detail/lru_cache.hpp
+-rw-rw-rw-   0        0        0    33188 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/detail/meta_kernel.hpp
+-rw-rw-rw-   0        0        0     2335 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/detail/mpl_vector_to_tuple.hpp
+-rw-rw-rw-   0        0        0     2134 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/detail/nvidia_compute_capability.hpp
+-rw-rw-rw-   0        0        0     7414 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/detail/parameter_cache.hpp
+-rw-rw-rw-   0        0        0     2173 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/detail/path.hpp
+-rw-rw-rw-   0        0        0     2670 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/detail/print_range.hpp
+-rw-rw-rw-   0        0        0     2620 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/detail/read_write_single_value.hpp
+-rw-rw-rw-   0        0        0     1603 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/detail/sha1.hpp
+-rw-rw-rw-   0        0        0     1871 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/detail/variadic_macros.hpp
+-rw-rw-rw-   0        0        0     1541 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/detail/vendor.hpp
+-rw-rw-rw-   0        0        0     1279 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/detail/work_size.hpp
+-rw-rw-rw-   0        0        0    21876 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/device.hpp
+-rw-rw-rw-   0        0        0    10618 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/event.hpp
+drwxrwxrwx   0        0        0        0 2023-07-12 05:46:18.512357 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/exception/
+-rw-rw-rw-   0        0        0     2663 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/exception/context_error.hpp
+-rw-rw-rw-   0        0        0     1369 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/exception/no_device_found.hpp
+-rw-rw-rw-   0        0        0     6865 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/exception/opencl_error.hpp
+-rw-rw-rw-   0        0        0     1765 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/exception/program_build_failure.hpp
+-rw-rw-rw-   0        0        0     2271 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/exception/unsupported_extension_error.hpp
+-rw-rw-rw-   0        0        0      881 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/exception.hpp
+drwxrwxrwx   0        0        0        0 2023-07-12 05:46:18.526364 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/experimental/
+-rw-rw-rw-   0        0        0     1517 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/experimental/clamp_range.hpp
+-rw-rw-rw-   0        0        0     1500 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/experimental/malloc.hpp
+-rw-rw-rw-   0        0        0     2055 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/experimental/sort_by_transform.hpp
+-rw-rw-rw-   0        0        0     1380 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/experimental/tabulate.hpp
+-rw-rw-rw-   0        0        0    12605 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/function.hpp
+drwxrwxrwx   0        0        0        0 2023-07-12 05:46:18.590410 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/functional/
+-rw-rw-rw-   0        0        0     1251 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/functional/as.hpp
+-rw-rw-rw-   0        0        0     3090 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/functional/atomic.hpp
+-rw-rw-rw-   0        0        0     7491 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/functional/bind.hpp
+-rw-rw-rw-   0        0        0     1146 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/functional/common.hpp
+-rw-rw-rw-   0        0        0     1281 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/functional/convert.hpp
+drwxrwxrwx   0        0        0        0 2023-07-12 05:46:18.609445 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/functional/detail/
+-rw-rw-rw-   0        0        0     1291 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/functional/detail/macros.hpp
+-rw-rw-rw-   0        0        0     1483 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/functional/detail/nvidia_ballot.hpp
+-rw-rw-rw-   0        0        0     1268 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/functional/detail/nvidia_popcount.hpp
+-rw-rw-rw-   0        0        0     4349 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/functional/detail/unpack.hpp
+-rw-rw-rw-   0        0        0     2183 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/functional/field.hpp
+-rw-rw-rw-   0        0        0     1479 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/functional/geometry.hpp
+-rw-rw-rw-   0        0        0     1959 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/functional/get.hpp
+-rw-rw-rw-   0        0        0     2664 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/functional/hash.hpp
+-rw-rw-rw-   0        0        0     1617 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/functional/identity.hpp
+-rw-rw-rw-   0        0        0     1206 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/functional/integer.hpp
+-rw-rw-rw-   0        0        0     4931 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/functional/logical.hpp
+-rw-rw-rw-   0        0        0     4361 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/functional/math.hpp
+-rw-rw-rw-   0        0        0     3173 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/functional/operator.hpp
+-rw-rw-rw-   0        0        0     1857 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/functional/popcount.hpp
+-rw-rw-rw-   0        0        0     2022 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/functional/relational.hpp
+-rw-rw-rw-   0        0        0     1377 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/functional.hpp
+drwxrwxrwx   0        0        0        0 2023-07-12 05:46:18.635427 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/image/
+-rw-rw-rw-   0        0        0     5859 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/image/image1d.hpp
+-rw-rw-rw-   0        0        0     8038 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/image/image2d.hpp
+-rw-rw-rw-   0        0        0     8315 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/image/image3d.hpp
+-rw-rw-rw-   0        0        0     4125 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/image/image_format.hpp
+-rw-rw-rw-   0        0        0     4810 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/image/image_object.hpp
+-rw-rw-rw-   0        0        0     6334 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/image/image_sampler.hpp
+-rw-rw-rw-   0        0        0      919 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/image.hpp
+-rw-rw-rw-   0        0        0      561 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/image2d.hpp
+-rw-rw-rw-   0        0        0      561 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/image3d.hpp
+-rw-rw-rw-   0        0        0      571 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/image_format.hpp
+-rw-rw-rw-   0        0        0      573 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/image_sampler.hpp
+drwxrwxrwx   0        0        0        0 2023-07-12 05:46:18.654433 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/interop/
+drwxrwxrwx   0        0        0        0 2023-07-12 05:46:18.658427 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/interop/eigen/
+-rw-rw-rw-   0        0        0     2738 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/interop/eigen/core.hpp
+-rw-rw-rw-   0        0        0      633 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/interop/eigen.hpp
+drwxrwxrwx   0        0        0        0 2023-07-12 05:46:18.671272 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/interop/opencv/
+-rw-rw-rw-   0        0        0     4886 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/interop/opencv/core.hpp
+-rw-rw-rw-   0        0        0     1092 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/interop/opencv/highgui.hpp
+-rw-rw-rw-   0        0        0     1433 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/interop/opencv/ocl.hpp
+-rw-rw-rw-   0        0        0      690 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/interop/opencv.hpp
+drwxrwxrwx   0        0        0        0 2023-07-12 05:46:18.706284 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/interop/opengl/
+-rw-rw-rw-   0        0        0     3851 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/interop/opengl/acquire.hpp
+-rw-rw-rw-   0        0        0      745 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/interop/opengl/cl_gl.hpp
+-rw-rw-rw-   0        0        0      765 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/interop/opengl/cl_gl_ext.hpp
+-rw-rw-rw-   0        0        0     4704 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/interop/opengl/context.hpp
+-rw-rw-rw-   0        0        0      679 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/interop/opengl/gl.hpp
+-rw-rw-rw-   0        0        0     2934 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/interop/opengl/opengl_buffer.hpp
+-rw-rw-rw-   0        0        0     3767 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/interop/opengl/opengl_renderbuffer.hpp
+-rw-rw-rw-   0        0        0     4075 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/interop/opengl/opengl_texture.hpp
+-rw-rw-rw-   0        0        0      965 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/interop/opengl.hpp
+drwxrwxrwx   0        0        0        0 2023-07-12 05:46:18.729514 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/interop/qt/
+-rw-rw-rw-   0        0        0     2242 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/interop/qt/qimage.hpp
+-rw-rw-rw-   0        0        0      712 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/interop/qt/qpoint.hpp
+-rw-rw-rw-   0        0        0      719 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/interop/qt/qpointf.hpp
+-rw-rw-rw-   0        0        0      742 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/interop/qt/qtcore.hpp
+-rw-rw-rw-   0        0        0      641 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/interop/qt/qtgui.hpp
+-rw-rw-rw-   0        0        0     1430 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/interop/qt/qvector.hpp
+-rw-rw-rw-   0        0        0      670 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/interop/qt.hpp
+drwxrwxrwx   0        0        0        0 2023-07-12 05:46:18.745993 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/interop/vtk/
+-rw-rw-rw-   0        0        0     2113 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/interop/vtk/bounds.hpp
+-rw-rw-rw-   0        0        0     2742 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/interop/vtk/data_array.hpp
+-rw-rw-rw-   0        0        0     1339 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/interop/vtk/matrix4x4.hpp
+-rw-rw-rw-   0        0        0     1896 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/interop/vtk/points.hpp
+-rw-rw-rw-   0        0        0      781 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/interop/vtk.hpp
+drwxrwxrwx   0        0        0        0 2023-07-12 05:46:18.792993 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/iterator/
+-rw-rw-rw-   0        0        0     8565 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/iterator/buffer_iterator.hpp
+-rw-rw-rw-   0        0        0     5785 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/iterator/constant_buffer_iterator.hpp
+-rw-rw-rw-   0        0        0     4415 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/iterator/constant_iterator.hpp
+-rw-rw-rw-   0        0        0     4787 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/iterator/counting_iterator.hpp
+drwxrwxrwx   0        0        0        0 2023-07-12 05:46:18.803993 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/iterator/detail/
+-rw-rw-rw-   0        0        0     1726 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/iterator/detail/get_base_iterator_buffer.hpp
+-rw-rw-rw-   0        0        0     6076 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/iterator/detail/swizzle_iterator.hpp
+-rw-rw-rw-   0        0        0     4078 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/iterator/discard_iterator.hpp
+-rw-rw-rw-   0        0        0     5169 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/iterator/function_input_iterator.hpp
+-rw-rw-rw-   0        0        0     6505 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/iterator/permutation_iterator.hpp
+-rw-rw-rw-   0        0        0     9894 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/iterator/strided_iterator.hpp
+-rw-rw-rw-   0        0        0     7979 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/iterator/transform_iterator.hpp
+-rw-rw-rw-   0        0        0    10751 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/iterator/zip_iterator.hpp
+-rw-rw-rw-   0        0        0     1168 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/iterator.hpp
+-rw-rw-rw-   0        0        0    18118 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/kernel.hpp
+drwxrwxrwx   0        0        0        0 2023-07-12 05:46:18.837997 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/lambda/
+-rw-rw-rw-   0        0        0    11279 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/lambda/context.hpp
+-rw-rw-rw-   0        0        0    25620 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/lambda/functional.hpp
+-rw-rw-rw-   0        0        0     4373 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/lambda/get.hpp
+-rw-rw-rw-   0        0        0     2302 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/lambda/make_pair.hpp
+-rw-rw-rw-   0        0        0     5041 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/lambda/make_tuple.hpp
+-rw-rw-rw-   0        0        0      816 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/lambda/placeholder.hpp
+-rw-rw-rw-   0        0        0     2589 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/lambda/placeholders.hpp
+-rw-rw-rw-   0        0        0     4232 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/lambda/result_of.hpp
+-rw-rw-rw-   0        0        0      884 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/lambda.hpp
+drwxrwxrwx   0        0        0        0 2023-07-12 05:46:18.846993 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/memory/
+-rw-rw-rw-   0        0        0     2343 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/memory/local_buffer.hpp
+-rw-rw-rw-   0        0        0     4630 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/memory/svm_ptr.hpp
+-rw-rw-rw-   0        0        0      738 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/memory.hpp
+-rw-rw-rw-   0        0        0     7258 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/memory_object.hpp
+-rw-rw-rw-   0        0        0     4162 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/pipe.hpp
+-rw-rw-rw-   0        0        0     7678 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/platform.hpp
+-rw-rw-rw-   0        0        0    26141 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/program.hpp
+drwxrwxrwx   0        0        0        0 2023-07-12 05:46:18.885340 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/random/
+-rw-rw-rw-   0        0        0     3068 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/random/bernoulli_distribution.hpp
+-rw-rw-rw-   0        0        0      825 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/random/default_random_engine.hpp
+-rw-rw-rw-   0        0        0     5557 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/random/discrete_distribution.hpp
+-rw-rw-rw-   0        0        0     7736 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/random/linear_congruential_engine.hpp
+-rw-rw-rw-   0        0        0     8542 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/random/mersenne_twister_engine.hpp
+-rw-rw-rw-   0        0        0     4782 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/random/normal_distribution.hpp
+-rw-rw-rw-   0        0        0    14255 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/random/threefry_engine.hpp
+-rw-rw-rw-   0        0        0     3717 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/random/uniform_int_distribution.hpp
+-rw-rw-rw-   0        0        0     3590 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/random/uniform_real_distribution.hpp
+-rw-rw-rw-   0        0        0     1176 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/random.hpp
+-rw-rw-rw-   0        0        0      563 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/source.hpp
+-rw-rw-rw-   0        0        0     2041 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/svm.hpp
+-rw-rw-rw-   0        0        0     9676 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/system.hpp
+drwxrwxrwx   0        0        0        0 2023-07-12 05:46:18.929340 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/type_traits/
+-rw-rw-rw-   0        0        0     2253 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/type_traits/common_type.hpp
+drwxrwxrwx   0        0        0        0 2023-07-12 05:46:18.934340 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/type_traits/detail/
+-rw-rw-rw-   0        0        0      992 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/type_traits/detail/capture_traits.hpp
+-rw-rw-rw-   0        0        0     1390 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/type_traits/is_device_iterator.hpp
+-rw-rw-rw-   0        0        0     2616 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/type_traits/is_fundamental.hpp
+-rw-rw-rw-   0        0        0     1143 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/type_traits/is_vector_type.hpp
+-rw-rw-rw-   0        0        0     2415 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/type_traits/make_vector_type.hpp
+-rw-rw-rw-   0        0        0     1351 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/type_traits/result_of.hpp
+-rw-rw-rw-   0        0        0     2438 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/type_traits/scalar_type.hpp
+-rw-rw-rw-   0        0        0     1175 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/type_traits/type_definition.hpp
+-rw-rw-rw-   0        0        0     3833 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/type_traits/type_name.hpp
+-rw-rw-rw-   0        0        0     2258 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/type_traits/vector_size.hpp
+-rw-rw-rw-   0        0        0     1131 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/type_traits.hpp
+drwxrwxrwx   0        0        0        0 2023-07-12 05:46:18.965340 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/types/
+-rw-rw-rw-   0        0        0      569 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/types/builtin.hpp
+-rw-rw-rw-   0        0        0     5102 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/types/complex.hpp
+-rw-rw-rw-   0        0        0     6195 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/types/fundamental.hpp
+-rw-rw-rw-   0        0        0     3294 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/types/pair.hpp
+-rw-rw-rw-   0        0        0     1800 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/types/size_t.hpp
+-rw-rw-rw-   0        0        0     5886 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/types/struct.hpp
+-rw-rw-rw-   0        0        0     9023 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/types/tuple.hpp
+-rw-rw-rw-   0        0        0      895 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/types.hpp
+-rw-rw-rw-   0        0        0     2502 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/user_event.hpp
+drwxrwxrwx   0        0        0        0 2023-07-12 05:46:18.989344 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/utility/
+-rw-rw-rw-   0        0        0     2262 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/utility/dim.hpp
+-rw-rw-rw-   0        0        0     4040 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/utility/extents.hpp
+-rw-rw-rw-   0        0        0     2857 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/utility/invoke.hpp
+-rw-rw-rw-   0        0        0     5665 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/utility/program_cache.hpp
+-rw-rw-rw-   0        0        0     1366 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/utility/source.hpp
+-rw-rw-rw-   0        0        0     5956 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/utility/wait_list.hpp
+-rw-rw-rw-   0        0        0      844 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/utility.hpp
+-rw-rw-rw-   0        0        0      683 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/version.hpp
+-rw-rw-rw-   0        0        0      569 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/wait_list.hpp
+-rw-rw-rw-   0        0        0     1567 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/include/boost/compute.hpp
+drwxrwxrwx   0        0        0        0 2023-07-12 05:46:18.993344 gpboost-1.2.2/compile/external_libs/compute/meta/
+-rw-rw-rw-   0        0        0      282 2021-01-29 13:27:37.000000 gpboost-1.2.2/compile/external_libs/compute/meta/libraries.json
+drwxrwxrwx   0        0        0        0 2023-07-12 05:46:18.998343 gpboost-1.2.2/compile/external_libs/eigen/
+-rw-rw-rw-   0        0        0    25206 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/CMakeLists.txt
+drwxrwxrwx   0        0        0        0 2023-07-12 05:46:19.057880 gpboost-1.2.2/compile/external_libs/eigen/Eigen/
+-rw-rw-rw-   0        0        0     1206 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/Cholesky
+-rw-rw-rw-   0        0        0    12893 2023-06-20 05:55:10.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/Core
+-rw-rw-rw-   0        0        0      129 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/Dense
+-rw-rw-rw-   0        0        0     1837 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/Eigenvalues
+-rw-rw-rw-   0        0        0     1999 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/Geometry
+-rw-rw-rw-   0        0        0      858 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/Householder
+-rw-rw-rw-   0        0        0     2131 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/IterativeLinearSolvers
+-rw-rw-rw-   0        0        0      926 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/Jacobi
+-rw-rw-rw-   0        0        0     1472 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/LU
+-rw-rw-rw-   0        0        0     2521 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/OrderingMethods
+-rw-rw-rw-   0        0        0     1322 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/QR
+-rw-rw-rw-   0        0        0     1634 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/SVD
+-rw-rw-rw-   0        0        0      922 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/Sparse
+-rw-rw-rw-   0        0        0     1272 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/SparseCholesky
+-rw-rw-rw-   0        0        0     2309 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/SparseCore
+-rw-rw-rw-   0        0        0     1864 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/SparseLU
+-rw-rw-rw-   0        0        0     1231 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/SparseQR
+drwxrwxrwx   0        0        0        0 2023-07-12 05:46:17.411985 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/
+drwxrwxrwx   0        0        0        0 2023-07-12 05:46:19.067880 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Cholesky/
+-rw-rw-rw-   0        0        0    25560 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Cholesky/LDLT.h
+-rw-rw-rw-   0        0        0    19398 2023-01-16 16:29:13.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Cholesky/LLT.h
+-rw-rw-rw-   0        0        0     4073 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Cholesky/LLT_LAPACKE.h
+drwxrwxrwx   0        0        0        0 2023-07-12 05:46:19.377882 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/
+-rw-rw-rw-   0        0        0    19627 2021-08-16 05:28:02.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/ArithmeticSequence.h
+-rw-rw-rw-   0        0        0    17144 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/Array.h
+-rw-rw-rw-   0        0        0     8443 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/ArrayBase.h
+-rw-rw-rw-   0        0        0     6984 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/ArrayWrapper.h
+-rw-rw-rw-   0        0        0     2828 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/Assign.h
+-rw-rw-rw-   0        0        0    41938 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/AssignEvaluator.h
+-rw-rw-rw-   0        0        0    12666 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/Assign_MKL.h
+-rw-rw-rw-   0        0        0    14263 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/BandMatrix.h
+-rw-rw-rw-   0        0        0    18852 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/Block.h
+-rw-rw-rw-   0        0        0     4571 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/BooleanRedux.h
+-rw-rw-rw-   0        0        0     6145 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/CommaInitializer.h
+-rw-rw-rw-   0        0        0     7165 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/ConditionEstimator.h
+-rw-rw-rw-   0        0        0    65712 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/CoreEvaluators.h
+-rw-rw-rw-   0        0        0     4877 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/CoreIterators.h
+-rw-rw-rw-   0        0        0     8131 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/CwiseBinaryOp.h
+-rw-rw-rw-   0        0        0    37252 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/CwiseNullaryOp.h
+-rw-rw-rw-   0        0        0     8453 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/CwiseTernaryOp.h
+-rw-rw-rw-   0        0        0     3980 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/CwiseUnaryOp.h
+-rw-rw-rw-   0        0        0     5583 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/CwiseUnaryView.h
+-rw-rw-rw-   0        0        0    31179 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/DenseBase.h
+-rw-rw-rw-   0        0        0    24905 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/DenseCoeffsBase.h
+-rw-rw-rw-   0        0        0    23343 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/DenseStorage.h
+-rw-rw-rw-   0        0        0     9967 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/Diagonal.h
+-rw-rw-rw-   0        0        0    15061 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/DiagonalMatrix.h
+-rw-rw-rw-   0        0        0     1016 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/DiagonalProduct.h
+-rw-rw-rw-   0        0        0    11964 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/Dot.h
+-rw-rw-rw-   0        0        0     5911 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/EigenBase.h
+-rw-rw-rw-   0        0        0     4915 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/ForceAlignedAccess.h
+-rw-rw-rw-   0        0        0     5914 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/Fuzzy.h
+-rw-rw-rw-   0        0        0    22144 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/GeneralProduct.h
+-rw-rw-rw-   0        0        0    35664 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/GenericPacketMath.h
+-rw-rw-rw-   0        0        0    11737 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/GlobalFunctions.h
+-rw-rw-rw-   0        0        0     8496 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/IO.h
+-rw-rw-rw-   0        0        0     9857 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/IndexedView.h
+-rw-rw-rw-   0        0        0     3566 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/Inverse.h
+-rw-rw-rw-   0        0        0     7398 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/Map.h
+-rw-rw-rw-   0        0        0    11520 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/MapBase.h
+-rw-rw-rw-   0        0        0    60856 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/MathFunctions.h
+-rw-rw-rw-   0        0        0     7092 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/MathFunctionsImpl.h
+-rw-rw-rw-   0        0        0    24859 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/Matrix.h
+-rw-rw-rw-   0        0        0    24403 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/MatrixBase.h
+-rw-rw-rw-   0        0        0     2543 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/NestByValue.h
+-rw-rw-rw-   0        0        0     3729 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/NoAlias.h
+-rw-rw-rw-   0        0        0    11924 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/NumTraits.h
+-rw-rw-rw-   0        0        0     9429 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/PartialReduxEvaluator.h
+-rw-rw-rw-   0        0        0    21353 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/PermutationMatrix.h
+-rw-rw-rw-   0        0        0    50200 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/PlainObjectBase.h
+-rw-rw-rw-   0        0        0     7524 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/Product.h
+-rw-rw-rw-   0        0        0    54996 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/ProductEvaluators.h
+-rw-rw-rw-   0        0        0     7974 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/Random.h
+-rw-rw-rw-   0        0        0    19685 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/Redux.h
+-rw-rw-rw-   0        0        0    18392 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/Ref.h
+-rw-rw-rw-   0        0        0     5773 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/Replicate.h
+-rw-rw-rw-   0        0        0    17455 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/Reshaped.h
+-rw-rw-rw-   0        0        0     4335 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/ReturnByValue.h
+-rw-rw-rw-   0        0        0     7672 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/Reverse.h
+-rw-rw-rw-   0        0        0     6236 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/Select.h
+-rw-rw-rw-   0        0        0    15238 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/SelfAdjointView.h
+-rw-rw-rw-   0        0        0     1744 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/SelfCwiseBinaryOp.h
+-rw-rw-rw-   0        0        0     6985 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/Solve.h
+-rw-rw-rw-   0        0        0     9514 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/SolveTriangular.h
+-rw-rw-rw-   0        0        0     6338 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/SolverBase.h
+-rw-rw-rw-   0        0        0     8974 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/StableNorm.h
+-rw-rw-rw-   0        0        0    21903 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/StlIterators.h
+-rw-rw-rw-   0        0        0     4299 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/Stride.h
+-rw-rw-rw-   0        0        0     2833 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/Swap.h
+-rw-rw-rw-   0        0        0    18010 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/Transpose.h
+-rw-rw-rw-   0        0        0    13860 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/Transpositions.h
+-rw-rw-rw-   0        0        0    39110 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/TriangularMatrix.h
+-rw-rw-rw-   0        0        0     3584 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/VectorBlock.h
+-rw-rw-rw-   0        0        0    35901 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/VectorwiseOp.h
+-rw-rw-rw-   0        0        0     9613 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/Visitor.h
+drwxrwxrwx   0        0        0        0 2023-07-12 05:46:17.400952 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/arch/
+drwxrwxrwx   0        0        0        0 2023-07-12 05:46:19.394882 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/arch/AVX/
+-rw-rw-rw-   0        0        0    17687 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/arch/AVX/Complex.h
+-rw-rw-rw-   0        0        0     8330 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/arch/AVX/MathFunctions.h
+-rw-rw-rw-   0        0        0    66422 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/arch/AVX/PacketMath.h
+-rw-rw-rw-   0        0        0     2679 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/arch/AVX/TypeCasting.h
+drwxrwxrwx   0        0        0        0 2023-07-12 05:46:19.411882 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/arch/AVX512/
+-rw-rw-rw-   0        0        0    18628 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/arch/AVX512/Complex.h
+-rw-rw-rw-   0        0        0    16230 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/arch/AVX512/MathFunctions.h
+-rw-rw-rw-   0        0        0    90467 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/arch/AVX512/PacketMath.h
+-rw-rw-rw-   0        0        0     2223 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/arch/AVX512/TypeCasting.h
+drwxrwxrwx   0        0        0        0 2023-07-12 05:46:19.439882 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/arch/AltiVec/
+-rw-rw-rw-   0        0        0    16847 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/arch/AltiVec/Complex.h
+-rw-rw-rw-   0        0        0     2413 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/arch/AltiVec/MathFunctions.h
+-rw-rw-rw-   0        0        0   120436 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/arch/AltiVec/MatrixProduct.h
+-rw-rw-rw-   0        0        0     5908 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/arch/AltiVec/MatrixProductCommon.h
+-rw-rw-rw-   0        0        0    31464 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/arch/AltiVec/MatrixProductMMA.h
+-rw-rw-rw-   0        0        0   102544 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/arch/AltiVec/PacketMath.h
+drwxrwxrwx   0        0        0        0 2023-07-12 05:46:19.443882 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/arch/CUDA/
+-rw-rw-rw-   0        0        0    16946 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/arch/CUDA/Complex.h
+drwxrwxrwx   0        0        0        0 2023-07-12 05:46:19.474883 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/arch/Default/
+-rw-rw-rw-   0        0        0    27842 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/arch/Default/BFloat16.h
+-rw-rw-rw-   0        0        0     2018 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/arch/Default/ConjHelper.h
+-rw-rw-rw-   0        0        0    69591 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/arch/Default/GenericPacketMathFunctions.h
+-rw-rw-rw-   0        0        0     4110 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/arch/Default/GenericPacketMathFunctionsFwd.h
+-rw-rw-rw-   0        0        0    35763 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/arch/Default/Half.h
+-rw-rw-rw-   0        0        0     1795 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/arch/Default/Settings.h
+-rw-rw-rw-   0        0        0     3866 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/arch/Default/TypeCasting.h
+drwxrwxrwx   0        0        0        0 2023-07-12 05:46:19.484947 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/arch/GPU/
+-rw-rw-rw-   0        0        0     2798 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/arch/GPU/MathFunctions.h
+-rw-rw-rw-   0        0        0    58732 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/arch/GPU/PacketMath.h
+-rw-rw-rw-   0        0        0     2336 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/arch/GPU/TypeCasting.h
+drwxrwxrwx   0        0        0        0 2023-07-12 05:46:17.398953 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/arch/HIP/
+drwxrwxrwx   0        0        0        0 2023-07-12 05:46:19.485916 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/arch/HIP/hcc/
+-rw-rw-rw-   0        0        0      714 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/arch/HIP/hcc/math_constants.h
+drwxrwxrwx   0        0        0        0 2023-07-12 05:46:19.500914 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/arch/MSA/
+-rw-rw-rw-   0        0        0    20551 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/arch/MSA/Complex.h
+-rw-rw-rw-   0        0        0    16546 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/arch/MSA/MathFunctions.h
+-rw-rw-rw-   0        0        0    34948 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/arch/MSA/PacketMath.h
+drwxrwxrwx   0        0        0        0 2023-07-12 05:46:19.523918 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/arch/NEON/
+-rw-rw-rw-   0        0        0    26566 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/arch/NEON/Complex.h
+-rw-rw-rw-   0        0        0     6998 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/arch/NEON/GeneralBlockPanelKernel.h
+-rw-rw-rw-   0        0        0     3158 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/arch/NEON/MathFunctions.h
+-rw-rw-rw-   0        0        0   200985 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/arch/NEON/PacketMath.h
+-rw-rw-rw-   0        0        0    52705 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/arch/NEON/TypeCasting.h
+drwxrwxrwx   0        0        0        0 2023-07-12 05:46:19.538953 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/arch/SSE/
+-rw-rw-rw-   0        0        0    19911 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/arch/SSE/Complex.h
+-rw-rw-rw-   0        0        0     6964 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/arch/SSE/MathFunctions.h
+-rw-rw-rw-   0        0        0    65976 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/arch/SSE/PacketMath.h
+-rw-rw-rw-   0        0        0     3792 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/arch/SSE/TypeCasting.h
+drwxrwxrwx   0        0        0        0 2023-07-12 05:46:19.550960 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/arch/SVE/
+-rw-rw-rw-   0        0        0     1238 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/arch/SVE/MathFunctions.h
+-rw-rw-rw-   0        0        0    22052 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/arch/SVE/PacketMath.h
+-rw-rw-rw-   0        0        0     1400 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/arch/SVE/TypeCasting.h
+drwxrwxrwx   0        0        0        0 2023-07-12 05:46:19.570913 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/arch/SYCL/
+-rw-rw-rw-   0        0        0     7660 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/arch/SYCL/InteropHeaders.h
+-rw-rw-rw-   0        0        0    12840 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/arch/SYCL/MathFunctions.h
+-rw-rw-rw-   0        0        0    28456 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/arch/SYCL/PacketMath.h
+-rw-rw-rw-   0        0        0    22550 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/arch/SYCL/SyclMemoryModel.h
+-rw-rw-rw-   0        0        0     2711 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/arch/SYCL/TypeCasting.h
+drwxrwxrwx   0        0        0        0 2023-07-12 05:46:19.584027 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/arch/ZVector/
+-rw-rw-rw-   0        0        0    20370 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/arch/ZVector/Complex.h
+-rw-rw-rw-   0        0        0     8257 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/arch/ZVector/MathFunctions.h
+-rw-rw-rw-   0        0        0    37940 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/arch/ZVector/PacketMath.h
+drwxrwxrwx   0        0        0        0 2023-07-12 05:46:19.607029 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/functors/
+-rw-rw-rw-   0        0        0     6863 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/functors/AssignmentFunctors.h
+-rw-rw-rw-   0        0        0    21424 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/functors/BinaryFunctors.h
+-rw-rw-rw-   0        0        0     8523 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/functors/NullaryFunctors.h
+-rw-rw-rw-   0        0        0     4481 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/functors/StlFunctors.h
+-rw-rw-rw-   0        0        0      632 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/functors/TernaryFunctors.h
+-rw-rw-rw-   0        0        0    41300 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/functors/UnaryFunctors.h
+drwxrwxrwx   0        0        0        0 2023-07-12 05:46:19.690927 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/products/
+-rw-rw-rw-   0        0        0   112056 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/products/GeneralBlockPanelKernel.h
+-rw-rw-rw-   0        0        0    20621 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/products/GeneralMatrixMatrix.h
+-rw-rw-rw-   0        0        0    16265 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/products/GeneralMatrixMatrixTriangular.h
+-rw-rw-rw-   0        0        0     7081 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/products/GeneralMatrixMatrixTriangular_BLAS.h
+-rw-rw-rw-   0        0        0     5230 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/products/GeneralMatrixMatrix_BLAS.h
+-rw-rw-rw-   0        0        0    22242 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/products/GeneralMatrixVector.h
+-rw-rw-rw-   0        0        0     6504 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/products/GeneralMatrixVector_BLAS.h
+-rw-rw-rw-   0        0        0     5762 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/products/Parallelizer.h
+-rw-rw-rw-   0        0        0    21898 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/products/SelfadjointMatrixMatrix.h
+-rw-rw-rw-   0        0        0    11865 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/products/SelfadjointMatrixMatrix_BLAS.h
+-rw-rw-rw-   0        0        0    10220 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/products/SelfadjointMatrixVector.h
+-rw-rw-rw-   0        0        0     5327 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/products/SelfadjointMatrixVector_BLAS.h
+-rw-rw-rw-   0        0        0     6297 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/products/SelfadjointProduct.h
+-rw-rw-rw-   0        0        0     4198 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/products/SelfadjointRank2Update.h
+-rw-rw-rw-   0        0        0    21459 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/products/TriangularMatrixMatrix.h
+-rw-rw-rw-   0        0        0    14184 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/products/TriangularMatrixMatrix_BLAS.h
+-rw-rw-rw-   0        0        0    15072 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/products/TriangularMatrixVector.h
+-rw-rw-rw-   0        0        0    10826 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/products/TriangularMatrixVector_BLAS.h
+-rw-rw-rw-   0        0        0    15015 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/products/TriangularSolverMatrix.h
+-rw-rw-rw-   0        0        0     6874 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/products/TriangularSolverMatrix_BLAS.h
+-rw-rw-rw-   0        0        0     6030 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/products/TriangularSolverVector.h
+drwxrwxrwx   0        0        0        0 2023-07-12 05:46:19.778654 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/util/
+-rw-rw-rw-   0        0        0    27402 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/util/BlasUtil.h
+-rw-rw-rw-   0        0        0    20388 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/util/ConfigureVectorization.h
+-rw-rw-rw-   0        0        0    22493 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/util/Constants.h
+-rw-rw-rw-   0        0        0     4998 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/util/DisableStupidWarnings.h
+-rw-rw-rw-   0        0        0    15877 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/util/ForwardDeclarations.h
+-rw-rw-rw-   0        0        0     6711 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/util/IndexedViewHelper.h
+-rw-rw-rw-   0        0        0    11167 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/util/IntegralConstant.h
+-rw-rw-rw-   0        0        0     4405 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/util/MKL_support.h
+-rw-rw-rw-   0        0        0    53933 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/util/Macros.h
+-rw-rw-rw-   0        0        0    47516 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/util/Memory.h
+-rw-rw-rw-   0        0        0    29449 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/util/Meta.h
+-rw-rw-rw-   0        0        0       88 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/util/NonMPL2.h
+-rw-rw-rw-   0        0        0     1055 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/util/ReenableStupidWarnings.h
+-rw-rw-rw-   0        0        0     1483 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/util/ReshapedHelper.h
+-rw-rw-rw-   0        0        0    10897 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/util/StaticAssert.h
+-rw-rw-rw-   0        0        0    12280 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/util/SymbolicIndex.h
+-rw-rw-rw-   0        0        0    36712 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/util/XprHelper.h
+drwxrwxrwx   0        0        0        0 2023-07-12 05:46:19.851645 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Eigenvalues/
+-rw-rw-rw-   0        0        0    12905 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Eigenvalues/ComplexEigenSolver.h
+-rw-rw-rw-   0        0        0    17736 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Eigenvalues/ComplexSchur.h
+-rw-rw-rw-   0        0        0     4269 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Eigenvalues/ComplexSchur_LAPACKE.h
+-rw-rw-rw-   0        0        0    23592 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Eigenvalues/EigenSolver.h
+-rw-rw-rw-   0        0        0    17594 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Eigenvalues/GeneralizedEigenSolver.h
+-rw-rw-rw-   0        0        0     9942 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Eigenvalues/GeneralizedSelfAdjointEigenSolver.h
+-rw-rw-rw-   0        0        0    14713 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Eigenvalues/HessenbergDecomposition.h
+-rw-rw-rw-   0        0        0     5733 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Eigenvalues/MatrixBaseEigenvalues.h
+-rw-rw-rw-   0        0        0    24297 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Eigenvalues/RealQZ.h
+-rw-rw-rw-   0        0        0    21636 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Eigenvalues/RealSchur.h
+-rw-rw-rw-   0        0        0     3727 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Eigenvalues/RealSchur_LAPACKE.h
+-rw-rw-rw-   0        0        0    34768 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Eigenvalues/SelfAdjointEigenSolver.h
+-rw-rw-rw-   0        0        0     4191 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Eigenvalues/SelfAdjointEigenSolver_LAPACKE.h
+-rw-rw-rw-   0        0        0    23099 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Eigenvalues/Tridiagonalization.h
+drwxrwxrwx   0        0        0        0 2023-07-12 05:46:19.914645 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Geometry/
+-rw-rw-rw-   0        0        0    19425 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Geometry/AlignedBox.h
+-rw-rw-rw-   0        0        0     8650 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Geometry/AngleAxis.h
+-rw-rw-rw-   0        0        0     3738 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Geometry/EulerAngles.h
+-rw-rw-rw-   0        0        0    21036 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Geometry/Homogeneous.h
+-rw-rw-rw-   0        0        0    12244 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Geometry/Hyperplane.h
+-rw-rw-rw-   0        0        0     9190 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Geometry/OrthoMethods.h
+-rw-rw-rw-   0        0        0    10044 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Geometry/ParametrizedLine.h
+-rw-rw-rw-   0        0        0    35237 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Geometry/Quaternion.h
+-rw-rw-rw-   0        0        0     7061 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Geometry/Rotation2D.h
+-rw-rw-rw-   0        0        0     8269 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Geometry/RotationBase.h
+-rw-rw-rw-   0        0        0     6912 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Geometry/Scaling.h
+-rw-rw-rw-   0        0        0    63473 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Geometry/Transform.h
+-rw-rw-rw-   0        0        0     7866 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Geometry/Translation.h
+-rw-rw-rw-   0        0        0     6356 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Geometry/Umeyama.h
+drwxrwxrwx   0        0        0        0 2023-07-12 05:46:19.918653 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Geometry/arch/
+-rw-rw-rw-   0        0        0     5841 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Geometry/arch/Geometry_SIMD.h
+drwxrwxrwx   0        0        0        0 2023-07-12 05:46:19.930653 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Householder/
+-rw-rw-rw-   0        0        0     4894 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Householder/BlockHouseholder.h
+-rw-rw-rw-   0        0        0     5541 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Householder/Householder.h
+-rw-rw-rw-   0        0        0    24114 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Householder/HouseholderSequence.h
+drwxrwxrwx   0        0        0        0 2023-07-12 05:46:19.960655 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/IterativeLinearSolvers/
+-rw-rw-rw-   0        0        0     6981 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/IterativeLinearSolvers/BasicPreconditioners.h
+-rw-rw-rw-   0        0        0     7062 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/IterativeLinearSolvers/BiCGSTAB.h
+-rw-rw-rw-   0        0        0     9116 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/IterativeLinearSolvers/ConjugateGradient.h
+-rw-rw-rw-   0        0        0    15442 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/IterativeLinearSolvers/IncompleteCholesky.h
+-rw-rw-rw-   0        0        0    15415 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/IterativeLinearSolvers/IncompleteLUT.h
+-rw-rw-rw-   0        0        0    13793 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/IterativeLinearSolvers/IterativeSolverBase.h
+-rw-rw-rw-   0        0        0     7547 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/IterativeLinearSolvers/LeastSquareConjugateGradient.h
+-rw-rw-rw-   0        0        0     4273 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/IterativeLinearSolvers/SolveWithGuess.h
+drwxrwxrwx   0        0        0        0 2023-07-12 05:46:19.964654 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Jacobi/
+-rw-rw-rw-   0        0        0    16866 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Jacobi/Jacobi.h
+drwxrwxrwx   0        0        0        0 2023-07-12 05:46:19.984728 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/LU/
+-rw-rw-rw-   0        0        0     3556 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/LU/Determinant.h
+-rw-rw-rw-   0        0        0    33188 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/LU/FullPivLU.h
+-rw-rw-rw-   0        0        0    15519 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/LU/InverseImpl.h
+-rw-rw-rw-   0        0        0    22475 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/LU/PartialPivLU.h
+-rw-rw-rw-   0        0        0     3638 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/LU/PartialPivLU_LAPACKE.h
+drwxrwxrwx   0        0        0        0 2023-07-12 05:46:19.989733 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/LU/arch/
+-rw-rw-rw-   0        0        0    13796 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/LU/arch/InverseSize4.h
+drwxrwxrwx   0        0        0        0 2023-07-12 05:46:20.004732 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/OrderingMethods/
+-rw-rw-rw-   0        0        0    16540 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/OrderingMethods/Amd.h
+-rw-rw-rw-   0        0        0    63544 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/OrderingMethods/Eigen_Colamd.h
+-rw-rw-rw-   0        0        0     5401 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/OrderingMethods/Ordering.h
+drwxrwxrwx   0        0        0        0 2023-07-12 05:46:20.034731 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/QR/
+-rw-rw-rw-   0        0        0    26172 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/QR/ColPivHouseholderQR.h
+-rw-rw-rw-   0        0        0     4759 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/QR/ColPivHouseholderQR_LAPACKE.h
+-rw-rw-rw-   0        0        0    24064 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/QR/CompleteOrthogonalDecomposition.h
+-rw-rw-rw-   0        0        0    27481 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/QR/FullPivHouseholderQR.h
+-rw-rw-rw-   0        0        0    15075 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/QR/HouseholderQR.h
+-rw-rw-rw-   0        0        0     3061 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/QR/HouseholderQR_LAPACKE.h
+drwxrwxrwx   0        0        0        0 2023-07-12 05:46:20.059650 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/SVD/
+-rw-rw-rw-   0        0        0    54995 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/SVD/BDCSVD.h
+-rw-rw-rw-   0        0        0    33798 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/SVD/JacobiSVD.h
+-rw-rw-rw-   0        0        0     5190 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/SVD/JacobiSVD_LAPACKE.h
+-rw-rw-rw-   0        0        0    14620 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/SVD/SVDBase.h
+-rw-rw-rw-   0        0        0    16371 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/SVD/UpperBidiagonalization.h
+drwxrwxrwx   0        0        0        0 2023-07-12 05:46:20.069654 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/SparseCholesky/
+-rw-rw-rw-   0        0        0    25058 2023-01-16 21:22:35.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/SparseCholesky/SimplicialCholesky.h
+-rw-rw-rw-   0        0        0     6121 2023-01-17 05:50:15.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/SparseCholesky/SimplicialCholesky_impl.h
+drwxrwxrwx   0        0        0        0 2023-07-12 05:46:20.204655 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/SparseCore/
+-rw-rw-rw-   0        0        0    11048 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/SparseCore/AmbiVector.h
+-rw-rw-rw-   0        0        0     9017 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/SparseCore/CompressedStorage.h
+-rw-rw-rw-   0        0        0    13518 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/SparseCore/ConservativeSparseSparseProduct.h
+-rw-rw-rw-   0        0        0     2258 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/SparseCore/MappedSparseMatrix.h
+-rw-rw-rw-   0        0        0    11638 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/SparseCore/SparseAssign.h
+-rw-rw-rw-   0        0        0    24931 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/SparseCore/SparseBlock.h
+-rw-rw-rw-   0        0        0     6691 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/SparseCore/SparseColEtree.h
+-rw-rw-rw-   0        0        0    13976 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/SparseCore/SparseCompressedBase.h
+-rw-rw-rw-   0        0        0    26156 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/SparseCore/SparseCwiseBinaryOp.h
+-rw-rw-rw-   0        0        0     4887 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/SparseCore/SparseCwiseUnaryOp.h
+-rw-rw-rw-   0        0        0    13598 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/SparseCore/SparseDenseProduct.h
+-rw-rw-rw-   0        0        0     5946 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/SparseCore/SparseDiagonalProduct.h
+-rw-rw-rw-   0        0        0     3178 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/SparseCore/SparseDot.h
+-rw-rw-rw-   0        0        0     1136 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/SparseCore/SparseFuzzy.h
+-rw-rw-rw-   0        0        0    12894 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/SparseCore/SparseMap.h
+-rw-rw-rw-   0        0        0    58993 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/SparseCore/SparseMatrix.h
+-rw-rw-rw-   0        0        0    17849 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/SparseCore/SparseMatrixBase.h
+-rw-rw-rw-   0        0        0     7507 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/SparseCore/SparsePermutation.h
+-rw-rw-rw-   0        0        0     7774 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/SparseCore/SparseProduct.h
+-rw-rw-rw-   0        0        0     1748 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/SparseCore/SparseRedux.h
+-rw-rw-rw-   0        0        0    15997 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/SparseCore/SparseRef.h
+-rw-rw-rw-   0        0        0    26548 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/SparseCore/SparseSelfAdjointView.h
+-rw-rw-rw-   0        0        0     4548 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/SparseCore/SparseSolverBase.h
+-rw-rw-rw-   0        0        0     8902 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/SparseCore/SparseSparseProductWithPruning.h
+-rw-rw-rw-   0        0        0     3267 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/SparseCore/SparseTranspose.h
+-rw-rw-rw-   0        0        0     6626 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/SparseCore/SparseTriangularView.h
+-rw-rw-rw-   0        0        0     7013 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/SparseCore/SparseUtil.h
+-rw-rw-rw-   0        0        0    15310 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/SparseCore/SparseVector.h
+-rw-rw-rw-   0        0        0     8381 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/SparseCore/SparseView.h
+-rw-rw-rw-   0        0        0     9972 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/SparseCore/TriangularSolver.h
+drwxrwxrwx   0        0        0        0 2023-07-12 05:46:20.277653 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/SparseLU/
+-rw-rw-rw-   0        0        0    34239 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/SparseLU/SparseLU.h
+-rw-rw-rw-   0        0        0     4369 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/SparseLU/SparseLUImpl.h
+-rw-rw-rw-   0        0        0     7828 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/SparseLU/SparseLU_Memory.h
+-rw-rw-rw-   0        0        0     5084 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/SparseLU/SparseLU_Structs.h
+-rw-rw-rw-   0        0        0    13212 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/SparseLU/SparseLU_SupernodalMatrix.h
+-rw-rw-rw-   0        0        0     2129 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/SparseLU/SparseLU_Utils.h
+-rw-rw-rw-   0        0        0     6893 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/SparseLU/SparseLU_column_bmod.h
+-rw-rw-rw-   0        0        0     6763 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/SparseLU/SparseLU_column_dfs.h
+-rw-rw-rw-   0        0        0     3788 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/SparseLU/SparseLU_copy_to_ucol.h
+-rw-rw-rw-   0        0        0    10497 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/SparseLU/SparseLU_gemm_kernel.h
+-rw-rw-rw-   0        0        0     4307 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/SparseLU/SparseLU_heap_relax_snode.h
+-rw-rw-rw-   0        0        0     5853 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/SparseLU/SparseLU_kernel_bmod.h
+-rw-rw-rw-   0        0        0     8708 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/SparseLU/SparseLU_panel_bmod.h
+-rw-rw-rw-   0        0        0     9286 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/SparseLU/SparseLU_panel_dfs.h
+-rw-rw-rw-   0        0        0     5116 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/SparseLU/SparseLU_pivotL.h
+-rw-rw-rw-   0        0        0     4681 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/SparseLU/SparseLU_pruneL.h
+-rw-rw-rw-   0        0        0     2972 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/SparseLU/SparseLU_relax_snode.h
+drwxrwxrwx   0        0        0        0 2023-07-12 05:46:20.282652 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/SparseQR/
+-rw-rw-rw-   0        0        0    29925 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/SparseQR/SparseQR.h
+drwxrwxrwx   0        0        0        0 2023-07-12 05:46:20.313653 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/misc/
+-rw-rw-rw-   0        0        0     2995 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/misc/Image.h
+-rw-rw-rw-   0        0        0     2821 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/misc/Kernel.h
+-rw-rw-rw-   0        0        0     1803 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/misc/RealSvd2x2.h
+-rw-rw-rw-   0        0        0    31000 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/misc/blas.h
+-rw-rw-rw-   0        0        0     7986 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/misc/lapack.h
+-rw-rw-rw-   0        0        0  1074661 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/misc/lapacke.h
+-rw-rw-rw-   0        0        0      491 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/misc/lapacke_mangling.h
+drwxrwxrwx   0        0        0        0 2023-07-12 05:46:20.358670 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/plugins/
+-rw-rw-rw-   0        0        0    14418 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/plugins/ArrayCwiseBinaryOps.h
+-rw-rw-rw-   0        0        0    21084 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/plugins/ArrayCwiseUnaryOps.h
+-rw-rw-rw-   0        0        0    60448 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/plugins/BlockMethods.h
+-rw-rw-rw-   0        0        0     4943 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/plugins/CommonCwiseBinaryOps.h
+-rw-rw-rw-   0        0        0     7431 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/plugins/CommonCwiseUnaryOps.h
+-rw-rw-rw-   0        0        0    12545 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/plugins/IndexedViewMethods.h
+-rw-rw-rw-   0        0        0     6527 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/plugins/MatrixCwiseBinaryOps.h
+-rw-rw-rw-   0        0        0     3445 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/plugins/MatrixCwiseUnaryOps.h
+-rw-rw-rw-   0        0        0     7064 2021-03-12 08:57:32.000000 gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/plugins/ReshapedMethods.h
+drwxrwxrwx   0        0        0        0 2023-07-12 05:46:20.372724 gpboost-1.2.2/compile/external_libs/fast_double_parser/
+-rw-rw-rw-   0        0        0     2661 2021-01-29 13:27:40.000000 gpboost-1.2.2/compile/external_libs/fast_double_parser/CMakeLists.txt
+-rw-rw-rw-   0        0        0    11544 2021-01-29 13:27:40.000000 gpboost-1.2.2/compile/external_libs/fast_double_parser/LICENSE
+-rw-rw-rw-   0        0        0     1392 2021-01-29 13:27:40.000000 gpboost-1.2.2/compile/external_libs/fast_double_parser/LICENSE.BSL
+drwxrwxrwx   0        0        0        0 2023-07-12 05:46:20.377728 gpboost-1.2.2/compile/external_libs/fast_double_parser/include/
+-rw-rw-rw-   0        0        0    50746 2021-01-29 13:27:40.000000 gpboost-1.2.2/compile/external_libs/fast_double_parser/include/fast_double_parser.h
+drwxrwxrwx   0        0        0        0 2023-07-12 05:46:20.386726 gpboost-1.2.2/compile/external_libs/fmt/
+-rw-rw-rw-   0        0        0    13412 2021-01-29 13:27:53.000000 gpboost-1.2.2/compile/external_libs/fmt/CMakeLists.txt
+-rw-rw-rw-   0        0        0     1435 2021-01-29 13:27:53.000000 gpboost-1.2.2/compile/external_libs/fmt/LICENSE.rst
+drwxrwxrwx   0        0        0        0 2023-07-12 05:46:17.412980 gpboost-1.2.2/compile/external_libs/fmt/include/
+drwxrwxrwx   0        0        0        0 2023-07-12 05:46:20.438736 gpboost-1.2.2/compile/external_libs/fmt/include/fmt/
+-rw-rw-rw-   0        0        0    36920 2021-01-29 13:27:53.000000 gpboost-1.2.2/compile/external_libs/fmt/include/fmt/chrono.h
+-rw-rw-rw-   0        0        0    24252 2021-01-29 13:27:53.000000 gpboost-1.2.2/compile/external_libs/fmt/include/fmt/color.h
+-rw-rw-rw-   0        0        0    24772 2021-01-29 13:27:53.000000 gpboost-1.2.2/compile/external_libs/fmt/include/fmt/compile.h
+-rw-rw-rw-   0        0        0    73420 2021-01-29 13:27:53.000000 gpboost-1.2.2/compile/external_libs/fmt/include/fmt/core.h
+-rw-rw-rw-   0        0        0   112636 2021-01-29 13:27:53.000000 gpboost-1.2.2/compile/external_libs/fmt/include/fmt/format-inl.h
+-rw-rw-rw-   0        0        0   136849 2021-01-29 13:27:53.000000 gpboost-1.2.2/compile/external_libs/fmt/include/fmt/format.h
+-rw-rw-rw-   0        0        0     2383 2021-01-29 13:27:53.000000 gpboost-1.2.2/compile/external_libs/fmt/include/fmt/locale.h
+-rw-rw-rw-   0        0        0    14160 2021-01-29 13:27:53.000000 gpboost-1.2.2/compile/external_libs/fmt/include/fmt/os.h
+-rw-rw-rw-   0        0        0     6082 2021-01-29 13:27:53.000000 gpboost-1.2.2/compile/external_libs/fmt/include/fmt/ostream.h
+-rw-rw-rw-   0        0        0       77 2021-01-29 13:27:53.000000 gpboost-1.2.2/compile/external_libs/fmt/include/fmt/posix.h
+-rw-rw-rw-   0        0        0    24008 2021-01-29 13:27:53.000000 gpboost-1.2.2/compile/external_libs/fmt/include/fmt/printf.h
+-rw-rw-rw-   0        0        0    12939 2021-01-29 13:27:53.000000 gpboost-1.2.2/compile/external_libs/fmt/include/fmt/ranges.h
+drwxrwxrwx   0        0        0        0 2023-07-12 05:46:17.413987 gpboost-1.2.2/compile/include/
+drwxrwxrwx   0        0        0        0 2023-07-12 05:46:20.489644 gpboost-1.2.2/compile/include/GPBoost/
+-rw-rw-rw-   0        0        0     3291 2023-02-22 08:53:45.000000 gpboost-1.2.2/compile/include/GPBoost/DF_utils.h
+-rw-rw-rw-   0        0        0    10592 2023-06-16 12:23:42.000000 gpboost-1.2.2/compile/include/GPBoost/GP_utils.h
+-rw-rw-rw-   0        0        0     2966 2023-02-16 13:06:27.000000 gpboost-1.2.2/compile/include/GPBoost/Vecchia_utils.h
+-rw-rw-rw-   0        0        0    37137 2023-03-21 14:12:45.000000 gpboost-1.2.2/compile/include/GPBoost/cov_fcts.h
+-rw-rw-rw-   0        0        0   159122 2023-07-11 08:48:23.000000 gpboost-1.2.2/compile/include/GPBoost/likelihoods.h
+-rw-rw-rw-   0        0        0    58750 2023-03-23 10:35:29.000000 gpboost-1.2.2/compile/include/GPBoost/re_comp.h
+-rw-rw-rw-   0        0        0    25805 2023-06-08 12:21:36.000000 gpboost-1.2.2/compile/include/GPBoost/re_model.h
+-rw-rw-rw-   0        0        0   372256 2023-07-10 13:01:24.000000 gpboost-1.2.2/compile/include/GPBoost/re_model_template.h
+-rw-rw-rw-   0        0        0    20177 2023-03-01 14:13:16.000000 gpboost-1.2.2/compile/include/GPBoost/sparse_matrix_utils.h
+-rw-rw-rw-   0        0        0     2519 2023-01-18 12:49:42.000000 gpboost-1.2.2/compile/include/GPBoost/type_defs.h
+-rw-rw-rw-   0        0        0     5255 2023-06-12 14:01:00.000000 gpboost-1.2.2/compile/include/GPBoost/utils.h
+drwxrwxrwx   0        0        0        0 2023-07-12 05:46:20.568652 gpboost-1.2.2/compile/include/LightGBM/
+-rw-rw-rw-   0        0        0     2442 2021-01-29 13:27:06.000000 gpboost-1.2.2/compile/include/LightGBM/application.h
+-rw-rw-rw-   0        0        0    17644 2021-01-29 13:27:06.000000 gpboost-1.2.2/compile/include/LightGBM/bin.h
+-rw-rw-rw-   0        0        0    11258 2021-01-29 13:27:06.000000 gpboost-1.2.2/compile/include/LightGBM/boosting.h
+-rw-rw-rw-   0        0        0    92126 2023-06-08 12:32:18.000000 gpboost-1.2.2/compile/include/LightGBM/c_api.h
+-rw-rw-rw-   0        0        0    69980 2023-06-08 08:36:07.000000 gpboost-1.2.2/compile/include/LightGBM/config.h
+drwxrwxrwx   0        0        0        0 2023-07-12 05:46:20.577652 gpboost-1.2.2/compile/include/LightGBM/cuda/
+-rw-rw-rw-   0        0        0      716 2021-01-29 13:27:06.000000 gpboost-1.2.2/compile/include/LightGBM/cuda/cuda_utils.h
+-rw-rw-rw-   0        0        0     2550 2021-01-29 13:27:06.000000 gpboost-1.2.2/compile/include/LightGBM/cuda/vector_cudahost.h
+-rw-rw-rw-   0        0        0    25455 2021-01-29 13:27:06.000000 gpboost-1.2.2/compile/include/LightGBM/dataset.h
+-rw-rw-rw-   0        0        0     3760 2021-01-29 13:27:06.000000 gpboost-1.2.2/compile/include/LightGBM/dataset_loader.h
+-rw-rw-rw-   0        0        0      643 2022-01-18 10:17:34.000000 gpboost-1.2.2/compile/include/LightGBM/export.h
+-rw-rw-rw-   0        0        0    19974 2021-01-29 13:27:06.000000 gpboost-1.2.2/compile/include/LightGBM/feature_group.h
+-rw-rw-rw-   0        0        0     2992 2023-05-26 15:59:37.000000 gpboost-1.2.2/compile/include/LightGBM/meta.h
+-rw-rw-rw-   0        0        0     4618 2022-07-18 13:57:09.000000 gpboost-1.2.2/compile/include/LightGBM/metric.h
+-rw-rw-rw-   0        0        0     1305 2023-03-08 16:18:29.000000 gpboost-1.2.2/compile/include/LightGBM/nesterov_boosting.h
+-rw-rw-rw-   0        0        0    12281 2021-08-17 07:03:57.000000 gpboost-1.2.2/compile/include/LightGBM/network.h
+-rw-rw-rw-   0        0        0     5021 2022-07-18 13:42:05.000000 gpboost-1.2.2/compile/include/LightGBM/objective_function.h
+-rw-rw-rw-   0        0        0     1312 2021-01-29 13:27:06.000000 gpboost-1.2.2/compile/include/LightGBM/prediction_early_stop.h
+-rw-rw-rw-   0        0        0     8210 2021-01-29 13:27:06.000000 gpboost-1.2.2/compile/include/LightGBM/train_share_states.h
+-rw-rw-rw-   0        0        0    26928 2021-01-29 13:27:06.000000 gpboost-1.2.2/compile/include/LightGBM/tree.h
+-rw-rw-rw-   0        0        0     4000 2021-02-02 09:08:55.000000 gpboost-1.2.2/compile/include/LightGBM/tree_learner.h
+drwxrwxrwx   0        0        0        0 2023-07-12 05:46:20.624006 gpboost-1.2.2/compile/include/LightGBM/utils/
+-rw-rw-rw-   0        0        0     5094 2021-01-29 13:27:06.000000 gpboost-1.2.2/compile/include/LightGBM/utils/array_args.h
+-rw-rw-rw-   0        0        0    35505 2022-11-18 12:31:49.000000 gpboost-1.2.2/compile/include/LightGBM/utils/common.h
+-rw-rw-rw-   0        0        0     5331 2021-01-29 13:27:06.000000 gpboost-1.2.2/compile/include/LightGBM/utils/common_legacy_solaris.h
+-rw-rw-rw-   0        0        0     2753 2021-01-29 13:27:06.000000 gpboost-1.2.2/compile/include/LightGBM/utils/file_io.h
+-rw-rw-rw-   0        0        0     9232 2021-01-29 13:27:06.000000 gpboost-1.2.2/compile/include/LightGBM/utils/json11.h
+-rw-rw-rw-   0        0        0     7042 2022-12-14 12:42:54.000000 gpboost-1.2.2/compile/include/LightGBM/utils/log.h
+-rw-rw-rw-   0        0        0     2391 2021-01-29 13:27:06.000000 gpboost-1.2.2/compile/include/LightGBM/utils/openmp_wrapper.h
+-rw-rw-rw-   0        0        0     2170 2021-01-29 13:27:06.000000 gpboost-1.2.2/compile/include/LightGBM/utils/pipeline_reader.h
+-rw-rw-rw-   0        0        0     3025 2021-01-29 13:27:06.000000 gpboost-1.2.2/compile/include/LightGBM/utils/random.h
+-rw-rw-rw-   0        0        0    11689 2021-01-29 13:27:06.000000 gpboost-1.2.2/compile/include/LightGBM/utils/text_reader.h
+-rw-rw-rw-   0        0        0     6744 2021-01-29 13:27:06.000000 gpboost-1.2.2/compile/include/LightGBM/utils/threading.h
+drwxrwxrwx   0        0        0        0 2023-07-12 05:46:20.635985 gpboost-1.2.2/compile/include/LightGBM/utils/yamc/
+-rw-rw-rw-   0        0        0     6461 2021-01-29 13:27:06.000000 gpboost-1.2.2/compile/include/LightGBM/utils/yamc/alternate_shared_mutex.hpp
+-rw-rw-rw-   0        0        0     4492 2021-01-29 13:27:06.000000 gpboost-1.2.2/compile/include/LightGBM/utils/yamc/yamc_rwlock_sched.hpp
+-rw-rw-rw-   0        0        0     5247 2021-01-29 13:27:06.000000 gpboost-1.2.2/compile/include/LightGBM/utils/yamc/yamc_shared_lock.hpp
+drwxrwxrwx   0        0        0        0 2023-07-12 05:46:17.418952 gpboost-1.2.2/compile/src/
+drwxrwxrwx   0        0        0        0 2023-07-12 05:46:20.659959 gpboost-1.2.2/compile/src/GPBoost/
+-rw-rw-rw-   0        0        0     5769 2023-06-05 13:51:38.000000 gpboost-1.2.2/compile/src/GPBoost/DF_utils.cpp
+-rw-rw-rw-   0        0        0     1688 2023-03-23 08:06:54.000000 gpboost-1.2.2/compile/src/GPBoost/GP_utils.cpp
+-rw-rw-rw-   0        0        0    12100 2023-03-22 13:36:07.000000 gpboost-1.2.2/compile/src/GPBoost/Vecchia_utils.cpp
+-rw-rw-rw-   0        0        0    35151 2023-06-08 12:23:19.000000 gpboost-1.2.2/compile/src/GPBoost/re_model.cpp
+-rw-rw-rw-   0        0        0    11520 2023-01-18 10:31:49.000000 gpboost-1.2.2/compile/src/GPBoost/sparse_matrix_utils.cpp
+drwxrwxrwx   0        0        0        0 2023-07-12 05:46:20.669958 gpboost-1.2.2/compile/src/LightGBM/
+drwxrwxrwx   0        0        0        0 2023-07-12 05:46:20.679067 gpboost-1.2.2/compile/src/LightGBM/application/
+-rw-rw-rw-   0        0        0    10556 2021-01-29 13:27:06.000000 gpboost-1.2.2/compile/src/LightGBM/application/application.cpp
+-rw-rw-rw-   0        0        0    12217 2021-01-29 13:27:06.000000 gpboost-1.2.2/compile/src/LightGBM/application/predictor.hpp
+drwxrwxrwx   0        0        0        0 2023-07-12 05:46:20.725959 gpboost-1.2.2/compile/src/LightGBM/boosting/
+-rw-rw-rw-   0        0        0     2299 2021-01-29 13:27:06.000000 gpboost-1.2.2/compile/src/LightGBM/boosting/boosting.cpp
+-rw-rw-rw-   0        0        0     7604 2021-01-29 13:27:06.000000 gpboost-1.2.2/compile/src/LightGBM/boosting/dart.hpp
+-rw-rw-rw-   0        0        0    35974 2023-06-07 14:42:25.000000 gpboost-1.2.2/compile/src/LightGBM/boosting/gbdt.cpp
+-rw-rw-rw-   0        0        0    21149 2023-03-08 16:27:29.000000 gpboost-1.2.2/compile/src/LightGBM/boosting/gbdt.h
+-rw-rw-rw-   0        0        0    25165 2023-03-08 16:17:44.000000 gpboost-1.2.2/compile/src/LightGBM/boosting/gbdt_model_text.cpp
+-rw-rw-rw-   0        0        0     5028 2023-03-08 16:18:13.000000 gpboost-1.2.2/compile/src/LightGBM/boosting/gbdt_prediction.cpp
+-rw-rw-rw-   0        0        0     6952 2021-01-29 13:27:06.000000 gpboost-1.2.2/compile/src/LightGBM/boosting/goss.hpp
+-rw-rw-rw-   0        0        0     2643 2021-01-29 13:27:06.000000 gpboost-1.2.2/compile/src/LightGBM/boosting/prediction_early_stop.cpp
+-rw-rw-rw-   0        0        0     8180 2021-01-29 13:27:06.000000 gpboost-1.2.2/compile/src/LightGBM/boosting/rf.hpp
+-rw-rw-rw-   0        0        0     6352 2023-03-08 16:18:22.000000 gpboost-1.2.2/compile/src/LightGBM/boosting/score_updater.hpp
+-rw-rw-rw-   0        0        0   102606 2023-06-10 06:06:39.000000 gpboost-1.2.2/compile/src/LightGBM/c_api.cpp
+drwxrwxrwx   0        0        0        0 2023-07-12 05:46:20.792550 gpboost-1.2.2/compile/src/LightGBM/io/
+-rw-rw-rw-   0        0        0    30211 2021-01-29 13:27:06.000000 gpboost-1.2.2/compile/src/LightGBM/io/bin.cpp
+-rw-rw-rw-   0        0        0    17277 2023-06-08 05:27:49.000000 gpboost-1.2.2/compile/src/LightGBM/io/config.cpp
+-rw-rw-rw-   0        0        0    27684 2023-06-08 10:01:19.000000 gpboost-1.2.2/compile/src/LightGBM/io/config_auto.cpp
+-rw-rw-rw-   0        0        0    58412 2023-05-26 15:43:08.000000 gpboost-1.2.2/compile/src/LightGBM/io/dataset.cpp
+-rw-rw-rw-   0        0        0    61416 2021-01-29 13:27:06.000000 gpboost-1.2.2/compile/src/LightGBM/io/dataset_loader.cpp
+-rw-rw-rw-   0        0        0    18916 2021-01-29 13:27:06.000000 gpboost-1.2.2/compile/src/LightGBM/io/dense_bin.hpp
+-rw-rw-rw-   0        0        0     5635 2021-01-29 13:27:06.000000 gpboost-1.2.2/compile/src/LightGBM/io/file_io.cpp
+-rw-rw-rw-   0        0        0    23192 2023-01-11 16:33:16.000000 gpboost-1.2.2/compile/src/LightGBM/io/json11.cpp
+-rw-rw-rw-   0        0        0    20698 2022-11-18 12:33:52.000000 gpboost-1.2.2/compile/src/LightGBM/io/metadata.cpp
+-rw-rw-rw-   0        0        0     8717 2021-01-29 13:27:06.000000 gpboost-1.2.2/compile/src/LightGBM/io/multi_val_dense_bin.hpp
+-rw-rw-rw-   0        0        0    12550 2021-01-29 13:27:06.000000 gpboost-1.2.2/compile/src/LightGBM/io/multi_val_sparse_bin.hpp
+-rw-rw-rw-   0        0        0     8131 2021-01-29 13:27:06.000000 gpboost-1.2.2/compile/src/LightGBM/io/parser.cpp
+-rw-rw-rw-   0        0        0     3643 2021-01-29 13:27:06.000000 gpboost-1.2.2/compile/src/LightGBM/io/parser.hpp
+-rw-rw-rw-   0        0        0    23759 2021-01-29 13:27:06.000000 gpboost-1.2.2/compile/src/LightGBM/io/sparse_bin.hpp
+-rw-rw-rw-   0        0        0    16886 2021-01-29 13:27:06.000000 gpboost-1.2.2/compile/src/LightGBM/io/train_share_states.cpp
+-rw-rw-rw-   0        0        0    42401 2021-01-29 13:27:06.000000 gpboost-1.2.2/compile/src/LightGBM/io/tree.cpp
+-rw-rw-rw-   0        0        0      954 2021-01-29 13:27:06.000000 gpboost-1.2.2/compile/src/LightGBM/main.cpp
+drwxrwxrwx   0        0        0        0 2023-07-12 05:46:20.831550 gpboost-1.2.2/compile/src/LightGBM/metric/
+-rw-rw-rw-   0        0        0    14303 2023-06-08 12:34:32.000000 gpboost-1.2.2/compile/src/LightGBM/metric/binary_metric.hpp
+-rw-rw-rw-   0        0        0     5842 2021-01-29 13:27:06.000000 gpboost-1.2.2/compile/src/LightGBM/metric/dcg_calculator.cpp
+-rw-rw-rw-   0        0        0     5697 2022-07-18 14:03:05.000000 gpboost-1.2.2/compile/src/LightGBM/metric/map_metric.hpp
+-rw-rw-rw-   0        0        0     3330 2023-06-05 15:51:25.000000 gpboost-1.2.2/compile/src/LightGBM/metric/metric.cpp
+-rw-rw-rw-   0        0        0    13595 2022-07-18 14:03:24.000000 gpboost-1.2.2/compile/src/LightGBM/metric/multiclass_metric.hpp
+-rw-rw-rw-   0        0        0     3295 2022-07-18 13:57:02.000000 gpboost-1.2.2/compile/src/LightGBM/metric/random_effects_metric.hpp
+-rw-rw-rw-   0        0        0     6163 2022-07-18 14:03:36.000000 gpboost-1.2.2/compile/src/LightGBM/metric/rank_metric.hpp
+-rw-rw-rw-   0        0        0    18729 2023-06-08 12:34:13.000000 gpboost-1.2.2/compile/src/LightGBM/metric/regression_metric.hpp
+-rw-rw-rw-   0        0        0    13207 2022-07-18 14:03:59.000000 gpboost-1.2.2/compile/src/LightGBM/metric/xentropy_metric.hpp
+drwxrwxrwx   0        0        0        0 2023-07-12 05:46:20.864506 gpboost-1.2.2/compile/src/LightGBM/network/
+-rw-rw-rw-   0        0        0     3607 2021-01-29 13:27:06.000000 gpboost-1.2.2/compile/src/LightGBM/network/ifaddrs_patch.cpp
+-rw-rw-rw-   0        0        0      944 2021-01-29 13:27:06.000000 gpboost-1.2.2/compile/src/LightGBM/network/ifaddrs_patch.h
+-rw-rw-rw-   0        0        0     6410 2021-01-29 13:27:06.000000 gpboost-1.2.2/compile/src/LightGBM/network/linker_topo.cpp
+-rw-rw-rw-   0        0        0     9330 2021-01-29 13:27:06.000000 gpboost-1.2.2/compile/src/LightGBM/network/linkers.h
+-rw-rw-rw-   0        0        0     1901 2021-01-29 13:27:06.000000 gpboost-1.2.2/compile/src/LightGBM/network/linkers_mpi.cpp
+-rw-rw-rw-   0        0        0     7905 2021-01-29 13:27:06.000000 gpboost-1.2.2/compile/src/LightGBM/network/linkers_socket.cpp
+-rw-rw-rw-   0        0        0    14102 2021-08-17 07:04:55.000000 gpboost-1.2.2/compile/src/LightGBM/network/network.cpp
+-rw-rw-rw-   0        0        0     8890 2022-01-14 16:36:55.000000 gpboost-1.2.2/compile/src/LightGBM/network/socket_wrapper.hpp
+drwxrwxrwx   0        0        0        0 2023-07-12 05:46:20.891138 gpboost-1.2.2/compile/src/LightGBM/objective/
+-rw-rw-rw-   0        0        0     7605 2021-02-03 09:55:22.000000 gpboost-1.2.2/compile/src/LightGBM/objective/binary_objective.hpp
+-rw-rw-rw-   0        0        0     9194 2021-01-29 13:27:06.000000 gpboost-1.2.2/compile/src/LightGBM/objective/multiclass_objective.hpp
+-rw-rw-rw-   0        0        0     5549 2023-06-08 04:45:15.000000 gpboost-1.2.2/compile/src/LightGBM/objective/objective_function.cpp
+-rw-rw-rw-   0        0        0    13401 2021-01-29 13:27:06.000000 gpboost-1.2.2/compile/src/LightGBM/objective/rank_objective.hpp
+-rw-rw-rw-   0        0        0    35283 2023-06-10 06:07:26.000000 gpboost-1.2.2/compile/src/LightGBM/objective/regression_objective.hpp
+-rw-rw-rw-   0        0        0     9779 2021-01-29 13:27:06.000000 gpboost-1.2.2/compile/src/LightGBM/objective/xentropy_objective.hpp
+drwxrwxrwx   0        0        0        0 2023-07-12 05:46:20.984087 gpboost-1.2.2/compile/src/LightGBM/treelearner/
+-rw-rw-rw-   0        0        0     8004 2021-01-29 13:27:06.000000 gpboost-1.2.2/compile/src/LightGBM/treelearner/col_sampler.hpp
+-rw-rw-rw-   0        0        0     6267 2021-01-29 13:27:06.000000 gpboost-1.2.2/compile/src/LightGBM/treelearner/cost_effective_gradient_boosting.hpp
+-rw-rw-rw-   0        0        0     7898 2021-01-29 13:27:06.000000 gpboost-1.2.2/compile/src/LightGBM/treelearner/cuda_kernel_launcher.cu
+-rw-rw-rw-   0        0        0     2662 2021-01-29 13:27:06.000000 gpboost-1.2.2/compile/src/LightGBM/treelearner/cuda_kernel_launcher.h
+-rw-rw-rw-   0        0        0    41258 2021-01-29 13:27:06.000000 gpboost-1.2.2/compile/src/LightGBM/treelearner/cuda_tree_learner.cpp
+-rw-rw-rw-   0        0        0    11541 2021-01-29 13:27:06.000000 gpboost-1.2.2/compile/src/LightGBM/treelearner/cuda_tree_learner.h
+-rw-rw-rw-   0        0        0    12159 2021-01-29 13:27:06.000000 gpboost-1.2.2/compile/src/LightGBM/treelearner/data_parallel_tree_learner.cpp
+-rw-rw-rw-   0        0        0     5831 2021-01-29 13:27:06.000000 gpboost-1.2.2/compile/src/LightGBM/treelearner/data_partition.hpp
+-rw-rw-rw-   0        0        0    52366 2021-09-20 10:49:45.000000 gpboost-1.2.2/compile/src/LightGBM/treelearner/feature_histogram.hpp
+-rw-rw-rw-   0        0        0     3634 2021-01-29 13:27:06.000000 gpboost-1.2.2/compile/src/LightGBM/treelearner/feature_parallel_tree_learner.cpp
+-rw-rw-rw-   0        0        0    54339 2021-01-29 13:27:06.000000 gpboost-1.2.2/compile/src/LightGBM/treelearner/gpu_tree_learner.cpp
+-rw-rw-rw-   0        0        0    11788 2021-01-29 13:27:06.000000 gpboost-1.2.2/compile/src/LightGBM/treelearner/gpu_tree_learner.h
+drwxrwxrwx   0        0        0        0 2023-07-12 05:46:20.992087 gpboost-1.2.2/compile/src/LightGBM/treelearner/kernels/
+-rw-rw-rw-   0        0        0    37797 2021-01-29 13:27:06.000000 gpboost-1.2.2/compile/src/LightGBM/treelearner/kernels/histogram_16_64_256.cu
+-rw-rw-rw-   0        0        0     5555 2021-01-29 13:27:06.000000 gpboost-1.2.2/compile/src/LightGBM/treelearner/kernels/histogram_16_64_256.hu
+-rw-rw-rw-   0        0        0     5328 2021-01-29 13:27:06.000000 gpboost-1.2.2/compile/src/LightGBM/treelearner/leaf_splits.hpp
+-rw-rw-rw-   0        0        0    15019 2021-01-29 13:27:06.000000 gpboost-1.2.2/compile/src/LightGBM/treelearner/linear_tree_learner.cpp
+-rw-rw-rw-   0        0        0     4837 2021-01-29 13:27:06.000000 gpboost-1.2.2/compile/src/LightGBM/treelearner/linear_tree_learner.h
+-rw-rw-rw-   0        0        0    49014 2021-01-29 13:27:06.000000 gpboost-1.2.2/compile/src/LightGBM/treelearner/monotone_constraints.hpp
+drwxrwxrwx   0        0        0        0 2023-07-12 05:46:21.005092 gpboost-1.2.2/compile/src/LightGBM/treelearner/ocl/
+-rw-rw-rw-   0        0        0    42887 2021-01-29 13:27:06.000000 gpboost-1.2.2/compile/src/LightGBM/treelearner/ocl/histogram16.cl
+-rw-rw-rw-   0        0        0    34143 2021-01-29 13:27:06.000000 gpboost-1.2.2/compile/src/LightGBM/treelearner/ocl/histogram256.cl
+-rw-rw-rw-   0        0        0    34823 2021-01-29 13:27:06.000000 gpboost-1.2.2/compile/src/LightGBM/treelearner/ocl/histogram64.cl
+-rw-rw-rw-   0        0        0     8669 2021-01-29 13:27:06.000000 gpboost-1.2.2/compile/src/LightGBM/treelearner/parallel_tree_learner.h
+-rw-rw-rw-   0        0        0    36564 2021-02-02 10:54:50.000000 gpboost-1.2.2/compile/src/LightGBM/treelearner/serial_tree_learner.cpp
+-rw-rw-rw-   0        0        0     9578 2021-02-02 10:42:52.000000 gpboost-1.2.2/compile/src/LightGBM/treelearner/serial_tree_learner.h
+-rw-rw-rw-   0        0        0     9312 2021-01-29 13:27:06.000000 gpboost-1.2.2/compile/src/LightGBM/treelearner/split_info.hpp
+-rw-rw-rw-   0        0        0     2336 2021-01-29 13:27:06.000000 gpboost-1.2.2/compile/src/LightGBM/treelearner/tree_learner.cpp
+-rw-rw-rw-   0        0        0    22729 2021-01-29 13:27:06.000000 gpboost-1.2.2/compile/src/LightGBM/treelearner/voting_parallel_tree_learner.cpp
+drwxrwxrwx   0        0        0        0 2023-07-12 05:46:21.061087 gpboost-1.2.2/gpboost/
+-rw-rw-rw-   0        0        0        6 2023-07-12 05:46:00.000000 gpboost-1.2.2/gpboost/VERSION.txt
+-rw-rw-rw-   0        0        0     1455 2022-08-25 10:12:18.000000 gpboost-1.2.2/gpboost/__init__.py
+-rw-rw-rw-   0        0        0   290536 2023-06-19 06:45:59.000000 gpboost-1.2.2/gpboost/basic.py
+-rw-rw-rw-   0        0        0     9214 2021-03-03 12:29:59.000000 gpboost-1.2.2/gpboost/callback.py
+-rw-rw-rw-   0        0        0     3434 2021-02-05 14:38:10.000000 gpboost-1.2.2/gpboost/compat.py
+-rw-rw-rw-   0        0        0    61299 2023-06-23 12:32:27.000000 gpboost-1.2.2/gpboost/engine.py
+-rw-rw-rw-   0        0        0     1556 2021-02-05 14:41:41.000000 gpboost-1.2.2/gpboost/libpath.py
+-rw-rw-rw-   0        0        0    25829 2021-02-05 14:43:16.000000 gpboost-1.2.2/gpboost/plotting.py
+-rw-rw-rw-   0        0        0    60509 2023-07-11 08:44:02.000000 gpboost-1.2.2/gpboost/sklearn.py
+drwxrwxrwx   0        0        0        0 2023-07-12 05:46:21.079087 gpboost-1.2.2/gpboost.egg-info/
+-rw-rw-rw-   0        0        0     8581 2023-07-12 05:46:16.000000 gpboost-1.2.2/gpboost.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    56207 2023-07-12 05:46:17.000000 gpboost-1.2.2/gpboost.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-12 05:46:16.000000 gpboost-1.2.2/gpboost.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-12 05:46:16.000000 gpboost-1.2.2/gpboost.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      128 2023-07-12 05:46:16.000000 gpboost-1.2.2/gpboost.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-12 05:46:16.000000 gpboost-1.2.2/gpboost.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-12 05:46:21.081087 gpboost-1.2.2/setup.cfg
+-rw-rw-rw-   0        0        0    16099 2022-05-06 08:19:13.000000 gpboost-1.2.2/setup.py
```

### Comparing `gpboost-1.2.1.1/LICENSE` & `gpboost-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/MANIFEST.in` & `gpboost-1.2.2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/PKG-INFO` & `gpboost-1.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpboost
-Version: 1.2.1.1
+Version: 1.2.2
 Summary: GPBoost Python Package
 Home-page: https://github.com/fabsig/GPBoost
 Maintainer: Fabio Sigrist
 Maintainer-email: fabiosigrist@gmail.com
 License: Apache License, Version 2.0, + see LICENSE file
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
@@ -44,15 +44,14 @@
   * [Installation from source](#installation-from-source)
 
 
 ## Examples and documentation
 
 * [**Detailed Python examples**](https://github.com/fabsig/GPBoost/tree/master/examples/python-guide):
   * [GPBoost and LaGaBoost algorithms](https://github.com/fabsig/GPBoost/tree/master/examples/python-guide/GPBoost_algorithm.py) for Gaussian data ("regression") and non-Gaussian data ("classification", etc.) combining tree-boosting with Gaussian process and random effects models
-  * [Parameter tuning](https://github.com/fabsig/GPBoost/tree/master/examples/python-guide/parameter_tuning.py) using deterministic or random grid search
   * [Generalized linear Gaussian process and mixed effects models](https://github.com/fabsig/GPBoost/tree/master/examples/python-guide/generalized_linear_Gaussian_process_mixed_effects_models.py)
   * [GPBoost algorithm applied to panel data](https://github.com/fabsig/GPBoost/tree/master/examples/python-guide/panel_data_example.py)
 * The **documentation at [https://gpboost.readthedocs.io](https://gpboost.readthedocs.io/en/latest/Python_package.html)**
 * Blog posts on how to 
    * [Combine tree-boosting with grouped random effects models](https://towardsdatascience.com/tree-boosted-mixed-effects-models-4df610b624cb) 
    * [Combine tree-boosting with Gaussian processes for spatial data](https://towardsdatascience.com/tree-boosting-for-spatial-data-789145d6d97d)
    * [GPBoost for generalized linear mixed effects models (GLMMs)](https://towardsdatascience.com/generalized-linear-mixed-effects-models-in-r-and-python-with-gpboost-89297622820c)
```

### Comparing `gpboost-1.2.1.1/README.md` & `gpboost-1.2.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,14 @@
   * [Installation from source](#installation-from-source)
 
 
 ## Examples and documentation
 
 * [**Detailed Python examples**](https://github.com/fabsig/GPBoost/tree/master/examples/python-guide):
   * [GPBoost and LaGaBoost algorithms](https://github.com/fabsig/GPBoost/tree/master/examples/python-guide/GPBoost_algorithm.py) for Gaussian data ("regression") and non-Gaussian data ("classification", etc.) combining tree-boosting with Gaussian process and random effects models
-  * [Parameter tuning](https://github.com/fabsig/GPBoost/tree/master/examples/python-guide/parameter_tuning.py) using deterministic or random grid search
   * [Generalized linear Gaussian process and mixed effects models](https://github.com/fabsig/GPBoost/tree/master/examples/python-guide/generalized_linear_Gaussian_process_mixed_effects_models.py)
   * [GPBoost algorithm applied to panel data](https://github.com/fabsig/GPBoost/tree/master/examples/python-guide/panel_data_example.py)
 * The **documentation at [https://gpboost.readthedocs.io](https://gpboost.readthedocs.io/en/latest/Python_package.html)**
 * Blog posts on how to 
    * [Combine tree-boosting with grouped random effects models](https://towardsdatascience.com/tree-boosted-mixed-effects-models-4df610b624cb) 
    * [Combine tree-boosting with Gaussian processes for spatial data](https://towardsdatascience.com/tree-boosting-for-spatial-data-789145d6d97d)
    * [GPBoost for generalized linear mixed effects models (GLMMs)](https://towardsdatascience.com/generalized-linear-mixed-effects-models-in-r-and-python-with-gpboost-89297622820c)
```

### Comparing `gpboost-1.2.1.1/compile/CMakeIntegratedOpenCL.cmake` & `gpboost-1.2.2/compile/CMakeIntegratedOpenCL.cmake`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/CMakeLists.txt` & `gpboost-1.2.2/compile/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/CSparse/Doc/LICENSE.txt` & `gpboost-1.2.2/compile/external_libs/CSparse/Doc/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/CSparse/Include/cs.h` & `gpboost-1.2.2/compile/external_libs/CSparse/Include/cs.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/CSparse/Source/cs_dfs.c` & `gpboost-1.2.2/compile/external_libs/CSparse/Source/cs_dfs.c`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/CSparse/Source/cs_reach.c` & `gpboost-1.2.2/compile/external_libs/CSparse/Source/cs_reach.c`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/CSparse/Source/cs_spsolve.c` & `gpboost-1.2.2/compile/external_libs/CSparse/Source/cs_spsolve.c`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/OptimLib/LICENSE` & `gpboost-1.2.2/compile/external_libs/OptimLib/LICENSE`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/OptimLib/constrained/sumt.hpp` & `gpboost-1.2.2/compile/external_libs/OptimLib/constrained/sumt.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/OptimLib/line_search/more_thuente.hpp` & `gpboost-1.2.2/compile/external_libs/OptimLib/line_search/more_thuente.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/OptimLib/misc/determine_bounds_type.hpp` & `gpboost-1.2.2/compile/external_libs/OptimLib/misc/determine_bounds_type.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/OptimLib/misc/error_reporting.hpp` & `gpboost-1.2.2/compile/external_libs/OptimLib/misc/error_reporting.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/OptimLib/misc/error_reporting.ipp` & `gpboost-1.2.2/compile/external_libs/OptimLib/misc/error_reporting.ipp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/OptimLib/misc/jacobian_adjust.hpp` & `gpboost-1.2.2/compile/external_libs/OptimLib/misc/jacobian_adjust.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/OptimLib/misc/matrix_ops/abs.hpp` & `gpboost-1.2.2/compile/external_libs/OptimLib/misc/matrix_ops/abs.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/OptimLib/misc/matrix_ops/abs_max.hpp` & `gpboost-1.2.2/compile/external_libs/OptimLib/misc/matrix_ops/abs_max.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/OptimLib/misc/matrix_ops/access.hpp` & `gpboost-1.2.2/compile/external_libs/OptimLib/misc/matrix_ops/access.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/OptimLib/misc/matrix_ops/accu.hpp` & `gpboost-1.2.2/compile/external_libs/OptimLib/misc/matrix_ops/accu.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/OptimLib/misc/matrix_ops/array_add.hpp` & `gpboost-1.2.2/compile/external_libs/OptimLib/misc/matrix_ops/array_add.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/OptimLib/misc/matrix_ops/array_div.hpp` & `gpboost-1.2.2/compile/external_libs/OptimLib/misc/matrix_ops/array_div.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/OptimLib/misc/matrix_ops/array_mult.hpp` & `gpboost-1.2.2/compile/external_libs/OptimLib/misc/matrix_ops/array_mult.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/OptimLib/misc/matrix_ops/as_scalar.hpp` & `gpboost-1.2.2/compile/external_libs/OptimLib/misc/matrix_ops/as_scalar.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/OptimLib/misc/matrix_ops/cos.hpp` & `gpboost-1.2.2/compile/external_libs/OptimLib/misc/matrix_ops/cos.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/OptimLib/misc/matrix_ops/cout.hpp` & `gpboost-1.2.2/compile/external_libs/OptimLib/misc/matrix_ops/cout.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/OptimLib/misc/matrix_ops/diagmat.hpp` & `gpboost-1.2.2/compile/external_libs/OptimLib/misc/matrix_ops/diagmat.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/OptimLib/misc/matrix_ops/diagvec.hpp` & `gpboost-1.2.2/compile/external_libs/OptimLib/misc/matrix_ops/diagvec.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/OptimLib/misc/matrix_ops/dot.hpp` & `gpboost-1.2.2/compile/external_libs/OptimLib/misc/matrix_ops/dot.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/OptimLib/misc/matrix_ops/endl.hpp` & `gpboost-1.2.2/compile/external_libs/OptimLib/misc/matrix_ops/endl.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/OptimLib/misc/matrix_ops/eval.hpp` & `gpboost-1.2.2/compile/external_libs/OptimLib/misc/matrix_ops/eval.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/OptimLib/misc/matrix_ops/exp.hpp` & `gpboost-1.2.2/compile/external_libs/OptimLib/misc/matrix_ops/exp.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/OptimLib/misc/matrix_ops/eye.hpp` & `gpboost-1.2.2/compile/external_libs/OptimLib/misc/matrix_ops/eye.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/OptimLib/misc/matrix_ops/get_sort_index.hpp` & `gpboost-1.2.2/compile/external_libs/OptimLib/misc/matrix_ops/get_sort_index.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/OptimLib/misc/matrix_ops/hadamard.hpp` & `gpboost-1.2.2/compile/external_libs/OptimLib/misc/matrix_ops/hadamard.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/OptimLib/misc/matrix_ops/index_min.hpp` & `gpboost-1.2.2/compile/external_libs/OptimLib/misc/matrix_ops/index_min.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/OptimLib/misc/matrix_ops/inv.hpp` & `gpboost-1.2.2/compile/external_libs/OptimLib/misc/matrix_ops/inv.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/OptimLib/misc/matrix_ops/is_finite.hpp` & `gpboost-1.2.2/compile/external_libs/OptimLib/misc/matrix_ops/is_finite.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/OptimLib/misc/matrix_ops/log.hpp` & `gpboost-1.2.2/compile/external_libs/OptimLib/misc/matrix_ops/log.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/OptimLib/misc/matrix_ops/max.hpp` & `gpboost-1.2.2/compile/external_libs/OptimLib/misc/matrix_ops/max.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/OptimLib/misc/matrix_ops/min.hpp` & `gpboost-1.2.2/compile/external_libs/OptimLib/misc/matrix_ops/min.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/OptimLib/misc/matrix_ops/ncol.hpp` & `gpboost-1.2.2/compile/external_libs/OptimLib/misc/matrix_ops/ncol.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/OptimLib/misc/matrix_ops/norm.hpp` & `gpboost-1.2.2/compile/external_libs/OptimLib/misc/matrix_ops/norm.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/OptimLib/misc/matrix_ops/ones.hpp` & `gpboost-1.2.2/compile/external_libs/OptimLib/misc/matrix_ops/ones.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/OptimLib/misc/matrix_ops/pow.hpp` & `gpboost-1.2.2/compile/external_libs/OptimLib/misc/matrix_ops/pow.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/OptimLib/misc/matrix_ops/randi.hpp` & `gpboost-1.2.2/compile/external_libs/OptimLib/misc/matrix_ops/randi.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/OptimLib/misc/matrix_ops/randn.hpp` & `gpboost-1.2.2/compile/external_libs/OptimLib/misc/matrix_ops/randn.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/OptimLib/misc/matrix_ops/randu.hpp` & `gpboost-1.2.2/compile/external_libs/OptimLib/misc/matrix_ops/randu.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/OptimLib/misc/matrix_ops/reset_negative_values.hpp` & `gpboost-1.2.2/compile/external_libs/OptimLib/misc/matrix_ops/reset_negative_values.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/OptimLib/misc/matrix_ops/set_size.hpp` & `gpboost-1.2.2/compile/external_libs/OptimLib/misc/matrix_ops/set_size.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/OptimLib/misc/matrix_ops/size.hpp` & `gpboost-1.2.2/compile/external_libs/OptimLib/misc/matrix_ops/size.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/OptimLib/misc/matrix_ops/solve.hpp` & `gpboost-1.2.2/compile/external_libs/OptimLib/misc/matrix_ops/solve.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/OptimLib/misc/matrix_ops/sqrt.hpp` & `gpboost-1.2.2/compile/external_libs/OptimLib/misc/matrix_ops/sqrt.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/OptimLib/misc/matrix_ops/sum.hpp` & `gpboost-1.2.2/compile/external_libs/OptimLib/misc/matrix_ops/sum.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/OptimLib/misc/matrix_ops/transpose.hpp` & `gpboost-1.2.2/compile/external_libs/OptimLib/misc/matrix_ops/transpose.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/OptimLib/misc/matrix_ops/zeros.hpp` & `gpboost-1.2.2/compile/external_libs/OptimLib/misc/matrix_ops/zeros.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/OptimLib/misc/misc.hpp` & `gpboost-1.2.2/compile/external_libs/OptimLib/misc/misc.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/OptimLib/misc/numerical_gradient.hpp` & `gpboost-1.2.2/compile/external_libs/OptimLib/misc/numerical_gradient.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/OptimLib/misc/numerical_hessian.hpp` & `gpboost-1.2.2/compile/external_libs/OptimLib/misc/numerical_hessian.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/OptimLib/misc/optim_matdefs.hpp` & `gpboost-1.2.2/compile/external_libs/OptimLib/misc/optim_matdefs.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/OptimLib/misc/optim_options.hpp` & `gpboost-1.2.2/compile/external_libs/OptimLib/misc/optim_options.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/OptimLib/misc/optim_structs.hpp` & `gpboost-1.2.2/compile/external_libs/OptimLib/misc/optim_structs.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/OptimLib/misc/optim_trace.hpp` & `gpboost-1.2.2/compile/external_libs/OptimLib/misc/optim_trace.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/OptimLib/misc/transform_vals.hpp` & `gpboost-1.2.2/compile/external_libs/OptimLib/misc/transform_vals.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/OptimLib/misc/unit_vec.hpp` & `gpboost-1.2.2/compile/external_libs/OptimLib/misc/unit_vec.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/OptimLib/misc/unit_vec.ipp` & `gpboost-1.2.2/compile/external_libs/OptimLib/misc/unit_vec.ipp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/OptimLib/optim.hpp` & `gpboost-1.2.2/compile/external_libs/OptimLib/optim.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/OptimLib/unconstrained/bfgs.hpp` & `gpboost-1.2.2/compile/external_libs/OptimLib/unconstrained/bfgs.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/OptimLib/unconstrained/cg.hpp` & `gpboost-1.2.2/compile/external_libs/OptimLib/unconstrained/cg.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/OptimLib/unconstrained/de.hpp` & `gpboost-1.2.2/compile/external_libs/OptimLib/unconstrained/de.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/OptimLib/unconstrained/de_prmm.hpp` & `gpboost-1.2.2/compile/external_libs/OptimLib/unconstrained/de_prmm.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/OptimLib/unconstrained/gd.hpp` & `gpboost-1.2.2/compile/external_libs/OptimLib/unconstrained/gd.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/OptimLib/unconstrained/gd.ipp` & `gpboost-1.2.2/compile/external_libs/OptimLib/unconstrained/gd.ipp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/OptimLib/unconstrained/lbfgs.hpp` & `gpboost-1.2.2/compile/external_libs/OptimLib/unconstrained/lbfgs.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/OptimLib/unconstrained/newton.hpp` & `gpboost-1.2.2/compile/external_libs/OptimLib/unconstrained/newton.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/OptimLib/unconstrained/nm.hpp` & `gpboost-1.2.2/compile/external_libs/OptimLib/unconstrained/nm.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/OptimLib/unconstrained/pso.hpp` & `gpboost-1.2.2/compile/external_libs/OptimLib/unconstrained/pso.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/OptimLib/unconstrained/pso_dv.hpp` & `gpboost-1.2.2/compile/external_libs/OptimLib/unconstrained/pso_dv.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/OptimLib/zeros/broyden.hpp` & `gpboost-1.2.2/compile/external_libs/OptimLib/zeros/broyden.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/OptimLib/zeros/broyden_df.hpp` & `gpboost-1.2.2/compile/external_libs/OptimLib/zeros/broyden_df.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/CMakeLists.txt` & `gpboost-1.2.2/compile/external_libs/compute/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/cmake/FindBolt.cmake` & `gpboost-1.2.2/compile/external_libs/compute/cmake/FindBolt.cmake`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/cmake/FindEigen.cmake` & `gpboost-1.2.2/compile/external_libs/compute/cmake/FindEigen.cmake`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/cmake/FindTBB.cmake` & `gpboost-1.2.2/compile/external_libs/compute/cmake/FindTBB.cmake`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/cmake/opencl/FindOpenCL.cmake` & `gpboost-1.2.2/compile/external_libs/compute/cmake/opencl/FindOpenCL.cmake`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/accumulate.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/accumulate.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/adjacent_difference.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/adjacent_difference.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/adjacent_find.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/adjacent_find.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/all_of.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/all_of.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/any_of.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/any_of.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/binary_search.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/binary_search.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/copy.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/copy.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/copy_if.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/copy_if.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/copy_n.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/copy_n.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/count.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/count.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/count_if.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/count_if.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/detail/balanced_path.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/detail/balanced_path.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/detail/binary_find.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/detail/binary_find.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/detail/compact.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/detail/compact.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/detail/copy_on_device.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/detail/copy_on_device.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/detail/copy_to_device.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/detail/copy_to_device.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/detail/copy_to_host.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/detail/copy_to_host.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/detail/count_if_with_ballot.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/detail/count_if_with_ballot.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/detail/count_if_with_reduce.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/detail/count_if_with_reduce.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/detail/count_if_with_threads.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/detail/count_if_with_threads.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/detail/find_extrema.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/detail/find_extrema.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/detail/find_extrema_on_cpu.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/detail/find_extrema_on_cpu.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/detail/find_extrema_with_atomics.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/detail/find_extrema_with_atomics.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/detail/find_extrema_with_reduce.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/detail/find_extrema_with_reduce.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/detail/find_if_with_atomics.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/detail/find_if_with_atomics.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/detail/inplace_reduce.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/detail/inplace_reduce.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/detail/insertion_sort.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/detail/insertion_sort.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/detail/merge_path.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/detail/merge_path.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/detail/merge_sort_on_cpu.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/detail/merge_sort_on_cpu.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/detail/merge_sort_on_gpu.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/detail/merge_sort_on_gpu.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/detail/merge_with_merge_path.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/detail/merge_with_merge_path.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/detail/radix_sort.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/detail/radix_sort.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/detail/random_fill.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/detail/random_fill.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/detail/reduce_by_key.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/detail/reduce_by_key.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/detail/reduce_by_key_with_scan.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/detail/reduce_by_key_with_scan.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/detail/reduce_on_cpu.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/detail/reduce_on_cpu.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/detail/reduce_on_gpu.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/detail/reduce_on_gpu.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/detail/scan.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/detail/scan.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/detail/scan_on_cpu.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/detail/scan_on_cpu.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/detail/scan_on_gpu.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/detail/scan_on_gpu.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/detail/search_all.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/detail/search_all.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/detail/serial_accumulate.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/detail/serial_accumulate.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/detail/serial_count_if.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/detail/serial_count_if.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/detail/serial_find_extrema.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/detail/serial_find_extrema.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/detail/serial_merge.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/detail/serial_merge.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/detail/serial_reduce.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/detail/serial_reduce.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/detail/serial_reduce_by_key.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/detail/serial_reduce_by_key.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/detail/serial_scan.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/detail/serial_scan.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/equal.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/equal.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/equal_range.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/equal_range.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/exclusive_scan.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/exclusive_scan.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/fill.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/fill.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/fill_n.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/fill_n.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/find.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/find.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/find_end.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/find_end.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/find_if.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/find_if.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/find_if_not.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/find_if_not.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/for_each.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/for_each.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/for_each_n.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/for_each_n.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/gather.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/gather.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/generate.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/generate.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/generate_n.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/generate_n.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/includes.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/includes.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/inclusive_scan.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/inclusive_scan.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/inner_product.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/inner_product.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/inplace_merge.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/inplace_merge.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/iota.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/iota.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/is_partitioned.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/is_partitioned.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/is_permutation.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/is_permutation.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/is_sorted.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/is_sorted.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/lexicographical_compare.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/lexicographical_compare.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/lower_bound.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/lower_bound.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/max_element.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/max_element.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/merge.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/merge.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/min_element.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/min_element.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/minmax_element.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/minmax_element.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/mismatch.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/mismatch.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/next_permutation.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/next_permutation.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/none_of.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/none_of.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/nth_element.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/nth_element.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/partial_sum.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/partial_sum.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/partition.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/partition.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/partition_copy.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/partition_copy.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/partition_point.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/partition_point.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/prev_permutation.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/prev_permutation.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/random_shuffle.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/random_shuffle.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/reduce.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/reduce.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/reduce_by_key.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/reduce_by_key.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/remove.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/remove.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/remove_if.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/remove_if.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/replace.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/replace.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/replace_copy.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/replace_copy.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/reverse.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/reverse.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/reverse_copy.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/reverse_copy.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/rotate.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/rotate.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/rotate_copy.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/rotate_copy.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/scatter.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/scatter.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/scatter_if.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/scatter_if.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/search.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/search.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/search_n.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/search_n.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/set_difference.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/set_difference.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/set_intersection.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/set_intersection.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/set_symmetric_difference.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/set_symmetric_difference.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/set_union.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/set_union.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/sort.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/sort.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/sort_by_key.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/sort_by_key.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/stable_partition.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/stable_partition.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/stable_sort.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/stable_sort.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/stable_sort_by_key.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/stable_sort_by_key.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/swap_ranges.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/swap_ranges.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/transform.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/transform.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/transform_if.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/transform_if.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/transform_reduce.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/transform_reduce.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/unique.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/unique.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/unique_copy.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/unique_copy.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm/upper_bound.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm/upper_bound.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/algorithm.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/algorithm.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/allocator/buffer_allocator.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/allocator/buffer_allocator.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/allocator/pinned_allocator.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/allocator/pinned_allocator.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/allocator.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/allocator.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/async/future.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/async/future.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/async/wait.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/async/wait.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/async/wait_guard.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/async/wait_guard.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/async.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/async.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/buffer.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/buffer.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/cl.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/cl.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/cl_ext.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/cl_ext.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/closure.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/closure.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/command_queue.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/command_queue.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/config.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/config.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/container/array.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/container/array.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/container/basic_string.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/container/basic_string.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/container/detail/scalar.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/container/detail/scalar.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/container/dynamic_bitset.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/container/dynamic_bitset.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/container/flat_map.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/container/flat_map.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/container/flat_set.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/container/flat_set.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/container/mapped_view.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/container/mapped_view.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/container/stack.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/container/stack.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/container/string.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/container/string.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/container/valarray.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/container/valarray.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/container/vector.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/container/vector.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/container.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/container.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/context.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/context.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/core.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/core.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/detail/assert_cl_success.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/detail/assert_cl_success.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/detail/buffer_value.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/detail/buffer_value.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/detail/cl_versions.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/detail/cl_versions.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/detail/device_ptr.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/detail/device_ptr.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/detail/diagnostic.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/detail/diagnostic.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/detail/duration.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/detail/duration.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/detail/get_object_info.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/detail/get_object_info.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/detail/getenv.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/detail/getenv.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/detail/global_static.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/detail/global_static.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/detail/is_buffer_iterator.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/detail/is_buffer_iterator.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/detail/is_contiguous_iterator.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/detail/is_contiguous_iterator.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/detail/iterator_plus_distance.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/detail/iterator_plus_distance.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/detail/iterator_range_size.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/detail/iterator_range_size.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/detail/iterator_traits.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/detail/iterator_traits.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/detail/literal.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/detail/literal.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/detail/lru_cache.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/detail/lru_cache.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/detail/meta_kernel.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/detail/meta_kernel.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/detail/mpl_vector_to_tuple.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/detail/mpl_vector_to_tuple.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/detail/nvidia_compute_capability.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/detail/nvidia_compute_capability.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/detail/parameter_cache.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/detail/parameter_cache.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/detail/path.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/detail/path.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/detail/print_range.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/detail/print_range.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/detail/read_write_single_value.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/detail/read_write_single_value.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/detail/sha1.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/detail/sha1.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/detail/variadic_macros.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/detail/variadic_macros.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/detail/vendor.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/detail/vendor.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/detail/work_size.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/detail/work_size.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/device.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/device.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/event.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/event.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/exception/context_error.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/exception/context_error.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/exception/no_device_found.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/exception/no_device_found.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/exception/opencl_error.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/exception/opencl_error.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/exception/program_build_failure.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/exception/program_build_failure.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/exception/unsupported_extension_error.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/exception/unsupported_extension_error.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/exception.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/exception.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/experimental/clamp_range.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/experimental/clamp_range.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/experimental/malloc.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/experimental/malloc.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/experimental/sort_by_transform.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/experimental/sort_by_transform.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/experimental/tabulate.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/experimental/tabulate.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/function.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/function.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/functional/as.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/functional/as.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/functional/atomic.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/functional/atomic.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/functional/bind.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/functional/bind.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/functional/common.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/functional/common.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/functional/convert.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/functional/convert.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/functional/detail/macros.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/functional/detail/macros.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/functional/detail/nvidia_ballot.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/functional/detail/nvidia_ballot.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/functional/detail/nvidia_popcount.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/functional/detail/nvidia_popcount.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/functional/detail/unpack.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/functional/detail/unpack.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/functional/field.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/functional/field.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/functional/geometry.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/functional/geometry.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/functional/get.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/functional/get.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/functional/hash.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/functional/hash.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/functional/identity.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/functional/identity.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/functional/integer.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/functional/integer.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/functional/logical.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/functional/logical.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/functional/math.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/functional/math.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/functional/operator.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/functional/operator.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/functional/popcount.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/functional/popcount.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/functional/relational.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/functional/relational.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/functional.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/functional.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/image/image1d.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/image/image1d.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/image/image2d.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/image/image2d.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/image/image3d.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/image/image3d.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/image/image_format.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/image/image_format.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/image/image_object.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/image/image_object.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/image/image_sampler.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/image/image_sampler.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/image.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/image.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/image2d.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/image2d.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/image3d.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/image3d.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/image_format.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/image_format.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/image_sampler.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/image_sampler.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/interop/eigen/core.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/interop/eigen/core.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/interop/eigen.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/interop/eigen.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/interop/opencv/core.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/interop/opencv/core.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/interop/opencv/highgui.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/interop/opencv/highgui.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/interop/opencv/ocl.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/interop/opencv/ocl.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/interop/opencv.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/interop/opencv.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/interop/opengl/acquire.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/interop/opengl/acquire.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/interop/opengl/cl_gl.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/interop/opengl/cl_gl.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/interop/opengl/cl_gl_ext.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/interop/opengl/cl_gl_ext.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/interop/opengl/context.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/interop/opengl/context.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/interop/opengl/gl.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/interop/opengl/gl.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/interop/opengl/opengl_buffer.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/interop/opengl/opengl_buffer.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/interop/opengl/opengl_renderbuffer.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/interop/opengl/opengl_renderbuffer.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/interop/opengl/opengl_texture.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/interop/opengl/opengl_texture.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/interop/opengl.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/interop/opengl.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/interop/qt/qimage.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/interop/qt/qimage.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/interop/qt/qpoint.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/interop/qt/qpoint.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/interop/qt/qpointf.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/interop/qt/qpointf.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/interop/qt/qtcore.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/interop/qt/qtcore.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/interop/qt/qtgui.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/interop/qt/qtgui.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/interop/qt/qvector.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/interop/qt/qvector.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/interop/qt.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/interop/qt.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/interop/vtk/bounds.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/interop/vtk/bounds.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/interop/vtk/data_array.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/interop/vtk/data_array.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/interop/vtk/matrix4x4.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/interop/vtk/matrix4x4.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/interop/vtk/points.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/interop/vtk/points.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/interop/vtk.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/interop/vtk.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/iterator/buffer_iterator.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/iterator/buffer_iterator.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/iterator/constant_buffer_iterator.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/iterator/constant_buffer_iterator.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/iterator/constant_iterator.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/iterator/constant_iterator.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/iterator/counting_iterator.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/iterator/counting_iterator.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/iterator/detail/get_base_iterator_buffer.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/iterator/detail/get_base_iterator_buffer.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/iterator/detail/swizzle_iterator.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/iterator/detail/swizzle_iterator.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/iterator/discard_iterator.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/iterator/discard_iterator.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/iterator/function_input_iterator.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/iterator/function_input_iterator.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/iterator/permutation_iterator.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/iterator/permutation_iterator.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/iterator/strided_iterator.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/iterator/strided_iterator.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/iterator/transform_iterator.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/iterator/transform_iterator.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/iterator/zip_iterator.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/iterator/zip_iterator.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/iterator.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/iterator.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/kernel.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/kernel.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/lambda/context.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/lambda/context.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/lambda/functional.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/lambda/functional.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/lambda/get.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/lambda/get.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/lambda/make_pair.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/lambda/make_pair.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/lambda/make_tuple.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/lambda/make_tuple.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/lambda/placeholder.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/lambda/placeholder.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/lambda/placeholders.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/lambda/placeholders.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/lambda/result_of.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/lambda/result_of.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/lambda.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/lambda.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/memory/local_buffer.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/memory/local_buffer.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/memory/svm_ptr.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/memory/svm_ptr.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/memory.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/memory.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/memory_object.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/memory_object.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/pipe.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/pipe.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/platform.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/platform.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/program.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/program.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/random/bernoulli_distribution.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/random/bernoulli_distribution.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/random/default_random_engine.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/random/default_random_engine.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/random/discrete_distribution.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/random/discrete_distribution.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/random/linear_congruential_engine.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/random/linear_congruential_engine.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/random/mersenne_twister_engine.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/random/mersenne_twister_engine.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/random/normal_distribution.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/random/normal_distribution.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/random/threefry_engine.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/random/threefry_engine.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/random/uniform_int_distribution.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/random/uniform_int_distribution.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/random/uniform_real_distribution.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/random/uniform_real_distribution.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/random.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/random.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/source.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/source.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/svm.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/svm.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/system.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/system.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/type_traits/common_type.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/type_traits/common_type.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/type_traits/detail/capture_traits.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/type_traits/detail/capture_traits.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/type_traits/is_device_iterator.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/type_traits/is_device_iterator.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/type_traits/is_fundamental.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/type_traits/is_fundamental.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/type_traits/is_vector_type.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/type_traits/is_vector_type.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/type_traits/make_vector_type.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/type_traits/make_vector_type.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/type_traits/result_of.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/type_traits/result_of.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/type_traits/scalar_type.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/type_traits/scalar_type.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/type_traits/type_definition.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/type_traits/type_definition.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/type_traits/type_name.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/type_traits/type_name.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/type_traits/vector_size.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/type_traits/vector_size.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/type_traits.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/type_traits.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/types/builtin.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/types/builtin.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/types/complex.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/types/complex.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/types/fundamental.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/types/fundamental.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/types/pair.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/types/pair.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/types/size_t.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/types/size_t.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/types/struct.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/types/struct.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/types/tuple.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/types/tuple.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/types.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/types.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/user_event.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/user_event.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/utility/dim.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/utility/dim.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/utility/extents.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/utility/extents.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/utility/invoke.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/utility/invoke.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/utility/program_cache.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/utility/program_cache.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/utility/source.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/utility/source.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/utility/wait_list.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/utility/wait_list.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/utility.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/utility.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/version.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/version.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute/wait_list.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute/wait_list.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/compute/include/boost/compute.hpp` & `gpboost-1.2.2/compile/external_libs/compute/include/boost/compute.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/CMakeLists.txt` & `gpboost-1.2.2/compile/external_libs/eigen/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/Cholesky` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/Cholesky`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/Core` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/Core`

 * *Files 1% similar despite different names*

```diff
@@ -195,15 +195,15 @@
   #include "src/Core/arch/SSE/MathFunctions.h"
   #include "src/Core/arch/AVX/MathFunctions.h"
 #elif defined EIGEN_VECTORIZE_SSE
   #include "src/Core/arch/SSE/PacketMath.h"
   #include "src/Core/arch/SSE/TypeCasting.h"
   #include "src/Core/arch/SSE/MathFunctions.h"
   #include "src/Core/arch/SSE/Complex.h"
-#elif defined(EIGEN_VECTORIZE_ALTIVEC) || defined(EIGEN_VECTORIZE_VSX)
+#elif (defined(EIGEN_VECTORIZE_ALTIVEC) || defined(EIGEN_VECTORIZE_VSX)) && !defined(__APPLE__)
   #include "src/Core/arch/AltiVec/PacketMath.h"
   #include "src/Core/arch/AltiVec/MathFunctions.h"
   #include "src/Core/arch/AltiVec/Complex.h"
 #elif defined EIGEN_VECTORIZE_NEON
   #include "src/Core/arch/NEON/PacketMath.h"
   #include "src/Core/arch/NEON/TypeCasting.h"
   #include "src/Core/arch/NEON/MathFunctions.h"
@@ -335,15 +335,15 @@
 #include "src/Core/products/TriangularMatrixMatrix.h"
 #include "src/Core/products/TriangularSolverMatrix.h"
 #include "src/Core/products/TriangularSolverVector.h"
 #include "src/Core/BandMatrix.h"
 #include "src/Core/CoreIterators.h"
 #include "src/Core/ConditionEstimator.h"
 
-#if defined(EIGEN_VECTORIZE_ALTIVEC) || defined(EIGEN_VECTORIZE_VSX)
+#if (defined(EIGEN_VECTORIZE_ALTIVEC) || defined(EIGEN_VECTORIZE_VSX)) && !defined(__APPLE__)
   #include "src/Core/arch/AltiVec/MatrixProduct.h"
 #elif defined EIGEN_VECTORIZE_NEON
   #include "src/Core/arch/NEON/GeneralBlockPanelKernel.h"
 #endif
 
 #include "src/Core/BooleanRedux.h"
 #include "src/Core/Select.h"
```

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/Eigenvalues` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/Eigenvalues`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/Geometry` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/Geometry`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/Householder` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/Householder`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/IterativeLinearSolvers` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/IterativeLinearSolvers`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/Jacobi` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/Jacobi`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/LU` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/LU`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/OrderingMethods` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/OrderingMethods`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/QR` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/QR`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/SVD` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/SVD`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/Sparse` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/Sparse`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/SparseCholesky` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/SparseCholesky`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/SparseCore` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/SparseCore`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/SparseLU` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/SparseLU`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/SparseQR` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/SparseQR`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Cholesky/LDLT.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Cholesky/LDLT.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Cholesky/LLT.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Cholesky/LLT.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Cholesky/LLT_LAPACKE.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Cholesky/LLT_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/ArithmeticSequence.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/ArithmeticSequence.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/Array.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/Array.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/ArrayBase.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/ArrayBase.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/ArrayWrapper.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/ArrayWrapper.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/Assign.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/Assign.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/AssignEvaluator.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/AssignEvaluator.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/Assign_MKL.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/Assign_MKL.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/BandMatrix.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/BandMatrix.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/Block.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/Block.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/BooleanRedux.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/BooleanRedux.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/CommaInitializer.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/CommaInitializer.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/ConditionEstimator.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/ConditionEstimator.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/CoreEvaluators.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/CoreEvaluators.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/CoreIterators.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/CoreIterators.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/CwiseBinaryOp.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/CwiseBinaryOp.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/CwiseNullaryOp.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/CwiseNullaryOp.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/CwiseTernaryOp.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/CwiseTernaryOp.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/CwiseUnaryOp.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/CwiseUnaryOp.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/CwiseUnaryView.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/CwiseUnaryView.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/DenseBase.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/DenseBase.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/DenseCoeffsBase.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/DenseCoeffsBase.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/DenseStorage.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/DenseStorage.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/Diagonal.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/Diagonal.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/DiagonalMatrix.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/DiagonalMatrix.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/DiagonalProduct.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/DiagonalProduct.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/Dot.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/Dot.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/EigenBase.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/EigenBase.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/ForceAlignedAccess.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/ForceAlignedAccess.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/Fuzzy.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/Fuzzy.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/GeneralProduct.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/GeneralProduct.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/GenericPacketMath.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/GenericPacketMath.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/GlobalFunctions.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/GlobalFunctions.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/IO.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/IO.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/IndexedView.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/IndexedView.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/Inverse.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/Inverse.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/Map.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/Map.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/MapBase.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/MapBase.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/MathFunctions.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/MathFunctionsImpl.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/MathFunctionsImpl.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/Matrix.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/Matrix.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/MatrixBase.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/MatrixBase.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/NestByValue.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/NestByValue.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/NoAlias.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/NoAlias.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/NumTraits.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/NumTraits.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/PartialReduxEvaluator.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/PartialReduxEvaluator.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/PermutationMatrix.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/PermutationMatrix.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/PlainObjectBase.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/PlainObjectBase.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/Product.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/Product.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/ProductEvaluators.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/ProductEvaluators.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/Random.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/Random.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/Redux.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/Redux.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/Ref.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/Ref.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/Replicate.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/Replicate.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/Reshaped.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/Reshaped.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/ReturnByValue.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/ReturnByValue.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/Reverse.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/Reverse.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/Select.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/Select.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/SelfAdjointView.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/SelfAdjointView.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/SelfCwiseBinaryOp.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/SelfCwiseBinaryOp.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/Solve.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/Solve.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/SolveTriangular.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/SolveTriangular.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/SolverBase.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/SolverBase.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/StableNorm.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/StableNorm.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/StlIterators.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/StlIterators.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/Stride.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/Stride.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/Swap.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/Swap.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/Transpose.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/Transpose.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/Transpositions.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/Transpositions.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/TriangularMatrix.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/TriangularMatrix.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/VectorBlock.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/VectorBlock.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/VectorwiseOp.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/VectorwiseOp.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/Visitor.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/Visitor.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/arch/AVX/Complex.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/arch/AVX/Complex.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/arch/AVX/MathFunctions.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/arch/AVX/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/arch/AVX/PacketMath.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/arch/AVX/PacketMath.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/arch/AVX/TypeCasting.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/arch/AVX/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/arch/AVX512/Complex.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/arch/AVX512/Complex.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/arch/AVX512/MathFunctions.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/arch/AVX512/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/arch/AVX512/PacketMath.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/arch/AVX512/PacketMath.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/arch/AVX512/TypeCasting.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/arch/AVX512/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/arch/AltiVec/Complex.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/arch/AltiVec/Complex.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/arch/AltiVec/MathFunctions.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/arch/AltiVec/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/arch/AltiVec/MatrixProduct.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/arch/AltiVec/MatrixProduct.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/arch/AltiVec/MatrixProductCommon.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/arch/AltiVec/MatrixProductCommon.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/arch/AltiVec/MatrixProductMMA.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/arch/AltiVec/MatrixProductMMA.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/arch/AltiVec/PacketMath.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/arch/AltiVec/PacketMath.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/arch/CUDA/Complex.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/arch/CUDA/Complex.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/arch/Default/BFloat16.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/arch/Default/BFloat16.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/arch/Default/ConjHelper.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/arch/Default/ConjHelper.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/arch/Default/GenericPacketMathFunctions.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/arch/Default/GenericPacketMathFunctions.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/arch/Default/GenericPacketMathFunctionsFwd.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/arch/Default/GenericPacketMathFunctionsFwd.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/arch/Default/Half.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/arch/Default/Half.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/arch/Default/Settings.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/arch/Default/Settings.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/arch/Default/TypeCasting.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/arch/Default/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/arch/GPU/MathFunctions.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/arch/GPU/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/arch/GPU/PacketMath.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/arch/GPU/PacketMath.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/arch/GPU/TypeCasting.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/arch/GPU/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/arch/HIP/hcc/math_constants.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/arch/HIP/hcc/math_constants.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/arch/MSA/Complex.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/arch/MSA/Complex.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/arch/MSA/MathFunctions.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/arch/MSA/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/arch/MSA/PacketMath.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/arch/MSA/PacketMath.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/arch/NEON/Complex.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/arch/NEON/Complex.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/arch/NEON/GeneralBlockPanelKernel.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/arch/NEON/GeneralBlockPanelKernel.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/arch/NEON/MathFunctions.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/arch/NEON/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/arch/NEON/PacketMath.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/arch/NEON/PacketMath.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/arch/NEON/TypeCasting.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/arch/NEON/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/arch/SSE/Complex.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/arch/SSE/Complex.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/arch/SSE/MathFunctions.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/arch/SSE/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/arch/SSE/PacketMath.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/arch/SSE/PacketMath.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/arch/SSE/TypeCasting.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/arch/SSE/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/arch/SVE/MathFunctions.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/arch/SVE/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/arch/SVE/PacketMath.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/arch/SVE/PacketMath.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/arch/SVE/TypeCasting.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/arch/SVE/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/arch/SYCL/InteropHeaders.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/arch/SYCL/InteropHeaders.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/arch/SYCL/MathFunctions.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/arch/SYCL/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/arch/SYCL/PacketMath.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/arch/SYCL/PacketMath.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/arch/SYCL/SyclMemoryModel.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/arch/SYCL/SyclMemoryModel.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/arch/SYCL/TypeCasting.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/arch/SYCL/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/arch/ZVector/Complex.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/arch/ZVector/Complex.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/arch/ZVector/MathFunctions.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/arch/ZVector/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/arch/ZVector/PacketMath.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/arch/ZVector/PacketMath.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/functors/AssignmentFunctors.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/functors/AssignmentFunctors.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/functors/BinaryFunctors.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/functors/BinaryFunctors.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/functors/NullaryFunctors.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/functors/NullaryFunctors.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/functors/StlFunctors.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/functors/StlFunctors.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/functors/TernaryFunctors.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/functors/TernaryFunctors.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/functors/UnaryFunctors.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/functors/UnaryFunctors.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/products/GeneralBlockPanelKernel.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/products/GeneralBlockPanelKernel.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/products/GeneralMatrixMatrix.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/products/GeneralMatrixMatrix.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/products/GeneralMatrixMatrixTriangular.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/products/GeneralMatrixMatrixTriangular.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/products/GeneralMatrixMatrixTriangular_BLAS.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/products/GeneralMatrixMatrixTriangular_BLAS.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/products/GeneralMatrixMatrix_BLAS.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/products/GeneralMatrixMatrix_BLAS.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/products/GeneralMatrixVector.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/products/GeneralMatrixVector.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/products/GeneralMatrixVector_BLAS.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/products/GeneralMatrixVector_BLAS.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/products/Parallelizer.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/products/Parallelizer.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/products/SelfadjointMatrixMatrix.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/products/SelfadjointMatrixMatrix.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/products/SelfadjointMatrixMatrix_BLAS.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/products/SelfadjointMatrixMatrix_BLAS.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/products/SelfadjointMatrixVector.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/products/SelfadjointMatrixVector.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/products/SelfadjointMatrixVector_BLAS.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/products/SelfadjointMatrixVector_BLAS.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/products/SelfadjointProduct.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/products/SelfadjointProduct.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/products/SelfadjointRank2Update.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/products/SelfadjointRank2Update.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/products/TriangularMatrixMatrix.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/products/TriangularMatrixMatrix.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/products/TriangularMatrixMatrix_BLAS.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/products/TriangularMatrixMatrix_BLAS.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/products/TriangularMatrixVector.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/products/TriangularMatrixVector.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/products/TriangularMatrixVector_BLAS.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/products/TriangularMatrixVector_BLAS.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/products/TriangularSolverMatrix.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/products/TriangularSolverMatrix.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/products/TriangularSolverMatrix_BLAS.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/products/TriangularSolverMatrix_BLAS.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/products/TriangularSolverVector.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/products/TriangularSolverVector.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/util/BlasUtil.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/util/BlasUtil.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/util/ConfigureVectorization.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/util/ConfigureVectorization.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/util/Constants.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/util/Constants.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/util/DisableStupidWarnings.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/util/DisableStupidWarnings.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/util/ForwardDeclarations.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/util/ForwardDeclarations.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/util/IndexedViewHelper.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/util/IndexedViewHelper.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/util/IntegralConstant.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/util/IntegralConstant.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/util/MKL_support.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/util/MKL_support.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/util/Macros.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/util/Macros.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/util/Memory.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/util/Memory.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/util/Meta.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/util/Meta.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/util/ReenableStupidWarnings.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/util/ReenableStupidWarnings.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/util/ReshapedHelper.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/util/ReshapedHelper.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/util/StaticAssert.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/util/StaticAssert.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/util/SymbolicIndex.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/util/SymbolicIndex.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Core/util/XprHelper.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Core/util/XprHelper.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Eigenvalues/ComplexEigenSolver.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Eigenvalues/ComplexEigenSolver.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Eigenvalues/ComplexSchur.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Eigenvalues/ComplexSchur.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Eigenvalues/ComplexSchur_LAPACKE.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Eigenvalues/ComplexSchur_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Eigenvalues/EigenSolver.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Eigenvalues/EigenSolver.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Eigenvalues/GeneralizedEigenSolver.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Eigenvalues/GeneralizedEigenSolver.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Eigenvalues/GeneralizedSelfAdjointEigenSolver.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Eigenvalues/GeneralizedSelfAdjointEigenSolver.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Eigenvalues/HessenbergDecomposition.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Eigenvalues/HessenbergDecomposition.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Eigenvalues/MatrixBaseEigenvalues.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Eigenvalues/MatrixBaseEigenvalues.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Eigenvalues/RealQZ.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Eigenvalues/RealQZ.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Eigenvalues/RealSchur.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Eigenvalues/RealSchur.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Eigenvalues/RealSchur_LAPACKE.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Eigenvalues/RealSchur_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Eigenvalues/SelfAdjointEigenSolver.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Eigenvalues/SelfAdjointEigenSolver.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Eigenvalues/SelfAdjointEigenSolver_LAPACKE.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Eigenvalues/SelfAdjointEigenSolver_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Eigenvalues/Tridiagonalization.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Eigenvalues/Tridiagonalization.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Geometry/AlignedBox.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Geometry/AlignedBox.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Geometry/AngleAxis.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Geometry/AngleAxis.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Geometry/EulerAngles.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Geometry/EulerAngles.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Geometry/Homogeneous.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Geometry/Homogeneous.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Geometry/Hyperplane.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Geometry/Hyperplane.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Geometry/OrthoMethods.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Geometry/OrthoMethods.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Geometry/ParametrizedLine.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Geometry/ParametrizedLine.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Geometry/Quaternion.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Geometry/Quaternion.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Geometry/Rotation2D.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Geometry/Rotation2D.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Geometry/RotationBase.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Geometry/RotationBase.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Geometry/Scaling.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Geometry/Scaling.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Geometry/Transform.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Geometry/Transform.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Geometry/Translation.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Geometry/Translation.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Geometry/Umeyama.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Geometry/Umeyama.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Geometry/arch/Geometry_SIMD.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Geometry/arch/Geometry_SIMD.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Householder/BlockHouseholder.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Householder/BlockHouseholder.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Householder/Householder.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Householder/Householder.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Householder/HouseholderSequence.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Householder/HouseholderSequence.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/IterativeLinearSolvers/BasicPreconditioners.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/IterativeLinearSolvers/BasicPreconditioners.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/IterativeLinearSolvers/BiCGSTAB.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/IterativeLinearSolvers/BiCGSTAB.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/IterativeLinearSolvers/ConjugateGradient.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/IterativeLinearSolvers/ConjugateGradient.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/IterativeLinearSolvers/IncompleteCholesky.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/IterativeLinearSolvers/IncompleteCholesky.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/IterativeLinearSolvers/IncompleteLUT.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/IterativeLinearSolvers/IncompleteLUT.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/IterativeLinearSolvers/IterativeSolverBase.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/IterativeLinearSolvers/IterativeSolverBase.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/IterativeLinearSolvers/LeastSquareConjugateGradient.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/IterativeLinearSolvers/LeastSquareConjugateGradient.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/IterativeLinearSolvers/SolveWithGuess.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/IterativeLinearSolvers/SolveWithGuess.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/Jacobi/Jacobi.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/Jacobi/Jacobi.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/LU/Determinant.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/LU/Determinant.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/LU/FullPivLU.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/LU/FullPivLU.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/LU/InverseImpl.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/LU/InverseImpl.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/LU/PartialPivLU.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/LU/PartialPivLU.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/LU/PartialPivLU_LAPACKE.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/LU/PartialPivLU_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/LU/arch/InverseSize4.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/LU/arch/InverseSize4.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/OrderingMethods/Amd.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/OrderingMethods/Amd.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/OrderingMethods/Eigen_Colamd.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/OrderingMethods/Eigen_Colamd.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/OrderingMethods/Ordering.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/OrderingMethods/Ordering.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/QR/ColPivHouseholderQR.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/QR/ColPivHouseholderQR.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/QR/ColPivHouseholderQR_LAPACKE.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/QR/ColPivHouseholderQR_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/QR/CompleteOrthogonalDecomposition.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/QR/CompleteOrthogonalDecomposition.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/QR/FullPivHouseholderQR.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/QR/FullPivHouseholderQR.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/QR/HouseholderQR.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/QR/HouseholderQR.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/QR/HouseholderQR_LAPACKE.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/QR/HouseholderQR_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/SVD/BDCSVD.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/SVD/BDCSVD.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/SVD/JacobiSVD.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/SVD/JacobiSVD.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/SVD/JacobiSVD_LAPACKE.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/SVD/JacobiSVD_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/SVD/SVDBase.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/SVD/SVDBase.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/SVD/UpperBidiagonalization.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/SVD/UpperBidiagonalization.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/SparseCholesky/SimplicialCholesky.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/SparseCholesky/SimplicialCholesky.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/SparseCholesky/SimplicialCholesky_impl.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/SparseCholesky/SimplicialCholesky_impl.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/SparseCore/AmbiVector.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/SparseCore/AmbiVector.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/SparseCore/CompressedStorage.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/SparseCore/CompressedStorage.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/SparseCore/ConservativeSparseSparseProduct.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/SparseCore/ConservativeSparseSparseProduct.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/SparseCore/MappedSparseMatrix.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/SparseCore/MappedSparseMatrix.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/SparseCore/SparseAssign.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/SparseCore/SparseAssign.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/SparseCore/SparseBlock.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/SparseCore/SparseBlock.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/SparseCore/SparseColEtree.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/SparseCore/SparseColEtree.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/SparseCore/SparseCompressedBase.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/SparseCore/SparseCompressedBase.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/SparseCore/SparseCwiseBinaryOp.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/SparseCore/SparseCwiseBinaryOp.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/SparseCore/SparseCwiseUnaryOp.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/SparseCore/SparseCwiseUnaryOp.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/SparseCore/SparseDenseProduct.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/SparseCore/SparseDenseProduct.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/SparseCore/SparseDiagonalProduct.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/SparseCore/SparseDiagonalProduct.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/SparseCore/SparseDot.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/SparseCore/SparseDot.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/SparseCore/SparseFuzzy.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/SparseCore/SparseFuzzy.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/SparseCore/SparseMap.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/SparseCore/SparseMap.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/SparseCore/SparseMatrix.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/SparseCore/SparseMatrix.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/SparseCore/SparseMatrixBase.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/SparseCore/SparseMatrixBase.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/SparseCore/SparsePermutation.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/SparseCore/SparsePermutation.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/SparseCore/SparseProduct.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/SparseCore/SparseProduct.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/SparseCore/SparseRedux.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/SparseCore/SparseRedux.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/SparseCore/SparseRef.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/SparseCore/SparseRef.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/SparseCore/SparseSelfAdjointView.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/SparseCore/SparseSelfAdjointView.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/SparseCore/SparseSolverBase.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/SparseCore/SparseSolverBase.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/SparseCore/SparseSparseProductWithPruning.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/SparseCore/SparseSparseProductWithPruning.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/SparseCore/SparseTranspose.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/SparseCore/SparseTranspose.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/SparseCore/SparseTriangularView.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/SparseCore/SparseTriangularView.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/SparseCore/SparseUtil.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/SparseCore/SparseUtil.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/SparseCore/SparseVector.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/SparseCore/SparseVector.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/SparseCore/SparseView.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/SparseCore/SparseView.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/SparseCore/TriangularSolver.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/SparseCore/TriangularSolver.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/SparseLU/SparseLU.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/SparseLU/SparseLU.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/SparseLU/SparseLUImpl.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/SparseLU/SparseLUImpl.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/SparseLU/SparseLU_Memory.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/SparseLU/SparseLU_Memory.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/SparseLU/SparseLU_Structs.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/SparseLU/SparseLU_Structs.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/SparseLU/SparseLU_SupernodalMatrix.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/SparseLU/SparseLU_SupernodalMatrix.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/SparseLU/SparseLU_Utils.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/SparseLU/SparseLU_Utils.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/SparseLU/SparseLU_column_bmod.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/SparseLU/SparseLU_column_bmod.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/SparseLU/SparseLU_column_dfs.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/SparseLU/SparseLU_column_dfs.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/SparseLU/SparseLU_copy_to_ucol.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/SparseLU/SparseLU_copy_to_ucol.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/SparseLU/SparseLU_gemm_kernel.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/SparseLU/SparseLU_gemm_kernel.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/SparseLU/SparseLU_heap_relax_snode.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/SparseLU/SparseLU_heap_relax_snode.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/SparseLU/SparseLU_kernel_bmod.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/SparseLU/SparseLU_kernel_bmod.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/SparseLU/SparseLU_panel_bmod.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/SparseLU/SparseLU_panel_bmod.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/SparseLU/SparseLU_panel_dfs.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/SparseLU/SparseLU_panel_dfs.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/SparseLU/SparseLU_pivotL.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/SparseLU/SparseLU_pivotL.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/SparseLU/SparseLU_pruneL.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/SparseLU/SparseLU_pruneL.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/SparseLU/SparseLU_relax_snode.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/SparseLU/SparseLU_relax_snode.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/SparseQR/SparseQR.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/SparseQR/SparseQR.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/misc/Image.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/misc/Image.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/misc/Kernel.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/misc/Kernel.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/misc/RealSvd2x2.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/misc/RealSvd2x2.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/misc/blas.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/misc/blas.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/misc/lapack.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/misc/lapack.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/misc/lapacke.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/misc/lapacke.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/plugins/ArrayCwiseBinaryOps.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/plugins/ArrayCwiseBinaryOps.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/plugins/ArrayCwiseUnaryOps.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/plugins/ArrayCwiseUnaryOps.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/plugins/BlockMethods.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/plugins/BlockMethods.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/plugins/CommonCwiseBinaryOps.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/plugins/CommonCwiseBinaryOps.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/plugins/CommonCwiseUnaryOps.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/plugins/CommonCwiseUnaryOps.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/plugins/IndexedViewMethods.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/plugins/IndexedViewMethods.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/plugins/MatrixCwiseBinaryOps.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/plugins/MatrixCwiseBinaryOps.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/plugins/MatrixCwiseUnaryOps.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/plugins/MatrixCwiseUnaryOps.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/eigen/Eigen/src/plugins/ReshapedMethods.h` & `gpboost-1.2.2/compile/external_libs/eigen/Eigen/src/plugins/ReshapedMethods.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/fast_double_parser/CMakeLists.txt` & `gpboost-1.2.2/compile/external_libs/fast_double_parser/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/fast_double_parser/LICENSE` & `gpboost-1.2.2/compile/external_libs/fast_double_parser/LICENSE`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/fast_double_parser/LICENSE.BSL` & `gpboost-1.2.2/compile/external_libs/fast_double_parser/LICENSE.BSL`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/fast_double_parser/include/fast_double_parser.h` & `gpboost-1.2.2/compile/external_libs/fast_double_parser/include/fast_double_parser.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/fmt/CMakeLists.txt` & `gpboost-1.2.2/compile/external_libs/fmt/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/fmt/LICENSE.rst` & `gpboost-1.2.2/compile/external_libs/fmt/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/fmt/include/fmt/chrono.h` & `gpboost-1.2.2/compile/external_libs/fmt/include/fmt/chrono.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/fmt/include/fmt/color.h` & `gpboost-1.2.2/compile/external_libs/fmt/include/fmt/color.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/fmt/include/fmt/compile.h` & `gpboost-1.2.2/compile/external_libs/fmt/include/fmt/compile.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/fmt/include/fmt/core.h` & `gpboost-1.2.2/compile/external_libs/fmt/include/fmt/core.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/fmt/include/fmt/format-inl.h` & `gpboost-1.2.2/compile/external_libs/fmt/include/fmt/format-inl.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/fmt/include/fmt/format.h` & `gpboost-1.2.2/compile/external_libs/fmt/include/fmt/format.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/fmt/include/fmt/locale.h` & `gpboost-1.2.2/compile/external_libs/fmt/include/fmt/locale.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/fmt/include/fmt/os.h` & `gpboost-1.2.2/compile/external_libs/fmt/include/fmt/os.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/fmt/include/fmt/ostream.h` & `gpboost-1.2.2/compile/external_libs/fmt/include/fmt/ostream.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/fmt/include/fmt/printf.h` & `gpboost-1.2.2/compile/external_libs/fmt/include/fmt/printf.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/external_libs/fmt/include/fmt/ranges.h` & `gpboost-1.2.2/compile/external_libs/fmt/include/fmt/ranges.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/include/GPBoost/DF_utils.h` & `gpboost-1.2.2/compile/include/GPBoost/DF_utils.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/include/GPBoost/GP_utils.h` & `gpboost-1.2.2/compile/include/GPBoost/GP_utils.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/include/GPBoost/Vecchia_utils.h` & `gpboost-1.2.2/compile/include/GPBoost/Vecchia_utils.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/include/GPBoost/cov_fcts.h` & `gpboost-1.2.2/compile/include/GPBoost/cov_fcts.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/include/GPBoost/likelihoods.h` & `gpboost-1.2.2/compile/include/GPBoost/likelihoods.h`

 * *Files 14% similar despite different names*

```diff
@@ -1,3108 +1,3222 @@
-/*!
-* This file is part of GPBoost a C++ library for combining
-*	boosting with Gaussian process and mixed effects models
-*
-* Copyright (c) 2020 Fabio Sigrist. All rights reserved.
-*
-* Licensed under the Apache License Version 2.0. See LICENSE file in the project root for license information.
-* 
-* 
-*  EXPLANATIONS ON PARAMETERIZATIONS USED
-* 
-* For a "gamma" likelihood, the following density is used:
-*	f(y) = lambda^gamma / Gamma(gamma) * y^(gamma - 1) * exp(-lambda * y)
-*		- lambda = gamma * exp(-location_par) (i.e., mean(y) = exp(-location_par)
-*		- lambda = rate parameter, gamma = shape parameter, location_par = random plus fixed effects
-*		
-*/
-#ifndef GPB_LIKELIHOODS_
-#define GPB_LIKELIHOODS_
-
-#define _USE_MATH_DEFINES // for M_SQRT1_2 and M_PI
-#include <cmath>
-
-#include <GPBoost/type_defs.h>
-#include <GPBoost/sparse_matrix_utils.h>
-#include <GPBoost/DF_utils.h>
-#include <GPBoost/utils.h>
-
-#include <string>
-#include <set>
-#include <string>
-#include <vector>
-
-#include <LightGBM/utils/log.h>
-using LightGBM::Log;
-#include <LightGBM/meta.h>
-using LightGBM::label_t;
-
-//Mathematical constants usually defined in cmath
-#ifndef M_SQRT2
-#define M_SQRT2      1.414213562373095048801688724209698079 //sqrt(2)
-#endif
-
-#include <chrono>  // only for debugging
-#include <thread> // only for debugging
-
-namespace GPBoost {
-
-	/*!
-	* \brief This class implements the likelihoods for the Gaussian proceses
-	* The template parameters <T_mat, T_chol> can be <den_mat_t, chol_den_mat_t> , <sp_mat_t, chol_sp_mat_t>, <sp_mat_rm_t, chol_sp_mat_rm_t>
-	*/
-	template<typename T_mat, typename T_chol>
-	class Likelihood {
-	public:
-		/*! \brief Constructor */
-		Likelihood();
-
-		/*!
-		* \brief Constructor
-		* \param type Type of likelihood
-		* \param num_data Number of data points
-		* \param num_re Number of random effects
-		* \param Indicates whether the vector a_vec_ / a=ZSigmaZt^-1 is used or not
-		*/
-		Likelihood(string_t type,
-			data_size_t num_data,
-			data_size_t num_re,
-			bool has_a_vec) {
-			string_t likelihood = ParseLikelihoodAlias(type);
-			if (SUPPORTED_LIKELIHOODS_.find(likelihood) == SUPPORTED_LIKELIHOODS_.end()) {
-				Log::REFatal("Likelihood of type '%s' is not supported.", likelihood.c_str());
-			}
-			likelihood_type_ = likelihood;
-			num_data_ = num_data;
-			num_re_ = num_re;
-			num_aux_pars_ = 0;
-			if (likelihood_type_ == "gamma") {
-				aux_pars_ = { 1. };//shape parameter
-				names_aux_pars_ = { "shape" };
-				num_aux_pars_ = 1;
-			}
-			else if (likelihood_type_ == "gaussian") {
-				aux_pars_ = { 1. };//1 / sqrt(variance)
-				names_aux_pars_ = { "inverse_std_dev" };
-			}
-			chol_fact_pattern_analyzed_ = false;
-			has_a_vec_ = has_a_vec;
-		}
-
-		/*!
-		* \brief Initialize mode vector_ (used in Laplace approximation for non-Gaussian data)
-		*/
-		void InitializeModeAvec() {
-			mode_ = vec_t::Zero(num_re_);
-			mode_previous_value_ = vec_t::Zero(num_re_);
-			if (has_a_vec_) {
-				a_vec_ = vec_t::Zero(num_re_);
-				a_vec_previous_value_ = vec_t::Zero(num_re_);
-			}
-			mode_initialized_ = true;
-			first_deriv_ll_ = vec_t(num_data_);
-			second_deriv_neg_ll_ = vec_t(num_data_);
-			mode_has_been_calculated_ = false;
-			na_or_inf_during_last_call_to_find_mode_ = false;
-			na_or_inf_during_second_last_call_to_find_mode_ = false;
-		}
-
-		/*!
-		* \brief Reset mode to previous value. This is used if too large step-sizes are done which result in increases in the objective function.
-		"			The values (covariance parameters and linear coefficients) are then discarded and consequently the mode should also be reset to the previous value)
-		*/
-		void ResetModeToPreviousValue() {
-			CHECK(mode_initialized_);
-			mode_ = mode_previous_value_;
-			if (has_a_vec_) {
-				a_vec_ = a_vec_previous_value_;
-			}
-			na_or_inf_during_last_call_to_find_mode_ = na_or_inf_during_second_last_call_to_find_mode_;
-		}
-
-		/*! \brief Destructor */
-		~Likelihood() {
-		}
-
-		/*!
-		* \brief Returns the type of likelihood
-		*/
-		string_t GetLikelihood() const {
-			return(likelihood_type_);
-		}
-
-		/*!
-		* \brief Set the type of likelihood
-		* \param type Likelihood name
-		*/
-		void SetLikelihood(const string_t& type) {
-			string_t likelihood = ParseLikelihoodAlias(type);
-			if (SUPPORTED_LIKELIHOODS_.find(likelihood) == SUPPORTED_LIKELIHOODS_.end()) {
-				Log::REFatal("Likelihood of type '%s' is not supported.", likelihood.c_str());
-			}
-			likelihood_type_ = likelihood;
-			chol_fact_pattern_analyzed_ = false;
-		}
-
-		/*!
-		* \brief Returns the type of the response variable (label). Either "double" or "int"
-		*/
-		string_t label_type() const {
-			if (likelihood_type_ == "bernoulli_probit" || likelihood_type_ == "bernoulli_logit" ||
-				likelihood_type_ == "poisson") {
-				return("int");
-			}
-			else {
-				return("double");
-			}
-		}
-
-		/*!
-		* \brief Returns a pointer to mode_
-		*/
-		const vec_t* GetMode() const {
-			return(&mode_);
-		}
-
-		/*!
-		* \brief Returns a pointer to first_deriv_ll_
-		*/
-		const vec_t* GetFirstDerivLL() const {
-			return(&first_deriv_ll_);
-		}
-
-		/*!
-		* \brief Checks whether the response variables (labels) have the correct values
-		* \param y_data Response variable data
-		* \param num_data Number of data points
-		*/
-		template <typename T>//T can be double or float
-		void CheckY(const T* y_data, 
-			const data_size_t num_data) const {
-			if (likelihood_type_ == "bernoulli_probit" || likelihood_type_ == "bernoulli_logit") {
-				//#pragma omp parallel for schedule(static)//problematic with error message below... 
-				for (data_size_t i = 0; i < num_data; ++i) {
-					if (fabs(y_data[i]) >= EPSILON_NUMBERS && !TwoNumbersAreEqual<T>(y_data[i], 1.)) {
-						Log::REFatal("Response variable (label) data needs to be 0 or 1 for likelihood of type '%s' ", likelihood_type_.c_str());
-					}
-				}
-			}
-			else if (likelihood_type_ == "poisson") {
-				for (data_size_t i = 0; i < num_data; ++i) {
-					if (y_data[i] < 0) {
-						Log::REFatal("Found negative response variable. Response variable cannot be negative for likelihood of type '%s' ", likelihood_type_.c_str());
-					}
-					else {
-						double intpart;
-						if (std::modf(y_data[i], &intpart) != 0.0) {
-							Log::REFatal("Found non-integer response variable. Response variable can only be integer valued for likelihood of type '%s' ", likelihood_type_.c_str());
-						}
-					}
-				}
-			}
-			else if (likelihood_type_ == "gamma") {
-				for (data_size_t i = 0; i < num_data; ++i) {
-					if (y_data[i] < 0) {
-						Log::REFatal("Found negative response variable. Response variable cannot be negative for likelihood of type '%s' ", likelihood_type_.c_str());
-					}
-				}
-			}
-			else {
-				Log::REFatal("GPModel: Likelihood of type '%s' is not supported ", likelihood_type_.c_str());
-			}
-		}//end CheckY
-
-		/*!
-		* \brief Determine initial value for intercept (=constant)
-		* \param y_data Response variable data
-		* \param num_data Number of data points
-		* param rand_eff_var Variance of random effects
-		*/
-		double FindInitialIntercept(const double* y_data, 
-			const data_size_t num_data,
-			double rand_eff_var) const {
-			CHECK(rand_eff_var > 0.);
-			double init_intercept = 0.;
-			if (likelihood_type_ == "gaussian") {
-#pragma omp parallel for schedule(static) reduction(+:init_intercept)
-				for (data_size_t i = 0; i < num_data; ++i) {
-					init_intercept += y_data[i];
-				}
-				init_intercept /= num_data;
-			}
-			else if (likelihood_type_ == "bernoulli_probit" || likelihood_type_ == "bernoulli_logit") {
-				double pavg = 0.;
-#pragma omp parallel for schedule(static) reduction(+:pavg)
-				for (data_size_t i = 0; i < num_data; ++i) {
-					pavg += bool(y_data[i] > 0);
-				}
-				pavg /= num_data;
-				pavg = std::min(pavg, 1.0 - 1e-15);
-				pavg = std::max<double>(pavg, 1e-15);
-				if (likelihood_type_ == "bernoulli_logit") {
-					init_intercept = std::log(pavg / (1.0 - pavg));
-				}
-				else {
-					init_intercept = normalQF(pavg);
-				}
-			}
-			else if (likelihood_type_ == "poisson" || likelihood_type_ == "gamma") {
-				double avg = 0.;
-#pragma omp parallel for schedule(static) reduction(+:avg)
-				for (data_size_t i = 0; i < num_data; ++i) {
-					avg += y_data[i];
-				}
-				avg /= num_data;
-				init_intercept = SafeLog(avg) - 0.5 * rand_eff_var; // log-normal distribution: mean of exp(beta_0 + Zb) = exp(beta_0 + 0.5 * sigma^2) => use beta_0 = mean(y) - 0.5 * sigma^2
-			}
-			else {
-				Log::REFatal("FindInitialIntercept: Likelihood of type '%s' is not supported.", likelihood_type_.c_str());
-			}
-			return(init_intercept);
-		}//end FindInitialIntercept
-
-		/*!
-		* \brief Determine initial value for intercept (=constant)
-		* \param y_data Response variable data
-		* \param num_data Number of data points
-		* \param rand_eff_var Variance of random effects
-		*/
-		bool ShouldHaveIntercept(const double* y_data, 
-			const data_size_t num_data,
-			double rand_eff_var) const {
-			bool ret_val = false;
-			if (likelihood_type_ == "poisson" || likelihood_type_ == "gamma") {
-				ret_val = true;
-			}
-			else {
-				double beta_zero = FindInitialIntercept(y_data, num_data, rand_eff_var);
-				if (std::abs(beta_zero) > 0.1) {
-					ret_val = true;
-				}
-			}
-			return(ret_val);
-		}
-
-		/*!
-		* \brief Determine initial value for additional likelihood parameters (e.g., shape for gamma)
-		* \param y_data Response variable data
-		* \param num_data Number of data points
-		*/
-		const double* FindInitialAuxPars(const double* y_data,
-			const data_size_t num_data) {
-			if (likelihood_type_ == "gamma") {
-				// Use a simple "MLE" approach for the shape parameter ignoring random and fixed effects and 
-				//	using the approximation: ln(k) - digamma(k) approx = (1 + 1 / (6k + 1)) / (2k), where k = shape
-				//	See https://en.wikipedia.org/wiki/Gamma_distribution#Maximum_likelihood_estimation (as of 02.03.2023)
-				double log_avg = 0., avg_log = 0.;
-#pragma omp parallel for schedule(static) reduction(+:log_avg, avg_log)
-				for (data_size_t i = 0; i < num_data; ++i) {
-					log_avg += y_data[i];
-					avg_log += std::log(y_data[i]);
-				}
-				log_avg /= num_data;
-				log_avg = std::log(log_avg);
-				avg_log /= num_data;
-				double s = log_avg - avg_log;
-				aux_pars_[0] = (3. - s + std::sqrt((s - 3.) * (s - 3.) + 24. * s)) / (12. * s);
-			}
-			else if (likelihood_type_ != "gaussian" && likelihood_type_ != "bernoulli_probit" &&
-				likelihood_type_ != "bernoulli_logit" && likelihood_type_ != "poisson") {
-				Log::REFatal("FindInitialAuxPars: Likelihood of type '%s' is not supported ", likelihood_type_.c_str());
-			}
-			return(aux_pars_.data());
-		}//end FindInitialAuxPars
-
-		/*!
-		* \brief Returns the number of additional parameters
-		*/
-		int NumAuxPars() const {
-			return(num_aux_pars_);
-		}
-
-		/*!
-		* \brief Returns a pointer to aux_pars_
-		*/
-		const double* GetAuxPars() const {
-			return(aux_pars_.data());
-		}
-
-		/*!
-		* \brief Set aux_pars_
-		* \param aux_pars New values for aux_pars_
-		*/
-		void SetAuxPars(const double* aux_pars) {
-			if (likelihood_type_ == "gamma") {
-				CHECK(aux_pars[0] > 0);
-				aux_pars_[0] = aux_pars[0];
-			}
-			else if (likelihood_type_ == "gaussian") {
-				CHECK(aux_pars[0] > 0);
-				aux_pars_[0] = aux_pars[0];
-			}
-			normalizing_constant_has_been_calculated_ = false;
-			aux_pars_have_been_set_ = true;
-		}
-
-		const char* GetNameAuxPars(int ind_aux_par) const {
-			CHECK(ind_aux_par < num_aux_pars_);
-			return(names_aux_pars_[ind_aux_par].c_str());
-		}
-
-		void GetNameFirstAuxPar(string_t& name) const {
-			name = names_aux_pars_[0];
-		}
-
-		bool AuxParsHaveBeenSet() const {
-			return(aux_pars_have_been_set_);
-		}
-
-		/*!
-		* \brief Calculate auxiliary quantity for the logarithm of normalizing constant of the likelihood
-		* \param y_data Response variable data if response variable is continuous
-		* \param y_data_int Response variable data if response variable is integer-valued
-		* \param num_data Number of data points
-		*/
-		void CalculateAuxQuantLogNormalizingConstant(const double* y_data,
-			const int*,
-			const data_size_t num_data) {
-			if (!aux_normalizing_constant_has_been_calculated_) {
-				if (likelihood_type_ == "gamma") {
-					double log_aux_normalizing_constant = 0.;
-#pragma omp parallel for schedule(static) reduction(+:log_aux_normalizing_constant)
-					for (data_size_t i = 0; i < num_data; ++i) {
-						log_aux_normalizing_constant += AuxQuantLogNormalizingConstantGamma(y_data[i]);
-					}
-					aux_log_normalizing_constant_ = log_aux_normalizing_constant;
-				}
-				else if (likelihood_type_ != "gaussian" && likelihood_type_ != "bernoulli_probit" &&
-					likelihood_type_ != "bernoulli_logit" && likelihood_type_ != "poisson") {
-					Log::REFatal("CalculateAuxQuantLogNormalizingConstant: Likelihood of type '%s' is not supported ", likelihood_type_.c_str());
-				}
-				aux_normalizing_constant_has_been_calculated_ = true;
-			}
-		}//end CalculateAuxQuantLogNormalizingConstant
-
-		inline double AuxQuantLogNormalizingConstantGamma(const double y) const {
-			return(std::log(y));
-		}
-
-		/*!
-		* \brief Calculate the logarithm of the normalizing constant of the likelihood
-		* \param y_data Response variable data if response variable is continuous
-		* \param y_data_int Response variable data if response variable is integer-valued
-		* \param num_data Number of data points
-		*/
-		void CalculateLogNormalizingConstant(const double* y_data,
-			const int* y_data_int,
-			const data_size_t num_data) {
-			if (!normalizing_constant_has_been_calculated_) {
-				CalculateAuxQuantLogNormalizingConstant(y_data, y_data_int, num_data);
-				if (likelihood_type_ == "poisson") {
-					double aux_const = 0.;
-#pragma omp parallel for schedule(static) if (num_data >= 128) reduction(+:aux_const)
-					for (data_size_t i = 0; i < num_data; ++i) {
-						aux_const += LogNormalizingConstantPoisson(y_data_int[i]);
-					}
-					log_normalizing_constant_ = aux_const;
-				}
-				else if (likelihood_type_ == "gamma") {
-					log_normalizing_constant_ = LogNormalizingConstantGamma(1., num_data, false);//note: the first argument is not used
-				}
-				else if (likelihood_type_ != "gaussian" && likelihood_type_ != "bernoulli_probit" &&
-					likelihood_type_ != "bernoulli_logit") {
-					Log::REFatal("CalculateLogNormalizingConstant: Likelihood of type '%s' is not supported ", likelihood_type_.c_str());
-				}
-				normalizing_constant_has_been_calculated_ = true;
-			}
-		}//end CalculateLogNormalizingConstant
-
-		inline double LogNormalizingConstantPoisson(const int y) const {
-			if (y > 1) {
-				double log_factorial = 0.;
-				for (int k = 2; k <= y; ++k) {
-					log_factorial += std::log(k);
-				}
-				return(-log_factorial);
-			}
-			else {
-				return(0.);
-			}
-		}
-
-		inline double LogNormalizingConstantGamma(const double y, const int num_data, bool calculate_aux_const) const {
-			if (TwoNumbersAreEqual<double>(aux_pars_[0], 1.)) {
-				return(0.);
-			}
-			else {
-				if (calculate_aux_const) {
-					return((aux_pars_[0] - 1.) * AuxQuantLogNormalizingConstantGamma(y) +
-						num_data * (aux_pars_[0] * std::log(aux_pars_[0]) - std::lgamma(aux_pars_[0])));
-				}
-				else {
-					return((aux_pars_[0] - 1.) * aux_log_normalizing_constant_ +
-						num_data * (aux_pars_[0] * std::log(aux_pars_[0]) - std::lgamma(aux_pars_[0])));
-				}
-			}
-		}
-
-		/*!
-		* \brief Evaluate the log-likelihood conditional on the latent variable (=location_par)
-		* \param y_data Response variable data if response variable is continuous
-		* \param y_data_int Response variable data if response variable is integer-valued
-		* \param location_par Location parameter (random plus fixed effects)
-		* \param num_data Number of data points
-		*/
-		double LogLikelihood(const double* y_data,
-			const int* y_data_int,
-			const double* location_par,
-			const data_size_t num_data) {
-			CalculateLogNormalizingConstant(y_data, y_data_int, num_data);
-			double ll = 0.;
-			if (likelihood_type_ == "bernoulli_probit") {
-#pragma omp parallel for schedule(static) if (num_data >= 128) reduction(+:ll)
-				for (data_size_t i = 0; i < num_data; ++i) {
-					ll += LogLikBernoulliProbit(y_data_int[i], location_par[i]);
-				}
-			}
-			else if (likelihood_type_ == "bernoulli_logit") {
-#pragma omp parallel for schedule(static) if (num_data >= 128) reduction(+:ll)
-				for (data_size_t i = 0; i < num_data; ++i) {
-					ll += LogLikBernoulliLogit(y_data_int[i], location_par[i]);
-				}
-			}
-			else if (likelihood_type_ == "poisson") {
-#pragma omp parallel for schedule(static) if (num_data >= 128) reduction(+:ll)
-				for (data_size_t i = 0; i < num_data; ++i) {
-					ll += LogLikPoisson(y_data_int[i], location_par[i], false);
-				}
-				ll += log_normalizing_constant_;
-			}
-			else if (likelihood_type_ == "gamma") {
-#pragma omp parallel for schedule(static) if (num_data >= 128) reduction(+:ll)
-				for (data_size_t i = 0; i < num_data; ++i) {
-					ll += LogLikGamma(y_data[i], location_par[i], false);
-				}
-				ll += log_normalizing_constant_;
-			}
-			else if (likelihood_type_ == "gaussian") {
-#pragma omp parallel for schedule(static) if (num_data >= 128) reduction(+:ll)
-				for (data_size_t i = 0; i < num_data; ++i) {
-					ll += LogLikGaussian(y_data[i], location_par[i]);
-				}
-			}
-			else {
-				Log::REFatal("LogLikelihood: Likelihood of type '%s' is not supported.", likelihood_type_.c_str());
-			}
-			return(ll);
-		}//end LogLikelihood
-
-		/*!
-		* \brief Evaluate the log-likelihood conditional on the latent variable (=location_par)
-		* \param y_data Response variable data if response variable is continuous
-		* \param y_data_int Response variable data if response variable is integer-valued
-		* \param location_par Location parameter (random plus fixed effects)
-		*/
-		inline double LogLikelihood(const double y_data,
-			const int y_data_int,
-			const double location_par) const {
-			if (likelihood_type_ == "bernoulli_probit") {
-				return(LogLikBernoulliProbit(y_data_int, location_par));
-			}
-			else if (likelihood_type_ == "bernoulli_logit") {
-				return(LogLikBernoulliLogit(y_data_int, location_par));
-			}
-			else if (likelihood_type_ == "poisson") {
-				return(LogLikPoisson(y_data_int, location_par, true));
-			}
-			else if (likelihood_type_ == "gamma") {
-				return(LogLikGamma(y_data, location_par, true));
-			}
-			else if (likelihood_type_ == "gaussian") {
-				return(LogLikGaussian(y_data, location_par));
-			}
-			else {
-				Log::REFatal("LogLikelihood: Likelihood of type '%s' is not supported.", likelihood_type_.c_str());
-				return(-1e99);
-			}
-		}//end LogLikelihood
-
-		inline double LogLikBernoulliProbit(const int y, const double location_par) const {
-			if (y == 0) {
-				return std::log(1 - normalCDF(location_par));
-			}
-			else {
-				return std::log(normalCDF(location_par));
-			}
-		}
-
-		inline double LogLikBernoulliLogit(const int y, const double location_par) const {
-			return (y * location_par - std::log(1 + std::exp(location_par)));
-			//Alternative version:
-			//if (y == 0) {
-			//	ll += std::log(1 - CondMeanLikelihood(location_par));//CondMeanLikelihood = logistic function
-			//}
-			//else {
-			//	ll += std::log(CondMeanLikelihood(location_par));
-			//}
-		}
-
-		inline double LogLikPoisson(const int y, const double location_par, bool incl_norm_const) const {
-			if (incl_norm_const) {
-				return (y * location_par - std::exp(location_par) + LogNormalizingConstantPoisson(y));
-			}
-			else {
-				return (y * location_par - std::exp(location_par));
-			}
-		}
-
-		inline double LogLikGamma(const double y, const double location_par, bool incl_norm_const) const {
-			if (incl_norm_const) {
-				return (-aux_pars_[0] * (location_par + y * std::exp(-location_par)) + LogNormalizingConstantGamma(y, 1, true));
-			}
-			else {
-				return (-aux_pars_[0] * (location_par + y * std::exp(-location_par)));
-			}
-		}
-
-		inline double LogLikGaussian(const double y, const double location_par) const {
-			return (std::log(aux_pars_[0]) + normalLogPDF(aux_pars_[0] * (y - location_par)));//aux_pars_[0] = 1. / std::sqrt(variance)
-		}
-
-		/*!
-		* \brief Calculate the first derivative of the log-likelihood with respect to the location parameter
-		* \param y_data Response variable data if response variable is continuous
-		* \param y_data_int Response variable data if response variable is integer-valued
-		* \param location_par Location parameter (random plus fixed effects)
-		* \param num_data Number of data points
-		*/
-		void CalcFirstDerivLogLik(const double* y_data, 
-			const int* y_data_int,
-			const double* location_par, 
-			const data_size_t num_data) {
-			if (likelihood_type_ == "bernoulli_probit") {
-#pragma omp parallel for schedule(static) if (num_data >= 128)
-				for (data_size_t i = 0; i < num_data; ++i) {
-					first_deriv_ll_[i] = FirstDerivLogLikBernoulliProbit(y_data_int[i], location_par[i]);
-				}
-			}
-			else if (likelihood_type_ == "bernoulli_logit") {
-#pragma omp parallel for schedule(static) if (num_data >= 128)
-				for (data_size_t i = 0; i < num_data; ++i) {
-					first_deriv_ll_[i] = FirstDerivLogLikBernoulliLogit(y_data_int[i], location_par[i]);
-				}
-			}
-			else if (likelihood_type_ == "poisson") {
-#pragma omp parallel for schedule(static) if (num_data >= 128)
-				for (data_size_t i = 0; i < num_data; ++i) {
-					first_deriv_ll_[i] = FirstDerivLogLikPoisson(y_data_int[i], location_par[i]);
-				}
-			}
-			else if (likelihood_type_ == "gamma") {
-#pragma omp parallel for schedule(static) if (num_data >= 128)
-				for (data_size_t i = 0; i < num_data; ++i) {
-					first_deriv_ll_[i] = FirstDerivLogLikGamma(y_data[i], location_par[i]);
-				}
-			}
-			else if (likelihood_type_ == "gaussian") {
-#pragma omp parallel for schedule(static) if (num_data >= 128)
-				for (data_size_t i = 0; i < num_data; ++i) {
-					first_deriv_ll_[i] = FirstDerivLogLikGaussian(y_data[i], location_par[i]);
-				}
-			}
-			else {
-				Log::REFatal("CalcFirstDerivLogLik: Likelihood of type '%s' is not supported.", likelihood_type_.c_str());
-			}
-		}//end CalcFirstDerivLogLik
-
-		/*!
-		* \brief Calculate the first derivative of the log-likelihood with respect to the location parameter
-		* \param y_data Response variable data if response variable is continuous
-		* \param y_data_int Response variable data if response variable is integer-valued
-		* \param location_par Location parameter (random plus fixed effects)
-		*/
-		inline double CalcFirstDerivLogLik(const double y_data,
-			const int y_data_int,
-			const double location_par) const {
-			if (likelihood_type_ == "bernoulli_probit") {
-				return(FirstDerivLogLikBernoulliProbit(y_data_int, location_par));
-			}
-			else if (likelihood_type_ == "bernoulli_logit") {
-				return(FirstDerivLogLikBernoulliLogit(y_data_int, location_par));
-			}
-			else if (likelihood_type_ == "poisson") {
-				return(FirstDerivLogLikPoisson(y_data_int, location_par));
-			}
-			else if (likelihood_type_ == "gamma") {
-				return(FirstDerivLogLikGamma(y_data, location_par));
-			}
-			else if (likelihood_type_ == "gaussian") {
-				return(FirstDerivLogLikGaussian(y_data, location_par));
-			}
-			else {
-				Log::REFatal("CalcFirstDerivLogLik: Likelihood of type '%s' is not supported.", likelihood_type_.c_str());
-				return(0.);
-			}
-		}//end CalcFirstDerivLogLik
-
-		inline double FirstDerivLogLikBernoulliProbit(const int y, const double location_par) const {
-			if (y == 0) {
-				return (-normalPDF(location_par) / (1 - normalCDF(location_par)));
-			}
-			else {
-				return (normalPDF(location_par) / normalCDF(location_par));
-			}
-		}
-
-		inline double FirstDerivLogLikBernoulliLogit(const int y, const double location_par) const {
-			return (y - CondMeanLikelihood(location_par));//CondMeanLikelihood = logistic(x)
-		}
-
-		inline double FirstDerivLogLikPoisson(const int y, const double location_par) const {
-			return (y - std::exp(location_par));
-		}
-
-		inline double FirstDerivLogLikGamma(const double y, const double location_par) const {
-			return (aux_pars_[0] * (y * std::exp(-location_par) - 1.));
-		}
-
-		inline double FirstDerivLogLikGaussian(const double y, const double location_par) const {
-			return (aux_pars_[0] * aux_pars_[0] * (y - location_par));
-		}
-
-		/*!
-		* \brief Calculate the second derivative of the negative (!) log-likelihood with respect to the location parameter
-		* \param y_data Response variable data if response variable is continuous
-		* \param y_data_int Response variable data if response variable is integer-valued
-		* \param location_par Location parameter (random plus fixed effects)
-		* \param num_data Number of data points
-		*/
-		void CalcSecondDerivNegLogLik(const double* y_data, 
-			const int* y_data_int,
-			const double* location_par, 
-			const data_size_t num_data) {
-			if (likelihood_type_ == "bernoulli_probit") {
-#pragma omp parallel for schedule(static) if (num_data >= 128)
-				for (data_size_t i = 0; i < num_data; ++i) {
-					second_deriv_neg_ll_[i] = SecondDerivNegLogLikBernoulliProbit(y_data_int[i], location_par[i]);
-				}
-			}
-			else if (likelihood_type_ == "bernoulli_logit") {
-#pragma omp parallel for schedule(static) if (num_data >= 128)
-				for (data_size_t i = 0; i < num_data; ++i) {
-					second_deriv_neg_ll_[i] = SecondDerivNegLogLikBernoulliLogit(location_par[i]);
-				}
-			}
-			else if (likelihood_type_ == "poisson") {
-#pragma omp parallel for schedule(static) if (num_data >= 128)
-				for (data_size_t i = 0; i < num_data; ++i) {
-					second_deriv_neg_ll_[i] = SecondDerivNegLogLikPoisson(location_par[i]);
-				}
-			}
-			else if (likelihood_type_ == "gamma") {
-#pragma omp parallel for schedule(static) if (num_data >= 128)
-				for (data_size_t i = 0; i < num_data; ++i) {
-					second_deriv_neg_ll_[i] = SecondDerivNegLogLikGamma(y_data[i], location_par[i]);
-				}
-			}
-			else if (likelihood_type_ == "gaussian") {
-#pragma omp parallel for schedule(static) if (num_data >= 128)
-				for (data_size_t i = 0; i < num_data; ++i) {
-					second_deriv_neg_ll_[i] = SecondDerivNegLogLikGaussian();
-				}
-			}
-			else {
-				Log::REFatal("CalcSecondDerivNegLogLik: Likelihood of type '%s' is not supported.", likelihood_type_.c_str());
-			}
-		}// end CalcSecondDerivNegLogLik
-
-		/*!
-		* \brief Calculate the second derivative of the negative (!) log-likelihood with respect to the location parameter
-		* \param y_data Response variable data if response variable is continuous
-		* \param y_data_int Response variable data if response variable is integer-valued
-		* \param location_par Location parameter (random plus fixed effects)
-		*/
-		inline double CalcSecondDerivNegLogLik(const double y_data,
-			const int y_data_int,
-			const double location_par) const {
-			if (likelihood_type_ == "bernoulli_probit") {
-				return(SecondDerivNegLogLikBernoulliProbit(y_data_int, location_par));
-			}
-			else if (likelihood_type_ == "bernoulli_logit") {
-				return(SecondDerivNegLogLikBernoulliLogit(location_par));
-			}
-			else if (likelihood_type_ == "poisson") {
-				return(SecondDerivNegLogLikPoisson(location_par));
-			}
-			else if (likelihood_type_ == "gamma") {
-				return(SecondDerivNegLogLikGamma(y_data, location_par));
-			}
-			else if (likelihood_type_ == "gaussian") {
-				return(SecondDerivNegLogLikGaussian());
-			}
-			else {
-				Log::REFatal("CalcSecondDerivNegLogLik: Likelihood of type '%s' is not supported.", likelihood_type_.c_str());
-				return(1.);
-			}
-		}// end CalcSecondDerivNegLogLik
-
-		inline double SecondDerivNegLogLikBernoulliProbit(const int y, const double location_par) const {
-			double dnorm = normalPDF(location_par);
-			double pnorm = normalCDF(location_par);
-			if (y == 0) {
-				double dnorm_frac_one_min_pnorm = dnorm / (1. - pnorm);
-				return (-dnorm_frac_one_min_pnorm * (location_par - dnorm_frac_one_min_pnorm));
-			}
-			else {
-				double dnorm_frac_pnorm = dnorm / pnorm;
-				return(dnorm_frac_pnorm * (location_par + dnorm_frac_pnorm));
-			}
-		}
-
-		inline double SecondDerivNegLogLikBernoulliLogit(const double location_par) const {
-			double exp_loc_i = std::exp(location_par);
-			return (exp_loc_i * std::pow(1. + exp_loc_i, -2));
-		}
-
-		inline double SecondDerivNegLogLikPoisson(const double location_par) const {
-			return std::exp(location_par);
-		}
-
-		inline double SecondDerivNegLogLikGamma(const double y, const double location_par) const {
-			return (aux_pars_[0] * y * std::exp(-location_par));
-		}
-
-		inline double SecondDerivNegLogLikGaussian() const {
-			return (aux_pars_[0] * aux_pars_[0]);//aux_pars_[0] = 1 / sqrt(variance)
-		}
-
-		/*!
-		* \brief Calculate the third derivative of the log-likelihood with respect to the location parameter
-		* \param y_data Response variable data if response variable is continuous
-		* \param y_data_int Response variable data if response variable is integer-valued
-		* \param location_par Location parameter (random plus fixed effects)
-		* \param num_data Number of data points
-		* \param[out] third_deriv Third derivative of the log-likelihood with respect to the location parameter. Need to pre-allocate memory of size num_data
-		*/
-		void CalcThirdDerivLogLik(const double* y_data, 
-			const int* y_data_int,
-			const double* location_par, 
-			const data_size_t num_data, 
-			double* third_deriv) const {
-			if (likelihood_type_ == "bernoulli_probit") {
-#pragma omp parallel for schedule(static) if (num_data >= 128)
-				for (data_size_t i = 0; i < num_data; ++i) {
-					double dnorm = normalPDF(location_par[i]);
-					double pnorm = normalCDF(location_par[i]);
-					if (y_data_int[i] == 0) {
-						double dnorm_frac_one_min_pnorm = dnorm / (1. - pnorm);
-						third_deriv[i] = dnorm_frac_one_min_pnorm * (1 - location_par[i] * location_par[i] +
-							dnorm_frac_one_min_pnorm * (3 * location_par[i] - 2 * dnorm_frac_one_min_pnorm));
-					}
-					else {
-						double dnorm_frac_pnorm = dnorm / pnorm;
-						third_deriv[i] = dnorm_frac_pnorm * (location_par[i] * location_par[i] - 1 +
-							dnorm_frac_pnorm * (3 * location_par[i] + 2 * dnorm_frac_pnorm));
-					}
-				}
-			}
-			else if (likelihood_type_ == "bernoulli_logit") {
-#pragma omp parallel for schedule(static) if (num_data >= 128)
-				for (data_size_t i = 0; i < num_data; ++i) {
-					double exp_loc_i = std::exp(location_par[i]);
-					third_deriv[i] = -exp_loc_i * (1. - exp_loc_i) * std::pow(1 + exp_loc_i, -3);
-				}
-			}
-			else if (likelihood_type_ == "poisson") {
-#pragma omp parallel for schedule(static) if (num_data >= 128)
-				for (data_size_t i = 0; i < num_data; ++i) {
-					third_deriv[i] = -std::exp(location_par[i]);
-				}
-			}
-			else if (likelihood_type_ == "gamma") {
-#pragma omp parallel for schedule(static) if (num_data >= 128)
-				for (data_size_t i = 0; i < num_data; ++i) {
-					third_deriv[i] = aux_pars_[0] * y_data[i] * std::exp(-location_par[i]);
-				}
-			}
-			else {
-				Log::REFatal("CalcThirdDerivLogLik: Likelihood of type '%s' is not supported.", likelihood_type_.c_str());
-			}
-		}//end CalcThirdDerivLogLik
-
-		/*!
-		* \brief Calculates the gradient of the negative log-likelihood with respect to the additional parameters of the likelihood (e.g., shape for gamma)
-		* \param y_data Response variable data if response variable is continuous
-		* \param location_par Location parameter (random plus fixed effects)
-		* \param num_data Number of data points
-		* \param[out] grad Gradient
-		*/
-		void CalcGradNegLogLikAuxPars(const double* y_data,
-			const double* location_par,
-			const data_size_t num_data,
-			double* grad) const {
-			if (likelihood_type_ == "gamma") {
-				double neg_log_grad = 0.;//gradient for shape parameter is calculated on the log-scale
-#pragma omp parallel for schedule(static) reduction(+:neg_log_grad)
-				for (data_size_t i = 0; i < num_data; ++i) {
-					neg_log_grad += location_par[i] + y_data[i] * std::exp(-location_par[i]);
-				}
-				neg_log_grad -= num_data * (std::log(aux_pars_[0]) + 1. - digamma(aux_pars_[0]));
-				neg_log_grad -= aux_log_normalizing_constant_;
-				neg_log_grad *= aux_pars_[0];
-				grad[0] = neg_log_grad;
-			}
-			else if (likelihood_type_ != "gaussian" && likelihood_type_ != "bernoulli_probit" &&
-				likelihood_type_ != "bernoulli_logit" && likelihood_type_ != "poisson") {
-				Log::REFatal("CalcGradNegLogLikAuxPars: Likelihood of type '%s' is not supported.", likelihood_type_.c_str());
-			}
-		}//end CalcGradNegLogLikAuxPars
-
-		/*!
-		* \brief Calculates the second and the negative third derivative of the log-likelihood with respect to 
-		*			(i) once and twice the location parameter and (ii) an additional parameter of the likelihood 
-		* \param y_data Response variable data if response variable is continuous
-		* \param location_par Location parameter (random plus fixed effects)
-		* \param num_data Number of data points
-		* \param ind_aux_par Index of aux_pars_ wrt which the gradient is calculated (currently no used as there is only one)
-		* \param[out] second_deriv Second derivative
-		* \param[out] neg_third_deriv Negative third derivative
-		*/
-		void CalcSecondNegThirdDerivLogLikAuxParsLocPar(const double* y_data,
-			const double* location_par,
-			const data_size_t num_data,
-			int ind_aux_par,
-			double* second_deriv,
-			double* neg_third_deriv) const {
-			if (likelihood_type_ == "gamma") {
-				CHECK(ind_aux_par == 0);
-#pragma omp parallel for schedule(static)
-				for (data_size_t i = 0; i < num_data; ++i) {
-					second_deriv[i] = aux_pars_[0] * (y_data[i] * std::exp(-location_par[i]) - 1.);
-					neg_third_deriv[i] = second_deriv[i] + aux_pars_[0];
-				}
-			}
-			else if (likelihood_type_ != "gaussian" && likelihood_type_ != "bernoulli_probit" &&
-				likelihood_type_ != "bernoulli_logit" && likelihood_type_ != "poisson") {
-				Log::REFatal("CalcSecondDerivNegLogLikAuxParsLocPar: Likelihood of type '%s' is not supported.", likelihood_type_.c_str());
-			}
-		}//end CalcSecondNegThirdDerivLogLikAuxParsLocPar
-
-		/*!
-		* \brief Calculate the mean of the likelihood conditional on the (predicted) latent variable
-		*			Used for adaptive Gauss-Hermite quadrature for the prediction of the response variable
-		*/
-		inline double CondMeanLikelihood(const double value) const {
-			if (likelihood_type_ == "gaussian") {
-				return value;
-			}
-			else if (likelihood_type_ == "bernoulli_probit") {
-				return normalCDF(value);
-			}
-			else if (likelihood_type_ == "bernoulli_logit") {
-				return 1. / (1. + std::exp(-value));
-			}
-			else if (likelihood_type_ == "poisson") {
-				return std::exp(value);
-			}
-			else if (likelihood_type_ == "gamma") {
-				return std::exp(value);
-			}
-			else {
-				Log::REFatal("CondMeanLikelihood: Likelihood of type '%s' is not supported.", likelihood_type_.c_str());
-				return 0.;
-			}
-		}
-
-		/*!
-		* \brief Calculate the first derivative of the logarithm of the mean of the likelihood conditional on the (predicted) latent variable
-		*			Used for adaptive Gauss-Hermite quadrature for the prediction of the response variable
-		*/
-		inline double FirstDerivLogCondMeanLikelihood(const double value) const {
-			if (likelihood_type_ == "bernoulli_logit") {
-				return 1. / (1. + std::exp(value));
-			}
-			else if (likelihood_type_ == "poisson") {
-				return 1.;
-			}
-			else if (likelihood_type_ == "gamma") {
-				return 1.;
-			}
-			else {
-				Log::REFatal("FirstDerivLogCondMeanLikelihood: Likelihood of type '%s' is not supported.", likelihood_type_.c_str());
-				return 0.;
-			}
-		}
-
-		/*!
-		* \brief Calculate the second derivative of the logarithm of the mean of the likelihood conditional on the (predicted) latent variable
-		*			Used for adaptive Gauss-Hermite quadrature for the prediction of the response variable
-		*/
-		inline double SecondDerivLogCondMeanLikelihood(const double value) const {
-			if (likelihood_type_ == "bernoulli_logit") {
-				double exp_x = std::exp(value);
-				return -exp_x / ((1. + exp_x) * (1. + exp_x));
-			}
-			else if (likelihood_type_ == "poisson") {
-				return 0.;
-			}
-			else if (likelihood_type_ == "gamma") {
-				return 0.;
-			}
-			else {
-				Log::REFatal("SecondDerivLogCondMeanLikelihood: Likelihood of type '%s' is not supported.", likelihood_type_.c_str());
-				return 0.;
-			}
-		}
-
-		/*!
-		* \brief Do Cholesky decomposition
-		* \param[out] chol_fact Cholesky factor
-		* \param psi Matrix for which the Cholesky decomposition should be done
-		*/
-		template <class T_mat_1,  typename std::enable_if <std::is_same<sp_mat_t, T_mat_1>::value ||
-			std::is_same<sp_mat_rm_t, T_mat_1>::value>::type * = nullptr >
-		void CalcChol(T_chol& chol_fact, const T_mat_1& psi) {
-			if (!chol_fact_pattern_analyzed_) {
-				chol_fact.analyzePattern(psi);
-				chol_fact_pattern_analyzed_ = true;
-			}
-			chol_fact.factorize(psi);
-		}
-		template <class T_mat_1, typename std::enable_if <std::is_same<den_mat_t, T_mat_1>::value>::type * = nullptr  >
-		void CalcChol(T_chol& chol_fact, const T_mat_1& psi) {
-			chol_fact.compute(psi);
-		}
-
-		/*!
-		* \brief Find the mode of the posterior of the latent random effects using Newton's method and calculate the approximative marginal log-likelihood..
-		*		Calculations are done using a numerically stable variant based on factorizing ("inverting") B = (Id + Wsqrt * Z*Sigma*Zt * Wsqrt).
-		*		In the notation of the paper: "Sigma = Z*Sigma*Z^T" and "Z = Id".
-		*		This version is used for the Laplace approximation when dense matrices are used (e.g. GP models).
-		* \param y_data Response variable data if response variable is continuous
-		* \param y_data_int Response variable data if response variable is integer-valued
-		* \param fixed_effects Fixed effects component of location parameter
-		* \param num_data Number of data points
-		* \param ZSigmaZt Covariance matrix of latent random effect
-		* \param[out] approx_marginal_ll Approximate marginal log-likelihood evaluated at the mode
-		*/
-		void FindModePostRandEffCalcMLLStable(const double* y_data,
-			const int* y_data_int,
-			const double* fixed_effects,
-			const data_size_t num_data,
-			const std::shared_ptr<T_mat> ZSigmaZt,
-			double& approx_marginal_ll) {
-			// Initialize variables
-			if (!mode_initialized_) {
-				InitializeModeAvec();
-			}
-			else {
-				mode_previous_value_ = mode_;
-				a_vec_previous_value_ = a_vec_;
-				na_or_inf_during_second_last_call_to_find_mode_ = na_or_inf_during_last_call_to_find_mode_;
-			}
-			bool no_fixed_effects = (fixed_effects == nullptr);
-			vec_t location_par;
-			// Initialize objective function (LA approx. marginal likelihood) for use as convergence criterion
-			if (no_fixed_effects) {
-				approx_marginal_ll = -0.5 * (a_vec_.dot(mode_)) + LogLikelihood(y_data, y_data_int, mode_.data(), num_data);
-			}
-			else {
-				location_par = vec_t(num_data);
-#pragma omp parallel for schedule(static)
-				for (data_size_t i = 0; i < num_data; ++i) {
-					location_par[i] = mode_[i] + fixed_effects[i];
-				}
-				approx_marginal_ll = -0.5 * (a_vec_.dot(mode_)) + LogLikelihood(y_data, y_data_int, location_par.data(), num_data);
-			}
-			double approx_marginal_ll_new = approx_marginal_ll;
-			vec_t rhs, v_aux;//auxiliary variables
-			vec_t Wsqrt(num_data);//diagonal matrix with square root of negative second derivatives on the diagonal (sqrt of negative Hessian of log-likelihood)
-			T_mat Id_plus_Wsqrt_ZSigmaZt_Wsqrt(num_data, num_data);
-			// Start finding mode 
-			int it;
-			bool terminate_optim = false;
-			bool has_NA_or_Inf = false;
-			for (it = 0; it < MAXIT_MODE_NEWTON_; ++it) {
-				// Calculate first and second derivative of log-likelihood
-				if (no_fixed_effects) {
-					CalcFirstDerivLogLik(y_data, y_data_int, mode_.data(), num_data);
-					CalcSecondDerivNegLogLik(y_data, y_data_int, mode_.data(), num_data);
-				}
-				else {
-					CalcFirstDerivLogLik(y_data, y_data_int, location_par.data(), num_data);
-					CalcSecondDerivNegLogLik(y_data, y_data_int, location_par.data(), num_data);
-				}
-				// Calculate Cholesky factor of matrix B = Id + Wsqrt * Z*Sigma*Zt * Wsqrt
-				Wsqrt.array() = second_deriv_neg_ll_.array().sqrt();
-				Id_plus_Wsqrt_ZSigmaZt_Wsqrt.setIdentity();
-				Id_plus_Wsqrt_ZSigmaZt_Wsqrt += (Wsqrt.asDiagonal() * (*ZSigmaZt) * Wsqrt.asDiagonal());
-				CalcChol<T_mat>(chol_fact_Id_plus_Wsqrt_Sigma_Wsqrt_, Id_plus_Wsqrt_ZSigmaZt_Wsqrt);
-				// Update mode and a_vec_
-				rhs.array() = second_deriv_neg_ll_.array() * mode_.array() + first_deriv_ll_.array();
-				v_aux = Wsqrt.asDiagonal() * (*ZSigmaZt) * rhs;
-				a_vec_ = rhs - Wsqrt.asDiagonal() * (chol_fact_Id_plus_Wsqrt_Sigma_Wsqrt_.solve(v_aux));
-				mode_ = (*ZSigmaZt) * a_vec_;
-				// Calculate new objective function
-				if (no_fixed_effects) {
-					approx_marginal_ll_new = -0.5 * (a_vec_.dot(mode_)) + LogLikelihood(y_data, y_data_int, mode_.data(), num_data);
-				}
-				else {
-					// Update location parameter of log-likelihood for calculation of approx. marginal log-likelihood (objective function)
-#pragma omp parallel for schedule(static)
-					for (data_size_t i = 0; i < num_data; ++i) {
-						location_par[i] = mode_[i] + fixed_effects[i];
-					}
-					approx_marginal_ll_new = -0.5 * (a_vec_.dot(mode_)) + LogLikelihood(y_data, y_data_int, location_par.data(), num_data);
-				}
-				if (std::isnan(approx_marginal_ll_new) || std::isinf(approx_marginal_ll_new)) {
-					has_NA_or_Inf = true;
-					Log::REDebug(NA_OR_INF_WARNING_);
-					break;
-				}
-				// Check convergence
-				if (it == 0) {
-					if (std::abs(approx_marginal_ll_new - approx_marginal_ll) < DELTA_REL_CONV_ * std::abs(approx_marginal_ll)) { // allow for decreases in first iteration
-						terminate_optim = true;
-					}
-				}
-				else {
-					if ((approx_marginal_ll_new - approx_marginal_ll) < DELTA_REL_CONV_ * std::abs(approx_marginal_ll)) {
-						terminate_optim = true;
-					}
-				}
-				if (terminate_optim) {
-					if (approx_marginal_ll_new < approx_marginal_ll) {
-						Log::REDebug(NO_INCREASE_IN_MLL_WARNING_);
-					}
-					approx_marginal_ll = approx_marginal_ll_new;
-					break;
-				}
-				else {
-					approx_marginal_ll = approx_marginal_ll_new;
-				}
-			}
-			if (it == MAXIT_MODE_NEWTON_) {
-				Log::REDebug(NO_CONVERGENCE_WARNING_);
-			}
-			if (has_NA_or_Inf) {
-				approx_marginal_ll = approx_marginal_ll_new;
-				na_or_inf_during_last_call_to_find_mode_ = true;
-			}
-			else {
-				if (no_fixed_effects) {
-					CalcFirstDerivLogLik(y_data, y_data_int, mode_.data(), num_data);//first derivative is not used here anymore but since it is reused in gradient calculation and in prediction, we calculate it once more
-					CalcSecondDerivNegLogLik(y_data, y_data_int, mode_.data(), num_data);
-				}
-				else {
-					CalcFirstDerivLogLik(y_data, y_data_int, location_par.data(), num_data);//first derivative is not used here anymore but since it is reused in gradient calculation and in prediction, we calculate it once more
-					CalcSecondDerivNegLogLik(y_data, y_data_int, location_par.data(), num_data);
-				}
-				Wsqrt.array() = second_deriv_neg_ll_.array().sqrt();
-				Id_plus_Wsqrt_ZSigmaZt_Wsqrt.setIdentity();
-				Id_plus_Wsqrt_ZSigmaZt_Wsqrt += (Wsqrt.asDiagonal() * (*ZSigmaZt) * Wsqrt.asDiagonal());
-				CalcChol<T_mat>(chol_fact_Id_plus_Wsqrt_Sigma_Wsqrt_, Id_plus_Wsqrt_ZSigmaZt_Wsqrt);
-				approx_marginal_ll -= ((T_mat)chol_fact_Id_plus_Wsqrt_Sigma_Wsqrt_.matrixL()).diagonal().array().log().sum();
-				mode_has_been_calculated_ = true;
-				na_or_inf_during_last_call_to_find_mode_ = false;
-			}
-		}//end FindModePostRandEffCalcMLLStable
-
-		/*!
-		* \brief Find the mode of the posterior of the latent random effects using Newton's method and calculate the approximative marginal log-likelihood.
-		*		Calculations are done on the random effects (b) scale and not the "data scale" (Zb) using 
-		*		a numerically stable variant based on factorizing ("inverting") B = (Id + ZtWZsqrt * Sigma * ZtWZsqrt).
-		*		This version is used for the Laplace approximation when there is only one Gaussian process and
-		*		there are a lot of multiple observations at the same location, i.e., the dimenion of the random effects b is much smaller than Zb
-		* \param y_data Response variable data if response variable is continuous
-		* \param y_data_int Response variable data if response variable is integer-valued
-		* \param fixed_effects Fixed effects component of location parameter
-		* \param num_data Number of data points
-		* \param Sigma Covariance matrix of latent random effect
-		* \param random_effects_indices_of_data Indices that indicate to which random effect every data point is related
-		* \param[out] approx_marginal_ll Approximate marginal log-likelihood evaluated at the mode
-		*/
-		void FindModePostRandEffCalcMLLOnlyOneGPCalculationsOnREScale(const double* y_data,
-			const int* y_data_int,
-			const double* fixed_effects,
-			const data_size_t num_data,
-			const std::shared_ptr<T_mat> Sigma,
-			const data_size_t * const random_effects_indices_of_data,
-			double& approx_marginal_ll) {
-			// Initialize variables
-			if (!mode_initialized_) {
-				InitializeModeAvec();
-			}
-			else {
-				mode_previous_value_ = mode_;
-				a_vec_previous_value_ = a_vec_;
-				na_or_inf_during_second_last_call_to_find_mode_ = na_or_inf_during_last_call_to_find_mode_;
-			}
-			vec_t location_par(num_data);//location parameter = mode of random effects + fixed effects
-			if (fixed_effects == nullptr) {
-#pragma omp parallel for schedule(static)
-				for (data_size_t i = 0; i < num_data; ++i) {
-					location_par[i] = mode_[random_effects_indices_of_data[i]];
-				}
-			}
-			else {
-#pragma omp parallel for schedule(static)
-				for (data_size_t i = 0; i < num_data; ++i) {
-					location_par[i] = mode_[random_effects_indices_of_data[i]] + fixed_effects[i];
-				}
-			}
-			// Initialize objective function (LA approx. marginal likelihood) for use as convergence criterion
-			approx_marginal_ll = -0.5 * (a_vec_.dot(mode_)) + LogLikelihood(y_data, y_data_int, location_par.data(), num_data);
-			double approx_marginal_ll_new = approx_marginal_ll;
-			vec_t diag_sqrt_ZtWZ(num_re_);//sqrt of diagonal matrix ZtWZ
-			T_mat Id_plus_ZtWZsqrt_Sigma_ZtWZsqrt(num_re_, num_re_);
-			vec_t rhs, v_aux;
-			int it;
-			bool terminate_optim = false;
-			bool has_NA_or_Inf = false;
-			for (it = 0; it < MAXIT_MODE_NEWTON_; ++it) {
-				// Calculate first and second derivative of log-likelihood
-				CalcFirstDerivLogLik(y_data, y_data_int, location_par.data(), num_data);
-				CalcSecondDerivNegLogLik(y_data, y_data_int, location_par.data(), num_data);
-				// Calculate right hand side for mode update
-				CalcZtVGivenIndices(num_data, num_re_, random_effects_indices_of_data, second_deriv_neg_ll_, diag_sqrt_ZtWZ, true);
-				rhs = (diag_sqrt_ZtWZ.array() * mode_.array()).matrix();//rhs = ZtWZ * mode_ + Zt * first_deriv_ll_ for updating mode
-				CalcZtVGivenIndices(num_data, num_re_, random_effects_indices_of_data, first_deriv_ll_, rhs, false);
-				// Calculate Cholesky factor of matrix B = Id + ZtWZsqrt * Sigma * ZtWZsqrt
-				diag_sqrt_ZtWZ.array() = diag_sqrt_ZtWZ.array().sqrt();
-				Id_plus_ZtWZsqrt_Sigma_ZtWZsqrt.setIdentity();
-				Id_plus_ZtWZsqrt_Sigma_ZtWZsqrt += diag_sqrt_ZtWZ.asDiagonal() * (*Sigma) * diag_sqrt_ZtWZ.asDiagonal();
-				CalcChol<T_mat>(chol_fact_Id_plus_Wsqrt_Sigma_Wsqrt_, Id_plus_ZtWZsqrt_Sigma_ZtWZsqrt);//this is the bottleneck (for large data and sparse matrices)
-				// Update mode and a_vec_
-				v_aux = (*Sigma) * rhs;
-				v_aux.array() *= diag_sqrt_ZtWZ.array();
-				a_vec_ = -chol_fact_Id_plus_Wsqrt_Sigma_Wsqrt_.solve(v_aux);
-				a_vec_.array() *= diag_sqrt_ZtWZ.array();
-				a_vec_.array() += rhs.array();
-				mode_ = (*Sigma) * a_vec_;
-				// Update location parameter of log-likelihood for calculation of approx. marginal log-likelihood (objective function)
-				if (fixed_effects == nullptr) {
-#pragma omp parallel for schedule(static)
-					for (data_size_t i = 0; i < num_data; ++i) {
-						location_par[i] = mode_[random_effects_indices_of_data[i]];
-					}
-				}
-				else {
-#pragma omp parallel for schedule(static)
-					for (data_size_t i = 0; i < num_data; ++i) {
-						location_par[i] = mode_[random_effects_indices_of_data[i]] + fixed_effects[i];
-					}
-				}
-				// Calculate new objective function
-				approx_marginal_ll_new = -0.5 * (a_vec_.dot(mode_)) + LogLikelihood(y_data, y_data_int, location_par.data(), num_data);
-				if (std::isnan(approx_marginal_ll_new) || std::isinf(approx_marginal_ll_new)) {
-					has_NA_or_Inf = true;
-					Log::REDebug(NA_OR_INF_WARNING_);
-					break;
-				}
-				// Check convergence
-				if (it == 0) {
-					if (std::abs(approx_marginal_ll_new - approx_marginal_ll) < DELTA_REL_CONV_ * std::abs(approx_marginal_ll)) { // allow for decreases in first iteration
-						terminate_optim = true;
-					}
-				}
-				else {
-					if ((approx_marginal_ll_new - approx_marginal_ll) < DELTA_REL_CONV_ * std::abs(approx_marginal_ll)) {
-						terminate_optim = true;
-					}
-				}
-				if (terminate_optim) {
-					if (approx_marginal_ll_new < approx_marginal_ll) {
-						Log::REDebug(NO_INCREASE_IN_MLL_WARNING_);
-					}
-					approx_marginal_ll = approx_marginal_ll_new;
-					break;
-				}
-				else {
-					approx_marginal_ll = approx_marginal_ll_new;
-				}
-			}//end loop for finding mode
-			if (it == MAXIT_MODE_NEWTON_) {
-				Log::REDebug(NO_CONVERGENCE_WARNING_);
-			}
-			if (has_NA_or_Inf) {
-				approx_marginal_ll = approx_marginal_ll_new;
-				na_or_inf_during_last_call_to_find_mode_ = true;
-			}
-			else {
-				CalcFirstDerivLogLik(y_data, y_data_int, location_par.data(), num_data);//first derivative is not used here anymore but since it is reused in gradient calculation and in prediction, we calculate it once more
-				CalcSecondDerivNegLogLik(y_data, y_data_int, location_par.data(), num_data);
-				CalcZtVGivenIndices(num_data, num_re_, random_effects_indices_of_data, second_deriv_neg_ll_, diag_sqrt_ZtWZ, true);
-				diag_sqrt_ZtWZ.array() = diag_sqrt_ZtWZ.array().sqrt();
-				Id_plus_ZtWZsqrt_Sigma_ZtWZsqrt.setIdentity();
-				Id_plus_ZtWZsqrt_Sigma_ZtWZsqrt += diag_sqrt_ZtWZ.asDiagonal() * (*Sigma) * diag_sqrt_ZtWZ.asDiagonal();
-				CalcChol<T_mat>(chol_fact_Id_plus_Wsqrt_Sigma_Wsqrt_, Id_plus_ZtWZsqrt_Sigma_ZtWZsqrt);
-				approx_marginal_ll -= ((T_mat)chol_fact_Id_plus_Wsqrt_Sigma_Wsqrt_.matrixL()).diagonal().array().log().sum();
-				mode_has_been_calculated_ = true;
-				na_or_inf_during_last_call_to_find_mode_ = false;
-			}
-		}//end FindModePostRandEffCalcMLLOnlyOneGPCalculationsOnREScale
-
-		/*!
-		* \brief Find the mode of the posterior of the latent random effects using Newton's method and calculate the approximative marginal log-likelihood.
-		*		Calculations are done by directly factorizing ("inverting) (Sigma^-1 + Zt*W*Z).
-		*		NOTE: IT IS ASSUMED THAT SIGMA IS A DIAGONAL MATRIX
-		*		This version is used for the Laplace approximation when there are only grouped random effects.
-		* \param y_data Response variable data if response variable is continuous
-		* \param y_data_int Response variable data if response variable is integer-valued
-		* \param fixed_effects Fixed effects component of location parameter
-		* \param num_data Number of data points
-		* \param SigmaI Inverse covariance matrix of latent random effect. Currently, this needs to be a diagonal matrix
-		* \param Zt Transpose Z^T of random effect design matrix that relates latent random effects to observations/likelihoods
-		* \param[out] approx_marginal_ll Approximate marginal log-likelihood evaluated at the mode
-		*/
-		void FindModePostRandEffCalcMLLGroupedRE(const double* y_data,
-			const int* y_data_int,
-			const double* fixed_effects,
-			const data_size_t num_data,
-			const sp_mat_t& SigmaI,
-			const sp_mat_t& Zt,
-			double& approx_marginal_ll) {
-			// Initialize variables
-			if (!mode_initialized_) {
-				InitializeModeAvec();
-			}
-			else {
-				mode_previous_value_ = mode_;
-				na_or_inf_during_second_last_call_to_find_mode_ = na_or_inf_during_last_call_to_find_mode_;
-			}
-			sp_mat_t Z = Zt.transpose();
-			vec_t location_par = Z * mode_;//location parameter = mode of random effects + fixed effects
-			if (fixed_effects != nullptr) {
-#pragma omp parallel for schedule(static)
-				for (data_size_t i = 0; i < num_data; ++i) {
-					location_par[i] += fixed_effects[i];
-				}
-			}
-			// Initialize objective function (LA approx. marginal likelihood) for use as convergence criterion
-			approx_marginal_ll = -0.5 * (mode_.dot(SigmaI * mode_)) + LogLikelihood(y_data, y_data_int, location_par.data(), num_data);
-			double approx_marginal_ll_new = approx_marginal_ll;
-			sp_mat_t SigmaI_plus_ZtWZ;
-			vec_t rhs;
-			// Start finding mode 
-			int it;
-			bool terminate_optim = false;
-			bool has_NA_or_Inf = false;
-			for (it = 0; it < MAXIT_MODE_NEWTON_; ++it) {
-				// Calculate first and second derivative of log-likelihood
-				CalcFirstDerivLogLik(y_data, y_data_int, location_par.data(), num_data);
-				CalcSecondDerivNegLogLik(y_data, y_data_int, location_par.data(), num_data);
-				// Calculate Cholesky factor and update mode
-				rhs = Zt * first_deriv_ll_ - SigmaI * mode_;//right hand side for updating mode
-				SigmaI_plus_ZtWZ = SigmaI + Zt * second_deriv_neg_ll_.asDiagonal() * Z;
-				SigmaI_plus_ZtWZ.makeCompressed();
-				if (!chol_fact_pattern_analyzed_) {
-					chol_fact_SigmaI_plus_ZtWZ_grouped_.analyzePattern(SigmaI_plus_ZtWZ);
-					chol_fact_pattern_analyzed_ = true;
-				}
-				chol_fact_SigmaI_plus_ZtWZ_grouped_.factorize(SigmaI_plus_ZtWZ);
-				mode_ += chol_fact_SigmaI_plus_ZtWZ_grouped_.solve(rhs);
-				// Update location parameter of log-likelihood for calculation of approx. marginal log-likelihood (objective function)
-				location_par = Z * mode_;
-				if (fixed_effects != nullptr) {
-#pragma omp parallel for schedule(static)
-					for (data_size_t i = 0; i < num_data; ++i) {
-						location_par[i] += fixed_effects[i];
-					}
-				}
-				// Calculate new objective function
-				approx_marginal_ll_new = -0.5 * (mode_.dot(SigmaI * mode_)) + LogLikelihood(y_data, y_data_int, location_par.data(), num_data);
-				if (std::isnan(approx_marginal_ll_new) || std::isinf(approx_marginal_ll_new)) {
-					has_NA_or_Inf = true;
-					Log::REDebug(NA_OR_INF_WARNING_);
-					break;
-				}
-				// Check convergence
-				if (it == 0) {
-					if (std::abs(approx_marginal_ll_new - approx_marginal_ll) < DELTA_REL_CONV_ * std::abs(approx_marginal_ll)) { // allow for decreases in first iteration
-						terminate_optim = true;
-					}
-				}
-				else {
-					if ((approx_marginal_ll_new - approx_marginal_ll) < DELTA_REL_CONV_ * std::abs(approx_marginal_ll)) {
-						terminate_optim = true;
-					}
-				}
-				if (terminate_optim) {
-					if (approx_marginal_ll_new < approx_marginal_ll) {
-						Log::REDebug(NO_INCREASE_IN_MLL_WARNING_);
-					}
-					approx_marginal_ll = approx_marginal_ll_new;
-					break;
-				}
-				else {
-					approx_marginal_ll = approx_marginal_ll_new;
-				}
-			}//end mode finding algorithm
-			if (it == MAXIT_MODE_NEWTON_) {
-				Log::REDebug(NO_CONVERGENCE_WARNING_);
-			}
-			if (has_NA_or_Inf) {
-				approx_marginal_ll = approx_marginal_ll_new;
-				na_or_inf_during_last_call_to_find_mode_ = true;
-			}
-			else {
-				CalcFirstDerivLogLik(y_data, y_data_int, location_par.data(), num_data);//first derivative is not used here anymore but since it is reused in gradient calculation and in prediction, we calculate it once more
-				CalcSecondDerivNegLogLik(y_data, y_data_int, location_par.data(), num_data);
-				SigmaI_plus_ZtWZ = SigmaI + Zt * second_deriv_neg_ll_.asDiagonal() * Z;
-				SigmaI_plus_ZtWZ.makeCompressed();
-				chol_fact_SigmaI_plus_ZtWZ_grouped_.factorize(SigmaI_plus_ZtWZ);
-				approx_marginal_ll += -((sp_mat_t)chol_fact_SigmaI_plus_ZtWZ_grouped_.matrixL()).diagonal().array().log().sum() + 0.5 * SigmaI.diagonal().array().log().sum();
-				mode_has_been_calculated_ = true;
-				na_or_inf_during_last_call_to_find_mode_ = false;
-			}
-		}//end FindModePostRandEffCalcMLLGroupedRE
-
-		/*!
-		* \brief Find the mode of the posterior of the latent random effects using Newton's method and calculate the approximative marginal log-likelihood.
-		*		Calculations are done by directly factorizing ("inverting) (Sigma^-1 + Zt*W*Z).
-		*		This version is used for the Laplace approximation when there are only grouped random effects with only one grouping variable.
-		* \param y_data Response variable data if response variable is continuous
-		* \param y_data_int Response variable data if response variable is integer-valued
-		* \param fixed_effects Fixed effects component of location parameter
-		* \param num_data Number of data points
-		* \param sigma2 Variance of random effects
-		* \param random_effects_indices_of_data Indices that indicate to which random effect every data point is related
-		* \param[out] approx_marginal_ll Approximate marginal log-likelihood evaluated at the mode
-		*/
-		void FindModePostRandEffCalcMLLOnlyOneGroupedRECalculationsOnREScale(const double* y_data,
-			const int* y_data_int,
-			const double* fixed_effects,
-			const data_size_t num_data,
-			const double sigma2,
-			const data_size_t* const random_effects_indices_of_data,
-			double& approx_marginal_ll) {
-			// Initialize variables
-			if (!mode_initialized_) {
-				InitializeModeAvec();
-			}
-			else {
-				mode_previous_value_ = mode_;
-				na_or_inf_during_second_last_call_to_find_mode_ = na_or_inf_during_last_call_to_find_mode_;
-			}
-			vec_t location_par(num_data);//location parameter = mode of random effects + fixed effects
-			if (fixed_effects == nullptr) {
-#pragma omp parallel for schedule(static)
-				for (data_size_t i = 0; i < num_data; ++i) {
-					location_par[i] = mode_[random_effects_indices_of_data[i]];
-				}
-			}
-			else {
-#pragma omp parallel for schedule(static)
-				for (data_size_t i = 0; i < num_data; ++i) {
-					location_par[i] = mode_[random_effects_indices_of_data[i]] + fixed_effects[i];
-				}
-			}
-			// Initialize objective function (LA approx. marginal likelihood) for use as convergence criterion
-			approx_marginal_ll = -0.5 / sigma2 * (mode_.dot(mode_)) + LogLikelihood(y_data, y_data_int, location_par.data(), num_data);
-			double approx_marginal_ll_new = approx_marginal_ll;
-			vec_t rhs;
-			diag_SigmaI_plus_ZtWZ_ = vec_t(num_re_);
-			// Start finding mode 
-			int it;
-			bool terminate_optim = false;
-			bool has_NA_or_Inf = false;
-			for (it = 0; it < MAXIT_MODE_NEWTON_; ++it) {
-				// Calculate first and second derivative of log-likelihood
-				CalcFirstDerivLogLik(y_data, y_data_int, location_par.data(), num_data);
-				CalcSecondDerivNegLogLik(y_data, y_data_int, location_par.data(), num_data);
-				// Calculate rhs for mode update
-				rhs = - mode_ / sigma2;//right hand side for updating mode
-				CalcZtVGivenIndices(num_data, num_re_, random_effects_indices_of_data, first_deriv_ll_, rhs, false);
-				// Update mode
-				CalcZtVGivenIndices(num_data, num_re_, random_effects_indices_of_data, second_deriv_neg_ll_, diag_SigmaI_plus_ZtWZ_, true);
-				diag_SigmaI_plus_ZtWZ_.array() += 1. / sigma2;
-				mode_ += (rhs.array() / diag_SigmaI_plus_ZtWZ_.array()).matrix();
-				// Update location parameter of log-likelihood for calculation of approx. marginal log-likelihood (objective function)
-				if (fixed_effects == nullptr) {
-#pragma omp parallel for schedule(static)
-					for (data_size_t i = 0; i < num_data; ++i) {
-						location_par[i] = mode_[random_effects_indices_of_data[i]];
-					}
-				}
-				else {
-#pragma omp parallel for schedule(static)
-					for (data_size_t i = 0; i < num_data; ++i) {
-						location_par[i] = mode_[random_effects_indices_of_data[i]] + fixed_effects[i];
-					}
-				}
-				// Calculate new objective function
-				approx_marginal_ll_new = -0.5 / sigma2 * (mode_.dot(mode_)) + LogLikelihood(y_data, y_data_int, location_par.data(), num_data);
-				if (std::isnan(approx_marginal_ll_new) || std::isinf(approx_marginal_ll_new)) {
-					has_NA_or_Inf = true;
-					Log::REDebug(NA_OR_INF_WARNING_);
-					break;
-				}
-				// Check convergence
-				if (it == 0) {
-					if (std::abs(approx_marginal_ll_new - approx_marginal_ll) < DELTA_REL_CONV_ * std::abs(approx_marginal_ll)) { // allow for decreases in first iteration
-						terminate_optim = true;
-					}
-				}
-				else {
-					if ((approx_marginal_ll_new - approx_marginal_ll) < DELTA_REL_CONV_ * std::abs(approx_marginal_ll)) {
-						terminate_optim = true;
-					}
-				}
-				if (terminate_optim) {
-					if (approx_marginal_ll_new < approx_marginal_ll) {
-						Log::REDebug(NO_INCREASE_IN_MLL_WARNING_);
-					}
-					approx_marginal_ll = approx_marginal_ll_new;
-					break;
-				}
-				else {
-					approx_marginal_ll = approx_marginal_ll_new;
-				}
-			}//end mode finding algorithm
-			if (it == MAXIT_MODE_NEWTON_) {
-				Log::REDebug(NO_CONVERGENCE_WARNING_);
-			}
-			if (has_NA_or_Inf) {
-				approx_marginal_ll = approx_marginal_ll_new;
-				na_or_inf_during_last_call_to_find_mode_ = true;
-			}
-			else {
-				CalcFirstDerivLogLik(y_data, y_data_int, location_par.data(), num_data);//first derivative is not used here anymore but since it is reused in gradient calculation and in prediction, we calculate it once more
-				CalcSecondDerivNegLogLik(y_data, y_data_int, location_par.data(), num_data);
-				CalcZtVGivenIndices(num_data, num_re_, random_effects_indices_of_data, second_deriv_neg_ll_, diag_SigmaI_plus_ZtWZ_, true);
-				diag_SigmaI_plus_ZtWZ_.array() += 1. / sigma2;
-				approx_marginal_ll -= 0.5 * diag_SigmaI_plus_ZtWZ_.array().log().sum() + 0.5 * num_re_ * std::log(sigma2);
-				mode_has_been_calculated_ = true;
-				na_or_inf_during_last_call_to_find_mode_ = false;
-			}
-		}//end FindModePostRandEffCalcMLLOnlyOneGroupedRECalculationsOnREScale
-
-		/*!
-		* \brief Find the mode of the posterior of the latent random effects using Newton's method and calculate the approximative marginal log-likelihood.
-		*		Calculations are done by factorizing ("inverting) (Sigma^-1 + W) where it is assumed that an approximate Cholesky factor
-		*		of Sigma^-1 has previously been calculated using a Vecchia approximation.
-		*		This version is used for the Laplace approximation when there are only GP random effects and the Vecchia approximation is used.
-		*		Caveat: Sigma^-1 + W can be not very sparse
-		* \param y_data Response variable data if response variable is continuous
-		* \param y_data_int Response variable data if response variable is integer-valued
-		* \param fixed_effects Fixed effects component of location parameter
-		* \param num_data Number of data points
-		* \param B Matrix B in Vecchia approximation Sigma^-1 = B^T D^-1 B ("=" Cholesky factor)
-		* \param D_inv Diagonal matrix D^-1 in Vecchia approximation Sigma^-1 = B^T D^-1 B
-		* \param[out] approx_marginal_ll Approximate marginal log-likelihood evaluated at the mode
-		*/
-		void FindModePostRandEffCalcMLLVecchia(const double* y_data,
-			const int* y_data_int,
-			const double* fixed_effects,
-			const data_size_t num_data,
-			const sp_mat_t& B,
-			const sp_mat_t& D_inv,
-			double& approx_marginal_ll) {
-			// Initialize variables
-			if (!mode_initialized_) {
-				InitializeModeAvec();
-			}
-			else {
-				mode_previous_value_ = mode_;
-				na_or_inf_during_second_last_call_to_find_mode_ = na_or_inf_during_last_call_to_find_mode_;
-			}
-			bool no_fixed_effects = (fixed_effects == nullptr);
-			sp_mat_t SigmaI = B.transpose() * D_inv * B;
-			vec_t location_par;//location parameter = mode of random effects + fixed effects
-			sp_mat_t SigmaI_plus_W;
-			vec_t rhs, B_mode;
-			// Initialize objective function (LA approx. marginal likelihood) for use as convergence criterion
-			B_mode = B * mode_;
-			if (no_fixed_effects) {
-				approx_marginal_ll = -0.5 * (B_mode.dot(D_inv * B_mode)) + LogLikelihood(y_data, y_data_int, mode_.data(), num_data);
-			}
-			else {
-				location_par = vec_t(num_data);
-#pragma omp parallel for schedule(static)
-				for (data_size_t i = 0; i < num_data; ++i) {
-					location_par[i] = mode_[i] + fixed_effects[i];
-				}
-				approx_marginal_ll = -0.5 * (B_mode.dot(D_inv * B_mode)) + LogLikelihood(y_data, y_data_int, location_par.data(), num_data);
-			}
-			double approx_marginal_ll_new = approx_marginal_ll;
-			// Start finding mode 
-			int it;
-			bool terminate_optim = false;
-			bool has_NA_or_Inf = false;
-			for (it = 0; it < MAXIT_MODE_NEWTON_; ++it) {
-				// Calculate first and second derivative of log-likelihood
-				if (no_fixed_effects) {
-					CalcFirstDerivLogLik(y_data, y_data_int, mode_.data(), num_data);
-					CalcSecondDerivNegLogLik(y_data, y_data_int, mode_.data(), num_data);
-				}
-				else {
-					CalcFirstDerivLogLik(y_data, y_data_int, location_par.data(), num_data);
-					CalcSecondDerivNegLogLik(y_data, y_data_int, location_par.data(), num_data);
-				}
-				// Calculate Cholesky factor and update mode
-				rhs.array() = second_deriv_neg_ll_.array() * mode_.array() + first_deriv_ll_.array();//right hand side for updating mode
-				SigmaI_plus_W = SigmaI;
-				SigmaI_plus_W.diagonal().array() += second_deriv_neg_ll_.array();
-				SigmaI_plus_W.makeCompressed();
-				//Calculation of the Cholesky factor is the bottleneck
-				if (!chol_fact_pattern_analyzed_) {
-					chol_fact_SigmaI_plus_ZtWZ_vecchia_.analyzePattern(SigmaI_plus_W);
-					chol_fact_pattern_analyzed_ = true;
-				}
-				chol_fact_SigmaI_plus_ZtWZ_vecchia_.factorize(SigmaI_plus_W);//This is the bottleneck for large data
-				//Log::REInfo("SigmaI_plus_W: number non zeros = %d", (int)SigmaI_plus_W.nonZeros());//only for debugging
-				//Log::REInfo("chol_fact_SigmaI_plus_ZtWZ: Number non zeros = %d", (int)((sp_mat_t)chol_fact_SigmaI_plus_ZtWZ_vecchia_.matrixL()).nonZeros());//only for debugging
-				mode_ = chol_fact_SigmaI_plus_ZtWZ_vecchia_.solve(rhs);
-				// Calculate new objective function
-				B_mode = B * mode_;
-				if (no_fixed_effects) {
-					approx_marginal_ll_new = -0.5 * (B_mode.dot(D_inv * B_mode)) + LogLikelihood(y_data, y_data_int, mode_.data(), num_data);
-				}
-				else {
-					// Update location parameter of log-likelihood for calculation of approx. marginal log-likelihood (objective function)
-#pragma omp parallel for schedule(static)
-					for (data_size_t i = 0; i < num_data; ++i) {
-						location_par[i] = mode_[i] + fixed_effects[i];
-					}
-					approx_marginal_ll_new = -0.5 * (B_mode.dot(D_inv * B_mode)) + LogLikelihood(y_data, y_data_int, location_par.data(), num_data);
-				}
-				if (std::isnan(approx_marginal_ll_new) || std::isinf(approx_marginal_ll_new)) {
-					has_NA_or_Inf = true;
-					Log::REDebug(NA_OR_INF_WARNING_);
-					break;
-				}
-				// Check convergence
-				if (it == 0) {
-					if (std::abs(approx_marginal_ll_new - approx_marginal_ll) < DELTA_REL_CONV_ * std::abs(approx_marginal_ll)) { // allow for decreases in first iteration
-						terminate_optim = true;
-					}
-				}
-				else {
-					if ((approx_marginal_ll_new - approx_marginal_ll) < DELTA_REL_CONV_ * std::abs(approx_marginal_ll)) {
-						terminate_optim = true;
-					}
-				}
-				if (terminate_optim) {
-					if (approx_marginal_ll_new < approx_marginal_ll) {
-						Log::REDebug(NO_INCREASE_IN_MLL_WARNING_);
-					}
-					approx_marginal_ll = approx_marginal_ll_new;
-					break;
-				}
-				else {
-					approx_marginal_ll = approx_marginal_ll_new;
-				}
-			} // end loop for mode finding
-			if (it == MAXIT_MODE_NEWTON_) {
-				Log::REDebug(NO_CONVERGENCE_WARNING_);
-			}
-			if (has_NA_or_Inf) {
-				approx_marginal_ll = approx_marginal_ll_new;
-				na_or_inf_during_last_call_to_find_mode_ = true;
-			}
-			else {
-				if (no_fixed_effects) {
-					CalcFirstDerivLogLik(y_data, y_data_int, mode_.data(), num_data);//first derivative is not used here anymore but since it is reused in gradient calculation and in prediction, we calculate it once more
-					CalcSecondDerivNegLogLik(y_data, y_data_int, mode_.data(), num_data);
-				}
-				else {
-					CalcFirstDerivLogLik(y_data, y_data_int, location_par.data(), num_data);//first derivative is not used here anymore but since it is reused in gradient calculation and in prediction, we calculate it once more
-					CalcSecondDerivNegLogLik(y_data, y_data_int, location_par.data(), num_data);
-				}
-				SigmaI_plus_W = SigmaI;
-				SigmaI_plus_W.diagonal().array() += second_deriv_neg_ll_.array();
-				SigmaI_plus_W.makeCompressed();
-				chol_fact_SigmaI_plus_ZtWZ_vecchia_.factorize(SigmaI_plus_W);
-				approx_marginal_ll += -((sp_mat_t)chol_fact_SigmaI_plus_ZtWZ_vecchia_.matrixL()).diagonal().array().log().sum() + 0.5 * D_inv.diagonal().array().log().sum();
-				mode_has_been_calculated_ = true;
-				na_or_inf_during_last_call_to_find_mode_ = false;
-			}
-		}//end FindModePostRandEffCalcMLLVecchia
-
-		/*!
-		* \brief Calculate the gradient of the negative Laplace-approximated marginal log-likelihood wrt covariance parameters, 
-		*		fixed effects (e.g., for linear regression coefficients), and additional likelihood-related parameters.
-		*		Calculations are done using a numerically stable variant based on factorizing ("inverting") B = (Id + Wsqrt * Z*Sigma*Zt * Wsqrt).
-		*		In the notation of the paper: "Sigma = Z*Sigma*Z^T" and "Z = Id".
-		*		This version is used for the Laplace approximation when dense matrices are used (e.g. GP models).
-		* \param y_data Response variable data if response variable is continuous
-		* \param y_data_int Response variable data if response variable is integer-valued
-		* \param fixed_effects Fixed effects component of location parameter
-		* \param num_data Number of data points
-		* \param ZSigmaZt Covariance matrix of latent random effect
-		* \param re_comps_cluster_i Vector with different random effects components. We pass the component pointers to save memory in order to avoid passing a large collection of gardient covariance matrices in memory//TODO: better way than passing this? (relying on all gradients in a vector can lead to large memory consumption)
-		* \param calc_cov_grad If true, the gradient wrt the covariance parameters is calculated
-		* \param calc_F_grad If true, the gradient wrt the fixed effects mean function F is calculated
-		* \param calc_aux_par_grad If true, the gradient wrt additional likelihood parameters is calculated
-		* \param[out] cov_grad Gradient of approximate marginal log-likelihood wrt covariance parameters (needs to be preallocated of size num_cov_par)
-		* \param[out] fixed_effect_grad Gradient of approximate marginal log-likelihood wrt fixed effects F (note: this is passed as a Eigen vector in order to avoid the need for copying)
-		* \param[out] aux_par_grad Gradient wrt additional likelihood parameters
-		* \param calc_mode If true, the mode of the random effects posterior is calculated otherwise the values in mode and a_vec_ are used (default=false)
-		*/
-		void CalcGradNegMargLikelihoodLaplaceApproxStable(const double* y_data,
-			const int* y_data_int,
-			const double* fixed_effects,
-			const data_size_t num_data,
-			const std::shared_ptr<T_mat> ZSigmaZt,
-			const std::vector<std::shared_ptr<RECompBase<T_mat>>>& re_comps_cluster_i,
-			bool calc_cov_grad,
-			bool calc_F_grad,
-			bool calc_aux_par_grad,
-			double* cov_grad,
-			vec_t& fixed_effect_grad,
-			double* aux_par_grad,
-			bool calc_mode) {
-			if (calc_mode) {// Calculate mode and Cholesky factor of B = (Id + Wsqrt * ZSigmaZt * Wsqrt) at mode
-				double mll;//approximate marginal likelihood. This is a by-product that is not used here.
-				FindModePostRandEffCalcMLLStable(y_data, y_data_int, fixed_effects, num_data, ZSigmaZt, mll);
-			}
-			if (na_or_inf_during_last_call_to_find_mode_) {
-				Log::REFatal(NA_OR_INF_ERROR_);
-			}
-			CHECK(mode_has_been_calculated_);
-			// Initialize variables
-			bool no_fixed_effects = (fixed_effects == nullptr);
-			vec_t location_par;//location parameter = mode of random effects + fixed effects
-			double* location_par_ptr;
-			T_mat L_inv_Wsqrt(num_data, num_data);//diagonal matrix with square root of negative second derivatives on the diagonal (sqrt of negative Hessian of log-likelihood)
-			L_inv_Wsqrt.setIdentity();
-			L_inv_Wsqrt.diagonal().array() = second_deriv_neg_ll_.array().sqrt();
-			vec_t third_deriv(num_data);//vector of third derivatives of log-likelihood
-			if (no_fixed_effects) {
-				location_par_ptr = mode_.data();
-			}
-			else {
-				location_par = vec_t(num_data);
-#pragma omp parallel for schedule(static)
-				for (data_size_t i = 0; i < num_data; ++i) {
-					location_par[i] = mode_[i] + fixed_effects[i];
-				}
-				location_par_ptr = location_par.data();
-			}
-			CalcThirdDerivLogLik(y_data, y_data_int, location_par_ptr, num_data, third_deriv.data());
-			TriangularSolveGivenCholesky<T_chol, T_mat, T_mat, T_mat>(chol_fact_Id_plus_Wsqrt_Sigma_Wsqrt_, L_inv_Wsqrt, L_inv_Wsqrt, false);//L_inv_Wsqrt = L\Wsqrt
-			T_mat L_inv_Wsqrt_ZSigmaZt = L_inv_Wsqrt * (*ZSigmaZt);
-			// Calculate gradient of approx. marginal log-likelihood wrt the mode
-			//		Note: use (i) (Sigma^-1 + W)^-1 = Sigma - Sigma*(W^-1 + Sigma)^-1*Sigma = ZSigmaZt - L_inv_Wsqrt_ZSigmaZt^T*L_inv_Wsqrt_ZSigmaZt and (ii) "Z=Id"N
-			T_mat L_inv_Wsqrt_ZSigmaZt_sqr = L_inv_Wsqrt_ZSigmaZt.cwiseProduct(L_inv_Wsqrt_ZSigmaZt);
-			vec_t ZSigmaZtI_plus_W_inv_diag = (*ZSigmaZt).diagonal() - L_inv_Wsqrt_ZSigmaZt_sqr.transpose() * vec_t::Ones(L_inv_Wsqrt_ZSigmaZt_sqr.rows());// diagonal of (ZSigmaZt^-1 + W) ^ -1
-			vec_t d_mll_d_mode = (-0.5 * ZSigmaZtI_plus_W_inv_diag.array() * third_deriv.array()).matrix();// gradient of approx. marginal likelihood wrt the mode and thus also F here
-			// calculate gradient wrt covariance parameters
-			if (calc_cov_grad) {
-				T_mat WI_plus_Sigma_inv;//WI_plus_Sigma_inv = Wsqrt * L^T\(L\Wsqrt) = (W^-1 + Sigma)^-1
-				vec_t d_mode_d_par, SigmaDeriv_first_deriv_ll;
-				int par_count = 0;
-				double explicit_derivative;
-				for (int j = 0; j < (int)re_comps_cluster_i.size(); ++j) {
-					for (int ipar = 0; ipar < re_comps_cluster_i[j]->NumCovPar(); ++ipar) {
-						std::shared_ptr<T_mat> SigmaDeriv = re_comps_cluster_i[j]->GetZSigmaZtGrad(ipar, true, 1.);
-						if (ipar == 0) {
-							WI_plus_Sigma_inv = *SigmaDeriv;
-							CalcLtLGivenSparsityPattern<T_mat>(L_inv_Wsqrt, WI_plus_Sigma_inv, true);
-							//TODO (low-prio): calculate WI_plus_Sigma_inv only once for all relevant non-zero entries as in Gaussian case (see 'CalcPsiInv')
-							//					This is only relevant for multiple random effects and/or GPs
-						}
-						// calculate explicit derivative of approx. mariginal log-likelihood
-						explicit_derivative = -0.5 * (double)(a_vec_.transpose() * (*SigmaDeriv) * a_vec_) + 0.5 * (WI_plus_Sigma_inv.cwiseProduct(*SigmaDeriv)).sum();
-						// calculate implicit derivative (through mode) of approx. mariginal log-likelihood
-						SigmaDeriv_first_deriv_ll = (*SigmaDeriv) * first_deriv_ll_;//auxiliary variable for caclulating d_mode_d_par
-						d_mode_d_par = SigmaDeriv_first_deriv_ll;//derivative of mode wrt to a covariance parameter
-						d_mode_d_par -= ((*ZSigmaZt) * (L_inv_Wsqrt.transpose() * (L_inv_Wsqrt * SigmaDeriv_first_deriv_ll)));
-						cov_grad[par_count] = explicit_derivative + d_mll_d_mode.dot(d_mode_d_par);
-						par_count++;
-					}
-				}
-			}//end calc_cov_grad
-			// calculate gradient wrt fixed effects
-			vec_t ZSigmaZtI_plus_W_inv_d_mll_d_mode;// for implicit derivative
-			if (calc_F_grad || calc_aux_par_grad) {
-				vec_t L_inv_Wsqrt_ZSigmaZt_d_mll_d_mode = L_inv_Wsqrt_ZSigmaZt * d_mll_d_mode;// for implicit derivative
-				ZSigmaZtI_plus_W_inv_d_mll_d_mode = (*ZSigmaZt) * d_mll_d_mode - L_inv_Wsqrt_ZSigmaZt.transpose() * L_inv_Wsqrt_ZSigmaZt_d_mll_d_mode;
-			}
-			if (calc_F_grad) {
-				vec_t d_mll_d_F_implicit = (ZSigmaZtI_plus_W_inv_d_mll_d_mode.array() * second_deriv_neg_ll_.array()).matrix();// implicit derivative
-				fixed_effect_grad = -first_deriv_ll_ + d_mll_d_mode - d_mll_d_F_implicit;
-			}//end calc_F_grad
-			// calculate gradient wrt additional likelihood parameters
-			if (calc_aux_par_grad) {
-				vec_t neg_likelihood_deriv(num_aux_pars_);//derivative of the negative log-likelihood wrt additional parameters of the likelihood
-				vec_t second_deriv(num_data);//second derivative of the log-likelihood with respect to (i) the location parameter and (ii) an additional parameter of the likelihood
-				vec_t neg_third_deriv(num_data);//negative third derivative of the log-likelihood with respect to (i) two times the location parameter and (ii) an additional parameter of the likelihood
-				vec_t d_mode_d_aux_par;
-				CalcGradNegLogLikAuxPars(y_data, location_par_ptr, num_data, neg_likelihood_deriv.data());
-				for (int ind_ap = 0; ind_ap < num_aux_pars_; ++ind_ap) {
-					CalcSecondNegThirdDerivLogLikAuxParsLocPar(y_data, location_par_ptr, num_data, ind_ap, second_deriv.data(), neg_third_deriv.data());
-					double d_detmll_d_aux_par = 0., implicit_derivative = 0.;
-#pragma omp parallel for schedule(static) reduction(+:d_detmll_d_aux_par, implicit_derivative)
-					for (data_size_t i = 0; i < num_data; ++i) {
-						d_detmll_d_aux_par += neg_third_deriv[i] * ZSigmaZtI_plus_W_inv_diag[i];
-						implicit_derivative += second_deriv[i] * ZSigmaZtI_plus_W_inv_d_mll_d_mode[i];
-					}
-					aux_par_grad[ind_ap] = neg_likelihood_deriv[ind_ap] + 0.5 * d_detmll_d_aux_par + implicit_derivative;
-				}
-			}//end calc_aux_par_grad
-		}//end CalcGradNegMargLikelihoodLaplaceApproxStable
-
-		/*!
-		* \brief Calculate the gradient of the negative Laplace-approximated marginal log-likelihood wrt covariance parameters, 
-		*		fixed effects (e.g., for linear regression coefficients), and additional likelihood-related parameters.
-		*		Calculations are done on the random effects (b) scale and not the "data scale" (Zb) using
-		*		a numerically stable variant based on factorizing ("inverting") B = (Id + ZtWZsqrt * Sigma * ZtWZsqrt).
-		*		This version is used for the Laplace approximation when there is only one Gaussian process and
-		*		there are a lot of multiple observations at the same location, i.e., the dimenion of the random effects b is much smaller than Zb
-		* \param y_data Response variable data if response variable is continuous
-		* \param y_data_int Response variable data if response variable is integer-valued
-		* \param fixed_effects Fixed effects component of location parameter
-		* \param num_data Number of data points
-		* \param Sigma Covariance matrix of latent random effect
-		* \param random_effects_indices_of_data Indices that indicate to which random effect every data point is related
-		* \param re_comps_cluster_i Vector with different random effects components. We pass the component pointers to save memory in order to avoid passing a large collection of gardient covariance matrices in memory//TODO: better way than passing this? (relying on all gradients in a vector can lead to large memory consumption)
-		* \param calc_cov_grad If true, the gradient wrt the covariance parameters is calculated
-		* \param calc_F_grad If true, the gradient wrt the fixed effects mean function F is calculated
-		* \param calc_aux_par_grad If true, the gradient wrt additional likelihood parameters is calculated
-		* \param[out] cov_grad Gradient of approximate marginal log-likelihood wrt covariance parameters (needs to be preallocated of size num_cov_par)
-		* \param[out] fixed_effect_grad Gradient of approximate marginal log-likelihood wrt fixed effects F (note: this is passed as a Eigen vector in order to avoid the need for copying)
-		* \param[out] aux_par_grad Gradient wrt additional likelihood parameters
-		* \param calc_mode If true, the mode of the random effects posterior is calculated otherwise the values in mode and a_vec_ are used (default=false)
-		*/
-		void CalcGradNegMargLikelihoodLaplaceApproxOnlyOneGPCalculationsOnREScale(const double* y_data,
-			const int* y_data_int,
-			const double* fixed_effects,
-			const data_size_t num_data,
-			const std::shared_ptr<T_mat> Sigma,
-			const data_size_t* const random_effects_indices_of_data,
-			const std::vector<std::shared_ptr<RECompBase<T_mat>>>& re_comps_cluster_i,
-			bool calc_cov_grad,
-			bool calc_F_grad,
-			bool calc_aux_par_grad,
-			double* cov_grad,
-			vec_t& fixed_effect_grad,
-			double* aux_par_grad,
-			bool calc_mode) {
-			CHECK(re_comps_cluster_i.size() == 1);
-			if (calc_mode) {// Calculate mode and Cholesky factor of B = (Id + Wsqrt * ZSigmaZt * Wsqrt) at mode
-				double mll;//approximate marginal likelihood. This is a by-product that is not used here.
-				FindModePostRandEffCalcMLLOnlyOneGPCalculationsOnREScale(y_data, y_data_int, fixed_effects, num_data,
-					Sigma, random_effects_indices_of_data, mll);
-			}
-			if (na_or_inf_during_last_call_to_find_mode_) {
-				Log::REFatal(NA_OR_INF_ERROR_);
-			}
-			CHECK(mode_has_been_calculated_);
-			// Initialize variables
-			vec_t location_par(num_data);//location parameter = mode of random effects + fixed effects
-			if (fixed_effects == nullptr) {
-#pragma omp parallel for schedule(static)
-				for (data_size_t i = 0; i < num_data; ++i) {
-					location_par[i] = mode_[random_effects_indices_of_data[i]];
-				}
-			}
-			else {
-#pragma omp parallel for schedule(static)
-				for (data_size_t i = 0; i < num_data; ++i) {
-					location_par[i] = mode_[random_effects_indices_of_data[i]] + fixed_effects[i];
-				}
-			}
-			// Matrix ZtWZsqrt
-			vec_t diag_ZtWZ;
-			CalcZtVGivenIndices(num_data, num_re_, random_effects_indices_of_data, second_deriv_neg_ll_, diag_ZtWZ, true);
-			T_mat L_inv_ZtWZsqrt(num_re_, num_re_);//diagonal matrix with square root of diagonal of ZtWZ
-			L_inv_ZtWZsqrt.setIdentity();
-			L_inv_ZtWZsqrt.diagonal().array() = diag_ZtWZ.array().sqrt();
-			vec_t third_deriv(num_data);//vector of third derivatives of log-likelihood
-			CalcThirdDerivLogLik(y_data, y_data_int, location_par.data(), num_data, third_deriv.data());
-			vec_t diag_ZtThirdDerivZ;
-			CalcZtVGivenIndices(num_data, num_re_, random_effects_indices_of_data, third_deriv, diag_ZtThirdDerivZ, true);
-			TriangularSolveGivenCholesky<T_chol, T_mat, T_mat, T_mat>(chol_fact_Id_plus_Wsqrt_Sigma_Wsqrt_, L_inv_ZtWZsqrt, L_inv_ZtWZsqrt, false);//L_inv_ZtWZsqrt = L\ZtWZsqrt
-			T_mat L_inv_ZtWZsqrt_Sigma = L_inv_ZtWZsqrt * (*Sigma);
-			//Log::REInfo("CalcGradNegMargLikelihoodLaplaceApproxOnlyOneGPCalculationsOnREScale: L_inv_ZtWZsqrt: number non zeros = %d", GetNumberNonZeros<T_mat>(L_inv_ZtWZsqrt));//Only for debugging
-			//Log::REInfo("CalcGradNegMargLikelihoodLaplaceApproxOnlyOneGPCalculationsOnREScale: L_inv_ZtWZsqrt_Sigma: number non zeros = %d", GetNumberNonZeros<T_mat>(L_inv_ZtWZsqrt_Sigma));//Only for debugging
-			// Calculate gradient of approx. marginal log-likelihood wrt the mode
-			//		Note: use (i) (Sigma^-1 + W)^-1 = Sigma - Sigma*(W^-1 + Sigma)^-1*Sigma = ZSigmaZt - L_inv_ZtWZsqrt_Sigma^T*L_inv_ZtWZsqrt_Sigma
-			T_mat L_inv_ZtWZsqrt_Sigma_sqr = L_inv_ZtWZsqrt_Sigma.cwiseProduct(L_inv_ZtWZsqrt_Sigma);
-			vec_t SigmaI_plus_ZtWZ_inv_diag = (*Sigma).diagonal() - L_inv_ZtWZsqrt_Sigma_sqr.transpose() * vec_t::Ones(L_inv_ZtWZsqrt_Sigma_sqr.rows());// diagonal of (Sigma^-1 + ZtWZ) ^ -1
-			vec_t d_mll_d_mode = (-0.5 * SigmaI_plus_ZtWZ_inv_diag.array() * diag_ZtThirdDerivZ.array()).matrix();// gradient of approx. marginal likelihood wrt the mode
-			// calculate gradient wrt covariance parameters
-			if (calc_cov_grad) {
-				vec_t ZtFirstDeriv;
-				CalcZtVGivenIndices(num_data, num_re_, random_effects_indices_of_data, first_deriv_ll_, ZtFirstDeriv, true);
-				T_mat ZtWZI_Sigma_inv;//ZtWZI_Sigma_inv = ZtWZsqrt * L^T\(L\ZtWZsqrt) = ((ZtWZ)^-1 + Sigma)^-1
-				vec_t d_mode_d_par, SigmaDeriv_ZtFirstDeriv;
-				int par_count = 0;
-				double explicit_derivative;
-				for (int j = 0; j < (int)re_comps_cluster_i.size(); ++j) {
-					for (int ipar = 0; ipar < re_comps_cluster_i[j]->NumCovPar(); ++ipar) {
-						std::shared_ptr<T_mat> SigmaDeriv = re_comps_cluster_i[j]->GetZSigmaZtGrad(ipar, true, 1.);
-						if (ipar == 0) {
-							ZtWZI_Sigma_inv = *SigmaDeriv;
-							CalcLtLGivenSparsityPattern<T_mat>(L_inv_ZtWZsqrt, ZtWZI_Sigma_inv, true);
-							//TODO (low-prio): calculate ZtWZI_Sigma_inv only once for all relevant non-zero entries as in Gaussian case (see 'CalcPsiInv')
-							//					This is only relevant for multiple random effects and/or GPs
-						}
-						// calculate explicit derivative of approx. mariginal log-likelihood
-						explicit_derivative = -0.5 * (double)(a_vec_.transpose() * (*SigmaDeriv) * a_vec_) +
-							0.5 * (ZtWZI_Sigma_inv.cwiseProduct(*SigmaDeriv)).sum();
-						// calculate implicit derivative (through mode) of approx. mariginal log-likelihood
-						SigmaDeriv_ZtFirstDeriv = (*SigmaDeriv) * ZtFirstDeriv;//auxiliary variable for caclulating d_mode_d_par
-						d_mode_d_par = SigmaDeriv_ZtFirstDeriv;//derivative of mode wrt to a covariance parameter
-						d_mode_d_par -= ((*Sigma) * (L_inv_ZtWZsqrt.transpose() * (L_inv_ZtWZsqrt * SigmaDeriv_ZtFirstDeriv)));
-						cov_grad[par_count] = explicit_derivative + d_mll_d_mode.dot(d_mode_d_par);
-						par_count++;
-					}
-				}
-			}//end calc_cov_grad
-			// calculate gradient wrt fixed effects
-			vec_t SigmaI_plus_ZtWZ_inv_d_mll_d_mode;// for implicit derivative
-			if (calc_F_grad || calc_aux_par_grad) {
-				vec_t L_inv_ZtWZsqrt_Sigma_d_mll_d_mode = L_inv_ZtWZsqrt_Sigma * d_mll_d_mode;
-				SigmaI_plus_ZtWZ_inv_d_mll_d_mode = (*Sigma) * d_mll_d_mode - L_inv_ZtWZsqrt_Sigma.transpose() * L_inv_ZtWZsqrt_Sigma_d_mll_d_mode;
-			}
-			if (calc_F_grad) {
-				fixed_effect_grad = -first_deriv_ll_;
-#pragma omp parallel for schedule(static)
-				for (data_size_t i = 0; i < num_data; ++i) {
-					fixed_effect_grad[i] += -0.5 * third_deriv[i] * SigmaI_plus_ZtWZ_inv_diag[random_effects_indices_of_data[i]] -
-						second_deriv_neg_ll_[i] * SigmaI_plus_ZtWZ_inv_d_mll_d_mode[random_effects_indices_of_data[i]];
-				}
-			}//end calc_F_grad
-			// calculate gradient wrt additional likelihood parameters
-			if (calc_aux_par_grad) {
-				vec_t neg_likelihood_deriv(num_aux_pars_);//derivative of the negative log-likelihood wrt additional parameters of the likelihood
-				vec_t second_deriv(num_data);//second derivative of the log-likelihood with respect to (i) the location parameter and (ii) an additional parameter of the likelihood
-				vec_t neg_third_deriv(num_data);//negative third derivative of the log-likelihood with respect to (i) two times the location parameter and (ii) an additional parameter of the likelihood
-				vec_t d_mode_d_aux_par;
-				CalcGradNegLogLikAuxPars(y_data, location_par.data(), num_data, neg_likelihood_deriv.data());
-				for (int ind_ap = 0; ind_ap < num_aux_pars_; ++ind_ap) {
-					CalcSecondNegThirdDerivLogLikAuxParsLocPar(y_data, location_par.data(), num_data, ind_ap, second_deriv.data(), neg_third_deriv.data());
-					double d_detmll_d_aux_par = 0., implicit_derivative = 0.;
-#pragma omp parallel for schedule(static) reduction(+:d_detmll_d_aux_par, implicit_derivative)
-					for (data_size_t i = 0; i < num_data; ++i) {
-						d_detmll_d_aux_par += neg_third_deriv[i] * SigmaI_plus_ZtWZ_inv_diag[random_effects_indices_of_data[i]];
-						implicit_derivative += second_deriv[i] * SigmaI_plus_ZtWZ_inv_d_mll_d_mode[random_effects_indices_of_data[i]];
-					}
-					aux_par_grad[ind_ap] = neg_likelihood_deriv[ind_ap] + 0.5 * d_detmll_d_aux_par + implicit_derivative;
-				}
-			}//end calc_aux_par_grad
-		}//end CalcGradNegMargLikelihoodLaplaceApproxOnlyOneGPCalculationsOnREScale
-
-		/*!
-		* \brief Calculate the gradient of the negative Laplace-approximated marginal log-likelihood wrt covariance parameters, 
-		*		fixed effects (e.g., for linear regression coefficients), and additional likelihood-related parameters.
-		*		Calculations are done by directly factorizing ("inverting) (Sigma^-1 + Zt*W*Z).
-		*		NOTE: IT IS ASSUMED THAT SIGMA IS A DIAGONAL MATRIX
-		*		This version is used for the Laplace approximation when there are only grouped random effects.
-		* \param y_data Response variable data if response variable is continuous
-		* \param y_data_int Response variable data if response variable is integer-valued
-		* \param fixed_effects Fixed effects component of location parameter
-		* \param num_data Number of data points
-		* \param SigmaI Inverse covariance matrix of latent random effect. Currently, this needs to be a diagonal matrix
-		* \param Zt Transpose Z^T of random effect design matrix that relates latent random effects to observations/likelihoods
-		* \param calc_cov_grad If true, the gradient wrt the covariance parameters is calculated
-		* \param calc_F_grad If true, the gradient wrt the fixed effects mean function F is calculated
-		* \param calc_aux_par_grad If true, the gradient wrt additional likelihood parameters is calculated
-		* \param[out] cov_grad Gradient wrt covariance parameters (needs to be preallocated of size num_cov_par)
-		* \param[out] fixed_effect_grad Gradient wrt fixed effects F (note: this is passed as a Eigen vector in order to avoid the need for copying)
-		* \param[out] aux_par_grad Gradient wrt additional likelihood parameters
-		* \param calc_mode If true, the mode of the random effects posterior is calculated otherwise the values in mode and a_vec_ are used (default=false)
-		*/
-		void CalcGradNegMargLikelihoodLaplaceApproxGroupedRE(const double* y_data,
-			const int* y_data_int,
-			const double* fixed_effects,
-			const data_size_t num_data,
-			const sp_mat_t& SigmaI,
-			const sp_mat_t& Zt,
-			std::vector<data_size_t> cum_num_rand_eff_cluster_i,
-			bool calc_cov_grad,
-			bool calc_F_grad,
-			bool calc_aux_par_grad,
-			double* cov_grad,
-			vec_t& fixed_effect_grad,
-			double* aux_par_grad,
-			bool calc_mode) {
-			int num_REs = (int)SigmaI.cols();//number of random effect realizations
-			int num_comps = (int)cum_num_rand_eff_cluster_i.size() - 1;//number of different random effect components
-			if (calc_mode) {// Calculate mode and Cholesky factor of Sigma^-1 + W at mode
-				double mll;//approximate marginal likelihood. This is a by-product that is not used here.
-				FindModePostRandEffCalcMLLGroupedRE(y_data, y_data_int, fixed_effects, num_data, SigmaI, Zt, mll);
-			}
-			if (na_or_inf_during_last_call_to_find_mode_) {
-				Log::REFatal(NA_OR_INF_ERROR_);
-			}
-			CHECK(mode_has_been_calculated_);
-			// Initialize variables
-			sp_mat_t Z = Zt.transpose();
-			vec_t location_par = Z * mode_;//location parameter = mode of random effects + fixed effects
-			if (fixed_effects != nullptr) {
-#pragma omp parallel for schedule(static)
-				for (data_size_t i = 0; i < num_data; ++i) {
-					location_par[i] += fixed_effects[i];
-				}
-			}
-			vec_t third_deriv(num_data);//vector of third derivatives of log-likelihood
-			CalcThirdDerivLogLik(y_data, y_data_int, location_par.data(), num_data, third_deriv.data());
-			// Calculate (Sigma^-1 + Zt*W*Z)^-1
-			sp_mat_t L_inv(num_REs, num_REs);
-			L_inv.setIdentity();
-			if (chol_fact_SigmaI_plus_ZtWZ_grouped_.permutationP().size() > 0) {//Permutation is only used when having an ordering
-				L_inv = chol_fact_SigmaI_plus_ZtWZ_grouped_.permutationP() * L_inv;
-			}
-			sp_mat_t L = chol_fact_SigmaI_plus_ZtWZ_grouped_.matrixL();
-			TriangularSolve<sp_mat_t, sp_mat_t, sp_mat_t>(L, L_inv, L_inv, false);
-			L.resize(0, 0);
-			sp_mat_t SigmaI_plus_ZtWZ_inv;
-			// calculate gradient of approx. marginal likelihood wrt the mode
-			vec_t d_mll_d_mode(num_REs);
-			sp_mat_t Zt_third_deriv = Zt * third_deriv.asDiagonal();//every column of Z multiplied elementwise by third_deriv
-#pragma omp parallel for schedule(static)
-			for (int ire = 0; ire < num_REs; ++ire) {
-				//calculate Z^T * diag(diag_d_W_d_mode_i) * Z = Z^T * diag(Z.col(i) * third_deriv) * Z
-				d_mll_d_mode[ire] = 0.;
-				double entry_ij;
-				for (data_size_t i = 0; i < num_data; ++i) {
-					entry_ij = Zt_third_deriv.coeff(ire, i);
-					if (std::abs(entry_ij) > EPSILON_NUMBERS) {
-						vec_t L_inv_Zt_col_i = L_inv * Zt.col(i);
-						d_mll_d_mode[ire] += entry_ij * (L_inv_Zt_col_i.squaredNorm());
-					}
-				}
-				d_mll_d_mode[ire] *= -0.5;
-			}
-			// calculate gradient wrt covariance parameters
-			if (calc_cov_grad) {
-				sp_mat_t ZtWZ = Zt * second_deriv_neg_ll_.asDiagonal() * Z;
-				vec_t d_mode_d_par;//derivative of mode wrt to a covariance parameter
-				vec_t v_aux;//auxiliary variable for caclulating d_mode_d_par
-				vec_t SigmaI_mode = SigmaI * mode_;
-				double explicit_derivative;
-				sp_mat_t I_j(num_REs, num_REs);//Diagonal matrix with 1 on the diagonal for all random effects of component j and 0's otherwise
-				sp_mat_t I_j_ZtWZ;
-				for (int j = 0; j < num_comps; ++j) {
-					// calculate explicit derivative of approx. mariginal log-likelihood
-					std::vector<Triplet_t> triplets(cum_num_rand_eff_cluster_i[j + 1] - cum_num_rand_eff_cluster_i[j]);//for constructing I_j
-					explicit_derivative = 0.;
-#pragma omp parallel for schedule(static) reduction(+:explicit_derivative)
-					for (int i = cum_num_rand_eff_cluster_i[j]; i < cum_num_rand_eff_cluster_i[j + 1]; ++i) {
-						triplets[i - cum_num_rand_eff_cluster_i[j]] = Triplet_t(i, i, 1.);
-						explicit_derivative += SigmaI_mode[i] * mode_[i];
-					}
-					explicit_derivative *= -0.5;
-					I_j.setFromTriplets(triplets.begin(), triplets.end());
-					I_j_ZtWZ = I_j * ZtWZ;
-					SigmaI_plus_ZtWZ_inv = I_j_ZtWZ;
-					CalcLtLGivenSparsityPattern<sp_mat_t>(L_inv, SigmaI_plus_ZtWZ_inv, false);
-					explicit_derivative += 0.5 * (SigmaI_plus_ZtWZ_inv.cwiseProduct(I_j_ZtWZ)).sum();
-					// calculate implicit derivative (through mode) of approx. mariginal log-likelihood
-					d_mode_d_par = L_inv.transpose() * (L_inv * (I_j * (Zt * first_deriv_ll_)));
-					cov_grad[j] = explicit_derivative + d_mll_d_mode.dot(d_mode_d_par);
-				}
-			}//end calc_cov_grad
-			// calculate gradient wrt fixed effects
-			if (calc_F_grad) {
-				vec_t d_detmll_d_F(num_data);
-#pragma omp parallel for schedule(static)
-				for (int i = 0; i < num_data; ++i) {
-					vec_t L_inv_Zt_col_i = L_inv * Zt.col(i);
-					d_detmll_d_F[i] = -0.5 * third_deriv[i] * (L_inv_Zt_col_i.squaredNorm());
-
-				}
-				vec_t d_mll_d_modeT_SigmaI_plus_ZtWZ_inv_Zt_W = (((d_mll_d_mode.transpose() * L_inv.transpose()) * L_inv) * Zt) * second_deriv_neg_ll_.asDiagonal();
-				fixed_effect_grad = -first_deriv_ll_ + d_detmll_d_F - d_mll_d_modeT_SigmaI_plus_ZtWZ_inv_Zt_W;
-			}//end calc_F_grad
-			// calculate gradient wrt additional likelihood parameters
-			if (calc_aux_par_grad) {
-				vec_t neg_likelihood_deriv(num_aux_pars_);//derivative of the negative log-likelihood wrt additional parameters of the likelihood
-				vec_t second_deriv(num_data);//second derivative of the log-likelihood with respect to (i) the location parameter and (ii) an additional parameter of the likelihood
-				vec_t neg_third_deriv(num_data);//negative third derivative of the log-likelihood with respect to (i) two times the location parameter and (ii) an additional parameter of the likelihood
-				vec_t d_mode_d_aux_par;
-				CalcGradNegLogLikAuxPars(y_data, location_par.data(), num_data, neg_likelihood_deriv.data());
-				for (int ind_ap = 0; ind_ap < num_aux_pars_; ++ind_ap) {
-					CalcSecondNegThirdDerivLogLikAuxParsLocPar(y_data, location_par.data(), num_data, ind_ap, second_deriv.data(), neg_third_deriv.data());
-					sp_mat_t ZtdWZ = Zt * neg_third_deriv.asDiagonal() * Z;
-					SigmaI_plus_ZtWZ_inv = ZtdWZ;
-					CalcLtLGivenSparsityPattern<sp_mat_t>(L_inv, SigmaI_plus_ZtWZ_inv, false);
-					double d_detmll_d_aux_par = (SigmaI_plus_ZtWZ_inv.cwiseProduct(ZtdWZ)).sum();
-					d_mode_d_aux_par = L_inv.transpose() * (L_inv * (Zt * second_deriv));
-					double implicit_derivative = d_mll_d_mode.dot(d_mode_d_aux_par);
-					aux_par_grad[ind_ap] = neg_likelihood_deriv[ind_ap] + 0.5 * d_detmll_d_aux_par + implicit_derivative;
-				}
-			}//end calc_aux_par_grad
-		}//end CalcGradNegMargLikelihoodLaplaceApproxGroupedRE
-
-		/*!
-		* \brief Calculate the gradient of the negative Laplace-approximated marginal log-likelihood wrt covariance parameters, 
-		*		fixed effects (e.g., for linear regression coefficients), and additional likelihood-related parameters.
-		*		Calculations are done by directly factorizing ("inverting) (Sigma^-1 + Zt*W*Z).
-		*		This version is used for the Laplace approximation when there are only grouped random effects with only one grouping variable.
-		* \param y_data Response variable data if response variable is continuous
-		* \param y_data_int Response variable data if response variable is integer-valued
-		* \param fixed_effects Fixed effects component of location parameter
-		* \param num_data Number of data points
-		* \param sigma2 Variance of random effects
-		* \param random_effects_indices_of_data Indices that indicate to which random effect every data point is related
-		* \param calc_cov_grad If true, the gradient wrt the covariance parameters is calculated
-		* \param calc_F_grad If true, the gradient wrt the fixed effects mean function F is calculated
-		* \param calc_aux_par_grad If true, the gradient wrt additional likelihood parameters is calculated
-		* \param[out] cov_grad Gradient wrt covariance parameters (needs to be preallocated of size num_cov_par)
-		* \param[out] fixed_effect_grad Gradient wrt fixed effects F (note: this is passed as a Eigen vector in order to avoid the need for copying)
-		* \param[out] aux_par_grad Gradient wrt additional likelihood parameters
-		* \param calc_mode If true, the mode of the random effects posterior is calculated otherwise the values in mode and a_vec_ are used (default=false)
-		*/
-		void CalcGradNegMargLikelihoodLaplaceApproxOnlyOneGroupedRECalculationsOnREScale(const double* y_data,
-			const int* y_data_int,
-			const double* fixed_effects,
-			const data_size_t num_data,
-			const double sigma2,
-			const data_size_t* const random_effects_indices_of_data,
-			bool calc_cov_grad,
-			bool calc_F_grad,
-			bool calc_aux_par_grad,
-			double* cov_grad,
-			vec_t& fixed_effect_grad,
-			double* aux_par_grad,
-			bool calc_mode) {
-			if (calc_mode) {// Calculate mode and Cholesky factor of Sigma^-1 + W at mode
-				double mll;//approximate marginal likelihood. This is a by-product that is not used here.
-				FindModePostRandEffCalcMLLOnlyOneGroupedRECalculationsOnREScale(y_data, y_data_int, fixed_effects, num_data,
-					sigma2, random_effects_indices_of_data, mll);
-			}
-			if (na_or_inf_during_last_call_to_find_mode_) {
-				Log::REFatal(NA_OR_INF_ERROR_);
-			}
-			CHECK(mode_has_been_calculated_);
-			// Initialize variables
-			vec_t location_par(num_data);//location parameter = mode of random effects + fixed effects
-			if (fixed_effects == nullptr) {
-#pragma omp parallel for schedule(static)
-				for (data_size_t i = 0; i < num_data; ++i) {
-					location_par[i] = mode_[random_effects_indices_of_data[i]];
-				}
-			}
-			else {
-#pragma omp parallel for schedule(static)
-				for (data_size_t i = 0; i < num_data; ++i) {
-					location_par[i] = mode_[random_effects_indices_of_data[i]] + fixed_effects[i];
-				}
-			}
-			vec_t third_deriv(num_data);//vector of third derivatives of log-likelihood
-			CalcThirdDerivLogLik(y_data, y_data_int, location_par.data(), num_data, third_deriv.data());
-			// calculate gradient of approx. marginal likelihood wrt the mode
-			vec_t d_mll_d_mode;
-			CalcZtVGivenIndices(num_data, num_re_, random_effects_indices_of_data, third_deriv, d_mll_d_mode, true);
-			d_mll_d_mode.array() /= -2. * diag_SigmaI_plus_ZtWZ_.array();	   
-			// calculate gradient wrt covariance parameters
-			if (calc_cov_grad) {
-				vec_t diag_ZtWZ;
-				CalcZtVGivenIndices(num_data, num_re_, random_effects_indices_of_data, second_deriv_neg_ll_, diag_ZtWZ, true);
-				double explicit_derivative = -0.5 * (mode_.array() * mode_.array()).sum() / sigma2 +
-					0.5 * (diag_ZtWZ.array() / diag_SigmaI_plus_ZtWZ_.array()).sum();
-				// calculate implicit derivative (through mode) of approx. mariginal log-likelihood
-				vec_t d_mode_d_par;
-				CalcZtVGivenIndices(num_data, num_re_, random_effects_indices_of_data, first_deriv_ll_, d_mode_d_par, true);
-				d_mode_d_par.array() /= diag_SigmaI_plus_ZtWZ_.array();
-				cov_grad[0] = explicit_derivative + d_mll_d_mode.dot(d_mode_d_par);
-			}//end calc_cov_grad
-			// calculate gradient wrt fixed effects
-			if (calc_F_grad) {
-#pragma omp parallel for schedule(static)
-				for (int i = 0; i < num_data; ++i) {
-					fixed_effect_grad[i] = -first_deriv_ll_[i] - 
-						0.5 * third_deriv[i] / diag_SigmaI_plus_ZtWZ_[random_effects_indices_of_data[i]] - //=d_detmll_d_F
-						d_mll_d_mode[random_effects_indices_of_data[i]] * second_deriv_neg_ll_[i] / diag_SigmaI_plus_ZtWZ_[random_effects_indices_of_data[i]];//=implicit derivative = d_mll_d_mode * d_mode_d_F
-				}
-			}//end calc_F_grad
-			// calculate gradient wrt additional likelihood parameters
-			if (calc_aux_par_grad) {
-				vec_t neg_likelihood_deriv(num_aux_pars_);//derivative of the negative log-likelihood wrt additional parameters of the likelihood
-				vec_t second_deriv(num_data);//second derivative of the log-likelihood with respect to (i) the location parameter and (ii) an additional parameter of the likelihood
-				vec_t neg_third_deriv(num_data);//negative third derivative of the log-likelihood with respect to (i) two times the location parameter and (ii) an additional parameter of the likelihood
-				CalcGradNegLogLikAuxPars(y_data, location_par.data(), num_data, neg_likelihood_deriv.data());
-				for (int ind_ap = 0; ind_ap < num_aux_pars_; ++ind_ap) {
-					CalcSecondNegThirdDerivLogLikAuxParsLocPar(y_data, location_par.data(), num_data, ind_ap, second_deriv.data(), neg_third_deriv.data());
-					double d_detmll_d_aux_par = 0.;
-					double implicit_derivative = 0.;// = implicit derivative = d_mll_d_mode * d_mode_d_aux_par
-#pragma omp parallel for schedule(static) reduction(+:d_detmll_d_aux_par, implicit_derivative)
-					for (int i = 0; i < num_data; ++i) { 
-						d_detmll_d_aux_par += neg_third_deriv[i] / diag_SigmaI_plus_ZtWZ_[random_effects_indices_of_data[i]];
-						implicit_derivative += d_mll_d_mode[random_effects_indices_of_data[i]] * second_deriv[i] / diag_SigmaI_plus_ZtWZ_[random_effects_indices_of_data[i]];
-					}
-					aux_par_grad[ind_ap] = neg_likelihood_deriv[ind_ap] + 0.5 * d_detmll_d_aux_par + implicit_derivative;
-					//Equivalent code:
-					//vec_t Zt_second_deriv, diag_Zt_neg_third_deriv_Z;
-					//CalcZtVGivenIndices(num_data, num_re_, random_effects_indices_of_data, second_deriv, Zt_second_deriv, true);
-					//CalcZtVGivenIndices(num_data, num_re_, random_effects_indices_of_data, neg_third_deriv, diag_Zt_neg_third_deriv_Z, true);
-					//double d_detmll_d_aux_par = (diag_Zt_neg_third_deriv_Z.array() / diag_SigmaI_plus_ZtWZ_.array()).sum();
-					//double implicit_derivative = (d_mll_d_mode.array() * Zt_second_deriv.array() / diag_SigmaI_plus_ZtWZ_.array()).sum();
-				}
-			}//end calc_aux_par_grad
-		}//end CalcGradNegMargLikelihoodLaplaceApproxOnlyOneGroupedRECalculationsOnREScale
-
-		/*!
-		* \brief Calculate the gradient of the negative Laplace-approximated marginal log-likelihood wrt covariance parameters, 
-		*		fixed effects (e.g., for linear regression coefficients), and additional likelihood-related parameters.
-		*		Calculations are done by factorizing ("inverting) (Sigma^-1 + W) where it is assumed that an approximate Cholesky factor
-		*		of Sigma^-1 has previously been calculated using a Vecchia approximation.
-		*		This version is used for the Laplace approximation when there are only GP random effects and the Vecchia approximation is used.
-		*		Caveat: Sigma^-1 + W can be not very sparse
-		* \param y_data Response variable data if response variable is continuous
-		* \param y_data_int Response variable data if response variable is integer-valued
-		* \param fixed_effects Fixed effects component of location parameter
-		* \param num_data Number of data points
-		* \param B Matrix B in Vecchia approximation Sigma^-1 = B^T D^-1 B ("=" Cholesky factor)
-		* \param D_inv Diagonal matrix D^-1 in Vecchia approximation Sigma^-1 = B^T D^-1 B
-		* \param B_grad Derivatives of matrices B ( = derivative of matrix -A) for Vecchia approximation
-		* \param D_grad Derivatives of matrices D for Vecchia approximation
-		* \param calc_cov_grad If true, the gradient wrt the covariance parameters is calculated
-		* \param calc_F_grad If true, the gradient wrt the fixed effects mean function F is calculated
-		* \param calc_aux_par_grad If true, the gradient wrt additional likelihood parameters is calculated
-		* \param[out] cov_grad Gradient of approximate marginal log-likelihood wrt covariance parameters (needs to be preallocated of size num_cov_par)
-		* \param[out] fixed_effect_grad Gradient of approximate marginal log-likelihood wrt fixed effects F (note: this is passed as a Eigen vector in order to avoid the need for copying)
-		* \param[out] aux_par_grad Gradient wrt additional likelihood parameters
-		* \param calc_mode If true, the mode of the random effects posterior is calculated otherwise the values in mode and a_vec_ are used (default=false)
-		* \param num_comps_total Total number of random effect components ( = number of GPs)
-		*/
-		void CalcGradNegMargLikelihoodLaplaceApproxVecchia(const double* y_data,
-			const int* y_data_int,
-			const double* fixed_effects,
-			const data_size_t num_data,
-			const sp_mat_t& B,
-			const sp_mat_t& D_inv,
-			const std::vector<sp_mat_t>& B_grad,
-			const std::vector<sp_mat_t>& D_grad,
-			bool calc_cov_grad,
-			bool calc_F_grad,
-			bool calc_aux_par_grad,
-			double* cov_grad,
-			vec_t& fixed_effect_grad,
-			double* aux_par_grad,
-			bool calc_mode,
-			int num_comps_total) {
-			if (calc_mode) {// Calculate mode and Cholesky factor of Sigma^-1 + W at mode
-				double mll;//approximate marginal likelihood. This is a by-product that is not used here.
-				FindModePostRandEffCalcMLLVecchia(y_data, y_data_int, fixed_effects, num_data, B, D_inv, mll);
-			}
-			if (na_or_inf_during_last_call_to_find_mode_) {
-				Log::REFatal(NA_OR_INF_ERROR_);
-			}
-			CHECK(mode_has_been_calculated_);
-			// Initialize variables
-			bool no_fixed_effects = (fixed_effects == nullptr);
-			vec_t location_par;//location parameter = mode of random effects + fixed effects
-			double* location_par_ptr;
-			vec_t third_deriv(num_data);//vector of third derivatives of log-likelihood
-			if (no_fixed_effects) {
-				location_par_ptr = mode_.data();
-			}
-			else {
-				location_par = vec_t(num_data);
-#pragma omp parallel for schedule(static)
-				for (data_size_t i = 0; i < num_data; ++i) {
-					location_par[i] = mode_[i] + fixed_effects[i];
-				}
-				location_par_ptr = location_par.data();
-			}
-			CalcThirdDerivLogLik(y_data, y_data_int, location_par_ptr, num_data, third_deriv.data());
-			// Calculate (Sigma^-1 + W)^-1
-			sp_mat_t L_inv(num_data, num_data);
-			L_inv.setIdentity();
-			TriangularSolveGivenCholesky<chol_sp_mat_t, sp_mat_t, sp_mat_t, sp_mat_t>(chol_fact_SigmaI_plus_ZtWZ_vecchia_, L_inv, L_inv, false);
-			vec_t d_mll_d_mode, SigmaI_plus_W_inv_d_mll_d_mode, SigmaI_plus_W_inv_diag;
-			sp_mat_t SigmaI_plus_W_inv;
-			// Calculate gradient wrt covariance parameters
-			if (calc_cov_grad) {
-				double explicit_derivative;
-				int num_par = (int)B_grad.size();
-				sp_mat_t SigmaI_deriv, BgradT_Dinv_B, Bt_Dinv_Bgrad;
-				sp_mat_t D_inv_B = D_inv * B;
-				for (int j = 0; j < num_par; ++j) {
-					// Calculate SigmaI_deriv
-					if (num_comps_total == 1 && j == 0) {
-						SigmaI_deriv = - B.transpose() * D_inv_B;//SigmaI_deriv = -SigmaI for variance parameters if there is only one GP
-					}
-					else {
-						SigmaI_deriv = B_grad[j].transpose() * D_inv_B;
-						Bt_Dinv_Bgrad = SigmaI_deriv.transpose();
-						SigmaI_deriv += Bt_Dinv_Bgrad - D_inv_B.transpose() * D_grad[j] * D_inv_B;
-						Bt_Dinv_Bgrad.resize(0, 0);
-					}
-					if (j == 0) {
-						// Calculate SigmaI_plus_W_inv = L_inv.transpose() * L_inv at non-zero entries of SigmaI_deriv
-						//	Note: fully calculating SigmaI_plus_W_inv = L_inv.transpose() * L_inv is very slow
-						SigmaI_plus_W_inv = SigmaI_deriv;
-						CalcLtLGivenSparsityPattern<sp_mat_t>(L_inv, SigmaI_plus_W_inv, true);
-						d_mll_d_mode = -0.5 * (SigmaI_plus_W_inv.diagonal().array() * third_deriv.array()).matrix();
-					}//end if j == 0
-					SigmaI_plus_W_inv_d_mll_d_mode = L_inv.transpose() * (L_inv * d_mll_d_mode);
-					vec_t SigmaI_deriv_mode = SigmaI_deriv * mode_;
-					explicit_derivative = 0.5 * (mode_.dot(SigmaI_deriv_mode) + (SigmaI_deriv.cwiseProduct(SigmaI_plus_W_inv)).sum());
-					if (num_comps_total == 1 && j == 0) {
-						explicit_derivative += 0.5 * num_data;
-					}
-					else {
-						explicit_derivative += 0.5 * (D_inv.diagonal().array() * D_grad[j].diagonal().array()).sum();
-					}
-					cov_grad[j] = explicit_derivative - SigmaI_plus_W_inv_d_mll_d_mode.dot(SigmaI_deriv_mode);//add implicit derivative
-				}
-			}//end calc_cov_grad
-			if (calc_F_grad || calc_aux_par_grad) {
-				if (!calc_cov_grad) {
-					sp_mat_t L_inv_sqr = L_inv.cwiseProduct(L_inv);
-					SigmaI_plus_W_inv_diag = L_inv_sqr.transpose() * vec_t::Ones(L_inv_sqr.rows());// diagonal of (Sigma^-1 + W) ^ -1
-					d_mll_d_mode = (-0.5 * SigmaI_plus_W_inv_diag.array() * third_deriv.array()).matrix();// gradient of approx. marginal likelihood wrt the mode and thus also F here
-					SigmaI_plus_W_inv_d_mll_d_mode = L_inv.transpose() * (L_inv * d_mll_d_mode);
-				}
-				else if (calc_aux_par_grad) {
-					SigmaI_plus_W_inv_diag = SigmaI_plus_W_inv.diagonal();
-				}
-			}
-			// Calculate gradient wrt fixed effects
-			if (calc_F_grad) {
-				vec_t d_mll_d_F_implicit = -(SigmaI_plus_W_inv_d_mll_d_mode.array() * second_deriv_neg_ll_.array()).matrix();// implicit derivative
-				fixed_effect_grad = -first_deriv_ll_ + d_mll_d_mode + d_mll_d_F_implicit;
-			}//end calc_F_grad
-			// calculate gradient wrt additional likelihood parameters
-			if (calc_aux_par_grad) {
-				vec_t neg_likelihood_deriv(num_aux_pars_);//derivative of the negative log-likelihood wrt additional parameters of the likelihood
-				vec_t second_deriv(num_data);//second derivative of the log-likelihood with respect to (i) the location parameter and (ii) an additional parameter of the likelihood
-				vec_t neg_third_deriv(num_data);//negative third derivative of the log-likelihood with respect to (i) two times the location parameter and (ii) an additional parameter of the likelihood
-				vec_t d_mode_d_aux_par;
-				CalcGradNegLogLikAuxPars(y_data, location_par_ptr, num_data, neg_likelihood_deriv.data());
-				for (int ind_ap = 0; ind_ap < num_aux_pars_; ++ind_ap) {
-					CalcSecondNegThirdDerivLogLikAuxParsLocPar(y_data, location_par_ptr, num_data, ind_ap, second_deriv.data(), neg_third_deriv.data());
-					double d_detmll_d_aux_par = 0., implicit_derivative = 0.;
-#pragma omp parallel for schedule(static) reduction(+:d_detmll_d_aux_par, implicit_derivative)
-					for (data_size_t i = 0; i < num_data; ++i) {
-						d_detmll_d_aux_par += neg_third_deriv[i] * SigmaI_plus_W_inv_diag[i];
-						implicit_derivative += second_deriv[i] * SigmaI_plus_W_inv_d_mll_d_mode[i];
-					}
-					aux_par_grad[ind_ap] = neg_likelihood_deriv[ind_ap] + 0.5 * d_detmll_d_aux_par + implicit_derivative;
-				}
-			}//end calc_aux_par_grad
-		}//end CalcGradNegMargLikelihoodLaplaceApproxVecchia
-
-		/*!
-		* \brief Make predictions for the (latent) random effects when using the Laplace approximation.
-		*		Calculations are done using a numerically stable variant based on factorizing ("inverting") B = (Id + Wsqrt * Z*Sigma*Zt * Wsqrt).
-		*		In the notation of the paper: "Sigma = Z*Sigma*Z^T" and "Z = Id".
-		*		This version is used for the Laplace approximation when dense matrices are used (e.g. GP models).
-		* \param y_data Response variable data if response variable is continuous
-		* \param y_data_int Response variable data if response variable is integer-valued
-		* \param fixed_effects Fixed effects component of location parameter
-		* \param num_data Number of data points
-		* \param ZSigmaZt Covariance matrix of latent random effect
-		* \param Cross_Cov Cross covariance matrix between predicted and obsreved random effects ("=Cov(y_p,y)")
-		* \param pred_mean[out] Predictive mean
-		* \param pred_cov[out] Predictive covariance matrix
-		* \param pred_var[out] Predictive variances
-		* \param calc_pred_cov If true, predictive covariance matrix is also calculated
-		* \param calc_pred_var If true, predictive variances are also calculated
-		* \param calc_mode If true, the mode of the random effects posterior is calculated otherwise the values in mode and a_vec_ are used (default=false)
-		*/
-		void PredictLaplaceApproxStable(const double* y_data,
-			const int* y_data_int,
-			const double* fixed_effects,
-			const data_size_t num_data,
-			const std::shared_ptr<T_mat> ZSigmaZt,
-			const T_mat& Cross_Cov,
-			vec_t& pred_mean,
-			T_mat& pred_cov,
-			vec_t& pred_var,
-			bool calc_pred_cov,
-			bool calc_pred_var,
-			bool calc_mode) {
-			if (calc_mode) {// Calculate mode and Cholesky factor of B = (Id + Wsqrt * ZSigmaZt * Wsqrt) at mode
-				double mll;//approximate marginal likelihood. This is a by-product that is not used here.
-				FindModePostRandEffCalcMLLStable(y_data, y_data_int, fixed_effects, num_data, ZSigmaZt, mll);
-			}
-			if (na_or_inf_during_last_call_to_find_mode_) {
-				Log::REFatal(NA_OR_INF_ERROR_);
-			}
-			CHECK(mode_has_been_calculated_);
-			pred_mean = Cross_Cov * first_deriv_ll_;
-			if (calc_pred_cov || calc_pred_var) {
-				sp_mat_t Wsqrt(num_data, num_data);//diagonal matrix with square root of negative second derivatives on the diagonal (sqrt of negative Hessian of log-likelihood)
-				Wsqrt.setIdentity();
-				Wsqrt.diagonal().array() = second_deriv_neg_ll_.array().sqrt();
-				T_mat Maux = Wsqrt * Cross_Cov.transpose();
-				TriangularSolveGivenCholesky<T_chol, T_mat, T_mat, T_mat>(chol_fact_Id_plus_Wsqrt_Sigma_Wsqrt_, Maux, Maux, false);
-				if (calc_pred_cov) {
-					pred_cov -= (T_mat)(Maux.transpose() * Maux);
-				}
-				if (calc_pred_var) {
-					Maux = Maux.cwiseProduct(Maux);
-#pragma omp parallel for schedule(static)
-					for (int i = 0; i < (int)pred_mean.size(); ++i) {
-						pred_var[i] -= Maux.col(i).sum();
-					}
-				}
-			}
-		}//end PredictLaplaceApproxStable
-
-		/*!
-		* \brief Make predictions for the (latent) random effects when using the Laplace approximation.
-		*		Calculations are done using a numerically stable variant based on factorizing ("inverting") B = (Id + Wsqrt * Z*Sigma*Zt * Wsqrt).
-		*		In the notation of the paper: "Sigma = Z*Sigma*Z^T" and "Z = Id".
-		*		This version is used for the Laplace approximation when dense matrices are used (e.g. GP models).
-		* \param y_data Response variable data if response variable is continuous
-		* \param y_data_int Response variable data if response variable is integer-valued
-		* \param fixed_effects Fixed effects component of location parameter
-		* \param num_data Number of data points
-		* \param Sigma Covariance matrix of latent random effect
-		* \param random_effects_indices_of_data Indices that indicate to which random effect every data point is related
-		* \param Cross_Cov Cross covariance matrix between predicted and obsreved random effects ("=Cov(y_p,y)")
-		* \param pred_mean[out] Predictive mean
-		* \param pred_cov[out] Predictive covariance matrix
-		* \param pred_var[out] Predictive variances
-		* \param calc_pred_cov If true, predictive covariance matrix is also calculated
-		* \param calc_pred_var If true, predictive variances are also calculated
-		* \param calc_mode If true, the mode of the random effects posterior is calculated otherwise the values in mode and a_vec_ are used (default=false)
-		*/
-		void PredictLaplaceApproxOnlyOneGPCalculationsOnREScale(const double* y_data,
-			const int* y_data_int,
-			const double* fixed_effects,
-			const data_size_t num_data,
-			const std::shared_ptr<T_mat> Sigma,
-			const data_size_t* const random_effects_indices_of_data,
-			const T_mat& Cross_Cov,
-			vec_t& pred_mean,
-			T_mat& pred_cov,
-			vec_t& pred_var,
-			bool calc_pred_cov,
-			bool calc_pred_var,
-			bool calc_mode) {
-			if (calc_mode) {// Calculate mode and Cholesky factor of B = (Id + Wsqrt * ZSigmaZt * Wsqrt) at mode
-				double mll;//approximate marginal likelihood. This is a by-product that is not used here.
-				FindModePostRandEffCalcMLLOnlyOneGPCalculationsOnREScale(y_data, y_data_int, fixed_effects,
-					num_data, Sigma, random_effects_indices_of_data, mll);
-			}
-			if (na_or_inf_during_last_call_to_find_mode_) {
-				Log::REFatal(NA_OR_INF_ERROR_);
-			}
-			CHECK(mode_has_been_calculated_);
-			vec_t ZtFirstDeriv;
-			CalcZtVGivenIndices(num_data, num_re_, random_effects_indices_of_data, first_deriv_ll_, ZtFirstDeriv, true);
-			pred_mean = Cross_Cov * ZtFirstDeriv;
-			if (calc_pred_cov || calc_pred_var) {
-				vec_t diag_ZtWZ;
-				CalcZtVGivenIndices(num_data, num_re_, random_effects_indices_of_data, second_deriv_neg_ll_, diag_ZtWZ, true);
-				sp_mat_t ZtWZsqrt(num_re_, num_re_);//diagonal matrix with square root of diagonal of ZtWZ
-				ZtWZsqrt.setIdentity();
-				ZtWZsqrt.diagonal().array() = diag_ZtWZ.array().sqrt();
-				T_mat Maux = ZtWZsqrt * Cross_Cov.transpose();
-				TriangularSolveGivenCholesky<T_chol, T_mat, T_mat, T_mat>(chol_fact_Id_plus_Wsqrt_Sigma_Wsqrt_, Maux, Maux, false);//Maux = L\(ZtWZsqrt * Cross_Cov^T)
-				if (calc_pred_cov) {
-					pred_cov -= (T_mat)(Maux.transpose() * Maux);
-				}
-				if (calc_pred_var) {
-					Maux = Maux.cwiseProduct(Maux);
-#pragma omp parallel for schedule(static)
-					for (int i = 0; i < (int)pred_mean.size(); ++i) {
-						pred_var[i] -= Maux.col(i).sum();
-					}
-				}
-			}
-		}//end PredictLaplaceApproxOnlyOneGPCalculationsOnREScale
-
-		/*!
-		* \brief Make predictions for the (latent) random effects when using the Laplace approximation.
-		*		Calculations are done by directly factorizing ("inverting) (Sigma^-1 + Zt*W*Z).
-		*		NOTE: IT IS ASSUMED THAT SIGMA IS A DIAGONAL MATRIX
-		*		This version is used for the Laplace approximation when there are only grouped random effects.
-		* \param y_data Response variable data if response variable is continuous
-		* \param y_data_int Response variable data if response variable is integer-valued
-		* \param fixed_effects Fixed effects component of location parameter
-		* \param num_data Number of data points
-		* \param SigmaI Inverse covariance matrix of latent random effect. Currently, this needs to be a diagonal matrix
-		* \param Zt Transpose Z^T of random effect design matrix that relates latent random effects to observations/likelihoods
-		* \param Ztilde matrix which relates existing random effects to prediction samples
-		* \param Sigma Covariance matrix of random effects
-		* \param pred_mean[out] Predictive mean
-		* \param pred_cov[out] Predictive covariance matrix
-		* \param pred_var[out] Predictive variances
-		* \param calc_pred_cov If true, predictive covariance matrix is also calculated
-		* \param calc_pred_var If true, predictive variances are also calculated
-		* \param calc_mode If true, the mode of the random effects posterior is calculated otherwise the values in mode and a_vec_ are used (default=false)
-		*/
-		void PredictLaplaceApproxGroupedRE(const double* y_data,
-			const int* y_data_int,
-			const double* fixed_effects,
-			const data_size_t num_data,
-			const sp_mat_t& SigmaI,
-			const sp_mat_t& Zt,
-			const sp_mat_t& Ztilde,
-			const sp_mat_t& Sigma,
-			vec_t& pred_mean,
-			T_mat& pred_cov,
-			vec_t& pred_var,
-			bool calc_pred_cov,
-			bool calc_pred_var,
-			bool calc_mode) {
-			if (calc_mode) {// Calculate mode and Cholesky factor of B = (Id + Wsqrt * ZSigmaZt * Wsqrt) at mode
-				double mll;//approximate marginal likelihood. This is a by-product that is not used here.
-				FindModePostRandEffCalcMLLGroupedRE(y_data, y_data_int, fixed_effects, num_data, SigmaI, Zt, mll);
-			}
-			if (na_or_inf_during_last_call_to_find_mode_) {
-				Log::REFatal(NA_OR_INF_ERROR_);
-			}
-			CHECK(mode_has_been_calculated_);
-			vec_t v_aux = Zt * first_deriv_ll_;
-			vec_t v_aux2 = Sigma * v_aux;
-			pred_mean = Ztilde * v_aux2;
-			if (calc_pred_cov || calc_pred_var) {
-				// calculate Maux = L\(Z^T * second_deriv_neg_ll_.asDiagonal() * Cross_Cov^T)
-				sp_mat_t Cross_Cov = Ztilde * Sigma * Zt;
-				sp_mat_t Maux = Zt * second_deriv_neg_ll_.asDiagonal() * Cross_Cov.transpose();
-				TriangularSolveGivenCholesky<chol_sp_mat_t, sp_mat_t, sp_mat_t, sp_mat_t>(chol_fact_SigmaI_plus_ZtWZ_grouped_, Maux, Maux, false);
-				if (calc_pred_cov) {
-					pred_cov += (T_mat)(Maux.transpose() * Maux); 
-					pred_cov -= (T_mat)(Cross_Cov * second_deriv_neg_ll_.asDiagonal() * Cross_Cov.transpose());
-				}
-				if (calc_pred_var) {
-					sp_mat_t Maux3 = Cross_Cov.cwiseProduct(Cross_Cov * second_deriv_neg_ll_.asDiagonal());
-					Maux = Maux.cwiseProduct(Maux);
-#pragma omp parallel for schedule(static)
-					for (int i = 0; i < (int)pred_mean.size(); ++i) {
-						pred_var[i] += Maux.col(i).sum() - Maux3.row(i).sum();
-					}
-				}
-			}
-		}//end PredictLaplaceApproxGroupedRE
-
-		/*!
-		* \brief Make predictions for the (latent) random effects when using the Laplace approximation.
-		*		Calculations are done by directly factorizing ("inverting) (Sigma^-1 + Zt*W*Z).
-		*		This version is used for the Laplace approximation when there are only grouped random effects with only one grouping variable.
-		* \param y_data Response variable data if response variable is continuous
-		* \param y_data_int Response variable data if response variable is integer-valued
-		* \param fixed_effects Fixed effects component of location parameter
-		* \param num_data Number of data points
-		* \param sigma2 Variance of random effects
-		* \param random_effects_indices_of_data Indices that indicate to which random effect every data point is related
-		* \param Cross_Cov Cross covariance matrix between predicted and obsreved random effects ("=Cov(y_p,y)")
-		* \param pred_mean[out] Predictive mean
-		* \param pred_cov[out] Predictive covariance matrix
-		* \param pred_var[out] Predictive variances
-		* \param calc_pred_cov If true, predictive covariance matrix is also calculated
-		* \param calc_pred_var If true, predictive variances are also calculated
-		* \param calc_mode If true, the mode of the random effects posterior is calculated otherwise the values in mode and a_vec_ are used (default=false)
-		*/
-		void PredictLaplaceApproxOnlyOneGroupedRECalculationsOnREScale(const double* y_data,
-			const int* y_data_int,
-			const double* fixed_effects,
-			const data_size_t num_data,
-			const double sigma2,
-			const data_size_t* const random_effects_indices_of_data,
-			const T_mat& Cross_Cov,
-			vec_t& pred_mean,
-			T_mat& pred_cov,
-			vec_t& pred_var,
-			bool calc_pred_cov,
-			bool calc_pred_var,
-			bool calc_mode) {
-			if (calc_mode) {// Calculate mode and Cholesky factor of B = (Id + Wsqrt * ZSigmaZt * Wsqrt) at mode
-				double mll;//approximate marginal likelihood. This is a by-product that is not used here.
-				FindModePostRandEffCalcMLLOnlyOneGroupedRECalculationsOnREScale(y_data, y_data_int, fixed_effects, num_data,
-					sigma2, random_effects_indices_of_data, mll);
-			}
-			if (na_or_inf_during_last_call_to_find_mode_) {
-				Log::REFatal(NA_OR_INF_ERROR_);
-			}
-			CHECK(mode_has_been_calculated_);
-			vec_t ZtFirstDeriv;
-			CalcZtVGivenIndices(num_data, num_re_, random_effects_indices_of_data, first_deriv_ll_, ZtFirstDeriv, true);
-			pred_mean = Cross_Cov * ZtFirstDeriv;
-			if (calc_pred_cov || calc_pred_var) {
-				vec_t diag_Sigma_plus_ZtWZI(num_re_);
-				diag_Sigma_plus_ZtWZI.array() = 1. / diag_SigmaI_plus_ZtWZ_.array();
-				diag_Sigma_plus_ZtWZI.array() /= sigma2;
-				diag_Sigma_plus_ZtWZI.array() -= 1.;
-				diag_Sigma_plus_ZtWZI.array() /= sigma2;
-				if (calc_pred_cov) {
-					T_mat Maux = Cross_Cov * diag_Sigma_plus_ZtWZI.asDiagonal() * Cross_Cov.transpose();
-					pred_cov += Maux;
-				}
-				if (calc_pred_var) {
-					T_mat Maux = Cross_Cov * diag_Sigma_plus_ZtWZI.asDiagonal();
-					T_mat Maux2 = Cross_Cov.cwiseProduct(Maux);
-#pragma omp parallel for schedule(static)
-					for (int i = 0; i < (int)pred_mean.size(); ++i) {
-						pred_var[i] += Maux2.row(i).sum();
-					}
-				}
-			}
-		}//end PredictLaplaceApproxOnlyOneGroupedRECalculationsOnREScale
-
-		/*!
-		* \brief Make predictions for the (latent) random effects when using the Laplace approximation.
-		*		Calculations are done by factorizing ("inverting) (Sigma^-1 + W) where it is assumed that an approximate Cholesky factor
-		*		of Sigma^-1 has previously been calculated using a Vecchia approximation.
-		*		This version is used for the Laplace approximation when there are only GP random effects and the Vecchia approximation is used.
-		*		Caveat: Sigma^-1 + W can be not very sparse
-		* \param y_data Response variable data if response variable is continuous
-		* \param y_data_int Response variable data if response variable is integer-valued
-		* \param fixed_effects Fixed effects component of location parameter
-		* \param num_data Number of data points
-		* \param B Matrix B in Vecchia approximation for observed locations, Sigma^-1 = B^T D^-1 B ("=" Cholesky factor)
-		* \param D_inv Diagonal matrix D^-1 in Vecchia approximation for observed locations
-		* \param Bpo Lower left part of matrix B in joint Vecchia approximation for observed and prediction locations with non-zero off-diagonal entries corresponding to the nearest neighbors of the prediction locations among the observed locations
-		* \param Bp Lower right part of matrix B in joint Vecchia approximation for observed and prediction locations with non-zero off-diagonal entries corresponding to the nearest neighbors of the prediction locations among the prediction locations
-		* \param Dp Diagonal matrix with lower right part of matrix D in joint Vecchia approximation for observed and prediction locations
-		* \param pred_mean[out] Predictive mean
-		* \param pred_cov[out] Predictive covariance matrix
-		* \param pred_var[out] Predictive variances
-		* \param calc_pred_cov If true, predictive covariance matrix is also calculated
-		* \param calc_pred_var If true, predictive variances are also calculated
-		* \param calc_mode If true, the mode of the random effects posterior is calculated otherwise the values in mode and a_vec_ are used (default=false)
-		* \param CondObsOnly If true, the nearest neighbors for the predictions are found only among the observed data and Bp is an identity matrix
-		*/
-		void PredictLaplaceApproxVecchia(const double* y_data,
-			const int* y_data_int,
-			const double* fixed_effects,
-			const data_size_t num_data,
-			const sp_mat_t& B,
-			const sp_mat_t& D_inv,
-			const sp_mat_t& Bpo,
-			sp_mat_t& Bp,
-			const vec_t& Dp,
-			vec_t& pred_mean,
-			T_mat& pred_cov,
-			vec_t& pred_var,
-			bool calc_pred_cov,
-			bool calc_pred_var,
-			bool calc_mode,
-			bool CondObsOnly) {
-			if (calc_mode) {// Calculate mode and Cholesky factor of Sigma^-1 + W at mode
-				double mll;//approximate marginal likelihood. This is a by-product that is not used here.
-				FindModePostRandEffCalcMLLVecchia(y_data, y_data_int, fixed_effects, num_data, B, D_inv, mll);
-			}
-			if (na_or_inf_during_last_call_to_find_mode_) {
-				Log::REFatal(NA_OR_INF_ERROR_);
-			}
-			CHECK(mode_has_been_calculated_);
-			int num_pred = (int)Bp.cols();
-			CHECK((int)Dp.size() == num_pred);
-			if (CondObsOnly) {
-				pred_mean = -Bpo * mode_;
-			}
-			else {
-				vec_t Bpo_mode = Bpo * mode_;
-				pred_mean = -Bp.triangularView<Eigen::UpLoType::UnitLower>().solve(Bpo_mode);
-			}
-			if (calc_pred_cov || calc_pred_var) {
-				sp_mat_t Bp_inv, Bp_inv_Dp;
-				sp_mat_t Maux; //Maux = L\(Bpo^T * Bp^-1), L = Chol(Sigma^-1 + W)
-				if (CondObsOnly) {
-					Maux = Bpo.transpose();//Bp = Id
-				}
-				else {
-					Bp_inv = sp_mat_t(Bp.rows(), Bp.cols());
-					Bp_inv.setIdentity();
-					TriangularSolve<sp_mat_t, sp_mat_t, sp_mat_t>(Bp, Bp_inv, Bp_inv, false);
-					//Bp.triangularView<Eigen::UpLoType::UnitLower>().solveInPlace(Bp_inv);//much slower
-					Maux = Bpo.transpose() * Bp_inv.transpose();
-					Bp_inv_Dp = Bp_inv * Dp.asDiagonal();
-				}
-				TriangularSolveGivenCholesky<chol_sp_mat_t, sp_mat_t, sp_mat_t, sp_mat_t>(chol_fact_SigmaI_plus_ZtWZ_vecchia_, Maux, Maux, false);
-				if (calc_pred_cov) {
-					if (CondObsOnly) {
-						pred_cov = Maux.transpose() * Maux;
-						pred_cov.diagonal().array() += Dp.array();
-					}
-					else {
-						pred_cov = Bp_inv_Dp * Bp_inv.transpose() + Maux.transpose() * Maux;
-					}
-				}
-				if (calc_pred_var) {
-					pred_var = vec_t(num_pred);
-					Maux = Maux.cwiseProduct(Maux);
-					if (CondObsOnly) {
-#pragma omp parallel for schedule(static)
-						for (int i = 0; i < num_pred; ++i) {
-							pred_var[i] = Dp[i] + Maux.col(i).sum();
-						}
-					}
-					else {
-#pragma omp parallel for schedule(static)
-						for (int i = 0; i < num_pred; ++i) {
-							pred_var[i] = (Bp_inv_Dp.row(i)).dot(Bp_inv.row(i)) + Maux.col(i).sum();
-						}
-					}
-				}
-			}//end calc_pred_cov || calc_pred_var
-		}//end PredictLaplaceApproxVecchia
-
-//Note: the following is currently not used
-//		/*!
-//		* \brief Calculate variance of Laplace-approximated posterior
-//		* \param ZSigmaZt Covariance matrix of latent random effect
-//		* \param[out] pred_var Variance of Laplace-approximated posterior
-//		*/
-//		void CalcVarLaplaceApproxStable(const std::shared_ptr<T_mat> ZSigmaZt,
-//			vec_t& pred_var) {
-//			if (na_or_inf_during_last_call_to_find_mode_) {
-//				Log::REFatal(NA_OR_INF_ERROR_);
-//			}
-//			CHECK(mode_has_been_calculated_);
-//			pred_var = vec_t(num_re_);
-//			vec_t diag_Wsqrt(second_deriv_neg_ll_.size());
-//			diag_Wsqrt.array() = second_deriv_neg_ll_.array().sqrt();
-//			T_mat L_inv_W_sqrt_ZSigmaZt = diag_Wsqrt.asDiagonal() * (*ZSigmaZt);
-//			TriangularSolveGivenCholesky<T_chol, T_mat, T_mat, T_mat>(chol_fact_Id_plus_Wsqrt_Sigma_Wsqrt_, L_inv_W_sqrt_ZSigmaZt, L_inv_W_sqrt_ZSigmaZt, false);
-//#pragma omp parallel for schedule(static)
-//			for (int i = 0; i < num_re_; ++i) {
-//				pred_var[i] = (*ZSigmaZt).coeff(i,i) - L_inv_W_sqrt_ZSigmaZt.col(i).squaredNorm();
-//			}
-//		}//end CalcVarLaplaceApproxStable
-
-		/*!
-		* \brief Calculate variance of Laplace-approximated posterior
-		* \param Sigma Covariance matrix of latent random effect
-		* \param random_effects_indices_of_data Indices that indicate to which random effect every data point is related
-		* \param[out] pred_var Variance of Laplace-approximated posterior
-		*/
-		void CalcVarLaplaceApproxOnlyOneGPCalculationsOnREScale(const std::shared_ptr<T_mat> Sigma,
-			const data_size_t* const random_effects_indices_of_data,
-			vec_t& pred_var) {
-			if (na_or_inf_during_last_call_to_find_mode_) {
-				Log::REFatal(NA_OR_INF_ERROR_);
-			}
-			CHECK(mode_has_been_calculated_);
-			pred_var = vec_t(num_re_);
-			vec_t diag_ZtWZ_sqrt;
-			CalcZtVGivenIndices((data_size_t)second_deriv_neg_ll_.size(), num_re_, random_effects_indices_of_data, second_deriv_neg_ll_, diag_ZtWZ_sqrt, true);
-			diag_ZtWZ_sqrt.array() = diag_ZtWZ_sqrt.array().sqrt();
-			T_mat L_inv_ZtWZ_sqrt_Sigma = diag_ZtWZ_sqrt.asDiagonal() * (*Sigma);
-			TriangularSolveGivenCholesky<T_chol, T_mat, T_mat, T_mat>(chol_fact_Id_plus_Wsqrt_Sigma_Wsqrt_, L_inv_ZtWZ_sqrt_Sigma, L_inv_ZtWZ_sqrt_Sigma, false);
-#pragma omp parallel for schedule(static)
-			for (int i = 0; i < num_re_; ++i) {
-				pred_var[i] = (*Sigma).coeff(i, i) - L_inv_ZtWZ_sqrt_Sigma.col(i).squaredNorm();
-			}
-		}//end CalcVarLaplaceApproxOnlyOneGPCalculationsOnREScale
-
-		/*!
-		* \brief Calculate variance of Laplace-approximated posterior
-		* \param[out] pred_var Variance of Laplace-approximated posterior
-		*/
-		void CalcVarLaplaceApproxGroupedRE(vec_t& pred_var) {
-			if (na_or_inf_during_last_call_to_find_mode_) {
-				Log::REFatal(NA_OR_INF_ERROR_);
-			}
-			CHECK(mode_has_been_calculated_);
-			pred_var = vec_t(num_re_);
-			sp_mat_t L_inv(num_re_, num_re_);
-			L_inv.setIdentity();
-			TriangularSolveGivenCholesky<chol_sp_mat_t, sp_mat_t, sp_mat_t, sp_mat_t>(chol_fact_SigmaI_plus_ZtWZ_grouped_, L_inv, L_inv, false);
-#pragma omp parallel for schedule(static)
-			for (int i = 0; i < num_re_; ++i) {
-				pred_var[i] = L_inv.col(i).squaredNorm();
-			}
-		}//end CalcVarLaplaceApproxGroupedRE
-
-		/*!
-		* \brief Calculate variance of Laplace-approximated posterior
-		* \param[out] pred_var Variance of Laplace-approximated posterior
-		*/
-		void CalcVarLaplaceApproxOnlyOneGroupedRECalculationsOnREScale(vec_t& pred_var) {
-			if (na_or_inf_during_last_call_to_find_mode_) {
-				Log::REFatal(NA_OR_INF_ERROR_);
-			}
-			CHECK(mode_has_been_calculated_);
-			pred_var = vec_t(num_re_);
-			pred_var.array() = diag_SigmaI_plus_ZtWZ_.array().inverse();
-		}//end CalcVarLaplaceApproxOnlyOneGroupedRECalculationsOnREScale
-
-		/*!
-		* \brief Calculate variance of Laplace-approximated posterior
-		* \param[out] pred_var Variance of Laplace-approximated posterior
-		*/
-		void CalcVarLaplaceApproxVecchia(vec_t& pred_var) {
-			if (na_or_inf_during_last_call_to_find_mode_) {
-				Log::REFatal(NA_OR_INF_ERROR_);
-			}
-			CHECK(mode_has_been_calculated_);
-			pred_var = vec_t(num_re_);
-			sp_mat_t L_inv(num_re_, num_re_);
-			L_inv.setIdentity();
-			TriangularSolveGivenCholesky<chol_sp_mat_t, sp_mat_t, sp_mat_t, sp_mat_t>(chol_fact_SigmaI_plus_ZtWZ_vecchia_, L_inv, L_inv, false);
-#pragma omp parallel for schedule(static)
-			for (int i = 0; i < num_re_; ++i) {
-				pred_var[i] = L_inv.col(i).squaredNorm();
-			}
-		}//end CalcVarLaplaceApproxVecchia
-
-		/*!
-		* \brief Make predictions for the response variable (label) based on predictions for the mean and variance of the latent random effects
-		* \param pred_mean[out] Predictive mean of latent random effects. The Predictive mean for the response variables is written on this
-		* \param pred_var[out] Predictive variances of latent random effects. The predicted variance for the response variables is written on this
-		* \param predict_var If true, predictive variances are also calculated
-		*/
-		void PredictResponse(vec_t& pred_mean, 
-			vec_t& pred_var, 
-			bool predict_var) {
-			if (likelihood_type_ == "bernoulli_probit") {
-#pragma omp parallel for schedule(static)
-				for (int i = 0; i < (int)pred_mean.size(); ++i) {
-					pred_mean[i] = normalCDF(pred_mean[i] / std::sqrt(1. + pred_var[i]));
-				}
-				if (predict_var) {
-#pragma omp parallel for schedule(static)
-					for (int i = 0; i < (int)pred_mean.size(); ++i) {
-						pred_var[i] = pred_mean[i] * (1. - pred_mean[i]);
-					}
-				}
-			}
-			else if (likelihood_type_ == "bernoulli_logit") {
-#pragma omp parallel for schedule(static)
-				for (int i = 0; i < (int)pred_mean.size(); ++i) {
-					pred_mean[i] = RespMeanAdaptiveGHQuadrature(pred_mean[i], pred_var[i]);
-				}
-				if (predict_var) {
-#pragma omp parallel for schedule(static)
-					for (int i = 0; i < (int)pred_mean.size(); ++i) {
-						pred_var[i] = pred_mean[i] * (1. - pred_mean[i]);
-					}
-				}
-			}
-			else if (likelihood_type_ == "poisson") {
-#pragma omp parallel for schedule(static)
-				for (int i = 0; i < (int)pred_mean.size(); ++i) {
-					double pm = std::exp(pred_mean[i] + 0.5 * pred_var[i]);
-					//double pm = RespMeanAdaptiveGHQuadrature(pred_mean[i], pred_var[i]);// alternative version using quadrature
-					if (predict_var) {
-						pred_var[i] = pm * ((std::exp(pred_var[i]) - 1.) * pm + 1.);
-						//double psm = RespMeanAdaptiveGHQuadrature(2 * pred_mean[i], 4 * pred_var[i]);// alternative version using quadrature
-						//pred_var[i] = psm - pm * pm + pm;
-					}
-					pred_mean[i] = pm;
-				}
-			}
-			else if (likelihood_type_ == "gamma") {
-#pragma omp parallel for schedule(static)
-				for (int i = 0; i < (int)pred_mean.size(); ++i) {
-					double pm = std::exp(pred_mean[i] + 0.5 * pred_var[i]);
-					//double pm = RespMeanAdaptiveGHQuadrature(pred_mean[i], pred_var[i]);// alternative version using quadrature
-					if (predict_var) {
-						pred_var[i] = (std::exp(pred_var[i]) - 1.) * pm * pm + std::exp(2 * pred_mean[i] + 2 * pred_var[i]) / aux_pars_[0];
-						//double psm = RespMeanAdaptiveGHQuadrature(2 * pred_mean[i], 4 * pred_var[i]);// alternative version using quadrature
-						//pred_var[i] = psm - pm * pm + psm / aux_pars_[0];
-					}
-					pred_mean[i] = pm;
-				}
-			}
-		}//end PredictResponse
-
-		/*!
-		* \brief Adaptive GH quadrature to calculate predictive mean of response variable
-		* \param latent_mean Predictive mean of latent random effects
-		* \param latent_var Predictive variances of latent random effects
-		*/
-		double RespMeanAdaptiveGHQuadrature(const double latent_mean,
-			const double latent_var) {
-			// Find mode of integrand
-			double mode_integrand_last, update;
-			double mode_integrand = 0.;
-			double sigma2_inv = 1. / latent_var;
-			double sqrt_sigma2_inv = std::sqrt(sigma2_inv);
-			for (int it = 0; it < 100; ++it) {
-				mode_integrand_last = mode_integrand;
-				update = (FirstDerivLogCondMeanLikelihood(mode_integrand) - sigma2_inv * (mode_integrand - latent_mean))
-					/ (SecondDerivLogCondMeanLikelihood(mode_integrand) - sigma2_inv);
-				mode_integrand -= update;
-				if (std::abs(update) / std::abs(mode_integrand_last) < DELTA_REL_CONV_) {
-					break;
-				}
-			}
-			// Adaptive GH quadrature
-			double sqrt2_sigma_hat = M_SQRT2 / std::sqrt(-SecondDerivLogCondMeanLikelihood(mode_integrand) + sigma2_inv);
-			double x_val;
-			double mean_resp = 0.;
-			for (int j = 0; j < order_GH_; ++j) {
-				x_val = sqrt2_sigma_hat * GH_nodes_[j] + mode_integrand;
-				mean_resp += adaptive_GH_weights_[j] * CondMeanLikelihood(x_val) * normalPDF(sqrt_sigma2_inv * (x_val - latent_mean));
-			}
-			mean_resp *= sqrt2_sigma_hat * sqrt_sigma2_inv;
-			return mean_resp;
-		}//end RespMeanAdaptiveGHQuadrature
-
-		/*!
-		* \brief Calculate test negative log-likelihood using adaptive GH quadrature
-		* \param y_test Test response variable
-		* \param pred_mean Predictive mean of latent random effects
-		* \param pred_var Predictive variances of latent random effects
-		* \param num_data Number of data points
-		*/
-		inline double TestNegLogLikelihoodAdaptiveGHQuadrature(const label_t* y_test,
-			const double* pred_mean,
-			const double* pred_var,
-			const data_size_t num_data) const {
-			double ll = 0.;
-#pragma omp parallel for schedule(static) if (num_data >= 128) reduction(+:ll)
-			for (data_size_t i = 0; i < num_data; ++i) {
-				int y_test_int = 1;
-				double y_test_d = static_cast<double>(y_test[i]);
-// Note: we need to convert from float to double as label_t is float. Unfortunately, the lightGBM part does not allow for setting the LABEL_T_USE_DOUBLE macro in meta.h (multiple bugs...)
-				if (label_type() == "int") {
-					y_test_int = static_cast<int>(y_test[i]);
-				}
-				// Find mode of integrand
-				double mode_integrand_last, update;
-				double mode_integrand = 0.;
-				double sigma2_inv = 1. / pred_var[i];
-				double sqrt_sigma2_inv = std::sqrt(sigma2_inv);
-				for (int it = 0; it < 100; ++it) {
-					mode_integrand_last = mode_integrand;
-					update = (CalcFirstDerivLogLik(y_test_d, y_test_int, mode_integrand) - sigma2_inv * (mode_integrand - pred_mean[i]))
-						/ (-CalcSecondDerivNegLogLik(y_test_d, y_test_int, mode_integrand) - sigma2_inv);
-					mode_integrand -= update;
-					if (std::abs(update) / std::abs(mode_integrand_last) < DELTA_REL_CONV_) {
-						break;
-					}
-				}
-				// Adaptive GH quadrature
-				double sqrt2_sigma_hat = M_SQRT2 / std::sqrt(CalcSecondDerivNegLogLik(y_test_d, y_test_int, mode_integrand) + sigma2_inv);
-				double x_val;
-				double likelihood = 0.;
-				for (int j = 0; j < order_GH_; ++j) {
-					x_val = sqrt2_sigma_hat * GH_nodes_[j] + mode_integrand;
-					likelihood += adaptive_GH_weights_[j] * std::exp(LogLikelihood(y_test_d, y_test_int, x_val)) * normalPDF(sqrt_sigma2_inv * (x_val - pred_mean[i]));
-				}
-				likelihood *= sqrt2_sigma_hat * sqrt_sigma2_inv;
-				ll += std::log(likelihood);
-			}
-			return -ll;
-		}//end TestNegLogLikelihoodAdaptiveGHQuadrature
-
-		/*! \brief Set matrix inversion properties and choices for iterative methods. This function is calle from re_model_template.h which also holds these variables */
-		void SetMatrixInversionProperties(const string_t& matrix_inversion_method,
-			int cg_max_num_it,
-			int cg_max_num_it_tridiag,
-			double cg_delta_conv,
-			int num_rand_vec_trace,
-			bool reuse_rand_vec_trace,
-			int seed_rand_vec_trace,
-			const string_t& cg_preconditioner_type,
-			int piv_chol_rank,
-			int rank_pred_approx_matrix_lanczos) {
-			matrix_inversion_method_ = matrix_inversion_method;
-			cg_max_num_it_ = cg_max_num_it;
-			cg_max_num_it_tridiag_ = cg_max_num_it_tridiag;
-			cg_delta_conv_ = cg_delta_conv;
-			num_rand_vec_trace_ = num_rand_vec_trace;
-			reuse_rand_vec_trace_ = reuse_rand_vec_trace;
-			seed_rand_vec_trace_ = seed_rand_vec_trace;
-			cg_preconditioner_type_ = cg_preconditioner_type;
-			piv_chol_rank_ = piv_chol_rank;
-			rank_pred_approx_matrix_lanczos_ = rank_pred_approx_matrix_lanczos;
-		}//end SetMatrixInversionProperties
-
-		static string_t ParseLikelihoodAlias(const string_t& likelihood) {
-			if (likelihood == string_t("binary") || likelihood == string_t("bernoulli_probit") || likelihood == string_t("binary_probit")) {
-				return "bernoulli_probit";
-			}
-			else if (likelihood == string_t("bernoulli_logit") || likelihood == string_t("binary_logit")) {
-				return "bernoulli_logit";
-			}
-			else if (likelihood == string_t("gaussian") || likelihood == string_t("regression")) {
-				return "gaussian";
-			}
-			return likelihood;
-		}
-
-	private:
-		/*! \brief Number of data points */
-		data_size_t num_data_;
-		/*! \brief Number (dimension) of random effects (= length of mode_) */
-		data_size_t num_re_;
-		/*! \brief Posterior mode used for Laplace approximation */
-		vec_t mode_;
-		/*! \brief Saving a previously found value allows for reseting the mode when having a too large step size. */
-		vec_t mode_previous_value_;
-		/*! \brief Auxiliary variable a=ZSigmaZt^-1 mode_b used for Laplace approximation */
-		vec_t a_vec_;
-		/*! \brief Saving a previously found value allows for reseting the mode when having a too large step size. */
-		vec_t a_vec_previous_value_;
-		/*! \brief Indicates whether the vector a_vec_ / a=ZSigmaZt^-1 is used or not */
-		bool has_a_vec_;
-		/*! \brief First derivatives of the log-likelihood */
-		vec_t first_deriv_ll_;
-		/*! \brief Second derivatives of the negative log-likelihood (diagonal of matrix "W") */
-		vec_t second_deriv_neg_ll_;
-		/*! \brief Diagonal of matrix Sigma^-1 + Zt * W * Z in Laplace approximation (used only in version 'GroupedRE' when there is only one random effect and ZtWZ is diagonal. Otherwise 'diag_SigmaI_plus_ZtWZ_' is used for grouped REs) */
-		vec_t diag_SigmaI_plus_ZtWZ_;
-		/*! \brief Cholesky factors of matrix Sigma^-1 + Zt * W * Z in Laplace approximation (used only in version'GroupedRE' if there is more than one random effect). */
-		chol_sp_mat_t chol_fact_SigmaI_plus_ZtWZ_grouped_;
-		/*! \brief Cholesky factors of matrix Sigma^-1 + Zt * W * Z in Laplace approximation (used only in version 'Vecchia') */
-		chol_sp_mat_t chol_fact_SigmaI_plus_ZtWZ_vecchia_;
-		/*! 
-		* \brief Cholesky factors of matrix B = I + Wsqrt *  Z * Sigma * Zt * Wsqrt in Laplace approximation (for version 'Stable') 
-		*		or of matrix B = Id + ZtWZsqrt * Sigma * ZtWZsqrt (for version 'OnlyOneGPCalculationsOnREScale')
-		*/
-		T_chol chol_fact_Id_plus_Wsqrt_Sigma_Wsqrt_;
-		/*! \brief If true, the pattern for the Cholesky factor (chol_fact_Id_plus_Wsqrt_Sigma_Wsqrt_, chol_fact_SigmaI_plus_ZtWZ_grouped_, or chol_fact_SigmaI_plus_ZtWZ_vecchia_) has been analyzed */
-		bool chol_fact_pattern_analyzed_ = false;
-		/*! \brief If true, the mode has been initialized to 0 */
-		bool mode_initialized_ = false;
-		/*! \brief If true, the mode has been determined */
-		bool mode_has_been_calculated_ = false;
-		/*! \brief If true, NA or Inf has occurred during the last call to find mode */
-		bool na_or_inf_during_last_call_to_find_mode_ = false;
-		/*! \brief If true, NA or Inf has occurred during the second last call to find mode when mode_previous_value_ was calculated */
-		bool na_or_inf_during_second_last_call_to_find_mode_ = false;
-		/*! \brief Normalizing constant of the log-likelihood (not all likelihoods have one) */
-		double log_normalizing_constant_;
-		/*! \brief If true, the function 'CalculateLogNormalizingConstant' has been called */
-		bool normalizing_constant_has_been_calculated_ = false;
-		/*! \brief Auxiliary quantities that do not depend on aux_pars_ for normalizing constant for likelihoods (not all likelihoods have one, for gamma this is sum( log(y) ) ) */
-		double aux_log_normalizing_constant_;
-		/*! \brief If true, the function 'CalculateAuxQuantLogNormalizingConstant' has been called */
-		bool aux_normalizing_constant_has_been_calculated_ = false;
-
-		/*! \brief Type of likelihood  */
-		string_t likelihood_type_ = "gaussian";
-		/*! \brief List of supported covariance likelihoods */
-		const std::set<string_t> SUPPORTED_LIKELIHOODS_{ "gaussian", "bernoulli_probit", "bernoulli_logit", "poisson", "gamma" };
-		/*! \brief Maximal number of iteration done for finding posterior mode with Newton's method */
-		int MAXIT_MODE_NEWTON_ = 1000;
-		/*! \brief Used for checking convergence in mode finding algorithm (terminate if relative change in Laplace approx. is below this value) */
-		double DELTA_REL_CONV_ = 1e-6;
-		/*! \brief Number of additional parameters for likelihoods  */
-		int num_aux_pars_;
-		/*! \brief Additional parameters for likelihoods. For "gamma", aux_pars_[0] = shape parameter, for gaussian, aux_pars_[0] = 1 / sqrt(variance) */
-		std::vector<double> aux_pars_;
-		/*! \brief Names of additional parameters for likelihoods */
-		std::vector<string_t> names_aux_pars_;
-		/*! \brief True, if the function 'SetAuxPars' has been called */
-		bool aux_pars_have_been_set_ = false;
-
-		// MATRIX INVERSION PROPERTIES
-		/*! \brief Matrix inversion method */
-		string_t matrix_inversion_method_ = "cholesky";
-		/*! \brief Maximal number of iterations for conjugate gradient algorithm */
-		int cg_max_num_it_ = 1000;
-		/*! \brief Maximal number of iterations for conjugate gradient algorithm when being run as Lanczos algorithm for tridiagonalization */
-		int cg_max_num_it_tridiag_ = 1000;
-		/*! \brief Tolerance level for L2 norm of residuals for checking convergence in conjugate gradient algorithm when being used for parameter estimation */
-		double cg_delta_conv_ = 1e-3;
-		/*! \brief Number of random vectors (e.g. Rademacher) for stochastic approximation of the trace of a matrix */
-		int num_rand_vec_trace_ = 50;
-		/*! \brief If true, random vectors (e.g. Rademacher) for stochastic approximation of the trace of a matrix are sampled only once at the beginning and then reused in later trace approximations, otherwise they are sampled everytime a trace is calculated */
-		bool reuse_rand_vec_trace_ = true;
-		/*! \brief Seed number to generate random vectors (e.g. Rademacher) */
-		int seed_rand_vec_trace_ = 1;
-		/*! \brief Type of preconditoner used for the conjugate gradient algorithm */
-		string_t cg_preconditioner_type_ = "Sigma_inv_plus_BtWB";
-		/*! \brief Rank of the pivoted Cholesky decomposition used as preconditioner in conjugate gradient algorithms */
-		int piv_chol_rank_ = 50;
-		/*! \brief Rank of the matrix for approximating predictive covariance matrices obtained using the Lanczos algorithm */
-		int rank_pred_approx_matrix_lanczos_ = 1000;
-		/*! \brief If true, cg_max_num_it and cg_max_num_it_tridiag are reduced by 2/3 (multiplied by 1/3) for the mode finding of the Laplace approximation in the first gradient step when finding a learning rate that reduces the ll */
-		bool reduce_cg_max_num_it_first_optim_step_ = true;
-
-		/*! \brief Order of the Gauss-Hermite quadrature */
-		int order_GH_ = 30;
-		/*! \brief Nodes and weights for the Gauss-Hermite quadrature */
-		// Source: https://keisan.casio.com/exec/system/1281195844
-		const std::vector<double> GH_nodes_ = { -6.863345293529891581061,
-										-6.138279220123934620395,
-										-5.533147151567495725118,
-										-4.988918968589943944486,
-										-4.48305535709251834189,
-										-4.003908603861228815228,
-										-3.544443873155349886925,
-										-3.099970529586441748689,
-										-2.667132124535617200571,
-										-2.243391467761504072473,
-										-1.826741143603688038836,
-										-1.415527800198188511941,
-										-1.008338271046723461805,
-										-0.6039210586255523077782,
-										-0.2011285765488714855458,
-										0.2011285765488714855458,
-										0.6039210586255523077782,
-										1.008338271046723461805,
-										1.415527800198188511941,
-										1.826741143603688038836,
-										2.243391467761504072473,
-										2.667132124535617200571,
-										3.099970529586441748689,
-										3.544443873155349886925,
-										4.003908603861228815228,
-										4.48305535709251834189,
-										4.988918968589943944486,
-										5.533147151567495725118,
-										6.138279220123934620395,
-										6.863345293529891581061 };
-		const std::vector<double> GH_weights_ = { 2.908254700131226229411E-21,
-										2.8103336027509037088E-17,
-										2.87860708054870606219E-14,
-										8.106186297463044204E-12,
-										9.1785804243785282085E-10,
-										5.10852245077594627739E-8,
-										1.57909488732471028835E-6,
-										2.9387252289229876415E-5,
-										3.48310124318685523421E-4,
-										0.00273792247306765846299,
-										0.0147038297048266835153,
-										0.0551441768702342511681,
-										0.1467358475408900997517,
-										0.2801309308392126674135,
-										0.386394889541813862556,
-										0.3863948895418138625556,
-										0.2801309308392126674135,
-										0.1467358475408900997517,
-										0.0551441768702342511681,
-										0.01470382970482668351528,
-										0.002737922473067658462989,
-										3.48310124318685523421E-4,
-										2.938725228922987641501E-5,
-										1.579094887324710288346E-6,
-										5.1085224507759462774E-8,
-										9.1785804243785282085E-10,
-										8.10618629746304420399E-12,
-										2.87860708054870606219E-14,
-										2.81033360275090370876E-17,
-										2.9082547001312262294E-21 };
-		const std::vector<double> adaptive_GH_weights_ = { 0.83424747101276179534,
-										0.64909798155426670071,
-										0.56940269194964050397,
-										0.52252568933135454964,
-										0.491057995832882696506,
-										0.46837481256472881677,
-										0.45132103599118862129,
-										0.438177022652683703695,
-										0.4279180629327437485828,
-										0.4198950037368240886418,
-										0.413679363611138937184,
-										0.4089815750035316024972,
-										0.4056051233256844363121,
-										0.403419816924804022553,
-										0.402346066701902927115,
-										0.4023460667019029271154,
-										0.4034198169248040225528,
-										0.4056051233256844363121,
-										0.4089815750035316024972,
-										0.413679363611138937184,
-										0.4198950037368240886418,
-										0.427918062932743748583,
-										0.4381770226526837037,
-										0.45132103599118862129,
-										0.46837481256472881677,
-										0.4910579958328826965056,
-										0.52252568933135454964,
-										0.56940269194964050397,
-										0.64909798155426670071,
-										0.83424747101276179534 };
-
-		const char* NA_OR_INF_WARNING_ = "Mode finding algorithm for Laplace approximation: NA or Inf occurred. "
-			"This is not necessary a problem as it might have been the cause of a too large learning rate which, "
-			"consequently, might have been decreased by the optimization algorithm ";
-		const char* NA_OR_INF_ERROR_ = "NA or Inf occurred in the mode finding algorithm for the Laplace approximation ";
-		const char* NO_INCREASE_IN_MLL_WARNING_ = "Mode finding algorithm for Laplace approximation: "
-			"The approximate marginal log-likelihood (=convergence criterion) has decreased and the algorithm has thus been terminated ";
-		const char* NO_CONVERGENCE_WARNING_ = "Algorithm for finding mode for Laplace approximation has not "
-			"converged after the maximal number of iterations ";
-
-	};//end class Likelihood
-
-}  // namespace GPBoost
-
-#endif   // GPB_LIKELIHOODS_
+/*!
+* This file is part of GPBoost a C++ library for combining
+*	boosting with Gaussian process and mixed effects models
+*
+* Copyright (c) 2020 Fabio Sigrist. All rights reserved.
+*
+* Licensed under the Apache License Version 2.0. See LICENSE file in the project root for license information.
+*
+*
+*  EXPLANATIONS ON PARAMETERIZATIONS USED
+*
+* For a "gamma" likelihood, the following density is used:
+*	f(y) = lambda^gamma / Gamma(gamma) * y^(gamma - 1) * exp(-lambda * y)
+*		- lambda = gamma * exp(-location_par) (i.e., mean(y) = exp(location_par)
+*		- lambda = rate parameter, gamma = shape parameter, location_par = random plus fixed effects
+*
+*/
+#ifndef GPB_LIKELIHOODS_
+#define GPB_LIKELIHOODS_
+
+#define _USE_MATH_DEFINES // for M_SQRT1_2 and M_PI
+#include <cmath>
+
+#include <GPBoost/type_defs.h>
+#include <GPBoost/sparse_matrix_utils.h>
+#include <GPBoost/DF_utils.h>
+#include <GPBoost/utils.h>
+
+#include <string>
+#include <set>
+#include <string>
+#include <vector>
+
+#include <LightGBM/utils/log.h>
+using LightGBM::Log;
+#include <LightGBM/meta.h>
+using LightGBM::label_t;
+
+//Mathematical constants usually defined in cmath
+#ifndef M_SQRT2
+#define M_SQRT2      1.414213562373095048801688724209698079 //sqrt(2)
+#endif
+
+#include <chrono>  // only for debugging
+#include <thread> // only for debugging
+
+namespace GPBoost {
+
+	// Forward declaration
+	template<typename T_mat, typename T_chol>
+	class REModelTemplate;
+
+	/*!
+	* \brief This class implements the likelihoods for the Gaussian proceses
+	* The template parameters <T_mat, T_chol> can be <den_mat_t, chol_den_mat_t> , <sp_mat_t, chol_sp_mat_t>, <sp_mat_rm_t, chol_sp_mat_rm_t>
+	*/
+	template<typename T_mat, typename T_chol>
+	class Likelihood {
+	public:
+		/*! \brief Constructor */
+		Likelihood();
+
+		/*!
+		* \brief Constructor
+		* \param type Type of likelihood
+		* \param num_data Number of data points
+		* \param num_re Number of random effects
+		* \param Indicates whether the vector a_vec_ / a=ZSigmaZt^-1 is used or not
+		*/
+		Likelihood(string_t type,
+			data_size_t num_data,
+			data_size_t num_re,
+			bool has_a_vec) {
+			string_t likelihood = ParseLikelihoodAlias(type);
+			likelihood = ParseLikelihoodAliasGradientDescent(likelihood);
+			if (SUPPORTED_LIKELIHOODS_.find(likelihood) == SUPPORTED_LIKELIHOODS_.end()) {
+				Log::REFatal("Likelihood of type '%s' is not supported.", likelihood.c_str());
+			}
+			likelihood_type_ = likelihood;
+			num_data_ = num_data;
+			num_re_ = num_re;
+			num_aux_pars_ = 0;
+			if (likelihood_type_ == "gamma") {
+				aux_pars_ = { 1. };//shape parameter
+				names_aux_pars_ = { "shape" };
+				num_aux_pars_ = 1;
+			}
+			else if (likelihood_type_ == "gaussian") {
+				aux_pars_ = { 1. };//1 / sqrt(variance)
+				names_aux_pars_ = { "inverse_std_dev" };
+			}
+			chol_fact_pattern_analyzed_ = false;
+			has_a_vec_ = has_a_vec;
+			DetermineWhetherToCapChangeModeNewton();
+		}
+
+		/*!
+		* \brief Determine cap_change_mode_newton_
+		*/
+		void DetermineWhetherToCapChangeModeNewton() {
+			if (likelihood_type_ == "gamma" || likelihood_type_ == "poisson") {
+				cap_change_mode_newton_ = true;
+			}
+			else {
+				cap_change_mode_newton_ = false;
+			}
+		}
+
+		/*!
+		* \brief Initialize mode vector_ (used in Laplace approximation for non-Gaussian data)
+		*/
+		void InitializeModeAvec() {
+			mode_ = vec_t::Zero(num_re_);
+			mode_previous_value_ = vec_t::Zero(num_re_);
+			if (has_a_vec_) {
+				a_vec_ = vec_t::Zero(num_re_);
+				a_vec_previous_value_ = vec_t::Zero(num_re_);
+			}
+			mode_initialized_ = true;
+			first_deriv_ll_ = vec_t(num_data_);
+			second_deriv_neg_ll_ = vec_t(num_data_);
+			mode_has_been_calculated_ = false;
+			na_or_inf_during_last_call_to_find_mode_ = false;
+			na_or_inf_during_second_last_call_to_find_mode_ = false;
+		}
+
+		/*!
+		* \brief Reset mode to previous value. This is used if too large step-sizes are done which result in increases in the objective function.
+		"			The values (covariance parameters and linear coefficients) are then discarded and consequently the mode should also be reset to the previous value)
+		*/
+		void ResetModeToPreviousValue() {
+			CHECK(mode_initialized_);
+			mode_ = mode_previous_value_;
+			if (has_a_vec_) {
+				a_vec_ = a_vec_previous_value_;
+			}
+			na_or_inf_during_last_call_to_find_mode_ = na_or_inf_during_second_last_call_to_find_mode_;
+		}
+
+		/*! \brief Destructor */
+		~Likelihood() {
+		}
+
+		/*!
+		* \brief Returns the type of likelihood
+		*/
+		string_t GetLikelihood() const {
+			return(likelihood_type_);
+		}
+
+		/*!
+		* \brief Set the type of likelihood
+		* \param type Likelihood name
+		*/
+		void SetLikelihood(const string_t& type) {
+			string_t likelihood = ParseLikelihoodAlias(type);
+			likelihood = ParseLikelihoodAliasGradientDescent(likelihood);
+			if (SUPPORTED_LIKELIHOODS_.find(likelihood) == SUPPORTED_LIKELIHOODS_.end()) {
+				Log::REFatal("Likelihood of type '%s' is not supported.", likelihood.c_str());
+			}
+			likelihood_type_ = likelihood;
+			chol_fact_pattern_analyzed_ = false;
+			DetermineWhetherToCapChangeModeNewton();
+		}
+
+		/*!
+		* \brief Returns the type of the response variable (label). Either "double" or "int"
+		*/
+		string_t label_type() const {
+			if (likelihood_type_ == "bernoulli_probit" || likelihood_type_ == "bernoulli_logit" ||
+				likelihood_type_ == "poisson") {
+				return("int");
+			}
+			else {
+				return("double");
+			}
+		}
+
+		/*!
+		* \brief Returns a pointer to mode_
+		*/
+		const vec_t* GetMode() const {
+			return(&mode_);
+		}
+
+		/*!
+		* \brief Returns a pointer to first_deriv_ll_
+		*/
+		const vec_t* GetFirstDerivLL() const {
+			return(&first_deriv_ll_);
+		}
+
+		/*!
+		* \brief Checks whether the response variables (labels) have the correct values
+		* \param y_data Response variable data
+		* \param num_data Number of data points
+		*/
+		template <typename T>//T can be double or float
+		void CheckY(const T* y_data,
+			const data_size_t num_data) const {
+			if (likelihood_type_ == "bernoulli_probit" || likelihood_type_ == "bernoulli_logit") {
+				//#pragma omp parallel for schedule(static)//problematic with error message below... 
+				for (data_size_t i = 0; i < num_data; ++i) {
+					if (fabs(y_data[i]) >= EPSILON_NUMBERS && !TwoNumbersAreEqual<T>(y_data[i], 1.)) {
+						Log::REFatal("Response variable (label) data needs to be 0 or 1 for likelihood of type '%s' ", likelihood_type_.c_str());
+					}
+				}
+			}
+			else if (likelihood_type_ == "poisson") {
+				for (data_size_t i = 0; i < num_data; ++i) {
+					if (y_data[i] < 0) {
+						Log::REFatal("Found negative response variable. Response variable cannot be negative for likelihood of type '%s' ", likelihood_type_.c_str());
+					}
+					else {
+						double intpart;
+						if (std::modf(y_data[i], &intpart) != 0.0) {
+							Log::REFatal("Found non-integer response variable. Response variable can only be integer valued for likelihood of type '%s' ", likelihood_type_.c_str());
+						}
+					}
+				}
+			}
+			else if (likelihood_type_ == "gamma") {
+				for (data_size_t i = 0; i < num_data; ++i) {
+					if (y_data[i] < 0) {
+						Log::REFatal("Found negative response variable. Response variable cannot be negative for likelihood of type '%s' ", likelihood_type_.c_str());
+					}
+				}
+			}
+			else {
+				Log::REFatal("GPModel: Likelihood of type '%s' is not supported ", likelihood_type_.c_str());
+			}
+		}//end CheckY
+
+		/*!
+		* \brief Determine initial value for intercept (=constant)
+		* \param y_data Response variable data
+		* \param num_data Number of data points
+		* param rand_eff_var Variance of random effects
+		*/
+		double FindInitialIntercept(const double* y_data,
+			const data_size_t num_data,
+			double rand_eff_var) const {
+			CHECK(rand_eff_var > 0.);
+			double init_intercept = 0.;
+			if (likelihood_type_ == "gaussian") {
+#pragma omp parallel for schedule(static) reduction(+:init_intercept)
+				for (data_size_t i = 0; i < num_data; ++i) {
+					init_intercept += y_data[i];
+				}
+				init_intercept /= num_data;
+			}
+			else if (likelihood_type_ == "bernoulli_probit" || likelihood_type_ == "bernoulli_logit") {
+				double pavg = 0.;
+#pragma omp parallel for schedule(static) reduction(+:pavg)
+				for (data_size_t i = 0; i < num_data; ++i) {
+					pavg += bool(y_data[i] > 0);
+				}
+				pavg /= num_data;
+				pavg = std::min(pavg, 1.0 - 1e-15);
+				pavg = std::max<double>(pavg, 1e-15);
+				if (likelihood_type_ == "bernoulli_logit") {
+					init_intercept = std::log(pavg / (1.0 - pavg));
+				}
+				else {
+					init_intercept = normalQF(pavg);
+				}
+			}
+			else if (likelihood_type_ == "poisson" || likelihood_type_ == "gamma") {
+				double avg = 0.;
+#pragma omp parallel for schedule(static) reduction(+:avg)
+				for (data_size_t i = 0; i < num_data; ++i) {
+					avg += y_data[i];
+				}
+				avg /= num_data;
+				init_intercept = SafeLog(avg) - 0.5 * rand_eff_var; // log-normal distribution: mean of exp(beta_0 + Zb) = exp(beta_0 + 0.5 * sigma^2) => use beta_0 = mean(y) - 0.5 * sigma^2
+			}
+			else {
+				Log::REFatal("FindInitialIntercept: Likelihood of type '%s' is not supported.", likelihood_type_.c_str());
+			}
+			return(init_intercept);
+		}//end FindInitialIntercept
+
+		/*!
+		* \brief Determine initial value for intercept (=constant)
+		* \param y_data Response variable data
+		* \param num_data Number of data points
+		* \param rand_eff_var Variance of random effects
+		*/
+		bool ShouldHaveIntercept(const double* y_data,
+			const data_size_t num_data,
+			double rand_eff_var) const {
+			bool ret_val = false;
+			if (likelihood_type_ == "poisson" || likelihood_type_ == "gamma") {
+				ret_val = true;
+			}
+			else {
+				double beta_zero = FindInitialIntercept(y_data, num_data, rand_eff_var);
+				if (std::abs(beta_zero) > 0.1) {
+					ret_val = true;
+				}
+			}
+			return(ret_val);
+		}
+
+		/*!
+		* \brief Determine initial value for additional likelihood parameters (e.g., shape for gamma)
+		* \param y_data Response variable data
+		* \param num_data Number of data points
+		*/
+		const double* FindInitialAuxPars(const double* y_data,
+			const data_size_t num_data) {
+			if (likelihood_type_ == "gamma") {
+				// Use a simple "MLE" approach for the shape parameter ignoring random and fixed effects and 
+				//	using the approximation: ln(k) - digamma(k) approx = (1 + 1 / (6k + 1)) / (2k), where k = shape
+				//	See https://en.wikipedia.org/wiki/Gamma_distribution#Maximum_likelihood_estimation (as of 02.03.2023)
+				double log_avg = 0., avg_log = 0.;
+#pragma omp parallel for schedule(static) reduction(+:log_avg, avg_log)
+				for (data_size_t i = 0; i < num_data; ++i) {
+					log_avg += y_data[i];
+					avg_log += std::log(y_data[i]);
+				}
+				log_avg /= num_data;
+				log_avg = std::log(log_avg);
+				avg_log /= num_data;
+				double s = log_avg - avg_log;
+				aux_pars_[0] = (3. - s + std::sqrt((s - 3.) * (s - 3.) + 24. * s)) / (12. * s);
+			}
+			else if (likelihood_type_ != "gaussian" && likelihood_type_ != "bernoulli_probit" &&
+				likelihood_type_ != "bernoulli_logit" && likelihood_type_ != "poisson") {
+				Log::REFatal("FindInitialAuxPars: Likelihood of type '%s' is not supported ", likelihood_type_.c_str());
+			}
+			return(aux_pars_.data());
+		}//end FindInitialAuxPars
+
+		/*!
+		* \brief Returns the number of additional parameters
+		*/
+		int NumAuxPars() const {
+			return(num_aux_pars_);
+		}
+
+		/*!
+		* \brief Returns a pointer to aux_pars_
+		*/
+		const double* GetAuxPars() const {
+			return(aux_pars_.data());
+		}
+
+		/*!
+		* \brief Set aux_pars_
+		* \param aux_pars New values for aux_pars_
+		*/
+		void SetAuxPars(const double* aux_pars) {
+			if (likelihood_type_ == "gamma") {
+				CHECK(aux_pars[0] > 0);
+				aux_pars_[0] = aux_pars[0];
+			}
+			else if (likelihood_type_ == "gaussian") {
+				CHECK(aux_pars[0] > 0);
+				aux_pars_[0] = aux_pars[0];
+			}
+			normalizing_constant_has_been_calculated_ = false;
+			aux_pars_have_been_set_ = true;
+		}
+
+		const char* GetNameAuxPars(int ind_aux_par) const {
+			CHECK(ind_aux_par < num_aux_pars_);
+			return(names_aux_pars_[ind_aux_par].c_str());
+		}
+
+		void GetNameFirstAuxPar(string_t& name) const {
+			name = names_aux_pars_[0];
+		}
+
+		bool AuxParsHaveBeenSet() const {
+			return(aux_pars_have_been_set_);
+		}
+
+		/*!
+		* \brief Calculate auxiliary quantity for the logarithm of normalizing constant of the likelihood
+		* \param y_data Response variable data if response variable is continuous
+		* \param y_data_int Response variable data if response variable is integer-valued
+		* \param num_data Number of data points
+		*/
+		void CalculateAuxQuantLogNormalizingConstant(const double* y_data,
+			const int*,
+			const data_size_t num_data) {
+			if (!aux_normalizing_constant_has_been_calculated_) {
+				if (likelihood_type_ == "gamma") {
+					double log_aux_normalizing_constant = 0.;
+#pragma omp parallel for schedule(static) reduction(+:log_aux_normalizing_constant)
+					for (data_size_t i = 0; i < num_data; ++i) {
+						log_aux_normalizing_constant += AuxQuantLogNormalizingConstantGamma(y_data[i]);
+					}
+					aux_log_normalizing_constant_ = log_aux_normalizing_constant;
+				}
+				else if (likelihood_type_ != "gaussian" && likelihood_type_ != "bernoulli_probit" &&
+					likelihood_type_ != "bernoulli_logit" && likelihood_type_ != "poisson") {
+					Log::REFatal("CalculateAuxQuantLogNormalizingConstant: Likelihood of type '%s' is not supported ", likelihood_type_.c_str());
+				}
+				aux_normalizing_constant_has_been_calculated_ = true;
+			}
+		}//end CalculateAuxQuantLogNormalizingConstant
+
+		inline double AuxQuantLogNormalizingConstantGamma(const double y) const {
+			return(std::log(y));
+		}
+
+		/*!
+		* \brief Calculate the logarithm of the normalizing constant of the likelihood
+		* \param y_data Response variable data if response variable is continuous
+		* \param y_data_int Response variable data if response variable is integer-valued
+		* \param num_data Number of data points
+		*/
+		void CalculateLogNormalizingConstant(const double* y_data,
+			const int* y_data_int,
+			const data_size_t num_data) {
+			if (!normalizing_constant_has_been_calculated_) {
+				CalculateAuxQuantLogNormalizingConstant(y_data, y_data_int, num_data);
+				if (likelihood_type_ == "poisson") {
+					double aux_const = 0.;
+#pragma omp parallel for schedule(static) if (num_data >= 128) reduction(+:aux_const)
+					for (data_size_t i = 0; i < num_data; ++i) {
+						aux_const += LogNormalizingConstantPoisson(y_data_int[i]);
+					}
+					log_normalizing_constant_ = aux_const;
+				}
+				else if (likelihood_type_ == "gamma") {
+					log_normalizing_constant_ = LogNormalizingConstantGamma(1., num_data, false);//note: the first argument is not used
+				}
+				else if (likelihood_type_ != "gaussian" && likelihood_type_ != "bernoulli_probit" &&
+					likelihood_type_ != "bernoulli_logit") {
+					Log::REFatal("CalculateLogNormalizingConstant: Likelihood of type '%s' is not supported ", likelihood_type_.c_str());
+				}
+				normalizing_constant_has_been_calculated_ = true;
+			}
+		}//end CalculateLogNormalizingConstant
+
+		inline double LogNormalizingConstantPoisson(const int y) const {
+			if (y > 1) {
+				double log_factorial = 0.;
+				for (int k = 2; k <= y; ++k) {
+					log_factorial += std::log(k);
+				}
+				return(-log_factorial);
+			}
+			else {
+				return(0.);
+			}
+		}
+
+		inline double LogNormalizingConstantGamma(const double y, const int num_data, bool calculate_aux_const) const {
+			if (TwoNumbersAreEqual<double>(aux_pars_[0], 1.)) {
+				return(0.);
+			}
+			else {
+				if (calculate_aux_const) {
+					return((aux_pars_[0] - 1.) * AuxQuantLogNormalizingConstantGamma(y) +
+						num_data * (aux_pars_[0] * std::log(aux_pars_[0]) - std::lgamma(aux_pars_[0])));
+				}
+				else {
+					return((aux_pars_[0] - 1.) * aux_log_normalizing_constant_ +
+						num_data * (aux_pars_[0] * std::log(aux_pars_[0]) - std::lgamma(aux_pars_[0])));
+				}
+			}
+		}
+
+		/*!
+		* \brief Evaluate the log-likelihood conditional on the latent variable (=location_par)
+		* \param y_data Response variable data if response variable is continuous
+		* \param y_data_int Response variable data if response variable is integer-valued
+		* \param location_par Location parameter (random plus fixed effects)
+		* \param num_data Number of data points
+		*/
+		double LogLikelihood(const double* y_data,
+			const int* y_data_int,
+			const double* location_par,
+			const data_size_t num_data) {
+			CalculateLogNormalizingConstant(y_data, y_data_int, num_data);
+			double ll = 0.;
+			if (likelihood_type_ == "bernoulli_probit") {
+#pragma omp parallel for schedule(static) if (num_data >= 128) reduction(+:ll)
+				for (data_size_t i = 0; i < num_data; ++i) {
+					ll += LogLikBernoulliProbit(y_data_int[i], location_par[i]);
+				}
+			}
+			else if (likelihood_type_ == "bernoulli_logit") {
+#pragma omp parallel for schedule(static) if (num_data >= 128) reduction(+:ll)
+				for (data_size_t i = 0; i < num_data; ++i) {
+					ll += LogLikBernoulliLogit(y_data_int[i], location_par[i]);
+				}
+			}
+			else if (likelihood_type_ == "poisson") {
+#pragma omp parallel for schedule(static) if (num_data >= 128) reduction(+:ll)
+				for (data_size_t i = 0; i < num_data; ++i) {
+					ll += LogLikPoisson(y_data_int[i], location_par[i], false);
+				}
+				ll += log_normalizing_constant_;
+			}
+			else if (likelihood_type_ == "gamma") {
+#pragma omp parallel for schedule(static) if (num_data >= 128) reduction(+:ll)
+				for (data_size_t i = 0; i < num_data; ++i) {
+					ll += LogLikGamma(y_data[i], location_par[i], false);
+				}
+				ll += log_normalizing_constant_;
+			}
+			else if (likelihood_type_ == "gaussian") {
+#pragma omp parallel for schedule(static) if (num_data >= 128) reduction(+:ll)
+				for (data_size_t i = 0; i < num_data; ++i) {
+					ll += LogLikGaussian(y_data[i], location_par[i]);
+				}
+			}
+			else {
+				Log::REFatal("LogLikelihood: Likelihood of type '%s' is not supported.", likelihood_type_.c_str());
+			}
+			return(ll);
+		}//end LogLikelihood
+
+		/*!
+		* \brief Evaluate the log-likelihood conditional on the latent variable (=location_par)
+		* \param y_data Response variable data if response variable is continuous
+		* \param y_data_int Response variable data if response variable is integer-valued
+		* \param location_par Location parameter (random plus fixed effects)
+		*/
+		inline double LogLikelihood(const double y_data,
+			const int y_data_int,
+			const double location_par) const {
+			if (likelihood_type_ == "bernoulli_probit") {
+				return(LogLikBernoulliProbit(y_data_int, location_par));
+			}
+			else if (likelihood_type_ == "bernoulli_logit") {
+				return(LogLikBernoulliLogit(y_data_int, location_par));
+			}
+			else if (likelihood_type_ == "poisson") {
+				return(LogLikPoisson(y_data_int, location_par, true));
+			}
+			else if (likelihood_type_ == "gamma") {
+				return(LogLikGamma(y_data, location_par, true));
+			}
+			else if (likelihood_type_ == "gaussian") {
+				return(LogLikGaussian(y_data, location_par));
+			}
+			else {
+				Log::REFatal("LogLikelihood: Likelihood of type '%s' is not supported.", likelihood_type_.c_str());
+				return(-1e99);
+			}
+		}//end LogLikelihood
+
+		inline double LogLikBernoulliProbit(const int y, const double location_par) const {
+			if (y == 0) {
+				return std::log(1 - normalCDF(location_par));
+			}
+			else {
+				return std::log(normalCDF(location_par));
+			}
+		}
+
+		inline double LogLikBernoulliLogit(const int y, const double location_par) const {
+			return (y * location_par - std::log(1 + std::exp(location_par)));
+			//Alternative version:
+			//if (y == 0) {
+			//	ll += std::log(1 - CondMeanLikelihood(location_par));//CondMeanLikelihood = logistic function
+			//}
+			//else {
+			//	ll += std::log(CondMeanLikelihood(location_par));
+			//}
+		}
+
+		inline double LogLikPoisson(const int y, const double location_par, bool incl_norm_const) const {
+			if (incl_norm_const) {
+				return (y * location_par - std::exp(location_par) + LogNormalizingConstantPoisson(y));
+			}
+			else {
+				return (y * location_par - std::exp(location_par));
+			}
+		}
+
+		inline double LogLikGamma(const double y, const double location_par, bool incl_norm_const) const {
+			if (incl_norm_const) {
+				return (-aux_pars_[0] * (location_par + y * std::exp(-location_par)) + LogNormalizingConstantGamma(y, 1, true));
+			}
+			else {
+				return (-aux_pars_[0] * (location_par + y * std::exp(-location_par)));
+			}
+		}
+
+		inline double LogLikGaussian(const double y, const double location_par) const {
+			return (std::log(aux_pars_[0]) + normalLogPDF(aux_pars_[0] * (y - location_par)));//aux_pars_[0] = 1. / std::sqrt(variance)
+		}
+
+		/*!
+		* \brief Calculate the first derivative of the log-likelihood with respect to the location parameter
+		* \param y_data Response variable data if response variable is continuous
+		* \param y_data_int Response variable data if response variable is integer-valued
+		* \param location_par Location parameter (random plus fixed effects)
+		* \param num_data Number of data points
+		*/
+		void CalcFirstDerivLogLik(const double* y_data,
+			const int* y_data_int,
+			const double* location_par,
+			const data_size_t num_data) {
+			if (likelihood_type_ == "bernoulli_probit") {
+#pragma omp parallel for schedule(static) if (num_data >= 128)
+				for (data_size_t i = 0; i < num_data; ++i) {
+					first_deriv_ll_[i] = FirstDerivLogLikBernoulliProbit(y_data_int[i], location_par[i]);
+				}
+			}
+			else if (likelihood_type_ == "bernoulli_logit") {
+#pragma omp parallel for schedule(static) if (num_data >= 128)
+				for (data_size_t i = 0; i < num_data; ++i) {
+					first_deriv_ll_[i] = FirstDerivLogLikBernoulliLogit(y_data_int[i], location_par[i]);
+				}
+			}
+			else if (likelihood_type_ == "poisson") {
+#pragma omp parallel for schedule(static) if (num_data >= 128)
+				for (data_size_t i = 0; i < num_data; ++i) {
+					first_deriv_ll_[i] = FirstDerivLogLikPoisson(y_data_int[i], location_par[i]);
+				}
+			}
+			else if (likelihood_type_ == "gamma") {
+#pragma omp parallel for schedule(static) if (num_data >= 128)
+				for (data_size_t i = 0; i < num_data; ++i) {
+					first_deriv_ll_[i] = FirstDerivLogLikGamma(y_data[i], location_par[i]);
+				}
+			}
+			else if (likelihood_type_ == "gaussian") {
+#pragma omp parallel for schedule(static) if (num_data >= 128)
+				for (data_size_t i = 0; i < num_data; ++i) {
+					first_deriv_ll_[i] = FirstDerivLogLikGaussian(y_data[i], location_par[i]);
+				}
+			}
+			else {
+				Log::REFatal("CalcFirstDerivLogLik: Likelihood of type '%s' is not supported.", likelihood_type_.c_str());
+			}
+		}//end CalcFirstDerivLogLik
+
+		/*!
+		* \brief Calculate the first derivative of the log-likelihood with respect to the location parameter
+		* \param y_data Response variable data if response variable is continuous
+		* \param y_data_int Response variable data if response variable is integer-valued
+		* \param location_par Location parameter (random plus fixed effects)
+		*/
+		inline double CalcFirstDerivLogLik(const double y_data,
+			const int y_data_int,
+			const double location_par) const {
+			if (likelihood_type_ == "bernoulli_probit") {
+				return(FirstDerivLogLikBernoulliProbit(y_data_int, location_par));
+			}
+			else if (likelihood_type_ == "bernoulli_logit") {
+				return(FirstDerivLogLikBernoulliLogit(y_data_int, location_par));
+			}
+			else if (likelihood_type_ == "poisson") {
+				return(FirstDerivLogLikPoisson(y_data_int, location_par));
+			}
+			else if (likelihood_type_ == "gamma") {
+				return(FirstDerivLogLikGamma(y_data, location_par));
+			}
+			else if (likelihood_type_ == "gaussian") {
+				return(FirstDerivLogLikGaussian(y_data, location_par));
+			}
+			else {
+				Log::REFatal("CalcFirstDerivLogLik: Likelihood of type '%s' is not supported.", likelihood_type_.c_str());
+				return(0.);
+			}
+		}//end CalcFirstDerivLogLik
+
+		inline double FirstDerivLogLikBernoulliProbit(const int y, const double location_par) const {
+			if (y == 0) {
+				return (-normalPDF(location_par) / (1 - normalCDF(location_par)));
+			}
+			else {
+				return (normalPDF(location_par) / normalCDF(location_par));
+			}
+		}
+
+		inline double FirstDerivLogLikBernoulliLogit(const int y, const double location_par) const {
+			return (y - CondMeanLikelihood(location_par));//CondMeanLikelihood = logistic(x)
+		}
+
+		inline double FirstDerivLogLikPoisson(const int y, const double location_par) const {
+			return (y - std::exp(location_par));
+		}
+
+		inline double FirstDerivLogLikGamma(const double y, const double location_par) const {
+			return (aux_pars_[0] * (y * std::exp(-location_par) - 1.));
+		}
+
+		inline double FirstDerivLogLikGaussian(const double y, const double location_par) const {
+			return (aux_pars_[0] * aux_pars_[0] * (y - location_par));
+		}
+
+		/*!
+		* \brief Calculate the second derivative of the negative (!) log-likelihood with respect to the location parameter
+		* \param y_data Response variable data if response variable is continuous
+		* \param y_data_int Response variable data if response variable is integer-valued
+		* \param location_par Location parameter (random plus fixed effects)
+		* \param num_data Number of data points
+		*/
+		void CalcSecondDerivNegLogLik(const double* y_data,
+			const int* y_data_int,
+			const double* location_par,
+			const data_size_t num_data) {
+			if (likelihood_type_ == "bernoulli_probit") {
+#pragma omp parallel for schedule(static) if (num_data >= 128)
+				for (data_size_t i = 0; i < num_data; ++i) {
+					second_deriv_neg_ll_[i] = SecondDerivNegLogLikBernoulliProbit(y_data_int[i], location_par[i]);
+				}
+			}
+			else if (likelihood_type_ == "bernoulli_logit") {
+#pragma omp parallel for schedule(static) if (num_data >= 128)
+				for (data_size_t i = 0; i < num_data; ++i) {
+					second_deriv_neg_ll_[i] = SecondDerivNegLogLikBernoulliLogit(location_par[i]);
+				}
+			}
+			else if (likelihood_type_ == "poisson") {
+#pragma omp parallel for schedule(static) if (num_data >= 128)
+				for (data_size_t i = 0; i < num_data; ++i) {
+					second_deriv_neg_ll_[i] = SecondDerivNegLogLikPoisson(location_par[i]);
+				}
+			}
+			else if (likelihood_type_ == "gamma") {
+#pragma omp parallel for schedule(static) if (num_data >= 128)
+				for (data_size_t i = 0; i < num_data; ++i) {
+					second_deriv_neg_ll_[i] = SecondDerivNegLogLikGamma(y_data[i], location_par[i]);
+				}
+			}
+			else if (likelihood_type_ == "gaussian") {
+#pragma omp parallel for schedule(static) if (num_data >= 128)
+				for (data_size_t i = 0; i < num_data; ++i) {
+					second_deriv_neg_ll_[i] = SecondDerivNegLogLikGaussian();
+				}
+			}
+			else {
+				Log::REFatal("CalcSecondDerivNegLogLik: Likelihood of type '%s' is not supported.", likelihood_type_.c_str());
+			}
+		}// end CalcSecondDerivNegLogLik
+
+		/*!
+		* \brief Calculate the second derivative of the negative (!) log-likelihood with respect to the location parameter
+		* \param y_data Response variable data if response variable is continuous
+		* \param y_data_int Response variable data if response variable is integer-valued
+		* \param location_par Location parameter (random plus fixed effects)
+		*/
+		inline double CalcSecondDerivNegLogLik(const double y_data,
+			const int y_data_int,
+			const double location_par) const {
+			if (likelihood_type_ == "bernoulli_probit") {
+				return(SecondDerivNegLogLikBernoulliProbit(y_data_int, location_par));
+			}
+			else if (likelihood_type_ == "bernoulli_logit") {
+				return(SecondDerivNegLogLikBernoulliLogit(location_par));
+			}
+			else if (likelihood_type_ == "poisson") {
+				return(SecondDerivNegLogLikPoisson(location_par));
+			}
+			else if (likelihood_type_ == "gamma") {
+				return(SecondDerivNegLogLikGamma(y_data, location_par));
+			}
+			else if (likelihood_type_ == "gaussian") {
+				return(SecondDerivNegLogLikGaussian());
+			}
+			else {
+				Log::REFatal("CalcSecondDerivNegLogLik: Likelihood of type '%s' is not supported.", likelihood_type_.c_str());
+				return(1.);
+			}
+		}// end CalcSecondDerivNegLogLik
+
+		inline double SecondDerivNegLogLikBernoulliProbit(const int y, const double location_par) const {
+			double dnorm = normalPDF(location_par);
+			double pnorm = normalCDF(location_par);
+			if (y == 0) {
+				double dnorm_frac_one_min_pnorm = dnorm / (1. - pnorm);
+				return (-dnorm_frac_one_min_pnorm * (location_par - dnorm_frac_one_min_pnorm));
+			}
+			else {
+				double dnorm_frac_pnorm = dnorm / pnorm;
+				return(dnorm_frac_pnorm * (location_par + dnorm_frac_pnorm));
+			}
+		}
+
+		inline double SecondDerivNegLogLikBernoulliLogit(const double location_par) const {
+			double exp_loc_i = std::exp(location_par);
+			return (exp_loc_i * std::pow(1. + exp_loc_i, -2));
+		}
+
+		inline double SecondDerivNegLogLikPoisson(const double location_par) const {
+			return std::exp(location_par);
+		}
+
+		inline double SecondDerivNegLogLikGamma(const double y, const double location_par) const {
+			return (aux_pars_[0] * y * std::exp(-location_par));
+		}
+
+		inline double SecondDerivNegLogLikGaussian() const {
+			return (aux_pars_[0] * aux_pars_[0]);//aux_pars_[0] = 1 / sqrt(variance)
+		}
+
+		/*!
+		* \brief Calculate the third derivative of the log-likelihood with respect to the location parameter
+		* \param y_data Response variable data if response variable is continuous
+		* \param y_data_int Response variable data if response variable is integer-valued
+		* \param location_par Location parameter (random plus fixed effects)
+		* \param num_data Number of data points
+		* \param[out] third_deriv Third derivative of the log-likelihood with respect to the location parameter. Need to pre-allocate memory of size num_data
+		*/
+		void CalcThirdDerivLogLik(const double* y_data,
+			const int* y_data_int,
+			const double* location_par,
+			const data_size_t num_data,
+			double* third_deriv) const {
+			if (likelihood_type_ == "bernoulli_probit") {
+#pragma omp parallel for schedule(static) if (num_data >= 128)
+				for (data_size_t i = 0; i < num_data; ++i) {
+					double dnorm = normalPDF(location_par[i]);
+					double pnorm = normalCDF(location_par[i]);
+					if (y_data_int[i] == 0) {
+						double dnorm_frac_one_min_pnorm = dnorm / (1. - pnorm);
+						third_deriv[i] = dnorm_frac_one_min_pnorm * (1 - location_par[i] * location_par[i] +
+							dnorm_frac_one_min_pnorm * (3 * location_par[i] - 2 * dnorm_frac_one_min_pnorm));
+					}
+					else {
+						double dnorm_frac_pnorm = dnorm / pnorm;
+						third_deriv[i] = dnorm_frac_pnorm * (location_par[i] * location_par[i] - 1 +
+							dnorm_frac_pnorm * (3 * location_par[i] + 2 * dnorm_frac_pnorm));
+					}
+				}
+			}
+			else if (likelihood_type_ == "bernoulli_logit") {
+#pragma omp parallel for schedule(static) if (num_data >= 128)
+				for (data_size_t i = 0; i < num_data; ++i) {
+					double exp_loc_i = std::exp(location_par[i]);
+					third_deriv[i] = -exp_loc_i * (1. - exp_loc_i) * std::pow(1 + exp_loc_i, -3);
+				}
+			}
+			else if (likelihood_type_ == "poisson") {
+#pragma omp parallel for schedule(static) if (num_data >= 128)
+				for (data_size_t i = 0; i < num_data; ++i) {
+					third_deriv[i] = -std::exp(location_par[i]);
+				}
+			}
+			else if (likelihood_type_ == "gamma") {
+#pragma omp parallel for schedule(static) if (num_data >= 128)
+				for (data_size_t i = 0; i < num_data; ++i) {
+					third_deriv[i] = aux_pars_[0] * y_data[i] * std::exp(-location_par[i]);
+				}
+			}
+			else {
+				Log::REFatal("CalcThirdDerivLogLik: Likelihood of type '%s' is not supported.", likelihood_type_.c_str());
+			}
+		}//end CalcThirdDerivLogLik
+
+		/*!
+		* \brief Calculates the gradient of the negative log-likelihood with respect to the additional parameters of the likelihood (e.g., shape for gamma)
+		* \param y_data Response variable data if response variable is continuous
+		* \param location_par Location parameter (random plus fixed effects)
+		* \param num_data Number of data points
+		* \param[out] grad Gradient
+		*/
+		void CalcGradNegLogLikAuxPars(const double* y_data,
+			const double* location_par,
+			const data_size_t num_data,
+			double* grad) const {
+			if (likelihood_type_ == "gamma") {
+				double neg_log_grad = 0.;//gradient for shape parameter is calculated on the log-scale
+#pragma omp parallel for schedule(static) reduction(+:neg_log_grad)
+				for (data_size_t i = 0; i < num_data; ++i) {
+					neg_log_grad += location_par[i] + y_data[i] * std::exp(-location_par[i]);
+				}
+				neg_log_grad -= num_data * (std::log(aux_pars_[0]) + 1. - digamma(aux_pars_[0]));
+				neg_log_grad -= aux_log_normalizing_constant_;
+				neg_log_grad *= aux_pars_[0];
+				grad[0] = neg_log_grad;
+			}
+			else if (likelihood_type_ != "gaussian" && likelihood_type_ != "bernoulli_probit" &&
+				likelihood_type_ != "bernoulli_logit" && likelihood_type_ != "poisson") {
+				Log::REFatal("CalcGradNegLogLikAuxPars: Likelihood of type '%s' is not supported.", likelihood_type_.c_str());
+			}
+		}//end CalcGradNegLogLikAuxPars
+
+		/*!
+		* \brief Calculates the second and the negative third derivative of the log-likelihood with respect to
+		*			(i) once and twice the location parameter and (ii) an additional parameter of the likelihood
+		* \param y_data Response variable data if response variable is continuous
+		* \param location_par Location parameter (random plus fixed effects)
+		* \param num_data Number of data points
+		* \param ind_aux_par Index of aux_pars_ wrt which the gradient is calculated (currently no used as there is only one)
+		* \param[out] second_deriv Second derivative
+		* \param[out] neg_third_deriv Negative third derivative
+		*/
+		void CalcSecondNegThirdDerivLogLikAuxParsLocPar(const double* y_data,
+			const double* location_par,
+			const data_size_t num_data,
+			int ind_aux_par,
+			double* second_deriv,
+			double* neg_third_deriv) const {
+			if (likelihood_type_ == "gamma") {
+				CHECK(ind_aux_par == 0);
+#pragma omp parallel for schedule(static)
+				for (data_size_t i = 0; i < num_data; ++i) {
+					second_deriv[i] = aux_pars_[0] * (y_data[i] * std::exp(-location_par[i]) - 1.);
+					neg_third_deriv[i] = second_deriv[i] + aux_pars_[0];
+				}
+			}
+			else if (likelihood_type_ != "gaussian" && likelihood_type_ != "bernoulli_probit" &&
+				likelihood_type_ != "bernoulli_logit" && likelihood_type_ != "poisson") {
+				Log::REFatal("CalcSecondDerivNegLogLikAuxParsLocPar: Likelihood of type '%s' is not supported.", likelihood_type_.c_str());
+			}
+		}//end CalcSecondNegThirdDerivLogLikAuxParsLocPar
+
+		/*!
+		* \brief Calculate the mean of the likelihood conditional on the (predicted) latent variable
+		*			Used for adaptive Gauss-Hermite quadrature for the prediction of the response variable
+		*/
+		inline double CondMeanLikelihood(const double value) const {
+			if (likelihood_type_ == "gaussian") {
+				return value;
+			}
+			else if (likelihood_type_ == "bernoulli_probit") {
+				return normalCDF(value);
+			}
+			else if (likelihood_type_ == "bernoulli_logit") {
+				return 1. / (1. + std::exp(-value));
+			}
+			else if (likelihood_type_ == "poisson") {
+				return std::exp(value);
+			}
+			else if (likelihood_type_ == "gamma") {
+				return std::exp(value);
+			}
+			else {
+				Log::REFatal("CondMeanLikelihood: Likelihood of type '%s' is not supported.", likelihood_type_.c_str());
+				return 0.;
+			}
+		}
+
+		/*!
+		* \brief Calculate the first derivative of the logarithm of the mean of the likelihood conditional on the (predicted) latent variable
+		*			Used for adaptive Gauss-Hermite quadrature for the prediction of the response variable
+		*/
+		inline double FirstDerivLogCondMeanLikelihood(const double value) const {
+			if (likelihood_type_ == "bernoulli_logit") {
+				return 1. / (1. + std::exp(value));
+			}
+			else if (likelihood_type_ == "poisson") {
+				return 1.;
+			}
+			else if (likelihood_type_ == "gamma") {
+				return 1.;
+			}
+			else {
+				Log::REFatal("FirstDerivLogCondMeanLikelihood: Likelihood of type '%s' is not supported.", likelihood_type_.c_str());
+				return 0.;
+			}
+		}
+
+		/*!
+		* \brief Calculate the second derivative of the logarithm of the mean of the likelihood conditional on the (predicted) latent variable
+		*			Used for adaptive Gauss-Hermite quadrature for the prediction of the response variable
+		*/
+		inline double SecondDerivLogCondMeanLikelihood(const double value) const {
+			if (likelihood_type_ == "bernoulli_logit") {
+				double exp_x = std::exp(value);
+				return -exp_x / ((1. + exp_x) * (1. + exp_x));
+			}
+			else if (likelihood_type_ == "poisson") {
+				return 0.;
+			}
+			else if (likelihood_type_ == "gamma") {
+				return 0.;
+			}
+			else {
+				Log::REFatal("SecondDerivLogCondMeanLikelihood: Likelihood of type '%s' is not supported.", likelihood_type_.c_str());
+				return 0.;
+			}
+		}
+
+		/*!
+		* \brief Do Cholesky decomposition
+		* \param[out] chol_fact Cholesky factor
+		* \param psi Matrix for which the Cholesky decomposition should be done
+		*/
+		template <class T_mat_1, typename std::enable_if <std::is_same<sp_mat_t, T_mat_1>::value ||
+			std::is_same<sp_mat_rm_t, T_mat_1>::value>::type* = nullptr >
+		void CalcChol(T_chol& chol_fact, const T_mat_1& psi) {
+			if (!chol_fact_pattern_analyzed_) {
+				chol_fact.analyzePattern(psi);
+				chol_fact_pattern_analyzed_ = true;
+			}
+			chol_fact.factorize(psi);
+		}
+		template <class T_mat_1, typename std::enable_if <std::is_same<den_mat_t, T_mat_1>::value>::type* = nullptr  >
+		void CalcChol(T_chol& chol_fact, const T_mat_1& psi) {
+			chol_fact.compute(psi);
+		}
+
+		/*!
+		* \brief Find the mode of the posterior of the latent random effects using Newton's method and calculate the approximative marginal log-likelihood..
+		*		Calculations are done using a numerically stable variant based on factorizing ("inverting") B = (Id + Wsqrt * Z*Sigma*Zt * Wsqrt).
+		*		In the notation of the paper: "Sigma = Z*Sigma*Z^T" and "Z = Id".
+		*		This version is used for the Laplace approximation when dense matrices are used (e.g. GP models).
+		* \param y_data Response variable data if response variable is continuous
+		* \param y_data_int Response variable data if response variable is integer-valued
+		* \param fixed_effects Fixed effects component of location parameter
+		* \param num_data Number of data points
+		* \param ZSigmaZt Covariance matrix of latent random effect
+		* \param[out] approx_marginal_ll Approximate marginal log-likelihood evaluated at the mode
+		*/
+		void FindModePostRandEffCalcMLLStable(const double* y_data,
+			const int* y_data_int,
+			const double* fixed_effects,
+			const data_size_t num_data,
+			const std::shared_ptr<T_mat> ZSigmaZt,
+			double& approx_marginal_ll) {
+			// Initialize variables
+			if (!mode_initialized_) {
+				InitializeModeAvec();
+			}
+			else {
+				mode_previous_value_ = mode_;
+				a_vec_previous_value_ = a_vec_;
+				na_or_inf_during_second_last_call_to_find_mode_ = na_or_inf_during_last_call_to_find_mode_;
+			}
+			bool no_fixed_effects = (fixed_effects == nullptr);
+			vec_t location_par;
+			// Initialize objective function (LA approx. marginal likelihood) for use as convergence criterion
+			if (no_fixed_effects) {
+				approx_marginal_ll = -0.5 * (a_vec_.dot(mode_)) + LogLikelihood(y_data, y_data_int, mode_.data(), num_data);
+			}
+			else {
+				location_par = vec_t(num_data);
+#pragma omp parallel for schedule(static)
+				for (data_size_t i = 0; i < num_data; ++i) {
+					location_par[i] = mode_[i] + fixed_effects[i];
+				}
+				approx_marginal_ll = -0.5 * (a_vec_.dot(mode_)) + LogLikelihood(y_data, y_data_int, location_par.data(), num_data);
+			}
+			double approx_marginal_ll_new = approx_marginal_ll;
+			vec_t rhs, v_aux;//auxiliary variables
+			vec_t Wsqrt(num_data);//diagonal matrix with square root of negative second derivatives on the diagonal (sqrt of negative Hessian of log-likelihood)
+			T_mat Id_plus_Wsqrt_ZSigmaZt_Wsqrt(num_data, num_data);
+			// Start finding mode 
+			int it;
+			bool terminate_optim = false;
+			bool has_NA_or_Inf = false;
+			for (it = 0; it < MAXIT_MODE_NEWTON_; ++it) {
+				// Calculate first and second derivative of log-likelihood
+				if (no_fixed_effects) {
+					CalcFirstDerivLogLik(y_data, y_data_int, mode_.data(), num_data);
+					CalcSecondDerivNegLogLik(y_data, y_data_int, mode_.data(), num_data);
+				}
+				else {
+					CalcFirstDerivLogLik(y_data, y_data_int, location_par.data(), num_data);
+					CalcSecondDerivNegLogLik(y_data, y_data_int, location_par.data(), num_data);
+				}
+				// Calculate Cholesky factor of matrix B = Id + Wsqrt * Z*Sigma*Zt * Wsqrt
+				Wsqrt.array() = second_deriv_neg_ll_.array().sqrt();
+				Id_plus_Wsqrt_ZSigmaZt_Wsqrt.setIdentity();
+				Id_plus_Wsqrt_ZSigmaZt_Wsqrt += (Wsqrt.asDiagonal() * (*ZSigmaZt) * Wsqrt.asDiagonal());
+				CalcChol<T_mat>(chol_fact_Id_plus_Wsqrt_Sigma_Wsqrt_, Id_plus_Wsqrt_ZSigmaZt_Wsqrt);
+				// Update mode and a_vec_
+				rhs.array() = second_deriv_neg_ll_.array() * mode_.array() + first_deriv_ll_.array();
+				v_aux = Wsqrt.asDiagonal() * (*ZSigmaZt) * rhs;
+				a_vec_ = rhs - Wsqrt.asDiagonal() * (chol_fact_Id_plus_Wsqrt_Sigma_Wsqrt_.solve(v_aux));
+				mode_ = (*ZSigmaZt) * a_vec_;
+				// Calculate new objective function
+				if (no_fixed_effects) {
+					approx_marginal_ll_new = -0.5 * (a_vec_.dot(mode_)) + LogLikelihood(y_data, y_data_int, mode_.data(), num_data);
+				}
+				else {
+					// Update location parameter of log-likelihood for calculation of approx. marginal log-likelihood (objective function)
+#pragma omp parallel for schedule(static)
+					for (data_size_t i = 0; i < num_data; ++i) {
+						location_par[i] = mode_[i] + fixed_effects[i];
+					}
+					approx_marginal_ll_new = -0.5 * (a_vec_.dot(mode_)) + LogLikelihood(y_data, y_data_int, location_par.data(), num_data);
+				}
+				if (std::isnan(approx_marginal_ll_new) || std::isinf(approx_marginal_ll_new)) {
+					has_NA_or_Inf = true;
+					Log::REDebug(NA_OR_INF_WARNING_);
+					break;
+				}
+				// Check convergence
+				if (it == 0) {
+					if (std::abs(approx_marginal_ll_new - approx_marginal_ll) < DELTA_REL_CONV_ * std::abs(approx_marginal_ll)) { // allow for decreases in first iteration
+						terminate_optim = true;
+					}
+				}
+				else {
+					if ((approx_marginal_ll_new - approx_marginal_ll) < DELTA_REL_CONV_ * std::abs(approx_marginal_ll)) {
+						terminate_optim = true;
+					}
+				}
+				if (terminate_optim) {
+					if (approx_marginal_ll_new < approx_marginal_ll) {
+						Log::REDebug(NO_INCREASE_IN_MLL_WARNING_);
+					}
+					approx_marginal_ll = approx_marginal_ll_new;
+					break;
+				}
+				else {
+					approx_marginal_ll = approx_marginal_ll_new;
+				}
+			}
+			if (it == MAXIT_MODE_NEWTON_) {
+				Log::REDebug(NO_CONVERGENCE_WARNING_);
+			}
+			if (has_NA_or_Inf) {
+				approx_marginal_ll = approx_marginal_ll_new;
+				na_or_inf_during_last_call_to_find_mode_ = true;
+			}
+			else {
+				if (no_fixed_effects) {
+					CalcFirstDerivLogLik(y_data, y_data_int, mode_.data(), num_data);//first derivative is not used here anymore but since it is reused in gradient calculation and in prediction, we calculate it once more
+					CalcSecondDerivNegLogLik(y_data, y_data_int, mode_.data(), num_data);
+				}
+				else {
+					CalcFirstDerivLogLik(y_data, y_data_int, location_par.data(), num_data);//first derivative is not used here anymore but since it is reused in gradient calculation and in prediction, we calculate it once more
+					CalcSecondDerivNegLogLik(y_data, y_data_int, location_par.data(), num_data);
+				}
+				Wsqrt.array() = second_deriv_neg_ll_.array().sqrt();
+				Id_plus_Wsqrt_ZSigmaZt_Wsqrt.setIdentity();
+				Id_plus_Wsqrt_ZSigmaZt_Wsqrt += (Wsqrt.asDiagonal() * (*ZSigmaZt) * Wsqrt.asDiagonal());
+				CalcChol<T_mat>(chol_fact_Id_plus_Wsqrt_Sigma_Wsqrt_, Id_plus_Wsqrt_ZSigmaZt_Wsqrt);
+				approx_marginal_ll -= ((T_mat)chol_fact_Id_plus_Wsqrt_Sigma_Wsqrt_.matrixL()).diagonal().array().log().sum();
+				mode_has_been_calculated_ = true;
+				na_or_inf_during_last_call_to_find_mode_ = false;
+			}
+		}//end FindModePostRandEffCalcMLLStable
+
+		/*!
+		* \brief Find the mode of the posterior of the latent random effects using Newton's method and calculate the approximative marginal log-likelihood.
+		*		Calculations are done on the random effects (b) scale and not the "data scale" (Zb) using
+		*		a numerically stable variant based on factorizing ("inverting") B = (Id + ZtWZsqrt * Sigma * ZtWZsqrt).
+		*		This version is used for the Laplace approximation when there is only one Gaussian process and
+		*		there are a lot of multiple observations at the same location, i.e., the dimenion of the random effects b is much smaller than Zb
+		* \param y_data Response variable data if response variable is continuous
+		* \param y_data_int Response variable data if response variable is integer-valued
+		* \param fixed_effects Fixed effects component of location parameter
+		* \param num_data Number of data points
+		* \param Sigma Covariance matrix of latent random effect
+		* \param random_effects_indices_of_data Indices that indicate to which random effect every data point is related
+		* \param[out] approx_marginal_ll Approximate marginal log-likelihood evaluated at the mode
+		*/
+		void FindModePostRandEffCalcMLLOnlyOneGPCalculationsOnREScale(const double* y_data,
+			const int* y_data_int,
+			const double* fixed_effects,
+			const data_size_t num_data,
+			const std::shared_ptr<T_mat> Sigma,
+			const data_size_t* const random_effects_indices_of_data,
+			double& approx_marginal_ll) {
+			// Initialize variables
+			if (!mode_initialized_) {
+				InitializeModeAvec();
+			}
+			else {
+				mode_previous_value_ = mode_;
+				a_vec_previous_value_ = a_vec_;
+				na_or_inf_during_second_last_call_to_find_mode_ = na_or_inf_during_last_call_to_find_mode_;
+			}
+			vec_t location_par(num_data);//location parameter = mode of random effects + fixed effects
+			if (fixed_effects == nullptr) {
+#pragma omp parallel for schedule(static)
+				for (data_size_t i = 0; i < num_data; ++i) {
+					location_par[i] = mode_[random_effects_indices_of_data[i]];
+				}
+			}
+			else {
+#pragma omp parallel for schedule(static)
+				for (data_size_t i = 0; i < num_data; ++i) {
+					location_par[i] = mode_[random_effects_indices_of_data[i]] + fixed_effects[i];
+				}
+			}
+			// Initialize objective function (LA approx. marginal likelihood) for use as convergence criterion
+			approx_marginal_ll = -0.5 * (a_vec_.dot(mode_)) + LogLikelihood(y_data, y_data_int, location_par.data(), num_data);
+			double approx_marginal_ll_new = approx_marginal_ll;
+			vec_t diag_sqrt_ZtWZ(num_re_);//sqrt of diagonal matrix ZtWZ
+			T_mat Id_plus_ZtWZsqrt_Sigma_ZtWZsqrt(num_re_, num_re_);
+			vec_t rhs, v_aux;
+			int it;
+			bool terminate_optim = false;
+			bool has_NA_or_Inf = false;
+			for (it = 0; it < MAXIT_MODE_NEWTON_; ++it) {
+				// Calculate first and second derivative of log-likelihood
+				CalcFirstDerivLogLik(y_data, y_data_int, location_par.data(), num_data);
+				CalcSecondDerivNegLogLik(y_data, y_data_int, location_par.data(), num_data);
+				// Calculate right hand side for mode update
+				CalcZtVGivenIndices(num_data, num_re_, random_effects_indices_of_data, second_deriv_neg_ll_, diag_sqrt_ZtWZ, true);
+				rhs = (diag_sqrt_ZtWZ.array() * mode_.array()).matrix();//rhs = ZtWZ * mode_ + Zt * first_deriv_ll_ for updating mode
+				CalcZtVGivenIndices(num_data, num_re_, random_effects_indices_of_data, first_deriv_ll_, rhs, false);
+				// Calculate Cholesky factor of matrix B = Id + ZtWZsqrt * Sigma * ZtWZsqrt
+				diag_sqrt_ZtWZ.array() = diag_sqrt_ZtWZ.array().sqrt();
+				Id_plus_ZtWZsqrt_Sigma_ZtWZsqrt.setIdentity();
+				Id_plus_ZtWZsqrt_Sigma_ZtWZsqrt += diag_sqrt_ZtWZ.asDiagonal() * (*Sigma) * diag_sqrt_ZtWZ.asDiagonal();
+				CalcChol<T_mat>(chol_fact_Id_plus_Wsqrt_Sigma_Wsqrt_, Id_plus_ZtWZsqrt_Sigma_ZtWZsqrt);//this is the bottleneck (for large data and sparse matrices)
+				// Update mode and a_vec_
+				v_aux = (*Sigma) * rhs;
+				v_aux.array() *= diag_sqrt_ZtWZ.array();
+				a_vec_ = -chol_fact_Id_plus_Wsqrt_Sigma_Wsqrt_.solve(v_aux);
+				a_vec_.array() *= diag_sqrt_ZtWZ.array();
+				a_vec_.array() += rhs.array();
+				mode_ = (*Sigma) * a_vec_;
+				// Update location parameter of log-likelihood for calculation of approx. marginal log-likelihood (objective function)
+				if (fixed_effects == nullptr) {
+#pragma omp parallel for schedule(static)
+					for (data_size_t i = 0; i < num_data; ++i) {
+						location_par[i] = mode_[random_effects_indices_of_data[i]];
+					}
+				}
+				else {
+#pragma omp parallel for schedule(static)
+					for (data_size_t i = 0; i < num_data; ++i) {
+						location_par[i] = mode_[random_effects_indices_of_data[i]] + fixed_effects[i];
+					}
+				}
+				// Calculate new objective function
+				approx_marginal_ll_new = -0.5 * (a_vec_.dot(mode_)) + LogLikelihood(y_data, y_data_int, location_par.data(), num_data);
+				if (std::isnan(approx_marginal_ll_new) || std::isinf(approx_marginal_ll_new)) {
+					has_NA_or_Inf = true;
+					Log::REDebug(NA_OR_INF_WARNING_);
+					break;
+				}
+				// Check convergence
+				if (it == 0) {
+					if (std::abs(approx_marginal_ll_new - approx_marginal_ll) < DELTA_REL_CONV_ * std::abs(approx_marginal_ll)) { // allow for decreases in first iteration
+						terminate_optim = true;
+					}
+				}
+				else {
+					if ((approx_marginal_ll_new - approx_marginal_ll) < DELTA_REL_CONV_ * std::abs(approx_marginal_ll)) {
+						terminate_optim = true;
+					}
+				}
+				if (terminate_optim) {
+					if (approx_marginal_ll_new < approx_marginal_ll) {
+						Log::REDebug(NO_INCREASE_IN_MLL_WARNING_);
+					}
+					approx_marginal_ll = approx_marginal_ll_new;
+					break;
+				}
+				else {
+					approx_marginal_ll = approx_marginal_ll_new;
+				}
+			}//end loop for finding mode
+			if (it == MAXIT_MODE_NEWTON_) {
+				Log::REDebug(NO_CONVERGENCE_WARNING_);
+			}
+			if (has_NA_or_Inf) {
+				approx_marginal_ll = approx_marginal_ll_new;
+				na_or_inf_during_last_call_to_find_mode_ = true;
+			}
+			else {
+				CalcFirstDerivLogLik(y_data, y_data_int, location_par.data(), num_data);//first derivative is not used here anymore but since it is reused in gradient calculation and in prediction, we calculate it once more
+				CalcSecondDerivNegLogLik(y_data, y_data_int, location_par.data(), num_data);
+				CalcZtVGivenIndices(num_data, num_re_, random_effects_indices_of_data, second_deriv_neg_ll_, diag_sqrt_ZtWZ, true);
+				diag_sqrt_ZtWZ.array() = diag_sqrt_ZtWZ.array().sqrt();
+				Id_plus_ZtWZsqrt_Sigma_ZtWZsqrt.setIdentity();
+				Id_plus_ZtWZsqrt_Sigma_ZtWZsqrt += diag_sqrt_ZtWZ.asDiagonal() * (*Sigma) * diag_sqrt_ZtWZ.asDiagonal();
+				CalcChol<T_mat>(chol_fact_Id_plus_Wsqrt_Sigma_Wsqrt_, Id_plus_ZtWZsqrt_Sigma_ZtWZsqrt);
+				approx_marginal_ll -= ((T_mat)chol_fact_Id_plus_Wsqrt_Sigma_Wsqrt_.matrixL()).diagonal().array().log().sum();
+				mode_has_been_calculated_ = true;
+				na_or_inf_during_last_call_to_find_mode_ = false;
+			}
+		}//end FindModePostRandEffCalcMLLOnlyOneGPCalculationsOnREScale
+
+		/*!
+		* \brief Find the mode of the posterior of the latent random effects using Newton's method and calculate the approximative marginal log-likelihood.
+		*		Calculations are done by directly factorizing ("inverting) (Sigma^-1 + Zt*W*Z).
+		*		NOTE: IT IS ASSUMED THAT SIGMA IS A DIAGONAL MATRIX
+		*		This version is used for the Laplace approximation when there are only grouped random effects.
+		* \param y_data Response variable data if response variable is continuous
+		* \param y_data_int Response variable data if response variable is integer-valued
+		* \param fixed_effects Fixed effects component of location parameter
+		* \param num_data Number of data points
+		* \param SigmaI Inverse covariance matrix of latent random effect. Currently, this needs to be a diagonal matrix
+		* \param Zt Transpose Z^T of random effect design matrix that relates latent random effects to observations/likelihoods
+		* \param[out] approx_marginal_ll Approximate marginal log-likelihood evaluated at the mode
+		*/
+		void FindModePostRandEffCalcMLLGroupedRE(const double* y_data,
+			const int* y_data_int,
+			const double* fixed_effects,
+			const data_size_t num_data,
+			const sp_mat_t& SigmaI,
+			const sp_mat_t& Zt,
+			double& approx_marginal_ll) {
+			// Initialize variables
+			if (!mode_initialized_) {
+				InitializeModeAvec();
+			}
+			else {
+				mode_previous_value_ = mode_;
+				na_or_inf_during_second_last_call_to_find_mode_ = na_or_inf_during_last_call_to_find_mode_;
+			}
+			sp_mat_t Z = Zt.transpose();
+			vec_t location_par = Z * mode_;//location parameter = mode of random effects + fixed effects
+			if (fixed_effects != nullptr) {
+#pragma omp parallel for schedule(static)
+				for (data_size_t i = 0; i < num_data; ++i) {
+					location_par[i] += fixed_effects[i];
+				}
+			}
+			// Initialize objective function (LA approx. marginal likelihood) for use as convergence criterion
+			approx_marginal_ll = -0.5 * (mode_.dot(SigmaI * mode_)) + LogLikelihood(y_data, y_data_int, location_par.data(), num_data);
+			double approx_marginal_ll_new = approx_marginal_ll;
+			sp_mat_t SigmaI_plus_ZtWZ;
+			vec_t rhs;
+			// Start finding mode 
+			int it;
+			bool terminate_optim = false;
+			bool has_NA_or_Inf = false;
+			for (it = 0; it < MAXIT_MODE_NEWTON_; ++it) {
+				// Calculate first and second derivative of log-likelihood
+				CalcFirstDerivLogLik(y_data, y_data_int, location_par.data(), num_data);
+				CalcSecondDerivNegLogLik(y_data, y_data_int, location_par.data(), num_data);
+				// Calculate Cholesky factor and update mode
+				rhs = Zt * first_deriv_ll_ - SigmaI * mode_;//right hand side for updating mode
+				SigmaI_plus_ZtWZ = SigmaI + Zt * second_deriv_neg_ll_.asDiagonal() * Z;
+				SigmaI_plus_ZtWZ.makeCompressed();
+				if (!chol_fact_pattern_analyzed_) {
+					chol_fact_SigmaI_plus_ZtWZ_grouped_.analyzePattern(SigmaI_plus_ZtWZ);
+					chol_fact_pattern_analyzed_ = true;
+				}
+				chol_fact_SigmaI_plus_ZtWZ_grouped_.factorize(SigmaI_plus_ZtWZ);
+				mode_ += chol_fact_SigmaI_plus_ZtWZ_grouped_.solve(rhs);
+				// Update location parameter of log-likelihood for calculation of approx. marginal log-likelihood (objective function)
+				location_par = Z * mode_;
+				if (fixed_effects != nullptr) {
+#pragma omp parallel for schedule(static)
+					for (data_size_t i = 0; i < num_data; ++i) {
+						location_par[i] += fixed_effects[i];
+					}
+				}
+				// Calculate new objective function
+				approx_marginal_ll_new = -0.5 * (mode_.dot(SigmaI * mode_)) + LogLikelihood(y_data, y_data_int, location_par.data(), num_data);
+				if (std::isnan(approx_marginal_ll_new) || std::isinf(approx_marginal_ll_new)) {
+					has_NA_or_Inf = true;
+					Log::REDebug(NA_OR_INF_WARNING_);
+					break;
+				}
+				// Check convergence
+				if (it == 0) {
+					if (std::abs(approx_marginal_ll_new - approx_marginal_ll) < DELTA_REL_CONV_ * std::abs(approx_marginal_ll)) { // allow for decreases in first iteration
+						terminate_optim = true;
+					}
+				}
+				else {
+					if ((approx_marginal_ll_new - approx_marginal_ll) < DELTA_REL_CONV_ * std::abs(approx_marginal_ll)) {
+						terminate_optim = true;
+					}
+				}
+				if (terminate_optim) {
+					if (approx_marginal_ll_new < approx_marginal_ll) {
+						Log::REDebug(NO_INCREASE_IN_MLL_WARNING_);
+					}
+					approx_marginal_ll = approx_marginal_ll_new;
+					break;
+				}
+				else {
+					approx_marginal_ll = approx_marginal_ll_new;
+				}
+			}//end mode finding algorithm
+			if (it == MAXIT_MODE_NEWTON_) {
+				Log::REDebug(NO_CONVERGENCE_WARNING_);
+			}
+			if (has_NA_or_Inf) {
+				approx_marginal_ll = approx_marginal_ll_new;
+				na_or_inf_during_last_call_to_find_mode_ = true;
+			}
+			else {
+				CalcFirstDerivLogLik(y_data, y_data_int, location_par.data(), num_data);//first derivative is not used here anymore but since it is reused in gradient calculation and in prediction, we calculate it once more
+				CalcSecondDerivNegLogLik(y_data, y_data_int, location_par.data(), num_data);
+				SigmaI_plus_ZtWZ = SigmaI + Zt * second_deriv_neg_ll_.asDiagonal() * Z;
+				SigmaI_plus_ZtWZ.makeCompressed();
+				chol_fact_SigmaI_plus_ZtWZ_grouped_.factorize(SigmaI_plus_ZtWZ);
+				approx_marginal_ll += -((sp_mat_t)chol_fact_SigmaI_plus_ZtWZ_grouped_.matrixL()).diagonal().array().log().sum() + 0.5 * SigmaI.diagonal().array().log().sum();
+				mode_has_been_calculated_ = true;
+				na_or_inf_during_last_call_to_find_mode_ = false;
+			}
+		}//end FindModePostRandEffCalcMLLGroupedRE
+
+		/*!
+		* \brief Find the mode of the posterior of the latent random effects using Newton's method and calculate the approximative marginal log-likelihood.
+		*		Calculations are done by directly factorizing ("inverting) (Sigma^-1 + Zt*W*Z).
+		*		This version is used for the Laplace approximation when there are only grouped random effects with only one grouping variable.
+		* \param y_data Response variable data if response variable is continuous
+		* \param y_data_int Response variable data if response variable is integer-valued
+		* \param fixed_effects Fixed effects component of location parameter
+		* \param num_data Number of data points
+		* \param sigma2 Variance of random effects
+		* \param random_effects_indices_of_data Indices that indicate to which random effect every data point is related
+		* \param[out] approx_marginal_ll Approximate marginal log-likelihood evaluated at the mode
+		*/
+		void FindModePostRandEffCalcMLLOnlyOneGroupedRECalculationsOnREScale(const double* y_data,
+			const int* y_data_int,
+			const double* fixed_effects,
+			const data_size_t num_data,
+			const double sigma2,
+			const data_size_t* const random_effects_indices_of_data,
+			double& approx_marginal_ll) {
+			// Initialize variables
+			if (!mode_initialized_) {
+				InitializeModeAvec();
+			}
+			else {
+				mode_previous_value_ = mode_;
+				na_or_inf_during_second_last_call_to_find_mode_ = na_or_inf_during_last_call_to_find_mode_;
+			}
+			vec_t location_par(num_data);//location parameter = mode of random effects + fixed effects
+			if (fixed_effects == nullptr) {
+#pragma omp parallel for schedule(static)
+				for (data_size_t i = 0; i < num_data; ++i) {
+					location_par[i] = mode_[random_effects_indices_of_data[i]];
+				}
+			}
+			else {
+#pragma omp parallel for schedule(static)
+				for (data_size_t i = 0; i < num_data; ++i) {
+					location_par[i] = mode_[random_effects_indices_of_data[i]] + fixed_effects[i];
+				}
+			}
+			// Initialize objective function (LA approx. marginal likelihood) for use as convergence criterion
+			approx_marginal_ll = -0.5 / sigma2 * (mode_.dot(mode_)) + LogLikelihood(y_data, y_data_int, location_par.data(), num_data);
+			double approx_marginal_ll_new = approx_marginal_ll;
+			vec_t rhs;
+			diag_SigmaI_plus_ZtWZ_ = vec_t(num_re_);
+			// Start finding mode 
+			int it;
+			bool terminate_optim = false;
+			bool has_NA_or_Inf = false;
+			for (it = 0; it < MAXIT_MODE_NEWTON_; ++it) {
+				// Calculate first and second derivative of log-likelihood
+				CalcFirstDerivLogLik(y_data, y_data_int, location_par.data(), num_data);
+				CalcSecondDerivNegLogLik(y_data, y_data_int, location_par.data(), num_data);
+				// Calculate rhs for mode update
+				rhs = -mode_ / sigma2;//right hand side for updating mode
+				CalcZtVGivenIndices(num_data, num_re_, random_effects_indices_of_data, first_deriv_ll_, rhs, false);
+				// Update mode
+				CalcZtVGivenIndices(num_data, num_re_, random_effects_indices_of_data, second_deriv_neg_ll_, diag_SigmaI_plus_ZtWZ_, true);
+				diag_SigmaI_plus_ZtWZ_.array() += 1. / sigma2;
+				mode_ += (rhs.array() / diag_SigmaI_plus_ZtWZ_.array()).matrix();
+				// Update location parameter of log-likelihood for calculation of approx. marginal log-likelihood (objective function)
+				if (fixed_effects == nullptr) {
+#pragma omp parallel for schedule(static)
+					for (data_size_t i = 0; i < num_data; ++i) {
+						location_par[i] = mode_[random_effects_indices_of_data[i]];
+					}
+				}
+				else {
+#pragma omp parallel for schedule(static)
+					for (data_size_t i = 0; i < num_data; ++i) {
+						location_par[i] = mode_[random_effects_indices_of_data[i]] + fixed_effects[i];
+					}
+				}
+				// Calculate new objective function
+				approx_marginal_ll_new = -0.5 / sigma2 * (mode_.dot(mode_)) + LogLikelihood(y_data, y_data_int, location_par.data(), num_data);
+				if (std::isnan(approx_marginal_ll_new) || std::isinf(approx_marginal_ll_new)) {
+					has_NA_or_Inf = true;
+					Log::REDebug(NA_OR_INF_WARNING_);
+					break;
+				}
+				// Check convergence
+				if (it == 0) {
+					if (std::abs(approx_marginal_ll_new - approx_marginal_ll) < DELTA_REL_CONV_ * std::abs(approx_marginal_ll)) { // allow for decreases in first iteration
+						terminate_optim = true;
+					}
+				}
+				else {
+					if ((approx_marginal_ll_new - approx_marginal_ll) < DELTA_REL_CONV_ * std::abs(approx_marginal_ll)) {
+						terminate_optim = true;
+					}
+				}
+				if (terminate_optim) {
+					if (approx_marginal_ll_new < approx_marginal_ll) {
+						Log::REDebug(NO_INCREASE_IN_MLL_WARNING_);
+					}
+					approx_marginal_ll = approx_marginal_ll_new;
+					break;
+				}
+				else {
+					approx_marginal_ll = approx_marginal_ll_new;
+				}
+			}//end mode finding algorithm
+			if (it == MAXIT_MODE_NEWTON_) {
+				Log::REDebug(NO_CONVERGENCE_WARNING_);
+			}
+			if (has_NA_or_Inf) {
+				approx_marginal_ll = approx_marginal_ll_new;
+				na_or_inf_during_last_call_to_find_mode_ = true;
+			}
+			else {
+				CalcFirstDerivLogLik(y_data, y_data_int, location_par.data(), num_data);//first derivative is not used here anymore but since it is reused in gradient calculation and in prediction, we calculate it once more
+				CalcSecondDerivNegLogLik(y_data, y_data_int, location_par.data(), num_data);
+				CalcZtVGivenIndices(num_data, num_re_, random_effects_indices_of_data, second_deriv_neg_ll_, diag_SigmaI_plus_ZtWZ_, true);
+				diag_SigmaI_plus_ZtWZ_.array() += 1. / sigma2;
+				approx_marginal_ll -= 0.5 * diag_SigmaI_plus_ZtWZ_.array().log().sum() + 0.5 * num_re_ * std::log(sigma2);
+				mode_has_been_calculated_ = true;
+				na_or_inf_during_last_call_to_find_mode_ = false;
+			}
+		}//end FindModePostRandEffCalcMLLOnlyOneGroupedRECalculationsOnREScale
+
+		/*!
+		* \brief Find the mode of the posterior of the latent random effects using Newton's method and calculate the approximative marginal log-likelihood.
+		*		Calculations are done by factorizing ("inverting) (Sigma^-1 + W) where it is assumed that an approximate Cholesky factor
+		*		of Sigma^-1 has previously been calculated using a Vecchia approximation.
+		*		This version is used for the Laplace approximation when there are only GP random effects and the Vecchia approximation is used.
+		*		Caveat: Sigma^-1 + W can be not very sparse
+		* \param y_data Response variable data if response variable is continuous
+		* \param y_data_int Response variable data if response variable is integer-valued
+		* \param fixed_effects Fixed effects component of location parameter
+		* \param num_data Number of data points
+		* \param B Matrix B in Vecchia approximation Sigma^-1 = B^T D^-1 B ("=" Cholesky factor)
+		* \param D_inv Diagonal matrix D^-1 in Vecchia approximation Sigma^-1 = B^T D^-1 B
+		* \param[out] approx_marginal_ll Approximate marginal log-likelihood evaluated at the mode
+		*/
+		void FindModePostRandEffCalcMLLVecchia(const double* y_data,
+			const int* y_data_int,
+			const double* fixed_effects,
+			const data_size_t num_data,
+			const sp_mat_t& B,
+			const sp_mat_t& D_inv,
+			double& approx_marginal_ll) {
+			// Initialize variables
+			if (!mode_initialized_) {
+				InitializeModeAvec();
+			}
+			else {
+				mode_previous_value_ = mode_;
+				na_or_inf_during_second_last_call_to_find_mode_ = na_or_inf_during_last_call_to_find_mode_;
+			}
+			bool no_fixed_effects = (fixed_effects == nullptr);
+			sp_mat_t SigmaI = B.transpose() * D_inv * B;
+			vec_t location_par;//location parameter = mode of random effects + fixed effects
+			sp_mat_t SigmaI_plus_W;
+			vec_t rhs, B_mode, mode_new;
+			vec_t mode_after_grad_aux, mode_after_grad_aux_lag1;//auxiliary variable used only if quasi_newton_for_mode_finding_
+			if (quasi_newton_for_mode_finding_) {
+				mode_after_grad_aux_lag1 = mode_;
+			}
+			// Initialize objective function (LA approx. marginal likelihood) for use as convergence criterion
+			B_mode = B * mode_;
+			if (no_fixed_effects) {
+				approx_marginal_ll = -0.5 * (B_mode.dot(D_inv * B_mode)) + LogLikelihood(y_data, y_data_int, mode_.data(), num_data);
+			}
+			else {
+				location_par = vec_t(num_data);
+#pragma omp parallel for schedule(static)
+				for (data_size_t i = 0; i < num_data; ++i) {
+					location_par[i] = mode_[i] + fixed_effects[i];
+				}
+				approx_marginal_ll = -0.5 * (B_mode.dot(D_inv * B_mode)) + LogLikelihood(y_data, y_data_int, location_par.data(), num_data);
+			}
+			double approx_marginal_ll_new = approx_marginal_ll;
+			// Start finding mode 
+			int it;
+			bool terminate_optim = false;
+			bool has_NA_or_Inf = false;
+			double lr_GD = 1.;// learning rate for gradient descent
+			for (it = 0; it < MAXIT_MODE_NEWTON_; ++it) {
+				// Calculate first and second derivative of log-likelihood
+				if (no_fixed_effects) {
+					CalcFirstDerivLogLik(y_data, y_data_int, mode_.data(), num_data);
+					CalcSecondDerivNegLogLik(y_data, y_data_int, mode_.data(), num_data);
+				}
+				else {
+					CalcFirstDerivLogLik(y_data, y_data_int, location_par.data(), num_data);
+					CalcSecondDerivNegLogLik(y_data, y_data_int, location_par.data(), num_data);
+				}
+				if (quasi_newton_for_mode_finding_) {
+					vec_t grad = first_deriv_ll_ - B.transpose() * (D_inv * (B * mode_));
+					sp_mat_t D_inv_B = D_inv * B;
+					sp_mat_t Bt_D_inv_B_aux = B.cwiseProduct(D_inv_B);
+					vec_t SigmaI_diag = Bt_D_inv_B_aux.transpose() * vec_t::Ones(Bt_D_inv_B_aux.rows());
+					grad.array() /= (second_deriv_neg_ll_.array() + SigmaI_diag.array());
+					//// Alternative way approximating W + Sigma^-1 with Bt * (W + D^-1) * B. 
+					//// Note: seems to work worse compared to above diagonal approach. Also, better to comment out "nesterov_acc_rate *= 0.5;"
+					//vec_t grad_aux = B.transpose().triangularView<Eigen::UpLoType::UnitUpper>().solve(grad);
+					//grad_aux.array() /= (D_inv.diagonal().array() + second_deriv_neg_ll_.array());
+					//grad = B.triangularView<Eigen::UpLoType::UnitLower>().solve(grad_aux);
+					lr_GD = 1.;
+					double nesterov_acc_rate = (1. - (3. / (6. + it)));//Nesterov acceleration factor
+					for (int ih = 0; ih < MAX_NUMBER_LR_SHRINKAGE_STEPS_; ++ih) {
+						mode_after_grad_aux = mode_ + lr_GD * grad;
+						REModelTemplate<T_mat, T_chol>::ApplyMomentumStep(it, mode_after_grad_aux, mode_after_grad_aux_lag1,
+							mode_new, nesterov_acc_rate, 0, false, 2, false);
+						if (cap_change_mode_newton_) {
+#pragma omp parallel for schedule(static)
+							for (data_size_t i = 0; i < num_data; ++i) {
+								double abs_change = std::abs(mode_new[i] - mode_[i]);
+								if (abs_change > MAX_CHANGE_MODE_NEWTON_) {
+									mode_new[i] = mode_[i] + (mode_new[i] - mode_[i]) / abs_change * MAX_CHANGE_MODE_NEWTON_;
+								}
+							}
+						}//end cap_change_mode_newton_
+						B_mode = B * mode_new;
+						if (no_fixed_effects) {
+							approx_marginal_ll_new = -0.5 * (B_mode.dot(D_inv * B_mode)) + LogLikelihood(y_data, y_data_int, mode_new.data(), num_data);
+						}
+						else {
+#pragma omp parallel for schedule(static)
+							for (data_size_t i = 0; i < num_data; ++i) {// Update location parameter of log-likelihood for calculation of approx. marginal log-likelihood (objective function)
+								location_par[i] = mode_new[i] + fixed_effects[i];
+							}
+							approx_marginal_ll_new = -0.5 * (B_mode.dot(D_inv * B_mode)) + LogLikelihood(y_data, y_data_int, location_par.data(), num_data);
+						}
+						if (approx_marginal_ll_new < approx_marginal_ll ||
+							std::isnan(approx_marginal_ll_new) || std::isinf(approx_marginal_ll_new)) {
+							lr_GD *= 0.5;
+							nesterov_acc_rate *= 0.5;
+						}
+						else {//approx_marginal_ll_new >= approx_marginal_ll
+							mode_ = mode_new;
+							break;
+						}
+					}// end loop over learnig rate halving procedure
+					mode_after_grad_aux_lag1 = mode_after_grad_aux;
+				}//end quasi_newton_for_mode_finding_
+				else {//Newton's method
+					// Calculate Cholesky factor and update mode
+					rhs.array() = second_deriv_neg_ll_.array() * mode_.array() + first_deriv_ll_.array();//right hand side for updating mode
+					SigmaI_plus_W = SigmaI;
+					SigmaI_plus_W.diagonal().array() += second_deriv_neg_ll_.array();
+					SigmaI_plus_W.makeCompressed();
+					//Calculation of the Cholesky factor is the bottleneck
+					if (!chol_fact_pattern_analyzed_) {
+						chol_fact_SigmaI_plus_ZtWZ_vecchia_.analyzePattern(SigmaI_plus_W);
+						chol_fact_pattern_analyzed_ = true;
+					}
+					chol_fact_SigmaI_plus_ZtWZ_vecchia_.factorize(SigmaI_plus_W);//This is the bottleneck for large data
+					//Log::REInfo("SigmaI_plus_W: number non zeros = %d", (int)SigmaI_plus_W.nonZeros());//only for debugging
+					//Log::REInfo("chol_fact_SigmaI_plus_ZtWZ: Number non zeros = %d", (int)((sp_mat_t)chol_fact_SigmaI_plus_ZtWZ_vecchia_.matrixL()).nonZeros());//only for debugging
+					if (cap_change_mode_newton_) {
+						mode_new = chol_fact_SigmaI_plus_ZtWZ_vecchia_.solve(rhs);
+#pragma omp parallel for schedule(static)
+						for (data_size_t i = 0; i < num_data; ++i) {
+							double abs_change = std::abs(mode_new[i] - mode_[i]);
+							if (abs_change > MAX_CHANGE_MODE_NEWTON_) {
+								mode_[i] = mode_[i] + (mode_new[i] - mode_[i]) / abs_change * MAX_CHANGE_MODE_NEWTON_;
+							}
+							else {
+								mode_[i] = mode_new[i];
+							}
+						}
+					}//end cap_change_mode_newton_
+					else {
+						mode_ = chol_fact_SigmaI_plus_ZtWZ_vecchia_.solve(rhs);
+					}
+					// Calculate new objective function
+					B_mode = B * mode_;
+					if (no_fixed_effects) {
+						approx_marginal_ll_new = -0.5 * (B_mode.dot(D_inv * B_mode)) + LogLikelihood(y_data, y_data_int, mode_.data(), num_data);
+					}
+					else {
+						// Update location parameter of log-likelihood for calculation of approx. marginal log-likelihood (objective function)
+#pragma omp parallel for schedule(static)
+						for (data_size_t i = 0; i < num_data; ++i) {
+							location_par[i] = mode_[i] + fixed_effects[i];
+						}
+						approx_marginal_ll_new = -0.5 * (B_mode.dot(D_inv * B_mode)) + LogLikelihood(y_data, y_data_int, location_par.data(), num_data);
+					}
+				}//end Newton's method
+				if (std::isnan(approx_marginal_ll_new) || std::isinf(approx_marginal_ll_new)) {
+					has_NA_or_Inf = true;
+					Log::REDebug(NA_OR_INF_WARNING_);
+					break;
+				}
+				// Check convergence
+				if (it == 0) {
+					if (std::abs(approx_marginal_ll_new - approx_marginal_ll) < DELTA_REL_CONV_ * std::abs(approx_marginal_ll)) { // allow for decreases in first iteration
+						terminate_optim = true;
+					}
+				}
+				else {
+					if ((approx_marginal_ll_new - approx_marginal_ll) < DELTA_REL_CONV_ * std::abs(approx_marginal_ll)) {
+						terminate_optim = true;
+					}
+				}
+				if (terminate_optim) {
+					if (approx_marginal_ll_new < approx_marginal_ll) {
+						Log::REDebug(NO_INCREASE_IN_MLL_WARNING_);
+					}
+					approx_marginal_ll = approx_marginal_ll_new;
+					break;
+				}
+				else {
+					approx_marginal_ll = approx_marginal_ll_new;
+				}
+			} // end loop for mode finding
+			if (it == MAXIT_MODE_NEWTON_) {
+				Log::REDebug(NO_CONVERGENCE_WARNING_);
+			}
+			if (has_NA_or_Inf) {
+				approx_marginal_ll = approx_marginal_ll_new;
+				na_or_inf_during_last_call_to_find_mode_ = true;
+			}
+			else {
+				if (no_fixed_effects) {
+					CalcFirstDerivLogLik(y_data, y_data_int, mode_.data(), num_data);//first derivative is not used here anymore but since it is reused in gradient calculation and in prediction, we calculate it once more
+					CalcSecondDerivNegLogLik(y_data, y_data_int, mode_.data(), num_data);
+				}
+				else {
+					CalcFirstDerivLogLik(y_data, y_data_int, location_par.data(), num_data);//first derivative is not used here anymore but since it is reused in gradient calculation and in prediction, we calculate it once more
+					CalcSecondDerivNegLogLik(y_data, y_data_int, location_par.data(), num_data);
+				}
+				SigmaI_plus_W = SigmaI;
+				SigmaI_plus_W.diagonal().array() += second_deriv_neg_ll_.array();
+				SigmaI_plus_W.makeCompressed();
+				if (!chol_fact_pattern_analyzed_) {
+					chol_fact_SigmaI_plus_ZtWZ_vecchia_.analyzePattern(SigmaI_plus_W);
+					chol_fact_pattern_analyzed_ = true;
+				}
+				chol_fact_SigmaI_plus_ZtWZ_vecchia_.factorize(SigmaI_plus_W);
+				approx_marginal_ll += -((sp_mat_t)chol_fact_SigmaI_plus_ZtWZ_vecchia_.matrixL()).diagonal().array().log().sum() + 0.5 * D_inv.diagonal().array().log().sum();
+				mode_has_been_calculated_ = true;
+				na_or_inf_during_last_call_to_find_mode_ = false;
+			}
+		}//end FindModePostRandEffCalcMLLVecchia
+
+		/*!
+		* \brief Calculate the gradient of the negative Laplace-approximated marginal log-likelihood wrt covariance parameters,
+		*		fixed effects (e.g., for linear regression coefficients), and additional likelihood-related parameters.
+		*		Calculations are done using a numerically stable variant based on factorizing ("inverting") B = (Id + Wsqrt * Z*Sigma*Zt * Wsqrt).
+		*		In the notation of the paper: "Sigma = Z*Sigma*Z^T" and "Z = Id".
+		*		This version is used for the Laplace approximation when dense matrices are used (e.g. GP models).
+		* \param y_data Response variable data if response variable is continuous
+		* \param y_data_int Response variable data if response variable is integer-valued
+		* \param fixed_effects Fixed effects component of location parameter
+		* \param num_data Number of data points
+		* \param ZSigmaZt Covariance matrix of latent random effect
+		* \param re_comps_cluster_i Vector with different random effects components. We pass the component pointers to save memory in order to avoid passing a large collection of gardient covariance matrices in memory//TODO: better way than passing this? (relying on all gradients in a vector can lead to large memory consumption)
+		* \param calc_cov_grad If true, the gradient wrt the covariance parameters is calculated
+		* \param calc_F_grad If true, the gradient wrt the fixed effects mean function F is calculated
+		* \param calc_aux_par_grad If true, the gradient wrt additional likelihood parameters is calculated
+		* \param[out] cov_grad Gradient of approximate marginal log-likelihood wrt covariance parameters (needs to be preallocated of size num_cov_par)
+		* \param[out] fixed_effect_grad Gradient of approximate marginal log-likelihood wrt fixed effects F (note: this is passed as a Eigen vector in order to avoid the need for copying)
+		* \param[out] aux_par_grad Gradient wrt additional likelihood parameters
+		* \param calc_mode If true, the mode of the random effects posterior is calculated otherwise the values in mode and a_vec_ are used (default=false)
+		*/
+		void CalcGradNegMargLikelihoodLaplaceApproxStable(const double* y_data,
+			const int* y_data_int,
+			const double* fixed_effects,
+			const data_size_t num_data,
+			const std::shared_ptr<T_mat> ZSigmaZt,
+			const std::vector<std::shared_ptr<RECompBase<T_mat>>>& re_comps_cluster_i,
+			bool calc_cov_grad,
+			bool calc_F_grad,
+			bool calc_aux_par_grad,
+			double* cov_grad,
+			vec_t& fixed_effect_grad,
+			double* aux_par_grad,
+			bool calc_mode) {
+			if (calc_mode) {// Calculate mode and Cholesky factor of B = (Id + Wsqrt * ZSigmaZt * Wsqrt) at mode
+				double mll;//approximate marginal likelihood. This is a by-product that is not used here.
+				FindModePostRandEffCalcMLLStable(y_data, y_data_int, fixed_effects, num_data, ZSigmaZt, mll);
+			}
+			if (na_or_inf_during_last_call_to_find_mode_) {
+				Log::REFatal(NA_OR_INF_ERROR_);
+			}
+			CHECK(mode_has_been_calculated_);
+			// Initialize variables
+			bool no_fixed_effects = (fixed_effects == nullptr);
+			vec_t location_par;//location parameter = mode of random effects + fixed effects
+			double* location_par_ptr;
+			T_mat L_inv_Wsqrt(num_data, num_data);//diagonal matrix with square root of negative second derivatives on the diagonal (sqrt of negative Hessian of log-likelihood)
+			L_inv_Wsqrt.setIdentity();
+			L_inv_Wsqrt.diagonal().array() = second_deriv_neg_ll_.array().sqrt();
+			vec_t third_deriv(num_data);//vector of third derivatives of log-likelihood
+			if (no_fixed_effects) {
+				location_par_ptr = mode_.data();
+			}
+			else {
+				location_par = vec_t(num_data);
+#pragma omp parallel for schedule(static)
+				for (data_size_t i = 0; i < num_data; ++i) {
+					location_par[i] = mode_[i] + fixed_effects[i];
+				}
+				location_par_ptr = location_par.data();
+			}
+			CalcThirdDerivLogLik(y_data, y_data_int, location_par_ptr, num_data, third_deriv.data());
+			TriangularSolveGivenCholesky<T_chol, T_mat, T_mat, T_mat>(chol_fact_Id_plus_Wsqrt_Sigma_Wsqrt_, L_inv_Wsqrt, L_inv_Wsqrt, false);//L_inv_Wsqrt = L\Wsqrt
+			T_mat L_inv_Wsqrt_ZSigmaZt = L_inv_Wsqrt * (*ZSigmaZt);
+			// Calculate gradient of approx. marginal log-likelihood wrt the mode
+			//		Note: use (i) (Sigma^-1 + W)^-1 = Sigma - Sigma*(W^-1 + Sigma)^-1*Sigma = ZSigmaZt - L_inv_Wsqrt_ZSigmaZt^T*L_inv_Wsqrt_ZSigmaZt and (ii) "Z=Id"N
+			T_mat L_inv_Wsqrt_ZSigmaZt_sqr = L_inv_Wsqrt_ZSigmaZt.cwiseProduct(L_inv_Wsqrt_ZSigmaZt);
+			vec_t ZSigmaZtI_plus_W_inv_diag = (*ZSigmaZt).diagonal() - L_inv_Wsqrt_ZSigmaZt_sqr.transpose() * vec_t::Ones(L_inv_Wsqrt_ZSigmaZt_sqr.rows());// diagonal of (ZSigmaZt^-1 + W) ^ -1
+			vec_t d_mll_d_mode = (-0.5 * ZSigmaZtI_plus_W_inv_diag.array() * third_deriv.array()).matrix();// gradient of approx. marginal likelihood wrt the mode and thus also F here
+			// calculate gradient wrt covariance parameters
+			if (calc_cov_grad) {
+				T_mat WI_plus_Sigma_inv;//WI_plus_Sigma_inv = Wsqrt * L^T\(L\Wsqrt) = (W^-1 + Sigma)^-1
+				vec_t d_mode_d_par, SigmaDeriv_first_deriv_ll;
+				int par_count = 0;
+				double explicit_derivative;
+				for (int j = 0; j < (int)re_comps_cluster_i.size(); ++j) {
+					for (int ipar = 0; ipar < re_comps_cluster_i[j]->NumCovPar(); ++ipar) {
+						std::shared_ptr<T_mat> SigmaDeriv = re_comps_cluster_i[j]->GetZSigmaZtGrad(ipar, true, 1.);
+						if (ipar == 0) {
+							WI_plus_Sigma_inv = *SigmaDeriv;
+							CalcLtLGivenSparsityPattern<T_mat>(L_inv_Wsqrt, WI_plus_Sigma_inv, true);
+							//TODO (low-prio): calculate WI_plus_Sigma_inv only once for all relevant non-zero entries as in Gaussian case (see 'CalcPsiInv')
+							//					This is only relevant for multiple random effects and/or GPs
+						}
+						// calculate explicit derivative of approx. mariginal log-likelihood
+						explicit_derivative = -0.5 * (double)(a_vec_.transpose() * (*SigmaDeriv) * a_vec_) + 0.5 * (WI_plus_Sigma_inv.cwiseProduct(*SigmaDeriv)).sum();
+						// calculate implicit derivative (through mode) of approx. mariginal log-likelihood
+						SigmaDeriv_first_deriv_ll = (*SigmaDeriv) * first_deriv_ll_;//auxiliary variable for caclulating d_mode_d_par
+						d_mode_d_par = SigmaDeriv_first_deriv_ll;//derivative of mode wrt to a covariance parameter
+						d_mode_d_par -= ((*ZSigmaZt) * (L_inv_Wsqrt.transpose() * (L_inv_Wsqrt * SigmaDeriv_first_deriv_ll)));
+						cov_grad[par_count] = explicit_derivative + d_mll_d_mode.dot(d_mode_d_par);
+						par_count++;
+					}
+				}
+			}//end calc_cov_grad
+			// calculate gradient wrt fixed effects
+			vec_t ZSigmaZtI_plus_W_inv_d_mll_d_mode;// for implicit derivative
+			if (calc_F_grad || calc_aux_par_grad) {
+				vec_t L_inv_Wsqrt_ZSigmaZt_d_mll_d_mode = L_inv_Wsqrt_ZSigmaZt * d_mll_d_mode;// for implicit derivative
+				ZSigmaZtI_plus_W_inv_d_mll_d_mode = (*ZSigmaZt) * d_mll_d_mode - L_inv_Wsqrt_ZSigmaZt.transpose() * L_inv_Wsqrt_ZSigmaZt_d_mll_d_mode;
+			}
+			if (calc_F_grad) {
+				vec_t d_mll_d_F_implicit = (ZSigmaZtI_plus_W_inv_d_mll_d_mode.array() * second_deriv_neg_ll_.array()).matrix();// implicit derivative
+				fixed_effect_grad = -first_deriv_ll_ + d_mll_d_mode - d_mll_d_F_implicit;
+			}//end calc_F_grad
+			// calculate gradient wrt additional likelihood parameters
+			if (calc_aux_par_grad) {
+				vec_t neg_likelihood_deriv(num_aux_pars_);//derivative of the negative log-likelihood wrt additional parameters of the likelihood
+				vec_t second_deriv(num_data);//second derivative of the log-likelihood with respect to (i) the location parameter and (ii) an additional parameter of the likelihood
+				vec_t neg_third_deriv(num_data);//negative third derivative of the log-likelihood with respect to (i) two times the location parameter and (ii) an additional parameter of the likelihood
+				vec_t d_mode_d_aux_par;
+				CalcGradNegLogLikAuxPars(y_data, location_par_ptr, num_data, neg_likelihood_deriv.data());
+				for (int ind_ap = 0; ind_ap < num_aux_pars_; ++ind_ap) {
+					CalcSecondNegThirdDerivLogLikAuxParsLocPar(y_data, location_par_ptr, num_data, ind_ap, second_deriv.data(), neg_third_deriv.data());
+					double d_detmll_d_aux_par = 0., implicit_derivative = 0.;
+#pragma omp parallel for schedule(static) reduction(+:d_detmll_d_aux_par, implicit_derivative)
+					for (data_size_t i = 0; i < num_data; ++i) {
+						d_detmll_d_aux_par += neg_third_deriv[i] * ZSigmaZtI_plus_W_inv_diag[i];
+						implicit_derivative += second_deriv[i] * ZSigmaZtI_plus_W_inv_d_mll_d_mode[i];
+					}
+					aux_par_grad[ind_ap] = neg_likelihood_deriv[ind_ap] + 0.5 * d_detmll_d_aux_par + implicit_derivative;
+				}
+			}//end calc_aux_par_grad
+		}//end CalcGradNegMargLikelihoodLaplaceApproxStable
+
+		/*!
+		* \brief Calculate the gradient of the negative Laplace-approximated marginal log-likelihood wrt covariance parameters,
+		*		fixed effects (e.g., for linear regression coefficients), and additional likelihood-related parameters.
+		*		Calculations are done on the random effects (b) scale and not the "data scale" (Zb) using
+		*		a numerically stable variant based on factorizing ("inverting") B = (Id + ZtWZsqrt * Sigma * ZtWZsqrt).
+		*		This version is used for the Laplace approximation when there is only one Gaussian process and
+		*		there are a lot of multiple observations at the same location, i.e., the dimenion of the random effects b is much smaller than Zb
+		* \param y_data Response variable data if response variable is continuous
+		* \param y_data_int Response variable data if response variable is integer-valued
+		* \param fixed_effects Fixed effects component of location parameter
+		* \param num_data Number of data points
+		* \param Sigma Covariance matrix of latent random effect
+		* \param random_effects_indices_of_data Indices that indicate to which random effect every data point is related
+		* \param re_comps_cluster_i Vector with different random effects components. We pass the component pointers to save memory in order to avoid passing a large collection of gardient covariance matrices in memory//TODO: better way than passing this? (relying on all gradients in a vector can lead to large memory consumption)
+		* \param calc_cov_grad If true, the gradient wrt the covariance parameters is calculated
+		* \param calc_F_grad If true, the gradient wrt the fixed effects mean function F is calculated
+		* \param calc_aux_par_grad If true, the gradient wrt additional likelihood parameters is calculated
+		* \param[out] cov_grad Gradient of approximate marginal log-likelihood wrt covariance parameters (needs to be preallocated of size num_cov_par)
+		* \param[out] fixed_effect_grad Gradient of approximate marginal log-likelihood wrt fixed effects F (note: this is passed as a Eigen vector in order to avoid the need for copying)
+		* \param[out] aux_par_grad Gradient wrt additional likelihood parameters
+		* \param calc_mode If true, the mode of the random effects posterior is calculated otherwise the values in mode and a_vec_ are used (default=false)
+		*/
+		void CalcGradNegMargLikelihoodLaplaceApproxOnlyOneGPCalculationsOnREScale(const double* y_data,
+			const int* y_data_int,
+			const double* fixed_effects,
+			const data_size_t num_data,
+			const std::shared_ptr<T_mat> Sigma,
+			const data_size_t* const random_effects_indices_of_data,
+			const std::vector<std::shared_ptr<RECompBase<T_mat>>>& re_comps_cluster_i,
+			bool calc_cov_grad,
+			bool calc_F_grad,
+			bool calc_aux_par_grad,
+			double* cov_grad,
+			vec_t& fixed_effect_grad,
+			double* aux_par_grad,
+			bool calc_mode) {
+			CHECK(re_comps_cluster_i.size() == 1);
+			if (calc_mode) {// Calculate mode and Cholesky factor of B = (Id + Wsqrt * ZSigmaZt * Wsqrt) at mode
+				double mll;//approximate marginal likelihood. This is a by-product that is not used here.
+				FindModePostRandEffCalcMLLOnlyOneGPCalculationsOnREScale(y_data, y_data_int, fixed_effects, num_data,
+					Sigma, random_effects_indices_of_data, mll);
+			}
+			if (na_or_inf_during_last_call_to_find_mode_) {
+				Log::REFatal(NA_OR_INF_ERROR_);
+			}
+			CHECK(mode_has_been_calculated_);
+			// Initialize variables
+			vec_t location_par(num_data);//location parameter = mode of random effects + fixed effects
+			if (fixed_effects == nullptr) {
+#pragma omp parallel for schedule(static)
+				for (data_size_t i = 0; i < num_data; ++i) {
+					location_par[i] = mode_[random_effects_indices_of_data[i]];
+				}
+			}
+			else {
+#pragma omp parallel for schedule(static)
+				for (data_size_t i = 0; i < num_data; ++i) {
+					location_par[i] = mode_[random_effects_indices_of_data[i]] + fixed_effects[i];
+				}
+			}
+			// Matrix ZtWZsqrt
+			vec_t diag_ZtWZ;
+			CalcZtVGivenIndices(num_data, num_re_, random_effects_indices_of_data, second_deriv_neg_ll_, diag_ZtWZ, true);
+			T_mat L_inv_ZtWZsqrt(num_re_, num_re_);//diagonal matrix with square root of diagonal of ZtWZ
+			L_inv_ZtWZsqrt.setIdentity();
+			L_inv_ZtWZsqrt.diagonal().array() = diag_ZtWZ.array().sqrt();
+			vec_t third_deriv(num_data);//vector of third derivatives of log-likelihood
+			CalcThirdDerivLogLik(y_data, y_data_int, location_par.data(), num_data, third_deriv.data());
+			vec_t diag_ZtThirdDerivZ;
+			CalcZtVGivenIndices(num_data, num_re_, random_effects_indices_of_data, third_deriv, diag_ZtThirdDerivZ, true);
+			TriangularSolveGivenCholesky<T_chol, T_mat, T_mat, T_mat>(chol_fact_Id_plus_Wsqrt_Sigma_Wsqrt_, L_inv_ZtWZsqrt, L_inv_ZtWZsqrt, false);//L_inv_ZtWZsqrt = L\ZtWZsqrt
+			T_mat L_inv_ZtWZsqrt_Sigma = L_inv_ZtWZsqrt * (*Sigma);
+			//Log::REInfo("CalcGradNegMargLikelihoodLaplaceApproxOnlyOneGPCalculationsOnREScale: L_inv_ZtWZsqrt: number non zeros = %d", GetNumberNonZeros<T_mat>(L_inv_ZtWZsqrt));//Only for debugging
+			//Log::REInfo("CalcGradNegMargLikelihoodLaplaceApproxOnlyOneGPCalculationsOnREScale: L_inv_ZtWZsqrt_Sigma: number non zeros = %d", GetNumberNonZeros<T_mat>(L_inv_ZtWZsqrt_Sigma));//Only for debugging
+			// Calculate gradient of approx. marginal log-likelihood wrt the mode
+			//		Note: use (i) (Sigma^-1 + W)^-1 = Sigma - Sigma*(W^-1 + Sigma)^-1*Sigma = ZSigmaZt - L_inv_ZtWZsqrt_Sigma^T*L_inv_ZtWZsqrt_Sigma
+			T_mat L_inv_ZtWZsqrt_Sigma_sqr = L_inv_ZtWZsqrt_Sigma.cwiseProduct(L_inv_ZtWZsqrt_Sigma);
+			vec_t SigmaI_plus_ZtWZ_inv_diag = (*Sigma).diagonal() - L_inv_ZtWZsqrt_Sigma_sqr.transpose() * vec_t::Ones(L_inv_ZtWZsqrt_Sigma_sqr.rows());// diagonal of (Sigma^-1 + ZtWZ) ^ -1
+			vec_t d_mll_d_mode = (-0.5 * SigmaI_plus_ZtWZ_inv_diag.array() * diag_ZtThirdDerivZ.array()).matrix();// gradient of approx. marginal likelihood wrt the mode
+			// calculate gradient wrt covariance parameters
+			if (calc_cov_grad) {
+				vec_t ZtFirstDeriv;
+				CalcZtVGivenIndices(num_data, num_re_, random_effects_indices_of_data, first_deriv_ll_, ZtFirstDeriv, true);
+				T_mat ZtWZI_Sigma_inv;//ZtWZI_Sigma_inv = ZtWZsqrt * L^T\(L\ZtWZsqrt) = ((ZtWZ)^-1 + Sigma)^-1
+				vec_t d_mode_d_par, SigmaDeriv_ZtFirstDeriv;
+				int par_count = 0;
+				double explicit_derivative;
+				for (int j = 0; j < (int)re_comps_cluster_i.size(); ++j) {
+					for (int ipar = 0; ipar < re_comps_cluster_i[j]->NumCovPar(); ++ipar) {
+						std::shared_ptr<T_mat> SigmaDeriv = re_comps_cluster_i[j]->GetZSigmaZtGrad(ipar, true, 1.);
+						if (ipar == 0) {
+							ZtWZI_Sigma_inv = *SigmaDeriv;
+							CalcLtLGivenSparsityPattern<T_mat>(L_inv_ZtWZsqrt, ZtWZI_Sigma_inv, true);
+							//TODO (low-prio): calculate ZtWZI_Sigma_inv only once for all relevant non-zero entries as in Gaussian case (see 'CalcPsiInv')
+							//					This is only relevant for multiple random effects and/or GPs
+						}
+						// calculate explicit derivative of approx. mariginal log-likelihood
+						explicit_derivative = -0.5 * (double)(a_vec_.transpose() * (*SigmaDeriv) * a_vec_) +
+							0.5 * (ZtWZI_Sigma_inv.cwiseProduct(*SigmaDeriv)).sum();
+						// calculate implicit derivative (through mode) of approx. mariginal log-likelihood
+						SigmaDeriv_ZtFirstDeriv = (*SigmaDeriv) * ZtFirstDeriv;//auxiliary variable for caclulating d_mode_d_par
+						d_mode_d_par = SigmaDeriv_ZtFirstDeriv;//derivative of mode wrt to a covariance parameter
+						d_mode_d_par -= ((*Sigma) * (L_inv_ZtWZsqrt.transpose() * (L_inv_ZtWZsqrt * SigmaDeriv_ZtFirstDeriv)));
+						cov_grad[par_count] = explicit_derivative + d_mll_d_mode.dot(d_mode_d_par);
+						par_count++;
+					}
+				}
+			}//end calc_cov_grad
+			// calculate gradient wrt fixed effects
+			vec_t SigmaI_plus_ZtWZ_inv_d_mll_d_mode;// for implicit derivative
+			if (calc_F_grad || calc_aux_par_grad) {
+				vec_t L_inv_ZtWZsqrt_Sigma_d_mll_d_mode = L_inv_ZtWZsqrt_Sigma * d_mll_d_mode;
+				SigmaI_plus_ZtWZ_inv_d_mll_d_mode = (*Sigma) * d_mll_d_mode - L_inv_ZtWZsqrt_Sigma.transpose() * L_inv_ZtWZsqrt_Sigma_d_mll_d_mode;
+			}
+			if (calc_F_grad) {
+				fixed_effect_grad = -first_deriv_ll_;
+#pragma omp parallel for schedule(static)
+				for (data_size_t i = 0; i < num_data; ++i) {
+					fixed_effect_grad[i] += -0.5 * third_deriv[i] * SigmaI_plus_ZtWZ_inv_diag[random_effects_indices_of_data[i]] -
+						second_deriv_neg_ll_[i] * SigmaI_plus_ZtWZ_inv_d_mll_d_mode[random_effects_indices_of_data[i]];
+				}
+			}//end calc_F_grad
+			// calculate gradient wrt additional likelihood parameters
+			if (calc_aux_par_grad) {
+				vec_t neg_likelihood_deriv(num_aux_pars_);//derivative of the negative log-likelihood wrt additional parameters of the likelihood
+				vec_t second_deriv(num_data);//second derivative of the log-likelihood with respect to (i) the location parameter and (ii) an additional parameter of the likelihood
+				vec_t neg_third_deriv(num_data);//negative third derivative of the log-likelihood with respect to (i) two times the location parameter and (ii) an additional parameter of the likelihood
+				vec_t d_mode_d_aux_par;
+				CalcGradNegLogLikAuxPars(y_data, location_par.data(), num_data, neg_likelihood_deriv.data());
+				for (int ind_ap = 0; ind_ap < num_aux_pars_; ++ind_ap) {
+					CalcSecondNegThirdDerivLogLikAuxParsLocPar(y_data, location_par.data(), num_data, ind_ap, second_deriv.data(), neg_third_deriv.data());
+					double d_detmll_d_aux_par = 0., implicit_derivative = 0.;
+#pragma omp parallel for schedule(static) reduction(+:d_detmll_d_aux_par, implicit_derivative)
+					for (data_size_t i = 0; i < num_data; ++i) {
+						d_detmll_d_aux_par += neg_third_deriv[i] * SigmaI_plus_ZtWZ_inv_diag[random_effects_indices_of_data[i]];
+						implicit_derivative += second_deriv[i] * SigmaI_plus_ZtWZ_inv_d_mll_d_mode[random_effects_indices_of_data[i]];
+					}
+					aux_par_grad[ind_ap] = neg_likelihood_deriv[ind_ap] + 0.5 * d_detmll_d_aux_par + implicit_derivative;
+				}
+			}//end calc_aux_par_grad
+		}//end CalcGradNegMargLikelihoodLaplaceApproxOnlyOneGPCalculationsOnREScale
+
+		/*!
+		* \brief Calculate the gradient of the negative Laplace-approximated marginal log-likelihood wrt covariance parameters,
+		*		fixed effects (e.g., for linear regression coefficients), and additional likelihood-related parameters.
+		*		Calculations are done by directly factorizing ("inverting) (Sigma^-1 + Zt*W*Z).
+		*		NOTE: IT IS ASSUMED THAT SIGMA IS A DIAGONAL MATRIX
+		*		This version is used for the Laplace approximation when there are only grouped random effects.
+		* \param y_data Response variable data if response variable is continuous
+		* \param y_data_int Response variable data if response variable is integer-valued
+		* \param fixed_effects Fixed effects component of location parameter
+		* \param num_data Number of data points
+		* \param SigmaI Inverse covariance matrix of latent random effect. Currently, this needs to be a diagonal matrix
+		* \param Zt Transpose Z^T of random effect design matrix that relates latent random effects to observations/likelihoods
+		* \param calc_cov_grad If true, the gradient wrt the covariance parameters is calculated
+		* \param calc_F_grad If true, the gradient wrt the fixed effects mean function F is calculated
+		* \param calc_aux_par_grad If true, the gradient wrt additional likelihood parameters is calculated
+		* \param[out] cov_grad Gradient wrt covariance parameters (needs to be preallocated of size num_cov_par)
+		* \param[out] fixed_effect_grad Gradient wrt fixed effects F (note: this is passed as a Eigen vector in order to avoid the need for copying)
+		* \param[out] aux_par_grad Gradient wrt additional likelihood parameters
+		* \param calc_mode If true, the mode of the random effects posterior is calculated otherwise the values in mode and a_vec_ are used (default=false)
+		*/
+		void CalcGradNegMargLikelihoodLaplaceApproxGroupedRE(const double* y_data,
+			const int* y_data_int,
+			const double* fixed_effects,
+			const data_size_t num_data,
+			const sp_mat_t& SigmaI,
+			const sp_mat_t& Zt,
+			std::vector<data_size_t> cum_num_rand_eff_cluster_i,
+			bool calc_cov_grad,
+			bool calc_F_grad,
+			bool calc_aux_par_grad,
+			double* cov_grad,
+			vec_t& fixed_effect_grad,
+			double* aux_par_grad,
+			bool calc_mode) {
+			int num_REs = (int)SigmaI.cols();//number of random effect realizations
+			int num_comps = (int)cum_num_rand_eff_cluster_i.size() - 1;//number of different random effect components
+			if (calc_mode) {// Calculate mode and Cholesky factor of Sigma^-1 + W at mode
+				double mll;//approximate marginal likelihood. This is a by-product that is not used here.
+				FindModePostRandEffCalcMLLGroupedRE(y_data, y_data_int, fixed_effects, num_data, SigmaI, Zt, mll);
+			}
+			if (na_or_inf_during_last_call_to_find_mode_) {
+				Log::REFatal(NA_OR_INF_ERROR_);
+			}
+			CHECK(mode_has_been_calculated_);
+			// Initialize variables
+			sp_mat_t Z = Zt.transpose();
+			vec_t location_par = Z * mode_;//location parameter = mode of random effects + fixed effects
+			if (fixed_effects != nullptr) {
+#pragma omp parallel for schedule(static)
+				for (data_size_t i = 0; i < num_data; ++i) {
+					location_par[i] += fixed_effects[i];
+				}
+			}
+			vec_t third_deriv(num_data);//vector of third derivatives of log-likelihood
+			CalcThirdDerivLogLik(y_data, y_data_int, location_par.data(), num_data, third_deriv.data());
+			// Calculate (Sigma^-1 + Zt*W*Z)^-1
+			sp_mat_t L_inv(num_REs, num_REs);
+			L_inv.setIdentity();
+			if (chol_fact_SigmaI_plus_ZtWZ_grouped_.permutationP().size() > 0) {//Permutation is only used when having an ordering
+				L_inv = chol_fact_SigmaI_plus_ZtWZ_grouped_.permutationP() * L_inv;
+			}
+			sp_mat_t L = chol_fact_SigmaI_plus_ZtWZ_grouped_.matrixL();
+			TriangularSolve<sp_mat_t, sp_mat_t, sp_mat_t>(L, L_inv, L_inv, false);
+			L.resize(0, 0);
+			sp_mat_t SigmaI_plus_ZtWZ_inv;
+			// calculate gradient of approx. marginal likelihood wrt the mode
+			vec_t d_mll_d_mode(num_REs);
+			sp_mat_t Zt_third_deriv = Zt * third_deriv.asDiagonal();//every column of Z multiplied elementwise by third_deriv
+#pragma omp parallel for schedule(static)
+			for (int ire = 0; ire < num_REs; ++ire) {
+				//calculate Z^T * diag(diag_d_W_d_mode_i) * Z = Z^T * diag(Z.col(i) * third_deriv) * Z
+				d_mll_d_mode[ire] = 0.;
+				double entry_ij;
+				for (data_size_t i = 0; i < num_data; ++i) {
+					entry_ij = Zt_third_deriv.coeff(ire, i);
+					if (std::abs(entry_ij) > EPSILON_NUMBERS) {
+						vec_t L_inv_Zt_col_i = L_inv * Zt.col(i);
+						d_mll_d_mode[ire] += entry_ij * (L_inv_Zt_col_i.squaredNorm());
+					}
+				}
+				d_mll_d_mode[ire] *= -0.5;
+			}
+			// calculate gradient wrt covariance parameters
+			if (calc_cov_grad) {
+				sp_mat_t ZtWZ = Zt * second_deriv_neg_ll_.asDiagonal() * Z;
+				vec_t d_mode_d_par;//derivative of mode wrt to a covariance parameter
+				vec_t v_aux;//auxiliary variable for caclulating d_mode_d_par
+				vec_t SigmaI_mode = SigmaI * mode_;
+				double explicit_derivative;
+				sp_mat_t I_j(num_REs, num_REs);//Diagonal matrix with 1 on the diagonal for all random effects of component j and 0's otherwise
+				sp_mat_t I_j_ZtWZ;
+				for (int j = 0; j < num_comps; ++j) {
+					// calculate explicit derivative of approx. mariginal log-likelihood
+					std::vector<Triplet_t> triplets(cum_num_rand_eff_cluster_i[j + 1] - cum_num_rand_eff_cluster_i[j]);//for constructing I_j
+					explicit_derivative = 0.;
+#pragma omp parallel for schedule(static) reduction(+:explicit_derivative)
+					for (int i = cum_num_rand_eff_cluster_i[j]; i < cum_num_rand_eff_cluster_i[j + 1]; ++i) {
+						triplets[i - cum_num_rand_eff_cluster_i[j]] = Triplet_t(i, i, 1.);
+						explicit_derivative += SigmaI_mode[i] * mode_[i];
+					}
+					explicit_derivative *= -0.5;
+					I_j.setFromTriplets(triplets.begin(), triplets.end());
+					I_j_ZtWZ = I_j * ZtWZ;
+					SigmaI_plus_ZtWZ_inv = I_j_ZtWZ;
+					CalcLtLGivenSparsityPattern<sp_mat_t>(L_inv, SigmaI_plus_ZtWZ_inv, false);
+					explicit_derivative += 0.5 * (SigmaI_plus_ZtWZ_inv.cwiseProduct(I_j_ZtWZ)).sum();
+					// calculate implicit derivative (through mode) of approx. mariginal log-likelihood
+					d_mode_d_par = L_inv.transpose() * (L_inv * (I_j * (Zt * first_deriv_ll_)));
+					cov_grad[j] = explicit_derivative + d_mll_d_mode.dot(d_mode_d_par);
+				}
+			}//end calc_cov_grad
+			// calculate gradient wrt fixed effects
+			if (calc_F_grad) {
+				vec_t d_detmll_d_F(num_data);
+#pragma omp parallel for schedule(static)
+				for (int i = 0; i < num_data; ++i) {
+					vec_t L_inv_Zt_col_i = L_inv * Zt.col(i);
+					d_detmll_d_F[i] = -0.5 * third_deriv[i] * (L_inv_Zt_col_i.squaredNorm());
+
+				}
+				vec_t d_mll_d_modeT_SigmaI_plus_ZtWZ_inv_Zt_W = (((d_mll_d_mode.transpose() * L_inv.transpose()) * L_inv) * Zt) * second_deriv_neg_ll_.asDiagonal();
+				fixed_effect_grad = -first_deriv_ll_ + d_detmll_d_F - d_mll_d_modeT_SigmaI_plus_ZtWZ_inv_Zt_W;
+			}//end calc_F_grad
+			// calculate gradient wrt additional likelihood parameters
+			if (calc_aux_par_grad) {
+				vec_t neg_likelihood_deriv(num_aux_pars_);//derivative of the negative log-likelihood wrt additional parameters of the likelihood
+				vec_t second_deriv(num_data);//second derivative of the log-likelihood with respect to (i) the location parameter and (ii) an additional parameter of the likelihood
+				vec_t neg_third_deriv(num_data);//negative third derivative of the log-likelihood with respect to (i) two times the location parameter and (ii) an additional parameter of the likelihood
+				vec_t d_mode_d_aux_par;
+				CalcGradNegLogLikAuxPars(y_data, location_par.data(), num_data, neg_likelihood_deriv.data());
+				for (int ind_ap = 0; ind_ap < num_aux_pars_; ++ind_ap) {
+					CalcSecondNegThirdDerivLogLikAuxParsLocPar(y_data, location_par.data(), num_data, ind_ap, second_deriv.data(), neg_third_deriv.data());
+					sp_mat_t ZtdWZ = Zt * neg_third_deriv.asDiagonal() * Z;
+					SigmaI_plus_ZtWZ_inv = ZtdWZ;
+					CalcLtLGivenSparsityPattern<sp_mat_t>(L_inv, SigmaI_plus_ZtWZ_inv, false);
+					double d_detmll_d_aux_par = (SigmaI_plus_ZtWZ_inv.cwiseProduct(ZtdWZ)).sum();
+					d_mode_d_aux_par = L_inv.transpose() * (L_inv * (Zt * second_deriv));
+					double implicit_derivative = d_mll_d_mode.dot(d_mode_d_aux_par);
+					aux_par_grad[ind_ap] = neg_likelihood_deriv[ind_ap] + 0.5 * d_detmll_d_aux_par + implicit_derivative;
+				}
+			}//end calc_aux_par_grad
+		}//end CalcGradNegMargLikelihoodLaplaceApproxGroupedRE
+
+		/*!
+		* \brief Calculate the gradient of the negative Laplace-approximated marginal log-likelihood wrt covariance parameters,
+		*		fixed effects (e.g., for linear regression coefficients), and additional likelihood-related parameters.
+		*		Calculations are done by directly factorizing ("inverting) (Sigma^-1 + Zt*W*Z).
+		*		This version is used for the Laplace approximation when there are only grouped random effects with only one grouping variable.
+		* \param y_data Response variable data if response variable is continuous
+		* \param y_data_int Response variable data if response variable is integer-valued
+		* \param fixed_effects Fixed effects component of location parameter
+		* \param num_data Number of data points
+		* \param sigma2 Variance of random effects
+		* \param random_effects_indices_of_data Indices that indicate to which random effect every data point is related
+		* \param calc_cov_grad If true, the gradient wrt the covariance parameters is calculated
+		* \param calc_F_grad If true, the gradient wrt the fixed effects mean function F is calculated
+		* \param calc_aux_par_grad If true, the gradient wrt additional likelihood parameters is calculated
+		* \param[out] cov_grad Gradient wrt covariance parameters (needs to be preallocated of size num_cov_par)
+		* \param[out] fixed_effect_grad Gradient wrt fixed effects F (note: this is passed as a Eigen vector in order to avoid the need for copying)
+		* \param[out] aux_par_grad Gradient wrt additional likelihood parameters
+		* \param calc_mode If true, the mode of the random effects posterior is calculated otherwise the values in mode and a_vec_ are used (default=false)
+		*/
+		void CalcGradNegMargLikelihoodLaplaceApproxOnlyOneGroupedRECalculationsOnREScale(const double* y_data,
+			const int* y_data_int,
+			const double* fixed_effects,
+			const data_size_t num_data,
+			const double sigma2,
+			const data_size_t* const random_effects_indices_of_data,
+			bool calc_cov_grad,
+			bool calc_F_grad,
+			bool calc_aux_par_grad,
+			double* cov_grad,
+			vec_t& fixed_effect_grad,
+			double* aux_par_grad,
+			bool calc_mode) {
+			if (calc_mode) {// Calculate mode and Cholesky factor of Sigma^-1 + W at mode
+				double mll;//approximate marginal likelihood. This is a by-product that is not used here.
+				FindModePostRandEffCalcMLLOnlyOneGroupedRECalculationsOnREScale(y_data, y_data_int, fixed_effects, num_data,
+					sigma2, random_effects_indices_of_data, mll);
+			}
+			if (na_or_inf_during_last_call_to_find_mode_) {
+				Log::REFatal(NA_OR_INF_ERROR_);
+			}
+			CHECK(mode_has_been_calculated_);
+			// Initialize variables
+			vec_t location_par(num_data);//location parameter = mode of random effects + fixed effects
+			if (fixed_effects == nullptr) {
+#pragma omp parallel for schedule(static)
+				for (data_size_t i = 0; i < num_data; ++i) {
+					location_par[i] = mode_[random_effects_indices_of_data[i]];
+				}
+			}
+			else {
+#pragma omp parallel for schedule(static)
+				for (data_size_t i = 0; i < num_data; ++i) {
+					location_par[i] = mode_[random_effects_indices_of_data[i]] + fixed_effects[i];
+				}
+			}
+			vec_t third_deriv(num_data);//vector of third derivatives of log-likelihood
+			CalcThirdDerivLogLik(y_data, y_data_int, location_par.data(), num_data, third_deriv.data());
+			// calculate gradient of approx. marginal likelihood wrt the mode
+			vec_t d_mll_d_mode;
+			CalcZtVGivenIndices(num_data, num_re_, random_effects_indices_of_data, third_deriv, d_mll_d_mode, true);
+			d_mll_d_mode.array() /= -2. * diag_SigmaI_plus_ZtWZ_.array();
+			// calculate gradient wrt covariance parameters
+			if (calc_cov_grad) {
+				vec_t diag_ZtWZ;
+				CalcZtVGivenIndices(num_data, num_re_, random_effects_indices_of_data, second_deriv_neg_ll_, diag_ZtWZ, true);
+				double explicit_derivative = -0.5 * (mode_.array() * mode_.array()).sum() / sigma2 +
+					0.5 * (diag_ZtWZ.array() / diag_SigmaI_plus_ZtWZ_.array()).sum();
+				// calculate implicit derivative (through mode) of approx. mariginal log-likelihood
+				vec_t d_mode_d_par;
+				CalcZtVGivenIndices(num_data, num_re_, random_effects_indices_of_data, first_deriv_ll_, d_mode_d_par, true);
+				d_mode_d_par.array() /= diag_SigmaI_plus_ZtWZ_.array();
+				cov_grad[0] = explicit_derivative + d_mll_d_mode.dot(d_mode_d_par);
+			}//end calc_cov_grad
+			// calculate gradient wrt fixed effects
+			if (calc_F_grad) {
+#pragma omp parallel for schedule(static)
+				for (int i = 0; i < num_data; ++i) {
+					fixed_effect_grad[i] = -first_deriv_ll_[i] -
+						0.5 * third_deriv[i] / diag_SigmaI_plus_ZtWZ_[random_effects_indices_of_data[i]] - //=d_detmll_d_F
+						d_mll_d_mode[random_effects_indices_of_data[i]] * second_deriv_neg_ll_[i] / diag_SigmaI_plus_ZtWZ_[random_effects_indices_of_data[i]];//=implicit derivative = d_mll_d_mode * d_mode_d_F
+				}
+			}//end calc_F_grad
+			// calculate gradient wrt additional likelihood parameters
+			if (calc_aux_par_grad) {
+				vec_t neg_likelihood_deriv(num_aux_pars_);//derivative of the negative log-likelihood wrt additional parameters of the likelihood
+				vec_t second_deriv(num_data);//second derivative of the log-likelihood with respect to (i) the location parameter and (ii) an additional parameter of the likelihood
+				vec_t neg_third_deriv(num_data);//negative third derivative of the log-likelihood with respect to (i) two times the location parameter and (ii) an additional parameter of the likelihood
+				CalcGradNegLogLikAuxPars(y_data, location_par.data(), num_data, neg_likelihood_deriv.data());
+				for (int ind_ap = 0; ind_ap < num_aux_pars_; ++ind_ap) {
+					CalcSecondNegThirdDerivLogLikAuxParsLocPar(y_data, location_par.data(), num_data, ind_ap, second_deriv.data(), neg_third_deriv.data());
+					double d_detmll_d_aux_par = 0.;
+					double implicit_derivative = 0.;// = implicit derivative = d_mll_d_mode * d_mode_d_aux_par
+#pragma omp parallel for schedule(static) reduction(+:d_detmll_d_aux_par, implicit_derivative)
+					for (int i = 0; i < num_data; ++i) {
+						d_detmll_d_aux_par += neg_third_deriv[i] / diag_SigmaI_plus_ZtWZ_[random_effects_indices_of_data[i]];
+						implicit_derivative += d_mll_d_mode[random_effects_indices_of_data[i]] * second_deriv[i] / diag_SigmaI_plus_ZtWZ_[random_effects_indices_of_data[i]];
+					}
+					aux_par_grad[ind_ap] = neg_likelihood_deriv[ind_ap] + 0.5 * d_detmll_d_aux_par + implicit_derivative;
+					//Equivalent code:
+					//vec_t Zt_second_deriv, diag_Zt_neg_third_deriv_Z;
+					//CalcZtVGivenIndices(num_data, num_re_, random_effects_indices_of_data, second_deriv, Zt_second_deriv, true);
+					//CalcZtVGivenIndices(num_data, num_re_, random_effects_indices_of_data, neg_third_deriv, diag_Zt_neg_third_deriv_Z, true);
+					//double d_detmll_d_aux_par = (diag_Zt_neg_third_deriv_Z.array() / diag_SigmaI_plus_ZtWZ_.array()).sum();
+					//double implicit_derivative = (d_mll_d_mode.array() * Zt_second_deriv.array() / diag_SigmaI_plus_ZtWZ_.array()).sum();
+				}
+			}//end calc_aux_par_grad
+		}//end CalcGradNegMargLikelihoodLaplaceApproxOnlyOneGroupedRECalculationsOnREScale
+
+		/*!
+		* \brief Calculate the gradient of the negative Laplace-approximated marginal log-likelihood wrt covariance parameters,
+		*		fixed effects (e.g., for linear regression coefficients), and additional likelihood-related parameters.
+		*		Calculations are done by factorizing ("inverting) (Sigma^-1 + W) where it is assumed that an approximate Cholesky factor
+		*		of Sigma^-1 has previously been calculated using a Vecchia approximation.
+		*		This version is used for the Laplace approximation when there are only GP random effects and the Vecchia approximation is used.
+		*		Caveat: Sigma^-1 + W can be not very sparse
+		* \param y_data Response variable data if response variable is continuous
+		* \param y_data_int Response variable data if response variable is integer-valued
+		* \param fixed_effects Fixed effects component of location parameter
+		* \param num_data Number of data points
+		* \param B Matrix B in Vecchia approximation Sigma^-1 = B^T D^-1 B ("=" Cholesky factor)
+		* \param D_inv Diagonal matrix D^-1 in Vecchia approximation Sigma^-1 = B^T D^-1 B
+		* \param B_grad Derivatives of matrices B ( = derivative of matrix -A) for Vecchia approximation
+		* \param D_grad Derivatives of matrices D for Vecchia approximation
+		* \param calc_cov_grad If true, the gradient wrt the covariance parameters is calculated
+		* \param calc_F_grad If true, the gradient wrt the fixed effects mean function F is calculated
+		* \param calc_aux_par_grad If true, the gradient wrt additional likelihood parameters is calculated
+		* \param[out] cov_grad Gradient of approximate marginal log-likelihood wrt covariance parameters (needs to be preallocated of size num_cov_par)
+		* \param[out] fixed_effect_grad Gradient of approximate marginal log-likelihood wrt fixed effects F (note: this is passed as a Eigen vector in order to avoid the need for copying)
+		* \param[out] aux_par_grad Gradient wrt additional likelihood parameters
+		* \param calc_mode If true, the mode of the random effects posterior is calculated otherwise the values in mode and a_vec_ are used (default=false)
+		* \param num_comps_total Total number of random effect components ( = number of GPs)
+		*/
+		void CalcGradNegMargLikelihoodLaplaceApproxVecchia(const double* y_data,
+			const int* y_data_int,
+			const double* fixed_effects,
+			const data_size_t num_data,
+			const sp_mat_t& B,
+			const sp_mat_t& D_inv,
+			const std::vector<sp_mat_t>& B_grad,
+			const std::vector<sp_mat_t>& D_grad,
+			bool calc_cov_grad,
+			bool calc_F_grad,
+			bool calc_aux_par_grad,
+			double* cov_grad,
+			vec_t& fixed_effect_grad,
+			double* aux_par_grad,
+			bool calc_mode,
+			int num_comps_total) {
+			if (calc_mode) {// Calculate mode and Cholesky factor of Sigma^-1 + W at mode
+				double mll;//approximate marginal likelihood. This is a by-product that is not used here.
+				FindModePostRandEffCalcMLLVecchia(y_data, y_data_int, fixed_effects, num_data, B, D_inv, mll);
+			}
+			if (na_or_inf_during_last_call_to_find_mode_) {
+				Log::REFatal(NA_OR_INF_ERROR_);
+			}
+			CHECK(mode_has_been_calculated_);
+			// Initialize variables
+			bool no_fixed_effects = (fixed_effects == nullptr);
+			vec_t location_par;//location parameter = mode of random effects + fixed effects
+			double* location_par_ptr;
+			vec_t third_deriv(num_data);//vector of third derivatives of log-likelihood
+			if (no_fixed_effects) {
+				location_par_ptr = mode_.data();
+			}
+			else {
+				location_par = vec_t(num_data);
+#pragma omp parallel for schedule(static)
+				for (data_size_t i = 0; i < num_data; ++i) {
+					location_par[i] = mode_[i] + fixed_effects[i];
+				}
+				location_par_ptr = location_par.data();
+			}
+			CalcThirdDerivLogLik(y_data, y_data_int, location_par_ptr, num_data, third_deriv.data());
+			// Calculate (Sigma^-1 + W)^-1
+			sp_mat_t L_inv(num_data, num_data);
+			L_inv.setIdentity();
+			TriangularSolveGivenCholesky<chol_sp_mat_t, sp_mat_t, sp_mat_t, sp_mat_t>(chol_fact_SigmaI_plus_ZtWZ_vecchia_, L_inv, L_inv, false);
+			vec_t d_mll_d_mode, SigmaI_plus_W_inv_d_mll_d_mode, SigmaI_plus_W_inv_diag;
+			sp_mat_t SigmaI_plus_W_inv;
+			// Calculate gradient wrt covariance parameters
+			if (calc_cov_grad) {
+				double explicit_derivative;
+				int num_par = (int)B_grad.size();
+				sp_mat_t SigmaI_deriv, BgradT_Dinv_B, Bt_Dinv_Bgrad;
+				sp_mat_t D_inv_B = D_inv * B;
+				for (int j = 0; j < num_par; ++j) {
+					// Calculate SigmaI_deriv
+					if (num_comps_total == 1 && j == 0) {
+						SigmaI_deriv = -B.transpose() * D_inv_B;//SigmaI_deriv = -SigmaI for variance parameters if there is only one GP
+					}
+					else {
+						SigmaI_deriv = B_grad[j].transpose() * D_inv_B;
+						Bt_Dinv_Bgrad = SigmaI_deriv.transpose();
+						SigmaI_deriv += Bt_Dinv_Bgrad - D_inv_B.transpose() * D_grad[j] * D_inv_B;
+						Bt_Dinv_Bgrad.resize(0, 0);
+					}
+					if (j == 0) {
+						// Calculate SigmaI_plus_W_inv = L_inv.transpose() * L_inv at non-zero entries of SigmaI_deriv
+						//	Note: fully calculating SigmaI_plus_W_inv = L_inv.transpose() * L_inv is very slow
+						SigmaI_plus_W_inv = SigmaI_deriv;
+						CalcLtLGivenSparsityPattern<sp_mat_t>(L_inv, SigmaI_plus_W_inv, true);
+						d_mll_d_mode = -0.5 * (SigmaI_plus_W_inv.diagonal().array() * third_deriv.array()).matrix();
+					}//end if j == 0
+					SigmaI_plus_W_inv_d_mll_d_mode = L_inv.transpose() * (L_inv * d_mll_d_mode);
+					vec_t SigmaI_deriv_mode = SigmaI_deriv * mode_;
+					explicit_derivative = 0.5 * (mode_.dot(SigmaI_deriv_mode) + (SigmaI_deriv.cwiseProduct(SigmaI_plus_W_inv)).sum());
+					if (num_comps_total == 1 && j == 0) {
+						explicit_derivative += 0.5 * num_data;
+					}
+					else {
+						explicit_derivative += 0.5 * (D_inv.diagonal().array() * D_grad[j].diagonal().array()).sum();
+					}
+					cov_grad[j] = explicit_derivative - SigmaI_plus_W_inv_d_mll_d_mode.dot(SigmaI_deriv_mode);//add implicit derivative
+				}
+			}//end calc_cov_grad
+			if (calc_F_grad || calc_aux_par_grad) {
+				if (!calc_cov_grad) {
+					sp_mat_t L_inv_sqr = L_inv.cwiseProduct(L_inv);
+					SigmaI_plus_W_inv_diag = L_inv_sqr.transpose() * vec_t::Ones(L_inv_sqr.rows());// diagonal of (Sigma^-1 + W) ^ -1
+					d_mll_d_mode = (-0.5 * SigmaI_plus_W_inv_diag.array() * third_deriv.array()).matrix();// gradient of approx. marginal likelihood wrt the mode and thus also F here
+					SigmaI_plus_W_inv_d_mll_d_mode = L_inv.transpose() * (L_inv * d_mll_d_mode);
+				}
+				else if (calc_aux_par_grad) {
+					SigmaI_plus_W_inv_diag = SigmaI_plus_W_inv.diagonal();
+				}
+			}
+			// Calculate gradient wrt fixed effects
+			if (calc_F_grad) {
+				vec_t d_mll_d_F_implicit = -(SigmaI_plus_W_inv_d_mll_d_mode.array() * second_deriv_neg_ll_.array()).matrix();// implicit derivative
+				fixed_effect_grad = -first_deriv_ll_ + d_mll_d_mode + d_mll_d_F_implicit;
+			}//end calc_F_grad
+			// calculate gradient wrt additional likelihood parameters
+			if (calc_aux_par_grad) {
+				vec_t neg_likelihood_deriv(num_aux_pars_);//derivative of the negative log-likelihood wrt additional parameters of the likelihood
+				vec_t second_deriv(num_data);//second derivative of the log-likelihood with respect to (i) the location parameter and (ii) an additional parameter of the likelihood
+				vec_t neg_third_deriv(num_data);//negative third derivative of the log-likelihood with respect to (i) two times the location parameter and (ii) an additional parameter of the likelihood
+				vec_t d_mode_d_aux_par;
+				CalcGradNegLogLikAuxPars(y_data, location_par_ptr, num_data, neg_likelihood_deriv.data());
+				for (int ind_ap = 0; ind_ap < num_aux_pars_; ++ind_ap) {
+					CalcSecondNegThirdDerivLogLikAuxParsLocPar(y_data, location_par_ptr, num_data, ind_ap, second_deriv.data(), neg_third_deriv.data());
+					double d_detmll_d_aux_par = 0., implicit_derivative = 0.;
+#pragma omp parallel for schedule(static) reduction(+:d_detmll_d_aux_par, implicit_derivative)
+					for (data_size_t i = 0; i < num_data; ++i) {
+						d_detmll_d_aux_par += neg_third_deriv[i] * SigmaI_plus_W_inv_diag[i];
+						implicit_derivative += second_deriv[i] * SigmaI_plus_W_inv_d_mll_d_mode[i];
+					}
+					aux_par_grad[ind_ap] = neg_likelihood_deriv[ind_ap] + 0.5 * d_detmll_d_aux_par + implicit_derivative;
+				}
+			}//end calc_aux_par_grad
+		}//end CalcGradNegMargLikelihoodLaplaceApproxVecchia
+
+		/*!
+		* \brief Make predictions for the (latent) random effects when using the Laplace approximation.
+		*		Calculations are done using a numerically stable variant based on factorizing ("inverting") B = (Id + Wsqrt * Z*Sigma*Zt * Wsqrt).
+		*		In the notation of the paper: "Sigma = Z*Sigma*Z^T" and "Z = Id".
+		*		This version is used for the Laplace approximation when dense matrices are used (e.g. GP models).
+		* \param y_data Response variable data if response variable is continuous
+		* \param y_data_int Response variable data if response variable is integer-valued
+		* \param fixed_effects Fixed effects component of location parameter
+		* \param num_data Number of data points
+		* \param ZSigmaZt Covariance matrix of latent random effect
+		* \param Cross_Cov Cross covariance matrix between predicted and obsreved random effects ("=Cov(y_p,y)")
+		* \param pred_mean[out] Predictive mean
+		* \param pred_cov[out] Predictive covariance matrix
+		* \param pred_var[out] Predictive variances
+		* \param calc_pred_cov If true, predictive covariance matrix is also calculated
+		* \param calc_pred_var If true, predictive variances are also calculated
+		* \param calc_mode If true, the mode of the random effects posterior is calculated otherwise the values in mode and a_vec_ are used (default=false)
+		*/
+		void PredictLaplaceApproxStable(const double* y_data,
+			const int* y_data_int,
+			const double* fixed_effects,
+			const data_size_t num_data,
+			const std::shared_ptr<T_mat> ZSigmaZt,
+			const T_mat& Cross_Cov,
+			vec_t& pred_mean,
+			T_mat& pred_cov,
+			vec_t& pred_var,
+			bool calc_pred_cov,
+			bool calc_pred_var,
+			bool calc_mode) {
+			if (calc_mode) {// Calculate mode and Cholesky factor of B = (Id + Wsqrt * ZSigmaZt * Wsqrt) at mode
+				double mll;//approximate marginal likelihood. This is a by-product that is not used here.
+				FindModePostRandEffCalcMLLStable(y_data, y_data_int, fixed_effects, num_data, ZSigmaZt, mll);
+			}
+			if (na_or_inf_during_last_call_to_find_mode_) {
+				Log::REFatal(NA_OR_INF_ERROR_);
+			}
+			CHECK(mode_has_been_calculated_);
+			pred_mean = Cross_Cov * first_deriv_ll_;
+			if (calc_pred_cov || calc_pred_var) {
+				sp_mat_t Wsqrt(num_data, num_data);//diagonal matrix with square root of negative second derivatives on the diagonal (sqrt of negative Hessian of log-likelihood)
+				Wsqrt.setIdentity();
+				Wsqrt.diagonal().array() = second_deriv_neg_ll_.array().sqrt();
+				T_mat Maux = Wsqrt * Cross_Cov.transpose();
+				TriangularSolveGivenCholesky<T_chol, T_mat, T_mat, T_mat>(chol_fact_Id_plus_Wsqrt_Sigma_Wsqrt_, Maux, Maux, false);
+				if (calc_pred_cov) {
+					pred_cov -= (T_mat)(Maux.transpose() * Maux);
+				}
+				if (calc_pred_var) {
+					Maux = Maux.cwiseProduct(Maux);
+#pragma omp parallel for schedule(static)
+					for (int i = 0; i < (int)pred_mean.size(); ++i) {
+						pred_var[i] -= Maux.col(i).sum();
+					}
+				}
+			}
+		}//end PredictLaplaceApproxStable
+
+		/*!
+		* \brief Make predictions for the (latent) random effects when using the Laplace approximation.
+		*		Calculations are done using a numerically stable variant based on factorizing ("inverting") B = (Id + Wsqrt * Z*Sigma*Zt * Wsqrt).
+		*		In the notation of the paper: "Sigma = Z*Sigma*Z^T" and "Z = Id".
+		*		This version is used for the Laplace approximation when dense matrices are used (e.g. GP models).
+		* \param y_data Response variable data if response variable is continuous
+		* \param y_data_int Response variable data if response variable is integer-valued
+		* \param fixed_effects Fixed effects component of location parameter
+		* \param num_data Number of data points
+		* \param Sigma Covariance matrix of latent random effect
+		* \param random_effects_indices_of_data Indices that indicate to which random effect every data point is related
+		* \param Cross_Cov Cross covariance matrix between predicted and obsreved random effects ("=Cov(y_p,y)")
+		* \param pred_mean[out] Predictive mean
+		* \param pred_cov[out] Predictive covariance matrix
+		* \param pred_var[out] Predictive variances
+		* \param calc_pred_cov If true, predictive covariance matrix is also calculated
+		* \param calc_pred_var If true, predictive variances are also calculated
+		* \param calc_mode If true, the mode of the random effects posterior is calculated otherwise the values in mode and a_vec_ are used (default=false)
+		*/
+		void PredictLaplaceApproxOnlyOneGPCalculationsOnREScale(const double* y_data,
+			const int* y_data_int,
+			const double* fixed_effects,
+			const data_size_t num_data,
+			const std::shared_ptr<T_mat> Sigma,
+			const data_size_t* const random_effects_indices_of_data,
+			const T_mat& Cross_Cov,
+			vec_t& pred_mean,
+			T_mat& pred_cov,
+			vec_t& pred_var,
+			bool calc_pred_cov,
+			bool calc_pred_var,
+			bool calc_mode) {
+			if (calc_mode) {// Calculate mode and Cholesky factor of B = (Id + Wsqrt * ZSigmaZt * Wsqrt) at mode
+				double mll;//approximate marginal likelihood. This is a by-product that is not used here.
+				FindModePostRandEffCalcMLLOnlyOneGPCalculationsOnREScale(y_data, y_data_int, fixed_effects,
+					num_data, Sigma, random_effects_indices_of_data, mll);
+			}
+			if (na_or_inf_during_last_call_to_find_mode_) {
+				Log::REFatal(NA_OR_INF_ERROR_);
+			}
+			CHECK(mode_has_been_calculated_);
+			vec_t ZtFirstDeriv;
+			CalcZtVGivenIndices(num_data, num_re_, random_effects_indices_of_data, first_deriv_ll_, ZtFirstDeriv, true);
+			pred_mean = Cross_Cov * ZtFirstDeriv;
+			if (calc_pred_cov || calc_pred_var) {
+				vec_t diag_ZtWZ;
+				CalcZtVGivenIndices(num_data, num_re_, random_effects_indices_of_data, second_deriv_neg_ll_, diag_ZtWZ, true);
+				sp_mat_t ZtWZsqrt(num_re_, num_re_);//diagonal matrix with square root of diagonal of ZtWZ
+				ZtWZsqrt.setIdentity();
+				ZtWZsqrt.diagonal().array() = diag_ZtWZ.array().sqrt();
+				T_mat Maux = ZtWZsqrt * Cross_Cov.transpose();
+				TriangularSolveGivenCholesky<T_chol, T_mat, T_mat, T_mat>(chol_fact_Id_plus_Wsqrt_Sigma_Wsqrt_, Maux, Maux, false);//Maux = L\(ZtWZsqrt * Cross_Cov^T)
+				if (calc_pred_cov) {
+					pred_cov -= (T_mat)(Maux.transpose() * Maux);
+				}
+				if (calc_pred_var) {
+					Maux = Maux.cwiseProduct(Maux);
+#pragma omp parallel for schedule(static)
+					for (int i = 0; i < (int)pred_mean.size(); ++i) {
+						pred_var[i] -= Maux.col(i).sum();
+					}
+				}
+			}
+		}//end PredictLaplaceApproxOnlyOneGPCalculationsOnREScale
+
+		/*!
+		* \brief Make predictions for the (latent) random effects when using the Laplace approximation.
+		*		Calculations are done by directly factorizing ("inverting) (Sigma^-1 + Zt*W*Z).
+		*		NOTE: IT IS ASSUMED THAT SIGMA IS A DIAGONAL MATRIX
+		*		This version is used for the Laplace approximation when there are only grouped random effects.
+		* \param y_data Response variable data if response variable is continuous
+		* \param y_data_int Response variable data if response variable is integer-valued
+		* \param fixed_effects Fixed effects component of location parameter
+		* \param num_data Number of data points
+		* \param SigmaI Inverse covariance matrix of latent random effect. Currently, this needs to be a diagonal matrix
+		* \param Zt Transpose Z^T of random effect design matrix that relates latent random effects to observations/likelihoods
+		* \param Ztilde matrix which relates existing random effects to prediction samples
+		* \param Sigma Covariance matrix of random effects
+		* \param pred_mean[out] Predictive mean
+		* \param pred_cov[out] Predictive covariance matrix
+		* \param pred_var[out] Predictive variances
+		* \param calc_pred_cov If true, predictive covariance matrix is also calculated
+		* \param calc_pred_var If true, predictive variances are also calculated
+		* \param calc_mode If true, the mode of the random effects posterior is calculated otherwise the values in mode and a_vec_ are used (default=false)
+		*/
+		void PredictLaplaceApproxGroupedRE(const double* y_data,
+			const int* y_data_int,
+			const double* fixed_effects,
+			const data_size_t num_data,
+			const sp_mat_t& SigmaI,
+			const sp_mat_t& Zt,
+			const sp_mat_t& Ztilde,
+			const sp_mat_t& Sigma,
+			vec_t& pred_mean,
+			T_mat& pred_cov,
+			vec_t& pred_var,
+			bool calc_pred_cov,
+			bool calc_pred_var,
+			bool calc_mode) {
+			if (calc_mode) {// Calculate mode and Cholesky factor of B = (Id + Wsqrt * ZSigmaZt * Wsqrt) at mode
+				double mll;//approximate marginal likelihood. This is a by-product that is not used here.
+				FindModePostRandEffCalcMLLGroupedRE(y_data, y_data_int, fixed_effects, num_data, SigmaI, Zt, mll);
+			}
+			if (na_or_inf_during_last_call_to_find_mode_) {
+				Log::REFatal(NA_OR_INF_ERROR_);
+			}
+			CHECK(mode_has_been_calculated_);
+			vec_t v_aux = Zt * first_deriv_ll_;
+			vec_t v_aux2 = Sigma * v_aux;
+			pred_mean = Ztilde * v_aux2;
+			if (calc_pred_cov || calc_pred_var) {
+				// calculate Maux = L\(Z^T * second_deriv_neg_ll_.asDiagonal() * Cross_Cov^T)
+				sp_mat_t Cross_Cov = Ztilde * Sigma * Zt;
+				sp_mat_t Maux = Zt * second_deriv_neg_ll_.asDiagonal() * Cross_Cov.transpose();
+				TriangularSolveGivenCholesky<chol_sp_mat_t, sp_mat_t, sp_mat_t, sp_mat_t>(chol_fact_SigmaI_plus_ZtWZ_grouped_, Maux, Maux, false);
+				if (calc_pred_cov) {
+					pred_cov += (T_mat)(Maux.transpose() * Maux);
+					pred_cov -= (T_mat)(Cross_Cov * second_deriv_neg_ll_.asDiagonal() * Cross_Cov.transpose());
+				}
+				if (calc_pred_var) {
+					sp_mat_t Maux3 = Cross_Cov.cwiseProduct(Cross_Cov * second_deriv_neg_ll_.asDiagonal());
+					Maux = Maux.cwiseProduct(Maux);
+#pragma omp parallel for schedule(static)
+					for (int i = 0; i < (int)pred_mean.size(); ++i) {
+						pred_var[i] += Maux.col(i).sum() - Maux3.row(i).sum();
+					}
+				}
+			}
+		}//end PredictLaplaceApproxGroupedRE
+
+		/*!
+		* \brief Make predictions for the (latent) random effects when using the Laplace approximation.
+		*		Calculations are done by directly factorizing ("inverting) (Sigma^-1 + Zt*W*Z).
+		*		This version is used for the Laplace approximation when there are only grouped random effects with only one grouping variable.
+		* \param y_data Response variable data if response variable is continuous
+		* \param y_data_int Response variable data if response variable is integer-valued
+		* \param fixed_effects Fixed effects component of location parameter
+		* \param num_data Number of data points
+		* \param sigma2 Variance of random effects
+		* \param random_effects_indices_of_data Indices that indicate to which random effect every data point is related
+		* \param Cross_Cov Cross covariance matrix between predicted and obsreved random effects ("=Cov(y_p,y)")
+		* \param pred_mean[out] Predictive mean
+		* \param pred_cov[out] Predictive covariance matrix
+		* \param pred_var[out] Predictive variances
+		* \param calc_pred_cov If true, predictive covariance matrix is also calculated
+		* \param calc_pred_var If true, predictive variances are also calculated
+		* \param calc_mode If true, the mode of the random effects posterior is calculated otherwise the values in mode and a_vec_ are used (default=false)
+		*/
+		void PredictLaplaceApproxOnlyOneGroupedRECalculationsOnREScale(const double* y_data,
+			const int* y_data_int,
+			const double* fixed_effects,
+			const data_size_t num_data,
+			const double sigma2,
+			const data_size_t* const random_effects_indices_of_data,
+			const T_mat& Cross_Cov,
+			vec_t& pred_mean,
+			T_mat& pred_cov,
+			vec_t& pred_var,
+			bool calc_pred_cov,
+			bool calc_pred_var,
+			bool calc_mode) {
+			if (calc_mode) {// Calculate mode and Cholesky factor of B = (Id + Wsqrt * ZSigmaZt * Wsqrt) at mode
+				double mll;//approximate marginal likelihood. This is a by-product that is not used here.
+				FindModePostRandEffCalcMLLOnlyOneGroupedRECalculationsOnREScale(y_data, y_data_int, fixed_effects, num_data,
+					sigma2, random_effects_indices_of_data, mll);
+			}
+			if (na_or_inf_during_last_call_to_find_mode_) {
+				Log::REFatal(NA_OR_INF_ERROR_);
+			}
+			CHECK(mode_has_been_calculated_);
+			vec_t ZtFirstDeriv;
+			CalcZtVGivenIndices(num_data, num_re_, random_effects_indices_of_data, first_deriv_ll_, ZtFirstDeriv, true);
+			pred_mean = Cross_Cov * ZtFirstDeriv;
+			if (calc_pred_cov || calc_pred_var) {
+				vec_t diag_Sigma_plus_ZtWZI(num_re_);
+				diag_Sigma_plus_ZtWZI.array() = 1. / diag_SigmaI_plus_ZtWZ_.array();
+				diag_Sigma_plus_ZtWZI.array() /= sigma2;
+				diag_Sigma_plus_ZtWZI.array() -= 1.;
+				diag_Sigma_plus_ZtWZI.array() /= sigma2;
+				if (calc_pred_cov) {
+					T_mat Maux = Cross_Cov * diag_Sigma_plus_ZtWZI.asDiagonal() * Cross_Cov.transpose();
+					pred_cov += Maux;
+				}
+				if (calc_pred_var) {
+					T_mat Maux = Cross_Cov * diag_Sigma_plus_ZtWZI.asDiagonal();
+					T_mat Maux2 = Cross_Cov.cwiseProduct(Maux);
+#pragma omp parallel for schedule(static)
+					for (int i = 0; i < (int)pred_mean.size(); ++i) {
+						pred_var[i] += Maux2.row(i).sum();
+					}
+				}
+			}
+		}//end PredictLaplaceApproxOnlyOneGroupedRECalculationsOnREScale
+
+		/*!
+		* \brief Make predictions for the (latent) random effects when using the Laplace approximation.
+		*		Calculations are done by factorizing ("inverting) (Sigma^-1 + W) where it is assumed that an approximate Cholesky factor
+		*		of Sigma^-1 has previously been calculated using a Vecchia approximation.
+		*		This version is used for the Laplace approximation when there are only GP random effects and the Vecchia approximation is used.
+		*		Caveat: Sigma^-1 + W can be not very sparse
+		* \param y_data Response variable data if response variable is continuous
+		* \param y_data_int Response variable data if response variable is integer-valued
+		* \param fixed_effects Fixed effects component of location parameter
+		* \param num_data Number of data points
+		* \param B Matrix B in Vecchia approximation for observed locations, Sigma^-1 = B^T D^-1 B ("=" Cholesky factor)
+		* \param D_inv Diagonal matrix D^-1 in Vecchia approximation for observed locations
+		* \param Bpo Lower left part of matrix B in joint Vecchia approximation for observed and prediction locations with non-zero off-diagonal entries corresponding to the nearest neighbors of the prediction locations among the observed locations
+		* \param Bp Lower right part of matrix B in joint Vecchia approximation for observed and prediction locations with non-zero off-diagonal entries corresponding to the nearest neighbors of the prediction locations among the prediction locations
+		* \param Dp Diagonal matrix with lower right part of matrix D in joint Vecchia approximation for observed and prediction locations
+		* \param pred_mean[out] Predictive mean
+		* \param pred_cov[out] Predictive covariance matrix
+		* \param pred_var[out] Predictive variances
+		* \param calc_pred_cov If true, predictive covariance matrix is also calculated
+		* \param calc_pred_var If true, predictive variances are also calculated
+		* \param calc_mode If true, the mode of the random effects posterior is calculated otherwise the values in mode and a_vec_ are used (default=false)
+		* \param CondObsOnly If true, the nearest neighbors for the predictions are found only among the observed data and Bp is an identity matrix
+		*/
+		void PredictLaplaceApproxVecchia(const double* y_data,
+			const int* y_data_int,
+			const double* fixed_effects,
+			const data_size_t num_data,
+			const sp_mat_t& B,
+			const sp_mat_t& D_inv,
+			const sp_mat_t& Bpo,
+			sp_mat_t& Bp,
+			const vec_t& Dp,
+			vec_t& pred_mean,
+			T_mat& pred_cov,
+			vec_t& pred_var,
+			bool calc_pred_cov,
+			bool calc_pred_var,
+			bool calc_mode,
+			bool CondObsOnly) {
+			if (calc_mode) {// Calculate mode and Cholesky factor of Sigma^-1 + W at mode
+				double mll;//approximate marginal likelihood. This is a by-product that is not used here.
+				FindModePostRandEffCalcMLLVecchia(y_data, y_data_int, fixed_effects, num_data, B, D_inv, mll);
+			}
+			if (na_or_inf_during_last_call_to_find_mode_) {
+				Log::REFatal(NA_OR_INF_ERROR_);
+			}
+			CHECK(mode_has_been_calculated_);
+			int num_pred = (int)Bp.cols();
+			CHECK((int)Dp.size() == num_pred);
+			if (CondObsOnly) {
+				pred_mean = -Bpo * mode_;
+			}
+			else {
+				vec_t Bpo_mode = Bpo * mode_;
+				pred_mean = -Bp.triangularView<Eigen::UpLoType::UnitLower>().solve(Bpo_mode);
+			}
+			if (calc_pred_cov || calc_pred_var) {
+				sp_mat_t Bp_inv, Bp_inv_Dp;
+				sp_mat_t Maux; //Maux = L\(Bpo^T * Bp^-1), L = Chol(Sigma^-1 + W)
+				if (CondObsOnly) {
+					Maux = Bpo.transpose();//Bp = Id
+				}
+				else {
+					Bp_inv = sp_mat_t(Bp.rows(), Bp.cols());
+					Bp_inv.setIdentity();
+					TriangularSolve<sp_mat_t, sp_mat_t, sp_mat_t>(Bp, Bp_inv, Bp_inv, false);
+					//Bp.triangularView<Eigen::UpLoType::UnitLower>().solveInPlace(Bp_inv);//much slower
+					Maux = Bpo.transpose() * Bp_inv.transpose();
+					Bp_inv_Dp = Bp_inv * Dp.asDiagonal();
+				}
+				TriangularSolveGivenCholesky<chol_sp_mat_t, sp_mat_t, sp_mat_t, sp_mat_t>(chol_fact_SigmaI_plus_ZtWZ_vecchia_, Maux, Maux, false);
+				if (calc_pred_cov) {
+					if (CondObsOnly) {
+						pred_cov = Maux.transpose() * Maux;
+						pred_cov.diagonal().array() += Dp.array();
+					}
+					else {
+						pred_cov = Bp_inv_Dp * Bp_inv.transpose() + Maux.transpose() * Maux;
+					}
+				}
+				if (calc_pred_var) {
+					pred_var = vec_t(num_pred);
+					Maux = Maux.cwiseProduct(Maux);
+					if (CondObsOnly) {
+#pragma omp parallel for schedule(static)
+						for (int i = 0; i < num_pred; ++i) {
+							pred_var[i] = Dp[i] + Maux.col(i).sum();
+						}
+					}
+					else {
+#pragma omp parallel for schedule(static)
+						for (int i = 0; i < num_pred; ++i) {
+							pred_var[i] = (Bp_inv_Dp.row(i)).dot(Bp_inv.row(i)) + Maux.col(i).sum();
+						}
+					}
+				}
+			}//end calc_pred_cov || calc_pred_var
+		}//end PredictLaplaceApproxVecchia
+
+//Note: the following is currently not used
+//		/*!
+//		* \brief Calculate variance of Laplace-approximated posterior
+//		* \param ZSigmaZt Covariance matrix of latent random effect
+//		* \param[out] pred_var Variance of Laplace-approximated posterior
+//		*/
+//		void CalcVarLaplaceApproxStable(const std::shared_ptr<T_mat> ZSigmaZt,
+//			vec_t& pred_var) {
+//			if (na_or_inf_during_last_call_to_find_mode_) {
+//				Log::REFatal(NA_OR_INF_ERROR_);
+//			}
+//			CHECK(mode_has_been_calculated_);
+//			pred_var = vec_t(num_re_);
+//			vec_t diag_Wsqrt(second_deriv_neg_ll_.size());
+//			diag_Wsqrt.array() = second_deriv_neg_ll_.array().sqrt();
+//			T_mat L_inv_W_sqrt_ZSigmaZt = diag_Wsqrt.asDiagonal() * (*ZSigmaZt);
+//			TriangularSolveGivenCholesky<T_chol, T_mat, T_mat, T_mat>(chol_fact_Id_plus_Wsqrt_Sigma_Wsqrt_, L_inv_W_sqrt_ZSigmaZt, L_inv_W_sqrt_ZSigmaZt, false);
+//#pragma omp parallel for schedule(static)
+//			for (int i = 0; i < num_re_; ++i) {
+//				pred_var[i] = (*ZSigmaZt).coeff(i,i) - L_inv_W_sqrt_ZSigmaZt.col(i).squaredNorm();
+//			}
+//		}//end CalcVarLaplaceApproxStable
+
+		/*!
+		* \brief Calculate variance of Laplace-approximated posterior
+		* \param Sigma Covariance matrix of latent random effect
+		* \param random_effects_indices_of_data Indices that indicate to which random effect every data point is related
+		* \param[out] pred_var Variance of Laplace-approximated posterior
+		*/
+		void CalcVarLaplaceApproxOnlyOneGPCalculationsOnREScale(const std::shared_ptr<T_mat> Sigma,
+			const data_size_t* const random_effects_indices_of_data,
+			vec_t& pred_var) {
+			if (na_or_inf_during_last_call_to_find_mode_) {
+				Log::REFatal(NA_OR_INF_ERROR_);
+			}
+			CHECK(mode_has_been_calculated_);
+			pred_var = vec_t(num_re_);
+			vec_t diag_ZtWZ_sqrt;
+			CalcZtVGivenIndices((data_size_t)second_deriv_neg_ll_.size(), num_re_, random_effects_indices_of_data, second_deriv_neg_ll_, diag_ZtWZ_sqrt, true);
+			diag_ZtWZ_sqrt.array() = diag_ZtWZ_sqrt.array().sqrt();
+			T_mat L_inv_ZtWZ_sqrt_Sigma = diag_ZtWZ_sqrt.asDiagonal() * (*Sigma);
+			TriangularSolveGivenCholesky<T_chol, T_mat, T_mat, T_mat>(chol_fact_Id_plus_Wsqrt_Sigma_Wsqrt_, L_inv_ZtWZ_sqrt_Sigma, L_inv_ZtWZ_sqrt_Sigma, false);
+#pragma omp parallel for schedule(static)
+			for (int i = 0; i < num_re_; ++i) {
+				pred_var[i] = (*Sigma).coeff(i, i) - L_inv_ZtWZ_sqrt_Sigma.col(i).squaredNorm();
+			}
+		}//end CalcVarLaplaceApproxOnlyOneGPCalculationsOnREScale
+
+		/*!
+		* \brief Calculate variance of Laplace-approximated posterior
+		* \param[out] pred_var Variance of Laplace-approximated posterior
+		*/
+		void CalcVarLaplaceApproxGroupedRE(vec_t& pred_var) {
+			if (na_or_inf_during_last_call_to_find_mode_) {
+				Log::REFatal(NA_OR_INF_ERROR_);
+			}
+			CHECK(mode_has_been_calculated_);
+			pred_var = vec_t(num_re_);
+			sp_mat_t L_inv(num_re_, num_re_);
+			L_inv.setIdentity();
+			TriangularSolveGivenCholesky<chol_sp_mat_t, sp_mat_t, sp_mat_t, sp_mat_t>(chol_fact_SigmaI_plus_ZtWZ_grouped_, L_inv, L_inv, false);
+#pragma omp parallel for schedule(static)
+			for (int i = 0; i < num_re_; ++i) {
+				pred_var[i] = L_inv.col(i).squaredNorm();
+			}
+		}//end CalcVarLaplaceApproxGroupedRE
+
+		/*!
+		* \brief Calculate variance of Laplace-approximated posterior
+		* \param[out] pred_var Variance of Laplace-approximated posterior
+		*/
+		void CalcVarLaplaceApproxOnlyOneGroupedRECalculationsOnREScale(vec_t& pred_var) {
+			if (na_or_inf_during_last_call_to_find_mode_) {
+				Log::REFatal(NA_OR_INF_ERROR_);
+			}
+			CHECK(mode_has_been_calculated_);
+			pred_var = vec_t(num_re_);
+			pred_var.array() = diag_SigmaI_plus_ZtWZ_.array().inverse();
+		}//end CalcVarLaplaceApproxOnlyOneGroupedRECalculationsOnREScale
+
+		/*!
+		* \brief Calculate variance of Laplace-approximated posterior
+		* \param[out] pred_var Variance of Laplace-approximated posterior
+		*/
+		void CalcVarLaplaceApproxVecchia(vec_t& pred_var) {
+			if (na_or_inf_during_last_call_to_find_mode_) {
+				Log::REFatal(NA_OR_INF_ERROR_);
+			}
+			CHECK(mode_has_been_calculated_);
+			pred_var = vec_t(num_re_);
+			sp_mat_t L_inv(num_re_, num_re_);
+			L_inv.setIdentity();
+			TriangularSolveGivenCholesky<chol_sp_mat_t, sp_mat_t, sp_mat_t, sp_mat_t>(chol_fact_SigmaI_plus_ZtWZ_vecchia_, L_inv, L_inv, false);
+#pragma omp parallel for schedule(static)
+			for (int i = 0; i < num_re_; ++i) {
+				pred_var[i] = L_inv.col(i).squaredNorm();
+			}
+		}//end CalcVarLaplaceApproxVecchia
+
+		/*!
+		* \brief Make predictions for the response variable (label) based on predictions for the mean and variance of the latent random effects
+		* \param pred_mean[out] Predictive mean of latent random effects. The Predictive mean for the response variables is written on this
+		* \param pred_var[out] Predictive variances of latent random effects. The predicted variance for the response variables is written on this
+		* \param predict_var If true, predictive variances are also calculated
+		*/
+		void PredictResponse(vec_t& pred_mean,
+			vec_t& pred_var,
+			bool predict_var) {
+			if (likelihood_type_ == "bernoulli_probit") {
+#pragma omp parallel for schedule(static)
+				for (int i = 0; i < (int)pred_mean.size(); ++i) {
+					pred_mean[i] = normalCDF(pred_mean[i] / std::sqrt(1. + pred_var[i]));
+				}
+				if (predict_var) {
+#pragma omp parallel for schedule(static)
+					for (int i = 0; i < (int)pred_mean.size(); ++i) {
+						pred_var[i] = pred_mean[i] * (1. - pred_mean[i]);
+					}
+				}
+			}
+			else if (likelihood_type_ == "bernoulli_logit") {
+#pragma omp parallel for schedule(static)
+				for (int i = 0; i < (int)pred_mean.size(); ++i) {
+					pred_mean[i] = RespMeanAdaptiveGHQuadrature(pred_mean[i], pred_var[i]);
+				}
+				if (predict_var) {
+#pragma omp parallel for schedule(static)
+					for (int i = 0; i < (int)pred_mean.size(); ++i) {
+						pred_var[i] = pred_mean[i] * (1. - pred_mean[i]);
+					}
+				}
+			}
+			else if (likelihood_type_ == "poisson") {
+#pragma omp parallel for schedule(static)
+				for (int i = 0; i < (int)pred_mean.size(); ++i) {
+					double pm = std::exp(pred_mean[i] + 0.5 * pred_var[i]);
+					//double pm = RespMeanAdaptiveGHQuadrature(pred_mean[i], pred_var[i]);// alternative version using quadrature
+					if (predict_var) {
+						pred_var[i] = pm * ((std::exp(pred_var[i]) - 1.) * pm + 1.);
+						//double psm = RespMeanAdaptiveGHQuadrature(2 * pred_mean[i], 4 * pred_var[i]);// alternative version using quadrature
+						//pred_var[i] = psm - pm * pm + pm;
+					}
+					pred_mean[i] = pm;
+				}
+			}
+			else if (likelihood_type_ == "gamma") {
+#pragma omp parallel for schedule(static)
+				for (int i = 0; i < (int)pred_mean.size(); ++i) {
+					double pm = std::exp(pred_mean[i] + 0.5 * pred_var[i]);
+					//double pm = RespMeanAdaptiveGHQuadrature(pred_mean[i], pred_var[i]);// alternative version using quadrature
+					if (predict_var) {
+						pred_var[i] = (std::exp(pred_var[i]) - 1.) * pm * pm + std::exp(2 * pred_mean[i] + 2 * pred_var[i]) / aux_pars_[0];
+						//double psm = RespMeanAdaptiveGHQuadrature(2 * pred_mean[i], 4 * pred_var[i]);// alternative version using quadrature
+						//pred_var[i] = psm - pm * pm + psm / aux_pars_[0];
+					}
+					pred_mean[i] = pm;
+				}
+			}
+		}//end PredictResponse
+
+		/*!
+		* \brief Adaptive GH quadrature to calculate predictive mean of response variable
+		* \param latent_mean Predictive mean of latent random effects
+		* \param latent_var Predictive variances of latent random effects
+		*/
+		double RespMeanAdaptiveGHQuadrature(const double latent_mean,
+			const double latent_var) {
+			// Find mode of integrand
+			double mode_integrand_last, update;
+			double mode_integrand = 0.;
+			double sigma2_inv = 1. / latent_var;
+			double sqrt_sigma2_inv = std::sqrt(sigma2_inv);
+			for (int it = 0; it < 100; ++it) {
+				mode_integrand_last = mode_integrand;
+				update = (FirstDerivLogCondMeanLikelihood(mode_integrand) - sigma2_inv * (mode_integrand - latent_mean))
+					/ (SecondDerivLogCondMeanLikelihood(mode_integrand) - sigma2_inv);
+				mode_integrand -= update;
+				if (std::abs(update) / std::abs(mode_integrand_last) < DELTA_REL_CONV_) {
+					break;
+				}
+			}
+			// Adaptive GH quadrature
+			double sqrt2_sigma_hat = M_SQRT2 / std::sqrt(-SecondDerivLogCondMeanLikelihood(mode_integrand) + sigma2_inv);
+			double x_val;
+			double mean_resp = 0.;
+			for (int j = 0; j < order_GH_; ++j) {
+				x_val = sqrt2_sigma_hat * GH_nodes_[j] + mode_integrand;
+				mean_resp += adaptive_GH_weights_[j] * CondMeanLikelihood(x_val) * normalPDF(sqrt_sigma2_inv * (x_val - latent_mean));
+			}
+			mean_resp *= sqrt2_sigma_hat * sqrt_sigma2_inv;
+			return mean_resp;
+		}//end RespMeanAdaptiveGHQuadrature
+
+		/*!
+		* \brief Calculate test negative log-likelihood using adaptive GH quadrature
+		* \param y_test Test response variable
+		* \param pred_mean Predictive mean of latent random effects
+		* \param pred_var Predictive variances of latent random effects
+		* \param num_data Number of data points
+		*/
+		inline double TestNegLogLikelihoodAdaptiveGHQuadrature(const label_t* y_test,
+			const double* pred_mean,
+			const double* pred_var,
+			const data_size_t num_data) const {
+			double ll = 0.;
+#pragma omp parallel for schedule(static) if (num_data >= 128) reduction(+:ll)
+			for (data_size_t i = 0; i < num_data; ++i) {
+				int y_test_int = 1;
+				double y_test_d = static_cast<double>(y_test[i]);
+				// Note: we need to convert from float to double as label_t is float. Unfortunately, the lightGBM part does not allow for setting the LABEL_T_USE_DOUBLE macro in meta.h (multiple bugs...)
+				if (label_type() == "int") {
+					y_test_int = static_cast<int>(y_test[i]);
+				}
+				// Find mode of integrand
+				double mode_integrand_last, update;
+				double mode_integrand = 0.;
+				double sigma2_inv = 1. / pred_var[i];
+				double sqrt_sigma2_inv = std::sqrt(sigma2_inv);
+				for (int it = 0; it < 100; ++it) {
+					mode_integrand_last = mode_integrand;
+					update = (CalcFirstDerivLogLik(y_test_d, y_test_int, mode_integrand) - sigma2_inv * (mode_integrand - pred_mean[i]))
+						/ (-CalcSecondDerivNegLogLik(y_test_d, y_test_int, mode_integrand) - sigma2_inv);
+					mode_integrand -= update;
+					if (std::abs(update) / std::abs(mode_integrand_last) < DELTA_REL_CONV_) {
+						break;
+					}
+				}
+				// Adaptive GH quadrature
+				double sqrt2_sigma_hat = M_SQRT2 / std::sqrt(CalcSecondDerivNegLogLik(y_test_d, y_test_int, mode_integrand) + sigma2_inv);
+				double x_val;
+				double likelihood = 0.;
+				for (int j = 0; j < order_GH_; ++j) {
+					x_val = sqrt2_sigma_hat * GH_nodes_[j] + mode_integrand;
+					likelihood += adaptive_GH_weights_[j] * std::exp(LogLikelihood(y_test_d, y_test_int, x_val)) * normalPDF(sqrt_sigma2_inv * (x_val - pred_mean[i]));
+				}
+				likelihood *= sqrt2_sigma_hat * sqrt_sigma2_inv;
+				ll += std::log(likelihood);
+			}
+			return -ll;
+		}//end TestNegLogLikelihoodAdaptiveGHQuadrature
+
+		/*! \brief Set matrix inversion properties and choices for iterative methods. This function is calle from re_model_template.h which also holds these variables */
+		void SetMatrixInversionProperties(const string_t& matrix_inversion_method,
+			int cg_max_num_it,
+			int cg_max_num_it_tridiag,
+			double cg_delta_conv,
+			int num_rand_vec_trace,
+			bool reuse_rand_vec_trace,
+			int seed_rand_vec_trace,
+			const string_t& cg_preconditioner_type,
+			int piv_chol_rank,
+			int rank_pred_approx_matrix_lanczos) {
+			matrix_inversion_method_ = matrix_inversion_method;
+			cg_max_num_it_ = cg_max_num_it;
+			cg_max_num_it_tridiag_ = cg_max_num_it_tridiag;
+			cg_delta_conv_ = cg_delta_conv;
+			num_rand_vec_trace_ = num_rand_vec_trace;
+			reuse_rand_vec_trace_ = reuse_rand_vec_trace;
+			seed_rand_vec_trace_ = seed_rand_vec_trace;
+			cg_preconditioner_type_ = cg_preconditioner_type;
+			piv_chol_rank_ = piv_chol_rank;
+			rank_pred_approx_matrix_lanczos_ = rank_pred_approx_matrix_lanczos;
+		}//end SetMatrixInversionProperties
+
+		static string_t ParseLikelihoodAlias(const string_t& likelihood) {
+			if (likelihood == string_t("binary") || likelihood == string_t("bernoulli_probit") || likelihood == string_t("binary_probit")) {
+				return "bernoulli_probit";
+			}
+			else if (likelihood == string_t("bernoulli_logit") || likelihood == string_t("binary_logit")) {
+				return "bernoulli_logit";
+			}
+			else if (likelihood == string_t("gaussian") || likelihood == string_t("regression")) {
+				return "gaussian";
+			}
+			return likelihood;
+		}
+
+		string_t ParseLikelihoodAliasGradientDescent(const string_t& likelihood) {
+			if (likelihood.size() > 13) {
+				if (likelihood.substr(likelihood.size() - 13) == string_t("_quasi-newton")) {
+					quasi_newton_for_mode_finding_ = true;
+					DELTA_REL_CONV_ = 1e-9;
+					return likelihood.substr(0, likelihood.size() - 13);
+				}
+			}
+			return likelihood;
+		}
+
+	private:
+		/*! \brief Number of data points */
+		data_size_t num_data_;
+		/*! \brief Number (dimension) of random effects (= length of mode_) */
+		data_size_t num_re_;
+		/*! \brief Posterior mode used for Laplace approximation */
+		vec_t mode_;
+		/*! \brief Saving a previously found value allows for reseting the mode when having a too large step size. */
+		vec_t mode_previous_value_;
+		/*! \brief Auxiliary variable a=ZSigmaZt^-1 mode_b used for Laplace approximation */
+		vec_t a_vec_;
+		/*! \brief Saving a previously found value allows for reseting the mode when having a too large step size. */
+		vec_t a_vec_previous_value_;
+		/*! \brief Indicates whether the vector a_vec_ / a=ZSigmaZt^-1 is used or not */
+		bool has_a_vec_;
+		/*! \brief First derivatives of the log-likelihood */
+		vec_t first_deriv_ll_;
+		/*! \brief Second derivatives of the negative log-likelihood (diagonal of matrix "W") */
+		vec_t second_deriv_neg_ll_;
+		/*! \brief Diagonal of matrix Sigma^-1 + Zt * W * Z in Laplace approximation (used only in version 'GroupedRE' when there is only one random effect and ZtWZ is diagonal. Otherwise 'diag_SigmaI_plus_ZtWZ_' is used for grouped REs) */
+		vec_t diag_SigmaI_plus_ZtWZ_;
+		/*! \brief Cholesky factors of matrix Sigma^-1 + Zt * W * Z in Laplace approximation (used only in version'GroupedRE' if there is more than one random effect). */
+		chol_sp_mat_t chol_fact_SigmaI_plus_ZtWZ_grouped_;
+		/*! \brief Cholesky factors of matrix Sigma^-1 + Zt * W * Z in Laplace approximation (used only in version 'Vecchia') */
+		chol_sp_mat_t chol_fact_SigmaI_plus_ZtWZ_vecchia_;
+		/*!
+		* \brief Cholesky factors of matrix B = I + Wsqrt *  Z * Sigma * Zt * Wsqrt in Laplace approximation (for version 'Stable')
+		*		or of matrix B = Id + ZtWZsqrt * Sigma * ZtWZsqrt (for version 'OnlyOneGPCalculationsOnREScale')
+		*/
+		T_chol chol_fact_Id_plus_Wsqrt_Sigma_Wsqrt_;
+		/*! \brief If true, the pattern for the Cholesky factor (chol_fact_Id_plus_Wsqrt_Sigma_Wsqrt_, chol_fact_SigmaI_plus_ZtWZ_grouped_, or chol_fact_SigmaI_plus_ZtWZ_vecchia_) has been analyzed */
+		bool chol_fact_pattern_analyzed_ = false;
+		/*! \brief If true, the mode has been initialized to 0 */
+		bool mode_initialized_ = false;
+		/*! \brief If true, the mode has been determined */
+		bool mode_has_been_calculated_ = false;
+		/*! \brief If true, NA or Inf has occurred during the last call to find mode */
+		bool na_or_inf_during_last_call_to_find_mode_ = false;
+		/*! \brief If true, NA or Inf has occurred during the second last call to find mode when mode_previous_value_ was calculated */
+		bool na_or_inf_during_second_last_call_to_find_mode_ = false;
+		/*! \brief Normalizing constant of the log-likelihood (not all likelihoods have one) */
+		double log_normalizing_constant_;
+		/*! \brief If true, the function 'CalculateLogNormalizingConstant' has been called */
+		bool normalizing_constant_has_been_calculated_ = false;
+		/*! \brief Auxiliary quantities that do not depend on aux_pars_ for normalizing constant for likelihoods (not all likelihoods have one, for gamma this is sum( log(y) ) ) */
+		double aux_log_normalizing_constant_;
+		/*! \brief If true, the function 'CalculateAuxQuantLogNormalizingConstant' has been called */
+		bool aux_normalizing_constant_has_been_calculated_ = false;
+
+		/*! \brief Type of likelihood  */
+		string_t likelihood_type_ = "gaussian";
+		/*! \brief List of supported covariance likelihoods */
+		const std::set<string_t> SUPPORTED_LIKELIHOODS_{ "gaussian", "bernoulli_probit", "bernoulli_logit", "poisson", "gamma" };
+		/*! \brief Maximal number of iteration done for finding posterior mode with Newton's method */
+		int MAXIT_MODE_NEWTON_ = 1000;
+		/*! \brief Used for checking convergence in mode finding algorithm (terminate if relative change in Laplace approx. is below this value) */
+		double DELTA_REL_CONV_ = 1e-6;
+		/*! \brief If true, a quasi-Newton method instead of Newton's method is used for finding the maximal mode. Only supported for the Vecchia approximation */
+		bool quasi_newton_for_mode_finding_ = false;
+		/*! \brief Maximal number of steps for which learning rate shrinkage is done in the quasi-Newton method for mode finding in Laplace approximation */
+		int MAX_NUMBER_LR_SHRINKAGE_STEPS_ = 30;
+		/*! \brief If true, the mode can only change by 'MAX_CHANGE_MODE_NEWTON_' in Newton's method */
+		bool cap_change_mode_newton_ = false;
+		/*! \brief Maximally allowed change for mode in Newton's method for those likelihoods where a cap is enforced */
+		double MAX_CHANGE_MODE_NEWTON_ = std::log(100.);
+		/*! \brief Number of additional parameters for likelihoods  */
+		int num_aux_pars_;
+		/*! \brief Additional parameters for likelihoods. For "gamma", aux_pars_[0] = shape parameter, for gaussian, aux_pars_[0] = 1 / sqrt(variance) */
+		std::vector<double> aux_pars_;
+		/*! \brief Names of additional parameters for likelihoods */
+		std::vector<string_t> names_aux_pars_;
+		/*! \brief True, if the function 'SetAuxPars' has been called */
+		bool aux_pars_have_been_set_ = false;
+
+		// MATRIX INVERSION PROPERTIES
+		/*! \brief Matrix inversion method */
+		string_t matrix_inversion_method_ = "cholesky";
+		/*! \brief Maximal number of iterations for conjugate gradient algorithm */
+		int cg_max_num_it_ = 1000;
+		/*! \brief Maximal number of iterations for conjugate gradient algorithm when being run as Lanczos algorithm for tridiagonalization */
+		int cg_max_num_it_tridiag_ = 1000;
+		/*! \brief Tolerance level for L2 norm of residuals for checking convergence in conjugate gradient algorithm when being used for parameter estimation */
+		double cg_delta_conv_ = 1e-3;
+		/*! \brief Number of random vectors (e.g. Rademacher) for stochastic approximation of the trace of a matrix */
+		int num_rand_vec_trace_ = 50;
+		/*! \brief If true, random vectors (e.g. Rademacher) for stochastic approximation of the trace of a matrix are sampled only once at the beginning and then reused in later trace approximations, otherwise they are sampled everytime a trace is calculated */
+		bool reuse_rand_vec_trace_ = true;
+		/*! \brief Seed number to generate random vectors (e.g. Rademacher) */
+		int seed_rand_vec_trace_ = 1;
+		/*! \brief Type of preconditoner used for the conjugate gradient algorithm */
+		string_t cg_preconditioner_type_ = "Sigma_inv_plus_BtWB";
+		/*! \brief Rank of the pivoted Cholesky decomposition used as preconditioner in conjugate gradient algorithms */
+		int piv_chol_rank_ = 50;
+		/*! \brief Rank of the matrix for approximating predictive covariance matrices obtained using the Lanczos algorithm */
+		int rank_pred_approx_matrix_lanczos_ = 1000;
+		/*! \brief If true, cg_max_num_it and cg_max_num_it_tridiag are reduced by 2/3 (multiplied by 1/3) for the mode finding of the Laplace approximation in the first gradient step when finding a learning rate that reduces the ll */
+		bool reduce_cg_max_num_it_first_optim_step_ = true;
+
+		/*! \brief Order of the Gauss-Hermite quadrature */
+		int order_GH_ = 30;
+		/*! \brief Nodes and weights for the Gauss-Hermite quadrature */
+		// Source: https://keisan.casio.com/exec/system/1281195844
+		const std::vector<double> GH_nodes_ = { -6.863345293529891581061,
+										-6.138279220123934620395,
+										-5.533147151567495725118,
+										-4.988918968589943944486,
+										-4.48305535709251834189,
+										-4.003908603861228815228,
+										-3.544443873155349886925,
+										-3.099970529586441748689,
+										-2.667132124535617200571,
+										-2.243391467761504072473,
+										-1.826741143603688038836,
+										-1.415527800198188511941,
+										-1.008338271046723461805,
+										-0.6039210586255523077782,
+										-0.2011285765488714855458,
+										0.2011285765488714855458,
+										0.6039210586255523077782,
+										1.008338271046723461805,
+										1.415527800198188511941,
+										1.826741143603688038836,
+										2.243391467761504072473,
+										2.667132124535617200571,
+										3.099970529586441748689,
+										3.544443873155349886925,
+										4.003908603861228815228,
+										4.48305535709251834189,
+										4.988918968589943944486,
+										5.533147151567495725118,
+										6.138279220123934620395,
+										6.863345293529891581061 };
+		const std::vector<double> GH_weights_ = { 2.908254700131226229411E-21,
+										2.8103336027509037088E-17,
+										2.87860708054870606219E-14,
+										8.106186297463044204E-12,
+										9.1785804243785282085E-10,
+										5.10852245077594627739E-8,
+										1.57909488732471028835E-6,
+										2.9387252289229876415E-5,
+										3.48310124318685523421E-4,
+										0.00273792247306765846299,
+										0.0147038297048266835153,
+										0.0551441768702342511681,
+										0.1467358475408900997517,
+										0.2801309308392126674135,
+										0.386394889541813862556,
+										0.3863948895418138625556,
+										0.2801309308392126674135,
+										0.1467358475408900997517,
+										0.0551441768702342511681,
+										0.01470382970482668351528,
+										0.002737922473067658462989,
+										3.48310124318685523421E-4,
+										2.938725228922987641501E-5,
+										1.579094887324710288346E-6,
+										5.1085224507759462774E-8,
+										9.1785804243785282085E-10,
+										8.10618629746304420399E-12,
+										2.87860708054870606219E-14,
+										2.81033360275090370876E-17,
+										2.9082547001312262294E-21 };
+		const std::vector<double> adaptive_GH_weights_ = { 0.83424747101276179534,
+										0.64909798155426670071,
+										0.56940269194964050397,
+										0.52252568933135454964,
+										0.491057995832882696506,
+										0.46837481256472881677,
+										0.45132103599118862129,
+										0.438177022652683703695,
+										0.4279180629327437485828,
+										0.4198950037368240886418,
+										0.413679363611138937184,
+										0.4089815750035316024972,
+										0.4056051233256844363121,
+										0.403419816924804022553,
+										0.402346066701902927115,
+										0.4023460667019029271154,
+										0.4034198169248040225528,
+										0.4056051233256844363121,
+										0.4089815750035316024972,
+										0.413679363611138937184,
+										0.4198950037368240886418,
+										0.427918062932743748583,
+										0.4381770226526837037,
+										0.45132103599118862129,
+										0.46837481256472881677,
+										0.4910579958328826965056,
+										0.52252568933135454964,
+										0.56940269194964050397,
+										0.64909798155426670071,
+										0.83424747101276179534 };
+
+		const char* NA_OR_INF_WARNING_ = "Mode finding algorithm for Laplace approximation: NA or Inf occurred. "
+			"This is not necessary a problem as it might have been the cause of a too large learning rate which, "
+			"consequently, might have been decreased by the optimization algorithm ";
+		const char* NA_OR_INF_ERROR_ = "NA or Inf occurred in the mode finding algorithm for the Laplace approximation ";
+		const char* NO_INCREASE_IN_MLL_WARNING_ = "Mode finding algorithm for Laplace approximation: "
+			"The approximate marginal log-likelihood (=convergence criterion) has decreased and the algorithm has thus been terminated ";
+		const char* NO_CONVERGENCE_WARNING_ = "Algorithm for finding mode for Laplace approximation has not "
+			"converged after the maximal number of iterations ";
+
+	};//end class Likelihood
+
+}  // namespace GPBoost
+
+#endif   // GPB_LIKELIHOODS_
```

### Comparing `gpboost-1.2.1.1/compile/include/GPBoost/re_comp.h` & `gpboost-1.2.2/compile/include/GPBoost/re_comp.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/include/GPBoost/re_model.h` & `gpboost-1.2.2/compile/include/GPBoost/re_model.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/include/GPBoost/re_model_template.h` & `gpboost-1.2.2/compile/include/GPBoost/re_model_template.h`

 * *Files 1% similar despite different names*

```diff
@@ -1100,15 +1100,15 @@
 						} // end trace output
 					}// end not na_or_inf_occurred
 					// Check whether to terminate
 					if (terminate_optim) {
 						num_it = it + 1;
 						break;
 					}
-					////increase learning rates again
+					////increase learning rates again (not used)
 					//else if (optimizer_cov_pars_ == "gradient_descent" && (it + 1) >= 10 && learning_rate_decreased_first_time_ &&
 					//	!learning_rate_increased_after_descrease_ && !na_or_inf_occurred) {
 					//	if ((neg_log_likelihood_lag1_ - neg_log_likelihood_) < INCREASE_LR_CHANGE_LL_THRESHOLD_ * std::abs(neg_log_likelihood_lag1_)) {
 					//		if (has_covariates_) {
 					//			lr_coef_ /= LR_SHRINKAGE_FACTOR_;
 					//		}
 					//		if (learn_covariance_parameters) {
@@ -2933,14 +2933,51 @@
 			HTYAux *= marg_variance;
 			vec_t new_leaf_values = HTPsiInvH.llt().solve(HTYAux);
 			for (int i = 0; i < num_leaves; ++i) {
 				leaf_values[i] = new_leaf_values[i];
 			}
 		}//end NewtonUpdateLeafValues
 
+		/*!
+		* \brief Apply a momentum step
+		* \param it Iteration number
+		* \param pars Parameters
+		* \param pars_lag1 Parameters from last iteration
+		* \param[out] pars_acc Accelerated parameters
+		* \param nesterov_acc_rate Nesterov acceleration speed
+		* \param nesterov_schedule_version Which version of Nesterov schedule should be used. Default = 0
+		* \param exclude_first_log_scale If true, no momentum is applied to the first value and the momentum step is done on the log-scale for the other values. Default = true
+		* \param momentum_offset Number of iterations for which no mometum is applied in the beginning
+		* \param log_scale If true, the momentum step is done on the log-scale
+		*/
+		static void ApplyMomentumStep(int it,
+			vec_t& pars,
+			vec_t& pars_lag1,
+			vec_t& pars_acc,
+			double nesterov_acc_rate,
+			int nesterov_schedule_version,
+			bool exclude_first_log_scale,
+			int momentum_offset,
+			bool log_scale) {
+			double mu = NesterovSchedule(it, nesterov_schedule_version, nesterov_acc_rate, momentum_offset);
+			int num_par = (int)pars.size();
+			if (exclude_first_log_scale) {
+				pars_acc[0] = pars[0];
+				pars_acc.segment(1, num_par - 1) = ((mu + 1.) * (pars.segment(1, num_par - 1).array().log()) - mu * (pars_lag1.segment(1, num_par - 1).array().log())).exp().matrix();//Momentum is added on the log scale
+			}
+			else {
+				if (log_scale) {
+					pars_acc = ((mu + 1.) * (pars.array().log()) - mu * (pars_lag1.array().log())).exp().matrix();
+				}
+				else {
+					pars_acc = (mu + 1) * pars - mu * pars_lag1;
+				}
+			}
+		}// end ApplyMomentumStep
+
 	private:
 
 		// RESPONSE DATA
 		/*! \brief Number of data points */
 		data_size_t num_data_;
 		/*! \brief If true, the response variables have a Gaussian likelihood, otherwise not */
 		data_size_t gauss_likelihood_ = true;
@@ -3294,15 +3331,15 @@
 		const char* DUPLICATES_PRED_VECCHIA_LATENT_ = "Duplicates found among training and test coordinates. "
 			"This is not supported for predictions with a Vecchia approximation for the latent process ('latent_') ";
 
 		/*! Random number generator */
 		RNG_t rng_;
 
 		/*! \brief Nesterov schedule */
-		double NesterovSchedule(int iter,
+		static double NesterovSchedule(int iter,
 			int momentum_schedule_version,
 			double nesterov_acc_rate, 
 			int momentum_offset) {
 			if (iter < momentum_offset) {
 				return(0.);
 			}
 			else {
@@ -3310,18 +3347,18 @@
 					return(nesterov_acc_rate);
 				}
 				else if (momentum_schedule_version == 1) {
 					return(1. - (3. / (6. + iter)));
 				}
 				else {
 					Log::REFatal("NesterovSchedule: version = %d is not supported ", momentum_schedule_version);
-					return(0.);
 				}
 			}
-		}
+			return(0.);
+		}//end NesterovSchedule
 
 		/*! \brief mutex for threading safe call */
 		std::mutex mutex_;
 
 		/*! \brief Constructs identity matrices if sparse matrices are used (used for calculating inverse covariance matrix) */
 		template <class T_aux = T_mat, typename std::enable_if <std::is_same<sp_mat_t, T_aux>::value || std::is_same<sp_mat_rm_t, T_aux>::value>::type* = nullptr >
 		void ConstructI(data_size_t cluster_i) {
@@ -5714,51 +5751,14 @@
 						}
 					}//end not only_grouped_REs_use_woodbury_identity_
 				}//end not gp_approx_ == "vecchia"
 			}
 		}//end CalcYTPsiIInvY
 
 		/*!
-		* \brief Apply a momentum step
-		* \param it Iteration number
-		* \param pars Parameters
-		* \param pars_lag1 Parameters from last iteration
-		* \param[out] pars_acc Accelerated parameters
-		* \param nesterov_acc_rate Nesterov acceleration speed
-		* \param nesterov_schedule_version Which version of Nesterov schedule should be used. Default = 0
-		* \param exclude_first_log_scale If true, no momentum is applied to the first value and the momentum step is done on the log-scale for the other values. Default = true
-		* \param momentum_offset Number of iterations for which no mometum is applied in the beginning
-		* \param log_scale If true, the momentum step is done on the log-scale
-		*/
-		void ApplyMomentumStep(int it, 
-			vec_t& pars, 
-			vec_t& pars_lag1, 
-			vec_t& pars_acc, 
-			double nesterov_acc_rate,
-			int nesterov_schedule_version, 
-			bool exclude_first_log_scale, 
-			int momentum_offset, 
-			bool log_scale) {
-			double mu = NesterovSchedule(it, nesterov_schedule_version, nesterov_acc_rate, momentum_offset);
-			int num_par = (int)pars.size();
-			if (exclude_first_log_scale) {
-				pars_acc[0] = pars[0];
-				pars_acc.segment(1, num_par - 1) = ((mu + 1.) * (pars.segment(1, num_par - 1).array().log()) - mu * (pars_lag1.segment(1, num_par - 1).array().log())).exp().matrix();//Momentum is added on the log scale
-			}
-			else {
-				if (log_scale) {
-					pars_acc = ((mu + 1.) * (pars.array().log()) - mu * (pars_lag1.array().log())).exp().matrix();
-				}
-				else {
-					pars_acc = (mu + 1) * pars - mu * pars_lag1;
-				}
-			}
-		}
-
-		/*!
 		* \brief Update linear fixed-effect coefficients using generalized least squares (GLS)
 		* \param X Covariate data for linear fixed-effect
 		* \param[out] beta Linear regression coefficients
 		*/
 		void UpdateCoefGLS(den_mat_t& X,
 			vec_t& beta) {
 			vec_t y_aux(num_data_);
```

### Comparing `gpboost-1.2.1.1/compile/include/GPBoost/sparse_matrix_utils.h` & `gpboost-1.2.2/compile/include/GPBoost/sparse_matrix_utils.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/include/GPBoost/type_defs.h` & `gpboost-1.2.2/compile/include/GPBoost/type_defs.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/include/GPBoost/utils.h` & `gpboost-1.2.2/compile/include/GPBoost/utils.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/include/LightGBM/application.h` & `gpboost-1.2.2/compile/include/LightGBM/application.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/include/LightGBM/bin.h` & `gpboost-1.2.2/compile/include/LightGBM/bin.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/include/LightGBM/boosting.h` & `gpboost-1.2.2/compile/include/LightGBM/boosting.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/include/LightGBM/c_api.h` & `gpboost-1.2.2/compile/include/LightGBM/c_api.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/include/LightGBM/config.h` & `gpboost-1.2.2/compile/include/LightGBM/config.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/include/LightGBM/cuda/cuda_utils.h` & `gpboost-1.2.2/compile/include/LightGBM/cuda/cuda_utils.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/include/LightGBM/cuda/vector_cudahost.h` & `gpboost-1.2.2/compile/include/LightGBM/cuda/vector_cudahost.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/include/LightGBM/dataset.h` & `gpboost-1.2.2/compile/include/LightGBM/dataset.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/include/LightGBM/dataset_loader.h` & `gpboost-1.2.2/compile/include/LightGBM/dataset_loader.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/include/LightGBM/export.h` & `gpboost-1.2.2/compile/include/LightGBM/export.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/include/LightGBM/feature_group.h` & `gpboost-1.2.2/compile/include/LightGBM/feature_group.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/include/LightGBM/meta.h` & `gpboost-1.2.2/compile/include/LightGBM/meta.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/include/LightGBM/metric.h` & `gpboost-1.2.2/compile/include/LightGBM/metric.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/include/LightGBM/nesterov_boosting.h` & `gpboost-1.2.2/compile/include/LightGBM/nesterov_boosting.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/include/LightGBM/network.h` & `gpboost-1.2.2/compile/include/LightGBM/network.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/include/LightGBM/objective_function.h` & `gpboost-1.2.2/compile/include/LightGBM/objective_function.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/include/LightGBM/prediction_early_stop.h` & `gpboost-1.2.2/compile/include/LightGBM/prediction_early_stop.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/include/LightGBM/train_share_states.h` & `gpboost-1.2.2/compile/include/LightGBM/train_share_states.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/include/LightGBM/tree.h` & `gpboost-1.2.2/compile/include/LightGBM/tree.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/include/LightGBM/tree_learner.h` & `gpboost-1.2.2/compile/include/LightGBM/tree_learner.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/include/LightGBM/utils/array_args.h` & `gpboost-1.2.2/compile/include/LightGBM/utils/array_args.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/include/LightGBM/utils/common.h` & `gpboost-1.2.2/compile/include/LightGBM/utils/common.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/include/LightGBM/utils/common_legacy_solaris.h` & `gpboost-1.2.2/compile/include/LightGBM/utils/common_legacy_solaris.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/include/LightGBM/utils/file_io.h` & `gpboost-1.2.2/compile/include/LightGBM/utils/file_io.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/include/LightGBM/utils/json11.h` & `gpboost-1.2.2/compile/include/LightGBM/utils/json11.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/include/LightGBM/utils/log.h` & `gpboost-1.2.2/compile/include/LightGBM/utils/log.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/include/LightGBM/utils/openmp_wrapper.h` & `gpboost-1.2.2/compile/include/LightGBM/utils/openmp_wrapper.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/include/LightGBM/utils/pipeline_reader.h` & `gpboost-1.2.2/compile/include/LightGBM/utils/pipeline_reader.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/include/LightGBM/utils/random.h` & `gpboost-1.2.2/compile/include/LightGBM/utils/random.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/include/LightGBM/utils/text_reader.h` & `gpboost-1.2.2/compile/include/LightGBM/utils/text_reader.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/include/LightGBM/utils/threading.h` & `gpboost-1.2.2/compile/include/LightGBM/utils/threading.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/include/LightGBM/utils/yamc/alternate_shared_mutex.hpp` & `gpboost-1.2.2/compile/include/LightGBM/utils/yamc/alternate_shared_mutex.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/include/LightGBM/utils/yamc/yamc_rwlock_sched.hpp` & `gpboost-1.2.2/compile/include/LightGBM/utils/yamc/yamc_rwlock_sched.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/include/LightGBM/utils/yamc/yamc_shared_lock.hpp` & `gpboost-1.2.2/compile/include/LightGBM/utils/yamc/yamc_shared_lock.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/src/GPBoost/DF_utils.cpp` & `gpboost-1.2.2/compile/src/GPBoost/DF_utils.cpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/src/GPBoost/GP_utils.cpp` & `gpboost-1.2.2/compile/src/GPBoost/GP_utils.cpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/src/GPBoost/Vecchia_utils.cpp` & `gpboost-1.2.2/compile/src/GPBoost/Vecchia_utils.cpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/src/GPBoost/re_model.cpp` & `gpboost-1.2.2/compile/src/GPBoost/re_model.cpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/src/GPBoost/sparse_matrix_utils.cpp` & `gpboost-1.2.2/compile/src/GPBoost/sparse_matrix_utils.cpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/src/LightGBM/application/application.cpp` & `gpboost-1.2.2/compile/src/LightGBM/application/application.cpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/src/LightGBM/application/predictor.hpp` & `gpboost-1.2.2/compile/src/LightGBM/application/predictor.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/src/LightGBM/boosting/boosting.cpp` & `gpboost-1.2.2/compile/src/LightGBM/boosting/boosting.cpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/src/LightGBM/boosting/dart.hpp` & `gpboost-1.2.2/compile/src/LightGBM/boosting/dart.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/src/LightGBM/boosting/gbdt.cpp` & `gpboost-1.2.2/compile/src/LightGBM/boosting/gbdt.cpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/src/LightGBM/boosting/gbdt.h` & `gpboost-1.2.2/compile/src/LightGBM/boosting/gbdt.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/src/LightGBM/boosting/gbdt_model_text.cpp` & `gpboost-1.2.2/compile/src/LightGBM/boosting/gbdt_model_text.cpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/src/LightGBM/boosting/gbdt_prediction.cpp` & `gpboost-1.2.2/compile/src/LightGBM/boosting/gbdt_prediction.cpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/src/LightGBM/boosting/goss.hpp` & `gpboost-1.2.2/compile/src/LightGBM/boosting/goss.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/src/LightGBM/boosting/prediction_early_stop.cpp` & `gpboost-1.2.2/compile/src/LightGBM/boosting/prediction_early_stop.cpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/src/LightGBM/boosting/rf.hpp` & `gpboost-1.2.2/compile/src/LightGBM/boosting/rf.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/src/LightGBM/boosting/score_updater.hpp` & `gpboost-1.2.2/compile/src/LightGBM/boosting/score_updater.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/src/LightGBM/c_api.cpp` & `gpboost-1.2.2/compile/src/LightGBM/c_api.cpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/src/LightGBM/io/bin.cpp` & `gpboost-1.2.2/compile/src/LightGBM/io/bin.cpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/src/LightGBM/io/config.cpp` & `gpboost-1.2.2/compile/src/LightGBM/io/config.cpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/src/LightGBM/io/config_auto.cpp` & `gpboost-1.2.2/compile/src/LightGBM/io/config_auto.cpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/src/LightGBM/io/dataset.cpp` & `gpboost-1.2.2/compile/src/LightGBM/io/dataset.cpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/src/LightGBM/io/dataset_loader.cpp` & `gpboost-1.2.2/compile/src/LightGBM/io/dataset_loader.cpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/src/LightGBM/io/dense_bin.hpp` & `gpboost-1.2.2/compile/src/LightGBM/io/dense_bin.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/src/LightGBM/io/file_io.cpp` & `gpboost-1.2.2/compile/src/LightGBM/io/file_io.cpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/src/LightGBM/io/json11.cpp` & `gpboost-1.2.2/compile/src/LightGBM/io/json11.cpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/src/LightGBM/io/metadata.cpp` & `gpboost-1.2.2/compile/src/LightGBM/io/metadata.cpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/src/LightGBM/io/multi_val_dense_bin.hpp` & `gpboost-1.2.2/compile/src/LightGBM/io/multi_val_dense_bin.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/src/LightGBM/io/multi_val_sparse_bin.hpp` & `gpboost-1.2.2/compile/src/LightGBM/io/multi_val_sparse_bin.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/src/LightGBM/io/parser.cpp` & `gpboost-1.2.2/compile/src/LightGBM/io/parser.cpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/src/LightGBM/io/parser.hpp` & `gpboost-1.2.2/compile/src/LightGBM/io/parser.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/src/LightGBM/io/sparse_bin.hpp` & `gpboost-1.2.2/compile/src/LightGBM/io/sparse_bin.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/src/LightGBM/io/train_share_states.cpp` & `gpboost-1.2.2/compile/src/LightGBM/io/train_share_states.cpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/src/LightGBM/io/tree.cpp` & `gpboost-1.2.2/compile/src/LightGBM/io/tree.cpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/src/LightGBM/main.cpp` & `gpboost-1.2.2/compile/src/LightGBM/main.cpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/src/LightGBM/metric/binary_metric.hpp` & `gpboost-1.2.2/compile/src/LightGBM/metric/binary_metric.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/src/LightGBM/metric/dcg_calculator.cpp` & `gpboost-1.2.2/compile/src/LightGBM/metric/dcg_calculator.cpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/src/LightGBM/metric/map_metric.hpp` & `gpboost-1.2.2/compile/src/LightGBM/metric/map_metric.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/src/LightGBM/metric/metric.cpp` & `gpboost-1.2.2/compile/src/LightGBM/metric/metric.cpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/src/LightGBM/metric/multiclass_metric.hpp` & `gpboost-1.2.2/compile/src/LightGBM/metric/multiclass_metric.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/src/LightGBM/metric/random_effects_metric.hpp` & `gpboost-1.2.2/compile/src/LightGBM/metric/random_effects_metric.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/src/LightGBM/metric/rank_metric.hpp` & `gpboost-1.2.2/compile/src/LightGBM/metric/rank_metric.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/src/LightGBM/metric/regression_metric.hpp` & `gpboost-1.2.2/compile/src/LightGBM/metric/regression_metric.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/src/LightGBM/metric/xentropy_metric.hpp` & `gpboost-1.2.2/compile/src/LightGBM/metric/xentropy_metric.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/src/LightGBM/network/ifaddrs_patch.cpp` & `gpboost-1.2.2/compile/src/LightGBM/network/ifaddrs_patch.cpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/src/LightGBM/network/ifaddrs_patch.h` & `gpboost-1.2.2/compile/src/LightGBM/network/ifaddrs_patch.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/src/LightGBM/network/linker_topo.cpp` & `gpboost-1.2.2/compile/src/LightGBM/network/linker_topo.cpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/src/LightGBM/network/linkers.h` & `gpboost-1.2.2/compile/src/LightGBM/network/linkers.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/src/LightGBM/network/linkers_mpi.cpp` & `gpboost-1.2.2/compile/src/LightGBM/network/linkers_mpi.cpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/src/LightGBM/network/linkers_socket.cpp` & `gpboost-1.2.2/compile/src/LightGBM/network/linkers_socket.cpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/src/LightGBM/network/network.cpp` & `gpboost-1.2.2/compile/src/LightGBM/network/network.cpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/src/LightGBM/network/socket_wrapper.hpp` & `gpboost-1.2.2/compile/src/LightGBM/network/socket_wrapper.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/src/LightGBM/objective/binary_objective.hpp` & `gpboost-1.2.2/compile/src/LightGBM/objective/binary_objective.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/src/LightGBM/objective/multiclass_objective.hpp` & `gpboost-1.2.2/compile/src/LightGBM/objective/multiclass_objective.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/src/LightGBM/objective/objective_function.cpp` & `gpboost-1.2.2/compile/src/LightGBM/objective/objective_function.cpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/src/LightGBM/objective/rank_objective.hpp` & `gpboost-1.2.2/compile/src/LightGBM/objective/rank_objective.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/src/LightGBM/objective/regression_objective.hpp` & `gpboost-1.2.2/compile/src/LightGBM/objective/regression_objective.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/src/LightGBM/objective/xentropy_objective.hpp` & `gpboost-1.2.2/compile/src/LightGBM/objective/xentropy_objective.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/src/LightGBM/treelearner/col_sampler.hpp` & `gpboost-1.2.2/compile/src/LightGBM/treelearner/col_sampler.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/src/LightGBM/treelearner/cost_effective_gradient_boosting.hpp` & `gpboost-1.2.2/compile/src/LightGBM/treelearner/cost_effective_gradient_boosting.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/src/LightGBM/treelearner/cuda_kernel_launcher.cu` & `gpboost-1.2.2/compile/src/LightGBM/treelearner/cuda_kernel_launcher.cu`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/src/LightGBM/treelearner/cuda_kernel_launcher.h` & `gpboost-1.2.2/compile/src/LightGBM/treelearner/cuda_kernel_launcher.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/src/LightGBM/treelearner/cuda_tree_learner.cpp` & `gpboost-1.2.2/compile/src/LightGBM/treelearner/cuda_tree_learner.cpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/src/LightGBM/treelearner/cuda_tree_learner.h` & `gpboost-1.2.2/compile/src/LightGBM/treelearner/cuda_tree_learner.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/src/LightGBM/treelearner/data_parallel_tree_learner.cpp` & `gpboost-1.2.2/compile/src/LightGBM/treelearner/data_parallel_tree_learner.cpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/src/LightGBM/treelearner/data_partition.hpp` & `gpboost-1.2.2/compile/src/LightGBM/treelearner/data_partition.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/src/LightGBM/treelearner/feature_histogram.hpp` & `gpboost-1.2.2/compile/src/LightGBM/treelearner/feature_histogram.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/src/LightGBM/treelearner/feature_parallel_tree_learner.cpp` & `gpboost-1.2.2/compile/src/LightGBM/treelearner/feature_parallel_tree_learner.cpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/src/LightGBM/treelearner/gpu_tree_learner.cpp` & `gpboost-1.2.2/compile/src/LightGBM/treelearner/gpu_tree_learner.cpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/src/LightGBM/treelearner/gpu_tree_learner.h` & `gpboost-1.2.2/compile/src/LightGBM/treelearner/gpu_tree_learner.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/src/LightGBM/treelearner/kernels/histogram_16_64_256.cu` & `gpboost-1.2.2/compile/src/LightGBM/treelearner/kernels/histogram_16_64_256.cu`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/src/LightGBM/treelearner/kernels/histogram_16_64_256.hu` & `gpboost-1.2.2/compile/src/LightGBM/treelearner/kernels/histogram_16_64_256.hu`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/src/LightGBM/treelearner/leaf_splits.hpp` & `gpboost-1.2.2/compile/src/LightGBM/treelearner/leaf_splits.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/src/LightGBM/treelearner/linear_tree_learner.cpp` & `gpboost-1.2.2/compile/src/LightGBM/treelearner/linear_tree_learner.cpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/src/LightGBM/treelearner/linear_tree_learner.h` & `gpboost-1.2.2/compile/src/LightGBM/treelearner/linear_tree_learner.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/src/LightGBM/treelearner/monotone_constraints.hpp` & `gpboost-1.2.2/compile/src/LightGBM/treelearner/monotone_constraints.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/src/LightGBM/treelearner/ocl/histogram16.cl` & `gpboost-1.2.2/compile/src/LightGBM/treelearner/ocl/histogram16.cl`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/src/LightGBM/treelearner/ocl/histogram256.cl` & `gpboost-1.2.2/compile/src/LightGBM/treelearner/ocl/histogram256.cl`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/src/LightGBM/treelearner/ocl/histogram64.cl` & `gpboost-1.2.2/compile/src/LightGBM/treelearner/ocl/histogram64.cl`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/src/LightGBM/treelearner/parallel_tree_learner.h` & `gpboost-1.2.2/compile/src/LightGBM/treelearner/parallel_tree_learner.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/src/LightGBM/treelearner/serial_tree_learner.cpp` & `gpboost-1.2.2/compile/src/LightGBM/treelearner/serial_tree_learner.cpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/src/LightGBM/treelearner/serial_tree_learner.h` & `gpboost-1.2.2/compile/src/LightGBM/treelearner/serial_tree_learner.h`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/src/LightGBM/treelearner/split_info.hpp` & `gpboost-1.2.2/compile/src/LightGBM/treelearner/split_info.hpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/src/LightGBM/treelearner/tree_learner.cpp` & `gpboost-1.2.2/compile/src/LightGBM/treelearner/tree_learner.cpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/compile/src/LightGBM/treelearner/voting_parallel_tree_learner.cpp` & `gpboost-1.2.2/compile/src/LightGBM/treelearner/voting_parallel_tree_learner.cpp`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/gpboost/__init__.py` & `gpboost-1.2.2/gpboost/__init__.py`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/gpboost/basic.py` & `gpboost-1.2.2/gpboost/basic.py`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/gpboost/callback.py` & `gpboost-1.2.2/gpboost/callback.py`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/gpboost/compat.py` & `gpboost-1.2.2/gpboost/compat.py`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/gpboost/engine.py` & `gpboost-1.2.2/gpboost/engine.py`

 * *Files 1% similar despite different names*

```diff
@@ -1110,16 +1110,17 @@
                 if current_score > best_score:
                     current_score_is_better = True
             else:
                 current_score = np.min(cvbst[next(iter(cvbst))])
                 if current_score < best_score:
                     current_score_is_better = True
         except Exception as err:
-            print("Error for parameter combination " + str(counter_num_comb) +
-                  " of " + str(len(try_param_combs)) + ": " + str(param_comb) + ". Error message: ")
+            if verbose_eval < 1:
+                print("Error for parameter combination " + str(counter_num_comb) +
+                      " of " + str(len(try_param_combs)) + ": " + str(param_comb) + ". Error message: ")
             print(str(err))
         if current_score_is_better:
             best_score = current_score
             best_params = param_comb
             if higher_better:
                 best_num_boost_round = np.argmax(cvbst[next(iter(cvbst))])
             else:
```

### Comparing `gpboost-1.2.1.1/gpboost/libpath.py` & `gpboost-1.2.2/gpboost/libpath.py`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/gpboost/plotting.py` & `gpboost-1.2.2/gpboost/plotting.py`

 * *Files identical despite different names*

### Comparing `gpboost-1.2.1.1/gpboost/sklearn.py` & `gpboost-1.2.2/gpboost/sklearn.py`

 * *Files 0% similar despite different names*

```diff
@@ -932,15 +932,15 @@
                    + _base_doc[_base_doc.find('eval_metric :'):])
 
     def predict(self, X, raw_score=False, start_iteration=0, num_iteration=None,
                 pred_leaf=False, pred_contrib=False,
                 group_data_pred=None, group_rand_coef_data_pred=None,
                 gp_coords_pred=None, gp_rand_coef_data_pred=None,
                 cluster_ids_pred=None, vecchia_pred_type=None,
-                num_neighbors_pred=-1, predict_cov_mat=False, predict_var=False, **kwargs):
+                num_neighbors_pred=None, predict_cov_mat=False, predict_var=False, **kwargs):
         """Docstring is inherited from the GPBoostModel."""
         result = self.predict_proba(X=X, raw_score=raw_score, start_iteration=start_iteration, num_iteration=num_iteration,
                                     pred_leaf=pred_leaf, pred_contrib=pred_contrib,
                                     group_data_pred=group_data_pred, group_rand_coef_data_pred=group_rand_coef_data_pred,
                                     gp_coords_pred=gp_coords_pred, gp_rand_coef_data_pred=gp_rand_coef_data_pred,
                                     cluster_ids_pred=cluster_ids_pred, vecchia_pred_type=vecchia_pred_type,
                                     num_neighbors_pred=num_neighbors_pred, predict_cov_mat=predict_cov_mat, predict_var=predict_var,
```

### Comparing `gpboost-1.2.1.1/gpboost.egg-info/PKG-INFO` & `gpboost-1.2.2/gpboost.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpboost
-Version: 1.2.1.1
+Version: 1.2.2
 Summary: GPBoost Python Package
 Home-page: https://github.com/fabsig/GPBoost
 Maintainer: Fabio Sigrist
 Maintainer-email: fabiosigrist@gmail.com
 License: Apache License, Version 2.0, + see LICENSE file
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
@@ -44,15 +44,14 @@
   * [Installation from source](#installation-from-source)
 
 
 ## Examples and documentation
 
 * [**Detailed Python examples**](https://github.com/fabsig/GPBoost/tree/master/examples/python-guide):
   * [GPBoost and LaGaBoost algorithms](https://github.com/fabsig/GPBoost/tree/master/examples/python-guide/GPBoost_algorithm.py) for Gaussian data ("regression") and non-Gaussian data ("classification", etc.) combining tree-boosting with Gaussian process and random effects models
-  * [Parameter tuning](https://github.com/fabsig/GPBoost/tree/master/examples/python-guide/parameter_tuning.py) using deterministic or random grid search
   * [Generalized linear Gaussian process and mixed effects models](https://github.com/fabsig/GPBoost/tree/master/examples/python-guide/generalized_linear_Gaussian_process_mixed_effects_models.py)
   * [GPBoost algorithm applied to panel data](https://github.com/fabsig/GPBoost/tree/master/examples/python-guide/panel_data_example.py)
 * The **documentation at [https://gpboost.readthedocs.io](https://gpboost.readthedocs.io/en/latest/Python_package.html)**
 * Blog posts on how to 
    * [Combine tree-boosting with grouped random effects models](https://towardsdatascience.com/tree-boosted-mixed-effects-models-4df610b624cb) 
    * [Combine tree-boosting with Gaussian processes for spatial data](https://towardsdatascience.com/tree-boosting-for-spatial-data-789145d6d97d)
    * [GPBoost for generalized linear mixed effects models (GLMMs)](https://towardsdatascience.com/generalized-linear-mixed-effects-models-in-r-and-python-with-gpboost-89297622820c)
```

### Comparing `gpboost-1.2.1.1/gpboost.egg-info/SOURCES.txt` & `gpboost-1.2.2/gpboost.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 LICENSE
 MANIFEST.in
 README.md
 _IS_SOURCE_PACKAGE.txt
 setup.py
 compile/CMakeIntegratedOpenCL.cmake
 compile/CMakeLists.txt
-compile/Release/lib_gpboost.dll
 compile/external_libs/CSparse/Doc/LICENSE.txt
 compile/external_libs/CSparse/Include/cs.h
 compile/external_libs/CSparse/Source/cs_dfs.c
 compile/external_libs/CSparse/Source/cs_reach.c
 compile/external_libs/CSparse/Source/cs_spsolve.c
 compile/external_libs/OptimLib/LICENSE
 compile/external_libs/OptimLib/NOTICE.txt
```

### Comparing `gpboost-1.2.1.1/setup.py` & `gpboost-1.2.2/setup.py`

 * *Files identical despite different names*

